# React useEffect Hook Unexpected Behavior

This repository demonstrates a common issue with React's `useEffect` hook where the effect only runs once instead of on every state change.  The problem lies in the dependency array, which is incorrectly left empty.

## Problem

The provided `bug.js` file shows an example where the `useEffect` hook logs a message to the console.  It was expected that the message would be logged every time the `count` state variable changes. However, because of the empty dependency array [], the effect runs only once when the component mounts.

## Solution

The `bugSolution.js` file provides a corrected version of the code. The solution includes the `count` state variable in the dependency array. This ensures that the effect runs whenever the `count` value changes.