# Challenge: Default Arguments

## Description

Default Arguments in Python 

## Solution

```python
# Provide your solution here.
def default_args(item, price=1000):
    print(item, "cost is ", price)

if __name__ == "__main__":
    default_args(item="bangles")
    default_args(item="shirt", price=100)
