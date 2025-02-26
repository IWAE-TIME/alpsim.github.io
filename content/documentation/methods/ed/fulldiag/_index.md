
---
title: Full Diagonalization 
math: true
weight: 4
---

Full diagonalization of matrices is a powerful numerical method for understanding small quantum systems, especially when the excited states of a quantum system is required. We will focus on two numerical methods [**Jacobi rotation**](jacobi) and **QR factorization**, which are widely used in computational physics.

### 1. Jacobi Rotation Method

The Jacobi method is an iterative algorithm for diagonalizing symmetric matrices. It works by systematically eliminating off-diagonal elements through a series of rotations.

- **Key Idea**: The method applies a sequence of orthogonal transformations (rotations) to the matrix, gradually reducing the magnitude of the off-diagonal elements. Each rotation targets the largest off-diagonal element and zeros it out.
  
- **Algorithm**:
  1. Identify the largest off-diagonal element \( A_{ij} \) in the matrix \( A \).
  2. Construct a rotation matrix \( R \) that zeroes out \( A_{ij} \).
  3. Update the matrix \( A \) as \( A' = R^T A R \).
  4. Repeat the process until all off-diagonal elements are sufficiently small.

- **Advantages**:
  - Simple and robust for small to medium-sized matrices.
  - Guaranteed to converge for symmetric matrices.

- **Limitations**:
  - Slow convergence for large matrices.
  - Not efficient for sparse matrices.

- **Application in Quantum Mechanics**: The Jacobi method is often used to diagonalize Hamiltonians in small quantum systems, such as spin chains or small molecular systems.

---

### 2. QR Factorization

The QR algorithm is one of the most widely used numerical methods for diagonalizing general matrices. It is based on the decomposition of a matrix into an orthogonal matrix \( Q \) and an upper triangular matrix \( R \).

- **Key Idea**: The QR algorithm iteratively applies the QR decomposition to a matrix, converging it to a diagonal or triangular form containing the eigenvalues.

- **Algorithm**:
  1. Factorize the matrix \( A \) into \( Q \) and \( R \): \( A = QR \).
  2. Compute the updated matrix \( A' = RQ \).
  3. Repeat the process until \( A' \) converges to a diagonal matrix (for symmetric matrices) or a triangular matrix (for non-symmetric matrices).

- **Advantages**:
  - Efficient for large matrices.
  - Works for both symmetric and non-symmetric matrices.

- **Limitations**:
  - Requires multiple iterations for convergence.
  - Computationally expensive for very large matrices.

- **Application in Quantum Mechanics**: The QR algorithm is commonly used to diagonalize large Hamiltonians in many-body quantum systems, such as those arising in condensed matter physics or quantum chemistry.

---



## Comparison of Numerical Methods

| Method              | Matrix Type       | Efficiency       | Applications in Quantum Mechanics          |
|---------------------|-------------------|------------------|-------------------------------------------|
| Jacobi Rotation     | Symmetric         | Small matrices   | Small quantum systems, spin chains        |
| QR Factorization    | General           | Large matrices   | Many-body systems, quantum chemistry      |
| Lanczos Algorithm   | Sparse symmetric  | Very large       | Lattice models, quantum field theory      |
| Power Iteration     | General           | Dominant eigen   | Ground state calculations                 |
| Arnoldi Iteration   | Non-symmetric     | Large sparse     | Open quantum systems, dissipative systems |

---

## Conclusion

Numerical methods for matrix diagonalization are indispensable tools in quantum mechanics, enabling the study of complex systems that cannot be solved analytically. Techniques such as Jacobi rotation, QR factorization, Lanczos algorithm, power iteration, and Arnoldi iteration provide efficient and accurate ways to approximate eigenvalues and eigenvectors, even for large or sparse matrices. The choice of method depends on the specific properties of the matrix and the physical system under investigation. By leveraging these numerical techniques, researchers can gain deeper insights into the behavior of quantum systems, from small molecules to large-scale many-body problems.

## Introduction

The `fulldiag` package uses LAPACK library for a complete diagonalization of the Hamiltonian. Hence, it can be used for computing thermodynamic properties of any model that can be defined using the ALPS libraries. The main limitation is one of size, i.e., memory and CPU time may become unacceptable at sizes where other, more specialized applications still work well.

Release 1.3 allows the computation of magnetic or charge properties properties for models with a coupling to a conserved quantity of the form $-hS\_z$ or $-\mu N$, i.e., a SITETERM $-h S_z(i)$ or $-\mu n(i)$. In fact, adaptation to other situations with a coupling to a conserved quantity should be relatively straightforward by changing a few lines in the source file fulldiag.h (this is just not supported at the moment, since it requires the modification of at least 5 strings by the user). If the conserved quantity is not present, two quantities less will be evaluated (see below).

**Warning:** Incorrect results may be obtained if the supposed conserved quantity does actually not commute with the Hamiltonian. Incorrect results will also in general be obtained if the coefficients are not of the above form, and the magnetic field $h$ or chemical potential $\mu$ are changed by `fulldiag_evaluate`.


## Running a computation

is discussed in the `fulldiag` tutorial. After obtaining the full spectrum using the `fulldiag` program, the evaluation program `fulldiag_evaluate` can be used to efficiently produce XML plot files of the thermodynamic as well as magnetic properties, specified below.

### Input parameters

The parameters for the `fulldiag` application are all described among the common input parameters (note in particular the additional parameters for exact diagonalization).
The following further parameters are used only by `fulldiag_evaluate`:

| **Parameter** | **Default** | **Meaning** |
| :------------ | :---------- | :---------- |
| T_MIN |  | lowest temperature for which obervables are calculated |
| T_MAX |  | highest temperature for which obervables are calculated |
| DELTA_T | | temperature step width |
| couple | | couple mu changes the coupling from the default $-h S_z$ to $-\ mu N$. It also changes the meaning of a few other parameters and quantities (see below). |
| H_MIN (MU_MIN) | | lowest magnetic field (chemical potential if --couple mu is specified) for which obervables are calculated |
| H_MAX (MU_MAX) | | highest magnetic field (chemical potential if --couple mu is specified) for which obervables are calculated |
| DELTA_H (DELTA_MU) | | magnetic field step width (chemical potential step width if --couple mu is specified) |
| versus | | versus h (versus mu if --couple mu is specified) puts the magnetic field (chemical potential) on the $x$-axis rather than temperature |
| MEASURE_MAGNETIC_PROPERTIES (MEASURE_CHARGE_PROPERTIES) | 1 | turns on (1) or off (0) the evaluation of magnetic (or charge) properties (see below). Recall that with the current version of `fulldiag`, such measurements are possible only for models with a conserved total $S_z$ or $N$. A corresponding CONSERVED_QUANTUMNUMBERS=... must also be specified in the parameters of `fulldiag`. |
| DENSITIES | 1 | specify whether to normalize quantities per site (1) or for the total system (0) |

All these parameters can be overwritten by the command line argument with the same name.

## Evaluation of thermodynamic properties

The `fulldiag_evaluate` program takes an XML output file of `fulldiag`, 

    fulldiag_evaluate [--T_MIN ...] [--T_MAX ...] [--DELTA_T ...]
        [--H_MIN ...] [--H_MAX ... ] [--DELTA_H ... ] [--versus h]
        [--DENSITIES ...] inputfile [outputfileprefix]</tt>

or 

    fulldiag_evaluate --couple mu [--T_MIN ...] [--T_MAX ...] [--DELTA_T ...]
        [--MU_MIN ...] [--MU_MAX ... ] [--DELTA_MU ...] [--versus mu]
        [--DENSITIES ...] inputfile [outputfileprefix]</tt>

Two optional ranges for temperature (T_MIN, T_MAX, DELTA_T) and magnetic field (H_MIN, H_MAX, DELTA_H) or chemical potential (MU_MIN, MU_MAX, DELTA_MU) can be specified. `fulldiag_evaluate` produces XML plot files (`outputfileprefix.plot.energy.xml` etc., where outputfileprefix is derived from the name of the inputfile if not specified) for the following quantities versus temperature:

- Energy [Density]
- Free Energy [Density]
- Entropy [Density]
- Specific Heat [Density]
- Magnetization [Density] (if MEASURE_MAGNETIC_PROPERTIES=1, and without couple mu)
- Uniform Susceptibility [Density] (if MEASURE_MAGNETIC_PROPERTIES=1, and without couple mu)
- Particle number [Density] (if MEASURE_CHARGE_PROPERTIES=1, and with couple mu)
- Compressibility [Density] (if MEASURE_CHARGE_PROPERTIES=1, and with couple mu)

Note that quantities are output as densities, i.e., normalized to the number of sites if the parameter DENSITIES=1, while output is for the total system if DENSITIES=0. By default, plots are produced with temperature on the $x$-axis. Use the argument --versus h (--versus mu) in order to obtain plots with magnetic field (chemical potential) on the $x$-axis

`fulldiag` stores information including eigenvalues and a result for the accessible physical quantities (measured for the total system). These are of interest mainly to specialists and, as we hope, self-explanatory if needed.

## Contributors

The following persons have contributed to the `fulldiag` application:

- Matthias Troyer
- Andreas Honecker 


