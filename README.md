# difference-between-the-is-and-in-operators
 Day 1: Python is vs in Operators
markdown
# 🐍 Python Basics – Day 1  
## Difference Between `is` and `in` Operators in Python

Understanding Python's `is` and `in` operators is crucial for writing clean and correct code.

---

### 🔹 `is` — Identity Operator  
The `is` operator checks whether two variables refer to the **same object in memory**.

```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)  # True: a and b are the same object
print(a is c)  # False: c is a different object with same content
Use it for identity comparison, like checking if a variable is None:
if my_var is None:
    print("No value assigned")
🔹 in — Membership Operator
The in operator checks whether a value exists in an iterable (like lists, strings, or tuples).

fruits = ['apple', 'banana', 'cherry']

print('banana' in fruits)  # True
print('mango' in fruits)   # False

text = "hello world"
print('h' in text)         # True
📊 Summary Table
Operator	Purpose	Example Use Case
is	Identity (same object)	Checking if a is None
in	Membership (exists in group)	Checking if 'x' in my_list

✅ Quick Tips
Use is for identity checks (e.g., None, singleton values).

Use in to check for membership in collections.

is does not check for equality — that’s what == is for.
