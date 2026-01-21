# Python Practice Task  

## Task: Dynamic Reverse Pyramid Pattern  

###  Problem Statement  
Write a Python program that prints a **reverse pyramid pattern** of stars (`*`) based on the number of rows entered by the user.  

- The number of stars **decreases** each row.  
- The stars are aligned in the center by adding spaces before them.  

---

### Example Output  

#### For 3 rows:
```
```
*****
 *** 
  *
```
```

#### For 5 rows:
```
```
********* 
 ******* 
  ***** 
   *** 
    *
```
````

### Starter Code  

```python
# Take number of rows from user
rows = int(input("Enter number of rows: "))

for i in range(rows):
    # Print leading spaces
    print(" " * i, end="")
    # Print stars (formula makes it odd numbers: 2*rows-1, 2*rows-3, ...)
    print("*" * (2 * (rows - i) - 1))
````

---

### Hint

* Use `" " * i` to shift stars to the right.
* Use `"*" * (2 * (rows - i) - 1)` to print stars in decreasing odd sequence.
