# Challenge: If you can't sleep, just count sheep!!

## Description

Given a non-negative integer, 3 for example, return a string with a murmur: `"1 sheep...2 sheep...3 sheep...".` Input will always be valid, i.e. no negative integers.

## Solution

```python
# Provide your solution here.
def count_sheep(n):
    # your code
    sum =""
    for i in range(1,n+1):
        sum += f'{i}'+ " sheep..."
    return sum
