# Maze-Solver
## 🧩 My Maze Solver Project 🤖
I'm excited to share a hands-on project I've completed as part of my journey into Artificial Intelligence! I built a Maze Solver using Python that employs two fundamental search algorithms: Depth-First Search (DFS) and Breadth-First Search (BFS). Here’s a breakdown of the project:

## 🚀 Project Overview:
The Maze Solver reads a maze from a text file and finds the shortest path from the start point "A" to the goal point "B". The maze consists of walls and open paths, and the program visualizes the search process and the solution path.

## 🔍 Key Components:
### Node Class:
Represents each state in the maze, keeping track of the current position (state), the parent node (parent), and the action taken to reach that node (action).

### StackFrontier Class:
Implements a stack data structure to manage nodes for the DFS algorithm, supporting operations to add nodes, check if a state exists, and remove nodes.

### QueueFrontier Class:
Extends the StackFrontier class to implement a queue for managing nodes in the BFS algorithm.

### Maze Class:
Handles the reading of the maze from a file, validates the start and goal positions, tracks walls, and defines the methods to find neighbors and solve the maze.

The solve method employs DFS to explore the maze and find the path to the goal, counting the number of explored states.
Visualization:

Utilizes the Pillow library to create a visual representation of the maze and the solution. The solution path is highlighted alongside the explored paths.

## 🌟 How It Works:
### Input: 
A text file containing the maze structure, where "A" represents the start, "B" represents the goal, and walls are represented by other characters.

### Search Algorithms:

### DFS: The solver explores paths deeply, going to the end of a path before backtracking to find other paths.

### BFS (optional): Can be implemented by switching the frontier to a queue to ensure the shortest path is found.
### Output: 
After solving the maze, the program prints the maze with the solution path and saves an image visualizing the maze and the explored states.
