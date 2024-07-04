# Sudoku Solver

This project implements a Sudoku Solver using a backtracking algorithm in C++. The solver reads a Sudoku puzzle from standard input, attempts to solve it, and prints the solved puzzle if a solution exists.

## Features

- Solves a 9x9 Sudoku puzzle.
- Validates the placement of numbers using standard Sudoku rules.
- Utilizes backtracking to find a solution.

## Getting Started

### Prerequisites

- C++ compiler (e.g., `g++`)



## Usage

1. Run the executable:
    ```sh
    ./SudokuSolver
    ```

2. Enter the Sudoku puzzle (use 0 for empty cells):
    ```
    5 3 0 0 7 0 0 0 0
    6 0 0 1 9 5 0 0 0
    0 9 8 0 0 0 0 6 0
    8 0 0 0 6 0 0 0 3
    4 0 0 8 0 3 0 0 1
    7 0 0 0 2 0 0 0 6
    0 6 0 0 0 0 2 8 0
    0 0 0 4 1 9 0 0 5
    0 0 0 0 8 0 0 7 9
    ```

3. The solved Sudoku puzzle will be printed if a solution exists:
    ```
    5 3 4 6 7 8 9 1 2
    6 7 2 1 9 5 3 4 8
    1 9 8 3 4 2 5 6 7
    8 5 9 7 6 1 4 2 3
    4 2 6 8 5 3 7 9 1
    7 1 3 9 2 4 8 5 6
    9 6 1 5 3 7 2 8 4
    2 8 7 4 1 9 6 3 5
    3 4 5 2 8 6 1 7 9
    ```

4. If no solution exists, the following message will be displayed:
    ```
    No solution exists for the given Sudoku puzzle.
    ```

## Code Explanation

### Functions

- `void print(int board[9][9], int n)`: Prints the Sudoku board.
- `bool isValid(int board[9][9], int i, int j, int num, int n)`: Checks if placing a number at the given position is valid.
- `bool SudokuSolver(int board[9][9], int i, int j, int n)`: Solves the Sudoku puzzle using backtracking.
- `int main()`: Reads the Sudoku puzzle, calls the solver, and prints the result.





## Acknowledgments

- Inspired by classic Sudoku solving algorithms.


