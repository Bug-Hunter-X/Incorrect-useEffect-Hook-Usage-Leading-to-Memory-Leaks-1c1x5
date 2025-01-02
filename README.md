# Incorrect useEffect Hook Usage Leading to Memory Leaks

This repository demonstrates a common React error involving the `useEffect` hook and how to fix it. The original code lacks a cleanup function within the `useEffect` hook, leading to potential memory leaks. The solution showcases the correct implementation by including a return function to perform cleanup on unmount.

## Bug Description:

The `useEffect` hook in the `bug.js` file is missing a cleanup function. This can result in memory leaks, as the effect's side effects might not be properly cleaned up when the component unmounts.

## Solution:

The `bugSolution.js` file contains the corrected code. The addition of a return function within the `useEffect` hook ensures that any side effects (like timers or event listeners) are properly cleaned up when the component is unmounted.
