# Python Task – Polymorphism with Shapes

## Problem Statement
Demonstrate **polymorphism** in Python by creating a base class and multiple subclasses representing different shapes, each calculating its **area**.

---

## Requirements
1. Create a **base class** `Shape` with a method `area()`.
2. Create at least **three subclasses** that override the `area()` method:
   - `Circle` → area = π × r²
   - `Rectangle` → area = length × width
   - `Triangle` → area = 0.5 × base × height
3. Write a function `print_area(shape)` that takes any `Shape` object and prints its area.
4. Demonstrate **polymorphism** by passing different shape objects to the function.

---

## Example Code

```python
import math

# Base class
class Shape:
    def area(self):
        return 0

# Subclass Circle
class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return math.pi * (self.radius ** 2)

# Subclass Rectangle
class Rectangle(Shape):
    def __init__(self, length, width):
        self.length = length
        self.width = width

    def area(self):
        return self.length * self.width

# Subclass Triangle
class Triangle(Shape):
    def __init__(self, base, height):
        self.base = base
        self.height = height

    def area(self):
        return 0.5 * self.base * self.height

# Function that demonstrates polymorphism
def print_area(shape):
    print(f"Area: {shape.area()}")


# ✅ Example usage
circle = Circle(5)
rectangle = Rectangle(4, 6)
triangle = Triangle(3, 7)

print_area(circle)     # Output: Area: 78.53981633974483
print_area(rectangle)  # Output: Area: 24
print_area(triangle)   # Output: Area: 10.5
````

---

## 🎯 Sample Output

```
Area: 78.53981633974483
Area: 24
Area: 10.5
```

---

## 💡 Concept Highlight

* **Polymorphism** allows the same function (`print_area`) to work differently depending on the **object type** (`Circle`, `Rectangle`, `Triangle`) passed.
* The `area()` method is **overridden** in each subclass to provide the correct implementation for that shape.
