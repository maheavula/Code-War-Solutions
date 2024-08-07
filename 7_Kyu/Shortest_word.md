# Challenge: Shortest word

## Description

Simple, given a string of words, return the length of the shortest word(s).

String will never be empty and you do not need to account for different data types.

## Solution

```python
# Provide your solution here.
def find_short(s):
    lst = []
    stp = s.split()
    for i in stp:
        lst.append(len(i))
    return min(lst)
