### Class 12 Reading Notes

## Spring MVC Request Mapping

Request mapping in Spring MVC is the annotation for routing requests in the Controller.

The generic syntax for request mapping is `@RequestMapping(value = "/route/example", method = GET)` follow by `@ResponseBody` and a function to handle the route. The two necessary elements are the `value` and `method`. If `method` isn't specified, then the route will map to any request, and that sounds pretty dangerous right?

There are a bunch of other optional elements that can be passed into the request mapping annotation. For instance, headers can be handled with `headers = "someKey=someValue"` and query parameters with `params = {"red", "green", "blue", "alpha"}`. Path variables can also be added to the path value with curly braces, `/route/example/{varName}`.

Another key feature is specifying media types. If you can support multiple types of responses, then a GET request might include `produces = {"application/json", "application/xml"}`.

As of Spring Framework 4.3, the preferable method for request mapping is with the more explicit versions. `@GetMapping`, `@PostMapping`, `@PutMapping`, `@DeleteMapping`, and `@PatchMapping` are all available to make the routes more readable. `HEAD`, `OPTIONS`, and `TRACE` methods do not have the direct versions available.

[Return to table of contents](../README.md)
