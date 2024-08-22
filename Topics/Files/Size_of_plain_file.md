# Challenge: file size of a plain file.

## Description

Write a Python program to get the file size of a plain file.

## Solution

```python
# Provide your solution here.
def file():
    import os
    with open('test.txt','r') as f:
        statinfo = os.stat('test.txt')
        return statinfo.st_size

if __name__ == '__main__':
    result = file()
    print(result)
