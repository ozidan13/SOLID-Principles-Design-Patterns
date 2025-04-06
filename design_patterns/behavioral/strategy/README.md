# Strategy Pattern

## Intent
Define a family of algorithms, encapsulate each one, and make them interchangeable. Strategy lets the algorithm vary independently from clients that use it.

## Problem
How to define a class that will have one behavior that is similar to other behaviors in a list but vary in some way?

## Solution
The Strategy pattern suggests defining a family of algorithms, putting each of them into a separate class, and making their objects interchangeable. The original object, called context, holds a reference to a strategy object and delegates it the work. The Context isn't responsible for selecting an appropriate algorithm — instead, the client passes the desired strategy to the context.

## Key Participants
- **Strategy**: Declares an interface common to all supported algorithms
- **ConcreteStrategy**: Implements the algorithm using the Strategy interface
- **Context**: Is configured with a ConcreteStrategy object and maintains a reference to a Strategy object

## Applicability
Use the Strategy pattern when:
- Many related classes differ only in their behavior
- You need different variants of an algorithm
- An algorithm uses data that clients shouldn't know about
- A class defines many behaviors, and these appear as multiple conditional statements in its operations

## Benefits
- Provides an alternative to subclassing for varying behavior
- Eliminates conditional statements
- Encapsulates the algorithm implementation details
- Allows algorithm to vary independently from the clients that use it
- Enables runtime switching between algorithms

[View Interactive Demo](./index.html)
