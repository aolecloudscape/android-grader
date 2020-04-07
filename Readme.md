# Android Appium Grader

This repository contains the Dockerfiles to build the grader. It is meant to integrate into A+.

There is an android emulator contained inside the produced Docker image, which has the following characteristics: 


| Component     | Version       |
| ------------- |:-------------:|
| Java                   | jdk1.8.0_131 |
| Android SDK            | 25.2.3       |
| Android Build Tools    | 25.0.3       |
| Android Virtual Device | 25           |

### Dockerfiles

There are 2 Dockerfiles:
  - **Dockerfile.armeabi-v7a**: Using the armeabi-v7a emulator. Appium 1.6.5
  - **Dockerfile.x86**: Using the x86 emulator with KVM. Appium 1.6.5

