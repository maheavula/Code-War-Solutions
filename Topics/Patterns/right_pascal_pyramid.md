# Challenge: print right pascal pyramid pattern

## Description

write a program to print this pattern


![rightpascal](https://github.com/user-attachments/assets/2e197ced-0211-4a12-853c-694da6e93ac1)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(rows):
        for j in range(rows, 0, -1):
            if j > i:
                print(" ", end=" ")
            else:
                print("*", end=" ")
        print(" ")
    for i in range(rows):
        for j in range(rows):
            if i > j:
                print(" ", end=" ")
            else:
                print("*", end=" ")
        print(" ")

pattern(6)




    


