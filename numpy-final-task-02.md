## Python Task – Ultimate NumPy Operations Practice

## Task

Write a Python program using **NumPy** that demonstrates:

1. Creating **1D and 2D arrays**  
2. Accessing elements using **indexing**  
3. Extracting elements using **slicing**  
4. Checking and converting **data types**  
5. **Reshaping** arrays  
6. **Enumerated iteration** using `np.ndenumerate()`  
7. **Joining arrays** with `concatenate` and `stack`  
8. **Splitting arrays** with `split`  
9. **Searching** elements using `np.where()` and `np.searchsorted()`  
10. **Sorting** arrays with `np.sort()`  

---

## ✅ Requirements

1. Import **NumPy**.  
2. Create a **1D array** `[15, 5, 25, 10, 20, 30]`.  
3. Create a **2D array**:  

   ```python
   [[7, 8, 9],
    [4, 5, 6]]
````

4. Perform the following operations:

* **Indexing**: Print the 2nd element of the 1D array and the element at row=0, col=2 of the 2D array.
* **Slicing**: Extract `[5, 25, 10]` from the 1D array.
* **Data type**: Print the data type and convert the 1D array to `float`.
* **Reshape**: Convert the 1D array into a `2x3` 2D array.
* **Enumeration**: Use `np.ndenumerate()` on reshaped array to print indices and values.
* **Joining**:

  * Concatenate the 1D array with `[35, 40]`.
  * Stack arrays `[1, 2, 3]` and `[4, 5, 6]` along both axis 0 and 1.
* **Splitting**: Split the original 1D array into 3 equal parts.
* **Search**:

  * Find the indices where elements are equal to `10`.
  * Use `np.searchsorted()` to find the position of `18` in the sorted array.
* **Sort**:

  * Sort the 1D array in ascending order.
  * Sort each row of the 2D array.

---

##  Solution Code

```python
import numpy as np

# 1. Create arrays
arr1D = np.array([15, 5, 25, 10, 20, 30])
arr2D = np.array([[7, 8, 9],
                  [4, 5, 6]])

print("1D Array:", arr1D)
print("\n2D Array:\n", arr2D)

# 2. Indexing
print("\n2nd element of 1D array:", arr1D[1])
print("Element at row=0, col=2 of 2D array:", arr2D[0, 2])

# 3. Slicing
print("\nSliced 1D Array [5, 25, 10]:", arr1D[1:4])

# 4. Data type
print("\nData type of arr1D:", arr1D.dtype)
arr_float = arr1D.astype(float)
print("Converted to float:", arr_float)

# 5. Reshape
reshaped = arr1D.reshape(2, 3)
print("\nReshaped 2x3 Array:\n", reshaped)

# 6. Enumeration
print("\nEnumerating reshaped array:")
for idx, val in np.ndenumerate(reshaped):
    print(f"Index {idx} -> Value {val}")

# 7. Joining arrays
extra = np.array([35, 40])
joined = np.concatenate((arr1D, extra))
print("\nConcatenated 1D Array:", joined)

a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
stacked0 = np.stack((a, b), axis=0)
stacked1 = np.stack((a, b), axis=1)
print("\nStacked Arrays (axis=0):\n", stacked0)
print("Stacked Arrays (axis=1):\n", stacked1)

# 8. Splitting arrays
split_arrs = np.split(arr1D, 3)
print("\nSplitted 1D Array into 3 parts:")
for i, part in enumerate(split_arrs):
    print(f"Part {i+1}:", part)

# 9. Search
where_10 = np.where(arr1D == 10)
print("\nIndices where element=10:", where_10)

sorted_arr = np.sort(arr1D)
pos_18 = np.searchsorted(sorted_arr, 18)
print("Position to insert 18 in sorted array:", pos_18)

# 10. Sorting
print("\nSorted 1D Array:", sorted_arr)
print("Sorted 2D Array row-wise:\n", np.sort(arr2D))
```

---

## 🎯 Sample Output

```
1D Array: [15  5 25 10 20 30]

2D Array:
 [[7 8 9]
  [4 5 6]]

2nd element of 1D array: 5
Element at row=0, col=2 of 2D array: 9

Sliced 1D Array [5, 25, 10]: [ 5 25 10]

Data type of arr1D: int64
Converted to float: [15.  5. 25. 10. 20. 30.]

Reshaped 2x3 Array:
 [[15  5 25]
  [10 20 30]]

Enumerating reshaped array:
Index (0, 0) -> Value 15
Index (0, 1) -> Value 5
Index (0, 2) -> Value 25
Index (1, 0) -> Value 10
Index (1, 1) -> Value 20
Index (1, 2) -> Value 30

Concatenated 1D Array: [15  5 25 10 20 30 35 40]

Stacked Arrays (axis=0):
 [[1 2 3]
  [4 5 6]]
Stacked Arrays (axis=1):
 [[1 4]
  [2 5]
  [3 6]]

Splitted 1D Array into 3 parts:
Part 1: [15  5]
Part 2: [25 10]
Part 3: [20 30]

Indices where element=10: (array([3]),)
Position to insert 18 in sorted array: 3

Sorted 1D Array: [ 5 10 15 20 25 30]
Sorted 2D Array row-wise:
 [[7 8 9]
  [4 5 6]]
```

---

## 📘 Concepts Covered

✔ Array creation
✔ Indexing & slicing
✔ Data types & conversion
✔ Reshaping
✔ Enumeration with indices
✔ Joining & stacking
✔ Splitting arrays
✔ Searching with `where` and `searchsorted`
✔ Sorting arrays
