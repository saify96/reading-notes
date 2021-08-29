## Android Fundamentals
- Android package is an archive file with an .apk suffix, contains the contents of an Android app that are required at runtime and it is the file that Android-powered devices use to install the app.
- Android App Bundle is an archive file with an .aab suffix, contains the contents of an Android app project including some additional metadata that is not required at runtime. 

## Each Android app lives in its own security sandbox, protected by the following Android security features:

- The Android operating system is a multi-user Linux system in which each app is a different user.
- By default, the system assigns each app a unique Linux user ID.
- Each process has its own virtual machine (VM).
- By default, every app runs in its own Linux process.


## App components

### There are four different types of app components:

- Activities
  - An activity is the entry point for interacting with the user.
- Services
  - A service is a general-purpose entry point for keeping an app running in the background for all kinds of reasons.
- Broadcast receivers
  - A broadcast receiver is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements.
- Content providers
  - A content provider manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access.

### Android apps don't have a single entry point (there's no main() function).


## Activating components

- Three of the four component types—activities, services, and broadcast receivers—are activated by an asynchronous message called an intent.
- An intent is created with an Intent object, which defines a message to activate either a specific component (explicit intent) or a specific type of component (implicit intent).

## The manifest file

- Before the Android system can start an app component, the system must know that the component exists by reading the app's manifest file, AndroidManifest.xml. Your app must declare all its components in this file, which must be at the root of the app project directory.

- The primary task of the manifest is to inform the system about the app's components.

## Declaring app requirements

- There are a variety of devices powered by Android and not all of them provide the same features and capabilities. To prevent your app from being installed on devices that lack features needed by your app, it's important that you clearly define a profile for the types of devices your app supports by declaring device and software requirements in your manifest file.

