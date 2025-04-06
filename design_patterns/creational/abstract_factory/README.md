# Abstract Factory Pattern

## Intent
Provide an interface for creating families of related or dependent objects without specifying their concrete classes.

## Problem
How to create a system that is independent of how its products are created, composed, and represented, especially when families of related products are designed to be used together.

## Solution
The Abstract Factory pattern suggests defining an interface for creating all distinct products but leaves the actual product creation to concrete factory classes. Each factory type corresponds to a certain product variety.

## Key Participants
- **AbstractFactory**: Declares an interface for operations that create abstract product objects
- **ConcreteFactory**: Implements the operations to create concrete product objects
- **AbstractProduct**: Declares an interface for a type of product object
- **ConcreteProduct**: Defines a product object to be created by the corresponding concrete factory
- **Client**: Uses only interfaces declared by AbstractFactory and AbstractProduct classes

## Applicability
Use the Abstract Factory pattern when:
- A system should be independent of how its products are created, composed, and represented
- A system should be configured with one of multiple families of products
- A family of related product objects is designed to be used together
- You want to provide a class library of products, and you want to reveal just their interfaces, not their implementations

## Benefits
- Isolates concrete classes from the client
- Makes exchanging product families easy
- Promotes consistency among products
- Supports the "open/closed principle"

[View Interactive Demo](./index.html)
