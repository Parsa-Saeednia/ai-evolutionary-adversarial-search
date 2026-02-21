# AI Evolutionary and Search Experiments

Experimental study of classical Artificial Intelligence algorithms, including **Genetic Algorithms** and **game‑tree search methods**, applied to controlled problem settings.

This project was developed as part of the **Artificial Intelligence** course (Computer Engineering) at the **University of Tehran**, with an emphasis on **algorithmic behavior, parameter sensitivity, and empirical analysis**, rather than full system or game development.

## Overview

This project consists of two independent experimental components:

1. **Evolutionary optimization using Genetic Algorithms**, applied to a continuous parameter optimization problem.
2. **Search‑based decision making in a deterministic board game**, used as a testbed for analyzing game‑tree search behavior.

Both components are implemented and analyzed using **Jupyter notebooks**, which combine code, experiments, visualizations, and discussion in a single reproducible format.

## Project Orientation (For Reviewers)

This repository focuses on **algorithmic experimentation and analysis**.

Some components used in the experiments (such as base game logic) were **provided as course skeleton code** and are not the subject of evaluation.

If you are reviewing this project for technical assessment, the most relevant files are:

- `Genetic-Algorithm.ipynb` — **Evolutionary algorithm experiments and analysis**
- `Game.ipynb` — **Game‑tree search experiments and analytical discussion**

These notebooks contain the core implementations, experimental setups, and conclusions.

## Part I — Genetic Algorithm Experiments

The first part of the assignment explores **Genetic Algorithms (GA)** as a general‑purpose optimization technique.

The problem formulation involves optimizing a set of continuous parameters representing a mathematical model (based on Fourier series) in order to approximate a target function.

### Algorithmic Scope

The Genetic Algorithm experiments investigate standard evolutionary concepts, including:

- Solution representation and chromosome encoding
- Fitness function definition and evaluation
- Selection mechanisms and selection pressure
- Crossover and mutation operators
- Population‑based search dynamics

The goal is to understand how these design choices influence convergence behavior and solution quality.

### Experimental Focus

Rather than optimizing for a single best configuration, the experiments emphasize:

- Sensitivity of results to hyperparameters
- Stability of convergence across runs
- Trade‑offs between exploration and exploitation
- Common failure modes such as premature convergence

Results are visualized and discussed to support empirical observations.

## Part II — Game‑Tree Search Experiments

The second part of the assignment studies **search‑based decision making** in a deterministic, turn‑based board game environment.

A **base game framework and core mechanics were provided by the course teaching assistants**.  
The focus of this work is on **search algorithms and analysis**, not on implementing the game engine itself.

### Primary Experimental Artifact

The main analysis for this part is contained in **`Game.ipynb`**, which is the largest notebook in the repository (approximately **1935 lines**).

This notebook serves as an integrated experimental report, combining:
- Search algorithm logic
- Experimental configurations
- Observations and comparisons
- Analytical discussion

### Search Algorithms Examined

Within the provided game environment, the following classical game‑tree search techniques are examined:

- Minimax search
- Alpha–beta pruning
- Depth‑limited search
- Heuristic evaluation of non‑terminal states

These algorithms are treated as **objects of study**, with emphasis on their computational properties rather than competitive gameplay strength.

### Search Algorithms Examined

Within the provided game environment, the following classical game‑tree search techniques are examined:

- Minimax search
- Alpha–beta pruning
- Depth‑limited search
- Heuristic evaluation of non‑terminal states

These algorithms are treated as **objects of study**, with emphasis on their computational properties rather than competitive gameplay strength.

### Alternative Decision Models

The notebook also includes conceptual discussion of alternative decision‑making models, such as **Expectimax**, to contrast different assumptions about opponent behavior.

This discussion is comparative and analytical in nature.

## Repository Structure

├── Game.ipynb               # Game‑tree search experiments and analysis  
├── Genetic-Algorithm.ipynb  # Genetic Algorithm experiments and discussion  
├── README.md  
└── .gitignore

## How to Run

1. Install Python 3.x
2. Install common scientific dependencies if needed:

   pip install numpy matplotlib

3. Open and run the notebooks:
   - `Genetic-Algorithm.ipynb`
   - `Game.ipynb`

Each notebook is self‑contained and can be executed independently.

## Experimental Nature

The results obtained in this project align with classical theoretical expectations for evolutionary algorithms and search‑based decision making.

The emphasis is on **observing trends, limitations, and trade‑offs**, rather than producing optimal or competitive agents.

## Authorship and Attribution

### Provided Skeleton Code
The following components were provided by the course instructors and teaching assistants:

- Base game logic and environment used in `Game.ipynb`

These components define the problem environment but do **not** implement the experimental analysis.

### My Contributions
My work in this repository includes:
- Experimental design and configuration
- Implementation of search and optimization logic within the notebooks
- Parameter exploration and empirical evaluation
- Analytical discussion of algorithmic behavior and limitations

## License

This repository is released under the MIT License.

The license applies **only to my original code and documentation**.
Any instructor‑provided or TA‑provided materials remain the intellectual property of their original authors and are included solely for educational purposes.
