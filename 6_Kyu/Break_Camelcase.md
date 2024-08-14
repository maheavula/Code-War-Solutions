
# Challenge: Break Camelcase

## Description

Complete the solution so that the function will break up camel casing, using a space between words.

## Example
"camelCasing"  =>  "camel Casing"

"identifier"   =>  "identifier"

""             =>  ""

## Solution

```python
# Provide your solution here.
def solution(s):
    ss = ""
    for i in s:
        if i.isupper():
            ss += " " + i
        else:
            ss += i
    return ss
