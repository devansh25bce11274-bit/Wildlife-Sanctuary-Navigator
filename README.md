Wildlife-Sanctuary-Navigator

Wildlife Sanctuary Navigator (A* Pathfinding)
An intelligent graph-based navigation system for wildlife sanctuaries that finds the optimal path between locations using the A* algorithm, considering terrain and path difficulty.

Overview
The sanctuary is modeled as a graph:
Nodes → Locations (landmarks, camps, wildlife zones)
Edges → Paths with distance-based cost
The system uses A* to compute the shortest and most efficient route.

Concepts Used
Graph Theory
A* Algorithm → f(n) = g(n) + h(n)
Euclidean distance as heuristic
Cost variation (steep paths = 1.5×)

Tech Stack
Python
NetworkX
Matplotlib

Map Includes
Entry/Exit: Park Entrance, Forest Exit
Facilities: Visitor Center, Food Court, First Aid
Landmarks: Lake View, Hilltop, River Bank
Camps: Ranger Station, Camp Sites
Wildlife Zones: Tiger, Elephant, Deer, Birds,Crocodile
Output
Visual map with highlighted optimal path
Distance shown in title

How to Run
Bash
pip install networkx matplotlib
python filename.py
Input:

Start_point:
End_point:

Future Work
Danger-aware routing
GPS integration
Animation

Author
Devansh Singh
👨‍💻 Author
Devansh Singh
