# Python Assignment Solution

## Topic: Operators, Lists, Tuples, and Sets

---

# Part A: Theory Solutions (25 Marks)

## Q1. What are Operators in Python? Explain any five types of operators with suitable examples. (5 Marks)

### Answer:

Operators are special symbols used to perform operations on variables and values.

### Types of Operators

| Operator Type | Example                 |
| ------------- | ----------------------- |
| Arithmetic    | `+`, `-`, `*`, `/`, `%` |
| Comparison    | `==`, `!=`, `>`, `<`    |
| Assignment    | `=`, `+=`, `-=`         |
| Logical       | `and`, `or`, `not`      |
| Membership    | `in`, `not in`          |

### Example:

```python
a = 10
b = 5

print(a + b)      # Arithmetic
print(a > b)      # Comparison
print(a == 10)    # Comparison
print(a > 5 and b < 10)   # Logical
print(10 in [10,20,30])   # Membership
```

---

# Q2. What is a List? Explain any five features of a list. (5 Marks)

### Answer:

A List is an ordered, mutable collection used to store multiple items.

### Features

1. Ordered collection.
2. Mutable (can be modified).
3. Allows duplicate values.
4. Can store different data types.
5. Indexed (starts from 0).

### Example

```python
students = ["Aman", "Rahul", "Simran"]
print(students)
```

---

# Q3. Write any five commonly used List methods with syntax and examples. (5 Marks)

| Method   | Description                       | Example                   |
| -------- | --------------------------------- | ------------------------- |
| append() | Adds an item at the end           | `list.append("AI")`       |
| insert() | Inserts item at specific position | `list.insert(1,"Python")` |
| remove() | Removes a specific item           | `list.remove("AI")`       |
| sort()   | Sorts the list                    | `list.sort()`             |
| pop()    | Removes item by index             | `list.pop()`              |

### Example

```python
courses = ["Excel", "Python"]

courses.append("AI")
courses.insert(1, "Power BI")
courses.remove("Excel")

print(courses)
```

---

# Q4. What is a Tuple? Explain any five characteristics of tuples. Why are tuples called immutable? (5 Marks)

### Answer

A Tuple is an ordered collection that cannot be modified after creation.

### Characteristics

1. Ordered.
2. Immutable.
3. Allows duplicate values.
4. Indexed.
5. Faster than lists.

### Why is it Immutable?

Once a tuple is created, its elements cannot be added, removed, or changed.

### Example

```python
subjects = ("Python", "Excel", "AI")
print(subjects)
```

---

# Q5. What is a Set? Explain the following operations with examples. (5 Marks)

### Answer

A Set is an unordered collection of unique elements.

### Union

```python
A = {1,2,3}
B = {3,4,5}

print(A | B)
```

Output

```text
{1,2,3,4,5}
```

### Intersection

```python
print(A & B)
```

Output

```text
{3}
```

### Difference

```python
print(A - B)
```

Output

```text
{1,2}
```

### Symmetric Difference

```python
print(A ^ B)
```

Output

```text
{1,2,4,5}
```

---

# Part B: Practical Solutions (25 Marks)

---

## Q6. Student Names Using List (5 Marks)

```python
students = []

for i in range(5):
    name = input(f"Enter Student {i+1}: ")
    students.append(name)

print("\nStudent List:", students)
print("First Student:", students[0])
print("Last Student:", students[-1])
print("Total Students:", len(students))
```

---

## Q7. List Methods (5 Marks)

```python
students = ["Aman", "Rahul", "Simran", "Priya", "Karan"]

students.append("Neha")

students.insert(1, "Rohit")

students.remove("Rahul")

students.sort()

print("Updated Student List")
print(students)
```

---

## Q8. Marks Calculation Using Operators (6 Marks)

```python
m1 = float(input("Enter marks of Subject 1: "))
m2 = float(input("Enter marks of Subject 2: "))
m3 = float(input("Enter marks of Subject 3: "))

total = m1 + m2 + m3
average = total / 3
percentage = (total / 300) * 100

print("\nTotal Marks:", total)
print("Average Marks:", average)
print("Percentage:", percentage)

if percentage >= 40:
    print("Result: Pass")
else:
    print("Result: Fail")
```

---

## Q9. Tuple Operations (4 Marks)

```python
subjects = ("Python", "Excel", "Power BI", "AI", "SQL")

print("Subjects:", subjects)

print("First Subject:", subjects[0])

print("Last Subject:", subjects[-1])

print("Total Subjects:", len(subjects))

if "Python" in subjects:
    print("Python is available in the tuple.")
else:
    print("Python is not available.")
```

---

## Q10. Set Operations (5 Marks)

```python
morning = {"Aman", "Simran", "Rahul", "Priya"}

evening = {"Rahul", "Karan", "Simran", "Neha"}

print("Unique Students:")
print(morning | evening)

print("\nCommon Students:")
print(morning & evening)

print("\nOnly Morning Batch:")
print(morning - evening)

print("\nOnly Evening Batch:")
print(evening - morning)

print("\nTotal Unique Students:")
print(len(morning | evening))
```

---

# Sample Output

```text
Enter Student 1: Aman
Enter Student 2: Rahul
Enter Student 3: Simran
Enter Student 4: Priya
Enter Student 5: Karan

Student List:
['Aman', 'Rahul', 'Simran', 'Priya', 'Karan']

First Student: Aman
Last Student: Karan
Total Students: 5

Updated Student List:
['Aman', 'Karan', 'Neha', 'Priya', 'Rohit', 'Simran']

Enter marks of Subject 1: 80
Enter marks of Subject 2: 75
Enter marks of Subject 3: 90

Total Marks: 245.0
Average Marks: 81.67
Percentage: 81.67
Result: Pass

Subjects:
('Python', 'Excel', 'Power BI', 'AI', 'SQL')

First Subject: Python
Last Subject: SQL
Total Subjects: 5
Python is available in the tuple.

Unique Students:
{'Aman', 'Simran', 'Rahul', 'Priya', 'Karan', 'Neha'}

Common Students:
{'Rahul', 'Simran'}

Only Morning Batch:
{'Aman', 'Priya'}

Only Evening Batch:
{'Karan', 'Neha'}

Total Unique Students:
6
```

This solution covers all the required concepts: **operators, lists, list methods, tuples, sets, loops, conditions, indexing, membership operators, and built-in functions**.
