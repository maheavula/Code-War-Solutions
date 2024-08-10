# Challenge: print reverse pyramid pattern

## Description

write a program to print this pattern

![reversepyramid](https://github.com/user-attachments/assets/0c357e4a-162f-48bd-8af4-4f282a591673)

## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(rows,0,-1):
        for j in range(rows-i):
            print(" ", end=" ")

        for k in range(2 * i-1):
            print("*", end=" ")
        print(" ")

pattern(6)


