# Python Practice Task - Arithmetic Calculator

This is a simple Python practice task to understand and use **arithmetic operators**.

---

## Task Description

Write a Python program that:

1. Takes **two numbers** as input from the user.
2. Performs the following **arithmetic operations** and prints results:

   - Addition (`+`)
   - Subtraction (`-`)
   - Multiplication (`*`)
   - Division (`/`)
   - Modulus (`%`)
   - Exponent (`**`)
   - Floor Division (`//`)

---

## Example Output

```

Enter first number: 15
Enter second number: 4

Arithmetic Operations:
15 + 4 = 19
15 - 4 = 11
15 \* 4 = 60
15 / 4 = 3.75
15 % 4 = 3
15 \*\* 4 = 50625
15 // 4 = 3

````

---

## Solution Code

```python
# Arithmetic Calculator in Python

# Taking input from user
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

print("\nArithmetic Operations:")

# Addition
print(f"{num1} + {num2} = {num1 + num2}")

# Subtraction
print(f"{num1} - {num2} = {num1 - num2}")

# Multiplication
print(f"{num1} * {num2} = {num1 * num2}")

# Division
print(f"{num1} / {num2} = {num1 / num2}")

# Modulus
print(f"{num1} % {num2} = {num1 % num2}")

# Exponent
print(f"{num1} ** {num2} = {num1 ** num2}")

# Floor Division
print(f"{num1} // {num2} = {num1 // num2}")
````

---
