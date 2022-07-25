# Passing Functions as Props

## What does .map() return?

map returns an array of the same length as the original array.

## If I want to loop through an array and display each value in JSX, how do I do that in React?

We can use the **.map()** method

```jsx
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) => <li>{number}</li>);
```

## Each list item needs a unique

**string** as a `key`.

Most often you would use **IDs** from your data as `keys`

## What is the purpose of a key?

the **key** is used to identify a specific element in the array.

## What is the spread operator?

The **spread operator** is used to spread out an array into individual elements.

## List 4 things that the spread operator can do.

- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments

## Give an example of using the spread operator to combine two arrays.

```jsx
const array1 = [1, 2, 3];
const array2 = [4, 5, 6];
const array3 = [...array1, ...array2]; // [1, 2, 3, 4, 5, 6]
```

## Give an example of using the spread operator to add a new item to an array.

```jsx
const numbers = [1, 2, 3, 4, 5];
const newNumbers = [...numbers, 6]; // [1, 2, 3, 4, 5, 6]
```

## Give an example of using the spread operator to combine two objects into one.

```jsx
const obj1 = { name: "John" };
const obj2 = { age: 30 };
const obj3 = { ...obj1, ...obj2 }; // { name: 'John', age: 30 }
```

## In the video, what is the first step that the developer does to pass functions between components?

pass the function as a prop.

## In your own words, what does the increment function do?

increases the value of the state by 1.

## How can you pass a method from a parent component into a child component?

We can pass a method as a prop.

## How does the child component invoke a method that was passed to it from a parent component?

we can call the method using `this.props.methodName()`
