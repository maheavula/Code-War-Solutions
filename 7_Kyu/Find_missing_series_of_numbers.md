# Challenge: Find missing series of numbers 

## Description

You will get an array of numbers.

Every preceding number is smaller than the one following it.

Some numbers will be missing, for instance:

[-3,-2,1,5] //missing numbers are: -1,0,2,3,4

Your task is to return an array of those missing numbers:

[-1,0,2,3,4]

## Solution

```python
# Provide your solution here.
def find_missing_numbers(ss):
    if ss == []:
        return []
    else:
        lst = [i for i in range(ss[0], ss[-1]+1)]
        return [i for i in lst if i not in ss]
