# 🐍 Python Test Assignment

## Topic: Variables, Type Casting, Operators, Lists & List Methods

**Student Name:** ___________________

**Date:** ___________________

**Total Marks:** 50

---

# Part A – Theory (20 Marks)

### Q1. What is a variable in Python? Give one example. (2 Marks)

---

### Q2. What is type casting? Explain with an example. (2 Marks)

---

### Q3. What is the difference between `int()`, `float()`, and `str()`? (2 Marks)

---

### Q4. Write the output of the following code: (2 Marks)

```python
x = 10
y = 5

print(x + y)
print(x * y)
```

---

### Q5. What are Arithmetic Operators? Name any four arithmetic operators. (2 Marks)

---

### Q6. What is the difference between `==` and `=` operators? (2 Marks)

---

### Q7. What is a List in Python? Write one example. (2 Marks)

---

### Q8. Name any four List Methods. (2 Marks)

---

### Q9. Write the output of the following code: (2 Marks)

```python
numbers = [10, 20, 30]
numbers.append(40)

print(numbers)
```

---

### Q10. Explain the following code: (2 Marks)

```python
fruits = ["Apple", "Banana", "Mango"]

fruits.remove("Banana")

print(fruits)
```

---

# Part B – Practical (30 Marks)

## Student Fee Management System

### Task Requirements

Create a Python program that performs the following operations:

---

### Step 1: Variables and Type Casting

Ask the user to enter:

* Student Name
* Course Name
* Course Fee
* Amount Paid

Convert fee and paid amount into numeric values using type casting.

---

### Step 2: Operators

Calculate:

* Remaining Fee
* Fee Paid Percentage

Using arithmetic operators.

Formula:

```python
remaining_fee = fee - paid
paid_percentage = (paid / fee) * 100
```

---

### Step 3: Create a List

Create an empty list named `subjects`.

Ask the user to enter 5 subject names and store them in the list using:

```python
append()
```

---

### Step 4: Display List

Display:

* Complete List
* First Subject
* Last Subject

---

### Step 5: List Methods

Perform the following operations:

1. Add `"Python"` using `append()`
2. Insert `"AI"` at index 1 using `insert()`
3. Remove a subject entered by the user using `remove()`
4. Sort the list using `sort()`
5. Reverse the list using `reverse()`

Display the list after each operation.

---

### Step 6: Search Subject

Ask the user to enter a subject name.

Check whether the subject exists in the list using:

```python
in
```

Display:

```text
Subject Found
```

or

```text
Subject Not Found
```

---

### Step 7: Display Final Report

Display:

```text
Student Name
Course Name
Course Fee
Amount Paid
Remaining Fee
Paid Percentage
Final Subject List
```

---

# Bonus Challenge (5 Marks)

Create another list containing marks:

```python
marks = [85, 90, 78, 92, 88]
```

Display:

* Highest Mark
* Lowest Mark
* Total Marks
* Average Marks

using:

```python
max()
min()
sum()
len()
```

---

## Marking Scheme

| Section   | Marks  |
| --------- | ------ |
| Theory    | 20     |
| Practical | 30     |
| Bonus     | 5      |
| **Total** | **55** |

### Topics Covered

✅ Variables
✅ Type Casting
✅ Arithmetic Operators
✅ Comparison Operators
✅ Lists
✅ List Indexing
✅ List Methods (`append`, `insert`, `remove`, `sort`, `reverse`)
✅ Membership Operator (`in`)
✅ Built-in Functions (`max`, `min`, `sum`, `len`)
