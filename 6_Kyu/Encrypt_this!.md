# Challenge: Encrypt this!

## Description

Encrypt this!

You want to create secret messages which can be deciphered by the Decipher this! kata. Here are the conditions:

Your message is a string containing space separated words.
You need to encrypt each word in the message using the following rules:
The first letter must be converted to its ASCII code.
The second letter must be switched with the last letter
Keepin' it simple: There are no special characters in the input.

Examples:

encrypt_this("Hello") == "72olle"

encrypt_this("good") == "103doo"

encrypt_this("hello world") == "104olle 119drlo"

## Solution

```python
# Provide your solution here.
def encrypt_this(text):
    lst = text.split()
    stt = ""
    for i in lst:
        stt += str(ord(i[0]))
        if len(i) == 2:
            stt += i[1]
            stt += " "
        elif len(i) > 1:

            stt += i[-1]
            stt += i[2:-1]
            stt += i[1]
            stt += " "
        else:
            stt += " "
    return stt.strip()
