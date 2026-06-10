#  Python Tuple Practice 

##  Task 1: Basic Tuple Operations

### Problem

You are given the following tuple:

```python
fruits = ("apple", "banana", "cherry", "apple", "mango", "banana")
```

Perform these tasks:

1. Access first and last fruit.
2. Print the first 3 fruits as a new tuple.
3. Concatenate with `("grape", "kiwi")`.
4. Repeat the tuple twice.
5. Convert to list, add `"orange"`, then convert back to tuple.



##  Task 2: Access, Update & Unpack Tuples

### Problem

Given:

```python
student = ("Alice", 21, "Computer Science", "Delhi")
```

1. Print **name** and **city**.
2. Convert to list, change age → `22`, add `"Python"`, convert back to tuple.
3. Unpack into variables and print each separately.

## Task 3: Loop, Join & Multiply Tuples

### Problem

Given:

```python
numbers = (1, 2, 3, 4, 5)
letters = ("A", "B", "C")
```

1. Print all numbers using `for` loop.
2. Print all letters using `while` loop.
3. Join the two tuples.
4. Repeat `letters` 3 times and `numbers` 2 times.

## Task 4: Challenge – Mastering Tuples

### Problem

Given:

```python
student = ("Alice", 21, "Computer Science", "Delhi")
marks = (85, 90, 78, 92, 88)
```

Perform:

1. Access `student` name & city, first & last marks.
2. Update age → `22`, add `"Python"`.
3. Unpack `student` into variables.
4. Loop: print marks (`for` loop), print characters of name (`while` loop).
5. Join student & marks into one tuple.
6. Repeat `marks` twice, repeat `("Python",)` three times.


# ✅ Solutions: Python Tuple Practice

---

# Task 1: Basic Tuple Operations

```python
# Given Tuple
fruits = ("apple", "banana", "cherry", "apple", "mango", "banana")

# 1. Access first and last fruit
print("First Fruit:", fruits[0])
print("Last Fruit:", fruits[-1])

# 2. Print first 3 fruits
print("First 3 Fruits:", fruits[:3])

# 3. Concatenate with another tuple
new_fruits = fruits + ("grape", "kiwi")
print("After Concatenation:", new_fruits)

# 4. Repeat tuple twice
print("Repeated Tuple:", fruits * 2)

# 5. Convert to list, add orange, convert back to tuple
fruit_list = list(fruits)
fruit_list.append("orange")

fruits = tuple(fruit_list)

print("Updated Tuple:", fruits)
```

---

# Task 2: Access, Update & Unpack Tuples

```python
# Given Tuple
student = ("Alice", 21, "Computer Science", "Delhi")

# 1. Print name and city
print("Name:", student[0])
print("City:", student[3])

# 2. Update age and add Python
student_list = list(student)

student_list[1] = 22
student_list.append("Python")

student = tuple(student_list)

print("Updated Student Tuple:")
print(student)

# 3. Unpack tuple
name, age, course, city, skill = student

print("\nUnpacked Values:")
print("Name:", name)
print("Age:", age)
print("Course:", course)
print("City:", city)
print("Skill:", skill)
```

---

# Task 3: Loop, Join & Multiply Tuples

```python
# Given Tuples
numbers = (1, 2, 3, 4, 5)
letters = ("A", "B", "C")

# 1. Print numbers using for loop
print("Numbers:")

for num in numbers:
    print(num)

# 2. Print letters using while loop
print("\nLetters:")

i = 0

while i < len(letters):
    print(letters[i])
    i += 1

# 3. Join tuples
joined_tuple = numbers + letters

print("\nJoined Tuple:")
print(joined_tuple)

# 4. Repeat tuples
print("\nLetters Repeated 3 Times:")
print(letters * 3)

print("\nNumbers Repeated 2 Times:")
print(numbers * 2)
```

---

# Task 4: Challenge – Mastering Tuples

```python
# Given Tuples
student = ("Alice", 21, "Computer Science", "Delhi")
marks = (85, 90, 78, 92, 88)

# 1. Access name, city, first and last marks
print("Name:", student[0])
print("City:", student[3])

print("First Mark:", marks[0])
print("Last Mark:", marks[-1])

# 2. Update age and add Python
student_list = list(student)

student_list[1] = 22
student_list.append("Python")

student = tuple(student_list)

print("\nUpdated Student:")
print(student)

# 3. Unpack student tuple
name, age, course, city, skill = student

print("\nUnpacked Values")
print("Name:", name)
print("Age:", age)
print("Course:", course)
print("City:", city)
print("Skill:", skill)

# 4. Loop Marks (for loop)
print("\nMarks:")

for mark in marks:
    print(mark)

# Print characters of name (while loop)
print("\nCharacters in Name:")

i = 0

while i < len(name):
    print(name[i])
    i += 1

# 5. Join student and marks
combined = student + marks

print("\nCombined Tuple:")
print(combined)

# 6. Repeat tuples
print("\nMarks Repeated Twice:")
print(marks * 2)

print("\nPython Repeated Three Times:")
print(("Python",) * 3)
```
