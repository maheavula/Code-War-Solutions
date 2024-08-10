# Challenge: print left pascal pyramid pattern

## Description

write a program to print this pattern


![leftpascalpyramid](https://github.com/user-attachments/assets/bd4fc4fb-d17b-49f4-bcb8-cbc047087e73)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(0,rows):
        for j in range(i+1):
            print("*", end=" ")
        print()
    for m in range(rows-1,0,-1):
        for j in range(m):
            print("*", end=" ")
        print()

pattern(6)


    


