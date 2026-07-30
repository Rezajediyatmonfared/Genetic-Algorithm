# Genetic Algorithm Optimization Projects

A curated collection of four independent Python projects that demonstrate how **Genetic Algorithms (GAs)** can solve classic optimization and search problems with elegant, biologically inspired techniques.

This repository is designed to be both **educational** and **practical**: it introduces the core mechanics of evolutionary computation and applies them to well-known problems in optimization, combinatorial search, and constraint handling.

---

## Table of Contents

- [Overview](#overview)
- [Projects Included](#projects-included)
- [Genetic Algorithm Workflow](#genetic-algorithm-workflow)
- [Core Genetic Operators](#core-genetic-operators)
- [Repository Structure](#repository-structure)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Results and Visualizations](#results-and-visualizations)
- [Technologies Used](#technologies-used)
- [Future Improvements](#future-improvements)

---

## Overview

Genetic Algorithms are a family of **metaheuristic optimization methods** inspired by natural selection, genetics, and evolution.

Instead of searching for one solution directly, a GA works with a **population** of candidate solutions and improves them over generations using:

- **Fitness evaluation** to measure solution quality
- **Selection** to preserve stronger candidates
- **Crossover** to combine useful traits from parents
- **Mutation** to maintain diversity and avoid premature convergence
- **Replacement** to iterate toward better generations

These projects show how the same evolutionary framework can be adapted to very different problem types.

---

## Projects Included

### 1. Standard / Simple Genetic Algorithm (SGA)

A foundational implementation of a genetic algorithm for a basic optimization task such as:

- maximizing a mathematical function
- matching a target bitstring
- solving a simple search problem

**Highlights:**
- Binary chromosome encoding
- Roulette-wheel selection
- Single-point crossover
- Bit-flip mutation
- Generation-by-generation fitness tracking
- Convergence curve visualization

---

### 2. Traveling Salesperson Problem (TSP)

A classic combinatorial optimization problem where the goal is to find the shortest route that visits each city exactly once and returns to the starting point.

**Highlights:**
- Permutation-based chromosome representation
- Ordered Crossover (OX) or PMX crossover
- Swap or inversion mutation
- Distance-based fitness function
- Route visualization on a 2D map

---

### 3. Knapsack Problem

A constrained optimization problem in which the objective is to maximize total value without exceeding a fixed weight capacity.

**Highlights:**
- Custom item definitions with weights and values
- Constraint handling through penalty or repair strategies
- Fitness evaluation based on total value and capacity limits
- Progress tracking across generations
- Visualization of optimization behavior

---

### 4. 8-Queens Puzzle

A well-known chess puzzle that requires placing 8 queens on an \(8 \times 8\) board so that no two queens attack each other.

**Highlights:**
- Array-based board representation
- Conflict-minimization fitness function
- Maximum fitness target of 28 non-attacking pairs
- Final board visualization
- Elegant example of GA-based constraint solving

---

## Genetic Algorithm Workflow

Each project follows the same evolutionary cycle:

1. **Initialize** a population of random solutions
2. **Evaluate** each individual using a fitness function
3. **Select** the best candidates for reproduction
4. **Crossover** parents to create offspring
5. **Mutate** offspring to preserve diversity
6. **Replace** the current population with the new generation
7. **Repeat** until the stopping condition is met

Stopping conditions may include:
- reaching the maximum number of generations
- reaching an optimal or near-optimal fitness score
- convergence of the population

---

## Core Genetic Operators

The repository demonstrates several common GA operators:

- **Selection:** roulette wheel, tournament, or fitness-based selection
- **Crossover:** single-point, ordered crossover, PMX
- **Mutation:** bit-flip, swap, inversion
- **Replacement:** generational update strategy
- **Fitness Evaluation:** problem-specific scoring functions

---

## Repository Structure
```text
├── project1_sga/
├── project2_tsp/
├── project3_knapsack/
├── project4_8queens/
├── README.md
└── requirements.txt
