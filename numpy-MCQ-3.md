## Python Objective Task – NumPy (Aggregation, Random, Joining & Splitting)

## Instructions

Each question has **one correct answer**.

---

### **Q1.** Which NumPy function returns the **sum of all elements** in an array?

A) `np.add(arr)`
B) `np.sum(arr)`
C) `np.total(arr)`
D) `arr.sumAll()`

---

### **Q2.** What will the following code print?

```python
import numpy as np
arr = np.array([2, 4, 6, 8])
print(arr.mean())
```

A) `4`
B) `5`
C) `6`
D) `20`

---

### **Q3.** Which function returns the **maximum value** of an array?

A) `arr.max()`
B) `np.maximum(arr)`
C) `np.max(arr)`
D) Both A and C

---

### **Q4.** Which of the following is used to generate a random integer between 1 and 10?

A) `np.random.randint(1, 10)`
B) `np.random.randint(10)`
C) `np.randint(1, 10)`
D) Both A and B

---

### **Q5.** What will this code output?

```python
import numpy as np
arr1 = np.array([1,2,3])
arr2 = np.array([4,5,6])
print(np.concatenate((arr1, arr2)))
```

A) `[1,2,3,4,5,6]`
B) `[[1,2,3],[4,5,6]]`
C) `[5,7,9]`
D) Error

---

### **Q6.** Which NumPy function stacks arrays horizontally (column-wise)?

A) `np.vstack()`
B) `np.hstack()`
C) `np.column_stack()`
D) Both B and C

---

### **Q7.** What will the following code print?

```python
import numpy as np
arr = np.array([1,2,3,4,5,6])
print(np.split(arr, 3))
```

A) `[array([1,2]), array([3,4]), array([5,6])]`
B) `[array([1,2,3]), array([4,5,6])]`
C) `[[1,2,3],[4,5,6]]`
D) Error

---

### **Q8.** Which function is used to get both **min and max values with their indices**?

A) `np.argminmax(arr)`
B) `np.where(arr)`
C) `np.argmin(arr), np.argmax(arr)`
D) `np.index(arr)`

# Answer Key – NumPy Advanced Objective Task

* **Q1 → B) `np.sum(arr)`**
  (`np.sum` returns the sum of all elements in the array.)

* **Q2 → B) `5`**
  (Mean of `[2,4,6,8]` → `(2+4+6+8)/4 = 20/4 = 5`.)

* **Q3 → D) Both A and C**
  (`arr.max()` and `np.max(arr)` both give maximum value.)

* **Q4 → A) `np.random.randint(1, 10)`**
  (Generates random integer between 1 and 9 inclusive. Option B starts from 0, so not equivalent.)

* **Q5 → A) `[1,2,3,4,5,6]`**
  (`np.concatenate` merges arrays into one.)

* **Q6 → D) Both B and C**
  (`np.hstack` and `np.column_stack` both stack arrays horizontally.)

* **Q7 → A) `[array([1,2]), array([3,4]), array([5,6])]`**
  (`np.split(arr, 3)` splits into 3 equal parts.)

* **Q8 → C) `np.argmin(arr), np.argmax(arr)`**
  (Returns indices of minimum and maximum values.)
