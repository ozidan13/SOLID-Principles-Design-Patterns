# Open-Closed Principle (OCP)

## Definition
The Open-Closed Principle states that software entities (classes, modules, functions, etc.) should be open for extension but closed for modification.

## Problem
When a system needs to change or add new functionality, modifying existing code can introduce bugs and require re-testing the entire system.

## Solution
Design systems so that new functionality can be added by creating new classes, extending existing ones, or implementing interfaces rather than changing existing code.

## Core Idea
Make your code extensible without having to modify the existing codebase. This often involves using abstractions (interfaces, abstract classes) and dependency injection.

## Benefits
- Reduced risk when extending functionality
- Improved maintainability and stability
- Minimizes the need for regression testing
- Promotes the use of interfaces and abstractions
- Enhances code reusability

[View Interactive Demo](./index.html)
