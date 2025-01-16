# Infinite Re-renders in React useEffect Hook

This repository demonstrates a common error in React applications: infinite re-renders caused by a missing dependency array in the `useEffect` hook.

## The Problem

The `useEffect` hook in the `bug.js` file is missing a dependency array. This causes the effect to run after every render, triggering a continuous update cycle that results in an infinite loop.

## The Solution

The solution, provided in `bugSolution.js`, adds a dependency array to the `useEffect` hook. This array specifies that the effect should only run when the `count` variable changes.  This prevents the infinite loop.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the infinite re-renders in the console and the unresponsive application.
5. Examine the corrected code in `bugSolution.js` to understand the solution.
