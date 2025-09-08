# Date and Time Information Script

This simple Python script demonstrates how to use the built-in `datetime` module to extract and format the current date and time.

## Features

The script does the following:

- Gets the current date and time.
- Prints the full date and time.
- Extracts and prints:
  - The current **year**
  - The full **weekday name** (e.g., Monday)
  - The abbreviated **weekday name** (e.g., Mon)
  - The **weekday number** (0 = Sunday, 6 = Saturday)
  - The **day of the month**
  - The abbreviated **month name** (e.g., Sep)

## Code

```python
import datetime

x = datetime.datetime.now()

print(x)                    # Full date and time
print(x.year)               # Year (e.g., 2025)
print(x.strftime("%A"))     # Full weekday name (e.g., Monday)
print(x.strftime("%a"))     # Abbreviated weekday name (e.g., Mon)
print(x.strftime("%w"))     # Weekday number (0 = Sunday, 6 = Saturday)
print(x.strftime("%d"))     # Day of the month (e.g., 08)
print(x.strftime("%b"))     # Abbreviated month name (e.g., Sep)
````

## Output Example

If run on **Monday, September 8, 2025**, the output might look like this:

```
2025-09-08 14:23:45.123456
2025
Monday
Mon
1
08
Sep
```

(Note: The exact date and time will vary depending on when you run the script.)

## Requirements

* Python 3.x (No additional libraries needed)
