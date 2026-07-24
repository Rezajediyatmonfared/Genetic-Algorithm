Genetic Algorithm Optimization Projects

This repository contains a collection of four independent projects demonstrating the power and application of Genetic Algorithms (GAs) to solve complex optimization and search problems.

Genetic Algorithms are metaheuristic optimization techniques inspired by the process of natural selection, biological evolution, and genetics. These projects are implemented in Python and cover both fundamental concepts and classic computer science problems.



📋 Table of Contents





Overview of Genetic Algorithms



Included Projects





Project 1: Standard/Simple Genetic Algorithm (SGA)



Project 2: Traveling Salesperson Problem (TSP)



Project 3: Knapsack Problem



Project 4: 8-Queens Puzzle



Repository Directory Structure



Installation & Setup



How to Run



Core Genetic Operators Used



🧠 Overview of Genetic Algorithms

Genetic Algorithms operate on a population of potential solutions (called chromosomes or individuals). Over successive generations, the population evolves toward an optimal solution by mimicking biological processes:





Fitness Evaluation: Each individual is evaluated using a problem-specific fitness function.



Selection: Individuals with higher fitness are selected with higher probability to pass their genes to the next generation.



Crossover (Recombination): Pairs of parent individuals exchange genetic material to produce new offspring.



Mutation: Random changes are introduced into offspring genes to maintain genetic diversity and prevent premature convergence.



Replacement: The new generation replaces the old one, and the process repeats until a termination criterion is met (e.g., maximum generations reached or target fitness achieved).



🚀 Included Projects

Project 1: Standard/Simple Genetic Algorithm (SGA)





Description: A foundational implementation of a genetic algorithm designed to solve a basic search problem (such as optimizing a mathematical function ( f(x) ) or matching a target text string/bitstring).



Key Focus: Demonstrates binary encoding, simple single-point crossover, bit-flip mutation, and roulette-wheel selection.



Features:





Real-time generation logging (best fitness, average fitness).



Visualization of the fitness convergence curve over generations.

Project 2: Traveling Salesperson Problem (TSP)





Description: Finds the shortest possible route that visits a set of coordinates/cities exactly once and returns to the origin city.



Key Focus: Illustrates permutation encoding (where genes represent the visit order of cities).



Features:





Dynamic coordinate plotting of the cities.



Custom operators: Ordered Crossover (OX) or PMX (Partially Mapped Crossover) to avoid duplicate cities, and Swap/Inversion Mutation.



Visual output showing the optimized route mapped on a 2D plane.

Project 3: Knapsack Problem





Description: Given a set of items, each with a weight and a value, determine the number of each item to include in a collection so that the total weight is less than or equal to a given limit and the total value is as large as possible.



Key Focus: Deals with constrained optimization where invalid solutions (exceeding weight capacity) are either penalized or repaired during the fitness evaluation.



Features:





Customizable item lists (weights, values) and knapsack weight capacity.



Visualization of total value vs. total weight progression across generations.

Project 4: 8-Queens Puzzle





Description: The classic chess puzzle of placing 8 queens on an ( 8 \times 8 ) chessboard such that no two queens threaten each other (no two share the same row, column, or diagonal).



Key Focus: Shows how to represent chessboard configurations as arrays and construct a fitness function based on minimizing conflicts.



Features:





Fitness function defined by the number of non-attacking queen pairs (target maximum = 28).



Visual text/graphical representation of the final chessboard layout.



