# 🐍 Python Fundamentals Assignment

## 📖 Overview

This assignment is designed for beginners to practice the fundamental concepts of Python programming. Students will learn how to work with variables, data types, user input, string methods, arithmetic operators, and assignment operators while creating a simple **Student Profile and Marks Calculator** program.


## 📝 Assignment Tasks

### Task 1: Variables and User Input

Create variables to store:

* Student Name
* Course Name
* Age
* City

Display all values entered by the user.

---

### Task 2: Data Types

Use the `type()` function to display the data type of each variable.

---

### Task 3: String Methods

Perform the following operations on the student's name:

* Convert to uppercase
* Convert to lowercase
* Count total characters
* Replace a character

---

### Task 4: Arithmetic Operators

Accept marks for three subjects and calculate:

* Total Marks
* Average Marks
* Percentage

---

### Task 5: Assignment Operators

Perform operations on a variable named `score`:

```python
score = 50

score += 10
score -= 5
score *= 2
score /= 5
```

Display the value after each operation.

---

### Task 6: Final Student Report

Generate a formatted report containing:

* Name
* Course
* Age
* City
* Total Marks
* Average
* Percentage

---

## ⭐ Bonus Challenge

Create a variable:

```python
balance = 1000
```

Perform:

```python
balance += 500
balance -= 200
balance *= 2
balance //= 3
```

Display the balance after each operation.

---

## 📂 Expected Output

```text
========== STUDENT REPORT ==========

Name        : Aman
Course      : Python Programming
Age         : 20
City        : Chandigarh

Total Marks : 255
Average     : 85.0
Percentage  : 85.0%

====================================
```

# 🐍 Python Fundamentals Assignment – Solution

```python
# ==========================================
# PYTHON FUNDAMENTALS ASSIGNMENT SOLUTION
# Student Profile and Marks Calculator
# ==========================================

# ------------------------------------------
# Task 1: Variables and User Input
# ------------------------------------------

name = input("Enter Student Name: ")
course = input("Enter Course Name: ")
age = int(input("Enter Age: "))
city = input("Enter City: ")

print("\n===== STUDENT DETAILS =====")
print("Name   :", name)
print("Course :", course)
print("Age    :", age)
print("City   :", city)

# ------------------------------------------
# Task 2: Data Types
# ------------------------------------------

print("\n===== DATA TYPES =====")
print("Name Data Type   :", type(name))
print("Course Data Type :", type(course))
print("Age Data Type    :", type(age))
print("City Data Type   :", type(city))

# ------------------------------------------
# Task 3: String Methods
# ------------------------------------------

print("\n===== STRING METHODS =====")

print("Uppercase Name :", name.upper())
print("Lowercase Name :", name.lower())
print("Total Characters :", len(name))

old_char = input("Enter character to replace: ")
new_char = input("Enter new character: ")

print("Updated Name :", name.replace(old_char, new_char))

# ------------------------------------------
# Task 4: Arithmetic Operators
# ------------------------------------------

print("\n===== MARKS CALCULATION =====")

mark1 = float(input("Enter Marks of Subject 1: "))
mark2 = float(input("Enter Marks of Subject 2: "))
mark3 = float(input("Enter Marks of Subject 3: "))

total = mark1 + mark2 + mark3
average = total / 3
percentage = (total / 300) * 100

print("\nTotal Marks :", total)
print("Average Marks :", round(average, 2))
print("Percentage :", round(percentage, 2), "%")

# ------------------------------------------
# Task 5: Assignment Operators
# ------------------------------------------

print("\n===== ASSIGNMENT OPERATORS =====")

score = 50
print("Initial Score :", score)

score += 10
print("After += 10 :", score)

score -= 5
print("After -= 5 :", score)

score *= 2
print("After *= 2 :", score)

score /= 5
print("After /= 5 :", score)

# ------------------------------------------
# Task 6: Final Student Report
# ------------------------------------------

print("\n")
print("=" * 40)
print("         STUDENT REPORT")
print("=" * 40)

print("Name        :", name)
print("Course      :", course)
print("Age         :", age)
print("City        :", city)

print("\nTotal Marks :", total)
print("Average     :", round(average, 2))
print("Percentage  :", round(percentage, 2), "%")

print("=" * 40)

# ------------------------------------------
# Bonus Challenge
# ------------------------------------------

print("\n===== BONUS CHALLENGE =====")

balance = 1000
print("Initial Balance :", balance)

balance += 500
print("After += 500 :", balance)

balance -= 200
print("After -= 200 :", balance)

balance *= 2
print("After *= 2 :", balance)

balance //= 3
print("After //= 3 :", balance)
```

## Sample Output

```text
Enter Student Name: Aman
Enter Course Name: Python Programming
Enter Age: 20
Enter City: Chandigarh

===== STUDENT DETAILS =====
Name   : Aman
Course : Python Programming
Age    : 20
City   : Chandigarh

===== DATA TYPES =====
Name Data Type   : <class 'str'>
Course Data Type : <class 'str'>
Age Data Type    : <class 'int'>
City Data Type   : <class 'str'>

===== STRING METHODS =====
Uppercase Name : AMAN
Lowercase Name : aman
Total Characters : 4

===== MARKS CALCULATION =====
Total Marks : 255.0
Average Marks : 85.0
Percentage : 85.0 %

===== ASSIGNMENT OPERATORS =====
Initial Score : 50
After += 10 : 60
After -= 5 : 55
After *= 2 : 110
After /= 5 : 22.0

========================================
         STUDENT REPORT
========================================
Name        : Aman
Course      : Python Programming
Age         : 20
City        : Chandigarh

Total Marks : 255.0
Average     : 85.0
Percentage  : 85.0 %
========================================

===== BONUS CHALLENGE =====
Initial Balance : 1000
After += 500 : 1500
After -= 200 : 1300
After *= 2 : 2600
After //= 3 : 866
```
