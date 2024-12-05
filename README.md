# Description
This repository contains MATLAB scripts designed to process and visualize data from Scanning Electrochemical Cell Microscopy (SECCM) experiments. The code extracts key parameters from SECCM raw files, defines measurement maps, and generates plots to facilitate the analysis of localized electrochemical behavior.

# Features
Extracts and processes raw SECCM data.

Defines map sizes based on user-specified landing configurations.

Plots OCP and PDP curves for each landing point.

Generates spatially resolved maps for Eocp, Ecorr, and final current.

# How It Works

A- Map Definition:
The code begins by defining the size of the measurement map:

1) Number of landings in the X and Y directions.

2) Separating distance between adjacent landings.

B- Measurements at Each Landing:
At every landing, three key measurements are identified and processed:

1) Tip Down: Initial data recorded when the SECCM tip contacts the surface.

2) OCP vs Time: Open Circuit Potential measurement over time.

3) PDP (Current vs Potential): Potentiodynamic Polarization measurement.

C- Plotting Curves for Each Landing:

1) Tip down curves (Current vs time)
  
2) OCP curves (potential vs. time).

3) PDP curves (current vs. potential).

D- Data Extraction for Map Generation:
The code extracts specific parameters from the raw data to generate spatially resolved maps:

1) OCP Data (Eocp): The potential recorded at the end of the OCP measurement.

2) Ecorr: The potential corresponding to the minimum current (I) in the PDP measurement.

3) Final Current: The last recorded current value in the PDP measurement.


# Usage
1) Place SECCM raw data files in the designated data/ folder.

2) Specify the number of landings in X and Y and the separation distance in the script configuration.

3) Run the main script to process data and generate plots


# License
MIT License

