# Android Appium Grader

This repository contains the Dockerfiles to build the Android grader. The Docker image includes an Android emulator, the Appium test automation framework, and the Android SDK. The Android SDK is used for communication by Appium to send commands to the emulator. Headless support is supported by xvfb (X virtual framebuffer).

The software versions included are: 

| Component     | Version       |
| ------------- |:-------------:|
| Java                   | jdk1.8.0_131 |
| Android SDK            | 25.2.3       |
| Android Build Tools    | 25.0.3       |
| Android Virtual Device | 25           |
| Appium                 | 1.6.5        |


This image also includes scripts for conveniently integrating to the A+ learning management system. The scripts parse the output of the testing system and send back the results to A+ via an API.

### Dockerfiles

There are 2 Dockerfiles:
  - **Dockerfile.x86**: Builds a Docker image with an x86 emulator with KVM support. This type of emulator is much faster and is the recommended approach.
  - **Dockerfile.armeabi-v7a**: Builds a Docker image with an armeabi-v7a emulator. This emulator is quite slow and should be used only when the host OS does not provide KVM support.

  Note that the same android application binary (apk) can be installed in any of the emulators without anz special compilation parameters.

### Running the containers

Instructions on running the containers as well as sample exercises are provided in a separate repository: https://github.com/aolecloudscape/android-exercises

