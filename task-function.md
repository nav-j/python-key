```markdown
#  Python Practice Task

## Task: Student Grade Calculator

###  Problem Statement
Write a Python program that:

1. Defines a **function** `calculate_grade(marks)` that:
   - Takes **marks** (0–100) as input.
   - Returns the **grade** based on the following rules:
     - 90–100 → A  
     - 75–89 → B  
     - 50–74 → C  
     - Below 50 → Fail  

2. In the `main()` function:
   - Ask the user to enter a student’s name and marks.  
   - Call the `calculate_grade()` function.  
   - Print the student’s name, marks, and grade.  

---

### 💻 Example Output
```

Enter student name: Alice
Enter marks: 82

Student: Alice
Marks: 82
Grade: B

````

---

### 📝 Starter Code
```python
# Function to calculate grade
def calculate_grade(marks):
    if marks >= 90:
        return "A"
    elif marks >= 75:
        return "B"
    elif marks >= 50:
        return "C"
    else:
        return "Fail"

# Main function
def main():
    name = input("Enter student name: ")
    marks = int(input("Enter marks: "))
    
    grade = calculate_grade(marks)
    
    print("\nStudent:", name)
    print("Marks:", marks)
    print("Grade:", grade)

# Call main function
main()
````

---

### 🚀 How to Run

1. Save the code in a file named **`grade_calculator.py`**
2. Open terminal/command prompt and run:

   ```bash
   python grade_calculator.py
   ```
3. Enter a student name and marks when prompted.

---

### 🎯 Learning Outcome

* Understand **functions** in Python.
* Practice **if-elif-else** conditions.
* Learn how to **take user input** and display results.
