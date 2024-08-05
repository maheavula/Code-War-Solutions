# Challenge: Find the missing number

## Description

You are given an unsorted array containing all the integers from 0 to 100 inclusively. However, one number is missing. Write a function to find and return this number. What are the time and space complexities of your solution?

## Solution

```python
# Provide your solution here.
def missing_no(nums):
    sum = 0
    summ = 5050
    for i in nums:
        sum += i
    return summ - sum
