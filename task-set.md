# Python Practice Task - Set Operations Playground

A beginner-friendly Python practice task to explore **set operations**.

---

## Task Description

Write a Python program that:

1. Takes **two sets of numbers** as input from the user (entered in one line, separated by spaces).
2. Performs the following **set operations**:
   - **Union** → All unique elements from both sets.
   - **Intersection** → Common elements in both sets.
   - **Difference** → Elements present in the first set but not in the second.
   - **Symmetric Difference** → Elements in either set but not both.

---

## Example Run

```

Enter first set (numbers separated by space): 1 2 3 4
Enter second set (numbers separated by space): 3 4 5 6

\--- Results ---
Union: {1, 2, 3, 4, 5, 6}
Intersection: {3, 4}
Difference (First - Second): {1, 2}
Symmetric Difference: {1, 2, 5, 6}

````

---

## Solution Code

```python
# Set Operations Playground

# Taking input from user
first_set = set(map(int, input("Enter first set (numbers separated by space): ").split()))
second_set = set(map(int, input("Enter second set (numbers separated by space): ").split()))

# Performing set operations
print("\n--- Results ---")
print("Union:", first_set | second_set)
print("Intersection:", first_set & second_set)
print("Difference (First - Second):", first_set - second_set)
print("Symmetric Difference:", first_set ^ second_set)
````

---

##  Learning Outcome

* Understand the concept of **sets** in Python.
* Practice basic **set operations**: union, intersection, difference, and symmetric difference.
* Learn how sets automatically remove duplicate elements.

