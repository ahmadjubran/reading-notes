# Redux Basic

## What is Redux?

Redux is a predictable state container for JavaScript apps.

## Why use Redux?

- Redux helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test.
- Redux is a great choice for JavaScript apps that have a medium or large size codebase, and are being built by a small team of developers.

## What are the three principles of Redux?

- Single source of truth
- State is read-only
- Changes are made with pure functions

## Terminology

- **Action** - An action is a plain JavaScript object that has a type property. Actions are the only way to get data into the store. You send them to the store using store.dispatch().
- **Action Creator** - An action creator is a function that creates and returns an action.
- **Reducer** - A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change.
- **Store** - The store is the object that brings them together. The store has the following responsibilities:
  - Holds application state;
  - Allows access to state via getState();
  - Allows state to be updated via dispatch(action);
  - Registers listeners via subscribe(listener);
  - Handles unregistering of listeners via the function returned by subscribe(listener).
- **Dispatch** - The only way to update the state is to emit an action, an object describing what happened. This is the only way to trigger a state change.
- **Selector** - Selectors are pure functions that take Redux state as an argument, and return data that is derived from that state. They are used to extract data from the Redux store state, using createSelector.

## Redux Flow

1. The store is created using createStore().
2. The store calls the reducer function you gave it.
3. The root reducer may combine the output of multiple reducers into a single state tree.
4. The Redux store saves the complete state tree returned by the root reducer.
5. The only way to change the state inside it is to dispatch an action on it.
6. The current Redux store state is passed to the mapStateToProps() function.
7. The mapStateToProps() function should return a plain object, which will be merged into the component’s props.
8. If the Redux store state changes, the mapStateToProps() function will be called again. The component will be re-rendered with the new state.

![Alt text](https://d33wubrfki0l68.cloudfront.net/01cc198232551a7e180f4e9e327b5ab22d9d14e7/b33f4/assets/images/reduxdataflowdiagram-49fa8c3968371d9ef6f2a1486bd40a26.gif)
