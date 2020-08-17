### Class 06 Reading Notes

## Node.js

Node.js is a Javascript runtime built on Chrome's V8 engine. This means it's not built to run in a browser, but uses the engine execute Javascript code independently. It can be used directly in a terminal as a REPL, for instance.

While Node is not required for a deployed back end, it is hard to match for developement. It can be managed easily in combination with a package manager like npm or Yarn. And it's very local friendly.

One major advantage to Node as a server is that it's single-threaded and event driven. Some other server options, such as Apache, will create a thread to handle a request and pause the code while resolving. If other requests come in, a new thread will be created. The downside to this is that many threads can quickly become sluggish. Node instead operates in one thread and continues to run code while resolving requests. It simply creates a callback function that will trigger once a request is resolved so it can move on to other requests in the meantime. This process is what allows Node to be asynchronous.

This does come with some risks. An error on the single thread could crash the whole server if not handled well. And resource intensive operations can bog down the process. Which is why flow control is so important with Javascript.

The really special thing about Node.js is that it allows Javascript to fill many more roles. Instead of having to switch between languages for different purposes, Javascript can now also be used as a scripting language. While it might not be the perfect language for every purpose, it allows developers the ability to create full stack web pages and handle data analysis and scripting all in one language.

[Return to table of contents](../README.md)
