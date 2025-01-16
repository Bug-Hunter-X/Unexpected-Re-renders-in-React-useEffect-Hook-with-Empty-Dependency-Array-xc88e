# Unexpected Re-renders in React useEffect Hook

This repository demonstrates an uncommon bug related to the React `useEffect` hook where unexpected re-renders occur even with an empty dependency array `[]`.  The component re-renders unnecessarily, leading to performance issues and potential logic errors.

## Bug Description

The `useEffect` hook with an empty dependency array should typically only run once, after the component mounts. However, in this case, the component re-renders multiple times despite no state changes. This is likely caused by an external factor subtly triggering updates.