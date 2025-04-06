# Memento Pattern

## Intent
Without violating encapsulation, capture and externalize an object's internal state so that the object can be restored to this state later.

## Problem
How to capture an object's internal state without exposing its implementation details, and how to restore an object to a previous state?

## Solution
The Memento pattern suggests creating a memento object that serves as a snapshot of the originator's state. The originator creates the memento and uses it to restore its previous state. The caretaker is responsible for the memento's safekeeping without examining its contents.

## Key Participants
- **Originator**: Creates a memento containing a snapshot of its current internal state and uses the memento to restore its internal state
- **Memento**: Stores the internal state of the Originator object
- **Caretaker**: Keeps track of the memento but never modifies or examines the contents of a memento

## Applicability
Use the Memento pattern when:
- A snapshot of an object's state must be saved so it can be restored later
- A direct interface to obtaining the state would expose implementation details and break encapsulation
- You need to implement undo/redo functionality

## Benefits
- Preserves encapsulation boundaries
- Simplifies the originator by letting the caretaker maintain the history
- Provides a clean recovery capability
- Enables storing incremental changes to an object's state
- Supports transaction-like behavior and recovery mechanisms

[View Interactive Demo](./index.html)
