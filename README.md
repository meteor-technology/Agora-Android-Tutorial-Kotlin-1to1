# Android 1-to-1 Tutorial for Kotlin

This tutorial enables you to quickly get started in your development efforts to create an Android app with real-time video chat using the Agora Video SDK. 

**This repository is fork from [AgoraIO/Basic-Video-Call](https://github.com/AgoraIO/Basic-Video-Call).**

With this sample app you can:

- [Join](#join-a-channel) and [leave](#hang-up-and-end-the-call) a channel.
- [Mute and unmute audio](#mute-audio-and-video).
- [Enable or disable video](#mute-audio-and-video).
- [Choose between the front or rear camera](#toggle-cameras).

**Note:** This sample is written in [Kotlin](https://kotlinlang.org), a language officially supported by Android.

## Prerequisites

- Android Studio 3.5+.
- Android device (e.g. Pixel 4). A real device is recommended because some simulators have missing functionality or lack the performance necessary to run the sample.

## Quick Start

This section shows you how to prepare, build, and run the sample application.

### Obtain an App ID

To build and run the sample application, get an App ID:
1. Create a developer account at [agora.io](https://dashboard.agora.io/signin/). Once you finish the signup process, you will be redirected to the Dashboard.
2. Navigate in the Dashboard tree on the left to **Projects** > **Project List**.
3. Save the **App ID** from the Dashboard for later use.
4. Generate a temp **Access Token** (valid for 24 hours) from dashboard page with given channel name, save for later use.

4. Locate the file **app/src/main/res/values/strings.xml** and replace <#YOUR APP ID#> with the App ID in the dashboard.

```xml
<string name="agora_app_id"><#YOUR APP ID#></string>
<!-- Obtain a temp Access Token at https://dashboard.agora.io -->
<!-- You will need to deploy your own token server for production release -->
<!-- Leave this value empty if Security keys/Token is not enabled for your project -->
<string name="agora_access_token"><#YOUR TOKEN#></string>
```

### Run the Application

Ensure USB debugging is enabled on your device under **Settings > Developer options** and connect the device to your computer.

#### Using Android Studio (Recommended)

1. Open the sample application in Android Studio.
2. Select **File** > **Sync Project with Gradle Files**.
3. Build and run the sample project. This should display the application on your device.

**Note:** If your application does not compile in Android Studio,  check the **Build Error** window to troubleshoot: 
- You may need to install additional Android SDK support files.
- You may need to update the Kotlin version number `ext.kotlin_version` in the build.gradle file located in the root folder of the application.

## Resources

- You can find full API document at [Document Center](https://docs.agora.io/en/)
- You can file bugs about this demo at [issue](https://github.com/AgoraIO/Basic-Video-Call/issues)

## License

The MIT License (MIT)
