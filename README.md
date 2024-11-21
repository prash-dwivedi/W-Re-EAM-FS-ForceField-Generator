# W-Re EAM/FS Force Field Generator

## Overview
This repository contains a Python script for generating tabulated Finnis-Sinclair (FS) potentials for molecular dynamics (MD) simulations, specifically tailored for the Tungsten-Rhenium (W-Re) alloy system. The script employs the Chen potential to define interatomic interactions and outputs an `.eam.fs` file compatible with MD simulation software like LAMMPS.

## Key Features
- **Automated Tabulation**: Converts analytical EAM/FS potentials into tabulated formats, simplifying integration into MD simulations.
- **High Accuracy**: Uses high-resolution grids for embedding functions, electron densities, and pair potentials to minimize interpolation errors.
- **Customizable**: Easily extendable to include additional elements or alloy systems by modifying potential functions.
- **Efficient Workflow**: Saves time by automating the force field generation process, crucial for complex simulations involving W-Re alloys.

## How It Works
The script discretizes embedding functions, electron density functions, and pair potentials over a user-defined grid. This tabulation ensures smooth and efficient integration of potentials into MD simulations.

### Workflow
1. Modify the script to include your potential functions if needed.
2. Run the script to generate the `.eam.fs` file.
3. Use the generated file in your molecular dynamics simulations in LAMMPS or similar software.

### File Details
The main Python script that generates the W-Re EAM/FS force field file. It includes all potential definitions, functions for density and embedding, and the writing logic for `.eam.fs` files.

## Why It’s Useful
Accurate force fields are essential for reliable MD simulations, especially when dealing with alloy systems like W-Re. This repository provides a ready-to-use and extendable solution, saving computational and development time while maintaining precision in modeling interatomic interactions.

## Prerequisites
- Python 3.x
- NumPy library (if required for extensions)
- Basic familiarity with MD simulations and potential functions
