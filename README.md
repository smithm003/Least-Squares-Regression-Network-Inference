# Least-Squares-Regression-Network-Inference
Attempt at inferring pi vector from COVID data by using a least squares regression model

# Main-Motivation
Consider a population consisting of n different sub-populations (demes) divided up based on geographic location, age, etc. Under neutrality, we can assume that the frequencies $f_i(t)$ of a particular lineage in population $i$ at time $t$ depends linearly on the lineage frequencies $f_j(\tau)$ $(j=1,...n)$ at an earlier time $\tau<t$, \
$f_i(t)=\sum^n_{j=1}\mathbf{A}_{ij}(t;\tau)f_j(\tau)+noise$ \
where A is a right stochastic $n \times n$ matrix with non-negative elements and each row summing to 1. \ 



