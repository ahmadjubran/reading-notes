# Putting it all together

## What is the single responsibility principle and how does it apply to components?

SRP is a principle that states that a class should have only one reason to change. It is a way to make sure that a class is not too complex and that it is easy to test.

## What does it mean to build a ‘static’ version of your application?

It means that you can run your application without any dependencies. This is useful for testing and development.

## Once you have a static application, what do you need to add?

Identify The Minimal (but complete) Representation Of UI State

## What are the three questions you can ask to determine if something is state?

- Is it passed in from a parent via props? If so, it probably isn’t state.
- Does it remain unchanged over time? If so, it probably isn’t state.
- Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where state needs to live?

- Identify every component that renders something based on that state.
- Find a common owner component (a single component above all the components that need the state in the hierarchy).
- Either the common owner or another component higher up in the hierarchy should own the state.
- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## What is a “higher-order function”?

Functions that take other functions as arguments or return functions as results.

## Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

It will return a function that will take a number and return true if it is greater than the number passed in.

## Explain how either map or reduce operates, with regards to higher-order functions

The map method returns a new array with the results of the function applied to each element.

## Things I want to know more about
