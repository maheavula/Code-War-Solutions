# Challenge: Longest word in file

## Description

Write a python program to find the longest words.

## Solution

```python
# Provide your solution here.
def file():
    with open('test.txt','r') as f:
        words = f.read().split()
        max_len = len(max(words, key=len))
        return [word for word in words if len(word) == max_len]

if __name__ == '__main__':
    result = file()
    print(result)
