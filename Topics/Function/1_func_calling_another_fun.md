# Challenge: One function can call another function

## Description

One function can call another function in python

## Solution

```python
# Provide your solution here.
def m1():
    print("first function")
def m2():
    print("second function")
    m1()

if __name__ == "__main__":
    m2()

