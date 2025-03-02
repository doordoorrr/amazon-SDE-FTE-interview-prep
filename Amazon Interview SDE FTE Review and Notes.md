---
tags: [amazon]
title: Amazon Interview SDE FTE Review and Notes
created: '2025-03-01T23:07:12.204Z'
modified: '2025-03-02T05:43:18.188Z'
---

# Amazon Interview SDE FTE Review and Notes
**todo:** 
keep being u :)
### Tips
---
**Before Coding:** Ask clarifying questions before jumping in to code the problem. Voice your assumptions – this will help the interviewer steer you back on track if needed. Ask for examples and use them to validate your ideas.

**During Coding:** Explain your decision making. Describe your code. Write syntactically correct real code vs. pseudocode. Try to be consistent in your naming conventions and it will make testing/optimizing easier later. If you forget a specific API or specific link into an array, etc., you’re welcome to ask the interviewer who should be able to help you.

**After Coding:** Test your code and talk through optimizing the solution if it can be further optimized if there is more time. Most important here is that you should focus on having a working and fully coded solution on the board to the problem by the end of each interview. If it’s easier for you to start with an inefficient brute force approach and then optimize from there at the end, it’s a perfectly valid approach. Just state that up front with your interviewer. Brute force solution is better than an incomplete solution.

**Clarifying Questions**
Always ask clarifying questions to ensure you fully understand the problem. For example:

- Input/output format (e.g., "Can the input array be empty?").

- Edge cases (e.g., "What should the output be if the input is invalid?").

- Constraints (e.g., "What’s the expected range of input size?").

**Coding Best Practices**
- Modular Code: Write clean, modular code with helper functions if needed. This shows you can write maintainable code.

- Naming Conventions: Use meaningful variable names (e.g., maxProfit instead of mp).

Edge Cases: Always test for edge cases (e.g., empty input, large input, negative numbers).

**Optimization**
- Start with a brute-force solution if you’re unsure of the optimal approach. Then, optimize step by step.

- Explain your thought process as you optimize (e.g., "This approach has O(n²) time complexity, but we can improve it to O(n) by using a hash map.").
---
## Round Structure
1. Tech/LP
    Focus on **medium leetcode** problems. Be ready to explain your thought process and optimize your solution.

    *"I was asked two DSA problems in this round; This was followed by two Leadership Principles (LP) questions. This was 30 min LP + 30 min coding(1 LC medium)"*

2. Tech/LP
    Similar to Round 1, but may involve **more complex problems or follow-up questions**. Practice problems involving trees, graphs, and dynamic programming.

    *"Started with two LP questions, followed by a matrix-based DSA problem. Expectation: Write optimal, modular code and handle follow-up questions."*

3. BAR RAIIIISERRR
    Be prepared to discuss your **past projects and how they align with Amazon’s principles**. If system design is included, practice designing basic systems (e.g., a parking lot system, a URL shortener, FACEBOOK which is questionable in an amazon interview... u get the point).
    





#### Leadership Principles to Focus On

  *Customer Obsession:* Think of a time you went above and beyond to help a customer or user.

  *Ownership:* Share a story where you took responsibility for a project or task.

  *Invent and Simplify*: Describe a time you came up with a creative solution to a problem.

  *Learn and Be Curious*: Talk about how you learned a new skill or technology to solve a problem. 


*"Just understand the design patterns and go through some common questions. Try and think what patterns you can apply. Implement one or two to understand how much time you will take..in this round you don't have to write all the getter setters and the boilerplate code. You can just tell it to the interviewer that you are gonna skip it to save time. And practicing one or two questions will help you in getting an idea of how much time you need to spend on writing code and which code you should skip. Best of luck"*

----
## Data Structures & Algorithms Key Topics:


	- Arrays, Strings, Linked Lists, Stacks, Queues
	- Trees (Binary Trees, BST, Tries)
	- Graphs (BFS, DFS, Shortest Path)
	- Hash tables, Heaps
	- Sorting and Search Algorithms 
	- Dynamic Programming, Recursion, Backtracking

Practice Platforms:
-
	- LeetCode (+ CrackTech)
	- Neetcode
	- Grind75
	- HackerRank
	- CodeForces (??)
----
 Focus on Amazons Recently Asked Q's
- 
[LeetCode Problems CheckList](LeetCode Problems CheckList.md)

	- CrackTech
	- glassdoor Amazon SDE interview questions
	- low level design questions
		- show off: OOP & design patterns
	- distrubuted systems design

----

# (LOW LEVEL) System Design
[Low-Level System Design](Low-Level System Design.md)

Key Topics:
-
      - OOP Principles: 
			- Encapsulation
			- Inheritance
			- Polymorphism
			- Abstraction
      - Design Patterns: 
		    - Singleton
		    - Factory
		    - Observer
      - Distributed Systems
			- Load Balancing 
			- Caching 
			- Databases
	  - Design Scalable Systems 
			- URL shortener
			- chat system
			- scalable key-value store 
			- monitoring system, track server-side errors in real time
			- distrubuted cache
			- rate limiter
			- web crawler 

		
### Common Low-Level Design Problems
- Design a Parking Lot
- Design a Library Management System
- Design a Chess Game
- Design a URL Shortener (basic version)

## Approach to Low-Level Design
- Clarify Requirements: Ask questions to understand the scope (e.g., "How many users will the system support?").

- Define Core Classes and Relationships: Identify the main entities and their relationships.

- Write Clean Code: Focus on modularity, readability, and scalability.

- Discuss Trade-offs: Be prepared to explain why you chose a particular design (e.g., "I used a hash map for O(1) lookups.")

---
# Master Amazon's LP Principles 
 
### Study The Principles:
	- Review all 16 Amazon LP's
### Prepare STAR Stories: 
		- Situation, Task, Action, Result
		- Prepare a story from my experience in STAR Formatt for all 16 principles

## Review Docs
### [Data Structures & Algorithms](Data Strucutures & Algorithms.md)
### [Design Patterns](Design Review.md)
### [Time/Space Complexity](Time/Space Complexity Review.md) 
### [Low-Level System Design](Low-Level System Design.md)
### [LeetCode Problems CheckList](LeetCode Problems CheckList.md)
### [Amazon Leadership Principles](Amazon Leadership Principles.md)
### [My Interview Questions](My Interview Questions.md)



