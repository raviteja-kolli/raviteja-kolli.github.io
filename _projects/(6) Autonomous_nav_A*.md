---
name: Autonomous Nav using A star algorithm
tools: [Python]
image: https://raviteja-kolli.github.io/assets/Astar.gif
description: This project implements an autonomous path-finding algorithm using the A (A-star) algorithm* for navigating a mobile robot on a two-dimensional grid
---

<br>
### Brief overview
<br>
The primary objective of this project was to develop a robust path-finding algorithm for a mobile robot that can navigate a 2D environment with obstacles using the A* algorithm. The algorithm utilizes a heuristic-based approach to determine the optimal path from a starting point to a destination while avoiding obstacles.

Implemented in Python, the algorithm leverages the heapq library for efficient handling of the priority queue during path exploration. The algorithm is tested within a predefined grid, and the results include the estimated path of the robot and the actual path followed.
<br>

### Hardware
* No specific hardware was used for this project as it was entirely implemented and tested through software simulation.

* The algorithm is designed to be applicable to mobile robots equipped with appropriate sensors for real-world navigation.

### Software and Approach

Python 3: Primary programming language used for implementing the A* algorithm.

Google Colab: Used for coding, testing, and visualizing the algorithm’s performance.

heapq Library: It is utilized for managing the open list of cells during path exploration, providing efficient sorting and retrieval.

The project implements the A* algorithm, which is a heuristic-based path-finding technique commonly used in robotics and AI for navigating from a start point to a goal while avoiding obstacles. The algorithm works as follows:

* Grid Initialization: The grid is initialized as a 5x5 matrix where each cell is either traversable or an obstacle. Obstacles are predefined and represented as black cells.

* Heuristic Calculation: The algorithm calculates a heuristic value for each cell using the Manhattan distance formula, providing an estimate of the distance to the goal.

* Path Exploration: Cells are explored using a priority queue managed by the heapq library. The algorithm prioritizes cells with the lowest cost (f = g + h), where g is the cost from the start to the current cell and h is the estimated cost to the goal.

* Path Tracing: Once the goal is reached, the path is reconstructed by tracing back from the goal cell to the start cell using parent pointers.

* Path Comparison: The estimated path and the actual path followed by the robot are compared to evaluate performance and identify any discrepancies.


### Results

The algorithm successfully generated accurate paths for the mobile robot navigating a 5x5 grid. The estimated path and the actual path followed were found to be identical, confirming the accuracy of the implementation. The output generated was:

Estimated path of Robot: [(0, 0), (0, 1), (1, 1), (1, 2), (1, 3), (2, 3), (3, 3), (3, 4), (4, 4)]
Path of the Robot: [(0, 0), (0, 1), (1, 1), (1, 2), (1, 3), (2, 3), (3, 3), (3, 4), (4, 4)]


### Future Scope 

* Testing the algorithm on larger grids to evaluate scalability and efficiency.
* Testing with different heuristic functions such as Euclidean distance or Dijkstra’s algorithm to improve performance and utilizing parallel processing techniques to enhance the algorithm’s speed and efficiency.


<p class="text-center">
{% include elements/button.html link="https://github.com/raviteja-kolli/Autonomous-Nav" text="GitHub" %}
</p>
