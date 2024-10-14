# Challenge:  Reduce but Grow

## Description

Given a non-empty array of integers, return the result of multiplying the values together in order. Example:

[1, 2, 3, 4] => 1 * 2 * 3 * 4 = 24

## Solution

```python
# Provide your solution here.
def grow(arr):
    fact = 1
    for i in arr:
        fact *= i
    return fact
