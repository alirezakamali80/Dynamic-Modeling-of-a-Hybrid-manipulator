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
