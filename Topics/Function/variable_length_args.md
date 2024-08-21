# Challenge: Variable-length argument in python

## Description

Variable-length argument in python

## Solution

```python
# Provide your solution here.
def total_cost(x, *y):
    sum = 0
    for i in y:
        sum += i
    print(x + sum)

if __name__ == "__main__":
    total_cost(10, 100, 100)

