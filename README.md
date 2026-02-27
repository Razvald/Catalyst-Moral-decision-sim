# Moral decision sim

Simulation platform for modeling and analyzing decision-making strategies of autonomous vehicles in ethically conflicting road scenarios.

## Overview

Autonomous vehicles inevitably face situations where a collision cannot be avoided and a decision must be made that minimizes overall harm. However, there is a lack of tools that allow systematic modeling, testing, and quantitative evaluation of such ethical trade-offs.

This project provides a simulation framework based on **CARLA** for:

- modeling ethically conflicting driving scenarios,
- implementing parameterized decision-making strategies,
- collecting quantitative metrics,
- visualizing and comparing the consequences of different policies.

The platform is designed for educational, research, and experimental purposes.

---

## Key Features

- Scenario-based simulation of unavoidable accident situations
- Parameterized decision-making agent based on a utility function
- Adjustable priority weights ("ethical slider"):
  - passenger safety
  - pedestrian safety
  - material damage minimization
- Telemetry and metrics collection:
  - passenger risk
  - number and severity of pedestrian injuries
  - material damage estimation
- Interactive dashboard for visualization and analysis
- Modular and extensible architecture

---

## Example Scenarios

- Sudden pedestrian crossing
- Group of pedestrians on the road
- Oncoming vehicle collision
- Obstacle avoidance with limited maneuvering space
- Narrow road and tunnel scenarios

---

## System Architecture

```

Scenario Generator → Simulation Engine → Decision Agent → Metrics Collector → Analytics Dashboard

````

---

## Technologies

- Simulation: CARLA
- Programming language: Python
- Data analysis: NumPy, Pandas
- Visualization: Matplotlib, Plotly
- Web interface: Streamlit

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ethical-av-simulator.git
   cd ethical-av-simulator
   ```

2. Create virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux / Mac
   venv\Scripts\activate     # Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Install and run CARLA simulator (see official CARLA documentation).

---

## Metrics

* Passenger injury risk
* Number of pedestrians affected
* Damage estimation
* Combined utility score

---

## Project Status

🚧 Work in progress (educational & research project)

---

## Team

* ML / Decision algorithms
* Simulation engineering
* Analytics & visualization

---