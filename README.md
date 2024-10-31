# Molecular Dynamics Analysis and Visualization

This project provides a script for analyzing and visualizing the results of molecular dynamics (MD) simulations of multiple proteins. The script extracts and compares the Root Mean Square Deviation (RMSD), Radius of Gyration (Rg), and Root Mean Square Fluctuation (RMSF) for a set of protein structures. These metrics help assess structural stability, compactness, and flexibility of proteins during simulations.

## Requirements

- **Gnuplot**: For plotting RMSD, Rg, and RMSF graphs.
- **Bash**: The script is written in Bash, which should be run in a Unix-like environment.
- **Protein pdb files**
- **mdp files** : These are required to run the MD Simulation #Set up according to forcefield used. #In this case used charmm 27 force field

## Directory Structure

Assume a directory structure like below:

- **MDG**: This is the main directory containing pdb protein files and `.xvg` files generated from MD simulations for each protein.
- **output**: The directory where the plots will be saved.

Each `.xvg` file should be formatted to contain the relevant MD simulation data for RMSD, Rg, or RMSF.

## MD Analysis Script Overview

The script performs the following tasks:
1. **Data Extraction**: Extracts data for RMSD, Rg, and RMSF from the `.xvg` files, formatting them for Gnuplot.
2. **Plotting**: Uses Gnuplot to generate line plots for RMSD, Rg, and RMSF across all proteins, including the `Wildtype`.

## How to Run the Script

1. Place all `.xvg` files for the proteins in the `MDG` directory.
2. Run the script in a terminal:
   ```bash
   ./your_script_name.sh
