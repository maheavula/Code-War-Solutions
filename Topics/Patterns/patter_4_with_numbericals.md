# Challenge: print numerical pattern

## Description

write a program to print this pattern

![pattern4](https://github.com/user-attachments/assets/e6acd0a9-af87-41eb-bf9e-0d8d27f4ef16)


## Solution

```python
# Provide your solution here.
rows = 6
for r in range(1,rows):
    for j in range(r):
        print(r, end=" ")
    print(" ")

    


