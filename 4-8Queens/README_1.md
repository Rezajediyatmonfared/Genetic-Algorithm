# N-Queens Solver with Genetic Algorithm

This project demonstrates how to solve the classic **N-Queens problem** using a **Genetic Algorithm (GA)** in Python.

The implementation represents each chessboard as a permutation, applies evolutionary operators such as **selection**, **crossover**, and **mutation**, and iteratively improves the population until a valid solution is found or the maximum number of generations is reached.

## What Is the N-Queens Problem?

The **N-Queens problem** asks:

> How can `N` queens be placed on an `N x N` chessboard so that no two queens attack each other?

Since queens can move horizontally, vertically, and diagonally, a valid solution must ensure:

- No two queens share the same row
- No two queens share the same column
- No two queens share the same diagonal

In this project, the problem is solved for `N = 8`, but the code can be adapted for other values of `N`.

## Why Use a Genetic Algorithm?

A Genetic Algorithm is a search and optimization technique inspired by natural evolution. It works well for combinatorial problems like N-Queens because it can efficiently explore a large search space without checking every possible arrangement.

This project uses a GA to:

- Generate a population of candidate boards
- Evaluate each board using a fitness function
- Select better candidates for reproduction
- Combine parents using crossover
- Introduce diversity using mutation
- Repeat until a valid solution is found

## Project Features

- Solves the N-Queens problem using a genetic algorithm
- Uses permutation-based board representation
- Prevents row and column conflicts by design
- Measures fitness based only on diagonal conflicts
- Includes tournament selection
- Uses ordered crossover logic for valid offspring generation
- Applies swap mutation
- Prints the final solution and a visual board layout

## Board Representation

Each board is represented as a list of integers.

Example:
```python
[4, 2, 0, 6, 1, 7, 5, 3]

