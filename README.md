# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: an infinite loop caused by improper state updates within the `useEffect` hook.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides the corrected implementation.  The issue arises from the state update within useEffect depending on the current state, leading to continuous re-renders and triggering the effect repeatedly. This can freeze or crash your application. 

## Solution:

The solution involves updating the state correctly using functional updates. This ensures that the `useEffect` hook doesn't trigger endlessly.
