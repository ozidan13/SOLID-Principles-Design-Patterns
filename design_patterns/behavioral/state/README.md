# State Pattern

## Intent
Allow an object to alter its behavior when its internal state changes. The object will appear to change its class.

## Problem
How to allow an object to change its behavior depending on its internal state without using massive conditionals?

## Solution
The State pattern suggests creating new classes for all possible states of an object and extracting all state-specific behaviors into these classes. The original object delegates the work to an instance of the appropriate state class.

## Key Participants
- **Context**: Defines the interface of interest to clients and maintains an instance of a ConcreteState subclass that defines the current state
- **State**: Defines an interface for encapsulating the behavior associated with a particular state of the Context
- **ConcreteState**: Each subclass implements behavior associated with a state of the Context

## Applicability
Use the State pattern when:
- An object's behavior depends on its state, and it must change its behavior at runtime depending on that state
- Operations have large, multipart conditional statements that depend on the object's state
- State transitions are explicit and numerous

## Benefits
- Localizes state-specific behavior and partitions behavior for different states
- Makes state transitions explicit
- State objects can be shared
- Eliminates the need for large conditional statements
- Improves cohesion by separating state-specific behavior from the Context

[View Interactive Demo](./index.html)
