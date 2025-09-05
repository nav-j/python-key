
#  Python Test Task – Library Management System

## Problem Statement
Write a Python program that simulates a **library management system** using both **Python basics** and **OOP concepts**.

---

## Requirements

1. Create a class `Book` with:
   - Attributes: `title`, `author`, `available` (default = True).  
   - Method: `display_info()` → prints book details.  

2. Create a class `Library` with:
   - Attribute: `books` (a list to store book objects).  
   - Methods:  
     - `add_book(book)` → adds a book to the library.  
     - `show_books()` → displays all books.  
     - `borrow_book(title)` → changes availability if the book is borrowed.  

3. In the main program:
   - Create a few books and add them to the library.  
   - Use a loop to display a menu:  
     1. Show all books  
     2. Borrow a book  
     3. Exit  

---

## ✅ Solution Code

```python
# 📚 Library Management System (Python Basics + OOP)

# Book class
class Book:
    def __init__(self, title, author):
        self.title = title
        self.author = author
        self.available = True

    def display_info(self):
        status = "Available" if self.available else "Not Available"
        print(f"{self.title} by {self.author} - {status}")

# Library class
class Library:
    def __init__(self):
        self.books = []

    def add_book(self, book):
        self.books.append(book)

    def show_books(self):
        if not self.books:
            print("No books in the library.")
        else:
            for book in self.books:
                book.display_info()

    def borrow_book(self, title):
        for book in self.books:
            if book.title.lower() == title.lower():
                if book.available:
                    book.available = False
                    print(f"You borrowed '{book.title}'.")
                else:
                    print(f"'{book.title}' is already borrowed.")
                return
        print("Book not found!")

# Main program
library = Library()

# Adding some books
library.add_book(Book("Python Basics", "John Doe"))
library.add_book(Book("OOP in Python", "Jane Smith"))
library.add_book(Book("Data Science 101", "Emily Brown"))

# Menu loop
while True:
    print("\n--- Library Menu ---")
    print("1. Show all books")
    print("2. Borrow a book")
    print("3. Exit")

    choice = input("Enter choice: ")

    if choice == "1":
        library.show_books()
    elif choice == "2":
        title = input("Enter book title: ")
        library.borrow_book(title)
    elif choice == "3":
        print("Exiting... Goodbye!")
        break
    else:
        print("Invalid choice. Try again.")
````

---

## 🖥 Example Run

```
--- Library Menu ---
1. Show all books
2. Borrow a book
3. Exit
Enter choice: 1
Python Basics by John Doe - Available
OOP in Python by Jane Smith - Available
Data Science 101 by Emily Brown - Available

--- Library Menu ---
1. Show all books
2. Borrow a book
3. Exit
Enter choice: 2
Enter book title: Python Basics
You borrowed 'Python Basics'.

--- Library Menu ---
1. Show all books
2. Borrow a book
3. Exit
Enter choice: 1
Python Basics by John Doe - Not Available
OOP in Python by Jane Smith - Available
Data Science 101 by Emily Brown - Available
```
