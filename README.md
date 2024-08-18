<div>
  <img src="https://raw.githubusercontent.com/GeorgeTelles/georgetelles/f69531ec6b293b5148563588a764c010015d315e/logo_clara.png" alt="logo clara" width="300" style="display: inline-block; vertical-align: top; margin-right: 10px;">
  <img src="https://raw.githubusercontent.com/GeorgeTelles/georgetelles/f69531ec6b293b5148563588a764c010015d315e/logo_dark.png" alt="logo dark" width="300" style="display: inline-block; vertical-align: top;">
</div>

# Portfolio Simulation with the Monte Carlo Method

## Introduction

Analyzing and optimizing financial portfolios are complex challenges that require advanced techniques to estimate the future behavior of assets and assess risk. A powerful and widely used tool for these purposes is the Monte Carlo method. This project demonstrates how to use this statistical technique to simulate the behavior of a financial portfolio over time, providing valuable insights into potential returns and associated risks.

The Monte Carlo method stands out for its ability to solve complex mathematical problems through the generation of multiple random samples. Essentially, it allows for the simulation of future scenarios to better understand asset behavior under different market conditions. This methodology is ideal for situations where analytical solutions are not feasible, offering a practical and realistic view of future scenarios.

## Monte Carlo Method with Cholesky Decomposition

The Monte Carlo technique used in this project is enhanced by Cholesky decomposition, which plays a crucial role in generating realistic daily returns that preserve correlations between portfolio assets. Here are the key aspects of this approach:

### Rationale of the Method

1. **Generation of Random Variables**: The first step is to create random variables that follow a specific distribution. In the context of finance, this means generating daily returns that reflect the statistical characteristics of the assets.

2. **Use of the Covariance Matrix**: The covariance matrix is essential for understanding how different assets move relative to each other. It describes the relationship between asset returns and is crucial for simulating scenarios that reflect the real behavior of assets.

### Implementation

The formula used to calculate simulated daily returns is:

\[ R_t = \mu + LZ_t \]

Where:
- \( R_t \) is the vector of daily returns.
- \( \mu \) is the vector of average returns.
- \( L \) is the lower triangular matrix obtained from the Cholesky decomposition of the covariance matrix.
- \( Z_t \) is a vector of normally distributed random numbers.

### Cholesky Decomposition

Cholesky decomposition is a mathematical technique that decomposes a covariance matrix \( \Sigma \) into two lower triangular matrices \( L \) and their transposes \( L^T \). This approach allows for the generation of daily returns with specific asset correlations, preserving the covariance matrix structure and ensuring realistic simulations.

### Simulation

The simulation process involves the following steps:

1. **Data Import**: Historical asset price data is used to calculate daily returns and covariance matrices.

2. **Parameter Configuration**: Define the number of simulations and the time horizon for the portfolio simulation.

3. **Return Simulation**: Use Cholesky decomposition to generate simulated daily returns that capture the covariance between assets.

4. **Portfolio Returns Calculation**: Simulate portfolio behavior over time by applying different asset weights and calculating the accumulated return.

5. **Visualization and Analysis**: Plot simulation results and identify portfolios with the best performance.

## Results and Insights

The simulation results provide a detailed view of portfolio behavior under various scenarios. The analysis includes identifying the best-performing portfolios and visualizing how different weight configurations impact accumulated returns.

This project not only demonstrates the practical application of the Monte Carlo method and Cholesky decomposition but also provides a powerful tool for portfolio analysis and optimization. It serves as an example of how advanced techniques can be used to solve complex problems practically and efficiently.

## Conclusion

Monte Carlo simulation is an indispensable technique in financial analysis, offering deep insights into portfolio behavior and the impact of market variables. By applying Cholesky decomposition, this project illustrates a robust approach to generating realistic and informative scenarios, essential for investors and analysts looking to optimize their investment strategies.

For more details on Cholesky decomposition and the Monte Carlo method, refer to the [Wikipedia page on Cholesky Decomposition](https://pt.wikipedia.org/wiki/Fatora%C3%A7%C3%A3o_de_Cholesky).

---

Share this project and discover how advanced statistical techniques can transform financial analysis. For more updates and insights, follow my profile on [LinkedIn](https://pt.linkedin.com/in/georgetelles).
