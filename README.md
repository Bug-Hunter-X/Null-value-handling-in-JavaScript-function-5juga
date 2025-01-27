# JavaScript Null Value Handling Bug

This repository demonstrates a common bug in JavaScript related to handling null values in functions.

## Bug Description

The `foo` function is designed to add two numbers. However, it does not explicitly handle cases where either `a` or `b` is null. This can lead to unexpected behavior or errors depending on how null values are treated by the JavaScript runtime.

## Bug Reproduction

1. Clone this repository.
2. Run `bug.js` using a JavaScript runtime (Node.js, for example).
3. Observe that when either `a` or `b` is null, the function returns null, which may not be the desired behavior in all cases.

## Solution

The `bugSolution.js` file demonstrates a possible solution by explicitly checking for null values before performing the addition operation. This way, the function can handle null gracefully and return a more sensible result.  We should also consider whether the default should be 0, null, or an error.