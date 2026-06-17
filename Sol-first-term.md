Here is the complete Python solution for the assignment:

```python
# Student Information & Performance Analyzer

# Step 1: Get User Input
name = input("Enter Full Name: ")
age = int(input("Enter Age: "))
course = input("Enter Course Name: ")

python_marks = float(input("Enter Python Marks: "))
ai_marks = float(input("Enter AI Marks: "))
web_marks = float(input("Enter Web Development Marks: "))

# Step 2: String Operations
print("\n----- STRING OPERATIONS -----")
print("Name in UPPERCASE :", name.upper())
print("Name in lowercase :", name.lower())
print("First 5 Characters:", name[:5])
print("Last 3 Characters :", name[-3:])
print("Total Characters  :", len(name))

# Step 3: Arithmetic Operations
total_marks = python_marks + ai_marks + web_marks
percentage = (total_marks / 300) * 100
average_marks = total_marks / 3

# Step 4: Comparison Operators
excellent = percentage >= 80
passed = percentage >= 50

# Step 5: Logical Operators
scholarship = (percentage >= 80) and (age <= 25)

# Step 6: Membership Operators
subjects = ["Python", "AI", "Web Development"]

subject_name = input("\nEnter a Subject to Search: ")

subject_found = subject_name in subjects

# Step 7: Generate Formatted Report
print("\n-----------------------------------")
print("         STUDENT REPORT")
print("-----------------------------------")
print(f"Name          : {name}")
print(f"Course        : {course}")
print(f"Age           : {age}")

print(f"\nTotal Marks   : {total_marks}")
print(f"Percentage    : {percentage:.2f}%")
print(f"Average Marks : {average_marks:.2f}")

print(f"\nExcellent     : {excellent}")
print(f"Passed        : {passed}")
print(f"Scholarship   : {scholarship}")

print(f"\nSubject Found : {subject_found}")
print("-----------------------------------")
```

### Sample Input

```text
Enter Full Name: Navjot Kaur
Enter Age: 20
Enter Course Name: BCA
Enter Python Marks: 90
Enter AI Marks: 85
Enter Web Development Marks: 80
Enter a Subject to Search: Python
```

### Sample Output

```text
----- STRING OPERATIONS -----
Name in UPPERCASE : NAVJOT KAUR
Name in lowercase : navjot kaur
First 5 Characters: Navjo
Last 3 Characters : aur
Total Characters  : 11

-----------------------------------
         STUDENT REPORT
-----------------------------------
Name          : Navjot Kaur
Course        : BCA
Age           : 20

Total Marks   : 255.0
Percentage    : 85.00%
Average Marks : 85.00

Excellent     : True
Passed        : True
Scholarship   : True

Subject Found : True
-----------------------------------
```

This solution covers **Data Types, Strings, Arithmetic Operators, Comparison Operators, Logical Operators, Membership Operators, User Input, and Formatted Output** in a single program.
