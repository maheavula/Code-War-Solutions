# Challenge: print right down mirror with * pattern

## Description

write a program to print this pattern


![rightdownmirror](https://github.com/user-attachments/assets/c6c2ed54-765e-43f4-b49d-357438fa1f89)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for r in range(rows):
        for c in range(rows):
            if r > c:
                print(" ", end=" ")
            else:
                print("*", end=" ")
        print(" ")

pattern(6)

    


