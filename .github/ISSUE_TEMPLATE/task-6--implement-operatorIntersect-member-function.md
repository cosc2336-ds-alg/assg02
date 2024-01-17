---
name: 'Task 6: Implement `operatorIntersect()` Member Function'
about: Task 6 for Students
title: 'Task 6: Implement `operatorIntersect()` Member Function'
labels: enhancement
assignees: ''

---

**Description**

Implement the described `operatorIntersect()` member function.  The intersection of two sets is a set containing only items that are in both of the two sets we are calculating the intersection of.

This function takes another `Set` as an input parameter and modifies this `Set` to become the intersection between this set and the other set given as a parameter to this function.


**Suggested Solution**

The algorithm for the intersection is a bit trickier than the union operation.  It is suggested you do the following

1. Iterate **BACKWARDS** through the items in this set (e.g. the `setItem` array)
   - For each item, check if it is in the other set by calling `containsItem()` for the item on the
     other set.
   - If the item is in the other set then you don't have to do anything because that means it is in both this set and the other set, so it should remain in the calculated set intersection.
   - But if `containsItem()` returns `false` then the item is not in both sets, so needs to be removed from the intersection you are calculating.  You should reuse `removeItem()` to remove the item from this set in the case it is not in the intersection.
   
**Additional Requirements**

- You are required to pass in the other set to this method as a `const` reference parameter.  We normally pass in objects by reference in C++ for performance reasons (the `Set` could contain millions of items).  But we will not be modifying the other set so it should be declared as a `const` parameter).
- You are required to reuse `containsItem()` to test if items in one set are in the other set, and thus are in or not in the set intersection.
- You are required to reuse `removeItem()` to remove items from this set that are not in the resulting set intersection.


