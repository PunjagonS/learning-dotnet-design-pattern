# Design Patterns in C#

This document provides an overview of the 23 standard GoF Design Patterns, categorized into three main groups.

---

## Summary:

- **Creational Patterns**: Focus on creating objects in a flexible and controlled manner.
- **Structural Patterns**: Focus on managing object compositions to form suitable structures.
- **Behavioral Patterns**: Focus on communication and responsibility sharing among objects.

---

## 1. Creational Patterns (Object Creation)

### 1.1 Abstract Factory (Used Occasionally)
> Creates families of related objects without specifying their concrete classes.

**Remark:** Useful in systems where a family of objects (e.g., GUI components for Windows vs Mac) must be interchangeable. However, dependency injection frameworks often reduce its usage.

### 1.2 Builder (Used Frequently)
> Separates the construction of a complex object from its representation, enabling step-by-step construction.

**Remark:** Highly useful when creating objects with many optional parameters, such as JSON payloads or configuration settings.

### 1.3 Factory Method (Used Frequently)
> Defines an interface for creating objects, letting subclasses decide which class to instantiate.

**Remark:** Common in frameworks and libraries for creating objects dynamically based on context or input.

### 1.4 Prototype (Rarely Used)
> Creates new objects by cloning existing instances.

**Remark:** Modern languages provide built-in cloning features, reducing the need for this pattern.

### 1.5 Singleton (Used Frequently)
> Ensures a class has only one instance and provides a global point of access to it.

**Remark:** Popular for managing shared resources like logging or database connections, but overuse can lead to tight coupling and testability issues.

---

## 2. Structural Patterns (Object Composition)

### 2.1 Adapter (Used Frequently)
> Converts the interface of one class into another interface that clients expect.

**Remark:** Essential for integrating legacy systems or incompatible APIs in modern systems.

### 2.2 Bridge (Used Occasionally)
> Separates abstraction from its implementation so that the two can vary independently.

**Remark:** Useful for applications requiring flexibility in combining abstractions and implementations, such as UI frameworks.

### 2.3 Composite (Used Occasionally)
> Treats individual objects and compositions of objects uniformly in a tree structure.

**Remark:** Ideal for hierarchical structures like menus, file systems, or organizational charts.

### 2.4 Decorator (Used Frequently)
> Dynamically adds behavior to objects without modifying their code.

**Remark:** Commonly used in middleware, logging, or extending functionality in a modular way.

### 2.5 Facade (Used Frequently)
> Provides a simplified interface to a complex subsystem.

**Remark:** Useful for creating APIs or gateways that hide internal complexities from users.

### 2.6 Flyweight (Rarely Used)
> Shares objects to minimize memory usage for a large number of similar objects.

**Remark:** Relevant for resource-intensive applications like game development or rendering systems with repeated elements.

### 2.7 Proxy (Used Frequently)
> Provides a surrogate or placeholder for another object to control access or add functionality.

**Remark:** Useful in scenarios like lazy loading, caching, or securing access to a resource.

---

## 3. Behavioral Patterns (Object Communication)

### 3.1 Chain of Responsibility (Rarely Used)
> Passes a request along a chain of handlers, allowing each to decide whether to handle it or pass it on.

**Remark:** Middleware frameworks like Express.js or ASP.NET pipelines often replace this pattern.

### 3.2 Command (Rarely Used)
> Encapsulates a request as an object, allowing parameterization and queuing of requests.

**Remark:** Often replaced by event-driven systems or message queues, but still useful in GUI systems for undo/redo functionality.

### 3.3 Interpreter (Rarely Used)
> Defines a grammar for a language and interprets its sentences.

**Remark:** Typically replaced by modern parsers or libraries for handling expressions and commands.

### 3.4 Iterator (Used Frequently)
> Provides a way to access elements of a collection sequentially without exposing its underlying structure.

**Remark:** Foundational in modern programming, used in `foreach` loops or custom collections.

### 3.5 Mediator (Used Occasionally)
> Reduces communication complexity between objects by having a mediator handle their interactions.

**Remark:** Useful in systems with multiple interacting components, such as chat applications or UI components.

### 3.6 Memento (Rarely Used)
> Captures and restores an object's state without violating encapsulation.

**Remark:** Primarily used in undo/redo systems but often replaced by state management or database snapshots.

### 3.7 Observer (Used Frequently)
> Notifies dependent objects when an object’s state changes.

**Remark:** Essential in event-driven architectures and state management systems like Redux or RxJS.

### 3.8 State (Used Frequently)
> Alters an object’s behavior when its state changes.

**Remark:** Useful in workflows or systems with finite state machines, such as ATMs or game entities.

### 3.9 Strategy (Used Frequently)
> Defines a family of algorithms and makes them interchangeable at runtime.

**Remark:** Commonly used for selecting algorithms dynamically, such as sorting or payment processing.

### 3.10 Template Method (Used Occasionally)
> Defines the skeleton of an algorithm, allowing subclasses to define specific steps.

**Remark:** Useful in frameworks where workflows are predefined but customizable, such as report generation.

### 3.11 Visitor (Rarely Used)
> Adds new operations to existing object structures without modifying their classes.

**Remark:** Primarily useful in systems with complex object hierarchies, such as compilers or ASTs.

---

> **Note:**
> This is an overview of GoF Design Patterns in C# to guide the selection of suitable patterns for specific use cases.

