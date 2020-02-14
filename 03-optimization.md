## Optimization (Search) Methods
- Mathematical/analytical solution -> applicable when the problem can be defined by mathematical equation and equation should be differentiable. 

- Iterative methods -> Numrical optimization

## SAmple Error/Loss Functions
Goal -> to find or search for the model or solution with the minimum loss or error. 

## Optimization (Gradient Descent)
===============================

Batch Gradient Descent
----------------------

* batch gradient descent performs parameters update in batch iteration (epoch)
+ fixed learning rate
+ straight trajectory
- slow if large dataset

Mini-batch Gradient Descent
---------------------------

* mini-batch uses random mini batches to perform parameters update for n epochs
+ faster than batch
+ can avoid redundant samples
- may not converge and probably require learning decay

Stochastic Gradient Descent
---------------------------

* stochastic gradient descent performs parameters update on each sample
* like mini-batch but with one example used for each learning step
+ faster than others
- more noise
- large variance since only one example used for each learning step

