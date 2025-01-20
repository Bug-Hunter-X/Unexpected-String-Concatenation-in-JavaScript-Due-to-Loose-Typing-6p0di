# Unexpected String Concatenation Bug in JavaScript

This repository demonstrates a common, yet subtle, bug in JavaScript related to its loose typing system. When performing arithmetic operations, JavaScript will automatically convert operands to strings if at least one of them is a string, leading to string concatenation instead of numerical addition.

## Bug Description
The `foo` function intends to add two numbers. However, due to the loose typing nature of JavaScript, when a number and a string are passed as arguments, the `+` operator performs string concatenation rather than numerical addition, producing unexpected results.

## How to Reproduce
1. Clone this repository.
2. Run `bug.js` using a JavaScript engine (Node.js, browser console, etc.).
3. Observe the unexpected output in the console.

## Solution
The `bugSolution.js` file provides a solution by explicitly converting the arguments to numbers before performing the addition operation, ensuring the correct numerical result.  Always type-check your inputs to avoid unexpected behavior.