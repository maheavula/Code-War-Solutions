# Challenge: print pattern M

## Description

write a program to print pattern M

## Solution

```python
# Provide your solution here.
res_str = ""

for r in range(0,5):
    for c in range(0,6):
        if (c == 0 or c == 5)  or ((r == 1)  and (c == 1 or c == 4) or (r == 2) and (c == 2 or c == 3)):
            res_str += "*"
        else:
            res_str += " "
    res_str += '\n'

print(res_str)
