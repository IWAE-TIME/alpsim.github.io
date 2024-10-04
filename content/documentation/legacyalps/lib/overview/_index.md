
---
title: Chapter 1. Overview
description: "ALPS Libraries Overview"
---

The ALPS libraries are part of the ALPS project (Parallel Algorithms for Lattice Models), which aims at providing generic parallel algorithms for classical and quantum lattice models and provides utility classes and algorithm for many other problems. It strives to increase software reuse in the physics community.

## Libraries

The following libraries are publicly available as part of the ALPS library project:

- [alps/general]()(\*): generally usefull classes and traits
- [alps/random]()(\*): extensions to the Boost and C++ random number libraries.
- [alps/osiris]()(\*): serialization and communication
- [alps/parser]()(\*): helper functions to parse and write XML files
- [alps/alea](): Monte Carlo measurements and evaluation
- [alps/graph](): Extensions to the Boost Graph library
- [alps/lattice](): lattices and graphs
- [alps/model](): quantum lattice models
- [alps/scheduler](): an automatically parallelizing scheduler for Monte Carlo simulations
- [alps/graph](): graph algorithms extending the Boost graph library
- [alps/hdf5](): a library to read an write HDF5 files from C++

Besides the helper tools for the scheduler library we have provided a few sample tools for the manipulation of the XML files created by the ALPS programs.
