

````markdown
# 🐍 Simple Student Score Program

This is a beginner-friendly Python program that practices **input, string functions, list functions, and operators**.

---

## 📌 Features
1. **Input**
   - Takes student name and marks as input from the user.

2. **String Operations**
   - Converts the name to **uppercase**.
   - Displays the **first character** of the name.

3. **List Operations**
   - Stores marks in a list.
   - Finds the **sum** of marks.
   - Adds an extra mark using `append()`.

4. **Operators**
   - Calculates the **average** marks.
   - Checks if the student has **Passed or Failed** using a comparison operator.

---

## 📝 Program Code

```python
# Step 1: Input
name = input("Enter student name: ")
mark1 = int(input("Enter first mark: "))
mark2 = int(input("Enter second mark: "))
extra_mark = int(input("Enter one more mark: "))

# Step 2: String operations
print("\n--- String ---")
print("Uppercase:", name.upper())
print("First character:", name[0])

# Step 3: List operations
marks = [mark1, mark2]
print("\n--- List ---")
print("Marks list:", marks)
print("Sum:", sum(marks))

marks.append(extra_mark)  # add one more mark
print("After appending:", marks)

# Step 4: Operators
average = sum(marks) / len(marks)  # arithmetic
print("\n--- Operators ---")
print("Average:", average)

if average >= 40:   # comparison
    print("Result: Pass")
else:
    print("Result: Fail")
````

---

## 💻 Sample Run

```
Enter student name: Raj
Enter first mark: 35
Enter second mark: 45
Enter one more mark: 50

--- String ---
Uppercase: RAJ
First character: R

--- List ---
Marks list: [35, 45]
Sum: 80
After appending: [35, 45, 50]

--- Operators ---
Average: 43.33
Result: Pass
```

---

## 🎯 Learning Outcomes

* How to take **user input** in Python.
* Using **string functions** like `.upper()` and indexing.
* Performing **list operations** like `append()` and `sum()`.
* Using **arithmetic and comparison operators**.

---

✅ A simple but complete exercise to practice Python basics!


