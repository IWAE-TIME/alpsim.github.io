
---
title: Class template basic_buffered_generator
description: "ALPS Random Number Generator"
---

`alps::basic_buffered_generator` — a concrete implementation of a buffered generator

## Synopsis
    // In header: <alps/random/buffered_generator.hpp>

    template<typename Generator, typename ResultType> 
    class basic_buffered_generator :
        public alps::buffered_generator< ResultType >
    {
    public:
        // types
        typedef Generator                                     generator_type;  // the date type of the generator used to fill the buffer 
        typedef buffered_generator< ResultType >::result_type result_type;     // the type of values generated 

        // construct/copy/destruct
        basic_buffered_generator(std::size_t = ALPS_BUFFERED_GENERATOR_BUFFER_SIZE);
        basic_buffered_generator(generator_type, 
                           std::size_t = ALPS_BUFFERED_GENERATOR_BUFFER_SIZE);

        // private member functions
        void fill_buffer(buffer_type &);
    };
    
## Description

This class template is a concrete derived class template for runtime-polymorphic generators. It uses the generator provided as template argument to fill the buffer of the buffered_generator base class. If the Generator is a reference type, a reference to the generator passed to the constructor is used. Otherwise a copy of the generator is used.

### Template Parameters

1. `typename Generator`
the type of the generator used to fill the buffer

2. `typename ResultType`
the type of values generated

### basic_buffered_generator public construct/copy/destruct

1. `basic_buffered_generator(std::size_t buffer_size = ALPS_BUFFERED_GENERATOR_BUFFER_SIZE);`

constructs a buffer of the size given as argument, and a default-generated Generator.

Parameters: `buffer_size` the size of the buffer

2. `basic_buffered_generator(generator_type gen, 
                         std::size_t buffer_size = ALPS_BUFFERED_GENERATOR_BUFFER_SIZE);`

constructs a buffered generator from the given argument If a reference type is specifed as Generator type, a reference to the generator gen is stored and used, otherweise the generator is copied.

Parameters:

 `buffer_size` the size of the buffer

 `gen` the generator used to generate values

### basic_buffered_generator private member functions

1. `void fill_buffer(buffer_type & buffer);`
fills the buffer using the generator
