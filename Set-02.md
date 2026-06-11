# 🐍 Python Set Assignment – Student Club Management System

## Objective

Practice Python **Sets** and their methods by managing members of different student clubs.

---

## Task

Create a Python program that performs the following operations:

### Step 1: Create Sets

Create two sets:

```python
science_club = {"Aman", "Riya", "Karan", "Simran"}
sports_club = {"Karan", "Simran", "Rahul", "Neha"}
```

---

### Step 2: Add a New Member

Ask the user to enter a new student name and add it to the Science Club using a set method.

---

### Step 3: Remove a Member

Ask the user for a member name to remove from the Sports Club.

---

### Step 4: Display Common Members

Find and display students who are members of both clubs.

---

### Step 5: Display All Members

Display all unique students from both clubs.

---

### Step 6: Find Exclusive Members

Display students who are only in the Science Club.

---

### Step 7: Check Membership

Ask the user for a student name and check whether they are in the Science Club.

---

### Step 8: Clear a Temporary Set

Create a temporary set:

```python
temp_set = {"Test1", "Test2", "Test3"}
```

Clear all elements from it and display the result.

---

# Methods to Use

Use the following set methods in your program:

* `add()`
* `remove()` or `discard()`
* `intersection()`
* `union()`
* `difference()`
* `clear()`

---

# Sample Output

```text
Enter a new Science Club member: Priya

Science Club:
{'Aman', 'Riya', 'Karan', 'Simran', 'Priya'}

Enter a Sports Club member to remove: Rahul

Sports Club:
{'Karan', 'Simran', 'Neha'}

Common Members:
{'Karan', 'Simran'}

All Members:
{'Aman', 'Riya', 'Karan', 'Simran', 'Neha', 'Priya'}

Science Club Only:
{'Aman', 'Riya', 'Priya'}

Enter a student name to search: Karan
Karan is a member of Science Club.

Temporary Set before clear:
{'Test1', 'Test2', 'Test3'}

Temporary Set after clear:
set()
```

---

# Solution

```python
# Student Club Management System

science_club = {"Aman", "Riya", "Karan", "Simran"}
sports_club = {"Karan", "Simran", "Rahul", "Neha"}

# Add member
new_member = input("Enter a new Science Club member: ")
science_club.add(new_member)

print("\nScience Club:")
print(science_club)

# Remove member
remove_member = input("\nEnter a Sports Club member to remove: ")
sports_club.discard(remove_member)

print("\nSports Club:")
print(sports_club)

# Common members
common_members = science_club.intersection(sports_club)
print("\nCommon Members:")
print(common_members)

# All members
all_members = science_club.union(sports_club)
print("\nAll Members:")
print(all_members)

# Science Club only
science_only = science_club.difference(sports_club)
print("\nScience Club Only:")
print(science_only)

# Membership check
search_name = input("\nEnter a student name to search: ")

if search_name in science_club:
    print(search_name, "is a member of Science Club.")
else:
    print(search_name, "is not a member of Science Club.")

# Clear set
temp_set = {"Test1", "Test2", "Test3"}

print("\nTemporary Set before clear:")
print(temp_set)

temp_set.clear()

print("\nTemporary Set after clear:")
print(temp_set)
```

This assignment covers the most commonly used set methods and gives hands-on practice with real-world data management.
