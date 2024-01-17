---
name: 'Task 1: Add Initial Stub Functions'
about: Task 1 for Students
title: 'Task 1: Add Initial Stub Functions'
labels: enhancement, good first issue
assignees: ''

---

**Description**

The first task is to add stub implementations of all of the following information member functions:

- `isEmpty()`
  - Returns a `bool` result.  No parameters given as input.
- `getSetSize()`
  - Returns an `int` result, the current number of items in the set.  No parameters are supplied as input to this member function.
- `containsItem()`
  - Returns a `bool` result of `true` if the asked for item is currently in the set, or `false` if the item is not in the set.  This function takes an `int` parameter as input which is the item to check if in the set or not.
- `str()`
  - Returns a `string` type.  Ultimately this function constructs a string showing all of the values currently contained in the set.  Initial for the stub function simply return the literal string "[ ]" (notice the space between the square brackets which is required).

All stub functions simply return a hard coded value for task 1.  All of these functions return information about the `Set` class, they do not change the data in the class.  Thus all of these member functions need to be declared as `const` member functions.  These stub functions should pass the first four test cases given for this assignment.

**Suggested Solution**

This is a warm up task.  You should be able to declare the functions and provide a stub/default implementation that passes the first 4 given test cases relatively simply once you understand how to add new function declarations and implementations into the `Set` class.

**Additional Requirements**

- All of these function are required to be `const` member functions.
