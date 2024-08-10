# Challenge: print pyramid with same digit 
## Description

write a program to print this pattern

![same_digit_pyramid](https://github.com/user-attachments/assets/8632cc58-c416-471e-a95a-042e5106e019)

## Solution

```python
# Provide your solution here.
rows = 6
num = rows
for r in range(1,rows):
    for j in range(r,rows ):
        print(num, end=" ")
    print(" ")

    


