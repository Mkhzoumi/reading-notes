# In memory storage

## What is a ‘call’?
+ ## it is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

## How many ‘calls’ can happen at once?
+ ## One call.

## What does LIFO mean?
+ ## it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
+ ## example:

```
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
```

## What causes a Stack Overflow?
+ ## stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.
+ ## example:

```
function callMyself(){
  callMyself();
}

callMyself();
```


## What is a ‘refrence error’?
+ ## it's when you try to use a variable that is not yet declared.

```
console.log(foo) // Uncaught ReferenceError: foo is not defined
```


## What is a ‘syntax error’?
+ ## when you have something that cannot be parsed in terms of syntax.

```
JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1
```

## What is a ‘range error’?
+ ## Try to manipulate an object with some kind of length and give it an invalid length.

```
var foo= []
foo.length = foo.length -1 // Uncaught RangeError: Invalid array length
```

## What is a ‘tyep error’?
+ ## when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

```
var foo = {}
foo.bar // undefined
foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined
```


## What is a breakpoint?
+ ## it allows you to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting.

## What does the word ‘debugger’ do in your code?
+ ## adds a breakpoint.





# [back](../README.md)