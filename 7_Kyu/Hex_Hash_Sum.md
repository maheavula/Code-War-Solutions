# Challenge: Hex Hash Sum

## Description

Complete the function that accepts a valid string and returns an integer.

Wait, that would be too easy! Every character of the string should be converted to the hex value of its ascii code, then the result should be the sum of the numbers in the hex strings (ignore letters).

Examples

"Yo" ==> "59 6f" ==> 5 + 9 + 6 = 20

"Hello, World!"  ==> 91

"Forty4Three"    ==> 113


## Solution

```python
# Provide your solution here.
def hex_hash(code):
    si = ""
    for i in code:
        si += hex(ord(i))[2:]
    tn = 0
    for i in si:
        if i.isdigit():
            tn += int(i)
    return tn
