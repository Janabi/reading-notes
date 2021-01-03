# Linked Lists

### What is eactly link list?
**It is a sequence of nodes, which contain items and lists, are connected to each other. There are two types of liked list which they are Sigly and Doubly.**

### Terminology in linked list:
- Linked List - A data structure that has a nodes which it links to other nodes.
- Singly - means that each node has only one single reference to other node, which it will probably be the next one.
- Doubly - means that each nodes has two references, which they will be the next and previous ones.
- Node - they are a set of items or links that related to its linked lists, this node contains a data.
- Next - It is a reference for each node to have except the last one.
- Head - The first node inside the linked list.
- Current - It is kind of a pointer that tells you where your are currently at which node in the linked list.

### How does the linked list looks like
![Example of linked list](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/LinkedList1.PNG)

### How we are going to walk through all of the nodes inside a singly linked list
**It is first we declare the Head of the nodes, which is the first one we will begin. Then, we will go through a while loop. The condition of this loop is that if the Current node's value is not equal to 'null' then continue going on the Next node until you reach the last one.**

### How to add a node at the begining
**It is just making the Current for the Head and then we will add the new nodes by defining this newNode.next will equal to the Head and then we set the Head for newNode and make it the current node among the rest.**
![Adding Examplt at Head](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/LinkedList4.PNG)

### What if we want to add a node at certain position within the linked list
**It is just defining what the node will be Next the one we will added it AddBefore, so we would use the while loop until we notice that we reached the node value after the added one, then we used the AddBefore to add this node to that position.**
![Adding node at Certain Position](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/LLInsert5.PNG)

### Type of Data Structure
- Linear data structure - means that would be linear and walk next to each other.
- Non-linear data structure - means that the node itslef might have a multiple connection to other.

### Lists for all shapes and sizes
**Linked list might return a certain shapes to reach a proper connections between the nodes.**