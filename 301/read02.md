# react component lifecycle
## component lifecycle event: The methods that you are able to use on component. 
## react component lifecycle has three phases:
1. ## Mounting: it's the phase where the instant of component is being created and inserted into the DOM.
+ ## lifecycle events during mounting in order: Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount.
2. ## Updating: it's when a component is updated or stat changes.
+ ## lifecycle events during updating in order: static getDerivedStateFromProps, shouldComponentUpdate, render,getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps
3. ## Unmounting: it's when a component is being removed from the DOM.
+ ## lifecycle events during unmounting in order: componentWillUnmount.

# React props Vs state.
## What types of things can you pass in the props?
+ ## static information

## What is the big difference between props and state?
+ ## state is handled inside the component and you can update it inside the component but props are handled outside of the component and must be updated outside of the component.

## When do we re-render our application?
+ ## when we change the state inside of the application.

## What are some examples of things that we could store in state?
+ ## user inputs inside of a form


# [back](../README.md)
