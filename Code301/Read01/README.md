# Introduction to React and Components

## What Is React?

**React** is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “_**components**_”.

- **Components** are reusable pieces of code that we can compose into larger components.

- We use **components** to tell React what we want to see on the screen. When our data changes, React will efficiently update and re-render our components.

- A component takes in parameters, called `props` (short for “**properties**”), and returns a hierarchy of views to display via the `render` method.

- Passing **props** is how information `flows` in React apps, from parents to children.

### Characteristics of Components

- **Reusability** - Components can be used multiple times in our app.

- **Replaceable** - Components can be easily replaced by other components.

- **Not context specific** - Components can be used in any context.

- **Extensible** - Components can be easily extended.

- **Encapsulated** - Components are easy to understand and test.

- **Independent** - Components are designed to have minimal dependencies on other components.

## Advantages of using component-based architecture

1. Ease of deployment

1. Reduced cost

1. Ease of development

1. Reusable

1. Modification of technical complexity

1. Reliability

1. System maintenance and evolution

1. Independent

## Hello World in React

```jsx
const root = ReactDOM.createRoot(document.getElementById("root"));

root.render(<h1>Hello, world!</h1>);
```

## Introducing JSX

**JSX** is a syntax extension to `JavaScript`, and it produces `React` “**elements**”

### Why JSX?

- Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both

- using JSX is optional, but it is helpful as a visual aid when working with UI inside the JavaScript code.

## Rendering Elements

Unlike browser `DOM elements`, `React elements` are plain objects, and are cheap to create. **React DOM** takes care of updating the **DOM** to match the **React** elements.
