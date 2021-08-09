# Matrix Models using Quantum Computing, Deep Learning, and Lattice Monte Carlo

This documentation website collects figures and tables supplementing the publication at [https://arxiv.org/abs/2108.02942](https://arxiv.org/abs/2108.02942).

We group figures and tables by the three different computational approaches used in the paper: *quantum computing*, *deep learning*, and *lattice Monte Carlo*.
## Quantum Computation

For the quantum computing approach we truncated the Hilbert space and obtain a truncated Hamiltonian describing the quantum mechanics of matrices.
Then we compute the eigenvalues and eigenstates of this truncated (regularized) Hamiltonian using two different methods:

  1. exact diagonalization (using [`qutip`](https://qutip.org))
  2. hybrid quantum-classical eigensolvers (using [`qiskit`](https://qiskit.org))

For more details you can check the [Quantum Computing](./qc/qc.md) tab at the top.

## Deep Learning

For the deep learning approach we use a neural quantum state ansatz with a variational quantum Monte Carlo framework to compute the ground state of the quantum matrix model.
The neural ansatz for the quantum state is based on neural autoregressive flows as in [Han & Hartnoll (2020)](http://dx.doi.org/10.1103/PhysRevX.10.011069)

For more details you can check the [Deep Learning](./dl/dl.md) tab at the top.

## Lattice Monte Carlo

For the lattice Monte Carlo approach, we discretize the time direction of the system on a Euclidean lattice and solve the sum over all matrices configurations in the path integral by using Hybrid Monte Carlo methods.
The path integral calculation allows us to compute expectation values of observables for the ground state.
The details of the algorithm are the same as in [Berkowitz et al. (2018)](http://link.springer.com/10.1007/JHEP06(2018)124).

For more details you can check the [Lattice Monte Carlo](./mc/mc.md) tab at the top.