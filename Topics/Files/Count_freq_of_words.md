# Challenge: Count the frequency of words

## Description

Write a Python program to count the frequency of words in a file.

## Solution

```python
# Provide your solution here.
from collections import Counter
def file():
    with open('test.txt','r') as f:
        return Counter(f.read().split())

if __name__ == '__main__':
    result = file()
    print(result)
