# Challenge: print numerical pattern

## Description

write a program to print this pattern

![pattern3](https://github.com/user-attachments/assets/a1715065-9f3f-4a74-9c63-53b3f3ffeb35)

## Solution

```python
# Provide your solution here.
rows = 10
for r in range(1,rows):
    for j in range(1, r+1):
        print(r*j, end=" ")
    print(" ")

    


