# 🐍 Python Tasks Using `if`, `elif`, and `else`

## Task 1: Check Positive, Negative, or Zero

### Question:

Take a number from the user and check whether it is:

* Positive
* Negative
* Zero

### Example:

```python
num = int(input("Enter a number: "))

if num > 0:
    print("Positive Number")
elif num < 0:
    print("Negative Number")
else:
    print("Zero")
```

---

## Task 2: Student Grade Calculator

### Question:

Take marks from the user and display the grade:

| Marks    | Grade |
| -------- | ----- |
| 90-100   | A     |
| 80-89    | B     |
| 70-79    | C     |
| 60-69    | D     |
| Below 60 | Fail  |

### Example:

```python
marks = int(input("Enter Marks: "))

if marks >= 90:
    print("Grade A")
elif marks >= 80:
    print("Grade B")
elif marks >= 70:
    print("Grade C")
elif marks >= 60:
    print("Grade D")
else:
    print("Fail")
```

---

## Task 3: Find the Largest of Three Numbers

### Question:

Take three numbers from the user and display the largest number.

```python
a = int(input("Enter First Number: "))
b = int(input("Enter Second Number: "))
c = int(input("Enter Third Number: "))

if a > b and a > c:
    print("Largest:", a)
elif b > c:
    print("Largest:", b)
else:
    print("Largest:", c)
```

---

## Task 4: Login System

### Question:

Create a login system.

* Username = admin
* Password = 1234

```python
username = input("Enter Username: ")
password = input("Enter Password: ")

if username == "admin" and password == "1234":
    print("Login Successful")
elif username != "admin":
    print("Invalid Username")
else:
    print("Invalid Password")
```

---

## Task 5: Electricity Bill Category

### Question:

Check electricity usage category.

* Less than 100 units → Low Usage
* 100 to 300 units → Medium Usage
* Above 300 units → High Usage

```python
units = int(input("Enter Units: "))

if units < 100:
    print("Low Usage")
elif units <= 300:
    print("Medium Usage")
else:
    print("High Usage")
```

---

## Task 6: Age Eligibility Checker

### Question:

Check whether a person is:

* Child (0-12)
* Teenager (13-19)
* Adult (20-59)
* Senior Citizen (60+)

```python
age = int(input("Enter Age: "))

if age <= 12:
    print("Child")
elif age <= 19:
    print("Teenager")
elif age <= 59:
    print("Adult")
else:
    print("Senior Citizen")
```

---

## Task 7: ATM Withdrawal

### Question:

Assume account balance is ₹10,000.

* If withdrawal amount is less than balance → Withdrawal Successful
* If equal to balance → Account Empty
* Otherwise → Insufficient Balance

```python
balance = 10000
amount = int(input("Enter Withdrawal Amount: "))

if amount < balance:
    print("Withdrawal Successful")
elif amount == balance:
    print("Account Empty")
else:
    print("Insufficient Balance")
```

---

## Task 8: Simple Calculator

### Question:

Take two numbers and an operator (`+`, `-`, `*`, `/`) from the user and perform the operation.

```python
num1 = float(input("Enter First Number: "))
num2 = float(input("Enter Second Number: "))
op = input("Enter Operator (+,-,*,/): ")

if op == "+":
    print("Result:", num1 + num2)
elif op == "-":
    print("Result:", num1 - num2)
elif op == "*":
    print("Result:", num1 * num2)
elif op == "/":
    print("Result:", num1 / num2)
else:
    print("Invalid Operator")
```

---

# 🎯 Advanced Task

### Student Result Management System

Take:

* Student Name
* Marks in 5 Subjects

Calculate:

* Total Marks
* Percentage
* Grade using `if-elif-else`

Rules:

* 90%+ → A+
* 80%+ → A
* 70%+ → B
* 60%+ → C
* Below 60% → Fail

Also display:

* "Eligible for Scholarship" if percentage ≥ 85
* Otherwise "Not Eligible"

This task combines:
✅ Variables
✅ User Input
✅ Arithmetic Operators
✅ `if-elif-else`
✅ Percentage Calculation
✅ Output Formatting
