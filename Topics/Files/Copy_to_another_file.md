# Challenge: copy the contents of a file to another file .

## Description

Write a Python program to copy the contents of a file to another file .

## Solution

```python
# Provide your solution here.
def file():
    from shutil import copyfile
    copyfile('test.txt', 'unit testing.py')

    f = open('unit testing.py')
    print(f.read())
    
if __name__ == '__main__':
    file()
