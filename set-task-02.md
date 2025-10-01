# Python Sets – Task 2
## Objective

Practice **mathematical set operations, iteration, and frozen sets** in Python.

---

## Task

1. **Create Sets**

   * Create two sets:

     * `A = {1, 2, 3, 4, 5}`
     * `B = {4, 5, 6, 7, 8}`

2. **Mathematical Operations**

   * Find the **union** of A and B.
   * Find the **intersection** of A and B.
   * Find the **difference** (A − B).
   * Find the **symmetric difference** of A and B.

3. **Iteration**

   * Loop through set `A` and print each element.

---

## ✅ Solution

```python
# 1. Create Sets
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}

print("Set A:", A)
print("Set B:", B)

# 2. Mathematical Operations
print("\nUnion of A and B:", A.union(B))
print("Intersection of A and B:", A.intersection(B))
print("Difference (A - B):", A.difference(B))
print("Symmetric Difference:", A.symmetric_difference(B))

# 3. Iteration
print("\nIterating over set A:")
for item in A:
    print(item)

```

---

## Sample Output

```
Set A: {1, 2, 3, 4, 5}
Set B: {4, 5, 6, 7, 8}

Union of A and B: {1, 2, 3, 4, 5, 6, 7, 8}
Intersection of A and B: {4, 5}
Difference (A - B): {1, 2, 3}
Symmetric Difference: {1, 2, 3, 6, 7, 8}

Iterating over set A:
1
2
3
4
5

```

---

## Concepts Covered

✔ Union, Intersection, Difference, Symmetric Difference
✔ Iterating over a set
✔ Frozen sets (immutable sets)
✔ Error handling with immutable collections
