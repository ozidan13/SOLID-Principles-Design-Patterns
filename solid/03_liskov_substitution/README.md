# Liskov Substitution Principle (LSP)

## Definition
The Liskov Substitution Principle states that objects of a superclass should be replaceable with objects of a subclass without affecting the correctness of the program.

## Problem
When derived classes don't fully support the behavior of their base classes, using them as substitutes can lead to unexpected errors and violations of client expectations.

## Solution
Ensure that subclasses extend the base class without changing its behavior. Derived types must be completely substitutable for their base types.

## Core Idea
If S is a subtype of T, then objects of type T may be replaced with objects of type S without altering any of the desirable properties of the program.

## Benefits
- Ensures proper inheritance hierarchies
- Improves code reusability
- Reduces unexpected behaviors when using polymorphism
- Makes the system more robust
- Helps in creating better abstractions

[View Interactive Demo](./index.html)
