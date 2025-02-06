# React useEffect Infinite Loop

This repository demonstrates a common bug in React's `useEffect` hook: an infinite loop caused by incorrect dependency management.

The `bug.js` file contains the buggy code. The `bugSolution.js` file shows the corrected version.

## Bug Description
The component increments a counter. When the count goes above 5, it resets to 0. However, this is implemented incorrectly within the useEffect hook, creating an infinite loop because the component continuously updates the count state.