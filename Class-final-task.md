# Python Practice Task  

## Task: Bank Account Management  

### Problem Statement  
Write a Python program that simulates a simple **bank account system** using **classes and objects**.  

---

###  Requirements  

1. Create a class `BankAccount` with:  

   - **Attributes**:  
     * `account_holder`  
     * `balance` (default = 0)  

   - **Methods**:  
     * `deposit(amount)` → adds money to balance.  
     * `withdraw(amount)` → subtracts money if balance is sufficient, otherwise show error.  
     * `display_balance()` → prints the current balance.  

2. In the main program:  
   - Create an object of `BankAccount`.  
   - Perform deposit, withdrawal, and display balance operations.  

---

###  Example Output  

```
```
Account Holder: Alice
Initial Balance: 0

Depositing 500...
Balance after deposit: 500

Withdrawing 200...
Balance after withdrawal: 300

Withdrawing 500...
Insufficient balance!

Final Balance: 300
```
````

---

###  Starter Code  

```python
# Class definition
class BankAccount:
    def __init__(self, account_holder, balance=0):
        self.account_holder = account_holder
        self.balance = balance

    def deposit(self, amount):
        self.balance += amount
        print(f"Deposited {amount}. New Balance: {self.balance}")

    def withdraw(self, amount):
        if amount <= self.balance:
            self.balance -= amount
            print(f"Withdrew {amount}. New Balance: {self.balance}")
        else:
            print("Insufficient balance!")

    def display_balance(self):
        print(f"Account Holder: {self.account_holder}, Balance: {self.balance}")


# Main program
def main():
    # Create object of BankAccount
    acc1 = BankAccount("Alice")

    acc1.display_balance()
    acc1.deposit(500)
    acc1.withdraw(200)
    acc1.withdraw(500)
    acc1.display_balance()

# Run program
main()
````

---

###  Hint

* Use `self` to access attributes inside the class.
* Always check for sufficient balance before withdrawing.
* You can create multiple `BankAccount` objects for different users.
