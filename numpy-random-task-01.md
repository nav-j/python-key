# NumPy Random Functions – Practice Task

This task will help you practice **NumPy random functions**:

* `rand()` → generates random floats between 0 and 1
* `randint()` → generates random integers in a given range
* `choice()` → randomly selects elements from a list or array

---

## Task

### 1. Using `rand()`

* Create a **1D array of 5 random floats** between 0 and 1.
* Create a **2D array (3×3)** of random floats between 0 and 1.

---

### 2. Using `randint()`

* Generate **10 random integers** between 1 and 100.
* Generate a **2D array (2×5)** of random integers between 50 and 200.

---

### 3. Using `choice()`

* Randomly pick **5 elements** from the list `[10, 20, 30, 40, 50]`.
* Randomly pick **5 elements without replacement** from `[1, 2, 3, 4, 5, 6, 7, 8]`.

---

## ✅ Example Output

```
🎲 Using rand()
Random 1D floats: [0.123 0.567 0.876 0.234 0.678]
Random 2D floats:
 [[0.456 0.789 0.321]
  [0.654 0.234 0.912]
  [0.876 0.345 0.678]]

🎲 Using randint()
Random 10 integers: [23 98 12 55 78 44 67 88 91 15]
Random 2D integers:
 [[155 198 120  87 175]
  [ 65  90 150 199 180]]

🎲 Using choice()
Random choice (5 picks): [30 40 20 10 50]
Random choice without replacement: [6 2 8 4 5]
```

---

## Full Python Solution

```python
import numpy as np

# 1. rand() → random floats between 0 and 1
print("🎲 Using rand()")
rand_1d = np.random.rand(5)
print("Random 1D floats:", rand_1d)

rand_2d = np.random.rand(3, 3)
print("Random 2D floats:\n", rand_2d)

# 2. randint() → random integers
print("\n🎲 Using randint()")
rand_integers = np.random.randint(1, 101, size=10)  # 10 random integers between 1 and 100
print("Random 10 integers:", rand_integers)

rand_2d_int = np.random.randint(50, 201, size=(2, 5))  # 2x5 matrix
print("Random 2D integers:\n", rand_2d_int)

# 3. choice() → pick elements from a list/array
print("\n🎲 Using choice()")
choices1 = np.random.choice([10, 20, 30, 40, 50], size=5)
print("Random choice (5 picks):", choices1)

choices2 = np.random.choice([1, 2, 3, 4, 5, 6, 7, 8], size=5, replace=False)
print("Random choice without replacement:", choices2)
```

---

## Learning Goals

* Understand how to generate **random floats** using `rand()`.
* Learn how to generate **random integers** with `randint()`.
* Practice **sampling and shuffling data** using `choice()`.
