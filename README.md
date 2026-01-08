# Sudoku Solver with Tkinter GUI and Backtracking Algorithm

This is a graphical user interface (GUI) for solving Sudoku puzzles. It allows the user to input a puzzle, solve it, generate a new puzzle, or clear the current one. The difficulty level can also be set to "Easy", "Medium", or "Hard". The program uses tkinter for creating the GUI, and the PIL library for taking screenshots.


## Requirements

- Python 3.6 or higher
- tkinter
- PIL

``` bash
git clone https://github.com/uppercasee/SudokuSolver.git
cd SudokuSolver
python3 ./main.py
```

## Inputting a puzzle
Click on a cell in the grid to select it, and enter a number between 1 and 9. Once a cell is selected, the program will highlight the row, column, and 3x3 subgrid that the cell belongs to. If the number entered is invalid (i.e. it violates the Sudoku rules), an error message will be displayed. The program will also prevent the user from clicking the solve, generate, or clear buttons until a valid puzzle is entered.

## Solving a puzzle
Once a valid puzzle is entered, click the "Solve" button to solve it. The program will use a **backtracking algorithm** to fill in the empty cells in the grid. If the puzzle has no solution, an error message will be displayed.

## Generating a new puzzle
To generate a new puzzle, click the "Generate" button. The program will randomly generate a new Sudoku puzzle with the specified difficulty level (default is "Easy"). The generated puzzle will be displayed in the grid, and the user can then solve it.

## Clearing the current puzzle
To clear the current puzzle, click the "Clear" button. This will clear all the cells in the grid.

## Taking a screenshot
To take a screenshot of the current puzzle, press CTRL+S or go through the file menu. The program will take a screenshot of the GUI window, and save the image inside assets folder as  `sudoku-[current time].png`

## Future Improvements
Future improvements to this program could include adding additional features to the GUI, such as the ability to load puzzles from a file or save solved puzzles to a file. Additionally, the program could be optimized to solve puzzles more quickly, or to solve puzzles with multiple solutions.
