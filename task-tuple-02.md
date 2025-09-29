# Python Tuple Task – Loop, Join & Multiply

##  Task Description

In this exercise, you will practice working with **Python tuples** using the following concepts:

1. **Loop through tuples**

   * Use a `for` loop to print all animals.
   * Use a `while` loop to print all colors.

2. **Join tuples**

   * Combine two tuples (`animals` and `colors`) into a single tuple.

3. **Multiply tuples**

   * Repeat the `animals` tuple **2 times**.
   * Repeat the `colors` tuple **3 times**.

---

## ✅ Solution

```python
# Given tuples
animals = ("cat", "dog", "rabbit")
colors = ("red", "blue")

# 1. Loop through tuples
print("Animals using for loop:")
for animal in animals:
    print(animal)

print("\nColors using while loop:")
i = 0
while i < len(colors):
    print(colors[i])
    i += 1

# 2. Join Tuples
joined = animals + colors
print("\nJoined tuple:", joined)

# 3. Multiply Tuples
animals_repeated = animals * 2
print("Animals repeated 2 times:", animals_repeated)

colors_repeated = colors * 3
print("Colors repeated 3 times:", colors_repeated)
```

---

## 🖥️ Sample Output

```
Animals using for loop:
cat
dog
rabbit

Colors using while loop:
red
blue

Joined tuple: ('cat', 'dog', 'rabbit', 'red', 'blue')
Animals repeated 2 times: ('cat', 'dog', 'rabbit', 'cat', 'dog', 'rabbit')
Colors repeated 3 times: ('red', 'blue', 'red', 'blue', 'red', 'blue')
```

---

## 🎯 What You Learned

* Looping through tuples using **for** and **while**.
* Joining tuples using the `+` operator.
* Multiplying tuples using the `*` operator.
