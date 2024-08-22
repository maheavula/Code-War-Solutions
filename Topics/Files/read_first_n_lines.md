# Challenge: Read first n lines of file

## Description

Write a Python program to read first n lines of a file.

## Solution

```python
# Provide your solution here.
def file(n):
    from  itertools import islice
    with open('test.txt','r') as f:
        for line in islice(f, n):
            print(line)

if __name__ == '__main__':
    file(2)
