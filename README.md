# CI2024_lab2
## Traveling Salesman Problem (TSP) - Greedy Approach
This implementation uses a **greedy algorithm** to approximate a solution for the TSP:
- Starting from an initial city, it iteratively selects the closest unvisited city, minimizing travel cost at each step.
- After visiting all cities, it returns to the starting point to complete the tour.

### Steps
1. **Distance Matrix**: Distances between cities are computed using `geopy` and stored in a matrix.
2. **Graph Creation**: Using `networkx`, cities are represented as nodes in an undirected graph with edge weights as distances.
3. **Greedy Algorithm**: Begins at the closest city and repeatedly visits the nearest unvisited city, producing a full route upon return to the start.

### Limitations
The greedy approach is efficient and easy to implement but does not guarantee an optimal solution. It’s often used as a starting solution for further optimization methods (e.g., simulated annealing).

The function `tsp_cost` computes the total cost of the generated path.

---
