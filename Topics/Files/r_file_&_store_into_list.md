# Challenge: read a file line by line and store it into a list

## Description

Write a Python program to read a file line by line and store it into a list.

## Solution

```python
# Provide your solution here.
def file():
    lst = []
    with open('test.txt','r') as f:
        for line in f:
            lst.append(line)
        print(lst)

if __name__ == '__main__':
    file()
