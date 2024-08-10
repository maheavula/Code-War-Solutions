# Challenge: print two pyramids of stars pattern

## Description

write a program to print this pattern


![twopyramidstars](https://github.com/user-attachments/assets/cfb20924-6b27-4266-930f-aeb8a6d85dcb)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(0,rows):
        for j in range(i+1):
            print("*", end=" ")
        print()
    print("\n")
    for m in range(rows,0,-1):
        for j in range(m):
            print("*", end=" ")
        print()

pattern(6)
    


