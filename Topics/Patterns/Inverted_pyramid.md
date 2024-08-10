# Challenge: print numerical pattern

## Description

write a program to print this pattern

![inverted_pyramid](https://github.com/user-attachments/assets/c34c8268-543d-4e8a-962d-35f53482c8bb)


## Solution

```python
# Provide your solution here.
rows = 6
for r in range(1,rows):
    for j in range(r,rows ):
        print(r, end=" ")
    print(" ")
    


