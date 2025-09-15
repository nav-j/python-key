# Python Task – NumPy Arrays, Indexing & Slicing

## Task
Write a Python program using **NumPy** that demonstrates:

1. Creating arrays with a specific **data type**.  
2. Accessing elements using **indexing**.  
3. Extracting parts of the array using **slicing**.  

---

##  Requirements
1. Import **NumPy**.  
2. Create a **1D NumPy array** with values `[10, 20, 30, 40, 50]` and set its data type to `float`.  
3. Print the **data type** of the array.  
4. Access and print:  
   - The **first element**.  
   - The **last element**.  
5. Slice and print:  
   - The first **three elements**.  
   - The last **two elements**.  
   - Elements from index `1` to `3`.  

---

## Solution Code
```python
import numpy as np

# 1. Create a 1D NumPy array with float data type
arr = np.array([10, 20, 30, 40, 50], dtype=float)
print("Original Array:", arr)
print("Data Type:", arr.dtype)

# 2. Indexing
print("\nFirst Element:", arr[0])
print("Last Element:", arr[-1])

# 3. Slicing
print("\nFirst 3 Elements:", arr[:3])
print("Last 2 Elements:", arr[-2:])
print("Elements from index 1 to 3:", arr[1:4])
````

---

## Sample Output

```
Original Array: [10. 20. 30. 40. 50.]
Data Type: float64

First Element: 10.0
Last Element: 50.0

First 3 Elements: [10. 20. 30.]
Last 2 Elements: [40. 50.]
Elements from index 1 to 3: [20. 30. 40.]
```

---

✅ This task helps practice **NumPy array basics**, including **data types, indexing, and slicing**.
