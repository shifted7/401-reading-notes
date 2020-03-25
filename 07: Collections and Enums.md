# Reading 07: Collections and Enums

## C# In a Nutshell: Chapter 7 (pg 301-313,324-327)
- .NET Framework includes some types for handling collections of objects: resizable lists, linked lists, sorted and unsorted dictionaries, and arrays.
  - Only arrays are actually part of C#
    - The others are just classes

### Enumerations
- Computing has many different types of collections
- Universally needed is the ability to traverse the contents of the collection
- We have a pair of interfaces that provide this, and can be used on all these data structures
  - IEnumerator and IEnumerable
  - Usually the data structures do not implement the Enumerators, but just provide them, which allows other classes to handle the traversal operations
  - IEnumerable can be thought of as the Enumerator provider
- We can also just use foreach

### IEnumerable<T> and IEnumerator<T>
- Extended generic versions

### LinkedList<T>
- Generic doubly linked list
- Has AddFirst, AddLast, AddAfter, and AddBefore methods
- Has Remove methods as well
- Has property Count that tracks length, First that tracks the first node, and Last that tracks the last node
- Has additional methods Contains, Find, and FindLast

## C# In a Nutshell: Chapter 7 (pg 324-327)

## Microsoft docs: Collections
- Two ways to group objects: arrays and collections
- Arrays are good for fixed number of strongly-typed objects
- Collections are more flexible.

## Microsoft docs: Enumeration types
- Set of named constants of an underlying numeric type (int by default)
- Ex: enum Season {Monday = 1, Tuesday = 2, Wednesday =3 etc.}
