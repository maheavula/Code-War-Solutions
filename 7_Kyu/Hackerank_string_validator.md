# Challenge: Hackerank_string_validator

## Description

Python has built-in string validation methods for basic data. It can check if a string is composed of alphabetical characters, alphanumeric characters, digits, etc.

## Solution

```python
# Provide your solution here.
if __name__ == '__main__':
    s = input()
    
    print(any(i.isalnum() for i in s ))
    
    print(any(i.isalpha() for i in s))
    
    print(any(i.isdigit() for i in s))
    
    print(any(i.islower() for i in s))
    
    print(any(i.isupper() for i in s))
    

 
