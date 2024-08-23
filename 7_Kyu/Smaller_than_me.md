# Challenge: How many are smaller than me?

## Description

Write a function that given, an array arr, returns an array containing at each index i the amount of numbers that are smaller than arr[i] to the right.

## For example:

* Input [5, 4, 3, 2, 1] => Output [4, 3, 2, 1, 0]
* Input [1, 2, 0] => Output [1, 1, 0]

## Solution

```python
# Provide your solution here.
def smaller(arr):
    lst = []
    for i, j in enumerate(arr):
        count = 0
        for k in arr[i+1:]:
            if j > k:
                count += 1
        lst.append(count)
    return lst
