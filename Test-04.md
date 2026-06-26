# Python Assignment (50 Marks)

## Topic: Range, Array, Iterator, Functions, Regex & Exception Handling

**Total Marks: 50**

---

# Part A: Theory (20 Marks)

### Q1. What is the purpose of the `range()` function in Python? Write its syntax and one example. (4 Marks)

---

### Q2. What is an Array in Python? How is it different from a List? (4 Marks)

---

### Q3. What is an Iterator? Explain the use of `iter()` and `next()` with an example. (4 Marks)

---

### Q4. What is the purpose of a Function in Python? Differentiate between built-in and user-defined functions. (4 Marks)

---

### Q5. Explain:

a) Regular Expressions (Regex)
b) Exception Handling (`try-except`) (4 Marks)

---

# Part B: Practical Task (30 Marks)

## Student Marks Management System

Create a Python program that performs the following operations:

### Step 1: Student Count (3 Marks)

* Ask the user to enter the number of students.
* Use **try-except** to handle invalid input.

Example:

```python
Enter number of students: 5
```

---

### Step 2: Store Marks Using Array (5 Marks)

* Import the `array` module.
* Use `range()` and a `for` loop to accept marks for all students.
* Store marks in an integer array.

Example:

```python
Enter marks of Student 1: 80
Enter marks of Student 2: 75
Enter marks of Student 3: 90
```

---

### Step 3: Create Functions (5 Marks)

Create the following user-defined functions:

```python
calculate_average()
find_grade()
```

Requirements:

* `calculate_average()` should return the average marks.
* `find_grade()` should return a grade based on the average.

| Average Marks | Grade |
| ------------- | ----- |
| 90 and above  | A     |
| 80 – 89       | B     |
| 70 – 79       | C     |
| Below 70      | D     |

---

### Step 4: Use Iterator (5 Marks)

* Create an iterator from the marks array using `iter()`.
* Display all marks using `next()`.

Example:

```python
Marks Using Iterator:
80
75
90
```

---

### Step 5: Email Validation Using Regex (5 Marks)

* Ask the user to enter an email address.
* Use Regular Expression (`re`) to validate the email.

Example:

```python
Enter Email: student@gmail.com
Valid Email
```

---

### Step 6: Generate Report (7 Marks)

Display the following:

```python
----- STUDENT REPORT -----
```

* Total Marks
* Average Marks
* Highest Marks
* Lowest Marks
* Grade
* Email Status

Sample Output:

```python
----- STUDENT REPORT -----

Total Marks : 245
Average Marks : 81.67
Highest Marks : 90
Lowest Marks : 75
Grade : B

Email Status : Valid
```

---

# Marking Scheme

| Section                            | Marks        |
| ---------------------------------- | ------------ |
| Theory Questions                   | 20           |
| Student Count & Exception Handling | 3            |
| Array & Range Implementation       | 5            |
| Functions                          | 5            |
| Iterator Usage                     | 5            |
| Regex Validation                   | 5            |
| Report Generation                  | 7            |
| **Total**                          | **50 Marks** |

**Submission Requirements:**

1. Python Source Code (.py)
2. Screenshot of Program Output
3. Proper comments in the code explaining each section.

# practical solution

# Solution: Student Marks Management System

```python
from array import array
import re

# Function to calculate average
def calculate_average(marks):
    return sum(marks) / len(marks)

# Function to find grade
def find_grade(avg):
    if avg >= 90:
        return "A"
    elif avg >= 80:
        return "B"
    elif avg >= 70:
        return "C"
    else:
        return "D"

# Step 1: Get number of students
try:
    num_students = int(input("Enter number of students: "))

    # Step 2: Store marks in array
    marks = array('i')

    for i in range(num_students):
        mark = int(input(f"Enter marks of Student {i+1}: "))
        marks.append(mark)

    # Step 3: Calculate average and grade
    average = calculate_average(marks)
    grade = find_grade(average)

    # Step 4: Iterator
    print("\nMarks Using Iterator:")
    mark_iterator = iter(marks)

    for i in range(len(marks)):
        print(next(mark_iterator))

    # Step 5: Email Validation using Regex
    email = input("\nEnter Email Address: ")

    pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'

    if re.match(pattern, email):
        email_status = "Valid"
    else:
        email_status = "Invalid"

    # Step 6: Generate Report
    total_marks = sum(marks)
    highest_marks = max(marks)
    lowest_marks = min(marks)

    print("\n----- STUDENT REPORT -----")
    print(f"Total Marks   : {total_marks}")
    print(f"Average Marks : {average:.2f}")
    print(f"Highest Marks : {highest_marks}")
    print(f"Lowest Marks  : {lowest_marks}")
    print(f"Grade         : {grade}")
    print(f"Email Status  : {email_status}")

except ValueError:
    print("Error: Please enter valid numeric values.")
```

