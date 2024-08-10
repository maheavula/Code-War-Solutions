# Challenge: print simple half pyramid pattern

## Description

write a program to print this pattern

![haldpyramid](https://github.com/user-attachments/assets/72e47fe4-ffe7-4806-9fee-433d7ad6c927)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(rows):
        for j in range(i+1):
            print("*", end=" ")
        print(" ")

pattern(6)

    


