# Composite Pattern

## Intent
Compose objects into tree structures to represent part-whole hierarchies. Composite lets clients treat individual objects and compositions of objects uniformly.

## Problem
How to represent part-whole hierarchies of objects, where clients should be able to treat individual objects and compositions of objects uniformly?

## Solution
The Composite pattern suggests that you work with Products and Boxes through a common interface which declares methods for calculating the total price, rendering elements, etc.

## Key Participants
- **Component**: Declares the interface for objects in the composition and implements default behavior
- **Leaf**: Represents leaf objects in the composition (has no children)
- **Composite**: Defines behavior for components having children and stores child components
- **Client**: Manipulates objects in the composition through the Component interface

## Applicability
Use the Composite pattern when:
- You want to represent part-whole hierarchies of objects
- You want clients to be able to ignore the difference between compositions of objects and individual objects
- The structure can have any level of complexity
- Operations on objects and compositions need to be handled uniformly

## Benefits
- Defines class hierarchies containing primitive and complex objects
- Makes it easier to add new types of components
- Provides flexibility of structure with a manageable interface
- Makes client code simple by treating objects and compositions uniformly

[View Interactive Demo](./index.html)
