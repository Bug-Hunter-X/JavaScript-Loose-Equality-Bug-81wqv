# JavaScript Loose Equality Bug
This repository demonstrates a common error in JavaScript related to loose equality (==) and its interaction with null and undefined values. The bug involves the use of loose equality to check for null values, leading to incorrect results.

## The Problem
The `foo` function is intended to add two numbers. However, it uses loose equality (`==`) to check for null values which can lead to unexpected results.  Loose equality performs type coercion before comparison which can lead to unexpected behavior.  For example, `null == undefined` evaluates to `true` even though they are distinct values.

## The Solution
The solution uses strict equality (`===`) to check for null values, preventing type coercion and ensuring that only the values explicitly checked for are matched.  Strict equality is safer and more predictable. 

## How to Reproduce
1. Clone this repository.
2. Open `bug.js` and observe the behavior of the `foo` function using loose equality.
3. Open `bugSolution.js` and observe how using strict equality solves the problem.

