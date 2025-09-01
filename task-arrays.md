```markdown
#  Python Practice Task

## Task: Array Operations Playground

###  Problem Statement
Write a Python program that:

1. Starts with an **empty array**.  
2. Lets the user **perform operations** on the array using functions and built-in methods:  
   - `add_element(arr, value)` → use `.append()` to add an element at the end.  
   - `insert_element(arr, index, value)` → use `.insert()` to add at a specific position.  
   - `remove_element(arr, value)` → use `.remove()` to delete the first occurrence of a value.  
   - `pop_element(arr)` → use `.pop()` to remove the last element.  
   - `sort_array(arr)` → use `.sort()` to sort the array.  
   - `reverse_array(arr)` → use `.reverse()` to reverse the array.  

3. Print the updated array after each operation.  

---
```
### 💻 Example Output
```

Initial Array: \[]

Adding 10 → \[10]
Adding 5 → \[10, 5]
Inserting 7 at index 1 → \[10, 7, 5]
Removing 10 → \[7, 5]
Popping last element → \[7]
Adding 20, 3, 15 → \[7, 20, 3, 15]
Sorting → \[3, 7, 15, 20]
Reversing → \[20, 15, 7, 3]

````

---
```
### 📝 Starter Code
```python
# Functions using array methods
def add_element(arr, value):
    arr.append(value)

def insert_element(arr, index, value):
    arr.insert(index, value)

def remove_element(arr, value):
    if value in arr:
        arr.remove(value)

def pop_element(arr):
    if arr:
        arr.pop()

def sort_array(arr):
    arr.sort()

def reverse_array(arr):
    arr.reverse()

# Main function
def main():
    arr = []
    print("Initial Array:", arr)
    
    add_element(arr, 10)
    print("Adding 10 →", arr)
    
    add_element(arr, 5)
    print("Adding 5 →", arr)
    
    insert_element(arr, 1, 7)
    print("Inserting 7 at index 1 →", arr)
    
    remove_element(arr, 10)
    print("Removing 10 →", arr)
    
    pop_element(arr)
    print("Popping last element →", arr)
    
    add_element(arr, 20)
    add_element(arr, 3)
    add_element(arr, 15)
    print("Adding 20, 3, 15 →", arr)
    
    sort_array(arr)
    print("Sorting →", arr)
    
    reverse_array(arr)
    print("Reversing →", arr)

# Run program
main()
````
### 🎯 Learning Outcome

* Learn how to use **Python list methods**:
  `.append()`, `.insert()`, `.remove()`, `.pop()`, `.sort()`, `.reverse()`.
* Understand how arrays (lists) can be manipulated step by step.
* Strengthen problem-solving with **functions + array methods**.
