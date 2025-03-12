# Automated Planning for a Rover using PDDL

This project focuses on **automated planning** for a rover to achieve specific objectives while considering multiple constraints. The planning problem is modeled using **PDDL (Planning Domain Definition Language)**, and a server processes the domain and problem files to generate a valid plan. The results are then displayed in the terminal.

## Description

In this project, we define a **PDDL planning domain** and multiple **planning problems** related to a rover’s mission. The rover must navigate, collect samples, take images, and communicate data while considering constraints such as:

- **Battery levels and energy consumption**
- **Terrain conditions and obstacles**
- **Communication range and signal availability**
- **Resource management (e.g., limited sample storage)**

A **planning server** is used to process the PDDL domain and problem files, returning an optimized sequence of actions that allow the rover to achieve its goals.

## Technologies Used

- **PDDL**: Defines the domain and problem for automated planning.
- **Planning-as-a-Service**: Uses [Planning.Domains Solver](https://solver.planning.domains) for remote execution.
- **Fast Downward / OPTIC / other planners**: Alternative local planners.
- **Python**: Handles communication with the planning server and processes results.
- **Flask (optional)**: If a custom planning server is used.
- **VS Code PDDL Extension**: Provides syntax highlighting and integration.

## Requirements

To work comfortably with **PDDL** in **VS Code**, install the **PDDL extension**:

🔹 [PDDL Extension for VS Code](https://marketplace.visualstudio.com/items?itemName=jan-dolejsi.pddl)

Additionally, configure **Planning-as-a-Service** to use the online planner:

1. Open **VS Code** settings (`Ctrl + alt + P`).
2. Search for `pddl.planningService`.
3. Set it to:  
