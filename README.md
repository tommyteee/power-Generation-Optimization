Power Generation Optimization Using Pyomo and Gurobi

<img width="371" alt="image" src="https://github.com/user-attachments/assets/e908549f-c36d-4d28-9363-0b9a8041aed6" />


Overview

This project formulates and solves a power generation optimization problem to minimize total generation costs while ensuring that power supply meets demand constraints. The model optimizes generator outputs while respecting generation limits and system constraints. The optimization is implemented using Pyomo and solved with the Gurobi solver.

Key Features

Models power generation scheduling using linear programming

Ensures generation meets demand at all times

Incorporates generation capacity constraints

Uses Gurobi, a high-performance solver for mixed-integer programming

Installation

1. Install Required Packages

Ensure you have the following dependencies installed:

pip install pyomo pandas openpyxl

2. Install Gurobi Solver

Since this project uses Gurobi, you need to install and license it:

Download Gurobi from Gurobi Official Website

Ensure Gurobi is installed and set the correct path in the script if necessary

How to Run the Project

Ensure Excel input file (inputs.xlsx) is correctly formatted:

"gen" sheet: id, cost, limit

"load" sheet: id, value

Run the Python script:

python power_generation_optimization.py

View the results, which include:

Optimal power generation values for each generator

Total minimized generation cost
