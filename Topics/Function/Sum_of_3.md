# Challenge: Sum of three numbers

## Description

Write a Python function to find the maximum of three numbers.

## Solution

```python
# Provide your solution here.
def max(a,b,c):
    if a > b and a > c:
        return a
    elif b > c and b > a:
        return b
    else:
        return c

if __name__ == "__main__":
    result = max(9,8,6)
    print(result)
