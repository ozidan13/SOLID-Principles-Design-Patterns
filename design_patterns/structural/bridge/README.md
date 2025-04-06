# Bridge Pattern

## Intent
Decouple an abstraction from its implementation so that the two can vary independently.

## Problem
How to avoid a permanent binding between an abstraction and its implementation, especially when the implementation must be selected or switched at run-time?

## Solution
The Bridge pattern suggests splitting a large class or a set of closely related classes into two separate hierarchies—abstraction and implementation—which can be developed independently of each other.

## Key Participants
- **Abstraction**: Defines the abstraction's interface and maintains a reference to an implementation
- **RefinedAbstraction**: Extends the interface defined by Abstraction
- **Implementor**: Defines the interface for implementation classes
- **ConcreteImplementor**: Implements the Implementor interface

## Applicability
Use the Bridge pattern when:
- You want to avoid a permanent binding between an abstraction and its implementation
- Both the abstractions and their implementations should be extensible through subclasses
- Changes in the implementation should have no impact on the client code
- You want to hide implementation details completely from clients

## Benefits
- Decouples interface from implementation
- Improves extensibility
- Hides implementation details from clients
- Enables independent changes to abstractions and implementations

[View Interactive Demo](./index.html)
