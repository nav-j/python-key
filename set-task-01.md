# Python Sets – Task & Solution
This exercise covers **set creation, updating, removing, and performing set operations** in Python.

## Task

1. **Create a Set**

   * Create a set named `fruits` with values: `"apple"`, `"banana"`, `"cherry"`.
   * Print the set.

2. **Add Elements**

   * Add `"mango"` to the set.
   * Add multiple elements `"orange"` and `"grapes"` at once.

3. **Remove Elements**

   * Remove `"banana"` using `.remove()`.
   * Try removing `"kiwi"` safely using `.discard()`.

4. **Set Operations**

   * Create another set `tropical = {"mango", "papaya", "pineapple"}`.
   * Perform the following:

     * **Union** of `fruits` and `tropical`.
     * **Intersection** of `fruits` and `tropical`.
     * **Difference** between `fruits` and `tropical`.

5. **Set Methods**

   * Find the length of `fruits`.
   * Clear all elements from `tropical`.

---

##  Solution

```python
# 1. Create a Set
fruits = {"apple", "banana", "cherry"}
print("Initial fruits set:", fruits)

# 2. Add Elements
fruits.add("mango")
print("After adding mango:", fruits)

fruits.update(["orange", "grapes"])
print("After adding multiple:", fruits)

# 3. Remove Elements
fruits.remove("banana")  # will throw error if not present
print("After removing banana:", fruits)

fruits.discard("kiwi")   # safe, no error if not present
print("After discarding kiwi (no error):", fruits)

# 4. Set Operations
tropical = {"mango", "papaya", "pineapple"}

print("Union:", fruits.union(tropical))
print("Intersection:", fruits.intersection(tropical))
print("Difference:", fruits.difference(tropical))

# 5. Set Methods
print("Length of fruits:", len(fruits))

tropical.clear()
print("Tropical after clear:", tropical)
```

---

## 🖥️ Sample Output

```
Initial fruits set: {'apple', 'banana', 'cherry'}
After adding mango: {'apple', 'banana', 'cherry', 'mango'}
After adding multiple: {'apple', 'grapes', 'banana', 'cherry', 'mango', 'orange'}
After removing banana: {'apple', 'grapes', 'cherry', 'mango', 'orange'}
After discarding kiwi (no error): {'apple', 'grapes', 'cherry', 'mango', 'orange'}

Union: {'apple', 'grapes', 'cherry', 'mango', 'orange', 'papaya', 'pineapple'}
Intersection: {'mango'}
Difference: {'apple', 'grapes', 'cherry', 'orange'}

Length of fruits: 5
Tropical after clear: set()
```

---

##  Concepts Covered

✔ Set creation
✔ Adding elements (`add`, `update`)
✔ Removing elements (`remove`, `discard`)
✔ Union, Intersection, Difference
✔ Membership test (`in`)
✔ Length of set
✔ Clearing a set
