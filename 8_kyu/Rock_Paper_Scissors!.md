# Challenge: Rock Paper Scissors!

## Description

Let's play! You have to return which player won! In case of a draw return Draw!.

Examples(Input1, Input2 --> Output):

"scissors", "paper" --> "Player 1 won!"
"scissors", "rock" --> "Player 2 won!"
"paper", "paper" --> "Draw!"

## Solution

```python
# Provide your solution here.
def rps(p1, p2):
    lst = ['scissors', 'paper', 'rock']
    if p1 == p2:
        return "Draw!"
    elif p1 == lst[0] and p2 == lst[1]:
        return "Player 1 won!"
    elif p1 == lst[0] and p2 == lst[2]:
        return "Player 2 won!"
    elif p1 == lst[1] and p2 == lst[0]:
        return "Player 2 won!"
    elif p1 == lst[2] and p2 == lst[0]:
        return "Player 1 won!"
    elif p1 == lst[1] and p2 == "rock":
        return "Player 1 won!"
    elif p1 == lst[2] and p2 == lst[1]:
        return "Player 2 won!"
    else:
        pass
