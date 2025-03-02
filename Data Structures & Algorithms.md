---
tags: [amazon]
title: Data Structures & Algorithms
created: '2025-03-01T23:08:59.024Z'
modified: '2025-03-02T06:58:15.804Z'
---

# Data Structures & Algorithms
**todo:** 
fill out sections, review, displace the bottom notes
 Key Topics:
-
	- Arrays, Strings, Linked Lists, Stacks, Queues
	- Trees (Binary Trees, BST, Tries)
	- Graphs (BFS, DFS, Shortest Path)
	- Hash tables, Heaps
	- Sorting and Search Algorithms 
	- Dynamic Programming, Recursion, Backtracking
	- Vectors


# Review
- [ ] Arrays
    Common problems: Two Sum, Reverse String, Longest Substring Without Repeating Characters.

    Techniques: Sliding Window, Two Pointers.
- [ ] Strings


- [ ] Linked Lists
**Head** - front of list
**Tail** - end of list
**Nodes**- The node of a singly or a circular linked list has two parts: data and the address of the next node
  Common problems: Reverse Linked List, Detect Cycle, Merge Two Sorted Lists.
  **![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeS7qCbug7nhdn6mFQn9KbhU4zxQ7EnYbuJfu8oKVbD3eV8zYzyy8LLHF4YPxfC4h53RGdFtFNGnhEtA5T-spYRdl7I253IayHo5faqBVGK-Y1TKSNweqUz9Ku9xa18aMpRIGNGXcBeK1ROj1XwVXlLu3KK?key=e-2d-Tg1rURhdDRXhi3Q_cfU)**
  **![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcu-3Pq968WDhnBCSjMWl4X0CpeH9ao-0NDpjgYwXrkKfPJHcQ090Un6j8qugygsWlxfuESNSg3OK-TrVJXoliqMqGfzJcPxKn2UNdeWWw3xhxiPSjIvvmhv5ppqDtRzqVXxroyrIo5lZz_Hl6YsKldZIDu?key=e-2d-Tg1rURhdDRXhi3Q_cfU)**


 Definition for singly-linked list.

      struct ListNode {
		     int val;
		     ListNode *next;
             ListNode() : val(0), next(nullptr) {}
             ListNode(int x) : val(x), next(nullptr) {}
             ListNode(int x, ListNode *next) : val(x), next(next) {}
      };


  Techniques: Dummy Nodes, Fast and Slow Pointers.

- [ ] Stacks
A stack is like a physical stack. You can only work with what's on top **(FILO)**
-   push()  add on top of stack
    
-   pop()  returns and removes the data on top of the stack
    
-   peek()  return the data on top without removing it

- [ ] Queues
Que is like standing in line **(FIFO)**


