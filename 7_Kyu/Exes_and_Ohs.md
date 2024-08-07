# Challenge: Exes and Ohs

## Description

Check to see if a string has the same amount of 'x's and 'o's. The method must return a boolean and be case insensitive. The string can contain any char.

## Examples input/output:

XO("ooxx") => true

XO("xooxx") => false

XO("ooxXm") => true

XO("zpzpzpp") => true // when no 'x' and 'o' is present should return true

XO("zzoo") => false

## Solution

```python
# Provide your solution here.
def xo(s):
    countx = 0
    counto = 0
    count = 0
    for i in s:
        if i == 'o' or i == 'O':
            counto += 1
        elif i == 'x' or i == 'X':
            countx += 1
        elif i != 'o' or i != 'O' or i != 'x' or i != 'X':
            pass
        else:
            return False
    if countx == counto:
        return True
    else:
        return False
        
