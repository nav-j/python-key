
````markdown
# Python Lambda Function Example

This example shows the difference between a **normal function** (using `def`) and a **lambda function** in Python.

---

## Code Example

```python
# Normal function
def add(x, y):
    return x + y

# Lambda function (same thing)
add_lambda = lambda x, y: x + y

print(add_lambda(5, 3))  # Output: 8
````

---

## Explanation

* **Normal function (`def`)**
  A named function defined using the `def` keyword.

  ```python
  def add(x, y):
      return x + y
  ```

* **Lambda function (`lambda`)**
  An anonymous (nameless) function defined in a single line.

  ```python
  add_lambda = lambda x, y: x + y
  ```

Both return the same result when called:

```python
add_lambda(5, 3)  # ➝ 8
```

---

## ✅ Key Points

* `def` → Used for larger, reusable, and complex functions.
* `lambda` → Best for short, one-time, inline functions.
* Expression after `:` is automatically **returned** in a `lambda`.

---

## 🎯 Output

```
8
```
