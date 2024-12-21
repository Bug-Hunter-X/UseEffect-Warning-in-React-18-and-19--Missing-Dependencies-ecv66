# React 18/19 useEffect Warning: Missing Dependencies

This repository demonstrates a common issue encountered when upgrading to React 18 or 19 involving the `useEffect` hook.  Incorrectly specifying the dependency array in `useEffect` can lead to unexpected behavior and warnings in the console.

The `bug.js` file contains the problematic code. The `bugSolution.js` file provides a corrected version.

**Problem:**

The original code includes a `useEffect` hook without the correct dependency array.  This results in unnecessary re-renders and warnings in React 18+. 

**Solution:**

The solution demonstrates the correct way to define the dependency array.  By including `count` in the dependency array, the effect only runs when `count` changes.