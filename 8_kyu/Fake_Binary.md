# Challenge: Fake Binary

## Description

Given a string of digits, you should replace any digit below 5 with '0' and any digit 5 and above with '1'. Return the resulting string.

Note: input will never be an empty string

## Solution

```python
# Provide your solution here.
def fake_bin(x):
    st = ""
    for i in x:
        if int(i) < 5:
            st += "0"
        else:
            st += "1"
            
    return st
