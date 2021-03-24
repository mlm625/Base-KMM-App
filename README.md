# Base-KMM-App
A foundation for building KMM Apps with Jetpack compose and Swift UI.  This is similar to using
Android Studio to create a KMM project, but uses Jetpack compose for the Android UI portion of the
project setup. 

## Android Studio
Make sure you have the latest Canary build. 
- KMM is in alpha, but only available through preview.
- Jetpack Compose is only supported on Canary builds.

Get from: https://developer.android.com/studio/preview

## Temporary Workarounds
- Work around for https://youtrack.jetbrains.com/issue/KT-43944
- jcenter() is still used. Can't be removed until the Kotlinx dependencies move to mavenCentral.

## Apple Silicon
If you jumped in head first and got a new M1 laptop, read on.

### IOS Simulator Builds
Arm64 is excluded from all simulator builds. This does not affect production builds. The short
explanation is Xcode doesn't support this yet, even if you are running on apple silicon. 

For details, see https://stackoverflow.com/questions/63607158/xcode-12-building-for-ios-simulator-but-linking-in-object-file-built-for-ios

### Android Virtual Devices
- Don't worry about the Intel hardware acceleration errors when setting up Android AVD manager. You are not running on intel. 
- You do need to create arm64 versions of any android devices you want to develop on. AVD manager makes this super easy.


