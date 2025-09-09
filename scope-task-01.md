# Python Task – Simple Scope Practice

## Problem Statement
Write a Python program to **demonstrate local and global variables** and understand how variable scope works in functions.

---

## 📝 Requirements
1. Create a **global variable** `name = "Alice"`.
2. Write a function `greet_local()` that declares a **local variable** `name = "Bob"` and prints:
```

Hello, <name> from local!

```
3. Write another function `greet_global()` that prints:
```

Hello, <name> from global!

````
using the global variable.
4. Call both functions and observe the difference between **local** and **global** scope.

---

## 💻 Example Code

```python
name = "Alice"  # Global variable

def greet_local():
 name = "Bob"  # Local variable
 print("Hello,", name, "from local!")

def greet_global():
 print("Hello,", name, "from global!")


greet_local()
greet_global()
````

---

## 🎯 Expected Output

```
Hello, Bob from local!
Hello, Alice from global!
```

---

## 💡 Hints

* **Local variables** only exist inside the function they are declared.
* **Global variables** can be accessed anywhere outside functions.
