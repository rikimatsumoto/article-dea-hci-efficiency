# Benchmarking Human Capital Spending Efficiency Using Bootstrapped DEA

This repository provides code and resources to replicate the analysis from the article: ["Benchmarking Human Capital Spending Efficiency Using Monte Carlo Data Envelopment Analysis"](https://medium.com/@rikimatsumoto/benchmarking-human-capital-spending-efficiency-using-monte-carlo-data-envelopment-analysis-6b184d2a6c77). The analysis demonstrates how resampling and Data Envelopment Analysis (DEA) can be combined to assess the efficiency of public spending on human capital.

## Overview
Bootstrap Data Envelopment Analysis (BDEA) is an advanced approach to measuring efficiency under conditions of uncertainty. This repository focuses on benchmarking government spending on human capital—such as education and health—by applying MCDEA techniques to identify efficiency frontiers and assess performance across countries or regions.

The methodology involves:
1. Simulating multiple iterations of data using Monte Carlo techniques to account for variability.
2. Applying DEA to each simulation to calculate efficiency scores.
3. Aggregating results to obtain robust efficiency estimates.

## Features
- **Bootstrap re-sampling**: Resamples dataset to model uncertainty in estimated statistics of input-output relationships.
- **Data Envelopment Analysis (DEA)**: Evaluates the efficiency of decision-making units (DMUs).
- **Benchmarking Human Capital Efficiency**: Focuses on public spending in education and health, benchmarking countries’ performance.
- **Visualization**: Provides plots to illustrate efficiency scores and variability across simulations.

### Example Workflow:
1. **Bootstrap resampling**: Resample 1000 input-output data from the full dataset, representing education and health spending.
2. **Apply DEA**: Use the `Benchmarking` R package to calculate efficiency scores for each simulation.
3. **Aggregate Results**: Summarize the efficiency scores and generate visualizations using `ggplot2`.

## Example Output
| Country   | Simulated Efficiency Score (Mean) | Standard Deviation |
|-----------|-----------------------------------|-------------------|
| Country A | 0.85                              | 0.05              |
| Country B | 0.78                              | 0.10              |
| Country C | 0.90                              | 0.03              |

## License
This project is open-source under the MIT License. Feel free to use and modify it as needed.

## Reference
Matsumoto, Riki. [Benchmarking Human Capital Spending Efficiency Using Monte Carlo Data Envelopment Analysis](https://medium.com/@rikimatsumoto/benchmarking-human-capital-spending-efficiency-using-monte-carlo-data-envelopment-analysis-6b184d2a6c77). Medium, 2025.
