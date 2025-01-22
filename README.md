# Expo Go Crash: Invariant Violation: Objects are not valid as a React child

This repository demonstrates a bug in Expo Go where an 'Invariant Violation: Objects are not valid as a React child' error occurs when rendering images with incorrect image source data. The solution involves carefully verifying that the image source is a string URI and not an object.

## Bug Description
The Expo Go app crashes when trying to display an image using the Image component if the source is not a correctly formatted string URI.

## How to Reproduce
Clone this repository and run the app in Expo Go. The app will crash due to the error in the `bug.js` file.  This is because the image source is an object, not a string.

## Solution
The `bugSolution.js` file contains the corrected code. The solution ensures the image source is always a valid string URI.