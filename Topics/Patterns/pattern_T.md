# Challenge: print pattern T

## Description

write a program to print pattern T

## Solution

```python
# Provide your solution here.
res_str = ""

for r in range(0,7):
    for c in range(0,7):
        if (r == 0) or (c == 3):
            res_str += "*"
        else:
            res_str += " "
    res_str += '\n'
print(res_str)
