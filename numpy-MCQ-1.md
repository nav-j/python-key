Perfect 👍 I’ll convert your **NumPy test** into a nicely formatted **README.md** so it looks professional for students to practice.

---

````markdown
# 🧮 NumPy MCQ & Practice Test  

This test will help you practice the basics of **NumPy for Data Science**.  

---

## 📌 Questions  

### 1. What does NumPy stand for?  
- [ ] Number Picker  
- [ ] Numerical Platform  
- [x] Numerical Python  

---

### 2. What is the array object in NumPy called?  
- [x] ndarray  
- [ ] ar  
- [ ] numarr  

---

### 3. True or False. NumPy is an open source project and you can use it freely.  
- [x] True  
- [ ] False  

---

### 4. Consider the following array:  
```python
arr = np.array([[1, 2, 3], [4, 5, 6]])
````

How many dimensions does it have?

* [ ] 1
* [x] 2
* [ ] 3

---

### 5. Insert the correct method for creating a NumPy array.

```python
arr = np.array([1, 2, 3, 4, 5])
```

---

### 6. Insert the correct argument for creating a NumPy array with 2 dimensions.

```python
arr = np.array([1, 2, 3, 4], ndmin=2)
```

---

### 7. Insert the correct syntax for checking the number of dimensions of a NumPy array.

```python
arr = np.array([1, 2, 3, 4])
print(arr.ndim)
```

---

### 8. Consider the following code:

```python
import numpy as np
arr = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])
print(arr[1, 1, 0])
```

What will be the printed result?

* [ ] 1
* [ ] 3
* [x] 7
* [ ] 8

---

### 9. Insert the correct syntax for printing the first item in the array.

```python
arr = np.array([1, 2, 3, 4, 5])
print(arr[0])
```

---

### 10. Insert the correct syntax for printing the number 50 from the array.

```python
arr = np.array([10, 20, 30, 40, 50])
print(arr[4])
```

---

### 11. Insert the correct syntax for printing the number 50 from the array.

```python
arr = np.array([[10, 20, 30, 40], [50, 60, 70, 80]])
print(arr[1, 0])
```

---

### 12. Use negative index to print the last item in the array.

```python
arr = np.array([10, 20, 30, 40, 50])
print(arr[-1])
```

---

### 13. Consider the following code:

```python
import numpy as np
arr = np.array([1, 2, 3, 4, 5, 6, 7])
print(arr[:2])
```

What will be the printed result?

* [ ] \[1]
* [x] \[1 2]
* [ ] \[1 2 3]
* [ ] \[3 4 5 6 7]

---

### 14. Insert the correct slicing syntax to print everything from the 2nd to the 5th item.

```python
arr = np.array([10, 15, 20, 25, 30, 35, 40])
print(arr[1:5])
```

---

### 15. Insert the correct slicing syntax to print everything from the 3rd to the 5th item.

```python
arr = np.array([10, 15, 20, 25, 30, 35, 40])
print(arr[2:5])
```

---

### 16. Insert the correct slicing syntax to print every other item from the 2nd to the 5th item.

```python
arr = np.array([10, 15, 20, 25, 30, 35, 40])
print(arr[1:5:2])
```

---

### 17. Insert the correct slicing syntax to print every other item from the entire array.

```python
arr = np.array([10, 15, 20, 25, 30, 35, 40])
print(arr[::2])
```

---

### 18. Consider the following code:

```python
import numpy as np
arr = np.array([-1, 0, 1])
newarr = arr.astype(bool)
print(newarr)
```

What will be the printed result?

* [ ] \[ True True True]
* [x] \[ True False True]
* [ ] \[ False False True]
* [ ] \[ False True True]

---

### 19. Insert the correct NumPy syntax to print the data type of an array.

```python
arr = np.array([1, 2, 3, 4])
print(arr.dtype)
```

---

### 20. Insert the correct argument to specify that the array should be of type STRING.

```python
arr = np.array([1, 2, 3, 4], dtype='S')
```

---

### 21. Insert the correct method to change the data type to integer.

```python
arr = np.array([1.1, 2.1, 3.1])
newarr = arr.astype(int)
```

---

### 22. Consider the following code:

```python
import numpy as np
original_array = np.array([1, 2, 3])
x = original_array.copy()
x[0] = 5
print(original_array)
```

What will be the printed result?

* [x] \[1 2 3]
* [ ] \[5 2 3]

---

### 23. Use the correct method to make a copy of the array.

```python
arr = np.array([1, 2, 3, 4, 5])
x = arr.copy()
```

---

### 24. Use the correct method to make a view of the array.

```python
arr = np.array([1, 2, 3, 4, 5])
x = arr.view()
```

---

## ✅ Result

This test checks your understanding of:

* NumPy basics
* Array creation & attributes
* Indexing & slicing
* Data types & conversions
* Copy vs View in NumPy

---
