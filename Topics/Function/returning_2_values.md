# Challenge: Returning more than one values

## Description

Define a function that can return multiple values

## Solution

```python
# Provide your solution here.
def ret_mul_val(a,b):
    c = a + b
    d = a - b
    return c,d

if __name__ == "__main__":
    x , y = ret_mul_val(10,5)
    print("addition of a and b is ",+ x)
    print("subraction of a and b is",+ y)

