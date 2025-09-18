# Final Task 2 – NumPy Arrays (Operations & Reshaping)

## Task

Write a Python program that demonstrates the following **NumPy operations**:

1. **Array Creation & Reshaping**
   - Create a 1D array with numbers from **1 to 12**.
   - Reshape it into a **3x4 matrix**.

2. **Indexing & Slicing**
   - Print the **2nd row**.
   - Print the **last column**.
   - Slice the sub-matrix:

     ```
     [[5, 6],
      [9, 10]]
     ```

3. **Mathematical Operations**
   - Multiply the whole matrix by **2**.
   - Add another matrix of the same shape.
   - Perform element-wise multiplication.

4. **Aggregation Functions**
   - Find the **sum**, **mean**, and **max** of the array.
   - Find the **sum along axis=0** and **axis=1**.

5. **Splitting Arrays**
   - Split the matrix into **2 equal parts column-wise**.
   - Split the matrix into **3 equal parts row-wise**.

---

## 💻 Example Code

```python
import numpy as np

# 1. Array Creation & Reshaping
arr = np.arange(1, 13)   # 1 to 12
matrix = arr.reshape(3, 4)
print("Matrix:\n", matrix)

# 2. Indexing & Slicing
print("\n2nd row:", matrix[1])
print("Last column:", matrix[:, -1])
print("Sub-matrix:\n", matrix[1:3, 0:2])

# 3. Mathematical Operations
print("\nMatrix multiplied by 2:\n", matrix * 2)

other_matrix = np.array([[1, 1, 1, 1],
                         [2, 2, 2, 2],
                         [3, 3, 3, 3]])

print("Matrix + other_matrix:\n", matrix + other_matrix)
print("Element-wise multiplication:\n", matrix * other_matrix)

# 4. Aggregation Functions
print("\nSum of all elements:", np.sum(matrix))
print("Mean of all elements:", np.mean(matrix))
print("Max value:", np.max(matrix))
print("Sum along axis=0 (columns):", np.sum(matrix, axis=0))
print("Sum along axis=1 (rows):", np.sum(matrix, axis=1))

# 5. Splitting Arrays
row_split = np.split(matrix, 3, axis=0)
col_split = np.split(matrix, 2, axis=1)

print("\nRow-wise split:")
for part in row_split:
    print(part)

print("\nColumn-wise split:")
for part in col_split:
    print(part)
````

---

## Expected Output 

```
Matrix:
 [[ 1  2  3  4]
  [ 5  6  7  8]
  [ 9 10 11 12]]

2nd row: [5 6 7 8]
Last column: [ 4  8 12]
Sub-matrix:
 [[ 5  6]
  [ 9 10]]

Matrix multiplied by 2:
 [[ 2  4  6  8]
  [10 12 14 16]
  [18 20 22 24]]

Matrix + other_matrix:
 [[ 2  3  4  5]
  [ 7  8  9 10]
  [12 13 14 15]]

Element-wise multiplication:
 [[ 1  2  3  4]
  [10 12 14 16]
  [27 30 33 36]]

Sum of all elements: 78
Mean of all elements: 6.5
Max value: 12
Sum along axis=0 (columns): [15 18 21 24]
Sum along axis=1 (rows): [10 26 42]

Row-wise split:
 [[1 2 3 4]]
 [[5 6 7 8]]
 [[ 9 10 11 12]]

Column-wise split:
 [[1 2]
  [5 6]
  [9 10]]
 [[ 3  4]
  [ 7  8]
  [11 12]]
```

---

✅ This **Final Task 2** gives a full revision of:

* **Reshaping**
* **Indexing & slicing**
* **Mathematical operations**
* **Aggregation**
* **Splitting arrays**

---
