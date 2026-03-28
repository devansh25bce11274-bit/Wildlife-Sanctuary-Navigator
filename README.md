Wildlife Sanctuary Navigator

Intelligent Pathfinding System using A* Algorithm

The Wildlife Sanctuary Navigator is a graph-based simulation system designed to model navigation within a large wildlife sanctuary. The project applies the A* (A-Star) search algorithm to compute the most efficient route between different locations while considering terrain difficulty and environmental constraints.

This system demonstrates how artificial intelligence techniques can be used in real-world applications such as eco-tourism planning, wildlife monitoring, and smart navigation systems.


Problem Statement
Navigating large wildlife sanctuaries presents several challenges:
Uneven terrain and long travel distances
Restricted or sensitive wildlife zones
Lack of intelligent routing in traditional maps
No consideration of terrain difficulty (flat vs steep paths)
Most conventional mapping systems provide only static directions and fail to adapt to such dynamic conditions.
This project addresses these issues by creating an intelligent routing model that selects the most efficient path based on both distance and terrain conditions.


System Overview

The sanctuary is represented as a state-space graph, where:
Each location is modeled as a node
Each path between locations is modeled as a weighted edge
Edge weights represent distance and terrain difficulty
The system allows users to input a starting point and destination, after which it calculates the optimal path using A*.


AI Concepts and Methodology

1. Graph Representation
The entire sanctuary is structured as a graph:
Nodes → represent key locations such as landmarks, camps, and wildlife zones
Edges → represent paths connecting these locations
This abstraction allows efficient traversal and search operations.

3. A* Search Algorithm
The project uses the A* algorithm, a widely used informed search technique.
The evaluation function is:

f(n) = g(n) + h(n)
Where:
g(n) → actual cost from the start node to current node
h(n) → estimated cost from current node to goal
This combination ensures both accuracy and efficiency.

3. Heuristic Function
The heuristic used is Euclidean distance
It estimates the straight-line distance between two points
This ensures the algorithm remains admissible and optimal

5. Cost Function
The system incorporates terrain-based cost adjustment:
Flat paths → standard weight
Steep paths → multiplied cost (1.5×)
This makes the navigation more realistic and practical.


Technology Stack

The implementation uses the following tools and libraries:
Python 3.x → Core programming language
NetworkX → Graph creation, manipulation, and pathfinding
Matplotlib → Visualization of the map and routes
Math Module → Distance and heuristic calculations


Sanctuary Map Structure

The model includes multiple categories of locations to simulate a real sanctuary environment:
Entry and Exit Points
Park Entrance
Forest Exit
Visitor Facilities
Visitor Center
Food Court
First Aid Post
Research Center
Natural Landmarks
Sunset Point
River Bank
Lake View
Hilltop View
Grassland Field
Camping and Operational Areas
Ranger Station
Camp Site A
Camp Site B
Camp Site C
Camp Site D
Wildlife Zones
Tiger Zone
Elephant Corridor
Deer Park
Bird Sanctuary
Crocodile Point
These zones simulate restricted or sensitive areas within the sanctuary.


Visualization and Output

The system generates a graphical map that visually represents:
All nodes (locations) within the sanctuary
Edges (paths) connecting them
Different edge styles indicating terrain types
Highlighted optimal route computed by A*
Additional outputs include:
Total path distance displayed in the title
Console output showing the computed route


How to Run the Project

Follow the steps below to run the project locally:
1. Verify Python Installation

python --version

2. Install Required Libraries

pip install networkx matplotlib

3. Execute the Script

python filename.py

4. Provide User Input
Enter the starting and ending locations when prompted:

Start_point:
End_point:
Example Input

Start_point: Park_Entrance
End_point: Tiger_Zone


Expected Output

A graphical window displaying the sanctuary map
Highlighted optimal path between selected locations
Console output showing:
Shortest path sequence
Total distance


Applications

This project can be extended for real-world use cases such as:
Smart navigation in national parks
Wildlife monitoring and patrol routing
Eco-tourism planning systems
Emergency response route optimization


Future Enhancements

Dynamic routing based on real-time animal movement
Risk-aware navigation (avoid predator zones)
Integration with GPS and real-world maps
Interactive user interface
Route animation and simulation
Mobile or web-based deployment


Author
Devansh Singh



