# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook.  The provided code creates an infinite loop due to an incorrect dependency array.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders. However, if the dependency array is missing or incorrect, it can lead to unexpected re-renders and infinite loops.  This example showcases an infinite loop scenario caused by omitting necessary dependencies.

## Solution
The solution involves correctly specifying the dependency array for the `useEffect` hook.  By adding `count` to the dependency array, the effect only runs when the `count` value changes, preventing the infinite loop. 