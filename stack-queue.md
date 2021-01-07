# Stacks and Queues

## Stack
**It is a type of data structure which conatins a bunch of nodes, where these nodes hve a reference from each other.**

### Terminology related to the stack
- **_Push_** node or item that are added to the last of the stack list.
- **_Pop_** removes of the last node or item in the stack.
- **_Top_** the last node or item within the stack.
- **_Peek_** to view the value of top or last node of the stack.

***Check out the folowing figure to understand the stack how it looks like and the terminology that we've mentioned them before.***
![Stack Visualization](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/stack1.PNG)

### Stack Concept
- **_FILO_** stand for first in last out, which means the item that you are going to add it, will be the last node popped out of the stack.

- **_LIFO_** stand for last in first out, which means the item that you are going to add lately it, will be the first node popped out of the stack.

### Push and Pop a node in the stack
It is a simple process that you only need to push the new node and assign it as a top of the stack, then the you assign the next node as the original top. The same process would go with the pop.
![Push Node](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/pushStack3.PNG)

## What is Queue?

### Terminology related to the queue
- **_Enqueue_** node or item that is added to the queue.
- **_Dequeue_** node or item that is removed from the queue.
- **_Front_** the first node or item in the queue.
- **_Rear_** the last node or item in the queue.
- **_Peek_** to view the value of front or first node in the queue.
- **_IsEmpty_** to check if the queue is empty or not.
***By understanding the terminologies above, you will be then familiar on how the queue will look like as the following figure.***
![Queue Visualization](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Queue.PNG)

### Queue Concept
- **_FIFO_** stand for first in first out, which the first node that are added will be the first one will pop out of the queue.
- **_LILO_** stand for last in last out, which the last node in the queue will be the last node will pop out of the queue.


### Example of Enqueue in the Queue
The idea would be changing the net value of first node to be pointed out to the added node which is by using the method rear. Then, reassign the rear into the added node and make it next value to the null.
![Enqueue in Queue](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Enqueue3.PNG)