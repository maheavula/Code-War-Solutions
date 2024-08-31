# Challenge: Sort the odd

## Description

You will be given an array of numbers. You have to sort the odd numbers in ascending order while leaving the even numbers at their original positions.

## Examples

[7, 1]  =>  [1, 7]

[5, 8, 6, 3, 4]  =>  [3, 8, 6, 5, 4]

[9, 8, 7, 6, 5, 4, 3, 2, 1, 0]  =>  [1, 8, 3, 6, 5, 4, 7, 2, 9, 0]

## Solution

```python
# Provide your solution here.
def sort_array(source):
    odd_numbers = sorted([num for num in source if num % 2 != 0])
    result = []
    odd_index = 0
    for num in source:
        if num % 2 != 0:
            result.append(odd_numbers[odd_index])
            odd_index += 1
        else:
            result.append(num)
    return result
        
        
