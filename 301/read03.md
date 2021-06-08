# Lists and Keys

## What does .map() return?
## it returns an array.
## example:

```
const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);
```

## If I want to loop through an array and display each value in JSX, how do I do that in React?
## we use curly braces.
### example:

```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);
```

### Each list item needs a unique ____.
## key

```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);
```

## What is the purpose of a key?
## the keys help React identify which items have changed, are added, or are removed. 
+ ## Most often you would use IDs from your data as keys.


# The Spread Operator
## What is the spread operator?
+ ## it's a quick and usefull way to add items to array,combining arrays or objects, and spreading an array out into a function’s arguments.
+ ## in javascript: spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

## List 4 things that the spread operator can do.
1. ## Copying an array
2. ## Concatenating or combining arrays
3. ## Using Math functions
4. ## Using an array as arguments

## Give an example of using the spread operator to combine two arrays.

```
const myArray = [1,2,3]
const yourArray = [4,5,6]
const ourArray = [...myArray,...yourArray]
```

## Give an example of using the spread operator to add a new item to an array.

```
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
```

## Give an example of using the spread operator to combine two objects into one.

```
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
```


# [back](../README.md)

