# Analysis-of-Algorithms

This is in compliance with our Analysis of Algorithms project.

Below are the snippets of code, a brief explanation of how each data structure operates, and a screenshot of the terminal upon running it.

## Linked Lists

### Circular Linked Lists

![Circular Linked Lists]([Output/circular.png](https://raw.githubusercontent.com/Quinc0/Analysis-of-Algorithms-PT/refs/heads/Output/circular.png))

Circular Linked Lists are lists that are a lot like Singly Linked Lists except the last node points back to the first one, creating a loop. This type of linked list has continuous traversal due to the loop. The first node points to the second, the second to the third, and so on, until it reaches the last node which points back to the first node.

### Singly Linked Lists

![Singly Linked Lists](Output/singly.png)

Singly Linked Lists are lists of nodes that point only to the next node. Unlike Circular Linked Lists, the last node of this list points to `NULL`, ending the list. The first node points to the second, and so on. The last node points to `NULL` because it has nothing else to point to.

### Doubly Linked Lists

![Doubly Linked Lists](Output/doubly.png)

Doubly Linked Lists are lists where each node points to both the next node and the previous node. This allows traversal in both forward and backward directions. The first node points to the second, the second to the third, and so on. Each node also points back to its predecessor.

## Queues

![Queues](Output/queues.png)

A Queue is a First In, First Out (FIFO) data structure where elements are added to the back (enqueue) and removed from the front (dequeue). It is commonly used in scenarios where order needs to be preserved, such as processing tasks or handling requests.

## Heaps

![Heaps](Output/heaps.png)

A Heap is a complete binary tree that satisfies the heap property. In a max-heap, the value of each node is greater than or equal to the values of its children. In a min-heap, the value of each node is less than or equal to the values of its children. Heaps are often used to implement priority queues.

## Trees

![Trees](Output/trees.png)

A Tree is a hierarchical data structure consisting of nodes, with a root node at the top and child nodes below. Each node contains data and references to its children. A Binary Tree is a type of tree where each node has at most two children, referred to as the left child and right child.

## Graphs

![Graphs](Output/graphs.png)

A Graph is a collection of nodes (vertices) and edges that connect pairs of nodes. Graphs can be directed or undirected. Common operations on graphs include traversal methods.

## Stack

![Stack](Output/stack.png)

A Stack is a Last In, First Out (LIFO) data structure where elements are added to (push) and removed from (pop) the top of the stack. It is often used in scenarios requiring reverse order processing, such as undo mechanisms in text editors.

## Getting Started

To use the code provided in this repository, simply clone the repository and compile the C++ files using your preferred compiler.

```sh
git clone <repository-url>
cd <repository-directory>
g++ -o executable <filename.cpp>
./executable
