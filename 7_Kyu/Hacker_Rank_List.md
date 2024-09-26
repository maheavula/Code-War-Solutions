# Challenge: Hackerank List

## Description

You have an empty list. You need to perform a series of commands on this list. The commands are:

insert i e: Insert integer e at position i in the list.
print: Print the current state of the list.
remove e: Remove the first occurrence of integer e from the list.
append e: Add integer e to the end of the list.
sort: Sort the list in ascending order.
pop: Remove the last element from the list.
reverse: Reverse the order of the list.
You will be given a number n followed by n lines of commands. You need to perform each command in order and print the final state of the list.

## Example
Sample Input 0

12
insert 0 5
insert 1 10
insert 0 6
print
remove 6
append 9
append 1
sort
print
pop
reverse
print
Sample Output 0

[6, 5, 10]
[1, 5, 9, 10]
[9, 5, 1]

## Solution

```python
# Provide your solution here.
if __name__ == '__main__':
    N = int(input())
    lst = []
    for _ in  range(N):
        comd = input().split()
        
        if comd[0] == 'insert':
            lst.insert(int(comd[1]), int(comd[2]))
        elif comd[0] == 'remove':
            lst.remove(int(comd[1]))
        elif comd[0] == 'append':
            lst.append(int(comd[1]))
        elif comd[0] == 'sort':
            lst.sort()
        elif comd[0] == 'pop':
            lst.pop()
        elif comd[0] == 'reverse':
            lst.reverse()
        elif comd[0] == 'print':
            print(lst)
             
