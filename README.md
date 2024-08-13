
# Optimal Driver-Passenger Assignment Using Ant Colony Optimization

This project aims to reduce deadheading in ride-hailing services by optimizing the assignment of drivers (sources) to passengers (destinations). The solution uses Ant Colony Optimization (ACO) to find the optimal routes that minimize the total distance drivers travel without passengers. The street network of Chennai, Tamil Nadu, is used as a case study.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Visualization](#visualization)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Deadheading, or the distance traveled by drivers without passengers, is a significant inefficiency in ride-hailing services. This project leverages Ant Colony Optimization (ACO) to minimize deadheading by optimally assigning drivers to nearby passengers, using a street network graph fetched from OpenStreetMap (OSM).

## Features

- **Street Network Fetching**: Fetches and projects the street network of Chennai using OSMnx.
- **Random Driver and Passenger Generation**: Randomly selects locations on the network to represent drivers and passengers.
- **Deadheading Cost Calculation**: Computes the shortest path distances between all driver-passenger pairs.
- **Ant Colony Optimization**: Implements ACO to find the optimal assignment of drivers to passengers, minimizing deadheading.
- **Graph Visualization**: Visualizes the street network, with optimal driver-passenger routes highlighted.

## Technologies Used

- **Python**: Core programming language.
- **OSMnx**: For fetching and handling street network data.
- **NetworkX**: For graph processing and pathfinding.
- **Matplotlib**: For visualizing the network and routes.
- **NumPy**: For numerical operations and random node selection.
- **SciPy**: For optimization tasks.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/driver-passenger-assignment.git
   cd driver-passenger-assignment
   ```

2. **Install the required Python packages:**
   ```bash
   pip install osmnx networkx matplotlib numpy scipy
   ```

## Usage

1. **Run the script**: The script fetches the Chennai street network, generates random driver and passenger locations, and optimally assigns drivers to passengers using ACO.
   ```bash
   python driver_passenger_assignment.py
   ```

2. **Ant Colony Optimization (ACO)**: The script implements ACO to minimize the total deadheading distance by optimizing driver-passenger assignments.

3. **Output**: The output is a visualization of the street network with drivers, passengers, and optimal routes highlighted.

## Visualization

### Optimal Driver-Passenger Assignment using ACO

![Optimal Driver-Passenger Assignment](optimal_assignment.png)

- **Red Points**: Represent drivers.
- **Green Points**: Represent passengers.
- **Yellow Lines**: Represent the optimal routes for drivers to pick up their assigned passengers.

## Contributing

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request. If you find any issues or have suggestions for improvements, feel free to open an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

