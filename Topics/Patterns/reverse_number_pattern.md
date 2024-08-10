# Challenge: print reverse number pattern

## Description

write a program to print this pattern

![reverse_word](https://github.com/user-attachments/assets/032bb33b-3c86-4934-baae-324e0eb54699)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    for i in range(rows, 0, -1):
        for j in range(i):
            print(i, end=" ")
        print(" ")
pattern(6)


    


