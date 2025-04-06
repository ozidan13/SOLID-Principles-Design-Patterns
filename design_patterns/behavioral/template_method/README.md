# Template Method Pattern

## Intent
Define the skeleton of an algorithm in an operation, deferring some steps to subclasses. Template Method lets subclasses redefine certain steps of an algorithm without changing the algorithm's structure.

## Problem
How to implement an invariant part of an algorithm once and leave the variable parts to be implemented by client subclasses?

## Solution
The Template Method pattern suggests defining a template method that contains a skeleton of an algorithm with abstract primitive operations that subclasses override to provide concrete behavior. The template method ensures that the overall structure of the algorithm stays intact while subclasses provide specific implementations.

## Key Participants
- **AbstractClass**: Defines abstract primitive operations that concrete subclasses must implement, and implements a template method that uses these operations
- **ConcreteClass**: Implements the primitive operations to carry out subclass-specific steps of the algorithm

## Applicability
Use the Template Method pattern when:
- You want to implement the invariant parts of an algorithm once and let subclasses implement the behavior that can vary
- You want to control the point at which subclassing is allowed
- You want to exercise common behavior among subclasses to avoid code duplication

## Benefits
- Reuses common code in the parent class
- Controls the steps and their order in the algorithm
- Provides hooks for subclasses to extend the algorithm at specific points
- Reduces code duplication
- Follows the Hollywood Principle: "Don't call us, we'll call you"

[View Interactive Demo](./index.html)
