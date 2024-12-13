# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common closure issue in JavaScript when using `setTimeout` within a loop.  The expected behavior is to log numbers 0 through 9 with a one-second delay between each. However, due to the way closures work, all instances of `setTimeout` capture the final value of `i`, resulting in ten 10's being logged.

The `bug.js` file contains the problematic code. The `bugSolution.js` file provides a corrected version, illustrating how to properly capture the value of `i` using an immediately invoked function expression (IIFE).