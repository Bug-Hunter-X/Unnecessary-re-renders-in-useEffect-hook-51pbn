# Unnecessary Re-renders in React's useEffect Hook

This repository demonstrates a common React bug involving the `useEffect` hook.  The provided `MyComponent` uses `useEffect` without specifying dependencies, causing it to execute after every render. This leads to performance issues due to unnecessary re-renders and console logging. The solution demonstrates how to correctly use the dependencies array to control when the effect runs.

## Bug

The initial code causes unnecessary re-renders and console logs every time the component renders, leading to wasted processing power.  This is inefficient and can affect performance, especially as the application grows in complexity.