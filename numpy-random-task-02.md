# NumPy Random – Permutation & Shuffle Task

This task will help you practice **NumPy’s permutation and shuffle functions**, which are commonly used in **data sampling, randomization, and machine learning preprocessing**.

---

## Task

### 1. Using `np.random.permutation()`
- Generate a permutation of numbers from **0 to 9**.
- Generate a permutation of the array `[10, 20, 30, 40, 50]`.
- Show that the **original array is not changed**.

---

### 2. Using `np.random.shuffle()`
- Create a **1D array `[1, 2, 3, 4, 5]`** and shuffle it.
- Create a **2D array (3×3)** and shuffle it **row-wise**.
- Show that the **original array gets modified**.

---

## ✅ Example Output

```

🎲 Using permutation()
Permutation of 0–9: \[4 8 1 6 9 0 2 3 7 5]
Permutation of \[10 20 30 40 50]: \[20 40 50 10 30]
Original array after permutation: \[10 20 30 40 50]

🎲 Using shuffle()
Shuffled 1D array: \[3 5 2 1 4]
Shuffled 2D array:
\[\[ 7  8  9]
\[ 1  2  3]
\[ 4  5  6]]

````

---

## Full Python Solution

```python
import numpy as np

# 1. Using permutation()
print("🎲 Using permutation()")

# Permutation of numbers 0–9
perm1 = np.random.permutation(10)
print("Permutation of 0–9:", perm1)

# Permutation of a given array
arr = np.array([10, 20, 30, 40, 50])
perm2 = np.random.permutation(arr)
print("Permutation of [10,20,30,40,50]:", perm2)

# Original array remains unchanged
print("Original array after permutation:", arr)

# 2. Using shuffle()
print("\n🎲 Using shuffle()")

# Shuffle a 1D array
arr1 = np.array([1, 2, 3, 4, 5])
np.random.shuffle(arr1)
print("Shuffled 1D array:", arr1)

# Shuffle a 2D array row-wise
arr2 = np.array([[1, 2, 3],
                 [4, 5, 6],
                 [7, 8, 9]])
np.random.shuffle(arr2)
print("Shuffled 2D array (row-wise):\n", arr2)
````

---

## Learning Goals

* Understand the difference between **`permutation()`** and **`shuffle()`**.
* Learn how **`permutation()`** returns a new array while **`shuffle()`** modifies the original array.
* Practice **1D and 2D array randomization**.
  
