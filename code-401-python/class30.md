# Next- Forms and Conditional Rendering
---
### Custom Hooks
Custom Hook is a function that starts with the word "use" and can call other Hooks. Custom Hooks allow you to extract reusable logic from your components and share it across your application. They are a way to encapsulate stateful logic and abstract it away from your components, making your code more reusable, modular, and easier to understand.

Custom Hooks are a powerful feature of React that allow you to reuse stateful logic across your application. They can help you avoid duplication of code and make your components more reusable and maintainable.
---
### Lifting State Up

lifting state up refers to the process of moving shared state to a common ancestor component, rather than keeping it local to a specific component. This is often necessary when multiple components need to access and update the same state.

- Lifting state up is a common pattern in React that allows you to share state between components and manage it

---
### Thinking in React

In order to think in React you need to go though a couple of steps, and assuming that you as a developer have a design mock and some JSON data you need to do the following:

1. Break The UI Into A Component Hierarchy:
During this stage you need to find your components and look for their connections, and the best way to find that is to think of the single responsibility principle, where each component should be handling one thing only, then you start to look if this component is dependent on another to complete it's job.

2. Build A Static Version in React:
During this stage you will be trying to just build the components and make them work as intended, ad because you are building a static version remember, don't use state at all, as this version isn't supposed to be interactive.

3. Identify The Minimal (but complete) Representation Of UI State:
During this stage you need to start making the UI interactive using states, and to do that think of the minimal set of mutable state that your actually app needs.

4. Identify Where Your State Should Live:
In order to do this you need to think of a couple of things: - Where does the state make sense. - does it need direct access to another state higher in the hierarchy. - the last option if the state home isn't identified you need to build a new component to solely hold it.
---
### Memoization in React
Memoization is a technique in which the result of a function is cached and returned from the cache when the same input is provided again, rather than recalculating the result. It is a way of improving the performance of a function by avoiding unnecessary computation.

In React, memoization can be used to optimize the performance of components by avoiding unnecessary re-renders. When a component re-renders, it means that it is being updated with new props or state and its render method is being called again. This can be inefficient if the component is doing a lot of computation or if the props or state are not actually changing.