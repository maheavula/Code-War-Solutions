# Challenge: print different reverse number pyramid pattern

## Description

write a program to print this pattern

![anotherpyramidnum](https://github.com/user-attachments/assets/412a916a-855e-4318-9f00-3d33f59c5b6e)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(rows,0, -1):
        for j in range(i,0,-1):
            print(j, end=" ")
        print(" ")


pattern(6)

    


