# Challenge: print pattern Z

## Description

write a program to print pattern Z

## Solution

```python
# Provide your solution here.
res_str = ""

for r in range(0,5):
    for c in range(0,5):
        if (r == 0 or r == 4) or (c == 3 and r != 2 and r != 3) or (c == 2 and r == 2) or (c == 1 and r != 1 and r != 2):
            res_str += "*"
        else:
            res_str += " "
    res_str += '\n'
print(res_str)
