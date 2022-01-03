# 2022 January 3

## Problem Statement
Write a Python function to convert temperatures from fahrenheit to celsius. More specifically, your function should be able to read in a list of unspecified length and print out the celsius temperature for each item.

## Solution
Since the problem statement does not specify typing, we will create two different python functions: an integer input and output function that rounds the output per standard mathematic rounding using the python `round` function, and a float (which includes integer typing in python 3) input and output function that doesn't round the values.

### Integer Implementation
```
def f_to_c_int(temps: list[int]) -> list[int]:
    output_list = []
    for temp in temps:
        output_list.append(round(((temp-32)*(5/9))))
    return output_list
```

### Float Implementation
```
def f_to_c_float(temps: list[float]) -> list[float]:
    output_list = []
    for temp in temps:
        output_list.append(((temp-32)*(5/9)))
    return output_list
```