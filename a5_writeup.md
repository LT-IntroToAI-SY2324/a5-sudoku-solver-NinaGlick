# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

BFS is more efficient, as it runs each scenario in bresdth rather than depth, for this reason, the program saves more time, because if a scenario ends up being false and you have gone all the way through one scenario, you wasted much more time than you would have if you had done a small test each time for every possible solution. when an anser is likely to need much testing, DFS is better, but if you are unsure if it will need much testing, BFS is better.



2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

by using a stack model in DFS, the algorithm is able to test one scenario all the way through, while with queue model in BFS, the algorithm is able to scan through one level of scenarios in each test, and eliminate scenarios as necessary. I am not sure of other data structures or desig patterns that could have been used. 


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

this assigment can be adapted to make solve large sodokus, perhaps ones that are 4X4 or 5X5. Furthermore, it can be used to solve logic puzzles. the lessons learned from this assignment can help with sorting people into groups. If colleges need help deciding who to admit, they can use an algorithm like this to see the best way to have students who hae high test scores, high GPAs, and are wellrounded. by using a similar algorithm, and having a goal average GPA, test score, and activities list, the algorithm could see the best way to accept people based on these criterion and give the college the nest stats.


