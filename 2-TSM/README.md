# Traveling Salesman Problem (TSP) using Genetic Algorithm

This project solves the **Traveling Salesman Problem (TSP)** using a **Genetic Algorithm (GA)**.

## Project Description

The Traveling Salesman Problem is a classic optimization problem in which a salesman must visit a number of cities exactly once and return to the starting city, while minimizing the total travel distance.

In this project:

- A set of cities is defined using **2D coordinates (x, y)**.
- The goal is to find the **shortest possible route** that visits all cities once and returns to the origin.
- A **Genetic Algorithm** is used as the optimization technique.

## Problem Definition

Given:

- A number of cities (for example, **20 cities**)
- Each city represented by **x and y coordinates**

Find:

- The optimal route that minimizes the **total traveled distance**

## Method

The project uses a **Genetic Algorithm** with the following main steps:

### 1. Initial Population
A population of random candidate routes is generated.

### 2. Fitness Evaluation
Each route is evaluated based on its total travel distance.  
Shorter routes have better fitness.

### 3. Selection
Better candidate solutions are selected for reproduction using methods such as:

- **Tournament Selection**
- **Roulette Wheel Selection**

### 4. Crossover
Two parent routes are combined to produce new offspring.

Suggested crossover method:

- **Ordered Crossover (OX)**

### 5. Mutation
A mutation step is applied by randomly swapping two cities in a route.

### 6. Iteration
The algorithm repeats the cycle of:

- evaluation
- selection
- crossover
- mutation

for multiple generations until a stopping condition is reached.

## Objective Function

The objective is to minimize the total route distance:

\[
\text{Minimize } \sum_{i=1}^{n-1} d(city_i, city_{i+1}) + d(city_n, city_1)
\]

where \(d(a,b)\) is the Euclidean distance between two cities.

## Features

- Solves TSP using a metaheuristic approach
- Uses Genetic Algorithm operators
- Supports random population generation
- Can be extended with visualization and parameter tuning

## Possible Parameters

Some common parameters for this project may include:

- Population size
- Number of generations
- Mutation rate
- Crossover rate
- Selection strategy
- Stopping condition

## Project Structure

A possible project structure could be:
```bash
.
├── TSM.ipynb
├── TSM.pdf
└── README.md

