# Chain of Responsibility Pattern

## Intent
Avoid coupling the sender of a request to its receiver by giving more than one object a chance to handle the request. Chain the receiving objects and pass the request along the chain until an object handles it.

## Problem
How to decouple senders and receivers of a request based on type or attributes, and how to pass requests between multiple objects without explicitly specifying the processing object?

## Solution
The Chain of Responsibility pattern suggests organizing handlers into a chain where each handler has a reference to the next handler in the chain. Upon receiving a request, each handler decides either to process the request or to pass it to the next handler in the chain.

## Key Participants
- **Handler**: Defines an interface for handling requests and optionally implementing the successor link
- **ConcreteHandler**: Handles requests it is responsible for and can access its successor
- **Client**: Initiates the request to a ConcreteHandler object on the chain

## Applicability
Use the Chain of Responsibility pattern when:
- More than one object may handle a request, and the handler isn't known a priori
- You want to issue a request to one of several objects without specifying the receiver explicitly
- The set of objects that can handle a request should be specified dynamically

## Benefits
- Reduces coupling between sender and receivers
- Adds flexibility in assigning responsibilities to objects
- Allows multiple objects to handle the request
- Allows dynamic modification of the chain at runtime
- Follows the Single Responsibility Principle and Open/Closed Principle

[View Interactive Demo](./index.html)
