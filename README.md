# Genetic Algorithm Implementation

This code implements a simple genetic algorithm (GA) for optimization problems using binary chromosomes, tournament selection, one-point crossover, mutation, and replacement.

## Overview

**Genetic Algorithm** is a search heuristic inspired by the process of natural selection. This code demonstrates the main steps of a GA: initialization, selection, crossover, mutation, and replacement, using binary strings as chromosomes and fitness defined by the sum of bits.

## Features

- **Binary Chromosomes:** Each individual is represented as a binary string of fixed length (default: 20).
- **Population Initialization:** Randomly generates initial population.
- **Tournament Selection:** Selects parents based on their fitness (sum of bits).
- **One-Point Crossover:** Combines parents to create offspring by swapping segments at a random point.
- **Bit-Flip Mutation:** Randomly flips bits in the offspring with a given mutation rate.
- **Replacement:** Replaces the least fit individuals in the population with the new offspring.

## Usage

1. **Input Parameters:**  
   The program asks for the following inputs:
   - **Generation number:** Number of generations to run.
   - **Population number:** Number of individuals in the population.
   - **Tournament selection ratio:** Fraction of the population to consider for selection.
   - **Mutation ratio:** Fraction of bits to mutate in each offspring.

2. **Execution:**  
   The algorithm runs for the specified number of generations, printing the state of the population and the results of each step (selection, crossover, mutation, replacement) for each generation.

## Example

This will run the genetic algorithm for 3 generations, with a population of 5, tournament selection ratio of 0.4, and mutation ratio of 0.1.

## Code Structure

- **GeneticAlgorithm Class:**  
  - `__init__`: Initializes parameters and population.
  - `CreateChromo`: Randomly generates initial chromosomes.
  - `printChromo`: Prints current population and fitness.
  - `Tournament`: Selects parents using tournament selection.
  - `Crossover`: Performs one-point crossover on selected parents.
  - `Mutation`: Mutates offspring by flipping bits.
  - `Replace`: Replaces the least fit individuals with new offspring.

## Output

The program prints the population, selected parents, crossover results, mutation results, and replacement actions for each generation.

---

**Note:**  
This is a simplified GA for educational purposes. For real-world optimization, consider more advanced selection, crossover, and mutation strategies.

