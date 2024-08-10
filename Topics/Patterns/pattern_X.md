# Challenge: print a pattern X

## Description

write a program to print pattern X

## Solution

```python
# Provide your solution here.
res_str = ""

for r in range(0,5):
    for c in range(0,5):
        if (c == 0 and r != 1 and  r != 2 and r != 3) or (c == 4 and r != 1 and  r != 2 and r != 3) or (c == 1 and r != 0 and r != 2 and r != 4) or r == 2 and (c != 0 and c != 1 and c != 3 and c != 4) or  (c == 3 and r != 0 and r != 2 and r != 4):
            res_str += "*"
        else:
            res_str += " "
    res_str += '\n'
print(res_str)
