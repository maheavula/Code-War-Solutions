# Challenge: Square(n) of sum

## Description

Complete the square sum function so that it squares each number passed into it and then sums the results together.

## For example

for [1, 2, 2] it should return 9 because 1^2+2^2+2^2= 9.

## Solution

```python
# Provide your solution here.
def square_sum(numbers):
    return sum([i**2 for i in numbers])
