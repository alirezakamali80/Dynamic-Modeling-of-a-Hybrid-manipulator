# Dynamic Modeling of Double Segment Redundant Gough-Stewart Hybrid Manipulator

This repository accompanies the paper:

**Dynamic Modeling of Double Segment Redundant Gough-Stewart Hybrid Manipulator based on the Principle of Virtual Work**  
Presented at the *International Conference on Robotics and Mechatronics (ICRoM 2024)*.

## Abstract

This project focuses on the dynamic modeling of a hyper-redundant manipulator consisting of two Gough-Stewart platforms connected serially. By employing the **principle of virtual work**, the study derives dynamic equations for each segment and integrates them into a comprehensive model. Validation is performed using MATLAB and Simscape simulations.

## Problem Statement

Redundant manipulators, inspired by biological systems, are increasingly used in robotics for their flexibility and wide range of applications. However, their dynamic modeling is complex due to:
- Inter-segment force transmission.
- Complex governing equations.

This project addresses these challenges by:
- Formulating a dynamic model based on the principle of virtual work.
- Validating the model against simulated data.

## Methodology

1. **Single Segment Modeling:** The dynamic equations for a single Gough-Stewart manipulator are derived.
2. **Extension to Two Segments:** The outputs of the upper segment are transferred to the lower segment.
3. **Validation:** Results are compared with Simscape simulations to evaluate accuracy.

## Features

- Dynamic model for double-segment redundant Gough-Stewart manipulators.
- MATLAB scripts for solving:
  - Forward and inverse kinematics.
  - Dynamic equations.
- Simscape simulation files for validation.
- Comprehensive error analysis.

## Repository Structure

```plaintext
├── data
│   ├── trajectories    # Predefined trajectories (Helical, Lemniscate)
│   ├── parameters      # Manipulator geometry and mass properties
├── src
│   ├── dynamics        # Dynamic modeling scripts
│   ├── kinematics      # Forward and inverse kinematics scripts
│   ├── utils           # Helper functions for simulations
├── validation
│   ├── simscape_model  # Simscape files for validation
│   ├── results         # Comparison of analytical and simulated results
├── docs
│   ├── paper_summary.md  # Summary of the accompanying paper
│   ├── references.md     # Key references and links
├── README.md            # Project overview (this file)
```

## How to Use

### Prerequisites

- MATLAB (R2022b or newer).
- Simscape toolbox.

### Steps to Reproduce

1. Clone this repository:
   ```bash
   git clone https://github.com/alirezakamali80/dynamic-modeling-gsm.git
   ```
2. Navigate to the repository:
   ```bash
   cd dynamic-modeling-gsm
   ```
3. Open MATLAB and set the repository folder as the working directory.
4. Run the dynamic modeling scripts in `src/dynamics/` to derive forces and actuator lengths.
5. Use Simscape files in `validation/simscape_model` to compare results.

### Trajectories

- Helical motion: Translational and rotational components along three axes.
- Infinity motion: Lemniscate trajectory with smooth rotational dynamics.

## Results

- Dynamic errors for various trajectories remain below 2%.
- Validation confirmed using:
  - Root Mean Square Error (RMSE).
  - Force comparison plots.

### Key Findings

- Virtual work simplifies dynamic modeling for complex configurations.
- Accurate force predictions enable better control strategies.

## Future Work

- Extend the model for manipulators with more than two segments.
- Investigate control strategies leveraging this dynamic model.

## Contact

**Author:** Alireza Kamali Ardakani  
**Email:** [alirezakamali@ut.ac.ir](mailto:alirezakamali@ut.ac.ir)  
**GitHub:** [alirezakamali80](https://github.com/alirezakamali80)
