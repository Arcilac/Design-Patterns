# Design-Patterns

## Creation Patterns

### 1. Singleton
Ensures a class has only one instance and provides a global access point to that instance, useful for managing shared resources (like configurations or database connections).

### 2. Prototype
Allows for creating new objects by copying an existing object (prototype) instead of instantiating a new class. This helps avoid the overhead of creating complex instances.

### 3. Factory Method
Defines an interface for creating an object but allows subclasses to decide which class to instantiate. This facilitates object creation without tightly coupling code to concrete classes.

### 4. Abstract Factory
Provides an interface for creating families of related objects without specifying their concrete classes, ideal for managing different variants of a product set.

### 5. Builder
Separates the construction of a complex object from its representation, allowing the same construction process to create different representations of the same type of object.

## Structural Patterns

### 1. Adapter
Allows incompatible interfaces to work together by converting the interface of one class into another that the client expects, facilitating system integration.

### 2. Bridge
Separates an abstraction from its implementation so that both can vary independently, helping to avoid rigidity in code.

### 3. Composite
Allows treating individual objects and compositions of objects uniformly, making it easier to create hierarchical structures (like trees).

### 4. Decorator
Dynamically adds additional responsibilities to an object, providing a flexible way to extend functionality without using inheritance.

### 5. Facade
Provides a simplified interface to a set of interfaces in a subsystem, making the subsystem easier to use and hiding its complexity.

### 6. Flyweight
Uses sharing to support a large number of similar objects efficiently, reducing memory usage by reusing shared instances.

### 7. Proxy
Provides a surrogate or placeholder for another object, controlling access and allowing for additional functionalities like lazy loading or access control.

## Behavioral Patterns

### 1. Chain of Responsibility
Allows a request to pass along a chain of handlers, avoiding coupling the sender of a request to its receiver.

### 2. Command
Encapsulates a request as an object, allowing parameterization of clients with different requests, queuing, and supporting undoable operations.

### 3. Iterator
Provides a way to access elements of an aggregate object sequentially without exposing its underlying representation, making it easier to navigate collections.

### 4. Mediator
Defines an object that encapsulates how a set of objects interact, promoting loose coupling by preventing objects from referring to each other explicitly.

### 5. Memento
Captures and externalizes the internal state of an object without violating encapsulation, allowing the object to be restored to this state later.

### 6. Observer
Defines a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.

### 7. State
Allows an object to alter its behavior when its internal state changes, making it appear as if the object has changed its class.

### 8. Strategy
Defines a family of algorithms, encapsulates each one, and makes them interchangeable, allowing the algorithm to vary independently from the clients that use it.

### 9. Template Method
Defines the skeleton of an algorithm in an operation, deferring some steps to subclasses, allowing subclasses to redefine certain steps without changing the structure of the algorithm.

### 10. Visitor
Represents an operation to be performed on the elements of an object structure, allowing new operations to be defined without changing the classes of the elements on which it operates.

## React-Specific Patterns

### 1. Container/Presentational Pattern
Separates business logic (in container components) from presentation logic (in presentational components), improving clarity and reusability.

### 2. Higher-Order Components (HOC)
Functions that take a component and return a new component with added functionality, facilitating logic reuse.

### 3. Render Props
A technique for sharing code between React components using a prop whose value is a function, providing flexibility in rendering.

### 4. Hooks
Allow developers to use state and other React features without writing a class, simplifying state management in functional components.

### 5. Provider Pattern
Enables a component to make data available to all its child components without passing props explicitly, simplifying global state management.

### 6. Compound Pattern
Combines multiple components to create a more complex and functional user interface, promoting a closely related component relationship.

## Optimization and Performance Patterns

### 1. Memoization
An optimization technique that caches the results of costly operations to avoid repeated calculations, improving efficiency.

### 2. Lazy Loading
Delays the loading or initialization of an object until it is needed, enhancing initial load times.

### 3. Dynamic Import
Dynamically imports modules or components when required, helping to optimize application performance.

### 4. Import on Visibility
Loads resources when they enter the viewport of the browser, optimizing resource usage.

### 5. Import on Interaction
Loads resources when the user interacts with certain elements, enhancing user experience.

### 6. Route-Based Splitting
Splits the code based on the application's routes, loading only what's necessary for the current route.

### 7. Bundle Splitting
Divides the code into smaller bundles to optimize loading and improve response times.

### 8. Tree Shaking
Removes unused code from the final bundle, reducing size and improving load times.

### 9. Preload
Tells the browser to load important resources in advance, speeding up loading times.

### 10. Prefetch
Suggests to the browser to load resources that may be needed in the future, optimizing user experience.

### 11. List Virtualization
Renders only the visible elements in a long list, improving performance and efficiency by reducing the number of elements in the DOM.

## Server-Side and Static Rendering Patterns

### 1. Client-Side Rendering (CSR)
Renders the application in the client's browser using JavaScript, allowing for rich interactivity but potentially longer load times.

### 2. Server-Side Rendering (SSR)
Renders the application on the server and sends the complete HTML to the client, improving initial load times and SEO.

### 3. Static Rendering
Generates HTML pages at build time for faster performance since pre-rendered content is served.

### 4. Incremental Static Generation (ISG)
Combines static generation with on-demand regeneration for dynamic content without sacrificing performance.

### 5. Progressive Hydration
Hydrates components progressively, improving time to interactivity by prioritizing critical elements.

### 6. Streaming Server-Side Rendering
Sends parts of the page to the client as they are rendered on the server, enhancing user experience by displaying content faster.

### 7. React Server Components
Allows components to execute and render on the server to optimize performance and resource loading.

### 8. Selective Hydration
Hydrates only the most important or interactive components first, prioritizing user experience.

### 9. Islands Architecture
Renders most content statically, with "islands" of interactivity that enhance load and response times.

## Other Patterns

### 1. Module Pattern
Encapsulates related functionalities in a single object or module, providing privacy and organization of code, improving modularity.

### 2. Mixin Pattern
Allows adding functionality to a class without using inheritance, combining methods from different objects and facilitating code reuse.

### 3. PRPL Pattern
Focuses on:
- **Push critical resources:** Load critical resources first.
- **Render initial route:** Quickly render the initial route.
- **Pre-cache remaining routes:** Pre-load remaining routes to improve navigation.
- **Lazy-load remaining routes and resources:** Load remaining routes and resources on demand, optimizing loading.
