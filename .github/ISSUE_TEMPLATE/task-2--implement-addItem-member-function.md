---
name: 'Task 2: Implement `addItem()` Member Function'
about: Task 2 for Students
title: 'Task 2: Implement `addItem()` Member Function'
labels: enhancement
assignees: ''

---

**Description**

The second task is to give an initial implementation of the `addItem()` class member function.  This function is a `void` function, it does not return an explicit result.  It does change the `Set` implicitly by adding the indicated item into the set.  Thus this function is not a `const` member function like the previous functions since it modifies the `Set`.  This function takes an `int` parameter as input, which is the integer item to be added to the set.

In addition, when adding the implementation of `addItem()` you are also required to fix the stubs implementation to actually work in this task.  You do this by correctly implementing `addItem()` so that you have the information you need to return and implement the first 4 stub information methods.

**Suggested Solution**

The `Set` contains an member array named `setItem[]`.  You need to implement `addItem()` by appending the new item to the end of this array, and incrementing the `setSize` member variable.

**Additional Requirements**

- You are required to use an `ostringstream` when implementing the `str()` member method to construct a string of the set items.
- You are required to use the given `setItem[]` member array and `setSize` member variables as declared to implement saving the items of the set.
