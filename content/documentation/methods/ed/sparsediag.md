
---
title: Sparse Diagonalization
math: true
weight: 3
---

The Lanczos method is a powerful algorithm for finding a few extremal eigenvalues and their corresponding eigenvectors of large, sparse matrices. It is particularly useful for quantum lattices, where systems are often described by high-dimensional matrices that are too large to handle with dense matrix techniques. The Lanczos method exploits the sparsity of these matrices to efficiently compute the desired eigenvalues and eigenvectors.

The Hamiltonian matrix in quantum mechanics for systems with local interactions are **sparse**, meaning most of their entries are zero. Storing and manipulating dense matrices of size $N \times N$ requires $O(N^2)$ memory and $O(N^3)$ computational time for diagonalization. For large $N$, this becomes infeasible. The Lanczos method is designed to take advantage of this sparsity, requiring only matrix-vector products rather than explicit matrix storage or manipulation.

## The Lanczos Algorithm

The Lanczos method is an iterative algorithm that reduces a symmetric matrix $A$ of size $N \times N$ to a tridiagonal matrix $T$ of size $m \times m$, where $m \ll N$. The eigenvalues of $T$ approximate the extremal eigenvalues of $A$, and the corresponding eigenvectors can be reconstructed.

### Key Steps of the Lanczos Method

1. **Initialization**:
   - Choose a random starting vector $v_1$ with unit norm.
   - Set $\beta_0 = 0$ and $v_0 = 0$.

2. **Iteration**:
   For $j = 1, 2, \dots, m$:
   - Compute $w = A v_j - \beta\_{j-1} v\_{j-1}$.
   - Compute $\alpha_j = v_j^\top w$.
   - Compute $w = w - \alpha_j v_j$.
   - Compute $\beta_j = \|w\|$.
   - If $\beta_j = 0$, stop; otherwise, set $v\_{j+1} = w / \beta_j$.

3. **Tridiagonal Matrix**:
   After $m$ iterations, the matrix $T$ is constructed as:
   $$
   T = \begin{pmatrix}
   \alpha_1 & \beta_1 & 0 & \dots & 0 \\\
   \beta_1 & \alpha_2 & \beta_2 & \dots & 0 \\\
   0 & \beta_2 & \alpha_3 & \dots & 0 \\\
   \vdots & \vdots & \vdots & \ddots & \beta\_{m-1} \\\
   0 & 0 & 0 & \beta\_{m-1} & \alpha_m
   \end{pmatrix}
   $$

4. **Diagonalization of $T$**:
   - Diagonalize $T$ using standard dense matrix techniques (e.g., QR algorithm).
   - The eigenvalues of $T$ approximate the extremal eigenvalues of $A$.
   - The corresponding eigenvectors of $A$ can be reconstructed from the Lanczos vectors $v_j$.

### Advantages of the Lanczos Method

1. **Efficiency**:
   - Only matrix-vector products are required, making it suitable for sparse matrices.
   - Memory usage is $O(N \cdot m)$ instead of $O(N^2)$.

2. **Scalability**:
   - Works well for very large matrices where dense methods are infeasible.

3. **Focus on Extremal Eigenvalues**:
   - The Lanczos method is particularly effective at finding the largest or smallest eigenvalues and their eigenvectors.

### Challenges and Considerations

1. **Loss of Orthogonality**:
   - In finite-precision arithmetic, the Lanczos vectors $v_j$ can lose orthogonality, leading to spurious eigenvalues.
   - Remedies include reorthogonalization or using more advanced variants like the **Implicitly Restarted Lanczos Method**.

2. **Choice of $m$**:
   - The number of iterations $m$ must be chosen carefully to balance accuracy and computational cost.

3. **Convergence**:
   - Convergence to the extremal eigenvalues is typically fast, but interior eigenvalues may require many iterations.

## Sparse Diagonalization in ALPS

The `sparsediag` is an exact diagonalization program in ALPS, using the Lanczos algorithm of the IETL library to compute low-lying eigestates of the Hamiltonian. Hence, it can be used for computing ground-state properties of any model that can be defined using the ALPS libraries. The main limitation is the size of the quantum system, i.e., memory and CPU time may become unacceptable at sizes where other, more specialized applications still work well.

## Input Parameters in ALPS

The `sparsediag` code takes the following parameters:

| **Parameter** | **Default** | **Meaning** |
| :------------ | :---------- | :---------- |
| NUMBER_EIGENVALUES | 1 | the number of low-lying eigenstates to be calculated |


