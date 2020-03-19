# Reading 02: Unit Tests and Documentation

## Unit Testing Best Practices:
- 20 years ago, no one wrote tests for their own code. Now they do.
- First, what unit tests are not:
  - Storing data in a db, reads from disk
    - Unit tests don't deal with their environment
  - Don't count as other sorts of tests
    - Throwing thousands of requests is a smoke test, not a unit test
  - Don't exercise multiple components of system
- What Unit Testing Is
  - They isolate specific units of your code
    - In C#, unit is basically a method
- Unit Testing Tutorial
  - Ex: calculator
- Unit Testing Best Practices
  - 1. Arrange, Act, Assert
    - First, arrange everything we need to run the experiment
    - Second, we act, invoking the method and capturing the result
    - Finally, we assert the hypothesis
  - 2. One assert per method
  - 3. Avoid Test Interdependence
  - 4. Keep it Short, Sweet, and Visible
    - Do not abstract away any steps of the process to separate classes
    - Keep the logic together
  - 5. Recognize Test Setup Pain as a Smell
    - If your test is painful to arrange, that is a hint that your code is not modular enough
    - A heavy setup test is a brittle test
  - 6. Add them to the Build
    - Add the execution of your tests to the build, so that if a test fails, the build fails
    
## xUnit Documentation:

## Art of Readme

## ReadMe Best Practices

  
