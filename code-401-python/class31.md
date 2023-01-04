# Context API
---
## What is Global State
- In React, originally, the state is held and modified within the same React component. In most applications, different components may need to access and update the same state. This is achieved by introducing the global states in your app. The main purpose of the global state is to share a state among multiple components.

- There are three ways this communication can happen:

  - With a child component
  - With a parent component
  - With a sibling component
---
State traveling down State traveling down through the hierarchy is best managed using the mutable state at the highest level to determine immutable properties that define the lower-level components.

State traveling up You need to pass down a callback function for a higher-level component to know the state. In the following version, we add a global state to count the total number of button presses and update this state with a callback function called pushed, which is called whenever a button is pushed.

---
## Context API in React
Context provides a way to pass data through the component tree without having to pass props down manually at every level.
- When to Use Context Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.
- Before You Use Context
  - Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

  - If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.