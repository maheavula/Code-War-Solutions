# Challenge: print pattern U

## Description

write a program to print pattern U

## Solution

```python
# Provide your solution here.
res_str = ""

for r in range(0,11):
    for c in range(0,11):
        if c == 0 and r != 10 or c == 10 and r != 10 or (c != 0 and c != 10) and r == 10:
            res_str += "*"
        else:
            res_str += " "
    res_str += '\n'
print(res_str)
