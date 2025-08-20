
```markdown
# 📝 String Formatter (Python Task)

This is a simple Python program to practice **string functions**.

---

## 📌 Task Description

Write a Python program that:

1. Takes a sentence as input.  
2. Prints the following using string functions:
   - The sentence in **uppercase**  
   - The sentence in **lowercase**  
   - The sentence with all spaces replaced by `-`  
   - The sentence split into words  

---

## ✅ Example Output

```

Enter a sentence: Python is Fun

Uppercase: PYTHON IS FUN
Lowercase: python is fun
Replaced spaces: Python-is-Fun
Split into words: \['Python', 'is', 'Fun']

````

---

## 💻 Solution

```python
# String Formatter

# Step 1: Take input
sentence = input("Enter a sentence: ")

# Step 2: Apply string functions
print("Uppercase:", sentence.upper())
print("Lowercase:", sentence.lower())
print("Replaced spaces:", sentence.replace(" ", "-"))
print("Split into words:", sentence.split())
````

---

## 🎯 Learning Goals

* Using `.upper()` to convert text to uppercase
* Using `.lower()` to convert text to lowercase
* Using `.replace()` to substitute characters
* Using `.split()` to break a string into words

---
