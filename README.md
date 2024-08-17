# Common Hooks in React: useCallback & useRef

This repository contains examples and explanations of two commonly used React hooks: `useCallback` and `useRef`. These hooks are essential for optimizing performance and managing references in React components.


## Introduction

React hooks provide a powerful way to manage state, side effects, and other React component functionalities. Among them, `useCallback` and `useRef` are particularly useful for optimizing performance and handling references to DOM elements or other values across renders.

## useCallback

`useCallback` is a hook that returns a memoized version of the callback function that only changes if one of the dependencies has changed. This is particularly useful when passing callbacks to child components that rely on referential equality to prevent unnecessary re-renders.

### Example:

```javascript
const memoizedCallback = useCallback(() => {
  doSomething(a, b);
}, [a, b]);
```
### useRef
useRef is a hook that returns a mutable ref object whose .current property is initialized to the passed argument. This object persists for the lifetime of the component. useRef is commonly used to access DOM elements directly or store mutable values that do not cause re-renders when updated.

Example:
```
const inputEl = useRef(null);
const focusInput = () => {
  inputEl.current.focus();
};
```
## Getting Started 
1. Clone the repository:

   ```bash
   git clone <repository-url>

2. Navigate to the project directory:
     ```bash
    cd <project-directory>

3. npm install
     ```bash
    npm install

4. Start the development server:
     ```bash
    npm start/  npm run dev

## Acknowledgements
This project uses React and its hooks to demonstrate practical applications of state management and performance optimization.
