# Challenge: Reverse words

## Description

Complete the function that accepts a string parameter, and reverses each word in the string. All spaces in the string should be retained.


## Solution

```python
# Provide your solution here.
def reverse_words(text):
    return ' '.join([i[::-1] for i in text.split(' ')])
