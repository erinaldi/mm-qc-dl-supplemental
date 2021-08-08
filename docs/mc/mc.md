# Lattice Monte Carlo

This section collects the results of Markov Chain Monte Carlo integration of the lattice path integral for the bosonic matrix model with different gauge groups SU($N$) and gauge couplings $\lambda = g^2 N$.

We study the energy observable $E$ as a function of the lattice size $n_t$ and the temperature $T$ towards the continuum limit.

The code for the data analysis is in [this repository](https://github.com/erinaldi/bmn2-lattice).

## Simulations 

We report results for the following parameters.

Gauge groups:

* SU(2) and SU(3)

't Hooft couplings:

* $\lambda \in [0.5, 1.0, 2.0]$

Lattice sizes:

* $n_t \in [16, 24, 32, 48, 64, 96, 128, 192]$

Temperatures:

* $T \in [0.0025, 0.05, 0.1, 0.15, 0.2, 0.25, 0.3, 0.35, 0.4]$


## Results

The Markov Chain Monte Carlo (MCMC) chain for the energy observable at each of the parameters in [Simulations](#simulations) is plotted as a function of Molecular Dynamics Time Units (MDTU).

Figures are collected in [Energy figures](./figures.md).