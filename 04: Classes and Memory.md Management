# Reading 04: Classes and Memory Management

## Microsoft Docs: Classes

### Reference Types
- A type defined as a class is a reference type
  - Variable only holds a reference to created objects
- On creation, enough memory is allocated for the object on the heap
- Garbage collection uses some overhead

### Declaring Classes
- `class` keyword
- Fields, properties, methods, and events on a class are collectively called class members

### Creating objects
- `new` keyword
- variables use references

### Class inheritance
- Classes can inherit members from other classes
- public class Manager : Employee will cause the Manager class to inherit members from the employee class

## Microsoft Docs: Constructors
- Used to create objects

### Parameterless constructors
- Default constructor is created automatically, with no paramters

### Constructor syntax
- Is the same as the name of its type. 
- Is a method
- Can use expression body definition if just one line

### Static constructors
- A class can also have a static constructor

## Microsoft Docs: Properties
- Like a variable, but attached to an object
- Actually special methods called accessors

### Properties overview
- Way to get and set values
- Get property accessor returns property value
- Set property accessor assigns new value
- Can control read/write access of properties

### Properties with backing fields
- Properties have a private backing store

## Heaping Vs Stacking in .NET
- We don't have to actively worry about memory management and garbage collection in .NET, but we still need to keep them in mind.

### Stack vs Heap, what's the difference?
- Stack is responsible for what's executing in our code/been called
- Heap is responsible for keeping track of our objects (most of our data).

#### What goes on the stack and heap?
- Value types
- Reference types
- Pointers
- Reference types always go on the heap
- Values and pointers always go where declared

## Microsoft Docs: Fundamentals of Garbage Collection
