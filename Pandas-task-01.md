# Pandas Task – Series, DataFrames, CSV/JSON & Data Analysis

## Objective

Practice **Pandas fundamentals**: creating Series and DataFrames, working with CSV & JSON files, and performing basic data analysis.

---

## 📝 Task Instructions

### **Part 1 – Pandas Series**

1. Create a **Pandas Series** with values `[10, 20, 30, 40, 50]` and custom index `['a','b','c','d','e']`.
2. Access the value at index `'c'`.
3. Find the **sum** and **mean** of the Series.
4. Multiply all elements of the Series by 2.

---

### **Part 2 – Pandas DataFrame**

1. Create a DataFrame with the following data:

   | Name  | Age | Marks | City     |
   | ----- | --- | ----- | -------- |
   | John  | 20  | 85    | New York |
   | Alice | 19  | 92    | London   |
   | Bob   | 21  | 75    | Paris    |
   | Emma  | 22  | 90    | Tokyo    |
   | David | 20  | 60    | Sydney   |

2. Display the **first 3 rows**.

3. Display only the **Name** and **Marks** columns.

4. Filter students who scored **more than 80 Marks**.

5. Sort the DataFrame by **Age**.

6. Group by **City** and find the **average Marks** of students in each city.

---

### **Part 3 – Reading CSV & JSON**

1. Save the DataFrame as a **CSV file** (`students.csv`) and a **JSON file** (`students.json`).
2. Read both files back into Pandas using:

   * `pd.read_csv("students.csv")`
   * `pd.read_json("students.json")`
3. Display the first 5 rows after reading.

---

### **Part 4 – Analyzing Data**

1. Show the **summary statistics** (`.describe()`) of the DataFrame.
2. Find the student with the **highest Marks**.
3. Count how many students are in each **City**.
4. Find the **average Age** of all students.

---

## Expected Outcomes

* Understand **Pandas Series** operations (indexing, aggregation, element-wise operations).
* Gain confidence in **DataFrame creation, filtering, sorting, and grouping**.
* Learn how to **read & write CSV/JSON files**.
* Perform **basic data analysis** with Pandas.

---

## ✅ Sample Solution

```python
import pandas as pd

# ---------------- Part 1: Pandas Series ----------------
s = pd.Series([10, 20, 30, 40, 50], index=['a', 'b', 'c', 'd', 'e'])
print("Series:\n", s)
print("Value at index 'c':", s['c'])
print("Sum:", s.sum())
print("Mean:", s.mean())
print("Series * 2:\n", s * 2)

# ---------------- Part 2: Pandas DataFrame ----------------
data = {
    "Name": ["John", "Alice", "Bob", "Emma", "David"],
    "Age": [20, 19, 21, 22, 20],
    "Marks": [85, 92, 75, 90, 60],
    "City": ["New York", "London", "Paris", "Tokyo", "Sydney"]
}
df = pd.DataFrame(data)

print("\nFirst 3 rows:\n", df.head(3))
print("\nName & Marks:\n", df[["Name", "Marks"]])
print("\nMarks > 80:\n", df[df["Marks"] > 80])
print("\nSorted by Age:\n", df.sort_values(by="Age"))
print("\nAverage Marks by City:\n", df.groupby("City")["Marks"].mean())

# ---------------- Part 3: CSV & JSON ----------------
df.to_csv("students.csv", index=False)
df.to_json("students.json", orient="records")

df_csv = pd.read_csv("students.csv")
df_json = pd.read_json("students.json")

print("\nRead from CSV:\n", df_csv.head())
print("\nRead from JSON:\n", df_json.head())

# ---------------- Part 4: Data Analysis ----------------
print("\nSummary Statistics:\n", df.describe())
print("\nStudent with Highest Marks:\n", df.loc[df["Marks"].idxmax()])
print("\nStudents per City:\n", df["City"].value_counts())
print("\nAverage Age:", df["Age"].mean())
```

# 📊 Sample Output – Pandas Series, DataFrames, CSV/JSON & Data Analysis

This document shows the **expected sample output** when running the Pandas practice task.

---

### **Part 1 – Pandas Series**

```text
Series:
a    10
b    20
c    30
d    40
e    50
dtype: int64

Value at index 'c': 30
Sum: 150
Mean: 30.0
Series * 2:
a     20
b     40
c     60
d     80
e    100
dtype: int64
```

---

### **Part 2 – Pandas DataFrame**

```text
First 3 rows:
    Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
2    Bob   21     75     Paris

Name & Marks:
    Name  Marks
0   John     85
1  Alice     92
2    Bob     75
3   Emma     90
4  David     60

Marks > 80:
    Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
3   Emma   22     90     Tokyo

Sorted by Age:
    Name  Age  Marks      City
1  Alice   19     92    London
0   John   20     85  New York
4  David   20     60    Sydney
2    Bob   21     75     Paris
3   Emma   22     90     Tokyo

Average Marks by City:
City
London      92.0
New York    85.0
Paris       75.0
Sydney      60.0
Tokyo       90.0
Name: Marks, dtype: float64
```

---

### **Part 3 – Reading CSV & JSON**

```text
Read from CSV:
    Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
2    Bob   21     75     Paris
3   Emma   22     90     Tokyo
4  David   20     60    Sydney

Read from JSON:
    Name  Age  Marks      City
0   John   20     85  New York
1  Alice   19     92    London
2    Bob   21     75     Paris
3   Emma   22     90     Tokyo
4  David   20     60    Sydney
```

---

### **Part 4 – Data Analysis**

```text
Summary Statistics:
             Age      Marks
count   5.000000   5.000000
mean   20.400000  80.400000
std     1.140175  12.315302
min    19.000000  60.000000
25%    20.000000  75.000000
50%    20.000000  85.000000
75%    21.000000  90.000000
max    22.000000  92.000000

Student with Highest Marks:
Name     Alice
Age          19
Marks        92
City     London
Name: 1, dtype: object

Students per City:
New York    1
London      1
Paris       1
Tokyo       1
Sydney      1
Name: City, dtype: int64

Average Age: 20.4
```
