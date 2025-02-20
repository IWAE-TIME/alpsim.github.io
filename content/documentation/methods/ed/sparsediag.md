
---
title: Sparse Diagonalization (Lanczos) 
math: true
weight: 3
---

## Introduction

The `sparsediag` is an exact diagonalization program in ALPS, using the Lanczos algorithm of the IETL library to compute low-lying eigestates of the Hamiltonian. Hence, it can be used for computing ground-state properties of any model that can be defined using the ALPS libraries. The main limitation is one of size, i.e., memory and CPU time may become unacceptable at sizes where other, more specialized applications still work well.

## Running a computation

is discussed in the sparsediag tutorial

## Input parameters

In addition to the input parameters are explained here the sparsediag code takes the following parameter:

| **Parameter** | **Default** | **Meaning** |
| :------------ | :---------- | :---------- |
| NUMBER_EIGENVALUES | 1 | the number of low-lying eigenstates to be calculated |


