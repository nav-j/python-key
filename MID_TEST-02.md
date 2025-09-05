# Python Test Task – Banking System

## Problem Statement
Write a Python program that simulates a simple **banking system** using **classes, objects, loops, and conditionals**.

---

## Requirements

1. Create a class `BankAccount` with:
   - Attributes: `account_holder`, `balance` (default = 0).  
   - Methods:  
     - `deposit(amount)` → adds money to balance.  
     - `withdraw(amount)` → subtracts money if sufficient balance.  
     - `check_balance()` → prints current balance.  

2. In the main program:
   - Create one `BankAccount` object.  
   - Use a **looped menu** to perform operations:  
     1. Deposit Money  
     2. Withdraw Money  
     3. Check Balance  
     4. Exit  

---

## ✅ Solution Code

```python
# 🏦 Banking System (Python Basics + OOP)

# BankAccount class
class BankAccount:
    def __init__(self, account_holder, balance=0):
        self.account_holder = account_holder
        self.balance = balance

    def deposit(self, amount):
        if amount > 0:
            self.balance += amount
            print(f"Deposited: {amount}")
        else:
            print("Invalid deposit amount.")

    def withdraw(self, amount):
        if amount <= self.balance:
            self.balance -= amount
            print(f"Withdrew: {amount}")
        else:
            print("Insufficient balance!")

    def check_balance(self):
        print(f"Current Balance: {self.balance}")

# Main program
account = BankAccount("John Doe")

while True:
    print("\n--- Banking Menu ---")
    print("1. Deposit Money")
    print("2. Withdraw Money")
    print("3. Check Balance")
    print("4. Exit")

    choice = input("Enter choice: ")

    if choice == "1":
        amount = float(input("Enter deposit amount: "))
        account.deposit(amount)
    elif choice == "2":
        amount = float(input("Enter withdrawal amount: "))
        account.withdraw(amount)
    elif choice == "3":
        account.check_balance()
    elif choice == "4":
        print("Exiting... Goodbye!")
        break
    else:
        print("Invalid choice. Try again.")
````

---

## 🖥 Example Run

```
--- Banking Menu ---
1. Deposit Money
2. Withdraw Money
3. Check Balance
4. Exit
Enter choice: 1
Enter deposit amount: 1000
Deposited: 1000

--- Banking Menu ---
1. Deposit Money
2. Withdraw Money
3. Check Balance
4. Exit
Enter choice: 2
Enter withdrawal amount: 500
Withdrew: 500

--- Banking Menu ---
1. Deposit Money
2. Withdraw Money
3. Check Balance
4. Exit
Enter choice: 3
Current Balance: 500
```

---

## 🎯 Learning Outcomes

* ✅ Understanding **classes & objects** in Python
* ✅ Using **methods** to perform operations
* ✅ Applying **loops & conditionals** for menu-driven programs
* ✅ Handling **basic input/output** in Python

---

 This task is great for practicing both **Python basics** and **OOP concepts** together!
