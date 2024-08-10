# Challenge: print reverse pyramid number pattern

## Description

write a program to print this pattern

![reversepyramidnums](https://github.com/user-attachments/assets/bb099bbb-0dc5-4de3-b6dd-342f07193833)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(1,rows):
        for j in range(i,0,-1):
            print(j, end=" ")
        print(" ")


pattern(6)

    


