# Python Task – Pandas DataFrames & Data Cleaning

## Task

Write a Python program using **Pandas** to practice **DataFrame operations** and **data cleaning techniques**.

---

### **Dataset**

Create a DataFrame from the following student data:

| Name  | Age | Marks | City     |
| ----- | --- | ----- | -------- |
| John  | 20  | 85    | New York |
| Alice | 19  | NaN   | London   |
| Bob   | NaN | 75    | Paris    |
| Emma  | 22  | 90    | NaN      |
| David | 21  | 60    | Tokyo    |

---

### **Requirements**

#### 🧹 Data Cleaning

1. Display the **first 3 rows** of the DataFrame.
2. Check for **missing values**.
3. Fill missing **Age** values with the **average age**.
4. Fill missing **Marks** with the **median marks**.
5. Fill missing **City** with `"Unknown"`.

#### Operations

1. Show **statistics summary** (mean, median, min, max, etc.) of numeric columns.
2. Sort students by **Marks** in **descending order**.
3. Filter students who scored **more than 70**.
4. Group students by **City** and show the **average Marks** per city.

---

# Expected Output

* A **cleaned DataFrame** (no missing values).
* Summary statistics of numeric columns.
* A **sorted list** of students by marks (highest to lowest).
* A **filtered list** of students with marks > 70.
* Grouped results showing **average marks per city**.

---

## Example Solution

```python
import pandas as pd
import numpy as np

# Create DataFrame
data = {
    "Name": ["John", "Alice", "Bob", "Emma", "David"],
    "Age": [20, 19, np.nan, 22, 21],
    "Marks": [85, np.nan, 75, 90, 60],
    "City": ["New York", "London", "Paris", np.nan, "Tokyo"]
}
df = pd.DataFrame(data)

# Data Cleaning
print(df.head(3))                 # First 3 rows
print(df.isnull().sum())          # Missing values
df["Age"].fillna(df["Age"].mean(), inplace=True)
df["Marks"].fillna(df["Marks"].median(), inplace=True)
df["City"].fillna("Unknown", inplace=True)

# Operations
print(df.describe())                             # Statistics summary
print(df.sort_values(by="Marks", ascending=False)) # Sorted
print(df[df["Marks"] > 70])                      # Filtered
print(df.groupby("City")["Marks"].mean())        # Grouped
```
# Sample Output – Pandas DataFrames & Cleaning (Level-1)

---

### **1️⃣ Original DataFrame (First 3 rows)**

```text
    Name   Age  Marks     City
0   John  20.0   85.0  New York
1  Alice  19.0    NaN    London
2    Bob   NaN   75.0     Paris
```

---

### **2️⃣ Missing Values Count**

```text
Name     0
Age      1
Marks    1
City     1
dtype: int64
```

---

### **3️⃣ Cleaned DataFrame (After filling missing values)**

```text
    Name   Age  Marks      City
0   John  20.0   85.0  New York
1  Alice  19.0   75.0    London
2    Bob  20.5   75.0     Paris
3   Emma  22.0   90.0   Unknown
4  David  21.0   60.0     Tokyo
```

👉 Here:

* `Age` for Bob became **20.5** (mean of other ages).
* `Marks` for Alice became **75** (median of other marks).
* `City` for Emma became **"Unknown"**.

---

### **4️⃣ Statistics Summary**

```text
             Age      Marks
count   5.000000   5.000000
mean   20.900000  77.000000
std     1.140175  11.401754
min    19.000000  60.000000
25%    20.000000  75.000000
50%    20.500000  75.000000
75%    21.000000  85.000000
max    22.000000  90.000000
```

---

### **5️⃣ Sorted by Marks (Descending)**

```text
    Name   Age  Marks      City
3   Emma  22.0   90.0   Unknown
0   John  20.0   85.0  New York
1  Alice  19.0   75.0    London
2    Bob  20.5   75.0     Paris
4  David  21.0   60.0     Tokyo
```

---

### **6️⃣ Filter: Students with Marks > 70**

```text
    Name   Age  Marks      City
0   John  20.0   85.0  New York
1  Alice  19.0   75.0    London
2    Bob  20.5   75.0     Paris
3   Emma  22.0   90.0   Unknown
```

---

### **7️⃣ Grouped by City – Average Marks**

```text
City
London      75.0
New York    85.0
Paris       75.0
Tokyo       60.0
Unknown     90.0
Name: Marks, dtype: float64
```

---

✅ This is the **expected output** for the Level-1 Pandas cleaning & operations task.
