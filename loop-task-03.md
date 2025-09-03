```markdown
#  Python Practice Task  

## Task: Upright Pyramid Pattern  

### 📌 Problem Statement  
Write a Python program that prints an **upright pyramid pattern** of stars (`*`) based on the number of rows entered by the user.  

- The number of stars increases with each row.  
- Each row is centered using spaces.  

---

### ✅ Example Output  

#### For 3 rows:
```
```
  * 
 *** 
***** 
```
```
#### For 5 rows:
```

```
    *
   ***
  *****
 *******
*********

````

---

### 📝 Starter Code  

```python
# Take number of rows from user
rows = int(input("Enter number of rows: "))

for i in range(rows):
    # Print leading spaces (decreases each row)
    print(" " * (rows - i - 1), end="")
    # Print stars (increases each row: 1, 3, 5, ...)
    print("*" * (2 * i + 1))
````

---

### 💡 Hint

* Use `" " * (rows - i - 1)` to add spaces before stars.
* Use `"*" * (2 * i + 1)` to print stars in odd sequence (1, 3, 5, …).
