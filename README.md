# Graph Routing Using Dijkstra & A-star

## Project Overview
This project is the final assignment for the **Data Analysis Programming** course. The objective is to implement and analyze **Dijkstra’s Algorithm** and **A-star Algorithm** for shortest pathfinding problems in graph structures.

## Algorithms Implemented
- **Dijkstra’s Algorithm:** Finds the shortest path in a weighted graph with non-negative edge weights using a priority queue.
- **A-star Algorithm:** An informed search algorithm that finds the shortest path using a heuristic function to estimate the cost.

## Dataset
The dataset used for the project consists of graphs represented in **CSV format**, where:
- Each row represents an edge with **source node, destination node, and weight**.
- Additional random graph generation is implemented for testing scalability.

## Project Structure
- `data/`
- `notebooks/` 
- `README.md`

## Implementation Details
### **Dijkstra’s Algorithm**
- Uses a **priority queue (heap)** to explore nodes with the shortest known distance.
- Can find the shortest path from a single source node to all other nodes.
- **Time complexity:** O((V + E) log V) using a priority queue.

### **A* Algorithm**
- Utilizes an **evaluation function f(n) = g(n) + h(n)** where:
  - **g(n):** Cost from the start node to node n.
  - **h(n):** Heuristic estimated cost from node n to the goal.
- Uses a priority queue to select the most promising node first.
- **Time complexity:** O(E), but depends on the quality of the heuristic.

## Results & Insights
- **Performance Comparison:** A* generally performs better when a good heuristic is available, while Dijkstra is more reliable for generic shortest path problems.
- **Use Cases:**
  - Dijkstra is suitable for **network routing, road navigation, and logistics**.
  - A* is ideal for **game AI, robot pathfinding, and real-time navigation systems**.

## Contributors
- **Team 9**

## License
This project is licensed under the **MIT License**.
