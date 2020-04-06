# Reading 15: Dependency Injection
## Microsoft Docs: Dependency Injection in ASP.NET Core
- A dependency is any object that another object requires.
- We don't want to hardcode, because dependencies can change, and have their own dependencies.
- So, we use interfaces to pass objects to other objects, usually in class constructors

## Lecture
- Allows our components to be loosely coupled - fluid, piecse can be mixed/matched.
- Separates our controllers from the functionality -> services
- We use interface type objects
- Improves testability and separation of concerns, but introduces a learning curve.

## 30 Days of TDD: Day Five: Make Your Code SOLID
- Single Responsiblity Principle
  - Every method or class should have exactly one reason to change (only one task)
- Open/Close Principle
  - Objects should be open to extension, but closed to modification.
- Liskov Substitution Principle
  - We should be able to replace one object with another of the same type
- Interface Segregation Principle
  - Clients should not be forced to rely on interfaces they don't use
- Dependency Inversion Principle
  - Make coupling as loose as possible.
