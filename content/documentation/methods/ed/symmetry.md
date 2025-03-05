
---
title: Symmetry
math: true
weight: 2
---
The size of the Hilbert space of a Hamiltonian grows exponentially with the number of lattice sites, which limits the size of a quantum model that can be studied. It is, however, possible to reduce the full Hamiltonian matrix into several smaller matrices by block diagonalization with lattice and Hamiltonian symmetries. 

## Hilbert Space

The Hilbert space for a 4-site spin-$\frac{1}{2}$ system has dimension $2^4 = 16$. A basis for this space can be written as:

$$
\{ |s_1, s_2, s_3, s_4\rangle \}, \quad s_i \in \{\uparrow, \downarrow\}
$$

## Symmetries of the Hamiltonian

The Hamiltonian has several symmetries that can be used to block-diagonalize it, reducing the computational effort:

- **Total magnetization $\(S^z\_{\text{total}}\)$ conservation**:
   The total $S^z$ operator, $S^z\_{\text{total}} = \sum\_{i=1}^4 S_i^z$, commutes with $\mathcal{H}$. Thus, the Hamiltonian is block-diagonal in sectors of fixed $S^z\_{\text{total}}$.

- **Translational symmetry**:
   The Hamiltonian is invariant under translations $T$, where $T|s_1, s_2, s_3, s_4\rangle = |s_4, s_1, s_2, s_3\rangle$. This symmetry can be used to further block-diagonalize $\mathcal{H}$.

- **Spin inversion symmetry**:
   The Hamiltonian is invariant under spin inversion $P$, where $P|s_1, s_2, s_3, s_4\rangle = |-s_1, -s_2, -s_3, -s_4\rangle$. This symmetry can also be exploited.

- **Reflection symmetry**:
   The Hamiltonian is invariant under reflection $R$, where $R|s_1, s_2, s_3, s_4\rangle = |s_4, s_3, s_2, s_1\rangle$.

## Block-Diagonalization

We will use the total magnetization $S^z\_{\text{total}}$ and translational symmetry to reduce the Hilbert space.

### Step 1: Total Magnetization Sectors

The possible values of $S^z\_{\text{total}}$ are $-2, -1, 0, 1, 2$. We can divide the Hilbert space into these sectors:

- $S^z\_{\text{total}} = 2$: Only one state, $|\uparrow, \uparrow, \uparrow, \uparrow\rangle$.
- $S^z\_{\text{total}} = 1$: Four states, e.g., $|\downarrow, \uparrow, \uparrow, \uparrow\rangle$, $|\uparrow, \downarrow, \uparrow, \uparrow\rangle$, etc.
- $S^z\_{\text{total}} = 0$: Six states, e.g., $|\uparrow, \uparrow, \downarrow, \downarrow\rangle$, $|\uparrow, \downarrow, \uparrow, \downarrow\rangle$, etc.
- $S^z\_{\text{total}} = -1$: Four states, e.g., $|\downarrow, \downarrow, \downarrow, \uparrow\rangle$, $|\downarrow, \downarrow, \uparrow, \downarrow\rangle$, etc.
- $S^z\_{\text{total}} = -2$: Only one state, $|\downarrow, \downarrow, \downarrow, \downarrow\rangle$.

### Step 2: Translational Symmetry

Within each $S^z\_{\text{total}}$ sector, we can further block-diagonalize using translational symmetry. The translation operator $T$ has eigenvalues $e^{ik}$, where $k = 0, \pi/2, \pi, 3\pi/2$ (since $T^4 = 1$).

For example, in the $S^z\_{\text{total}} = 0$ sector, the states can be organized into momentum eigenstates:

$$
|\phi\rangle = \frac{1}{\sqrt{4}} \sum\_{n=0}^3 e^{ikn} T^n |\psi\rangle
$$

where $|\psi\rangle$ is a representative state in real space and $|\phi\rangle$ is a state in momentum space.

### Step 3: Constructing the Hamiltonian Blocks

For each $S^z\_{\text{total}}$ and momentum $k$, we construct the Hamiltonian matrix in the reduced basis. The matrix elements are:

$$
\langle \phi^{\prime} | \mathcal{H} | \phi \rangle = J \sum\_{i=1}^4 \langle \phi^{\prime} | \mathbf{S}\_i \cdot \mathbf{S}\_{i+1} | \phi \rangle
$$

### Step 4: Diagonalization

Finally, we diagonalize each block of the Hamiltonian to obtain the eigenvalues and eigenstates.

### Example: $S^z\_{\text{total}} = 0$ Sector

