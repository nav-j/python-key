# Python Task – NumPy Joining Arrays

## Task

Write a Python program that demonstrates how to **join arrays** in NumPy:

1. Create two **1D arrays**:

   ```
   [1, 2, 3]
   [4, 5, 6]
   ```
2. Join them using `np.concatenate()`.
3. Create two **2D arrays**:

   ```
   [[1, 2], [3, 4]]
   [[5, 6], [7, 8]]
   ```
4. Join them:

   * Along **axis=0** (row-wise).
   * Along **axis=1** (column-wise).

---

## Example Code

```python
import numpy as np

# 1. Create 1D arrays
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])

# Join 1D arrays
joined_1D = np.concatenate((arr1, arr2))
print("Joined 1D Array:", joined_1D)

# 2. Create 2D arrays
arr3 = np.array([[1, 2], [3, 4]])
arr4 = np.array([[5, 6], [7, 8]])

# Join along axis 0 (row-wise)
joined_axis0 = np.concatenate((arr3, arr4), axis=0)
print("\nJoined 2D Array (axis=0):\n", joined_axis0)

# Join along axis 1 (column-wise)
joined_axis1 = np.concatenate((arr3, arr4), axis=1)
print("\nJoined 2D Array (axis=1):\n", joined_axis1)
```

---

## Expected Output

```
Joined 1D Array: [1 2 3 4 5 6]

Joined 2D Array (axis=0):
 [[1 2]
  [3 4]
  [5 6]
  [7 8]]

Joined 2D Array (axis=1):
 [[1 2 5 6]
  [3 4 7 8]]
```

---

✅ This task helps practice **joining NumPy arrays** for both **1D and 2D arrays** using `np.concatenate()`.
