# In memory storage

## What is a ‘call’?

A call is a request to the storage system to store a piece of data.
The storage system will respond with a call ID, which can be used to retrieve the data later.

## How many ‘calls’ can happen at once?

The storage system is limited to a certain number of calls at once. This number is configurable.

## What does LIFO mean?

LIFO means ‘last in, first out’. This means that the most recent call will be the first to be retrieved.

## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```js
function firstFunction() {
  console.log("Hello from firstFunction");
}

function secondFunction() {
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
```

## What causes a Stack Overflow?

when there is a recursive function (a function that calls itself) without an exit point.

example:

```js
function callMyself() {
  callMyself();
}

callMyself();
```

## What is a ‘reference error’?

A reference error is when a variable is referenced before it is defined.

## What is a ‘syntax error’?

A syntax error is when the code is not written correctly.

## What is a ‘range error’?

A range error is when a variable is outside of the range of values it can take.

## What is a ‘type error’?

A type error is when a variable is not of the correct type.

## What is a breakpoint?

A breakpoint is a point in the code where the debugger stops.

## What does the word ‘debugger’ do in your code?

The debugger is a tool that allows you to stop the code at a certain point.
