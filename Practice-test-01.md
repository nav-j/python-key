## Python Test

### Student Name: ___________

### Date: ___________

### Total Marks: 40

---

## Part A – Theory

### Q1. What is a variable in Python? Give one example. (2 Marks)

### Q2. What is the difference between `int`, `float`, `str`, and `bool` data types? (3 Marks)

| Data Type | Description | Example |
| --------- | ----------- | ------- |
| int       |             |         |
| float     |             |         |
| str       |             |         |
| bool      |             |         |


### Q3. What is the purpose of the `input()` function in Python? (2 Marks)

### Q4. What is List and Tuple? Differentiate between List and Tuple. (5 Marks)

| Feature           | List | Tuple |
| ----------------- | ---- | ----- |
| Syntax            |      |       |
| Mutable/Immutable |      |       |
| Example           |      |       |

### Q5. Write the output of the following code: (3 Marks)

```python
x = 10
y = 5.5

print(type(x))
print(type(y))
```

Output:

### Q6. Fill in the blanks: (4 Marks)

1. A list is enclosed within __________.
2. A tuple is enclosed within __________.
3. The function used to take input from a user is __________.
4. `True` and `False` belong to the __________ data type.

### Q7. What are Operators? Explain its types.(5 Marks)

## Part B – Practical

### Scenario:

Create a **Student Information System** using Python.

### Requirements:

### Task 1: User Input & Variables (4 Marks)

Take the following inputs from the user:

* Student Name
* Roll Number
* Age
* Course

Store them in variables and print all the values.

Example Output:

```python
Enter Name: Your Name
```
### Task 2: Data Types (3 Marks)

Display the data type of each variable using:

Example Output:

```
Name Data Type: <class 'str'>
Age Data Type: <class 'int'>
```
### Task 3: Create a List (4 Marks)

Ask the user to enter marks of 3 subjects.

Store them in a list named `marks`.

Example:

```python
marks = [78, 85, 90]
```

Perform the following:

1. Print all marks.
2. Print highest mark.
3. Print lowest mark.
4. Print total marks.

### Task 4: Create a Tuple (4 Marks)

Create a tuple named `subjects`.

```python
subjects = ("Python", "Web Development", "Database")
```

Perform the following:

1. Print all subjects.
2. Print the first subject.
3. Print the last subject.
4. Count total subjects.

### Task 5: List Operations (4 Marks)

Perform these operations on the `marks` list:

1. Add one more mark using `append()`.
2. Remove a mark using `remove()`.
3. Sort the list.
4. Display the updated list.

### Task 6: Final Student Report (5 Marks)

Display all details in a formatted report:

Example Output:

```
========== STUDENT REPORT ==========
Name        : Rahul
Roll Number : 101
Age         : 20
Course      : B.Tech

Subjects    : ('Python', 'Web Development', 'Database')
Marks       : [78, 85, 90]

Highest Mark: 90
Lowest Mark : 78
Total Marks : 253
====================================
```
# Bonus Challenge  (2 Marks)

1. Calculate the average of all marks.
2. Display whether the student has passed or failed.If average is >=40 then Pass otherwise Fail.
