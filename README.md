# React Native FlatList Performance Issue

This repository demonstrates a common performance problem encountered when using `FlatList` in React Native with large datasets and computationally expensive item renderers. The issue manifests as slow rendering, dropped frames, and potential crashes.

## Problem

The provided `bug.js` file contains a `FlatList` component rendering a large dataset. Each item in the list is rendered by a `ComplexComponent` that performs unnecessary recalculations during rendering, leading to significant performance degradation.

## Solution

The `bugSolution.js` file presents a solution that addresses the performance issue by implementing techniques like `useMemo`, `React.memo`, and optimizing the `renderItem` function to minimize unnecessary re-renders and computations.

## Setup

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npx react-native run-android` or `npx react-native run-ios` to run the app.