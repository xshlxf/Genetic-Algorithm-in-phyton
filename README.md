# Genetic Algorithm for Resource Allocation in Distributed Systems

This project implements a Genetic Algorithm (GA) to optimize resource allocation in distributed computing environments. The algorithm aims to **minimize the makespan** and **maximize resource utilization** by efficiently assigning a set of tasks to a group of heterogeneous computing nodes.

## 💡 Problem Statement

Given:
- 5 nodes with different processing capacities.
- 10 tasks with specific resource demands.

Objective:
- Assign each task to a node in a way that minimizes the overall processing time (makespan) and balances the load across all nodes.

## ⚙️ How It Works

The GA evolves a population of possible solutions over multiple generations using:
- **Selection** (Tournament)
- **Crossover** (Uniform)
- **Mutation** (Random Reallocation)

Each individual represents a task-node assignment. The **fitness function** evaluates the quality of the assignment by computing:
- The total load on each node.
- The makespan (maximum load among nodes).

> Note: The fitness values are negative because the algorithm internally maximizes fitness, so minimizing the makespan is treated as maximizing its negative.

## 📊 Example Output

```text
Generation 1, Best Fitness: -2027
Generation 30, Best Fitness: -1027
Generation 50, Best Fitness: -1026
