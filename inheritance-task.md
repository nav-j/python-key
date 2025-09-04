# Python Practice Task – Employee Management (Inheritance)

##  Problem Statement
Write a Python program that uses **inheritance** to manage different types of employees.

### Requirements
1. Create a **base class** `Employee` with:
   * Attributes: `name`, `salary`.
   * Method: `display_info()` → prints employee details.
2. Create two **child classes**:
   * `Manager` → adds an attribute `department`.
   * `Developer` → adds an attribute `programming_language`.
3. Create objects of both classes and display their information.

---

## ✅ Solution Code

```python
# 👨‍💼 Employee Management using Inheritance

# Base class
class Employee:
    def __init__(self, name, salary):
        self.name = name
        self.salary = salary

    def display_info(self):
        print(f"Name: {self.name}")
        print(f"Salary: ${self.salary}")

# Child class - Manager
class Manager(Employee):
    def __init__(self, name, salary, department):
        super().__init__(name, salary)
        self.department = department

    def display_info(self):
        super().display_info()
        print(f"Department: {self.department}")
        print("-" * 30)

# Child class - Developer
class Developer(Employee):
    def __init__(self, name, salary, programming_language):
        super().__init__(name, salary)
        self.programming_language = programming_language

    def display_info(self):
        super().display_info()
        print(f"Programming Language: {self.programming_language}")
        print("-" * 30)

# Create objects
manager1 = Manager("Alice", 80000, "HR")
developer1 = Developer("Bob", 70000, "Python")

# Display info
manager1.display_info()
developer1.display_info()
````

---

## 🖥 Example Output

```
Name: Alice
Salary: $80000
Department: HR
------------------------------
Name: Bob
Salary: $70000
Programming Language: Python
------------------------------
```
