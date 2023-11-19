
# Cellular Anomaly Discovery Simulation

## Project Overview
This project is a Python-based simulation that draws inspiration from Conway's Game of Life, with a unique twist to explore concepts related to simulation theory. It utilizes a grid of cells where anomalies are randomly placed, and cells have the capability to 'discover' these anomalies based on certain conditions or proximity. The simulation aims to provide a visual and interactive representation of how the density of cells affects the rate at which anomalies are discovered, paralleling the philosophical exploration of simulation theory in relation to our universe.

## Technologies Used
- ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
- ![Pygame](https://img.shields.io/badge/Pygame-3776AB?style=for-the-badge&logo=pygame&logoColor=white)
- ![NumPy](https://img.shields.io/badge/NumPy-3776AB?style=for-the-badge&logo=numpy&logoColor=white)

## Simulation Details

### Concept
The simulation is built on a grid where each cell can either be 'alive' or 'dead', and certain cells are designated as 'anomalies'. The cells have the ability to discover these anomalies within a specific radius, mimicking the process of uncovering insights or evidence in the real world.

### Key Metrics
- **Environment Size:** Represents the scale or complexity of the simulation environment.
- **Time Passed:** Duration for which the simulation ran.
- **Total Discovery:** Number of anomalies discovered during the simulation.
- **Discovery Rate:** Percentage of anomalies discovered relative to the total number of cells.
- **Alive Colony:** Number of active cells at any given time.
- **Deceased:** Number of cells that have become inactive.

### Interpretation under Simulation Theory
The simulation serves as a metaphorical exploration of the possibility of humanity existing in a simulated environment. The key metrics provide insights into the challenges of discovering anomalies (evidence of being in a simulation), highlighting the rarity and difficulty of such endeavors.

## Installation and Running the Simulation
To run the simulation, ensure you have Python, Pygame, and NumPy installed in your environment. Clone the repository and run the main simulation script.

```bash
git clone <repository-url>
cd <repository-directory>
python simulation_base.py
```

## Results and Analysis
Example results from a simulation run:

- Environment Size: 7200
- Time Passed: 13 seconds
- Total Discovery: 202
- Discovery Rate: 1%
- Alive Colony: 20
- Deceased: 120

These results suggest a complex environment where the discovery of anomalies is rare, aligning with the challenges faced in proving simulation theory in our reality.

## Probability Calculation

### Understanding the Probability of Anomaly Detection
This section explains the mathematical probability of a living colony being exposed to at least one anomaly over a period of 10,000 years, represented as 10 seconds in the project's time scale, based on given simulation parameters.

#### Formula
1. **Probability of an Anomaly in One Update for One Colony:**  
   \\[ P_{\\text{anomaly, one update}} = \\frac{\\text{Total Anomalies Detected}}{\\text{Total Observations}} \\]  
   Where Total Observations = Total Number of Living Colonies × Number of Living Individuals (updates).

2. **Probability of Not Encountering an Anomaly in One Update for One Colony:**  
   \\[ P_{\\text{no anomaly, one update}} = 1 - P_{\\text{anomaly, one update}} \\]

3. **Probability of Not Encountering an Anomaly in All Updates for One Colony:**  
   \\[ P_{\\text{no anomaly, all updates}} = \\left( P_{\\text{no anomaly, one update}} \\right)^{\\text{Number of Living Individuals}} \\]

4. **Probability of At Least One Anomaly in All Updates for One Colony:**  
   \\[ P_{\\text{at least one anomaly}} = 1 - P_{\\text{no anomaly, all updates}} \\]

In the specific scenario of the project, this formula calculates the likelihood that a living colony will encounter at least one anomaly in the equivalent of 10,000 years.

## Contributing
Contributions to the project are welcome. Please ensure to follow the code of conduct and adhere to the contribution guidelines when submitting pull requests.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
