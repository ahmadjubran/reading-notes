# Redux Advance

## What is Redux Toolkit?

Redux Toolkit is a package that contains a set of tools to help you write Redux logic more easily. It is intended to be the standard way to write Redux logic, and includes packages we think are essential for building a Redux app. It is our attempt to help standardize Redux usage, improve usage through best practices, and provide a good development experience for Redux users.

## What is the purpose of Redux Toolkit?

Redux Toolkit is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

- "Configuring a Redux store is too complicated"
- "I have to add a lot of packages to get Redux to do anything useful"
- "Redux requires too much boilerplate code"

## Why should I use Redux Toolkit?

Redux Toolkit is our attempt to address these concerns. It is intended to be the standard way to write Redux logic, and includes packages we think are essential for building a Redux app. It is our attempt to help standardize Redux usage, improve usage through best practices, and provide a good development experience for Redux users.

## What is included in Redux Toolkit?

Redux Toolkit includes the following packages:

- configureStore() - A store creator that uses the most common Redux middleware out-of-the-box, and lets you add more as needed
- createReducer() - A helper that generates a reducer function for you based on the logic you provide
- createAction() - A helper that generates an action creator function for you based on the logic you provide
- createSlice() - A helper that generates a slice reducer with corresponding action creators and action types, all from a single configuration object
- createSelector() - A memoized selector that can compute derived data, allowing Redux to store the minimal possible state
- createEntityAdapter() - A set of standardized tools for managing normalized data in your store
- createAsyncThunk() - A helper that generates action creators and action types for async logic that follows a common pattern

## How do I use Redux Toolkit?

Redux Toolkit is available as the redux-toolkit package on npm. You can install it with npm or yarn:

```bash
npm install @reduxjs/toolkit
```

## What is createSlice in Redux Toolkit?

createSlice is a function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. The "slice" is the name we give to the generated reducer logic and actions.

## How do I use createSlice in Redux Toolkit?

- First, import the createSlice function from Redux Toolkit
- Then, call createSlice and pass in an initial state value, an object full of reducer functions, and a slice name
- The createSlice function will generate all the action creators and action types that we need to write the reducer logic
- Finally, export the generated reducer function by calling slice.reducer
