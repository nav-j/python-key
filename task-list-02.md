# Python Task – List Methods Practice

## Task
Write a Python program to **demonstrate different list methods** step by step.

---

## Requirements

1. Create a list of numbers and a list of strings.
2. Perform the following operations:
   - `append()` → Add a new element at the end.
   - `insert()` → Add an element at a specific index.
   - `extend()` → Combine two lists.
   - `remove()` → Remove a specific element.
   - `pop()` → Remove element by index.
   - `sort()` → Sort numbers in ascending order.
   - `reverse()` → Reverse the list.
   - `clear()` → Remove all elements.

---

## Solution Code

```python
# Python List Methods Task

# 1. Create a list of numbers and strings
numbers = [10, 20, 30, 40]
fruits = ["apple", "banana"]

print("Original numbers:", numbers)

# 2. append() → Add element at the end
numbers.append(50)
print("After append:", numbers)

# 3. insert() → Add element at a specific index
numbers.insert(1, 15)   # insert 15 at index 1
print("After insert:", numbers)

# 4. extend() → Combine two lists
numbers.extend(fruits)
print("After extend:", numbers)

# 5. remove() → Remove a specific element
numbers.remove(40)
print("After remove:", numbers)

# 6. pop() → Remove element by index
numbers.pop(2)   # remove element at index 2
print("After pop:", numbers)

# 9. sort() → Sort numbers in ascending order (only numbers part)
num_only = [10, 50, 30, 15]   # extract numbers
num_only.sort()
print("Sorted numbers:", num_only)

# 10. reverse() → Reverse the list
numbers.reverse()
print("Reversed:", numbers)

# 11. clear() → Remove all elements
numbers.clear()
print("After clear:", numbers)
````

---

## 🎯 Example Output

```
Original numbers: [10, 20, 30, 40]
After append: [10, 20, 30, 40, 50]
After insert: [10, 15, 20, 30, 40, 50]
After extend: [10, 15, 20, 30, 40, 50, 'apple', 'banana']
After remove: [10, 15, 20, 30, 50, 'apple', 'banana']
After pop: [10, 15, 30, 50, 'apple', 'banana']
Sorted numbers: [10, 15, 30, 50]
Reversed: ['banana', 'apple', 50, 30, 15, 10]
After clear: []
```

---

✅ This exercise helps you **master list operations in Python**.

