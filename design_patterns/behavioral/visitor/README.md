# Visitor Pattern

## Intent
Represent an operation to be performed on elements of an object structure. Visitor lets you define a new operation without changing the classes of the elements on which it operates.

## Problem
How to define operations that can be applied to objects without changing their classes, especially when those operations only make sense for some classes?

## Solution
The Visitor pattern suggests placing the new behavior in a separate class called visitor, instead of integrating it into existing classes. The original object that had to perform the behavior is now passed to one of the visitor's methods as an argument, providing access to all necessary data.

## Key Participants
- **Visitor**: Declares a visit operation for each class of ConcreteElement in the object structure
- **ConcreteVisitor**: Implements each operation declared by Visitor
- **Element**: Defines an accept operation that takes a visitor as an argument
- **ConcreteElement**: Implements the accept operation that takes a visitor as an argument
- **ObjectStructure**: Can enumerate its elements and may provide a high-level interface to allow the visitor to visit its elements

## Applicability
Use the Visitor pattern when:
- An object structure contains many classes of objects with differing interfaces, and you want to perform operations on these objects that depend on their concrete classes
- Many distinct and unrelated operations need to be performed on objects in an object structure, and you want to avoid "polluting" their classes with these operations
- The classes defining the object structure rarely change, but you often want to define new operations over the structure

## Benefits
- Makes adding new operations easy
- Gathers related operations and separates unrelated ones
- Allows operations on complex object structures
- Accumulates state as the visitor traverses the structure
- Separates algorithm from the objects on which it operates

[View Interactive Demo](./index.html)
