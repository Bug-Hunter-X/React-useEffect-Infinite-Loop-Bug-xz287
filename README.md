# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: causing an infinite loop by directly updating state without a dependency array or functional update.  The `bug.js` file shows the erroneous code, and `bugSolution.js` provides the corrected version.

The problem stems from directly modifying `count` within the `useEffect` hook without specifying a dependency array.  This creates a continuous update cycle, resulting in a crash.