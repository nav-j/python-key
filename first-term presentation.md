## Advanced Python Assignment: Student Information & Performance Analyzer

###  Objective

Create a Python program that uses:

* **Data Types** (`int`, `float`, `str`, `bool`, `list`)
* **Strings** (formatting, slicing, case conversion, length)
* **Operators** (arithmetic, comparison, logical, assignment, membership)

The program should take user input and generate a detailed report.

---

##  Task Requirements

### Step 1: Get User Input

Ask the user to enter:

1. Full Name
2. Age
3. Course Name
4. Python Marks
5. AI Marks
6. Web Development Marks

---

### Step 2: Perform String Operations

1. Display the name in **UPPERCASE**.
2. Display the name in **lowercase**.
3. Display the first 5 characters of the name.
4. Display the last 3 characters of the name.
5. Count the total number of characters in the name.

---

### Step 3: Perform Arithmetic Operations

1. Calculate the total marks.
2. Calculate the percentage.
3. Calculate the average marks.

---

### Step 4: Perform Comparison Operators

1. Check if percentage is greater than or equal to 80.
2. Check if percentage is greater than or equal to 50.

Store results in Boolean variables.

---

### Step 5: Perform Logical Operators

Create a scholarship eligibility check:

A student is eligible if:

* Percentage ≥ 80
* Age ≤ 25

Use logical operators and store the result in a Boolean variable.

---

### Step 6: Perform Membership Operators

1. Store all subjects in a list:

   ```python
   ["Python", "AI", "Web Development"]
   ```
2. Ask the user to enter a subject name.
3. Check whether the subject exists in the list.

---

### Step 7: Generate a Formatted Report

Display:

```text
-----------------------------------
         STUDENT REPORT
-----------------------------------
Name          : Navjot Kaur
Course        : BCA
Age           : 20

Total Marks   : 255
Percentage    : 85.00%
Average Marks : 85.00

Excellent     : True
Passed        : True
Scholarship   : True

Subject Found : True
-----------------------------------
```

---

# ✅ Solution Code

```python
# Student Information & Performance Analyzer

# User Input
name = input("Enter Full Name: ")
age = int(input("Enter Age: "))
course = input("Enter Course Name: ")

python_marks = float(input("Enter Python Marks: "))
ai_marks = float(input("Enter AI Marks: "))
web_marks = float(input("Enter Web Development Marks: "))

# String Operations
print("\n--- STRING OPERATIONS ---")
print("Uppercase Name:", name.upper())
print("Lowercase Name:", name.lower())
print("First 5 Characters:", name[:5])
print("Last 3 Characters:", name[-3:])
print("Total Characters:", len(name))

# Arithmetic Operations
total = python_marks + ai_marks + web_marks
percentage = (total / 300) * 100
average = total / 3

# Comparison Operators
excellent = percentage >= 80
passed = percentage >= 50

# Logical Operators
scholarship = (percentage >= 80) and (age <= 25)

# Membership Operators
subjects = ["Python", "AI", "Web Development"]
subject_search = input("\nEnter Subject to Search: ")

subject_found = subject_search in subjects

# Report
print("\n" + "-" * 35)
print("         STUDENT REPORT")
print("-" * 35)

print(f"Name          : {name}")
print(f"Course        : {course}")
print(f"Age           : {age}")

print(f"\nTotal Marks   : {total}")
print(f"Percentage    : {percentage:.2f}%")
print(f"Average Marks : {average:.2f}")

print(f"\nExcellent     : {excellent}")
print(f"Passed        : {passed}")
print(f"Scholarship   : {scholarship}")

print(f"\nSubject Found : {subject_found}")

print("-" * 35)
```

