# React useEffect Hook with Empty Dependency Array Bug

This repository demonstrates a common error when using the `useEffect` hook in React. The `useEffect` hook with an empty dependency array runs only once when the component mounts, not on every state change. This can cause unexpected behavior if the component's logic relies on state changes.

## Bug
The `bug.js` file contains a React component that uses the `useEffect` hook with an empty dependency array. The `console.log` statement inside the `useEffect` is only executed once when the component mounts, and it does not update on every click. 

## Solution
The `bugSolution.js` file demonstrates how to fix the bug.  We add the state variable 'count' to the dependency array, causing the `useEffect` to run whenever 'count' changes.