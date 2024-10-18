
---
title: Chapter 1. Overview
description: "ALPS Libraries Overview"
weight: 1
---

The ALPS libraries are part of the ALPS project (Parallel Algorithms for Lattice Models), which aims at providing generic parallel algorithms for classical and quantum lattice models and provides utility classes and algorithm for many other problems. It strives to increase software reuse in the physics community.

## Libraries

The following libraries are publicly available as part of the ALPS library project:

- [alps/general](../general): generally usefull classes and traits
- [alps/random](../random): extensions to the Boost and C++ random number libraries.
- [alps/osiris](../osiris): serialization and communication
- [alps/parser](../parser): helper functions to parse and write XML files
- [alps/alea](../alea): Monte Carlo measurements and evaluation
- [alps/graph](): Extensions to the Boost Graph library
- [alps/lattice](../lattice): lattices and graphs
- [alps/model](../model): quantum lattice models
- [alps/scheduler](../scheduler): an automatically parallelizing scheduler for Monte Carlo simulations
- [alps/hdf5](): a library to read an write HDF5 files from C++

Besides the helper tools for the scheduler library we have provided a few sample tools for the manipulation of the XML files created by the ALPS programs.
