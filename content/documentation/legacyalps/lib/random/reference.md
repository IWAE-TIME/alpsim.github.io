
---
title: Reference
description: "ALPS Random Library"
---

- [Header <alps/random/buffered_generator.hpp>](#header-alpsrandombuffered_generatorhpp)
- [Header <alps/random/buffered_rng.h>](#header-alpsrandombuffered_rngh)
- [Header <alps/random/buffered_uniform_01.hpp>](#header-alpsrandombuffered_uniform_01hpp)
- [Header <alps/random/parallel/mersenne_twister.hpp>](#header-alpsrandomparallelmersenne_twisterhpp)
- [Header <alps/random/multivariate_normal_distribution.hpp>](#header-alpsrandommultivariate_normal_distributionhpp)
- [Header <alps/random/parallel/detail/get_prime.hpp>](#header-alpsrandomparalleldetailget_primehpp)
- [Header <alps/random/parallel/detail/primelist_64.hpp>](#header-alpsrandomparalleldetailprimelist_64hpp)
- [Header <alps/random/parallel/primelist_64.hpp>](#header-alpsrandomparallelprimelist_64hpp)
- [Header <alps/random/parallel/detail/seed_macros.hpp>](#header-alpsrandomparalleldetailseed_macroshpp)
- [Header <alps/random/parallel/keyword.hpp>](#header-alpsrandomparallelkeywordhpp)
- [Header <alps/random/sprng/keyword.hpp>](#header-alpsrandomsprngkeywordhpp)
- [Header <alps/random/parallel/lcg64.hpp>](#header-alpsrandomparallellcg64hpp)
- [Header <alps/random/sprng/lcg64.hpp>](#header-alpsrandomsprnglcg64hpp)
- [Header <alps/random/parallel/mpi.hpp>](#header-alpsrandomparallelmpihpp)
- [Header <alps/random/parallel/seed.hpp>](#header-alpsrandomparallelseedhpp)
- [Header <alps/random/parallel/well.hpp>](#header-alpsrandomparallelwellhpp)
- [Header <alps/random/pseudo_des.h>](#header-alpsrandompseudo_desh)
- [Header <alps/random/rngfactory.h>](#header-alpsrandomrngfactoryh)
- [Header <alps/random/seed.h>](#header-alpsrandomseedh)
- [Header <alps/random/sprng/cmrg.hpp>](#header-alpsrandomsprngcmrghpp)
- [Header <alps/random/sprng/detail/buffer.hpp>](#header-alpsrandomsprngdetailbufferhpp)
- [Header <alps/random/sprng/lcg.hpp>](#header-alpsrandomsprnglcghpp)
- [Header <alps/random/sprng/lfg.hpp>](#header-alpsrandomsprnglfghpp)
- [Header <alps/random/sprng/mlfg.hpp>](#header-alpsrandomsprngmlfghpp)
- [Header <alps/random/sprng/pmlcg.hpp>](#header-alpsrandomsprngpmlcghpp)
- [Header <alps/random/uniform_on_sphere_n.h>](#header-alpsrandomuniform_on_sphere_nh)

### Header <alps/random/buffered_generator.hpp>

ALPS_BUFFERED_GENERATOR_BUFFER_SIZE

    namespace alps {
        template<typename ResultType> class buffered_generator;
        template<typename Generator, typename ResultType> 
            class basic_buffered_generator;
    }

### Header <alps/random/buffered_rng.h>

contains an efficient buffered implementation of a runtime-polymorphic random number generator

    namespace alps {
        class buffered_rng_base;
        template<typename RNG> class buffered_rng;
        std::ostream & operator<<(std::ostream &, const buffered_rng_base &);
        std::istream & operator>>(std::istream &, buffered_rng_base &);
    }
    
### Header <alps/random/buffered_uniform_01.hpp>

    namespace alps {
        template<typename RealType = double> class buffered_uniform_01;
        template<typename Engine, typename RealType = double> 
            class basic_buffered_uniform_01;
    }

### Header <alps/random/parallel/mersenne_twister.hpp>

    namespace alps {
        namespace random {
            namespace parallel {
                template<typename UIntType, int w, int n, int m, int r, UIntType a, 
                    int u, int s, UIntType b, int t, UIntType c, int l, 
                    UIntType val> 
                    void seed(boost::random::mersenne_twister< UIntType, w, n, m, r, a, u, s, b, t, c, l, val > & prng, 
                        unsigned int num, unsigned int total);
                template<typename UIntType, int w, int n, int m, int r, UIntType a, 
                    int u, int s, UIntType b, int t, UIntType c, int l, 
                    UIntType val, typename SeedType> 
                    void seed(boost::random::mersenne_twister< UIntType, w, n, m, r, a, u, s, b, t, c, l, val > & prng, 
                        unsigned int num, unsigned int total, 
                        SeedType const & the_seed);
                template<typename UIntType, int w, int n, int m, int r, UIntType a, 
                    int u, int s, UIntType b, int t, UIntType c, int l, 
                    UIntType val> 
                    void seed(boost::random::mersenne_twister< UIntType, w, n, m, r, a, u, s, b, t, c, l, val > & prng, 
                        unsigned int num, unsigned int total, lcg64a & engine);
                template<typename UIntType, int w, int n, int m, int r, UIntType a, 
                    int u, int s, UIntType b, int t, UIntType c, int l, 
                    UIntType val, typename Iterator> 
                    void seed(boost::random::mersenne_twister< UIntType, w, n, m, r, a, u, s, b, t, c, l, val > & prng, 
                        unsigned int num, unsigned int total, Iterator & first, 
                        Iterator const & last);
            }
        }
    }
    
### Header <alps/random/multivariate_normal_distribution.hpp>

    namespace alps {
        template<typename RealType = double> class multivariate_normal_distribution;
    }
    
### Header <alps/random/parallel/detail/get_prime.hpp>

### Header <alps/random/parallel/detail/primelist_64.hpp>

### Header <alps/random/parallel/primelist_64.hpp>

PRIMELISTSIZE1
STEP
PRIMELISTSIZE2

### Header <alps/random/parallel/detail/seed_macros.hpp>

    ALPS_RANDOM_PARALLEL_CONSTRUCTOR(z, n, P)
    ALPS_RANDOM_PARALLEL_ITERATOR_SEED_DEFAULT_IMPL(z, n, unused)
    ALPS_RANDOM_PARALLEL_ITERATOR_SEED_IMPL(z, n, unused)
    ALPS_RANDOM_PARALLEL_SEED_PARAMS(RNG, PARAMS, INIT)
    ALPS_RANDOM_PARALLEL_SEED(RNG)
    ALPS_RANDOM_PARALLEL_ITERATOR_SEED_PARAMS(PARAMS)
    ALPS_RANDOM_PARALLEL_ITERATOR_SEED()
    ALPS_RANDOM_PARALLEL_ITERATOR_SEED_DEFAULT()

### Header <alps/random/parallel/keyword.hpp>

    ALPS_RANDOM_MAXARITY

### Header <alps/random/sprng/keyword.hpp>

### Header <alps/random/parallel/lcg64.hpp>

contains a parallel 64-bit generator template and three good choices of parameters.

    namespace alps {
        typedef random::parallel::lcg64< uint64_t(0x87b0b0fdU)|uint64_t(0x27bb2ee6U)<< 32, uint64_t(481823773Ul)+(uint64_t(3380683238Ul)<< 32)> lcg64a;  // Instantiation of lcg64 with a good choice of multiplier. 
        typedef random::parallel::lcg64< uint64_t(0xe78b6955U)|uint64_t(0x2c6fe96eU)<< 32, uint64_t(3274024413Ul)+(uint64_t(3475904802Ul)<< 32)> lcg64b;  // Instantiation of lcg64 with a good choice of multiplier. 
        typedef random::parallel::lcg64< uint64_t(0x31a53f85U)|uint64_t(0x369dea0fU)<< 32, uint64_t(950651229Ul)+(uint64_t(3996309981Ul)<< 32)> lcg64c;  // Instantiation of lcg64 with a good choice of multiplier. 
        namespace random {
            namespace parallel {
                template<uint64_t a, uint64_t val> class lcg64;
            }
        }
    }
    
### Header <alps/random/sprng/lcg64.hpp>

### Header <alps/random/parallel/mpi.hpp>

    namespace alps {
        namespace random {
            namespace parallel {
                template<typename PRNG> 
                    void seed(PRNG &, boost::mpi::communicator const &);
                template<typename PRNG, typename SeedType> 
                    void seed(PRNG &, boost::mpi::communicator const &, SeedType const &);
                template<typename PRNG, typename Iterator> 
                    void seed(PRNG &, boost::mpi::communicator const &, Iterator &, 
                  Iterator const &);
                template<typename PRNG, typename SeedType> 
                    void broadcast_seed(PRNG &, boost::mpi::communicator const &, int, 
                            SeedType);
            }
        }
    }
    
### Header <alps/random/parallel/seed.hpp>

This header provides default implementations of the parallel seeding functions.

    namespace alps {
        namespace random {
            namespace parallel {
                template<typename PRNG> void seed(PRNG &, unsigned int, unsigned int);
                template<typename PRNG, typename SeedType> 
                    void seed(PRNG &, unsigned int, unsigned int, SeedType const &);
                template<typename PRNG, typename Iterator> 
                    void seed(PRNG &, unsigned int, unsigned int, Iterator &, 
                  Iterator const &);
            }
        }
    }
    
### Header <alps/random/parallel/well.hpp>

    namespace alps {
        namespace random {
            namespace parallel {
                template<typename UIntType, int statesize, UIntType val, typename F1, 
                    typename F2, typename F3, typename F4, typename F5, 
                    typename F6, typename F7, typename F8, int p1, int p2, int p3, 
                    UIntType mask = statesize-1, typename RNG = alps::lcg64a> 
                class well;

                typedef well< uint32_t, 16, 1584514050u, mat0neg<-16 >, mat0neg<-15 >, mat0pos< 11 >, zero, mat0neg<-2 >, mat0neg<-18 >, mat3neg<-28 >, mat4neg<-5 >, 13, 9, 1 > well512a;  // A 512-bit version of the WELL generator. 
                typedef well< uint32_t, 32, 2159746073u, identity, mat0pos< 8 >, mat0neg<-19 >, mat0neg<-14 >, mat0neg<-11 >, mat0neg<-7 >, mat0neg<-13 >, zero, 3, 24, 10 > well1024a;  // A 1024-bit version of the WELL generator. 
            }
        }
    }
    
    
### Header <alps/random/pseudo_des.h>

a random number generator using the pseudo-DES algorithm

    namespace alps {
        class pseudo_des;
    }
    
### Header <alps/random/rngfactory.h>

a factory to create random number generators from their name

    namespace alps {
        class RNGFactory;

        RNGFactory rng_factory;  // a factory to create random number generators from their name 
    }
    
### Header <alps/random/seed.h>

a generic seeding function for random number generators

    namespace alps {
        template<typename RNG> void seed_with_sequence(RNG &, uint32_t);
        template<typename RNG, typename INIGEN> 
            void seed_with_generator(RNG & rng, INIGEN & inigen);
    }
    
### Header <alps/random/sprng/cmrg.hpp>

### Header <alps/random/sprng/detail/buffer.hpp>

### Header <alps/random/sprng/lcg.hpp>

### Header <alps/random/sprng/lfg.hpp>

### Header <alps/random/sprng/mlfg.hpp>

### Header <alps/random/sprng/pmlcg.hpp>

### Header <alps/random/uniform_on_sphere_n.h>

    namespace alps {
        template<int N, typename RealType, typename Cont> class uniform_on_sphere_n;

        template<typename RealType, typename Cont> 
            class uniform_on_sphere_n<1, RealType, Cont>;
        template<typename RealType, typename Cont> 
            class uniform_on_sphere_n<2, RealType, Cont>;
        template<typename RealType, typename Cont> 
            class uniform_on_sphere_n<3, RealType, Cont>;
    }
