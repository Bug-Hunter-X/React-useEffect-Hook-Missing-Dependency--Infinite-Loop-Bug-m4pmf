# React useEffect Hook Missing Dependency Bug

This repository demonstrates a common error in React's `useEffect` hook: forgetting to include all necessary dependencies in the dependency array.  This can lead to infinite loops and unexpected behavior.

## The Bug
The `bug.js` file contains a component that uses `useEffect` to log the current count. However, the dependency array is missing a key dependency, resulting in the effect running on every render.