- [ ] Binary Trees
  Each node has up to two children - the left and right child.


  **Leaf**
  A tree node with no children.

  **Internal Node**
  A node with at least one child.

  **Parent**
  The node with a child is that child node’s parent.

  **Ancestors**
  Include the parent node, that parents parent node, and so on.

  **Root**
  The top node of the tree that has no parent.

  **Edge**
  The link from a node to a child.

  **Depth**
  The number of edges on the path from the root to the node. For example, the root node has a depth of zero.

  **Level**
  All nodes with the same depth make up a tree level.

  **Height**
  The largest depth of any node. A tree with one node has a height of zero. Minimum height of a BST is N - 1 (N being the # of nodes) and the minimum height is log2N.
    Common problems: Maximum Depth of Binary Tree, Validate BST, Lowest Common Ancestor.

    **Techniques:** Recursion, BFS, DFS.

- [ ] BST

  Has an ordering property where:
    - Left subtree’s keys must be ≤ node’s key
    - Right subtree’s keys must be ≥ node’s key

*Start by visiting root node, checking to see if it matches the desired key. Else if, check if desired key is less than the current node. If so, visit left child and repeat. Else if, check if desired key is greater than the current node. If so, visit the right child and repeat.*
**BST Insert Algorithm**
Inserts a new node in the proper location according to the BST ordering property. It starts with the root as the current node, and compares the new node with the current node to see if the new node’s key is less than/equal to or greater than/equal to the current node’s key. 

**BST Tree Traversal**

Visits all nodes in the tree once and performs an operation on each node

  
  

**BST Inorder Traversal**

Visits all nodes in a BST from smallest to largest, starting at the root, it prints the left subtree, current node, and then right subtree.

  

**BST GetHeight Algorithm**

If node is null, return -1. Otherwise, recursively compute left and right child subtree heights, and return 1 plus the greater of the 2 child subtree’s heights.

  

**BST Recursive Search Algorithm**

A single node and search key are passed as arguments.

Two base cases:

1.  If node == null, return null. If not, the search key is compared to the node’s key.
    
2.  When the search key == node key, return node. If the search key is less than the node’s key, recursion is called on the node’s left child and if the search key is greater than the node’s key, recursion is called on the node’s right child.

- [ ] Tries

- [ ] Graphs 

**Graph**

A data structure for representing connections among items. Made up of vertices connected by edges.

  

**Vertex**

Node that represents an item in a graph.

  

**Edge**

Represents the connection between two vertices in a graph.

  

**Adjacency**

Two vertices are adjacent if connected by and edge.

  

**Path and Path Length**

A path is a sequence of edges leading from a starting vertex to an ending vertex. The path length is the number of edges in the path.

  

**Distance**

The distance between two vertices is the number of edges on the shortest path between those vertices.

  

**Adjacency List**

A type of graph representation where each vertex has a list of adjacent vertices, each list item representing an edge.

  

**Sparse Graph**

A graph that has far fewer edges than the maximum possible.

  

**Adjacency Matrix**

Graph representation where each vertex is assigned to a matrix row and column. A matrix element is 1 if the corresponding two vertices have an edge or 0 if it does not.


    

  

**Directed Graph / Digraph**

Graph where vertices are connected by directed edges.

  

**Directed Edge**

A connection between a starting vertex and a terminating vertex.

  

**Cycle**

A path that starts and ends at the same vertex. A directed graph is cyclic if it contains a cycle and acyclic if the graph does not.

  

**Weighted Graph**

A graph where is edge has a weight (aka cost). Can be directed or undirected.

  

**Weight / Cost**

Represents some numerical values between vertex items, such as flight cost between airports or travel time between cities.

  

**Path Length / Cycle Length**

In a weighted graph, it is the sum of edge weights in the path / sum of edge weights in a cycle.

  

**Negative Edge Weight Cycle**

Cycle that has a cycle length less than 0 (aka the shortest path does not exist).
  Common problems: Number of Islands, Clone Graph, Shortest Path.

  Techniques: BFS, DFS, Dijkstra’s Algorithm.
- [ ] BFS
**Breadth-First Search**

A type of graph traversal that visits a starting distance, then all vertices that are distance 1 from that vertice, then all that are distance 2, and so on without revisiting a vertex.

-   Enqueue the starting vertex in a queue
    
-   While the queue is not empty, dequeue a vertex from the queue, visit the dequeued vertex, enqueues that vertex’s adjacent vertices (if already not discovered), and repeat.

- [ ] DFS
**Depth-First Search**

A graph traversal that visits a starting index, then visits every vertex along each path starting from that vertex to the path’s end before backtracking.

-   Push the starting vertex to a stack
    
-   While the stack is not empty, pop the vertex from the top of the stack
    
-   If the vertex hasn’t been visited, visit it and push the adjacent vertices to the stack
    

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdw_7LotcoWEG3pwJyeNHMlDlKjiV-0K7CO0jL-rz3LI--vTb_2EgIOIBu3b6DavotWef0gyUEr6fU7tEL2_mRFw2iYLfGkR-B_23mlddtpw7PPcysvCFXCnfmCuquWHG3AC2DKOrDuKYJFvckF41knVmoT?key=uwWIfGGJyPp2BAxqVpPwzA)

**Recursive Depth-First Search**

Implemented using the program stack instead of an explicit stack.

-   First called with the staring vertex (1 argument)
    
-   Visit vertex if not already visited and perform recursion for each adjacent vertex
- [ ] Shortest Path

- [ ] Hash tables
  -  A data structure that stores unordered items by mapping (or hashing) each item to a location in an array or vector.
    - Unique keys mapped onto an index location in an array for easy lookup

- [ ] Heaps

**Max-Heap**

A complete binary tree that maintains the property that a node’s key is greater than or equal to the node’s children’s keys (so a max-heap’s root node will always have the max key).

  

**Max-Heap Insert**

Inserts node into the tree’s last level, then swaps the node with it’s parent until there is no max-heap property violation. Insert for max-heap fills each level, left-to-right, before adding any new levels, so the height is always the minimum possible height.

  

**Percolating**

