# JavaScript Bug: Unexpected Behavior with Null or Undefined Parameters

This repository demonstrates a common bug in JavaScript related to handling null or undefined parameters in functions.  The `foo` function aims to add two numbers, but its handling of null or undefined values is flawed.

## Bug Description

The `foo` function uses a strict equality check (`===`) to check if either `a` or `b` is null. While this works for null values, it can cause issues if one of the parameters is undefined.

## Solution

The solution improves parameter handling by using loose equality (`==`) or checking for both null and undefined values.

## How to reproduce the bug

1. Clone the repository.
2. Run `node bug.js` to see the original, buggy behavior.
3. Run `node bugSolution.js` to see the corrected behavior.