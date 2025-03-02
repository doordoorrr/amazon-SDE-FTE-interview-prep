---
tags: [amazon]
title: Design Patterns Review
created: '2025-03-01T23:07:38.145Z'
modified: '2025-03-02T05:43:23.233Z'
---

# Design Patterns Review
**todo:** 
-  here? all of it lol 


1. Structural Pattern
2. Creational Pattern
3. Behavioral Pattern

There are various advantages of using design Patterns:

- The Design Patterns capture software engineering experiences.
- They are reusable and can be used in multiple projects.
- They provide transparency to software design.
- The Design Patterns provide a solution that helps to define the system architecture

## Creational Patterns
- [Singleton Pattern](https://python.plainenglish.io/design-patterns-in-python-singleton-5095a4c14f)

ensures a class only has one instance, and provides a global point of access to that instance

    public class Singleton {
	    private static Singleton instance;
	    private Singleton() {}  // Private constructor
	    
	    public static Singleton getInstance() {
	        if (instance == null) {
	            instance = new Singleton();
	        }
	        return instance;
	    }
    }
  


- Factory method/Template

    
	
- Abstract Factory

- Builder

- Prototype


## Structural Patterns
- Adapter

	    interface ITarget {
		    void Request();
	    }
	    class Adaptee {
		    public void SpecificRequest() {
		        Console.WriteLine(&quot;Adaptee's method called&quot;);
	    }
	    }
	    class Adapter : ITarget {
		    private Adaptee adaptee = new Adaptee();
		    
		    public void Request() {
		        adaptee.SpecificRequest();
         }
        }


- Bridge
- Filter
- Composite
- Decorator
- Facade
- Flyweight
- Proxy

## Behavioural Patterns
- Interpreter
- Template method/ pattern
- Chain of responsibility
- Command pattern
- Iterator pattern
- Strategy pattern
- Visitor pattern
 ### Resources:

**Design Patterns in Python: A Series**
 https://medium.com/@amirm.lavasani/design-patterns-in-python-a-series-f502b7804ae5
