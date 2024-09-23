---
Title: '.around()'
Description: 'Rounds each element in an array to the specified number of decimals.'
Subjects:
  - 'Computer Science'
  - 'Data Science'
Tags:
  - 'Arrays'
  - 'Functions'
  - 'Math'
  - 'NumPy'
CatalogContent:
  - 'learn-python-3'
  - 'paths/computer-science'
  - 'paths/data-science'
  - 'paths/data-science-foundations'
---

In NumPy, the **`.around()`** function rounds each element in an array to the specified number of decimals. By default, it rounds to the nearest integer if no decimal places are provided.

This function is useful for controlling the precision of floating-point values in NumPy arrays.

## Syntax

```pseudo
numpy.around(input_value, decimals=0, out=None)
```

- `input_value`: The input array or scalar containing the elements to be rounded.
- `decimals` (optional): The number of decimal places to round to. Default is 0, meaning rounding to the nearest integer. If negative, it rounds to the left of the decimal point.
- `out` (optional): A location where the result of the rounding will be stored. If no value is provided, a new array is returned.

## Example

```py
# Importing the 'numpy' library as 'np'
import numpy as np

# Creating an array of floating-point numbers
arr = np.array([1.2345, 2.718, -0.5678, -3.1416])

# Applying the around function
result = np.around(arr)

print(result)
```

The above example code results in the following output:
```shell
[ 1.  3. -1. -3.]
```

## Example 2

This example shows how to round to a specific number of decimal places using `.around()`:

```py
# Importing the 'numpy' library as 'np'
import numpy as np

# Creating an array of floating-point numbers
arr = np.array([1.2345, 2.718, -0.5678, -3.1416])

# Rounding to 2 decimal places
result = np.around(arr, decimals=2)

print(result)
```

The above example code results in the following output:

```shell
[ 1.23  2.72 -0.57 -3.14]
```

## Codebyte Example

```codebyte/python
import numpy as np

arr = np.array([1.234, 2.678, -0.567, -1.999])

result = np.around(arr, decimals=1)

print(result)
```
