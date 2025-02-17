# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common error in React 19's `useEffect` hook and its solution.  Improperly managing dependencies in `useEffect` can lead to unexpected infinite re-renders. 

## Bug
The `bug.js` file showcases a component that falls into an infinite loop due to a missing dependency in `useEffect`.  The `console.log` statement will show that the component renders repeatedly. 

## Solution
The `bugSolution.js` file corrects the problem by adding `count` to the dependency array of `useEffect`. This ensures the effect only runs when the `count` value actually changes. 

## How to reproduce
1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install`
4. Run `npm start`
5. Observe the console output and the component's behavior in the browser. Compare the original buggy behavior and fixed behavior.