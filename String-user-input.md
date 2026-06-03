## 📝 Python String Functions Practice Task

### 🎯 Objective

Create a Python program that uses the following string functions and concepts:

* `format()`
* `center()`
* `partition()`
* `join()`
* Indexing
* Slicing
* `count()`
* `startswith()`
* `endswith()`

---

## 📌 Task: Student Information Formatter

Write a Python program that performs the following operations:

### 1. User Information

Ask the user to enter:

* Full Name
* Course Name
* City

Display the information using `format()`:

```text
Student Rahul Sharma is enrolled in Python Programming and lives in Ludhiana.
```

---

### 2. Center the Name

Print the student's name centered in 40 spaces using `*`.

Example:

```text
************Rahul Sharma************
```

---

### 3. Partition the Course Name

Use `partition()` to split the course name at the first space.

Example:

```text
Input: Python Programming

Output:
('Python', ' ', 'Programming')
```

---

### 4. Join Words

Create a list:

```python
["Learn", "Code", "Grow"]
```

Join the words using `" | "` as a separator.

Output:

```text
Learn | Code | Grow
```

---

### 5. Indexing and Slicing

Using the student's name:

Display:

* First character
* Last character
* First 5 characters
* Middle part (excluding first and last character)

Example:

```text
First Character : R
Last Character  : a
First 5 Chars   : Rahul
Middle Part     : ahul Sharm
```

---

### 6. Count Characters

Count how many times the letter `'a'` appears in the name.

Example:

```text
Number of 'a' : 3
```

---

### 7. Check Start and End

Check:

* Does the name start with `"R"`?
* Does the name end with `"a"`?

Example:

```text
Starts with R : True
Ends with a   : True
```

---

## Expected Sample Output

```text
Enter Full Name: Rahul Sharma
Enter Course Name: Python Programming
Enter City: Ludhiana

Student Rahul Sharma is enrolled in Python Programming and lives in Ludhiana.

*************Rahul Sharma*************

Course Partition:
('Python', ' ', 'Programming')

Joined String:
Learn | Code | Grow

First Character : R
Last Character  : a
First 5 Chars   : Rahul
Middle Part     : ahul Sharm

Number of 'a' : 3

Starts with R : True
Ends with a   : True
```
## Solution

```python
# Student Information Formatter

# Taking user input
name = input("Enter Full Name: ")
course = input("Enter Course Name: ")
city = input("Enter City: ")

# 1. Using format()
print("\nStudent {} is enrolled in {} and lives in {}.".format(name, course, city))

# 2. Using center()
print("\n" + name.center(40, "*"))

# 3. Using partition()
course_parts = course.partition(" ")
print("\nCourse Partition:")
print(course_parts)

# 4. Using join()
words = ["Learn", "Code", "Grow"]
joined_string = " | ".join(words)
print("\nJoined String:")
print(joined_string)

# 5. Using Indexing and Slicing
print("\nIndexing and Slicing:")
print("First Character :", name[0])
print("Last Character  :", name[-1])
print("First 5 Chars   :", name[:5])
print("Middle Part     :", name[1:-1])

# 6. Using count()
print("\nCount Function:")
print("Number of 'a' :", name.lower().count('a'))

# 7. Using startswith() and endswith()
print("\nStartswith and Endswith:")
print("Starts with R :", name.startswith('R'))
print("Ends with a   :", name.endswith('a'))
```

### Sample Run

```text
Enter Full Name: Rahul Sharma
Enter Course Name: Python Programming
Enter City: Ludhiana

Student Rahul Sharma is enrolled in Python Programming and lives in Ludhiana.

*************Rahul Sharma*************

Course Partition:
('Python', ' ', 'Programming')

Joined String:
Learn | Code | Grow

Indexing and Slicing:
First Character : R
Last Character  : a
First 5 Chars   : Rahul
Middle Part     : ahul Sharm

Count Function:
Number of 'a' : 3

Startswith and Endswith:
Starts with R : True
Ends with a   : True
```

This solution demonstrates:

* `input()`
* `format()`
* `center()`
* `partition()`
* `join()`
* String indexing (`[0]`, `[-1]`)
* String slicing (`[:5]`, `[1:-1]`)
* `count()`
* `startswith()`
* `endswith()`
