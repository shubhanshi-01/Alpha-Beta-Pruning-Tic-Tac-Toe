# Tic-Tac-Toe Game with Alpha-Beta Pruning and Minimax Algorithm

## Description

This project is a Tic-Tac-Toe game implemented in Python where the user can play against the computer. The computer uses a combination of the Minimax algorithm and Alpha-Beta pruning to make intelligent moves.


## How to Run the Game

1. Clone the repository to your local machine.
2. Ensure you have Python installed on your system.
3. Open your terminal or command prompt.
4. Navigate to the directory where the project is located.
5. Run the `tictactoe.py` file followed by `runner.py`
6. Follow the on-screen instructions to play the game.

## Game Rules

Tic-Tac-Toe is a two-player game where each player takes turns marking a cell in a 3x3 grid with their symbol (usually 'X' for one player and 'O' for the other). The first player to get three of their symbols in a row (horizontally, vertically, or diagonally) wins the game. If the grid is filled without any player achieving three in a row, the game ends in a draw.

## Algorithm Explanation

### Minimax Algorithm

The Minimax algorithm is a decision-making algorithm used in game theory for minimizing the possible loss for a worst-case scenario. In the context of Tic-Tac-Toe, the algorithm evaluates all possible moves that the player and the opponent can make from the current game state. It then assigns a score to each possible outcome, assuming that the opponent will also make the best moves possible. The algorithm recursively explores the game tree until it reaches a terminal state (win, lose, or draw), assigning scores to each state along the way. Finally, it chooses the move that leads to the best possible outcome for the player.

### Alpha-Beta Pruning

Alpha-Beta pruning is an optimization technique used to reduce the number of nodes evaluated by the Minimax algorithm. It works by eliminating branches in the game tree that are guaranteed to be worse than previously examined branches. This is achieved by maintaining two values, alpha and beta, which represent the minimum score that the maximizing player is assured of and the maximum score that the minimizing player is assured of, respectively. During the search, if it is determined that a branch's score will not affect the final decision (i.e., it is worse than the current best option), that branch is pruned, and the search continues on other branches.

