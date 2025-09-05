# Python Practice Task – Multilevel Inheritance (Person → Student → Graduate)

## Problem Statement
Write a Python program that demonstrates **multilevel inheritance**.

### Requirements
1. Create a **base class** `Person` with:
   * Attribute: `name`.
   * Method: `display_name()` → prints the person’s name.
2. Create a **child class** `Student` that inherits from `Person` and adds:
   * Attribute: `student_id`.
   * Method: `display_student()` → prints name and student ID.
3. Create a **child class** `Graduate` that inherits from `Student` and adds:
   * Attribute: `degree`.
   * Method: `display_graduate()` → prints name, ID, and degree.
4. Create an object of `Graduate` and call all methods.

---

## ✅ Solution Code

```python
# Multilevel Inheritance Example

# Base class
class Person:
    def __init__(self, name):
        self.name = name

    def display_name(self):
        print(f"Name: {self.name}")

# Child class (inherits Person)
class Student(Person):
    def __init__(self, name, student_id):
        super().__init__(name)
        self.student_id = student_id

    def display_student(self):
        self.display_name()
        print(f"Student ID: {self.student_id}")

# Child class (inherits Student)
class Graduate(Student):
    def __init__(self, name, student_id, degree):
        super().__init__(name, student_id)
        self.degree = degree

    def display_graduate(self):
        self.display_student()
        print(f"Degree: {self.degree}")
        print("-" * 30)

# Create object
graduate1 = Graduate("Alice", "S123", "MSc Computer Science")

# Call methods
graduate1.display_graduate()
````

---

## 🖥 Example Output

```
Name: Alice
Student ID: S123
Degree: MSc Computer Science
------------------------------
```
