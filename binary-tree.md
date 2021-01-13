# Binary Tree
**Binary tree, it visalize as a natural tree where it has a root and leaves.**

## Terminology
- **_Root_** is the first node in the binary tree where it will contain another branches that are linked to it, Also it will consider as a parent.

- **_Node_** where each tree has as a set of nodes are looks like a natural tree.

- **_left child_** Where each parent node has in the left side of its branch.

- **_right child_** Where each parent node has in the right side of its branch.

- **_Edge_** is the connection  between the parent and its children.

- **_Lead_** is the last nodes in the tree where there will be no branches.

- **_Height_** is the number of the egdes along the binary tree.

## Binary Tree

![Sample Binary Tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)
**So all of what we are going to learn about tree which it will be specificly a binary type which means that each parent node will have two children. So let us assume that we will going to add a node in the binary tree, so how are we going to know where we should put this node exaclty.**

**Well, first thing, we will check the top parent node if exist or not. if yes it does, then we will move forward. Therefore, if the passing data value is leass than the parent data value. Then, assign it as a left child if it's not exist. If yes, then definitly the data will be then bigger than the parent node data value, then assign this value to the right node if it does not exist. Then if nothing works, so move to the child and check thier nodes again.**

**At the removing node function, we will do a process of walking through the entire node until reaching the one that is eactly equal to the same value that we just passed it as a parameter of the function.**

**Then how we are going to traverse the tree itself?**

By walking on  either one of these methods:
- Pre-order which it will start from the root, and then going forward.
- In-order which will start from the left and then top till the right.
- Post-order which will start from the right and then top till the left.

![Pre-order traversal](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/DepthTraversal11.PNG)