# Singleton Pattern

## Intent
Ensure a class has only one instance and provide a global point of access to it.

## Problem
Sometimes we need to have exactly one instance of a class. For example, we may need a single configuration manager or a single connection to a database. Creating multiple instances in these cases could lead to problems like inconsistent state, excessive resource usage, or incorrect behavior.

## Solution
The Singleton pattern solves this by:
1. Making the constructor private to prevent direct instantiation
2. Creating a static method that returns the same instance every time

## Key Participants
- **Singleton**: The class that implements the singleton pattern, controlling its own instantiation and providing a way to access its single instance.

## Applicability
Use the Singleton pattern when:
- There must be exactly one instance of a class, and it must be accessible from a well-known access point
- The sole instance should be extensible by subclassing, and clients should be able to use an extended instance without modifying their code

## Benefits
- Controlled access to sole instance
- Reduced namespace usage
- Permits refinement of operations and representation
- Permits a variable number of instances (can be extended to allow a controlled number of instances)

## Drawbacks
- Can make unit testing more difficult
- Can hide dependencies between classes
- Violates the single responsibility principle (managing its own creation and lifecycle)
- Requires special treatment in a multithreaded environment

[View Interactive Demo](./index.html)
