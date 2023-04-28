# Exercise: ContextAPI

## Description:

A `CounterContext` that provides a count state and two methods to increment and decrement the count. Two components, `IncrementButton` and `DecrementButton`, that use these methods to increment or decrement the count respectively. Then a third component, `CounterDisplay`, that displays the current count using data from the `CounterContext`.

- The `CounterContext` should provide a state called `count` with an initial value of `0`, and two methods, `increment` and `decrement`, that update the count state.
- The `IncrementButton` component should use the `increment` method from the CounterContext to increment the count when clicked.
- The `DecrementButton` component should use the `decrement` method from the CounterContext to decrement the count when clicked.
- The `CounterDisplay` component should display the current count using data from the `CounterContext`.

## Here are the steps to complete this exercise:

- Create a new file called `CounterContext.tsx`. Inside this file, create a new `CounterContext` using the `createContext` function from the react library.
- In CounterContext.tsx, create a new state variable called `count` with an initial value of `0`, using the `useState` hook from the react library.
- In `CounterContext.tsx`, create two new methods called `increment` and `decrement` that update the `count` state, using the `setState` function returned by the useState hook.
- Wrap the `IncrementButton` and `DecrementButton` components in the `CounterContext.Provider` component in order to provide the `count`, `increment`, and `decrement` values to these components.
- In `IncrementButton.tsx`, create a new button that calls the `increment` method from the CounterContext when clicked.
- In `DecrementButton.tsx`, create a new button that calls the `decrement` method from the CounterContext when clicked.
- In `CounterDisplay.tsx`, use the `useContext` hook from the react library to access the count value from the CounterContext. Render this value to the screen.
