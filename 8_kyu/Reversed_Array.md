# Challenge: Convert number to reversed array of digits

## Description

Given a random non-negative number, you have to return the digits of this number within an array in reverse order.

## Example(Input => Output):

35231 => [1,3,2,5,3]
0 => [0]

## Solution

```python
# Provide your solution here.
def digitize(n):
    lst = []
    word = str(n)
    for i in word[::-1]:
        
        lst.append(int(i))
    return lst

