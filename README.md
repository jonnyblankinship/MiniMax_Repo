# MiniMax_Readme

Introduction

This is a Tic-Tac-Toe game with an AI opponent that uses the minimax algorithm to determine its moves. The player will play against the computer, and the goal is to place three X's or O's in a row vertically, horizontally or diagonally. The code is implemented in Python 3.


Gameboard

The game board is represented by a 3x3 matrix where 0 represents an empty cell, -1 represents a cell occupied by the human player, and +1 represents a cell occupied by the computer player.


Functions

evaluate(state):
This function takes in the current state of the game board and returns +1 if the computer wins, -1 if the human wins and 0 if it's a draw.

wins(state, player):
This function tests if a specific player has won the game by checking all the possible winning combinations on the game board.

game_over(state):
This function tests if the game is over, i.e., either the human or the computer has won.

empty_cells(state):
This function returns a list of all the empty cells on the game board.

valid_move(x, y):
This function returns True if the cell on the board at coordinates (x, y) is empty.

set_move(x, y, player):
This function sets the move on the board at the specified coordinates (x, y) for the specified player.

minimax(state, depth, player):
This is the AI function that chooses the best move for the computer using the minimax algorithm. It takes in the current state of the board, the current depth in the game tree, and the current player. It returns a list containing the best row, best col, and the best score.

clean():
This function clears the console.


Requirements

- Python 3
- math
- random
- os
- platform
- time
- Usage

To play the game, simply run the code in a Python 3 environment. The user will play as the human player and will input their moves (0-9) corresponding to the 9 spaces on the board. The computer will then make its move using the minimax algorithm. The game will continue until a player wins or until all cells on the board are filled.
