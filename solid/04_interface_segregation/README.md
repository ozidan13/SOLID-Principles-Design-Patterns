# Interface Segregation Principle (ISP)

## Definition
The Interface Segregation Principle states that clients should not be forced to depend on interfaces they do not use. This principle promotes creating small, specific interfaces rather than large, monolithic ones.

## Problem
Large interfaces create unnecessary coupling between clients and implementations. When a class implements an interface with methods it doesn't need, it becomes bloated and harder to maintain.

## Solution
Split large interfaces into smaller, more specific ones so that clients only need to know about the methods that are of interest to them.

## Core Idea
Many client-specific interfaces are better than one general-purpose interface. Design fine-grained interfaces that are client-specific.

## Benefits
- Reduces the impact of changes
- Improves readability and maintainability
- Promotes decoupling
- Eliminates unused dependencies
- Makes implementations more focused and cohesive

[View Interactive Demo](./index.html)
