# Challenge: Generate 26 text files

## Description

Write a Python program to generate 26 text files named A.txt, B.txt, and so on up to Z.txt.

## Solution

```python
# Provide your solution here.
import string, os
def file():
    for letter in string.ascii_uppercase:
        with open(letter + '.text', 'w') as file:
            file.writelines(letter)

if __name__ == '__main__':
    file()
