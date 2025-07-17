🗺️ GPS Navigation System
![alt text](https://img.shields.io/badge/Language-Python-blue.svg)
![alt text](https://img.shields.io/badge/Libraries-NetworkX%20%7C%20Matplotlib-orange.svg)
![alt text](https://img.shields.io/badge/Status-Maintained-green.svg)
![alt text](https://img.shields.io/badge/License-MIT-brightgreen.svg)
A feature-rich GPS navigation system built with Python, leveraging graph-based algorithms for efficient route planning, traffic-aware shortest paths, amenity discovery, and interactive map visualization.
⚙️ Features
Admin Interface
Graph Management: Add/delete map locations (vertices).
Road Connectivity: Create/remove roads (edges).
Traffic Updates: Dynamically update traffic information on roads.
Amenity Handling: Attach amenities like hotels, restaurants, and petrol pumps to specific routes.
Persistence: Save and load the entire map state using graph_state.pkl and Python's pickle module.
Visualization: Display the full map with details on distances, traffic, and amenities via Matplotlib.
User Interface
Shortest Path Calculation: Compute the optimal route using Dijkstra’s algorithm, which accounts for both distance and traffic.
Multi-stop Routes: Plan journeys with one or more optional waypoints between the start and destination.
Interactive Visualization:
Display the full map for a general overview.
Highlight the calculated shortest path in red for clear visibility.
Optionally show amenities along the roads.
Amenity Finder: Discover hotels, restaurants, or petrol pumps available along the calculated route.
Travel Time Estimation: Get an estimated travel time based on the route's total distance and an average speed.
🛠️ Installation & Setup
Requirements
Python 3.x
pip package installer
Quick Start
Clone the repository:
Generated bash
git clone https://github.com/aravindp602/GPS-Navigation-System.git
cd GPS-Navigation-System
Use code with caution.
Bash
Create and activate a virtual environment:
Generated bash
python -m venv venv
Use code with caution.
Bash
macOS/Linux:
Generated bash
source venv/bin/activate
Use code with caution.
Bash
Windows:
Generated bash
venv\Scripts\activate
Use code with caution.
Bash
Install dependencies:
Generated bash
pip install -r requirements.txt
Use code with caution.
Bash
▶️ Running the Application
Execute the main script from your terminal:
Generated bash
python gps_navigation.py
Use code with caution.
Bash
You will be greeted with the main menu:
Generated text
Welcome to GPS Navigation System

Main Menu:
1. Admin Login
2. User Login
3. Exit
Enter your choice:
Use code with caution.
Text
👨‍💻 Usage Guide
Admin
Select 1. Admin Login from the main menu.
Enter the default password: admin.
You can now manage the map by adding/deleting places, roads, traffic info, and amenities.
User
Select 2. User Login from the main menu.
From the user menu, you can:
View the full map.
Calculate routes (with or without waypoints).
Discover amenities along your path.
Get travel time estimates for your journey.
🔬 Technical Details
Core Algorithm: The system uses Dijkstra’s shortest path algorithm for route computation.
Time Complexity: The algorithm has a time complexity of O((V + E) log V), ensuring efficient performance.
Graph Storage: An adjacency matrix is used for the graph representation, allowing for O(1) access to edge weights.
Data Persistence: The entire graph state (nodes, edges, traffic, amenities) is serialized and saved in graph_state.pkl via the pickle module.
Visualization: Map and route rendering is handled by Matplotlib and NetworkX.
🤝 Contributing
We welcome contributions! Please follow these steps to contribute:
Fork the repository.
Create a new branch for your feature:
Generated bash
git checkout -b feature/YourAmazingFeature
Use code with caution.
Bash
Make your changes and commit them with clear messages.
Push your branch to your forked repository.
Open a Pull Request.
📜 License
This project is licensed under the MIT License. See the LICENSE file for more details.
