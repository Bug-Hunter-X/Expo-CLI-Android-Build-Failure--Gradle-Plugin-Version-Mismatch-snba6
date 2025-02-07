# Expo CLI Android Build Failure: Gradle Plugin Version Mismatch

This repository demonstrates a bug and its solution related to Android Gradle Plugin version mismatches when building Android APKs using the Expo CLI.  The bug manifests as a build failure with an error indicating an incompatibility or missing Java JDK version.

## Bug Description

The Expo CLI build process fails due to an issue with the Android Gradle Plugin. The failure message might point to a version incompatibility or a problem locating a compatible JDK.  This is often caused by discrepancies in Gradle settings, conflicts with other Android projects, or an incorrectly configured Android SDK environment.

## How to Reproduce

1. Clone this repository.
2. Try to build the Android APK using `expo build:android`.
3. Observe the build failure and error messages.

## Solution

The provided `bugSolution.gradle` file shows the corrected Gradle configuration.  The key changes may involve:

* Specifying the correct Android Gradle Plugin version in the project's `build.gradle` file. 
* Ensuring the project has a properly configured JDK path and that the correct Java version is set in the environment variables.
* Checking for any dependency conflicts or outdated components that might be causing issues.

## Contributing

Contributions are welcome!  If you encounter similar issues or have further solutions, feel free to submit a pull request.
