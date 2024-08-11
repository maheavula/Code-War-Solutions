# Challenge: The robber language

## Description

The Robber Language (Rövarspråket) is a Swedish cant used by children to mislead people not familiar with the language. It's used by kids in several screenplays created by Astrid Lindgren.

The idea is that every consonant in a sentence is duplicated, with an o inserted in between (b becomes bob). Vowels are left untouched (a remains an a). It's quite hard for an untrained ear to understand a conversation encoded in this manner, especially if spoken rapidly.

Example
In this example, the consonants f, b and r are modified. The vowels o and a are left untouched.

'foo bar' => 'fofoo bobaror' (`fof-o-o bob-a-ror`)
Note: The dashes - in the example are added for readability and should not be included in the output.

The Assignment
Your task is to implement a function def robber_encode(sentence) which takes in a string sentence and returns the result, converted into robber language, as a string.

Notes
Only consonants should be modified; leave all other characters unchanged.
Both upper and lower case characters will be tested.
The case of the o character and the neighboring consonants should match (F => FOF and f => fof).
For the purpose of this kata, a character is considered a consonant if it's equal to one of the letters BCDFGHJKLMNPQRSTVWXYZ.

## Solution

```python
# Provide your solution here.
def function(sentence):
    consonants = 'BCDFGHJKLMNPQRSTVWXYZbcdfghjklmnpqrstvwxyz'
    encoded_sentence = ""
    for char in sentence:
        if char in consonants:
            if char.isupper():
                encoded_sentence += char + 'O' + char
            else:
                encoded_sentence += char + 'o' + char
        else:
            encoded_sentence += char
    return encoded_sentence
