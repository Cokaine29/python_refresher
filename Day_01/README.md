## 🔹 **PART 1: VARIABLES & DATA TYPES**

### 🔸 What is a Variable?

A **variable** is a name that refers to a value stored in memory.

```python
x = 10      # x is a variable storing an integer
name = "Niraj"  # name stores a string
```

👉 In Python, you **don’t declare** the type explicitly — Python is **dynamically typed**.

### 🔸 Data Types

| Type    | Example         | Description                       |
| ------- | --------------- | --------------------------------- |
| `int`   | `10`, `-5`      | Whole numbers                     |
| `float` | `3.14`, `-2.5`  | Decimal numbers                   |
| `str`   | `"hello"`       | Text / string                     |
| `bool`  | `True`, `False` | Boolean (logic-based)             |
| `list`  | `[1, 2, 3]`     | Ordered, mutable collection       |
| `tuple` | `(1, 2, 3)`     | Ordered, **immutable** collection |
| `dict`  | `{"a": 1}`      | Key-value pairs                   |
| `set`   | `{1, 2, 3}`     | Unordered, unique values          |

```python
age = 25
pi = 3.14
message = "Hello World"
is_student = True
marks = [85, 90, 92]
person = {"name": "Niraj", "age": 25}
unique_ids = {1, 2, 3}
```

### 🔸 Type Checking

```python
print(type(age))        # <class 'int'>
print(type(marks))      # <class 'list'>
```

---

## 🔹 **PART 2: CONDITIONAL STATEMENTS**

### 🔸 if, elif, else

```python
age = 20

if age >= 18:
    print("Adult")
elif age >= 13:
    print("Teenager")
else:
    print("Child")
```

🔹 **Comparison Operators:**

| Operator | Meaning          |
| -------- | ---------------- |
| `==`     | Equals           |
| `!=`     | Not equal        |
| `>`      | Greater          |
| `<`      | Lesser           |
| `>=`     | Greater or equal |
| `<=`     | Less or equal    |

🔹 **Logical Operators:**

| Operator | Use Case             |
| -------- | -------------------- |
| `and`    | Both conditions true |
| `or`     | At least one true    |
| `not`    | Reverses the result  |

```python
if age > 18 and is_student:
    print("College Student")
```

---

## 🔹 **PART 3: LOOPS**

### 🔸 for Loop

```python
for i in range(5):
    print(i)
```

✅ `range(n)` → generates numbers from `0 to n-1`

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

### 🔸 while Loop

```python
count = 0
while count < 5:
    print(count)
    count += 1
```

⛔ **Be careful of infinite loops!**

---

## 🔹 **PART 4: FUNCTIONS**

### 🔸 Defining and Calling

```python
def greet(name):
    return "Hello " + name

print(greet("Niraj"))
```

### 🔸 Parameters & Arguments

```python
def add(a, b=0):     # b has a default value
    return a + b

print(add(5))        # Output: 5
print(add(5, 3))     # Output: 8
```

### 🔸 Return vs Print

* `return` gives back the result to be used later.
* `print` just displays it.

---

## 🔹 **PART 5: LAMBDA EXPRESSIONS**

### 🔸 Anonymous Functions

```python
square = lambda x: x * x
print(square(4))    # Output: 16
```

Common in:

```python
nums = [1, 2, 3, 4]
squared = list(map(lambda x: x*x, nums))
print(squared)
```

---

## 🚀 Pro Tips for Professionals:

* ✅ Use `f-strings` for formatting:

  ```python
  name = "Niraj"
  print(f"Hello {name}")
  ```

* ✅ Write clean code: use proper indentation, naming, and comments.

* ✅ Understand `mutability` of data types. For example:

  ```python
  a = [1, 2]
  b = a
  b.append(3)
  print(a)   # Output: [1, 2, 3] - because lists are mutable
  ```

