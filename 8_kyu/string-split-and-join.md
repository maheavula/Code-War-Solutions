# Challenge: string-split-and-join

## Description

n Python, a string can be split on a delimiter.

## Example:

a = "this is a string"
a = a.split(" ") # a is converted to a list of strings.
print a
['this', 'is', 'a', 'string']

Joining a string is simple:

a = "-".join(a)
print a
this-is-a-string

## Solution

```python
# Provide your solution here.

def split_and_join(line):
    a = line.split()
    return "-".join(a)

if __name__ == '__main__':
    line = input()
    result = split_and_join(line)
    print(result)
