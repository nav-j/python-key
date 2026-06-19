# 🐍 Python Assignment (Theory + Practical)

## Topic: List, Tuple, Set, Dictionary, Loops, Functions & Range

**Student Name:** ___________________

**Date:** ___________________

**Total Marks:** 50

---

# Part A – Theory (20 Marks)

### Q1. What is a List in Python? Write one example. (2 Marks)

---

### Q2. What is the difference between a List and a Tuple? (2 Marks)

---

### Q3. What is a Set in Python? Why are sets useful? (2 Marks)

---

### Q4. What is a Dictionary? Write an example containing student information. (2 Marks)

---

### Q5. What is the purpose of the `range()` function? Give one example. (2 Marks)

---

### Q6. What is the difference between a `for` loop and a `while` loop? (2 Marks)

---

### Q7. What is a Function in Python? Why do we use functions? (2 Marks)

---

### Q8. Write the output:

```python
numbers = [10, 20, 30]

for num in numbers:
    print(num)
```

(2 Marks)

---

### Q9. What is the difference between `append()` and `add()` methods? (2 Marks)

---

### Q10. Explain the following code:

```python
student = {
    "name": "Aman",
    "course": "Python"
}

for key, value in student.items():
    print(key, value)
```

(2 Marks)

---

# Part B – Practical (30 Marks)

## Student Performance Management System

### Task Requirements

Create a Python program that performs the following operations:

### Step 1: Student Information (Dictionary)

Ask the user to enter:

* Student Name
* Roll Number
* Course Name

Store the information in a dictionary.

Example:

```python
student = {
    "name": "Aman",
    "roll_no": 101,
    "course": "Python"
}
```

---

### Step 2: Subject Marks (List)

Using a `for` loop and `range()`, ask the user to enter marks for 5 subjects.

Store the marks in a list.

---

### Step 3: Tuple Operations

Convert the marks list into a tuple.

Display:

* First Mark
* Last Mark
* First 3 Marks

---

### Step 4: Set Operations

Create a set from the marks tuple.

Display all unique marks.

---

### Step 5: Functions

Create the following functions:

```python
def total_marks(marks):
```

```python
def average_marks(marks):
```

```python
def highest_mark(marks):
```

```python
def lowest_mark(marks):
```

Use these functions to display:

* Total Marks
* Average Marks
* Highest Mark
* Lowest Mark

---

### Step 6: Loops

#### Using For Loop

Display all marks.

#### Using While Loop

Display all marks again.

---

### Step 7: Grade Analysis

Using a loop, count:

| Grade | Condition    |
| ----- | ------------ |
| A     | 90 and above |
| B     | 80–89        |
| C     | 70–79        |
| D     | Below 70     |

Display the number of students in each grade category.

---

### Step 8: Search Marks

Ask the user to enter a mark.

Check whether the mark exists in the tuple using:

```python
in
```

Display:

```text
Mark Found
```

or

```text
Mark Not Found
```

---

### Step 9: Display Student Information

Using a loop, display all key-value pairs stored in the dictionary.

Example Output:

```text
name : Aman
roll_no : 101
course : Python
```

---

# Bonus Challenge (5 Marks)

Add one more function:

```python
def pass_fail(marks):
```

If average marks are:

* 40 or above → Pass
* Below 40 → Fail

Display the final result. 🎯
