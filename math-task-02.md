
# Math Functions Script

This Python script demonstrates the use of common functions from Python’s built-in `math` module.

## Features

The script performs the following operations:

- Calculates the **square root** of a number.
- Rounds numbers **up** and **down** using `ceil()` and `floor()`.
- Prints the value of **π (pi)** using `math.pi`.

## Code

```python
import math

# Square root of 64
x = math.sqrt(64)
print(x)                # Outputs: 8.0

# Ceiling and floor operations
a = 1.4
z1 = math.ceil(23.9)    # Rounds up to 24
z2 = math.floor(a)      # Rounds down to 1
print(z1)
print(z2)

# Value of pi
p = math.pi
print(p)                # Outputs: 3.141592653589793
````

## Output

```
8.0
24
1
3.141592653589793
```

## Explanation

* `math.sqrt(64)` returns the square root of 64 → `8.0`.
* `math.ceil(23.9)` rounds **up** to `24`.
* `math.floor(1.4)` rounds **down** to `1`.
* `math.pi` gives the mathematical constant π → approximately `3.14159`.

## Requirements

* Python 3.x
* No external libraries required (uses built-in `math` module)
