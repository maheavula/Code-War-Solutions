# Challenge: print this pattern


## Description

write a program to print above pattern

![patternsomething](https://github.com/user-attachments/assets/6e7c9676-d572-4638-bf47-fba35ec8c724)

## Solution

```python
# Provide your solution here.
res_str = ""

for r in range(0,8):
    for c in range(0,7):
        if (r == 0 or r == 7 or r == 4) or ((r != 0) and (c == 0 or c == 3 or c == 6)):
            res_str += "0"
        else:
            res_str += " "
    res_str += '\n'

print(res_str)
