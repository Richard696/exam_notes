Optimization Methods
====================

Machine Learning - Finding an Optimal Model
-------------------------------------------

1. model selection
2. model parameter learning
  - feature engineering
  - hyper parameter selection
3. model evaluation

- available data is used to optimize function(m)
- closed form solution - problem can be solved mathematically
- problem too large? Search for solution

Search Methods
--------------

* calculus-based
  * direct-method
  * indirect-method
- guided random search techniques
  - simulated annealing
  - evolutionary algorithms
- enumerative techniques
  - dynamic programming

### Zero Order / Direct Search Methods

- even sampling / grid search
- random sampling / random search

### Machine Learning

- simple linear regression (one variable)

    x    y    predict  error
    x₁   y₁   w₀+w₁x₁  y₁-(w₀+w₁x₁)
    x₂   y₂   w₀+w₁x₂  y₂-(w₀+w₁x₂)
    ...  ...  ...      ...
    xn   yn   w₀+w₁xn  yn-(w₀+w₁xn)

- RSS - residual sum of square / sum of square errors

### Gradient Descent

    differentiatiable function g, fixed step length a, and initial point w
    k = 1
    repeat until stopping condition is met:
        w^k = w^(k-1) - a▽g(w^(k-1))
        k <- k + 1

    gradient: ▽g(w^(k-1))

### Newtons Method

    twice differentiable function g, and initial point w^0
    k = 1
    repeat until stopping condition is met
        solve the system ▽^2g(w^(k-1))w^k = ▽^2g(w^(k-1))w^(k-1) - ▽g(w^(k-1)) for w^k
        k <- k + 1

### Tangent & Curvature

At high curvature true point, approximation of the curve is better than
approximation by Tangent.
