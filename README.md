# React Native Uninitialized State Bug

This repository demonstrates a common bug in React Native: accessing a state variable before it has been initialized.  The bug is reproduced in `UninitializedStateBug.js`, and a solution is provided in `UninitializedStateSolution.js`.

## Bug Description

In functional components, if you try to access state within the render method before the component mounts and the state is set, you'll encounter an error because the state will be `undefined`.

## Solution

The best way to avoid this is to ensure state initialization occurs appropriately before use. We can do this with the help of useState hook and conditional rendering.