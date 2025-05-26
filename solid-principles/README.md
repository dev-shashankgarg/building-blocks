
# SOLID Principles Practice Sheet (Java)

A hands-on guide to mastering SOLID principles through implementation exercises in Java.

---

## 1. Single Responsibility Principle (SRP)
**Definition:** A class should have only one reason to change.

### Theory Focus
- Understand cohesion.
- Identify responsibilities in real-world entities.

### Practice Tasks
- **Basic:** Create a `Book` class with `title`, `author`, and content. Separate out `BookPrinter` or `BookRepository`.
- **Intermediate:** Design a `Report` system that separates data generation, formatting, and exporting.
- **Advanced:** Build a logger with split responsibilities: `LogFormatter`, `LogWriter`, `LogStorage`.

---

## 2. Open/Closed Principle (OCP)
**Definition:** Software entities should be open for extension but closed for modification.

### Theory Focus
- Use interfaces and abstract classes.
- Favor composition over inheritance.

### Practice Tasks
- **Basic:** Create a `Shape` interface with `area()` method. Extend it without modifying existing logic.
- **Intermediate:** Implement a payment system where new payment methods can be added.
- **Advanced:** Design a plugin-based notification system (Email, SMS, Slack).

---

## 3. Liskov Substitution Principle (LSP)
**Definition:** Subtypes must be substitutable for their base types.

### Theory Focus
- Understand behavioral subtyping.
- Avoid breaking the base class contract.

### Practice Tasks
- **Basic:** Create a `Bird` class and a `FlyingBird` interface. Handle `Penguin` edge case.
- **Intermediate:** Build a `MediaPlayer` and create `AudioPlayer`, `VideoPlayer`.
- **Advanced:** Model a `Transportation` system with `Vehicle`, `Car`, `ElectricCar`, `Bike`.

---

## 4. Interface Segregation Principle (ISP)
**Definition:** No client should be forced to depend on methods it does not use.

### Theory Focus
- Split fat interfaces.
- Favor client-specific interfaces.

### Practice Tasks
- **Basic:** Start with a `Worker` interface and split into `Workable`, `Feedable`.
- **Intermediate:** Model smart appliances with `Controllable`, `Monitorable`, `Schedulable`.
- **Advanced:** Design modular robot controls: `Moveable`, `Rechargeable`, `Scannable`.

---

## 5. Dependency Inversion Principle (DIP)
**Definition:** High-level modules should not depend on low-level modules. Both should depend on abstractions.

### Theory Focus
- Use interfaces for dependency injection.
- Explore constructor/setter injection.

### Practice Tasks
- **Basic:** Design a `LightBulb` system with a `Switch` interface.
- **Intermediate:** Implement a messaging app using `MessageSender` interface (Email/SMS).
- **Advanced:** Build an E-commerce checkout flow with `PaymentProcessor`, `Notifier`, `InventoryUpdater`.

---

## Extra Challenges

### Mini Project
- Design a modular **Library Management System** or **Food Delivery App** applying all SOLID principles.

### Peer Review
- Refactor an existing Java project using SOLID.

### TDD Integration
- Combine SOLID with JUnit to structure your code using test-driven development.

---

## Practice Tips
1. Create separate repos or folders per principle.
2. Start from a monolith, refactor using the principle.
3. Document changes and their design benefits.
4. Optional: Use Spring for real-world practice (DIP, ISP).
