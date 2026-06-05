## Python Assignment: Left Shift (`<<`) and Right Shift (`>>`) Operators

## Objective

Practice using Python's **left shift** and **right shift** bitwise operators.

---

## Task 1: Basic Left Shift

1. Create a variable `num` and assign it the value `7`.
2. Left shift the number by `2` positions.
3. Print the original value and the shifted value.

**Expected Output Format:**

```text
Original Number: 7
After Left Shift by 2: 28
```

---

## Task 2: Basic Right Shift

1. Create a variable `num` and assign it the value `32`.
2. Right shift the number by `3` positions.
3. Print the original value and the shifted value.

**Expected Output Format:**

```text
Original Number: 32
After Right Shift by 3: 4
```

---

## Task 3: User Input – Left Shift

1. Ask the user to enter a number.
2. Ask the user to enter the number of positions to shift left.
3. Display the result.

**Sample Run:**

```text
Enter a number: 5
Enter shift positions: 3

Result: 40
```

---

## Task 4: User Input – Right Shift

1. Ask the user to enter a number.
2. Ask the user to enter the number of positions to shift right.
3. Display the result.

**Sample Run:**

```text
Enter a number: 64
Enter shift positions: 2

Result: 16
```

---

## Task 5: Compare Left and Right Shift

For the number `10`:

1. Left shift by `1`.
2. Right shift by `1`.
3. Display all results in a table-like format.

**Expected Output:**

```text
Original Number : 10
Left Shift (<<1): 20
Right Shift (>>1): 5
```

# ✅ Solutions: Left Shift (`<<`) and Right Shift (`>>`) Operators

---

## Task 1: Basic Left Shift

```python
num = 7

shifted = num << 2

print("Original Number:", num)
print("After Left Shift by 2:", shifted)
```

**Output:**

```text
Original Number: 7
After Left Shift by 2: 28
```

---

## Task 2: Basic Right Shift

```python
num = 32

shifted = num >> 3

print("Original Number:", num)
print("After Right Shift by 3:", shifted)
```

**Output:**

```text
Original Number: 32
After Right Shift by 3: 4
```

---

## Task 3: User Input – Left Shift

```python
num = int(input("Enter a number: "))
shift = int(input("Enter shift positions: "))

result = num << shift

print("Result:", result)
```

**Sample Output:**

```text
Enter a number: 5
Enter shift positions: 3
Result: 40
```

---

## Task 4: User Input – Right Shift

```python
num = int(input("Enter a number: "))
shift = int(input("Enter shift positions: "))

result = num >> shift

print("Result:", result)
```

**Sample Output:**

```text
Enter a number: 64
Enter shift positions: 2
Result: 16
```

---

## Task 5: Compare Left and Right Shift

```python
num = 10

left_shift = num << 1
right_shift = num >> 1

print("Original Number :", num)
print("Left Shift (<<1):", left_shift)
print("Right Shift (>>1):", right_shift)
```

**Output:**

```text
Original Number : 10
Left Shift (<<1): 20
Right Shift (>>1): 5
```

---

# 🌟 Challenge Task Solution

```python
num = int(input("Enter a number: "))

print("\nLeft Shifts")
print(f"{num} << 1 = {num << 1}")
print(f"{num} << 2 = {num << 2}")
print(f"{num} << 3 = {num << 3}")

print("\nRight Shifts")
print(f"{num} >> 1 = {num >> 1}")
print(f"{num} >> 2 = {num >> 2}")
print(f"{num} >> 3 = {num >> 3}")
```

**Sample Output:**

```text
Enter a number: 8

Left Shifts
8 << 1 = 16
8 << 2 = 32
8 << 3 = 64

Right Shifts
8 >> 1 = 4
8 >> 2 = 2
8 >> 3 = 1
```

---

## Bonus Task: Using Assignment Operators

```python
num = 8

num <<= 2
print("After <<= 2 :", num)

num >>= 1
print("After >>= 1 :", num)
```

**Output:**

```text
After <<= 2 : 32
After >>= 1 : 16
```

This bonus task demonstrates the shorthand operators `<<=` and `>>=`.
