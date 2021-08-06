# Quantum Computing

We used a truncated (regularized) Hamiltonian for the matrix quantum mechanics models which is constructed by considering a truncated Hilbert space.

The truncated Hilbert space is constructed starting from the individual matrix degrees of freedom.

We consider two types of matrix quantum mechanics models:

- a bosonic 2-matrix model with SU(2) gauge group, which has 6 bosonic degrees of freedom in total.
- a supersymmetric 2-matrix model with SU(2) gauge group which corresponds to the [BMN model](https://arxiv.org/abs/hep-th/0202021) with the minimal number of degrees of freedom (`minimal BMN`), 6 bosons and 3 fermions.


## Software

### QuTiP

The calculation of the spectrum of the truncated Hamiltonian for the matrix quantum mechanics models is done using [`qutip`](https://www.qutip.org).

The annihilation operators are created for the states in a truncated Hilbert space with a cutoff $\Lambda$ on the number of modes.

The codes for the bosonic matrix model and the minimal BMN model are available in [this repository](https://github.com/erinaldi/bmn2-qutip).

### QISKIT

Software [`qiskit`](https://www.qiskit.org)

## Results

Under construction.