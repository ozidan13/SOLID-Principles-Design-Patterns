# Dependency Inversion Principle (DIP)

## Definition
The Dependency Inversion Principle states that high-level modules should not depend on low-level modules. Both should depend on abstractions. Additionally, abstractions should not depend on details; details should depend on abstractions.

## Problem
When high-level modules depend directly on low-level modules, changes in low-level modules can directly affect high-level modules, requiring modifications to them.

## Solution
Introduce abstractions that decouple high-level components from low-level components, allowing them to communicate without being directly dependent on each other.

## Core Idea
Depend on abstractions, not on concrete implementations. This principle inverts the traditional dependency flow, making high-level modules independent of the implementation details of low-level modules.

## Benefits
- Reduced coupling between modules
- Increased flexibility and reusability
- Easier testing through mocking of dependencies
- Better separation of concerns
- Facilitates development of loosely coupled systems

[View Interactive Demo](./index.html)
