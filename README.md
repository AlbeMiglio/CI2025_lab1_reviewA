# Advanced Heuristics for Optimization Problems

This project investigates the application of a **custom hybrid optimization algorithm** designed to tackle complex optimization problems.  
The objective was to develop a method that outperforms traditional heuristics such as **Simulated Annealing** in both efficiency and solution quality.

## Methodology

At the core of the project lies a **hybrid algorithm** that merges population-based exploration techniques (similar to Evolutionary Algorithms) with intensive local search procedures.  
This combination allows for both broad exploration of the solution space and fine-tuned exploitation of promising areas.

## Observations & Results

The algorithm’s effectiveness varied according to the complexity of the problem:

* **Problems 1 and 2** — The hybrid algorithm consistently outperformed standard Simulated Annealing.  
  The trade-off between computational cost and performance was highly favorable, making it the recommended choice for these cases.

* **Problem 3** — This case presented a significant challenge: generating a single **valid** initial solution required approximately 20 seconds.  
  Since the hybrid method relies on multiple solution generations, it became impractical due to time constraints.

  To address this limitation, two alternative strategies were explored:
  1. Executing the hybrid algorithm starting from an **invalid** initial solution.
  2. Applying a standard **Simulated Annealing** algorithm, optimized by initializing it with one randomly generated **valid** solution.

## Conclusion

A cost–performance analysis indicates that the optimal approach depends on the problem characteristics:

* When valid solutions can be generated efficiently, the **custom hybrid algorithm** offers superior performance.
* For computationally demanding problems—such as **Problem 3**—the **optimized Simulated Annealing** method is more practical and efficient.

---

work with: (https://github.com/LucaFavole)
