# Mutable vs Immutable in Python

## What does mutable mean?

A **mutable** object is one whose value **can be changed after it is created**.
When you modify it, **the reference (memory address) stays the same**.

**Example:** lists, dictionaries, sets

```python
lst = [1, 2, 3]
print(id(lst))

lst.append(4)
print(id(lst))  # same reference
```

---

## What does immutable mean?

An **immutable** object is one whose value **cannot be changed after creation**.
Any modification **creates a new object with a new reference**.

**Example:** integers, floats, strings, tuples

```python
a = 10
print(id(a))

a = a + 1
print(id(a))  # new reference
```

---

## Why integers are immutable?

Integers are immutable for **performance and safety**.
When you change an integer, Python **creates a new object** instead of modifying the old one.

This avoids unexpected changes when the same value is shared.

---

## Why lists are mutable?

Lists are mutable so we can **add, remove, or update elements efficiently**.
The same list object is updated in memory.

```python
lst = [1, 2]
lst[0] = 99  # allowed
```

---

## Common mutable vs immutable types in Python

### Immutable types

* int
* float
* complex
* bool
* str
* tuple
* frozenset
* bytes

### Mutable types

* list
* dict
* set
* bytearray
* custom class objects (by default)

---

## Quick summary

* **Immutable** → cannot change, new object is created
* **Mutable** → can change, same object is modified

This difference is important for **memory management, performance, and avoiding bugs**.
