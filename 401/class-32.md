### Class 32 Reading Notes

## Serverless

Servers are easiest to imagine as a box somewhere always running, waiting to receive requests, and do some work. To maintain a service on a server, it has to have the ability to handle peak traffic without going down. And the rest of the time, that capacity is beyond what is necessary.

Serverless is an architecture that removes that box. Instead, the operations that would be handled by the server are instead split between the front-end logic and a cloud provider's services. These services are considered event triggered and only last for the duration of their use.

There are some handy advantages to this system. One is that without the box, the client does not have to worry about as much provisioning and maintanence. A server goes down intermittently, but the services in the cloud are spread around massive server farms. When a server goes down, the client doesn't see a lapse in service and the cloud provider handles their maintanence.

Serverless can also provide a lower cost point especially for clients who do not have constant traffic. Instead, the charges are specifically for the events that are triggered and the space they take up. And if there's a sudden increase in traffic, more events can be created without the hassle of provisioning more servers just to have the need die down soon after.

There are some downsides too. By moving typically stored logic and dependencies to the front-end, the applications become a lot heavier. And splitting services into lighter, more modular event instances can actually hurt some larger computing abilities. If you're handling large scale data analysis, you might need some good old fashioned boxes to handle the less time efficient calculations.

[Return to table of contents](../README.md)
