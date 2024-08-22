# Challenge: File properties 

## Description

write a perogram to print the file properties ?

## Solution

```python
# Provide your solution here.
def file():
    with open('test.txt','w') as f:
        f.write('hello world')
        print("name is", f.name)
        print("mode is ", f.mode)
        print("is it readable, ", f.readable())
        print("is it writeable, ", f.writable())
        print("is it closed", f.closed)
    print("is it closed", f.closed)

if __name__ == '__main__':
    file()
