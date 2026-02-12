# Strategic Pathfinding: Bearing-Optimized Workout Generator

### 🗺️ Overview
This project implements a custom routing engine that generates workout paths of a target distance using real-world map data. Unlike standard GPS, this algorithm prioritizes a "natural" running feel by minimizing sharp turns and tracking vertical elevation gain.

### 🧩 Technical Approach
* **Modified DFS:** Explores the road network until a `goal_dist` is met.
* **Bearing-Aware Navigation:** Sorts neighbor nodes based on their angular difference from the current heading, prioritizing the straightest possible path.
* **Elevation Tracking:** Calculates cumulative uphill vertical gain.

### 📊 Visualization
![Interactive Route Map](https://nickzeng123.github.io/Route-Graph/)

### 📋 Installation
```bash
pip install osmnx networkx folium
python route_planner.py
