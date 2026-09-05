Absolutely. Here is an **Intermediate-level Pandas Test** suitable for a Python/Data Analytics class.

# 🐼 Pandas Practical Test — Python

**Total Marks: 50**
**Time: 90 Minutes**
**Level: Intermediate**

### Instructions

* Use **Python + Pandas**.
* Write and execute all programs.
* Display the output wherever required.
* Do not use Excel for calculations.

---

## Part A — Pandas Basics (10 Marks)

### Q1. Create a DataFrame — 5 Marks

Create the following DataFrame:

| Name   | Age | City       | Marks | Department |
| ------ | --: | ---------- | ----: | ---------- |
| Aman   |  21 | Delhi      |    85 | IT         |
| Simran |  22 | Chandigarh |    92 | HR         |
| Raj    |  20 | Ludhiana   |    76 | IT         |
| Neha   |  23 | Delhi      |    88 | Finance    |
| Karan  |  21 | Amritsar   |    69 | HR         |
| Priya  |  22 | Chandigarh |    95 | IT         |

Perform the following:

1. Display the first 3 rows.
2. Display the last 2 rows.
3. Display the column names.
4. Display the shape of the DataFrame.
5. Display the data types.

---

### Q2. Selecting Data — 5 Marks

Using the DataFrame from Q1:

1. Display only the `Name` and `Marks` columns.
2. Display the details of the student whose name is `Neha`.
3. Display students whose marks are greater than 80.
4. Display students from `Chandigarh`.

---

# Part B — Data Filtering and Modification (15 Marks)

### Q3. Filtering Data — 5 Marks

Using the same DataFrame:

1. Find students whose marks are between **70 and 90**.
2. Find students whose age is greater than 21.
3. Find students who belong to the **IT department**.
4. Find students from **Delhi or Chandigarh**.
5. Find students whose marks are greater than 80 and department is IT.

---

### Q4. Add and Modify Columns — 5 Marks

Perform the following:

1. Add a column called `Result`.

   * Marks >= 40 → `"Pass"`
   * Marks < 40 → `"Fail"`

2. Add a column called `Bonus`.

   * Students scoring 90 or above → 1000
   * Otherwise → 500

3. Increase all marks by **5 marks**.

4. Display the updated DataFrame.

---

### Q5. Delete and Rename Columns — 5 Marks

Perform the following:

1. Rename `Marks` to `Score`.
2. Rename `Department` to `Dept`.
3. Delete the `Bonus` column.
4. Display the final DataFrame.

---

# Part C — Missing Data and Statistics (10 Marks)

### Q6. Missing Values — 5 Marks

Create the following DataFrame:

```python
data = {
    "Name": ["Aman", "Simran", "Raj", "Neha", "Karan"],
    "Age": [21, 22, None, 23, 21],
    "Marks": [85, None, 76, 88, None],
    "City": ["Delhi", "Chandigarh", "Ludhiana", None, "Amritsar"]
}
```

Perform:

1. Display the DataFrame.
2. Check for missing values.
3. Count missing values in each column.
4. Replace missing `Age` with the average age.
5. Replace missing `Marks` with the average marks.

---

### Q7. Statistical Analysis — 5 Marks

Using the DataFrame from Q6:

Find:

1. Average marks
2. Maximum marks
3. Minimum marks
4. Average age
5. Standard deviation of marks

---

# Part D — GroupBy and Sorting (10 Marks)

### Q8. GroupBy — 5 Marks

Create this DataFrame:

```python
data = {
    "Name": ["Aman", "Simran", "Raj", "Neha", "Karan", "Priya"],
    "Department": ["IT", "HR", "IT", "Finance", "HR", "IT"],
    "Salary": [40000, 35000, 45000, 50000, 38000, 48000]
}
```

Perform:

1. Find the average salary of each department.
2. Find the maximum salary of each department.
3. Find the minimum salary of each department.
4. Find the number of employees in each department.

---

### Q9. Sorting — 5 Marks

Using the same DataFrame:

1. Sort employees by salary in ascending order.
2. Sort employees by salary in descending order.
3. Display the employee with the highest salary.
4. Display the top 3 highest-paid employees.

---

# Part E — Real-World Pandas Task (5 Marks)

### Q10. Sales Analysis — 5 Marks

Create the following DataFrame:

```python
data = {
    "Product": ["Laptop", "Mobile", "Laptop", "Tablet", "Mobile", "Tablet"],
    "Sales": [50000, 30000, 45000, 20000, 35000, 25000],
    "Quantity": [2, 3, 1, 4, 2, 3],
    "City": ["Delhi", "Mumbai", "Delhi", "Chandigarh", "Mumbai", "Delhi"]
}
```

Answer the following:

1. Find the total sales.
2. Find the average sales.
3. Find the product with the highest sales.
4. Find total sales for each product.
5. Find total sales for each city.

---

## 📊 Marks Distribution

| Section   | Topic                     |  Marks |
| --------- | ------------------------- | -----: |
| A         | Pandas Basics             |     10 |
| B         | Filtering & Modification  |     15 |
| C         | Missing Data & Statistics |     10 |
| D         | GroupBy & Sorting         |     10 |
| E         | Real-World Analysis       |      5 |
| **Total** |                           | **50** |

