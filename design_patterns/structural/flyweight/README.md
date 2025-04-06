# Flyweight Pattern

## Intent
Use sharing to support large numbers of fine-grained objects efficiently.

## Problem
How to support large numbers of objects that have part of their internal state in common where storing it externally would reduce overall memory usage?

## Solution
The Flyweight pattern suggests separating the intrinsic state (shared across many objects) from the extrinsic state (varies per object). The intrinsic state is stored in shared flyweight objects, while the extrinsic state is stored or computed by client objects.

## Key Participants
- **Flyweight**: Declares an interface through which flyweights can receive and act on extrinsic state
- **ConcreteFlyweight**: Implements the Flyweight interface and stores intrinsic state
- **FlyweightFactory**: Creates and manages flyweight objects and ensures flyweights are shared properly
- **Client**: Maintains references to flyweights and computes or stores extrinsic state of flyweights

## Applicability
Use the Flyweight pattern when:
- An application uses a large number of objects
- Storage costs are high because of the sheer quantity of objects
- Most object state can be made extrinsic (stored outside the object)
- Many groups of objects may be replaced by relatively few shared objects

## Benefits
- Reduces memory usage by sharing common parts of the state
- Improves performance in scenarios with many similar objects
- Makes code more maintainable by centralizing common state
- Can dramatically reduce the number of physically created objects

[View Interactive Demo](./index.html)
