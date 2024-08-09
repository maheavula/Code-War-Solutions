# Challenge: print pattern D

## Description

write a program to print D

## Solution

```python
# Provide your solution here.
res_str = ""

for r in range(0,8):
    for c in range(0,7):
        if ((c == 0 or c == 6) and r != 7 and r != 0) or (r == 0 or r == 7) and (c >= 0 and c <= 5):
            res_str += "*"
        else:
            res_str += " "
    res_str += '\n'

print(res_str)
