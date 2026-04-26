# Grover’s Algorithm for Feature Selection

## Overview

This project explores the application of Grover’s Algorithm and Grover Adaptive Search (GAS) to the problem of feature selection in machine learning. It demonstrates how quantum search techniques can be adapted to solve combinatorial optimization problems involving large feature spaces.

## Purpose

Feature selection is critical for improving model accuracy, reducing overfitting, and lowering computational cost. However, the number of possible feature subsets grows exponentially (2^n), making exhaustive search impractical for large datasets.

This project investigates whether quantum-inspired algorithms like Grover’s Algorithm can provide a more efficient way to search for optimal feature subsets.

## Technologies Used

* Python
* Qiskit (quantum simulation)
* Google Colab
* NumPy
* Matplotlib

## Key Concepts

* Grover’s Algorithm (quantum search)
* Grover Adaptive Search (optimization extension)
* Feature selection as a binary optimization problem
* Oracle-based evaluation functions
* Amplitude amplification

## Implementation

This project includes two implementations:

### 1. Grover Adaptive Search (Simple Oracle)

* Demonstrates GAS using a simplified scoring function
* Compares against classical exhaustive feature selection

Notebook:
https://colab.research.google.com/drive/1PopVyxSyo-NHtay_pnfnts1wTqPOIGDZ

---

### 2. Classical vs Quantum (Complex Oracle)

* Uses a more complex feature interaction model
* Evaluates scalability and performance differences

Notebook:
https://colab.research.google.com/drive/1Pxy9O-bR8GhVKZHLbIcMJLh9UDZ_qald

---

## Results

* Classical exhaustive search outperformed GAS in small feature spaces (~1s vs ~32s)
* This is expected due to:

  * Simulation overhead of quantum algorithms
  * Small problem size
* GAS shows theoretical advantages for:

  * Larger feature spaces
  * More complex evaluation functions

## My Contribution

* Designed feature selection as a binary optimization problem
* Implemented Grover Adaptive Search using Qiskit
* Built custom oracle functions for evaluating feature subsets
* Compared quantum-inspired approach against classical baseline
* Analyzed performance trade-offs and scalability limitations

## Key Takeaways

* Quantum algorithms offer **theoretical speedups**, not immediate practical gains
* Simulation on classical hardware introduces significant overhead
* GAS is better suited for **large-scale, high-complexity problems**

## Challenges

* Simulating quantum algorithms efficiently on classical hardware
* Designing an oracle function that reflects realistic feature interactions
* Managing exponential growth in feature space

## Future Work

* Run experiments on real quantum hardware
* Improve oracle complexity for more realistic datasets
* Explore hybrid classical-quantum approaches

## Paper

The full research paper is available in the `paper/` directory.
