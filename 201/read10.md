# *error handling and debugging*
## *variable scope:*
1. ## *global scope: variables were declared outside a function, it can be used anywhere.*
2. ## *function-level scope: variables were declared inside a function, it can only be used within the function.*

## *the stack*
## *javascript interpreter prossed one line of code at a time, so when statement need data from another function it stacks the other function on top of the corrent task.*
## *In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it.*
## *Each execution context can also access its parent's v a ri ables object.*

# *error objects*
## *Error objects can help you find where your mistakes are and browsers have tools to help you read them.*
## *there are seven types of error objects in javascript:*

| Object                    | Description                                                       |
| -----------               | -----------                                                       |
| error                     | Generic error - the other errors are all based upon this error    |
| Syntax Error              | Syntax has not been followed                                      |
| Ref erenceError           | Tried to reference a variable that is not declared/within scope   |
| TypeError                 | An unexpected data type that cannot be coerced                    |
| Range Error               | Numbers not in acceptable range                                   |
| URI Error                 | encodeURI ().decodeURI(),and similar methods used incorrectly     |
| Eval error                | eva l () function used incorrectly                                |

## *If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements.* 
## *Debugging is the process of finding errors.* 
## *if your code has an error, The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.*

# [back](../README.md)