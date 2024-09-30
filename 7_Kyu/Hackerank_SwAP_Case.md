# Challenge: Hackerank_Swap_Case

## Description
ou are given a string and your task is to swap cases. In other words, convert all lowercase letters to uppercase letters and vice versa.

## For Example:

Www.HackerRank.com → wWW.hACKERrANK.COM

Pythonist 2 → pYTHONIST 2  

## Solution

```python
# Provide your solution here.
def swap_case(s):
    new_s = ""
    for i in s:
        if i.islower():
            new_s += i.upper()
        elif i.isupper():
            new_s += i.lower()
        else:
            new_s += i
            
    return new_s

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
