# Python Task – NumPy 2D Arrays, Indexing & Slicing

## Task
Write a Python program using **NumPy** that demonstrates:

1. Creating a **2D array** with a specific **data type**.  
2. Accessing elements using **row & column indexing**.  
3. Extracting sub-arrays using **slicing**.  

---

## Requirements
1. Import **NumPy**.  

2. Create a **2D NumPy array**:

```

\[\[10, 20, 30],
\[40, 50, 60],
\[70, 80, 90]]

````
with data type = `float`.  

3. Print the **data type** of the array.  

4. Access and print:  
- The element at **row 0, column 1**.  
- The element at **last row, last column**.  

5. Slice and print:  
- The **first row**.  
- The **first two rows and first two columns**.  
- The **last column**.  

---

## Solution Code
```python
import numpy as np

# 1. Create a 2D NumPy array with float data type
arr = np.array([[10, 20, 30],
             [40, 50, 60],
             [70, 80, 90]], dtype=float)

print("Original Array:\n", arr)
print("Data Type:", arr.dtype)

# 2. Indexing
print("\nElement at row 0, col 1:", arr[0, 1])
print("Element at last row, last col:", arr[-1, -1])

# 3. Slicing
print("\nFirst Row:", arr[0, :])
print("First 2 Rows and First 2 Columns:\n", arr[:2, :2])
print("Last Column:", arr[:, -1])
````

---

##  Sample Output

```
Original Array:
 [[10. 20. 30.]
  [40. 50. 60.]
  [70. 80. 90.]]
Data Type: float64

Element at row 0, col 1: 20.0
Element at last row, last col: 90.0

First Row: [10. 20. 30.]
First 2 Rows and First 2 Columns:
 [[10. 20.]
  [40. 50.]]
Last Column: [30. 60. 90.]
```

---

✅ This task helps practice **NumPy 2D arrays**, including **indexing (row, col)** and **slicing sub-matrices**.
