#  String Playground (Python Assignment)

This program is a practice set to explore different **Python string functions** such as `format()`, `center()`, `partition()`, `join()`, indexing, slicing, and more.  

---

##  Tasks

### **1. Using `format()`**
Ask the user for their **name** and **age**, and print:  
```

My name is Alice and I am 20 years old.

```

---

### **2. Using `center()`**
Take the user’s name and print it **centered in 30 spaces**, padded with `*`.  
```

***********Alice***********\*

```

---

### **3. Using `partition()`**
Ask the user to enter a sentence. Split it into three parts based on the **first space**.  
```

Input: "Python is awesome"
Output: ('Python', ' ', 'is awesome')

````

---

### **4. Using `join()`**
Take a list of words:  
```python
["Python", "is", "fun"]
````

Join them with `-`:

```
Python-is-fun
```

---

### **5. Using Indexing & Slicing**

From the user’s name, print:

* First character
* Last character
* Middle part (excluding first & last)

---

### **6. Other String Functions**

On the same sentence (from Task 3), apply:

* `.count("a")` → Count how many times `a` appears
* `.startswith("P")` → Check if it starts with P
* `.endswith("!")` → Check if it ends with !

---

##  Example Output

```
Enter your name: Alice
Enter your age: 20
My name is Alice and I am 20 years old.

***********Alice************

Enter a sentence: Python is awesome
Partitioned: ('Python', ' ', 'is awesome')

Joined words: Python-is-fun

First character: A
Last character: e
Middle part: lic

Count of 'a': 1
Starts with P? True
Ends with !? False
```

---

##  Solution

```python
# String Playground

# 1. format()
name = input("Enter your name: ")
age = input("Enter your age: ")
print("My name is {} and I am {} years old.".format(name, age))

# 2. center()
print(name.center(30, "*"))

# 3. partition()
sentence = input("Enter a sentence: ")
print("Partitioned:", sentence.partition(" "))

# 4. join()
words = ["Python", "is", "fun"]
print("Joined words:", "-".join(words))

# 5. indexing & slicing
print("First character:", name[0])
print("Last character:", name[-1])
print("Middle part:", name[1:-1])

# 6. other string functions
print("Count of 'a':", sentence.count("a"))
print("Starts with P?", sentence.startswith("P"))
print("Ends with !?", sentence.endswith("!"))
```

---

##  Learning Goals

* Using `format()` for formatted output
* Centering strings with `center()`
* Splitting strings with `partition()`
* Joining lists into strings with `join()`
* Indexing & slicing strings
* Applying `.count()`, `.startswith()`, `.endswith()`

```

