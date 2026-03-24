<img src="http://i.giphy.com/huJEYlQEr3SBq.gif" alt="pathfinding with the A* algorithm" />

# Pathfinding Algorithms

## A* Pathfinding Algorithm

A* (A-star) is a widely used pathfinding algorithm designed to efficiently find the shortest path between two points. It combines the strengths of Dijkstra’s Algorithm (which guarantees the shortest path) and Greedy Best-First Search (which prioritizes speed).

The algorithm works by evaluating nodes based on a cost function:

- **g(n)**: The actual cost from the starting node to the current node  
- **h(n)**: A heuristic estimate of the cost from the current node to the target  
- **f(n) = g(n) + h(n)**: The total estimated cost of the path through the current node  

A* maintains two main sets:
- **Open Set**: Nodes that are discovered but not yet evaluated  
- **Closed Set**: Nodes that have already been evaluated  

At each step, A* selects the node from the open set with the lowest **f(n)** value, explores its neighbors, and updates their costs if a better path is found. This process continues until the target node is reached or no valid path exists.

By using a well-chosen heuristic (such as Manhattan distance for grid-based movement or Euclidean distance for continuous space), A* achieves a strong balance between accuracy and performance, making it a popular choice for real-time applications like games and simulations.
