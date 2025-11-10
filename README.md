# Activtity11_graphs

Task 1: 
Dijkstra’s algorithm fails on negative weights because it assumes that once the shortest path to a vertex is found, it cannot be improved later. However, if a graph contains negative edge weights, a path that initially seems longer may become shorter after passing through a negative edge. For example, consider three vertices A → B → C with weights A–B = 4 and B–C = -6, and a direct edge A–C = 5. Dijkstra would choose A–C (cost 5) as the shortest path first, but the real shortest path is A–B–C with a total cost of -2. Since Dijkstra never revisits nodes after marking them as final, it fails to find this correct path.
