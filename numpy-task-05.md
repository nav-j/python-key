# Python Task – Iteration in 3D NumPy Arrays

## Task

Write a Python program using **NumPy** that demonstrates **iteration in 3D arrays**:

1. Create a **3D array**.
2. Iterate over the **2D sub-arrays**.
3. Iterate over the **1D arrays** inside each 2D sub-array.
4. Iterate **element-wise** through the entire 3D array.

---

## Requirements

1. Import **NumPy**.
2. Create a **3D array** with the values:

```

\[
\[\[1, 2, 3], \[4, 5, 6]],
\[\[7, 8, 9], \[10, 11, 12]]
]

````

3. Print:
   - Each **2D array**.
   - Each **1D array** inside the 2D arrays.
   - Each **element** one by one.

---

## Solution Code

```python
import numpy as np

# 1. Create a 3D array
arr3D = np.array([
    [[1, 2, 3], [4, 5, 6]],
    [[7, 8, 9], [10, 11, 12]]
])

print("3D Array:\n", arr3D)

# 2. Iterate over 2D sub-arrays
print("\nIterating over 2D arrays:")
for two_d in arr3D:
    print(two_d)

# 3. Iterate over 1D arrays
print("\nIterating over 1D arrays inside each 2D array:")
for two_d in arr3D:
    for one_d in two_d:
        print(one_d)

# 4. Iterate element-wise
print("\nIterating element-wise through entire 3D array:")
for two_d in arr3D:
    for one_d in two_d:
        for elem in one_d:
            print(elem, end=" ")
````

---

## Sample Output

```
3D Array:
 [[[ 1  2  3]
  [ 4  5  6]]

 [[ 7  8  9]
  [10 11 12]]]

Iterating over 2D arrays:
[[1 2 3]
 [4 5 6]]
[[ 7  8  9]
 [10 11 12]]

Iterating over 1D arrays inside each 2D array:
[1 2 3]
[4 5 6]
[7 8 9]
[10 11 12]

Iterating element-wise through entire 3D array:
1 2 3 4 5 6 7 8 9 10 11 12
```

---

## ✅ Learning Outcome

This task helps practice **iteration at multiple levels** in a **3D NumPy array**:

* **2D arrays (matrices)**
* **1D arrays (rows)**
* **Individual elements**
