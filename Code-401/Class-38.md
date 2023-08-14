[Back to Home](../README.md)

## Reading Class-38: React 2

**1. Lifting State Up in React:**

Lifting state up involves moving state from a child to a parent component, enabling shared state and simplifying data flow.

Benefits:
- **Single Source of Truth**: Avoids duplication and inconsistencies.
- **Data Sharing**: Allows multiple components to access the same data.
- **Simpler Child Components**: Child components focus on presentation.
- **Easier Debugging**: Predictable data flow for debugging.
- **Scalability**: Helps maintain a clear data flow.

**2. Conditional Rendering in React:**

Conditional rendering shows different UI based on conditions, using JSX and JavaScript expressions.

Example:
```jsx
const Greeting = ({ isLoggedIn }) => {
  return isLoggedIn ? <h1>Welcome back!</h1> : <h1>Please log in.</h1>;
};
```

**3. Thinking in React:**

Methodology for designing React apps:
- **Component-Based**: Break UI into reusable components.
- **Single Responsibility**: Components have one task.
- **Data Flow**: Identify data flow between components.
- **Hierarchical Structure**: Reflect UI hierarchy in components.
- **Separation of Concerns**: Separate rendering from state.
- **Start with Static UI**: Design static UI structure first.
- **Identify State Needs**: Decide where state should be.
- **Unidirectional Data Flow**: Pass state down, actions up.
- **Iterate and Refine**: Develop iteratively, improving components.

*- Author: Almothana Almasri*