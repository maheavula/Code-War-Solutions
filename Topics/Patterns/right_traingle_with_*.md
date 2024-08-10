# Challenge: print right traingle with * pattern

## Description

write a program to print this pattern

![righttraingle](https://github.com/user-attachments/assets/78028a91-ae99-476d-8975-9262d1faafd9)


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

pattern(6)
    


