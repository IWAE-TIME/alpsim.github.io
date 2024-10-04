
---
title: Class template multivariate_normal_distribution
description: "ALPS Random Number Generator"
---

`alps::multivariate_normal_distribution` — a distribution creating correlated multi-variate normally distributed numbers

## Synopsis

// In header: <alps/random/multivariate_normal_distribution.hpp>

    template<typename RealType = double> 
    class multivariate_normal_distribution {
    public:
        // types
        typedef RealType                                  result_type;  // the type of random numbers produced 
        typedef RealType                                  input_type;   // the input type 
        typedef boost::numeric::ublas::vector< RealType > vector_type;  // the type of the vector of mean values 
        typedef boost::numeric::ublas::matrix< RealType > matrix_type;  // the type of the matrix storing the Cholesky decomposition of the covariance matrix 

        // construct/copy/destruct
        multivariate_normal_distribution(const matrix_type &, const vector_type &);
        explicit multivariate_normal_distribution(const matrix_type &);

        // public member functions
        vector_type const & mean() const;
        matrix_type const & cholesky() const;
        void reset();
        template<typename Engine> result_type operator()(Engine &);
    };
    
    
## Description

the multivariate normal distribution creates correlated random numbers with a specified mean vector and covariance matrix. Instead of using a vector as the result_type, the result_type is a scalar real number, and the operator() should be called once for each element of the vector.


### multivariate_normal_distribution public construct/copy/destruct

1. `multivariate_normal_distribution(const matrix_type & cholesky, 
                                 const vector_type & mean);`

the constructor of the multi-variate normal distribution
The Cholesky decomposition has to be a square matrix and its dimension has to be the same as that of the mean vector. Instead of a Cholesky decomposition any other square root of the covariance matrix could be passed.

Requires: `mean.size() == cholesky.size1()` and `cholesky.size1() == cholesky.size2()`

Parameters:

`cholesky` the Cholesky decomposition of the covariance matrix

`mean` the vector of mean values

2. `explicit multivariate_normal_distribution(const matrix_type & cholesky);`

the constructor of the multi-variate normal distribution with zero mean
Instead of a Cholesky decomposition any other square root of the covariance matrix could be passed.

Requires: `cholesky.size1() == cholesky.size2()`

Parameters:

`cholesky` the Cholesky decomposition of the covariance matrix

### multivariate_normal_distribution public member functions

1. `vector_type const & mean() const;`

Returns: the vector of mean values

2. `matrix_type const & cholesky() const;`

Returns: the Cholesky decomposition of the covariance marix

3. `void reset();`

purges the cache.

Purges the cache. The next call to `oeprator()` will create a new vector.

4. `template<typename Engine> result_type operator()(Engine & eng);`

Returns:

On the first call, it creates a vector of n multivariate normally distributed random numbers, caches it, and returns the first value. The next n-1 calls return the next elements of the vector. The n+1-st call again creates a new vector of multivariate normally distributed random numbers.

