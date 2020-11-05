### Class 39 Reading Notes

## AWS Kinesis

AWS Kinesis provides features for collecting analytics for your app. It's intallation is similar to other Amplify plugins:

`amplify add analytics`

`amplify push`

Add the dependency:

`implementation 'com.amplifyframework:aws-analytics-pinpoint:1.4.1'`

And add the plugin during the Amplify configurations:

`Amplify.addPlugin(new AWSPinpointAnalyticsPlugin(this));`

Note that this is assumes that the app is using Cognito as well.

Kinesis makes it easy to build and record events in an app. Much like other Amplify tools, it utilizes a builder structure to create events and then passes them to Analytics. By default, events are flushed to the network every 30 seconds. Check out this guide to learn the basics: [Amplify Analytics Setup](https://docs.amplify.aws/lib/analytics/getting-started/q/platform/android).

[Return to table of contents](../README.md)
