# Thinking in React

## How would you break a mock into a component heirarchy?
+ ## first you should  draw boxes around every component (and subcomponent) in the mock and give them all names.
+ ## use the single resposibility principle to decide what should be it's own component , (component should do only one thing).
+ ## arrange them into a hierarchy, Components that appear within another component in the mock should appear as a child in the hierarchy.


## What is the single responsibility principle and how does it apply to components?
+ ## techniques for deciding if you should create a new function or object.
+ ## component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.


## What does it mean to build a ‘static’ version of your application?
+ ## a version of app which use props but dont use state because this version doesnt have data changing over time (not interactive) .

## What are the three questions you can ask to determine if something is state?
1. ## Is it passed in from a parent via props? If so, it probably isn’t state.
2. ## Does it remain unchanged over time? If so, it probably isn’t state.
3. ## Can you compute it based on any other state or props in your component? If so, it isn’t state.

## How can you identify where state needs to live?
+ ## Identify every component that renders something based on that state.
+ ## Find a common owner component (a single component above all the components that need the state in the hierarchy).
+ ## Either the common owner or another component higher up in the hierarchy should own the state.
+ ## If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.






# [back](../README.md)
