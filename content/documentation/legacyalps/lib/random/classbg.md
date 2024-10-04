
---
title: Class template buffered_generator
description: "ALPS Random Number Generator"
---

`alps::buffered_generator` — abstract base class of a runtime-polymorphic buffered_generator

## Synopsis

    // In header: <alps/random/buffered_generator.hpp>

    template<typename ResultType> 
    class buffered_generator {
    public:
        // types
        typedef ResultType                 result_type;
        typedef std::vector< result_type > buffer_type;  // the data type of the buffer used 

        // construct/copy/destruct
        buffered_generator(std::size_t = ALPS_BUFFERED_GENERATOR_BUFFER_SIZE);
        buffered_generator(const buffered_generator &);
        buffered_generator& operator=(const buffered_generator &);
        ~buffered_generator();

        // public member functions
        result_type operator()();
        void reset();

        // private member functions
        void fill_buffer(buffer_type &);
    };

## Description

This class template is an abstract base class for runtime-polymorphic generators. In order to mask the abstraction penalty of a virtual `operator()`, the `buffered_generator` does not produce single numbers at each call, but instead a large buffer is filled in a virtual function call, and then numbers from this buffer used when `operator()` is called.

### Template Parameters

1. `typename ResultType`

the type of values generated

### buffered_generator public construct/copy/destruct

1. `buffered_generator(std::size_t buffer_size = ALPS_BUFFERED_GENERATOR_BUFFER_SIZE);`

the constructor of the buffered generator
Constructs a `buffered_generator` with a buffer of the size given as argument.

Parameters: `buffer_size` the size of the buffer

2. `buffered_generator(const buffered_generator & gen);`

the copy constructor copies the buffer

3. `buffered_generator& operator=(const buffered_generator & gen);`

non-trivial the assignment

4. `~buffered_generator();`

trivial virtual destructor

### buffered_generator public member functions

1. `result_type operator()();`

returns the next generated value
values are taken from the buffer, which is refilled by a call to `fill_buffer` when all values have been used up

2. `void reset();`

discards all elements in the buffers and forces a new call to `fill_buffer` when the next value is requested

### buffered_generator private member functions

1. `void fill_buffer(buffer_type &);`

pure virtual function to fill the buffer
A pure virtual function to fill the buffer. It needs to be implemented by the concrete derived classes
