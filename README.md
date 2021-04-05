A* search algorithm written in Python. Includes a maze visualization that was created with Pygame.

## Installation
Make sure Python3 and Pygame are installed on your machine. Run program with

```bash
python3 main.py
```

for both visuals/ non-visual. Algorithm will ask for a starting node, whether you want a step-by-step solution, and the heuristic of your choice (straight-line/fewest-nodes). Solution is then printed out to a text file.

## Contents
- Two folders, one for visuals, one for no visuals
- maze.py: Contains definitions for Maze class and the A* algorithm
- node.py: Contains definition for Node class
- main.py: Main program file that runs the algorithm
- maze.txt: Text file that contains the maze to run algorithm on.

## Constraints
The maze.txt file contains the maze for the algorithm. First line declares number of rows and columns. Subsequent lines define the maze nodes. Each node has 4 parts: Value-Direction-xCoord-yCoord. Value consists of one letter and a number. The letter dictates what color the node is (i.e Red or Blue). In order to traverse the maze, you have to alternate between different colored nodes (i.e, Red node -> Blue node -> Red node). The direction indicates the direction you have to go in order to get to the next node (i.e. node R0-S-31-40 has to traverse South to the next Blue node). xCoord and yCoord are used to calculate the Euclidean distance between nodes. This algorithm uses two heuristics (Straight-line distance and fewest nodes) to determine the optimal path.
