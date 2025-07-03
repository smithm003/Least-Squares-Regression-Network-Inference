# Least-Squares-Regression-Network-Inference
Attempt at inferring pi vector from COVID data by using a least squares regression model

# Background
Consider a population consisting of n different sub-populations (demes) divided up based on geographic location, age, etc. Under neutrality, we can assume that the frequencies $f_i(t)$ of a particular lineage in population $i$ at time $t$ depends linearly on the lineage frequencies $f_j(\tau)$ $(j=1,...n)$ at an earlier time $\tau<t$, \
$f_i(t)=\sum^n_{j=1}\mathbf{A}_{ij}(t;\tau)f_j(\tau)+noise$ \
where A is a right stochastic $n\times n$ matrix with non-negative elements and each row summing to 1. \
The coefficient $A\_{ij}$ represents the proportion of infections that population $i$ imports from population $j$ - hence A is referred to as the case importation matrix. 

# Equilibration-and-Reproductive-Value
The long-term expected frequency, denoted by $\pi_i$ is the same in all demes and depends only on the identity $i$ of the deme. The vector $\vec{\pi}=(\pi_1,...,\pi_n)^T$ composed of these primary deme-dependent long term frequencies is proportional to the left leading eiegnvector of the importation matrix and has an eigenvalue 1, and is also normalised to sum to 1 such that $\sum_i \pi_i=1$. It represents the expected contribution of deme $i$ to the futurew gene pool and is also called the class reproductive value. 

# Main-Motivation
The main motivation of this project is to identify the leading left eigenvector, $\pi$, from the COVID data available from the UK, initially using a least squares regression model under the assumption that the observed frequencies are in fact the true frequencies, and then attempting to take measurement noise into account




