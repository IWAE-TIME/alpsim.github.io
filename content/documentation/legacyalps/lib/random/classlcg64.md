
---
title: Class template lcg64
description: "ALPS Random Number Generator"
---

`alps::random::parallel::lcg64` — a 64-bit linear congruential generator

## Synopsis

    // In header: <alps/random/parallel/lcg64.hpp>

    template<uint64_t a, uint64_t val> 
    class lcg64 {
    public:
        // types
        typedef uint64_t result_type;  // The result type is a 64-bit unsigned integer. 

        // construct/copy/destruct
        lcg64(...);

        // public member functions
        void seed(...);
        result_type min() const;
        result_type max() const;
        result_type operator()();

        // public static functions
        static bool validation(uint64_t);

        // public data members
        static const bool has_fixed_range;  // This generator has a fixed range. 
        static const result_type min_value;  // The minimum vaue is 0. 
        static const result_type max_value;  // The maximum value is the largest unsigned 64 bit integer. 
        static const result_type max_streams;  // The maximum number of streams is 146138719, the number of primes among all 64-bit unsigned integer values. 
    };

## Description

A 64-bit parallel linear congruential generator, following the implementation of the SPRNG library

### lcg64 public construct/copy/destruct

1. `lcg64(...);`
  the constructors
  All standard and named parameter constructors of random number generator and parallel random number generators are provided

### lcg64 public member functions

1. `void seed(...);`
  the seed fuctions
  All standard and named parameter seed functions of random number generator and parallel random number generators are provided

2. `result_type min() const;`

  Returns: the minimum value 0

3. `result_type max() const;`

  Returns: the maximum value, the largest unsigned 64-bit integer

4. `result_type operator()();`

Returns: the next random number

### lcg64 public static functions

1. `static bool validation(uint64_t x);`
  the validation function
  The validation function checks whether the passed value is the 10'000-th integer generated from a default-seeded generator
