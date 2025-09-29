```

import mysql.connector

# Connect to MySQL
conn = mysql.connector.connect(
    host="localhost",
    user="root",
    password="",
    database="test"   # replace with your database name
)

cursor = conn.cursor()

# Run query
cursor.execute("SELECT * FROM costomers")

# Fetch results
for row in cursor.fetchall():
    print(row)

cursor.close()
conn.close()

```
