---
tags: [amazon]
title: Time/Space Complexity Review
created: '2025-03-01T23:10:05.969Z'
modified: '2025-03-02T05:17:32.750Z'
---



# Time/Space Complexity Review
## 1. Basics
### **What is Time Complexity?**

-   Time complexity measures how the runtime of an algorithm grows as the input size increases.
    
-   It’s expressed using  **Big O notation**  (e.g., O(n), O(n²), O(log n)).
    

### **What is Space Complexity?**

-   Space complexity measures how much additional memory an algorithm uses as the input size increases.
    
-   It’s also expressed using  **Big O notation**.
Common Time Complexities
--

 - O(1): Constant time (e.g., accessing an array element).
 - O(log n): Logarithmic time (e.g., binary search).
 - O(n): Linear time (e.g., iterating through an array).
 - O(n log n): Linearithmic time (e.g., merge sort).
 - O(n²): Quadratic time (e.g., nested loops).
 - O(2ⁿ): Exponential time (e.g., recursive Fibonacci).

#### **Common Space Complexities**

-   **O(1)**: Constant space (e.g., a single variable).
    
-   **O(n)**: Linear space (e.g., an array of size n).
    
-   **O(n²)**: Quadratic space (e.g., a 2D matrix).


#### **Tips for Analyzing Complexity**

-   **Count Operations**: Estimate the number of operations your algorithm performs.
    
-   **Consider Worst-Case Scenarios**: Focus on the worst-case time/space complexity.
    
-   **Optimize Trade-offs**: Sometimes, you can trade space for time (e.g., using a hash map for faster lookups).

### **What is Space Complexity?**

-   Space complexity measures how much additional memory an algorithm uses as the input size increases.
    
-   It’s also expressed using  **Big O notation**.
    

----------

## **2. Big O Notation**

Big O notation describes the  **upper bound**  of an algorithm’s complexity in the  **worst-case scenario**. Here’s a quick overview of common complexities:


| Complexity     | Description                                                      | Example                                  |
|----------------|------------------------------------------------------------------|------------------------------------------|
| **O(1)**       | **Constant** time/space. Doesn’t depend on input size.               | Accessing an array element.              |
| **O(log n)**   | **Logarithmic** time/space. Grows slowly as input size increases.    | Binary search.                           |
| **O(n)**       | **Linear** time/space. Grows proportionally with input size.         | Iterating through an array.              |
| **O(n log n)** | Linearithmic time/space. Common in efficient sorting algorithms. *n*-**log**-*n* | Merge sort, Quick sort.                  |
| **O(n²)**      | **Quadratic** time/space. Grows rapidly with input size.             | Nested loops.                            |
| **O(2ⁿ)**      | **Exponential** time/space. Grows very rapidly.                      | Recursive Fibonacci.                     |
| **O(n!)**      | **Factorial** time/space. Extremely slow for large inputs.           | Generating all permutations of a string. |

## **3. Steps to Calculate Time Complexity**

### **Step 1: Identify the Input Size (n)**

-   Determine what  **n**  represents (e.g., length of an array, number of nodes in a tree).
    

### **Step 2: Count the Operations**

-   Count how many times each operation is executed in terms of  **n**.
    
-   Focus on the  **dominant term**  (the term that grows fastest as  **n**  increases).
    

### **Step 3: Simplify Using Big O Rules**

-   **Drop Constants**: O(2n) → O(n).
    
-   **Drop Lower-Order Terms**: O(n² + n) → O(n²).
    
-   **Consider Worst-Case Scenario**: Assume the worst-case input.

## **4. Steps to Calculate Space Complexity**

### **Step 1: Identify the Input Size (n)**

-   Same as for time complexity.
    

### **Step 2: Count the Additional Memory Used**

-   Count the memory used by:
    
    -   Variables.
        
    -   Data structures (e.g., arrays, hash maps).
        
    -   Recursion stack.
        

### **Step 3: Simplify Using Big O Rules**

-   Same rules as for time complexity.
## **5. Examples of Time and Space Complexity Analysis**

### **Example 1: Linear Search**


	def linear_search(arr, target):
	    for i in range(len(arr)):  # O(n)
	        if arr[i] == target:   # O(1)
	            return i           # O(1)
	    return -1                  # O(1)

-   **Time Complexity**: O(n) (worst case: iterate through the entire array).
    
-   **Space Complexity**: O(1) (no additional memory used).
    

----------

### **Example 2: Binary Search**



	def binary_search(arr, target):
	    left, right = 0, len(arr) - 1  # O(1)
	    while left <= right:           # O(log n)
	        mid = (left + right) // 2  # O(1)
	        if arr[mid] == target:     # O(1)
	            return mid             # O(1)
	        elif arr[mid] < target:   # O(1)
	            left = mid + 1        # O(1)
	        else:                     # O(1)
	            right = mid - 1       # O(1)
	    return -1                     # O(1)

-   **Time Complexity**: O(log n) (halves the search space each iteration).
    
-   **Space Complexity**: O(1) (no additional memory used).
    

----------

### **Example 3: Bubble Sort**



	def bubble_sort(arr):
	    n = len(arr)                  # O(1)
	    for i in range(n):            # O(n)
	        for j in range(n - i - 1):# O(n)
	            if arr[j] > arr[j + 1]:# O(1)
	                arr[j], arr[j + 1] = arr[j + 1], arr[j]  # O(1)

-   **Time Complexity**: O(n²) (nested loops).
    
-   **Space Complexity**: O(1) (in-place sorting).
    

----------

### **Example 4: Recursive Fibonacci**

	
	def fibonacci(n):
	    if n <= 1:                    # O(1)
	        return n                  # O(1)
	    return fibonacci(n - 1) + fibonacci(n - 2)  # O(2ⁿ)

-   **Time Complexity**: O(2ⁿ) (each call branches into two more calls).
    
-   **Space Complexity**: O(n) (depth of recursion stack).

## 6. Common Patterns, and their Complexities!
*Time Complexity Patterns*
| Pattern                  | Time Complexity | Example                          |
|--------------------------|-----------------|----------------------------------|
| Single loop              | O(n)            | Iterating through an array.      |
| Nested Loop              | O(n^2)          | Bubble sort, checking all pairs. |
| Divide and Conquer       | O(log n)        | Binary Search                    |
| Recursion with Branching | O(2^n)          | Recursive Fibonacci.             |
| Sorting                  | O(n log n)      | merge sort, quick sort.          |
|                          |                 |                                  |

*Space Complexity Patterns*

| Pattern                   | Space Complexity | Example                        |
|---------------------------|------------------|--------------------------------|
| In-Place Algorithms       | O(1)             | Bubble sort: swapping elements |
| Recursion                 | O(n)             | Depth of Recursion Stack       |
| Additonal Data Structures | O(n)             | Storing elements in a hash map |


