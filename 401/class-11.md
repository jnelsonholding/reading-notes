### Class 11 Reading Notes

## Spring MVC and Thymeleaf

In the Spring framework, the data in the model is referred to as model attributes. The model attributes are available in Thymeleaf views.

Thymeleaf allows access of the values stored in the model through syntax similar to Javascript template literals: `${someObject.value}`. This can be wrapped into chunks of HTML for easy, repeatable rendering.

Thymleaf also has the ability to access http query parameters directly. For instance, `${param.thing}` would access the value of the parameter with the key "thing". If there are multiple parameters with the same key, they can be accessed by their index using square brackets.

Session attributes can also be added through the controller. Similarly to parameters, the view has access to session attributes through dot notations: `session.anAttribute`.

To access ServletContext attributes, add a `#` before the reference. For instance: `#servletContext.getAttribute(attr)`.

Perhaps the most exciting is beans. Thymeleaf can access beans using the `@` symbol: `${@urlService.getApplicationUrl()}`. The bean is handled similarly in the controller: `@Bean(name = "urlService")`.

[Return to table of contents](../README.md)