### Topics covered

**DataFrame creation → head/tail → shape → dtypes → column selection → filtering → conditions → adding columns → modifying data → rename/drop → missing values → fillna → statistics → groupby → sorting → real-world analysis**

If you want, I can also create a **separate answer/solution sheet with complete Python code for all 10 questions**.


Here is the **complete solution sheet** for the 50-mark Pandas test, with simple and classroom-friendly code.

# 🐼 Pandas Practical Test — Complete Solution

## Q1. Create a DataFrame — 5 Marks

```python
import pandas as pd

data = {
    "Name": ["Aman", "Simran", "Raj", "Neha", "Karan", "Priya"],
    "Age": [21, 22, 20, 23, 21, 22],
    "City": ["Delhi", "Chandigarh", "Ludhiana", "Delhi", "Amritsar", "Chandigarh"],
    "Marks": [85, 92, 76, 88, 69, 95],
    "Department": ["IT", "HR", "IT", "Finance", "HR", "IT"]
}

df = pd.DataFrame(data)

# 1. First 3 rows
print(df.head(3))

# 2. Last 2 rows
print(df.tail(2))

# 3. Column names
print(df.columns)

# 4. Shape
print(df.shape)

# 5. Data types
print(df.dtypes)
```

---

# Q2. Selecting Data — 5 Marks

```python
# 1. Name and Marks columns
print(df[["Name", "Marks"]])

# 2. Details of Neha
print(df[df["Name"] == "Neha"])

# 3. Students with marks greater than 80
print(df[df["Marks"] > 80])

# 4. Students from Chandigarh
print(df[df["City"] == "Chandigarh"])
```

### Using `loc`

The same questions can also be solved using `loc`:

```python
print(df.loc[df["Name"] == "Neha"])

print(df.loc[df["Marks"] > 80])

print(df.loc[df["City"] == "Chandigarh"])
```

---

# Q3. Filtering Data — 5 Marks

### 1. Marks between 70 and 90

```python
result = df[(df["Marks"] >= 70) & (df["Marks"] <= 90)]

print(result)
```

### 2. Age greater than 21

```python
print(df[df["Age"] > 21])
```

### 3. IT department

```python
print(df[df["Department"] == "IT"])
```

### 4. Delhi or Chandigarh

```python
print(df[df["City"].isin(["Delhi", "Chandigarh"])])
```

### 5. Marks greater than 80 AND IT department

```python
result = df[(df["Marks"] > 80) & (df["Department"] == "IT")]

print(result)
```

---

# Q4. Add and Modify Columns — 5 Marks

### 1. Add Result column

```python
df["Result"] = df["Marks"].apply(
    lambda x: "Pass" if x >= 40 else "Fail"
)
```

### 2. Add Bonus column

```python
df["Bonus"] = df["Marks"].apply(
    lambda x: 1000 if x >= 90 else 500
)
```

### 3. Increase marks by 5

```python
df["Marks"] = df["Marks"] + 5
```

### 4. Display DataFrame

```python
print(df)
```

### Shorter alternative using `loc`

```python
df.loc[df["Marks"] >= 40, "Result"] = "Pass"
df.loc[df["Marks"] < 40, "Result"] = "Fail"

df.loc[df["Marks"] >= 90, "Bonus"] = 1000
df.loc[df["Marks"] < 90, "Bonus"] = 500
```

---

# Q5. Delete and Rename Columns — 5 Marks

```python
# Rename Marks to Score
df.rename(columns={"Marks": "Score"}, inplace=True)

# Rename Department to Dept
df.rename(columns={"Department": "Dept"}, inplace=True)

# Delete Bonus
df.drop("Bonus", axis=1, inplace=True)

print(df)
```

### Important

```python
axis=1
```

means **column**.

```python
axis=0
```

means **row**.

---

# Q6. Missing Values — 5 Marks

```python
import pandas as pd

data = {
    "Name": ["Aman", "Simran", "Raj", "Neha", "Karan"],
    "Age": [21, 22, None, 23, 21],
    "Marks": [85, None, 76, 88, None],
    "City": ["Delhi", "Chandigarh", "Ludhiana", None, "Amritsar"]
}

df = pd.DataFrame(data)

# 1. Display DataFrame
print(df)
```

### 2. Check missing values

```python
print(df.isnull())
```

### 3. Count missing values

```python
print(df.isnull().sum())
```

### 4. Replace missing Age with average age

```python
df["Age"] = df["Age"].fillna(df["Age"].mean())
```

### 5. Replace missing Marks with average marks

```python
df["Marks"] = df["Marks"].fillna(df["Marks"].mean())

print(df)
```

### Complete solution

