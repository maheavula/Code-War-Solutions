# Challenge: Find the capitals

## Description

Write a function that takes a single non-empty string of only lowercase and uppercase ascii letters (word) as its argument, and returns an ordered list containing the indices of all capital (uppercase) letters in the string.

## Example (Input --> Output)

"CodEWaRs" --> [0,3,4,6]

## Solution

```python
# Provide your solution here.
def capitals(word):
    lst = []
    j=0
    for i in word:
        if i.isupper():
            lst.append(j)
        j += 1
    return lst
        
