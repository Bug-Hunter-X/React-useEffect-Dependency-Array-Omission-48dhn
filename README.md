# React useEffect Dependency Array Issue

This repository demonstrates a common error in React's `useEffect` hook: omitting necessary state variables from the dependency array.  This can lead to unexpected re-renders and infinite loops.

## Bug
The `bug.js` file contains a `useEffect` hook that's missing a crucial dependency. This causes the component to re-render infinitely, filling the console with messages and potentially freezing the browser.

## Solution
The `bugSolution.js` file shows the correct implementation.  The state variable `count` is added to the dependency array, ensuring the effect runs only when the `count` changes.