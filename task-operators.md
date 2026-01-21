# Operator Playground

This is a simple Python practice program to learn and use different **operators** in Python.

---

##  Features

1. **Arithmetic Operators**
   - Perform addition, subtraction, multiplication, and division.

2. **Comparison Operators**
   - Compare two numbers to check if one is greater or if both are equal.

3. **Logical Operators**
   - Check if both numbers are positive (`and`).
   - Check if at least one number is positive (`or`).

4. **Assignment Operators**
   - Use `+=` and `*=` to update a variable.

5. **Membership Operators**
   - Check if a character (`"a"`) exists inside a word.

6. **Identity Operators**
   - Check if two numbers are the same object using `is`.

---

##  Program Code

```python
# Operator Playground

# Step 1: Input
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))
word = input("Enter a word: ")

# Step 2: Arithmetic Operators
print("\n--- Arithmetic ---")
print("Addition:", num1 + num2)
print("Subtraction:", num1 - num2)
print("Multiplication:", num1 * num2)
print("Division:", num1 / num2)

# Step 3: Comparison Operators
print("\n--- Comparison ---")
print("Is first > second?", num1 > num2)
print("Are both equal?", num1 == num2)

# Step 4: Logical Operators
print("\n--- Logical ---")
print("Both positive?", num1 > 0 and num2 > 0)
print("At least one positive?", num1 > 0 or num2 > 0)

# Step 5: Assignment Operators
print("\n--- Assignment ---")
result = num1
result += num2   # add second number
result *= 2      # multiply by 2
print("Result after += and *= :", result)

# Step 6: Membership Operators
print("\n--- Membership ---")
print("Is 'a' in word?", "a" in word)

# Step 7: Identity Operators
print("\n--- Identity ---")
print("Are both numbers same object?", num1 is num2)
````

---

##  Sample Run

```
Enter first number: 10
Enter second number: 5
Enter a word: apple

--- Arithmetic ---
Addition: 15
Subtraction: 5
Multiplication: 50
Division: 2.0

--- Comparison ---
Is first > second? True
Are both equal? False

--- Logical ---
Both positive? True
At least one positive? True

--- Assignment ---
Result after += and *= : 30

--- Membership ---
Is 'a' in word? True

--- Identity ---
Are both numbers same object? False
```

---

##  Learning Outcomes

* Understand and apply different **Python operators**:

  * Arithmetic
  * Comparison
  * Logical
  * Assignment
  * Membership
  * Identity

✅ A complete beginner exercise to practice Python operators.
