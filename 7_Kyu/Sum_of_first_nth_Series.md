
# Challenge: Sum of the first nth term of Series

## Description

Task
Your task is to write a function which returns the n-th term of the following series, which is the sum of the first n terms of the sequence (n is the input parameter).

S
e
r
i
e
s
:
1
+
1
4
+
1
7
+
1
10
+
1
13
+
1
16
+
…


You will need to figure out the rule of the series to complete this.

Rules
You need to round the answer to 2 decimal places and return it as String.

If the given value is 0 then it should return "0.00".

You will only be given Natural Numbers as arguments.

Examples (Input --> Output)

n

1 --> 1 --> "1.00"

2 --> 1 + 1/4 --> "1.25"

5 --> 1 + 1/4 + 1/7 + 1/10 + 1/13 --> "1.57"

## Solution

```python
# Provide your solution here.
def series_sum(n):
    res = 0
    j = 4
    if n == 0:
        return f"{n:.2f}"
    for i in range(1,n):
        if n == 1:
            return f"{n:.2f}"
            break
        else:
            res += 1/j
            j += 3
    return f"{res+1:.2f}"
