# Mediator Pattern

## Intent
Define an object that encapsulates how a set of objects interact. Mediator promotes loose coupling by keeping objects from referring to each other explicitly, and it lets you vary their interaction independently.

## Problem
How to reduce the direct communication between objects, which can lead to complex dependencies making the system difficult to maintain?

## Solution
The Mediator pattern suggests creating a mediator object that acts as a communication hub for a set of components. Instead of objects communicating directly, they communicate via the mediator.

## Key Participants
- **Mediator**: Defines an interface for communicating with Colleague objects
- **ConcreteMediator**: Implements cooperative behavior by coordinating Colleague objects
- **Colleague**: Knows its Mediator and communicates with other Colleagues through its Mediator

## Applicability
Use the Mediator pattern when:
- A set of objects communicate in well-defined but complex ways
- Reusing an object is difficult because it communicates with many other objects
- A behavior that's distributed between several classes should be customizable without a lot of subclassing

## Benefits
- Reduces coupling between components
- Centralizes control logic in one place
- Simplifies object protocols
- Makes it easier to understand how objects interact
- Makes the system more maintainable by localizing the behavior

[View Interactive Demo](./index.html)
