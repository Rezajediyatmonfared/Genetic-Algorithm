# Knapsack Problem Using Genetic Algorithm

This project solves the **0/1 Knapsack Problem** using a **Genetic Algorithm (GA)**.

## Problem Statement

In the Knapsack Problem, we have a set of items, each with a **profit** and a **weight**.  
The goal is to select a subset of items such that:

- the **total weight** does not exceed the knapsack capacity
- the **total profit** is maximized

This is a classic optimization problem and is widely used in combinatorial optimization.

## Project Overview

This project implements a Genetic Algorithm to search for a high-quality solution to the knapsack problem.

Each solution is represented as a **binary chromosome**:

- `1` → the item is selected
- `0` → the item is not selected

The algorithm evolves a population of solutions over multiple generations using:

- **Initial population generation**
- **Crossover**
- **Mutation**
- **Fitness evaluation**
- **Sorting and selection**

## Input Parameters

The project uses the following main parameters:

- `N` → number of items
- `MAX_WEIGHT` → maximum allowed weight of the knapsack
- `objects` → list of items in the form `(profit, weight)`
- `POPULATION_SIZE` → number of individuals in the population
- `MUTATION_RATE` → mutation probability
- `EPOCH` → number of generations

## Example Data
```python
N = 7
MAX_WEIGHT = 14
objects = [(10,2), (5,3), (15,5), (7,7), (6,1), (18,4), (3,1)]

