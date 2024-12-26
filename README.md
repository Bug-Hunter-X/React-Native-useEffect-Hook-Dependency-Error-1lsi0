# React Native useEffect Hook Dependency Error

This repository demonstrates a common error in React Native applications involving the `useEffect` hook. The `useEffect` hook is not re-running when the state variable changes because the dependency array is missing the state variable.

## Problem

The provided `bug.js` file contains a React component that uses the `useState` hook to manage a counter. The `useEffect` hook is intended to log the current count to the console. However, due to an incorrect dependency array, the effect only runs once when the component mounts and not when the count changes.

## Solution

The `bugSolution.js` file demonstrates the corrected code. By including `count` in the dependency array, the `useEffect` hook now correctly updates whenever the `count` variable changes.