# Python Task – Enumerated Iteration Using `np.ndenumerate()`

## Task

Write a Python program that:

1. Creates a **2D NumPy array** with numbers from `1` to `6`.  
2. Iterates through the array using **`np.ndenumerate()`**.  
3. Prints each **index** and **value** during iteration.  

---

## Example Code

```python
import numpy as np

# Create a 2D array
arr = np.array([[1, 2, 3],
                [4, 5, 6]])

# Enumerated iteration using ndenumerate
print("Iterating with np.ndenumerate():")
for idx, val in np.ndenumerate(arr):
    print(f"Index {idx} -> Value {val}")
````

---

## 🎯 Expected Output

```
🔹 Iterating with np.ndenumerate():
Index (0, 0) -> Value 1
Index (0, 1) -> Value 2
Index (0, 2) -> Value 3
Index (1, 0) -> Value 4
Index (1, 1) -> Value 5
Index (1, 2) -> Value 6
