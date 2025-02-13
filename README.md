```markdown
# Population-Based Simulated Annealing for Binary Optimization

This repository implements a Population-Based Simulated Annealing (SA) algorithm to solve binary optimization problems, specifically the Min One problem. The goal is to minimize the number of `1`s in a binary vector.

 Problem Description

The Min One problem is defined as:

\[
\min z = f(x) = \sum_{i=1}^n x_i
\]

where \( x_i \in \{0, 1\} \). The goal is to find a binary vector \( x \) that minimizes the number of `1`s.

 Algorithm Steps

1. Generate Initial Population: Create a population of random binary vectors.
2. Evaluate Population: Calculate the objective value for each solution.
3. Define Best Solution: Identify the best solution in the initial population.
4. Set Initial Temperature: Initialize the temperature \( T = T_0 \).
5. Repeat for Iterations:
   - Generate neighbors for each population member.
   - Sort all neighbors and select the best solutions to form the new population.
   - Update the best solution ever found.
   - Reduce the temperature.
6. Visualize Results: Plot the convergence of the best objective value, temperature reduction, and population diversity.

 Code Structure

- Objective Function: Computes the number of `1`s in a binary vector.
- Neighbor Generation: Flips one random bit in a binary vector to generate a neighbor.
- Population-Based SA: Implements the population-based SA algorithm.
- Visualizations: Uses `matplotlib` to plot the convergence and diversity of the population.

 Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/population-based-sa.git
   cd population-based-sa
   ```

2. Install dependencies:
   ```bash
   pip install matplotlib
   ```

3. Run the script:
   ```bash
   python population_based_sa.py
   ```

4. View the results:
   - The script will display plots showing the convergence of the best objective value, temperature reduction, and population diversity.

 Example Output

# Plots

1. Best Objective Value vs. Iterations:
   - Shows how the best objective value improves over iterations.

2. Temperature vs. Iterations:
   - Shows how the temperature decreases over iterations.

3. Population Diversity (Boxplot):
   - Shows the distribution of objective values in the population over iterations.

# Console Output

```
Initial Population:
  Solution 1: [1, 0, 1, 0, 1, 0, 1, 0, 1, 0], Value: 5
  Solution 2: [0, 1, 0, 1, 0, 1, 0, 1, 0, 1], Value: 5
  Solution 3: [1, 1, 0, 0, 1, 0, 1, 0, 0, 1], Value: 5
  Solution 4: [0, 0, 1, 1, 0, 1, 0, 1, 1, 0], Value: 5
  Solution 5: [1, 0, 0, 1, 0, 1, 0, 0, 1, 0], Value: 4
Initial Best Solution: [1, 0, 0, 1, 0, 1, 0, 0, 1, 0], Best Value: 4
Initial Temperature: 100
--------------------------------------------------
Iteration 1:
  Temperature: 95.0
  Best Solution: [0, 0, 0, 1, 0, 1, 0, 0, 1, 0], Best Value: 3
  Population:
    Solution 1: [0, 0, 0, 1, 0, 1, 0, 0, 1, 0], Value: 3
    Solution 2: [1, 0, 0, 1, 0, 1, 0, 0, 1, 0], Value: 4
    Solution 3: [0, 0, 1, 1, 0, 1, 0, 0, 1, 0], Value: 4
    Solution 4: [0, 0, 0, 1, 0, 1, 0, 0, 1, 0], Value: 3
    Solution 5: [0, 0, 0, 1, 0, 1, 0, 0, 1, 0], Value: 3
--------------------------------------------------
...
Final Best Solution: [0, 0, 0, 0, 0, 0, 0, 0, 0, 0], Final Best Value: 0
```

 Parameters

- `pop_size`: Size of the population.
- `n`: Dimension of the binary vector.
- `num_neighbors`: Number of neighbors to generate for each population member.
- `temp`: Initial temperature.
- `cooling_rate`: Rate at which the temperature decreases.
- `iterations`: Number of iterations.

 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

 Contributing

Contributions are welcome! Please open an issue or submit a pull request.

 Contact

For questions or feedback, please contact [Your Name](mailto:your-email@example.com).
```

---

# Key Files

1. `population_based_sa.py`:
   - The main script implementing the Population-Based SA algorithm and visualizations.

2. `README.md`:
   - The documentation file explaining the project, usage, and example output.

3. `LICENSE`:
   - The license file (e.g., MIT License).

---

# How to Use

1. Clone the repository.
2. Install dependencies (`matplotlib`).
3. Run the script and observe the results in the console and plots.

---

Let me know if you need further assistance!
