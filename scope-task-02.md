# Python Task – Understanding Variable Scope

## Problem Statement
Demonstrate **local, global, and nonlocal variables** in Python and how **scope** affects variable behavior in functions.

---

## 📝 Requirements
1. **Global Variable**
   - Create a global variable `counter = 0`.
   - Write a function `increment_global()` that increments the global `counter` using the `global` keyword.
2. **Local Variable**
   - Write a function `increment_local()` that declares a local variable `counter = 0` and increments it.
   - Show that this does not affect the global `counter`.
3. **Nonlocal Variable**
   - Write a function `outer_function()` with a variable `counter = 0`.
   - Inside it, define `inner_function()` that uses the `nonlocal` keyword to modify `counter`.
   - Call `inner_function()` inside `outer_function()` and print the updated `counter`.
4. Demonstrate how **local, global, and nonlocal scopes** behave differently.

---

## 💻 Example Code

```python
# Global variable
counter = 0

# Function to modify global variable
def increment_global():
    global counter
    counter += 1
    print("Global counter:", counter)

# Function with local variable
def increment_local():
    counter = 0  # Local variable
    counter += 1
    print("Local counter:", counter)

# Function demonstrating nonlocal variable
def outer_function():
    counter = 0  # Enclosing (nonlocal) variable
    def inner_function():
        nonlocal counter
        counter += 1
        print("Nonlocal counter:", counter)
    inner_function()
    print("Outer counter after inner:", counter)


# ✅ Example usage
increment_global()   # Modifies global counter
increment_local()    # Modifies local counter only
outer_function()     # Modifies nonlocal counter
print("Global counter at end:", counter)
````

---

## 🎯 Sample Output

```
Global counter: 1
Local counter: 1
Nonlocal counter: 1
Outer counter after inner: 1
Global counter at end: 1
```

---

## 💡 Concept Highlight

* **Global:** accessible and modifiable anywhere with `global`.
* **Local:** exists only inside the function.
* **Nonlocal:** allows nested functions to modify variables in the enclosing scope.
