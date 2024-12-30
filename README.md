# Food Delivery Optimization Using Reinforcement Learning

## Project Overview
This project focuses on optimizing food delivery logistics in Lucknow using reinforcement learning (RL). The goal is to design an AI-based system that:
- Minimizes rider idle time.
- Reduces fuel costs and travel distances.
- Ensures on-time deliveries.
- Manages multiple pickups and drop-offs while adhering to capacity constraints.

By leveraging RL techniques, the system dynamically learns and adapts to optimize resource allocation and improve delivery efficiency.

## Features
- *Dynamic Order Assignment*: Assign orders to riders based on proximity, capacity, and delivery time constraints.
- *Route Optimization*: Plan the shortest delivery paths using RL and road network data.
- *Capacity Management*: Dynamically allocate riders during peak hours.

## Data Generation and Visualization
- Synthetic data was generated to simulate orders and rider locations within Lucknow's geographical boundaries.
- Interactive maps using Folium visualized rider and order locations.

## Reinforcement Learning Applications
### 1. Order Assignment
- *State*: Current rider location, remaining capacity, and active orders.
- *Actions*: Assign an order to a specific rider.
- *Rewards*: 
  - +10 for on-time delivery.
  - -5 for delays.

### 2. Route Optimization
- *State*: Current route and pending deliveries.
- *Actions*: Select the next delivery destination.
- *Rewards*:
  - +15 for shortest route.
  - -10 for detours.

### 3. Capacity Planning
- *State*: Incoming orders and rider availability.
- *Actions*: Dynamically allocate riders.
- *Rewards*:
  - +20 for efficient capacity usage.
  - -10 for exceeding capacity or missed deliveries.

## Performance Metrics
- *Total Reward*: Measures overall system efficiency.
- *Successful Deliveries*: Tracks timely and accurate deliveries.
- *Fuel Costs*: Evaluates cost-effectiveness.
- *Average Delivery Time*: Reflects customer satisfaction.

## Algorithm Design
1. *Parameter Analysis*: Evaluated delivery speeds, costs, and constraints.
2. *Data Preprocessing*: Generated synthetic data for orders and riders.
3. *Rider Assignment*: Used Q-learning to assign orders dynamically.
4. *Route Optimization*: Planned delivery paths to minimize travel distance and time.
5. *Capacity Planning*: Managed rider allocation during high demand.

## Requirements
- Python 3.x
- Libraries: numpy, pandas, matplotlib, seaborn, folium, fpdf, osmnx

## How to Run
1. Clone this repository: git clone [repository-url]
2. Install the required libraries: pip install -r requirements.txt
3. Run the Python scripts for data generation, RL training, and visualization.

## Future Scope
- Integrate real-time traffic data for better route optimization.
- Expand the system to handle larger datasets and other cities.

---

Author: Akash Srivastava  
Date: 30-12-2024
