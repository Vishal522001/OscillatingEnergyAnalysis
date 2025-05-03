# Oscillating Energy Analysis

## Project Overview
This repository contains the solution to the **Oscillating Energy Analysis** project, which models and calculates energy consumption based on an oscillating power function. The project implements both analytical and numerical integration methods, with visualizations of the power function and the integral. It also compares the results obtained using different numerical methods and calculates the associated errors.

## Problem Statement
The project involves calculating the energy consumption \( E(t) \) for a power function \( P(t) = a_1 \cdot t + \sin(2 \pi f_1 t) \) over the time range from \( t = 0 \) to \( t = 20 \) seconds, where:
- \( a_1 = 3.1338 \, \text{W} \) (derived from a given parameter),
- \( f_1 = 2 \, \text{Hz} \).

The objectives of the project are:
1. Calculate the exact energy consumption analytically.
2. Implement numerical integration methods to approximate the energy consumption.
3. Compare the results using different numerical methods.
4. Plot the power function \( P(t) \) and the integral results.
5. Calculate absolute and relative errors for each method.

## Files in this Repository
- **PowerFunction.java**: Contains the implementation of the power function \( P(t) \).
- **NumericalIntegration.java**: Implements three numerical integration methods.
- **PlotP.java**: Plots the power function \( P(t) \) over the range of 0 to 20 seconds.
- **ErrorCalculation.java**: Calculates the absolute and relative errors for each integration method.
- **Results.pdf**: A report documenting the exact result, plot, integration methods, UML diagrams, and error calculations.
- **IntegrationResults.txt**: Contains the results of the numerical integration methods and error calculations.

## Running the Code
1. **Clone this repository** to your local machine:
   ```bash
   git clone https://github.com/your-username/your-repository.git
   ```

2. **Compile the Java files**:
   ```bash
   javac *.java
   ```

3. **Run the main program**:
   - You can run the program by executing the main class that coordinates the integration, plotting, and error calculations (e.g., `Main.java` if you have a main class).
   ```bash
   java Main
   ```

4. The program will:
   - Display the plot of the power function \( P(t) \).
   - Calculate and display the results for the numerical integration methods.
   - Calculate and display the absolute and relative errors.

## Expected Output
The expected output includes:
- The plot of the power function \( P(t) \) for \( t = 0 \) to \( t = 20 \).
- The calculated results for each numerical integration method.
- Error analysis showing absolute and relative errors.

## Methodology
The project implements three numerical integration methods:
1. **Method 1**: Uses the value at \( y_0 \) as the height for the area.
2. **Method 2**: Uses the mean of \( y_0 \) and \( y_1 \) for the area.
3. **Method 3**: Uses linear interpolation between two consecutive points for the area.

These methods are implemented in `NumericalIntegration.java` and tested on the power function \( P(t) \).

## UML Diagram
The software structure is designed using Object-Oriented principles, and a UML diagram is provided in the `Results.pdf` to visualize the relationships between the classes.

## Error Calculations
The program calculates the absolute and relative errors between the numerical results and the exact analytical result.

## License
This project is open source and available under the [MIT License](LICENSE).
