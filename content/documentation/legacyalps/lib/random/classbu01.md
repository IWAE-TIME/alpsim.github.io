
---
title: Class template buffered_uniform_01
description: "ALPS Random Number Generator"
---

`alps::buffered_uniform_01` — the abstract base class of a runtime-polymorphic buffered random number generator generating double values in the interval \[0,1\]

## Synopsis
    // In header: <alps/random/buffered_uniform_01.hpp>

    template<typename RealType = double> 
    class buffered_uniform_01 : public alps::buffered_generator< RealType > {
    public:
        // types
        typedef RealType result_type;  // the type of random numbers 

        // construct/copy/destruct
        buffered_uniform_01(std::size_t = ALPS_BUFFERED_GENERATOR_BUFFER_SIZE);

        // public member functions
        result_type min() const;
        result_type max() const;
    };
    
## Description

This class template is an abstract base class template for runtime-polymorphic uniform random number generators producing numbers in the interval [0,1). It inherits from [`alps::buffered_generator`](../../random/classbg) and provides min() and () functions returning 0. and 1. respectively,

### Template Parameters

1. `typename RealType = double`

the floating point type of the random numbers, defaults to double

### buffered_uniform_01 public construct/copy/destruct

1. `buffered_uniform_01(std::size_t buffer_size = ALPS_BUFFERED_GENERATOR_BUFFER_SIZE);`

constructs the generator

Parameters: `buffer_size` the size of the buffer

### buffered_uniform_01 public member functions

1. `result_type min() const;`

Returns: 0.

2. `result_type max() const;`

Returns: 1.

