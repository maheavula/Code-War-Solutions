# Challenge: print reverse number 10 to 1 pattern

## Description

write a program to print this pattern

![reverse_10_1](https://github.com/user-attachments/assets/4a14da9b-00f0-475a-86b0-351df3136a52)


## Solution

```python
# Provide your solution here.
def pattern(start,stop):
    cur_val = stop
    for r in range(2,6):
        for c in range(start,stop):
            cur_val -= 1
            print(cur_val, end=" ")
        print(" ")
        start = stop
        stop += r
        cur_val = stop


pattern(1,2)



