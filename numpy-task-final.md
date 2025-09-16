# Python Task – NumPy Basics

## Task  
Write a Python program that uses **NumPy** to perform basic mathematical and array operations.

---

##  Requirements  
1. Import the **NumPy** library.  
2. Create a **NumPy array** of numbers from `1 to 10`.  
3. Perform the following operations:  
   - Find the **sum, mean, max, and min** of the array.  
   - Multiply all elements by `2`.  
   - Create a **reshaped 2D array (2x5)** from the original array.  
---

## 💻 Solution Code  

```python
import numpy as np

# 1. Create a NumPy array of numbers from 1 to 10
arr = np.arange(1, 11)
print("Original Array:", arr)

# 2. Basic operations
print("Sum:", np.sum(arr))
print("Mean:", np.mean(arr))
print("Max:", np.max(arr))
print("Min:", np.min(arr))

# 3. Multiply all elements by 2
print("\nArray multiplied by 2:", arr * 2)

# 4. Reshape into 2x5
reshaped = arr.reshape(2, 5)
print("\nReshaped 2x5 Array:\n", reshaped)

# 5. Generate a random 3x3 array (values between 0 and 1)
rand_arr = np.random.rand(3, 3)
print("\nRandom 3x3 Array:\n", rand_arr)

# 6. Transpose of the random array
print("\nTranspose of Random Array:\n", rand_arr.T)
````

---

## 🎯 Sample Output (Example)

```
Original Array: [ 1  2  3  4  5  6  7  8  9 10 ]
Sum: 55
Mean: 5.5
Max: 10
Min: 1

Array multiplied by 2: [ 2  4  6  8 10 12 14 16 18 20 ]

Reshaped 2x5 Array:
[[ 1  2  3  4  5]
 [ 6  7  8  9 10]]

---

✅ This assignment introduces you to **NumPy basics** like array creation, reshaping, random generation, and mathematical operations.

