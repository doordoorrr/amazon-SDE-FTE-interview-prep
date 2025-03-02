---
tags: [amazon]
title: (LOW LEVEL) System Design
created: '2025-03-01T23:35:26.786Z'
modified: '2025-03-02T06:20:35.778Z'
---

# (LOW LEVEL) System Design
**todo:** 
- study all sections, then review appraoch & design patterns for solving such problems, then kill it! **

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
      - service-oriented architectures, map-reduce, distributed caching, load balancing, and others
      - memory management, processes, threads, synchronization, paging, and multithreading few basic distributed computing concepts.
      - how browsers function at a high level, from DNS lookups and TCP/IP, to socket connections.
| Topic  |  Run Down |
|---|---|
| **OOP Principles:**   |   |
| Encapsulation  | hide internal details and expose only necessary functionality  |
| Inheritance  | create reusable code by deriving classes from base classes  |
| Polymorphism  | uses interfaces or abstract classes to allow objects to take multiple forms  |
| Abstraction  | simplify complex systems by modeling classes appropriate to the problem domain  |
| **Design Patterns**  |   |
|  Singleton | ensure a class only has one instance  |
| Factory  |  creat objects without specifying which class |
|  Observer | notify multiple objects when a state changes  |
|  **Distributed Systems Basics** |   |
| *Load Balancing*  |  Distrubute traffic accross servers to ensure no single server is overwhelmed.  |
| Caching   |  use in-memory storage to reduce database load |
| Databases   | understand relational (SQL) vs (NO SQL) unrelational databases   |
| **Design Scalable Systems**| |
| URL shortener  | design a system to convert long urls into short ones  |
|chat system   |  Design a real-time messaging system.  |
| scalable key-value store   |   |
| monitoring system, track server-side errors in real time  |   |
|  distrubuted cache |   |
|  rate limiter  |   Implement a system to limit the number of requests a user can make. |
| web crawler    |   |
| service-oriented architectures, map-reduce, distributed caching, load balancing, and others  |   |
| memory management, processes, threads, synchronization, paging, and multithreading few basic distributed computing concepts.  |   |
| how browsers function at a high level, from DNS lookups and TCP/IP, to socket connections.  |   |
## Approach to Low-Level Design
- Clarify Requirements: 
    - Ask questions to understand the scope (e.g., "How many users will the system support?").
    - Define functional and non function requirments 

- Define Core Classes and Relationships:
    -  Identify the main entities and their relationships.
    - Use UML diagrams to visualize the system.

- Write Clean Code: 
    - Focus on modularity, readability, and scalability.
    - Apply design patterns where appropriate. 

- Discuss Trade-offs: 
    - Be prepared to explain why you chose a particular design (e.g., "I used a hash map for O(1) lookups.").

### Common Low-Level Design Problems
- Design a Parking Lot
    - Entities: ParkingLot, ParkingSpot, Vehicle, Ticket.
    - Functionality: Park a vehicle, find available spots, calculate fees.

- Design a Library Management System
    - Entities: User, Librarian, Transaction.
    - Functionality: Add/remove books, issue/return books, serach for books. 

- Design a Chess Game
    - Entities: Board, piece, player, game. 
    - Functionality: Move pieces, check for win/lose conditons. 
  
- Design a URL Shortener (basic version)
    -


