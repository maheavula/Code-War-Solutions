# Challenge: Build Tower

## Description

Build a pyramid-shaped tower, as an array/list of strings, given a positive integer number of floors. A tower block is represented with "*" character.

For example, a tower with 3 floors looks like this:

[
  "  *  ",
  " *** ", 
  "*****"
]
And a tower with 6 floors looks like this:

[
  "     *     ", 
  "    ***    ", 
  "   *****   ", 
  "  *******  ", 
  " ********* ", 
  "***********"
]

## Solution

```python
# Provide your solution here.
def tower_builder(n_floors):
    lst = ""
    for r in range(1, n_floors+1):
        for c in range(n_floors - r):
            lst += " "
        for k in range(r*2-1):
            lst += "*"
        for c in range(n_floors - r):
            lst += " "
        lst += "\n"
    lstt = [lst[i:i+r*2-1] for i in range(0, len(lst), r*2-1)]
    return lstt
