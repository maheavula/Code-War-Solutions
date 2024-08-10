# Challenge: print alternative number pyramid pattern

## Description

write a program to print this pattern

![alternative_pyramid](https://github.com/user-attachments/assets/6d0d31e2-3fee-4d4d-9b0e-bb9aae45d905)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    i = 1
    while i <= rows:
        for m in range(1, rows):
            for j in range(m):
                print(i, end=" ")
            i += 2
            print(" ")

pattern(6)

    


