# Expo Constants.deviceName Android Bug

This repository demonstrates a bug where Expo's `Constants.deviceName` API returns an empty string on Android devices inconsistently. This can cause issues in applications that depend on reliable device name retrieval.

## Bug Description

The `Constants.deviceName` API is expected to return the device's name. However, in certain instances on Android, it unexpectedly returns an empty string. This behavior is not consistent and occurs sporadically, making it challenging to debug and reproduce consistently.  This inconsistency can negatively impact app functionality and user experience.

## Reproduction Steps

1. Clone this repository.
2. Run the app on an Android device (emulator or physical device).
3. Observe that `Constants.deviceName` sometimes returns an empty string.

## Solution

The provided solution offers a workaround to mitigate this issue by using a fallback mechanism if `Constants.deviceName` is empty.   Consider using additional device identifiers for more robust device identification, if needed. 