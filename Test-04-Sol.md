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
