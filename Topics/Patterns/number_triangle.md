# Challenge: print number triangle pattern

## Description

write a program to print this pattern

![numbertraingle](https://github.com/user-attachments/assets/3dcbd066-949f-424f-bd3b-0a411e678cb2)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for r in range(1, rows):
        num = 1
        for j in range(rows, 0, -1):
            if j > r:
                print(" ", end=" ")
            else:
                print(num, end=" ")
                num += 1
        print(" ")

pattern(6)

    


