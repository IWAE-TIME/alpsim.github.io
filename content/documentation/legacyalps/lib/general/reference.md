
---
title: Reference
description: "ALPS General Library"
weight: 3
---

- [Header <alps/alea.h>](#header-alpsaleah)
- [Header <alps/cctype.h>](#header-alpscctypeh)
- [Header <alps/expression.h>](#header-alpsexpressionh)
- [Header <alps/factory.h>](#header-alpsfactoryh)
- [Header <alps/fixed_capacity_deque.h>](#header-alpsfixed_capacity_dequeh)
- [Header <alps/fixed_capacity_fwd.h>](#header-alpsfixed_capacityfwdh)
- [Header <alps/fixed_capacity_traits.h>](#header-alpsfixed_capacity_traitsh)
- [Header <alps/fixed_capacity_vector.h>](#header-alpsfixed_capacity_vectorh)
- [Header <alps/functional.h>](#header-alpsfunctionalh)
- [Header <alps/lambda.hpp>](#header-alpslambdahpp)
- [Header <alps/lattice.h>](#header-alpslatticeh)
- [Header <alps/model.h>](#header-alpsmodelh)
- [Header <alps/multi_array.hpp>](#header-alpsmulti_arrayhpp)
- [Header <alps/osiris.h>](#header-alpsosirish)
- [Header <alps/plot.h>](#header-alpsploth)
- [Header <alps/random.h>](#header-alpsrandomh)
- [Header <alps/stringvalue.h>](#header-alpsstringvalueh)
- [Header <alps/xml.h>](#header-alpsxmlh)


### Header <alps/alea.h>

includes all headers in the alps/alea directory

### Header <alps/cctype.h>

A safe version of the standard cctype header.

Some cctype headers do not undefine harmful macros, so undefine them here.

### Header <alps/expression.h>

includes all headers in the alps/expression directory

### Header <alps/factory.h>

object factories

This header contains an implementation of an object factory

    namespace alps {
    template<typename KEY, typename BASE> class factory;
    }

### Header <alps/fixed_capacity_deque.h>

    namespace alps {
        template<typename T, std::size_t N, typename CheckingPolicy> 
            class fixed_capacity_deque;
        template<typename T, std::size_t N> 
            bool operator==(const fixed_capacity_deque< T, N > & x, 
                    const fixed_capacity_deque< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator<(const fixed_capacity_deque< T, N > & x, 
                   const fixed_capacity_deque< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator!=(const fixed_capacity_deque< T, N > & x, 
                    const fixed_capacity_deque< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator>(const fixed_capacity_deque< T, N > & x, 
                   const fixed_capacity_deque< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator<=(const fixed_capacity_deque< T, N > & x, 
                    const fixed_capacity_deque< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator>=(const fixed_capacity_deque< T, N > & x, 
                    const fixed_capacity_deque< T, N > & y);
        template<typename T, std::size_t N> 
            void swap(fixed_capacity_deque< T, N > & x, 
              fixed_capacity_deque< T, N > & y);
        namespace fixed_capacity {
            template<typename T, std::size_t N, typename Ref, typename Ptr> 
                struct deque_iterator;
        }
    }

### Header <alps/fixed_capacity_fwd.h>

### Header <alps/fixed_capacity_traits.h>

    namespace std {
    }
    namespace alps {
        template<typename C> 
            struct fixed_capacity_traits;
        template<typename T, std::size_t N, typename C> 
            struct fixed_capacity_traits<fixed_capacity_vector< T, N, C >>;
        template<typename T, std::size_t N, typename C> 
            struct fixed_capacity_traits<fixed_capacity_deque< T, N, C >>;
        template<typename T, typename C> 
            struct fixed_capacity_traits<std::stack< T, C >>;
        template<typename T, typename C> 
            struct fixed_capacity_traits<std::queue< T, C >>;
        template<typename T, typename C, typename Cmp> 
            struct fixed_capacity_traits<std::priority_queue< T, C, Cmp >>;
    }

### Header <alps/fixed_capacity_vector.h>

    namespace alps {
        template<typename T, std::size_t N, typename CheckingPolicy> 
            class fixed_capacity_vector;
        template<typename T, std::size_t N> 
            bool operator==(const fixed_capacity_vector< T, N > & x, 
                    const fixed_capacity_vector< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator<(const fixed_capacity_vector< T, N > & x, 
                   const fixed_capacity_vector< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator!=(const fixed_capacity_vector< T, N > & x, 
                    const fixed_capacity_vector< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator>(const fixed_capacity_vector< T, N > & x, 
                   const fixed_capacity_vector< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator<=(const fixed_capacity_vector< T, N > & x, 
                    const fixed_capacity_vector< T, N > & y);
        template<typename T, std::size_t N> 
            bool operator>=(const fixed_capacity_vector< T, N > & x, 
                    const fixed_capacity_vector< T, N > & y);
        template<typename T, std::size_t N> 
            void swap(fixed_capacity_vector< T, N > & x, 
              fixed_capacity_vector< T, N > & y);
    }

### Header <alps/functional.h>

extensions to the standard functional header

This header contains mathematical function objects not present in the standard or boost libraries.

    namespace alps {
        template<typename T> struct conj_mult;

        template<typename T> struct conj_mult<std::complex< T >>;
    }
    
### Header <alps/lambda.hpp>

    namespace boost {
        namespace lambda {
            template<typename Act, typename T> 
                struct plain_return_type_2<arithmetic_action< Act >, std::valarray< T >, std::valarray< T >>;
            template<typename Act, typename T, typename U> 
                struct plain_return_type_2<arithmetic_action< Act >, std::valarray< T >, U>;
            template<typename Act, typename T, typename U> 
                struct plain_return_type_2<arithmetic_action< Act >, U, std::valarray< T >>;
        }
    }
    
### Header <alps/lattice.h>

includes all headers in the alps/lattice directory

### Header <alps/model.h>

includes all headers in the alps/model directory

### Header <alps/multi_array.hpp>

extensions to `boost::multi_array`

This header defines some I/O extensions to `boost::multi_array` and fixes a problem with gcc-3.1 when `alps::multi_array` and `alps::serialization` are used together


access
    namespace alps {

        // ALPS de-serialization support for boost::multi_array. 
        template<typename T, std::size_t NumDims, typename Allocator> 
            alps::IDump & 
            operator>>(alps::IDump & dump, 
               boost::multi_array< T, NumDims, Allocator > & x);

        // ALPS serialization support for boost::multi_array. 
        template<typename T, std::size_t NumDims, typename Allocator> 
            alps::ODump & 
            operator<<(alps::ODump & dump, 
               const boost::multi_array< T, NumDims, Allocator > & x);
    }

    // writes a two-dimensional boost::multi_array to an output stream 
    template<typename T, typename Allocator> 
        std::ostream & 
        operator<<(std::ostream & out, 
             const boost::multi_array< T, 2, Allocator > & x);

    // writes a four-dimensional boost::multi_array to an output stream 
    template<typename T, typename Allocator> 
        std::ostream & 
        operator<<(std::ostream & out, 
             const boost::multi_array< T, 4, Allocator > & x);

### Header <alps/osiris.h>

includes all headers in the alps/osiris directory

### Header <alps/plot.h>

classes to create plots in XML format

This header contains classes to create plots in XML format, compatible with the ALPS XML schema for plot files on the http://xml.comp-phys.org/ web page

    namespace alps {
        namespace plot {
            template<typename C> class Point;
            template<typename C> class Set;
            template<typename C> class Plot;

            enum SetType;

            // write a plot to an XML file following the ALPS XML schema for plots on http://xml.comp-phys.org/
            template<typename C> 
                oxstream & operator<<(oxstream & out, const Plot< C > & p);
            template<typename C> 
                oxstream & operator<<(oxstream & o, const Set< C > & S);
        }
    }
    
### Header <alps/random.h>

includes all headers in the alps/random directory

### Header <alps/stringvalue.h>

implements a string class that can easily be assigned to and converted to any type

    namespace alps {
        template<typename StringBase> class lexical_cast_string;

        typedef lexical_cast_string StringValue;  // StringValue is now implemented using lexical_cast_string. 
    }

### Header <alps/xml.h>

includes all headers in the alps/parser directory
