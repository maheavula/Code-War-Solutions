# Challenge: Tuples

## Description

Given an integer, n, and n space-separated integers as input, create a tuple, t, of those n integers. Then compute and print the result of hash(t).

Note: hash() is one of the functions in the_builtins module, so it need not be imported.

## Example

Sample Input 0

2
1 2
Sample Output 0

3713081631934410656

## Solution

```python
# Provide your solution here.
if __name__ == '__main__':
    n = int(input())
    integer_list = map(int, input().split())
    hashh = tuple(integer_list)
    print(hash(hashh))
