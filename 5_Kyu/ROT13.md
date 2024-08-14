# Challenge: ROT13

## Description

ROT13 is a simple letter substitution cipher that replaces a letter with the letter 13 letters after it in the alphabet. ROT13 is an example of the Caesar cipher.

Create a function that takes a string and returns the string ciphered with Rot13. If there are numbers or special characters included in the string, they should be returned as they are. Only letters from the latin/english alphabet should be shifted, like in the original Rot13 "implementation".

Please note that using encode is considered cheating.

## Solution

```python
# Provide your solution here.
def rot13(string):
    alp_upper = [chr(c) for c in range(65, 91)]
    alp_lower = [chr(c) for c in range(97, 123)]
    nw_sting = ""
    for char in string:
        if char.isupper():
            ind1 = alp_upper.index(char)
            nw_ind1 = (ind1+13) % 26
            nw_sting += alp_upper[nw_ind1]
        elif char.islower():
            ind2 = alp_lower.index(char)
            nw_ind2 = (ind2 + 13) % 26
            nw_sting += alp_lower[nw_ind2]
        else:
            nw_sting += char
    return nw_sting

