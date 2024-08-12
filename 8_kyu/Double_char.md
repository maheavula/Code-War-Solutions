# Challenge: Double char

Given a string, you have to return a string in which each character (case-sensitive) is repeated once.

## Examples (Input -> Output):

* "String"      -> "SSttrriinngg"

* "Hello World" -> "HHeelllloo  WWoorrlldd"

* "1234!_ "     -> "11223344!!__  "


## Solution

```python
# Provide your solution here.
def double_char(s):
    ss =""
    for i in range(len(s)):
        ss += s[i]+s[i]
    
    return ss
