---
title: Ising Model
math: true
weight: 1
---

## Hamiltonian

The Ising model, named after Ernst Ising, is a useful lattice model in staistical mechanics for describing ferromagnetic or antiferromagnetic spin interactions. The model Hamiltonian is usually written as
$$
H = -J\sum_{\langle ij\rangle} \sigma_i\sigma_j -h\sum_{i} \sigma_i,
$$
where $\sigma_i$ takes dicrete values of $+1$ or $-1$, the indices $\langle ij\rangle$ label nearest-neighbor lattice sites, $J$ represents interaction strength between two neighboring sites, $h$ denotes the strength of an external magnetic field, $\sigma_i$ takes discrete values of $1$ and $-1$, representing up and down spin orientations, respectively. When $J>0$ ($J\lt 0$), the neighboring spins tend to align in the same (opposite) direction(s) to lower the system's energy, resulting in a ferromagnetic (antiferromagnetic) state at low temperatures. When the external field $h$ is turned on, it can compete with the nearest-neighbor interactions and disturb the ferro- or antiferro- magnetic states.


