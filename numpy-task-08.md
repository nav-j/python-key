# Python Task – NumPy Joining Arrays (`concatenate` & `stack`)

## Task

Write a Python program that demonstrates joining arrays using **`np.concatenate()`** and **`np.stack()`**:

1. Create two **1D arrays**:

   ```
   [1, 2, 3]
   [4, 5, 6]
   ```

   * Join them using `np.concatenate()`.
   * Stack them using `np.stack()` along different axes.

2. Create two **2D arrays**:

   ```
   [[1, 2], [3, 4]]
   [[5, 6], [7, 8]]
   ```

   * Join along **axis=0** and **axis=1** using `np.concatenate()`.
   * Stack them along **axis=0** and **axis=1** using `np.stack()`.

---

## Example Code

```python
import numpy as np

# 1. Create 1D arrays
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])

# Concatenate 1D arrays
joined_1D = np.concatenate((arr1, arr2))
print("Concatenated 1D Array:", joined_1D)

# Stack 1D arrays
stacked_axis0 = np.stack((arr1, arr2), axis=0)
stacked_axis1 = np.stack((arr1, arr2), axis=1)
print("\nStacked 1D Arrays (axis=0):\n", stacked_axis0)
print("\nStacked 1D Arrays (axis=1):\n", stacked_axis1)

# 2. Create 2D arrays
arr3 = np.array([[1, 2], [3, 4]])
arr4 = np.array([[5, 6], [7, 8]])

# Concatenate 2D arrays
joined_axis0 = np.concatenate((arr3, arr4), axis=0)
joined_axis1 = np.concatenate((arr3, arr4), axis=1)
print("\nConcatenated 2D Array (axis=0):\n", joined_axis0)
print("\nConcatenated 2D Array (axis=1):\n", joined_axis1)

# Stack 2D arrays
stacked_axis0_2D = np.stack((arr3, arr4), axis=0)
stacked_axis1_2D = np.stack((arr3, arr4), axis=1)
print("\nStacked 2D Arrays (axis=0):\n", stacked_axis0_2D)
print("\nStacked 2D Arrays (axis=1):\n", stacked_axis1_2D)
```

---

## Expected Output

```
Concatenated 1D Array: [1 2 3 4 5 6]

Stacked 1D Arrays (axis=0):
 [[1 2 3]
  [4 5 6]]

Stacked 1D Arrays (axis=1):
 [[1 4]
  [2 5]
  [3 6]]

Concatenated 2D Array (axis=0):
 [[1 2]
  [3 4]
  [5 6]
  [7 8]]

Concatenated 2D Array (axis=1):
 [[1 2 5 6]
  [3 4 7 8]]

Stacked 2D Arrays (axis=0):
 [[[1 2]
   [3 4]]

  [[5 6]
   [7 8]]]

Stacked 2D Arrays (axis=1):
 [[[1 2]
   [5 6]]

  [[3 4]
   [7 8]]]
```

---

✅ This task shows the difference between **`concatenate()`** (merges along existing axes) and **`stack()`** (creates a new dimension).
