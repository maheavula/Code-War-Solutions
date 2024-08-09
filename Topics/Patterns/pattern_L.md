# Challenge: print pattern L

## Description

write a program to print pattern L

## Solution

```python
# Provide your solution here.
res_str = ""

for r in range(0,8):
    for c in range(0,7):
        if (c == 0) or (r == 7):
            res_str += "*"
        else:
            res_str += " "
    res_str += "\n"

print(res_str)
