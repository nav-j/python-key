# ✅ Solution: Python Assignment (Theory + Practical)

---

# Part A – Theory Answers

### Q1. What is a List in Python?

A List is an ordered and mutable collection of items.

**Example:**

```python
fruits = ["apple", "banana", "mango"]
```

---

### Q2. What is the difference between a List and a Tuple?

| List                     | Tuple                         |
| ------------------------ | ----------------------------- |
| Mutable (can be changed) | Immutable (cannot be changed) |
| Uses `[]` brackets       | Uses `()` brackets            |

---

### Q3. What is a Set in Python?

A Set is an unordered collection of unique elements.

**Example:**

```python
numbers = {10, 20, 30}
```

**Use:** Removes duplicate values automatically.

---

### Q4. What is a Dictionary?

A Dictionary stores data in key-value pairs.

**Example:**

```python
student = {
    "name": "Aman",
    "roll_no": 101
}
```

---

### Q5. What is the purpose of the `range()` function?

The `range()` function generates a sequence of numbers.

**Example:**

```python
for i in range(1, 6):
    print(i)
```

Output:

```python
1
2
3
4
5
```

---

### Q6. Difference between `for` loop and `while` loop

| For Loop                                | While Loop                              |
| --------------------------------------- | --------------------------------------- |
| Used when number of iterations is known | Used when condition controls repetition |
| Simpler for sequences                   | More flexible                           |

---

### Q7. What is a Function in Python?

A Function is a block of reusable code that performs a specific task.

**Example:**

```python
def greet():
    print("Hello")
```

---

### Q8. Output

```python
numbers = [10, 20, 30]

for num in numbers:
    print(num)
```

Output:

```python
10
20
30
```

---

### Q9. Difference between `append()` and `add()`

| append()              | add()                |
| --------------------- | -------------------- |
| Used with Lists       | Used with Sets       |
| Adds one item to list | Adds one item to set |

Example:

```python
mylist.append(10)
myset.add(10)
```

---

### Q10. Explain the Code

```python
student = {
    "name": "Aman",
    "course": "Python"
}

for key, value in student.items():
    print(key, value)
```

**Answer:**
The code creates a dictionary and uses a `for` loop with `.items()` to display all keys and values.

Output:

```python
name Aman
course Python
```

---

# Part B – Practical Solution

```python
# ====================================
# Student Information Dictionary
# ====================================

name = input("Enter Student Name: ")
roll_no = int(input("Enter Roll Number: "))
course = input("Enter Course Name: ")

student = {
    "name": name,
    "roll_no": roll_no,
    "course": course
}

# ====================================
# Marks List using range()
# ====================================

marks = []

for i in range(1, 6):
    mark = int(input(f"Enter Marks for Subject {i}: "))
    marks.append(mark)

# ====================================
# Tuple Operations
# ====================================

marks_tuple = tuple(marks)

print("\n--- Tuple Operations ---")
print("First Mark:", marks_tuple[0])
print("Last Mark:", marks_tuple[-1])
print("First 3 Marks:", marks_tuple[:3])

# ====================================
# Set Operations
# ====================================

unique_marks = set(marks_tuple)

print("\nUnique Marks:", unique_marks)

# ====================================
# Functions
# ====================================

def total_marks(marks):
    return sum(marks)

def average_marks(marks):
    return sum(marks) / len(marks)

def highest_mark(marks):
    return max(marks)

def lowest_mark(marks):
    return min(marks)

def pass_fail(marks):
    avg = average_marks(marks)

    if avg >= 40:
        return "Pass"
    else:
        return "Fail"

# ====================================
# Function Calls
# ====================================

print("\n--- Marks Analysis ---")
print("Total Marks:", total_marks(marks_tuple))
print("Average Marks:", average_marks(marks_tuple))
print("Highest Mark:", highest_mark(marks_tuple))
print("Lowest Mark:", lowest_mark(marks_tuple))

# ====================================
# For Loop
# ====================================

print("\nMarks Using For Loop:")

for mark in marks_tuple:
    print(mark)

# ====================================
# While Loop
# ====================================

print("\nMarks Using While Loop:")

i = 0

while i < len(marks_tuple):
    print(marks_tuple[i])
    i += 1

# ====================================
# Grade Analysis
# ====================================

a = b = c = d = 0

for mark in marks_tuple:

    if mark >= 90:
        a += 1

    elif mark >= 80:
        b += 1

    elif mark >= 70:
        c += 1

    else:
        d += 1

print("\n--- Grade Summary ---")
print("A Grade:", a)
print("B Grade:", b)
print("C Grade:", c)
print("D Grade:", d)

# ====================================
# Search Marks
# ====================================

search = int(input("\nEnter Mark to Search: "))

if search in marks_tuple:
    print("Mark Found")
else:
    print("Mark Not Found")

# ====================================
# Display Dictionary
# ====================================

print("\n--- Student Information ---")

for key, value in student.items():
    print(key, ":", value)

# ====================================
# Pass / Fail Result
# ====================================

print("\nFinal Result:", pass_fail(marks_tuple))
```

### Sample Output

```text
Enter Student Name: Aman
Enter Roll Number: 101
Enter Course Name: Python

Enter Marks for Subject 1: 85
Enter Marks for Subject 2: 90
Enter Marks for Subject 3: 78
Enter Marks for Subject 4: 92
Enter Marks for Subject 5: 88

Total Marks: 433
Average Marks: 86.6
Highest Mark: 92
Lowest Mark: 78

A Grade: 2
B Grade: 2
C Grade: 1
D Grade: 0

Final Result: Pass
```