The $S^z\_{\text{total}} = 0$ sector consists of states with exactly 2 spins up ($\uparrow$) and 2 spins down ($\downarrow$). For a 4-site chain, there are $\binom{4}{2} = 6$ basis states in this sector:

$$
|\psi_1\rangle = |\uparrow, \uparrow, \downarrow, \downarrow\rangle, \quad |\psi_2\rangle = |\uparrow, \downarrow, \uparrow, \downarrow\rangle, \quad |\psi_3\rangle = |\uparrow, \downarrow, \downarrow, \uparrow\rangle, \\\
|\psi_4\rangle = |\downarrow, \uparrow, \uparrow, \downarrow\rangle, \quad |\psi_5\rangle = |\downarrow, \uparrow, \downarrow, \uparrow\rangle, \quad |\psi_6\rangle = |\downarrow, \downarrow, \uparrow, \uparrow\rangle
$$

#### Momentum Sectors
The momentum $k$ is given by $k = \frac{2\pi n}{4}$, where $n = 0, 1, 2, 3$. The translation operator $T$ acts on a state $|\psi_i\rangle$ as:

$$
T |\psi_i\rangle = e^{ik} |\psi_i\rangle.
$$

We construct translationally symmetric states for each momentum sector.

#### $S^z\_{\text{total}} = 0$ and $k = 0$ Sector
The momentum $k = 0$ sector consists of translationally symmetric states. For $S^z\_{\text{total}} = 0$, there is only one basis state:

$$
|\phi_1\rangle = \frac{1}{2} \left( |\psi_1\rangle + |\psi_2\rangle + |\psi_3\rangle + |\psi_4\rangle + |\psi_5\rangle + |\psi_6\rangle \right).
$$

The Hamiltonian matrix in this sector is:

$$
\mathcal{H} = \begin{pmatrix}
-J
\end{pmatrix}.
$$

#### $S^z\_{\text{total}} = 0$ and $k = 1$ Sector
The momentum $k = 1$ sector corresponds to $k = \frac{\pi}{2}$. For $S^z\_{\text{total}} = 0$, there is only one basis state:

$$
|\phi_1\rangle = \frac{1}{2} \left( |\psi_1\rangle + i|\psi_2\rangle - |\psi_3\rangle - i|\psi_4\rangle + |\psi_5\rangle + i|\psi_6\rangle \right).
$$

The Hamiltonian matrix in this sector is:

$$
\mathcal{H} = \begin{pmatrix}
-J
\end{pmatrix}.
$$

#### $S^z\_{\text{total}} = 0$ and $k = 2$ Sector
The momentum $k = 2$ sector corresponds to $k = \pi$. For $S_z = 0$, there are three basis states:

$$
|\phi_1\rangle = \frac{1}{\sqrt{2}} \left( |\psi_1\rangle - |\psi_6\rangle \right),
$$
$$
|\phi_2\rangle = \frac{1}{\sqrt{2}} \left( |\psi_2\rangle - |\psi_5\rangle \right),
$$
$$
|\phi_3\rangle = \frac{1}{\sqrt{2}} \left( |\psi_3\rangle - |\psi_4\rangle \right).
$$

The Hamiltonian matrix in this sector is:

$$
\mathcal{H} = J \begin{pmatrix}
-1 & 0 & 0 \\\
0 & -1 & 0 \\\
0 & 0 & -1 \\\
\end{pmatrix}.
$$

#### $S^z\_{\text{total}} = 0$ and $k = 3$ Sector
The momentum $k = 3$ sector corresponds to $k = \frac{3\pi}{2}$. For $S_z = 0$, there is only one basis state:

$$
|\phi_1\rangle = \frac{1}{2} \left( |\psi_1\rangle - i|\psi_2\rangle - |\psi_3\rangle + i|\psi_4\rangle + |\psi_5\rangle - i|\psi_6\rangle \right).
$$

The Hamiltonian matrix in this sector is:

$$
\mathcal{H} = \begin{pmatrix}
-J
\end{pmatrix}.
$$

#### Summary
- **$k = 0$**: 1 state, energy $-J$.
- **$k = 1$**: 1 state, energy $-J$.
- **$k = 2$**: 3 states, each with energy $-J$.
- **$k = 3$**: 1 state, energy $-J$.

The ground state energy in each sector is $-J$, and the $k = 2$ sector has three degenerate states.

---



### Final Result

After diagonalizing all blocks, we obtain the exact eigenvalues and eigenstates of the 4-site Heisenberg model with periodic boundary conditions. The use of symmetries significantly reduces the size of the matrices that need to be diagonalized.

This approach can be generalized to larger systems, although the computational cost still grows exponentially with system size.
