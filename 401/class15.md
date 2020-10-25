# Class 15 \| Binary Trees & Binary Search Tree
Article: [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)       

## Basic Concepts of Trees
- Root | this is like the *head* of a Linked List, the starting point of the tree
- Edges | these are the arrows or *next pointer* like in a List
- Trees are made up of **nodes** which contain a value
- In general, trees can have any number of child nodes from the root, however, in **binary tree**, there are only 2 child nodes from the root - a *left* child and *right* child
- Height | The height of a tree typically refers to the number of edges
- Leaves | the children at the very bottom of the tree are referred to as the leaves

> Important: Every node (except the root) has exactly 1 incoming ancestor. This means that in traversal, a node **cannot** traverse to the root through an aunt, it must use it's mother node.

## Looping over Tree Nodes
- Method 1 | **DFS**(Depth First Search)
  - go all the way down a path to the leaf and back up before going down the next set of edges etc. vertical searching
- Method 2 | **BFS**(Breadth First Search)
  - searches at each level, left to right before going to the next deeper level (usually faster)

## Additional Info
- When wanting to "find" a node, it's best to pick the traversal tactic that does the least amount of work, given what you know about the way your tree is designed
- **Binary Search** trees have an additional constraint over classic Binary Tree which is that the **left child** is less than the **root value** and the **right child** is greater than the **root value**
- Adding a node to a Binary Search tree needs more precision in the logic than a randomly assembled classic tree because of the special conditions with the greater and lesser than aspects of the root value

[Back to Home](README.md)