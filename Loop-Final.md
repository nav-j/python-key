There are **20 tasks plus 8 challenge tasks**. Providing complete solutions for all of them in one response would be extremely long.

I can provide them in parts:

### Part 1 (Tasks 1–5)

```python
# Task 1: Print Numbers from 1 to 10
for i in range(1, 11):
    print(i)
```

```python
# Task 2: Print Even Numbers from 1 to 50
for i in range(2, 51, 2):
    print(i)
```

```python
# Task 3: Multiplication Table
num = int(input("Enter a number: "))

for i in range(1, 11):
    print(f"{num} x {i} = {num * i}")
```

```python
# Task 4: Sum of First N Numbers
n = int(input("Enter a number: "))

total = 0
for i in range(1, n + 1):
    total += i

print("Sum =", total)
```

```python
# Task 5: Countdown
for i in range(10, 0, -1):
    print(i)

print("Blast Off!")
```

### Part 2 (Tasks 6–10)

```python
# Task 6: Factorial
num = int(input("Enter a number: "))

fact = 1
for i in range(1, num + 1):
    fact *= i

print("Factorial =", fact)
```

```python
# Task 7: Reverse a Number
num = int(input("Enter a number: "))
reverse = 0

while num > 0:
    digit = num % 10
    reverse = reverse * 10 + digit
    num //= 10

print("Reverse =", reverse)
```

```python
# Task 8: Count Digits
num = int(input("Enter a number: "))
count = 0

while num > 0:
    count += 1
    num //= 10

print("Digits =", count)
```

```python
# Task 9: Prime Number Check
num = int(input("Enter a number: "))

if num < 2:
    print("Not Prime")
else:
    prime = True

    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            prime = False
            break

    if prime:
        print("Prime Number")
    else:
        print("Not Prime")
```

```python
# Task 10: Fibonacci Series
n = int(input("How many terms? "))

a, b = 0, 1

for i in range(n):
    print(a, end=" ")
    a, b = b, a + b
```


## Part 3 (Tasks 11–15)

### Task 11: Number Guessing Game

```python
import random

secret = random.randint(1, 100)

while True:
    guess = int(input("Guess a number (1-100): "))

    if guess < secret:
        print("Too Low!")
    elif guess > secret:
        print("Too High!")
    else:
        print("🎉 Correct! You guessed the number.")
        break
```

---

## Task 12: Star Pattern

**Output**

```
*
**
***
****
*****
```

**Program**

```python
rows = 5

for i in range(1, rows + 1):
    for j in range(i):
        print("*", end="")
    print()
```

---

## Task 13: Inverted Star Pattern

**Output**

```
*****
****
***
**
*
```

**Program**

```python
rows = 5

for i in range(rows, 0, -1):
    for j in range(i):
        print("*", end="")
    print()
```

---

## Task 14: Pyramid Pattern

**Output**

```
    *
   ***
  *****
 *******
*********
```

**Program**

```python
rows = 5

for i in range(rows):
    # Print spaces
    for j in range(rows - i - 1):
        print(" ", end="")

    # Print stars
    for k in range(2 * i + 1):
        print("*", end="")

    print()
```

---

## Task 15: Login System (3 Attempts)

```python
correct_username = "admin"
correct_password = "1234"

attempts = 3

while attempts > 0:
    username = input("Enter Username: ")
    password = input("Enter Password: ")

    if username == correct_username and password == correct_password:
        print("✅ Login Successful")
        break
    else:
        attempts -= 1
        if attempts > 0:
            print("❌ Invalid Username or Password")
            print("Attempts Left:", attempts)
        else:
            print("🔒 Account Locked!")
```

### Sample Output

```
Enter Username: admin
Enter Password: 1111
❌ Invalid Username or Password
Attempts Left: 2

Enter Username: admin
Enter Password: 1234
✅ Login Successful
```


# Part 4 (Tasks 16–20)

---

## Task 16: ATM Menu Using `while` Loop

```python
balance = 5000

while True:
    print("\n====== ATM MENU ======")
    print("1. Check Balance")
    print("2. Deposit")
    print("3. Withdraw")
    print("4. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        print("Current Balance: ₹", balance)

    elif choice == 2:
        amount = float(input("Enter deposit amount: ₹"))
        balance += amount
        print("Deposit Successful!")
        print("Updated Balance: ₹", balance)

    elif choice == 3:
        amount = float(input("Enter withdrawal amount: ₹"))

        if amount <= balance:
            balance -= amount
            print("Withdrawal Successful!")
            print("Remaining Balance: ₹", balance)
        else:
            print("Insufficient Balance!")

    elif choice == 4:
        print("Thank you for using our ATM.")
        break

    else:
        print("Invalid Choice!")
```

---

# Task 17: Student Marks Calculator

```python
total = 0

for i in range(1, 6):
    marks = float(input(f"Enter marks of Subject {i}: "))
    total += marks

average = total / 5
percentage = (total / 500) * 100

print("\nTotal Marks:", total)
print("Average:", average)
print("Percentage:", percentage, "%")

if percentage >= 90:
    grade = "A+"
elif percentage >= 80:
    grade = "A"
elif percentage >= 70:
    grade = "B"
elif percentage >= 60:
    grade = "C"
elif percentage >= 50:
    grade = "D"
else:
    grade = "F"

print("Grade:", grade)
```

---

# Task 18: Password Strength Checker

```python
while True:
    password = input("Create Password: ")

    has_upper = False
    has_lower = False
    has_digit = False
    has_special = False

    for ch in password:
        if ch.isupper():
            has_upper = True
        elif ch.islower():
            has_lower = True
        elif ch.isdigit():
            has_digit = True
        else:
            has_special = True

    if (len(password) >= 8 and
        has_upper and
        has_lower and
        has_digit and
        has_special):

        print("Strong Password!")
        break

    else:
        print("Weak Password!")
        print("Password must contain:")
        print("- At least 8 characters")
        print("- One uppercase letter")
        print("- One lowercase letter")
        print("- One digit")
        print("- One special character")
```

---

# Task 19: Menu-Driven Calculator

```python
while True:
    print("\n===== Calculator =====")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exit")

    choice = int(input("Enter choice: "))

    if choice == 5:
        print("Calculator Closed.")
        break

    num1 = float(input("Enter First Number: "))
    num2 = float(input("Enter Second Number: "))

    if choice == 1:
        print("Result =", num1 + num2)

    elif choice == 2:
        print("Result =", num1 - num2)

    elif choice == 3:
        print("Result =", num1 * num2)

    elif choice == 4:
        if num2 != 0:
            print("Result =", num1 / num2)
        else:
            print("Division by Zero is not Allowed!")

    else:
        print("Invalid Choice!")
```

---

# Task 20: Quiz Game

```python
score = 0

questions = [
    ("What is the capital of India?", "Delhi"),
    ("Which language is used for AI and Data Science?", "Python"),
    ("How many continents are there?", "7"),
    ("What is 5 × 6?", "30"),
    ("Who developed Python?", "Guido van Rossum")
]

for question, answer in questions:
    user_answer = input(question + " : ")

    if user_answer.lower() == answer.lower():
        print("Correct!")
        score += 1
    else:
        print("Wrong! Correct Answer:", answer)

print("\n===== Quiz Completed =====")
print("Your Score:", score, "out of", len(questions))

percentage = (score / len(questions)) * 100
print("Percentage:", percentage, "%")

if percentage >= 80:
    print("Excellent!")
elif percentage >= 60:
    print("Good Job!")
elif percentage >= 40:
    print("Keep Practicing!")
else:
    print("Better Luck Next Time!")
```
