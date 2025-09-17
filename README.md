# Project Guide (Simulation Guide)

## Overview
The repository contains **3 examples** (`Example 1`, `Example 2`, `Example 3`) in the original manuscript.  
Each example directory includes:
- Initialization script: `initial_value.m`  
- Simulink model: `secureBipartiteFlocking.slx`  
- Plotting script: `draw_3dimbold.m`  

**Basic workflow (same for each example):**
1. Run initialization script: `initial_value.m`
2. Run/Simulate the Simulink model: `secureBipartiteFlocking.slx`
3. Run plotting script: `draw_3dimbold.m` to generate figures

> **Note:** The initialization script sets random initial conditions. Thus, the simulation results will differ on each run (non-deterministic).

---

## Requirements
- MATLAB (R2019b or later recommended)
- Simulink for the corresponding MATLAB version


# Additional Example: *New Example 1*

## Contents
The folder `New Example 1/` contains an updated version of the simulation, including:
- Initialization script: **`initial_value_largeagent.m`**  
- Simulink model: **`Bipartite_flocking_largeagent.slx`**  
- Plotting script: **`largeScaledraw_3dimbold.m`**  
- Pre-computed initialization data: **`initialStates.mat`**  

## Reproducible experiments (match the paper)
To exactly reproduce the results reported in the paper, load the provided **`initialStates.mat`** file before running the model:

```matlab
Run `initial_value_largeagent.m`;   % loads predefined initial conditions
Run `Bipartite_flocking_largeagent.slx`;
Run `largeScaledraw_3dimbold`。
```
