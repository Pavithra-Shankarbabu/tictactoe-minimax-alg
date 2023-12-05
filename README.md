# Tic Tac Toe Game

In this Python implementation of the classic game Tic Tac Toe, players and an AI opponent take turns placing their moves on a 3x3 board. The first player to make three consecutive marks in a row wins the game.


## Running


The program is run with the command line and can be called with a -d flag to set the difficulty, a -p flag to play against a human, and a -h flag for help.

* Playing with the AI (difficulty set to hard by default)

```python
$ python tic_tac_toe.py
```

* Playing with the AI with difficulty set (easy or hard)

```python
$ python tic_tac_toe.py -d easy
```

```python
$ python tic_tac_toe.py -d hard
```

* Playing with someone else (take turns in same screen)
```python
$ python tic_tac_toe.py -p human
```

* For more help run
```python
$ python tic_tac_toe.py -h
```

## Functions

The functions are used to implement a game of tic-tac-toe for a two-player game or playing against an AI. The functions print the board, get vacant spaces, check if someone has won, evaluate the board, use the minimax algorithm to find the best move, and then return the best move for the AI.

```Python
print_board()
```

Prints the current state of the game board on the console.

```Python
get_empty_spaces()
```

Returns a list of empty spaces on the board.

```Python
is_win()
```

Checks if a player has won the game.

```Python
evaluate()
```

Evaluates the board and returns a score for the AI's move.

```Python
minimax()
```

Implements the minimax algorithm for the AI's move.

```Python
get_best_move()
```
Returns the best move for the AI to make based on the current board.

```Python
play_game()
```

Initiates and plays the game. The player enters their move by specifying the row and column number of the board. The function checks if the move is valid and adds it to the board if it is valid. It then checks if the player has won the game or if the game is tied. If the game is still ongoing, the AI calculates its best move using the `get_best_move()` function and adds it to the board. It then checks if the AI has won the game or if the game is tied. If the game is still ongoing, the process continues until the game is over.

## Board Representation

The game board is represented by a 2D list of 3x3 size, where "X" represents the player's move, "O" represents the AI's move, and " " (empty string) represents an empty space on the board.

## AI opponent

The AI opponent uses the minimax algorithm to calculate the best move. This algorithm recursively explores all possible moves to a certain depth and returns the score for each move. The score is evaluated using the `evaluate()` function. The AI opponent chooses the move with the highest score.

## How to Play

To play the game, run the `play_game()` function in a Python environment.

## Example

Here's an example of a game being played:

```
     |     |
  X  |     |  O
_____|_____|_____
     |     |
     |  X  |
_____|_____|_____
     |     |
  O  |     |
     |     |
```

In this example, the player (represented by "X") has made the first move in the top-left corner. The AI opponent (represented by "O") has made the second move in the center. The player has made the third move in the center-left. The game is still ongoing.

## Requirements

Implementation of Tic Tac Toe requires Python 3.x.

Download the latest version of Python 3 from the official Python website: https://www.python.org/downloads/

Run the installer and follow the instructions.

Update your PATH environment variable so that you can access Python from the command line:

On Windows, use the Start menu to go to your system properties, then select the Advanced tab. Click Environment Variables, then edit the PATH variable so that it includes the path to the Python directory.

Confirm that Python is correctly installed by entering the following command into the command line:
python --version
You should see the version of Python you installed.

## Usage Instructions

To use this implementation of Tic Tac Toe, simply clone the repository and import the functions into your Python environment.

1.Open your terminal
2.Navigate to the directory where you would like to clone the repository.
3.Run the command to copy and download the files in to your local machine.
4.It will download the repository to your local machine.
5.To import the functions, open the python script you would like to use and add the following lines:
from Tic-Tac-Toe import *
import Tic-Tac-Toe.py


# Features Development

The game could be further developed by adding features such as:

1. A graphical user interface (GUI) to make the game more interactive

2. An option to play against another human player over a network

3. An option to save and load games

4. Keep track of wins and losses for players


## Conclusion

Python implementation of Tic Tac Toe is a fun and simple game that can be played on the console. It uses the minimax algorithm to provide a challenging opponent for the player. Try it out and see if you can beat the AI!
