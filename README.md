# 🎮 2048 Game

A Python implementation of the classic 2048 puzzle game using a
4×4 grid and keyboard-based controls.

The player moves numbered tiles in four directions. When two tiles
with the same value collide, they merge into a single tile with
double the value. The objective is to create the 2048 tile.

## ✨ Features

- 4×4 game board
- Move tiles Up, Down, Left, and Right
- Keyboard controls using W, A, S, and D
- Automatic generation of new tiles
- Merging of tiles with equal values
- Board compression after each move
- Win detection when the 2048 tile is created
- Game-over detection when no valid moves remain

## 🛠️ Technologies Used

- Python
- Random module

## 📂 Project Structure

'''text
2048-game-python/
│
├── 2048.py
├── logic.py
├── .gitignore
└── README.md'''

## How to Run
1. Clone the repository
git clone https://github.com/Rakshitha-Peddi/2048-game-python.git

2. Navigate to the project directory
cd 2048-game-python

3. Run the game
python3 2048.py

## How to Play

Use the following keys to move the tiles:

Key	Movement
W / w	Move Up
S / s	Move Down
A / a	Move Left
D / d	Move Right

## Game Rules
The game starts with a 4×4 grid.
A new 2 is added to an empty cell.
Tiles with the same value can be merged.
Each successful move can generate a new tile.
The game is won when a tile reaches 2048.
The game is lost when there are no empty cells and no possible merges.

## Concepts Used
Python functions
Nested lists
2D arrays / matrices
Loops
Conditional statements
Random number generation
List manipulation
Matrix transposition
Functions with return values
Boolean flags
Game-state checking
Problem-solving and algorithmic thinking

## Main Functions
1.start_game()

Creates the initial 4×4 game board and adds the first tile.

2.add_new_2(mat)

Adds a new 2 to an empty position in the board.

3.compress(mat)

Moves all non-zero tiles toward one side of the board.

4.merge(mat)

Combines adjacent tiles having the same value.

5.move_left(grid)

Performs compression and merging to move tiles to the left.

6.move_right(grid)

Reverses the grid, performs a left movement, and reverses it back.

7.move_up(grid)

Uses matrix transposition and left movement to move tiles upward.

8.move_down(grid)

Uses matrix transposition and right movement to move tiles downward.

9.get_current_state(mat)

Checks whether the game has been won, is still in progress, or has been lost.

## Future Improvements
Add a graphical user interface
Add score tracking
Add an undo option
Add high-score storage
Add animations and sound effects
Improve keyboard input handling
