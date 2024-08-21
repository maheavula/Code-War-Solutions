# Challenge: keyword variable length argument (**variable) in Python

## Description

keyword variable length argument (**variable) in Python

## Solution

```python
# Provide your solution here.
def dic_args(**kwargs):
    print(kwargs)

if __name__ == "__main__":
    dic_args(id=1, name="mahesh", age=22)