### Sample Output

```text
Enter number of students: 3
Enter marks of Student 1: 80
Enter marks of Student 2: 75
Enter marks of Student 3: 90

Marks Using Iterator:
80
75
90

Enter Email Address: student@gmail.com

----- STUDENT REPORT -----
Total Marks   : 245
Average Marks : 81.67
Highest Marks : 90
Lowest Marks  : 75
Grade         : B
Email Status  : Valid
```

### Concepts Used

* `range()`
* `array` module
* User-defined functions
* Iterator (`iter()` and `next()`)
* Regular Expressions (`re`)
* Exception Handling (`try-except`)
* Loops and Conditions
* User Input and Output

# Theory Solution

# Theory Solutions

## Q1. What is the purpose of the `range()` function in Python? Write its syntax and one example. (4 Marks)

### Answer:

The `range()` function is used to generate a sequence of numbers. It is commonly used with loops to repeat a block of code a specific number of times.

### Syntax:

```python
range(start, stop, step)
```

### Example:

```python
for i in range(1, 6):
    print(i)
```

### Output:

```text
1
2
3
4
5
```

---

## Q2. What is an Array in Python? How is it different from a List? (4 Marks)

### Answer:

An Array is a data structure used to store multiple values of the same data type in a single variable. Python provides arrays through the `array` module.

### Example:

```python
from array import array

numbers = array('i', [10, 20, 30, 40])
print(numbers)
```

### Difference Between Array and List

| Array                           | List                           |
| ------------------------------- | ------------------------------ |
| Stores same data type           | Can store different data types |
| Requires `array` module         | Built into Python              |
| Uses less memory                | Uses more memory               |
| Faster for numerical operations | More flexible                  |

---

## Q3. What is an Iterator? Explain the use of `iter()` and `next()` with an example. (4 Marks)

### Answer:

An Iterator is an object that allows us to access elements of a collection one at a time.

* `iter()` creates an iterator object.
* `next()` retrieves the next element from the iterator.

### Example:

```python
numbers = [10, 20, 30]

it = iter(numbers)

print(next(it))
print(next(it))
print(next(it))
```

### Output:

```text
10
20
30
```

### Benefits of Iterators:

* Access elements one by one.
* Save memory when working with large datasets.
* Used internally by loops.

---

## Q4. What is the purpose of a Function in Python? Differentiate between built-in and user-defined functions. (4 Marks)

### Answer:

A Function is a block of reusable code that performs a specific task. Functions help reduce code repetition and improve readability.

### Example:

```python
def greet():
    print("Welcome to Python")

greet()
```

### Types of Functions

#### 1. Built-in Functions

Functions that are already available in Python.

Examples:

```python
print()
len()
sum()
max()
```

#### 2. User-defined Functions

Functions created by the programmer using the `def` keyword.

Example:

```python
def add(a, b):
    return a + b
```

### Difference

| Built-in Function          | User-defined Function      |
| -------------------------- | -------------------------- |
| Already provided by Python | Created by programmer      |
| No definition required     | Must be defined before use |
| Example: `len()`           | Example: `add()`           |

---

## Q5. Explain: (4 Marks)

### (a) Regular Expressions (Regex)

Regular Expressions (Regex) are patterns used to search, validate, and manipulate text.

Python provides the `re` module for working with regex.

### Example:

```python
import re

email = "student@gmail.com"

pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'

if re.match(pattern, email):
    print("Valid Email")
```

### Uses of Regex:

* Email validation
* Phone number validation
* Searching text patterns
* Data extraction

---

### (b) Exception Handling (`try-except`)

Exception Handling is used to handle runtime errors and prevent the program from crashing.

### Syntax:

```python
try:
    # code that may cause an error
except:
    # code to handle the error
```

### Example:

```python
try:
    num = int(input("Enter a number: "))
    print(num)
except ValueError:
    print("Invalid Input")
```

### Output (if user enters text):

```text
Enter a number: abc
Invalid Input
```

### Benefits:

* Prevents program crashes.
* Handles unexpected errors gracefully.
* Improves program reliability and user experience.
