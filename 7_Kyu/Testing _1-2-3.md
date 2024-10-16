# Challenge: Testing 1-2-3

## Description

Your team is writing a fancy new text editor and you've been tasked with implementing the line numbering.

Write a function which takes a list of strings and returns each line prepended by the correct number.

The numbering starts at 1. The format is n: string. Notice the colon and space in between.

Examples: (Input --> Output)

[] --> []

["a", "b", "c"] --> ["1: a", "2: b", "3: c"]

## Solution

```python
# Provide your solution here.
def number(lines):
    dict = {}
    l = len(lines)
    j = 0
    for i in range(1,l+1):
        dict[i] = lines[j]
        j += 1
    return [f"{keys}: {values}" for keys, values in dict.items()]
