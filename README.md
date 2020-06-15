# Android Appium Grader

This repository contains the Dockerfiles to build the Android grader. It is meant to integrate into A+. See also <https://cloudscape.aalto.fi> for more details.

The produced Docker images have the following software installed.


| Component              | Version      |
| ---------------------- |-------------:|
| Java                   | jdk1.8.0_131 |
| Android SDK            | 25.2.3       |
| Android Build Tools    | 25.0.3       |
| Android Virtual Device | 25           |
| Appium                 | 1.6.5        |

### Dockerfiles

There are two Dockerfiles targeting different architectures of the Android emulator.

  - **Dockerfile.armeabi-v7a**: Using the armeabi-v7a emulator.
  - **Dockerfile.x86**: Using the x86 emulator with KVM.
