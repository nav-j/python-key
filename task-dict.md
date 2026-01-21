# Python Practice Task - Student Score Manager

A beginner-friendly Python practice task to understand and use **dictionaries** in Python.

---

## Task Description

Write a Python program that:

1. Takes input of **3 students and their scores** (name and score).
2. Stores the records in a **dictionary** where:
   - Key → Student name  
   - Value → Score  
3. Performs the following operations:
   - Print the **dictionary**.  
   - Print all **student names**.  
   - Print all **scores**.  
   - Find and print the **highest score** with the student’s name.  

---

## Example Run

```
```
Enter student 1 name: Alice
Enter Alice's score: 85
Enter student 2 name: Bob
Enter Bob's score: 92
Enter student 3 name: Charlie
Enter Charlie's score: 78

\--- Student Records ---
Student Records: {'Alice': 85, 'Bob': 92, 'Charlie': 78}
All Students: \['Alice', 'Bob', 'Charlie']
All Scores: \[85, 92, 78]
Top Scorer: Bob with 92

```
````

---

## Solution Code

```python
#  Student Score Manager

# Empty dictionary to store student records
student_scores = {}

# Taking input for 3 students
for i in range(3):
    name = input(f"Enter student {i+1} name: ")
    score = int(input(f"Enter {name}'s score: "))
    student_scores[name] = score  # store in dictionary

# Displaying results
print("\n--- Student Records ---")
print("Student Records:", student_scores)

print("All Students:", list(student_scores.keys()))
print("All Scores:", list(student_scores.values()))

# Finding top scorer
top_student = max(student_scores, key=student_scores.get)
print(f"Top Scorer: {top_student} with {student_scores[top_student]}")
````

---

##  Learning Outcome

* Learn how to create and use **dictionaries** in Python.
* Understand how to **store key-value pairs**.
* Practice retrieving **keys, values**, and finding the **maximum value**.
