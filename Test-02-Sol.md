# ✅ Solution: Python Test Assignment

## Topic: Variables, Type Casting, Operators, Lists & List Methods

---

# Part A – Theory Answers

### Q1. What is a variable in Python?

A variable is a name used to store data in memory.

**Example:**

```python
name = "Aman"
```

---

### Q2. What is type casting?

Type casting is the process of converting one data type into another.

**Example:**

```python
age = "25"
age = int(age)
```

---

### Q3. Difference between `int()`, `float()`, and `str()`

| Function  | Purpose                          |
| --------- | -------------------------------- |
| `int()`   | Converts value to integer        |
| `float()` | Converts value to decimal number |
| `str()`   | Converts value to string         |

---

### Q4. Output

```python
x = 10
y = 5

print(x + y)
print(x * y)
```

Output:

```text
15
50
```

---

### Q5. What are Arithmetic Operators?

Arithmetic operators are used to perform mathematical calculations.

Examples:

* `+` Addition
* `-` Subtraction
* `*` Multiplication
* `/` Division

---

### Q6. Difference between `==` and `=`

| Operator | Purpose             |
| -------- | ------------------- |
| `=`      | Assignment operator |
| `==`     | Comparison operator |

Example:

```python
x = 10      # Assign value
print(x == 10)   # Compare value
```

---

### Q7. What is a List?

A List is an ordered and mutable collection of items.

Example:

```python
fruits = ["Apple", "Banana", "Mango"]
```

---

### Q8. Any Four List Methods

* `append()`
* `insert()`
* `remove()`
* `sort()`

---

### Q9. Output

```python
numbers = [10, 20, 30]
numbers.append(40)

print(numbers)
```

Output:

```python
[10, 20, 30, 40]
```

---

### Q10. Explain the Code

```python
fruits = ["Apple", "Banana", "Mango"]

fruits.remove("Banana")

print(fruits)
```

**Answer:**
The `remove()` method deletes `"Banana"` from the list.

Output:

```python
['Apple', 'Mango']
```

---

# Part B – Practical Solution

```python
# =====================================
# Student Fee Management System
# =====================================

# Step 1: Variables and Type Casting

student_name = input("Enter Student Name: ")
course_name = input("Enter Course Name: ")

fee = float(input("Enter Course Fee: "))
paid = float(input("Enter Amount Paid: "))

# =====================================
# Step 2: Operators
# =====================================

remaining_fee = fee - paid
paid_percentage = (paid / fee) * 100

# =====================================
# Step 3: Create List
# =====================================

subjects = []

for i in range(1, 6):
    subject = input(f"Enter Subject {i}: ")
    subjects.append(subject)

# =====================================
# Step 4: Display List
# =====================================

print("\nComplete List:", subjects)
print("First Subject:", subjects[0])
print("Last Subject:", subjects[-1])

# =====================================
# Step 5: List Methods
# =====================================

subjects.append("Python")
print("\nAfter append():", subjects)

subjects.insert(1, "AI")
print("After insert():", subjects)

remove_subject = input("Enter subject to remove: ")

if remove_subject in subjects:
    subjects.remove(remove_subject)

print("After remove():", subjects)

subjects.sort()
print("After sort():", subjects)

subjects.reverse()
print("After reverse():", subjects)

# =====================================
# Step 6: Search Subject
# =====================================

search_subject = input("\nEnter subject to search: ")

if search_subject in subjects:
    print("Subject Found")
else:
    print("Subject Not Found")

# =====================================
# Step 7: Final Report
# =====================================

print("\n========== FINAL REPORT ==========")

print("Student Name:", student_name)
print("Course Name:", course_name)
print("Course Fee:", fee)
print("Amount Paid:", paid)
print("Remaining Fee:", remaining_fee)
print("Paid Percentage:", round(paid_percentage, 2), "%")
print("Final Subject List:", subjects)

# =====================================
# Bonus Challenge
# =====================================

marks = [85, 90, 78, 92, 88]

print("\n========== MARKS REPORT ==========")

print("Highest Mark:", max(marks))
print("Lowest Mark:", min(marks))
print("Total Marks:", sum(marks))
print("Average Marks:", sum(marks) / len(marks))
```

---

## Sample Output

```text
Enter Student Name: Aman
Enter Course Name: Python
Enter Course Fee: 12000
Enter Amount Paid: 10000

Enter Subject 1: HTML
Enter Subject 2: CSS
Enter Subject 3: JavaScript
Enter Subject 4: Python
Enter Subject 5: SQL

Complete List: ['HTML', 'CSS', 'JavaScript', 'Python', 'SQL']
First Subject: HTML
Last Subject: SQL

After append(): ['HTML', 'CSS', 'JavaScript', 'Python', 'SQL', 'Python']
After insert(): ['HTML', 'AI', 'CSS', 'JavaScript', 'Python', 'SQL', 'Python']

========== FINAL REPORT ==========
Student Name: Aman
Course Name: Python
Course Fee: 12000.0
Amount Paid: 10000.0
Remaining Fee: 2000.0
Paid Percentage: 83.33 %
```

### Concepts Used

✔ Variables
✔ User Input
✔ Type Casting (`float()`)
✔ Arithmetic Operators (`+`, `-`, `*`, `/`)
✔ Lists
✔ List Methods (`append`, `insert`, `remove`, `sort`, `reverse`)
✔ Membership Operator (`in`)
✔ Conditional Statements (`if-else`)
✔ Loops (`for`)
✔ Built-in Functions (`max`, `min`, `sum`, `len`)
