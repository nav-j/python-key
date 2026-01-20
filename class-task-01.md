# Python Practice Task – Student Information System

## Problem Statement
Write a Python program that uses **classes and objects** to manage student information.

### Requirements
1. Create a class `Student` with:
   * Attributes: `name`, `age`, `grade`.
   * A method `display_info()` to print student details.
2. Create **2 student objects** with different details.
3. Call the `display_info()` method for each object to show their information.

---

##  Solution Code

```python
#  Student Information System using Class & Objects

# Define a class
class Student:
    def __init__(self, name, age, grade):
        self.name = name
        self.age = age
        self.grade = grade

    # Method to display student information
    def display_info(self):
        print(f"Student Name: {self.name}")
        print(f"Age: {self.age}")
        print(f"Grade: {self.grade}")
        print("-" * 30)

# Create objects of Student class
student1 = Student("John", 15, "10th")
student2 = Student("Emma", 14, "9th")

# Call method to display info
student1.display_info()
student2.display_info()
````

---

## Example Output

```
Student Name: John
Age: 15
Grade: 10th
------------------------------
Student Name: Emma
Age: 14
Grade: 9th
------------------------------
```
