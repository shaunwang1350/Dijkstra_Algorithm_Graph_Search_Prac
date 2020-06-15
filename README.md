# Dijkstra_Algorithm_Graph_Search_Prac

## Summary:
In this project, I worked on CodeAcademy's module on Advanced Graph Search Algorithms, which included learning the implementation of Breath-First Search and Depth-First Search. At the end of this module, we instructed to create Dijkstra's Algorithm in Python. The run time for this algorithmn is O = ((E+V)Log V)

## Steps:
1. Instantiate a dictionary that will eventually map vertices to their distance from the start vertex
2. Assign the start vertex a distance of 0 in a min heap
3. Assign every other vertex a distance of infinity in a min heap
4. Remove the vertex with the smallest distance from the min heap and set that to the current vertex
5. For the current vertex, consider all of its adjacent vertices and calculate the distance to them as (distance to the current vertex) + (edge weight of current vertex to adjacent vertex).
6. If this new distance is less than the current distance, replace the current distance.
7. Repeat 4 and 5 until the heap is empty
8. After the heap is empty, return the distances