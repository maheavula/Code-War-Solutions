# Challenge: Pass function as a parameter to another function

## Description

Pass function as a parameter to another function

## Solution

```python
# Provide your solution here.
def display(a):
    print("display something in this function")

def message():
    print("message is display")

if __name__ == "__main__":
    display(message())
