# Challenge: Reverse words in a string

## Description

You need to write a function that reverses the words in a given string. A word can also fit an empty string. If this is not clear enough, here are some examples:

As the input may have trailing spaces, you will also need to ignore unneccesary whitespace.

## Example (Input --> Output)

"Hello World" --> "World Hello"

"Hi There." --> "There. Hi"

## Solution

```python
# Provide your solution here.
def reverse(st):
    return ' '.join([i for i in st.split()[::-1]])
