# Stacks and Queues

### Stack
its a type of data structure, consists of Nodes, each one of them references the next one in the stack, but they didnt reference to previous.

#### stack terminology
1. push: means to put an item into the stack.
2. pop: means to remove an item from the stack.
3. peek: means to view the value of the top node of the stack.
4. isEmpty: checking if the stack is empty return true else return false.

#### stack concepts
+ (FILO)first in last out: means that the first node added to the stack will be the last to popped out of the stack.
+ (LIFO) last in first out: last node added to the stack will be the first to popped out of the stack.

![stack-concept-img](https://miro.medium.com/max/814/0*pdhOeAK6wSh8ipTW.png)


#### push O(1)
+ when pushing a node to the stack its always a O(1) operation.
+ when we add a node to the stack we push it by assigning it as the new top and we make its next property equals to the original top.

here is the pseudocode of pushing a node to the stack:

```
ALOGORITHM push(value)
// INPUT <-- value to add, wrapped in Node internally
// OUTPUT <-- none
   node = new Node(value)
   node.next <-- Top
   top <-- Node
```

#### pop O(1)
+ removing a node from the top of the stack is also an O(1) operation.
+ when popping the top node out of the stack , the top node will be re-assigned to the node that lives below .
+ you must check isEmpty before popping to be sure that exception is not raised.

the pseudocode for a pop:

```
ALGORITHM pop()
// INPUT <-- No input
// OUTPUT <-- value of top Node in stack
// EXCEPTION if stack is empty

   Node temp <-- top
   top <-- top.next
   temp.next <-- null
   return temp.value
```

#### Peek O(1)
peek operation only inspecting the top node of the stack, in peek also you should check isEmpty before you peek so you will ensure not to raise an exception.

pseudocode of peek

```

ALGORITHM peek()
// INPUT <-- none
// OUTPUT <-- value of top Node in stack
// EXCEPTION if stack is empty

   return top.value
```

#### IsEmpty O(1)
return true if the stack is empty and false if not.

pseudocode of isEmpty 

```
ALGORITHM isEmpty()
// INPUT <-- none
// OUTPUT <-- boolean

return top = NULL
```

### Queue
#### terminology 
1. Enqueue - Nodes or items that are added to the queue.
2.Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
3. Front - This is the front/first Node of the queue.
4. Rear - This is the rear/last Node of the queue.
5. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
6. IsEmpty - returns true when queue is empty otherwise returns false.

#### queue concepts
+ (FIFO) first in first out: means the first item in the queue will be the first out of the queue.
+ (LILO) last in last out: means that the last item in the queue will be the last item out of the queue.

![queue](https://dz2cdn1.dzone.com/storage/temp/8350689-fifo-queue.png)

## [BACK](../README.md)