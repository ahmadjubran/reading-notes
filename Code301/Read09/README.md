# Functional Programming

## What is functional programming?

using functions to the best effect for creating clean and maintainable software.

## What is a pure function and how do we know if something is a pure function?

the function return values are identical for identical arguments (no variation with local static variables, non-local variables, mutable reference arguments or input streams)

They are also pure because they do not depend on any external state or input.

## What are the benefits of a pure function?

    Immutability
    No side effects
    No external dependencies
    Observation
    Referential transparency
    Functions as first-class entities

## What is immutability?

Immutability is the property of data that cannot be changed.

## What is Referential transparency?

Referential transparency is the property of data that can be accessed through a reference to the original object.

## What is a module?

Module is a collection of functions and variables that can be used together.

## What does the word ‘require’ do?

‘require’ is a function that loads a module.

## How do we bring another module into the file the we are working in?

    const module = require(‘module’);

## What do we have to do to make a module available?

    module.exports = {};
