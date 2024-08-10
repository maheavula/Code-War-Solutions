# Challenge: print square pattern with numbers

## Description

write a program to print this pattern

![squarenumber](https://github.com/user-attachments/assets/d924b151-ef41-4654-8d75-4b2b76aa895d)

## Solution

```python
# Provide your solution here.
def pattern(rows):
    for r in range(1, rows):
        for c in range(1, rows):
            if c <= r:
                print(r, end=" ")
            else:
                print(c, end=" ")
        print(" ")

pattern(6)

    


