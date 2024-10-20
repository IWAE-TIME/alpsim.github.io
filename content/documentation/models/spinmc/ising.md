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
   
## Expectation Value
The model can be exactly solved in 1D. For higher dimensions, Monte Carlo simulations can be used. Let a lattice spin configuration be $\sigma=\{ \sigma_i \}$, where $i$ labels sites throughout the lattice. If the energy of a spin configuration $\sigma$ is given by $E(\sigma)$, then the distribution probability for such a configuration can be calculated by
$$
P(\sigma)=\frac{e^{-\beta E(\sigma)}}{Z},
$$
where $\beta=1/(k_BT)$ is inverse temperature, $k_B$ is Boltzmann constant, and the partition function is given by 
$$
Z=\sum_{\sigma}e^{-\beta E(\sigma)},
$$
where the summation is over all possible spin configurations on the lattice.

If the distribution probability can be obtained, the expectation (average) value of any operator $\hat{O}$ can be obtained by
$$
\langle \hat{O}\rangle = \sum_{\sigma} O(\sigma)P(\sigma),
$$
where the value for the operator $\hat{O}$ in configuration $\sigma$ has been evaluated to be  $O(\sigma)$.

## Monte Carlo Simulation
The process of Monte Carlo simulation is to sample the states based on their configuration distribution probabilities. Apparently, configurations with larger distribution probability appear more frequently than those with smaller distribution probabilities. The design of a specific Monte Carlo algorithm should ensure ergodicity, which states that all possible configurations of the system should be attainable. Metropolis algorithm is one such algorithm to sample system configurations. The following outlines the steps of the algorithm with local spin updates:
1. Initialize a configuration: a random configuration $\sigma$ is assigned to the system.
2. Propose a configuration change: a change of the configuration $\sigma \rightarrow \sigma^{\prime}$ is proposed.
3. Calculate the probability ratio: the distribution probability ratio $w=\frac{P(\sigma^{\prime})}{P(\sigma)}$ can be evaluated.
4. Generate a uniform random number $r\in [0,1]$.
5. Accept the configuration change if $w\ge r$; and reject the change if $w\lt r$.

Successive configurations generated this way form a Markov chain. It can be proved that importance sampling Metropolis algorithm satisfies detailed balance equation
$$
P(\sigma)P(\sigma\rightarrow\sigma^{\prime})=P(\sigma^{'})P(\sigma^{\prime}\rightarrow\sigma),
$$
where $P(\sigma\rightarrow\sigma^{\prime})$ is the probability of transitioning from configuration $\sigma$ to $\sigma^{\prime}$.
Therefore, it is both ergodic and very efficient in visiting all important configurations of the system. When configuration states are successively generated from such a process, they are naturally autocorrelated. It is recommended that a measurement of physical quantities is performed only after a certain number of steps (autocorrelation length) have passed, making each measurement an independent sample for average. 

## Measurements
Several physical quantities of interest can be measured in the Monte Carlo simulation.

### Energy
Energy is the easiest quantity to measure in the simulation, since the initial energy $E$ can be evaluated once an initial configuration $\sigma$ is assigned to the system. When a spin change at lattice site is accepted, one can easily keep track of the energy change $\Delta E$ associated with the local spin flip. The new configuration $\sigma^{\prime}$ has, therefore, an energy $E^{\prime}=E+\Delta E$.

### Magnetization
Magnetization is defined as the sum of all spin values in the lattice
$$
M=\sum_i\sigma_i,
$$
which represents a preferred spin orientation direction. Without an external magnetic field, all lattice sites will have the same spin orientation (all $+1$ or $-1$ values) at zero temperature for ferromagnetic interactions ($J\gt 0$). The system will spontaneously pick one of the two states at zero temperature, resulting in the lowest energy for the lattice and the maximum value of magnetization $M$. As temperature increases, the perfect ferromagnetic state is disturbed, leading to a smaller $M$. As expected, the external magnetic field $h$ can also influence the spin orientations by aligning spins along the direction of the magnetic field to lower the system's energy.
