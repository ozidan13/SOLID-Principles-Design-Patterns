# Factory Method Pattern

## Intent
Define an interface for creating an object, but let subclasses decide which class to instantiate. Factory Method lets a class defer instantiation to subclasses.

## Problem
When a class cannot anticipate the type of objects it must create, or when a class wants its subclasses to specify the objects it creates.

## Solution
The Factory Method pattern suggests that you replace direct object construction calls with calls to a special factory method. Objects returned from a factory method are often referred to as "products."

## Key Participants
- **Creator**: The abstract class that declares the factory method
- **ConcreteCreator**: Classes that implement the factory method to produce concrete products
- **Product**: The interface for the type of object the factory creates
- **ConcreteProduct**: The specific implementations of the product interface

## Applicability
Use the Factory Method pattern when:
- A class can't anticipate the class of objects it must create
- A class wants its subclasses to specify the objects it creates
- Classes delegate responsibility to one of several helper subclasses, and you want to localize the knowledge of which helper subclass is the delegate

## Benefits
- Eliminates the need to bind application-specific classes into your code
- Provides hooks for subclasses to extend the factory process
- Connects parallel class hierarchies
- Promotes loose coupling

[View Interactive Demo](./index.html)
