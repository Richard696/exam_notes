Regularization
==============

- reduce variance-bias trade off
- avoid the model overfit
- total error = RSS + λ||w||
- high λ - low variance

===============================
Bias is the error in fitting a model

Bias high -> underfit
Bias low -> just nice
Bias very low -> overfit

===============================
Variance is the measure of the variation among the fits 
of different samples training sets on the same population

=================================
Bias & Variance

AS the complexity of the model increase, 
the bias decrease.
However, teh variance will increase as the model 
complexity increase to a threshold.

A good fit model has minimum error on the training set,
however it may not generalise well to the population.
Hence, the validation set might give a higher error.

Therefore, there is a  trade off between bias and variance.

-----------------------------------------
Identify High Bias and High Variance

HIgh bias:
- HIgh training error
- Validation erro is similar to training error

HIgh Variance:
- Low training error
- HIgh validation error

---------------------------------
Ways to Reduce Bias

- Increase training data
- Increase model complexity
    - Increase number of features (increase the information for the model to learn) -> normally used in linear model
    - Use model selection to increase model selection
        - Normally use in non-linear model

===============================================

Types
-----
Different between l1 and l2 is the penalty term


- l1 norm - λ||w₀|| + λ||w₁||
- l2 norm - λ||w₀^2|| + λ||w₁^2|| -> ridge regression -> square magnitude

Ridge Regression
----------------
- use l2 regularization
- reduce model complexity by shrinking model parameters
λ is the tuning parameter that decides how much we want to penalise the fexibility of our model.


Lasso Regression
----------------
- use l1 regularization
- least absolute shrinkage selector operator
- perform feature selection (eliminate some features)
- reduce other parameters
- useful when large number of features involved


Elastic net Regression
----------------------
- use both l1 and l2 regularization
- error = RSS + λ₁||w||¹ + λ₂||w||²
- alpha = λ₁ + λ₂
- l1_ratio = λ₁ / (λ₁ + λ₂)
- if l1_ratio = 1, λ₂ = 0, lasso regression
- if l1_ratio = 0, λ₁ = 0, ridge regression
- otherwise, combination of ridge and lasso regression
