---
title: Measurements
math: true
weight: 4
---

After the system reaches equilibrium, we can measure physical quantities such as:

### Magnetization:
  $$
  M = \frac{1}{N} \sum_i s_i^z,
  $$
  where $N$ is the total number of spins.
  
### Energy:
  $$
  E = -J \sum_{\langle i,j \rangle} s_i^z s_j^z - h \sum_i s_i^z.
  $$
  
### Magnetic susceptibility: 

The magnetic susceptibility $\chi$ measures the response of the system's magnetization to an external magnetic field. It is defined as:
$$
\chi = \frac{\partial \langle M \rangle}{\partial h},
$$
where $\langle M \rangle$ is the average magnetization, and $h$ is the external magnetic field. In Monte Carlo simulations, $\chi$ is computed from the fluctuations in the magnetization $M$ using the formula:
$$
\chi = \frac{\beta}{N} \left( \langle M^2 \rangle - \langle M \rangle^2 \right),
$$
where:
- $\beta = 1/(k_B T)$ is the inverse temperature,
- $N$ is the total number of spins,
- $\langle M \rangle$ is the average magnetization,
- $\langle M^2 \rangle$ is the average of the squared magnetization.

### Specific Heat:

The specific heat $C$ measures the system's heat capacity, or how much energy is required to change its temperature. It is defined as:
$$
C = \frac{\partial \langle E \rangle}{\partial T},
$$
where $\langle E \rangle$ is the average energy of the system.

In Monte Carlo simulations, $C$ is computed from the fluctuations in the energy $E$ using the formula:
$$
C = \frac{\beta^2}{N} \left( \langle E^2 \rangle - \langle E \rangle^2 \right),
$$
where:
- $\beta = 1/(k_B T)$ is the inverse temperature,
- $N$ is the total number of spins,
- $\langle E \rangle$ is the average energy,
- $\langle E^2 \rangle$ is the average of the squared energy.
