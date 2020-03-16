# Reading 01: Exception Handing and Debugging
## Try/Catch blocks
- Place code that might raise or throw an exception in a try block
- Place code to execute during exception inside a catch block
```using System;
using System.IO;
try
  {
  }
catch (<error name> e)
  {
  }
```

## Exception Handling
- Statement keywords
  - Selection statements: if else switch case
  - Iteration statements: do for foreach in while
  - Jump statements: break continue default goto return yield
  - Exception handling statements: throw try-catch try-finally try-catch-finally
  - Checked and unchecked: checked unchecked
  - fixed statement: fixed
  - lock statement: lock

## C# in a Nutshell - pg 158-166

## Therac-25
- Radiation therapy machine
- Six accidents in 80s resulting in injury and death caused by insufficient handling of exceptions

## Ariane-5
- 1996: Failed launch caused by attempt to convert floating point number to integer

