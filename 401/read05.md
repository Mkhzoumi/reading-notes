# linked list
### definition 
it's a sequence of nodes that are connected to each other, each node is a reference to the next node in the link.

### types of linked list:
+ singly linked list.
+ doubly linked list.
+ circular linked list.
+ doubly circular linked list.

### the most commonly used linked list is the singly linked list.

### Terminology
+ the linked list is considered as a data structure type, each node links to the next node in the list.
+ in a singly linked list each node has only one reference which points to the next node in the list.
+ in doubly linked list each node has two references, one for the next node and the other for the previous node.
+ nodes they are the items which live in the linked list.
+ next is a property for node which contains the reference to the next node.
+ head is a reference for the first node in the linked list.

### how the linked list look
in this picture you will see how the singly linked list looks like:

![singly](https://miro.medium.com/max/953/1*iiEWrP2IznA6HbmuIdK0lQ.png)

### Traversal
when we want to traverse a linked list we cant use regular loop methods like for or foreach, we depends on 'Next' property in each node to guide us to next reference.

one of the best ways to approach a traversal is by using while() , this will allow you to keep checking the Next node if its null.

in linked list if we try to traverse on a null node, the program will crash after it throws an error.

### adding new node to the front.

first thing you need to knwo is that you have to pay attention to all the references to be properly assigned.
the big O notation (both time and space complexity) of adding to the front method is always equals to O(1) .

#### adding steps:
+ first we use the Add() method to pass the value of the node.
+ then we want our newNode.Next to point to the same location that the Head is pointing at.
+ re assign Head to point at the newNode.

![adding](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/Linkedlist_insert_at_start.png)

```
public void push(int new_data)
{
    // 1 & 2: Allocate the Node &
    //         Put in the data
    Node new_node = new Node(new_data);
 
    // 3. Make next of new Node as head 
    new_node.next = head;
 
    // 4. Move the head to point to new Node 
    head = new_node;
}
```

### Add a node to the middle:

the big O notation of adding to the middle method is equals to O(n) because it uses a loop.

#### adding steps:
+ first we use the Add() method to pass the value of the node.
+ then use AddBefore or SddAfter method they are the same.
+ traverse while the next node is not null.
+ do a check for the value of the next node before moving current to the next node,if it equals to the value we want to put our newNode before.
+ set the newNode Next equal to the existing node.

![add-to-middle](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/Linkedlist_insert_middle.png)


#### there is another method to add to the middle with an O(1) compexity here is its code:

```
public void insertAfter(Node prev_node, int new_data)
{
    /* 1. Check if the given Node is null */
    if (prev_node == null)
    {
        System.out.println("The given previous node cannot be null");
        return;
    }
 
    /* 2. Allocate the Node &
    3. Put in the data*/
    Node new_node = new Node(new_data);
 
    /* 4. Make next of new Node as next of prev_node */
    new_node.next = prev_node.next;
 
    /* 5. make next of prev_node as new_node */
    prev_node.next = new_node;
}
```


#### linked list is a linear data structure type, that means in order to get to the end of it you have to go through all of the items in the list in order, on the other hand there is the non linear data structure in which items dont have to be arranged in order, you just can traverse the data non sequentially.

![linear](https://res.cloudinary.com/practicaldev/image/fetch/s--wF54a3fE--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/3bkjjgn42bsgj34gayc6.png)

## [BACK](../README.md)