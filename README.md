# Sudoku Solver
A simple Sudoku solver implemented in Python using a backtracking algorithm. This project provides a straightforward solution for solving 9x9 Sudoku puzzles and includes a formatted board output.

# Table of Contents
* Features
* Usage
* How It Works
* Example


# Features
Solves 9x9 Sudoku puzzles.
Prints the Sudoku board in a readable format before and after solving.
Uses a backtracking algorithm to find the solution.


# Usage
Open the sudoku_solver.py file in your preferred code editor.

Define your Sudoku puzzle in the sudoku_puzzle variable. Ensure that the puzzle is a 9x9 grid with zeros representing empty cells.

Run the script to see the solution:


python sudoku_solver.py

The script will print the board before and after solving.



# How It Works
print_board(board) - Formats and prints the Sudoku board.
find_empty(board) - Finds the next empty cell in the board.
valid(board, num, pos) - Checks if placing a number in a specific position is valid.
solve_sudoku(board) - Uses a backtracking algorithm to solve the Sudoku puzzle by filling empty cells with valid numbers.


# Example
Here is an example of a Sudoku puzzle and its solution:

Before Solving:

5+---------+---------+---------+
| 5  3  0 | 0  7  0 | 0  0  0 |
| 6  0  0 | 1  9  5 | 0  0  0 |
| 0  9  8 | 0  0  0 | 0  6  0 |
+---------+---------+---------+
| 8  0  0 | 0  6  0 | 0  0  3 |
| 4  0  0 | 8  0  3 | 0  0  1 |
| 7  0  0 | 0  2  0 | 0  0  6 |
+---------+---------+---------+
| 0  6  0 | 0  0  0 | 2  8  0 |
| 0  0  0 | 0  1  9 | 0  0  5 |
| 0  0  0 | 0  0  0 | 0  0  0 |
+---------+---------+---------+



After Solving:

+---------+---------+---------+
| 5  3  4 | 6  7  8 | 9  1  2 |
| 6  7  2 | 1  9  5 | 3  4  8 |
| 1  9  8 | 3  4  2 | 5  6  7 |
+---------+---------+---------+
| 8  5  9 | 7  6  1 | 4  2  3 |
| 4  2  6 | 8  5  3 | 7  9  1 |
| 7  1  3 | 9  2  4 | 8  5  6 |
+---------+---------+---------+
| 9  6  1 | 5  3  7 | 2  8  4 |
| 2  8  7 | 4  1  9 | 6  3  5 |
| 3  4  5 | 2  8  6 | 1  7  9 |
+---------+---------+---------+
9
