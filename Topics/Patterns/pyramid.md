# Challenge: print pyramid pattern

## Description

write a program to print this pattern

![pyramid](https://github.com/user-attachments/assets/9979a9a2-8bc5-4ef5-92b2-615f5285faca)



## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(rows):
        for j in range(rows-i):
            print(" ", end=" ")

        for k in range(2 * i+1):
            print("*", end=" ")
        print(" ")


pattern(6)


