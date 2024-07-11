# Grocery Queue Simulation

This project implements a simulation to model a grocery store's checkout process to determine the optimal number of cashiers needed. The simulation uses object-oriented programming in Python with the support of NumPy and Matplotlib functionalities.

## Files

- `Code.ipynb`: The main Jupyter notebook containing the simulation code.
- `Report.pdf`: A detailed report of the project, including methodology, results, and analysis.

## Requirements

- Python 3.x
- NumPy
- Matplotlib
- SciPy

## Installation

1. Clone the repository or download the files.
2. Install the required libraries using pip:

    ```sh
    pip install numpy matplotlib scipy
    ```

## Usage

### Running the Simulation

1. Open the `Code.ipynb` notebook using Jupyter Notebook or JupyterLab.
2. Run all the cells to execute the simulation. The notebook will:
    - Define the necessary classes for the simulation (Event, Schedule, Customer, Queue, ManagerQueue, GroceryStore).
    - Implement the simulation logic.
    - Run the simulation for different scenarios and analyze the results.

### Viewing the Report

For a detailed explanation of the project, including the modeling, simulation process, and results, refer to the `Report.pdf` file.

## Project Structure

### Event and Schedule Classes

These classes implement a priority queue for managing and running events based on their scheduled time.

### GroceryStore Class

The `GroceryStore` class initializes the simulation, generates customer arrivals, and manages queues and cashier interactions.

### Queue and ManagerQueue Classes

These classes handle the interactions between customers and cashiers or the manager, including serving customers and tracking queue lengths.

### Customer Class

The `Customer` class stores information about each customer's activity, including arrival time, service time, and whether they need assistance from the manager.

## Simulation Logic

The simulation follows these steps:
1. Customers arrive at the store and join the queue with the shortest line.
2. Cashiers serve customers based on a normally distributed service time.
3. 5% of customers require assistance from the manager, who follows a separate queue.
4. The simulation runs until the store closes, and all customers in the queue are served.

## Analysis

The simulation explores various metrics to determine the optimal number of cashiers:
- Average customer waiting time
- Average customer response time
- Maximum queue length
- Average queue length

## Results

The results from the simulation are compared with theoretical calculations to analyze the effectiveness of the model and to determine the optimal number of cashiers.
