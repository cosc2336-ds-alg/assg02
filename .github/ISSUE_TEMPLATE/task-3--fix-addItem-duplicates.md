---
name: 'Task 3: Fix `addItem()` to Handle Duplicate Items'
about: Task 3 for Students
title: 'Task 3: Fix `addItem()` to Handle Duplicate Items'
labels: enhancement
assignees: ''

---

**Description**

The `Set` data type should not contain duplicate items.  If `addItem()` is asked to add an item that is already in the set, the request should be silently ignored.  This task is to fix the implementation of `addItem()` to correctly ignore requests to add duplicate items in order to maintain a unique set of items.

**Suggested Solution**

You need to be reusing the `containsItem()` member function to determine if new requested additional item is a duplicate or not.

**Additional Requirements**

- You are required to reuse `containsItem()` in your handling of duplicates in `addItem()`

