```markdown
# Python Task – Star Pattern

This beginner-friendly Python program prints a simple **star pattern** using loops.

---

## Task

Write a Python program that prints the following pattern:

```
*
**
***
****
*****
---

## 💡 Hints

- Use a **for loop** to control the number of rows.  
- In each iteration, print stars (`*`) equal to the row number.  
- Python allows string multiplication (`"*" * n`) to repeat characters easily.  
```
---
## ✅ Expected Output
*
**
***
****
*****
---
```
## 📝 Example Solution

```python
# Star Pattern Program

rows = 5  # number of rows

for i in range(1, rows + 1):
    print("*" * i)
````

---

## 🎯 Concepts Practiced

* **Loops** (`for`)
* **String multiplication**
* **Basic output formatting**

