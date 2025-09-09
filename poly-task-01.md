# Python Task – Polymorphism with Animals

## Problem Statement
Demonstrate **polymorphism** in Python using a base class and multiple subclasses that override the same method.

---

##  Requirements
1. Create a **base class** `Animal` with a method `speak()`.
2. Create at least **three subclasses** (`Dog`, `Cat`, `Cow`) that **override** the `speak()` method.
   - `Dog` → `"Woof!"`
   - `Cat` → `"Meow!"`
   - `Cow` → `"Moo!"`
3. Write a function `animal_sound(animal)` that takes any object of type `Animal` and calls its `speak()` method.
4. Demonstrate **polymorphism** by passing different animal objects to the function.

---

## Example Code

```python
# Base class
class Animal:
    def speak(self):
        return "Some sound"

# Subclass Dog
class Dog(Animal):
    def speak(self):
        return "Woof!"

# Subclass Cat
class Cat(Animal):
    def speak(self):
        return "Meow!"

# Subclass Cow
class Cow(Animal):
    def speak(self):
        return "Moo!"

# Function that uses polymorphism
def animal_sound(animal):
    print(animal.speak())


# ✅ Example usage
dog = Dog()
cat = Cat()
cow = Cow()

animal_sound(dog)   # Output: Woof!
animal_sound(cat)   # Output: Meow!
animal_sound(cow)   # Output: Moo!
````

---

## 🎯 Expected Output

```
Woof!
Meow!
Moo!
```

---

## 💡 Concept Highlight

* **Polymorphism** means *many forms*.
* In this example, the `animal_sound()` function works differently depending on the object (`Dog`, `Cat`, `Cow`) passed to it.
* This shows how the **same interface** (`speak()`) can have **different implementations**.
