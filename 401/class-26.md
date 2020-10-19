### Class 26 Reading Notes

## Android Basics

We're using Java, but Android apps can also be written in Kotlin or C++. Either way, the end result is compiled into an Android Package (.apk file). These packages contain everything an Android device needs to install and run an app.

When an app is installed on an Android device, it is considered a user by the operating system. These users (apps) can each be assigned permissions and run on separate processes. Keeping all apps separate by default allows for better security management in the overall system.

### App Components

There are 4 types of components in Android apps:

- Activities
  - A direct interaction for a user
  - A single screen with a user interface
  - Similar to the View in an MVC structure but has more functionality
  - Implemented as a subclass of `Activity` class
- Services
  - Used for anything running in the background
  - Can be important (user is aware of it like music) or somewhat passive (user does not even know it's running)
  - Similar in some ways to the Controller in an MVC structure
  - Bound services can act as an API for other apps on the same device
  - Implemented as a subclass of `Service` class
- Broadcast Receivers
  - Allows an app to communicate with other apps, sending and receiving information
  - Sometimes results in status updates to the user, such as alarms or push notifications
  - Can be used to update other apps on availability of a service that has been updated
  - Implemented as a subclass of `BroadcastReceiver` class
- Content Providers
  - Manages shared app data in a persistent storage location
  - Similar in concept to the Model in an MVC structure, except that its intention is more geared towards shareable resources
  - Allows interaction between apps like borrowing a camera app to take a photo
  - Implemented as a subclass of `ContentProvider` class

### Component Activation

Activities, Services, and Broadcast Receivers are all activated using Intents. Intents act like messages that drive components to run. In some senses, this is similar to requests sent to a server. Intents can be explicit (requesting to view a specific activity) or they can be implicit (requesting to use a type of component). They can also carry varying levels of information like point a service at a URI (Uniform Resource Identifier) where some data is stored. However, when activating a Broadcast Receiver, the Intent will always be fairly basic, possibly just including the information to broadcast.

Content Providers are activated by Content Resolvers instead of Intents. This creates a layer of abstraction, separating the app providing the content from the inner workings of the app requesting it.

For more information, [check out the Android Docs on Fundamentals](https://developer.android.com/guide/components/fundamentals).

[Return to table of contents](../README.md)
