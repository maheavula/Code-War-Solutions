# Challenge: print downward pyramid with * pattern

## Description

write a program to print this pattern

![downpyramidwith](https://github.com/user-attachments/assets/20debc1a-70c8-4fec-9cdb-62917d71f226)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    return "\n".join(["* " * i for i in range(rows,0,-1)])
result = pattern(6)
print(result)
    


