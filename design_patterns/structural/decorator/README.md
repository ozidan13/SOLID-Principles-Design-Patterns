# Decorator Pattern

## Intent
Attach additional responsibilities to an object dynamically. Decorators provide a flexible alternative to subclassing for extending functionality.

## Problem
How to add functionality to individual objects without affecting other objects of the same class?

## Solution
The Decorator pattern suggests creating a set of decorator classes that wrap objects. These decorator classes implement the same interface as the original object and transparently add the desired behavior before/after delegating to the original object.

## Key Participants
- **Component**: Defines the interface for objects that can have responsibilities added to them dynamically
- **ConcreteComponent**: Defines an object to which additional responsibilities can be attached
- **Decorator**: Maintains a reference to a Component object and defines an interface that conforms to Component's interface
- **ConcreteDecorator**: Adds responsibilities to the component

## Applicability
Use the Decorator pattern when:
- You need to add responsibilities to individual objects dynamically and transparently
- You want to add responsibilities to objects without affecting other objects
- Extension by subclassing is impractical
- You want to keep new functionality separate from existing classes

## Benefits
- Provides greater flexibility than static inheritance
- Avoids feature-laden classes at the top of the hierarchy
- Enhances objects at runtime
- Enables combining multiple behaviors through layering
- Follows the Single Responsibility Principle

[View Interactive Demo](./index.html)
