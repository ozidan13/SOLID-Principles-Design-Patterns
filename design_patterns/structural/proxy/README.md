# Proxy Pattern

## Intent
Provide a surrogate or placeholder for another object to control access to it.

## Problem
How to control access to an object? How to provide additional functionality when accessing an object?

## Solution
The Proxy pattern suggests creating a new proxy class with the same interface as an original service object. The proxy object delegates all the real work to the service object but performs additional functionality before or after the service method is called.

## Key Participants
- **Subject**: Interface shared by the RealSubject and the Proxy
- **RealSubject**: The real object that the proxy represents
- **Proxy**: Maintains a reference that lets the proxy access the real subject, implements the same interface as the Subject

## Applicability
Use the Proxy pattern when:
- You need a more versatile or sophisticated reference to an object than a simple pointer
- You want to control access to the original object (Protection Proxy)
- You need to defer the full cost of creating and initializing an object until it's actually used (Virtual Proxy)
- You need additional operations when an object is accessed (Logging Proxy)

## Types of Proxies
- **Virtual Proxy**: Delays the creation of expensive objects until needed
- **Protection Proxy**: Controls access to the original object
- **Remote Proxy**: Represents an object in a different address space
- **Logging Proxy**: Logs method calls to the service object
- **Caching Proxy**: Caches expensive operations results

## Benefits
- Introduces a layer of indirection when accessing an object
- Allows performing operations before or after the request reaches the target object
- Controls the lifecycle of the service object
- Works even when the service object is not ready or available
- Implements deferred initialization and caching

[View Interactive Demo](./index.html)
