# Challenge: Reading entire file content

## Description

Write a Python program to read an entire text file.

## Solution

```python
# Provide your solution here.
def file():
    with open('test.txt','r') as f:
        content = f.read()
        print(content)

if __name__ == '__main__':
    file()
