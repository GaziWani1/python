# Objects / Data Types


## 🔹 Basic Object / Data Types

In Python, **everything is an object**. Each object belongs to a specific data type.

---

### 1️⃣ Numbers

Used to store numeric values.

**Types include:**

* `int` → whole numbers
* `float` → decimal numbers
* `complex` → complex numbers
* `binary`, `Decimal`, `Fraction`

```python
x = 1234          # integer
y = 2.4           # float
z = 3 + 4j        # complex
b = 0b111         # binary
```

---

### 2️⃣ String

Used to store text data. Strings are **immutable**.

```python
s1 = 'spam'
s2 = "Bob's"
s3 = b'a\x01c'    # bytes
s4 = u'spām'      # unicode
```

➡️ Once created, a string **cannot be changed**.

---

### 3️⃣ List

An **ordered, mutable** collection.

```python
my_list = [1, [2, 'three'], 4, 5]
nums = list(range(10))
```

✔ Can be modified
✔ Can store mixed data types

---

### 4️⃣ Tuple

An **ordered, immutable** collection.

```python
t = (1, 2, 3, 4)
```

✔ Faster than lists
❌ Cannot be modified

---

### 5️⃣ Dictionary (Dict)

Stores data as **key : value** pairs.

```python
food = {
    'food': 'spam',
    'taste': 'yum'
}
```

✔ Keys must be unique
✔ Very fast lookup

---

### 6️⃣ Set

An **unordered** collection of **unique** elements.

```python
s = {'a', 'b', 'c'}
```

✔ No duplicates
✔ Useful for mathematical operations

---

### 7️⃣ File

Used to read/write data from files.

```python
f = open('egg.txt')
f = open(r'C:\\ham.bin', 'wb')
```

➡️ Always close files or use a context manager.

---

### 8️⃣ Boolean

Represents truth values.

```python
x = True
y = False
```

Used heavily in conditions and loops.

---

### 9️⃣ None

Represents **no value**.

```python
x = None
```

Often used as a default placeholder.

---

### 🔟 Functions, Modules & Classes

```python
# Function
def greet():
    print("Hello")

# Class
class Person:
    pass
```

These are also **objects** in Python.

---

## 🚀 Advanced Python Concepts

---

### 🔸 Decorators

Used to **modify functions** without changing their code.

```python
def my_decorator(func):
    def wrapper():
        print("Before function")
        func()
        print("After function")
    return wrapper

@my_decorator
def say_hi():
    print("Hi")
```

---

### 🔸 Generators

Used to generate values **one at a time** using `yield`.

```python
def count_up(n):
    for i in range(n):
        yield i
```

✔ Memory efficient

---

### 🔸 Iterators

Objects that can be iterated using `next()`.

```python
nums = iter([1, 2, 3])
print(next(nums))
```

---

### 🔸 Comprehensions

Short and clean way to create collections.

```python
squares = [x*x for x in range(5)]
```

---

### 🔸 Context Manager

Manages resources automatically.

```python
with open('file.txt') as f:
    data = f.read()
```

✔ Automatically closes the file

---

### 🔸 Metaprogramming

Writing code that **manipulates code**.

```python
class MyClass(type):
    pass
```

Used in frameworks and advanced libraries.

---

## ✅ Summary

* Python is **object-oriented**
* Some objects are **mutable**, some **immutable**
* Advanced concepts make Python **powerful and flexible**

📌 This README is ideal for **interview prep, revision, and learning basics clearly**.

---

Happy Coding! 🚀
