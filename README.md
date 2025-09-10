# Search-Agent
An intelligent agent which performs depth-first and breadth-first searches to solve the Missionaries vs. Cannibals problem in state space searches.

# Usage
python search_agent.py

# Dependencies
Python 3.6+

# Description
### The Game
The missionaries versus cannibals problem, also known by other names throughout history ([https://www.wikiwand.com/en/articles/Missionaries_and_cannibals_problem]), involves three missionaries and three cannibals on one side of a river.  They have a boat which can carry exactly one or two people.  They need to cross the river, but at no time may the cannibals outnumber the missionaries on either side of the river.  

### The Program
As a state space or graph search problem, an AI intelligent agent must compute valid states to find the optimal path to the goal state.  A valid state means no missionaries become meals.  The AI program determines these states, expands them to find their neighbors, and expands neighbors as per the search algorithm used until all missionaries and cannibals are on the other side of the river.

### The Algorithms
Depth-first search (DFS) means checking the neighbors of the first neighbor state to the one just expanded before trying other neighbors.  In gaming, imagine exploring a cave system by taking all the lefts you can till the first dead end, then backtracking to the last fork and taking the leftmost tunnel not already explored, over and over till finding what you need.

Breadth-first search (BFS) means checking each neighbor of a state or node to find all their neighbors before trying any deeper layer of neighboring states.  Imagine exploring a pyramid buried all the way to the tip, but making sure you explore every room on each level before moving downward.

This program implements and runs both algorithms in the main() function.  The 3-on-3 MvC problem isn't a particularly big one, and the optimal path to the goal includes only 12 states.
