# Tic-Tac-Toe

A Python console Tic-Tac-Toe game where you play against the computer. Built in 7th grade.

## Overview

The computer is essentially unbeatable. Most games end in a draw, and the rest end in a computer win. It doesn't use any AI or machine learning, just hardcoded logic, multi-step simulated lookaheads, fork detection, and blocking algorithms.

## How the computer plays

The computer follows a priority order on each turn:

1. Win if it can
2. Block the player from winning
3. Create a fork (two simultaneous winning threats)
4. Block the player from forking
5. Take the center, then corners, then edges

The fork detection is what makes it hard to beat. The computer looks multiple moves ahead to identify situations where it can force two winning paths at once, making it impossible for the player to block both.

## How to run

```
python tictactoe.py
```

Enter your move as a row and column number when prompted. The board is a 3x3 grid indexed from 0.
