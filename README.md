# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?
A: Naked Twins heuristic is one of Sudoku strategies to reduce possibilities.
If two boxes in one unit have two same possible values then no other box in same unit could have these values,
since one of the twin boxes will have one of the two values and another box - another value.
So, if on a reducing step there are a unit with two boxes which have two same possible value, it is possible to
eliminate these values from another boxes from the unit.
This technique reduces the size of search space and helps solve problem faster.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?
A: Diagonal sudoku has one more rule: diagonal axes need to have all digits from 1 - 9 without duplication.
So the only thing we need is to add two more units - diagonal lines from A1 to I9 and diagonal from A9 to I1.
These rules create more constraints to the puzzle, so it is possible to eliminate more possibilites on each
problem reduction step

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
