# Dijkstra-s-Algorithm-Priority-Queue-Maze-Solver

This project is designed to demonstrate the practical implementation of Dijkstra’s algorithm using a priority queue for efficient graph traversal. The aim is to provide a visual representation of the algorithm in action, highlighting the shortest path in a weighted graph. We utilize the MakeCV library to handle graphical operations and visual effects.

# MakeCV
MakeCV is used for drawing and updating the graphical representation of the graph. It provides tools to:

Draw nodes and edges.
Update colors of nodes and edges during the execution of the algorithm to indicate status (unvisited, visiting, and visited).
Display text annotations for weights and path lengths.

# Priority Queue
A priority queue is employed to efficiently retrieve the next node with the smallest distance during the execution of Dijkstra's algorithm. This ensures that the algorithm always processes the most promising node next, significantly speeding up the search process in sparse and dense graphs.

# Dijkstra's Algorithm
Dijkstra's algorithm is used for finding the shortest path from a starting node (source) to all other nodes in a graph with non-negative edge weights. It operates by:

Marking the distance from the source to every other vertex as infinity initially, except for the source itself which is zero.
Adding each vertex to a priority queue with the priority as its current shortest distance.
Iteratively extracting the vertex with the smallest distance from the priority queue, updating the distances to its adjacent vertices, and adjusting their positions in the priority queue.

# Challenges

Understanding MakeCV
One of the primary challenges I faced during the development of this project was gaining a thorough understanding of the MakeCV library. The library's documentation was sparse and sometimes unclear.

Troubleshooting Graphical Updates
To overcome these issues, I initially relied heavily on print statements to debug the behavior of graphical elements. This approach helped me identify how MakeCV manages state changes in graphics, which was not immediately obvious from the documentation. By methodically printing out internal state information at key points in my rendering loop, I was able to map out how updates to graphical properties like vertex updates were being processed.

# How to use
The user begins by loading an image into the system. This image could represent anything from a simple maze to a complex network of city streets. The image serves as a background template on which the graph will be overlayed. Once the image is loaded, the user can place vertices directly on the image using a graphical interface provided by the MakeCV library.

The core functionality is invoked when the user selects two vertices and requests the shortest path calculation. The computeShortestPath function implements Dijkstra's algorithm using the vertices and edges previously defined.

This function ties together user interaction and algorithmic processing, offering a visual and practical approach to understanding and utilizing Dijkstra's algorithm. By integrating image handling, interactive graph construction, and pathfinding, the system provides a comprehensive tool for educational and planning purposes.

