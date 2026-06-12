# 🐍 Python Combined Theory + Practical Assignment

## Topic: Data Types, Variables, User Input, List & Tuple

### Student Name: ___________

### Date: ___________

### Total Marks: 50

---

# Part A – Theory (20 Marks)

### Q1. What is a variable in Python? Give one example. (2 Marks)

---

### Q2. What is the difference between `int`, `float`, `str`, and `bool` data types? (4 Marks)

| Data Type | Description | Example |
| --------- | ----------- | ------- |
| int       |             |         |
| float     |             |         |
| str       |             |         |
| bool      |             |         |

---

### Q3. What is the purpose of the `input()` function in Python? (2 Marks)

---

### Q4. Differentiate between List and Tuple. (4 Marks)

| Feature           | List | Tuple |
| ----------------- | ---- | ----- |
| Syntax            |      |       |
| Mutable/Immutable |      |       |
| Example           |      |       |

---

### Q5. Write the output of the following code: (4 Marks)

```python
x = 10
y = 5.5

print(type(x))
print(type(y))
```

Output:

---

---

### Q6. Fill in the blanks: (4 Marks)

1. A list is enclosed within __________.
2. A tuple is enclosed within __________.
3. The function used to take input from a user is __________.
4. `True` and `False` belong to the __________ data type.

---

# Part B – Practical (30 Marks)

## Scenario:

Create a **Student Information System** using Python.

### Requirements:

### Task 1: User Input & Variables (5 Marks)

Take the following inputs from the user:

* Student Name
* Roll Number
* Age
* Course

Store them in variables.

Example:

```python
name = input("Enter Name: ")
```

---

### Task 2: Data Types (5 Marks)

Display the data type of each variable using:

```python
type()
```

Example Output:

```
Name Data Type: <class 'str'>
Age Data Type: <class 'int'>
```

---

### Task 3: Create a List (5 Marks)

Ask the user to enter marks of 3 subjects.

Store them in a list named `marks`.

Example:

```python
marks = [78, 85, 90]
```

Perform the following:

1. Print all marks.
2. Print highest mark.
3. Print lowest mark.
4. Print total marks.

---

### Task 4: Create a Tuple (5 Marks)

Create a tuple named `subjects`.

```python
subjects = ("Python", "Web Development", "Database")
```

Perform the following:

1. Print all subjects.
2. Print the first subject.
3. Print the last subject.
4. Count total subjects.

---

### Task 5: List Operations (5 Marks)

Perform these operations on the `marks` list:

1. Add one more mark using `append()`.
2. Remove a mark using `remove()`.
3. Sort the list.
4. Display the updated list.

---

### Task 6: Final Student Report (5 Marks)

Display all details in a formatted report:

Example Output:

```
========== STUDENT REPORT ==========
Name        : Rahul
Roll Number : 101
Age         : 20
Course      : B.Tech

Subjects    : ('Python', 'Web Development', 'Database')
Marks       : [78, 85, 90]

Highest Mark: 90
Lowest Mark : 78
Total Marks : 253
====================================
```

---

# Bonus Challenge (Optional – 5 Extra Marks)

1. Calculate the average of all marks.
2. Display whether the student has passed or failed.

Condition:

```python
Average >= 40 → Pass
Average < 40  → Fail
```

---

# Learning Outcomes

After completing this assignment, students will be able to:

✅ Use variables in Python
✅ Accept user input
✅ Identify data types using `type()`
✅ Create and manipulate lists
✅ Create and access tuples
✅ Apply list methods (`append()`, `remove()`, `sort()`)
✅ Generate a formatted report using Python programs


# Solution

```python
# ======================================
# STUDENT INFORMATION SYSTEM
# ======================================

# Task 1: User Input & Variables

name = input("Enter Student Name: ")
roll_no = input("Enter Roll Number: ")
age = int(input("Enter Age: "))
course = input("Enter Course: ")

# --------------------------------------
# Task 2: Data Types
# --------------------------------------

print("\n===== DATA TYPES =====")
print("Name Data Type      :", type(name))
print("Roll No Data Type   :", type(roll_no))
print("Age Data Type       :", type(age))
print("Course Data Type    :", type(course))

# --------------------------------------
# Task 3: Create a List
# --------------------------------------

marks = []

mark1 = int(input("\nEnter Marks of Subject 1: "))
mark2 = int(input("Enter Marks of Subject 2: "))
mark3 = int(input("Enter Marks of Subject 3: "))

marks.append(mark1)
marks.append(mark2)
marks.append(mark3)

print("\n===== MARKS DETAILS =====")
print("Marks List :", marks)
print("Highest Mark :", max(marks))
print("Lowest Mark  :", min(marks))
print("Total Marks  :", sum(marks))

# --------------------------------------
# Task 4: Create a Tuple
# --------------------------------------

subjects = ("Python", "Web Development", "Database")

print("\n===== SUBJECT DETAILS =====")
print("Subjects :", subjects)
print("First Subject :", subjects[0])
print("Last Subject  :", subjects[-1])
print("Total Subjects :", len(subjects))

# --------------------------------------
# Task 5: List Operations
# --------------------------------------

new_mark = int(input("\nEnter One More Mark to Add: "))
marks.append(new_mark)

remove_mark = int(input("Enter Mark to Remove: "))

if remove_mark in marks:
    marks.remove(remove_mark)
    print("Mark Removed Successfully!")
else:
    print("Mark Not Found!")

marks.sort()

print("Updated Marks List :", marks)

# --------------------------------------
# Task 6: Final Student Report
# --------------------------------------

highest = max(marks)
lowest = min(marks)
total = sum(marks)
average = total / len(marks)

# Bonus Challenge
if average >= 40:
    result = "Pass"
else:
    result = "Fail"

print("\n")
print("=" * 40)
print("          STUDENT REPORT")
print("=" * 40)

print("Name         :", name)
print("Roll Number  :", roll_no)
print("Age          :", age)
print("Course       :", course)

print("\nSubjects     :", subjects)
print("Marks        :", marks)

print("\nHighest Mark :", highest)
print("Lowest Mark  :", lowest)
print("Total Marks  :", total)
print("Average      :", round(average, 2))
print("Result       :", result)

print("=" * 40)
```

### Sample Input

```text
Enter Student Name: Aman
Enter Roll Number: 101
Enter Age: 20
Enter Course: B.Tech

Enter Marks of Subject 1: 78
Enter Marks of Subject 2: 85
Enter Marks of Subject 3: 90

Enter One More Mark to Add: 95
Enter Mark to Remove: 78
```

### Sample Output

```text
========================================
          STUDENT REPORT
========================================
Name         : Aman
Roll Number  : 101
Age          : 20
Course       : B.Tech

Subjects     : ('Python', 'Web Development', 'Database')
Marks        : [85, 90, 95]

Highest Mark : 95
Lowest Mark  : 85
Total Marks  : 270
Average      : 90.0
Result       : Pass
========================================
```

This solution covers:

* Variables
* User Input
* Data Types (`str`, `int`)
* Lists
* Tuples
* List Methods (`append()`, `remove()`, `sort()`)
* Built-in Functions (`max()`, `min()`, `sum()`, `len()`)
* Conditional Statements (`if-else`)
* Formatted Report Generation
