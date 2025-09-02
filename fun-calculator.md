```markdown
# Python Practice Task

## Task: Calculator using Functions

###  Problem Statement
Write a Python program that:

1. Defines the following functions:
   - `add(x, y)` → returns the sum of two numbers.  
   - `subtract(x, y)` → returns the difference of two numbers.  
   - `multiply(x, y)` → returns the product of two numbers.  
   - `divide(x, y)` → returns the division of two numbers (handle division by zero).  

2. In the `main()` function:
   - Ask the user to enter two numbers.  
   - Ask the user to choose an operation (`+`, `-`, `*`, `/`).  
   - Call the respective function and print the result.  

---
```
### 💻 Example Output
```

Enter first number: 12
Enter second number: 4
Choose operation (+, -, \*, /): \*

Result: 12 \* 4 = 48

```
````

---

### 📝 Starter Code
```python
# Function for addition
def add(x, y):
    return x + y

# Function for subtraction
def subtract(x, y):
    return x - y

# Function for multiplication
def multiply(x, y):
    return x * y

# Function for division
def divide(x, y):
    if y == 0:
        return "Error! Division by zero."
    return x / y

# Main function
def main():
    a = float(input("Enter first number: "))
    b = float(input("Enter second number: "))
    op = input("Choose operation (+, -, *, /): ")
    
    if op == '+':
        print(f"Result: {a} + {b} = {add(a, b)}")
    elif op == '-':
        print(f"Result: {a} - {b} = {subtract(a, b)}")
    elif op == '*':
        print(f"Result: {a} * {b} = {multiply(a, b)}")
    elif op == '/':
        print(f"Result: {a} / {b} = {divide(a, b)}")
    else:
        print("Invalid operation!")

# Run program
main()
````
### 🎯 Learning Outcome

* Understand how to **define and use functions** in Python.
* Learn to handle **basic arithmetic operations**.
* Practice **user input handling** and conditional statements.
* Learn to manage **error cases** (like division by zero).
