# Numerical Recipes Coursework

This repository contains implementations of numerical simulations for two physics problems:

1. **Spacecraft in a Non-Spherical Gravitational Field** - Simulating the trajectory of a spacecraft orbiting the Moon with mass concentrations ("mascons")
2. **Absence of Transport in Disordered Lattices** - Analyzing quantum particle behavior in regular and disordered potential wells

## Spacecraft in a Non-Spherical Gravitational Field

This simulation explores how mass concentrations below the Moon's surface affect spacecraft orbits, similar to phenomena observed during Apollo missions.

### Features
- Simulation of spacecraft trajectories in radially symmetric gravitational fields
- Implementation of non-spherical gravitational corrections to model "mascons"
- Numerical calculation of orbital periods
- Analysis of trajectory sensitivity to gravitational field perturbations
- Determination of minimum safe orbit heights

### Technical Implementation
- Numerical integration of equations of motion using appropriate ODE solvers
- Visualization of spacecraft trajectories and height profiles
- Parameter sensitivity analysis
- Efficient implementation with runtime under a few minutes

## Absence of Transport in Disordered Lattices

This simulation demonstrates the quantum localization phenomenon, where a quantum particle gets trapped in randomly arranged potential wells despite having sufficient energy to travel through regularly arranged wells.

### Features
- Solution of the time-dependent Schrödinger equation in 1D
- Analysis of eigenvalues and eigenvectors of the discretized Hamiltonian
- Simulation of quantum wave packet propagation in free space
- Comparison of particle transport in regular versus disordered potentials
- Statistical analysis of transport probability across multiple random potential configurations

### Technical Implementation
- Discretization of the Schrödinger equation using appropriate boundary conditions
- Eigenvalue calculation for the Hamiltonian matrix
- Visualization of potential landscapes and probability distributions
- Integration of probability currents to calculate transport probabilities
- Monte Carlo simulation over random potential configurations

## Requirements
- Python 3.x
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook

## Project Structure
```
├── spacecraft/
│   ├── spacecraft.ipynb       # Main notebook for spacecraft simulation
│   └── visualization/         # Animation and visualization tools
├── quantum_lattice/
│   ├── quantum_lattice.ipynb  # Main notebook for quantum simulation
│   └── analysis/              # Analysis tools for quantum transport
├── utils/
│   ├── ode_solvers.py         # Implementation of ODE solvers
│   └── matrix_utils.py        # Matrix operation utilities
├── results/                   # Simulation results and figures
└── README.md                  # This file
```

## How to Run
1. Clone this repository
2. Install required dependencies: `pip install -r requirements.txt`
3. Open the Jupyter notebooks in the `spacecraft/` or `quantum_lattice/` directories
4. Execute the cells in sequence to reproduce the results

## Results

### Spacecraft Simulation
- The trajectory in a radially symmetric field is an elliptical orbit
- Non-spherical corrections lead to trajectory deviations and eventual lunar impact
- Sensitivity analysis reveals which coordinates are most affected by perturbations
- Minimum safe orbit heights are calculated to avoid lunar impact

### Quantum Lattice Simulation
- Demonstration of quantum wave packet propagation in free space
- Visualization of transport through regularly spaced potential wells
- Evidence of localization in randomly arranged potential wells
- Statistical analysis showing reduced transport probability in disordered potentials

## Notes
- Code is optimized for both accuracy and efficiency
- All simulations complete within a few minutes on standard hardware
- Error tolerances are set to match the required accuracy levels specified in
