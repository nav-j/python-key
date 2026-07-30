Here are some **Python encapsulation practice tasks** from beginner to intermediate level.

### Task 1: Student Information

Create a class `Student` with:

* A public variable `name`
* A protected variable `_course`
* A private variable `__marks`

Create a method `display()` to print all three values.

---

### Task 2: Bank Account

Create a class `BankAccount` with:

* Public variable `account_holder`
* Protected variable `_account_type`
* Private variable `__balance`

Create methods:

* `deposit(amount)` → Add money to balance
* `withdraw(amount)` → Withdraw money if sufficient balance
* `show_balance()` → Display the balance

**Example:**

```python
account = BankAccount("Anu", "Savings", 5000)
account.deposit(2000)
account.withdraw(1000)
account.show_balance()
```

Expected output:

```text
Balance: 6000
```

---

### Task 3: Employee Salary

Create a class `Employee` with:

* Public variable `name`
* Protected variable `_department`
* Private variable `__salary`

Create a method `display()` that displays all employee information.

Create another method `increase_salary(amount)` to increase the private salary.

---

### Task 4: Mobile Phone

Create a class `Mobile` with:

* Public variable `brand`
* Protected variable `_model`
* Private variable `__price`

Create methods:

* `display()` → Display mobile details
* `change_price(new_price)` → Change the private price
* `get_price()` → Return the current price

---

### Task 5: Login System ⭐

Create a class `User` with:

* Public variable `username`
* Private variable `__password`

Create methods:

* `set_password(new_password)`
* `check_password(password)`

The password should not be directly accessed outside the class.

**Example:**

```python
user = User("Anu", "abc123")

print(user.check_password("abc123"))
print(user.check_password("wrong"))
```

Expected output:

```text
True
False
```


## Solution

Sure! Here are the **solutions to all 5 encapsulation tasks**.

### 1. Student Information

```python
class Student:
    def __init__(self, name, course, marks):
        self.name = name          # Public
        self._course = course     # Protected
        self.__marks = marks      # Private

    def display(self):
        print("Name:", self.name)
        print("Course:", self._course)
        print("Marks:", self.__marks)


s = Student("Anu", "Python", 85)
s.display()
```

**Output:**

```text
Name: Anu
Course: Python
Marks: 85
```

---

### 2. Bank Account

```python
class BankAccount:
    def __init__(self, account_holder, account_type, balance):
        self.account_holder = account_holder
        self._account_type = account_type
        self.__balance = balance

    def deposit(self, amount):
        self.__balance += amount

    def withdraw(self, amount):
        if amount <= self.__balance:
            self.__balance -= amount
        else:
            print("Insufficient balance")

    def show_balance(self):
        print("Balance:", self.__balance)


account = BankAccount("Anu", "Savings", 5000)

account.deposit(2000)
account.withdraw(1000)
account.show_balance()
```

**Output:**

```text
Balance: 6000
```

Here, `__balance` is private, so it is accessed and modified through methods.

---

### 3. Employee Salary

```python
class Employee:
    def __init__(self, name, department, salary):
        self.name = name
        self._department = department
        self.__salary = salary

    def increase_salary(self, amount):
        self.__salary += amount

    def display(self):
        print("Name:", self.name)
        print("Department:", self._department)
        print("Salary:", self.__salary)


emp = Employee("Rohit", "IT", 30000)

emp.increase_salary(5000)
emp.display()
```

**Output:**

```text
Name: Rohit
Department: IT
Salary: 35000
```

---

### 4. Mobile Phone

```python
class Mobile:
    def __init__(self, brand, model, price):
        self.brand = brand
        self._model = model
        self.__price = price

    def change_price(self, new_price):
        self.__price = new_price

    def get_price(self):
        return self.__price

    def display(self):
        print("Brand:", self.brand)
        print("Model:", self._model)
        print("Price:", self.__price)


mobile = Mobile("Samsung", "Galaxy S25", 80000)

mobile.display()

mobile.change_price(75000)

print("New Price:", mobile.get_price())
```

**Output:**

```text
Brand: Samsung
Model: Galaxy S25
Price: 80000
New Price: 75000
```

---

### 5. Login System

```python
class User:
    def __init__(self, username, password):
        self.username = username
        self.__password = password

    def set_password(self, new_password):
        self.__password = new_password

    def check_password(self, password):
        return self.__password == password


user = User("Anu", "abc123")

print(user.check_password("abc123"))
print(user.check_password("wrong"))

user.set_password("xyz789")

print(user.check_password("xyz789"))
```

**Output:**

```text
True
False
True
```

### Encapsulation used in these examples

| Access Type   | Example        | Access                            |
| ------------- | -------------- | --------------------------------- |
| **Public**    | `self.name`    | Can be accessed directly          |
| **Protected** | `self._course` | Intended for class and subclasses |
| **Private**   | `self.__marks` | Accessed through class methods    |

**Main idea:** Encapsulation is used to **protect data and control how it is accessed or modified**.
