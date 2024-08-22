# Challenge: Write and display the content

## Description

Write a Python program to append text to a file and display the text.

## Solution

```python
# Provide your solution here.
def file():
    with open('test.txt','w') as f:
        f.write("this is new line of content")
    ff = open('test.txt') #it opens file in read mode
    print(ff.read())

if __name__ == '__main__':
    file()
