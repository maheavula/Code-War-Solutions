# Challenge: print inverted half pyramid pattern

## Description

write a program to print this pattern

![2024-08-10 15_45_48-mal detect 1 – C__Users_91630_AppData_Roaming_JetBrains_PyCharmCE2023 2_scratche](https://github.com/user-attachments/assets/d3efc28c-4563-4c7c-a1a5-f705e30dceb9)


## Solution

```python
# Provide your solution here.
def pattern(rows):
    num = rows
    for r in range(0,rows):
        b = 0
        for j in range(r, rows+1):
            print(b, end=" ")
            b += 1
        print(" ")

pattern(5)



    


