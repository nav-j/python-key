# Python Practice Task – Animal Inheritance

## Problem Statement
Write a Python program that demonstrates **simple inheritance** using animals.

### Requirements
1. Create a **base class** `Animal` with:
   * Attribute: `name`.
   * Method: `speak()` → prints a generic message.
2. Create a **child class** `Dog` that inherits from `Animal` and:
   * Overrides the `speak()` method to print `"Woof!"`.
3. Create an object of `Dog` and call both methods.

---

## ✅ Solution Code

```python
#  Simple Inheritance Example

# Base class
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        print(f"{self.name} makes a sound.")

# Child class
class Dog(Animal):
    def speak(self):
        print(f"{self.name} says Woof!")

# Create object
dog1 = Dog("Buddy")

# Call methods
dog1.speak()
````

---

## 🖥 Example Output

```
Buddy says Woof!
```
