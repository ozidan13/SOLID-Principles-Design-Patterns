# Adapter Pattern

## Intent
Convert the interface of a class into another interface clients expect. Adapter lets classes work together that couldn't otherwise because of incompatible interfaces.

## Problem
How can a class be reused that doesn't have an interface that a client requires?

## Solution
The Adapter pattern suggests defining a wrapper class that converts the incompatible interface of a class into an interface that clients require.

## Key Participants
- **Target**: Defines the domain-specific interface that Client uses
- **Adapter**: Adapts the interface of Adaptee to the Target interface
- **Adaptee**: Defines an existing interface that needs adapting
- **Client**: Collaborates with objects conforming to the Target interface

## Applicability
Use the Adapter pattern when:
- You want to use an existing class, but its interface does not match the one you need
- You want to create a reusable class that cooperates with unrelated or unforeseen classes
- You need to use several existing subclasses, but it's impractical to adapt their interface by subclassing every one

## Benefits
- Allows classes with incompatible interfaces to work together
- Increases reusability of existing code
- Introduces only one object, no changes to existing code
- Lets you add functionality to objects without changing the original code

[View Interactive Demo](./index.html)
