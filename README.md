WILDLIFE SANCTUARY NAVIGATOR

Overview
Navigating large wildlife sanctuaries is difficult due to uneven terrain and restricted animal areas. Traditional maps do not consider factors like path difficulty or safety zones.
This project represents the sanctuary as a state-space graph, where:
Locations are modeled as nodes
Paths between them are modeled as weighted edges
Using the A* search algorithm, the system determines the most efficient and practical route between two selected points.

AI Concepts Used
Graph Representation: Locations as nodes and connections as weighted edges
A Search Algorithm:* Based on the function
f(n) = g(n) + h(n)
Heuristic: Euclidean distance for estimating shortest path
Cost Adjustment:
Normal paths → standard cost
Steep paths → increased cost (1.5×)

Technology Stack
Python 3.x
NetworkX for graph modeling and pathfinding
Matplotlib for visualization
Python math module for distance calculations

Map Structure
The model includes different categories of locations:

Entry/Exit Points
Park Entrance
Forest Exit
Facilities

Visitor Center
Food Court
First Aid Post
Research Center

Natural Locations
Sunset Point
River Bank
Lake View
Hilltop View
Grassland Field

Camping Areas
Ranger Station
Camp Site A, B, C, D

Wildlife Zones
Tiger Zone
Elephant Corridor
Deer Park
Bird Sanctuary
Crocodile Point

Visualization Output
The generated map displays:
Nodes representing all locations
Different styles of edges for terrain types
A highlighted optimal route between selected points
Total path cost shown in the title

How to Run
Check Python installation:

python --version
Install dependencies:

pip install networkx matplotlib
Run the program:

python filename.py
Enter input when prompted:

Start_point:
End_point:
Example:

Start_point: Park_Entrance
End_point: Tiger_Zone

Output
A graphical window showing the sanctuary map and optimal route
Console output displaying:
Shortest path

Author
Devansh Singh
Total distance