The upward movement of a node in a max-heap.

  

**Max-Heap Remove**

Always removes the root by replacing the root with the last level’s last node, and swapping that node with its greatest child until there is no max-heap property violation.

  

**Min-Heap**

The same as a max-heap except a node’s key must be less than or equal to its children’s keys (so the root node is always the minimum key).

**Heap Storage**

Heaps are typically stored using arrays where the root is index 0, the root’s left child is index 1, the root’s right child is index 2, and so on.

  

**Calculation for Parent and Child Indices in a Heap**

Node  Parent Index  Child Indices (left, right)

i [(i - 1)/2]  2 * i +1, 2 * i +2

  

**Heapsort**

A sorting algorithm that uses the max-heaps properties by repeatedly removing the max and building a sorted array in reverse order.

  

**Heapify**

Operation used to turn an array into a heap. Heapifying to build a max-heap is done by percolating down on every non-leaf node in reverse order (because leaf nodes already satisfy the max heap property) starting at the internal node with the largest index.
- [ ] Sorting and Search Algorithms 

- [ ] Dynamic Programming
  Common problems: Fibonacci, Longest Increasing Subsequence, Knapsack.

  Techniques: Memoization, Tabulation.

- [ ] Recursion

- [ ] Backtracking

- [ ] Vectors
A vector is a dynamic array that can resize itself automatically when elements are added or removed.
#### **Key Features**

-   **Dynamic Sizing**: Unlike arrays, vectors can grow or shrink in size.
    
-   **Random Access**: Elements can be accessed in O(1) time using indices.
    
-   **Contiguous Memory**: Elements are stored in contiguous memory locations, making traversal efficient.
    
        #include <vector>
        #include <iostream>
        
        int main() {
            std::vector<int> vec = {1, 2, 3};  // Initialize vector
            vec.push_back(4);                   // Add element
            vec.pop_back();                     // Remove last element
            std::cout << vec[0];                // Access element (output: 1)
            return 0;
        }
        
- [ ] traversals
trees: DFS, BFS
Linear DS: interative traversal, recursive
graphs: DFS, BFS

### **Example: Tree Traversal in Python**



    class TreeNode:
        def __init__(self, val=0, left=None, right=None):
            self.val = val
            self.left = left
            self.right = right
    
    def inorder_traversal(root):
        if root:
            inorder_traversal(root.left)
            print(root.val)
            inorder_traversal(root.right)


- [ ] divide and conquer
A problem-solving paradigm where a problem is broken into smaller subproblems, solved recursively, and then combined to solve the original problem.
### **Key Steps**

1.  **Divide**: Break the problem into smaller subproblems.
    
2.  **Conquer**: Solve the subproblems recursively.
    
3.  **Combine**: Merge the solutions of subproblems to solve the original problem.
 - [ ] trade-offs between relational and non-relational databases
 
### **Relational Databases (SQL)**

-   **Structure**: Data is stored in tables with rows and columns.
    
-   **Schema**: Fixed schema (predefined structure).
    
-   **ACID Compliance**: Ensures data integrity (Atomicity, Consistency, Isolation, Durability).
    
-   **Use Cases**: Complex queries, transactions, and relationships (e.g., banking systems).
    

### **Non-Relational Databases (NoSQL)**

-   **Structure**: Data is stored in key-value pairs, documents, graphs, or wide-column stores.
    
-   **Schema**: Flexible schema (dynamic structure).
    
-   **Scalability**: Horizontally scalable (add more servers to handle load).
    
-   **Use Cases**: Large-scale applications, unstructured data (e.g., social media, IoT)
### **Example Use Cases**

-   **Relational**: Banking systems, inventory management.
    
-   **Non-Relational**: Social media platforms, real-time analytics.



------

You should also know some of the languages’ nuances, such as how memory management works, or the most commonly used collections, libraries, etc.

You’ll be expected to know the runtimes for common operations as well as how they use memory.

Consider reviewing common algorithms such as traversals, divide and conquer, breadth-first search vs. depth-first search and understand the trade-offs for each.

Knowing the runtimes, theoretical limitations, and basic implementation strategies of different classes of algorithms is more important than memorizing the specific details of any given algorithm.




given a problem definition, you should be able to formulate it as a machine learning problem and propose a solution, including ideas for data sources, annotation, modeling approaches, and potential pitfalls. Understand the basic AI/ML methods and algorithms. Revisit your favorite ML and AI textbooks.
