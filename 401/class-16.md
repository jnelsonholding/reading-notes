### Class 16 Reading Notes

## Spring Security

Security is based around authentication and authorization. Basically it's the concepts of identifying who wants something and what they are allowed to access.

In Spring Boot, `AuthenticationManager` is the main interface for handling authentication. It only contains the method `authenticate` which takes in an `Authentication` and returns one as well. If authentication fails, it will throw an `AuthenticationException` instead, or possibly a null if it just doesn't know what to do.

`AuthenticationProvider` is like `AuthenticationManager` except it provides an extra method, `supports`. `supports` will essentially respond to the question "is this auth type allowed" with a true or false.

Obviously this is a bit sparse, so you'll likely need to customize your access and link it to a collection of user info. `AuthenticationManagerBuilder` has methods for creating a storage of user data for auth purposes. Spring allows the `AuthenticationManagerBuilder` to be `@Autowired` into a `@Bean` for global access. However this will not work if a method is annotated with `@Override` because that will replace the global implementation and create a new local version.

So let's say we get an `Authentication` with its `authentication` field set to `true`. Next step is to handle authorization (AKA access control) for the caller using the `AccessDecisionManager`. The implementations available all delegate to an `AccessDecisionVoter`.

The `AccessDecisionVoter` looks at three things: the `Authentication`, a `S object` (a generic object with whatever the user is trying to access), and a collection of `ConfigAttribute` used to determine the level of permission required to access the secure object. A `ConfigAttribute` just returns a String to analyze the access level (such as `ROLE_ADMIN`).

Resource: [Spring Security Architecture](https://spring.io/guides/topicals/spring-security-architecture/)

[Return to table of contents](../README.md)
