---
draft: false
---

[[Expected Return]] is measured as the weighted sum of returns.

# Portfolio variance
Measured as the sum of individual variances of products and their interaction terms. 

For two assets, it is:
$$
\sigma_p^2=x_1^2\sigma_1^2+x_2^2\sigma_2^2+2x_1x_2\rho_{1,2}\sigma_1\sigma_2
$$
Where:
- $x_a$ is the weight / proportion of a given asset $a$.
- $\sigma_a$ is the variance of a given asset $a$.
- $\rho_{a,b}$ is the correlation of asset $a$ to asset $b$.

## Effect of Correlation

|Correlation|Risk Effect|
|---|---|
|+1|No diversification benefit|
|Between 0 and 1|Some risk reduction|
|0|Good diversification|
|-1|Maximum risk reduction|

For example:
- ρ = 1 → SD = 27.4%
- ρ = 0.26 → SD = 22%
- ρ = -1 → SD = 6.1%

Lower correlation → lower portfolio risk.

# High Diversification
Variance can be broken down to this equation:
$$\text{Total Variance} = \text{Systematic Risk} + \text{Unsystematic Risk}$$
Note that systematic risk has a bias weight term of [[Beta Sensitivity]] - how your portfolio reacts to the national economy.
$$\sigma_p^2 = \underbrace{\beta_p^2 \sigma_m^2}_{\text{Systematic Portfolio Risk}} + \underbrace{\sum x_i^2 \sigma_{\epsilon,i}^2}_{\text{Unsystematic Portfolio Risk}}$$

If you have a well-diversified portfolio, the "unsystematic" part becomes negligible, leaving you with a direct mathematical relationship:

$$\sigma_p^2 \approx \beta_p^2 \times \sigma_m^2$$

- **$\beta_p^2$**: Your portfolio's sensitivity squared.
- **$\sigma_m^2$**: The variance of the entire market.