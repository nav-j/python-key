# Python Task – File Handling (Notes Manager)

## Problem Statement
Write a Python program that acts as a simple **Notes Manager**.  
The program should allow the user to **write, append, and read** from a text file (`notes.txt`) using Python’s file handling features.  

---

## Requirements
1. **Create a file** `notes.txt` if it does not exist.
2. Provide a **menu-driven program** with the following options:
   - `1. Write` → Overwrite the file with new content.
   - `2. Append` → Add new content at the end of the file.
   - `3. Read` → Display the file contents.
   - `4. Exit` → Quit the program.
3. Handle cases where:
   - File does not exist.
   - File is empty.

---

## Expected output
```

Choose an option:

1. Write
2. Append
3. Read
4. Exit
   Enter choice: 1
   Enter your text: Hello, this is my first note!
   ✅ Notes saved successfully!

Enter choice: 2
Enter text to append: Adding more notes.
✅ Notes appended successfully!

Enter choice: 3
📖 File Content:
Hello, this is my first note!
Adding more notes.

Enter choice: 4
 Exiting program...

````

---

## 🔑 Features
- **Write Mode (`w`)** → Creates/overwrites the file with new content.  
- **Append Mode (`a`)** → Adds text to the end without deleting existing content.  
- **Read Mode (`r`)** → Displays all notes stored in the file.  
- **Error Handling** → Gracefully handles missing or empty file cases.  
- **Menu System** → Keeps running until the user chooses Exit.  

---

##  Solution Code

```python

filename = "notes.txt"

def write_file():
    text = input("Enter your text: ")
    with open(filename, "w") as f:
        f.write(text + "\n")
    print("✅ Notes saved successfully!\n")

def append_file():
    text = input("Enter text to append: ")
    with open(filename, "a") as f:
        f.write(text + "\n")
    print("✅ Notes appended successfully!\n")

def read_file():
    try:
        with open(filename, "r") as f:
            content = f.read()
            if content.strip() == "":
                print("📖 File is empty!\n")
            else:
                print("📖 File Content:\n" + content + "\n")
    except FileNotFoundError:
        print("⚠️ File does not exist yet. Please write something first!\n")

# Main Menu
while True:
    print("Choose an option:")
    print("1. Write")
    print("2. Append")
    print("3. Read")
    print("4. Exit")
    
    choice = input("Enter choice: ")

    if choice == "1":
        write_file()
    elif choice == "2":
        append_file()
    elif choice == "3":
        read_file()
    elif choice == "4":
        print("👋 Exiting program...")
        break
    else:
        print("❌ Invalid choice! Please try again.\n")
````
