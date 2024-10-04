
---
title: Class template well
description: "ALPS Random Number Generator"
---
`alps::random::parallel::well` — the WELL generator class template

## Synopsis

    // In header: <alps/random/parallel/well.hpp>

    template<typename UIntType, int statesize, UIntType val, typename F1, 
         typename F2, typename F3, typename F4, typename F5, typename F6, 
         typename F7, typename F8, int p1, int p2, int p3, 
         UIntType mask = statesize-1, typename RNG = alps::lcg64a> 
    class well {
    public:
        // types
        typedef UIntType result_type;

        // construct/copy/destruct
        well(...);

        // public member functions
        void seed(...);
        result_type min() const;
        result_type max() const;
        result_type operator()();

        // public static functions
        static bool validation(result_type);
    };

## Description
This class template implements the WELL generator of F. Panneton, P. L'Ecuyer and M. Matsumoto

### `well' public construct/copy/destruct

1. `well(...);`
  the constructors
  All standard and named parameter constructors of random number generator and parallel random number generators are provided

2. `well' public member functions

1. `void seed(...);`
  the seed fuctions
  All standard and named parameter seed functions of random number generator and parallel random number generators are provided

2. `result_type min() const;`

  Returns: the minimum value 0

3. `result_type max() const;`

  Returns: the maximum value, the largest unsigned 32-bit integer

4. `result_type operator()();`

  Returns: the next random number

### `well` public static functions

1. `static bool validation(result_type value);`
  the validation function
  The validation function checks whether the passed value is the 10'000-th integer generated from a default-seeded generator. The 10'000-th integer is determined with the original RNG of F. Panneton, P. L'Ecuyer and M. Matsumoto, see <http://www.iro.umontreal.ca/~panneton/WELLRNG.html>


