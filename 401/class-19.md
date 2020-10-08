### Class 19 Reading Notes

## Messaging

Messaging can be created using the WebSocket layer that sits above TCP. Spring allows for the use of STOMP (Streaming Text Oriented Messaging Protocol) which works over TCP.

STOMP can conveniently use JSON messages. And with Spring, you can handle the messages in a Controller. Much like a request mapping, `@MessageMapping` can be used to create a route for incoming messages.

In order to actually receive the messages, you can set up an `@EnableWebSocketMessageBroker` in `@Configuration`. This is where endpoints can be registered as well.

[Return to table of contents](../README.md)
