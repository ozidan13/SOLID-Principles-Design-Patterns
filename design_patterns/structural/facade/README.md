# Facade Pattern

## Intent
Provide a unified interface to a set of interfaces in a subsystem. Facade defines a higher-level interface that makes the subsystem easier to use.

## Problem
How to provide a simple interface to a complex subsystem without reducing its flexibility?

## Solution
The Facade pattern suggests creating a facade class with a simple interface that delegates client requests to appropriate objects within the subsystem. The Facade may also perform additional functionality before/after forwarding a request.

## Key Participants
- **Facade**: Provides a unified interface to a set of interfaces in a subsystem
- **Subsystem classes**: Implement subsystem functionality and handle work assigned by the Facade object
- **Client**: Communicates with the subsystem through the Facade

## Applicability
Use the Facade pattern when:
- You want to provide a simple interface to a complex subsystem
- There are many dependencies between clients and the implementation classes
- You want to layer your subsystems
- You need to have a unified entry point to each level of a layered software

## Benefits
- Shields clients from subsystem components
- Promotes weak coupling between the subsystem and its clients
- Reduces compilation dependencies
- Simplifies the use of complex systems
- Provides entry point to a specific layer of a layered software

[View Interactive Demo](./index.html)