```python
import pandas as pd

data = {
    "Name": ["Aman", "Simran", "Raj", "Neha", "Karan"],
    "Age": [21, 22, None, 23, 21],
    "Marks": [85, None, 76, 88, None],
    "City": ["Delhi", "Chandigarh", "Ludhiana", None, "Amritsar"]
}

df = pd.DataFrame(data)

print(df)

print(df.isnull())

print(df.isnull().sum())

df["Age"] = df["Age"].fillna(df["Age"].mean())

df["Marks"] = df["Marks"].fillna(df["Marks"].mean())

print(df)
```

---

# Q7. Statistical Analysis — 5 Marks

Using the DataFrame from Q6:

```python
# Average marks
print("Average Marks:", df["Marks"].mean())

# Maximum marks
print("Maximum Marks:", df["Marks"].max())

# Minimum marks
print("Minimum Marks:", df["Marks"].min())

# Average age
print("Average Age:", df["Age"].mean())

# Standard deviation
print("Standard Deviation:", df["Marks"].std())
```

### Useful Pandas functions

| Function  | Purpose            |
| --------- | ------------------ |
| `mean()`  | Average            |
| `max()`   | Maximum            |
| `min()`   | Minimum            |
| `std()`   | Standard deviation |
| `sum()`   | Total              |
| `count()` | Count              |

---

# Q8. GroupBy — 5 Marks

```python
import pandas as pd

data = {
    "Name": ["Aman", "Simran", "Raj", "Neha", "Karan", "Priya"],
    "Department": ["IT", "HR", "IT", "Finance", "HR", "IT"],
    "Salary": [40000, 35000, 45000, 50000, 38000, 48000]
}

df = pd.DataFrame(data)
```

### 1. Average salary by department

```python
print(df.groupby("Department")["Salary"].mean())
```

### 2. Maximum salary

```python
print(df.groupby("Department")["Salary"].max())
```

### 3. Minimum salary

```python
print(df.groupby("Department")["Salary"].min())
```

### 4. Number of employees

```python
print(df.groupby("Department")["Name"].count())
```

### One command for all four

```python
print(
    df.groupby("Department")["Salary"].agg(
        ["mean", "max", "min", "count"]
    )
)
```

This is a very useful **real-world Pandas technique**.

---

# Q9. Sorting — 5 Marks

### 1. Salary ascending

```python
print(df.sort_values("Salary"))
```

### 2. Salary descending

```python
print(df.sort_values("Salary", ascending=False))
```

### 3. Employee with highest salary

```python
print(df.loc[df["Salary"].idxmax()])
```

### 4. Top 3 highest-paid employees

```python
print(df.sort_values("Salary", ascending=False).head(3))
```

### Alternative

```python
print(df.nlargest(3, "Salary"))
```

---

# Q10. Sales Analysis — 5 Marks

```python
import pandas as pd

data = {
    "Product": ["Laptop", "Mobile", "Laptop", "Tablet", "Mobile", "Tablet"],
    "Sales": [50000, 30000, 45000, 20000, 35000, 25000],
    "Quantity": [2, 3, 1, 4, 2, 3],
    "City": ["Delhi", "Mumbai", "Delhi", "Chandigarh", "Mumbai", "Delhi"]
}

df = pd.DataFrame(data)

print(df)
```

### 1. Total sales

```python
print("Total Sales:", df["Sales"].sum())
```

**Output:**

```text
Total Sales: 205000
```

---

### 2. Average sales

```python
print("Average Sales:", df["Sales"].mean())
```

**Output:**

```text
Average Sales: 34166.67
```

---

### 3. Product with highest sales

```python
print(df.loc[df["Sales"].idxmax()])
```

**Output:**

```text
Product       Laptop
Sales          50000
Quantity            2
City            Delhi
```

---

### 4. Total sales for each product

```python
print(df.groupby("Product")["Sales"].sum())
```

**Output:**

```text
Product
Laptop     95000
Mobile     65000
Tablet     45000
```

---

### 5. Total sales for each city

```python
print(df.groupby("City")["Sales"].sum())
```

**Output:**

```text
City
Chandigarh    20000
Delhi        120000
Mumbai        65000
```

---

# ⭐ Bonus Challenge

For students who finish early, give them this additional task:

### Q11. Advanced Pandas Challenge

Using the Sales DataFrame:

1. Calculate **Total Revenue** using:

   ```text
   Sales × Quantity
   ```

2. Find the product having the highest total revenue.

3. Find the city having the highest total revenue.

4. Sort the DataFrame according to total revenue.

### Solution

```python
df["Total_Revenue"] = df["Sales"] * df["Quantity"]

print(df)
```

Find highest revenue:

```python
print(df.loc[df["Total_Revenue"].idxmax()])
```

Total revenue by product:

```python
print(
    df.groupby("Product")["Total_Revenue"].sum()
)
```

Total revenue by city:

```python
print(
    df.groupby("City")["Total_Revenue"].sum()
)
```

Sort by revenue:

```python
print(
    df.sort_values("Total_Revenue", ascending=False)
)
```

This solution covers the main intermediate Pandas skills: **DataFrame creation, selection, filtering, `loc`, `isin`, `apply`, `lambda`, `rename`, `drop`, `isnull`, `fillna`, statistics, `groupby`, `agg`, `sort_values`, `idxmax`, `nlargest`, and calculated columns**.
