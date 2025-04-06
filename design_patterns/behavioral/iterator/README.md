# Iterator Pattern

## Intent
Provide a way to access the elements of an aggregate object sequentially without exposing its underlying representation.

## Problem
How to access the elements of a collection without exposing its internal structure, and how to provide a standard way to traverse different collection types?

## Solution
The Iterator pattern suggests extracting the traversal behavior of a collection into a separate object called an iterator. This iterator provides a standard way to traverse a collection without exposing its internal structure.

## Key Participants
- **Iterator**: Defines an interface for accessing and traversing elements
- **ConcreteIterator**: Implements the Iterator interface and keeps track of the current position in the traversal
- **Aggregate**: Defines an interface for creating an Iterator object
- **ConcreteAggregate**: Implements the Iterator creation interface to return an instance of the proper ConcreteIterator

## Applicability
Use the Iterator pattern when:
- You want to access a collection's contents without exposing its internal representation
- You want to support multiple traversals of a collection
- You want to provide a uniform interface for traversing different collection types

## Benefits
- Simplifies the interface of the collection
- Supports variations in the traversal of a collection
- Provides a uniform way to access different collections
- Each iterator maintains its own traversal state
- Allows parallel traversal of the same collection

[View Interactive Demo](./index.html)
