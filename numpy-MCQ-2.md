## Python Objective Task – NumPy (Indexing, Slicing & Reshaping)

## Instructions

Each question has **one correct answer**.

---

### **Q1.** What will the following code print?

```python
import numpy as np
arr = np.array([10, 20, 30, 40, 50])
print(arr[2])
```

A) `20`
B) `30`
C) `40`
D) `50`

---

### **Q2.** Which slicing expression extracts `[20, 30, 40]` from `arr = np.array([10, 20, 30, 40, 50])`?

A) `arr[1:4]`
B) `arr[0:3]`
C) `arr[2:5]`
D) `arr[:3]`

---

### **Q3.** What will be the output?

```python
import numpy as np
arr = np.array([[1,2,3],[4,5,6]])
print(arr[1,2])
```

A) `2`
B) `3`
C) `5`
D) `6`

---

### **Q4.** Which statement selects the **first column** of a 2D array `arr`?

A) `arr[:,0]`
B) `arr[0,:]`
C) `arr[1,:]`
D) `arr[:1]`

---

### **Q5.** What will `arr.reshape(2,3)` do to the following array?

```python
arr = np.array([1,2,3,4,5,6])
```

A) Creates a 2x3 matrix `[[1,2,3],[4,5,6]]`
B) Creates a 3x2 matrix `[[1,2],[3,4],[5,6]]`
C) Flattens the array
D) Throws an error

---

### **Q6.** What will the following code print?

```python
import numpy as np
arr = np.array([[1,2],[3,4],[5,6]])
print(arr[0:2,1])
```

A) `[1, 3]`
B) `[2, 4]`
C) `[3, 5]`
D) `[4, 6]`

---

### **Q7.** Which NumPy function converts a multi-dimensional array into a **1D array**?

A) `arr.flatten()`
B) `arr.reshape(1)`
C) `arr.squeeze()`
D) Both A and C

---

### **Q8.** If an array `arr` has shape `(2, 3, 4)`, what is its total number of elements?

A) `6`
B) `12`
C) `24`
D) `9`

---
 **Answer Key** 

# Answer Key – NumPy (Indexing, Slicing & Reshaping)

### Q1 → **B**

✔ `arr[2]` → element at index 2 → `30`.

### Q2 → **A**

✔ `arr[1:4]` → elements at index `1,2,3` → `[20, 30, 40]`.

### Q3 → **D**

✔ `arr[1,2]` → row 1, col 2 → `6`.

### Q4 → **A**

✔ `arr[:,0]` → all rows, column 0 → first column.

### Q5 → **A**

✔ `arr.reshape(2,3)` → `[[1,2,3],[4,5,6]]`.

### Q6 → **B**

✔ `arr[0:2,1]` → column 1 values from row 0 & 1 → `[2, 4]`.

### Q7 → **D**

✔ Both `arr.flatten()` and `arr.squeeze()` can reduce dimensions, but flatten explicitly gives 1D.

### Q8 → **C**

✔ `(2*3*4) = 24` elements in total.
