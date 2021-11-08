# CS661-8-Puzzle-Problem

Goal of this program: Solve the 8-puzzle problem
Programming Language: Lisp
Approach: A* search using Manhattan value as the heuristic

Some important note:
1. My approach of solving this problem is by using recursion. After finding a result, then I use backtracking to find the correct path from start to result
2. For the sake of performing backtracking and keep the step count, I attached 2 additional numbers in from of every lists (board).

For example, if a board is (1 2 3 4 5 6 7 8 0), I would make it (3 10 1 2 3 4 5 6 7 8 0). 
3 in the beginning means the transaction between this board and the previous board is 0 got moved "DOWN" (1 = UP, 2 = RIGHT, 3 = DOWN, 4 = LEFT, 0 = STARTING POINT). I use this number to track each step until the beginning
10 means the total count of movement from start to this board

