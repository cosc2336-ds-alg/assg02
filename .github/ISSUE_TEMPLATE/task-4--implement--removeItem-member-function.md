---
name: 'Task 4: Implement `removeItem()` Member Function'
about: Task 4 for Students
title: 'Task 4: Implement `removeItem()` Member Function'
labels: enhancement
assignees: ''

---

**Description**

Implement the `removeItem()` member function to allow removal of existing items from the set.  As with `addItem()`, `removeItem()` should simply silently ignore a request to remove an item that is not already in the set.  You are required to reuse `containsItem()` to do this check again in your implementation of `removeItem()`.  Otherwise when removing an item, you need to maintain the array of items in your `Set` class so that it has no holes or missing values in the array.  This means you will be required to find the item to be removed, then to shift any items down 1 position in order to remove the requested item from the set.

**Suggested Solution**

Use `containsItem()` to first check if a request is being made to remove an item that is not actually currently in the set.

If the item is in the set, first search until you find the item position.  Then once you have the item position, you need to shift all items in indexes above this position down by 1 location.  You can not use swapping or other methods, you must shift items beyond the item to be removed down 1 position in order to pass the tests given for this task.  Be careful you correctly handle edge cases, when for example the item to be removed is at index 0, or the item is the last item in the `setItem` array.

Make sure you also update the `setSize` member variable after successfully removing an item.

**Additional Requirements**

- You are required to reuse `containsItem()` to check and silently ignore requests to remove items that are not currently in the set.
- You are required to shift down items to fill in holes left by the removal of items.

