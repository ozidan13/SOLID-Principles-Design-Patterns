# Command Pattern

## Intent
Encapsulate a request as an object, thereby allowing for parameterization of clients with different requests, queuing of requests, and logging of operations.

## Problem
How to decouple an object that invokes an operation from the one that knows how to perform it?

## Solution
The Command pattern suggests creating an intermediate object that encapsulates a request. This Command object can perform an action or trigger an event, and it can be passed to other components like any other object.

## Key Participants
- **Command**: Declares an interface for executing an operation
- **ConcreteCommand**: Defines a binding between a Receiver object and an action
- **Client**: Creates a ConcreteCommand object and sets its receiver
- **Invoker**: Asks the command to carry out the request
- **Receiver**: Knows how to perform the operations

## Applicability
Use the Command pattern when you want to:
- Parameterize objects with operations
- Queue operations, schedule their execution, or execute them remotely
- Support undoable operations
- Structure a system around high-level operations built on primitive operations
- Create a command history (for undo/redo)

## Benefits
- Decouples the object that invokes the operation from the one that performs it
- Commands are first-class objects that can be manipulated and extended
- Commands can be assembled into composite commands
- New commands can be added without changing existing code
- Supports logging, undoing, and transactional behavior

[View Interactive Demo](./index.html)
