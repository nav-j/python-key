# Python File Handling Task

## Problem Statement

This program demonstrates **file handling in Python** using different modes of the `open()` function:

* `x` → Create a new file (throws error if the file already exists).
* `w` → Write (overwrites file if it exists).
* `r` → Read file contents.
* `a` → Append data to the file.

---

## 📝 Steps Performed

1. **Create a new file** named `notes.txt` using mode `x`.

   * If the file already exists, the program will throw a `FileExistsError`.

2. **Write** 3 lines of text into the file using mode `w`.

3. **Read** and display the file contents using mode `r`.

4. **Append** 2 more lines of text using mode `a`.

5. **Read** the file again to display the updated contents.

---

##  Code

```python
# File Handling Task in Python

filename = "notes.txt"

# 1. Create a new file using 'x'
# (This will throw an error if file already exists)
with open(filename, "x") as f:
    print("File created successfully!")

# 2. Write 3 lines into the file using 'w'
with open(filename, "w") as f:
    f.write("Python is fun.\n")
    f.write("File handling is important.\n")
    f.write("Practice makes perfect.\n")
print("File written successfully!\n")

# 3. Read and display file contents using 'r'
print("Reading file contents:")
with open(filename, "r") as f:
    lines = f.readlines()
    for i, line in enumerate(lines, start=1):
        print(f"Line {i}: {line.strip()}")

# 4. Append 2 more lines using 'a'
with open(filename, "a") as f:
    f.write("Appending more notes here.\n")
    f.write("Learning never stops!\n")
print("\nAppending new lines...")
print("File updated successfully!\n")

# 5. Read again and display updated contents
print("Reading updated file contents:")
with open(filename, "r") as f:
    lines = f.readlines()
    for i, line in enumerate(lines, start=1):
        print(f"Line {i}: {line.strip()}")
```

---

## ✅ Example Output

```
File created successfully!
File written successfully!

Reading file contents:
Line 1: Python is fun.
Line 2: File handling is important.
Line 3: Practice makes perfect.

Appending new lines...
File updated successfully!

Reading updated file contents:
Line 1: Python is fun.
Line 2: File handling is important.
Line 3: Practice makes perfect.
Line 4: Appending more notes here.
Line 5: Learning never stops!
```
