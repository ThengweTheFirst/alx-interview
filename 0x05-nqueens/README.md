# 0x05. N Queens

## Overview
The N queens puzzle is a classic problem in chess. The challenge is to place N non-attacking queens on an N×N chessboard. In this project, we will write a Python program to solve the N queens problem using backtracking.

## Requirements
- All files will be interpreted/compiled on Ubuntu 14.04 LTS using Python 3 (version 3.4.3).
- All files should end with a new line.
- The first line of all your files should be exactly `#!/usr/bin/python3`.
- A README.md file, at the root of the folder of the project, is mandatory.
- Your code should use the PEP 8 style (version 1.7.*).
- All your files must be executable.

## Usage
To use the program, run the `nqueens` script with the value of N as an argument.

```bash
./nqueens N
```

- If the user called the program with the wrong number of arguments, it will print `Usage: nqueens N`, followed by a new line, and exit with the status 1.
- N must be an integer greater or equal to 4. If N is not an integer, it will print `N must be a number`, followed by a new line, and exit with the status 1.
- If N is smaller than 4, it will print `N must be at least 4`, followed by a new line, and exit with the status 1.

The program will print every possible solution to the N queens problem, one solution per line.

## Example
```bash
./nqueens.py 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]

./nqueens.py 6
[[0, 1], [1, 3], [2, 5], [3, 0], [4, 2], [5, 4]]
[[0, 2], [1, 5], [2, 1], [3, 4], [4, 0], [5, 3]]
[[0, 3], [1, 0], [2, 4], [3, 1], [4, 5], [5, 2]]
[[0, 4], [1, 2], [2, 0], [3, 5], [4, 3], [5, 1]]
```

## Algorithm
The solution to the N queens problem is implemented using backtracking. The algorithm explores all possible configurations of placing queens on the chessboard, ensuring that no two queens attack each other. It recursively places queens on the board row by row, backtracking when a conflict is detected.

The program will print all possible configurations where N queens can be placed on the board without attacking each other.

## Repo
This project is part of the ALX Interview Prep. You can find the code files in the [alx-interview/0x05-nqueens](https://github.com/alx-interview/0x05-nqueens) directory. The main script to run is [0-nqueens.py](https://github.com/alx-interview/0x05-nqueens/0-nqueens.py).
