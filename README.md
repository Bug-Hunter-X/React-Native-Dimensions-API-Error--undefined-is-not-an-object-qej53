# React Native Dimensions API Error: undefined is not an object

This repository demonstrates a common but often cryptic error in React Native related to the `Dimensions` API.  The error typically manifests as `undefined is not an object (evaluating 'Dimensions.get')`. This usually stems from issues with installation or linking of the necessary native modules.

## Bug Reproduction

The `DimensionsBug.js` file shows how to trigger the error. This is done by attempting to access `Dimensions.get('window')` without having properly set up the environment.

## Solution

The `DimensionsBugSolution.js` file presents a working example which shows how to fix the issue. The solution centers around double-checking the following:

1. **Ensure React Native and its dependencies are correctly installed.**
2. **Verify that the React Native project is properly linked to the native modules.**  This might involve running linking commands provided by your project setup (e.g., `react-native link`).
3. **Clean and rebuild your project.**  Sometimes a simple `react-native run-android` or `react-native run-ios` after cleaning the build folders can resolve the problem.
4. **Check for conflicting versions.** Ensure you have compatible versions of React Native, its dependencies and any other libraries that might use Dimensions.

This repository illustrates the error and provides a solution. For more advanced troubleshooting, refer to the official React Native documentation and community forums.