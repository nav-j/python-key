# Python Task – Number Pattern

This Python program prints a simple **number pattern** using loops.

---

## Task

Write a Python program that prints the following pattern:

```
```
1
12
123
1234
12345

```
```
---

## Hints

- Use a **for loop** to control the number of rows.  
- Inside the loop, use another **for loop** (or string join) to print numbers from **1 to i**.  
- Use `end=""` in the `print()` function so the numbers appear **side by side**.  

---

## Expected Output

```
```
1
12
123
1234
12345
```
````

---

## Example Solution

```python
# Number Pattern Program

rows = 5  # number of rows

for i in range(1, rows + 1):
    for j in range(1, i + 1):
        print(j, end="")
    print()
````

---

## Concepts Practiced

* **Nested loops** (`for` inside another `for`)
* **Number sequence printing**
* **Using `end=""` in print statements**

---

✅ A great exercise to strengthen your understanding of **loops** and **pattern printing** in Python!
