# Python Practice Task - List Manager

This is a beginner-friendly Python program to practice **list operations**.  
The program allows the user to input numbers and perform various list manipulations.

---

## Features

1. **Input**
   - Take a list of 5 numbers as input from the user.

2. **List Operations**
   - Print the original list.
   - Find and display the **sum, maximum, and minimum**.
   - Sort the list in ascending order.
   - Reverse the list in descending order.
   - Append a new number to the list.
   - Insert a number at a specific index (`2`).
   - Remove a specific number from the list.
   - Pop (remove) the last element from the list.
   - Check if a given number exists in the list (**membership operator `in`**).

---

## Program Code

```python
# List Manager

# Step 1: Input
numbers = list(map(int, input("Enter 5 numbers separated by space: ").split()))

# Step 2: Basic list info
print("\nOriginal list:", numbers)
print("Sum:", sum(numbers))
print("Max:", max(numbers))
print("Min:", min(numbers))

# Step 3: Sorting and reversing
print("Sorted:", sorted(numbers))       # ascending order
print("Reversed:", sorted(numbers, reverse=True))  # descending order

# Step 4: Append
new_num = int(input("\nEnter a number to append: "))
numbers.append(new_num)
print("After appending:", numbers)

# Step 5: Insert
insert_num = int(input("Enter a number to insert at index 2: "))
numbers.insert(2, insert_num)
print("After inserting:", numbers)

# Step 6: Remove
remove_num = int(input("Enter a number to remove: "))
if remove_num in numbers:
    numbers.remove(remove_num)
    print("After removing:", numbers)
else:
    print(remove_num, "not found in list!")

# Step 7: Pop
numbers.pop()  # removes last element
print("After popping last element:", numbers)

# Step 8: Membership check
search_num = int(input("Enter a number to search: "))
print(f"Is {search_num} in the list?", search_num in numbers)
````

---

## Sample Run

```
Enter 5 numbers separated by space: 10 5 20 15 8

Original list: [10, 5, 20, 15, 8]
Sum: 58
Max: 20
Min: 5
Sorted: [5, 8, 10, 15, 20]
Reversed: [20, 15, 10, 8, 5]

Enter a number to append: 25
After appending: [10, 5, 20, 15, 8, 25]

Enter a number to insert at index 2: 12
After inserting: [10, 5, 12, 20, 15, 8, 25]

Enter a number to remove: 15
After removing: [10, 5, 12, 20, 8, 25]

After popping last element: [10, 5, 12, 20, 8]

Enter a number to search: 20
Is 20 in the list? True
```

---

##  Learning Outcomes

* How to take **list input** from the user.
* Using built-in functions: `sum()`, `max()`, `min()`.
* Performing list methods: `append()`, `insert()`, `remove()`, `pop()`.
* Sorting and reversing lists.
* Checking membership with the `in` operator.

✅ A complete practice task for mastering Python **list operations**.


