# Challenge: Pattern of H

## Description

write a program to print H pattern

## Solution

```python
# Provide your solution here.

res_str = ""
for r in range(0,16):
    for c in range(0,16):
        if (c <= 4) or (c >= 11) or (r >= 6) and (r <= 9) and (c >= 1 and c ):
            res_str += "*"
        else:
            res_str += " "
    res_str += '\n'
print(res_str)

```
