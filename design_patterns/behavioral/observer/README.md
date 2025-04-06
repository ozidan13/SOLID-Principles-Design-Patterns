# Observer Pattern

## Intent
Define a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.

## Problem
How to establish relationships between objects where one object needs to notify an unknown number of other objects when its state changes?

## Solution
The Observer pattern suggests defining a subscription mechanism to notify multiple objects about any events that happen to the object they're observing. The subject maintains a list of observers and notifies them automatically of any state changes.

## Key Participants
- **Subject**: Knows its observers and provides an interface for attaching and detaching observers
- **ConcreteSubject**: Stores state of interest to ConcreteObserver objects and sends a notification when its state changes
- **Observer**: Defines an updating interface for objects that should be notified of changes in a subject
- **ConcreteObserver**: Maintains a reference to a ConcreteSubject object, stores state that should stay consistent with the subject's, and implements the Observer updating interface

## Applicability
Use the Observer pattern when:
- An abstraction has two aspects, one dependent on the other
- A change to one object requires changing others, and you don't know how many objects need to be changed
- An object should be able to notify other objects without making assumptions about what those objects are

## Benefits
- Supports loose coupling between the subject and its observers
- Allows sending data to other objects without knowing their exact types
- Enables adding new observers without modifying the subject
- Subjects and observers can exist and evolve independently
- Follows the Open/Closed Principle

[View Interactive Demo](./index.html)
