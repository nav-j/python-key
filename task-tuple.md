# 📘 Python Tuple Practice – Tasks & Solutions

## 🔹 Task 1: Basic Tuple Operations

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

### ✅ Solution

```python
fruits = ("apple", "banana", "cherry", "apple", "mango", "banana")

print("First fruit:", fruits[0])
print("Last fruit:", fruits[-1])

print("Count of 'apple':", fruits.count("apple"))
print("Index of 'cherry':", fruits.index("cherry"))

print("First three fruits:", fruits[:3])

new_tuple = fruits + ("grape", "kiwi")
print("After concatenation:", new_tuple)

repeated_tuple = fruits * 2
print("After repetition:", repeated_tuple)

fruits_list = list(fruits)
fruits_list.append("orange")
fruits = tuple(fruits_list)
print("After adding 'orange':", fruits)
```

---

## 🔹 Task 2: Access, Update & Unpack Tuples

### Problem

Given:

```python
student = ("Alice", 21, "Computer Science", "Delhi")
```

1. Print **name** and **city**.
2. Convert to list, change age → `22`, add `"Python"`, convert back to tuple.
3. Unpack into variables and print each separately.

### ✅ Solution

```python
student = ("Alice", 21, "Computer Science", "Delhi")

print("Name:", student[0])
print("City:", student[-1])

student_list = list(student)
student_list[1] = 22
student_list.append("Python")
student = tuple(student_list)
print("Updated tuple:", student)

name, age, branch, city, subject = student
print("Name:", name)
print("Age:", age)
print("Branch:", branch)
print("City:", city)
print("Subject:", subject)
```

---

## 🔹 Task 3: Loop, Join & Multiply Tuples

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

### ✅ Solution

```python
numbers = (1, 2, 3, 4, 5)
letters = ("A", "B", "C")

print("Numbers (for loop):")
for n in numbers:
    print(n)

print("\nLetters (while loop):")
i = 0
while i < len(letters):
    print(letters[i])
    i += 1

joined = numbers + letters
print("\nJoined tuple:", joined)

print("Letters repeated 3 times:", letters * 3)
print("Numbers repeated 2 times:", numbers * 2)
```

---

## 🔹 Task 4: Challenge – Mastering Tuples

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

### ✅ Solution

```python
student = ("Alice", 21, "Computer Science", "Delhi")
marks = (85, 90, 78, 92, 88)

print("Student Name:", student[0])
print("Student City:", student[-1])
print("First Mark:", marks[0])
print("Last Mark:", marks[-1])

student_list = list(student)
student_list[1] = 22
student_list.append("Python")
student = tuple(student_list)
print("\nUpdated Student Tuple:", student)

name, age, branch, city, subject = student
print("\nUnpacked:")
print("Name:", name)
print("Age:", age)
print("Branch:", branch)
print("City:", city)
print("Subject:", subject)

print("\nMarks with for loop:")
for m in marks:
    print(m)

print("\nCharacters in name with while loop:")
i = 0
while i < len(name):
    print(name[i])
    i += 1

profile = student + marks
print("\nProfile (joined tuple):", profile)

print("Marks repeated twice:", marks * 2)
print("Python repeated 3 times:", ("Python",) * 3)
```

---

✅ This single file covers:

* Accessing
* Updating
* Unpacking
* Looping (`for` + `while`)
* Joining
* Multiplying
