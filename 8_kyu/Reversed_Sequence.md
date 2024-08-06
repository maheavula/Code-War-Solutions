# Challenge: Reversed Sequence

## Description

Build a function that returns an array of integers from n to 1 where n>0.

## Example :
``n=5 --> [5,4,3,2,1]``

## Solution

```python
# Provide your solution here.
def reverse_seq(n):
    lst = []
    while n != 0:
        lst.append(n)
        n -= 1
    return lst
