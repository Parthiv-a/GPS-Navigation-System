# 🗺️ GPS Navigation System

![Language](https://img.shields.io/badge/Language-Python-blue.svg)
![Libraries](https://img.shields.io/badge/Libraries-NetworkX%20%7C%20Matplotlib-orange.svg)
![Status](https://img.shields.io/badge/Status-Maintained-green.svg)
![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)

A feature-rich GPS navigation system built with Python, leveraging graph-based algorithms for efficient route planning, traffic-aware shortest paths, amenity discovery, and interactive map visualization.

---

## ⚙️ Features

### Admin Interface
- **Graph Management**: Add/delete map locations (vertices).
- **Road Connectivity**: Create/remove roads (edges).
- **Traffic Updates**: Dynamically update traffic on roads.
- **Amenity Handling**: Attach hotels, restaurants, petrol pumps to nodes/edges.
- **Persistence**: Save/load entire map using `graph_state.pkl` and `pickle`.
- **Visualization**: Display map with distances, traffic, and amenities via Matplotlib.

### User Interface
- **Shortest Path**: Compute optimal route with Dijkstra’s algorithm (accounts for distance + traffic).
- **Multi-stop Routes**: Plan routes with optional waypoints.
- **Interactive Visualization**:  
  - Display full map  
  - Highlight route in red  
  - Optionally show amenities
- **Amenity Finder**: Discover hotels, restaurants, petrol pumps along the route.
- **Time Estimation**: Based on route distance and average speed.

---

## 🛠️ Installation & Setup

### Requirements
- Python 3.x
- `pip`

### Quick Start
```bash
git clone https://github.com/aravindp602/GPS-Navigation-System.git
cd GPS-Navigation-System
python -m venv venv
# macOS/Linux
source venv/bin/activate
# Windows
venv\Scripts\activate
pip install -r requirements.txt
```

##▶️ Running the Application
```bash

python gps_navigation.py
```
#You'll see:


Welcome to GPS Navigation System

Main Menu:
1. Admin Login
2. User Login
3. Exit
Enter your choice:
👨‍💻 Usage Guide
Admin
Select 1. Admin Login

Enter the default password: admin

Manage the map: add/delete places, roads, traffic, amenities.

User
Select 2. User Login

Explore:

View full map

Calculate routes (with or without waypoints)

Discover amenities along the route

Get travel time estimates

🔬 Technical Details
Core Algorithm: Dijkstra’s shortest path

Time complexity: O((V + E) log V)

Graph Storage: Adjacency matrix for O(1) access

Data Persistence: All states saved via pickle in graph_state.pkl

Visualization: Matplotlib-based rendering of map and routes

🤝 Contributing
We welcome contributions! Please follow these steps:

Fork the repo

Create a branch:

bash
Copy
Edit
git checkout -b feature/YourFeature
Make commits with clear messages

Push your branch and open a Pull Request

📜 License
This project is under the MIT License. See LICENSE for details.
