# Expo Linking.getInitialURL() - Intermittent Null Return on Android

This repository demonstrates a bug in Expo's `Linking.getInitialURL()` API on Android. The function intermittently returns `null`, even when a deep link is successfully opened, preventing the app from handling the intended action.  The issue seems related to timing and is difficult to consistently reproduce.

## Reproducing the Issue

Follow the instructions in the `bug.js` file to see the inconsistent behavior.  The issue is more likely to be observed on some devices than others and may require multiple attempts to reproduce consistently.

## Solution

The `bugSolution.js` file presents a possible workaround.  This approach involves checking the `getInitialURL()` result multiple times or using a more reliable alternative if available for your specific app.  This is not a perfect solution and depends on the implementation.

## Contributing

Contributions are welcome! If you have a more robust solution, or can identify the root cause of the issue, please open a pull request.