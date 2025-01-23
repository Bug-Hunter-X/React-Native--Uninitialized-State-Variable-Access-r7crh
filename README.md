# React Native: Uninitialized State Variable Access

This repository demonstrates a common error in React Native applications: attempting to access a state variable before it has been initialized.  This frequently occurs when dealing with asynchronous operations like data fetching.

## The Problem

The `bug.js` file illustrates the problematic scenario.  It tries to render data from the state before the asynchronous operation to populate it has finished, resulting in an error.

## The Solution

The `bugSolution.js` file provides a corrected implementation using the `useEffect` hook (for functional components) or conditional rendering (for class components) to ensure that the state is initialized before being accessed.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run the app (e.g., with Expo).
4. Observe the error message in `bug.js` and the correct behavior in `bugSolution.js`.