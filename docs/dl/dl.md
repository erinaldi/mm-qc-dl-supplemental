# Deep Learning

The bosonic matrix model can be represented with a collection of complex variables $x_i$ representing the elements of $N \times N$ Hermitean matrices, for a SU($N$) gauge group.
We have studied the matrix model with 2 Hermitean matrices, so we will use 6 complex variables $x_i$ to represent our quantum states.
A vector in this 6-dimensional space is said to be in the _coordinate basis_ of our system.

We represent each state using a quantum neural ansatz, where a neural network architecture is used to map the element of the basis into the corresponding quantum amplitude or wave function.
If we denote by $X$ the vector of $x_i$ coordinates, we aim to find the function $\psi_\theta(X)=\langle X|\psi_\theta\rangle$.

For simplicity, we choose to parametrize the wave function norm (separetely from the wave function phase) as
$|\psi_\theta(X)| = \sqrt{p_\theta(X)}$ where $p_\theta(X)$, the wave function probability distribution, takes the following form:

$$ p_\theta(X) = p(x_1; F^0_\theta) p(x_2; F^1_\theta(x_1)) p(x_3; F^2_\theta(x_1, x_2)) \ldots $$

This is an autoregressive form: the parameters $F^i_\theta$ of the distribution $p(x_i; F^{i-1}_\theta(\ldots))$ of one coordinates $x_i$ only depend on the _previous_ coordinates $x_{i-1}$, etc...

The parameters $F^{i}_\theta(\ldots)$ are obtained from a fully-connected feed-forward neural network.

## Sofware

The code used for the variational quantum monte carlo with quantum neural state based on autoregressive flows is in [this repository](https://github.com/hanxzh94/minimal_BMN_MQM).

## Results

Under construction