---
name: 'Task 5: Implement `operatorUnion()` Member Function'
about: Task 5 for Students
title: 'Task 5: Implement `operatorUnion()` Member Function'
labels: enhancement
assignees: ''

---

**Description**

Implement the described `operatorUnion()` member function.  The union of two sets is a set containing all items in either (or both) sets.

This function takes another `Set` as an input parameter and modifies this `Set` to become the union between this set and the other set given as a parameter to this function.


**Suggested Solution**

You are required to reuse the `Set` member function in implementing your union operation.  The suggested solution is to iterate over all of the items in the other set given as input, and call `addItem()` for every item in the other set to add each item to this set.  Since `addItem()` should ignore request to add duplciate items, the result will be that any items in the other set not already in this set will be added to this set, thus giving the union between the two sets as the result.

**Additional Requirements**

- You are required to reuse `addItem()` to implement your `operatorUnion()` member method.
- You are required to pass in the other set to this method as a `const` reference parameter.  We normally pass in objects by reference in C++ for performance reasons (the `Set` could contain millions of items).  But we will not be modifying the other set so it should be declared as a `const` parameter).


