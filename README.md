GPS Navigation System 🗺️
![alt text](https://img.shields.io/badge/Language-Python-blue.svg)
![alt text](https://img.shields.io/badge/Libraries-NetworkX%20%7C%20Matplotlib-orange.svg)
![alt text](https://img.shields.io/badge/Status-Maintained-green.svg)
![alt text](https://img.shields.io/badge/License-MIT-brightgreen.svg)
A sophisticated GPS navigation system built with Python and graph-based algorithms. This project provides a powerful command-line interface for both administrators to manage the map data and for users to find the most efficient routes between locations.
The system leverages Dijkstra's algorithm to calculate the shortest path, considering factors like distance and traffic. It's a comprehensive tool for route planning, amenity discovery, and traffic analysis.
✨ Features
This system is divided into two main interfaces: an Admin side for graph management and a User side for navigation.
🔧 Admin Features
Dynamic Map Management: Add or delete places (vertices) from the map.
Connectivity Control: Add new roads (edges) connecting different places.
Real-time Traffic Updates: Update traffic information on any road to influence route calculations.
Amenity Management: Add hotels, restaurants, and petrol pumps along specific routes.
Data Persistence: All map data, including places, connections, and amenities, is saved and can be reloaded.
Map Visualization: View the entire map graph with detailed information about distances and traffic.
🚀 User Features
Shortest Path Calculation: Find the quickest route between a source and a destination, accounting for distance and traffic.
Multi-stop Journeys: Plan routes that include one or more stops between the start and end points.
Interactive Map Visualization:
View the complete map.
See the calculated shortest path highlighted in red.
Display maps with or without amenity information on the roads.
Amenity Finder: Discover essential amenities like hotels, restaurants, and petrol pumps along your calculated route.
Travel Time Estimation: Get an estimated travel time for your journey based on the total distance and an average speed.
🛠️ Getting Started
Follow these steps to get the project running on your local machine.
Prerequisites
Ensure you have Python 3 installed on your system. You will also need the pip package manager.
Installation
Clone the repository:
Generated sh
git clone <your-repository-url>
cd <repository-directory>
Use code with caution.
Sh
Create a virtual environment (recommended):
Generated sh
python -m venv venv
Use code with caution.
Sh
Activate the environment:
On Windows: venv\Scripts\activate
On macOS/Linux: source venv/bin/activate
Install the required libraries:
Create a file named requirements.txt and add the following lines:
Generated code
networkx
matplotlib
Use code with caution.
Now, install them using pip:
Generated sh
pip install -r requirements.txt
Use code with caution.
Sh
How to Run the Application
Save the provided code as a Python file (e.g., gps_navigation.py).
Run the script from your terminal:
Generated sh
python gps_navigation.py
Use code with caution.
Sh
The application will start, presenting you with the main menu.
👨‍💻 How to Use the System
Upon starting the application, you will be greeted with the main menu.
Generated code
Welcome to GPS Navigation System

Main Menu:
1. Admin Login
2. User Login
3. Exit
Enter your choice:
Use code with caution.
Admin Usage
Select 1 for Admin Login.
Enter the password when prompted (the default password is admin).
Once logged in, you will have access to the admin menu to manage the map graph.
User Usage
Select 2 for User Login.
You will be presented with the user menu.
You can choose to view the map, find a route, or explore amenities.
When finding a route, you can enter a start and destination, and optionally add multiple stops along the way. The system will visualize the optimal path.
🔬 Technical Details & Complexity
The core of this navigation system is built on graph theory, with efficiency being a key consideration.
Dijkstra's Algorithm: The shortest path is calculated using Dijkstra's algorithm. The time complexity for this implementation is O((V+E)logV), where V is the number of vertices (places) and E is the number of edges (roads). This makes it highly efficient even for large maps.
Graph Representation: An adjacency matrix is used to represent the graph, allowing for constant-time edge weight lookups.
Data Persistence: The state of the graph (including all vertices, edges, traffic, and amenities) is saved to a file (graph_state.pkl) using Python's pickle module, ensuring that data is not lost between sessions.
🤝 Contributing
Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.
To contribute:
Fork the Project.
Create your Feature Branch (git checkout -b feature/AmazingFeature).
Commit your Changes (git commit -m 'Add some AmazingFeature').
Push to the Branch (git push origin feature/AmazingFeature).
Open a Pull Request.
📜 License
Distributed under the MIT License. See LICENSE for more information.
