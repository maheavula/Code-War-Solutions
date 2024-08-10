# Challenge: print diamond pattern

## Description

write a program to print this pattern


![diamond](https://github.com/user-attachments/assets/dbb67377-0971-4323-a518-4297e7ca650b)


## Solution

```python
# Provide your solution here.
# Provide your solution here.
def pattern(rows):
    for i in range(rows):
        for j in range(rows-i-1):
            print(" ", end=" ")

        for k in range(2 * i+1):
            print("*", end=" ")
        print(" ")
    for i in range(rows, 0, -1):
        for j in range(rows - i):
            print(" ", end=" ")

        for k in range(2 * i-1):
            print("*", end=" ")
        print(" ")


pattern(6)

    
