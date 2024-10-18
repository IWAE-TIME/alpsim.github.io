
---
title: Reference
description: "Reference for IETL Library"
weight: 2
---

# Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`namespace `[`ietl`](#d5/d9f/namespaceietl) | 
`namespace `[`ietl2lapack`](#dc/d50/namespaceietl2lapack) | 
`namespace `[`ietl::detail`](#de/db3/namespaceietl_1_1detail) | 
`namespace `[`ietl::solver`](#df/dd6/namespaceietl_1_1solver) | 
`namespace `[`ietl_lapack_dispatch`](#d3/d3e/namespaceietl__lapack__dispatch) | 

# namespace `ietl` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`enum `[`DesiredEigenvalue`](#d4/dfd/jacobi_8h_1a5e3508b9d7357572edd2fa59a61eadf6)            | 
`public template<>`  <br/>`T `[`real`](#d7/d3b/complex_8h_1ac0f1d378f644863e95702fcb7846c92d)`(T x)`            | 
`public template<>`  <br/>`T `[`real`](#d7/d3b/complex_8h_1a991ef7b85878fb4946d4b8f55eb85310)`(std::complex< T > x)`            | 
`public template<>`  <br/>`T `[`conj`](#d7/d3b/complex_8h_1a576f505cbb140b6aa72ec2126f2e0a7b)`(T x)`            | 
`public template<>`  <br/>`T `[`conj`](#d7/d3b/complex_8h_1a8020f454bca2499f9a560ac8ae018cab)`(std::complex< T > x)`            | 
`public template<>`  <br/>`T * `[`get_data`](#de/de9/ietl2lapack_8h_1a5c53bf26355edab0de7372ff9701bcc3)`(const std::vector< T > & v)`            | 
`public template<>`  <br/>`std::pair< typename `[`vectorspace_traits](#d4/d26/structietl_1_1vectorspace__traits)< VS >::magnitude_type, typename [vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type > `[`inverse`](#d0/db6/inverse_8h_1a758d8e36a08be916da068e2fba2164d2)`(const MATRIX & matrix,GEN & gen,const SOLVER & solver,ITER & iter,typename `[`vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::magnitude_type sigma,const VS & vec)`            | 
`public template<>`  <br/>`void `[`mult`](#d4/dfd/jacobi_8h_1a8c957647fac0f90519d0aebb2fd92d67)`(`[`jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator)`< Matrix, VS, Vector > const & m,typename `[`jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator)`< Matrix, VS, Vector >::vector_type const & x,typename `[`jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator)`< Matrix, VS, Vector >::vector_type & y)`            | 
`public template<>`  <br/>`std::pair< typename `[`vectorspace_traits](#d4/d26/structietl_1_1vectorspace__traits)< VS >::scalar_type, typename [vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type > `[`power`](#d3/d6a/power_8h_1aef26b6c6112cbc7fed1cca17a7923cf3)`(const MATRIX & m,GEN & start,IT & iter,const VS & vec)`            | 
`public template<>`  <br/>`std::pair< typename `[`ietl::number_traits](#db/d49/structietl_1_1number__traits)< typename [vectorspace_traits](#d4/d26/structietl_1_1vectorspace__traits)< VS >::scalar_type >::magnitude_type, typename [vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type > `[`rayleigh`](#d5/d7f/rayleigh_8h_1a04790e00af423fe2e3035c2bfb2438a1)`(const MATRIX & matrix,GEN & gen,SOLVER & solver,ITER & iter,const VS & vec)`            | 
`public template<>`  <br/>`void `[`project`](#d4/d60/vectorspace_8h_1a5cc4a334a92197692d8b5226b39907f6)`(typename `[`ietl::vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type & v,const VS & vs)`            | 
`public template<>`  <br/>[`ietl::vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type `[`new_vector`](#d4/d60/vectorspace_8h_1a9bf3f18605813d405be38701e1294918)`(const VS & vs)`            | 
`public template<>`  <br/>[`ietl::vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::size_type `[`vec_dimension`](#d4/d60/vectorspace_8h_1a18a05f2374565ba55c4bb32a063a0ec5)`(const VS & vs)`            | 
`public template<>`  <br/>`void `[`copy`](#d4/d60/vectorspace_8h_1aa32a4a3e0c568e74f7eb8070f0c7d676)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src,`[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & dst)`            | 
`public template<>`  <br/>[`number_traits`](#db/d49/structietl_1_1number__traits)`< typenameV::value_type >::magnitude_type `[`two_norm`](#d4/d60/vectorspace_8h_1a427e5b22ec64cf863698a432d55083a6)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src)`            | 
`public template<>`  <br/>`V::value_type `[`dot`](#d4/d60/vectorspace_8h_1a2265aff862612289e22e88c6faa62a74)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src1,const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src2)`            | 
`public template<>`  <br/>`void `[`mult`](#d4/d60/vectorspace_8h_1a8a8daeacc2aef9b5ec75ae0ffd2e7938)`(A a,const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src,`[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & dst)`            | 
`public template<>`  <br/>`void `[`generate`](#d4/d60/vectorspace_8h_1a473405870a25e2aca90eb6caf47d7ea7)`(`[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src,const GEN & gen)`            | 
`public template<>`  <br/>[`ietl::scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > `[`operator*`](#d4/d60/vectorspace_8h_1a4576633d2d4d497cab6bff2df3386e5c)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & v,S s)`            | 
`public template<>`  <br/>[`ietl::scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > `[`operator*`](#d4/d60/vectorspace_8h_1a7e34e26db0232f5075e7562eedec0f99)`(S s,const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & v)`            | 
`public template<>`  <br/>[`ietl::scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > `[`operator/`](#d4/d60/vectorspace_8h_1a9fcd114f63378b89a0db11b065a32777)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & v,S s)`            | 
`class `[`ietl::arnoldi_iteration`](#d7/d38/classietl_1_1arnoldi__iteration) | 
`class `[`ietl::bandlanczos`](#dd/dde/classietl_1_1bandlanczos) | 
`class `[`ietl::bandlanczos_iteration_nhighest`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest) | 
`class `[`ietl::bandlanczos_iteration_nlowest`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest) | 
`class `[`ietl::basic_iteration`](#d0/d85/classietl_1_1basic__iteration) | 
`class `[`ietl::basic_lanczos_iteration`](#d8/d08/classietl_1_1basic__lanczos__iteration) | 
`class `[`ietl::bicg_wrapper`](#d9/d8c/classietl_1_1bicg__wrapper) | 
`class `[`ietl::bicgstab_wrapper`](#d2/d5c/classietl_1_1bicgstab__wrapper) | 
`class `[`ietl::cg_wrapper`](#d4/d45/classietl_1_1cg__wrapper) | 
`class `[`ietl::cgs_wrapper`](#d6/dc2/classietl_1_1cgs__wrapper) | 
`class `[`ietl::cheby_wrapper`](#d6/d49/classietl_1_1cheby__wrapper) | 
`class `[`ietl::fixed_lanczos_iteration`](#de/dc1/classietl_1_1fixed__lanczos__iteration) | 
`class `[`ietl::FortranMatrix`](#d7/d65/classietl_1_1_fortran_matrix) | 
`class `[`ietl::gcr_wrapper`](#d8/d99/classietl_1_1gcr__wrapper) | 
`class `[`ietl::ietl_bicgstabl`](#df/d3c/classietl_1_1ietl__bicgstabl) | 
`class `[`ietl::ietl_cg`](#d2/d83/classietl_1_1ietl__cg) | 
`class `[`ietl::ietl_gmres`](#d1/d82/classietl_1_1ietl__gmres) | 
`class `[`ietl::indexer`](#d0/d6a/classietl_1_1indexer) | 
`class `[`ietl::Info`](#d9/db8/classietl_1_1_info) | 
`class `[`ietl::jacobi_davidson`](#d0/df4/classietl_1_1jacobi__davidson) | 
`class `[`ietl::jcd_gmres_solver`](#d4/de2/classietl_1_1jcd__gmres__solver) | 
`class `[`ietl::jcd_left_preconditioner`](#d2/d34/classietl_1_1jcd__left__preconditioner) | 
`class `[`ietl::jcd_simple_solver`](#de/d6e/classietl_1_1jcd__simple__solver) | 
`class `[`ietl::jcd_solver`](#dd/d41/classietl_1_1jcd__solver) | 
`class `[`ietl::jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator) | 
`class `[`ietl::jd`](#dc/de7/classietl_1_1jd) | 
`class `[`ietl::jd_iteration`](#d3/d34/classietl_1_1jd__iteration) | 
`class `[`ietl::lanczos`](#d1/d82/classietl_1_1lanczos) | 
`class `[`ietl::lanczos_iteration_nhighest`](#d4/d22/classietl_1_1lanczos__iteration__nhighest) | 
`class `[`ietl::lanczos_iteration_nlowest`](#d9/d8a/classietl_1_1lanczos__iteration__nlowest) | 
`class `[`ietl::lanczos_nlowest_better`](#de/d68/classietl_1_1lanczos__nlowest__better) | 
`class `[`ietl::qmr_wrapper`](#d1/d5e/classietl_1_1qmr__wrapper) | 
`class `[`ietl::richardson_wrapper`](#d6/d46/classietl_1_1richardson__wrapper) | 
`class `[`ietl::scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper) | 
`class `[`ietl::simple_arnoldi`](#d0/df4/classietl_1_1simple__arnoldi) | 
`class `[`ietl::tfqmr_wrapper`](#d9/d9d/classietl_1_1tfqmr__wrapper) | 
`class `[`ietl::Tmatrix`](#db/da5/classietl_1_1_tmatrix) | 
`class `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper) | 
`class `[`ietl::vectorspace`](#d7/d6c/classietl_1_1vectorspace) | 
`class `[`ietl::wrapper_vectorspace`](#d9/de5/classietl_1_1wrapper__vectorspace) | 
`struct `[`ietl::number_traits`](#db/d49/structietl_1_1number__traits) | 
`struct `[`ietl::number_traits< std::complex< T > >`](#df/dd2/structietl_1_1number__traits_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`ietl::real_type`](#d0/d22/structietl_1_1real__type) | 
`struct `[`ietl::real_type< std::complex< T > >`](#dc/d51/structietl_1_1real__type_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`ietl::vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits) | 

## Members

#### `enum `[`DesiredEigenvalue`](#d4/dfd/jacobi_8h_1a5e3508b9d7357572edd2fa59a61eadf6) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
Largest            | 
Smallest            | 

#### `public template<>`  <br/>`T `[`real`](#d7/d3b/complex_8h_1ac0f1d378f644863e95702fcb7846c92d)`(T x)` 

#### `public template<>`  <br/>`T `[`real`](#d7/d3b/complex_8h_1a991ef7b85878fb4946d4b8f55eb85310)`(std::complex< T > x)` 

#### `public template<>`  <br/>`T `[`conj`](#d7/d3b/complex_8h_1a576f505cbb140b6aa72ec2126f2e0a7b)`(T x)` 

#### `public template<>`  <br/>`T `[`conj`](#d7/d3b/complex_8h_1a8020f454bca2499f9a560ac8ae018cab)`(std::complex< T > x)` 

#### `public template<>`  <br/>`T * `[`get_data`](#de/de9/ietl2lapack_8h_1a5c53bf26355edab0de7372ff9701bcc3)`(const std::vector< T > & v)` 

#### `public template<>`  <br/>`std::pair< typename `[`vectorspace_traits](#d4/d26/structietl_1_1vectorspace__traits)< VS >::magnitude_type, typename [vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type > `[`inverse`](#d0/db6/inverse_8h_1a758d8e36a08be916da068e2fba2164d2)`(const MATRIX & matrix,GEN & gen,const SOLVER & solver,ITER & iter,typename `[`vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::magnitude_type sigma,const VS & vec)` 

#### `public template<>`  <br/>`void `[`mult`](#d4/dfd/jacobi_8h_1a8c957647fac0f90519d0aebb2fd92d67)`(`[`jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator)`< Matrix, VS, Vector > const & m,typename `[`jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator)`< Matrix, VS, Vector >::vector_type const & x,typename `[`jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator)`< Matrix, VS, Vector >::vector_type & y)` 

#### `public template<>`  <br/>`std::pair< typename `[`vectorspace_traits](#d4/d26/structietl_1_1vectorspace__traits)< VS >::scalar_type, typename [vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type > `[`power`](#d3/d6a/power_8h_1aef26b6c6112cbc7fed1cca17a7923cf3)`(const MATRIX & m,GEN & start,IT & iter,const VS & vec)` 

#### `public template<>`  <br/>`std::pair< typename `[`ietl::number_traits](#db/d49/structietl_1_1number__traits)< typename [vectorspace_traits](#d4/d26/structietl_1_1vectorspace__traits)< VS >::scalar_type >::magnitude_type, typename [vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type > `[`rayleigh`](#d5/d7f/rayleigh_8h_1a04790e00af423fe2e3035c2bfb2438a1)`(const MATRIX & matrix,GEN & gen,SOLVER & solver,ITER & iter,const VS & vec)` 

#### `public template<>`  <br/>`void `[`project`](#d4/d60/vectorspace_8h_1a5cc4a334a92197692d8b5226b39907f6)`(typename `[`ietl::vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type & v,const VS & vs)` 

#### `public template<>`  <br/>[`ietl::vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::vector_type `[`new_vector`](#d4/d60/vectorspace_8h_1a9bf3f18605813d405be38701e1294918)`(const VS & vs)` 

#### `public template<>`  <br/>[`ietl::vectorspace_traits`](#d4/d26/structietl_1_1vectorspace__traits)`< VS >::size_type `[`vec_dimension`](#d4/d60/vectorspace_8h_1a18a05f2374565ba55c4bb32a063a0ec5)`(const VS & vs)` 

#### `public template<>`  <br/>`void `[`copy`](#d4/d60/vectorspace_8h_1aa32a4a3e0c568e74f7eb8070f0c7d676)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src,`[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & dst)` 

#### `public template<>`  <br/>[`number_traits`](#db/d49/structietl_1_1number__traits)`< typenameV::value_type >::magnitude_type `[`two_norm`](#d4/d60/vectorspace_8h_1a427e5b22ec64cf863698a432d55083a6)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src)` 

#### `public template<>`  <br/>`V::value_type `[`dot`](#d4/d60/vectorspace_8h_1a2265aff862612289e22e88c6faa62a74)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src1,const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src2)` 

#### `public template<>`  <br/>`void `[`mult`](#d4/d60/vectorspace_8h_1a8a8daeacc2aef9b5ec75ae0ffd2e7938)`(A a,const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src,`[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & dst)` 

#### `public template<>`  <br/>`void `[`generate`](#d4/d60/vectorspace_8h_1a473405870a25e2aca90eb6caf47d7ea7)`(`[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & src,const GEN & gen)` 

#### `public template<>`  <br/>[`ietl::scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > `[`operator*`](#d4/d60/vectorspace_8h_1a4576633d2d4d497cab6bff2df3386e5c)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & v,S s)` 

#### `public template<>`  <br/>[`ietl::scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > `[`operator*`](#d4/d60/vectorspace_8h_1a7e34e26db0232f5075e7562eedec0f99)`(S s,const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & v)` 

#### `public template<>`  <br/>[`ietl::scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > `[`operator/`](#d4/d60/vectorspace_8h_1a9fcd114f63378b89a0db11b065a32777)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & v,S s)` 

# class `ietl::arnoldi_iteration` 

```
class ietl::arnoldi_iteration
  : public ietl::basic_iteration< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`arnoldi_iteration`](#d7/d38/classietl_1_1arnoldi__iteration_1a841c3ecdd022b68bf74f10fce9542cf1)`(unsigned int max_iter_,unsigned int desired_eigenvalues__,T reltol_,T abstol_)` | 
`public inline unsigned int `[`desired_eigenvalues`](#d7/d38/classietl_1_1arnoldi__iteration_1a1f99a5e982a3dd84556a54e9fec3e681)`()` | 
`protected unsigned int `[`desired_eigenvalues_`](#d7/d38/classietl_1_1arnoldi__iteration_1a60bb65b87c32420d29c5132ed0fc5106) | 

## Members

#### `public inline  `[`arnoldi_iteration`](#d7/d38/classietl_1_1arnoldi__iteration_1a841c3ecdd022b68bf74f10fce9542cf1)`(unsigned int max_iter_,unsigned int desired_eigenvalues__,T reltol_,T abstol_)` 

#### `public inline unsigned int `[`desired_eigenvalues`](#d7/d38/classietl_1_1arnoldi__iteration_1a1f99a5e982a3dd84556a54e9fec3e681)`()` 

#### `protected unsigned int `[`desired_eigenvalues_`](#d7/d38/classietl_1_1arnoldi__iteration_1a60bb65b87c32420d29c5132ed0fc5106) 

# class `ietl::bandlanczos` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`bandlanczos`](#dd/dde/classietl_1_1bandlanczos_1ac65f5ba3b79adb1dace399f3c30e5fce)`(const MATRIX & matrix,const VS & vec,const int & p)` | 
`public  `[`~bandlanczos`](#dd/dde/classietl_1_1bandlanczos_1a97034e3c9ff1c573cbb428cff880be44)`()` | 
`public template<>`  <br/>`void `[`calculate_eigenvalues`](#dd/dde/classietl_1_1bandlanczos_1ac330c07a65f807b4cc9fcab713c2666b)`(ITER & iter,const GEN & gen)` | 
`public template<>`  <br/>`void `[`calculate_eigenvectors`](#dd/dde/classietl_1_1bandlanczos_1ac351c170d47cf2f51b002d96d0a12756)`(ITER & iter,const GEN & gen)` | 
`public const std::vector< vector_type > & `[`eigenvectors`](#dd/dde/classietl_1_1bandlanczos_1abea287484c8910c91493c89109684c2f)`()` | 
`public const std::vector< int > & `[`multiplicities`](#dd/dde/classietl_1_1bandlanczos_1aaef699231b2f8b448a9b83a7d176ca74)`()` | 
`public const std::vector< magnitude_type > & `[`eigenvalues`](#dd/dde/classietl_1_1bandlanczos_1acf5c15c90cf86ce721cbad0824290251)`()` | 
`typedef `[`vector_type`](#dd/dde/classietl_1_1bandlanczos_1a6a7baab7397fae6b97dcf9465d8032e2) | 
`typedef `[`scalar_type`](#dd/dde/classietl_1_1bandlanczos_1ac3237443e2ae32dd069795ddbb5cbd37) | 
`typedef `[`magnitude_type`](#dd/dde/classietl_1_1bandlanczos_1a345884aa3f4273d90735f9999283a15f) | 
`typedef `[`eigenvec_type`](#dd/dde/classietl_1_1bandlanczos_1a6d6bfad7213695071642251f7e84b896) | 

## Members

#### `public  `[`bandlanczos`](#dd/dde/classietl_1_1bandlanczos_1ac65f5ba3b79adb1dace399f3c30e5fce)`(const MATRIX & matrix,const VS & vec,const int & p)` 

#### `public  `[`~bandlanczos`](#dd/dde/classietl_1_1bandlanczos_1a97034e3c9ff1c573cbb428cff880be44)`()` 

#### `public template<>`  <br/>`void `[`calculate_eigenvalues`](#dd/dde/classietl_1_1bandlanczos_1ac330c07a65f807b4cc9fcab713c2666b)`(ITER & iter,const GEN & gen)` 

#### `public template<>`  <br/>`void `[`calculate_eigenvectors`](#dd/dde/classietl_1_1bandlanczos_1ac351c170d47cf2f51b002d96d0a12756)`(ITER & iter,const GEN & gen)` 

#### `public const std::vector< vector_type > & `[`eigenvectors`](#dd/dde/classietl_1_1bandlanczos_1abea287484c8910c91493c89109684c2f)`()` 

#### `public const std::vector< int > & `[`multiplicities`](#dd/dde/classietl_1_1bandlanczos_1aaef699231b2f8b448a9b83a7d176ca74)`()` 

#### `public const std::vector< magnitude_type > & `[`eigenvalues`](#dd/dde/classietl_1_1bandlanczos_1acf5c15c90cf86ce721cbad0824290251)`()` 

#### `typedef `[`vector_type`](#dd/dde/classietl_1_1bandlanczos_1a6a7baab7397fae6b97dcf9465d8032e2) 

#### `typedef `[`scalar_type`](#dd/dde/classietl_1_1bandlanczos_1ac3237443e2ae32dd069795ddbb5cbd37) 

#### `typedef `[`magnitude_type`](#dd/dde/classietl_1_1bandlanczos_1a345884aa3f4273d90735f9999283a15f) 

#### `typedef `[`eigenvec_type`](#dd/dde/classietl_1_1bandlanczos_1a6d6bfad7213695071642251f7e84b896) 

# class `ietl::bandlanczos_iteration_nhighest` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`bandlanczos_iteration_nhighest`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a9dbd42db8e22e9631627f0cfd914711e)`(unsigned int max_iter,T def_tol,T dep_tol,T ghost_tol,bool ghost_discarding,unsigned int evs)` | 
`public inline bool `[`finished`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a8e6f5d1f4f1348effb3bb1c81a6017f7)`() const` | 
`public inline void `[`operator++`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a586c4693de6d236d999e4c9ff5cc5a0b)`()` | 
`public inline void `[`operator--`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a22ab5e94fc0b6e4f2aced716a950934e)`()` | 
`public inline bool `[`first`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1ae2ed8f7569b9b235303a1062d8e24c21)`()` | 
`public inline unsigned int `[`iterations`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1aafe8b08636839fe5ce8c3f6433aa4272)`()` | 
`public inline unsigned int `[`evs`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a8969b9d60dcaca4d9886743b06c7fb91)`()` | 
`public inline unsigned int `[`max_iter`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1ad00add547036c5694c3b9e9166a929e9)`()` | 
`public inline T `[`def_tol`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a559a423dc2436a544ea9820b22c25d85)`()` | 
`public inline T `[`dep_tol`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1acd011dd005e904d7dd9e840dcefd1b84)`()` | 
`public inline T `[`ghost_tol`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1ac106bc635929a04a51db1588db366b13)`()` | 
`public inline bool `[`ghost_discarding`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a95d014dcb9871c2ce9e735e58d7ccc6b)`()` | 
`public inline bool `[`low`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1af508a62778fdfa70d663bf46f0b6e093)`()` | 

## Members

#### `public inline  `[`bandlanczos_iteration_nhighest`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a9dbd42db8e22e9631627f0cfd914711e)`(unsigned int max_iter,T def_tol,T dep_tol,T ghost_tol,bool ghost_discarding,unsigned int evs)` 

#### `public inline bool `[`finished`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a8e6f5d1f4f1348effb3bb1c81a6017f7)`() const` 

#### `public inline void `[`operator++`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a586c4693de6d236d999e4c9ff5cc5a0b)`()` 

#### `public inline void `[`operator--`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a22ab5e94fc0b6e4f2aced716a950934e)`()` 

#### `public inline bool `[`first`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1ae2ed8f7569b9b235303a1062d8e24c21)`()` 

#### `public inline unsigned int `[`iterations`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1aafe8b08636839fe5ce8c3f6433aa4272)`()` 

#### `public inline unsigned int `[`evs`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a8969b9d60dcaca4d9886743b06c7fb91)`()` 

#### `public inline unsigned int `[`max_iter`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1ad00add547036c5694c3b9e9166a929e9)`()` 

#### `public inline T `[`def_tol`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a559a423dc2436a544ea9820b22c25d85)`()` 

#### `public inline T `[`dep_tol`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1acd011dd005e904d7dd9e840dcefd1b84)`()` 

#### `public inline T `[`ghost_tol`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1ac106bc635929a04a51db1588db366b13)`()` 

#### `public inline bool `[`ghost_discarding`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1a95d014dcb9871c2ce9e735e58d7ccc6b)`()` 

#### `public inline bool `[`low`](#dd/dd9/classietl_1_1bandlanczos__iteration__nhighest_1af508a62778fdfa70d663bf46f0b6e093)`()` 

# class `ietl::bandlanczos_iteration_nlowest` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`bandlanczos_iteration_nlowest`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a0da4937a685d616b8a96eac98324bb42)`(unsigned int max_iter,T def_tol,T dep_tol,T ghost_tol,bool ghost_discarding,unsigned int evs)` | 
`public inline bool `[`finished`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1aade17a4c867ec3add86c74a04ce28e33)`() const` | 
`public inline void `[`operator++`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a3182e689f98d8b8355e0085da4e9f4c3)`()` | 
`public inline void `[`operator--`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1aae52fbfd15d0fce03af0f87f5cb5674c)`()` | 
`public inline bool `[`first`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a7a5423d2446179ffcf62f3071a7e5576)`()` | 
`public inline unsigned int `[`iterations`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1ad80580caaf41e42922d01d7030ead6f8)`()` | 
`public inline unsigned int `[`evs`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a14633a589ca2a4f6bb604e6499b9a1a5)`()` | 
`public inline unsigned int `[`max_iter`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a91150b05679aa9a228519e39ae9cbda4)`()` | 
`public inline T `[`def_tol`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a251a00b0ca02c55699db8b7b7e923084)`()` | 
`public inline T `[`dep_tol`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a5e9851b63b939527b1d0eebaf154c151)`()` | 
`public inline T `[`ghost_tol`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1ac4165ee7d1913d74d022444b626d1777)`()` | 
`public inline bool `[`ghost_discarding`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1ae846ded21a1a8da055ee56abc148ce8e)`()` | 
`public inline bool `[`low`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1aa386d22f1e441098cb948f8ad448b355)`()` | 

## Members

#### `public inline  `[`bandlanczos_iteration_nlowest`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a0da4937a685d616b8a96eac98324bb42)`(unsigned int max_iter,T def_tol,T dep_tol,T ghost_tol,bool ghost_discarding,unsigned int evs)` 

#### `public inline bool `[`finished`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1aade17a4c867ec3add86c74a04ce28e33)`() const` 

#### `public inline void `[`operator++`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a3182e689f98d8b8355e0085da4e9f4c3)`()` 

#### `public inline void `[`operator--`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1aae52fbfd15d0fce03af0f87f5cb5674c)`()` 

#### `public inline bool `[`first`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a7a5423d2446179ffcf62f3071a7e5576)`()` 

#### `public inline unsigned int `[`iterations`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1ad80580caaf41e42922d01d7030ead6f8)`()` 

#### `public inline unsigned int `[`evs`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a14633a589ca2a4f6bb604e6499b9a1a5)`()` 

#### `public inline unsigned int `[`max_iter`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a91150b05679aa9a228519e39ae9cbda4)`()` 

#### `public inline T `[`def_tol`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a251a00b0ca02c55699db8b7b7e923084)`()` 

#### `public inline T `[`dep_tol`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1a5e9851b63b939527b1d0eebaf154c151)`()` 

#### `public inline T `[`ghost_tol`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1ac4165ee7d1913d74d022444b626d1777)`()` 

#### `public inline bool `[`ghost_discarding`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1ae846ded21a1a8da055ee56abc148ce8e)`()` 

#### `public inline bool `[`low`](#d4/df8/classietl_1_1bandlanczos__iteration__nlowest_1aa386d22f1e441098cb948f8ad448b355)`()` 

# class `ietl::basic_iteration` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`basic_iteration`](#d0/d85/classietl_1_1basic__iteration_1a50109ff489d95187b8ad1dfbd50f5738)`(unsigned int max_iter,T reltol,T abstol)` | 
`public inline bool `[`finished`](#d0/d85/classietl_1_1basic__iteration_1ae30b7ae6dfa9ffa67b6575f78ab562a4)`(T r,T lambda)` | 
`public inline bool `[`converged`](#d0/d85/classietl_1_1basic__iteration_1a2cca07fa77262fec1c49b324c9d62de7)`(T r,T lambda)` | 
`public inline void `[`operator++`](#d0/d85/classietl_1_1basic__iteration_1a96de1bfafde1dcfeef8fc0a83f18caaf)`()` | 
`public inline bool `[`first`](#d0/d85/classietl_1_1basic__iteration_1a2a3bf6a515cd45842cd7016c14eb1286)`()` | 
`public inline int `[`error_code`](#d0/d85/classietl_1_1basic__iteration_1aca8e9f5f79322d9fc4f7090b7c547764)`()` | 
`public inline unsigned int `[`iterations`](#d0/d85/classietl_1_1basic__iteration_1ac024ad94a6045378a91b874474efa2ad)`()` | 
`public inline T `[`relative_tolerance`](#d0/d85/classietl_1_1basic__iteration_1a2ef3730d3560a126d82e1d51cf821d74)`()` | 
`public inline T `[`absolute_tolerance`](#d0/d85/classietl_1_1basic__iteration_1a15eae9991cb7b3dc41abe5931c074bc5)`()` | 
`public inline unsigned int `[`max_iterations`](#d0/d85/classietl_1_1basic__iteration_1a9ee564c325f1738aaffb684af0c85054)`()` | 
`public inline void `[`fail`](#d0/d85/classietl_1_1basic__iteration_1afca503c0f09e234f3fc21e58e55fa7b7)`(int err_code)` | 
`public inline void `[`fail`](#d0/d85/classietl_1_1basic__iteration_1a8a98734534191a7464c0344f1abccf9c)`(int err_code,const std::string & msg)` | 
`protected int `[`error`](#d0/d85/classietl_1_1basic__iteration_1a8bca94a90771351a727f4f792e835a83) | 
`protected unsigned int `[`i`](#d0/d85/classietl_1_1basic__iteration_1acf5ebced511563f824f19c6e90959bad) | 
`protected unsigned int `[`max_iter_`](#d0/d85/classietl_1_1basic__iteration_1a907df1d1daed87e3bf1b99157510de12) | 
`protected T `[`rtol_`](#d0/d85/classietl_1_1basic__iteration_1adeb0e53ea2aed3577295854f8c4b3849) | 
`protected T `[`atol_`](#d0/d85/classietl_1_1basic__iteration_1a78e23a9f03e50819bcbacfc037cca60a) | 
`protected std::string `[`err_msg`](#d0/d85/classietl_1_1basic__iteration_1a1d73c6c4dbd4874911bec7085e7161d7) | 

## Members

#### `public inline  `[`basic_iteration`](#d0/d85/classietl_1_1basic__iteration_1a50109ff489d95187b8ad1dfbd50f5738)`(unsigned int max_iter,T reltol,T abstol)` 

#### `public inline bool `[`finished`](#d0/d85/classietl_1_1basic__iteration_1ae30b7ae6dfa9ffa67b6575f78ab562a4)`(T r,T lambda)` 

#### `public inline bool `[`converged`](#d0/d85/classietl_1_1basic__iteration_1a2cca07fa77262fec1c49b324c9d62de7)`(T r,T lambda)` 

#### `public inline void `[`operator++`](#d0/d85/classietl_1_1basic__iteration_1a96de1bfafde1dcfeef8fc0a83f18caaf)`()` 

#### `public inline bool `[`first`](#d0/d85/classietl_1_1basic__iteration_1a2a3bf6a515cd45842cd7016c14eb1286)`()` 

#### `public inline int `[`error_code`](#d0/d85/classietl_1_1basic__iteration_1aca8e9f5f79322d9fc4f7090b7c547764)`()` 

#### `public inline unsigned int `[`iterations`](#d0/d85/classietl_1_1basic__iteration_1ac024ad94a6045378a91b874474efa2ad)`()` 

#### `public inline T `[`relative_tolerance`](#d0/d85/classietl_1_1basic__iteration_1a2ef3730d3560a126d82e1d51cf821d74)`()` 

#### `public inline T `[`absolute_tolerance`](#d0/d85/classietl_1_1basic__iteration_1a15eae9991cb7b3dc41abe5931c074bc5)`()` 

#### `public inline unsigned int `[`max_iterations`](#d0/d85/classietl_1_1basic__iteration_1a9ee564c325f1738aaffb684af0c85054)`()` 

#### `public inline void `[`fail`](#d0/d85/classietl_1_1basic__iteration_1afca503c0f09e234f3fc21e58e55fa7b7)`(int err_code)` 

#### `public inline void `[`fail`](#d0/d85/classietl_1_1basic__iteration_1a8a98734534191a7464c0344f1abccf9c)`(int err_code,const std::string & msg)` 

#### `protected int `[`error`](#d0/d85/classietl_1_1basic__iteration_1a8bca94a90771351a727f4f792e835a83) 

#### `protected unsigned int `[`i`](#d0/d85/classietl_1_1basic__iteration_1acf5ebced511563f824f19c6e90959bad) 

#### `protected unsigned int `[`max_iter_`](#d0/d85/classietl_1_1basic__iteration_1a907df1d1daed87e3bf1b99157510de12) 

#### `protected T `[`rtol_`](#d0/d85/classietl_1_1basic__iteration_1adeb0e53ea2aed3577295854f8c4b3849) 

#### `protected T `[`atol_`](#d0/d85/classietl_1_1basic__iteration_1a78e23a9f03e50819bcbacfc037cca60a) 

#### `protected std::string `[`err_msg`](#d0/d85/classietl_1_1basic__iteration_1a1d73c6c4dbd4874911bec7085e7161d7) 

# class `ietl::basic_lanczos_iteration` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`basic_lanczos_iteration`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a061f81afe839b9e654ff2f4b3e431498)`(unsigned int max_iter,T r,T a)` | 
`public template<>`  <br/>`inline bool `[`finished`](#d8/d08/classietl_1_1basic__lanczos__iteration_1aa69986b221c4f97c3a3d6e50d949fc77)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` & tmatrix)` | 
`public inline bool `[`converged`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a6c942cf59067577e37a0ff2cff652cd2)`() const` | 
`public inline void `[`operator++`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a5e8a4d590856f9a6c8877d9400e1ef79)`()` | 
`public inline bool `[`first`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a7172fa44c1b227afe3dd67bcb054c926)`() const` | 
`public inline int `[`error_code`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a750ad5287ad386ba9e90760b3832a332)`() const` | 
`public inline unsigned int `[`iterations`](#d8/d08/classietl_1_1basic__lanczos__iteration_1ab27cbc21ac94c02266bd0516d85de7f5)`() const` | 
`public inline unsigned int `[`max_iterations`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a5a322687e994904af0b37c59bf5c5977)`()` | 
`public inline T `[`relative_tolerance`](#d8/d08/classietl_1_1basic__lanczos__iteration_1afc658e7a43fb1ca4dbbcfbd6db49c2b5)`() const` | 
`public inline T `[`absolute_tolerance`](#d8/d08/classietl_1_1basic__lanczos__iteration_1aeb4449b9054adb89e486e2b590711f76)`() const` | 
`public inline void `[`fail`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a415bc1504295769d8f59bb003d86243a)`(int err_code)` | 
`public inline void `[`fail`](#d8/d08/classietl_1_1basic__lanczos__iteration_1afc923bbfeba8954d7cbd9ea9c4fef4f9)`(int err_code,const std::string & msg)` | 
`protected int `[`error`](#d8/d08/classietl_1_1basic__lanczos__iteration_1aabf283578fca06a29aca738b243db24e) | 
`protected unsigned int `[`i`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a66a0446140d1aec980ab7a43fca2bd78) | 
`protected unsigned int `[`max_iter_`](#d8/d08/classietl_1_1basic__lanczos__iteration_1aebf5e71f32cae71ad9cc3c3f1f89ebb5) | 
`protected T `[`rtol_`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a8504a37e77d0faa81c97cb061b3782e7) | 
`protected T `[`atol_`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a242d0e8d3c817858ed87c6c6993e6abe) | 
`protected std::string `[`err_msg`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a64b39731fd31c52982260bedc7513c75) | 

## Members

#### `public inline  `[`basic_lanczos_iteration`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a061f81afe839b9e654ff2f4b3e431498)`(unsigned int max_iter,T r,T a)` 

#### `public template<>`  <br/>`inline bool `[`finished`](#d8/d08/classietl_1_1basic__lanczos__iteration_1aa69986b221c4f97c3a3d6e50d949fc77)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` & tmatrix)` 

#### `public inline bool `[`converged`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a6c942cf59067577e37a0ff2cff652cd2)`() const` 

#### `public inline void `[`operator++`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a5e8a4d590856f9a6c8877d9400e1ef79)`()` 

#### `public inline bool `[`first`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a7172fa44c1b227afe3dd67bcb054c926)`() const` 

#### `public inline int `[`error_code`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a750ad5287ad386ba9e90760b3832a332)`() const` 

#### `public inline unsigned int `[`iterations`](#d8/d08/classietl_1_1basic__lanczos__iteration_1ab27cbc21ac94c02266bd0516d85de7f5)`() const` 

#### `public inline unsigned int `[`max_iterations`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a5a322687e994904af0b37c59bf5c5977)`()` 

#### `public inline T `[`relative_tolerance`](#d8/d08/classietl_1_1basic__lanczos__iteration_1afc658e7a43fb1ca4dbbcfbd6db49c2b5)`() const` 

#### `public inline T `[`absolute_tolerance`](#d8/d08/classietl_1_1basic__lanczos__iteration_1aeb4449b9054adb89e486e2b590711f76)`() const` 

#### `public inline void `[`fail`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a415bc1504295769d8f59bb003d86243a)`(int err_code)` 

#### `public inline void `[`fail`](#d8/d08/classietl_1_1basic__lanczos__iteration_1afc923bbfeba8954d7cbd9ea9c4fef4f9)`(int err_code,const std::string & msg)` 

#### `protected int `[`error`](#d8/d08/classietl_1_1basic__lanczos__iteration_1aabf283578fca06a29aca738b243db24e) 

#### `protected unsigned int `[`i`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a66a0446140d1aec980ab7a43fca2bd78) 

#### `protected unsigned int `[`max_iter_`](#d8/d08/classietl_1_1basic__lanczos__iteration_1aebf5e71f32cae71ad9cc3c3f1f89ebb5) 

#### `protected T `[`rtol_`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a8504a37e77d0faa81c97cb061b3782e7) 

#### `protected T `[`atol_`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a242d0e8d3c817858ed87c6c6993e6abe) 

#### `protected std::string `[`err_msg`](#d8/d08/classietl_1_1basic__lanczos__iteration_1a64b39731fd31c52982260bedc7513c75) 

# class `ietl::bicg_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`bicg_wrapper`](#d9/d8c/classietl_1_1bicg__wrapper_1a54e55f1aeca932d5f325c2207b83149e)`(const Preconditioner M,Iteration iter)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d9/d8c/classietl_1_1bicg__wrapper_1ad960e706da90bc8fb9f61149e28f29e1)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`bicg_wrapper`](#d9/d8c/classietl_1_1bicg__wrapper_1a54e55f1aeca932d5f325c2207b83149e)`(const Preconditioner M,Iteration iter)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d9/d8c/classietl_1_1bicg__wrapper_1ad960e706da90bc8fb9f61149e28f29e1)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::bicgstab_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`bicgstab_wrapper`](#d2/d5c/classietl_1_1bicgstab__wrapper_1ae7fc560b1eebd1c5e5e12df359ae8df0)`(const Preconditioner M,Iteration iter)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d2/d5c/classietl_1_1bicgstab__wrapper_1a17a98f5da478300e2a49be6c07918796)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`bicgstab_wrapper`](#d2/d5c/classietl_1_1bicgstab__wrapper_1ae7fc560b1eebd1c5e5e12df359ae8df0)`(const Preconditioner M,Iteration iter)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d2/d5c/classietl_1_1bicgstab__wrapper_1a17a98f5da478300e2a49be6c07918796)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::cg_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`cg_wrapper`](#d4/d45/classietl_1_1cg__wrapper_1a1dcb5bd3c18e1a0c60514db8aef39275)`(const Preconditioner M,Iteration iter)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d4/d45/classietl_1_1cg__wrapper_1a0401ee508cf89f5306fd3d3531af775c)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`cg_wrapper`](#d4/d45/classietl_1_1cg__wrapper_1a1dcb5bd3c18e1a0c60514db8aef39275)`(const Preconditioner M,Iteration iter)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d4/d45/classietl_1_1cg__wrapper_1a0401ee508cf89f5306fd3d3531af775c)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::cgs_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`cgs_wrapper`](#d6/dc2/classietl_1_1cgs__wrapper_1a736faae3a89f3ff56766c8d27b79f629)`(const Preconditioner M,Iteration iter)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d6/dc2/classietl_1_1cgs__wrapper_1a3561dfbfacf3708b7c82db6da9984cb1)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`cgs_wrapper`](#d6/dc2/classietl_1_1cgs__wrapper_1a736faae3a89f3ff56766c8d27b79f629)`(const Preconditioner M,Iteration iter)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d6/dc2/classietl_1_1cgs__wrapper_1a3561dfbfacf3708b7c82db6da9984cb1)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::cheby_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`cheby_wrapper`](#d6/d49/classietl_1_1cheby__wrapper_1abbc86d3afa87ab760e231b0d1551141c)`(const Preconditioner M,Iteration iter,typename VectorB::value_type eigmin,typename VectorB::value_type eigmax)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d6/d49/classietl_1_1cheby__wrapper_1aacf4ea7fee384813e06e572da3039781)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`cheby_wrapper`](#d6/d49/classietl_1_1cheby__wrapper_1abbc86d3afa87ab760e231b0d1551141c)`(const Preconditioner M,Iteration iter,typename VectorB::value_type eigmin,typename VectorB::value_type eigmax)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d6/d49/classietl_1_1cheby__wrapper_1aacf4ea7fee384813e06e572da3039781)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::fixed_lanczos_iteration` 

```
class ietl::fixed_lanczos_iteration
  : public ietl::basic_lanczos_iteration< T, fixed_lanczos_iteration< T > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`fixed_lanczos_iteration`](#de/dc1/classietl_1_1fixed__lanczos__iteration_1a84d646bcaa5635e8c56bfd570915d723)`(unsigned int max_iter)` | 
`public template<>`  <br/>`inline bool `[`converged`](#de/dc1/classietl_1_1fixed__lanczos__iteration_1a8960bc65d268da4e04a5608d21835a0c)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` &) const` | 

## Members

#### `public inline  `[`fixed_lanczos_iteration`](#de/dc1/classietl_1_1fixed__lanczos__iteration_1a84d646bcaa5635e8c56bfd570915d723)`(unsigned int max_iter)` 

#### `public template<>`  <br/>`inline bool `[`converged`](#de/dc1/classietl_1_1fixed__lanczos__iteration_1a8960bc65d268da4e04a5608d21835a0c)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` &) const` 

# class `ietl::FortranMatrix` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline size_type `[`nrows`](#d7/d65/classietl_1_1_fortran_matrix_1abfa267d304ab76e72f3ef6eaaa4cce0a)`()` | 
`public inline size_type `[`ncols`](#d7/d65/classietl_1_1_fortran_matrix_1ac83b5aaf4b9dd7f50f1be1f90c183bbd)`()` | 
`public inline  `[`FortranMatrix`](#d7/d65/classietl_1_1_fortran_matrix_1a61dcf5fe638c83f9fa6f32151b6b2724)`(size_type n,size_type m)` | 
`public inline  `[`~FortranMatrix`](#d7/d65/classietl_1_1_fortran_matrix_1aad5394824748d4bf2a2d46253237c214)`()` | 
`public inline T * `[`data`](#d7/d65/classietl_1_1_fortran_matrix_1aaaa0fb3cce408260ab0b935dd1bcb1da)`()` | 
`public inline const T * `[`data`](#d7/d65/classietl_1_1_fortran_matrix_1a726633e827ae66d536ccf37fda747e1e)`() const` | 
`public inline T `[`operator()`](#d7/d65/classietl_1_1_fortran_matrix_1a7772d67b92509c329b3a8e369eee6691)`(size_type i,size_type j) const` | 
`public inline T & `[`operator()`](#d7/d65/classietl_1_1_fortran_matrix_1a2752a1d23cf77bf8f896ea3a0de9b84e)`(size_type i,size_type j)` | 
`public inline void `[`resize`](#d7/d65/classietl_1_1_fortran_matrix_1a5f6419328c4cbb5046eeda25d48e8fba)`(size_type n,size_type m)` | 
`public inline size_type `[`minor`](#d7/d65/classietl_1_1_fortran_matrix_1aeff818b57c71fe6d0d7b817fb0ebdb6b)`()` | 
`typedef `[`size_type`](#d7/d65/classietl_1_1_fortran_matrix_1a820443e29f88ce99ce470e8f0b4604a5) | 

## Members

#### `public inline size_type `[`nrows`](#d7/d65/classietl_1_1_fortran_matrix_1abfa267d304ab76e72f3ef6eaaa4cce0a)`()` 

#### `public inline size_type `[`ncols`](#d7/d65/classietl_1_1_fortran_matrix_1ac83b5aaf4b9dd7f50f1be1f90c183bbd)`()` 

#### `public inline  `[`FortranMatrix`](#d7/d65/classietl_1_1_fortran_matrix_1a61dcf5fe638c83f9fa6f32151b6b2724)`(size_type n,size_type m)` 

#### `public inline  `[`~FortranMatrix`](#d7/d65/classietl_1_1_fortran_matrix_1aad5394824748d4bf2a2d46253237c214)`()` 

#### `public inline T * `[`data`](#d7/d65/classietl_1_1_fortran_matrix_1aaaa0fb3cce408260ab0b935dd1bcb1da)`()` 

#### `public inline const T * `[`data`](#d7/d65/classietl_1_1_fortran_matrix_1a726633e827ae66d536ccf37fda747e1e)`() const` 

#### `public inline T `[`operator()`](#d7/d65/classietl_1_1_fortran_matrix_1a7772d67b92509c329b3a8e369eee6691)`(size_type i,size_type j) const` 

#### `public inline T & `[`operator()`](#d7/d65/classietl_1_1_fortran_matrix_1a2752a1d23cf77bf8f896ea3a0de9b84e)`(size_type i,size_type j)` 

#### `public inline void `[`resize`](#d7/d65/classietl_1_1_fortran_matrix_1a5f6419328c4cbb5046eeda25d48e8fba)`(size_type n,size_type m)` 

#### `public inline size_type `[`minor`](#d7/d65/classietl_1_1_fortran_matrix_1aeff818b57c71fe6d0d7b817fb0ebdb6b)`()` 

#### `typedef `[`size_type`](#d7/d65/classietl_1_1_fortran_matrix_1a820443e29f88ce99ce470e8f0b4604a5) 

# class `ietl::gcr_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`gcr_wrapper`](#d8/d99/classietl_1_1gcr__wrapper_1aa6b3effa1de19e178c5cd35cb8eb6bbf)`(const Preconditioner M,Iteration iter,int restart)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d8/d99/classietl_1_1gcr__wrapper_1a6418755e7c9401235b07136fc1f84860)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`gcr_wrapper`](#d8/d99/classietl_1_1gcr__wrapper_1aa6b3effa1de19e178c5cd35cb8eb6bbf)`(const Preconditioner M,Iteration iter,int restart)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d8/d99/classietl_1_1gcr__wrapper_1a6418755e7c9401235b07136fc1f84860)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::ietl_bicgstabl` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`ietl_bicgstabl`](#df/d3c/classietl_1_1ietl__bicgstabl_1a9572234dd8203734ff823ce8736a3c7f)`(unsigned int b,size_t maxiter,bool verbose)` | 
`public template<>`  <br/>`inline VECTOR `[`operator()`](#df/d3c/classietl_1_1ietl__bicgstabl_1a22e3c5353d36bdb977e2de08b9f6b69c)`(const MATRIX & A,const VECTOR & b,const VECTOR & x0,typename `[`number_traits`](#db/d49/structietl_1_1number__traits)`< SCALAR >::magnitude_type abs_tol)` | 
`protected unsigned int `[`BICGSTAB_L`](#df/d3c/classietl_1_1ietl__bicgstabl_1a0cece4e8b0902db32c3f2d9f8864e0aa) | 
`protected size_t `[`maxiter`](#df/d3c/classietl_1_1ietl__bicgstabl_1a4db42d1158235a2ca471b198a70b74c4) | 
`protected bool `[`verbose`](#df/d3c/classietl_1_1ietl__bicgstabl_1a956ce128a6ed0c7c18a2d19a387ba823) | 

## Members

#### `public inline  `[`ietl_bicgstabl`](#df/d3c/classietl_1_1ietl__bicgstabl_1a9572234dd8203734ff823ce8736a3c7f)`(unsigned int b,size_t maxiter,bool verbose)` 

#### `public template<>`  <br/>`inline VECTOR `[`operator()`](#df/d3c/classietl_1_1ietl__bicgstabl_1a22e3c5353d36bdb977e2de08b9f6b69c)`(const MATRIX & A,const VECTOR & b,const VECTOR & x0,typename `[`number_traits`](#db/d49/structietl_1_1number__traits)`< SCALAR >::magnitude_type abs_tol)` 

#### `protected unsigned int `[`BICGSTAB_L`](#df/d3c/classietl_1_1ietl__bicgstabl_1a0cece4e8b0902db32c3f2d9f8864e0aa) 

#### `protected size_t `[`maxiter`](#df/d3c/classietl_1_1ietl__bicgstabl_1a4db42d1158235a2ca471b198a70b74c4) 

#### `protected bool `[`verbose`](#df/d3c/classietl_1_1ietl__bicgstabl_1a956ce128a6ed0c7c18a2d19a387ba823) 

# class `ietl::ietl_cg` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`ietl_cg`](#d2/d83/classietl_1_1ietl__cg_1a3a2a5705c1d88e4ff54c4dae6ccb87c4)`(std::size_t max_iter,bool verbose)` | 
`public template<>`  <br/>`inline Vector `[`operator()`](#d2/d83/classietl_1_1ietl__cg_1a2d4482da80a2f0d4b90c222aa18e4c5e)`(Matrix const & A,Vector const & b,Vector const & x0,double abs_tol)` | 

## Members

#### `public inline  `[`ietl_cg`](#d2/d83/classietl_1_1ietl__cg_1a3a2a5705c1d88e4ff54c4dae6ccb87c4)`(std::size_t max_iter,bool verbose)` 

#### `public template<>`  <br/>`inline Vector `[`operator()`](#d2/d83/classietl_1_1ietl__cg_1a2d4482da80a2f0d4b90c222aa18e4c5e)`(Matrix const & A,Vector const & b,Vector const & x0,double abs_tol)` 

# class `ietl::ietl_gmres` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`ietl_gmres`](#d1/d82/classietl_1_1ietl__gmres_1acfae11d23a92ed6fc6c4d14c7c18dd22)`(std::size_t max_iter,bool verbose)` | 
`public template<>`  <br/>`inline Vector `[`operator()`](#d1/d82/classietl_1_1ietl__gmres_1a8257159a6ac0a04997ab2ed789541427)`(Matrix const & A,Vector const & b,Vector const & x0,double abs_tol)` | 

## Members

#### `public inline  `[`ietl_gmres`](#d1/d82/classietl_1_1ietl__gmres_1acfae11d23a92ed6fc6c4d14c7c18dd22)`(std::size_t max_iter,bool verbose)` 

#### `public template<>`  <br/>`inline Vector `[`operator()`](#d1/d82/classietl_1_1ietl__gmres_1a8257159a6ac0a04997ab2ed789541427)`(Matrix const & A,Vector const & b,Vector const & x0,double abs_tol)` 

# class `ietl::indexer` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`indexer`](#d0/d6a/classietl_1_1indexer_1ab87fc595a27079ad69c98a08bddaef4e)`(int pc)` | 
`public  `[`~indexer`](#d0/d6a/classietl_1_1indexer_1ae69d1c578e5aae061abd7eb12334bd0d)`()` | 
`public int `[`cnv`](#d0/d6a/classietl_1_1indexer_1a029450def6cade2a1e9b74e903891701)`(int j)` | 
`public void `[`next`](#d0/d6a/classietl_1_1indexer_1aa6e10c9dc695ec5004508939613bb0d1)`()` | 
`public void `[`deflate`](#d0/d6a/classietl_1_1indexer_1a8fc285ae87876711e365f9f001c9bb2a)`(int old)` | 

## Members

#### `public  `[`indexer`](#d0/d6a/classietl_1_1indexer_1ab87fc595a27079ad69c98a08bddaef4e)`(int pc)` 

#### `public  `[`~indexer`](#d0/d6a/classietl_1_1indexer_1ae69d1c578e5aae061abd7eb12334bd0d)`()` 

#### `public int `[`cnv`](#d0/d6a/classietl_1_1indexer_1a029450def6cade2a1e9b74e903891701)`(int j)` 

#### `public void `[`next`](#d0/d6a/classietl_1_1indexer_1aa6e10c9dc695ec5004508939613bb0d1)`()` 

#### `public void `[`deflate`](#d0/d6a/classietl_1_1indexer_1a8fc285ae87876711e365f9f001c9bb2a)`(int old)` 

# class `ietl::Info` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`Info`](#d9/db8/classietl_1_1_info_1a02bf634e49d28fa56da853b257d4f9f5)`()` | 
`public inline  `[`Info`](#d9/db8/classietl_1_1_info_1abb7d2275a78bef42f5615a0232d019dc)`(std::vector< int > M1,std::vector< int > M2,std::vector< int > Ma,std::vector< magnitude_type > Eigenvalue,std::vector< magnitude_type > Residuum,std::vector< errorinfo > Status)` | 
`public inline int `[`m1`](#d9/db8/classietl_1_1_info_1ae2609445225c8c336564303086b37e75)`(int i) const` | 
`public inline int `[`m2`](#d9/db8/classietl_1_1_info_1a1652209a8893aabb8f5d654772dafacb)`(int i) const` | 
`public inline int `[`ma`](#d9/db8/classietl_1_1_info_1a471035aa0a085e406cf2eb874ccdb7c0)`(int i) const` | 
`public inline int `[`size`](#d9/db8/classietl_1_1_info_1a47e47548b43ad7da9876aa3ad485aba1)`()` | 
`public inline magnitude_type `[`eigenvalue`](#d9/db8/classietl_1_1_info_1aa917fb745eef2913fd5e219c1317556f)`(int i) const` | 
`public inline magnitude_type `[`residual`](#d9/db8/classietl_1_1_info_1a05a3554164e611a20eb0bee4aefa114a)`(int i) const` | 
`public inline errorinfo `[`error_info`](#d9/db8/classietl_1_1_info_1aa72723002dcc793984472b7f35078144)`(int i) const` | 
`enum `[`errorinfo`](#d9/db8/classietl_1_1_info_1a4ccb5a38ee64c622f11be04a1a631665) | 

## Members

#### `public inline  `[`Info`](#d9/db8/classietl_1_1_info_1a02bf634e49d28fa56da853b257d4f9f5)`()` 

#### `public inline  `[`Info`](#d9/db8/classietl_1_1_info_1abb7d2275a78bef42f5615a0232d019dc)`(std::vector< int > M1,std::vector< int > M2,std::vector< int > Ma,std::vector< magnitude_type > Eigenvalue,std::vector< magnitude_type > Residuum,std::vector< errorinfo > Status)` 

#### `public inline int `[`m1`](#d9/db8/classietl_1_1_info_1ae2609445225c8c336564303086b37e75)`(int i) const` 

#### `public inline int `[`m2`](#d9/db8/classietl_1_1_info_1a1652209a8893aabb8f5d654772dafacb)`(int i) const` 

#### `public inline int `[`ma`](#d9/db8/classietl_1_1_info_1a471035aa0a085e406cf2eb874ccdb7c0)`(int i) const` 

#### `public inline int `[`size`](#d9/db8/classietl_1_1_info_1a47e47548b43ad7da9876aa3ad485aba1)`()` 

#### `public inline magnitude_type `[`eigenvalue`](#d9/db8/classietl_1_1_info_1aa917fb745eef2913fd5e219c1317556f)`(int i) const` 

#### `public inline magnitude_type `[`residual`](#d9/db8/classietl_1_1_info_1a05a3554164e611a20eb0bee4aefa114a)`(int i) const` 

#### `public inline errorinfo `[`error_info`](#d9/db8/classietl_1_1_info_1aa72723002dcc793984472b7f35078144)`(int i) const` 

#### `enum `[`errorinfo`](#d9/db8/classietl_1_1_info_1a4ccb5a38ee64c622f11be04a1a631665) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
ok            | 
no_eigenvalue            | 
not_calculated            | 

# class `ietl::jacobi_davidson` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`jacobi_davidson`](#d0/df4/classietl_1_1jacobi__davidson_1aef5f575728225ec63c5c330e4efc8f06)`(const MATRIX & matrix,const VS & vec,DesiredEigenvalue desired)` | 
`public  `[`~jacobi_davidson`](#d0/df4/classietl_1_1jacobi__davidson_1a7e2c3fedd146cd689bbd2ffa0573ade1)`()` | 
`public template<>`  <br/>`std::pair< magnitude_type, vector_type > `[`calculate_eigenvalue`](#d0/df4/classietl_1_1jacobi__davidson_1a8d7cf81006cda3a8f567a2f8fcc1cce1)`(const GEN & gen,SOLVER & solver,ITER & iter)` | 
`public template<>`  <br/>`std::pair< typename `[`jacobi_davidson](#d0/df4/classietl_1_1jacobi__davidson)< MATRIX, VS >::magnitude_type, typename [jacobi_davidson`](#d0/df4/classietl_1_1jacobi__davidson)`< MATRIX, VS >::vector_type > `[`calculate_eigenvalue`](#d0/df4/classietl_1_1jacobi__davidson_1acc0780b23a77e645847f6493c805252c)`(const GEN & gen,SOLVER & solver,ITER & iter)` | 
`typedef `[`vector_type`](#d0/df4/classietl_1_1jacobi__davidson_1aae956041e709b29da266a4a7c620cea7) | 
`typedef `[`scalar_type`](#d0/df4/classietl_1_1jacobi__davidson_1aa55cb21bec2a256aa027dc2a4dbf57ca) | 
`typedef `[`magnitude_type`](#d0/df4/classietl_1_1jacobi__davidson_1a122127ac5cc8721907c4f5acbccb6aa1) | 

## Members

#### `public  `[`jacobi_davidson`](#d0/df4/classietl_1_1jacobi__davidson_1aef5f575728225ec63c5c330e4efc8f06)`(const MATRIX & matrix,const VS & vec,DesiredEigenvalue desired)` 

#### `public  `[`~jacobi_davidson`](#d0/df4/classietl_1_1jacobi__davidson_1a7e2c3fedd146cd689bbd2ffa0573ade1)`()` 

#### `public template<>`  <br/>`std::pair< magnitude_type, vector_type > `[`calculate_eigenvalue`](#d0/df4/classietl_1_1jacobi__davidson_1a8d7cf81006cda3a8f567a2f8fcc1cce1)`(const GEN & gen,SOLVER & solver,ITER & iter)` 

#### `public template<>`  <br/>`std::pair< typename `[`jacobi_davidson](#d0/df4/classietl_1_1jacobi__davidson)< MATRIX, VS >::magnitude_type, typename [jacobi_davidson`](#d0/df4/classietl_1_1jacobi__davidson)`< MATRIX, VS >::vector_type > `[`calculate_eigenvalue`](#d0/df4/classietl_1_1jacobi__davidson_1acc0780b23a77e645847f6493c805252c)`(const GEN & gen,SOLVER & solver,ITER & iter)` 

#### `typedef `[`vector_type`](#d0/df4/classietl_1_1jacobi__davidson_1aae956041e709b29da266a4a7c620cea7) 

#### `typedef `[`scalar_type`](#d0/df4/classietl_1_1jacobi__davidson_1aa55cb21bec2a256aa027dc2a4dbf57ca) 

#### `typedef `[`magnitude_type`](#d0/df4/classietl_1_1jacobi__davidson_1a122127ac5cc8721907c4f5acbccb6aa1) 

# class `ietl::jcd_gmres_solver` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`jcd_gmres_solver`](#d4/de2/classietl_1_1jcd__gmres__solver_1ab7c0b19e61712fa345e5a94cc66fa5d6)`(Matrix const & matrix,VS const & vec,std::size_t max_iter,bool verbose)` | 
`public inline void `[`operator()`](#d4/de2/classietl_1_1jcd__gmres__solver_1a15c70024706c4ca01ca1d9f6a8ce9b04)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,vector_type & t,const magnitude_type & rel_tol)` | 
`typedef `[`vector_type`](#d4/de2/classietl_1_1jcd__gmres__solver_1acb793b84852425f5d778a4b5ae1dbdcc) | 
`typedef `[`scalar_type`](#d4/de2/classietl_1_1jcd__gmres__solver_1acf504b8e241fdf3df2d0b0162fb50416) | 
`typedef `[`magnitude_type`](#d4/de2/classietl_1_1jcd__gmres__solver_1a58620f68f3eddfd1cd85898295130b85) | 

## Members

#### `public inline  `[`jcd_gmres_solver`](#d4/de2/classietl_1_1jcd__gmres__solver_1ab7c0b19e61712fa345e5a94cc66fa5d6)`(Matrix const & matrix,VS const & vec,std::size_t max_iter,bool verbose)` 

#### `public inline void `[`operator()`](#d4/de2/classietl_1_1jcd__gmres__solver_1a15c70024706c4ca01ca1d9f6a8ce9b04)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,vector_type & t,const magnitude_type & rel_tol)` 

#### `typedef `[`vector_type`](#d4/de2/classietl_1_1jcd__gmres__solver_1acb793b84852425f5d778a4b5ae1dbdcc) 

#### `typedef `[`scalar_type`](#d4/de2/classietl_1_1jcd__gmres__solver_1acf504b8e241fdf3df2d0b0162fb50416) 

#### `typedef `[`magnitude_type`](#d4/de2/classietl_1_1jcd__gmres__solver_1a58620f68f3eddfd1cd85898295130b85) 

# class `ietl::jcd_left_preconditioner` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`jcd_left_preconditioner`](#d2/d34/classietl_1_1jcd__left__preconditioner_1ae92e28720e5c910d1ae0b6ba8666f268)`(const MATRIX & matrix,const VS & vec,const int & max_iter)` | 
`public void `[`operator()`](#d2/d34/classietl_1_1jcd__left__preconditioner_1a2475d4aa9c1d06b4ea351b36378be0c1)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,vector_type & t,const magnitude_type & rel_tol)` | 
`typedef `[`vector_type`](#d2/d34/classietl_1_1jcd__left__preconditioner_1a0c3ae11bf27ad2765980cd1fdf77cb8f) | 
`typedef `[`scalar_type`](#d2/d34/classietl_1_1jcd__left__preconditioner_1a2c0b66e1387d90ab3931ecc7ea7bbfe3) | 
`typedef `[`magnitude_type`](#d2/d34/classietl_1_1jcd__left__preconditioner_1a3001e97cf48eaccbce4ee9f1218289b9) | 

## Members

#### `public  `[`jcd_left_preconditioner`](#d2/d34/classietl_1_1jcd__left__preconditioner_1ae92e28720e5c910d1ae0b6ba8666f268)`(const MATRIX & matrix,const VS & vec,const int & max_iter)` 

#### `public void `[`operator()`](#d2/d34/classietl_1_1jcd__left__preconditioner_1a2475d4aa9c1d06b4ea351b36378be0c1)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,vector_type & t,const magnitude_type & rel_tol)` 

#### `typedef `[`vector_type`](#d2/d34/classietl_1_1jcd__left__preconditioner_1a0c3ae11bf27ad2765980cd1fdf77cb8f) 

#### `typedef `[`scalar_type`](#d2/d34/classietl_1_1jcd__left__preconditioner_1a2c0b66e1387d90ab3931ecc7ea7bbfe3) 

#### `typedef `[`magnitude_type`](#d2/d34/classietl_1_1jcd__left__preconditioner_1a3001e97cf48eaccbce4ee9f1218289b9) 

# class `ietl::jcd_simple_solver` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`jcd_simple_solver`](#de/d6e/classietl_1_1jcd__simple__solver_1ad6d31079ef1f88537de7fd196f238abf)`(const MATRIX & matrix,const VS & vec)` | 
`public void `[`operator()`](#de/d6e/classietl_1_1jcd__simple__solver_1af74fb1a2774b19ddb50019ee7cd13455)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,vector_type & t,const magnitude_type & rel_tol)` | 
`typedef `[`vector_type`](#de/d6e/classietl_1_1jcd__simple__solver_1aa4631df4d8fdd37f7deabb4a67519dec) | 
`typedef `[`scalar_type`](#de/d6e/classietl_1_1jcd__simple__solver_1a64ddc068e6e3b1e09f289696e0a8014c) | 
`typedef `[`magnitude_type`](#de/d6e/classietl_1_1jcd__simple__solver_1ab145fdbafc979540e8992eeeb6d0d0d9) | 

## Members

#### `public  `[`jcd_simple_solver`](#de/d6e/classietl_1_1jcd__simple__solver_1ad6d31079ef1f88537de7fd196f238abf)`(const MATRIX & matrix,const VS & vec)` 

#### `public void `[`operator()`](#de/d6e/classietl_1_1jcd__simple__solver_1af74fb1a2774b19ddb50019ee7cd13455)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,vector_type & t,const magnitude_type & rel_tol)` 

#### `typedef `[`vector_type`](#de/d6e/classietl_1_1jcd__simple__solver_1aa4631df4d8fdd37f7deabb4a67519dec) 

#### `typedef `[`scalar_type`](#de/d6e/classietl_1_1jcd__simple__solver_1a64ddc068e6e3b1e09f289696e0a8014c) 

#### `typedef `[`magnitude_type`](#de/d6e/classietl_1_1jcd__simple__solver_1ab145fdbafc979540e8992eeeb6d0d0d9) 

# class `ietl::jcd_solver` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>`inline  `[`jcd_solver`](#dd/d41/classietl_1_1jcd__solver_1a205828d199251c05171b9d4fca9d66ad)`(Matrix const & matrix,VS const & vec,Solver solv)` | 
`public template<>`  <br/>`inline void `[`replace_solver`](#dd/d41/classietl_1_1jcd__solver_1a1ae1e5609e13d748ec1aec5b95436030)`(Solver solv)` | 
`public inline void `[`operator()`](#dd/d41/classietl_1_1jcd__solver_1a854b18175194d35766abbb97e8b2e8a5)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,vector_type & t,const magnitude_type & rel_tol)` | 
`typedef `[`vector_type`](#dd/d41/classietl_1_1jcd__solver_1a11e4893d6d03117eab93404950fceebc) | 
`typedef `[`scalar_type`](#dd/d41/classietl_1_1jcd__solver_1a05893df8fefdd1437a52926eca61266d) | 
`typedef `[`magnitude_type`](#dd/d41/classietl_1_1jcd__solver_1aa7bcba444237ed7f19330e67a8649073) | 

## Members

#### `public template<>`  <br/>`inline  `[`jcd_solver`](#dd/d41/classietl_1_1jcd__solver_1a205828d199251c05171b9d4fca9d66ad)`(Matrix const & matrix,VS const & vec,Solver solv)` 

#### `public template<>`  <br/>`inline void `[`replace_solver`](#dd/d41/classietl_1_1jcd__solver_1a1ae1e5609e13d748ec1aec5b95436030)`(Solver solv)` 

#### `public inline void `[`operator()`](#dd/d41/classietl_1_1jcd__solver_1a854b18175194d35766abbb97e8b2e8a5)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,vector_type & t,const magnitude_type & rel_tol)` 

#### `typedef `[`vector_type`](#dd/d41/classietl_1_1jcd__solver_1a11e4893d6d03117eab93404950fceebc) 

#### `typedef `[`scalar_type`](#dd/d41/classietl_1_1jcd__solver_1a05893df8fefdd1437a52926eca61266d) 

#### `typedef `[`magnitude_type`](#dd/d41/classietl_1_1jcd__solver_1aa7bcba444237ed7f19330e67a8649073) 

# class `ietl::jcd_solver_operator` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator_1a1f27ab9599a1184900b430e6cbe033bf)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,const Matrix & m)` | 
`public void `[`operator()`](#d7/d82/classietl_1_1jcd__solver__operator_1aa62d4e1c2596c089637e6487a17c8abe)`(vector_type const & x,vector_type & y) const` | 
`typedef `[`vector_type`](#d7/d82/classietl_1_1jcd__solver__operator_1ae100c594504e96df362db1f7154ecb51) | 
`typedef `[`scalar_type`](#d7/d82/classietl_1_1jcd__solver__operator_1a7d8841dc76cdb91cb54d3116ce759d6e) | 
`typedef `[`magnitude_type`](#d7/d82/classietl_1_1jcd__solver__operator_1a2643e6aa1026a352fbfa1cd6437fd0b5) | 

## Members

#### `public inline  `[`jcd_solver_operator`](#d7/d82/classietl_1_1jcd__solver__operator_1a1f27ab9599a1184900b430e6cbe033bf)`(const vector_type & u,const magnitude_type & theta,const vector_type & r,const Matrix & m)` 

#### `public void `[`operator()`](#d7/d82/classietl_1_1jcd__solver__operator_1aa62d4e1c2596c089637e6487a17c8abe)`(vector_type const & x,vector_type & y) const` 

#### `typedef `[`vector_type`](#d7/d82/classietl_1_1jcd__solver__operator_1ae100c594504e96df362db1f7154ecb51) 

#### `typedef `[`scalar_type`](#d7/d82/classietl_1_1jcd__solver__operator_1a7d8841dc76cdb91cb54d3116ce759d6e) 

#### `typedef `[`magnitude_type`](#d7/d82/classietl_1_1jcd__solver__operator_1a2643e6aa1026a352fbfa1cd6437fd0b5) 

# class `ietl::jd` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`jd`](#dc/de7/classietl_1_1jd_1a58b839cbd68d2449dd7322f869344161)`(const MATRIX & A,VS & vspace,size_t v)` | 
`public template<>`  <br/>`inline void `[`eigensystem`](#dc/de7/classietl_1_1jd_1a61d8de72ae89eb272b4e27f05a3a7bdd)`(IT & iter,GEN & gen,size_type k_max,SOLV f,bool search_highest)` | 
`public template<>`  <br/>`inline void `[`eigensystem`](#dc/de7/classietl_1_1jd_1a9279b26920bbf3761ef0ecdd1eb75f70)`(IT & iter,GEN & gen,size_type k_max,PREC & K,SOLV f,bool search_highest)` | 
`public template<>`  <br/>`inline void `[`eigensystem_harmonic`](#dc/de7/classietl_1_1jd_1af14813821e3af8c21c48995f0f4866c7)`(IT & iter,GEN & gen,size_type k_max,real_type tau,SOLV & f)` | 
`public inline std::pair< real_type, vector_type > `[`eigenpair`](#dc/de7/classietl_1_1jd_1a61419cabcc09f9e4e0f6ff1e091cc5e3)`(size_type k)` | 
`public inline real_type `[`eigenvalue`](#dc/de7/classietl_1_1jd_1aec97ca797b49d0fb550089d8bb54705e)`(size_type k)` | 
`public inline real_set_type `[`eigenvalues`](#dc/de7/classietl_1_1jd_1ab9bec74122376da37e1032f55ad9fa51)`()` | 
`public inline vector_type `[`eigenvector`](#dc/de7/classietl_1_1jd_1ac3df14b86843344b9c144cc628a42e96)`(size_type k)` | 
`public inline void `[`reset`](#dc/de7/classietl_1_1jd_1a4c352afdeeb921af8964d10344e7d10a)`()` | 
`protected const MATRIX & `[`A_`](#dc/de7/classietl_1_1jd_1a84d693ab2d44f8885766ff0b7bddd558) | 
`protected VS & `[`vspace_`](#dc/de7/classietl_1_1jd_1a44629ba7f48f3c8213f334a8edffe747) | 
`protected size_type `[`n_`](#dc/de7/classietl_1_1jd_1ae89e07b14ea62bab7b3815e4d8f66b37) | 
`protected vector_set_type `[`X_`](#dc/de7/classietl_1_1jd_1a793e1648ddfcf75427a140b8b4a6d4da) | 
`protected real_set_type `[`Lambda_`](#dc/de7/classietl_1_1jd_1a1b94b2a28147e852e3b4083fa72c0fa6) | 
`protected size_t `[`verbose_`](#dc/de7/classietl_1_1jd_1ac7d66cd426e972a826e87a88816d4560) | 
`protected template<>`  <br/>`void `[`jdqr`](#dc/de7/classietl_1_1jd_1a8e10a24730048b3c273301f0c23c66fc)`(SOLVER & solver,IT & iter,GEN & gen,size_type k_max,bool search_highest)` | 
`protected template<>`  <br/>`void `[`jdqr_harmonic`](#dc/de7/classietl_1_1jd_1a91c42e06e1d6c6076a0b16db9bedb218)`(SOLVER & solver,IT & iter,GEN & gen,size_type k_max,real_type tau)` | 
`typedef `[`vector_type`](#dc/de7/classietl_1_1jd_1a431910c54e850ff038160f6864ce9f2c) | 
`typedef `[`scalar_type`](#dc/de7/classietl_1_1jd_1a239b5bb2152e6a901f11c93d31ba9110) | 
`typedef `[`size_type`](#dc/de7/classietl_1_1jd_1a4702478d1e1bc7e209073da7b8ae74ad) | 
`typedef `[`magnitude_type`](#dc/de7/classietl_1_1jd_1a5f834bf7bd5313dc29e7e504e9a1cf42) | 
`typedef `[`real_type`](#dc/de7/classietl_1_1jd_1a12d1391b4ccc4b0add850bce900051f0) | 
`typedef `[`vector_set_type`](#dc/de7/classietl_1_1jd_1aeadae2c7c7bc7b90d083dfe1a22985e6) | 
`typedef `[`real_set_type`](#dc/de7/classietl_1_1jd_1a66b52d9fff08f353cce0d9c8e0a72f5d) | 

## Members

#### `public inline  `[`jd`](#dc/de7/classietl_1_1jd_1a58b839cbd68d2449dd7322f869344161)`(const MATRIX & A,VS & vspace,size_t v)` 

#### `public template<>`  <br/>`inline void `[`eigensystem`](#dc/de7/classietl_1_1jd_1a61d8de72ae89eb272b4e27f05a3a7bdd)`(IT & iter,GEN & gen,size_type k_max,SOLV f,bool search_highest)` 

#### `public template<>`  <br/>`inline void `[`eigensystem`](#dc/de7/classietl_1_1jd_1a9279b26920bbf3761ef0ecdd1eb75f70)`(IT & iter,GEN & gen,size_type k_max,PREC & K,SOLV f,bool search_highest)` 

#### `public template<>`  <br/>`inline void `[`eigensystem_harmonic`](#dc/de7/classietl_1_1jd_1af14813821e3af8c21c48995f0f4866c7)`(IT & iter,GEN & gen,size_type k_max,real_type tau,SOLV & f)` 

#### `public inline std::pair< real_type, vector_type > `[`eigenpair`](#dc/de7/classietl_1_1jd_1a61419cabcc09f9e4e0f6ff1e091cc5e3)`(size_type k)` 

#### `public inline real_type `[`eigenvalue`](#dc/de7/classietl_1_1jd_1aec97ca797b49d0fb550089d8bb54705e)`(size_type k)` 

#### `public inline real_set_type `[`eigenvalues`](#dc/de7/classietl_1_1jd_1ab9bec74122376da37e1032f55ad9fa51)`()` 

#### `public inline vector_type `[`eigenvector`](#dc/de7/classietl_1_1jd_1ac3df14b86843344b9c144cc628a42e96)`(size_type k)` 

#### `public inline void `[`reset`](#dc/de7/classietl_1_1jd_1a4c352afdeeb921af8964d10344e7d10a)`()` 

#### `protected const MATRIX & `[`A_`](#dc/de7/classietl_1_1jd_1a84d693ab2d44f8885766ff0b7bddd558) 

#### `protected VS & `[`vspace_`](#dc/de7/classietl_1_1jd_1a44629ba7f48f3c8213f334a8edffe747) 

#### `protected size_type `[`n_`](#dc/de7/classietl_1_1jd_1ae89e07b14ea62bab7b3815e4d8f66b37) 

#### `protected vector_set_type `[`X_`](#dc/de7/classietl_1_1jd_1a793e1648ddfcf75427a140b8b4a6d4da) 

#### `protected real_set_type `[`Lambda_`](#dc/de7/classietl_1_1jd_1a1b94b2a28147e852e3b4083fa72c0fa6) 

#### `protected size_t `[`verbose_`](#dc/de7/classietl_1_1jd_1ac7d66cd426e972a826e87a88816d4560) 

#### `protected template<>`  <br/>`void `[`jdqr`](#dc/de7/classietl_1_1jd_1a8e10a24730048b3c273301f0c23c66fc)`(SOLVER & solver,IT & iter,GEN & gen,size_type k_max,bool search_highest)` 

#### `protected template<>`  <br/>`void `[`jdqr_harmonic`](#dc/de7/classietl_1_1jd_1a91c42e06e1d6c6076a0b16db9bedb218)`(SOLVER & solver,IT & iter,GEN & gen,size_type k_max,real_type tau)` 

#### `typedef `[`vector_type`](#dc/de7/classietl_1_1jd_1a431910c54e850ff038160f6864ce9f2c) 

#### `typedef `[`scalar_type`](#dc/de7/classietl_1_1jd_1a239b5bb2152e6a901f11c93d31ba9110) 

#### `typedef `[`size_type`](#dc/de7/classietl_1_1jd_1a4702478d1e1bc7e209073da7b8ae74ad) 

#### `typedef `[`magnitude_type`](#dc/de7/classietl_1_1jd_1a5f834bf7bd5313dc29e7e504e9a1cf42) 

#### `typedef `[`real_type`](#dc/de7/classietl_1_1jd_1a12d1391b4ccc4b0add850bce900051f0) 

#### `typedef `[`vector_set_type`](#dc/de7/classietl_1_1jd_1aeadae2c7c7bc7b90d083dfe1a22985e6) 

#### `typedef `[`real_set_type`](#dc/de7/classietl_1_1jd_1a66b52d9fff08f353cce0d9c8e0a72f5d) 

# class `ietl::jd_iteration` 

```
class ietl::jd_iteration
  : public ietl::basic_iteration< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`jd_iteration`](#d3/d34/classietl_1_1jd__iteration_1af1987cc93be8bfe8ba06d022ba918bb6)`(size_t max_iter,size_t m_min,size_t m_max,T reltol,T abstol)` | 
`public inline size_t `[`m_min`](#d3/d34/classietl_1_1jd__iteration_1a7ced1ae7d31fc2bcdcede9c9a4572abb)`() const` | 
`public inline size_t `[`m_max`](#d3/d34/classietl_1_1jd__iteration_1ae07794a3d877a7986e200d04f479e928)`() const` | 
`public inline const std::string & `[`error_msg`](#d3/d34/classietl_1_1jd__iteration_1a425cac9736c15d41423c3f2b4ad1b853)`()` | 

## Members

#### `public inline  `[`jd_iteration`](#d3/d34/classietl_1_1jd__iteration_1af1987cc93be8bfe8ba06d022ba918bb6)`(size_t max_iter,size_t m_min,size_t m_max,T reltol,T abstol)` 

#### `public inline size_t `[`m_min`](#d3/d34/classietl_1_1jd__iteration_1a7ced1ae7d31fc2bcdcede9c9a4572abb)`() const` 

#### `public inline size_t `[`m_max`](#d3/d34/classietl_1_1jd__iteration_1ae07794a3d877a7986e200d04f479e928)`() const` 

#### `public inline const std::string & `[`error_msg`](#d3/d34/classietl_1_1jd__iteration_1a425cac9736c15d41423c3f2b4ad1b853)`()` 

# class `ietl::lanczos` 

```
class ietl::lanczos
  : public ietl::Tmatrix< VS >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`lanczos`](#d1/d82/classietl_1_1lanczos_1a0089e62628d5c0a34fdbd379293325f0)`(const MATRIX & matrix,const VS & vec)` | 
`public template<>`  <br/>`inline void `[`calculate_eigenvalues`](#d1/d82/classietl_1_1lanczos_1a55fae88d2a7cd21f96d1c4bac32cf900)`(IT & iter,GEN gen)` | 
`public template<>`  <br/>`inline void `[`more_eigenvalues`](#d1/d82/classietl_1_1lanczos_1aef849820391bbb2566b9b02b5deec907)`(IT & iter)` | 
`public template<>`  <br/>`void `[`eigenvectors`](#d1/d82/classietl_1_1lanczos_1a9fbdea9cbb5ebed8f1d5f2279b3607b2)`(IN in_eigvals_start,IN in_eigvals_end,OUT eig_vectors,`[`Info`](#d9/db8/classietl_1_1_info)`< magnitude_type > & inf,GEN gen,int maxiter,int maxcount)` | 
`public inline std::vector< std::vector< magnitude_type > > const & `[`t_eigenvectors`](#d1/d82/classietl_1_1lanczos_1a06f771454bd0c45a00244551f8d74a6f)`()` | 
`public template<>`  <br/>`inline void `[`save`](#d1/d82/classietl_1_1lanczos_1a63514ffa9be592ea3b2c3743700b7ba4)`(Archive & ar) const` | 
`public template<>`  <br/>`inline void `[`load`](#d1/d82/classietl_1_1lanczos_1aa01c51785b42eca6b6c7ca3e45e71e32)`(Archive & ar)` | 
`public template<>`  <br/>`std::pair< typename `[`lanczos](#d1/d82/classietl_1_1lanczos)< MATRIX, VS >::magnitude_type, typename [lanczos`](#d1/d82/classietl_1_1lanczos)`< MATRIX, VS >::magnitude_type > `[`make_first_step`](#d1/d82/classietl_1_1lanczos_1aa7615f98a092227634b34ced92aabf5d)`(GEN gen)` | 
`typedef `[`vector_type`](#d1/d82/classietl_1_1lanczos_1a491a20a7e965baad6e2ab431b81d24bc) | 
`typedef `[`scalar_type`](#d1/d82/classietl_1_1lanczos_1a74f3e01ee5a157222af7b3ba4c292229) | 
`typedef `[`magnitude_type`](#d1/d82/classietl_1_1lanczos_1a7594d77bcb4bee206b17bd28c4b7028a) | 

## Members

#### `public  `[`lanczos`](#d1/d82/classietl_1_1lanczos_1a0089e62628d5c0a34fdbd379293325f0)`(const MATRIX & matrix,const VS & vec)` 

#### `public template<>`  <br/>`inline void `[`calculate_eigenvalues`](#d1/d82/classietl_1_1lanczos_1a55fae88d2a7cd21f96d1c4bac32cf900)`(IT & iter,GEN gen)` 

#### `public template<>`  <br/>`inline void `[`more_eigenvalues`](#d1/d82/classietl_1_1lanczos_1aef849820391bbb2566b9b02b5deec907)`(IT & iter)` 

#### `public template<>`  <br/>`void `[`eigenvectors`](#d1/d82/classietl_1_1lanczos_1a9fbdea9cbb5ebed8f1d5f2279b3607b2)`(IN in_eigvals_start,IN in_eigvals_end,OUT eig_vectors,`[`Info`](#d9/db8/classietl_1_1_info)`< magnitude_type > & inf,GEN gen,int maxiter,int maxcount)` 

#### `public inline std::vector< std::vector< magnitude_type > > const & `[`t_eigenvectors`](#d1/d82/classietl_1_1lanczos_1a06f771454bd0c45a00244551f8d74a6f)`()` 

#### `public template<>`  <br/>`inline void `[`save`](#d1/d82/classietl_1_1lanczos_1a63514ffa9be592ea3b2c3743700b7ba4)`(Archive & ar) const` 

#### `public template<>`  <br/>`inline void `[`load`](#d1/d82/classietl_1_1lanczos_1aa01c51785b42eca6b6c7ca3e45e71e32)`(Archive & ar)` 

#### `public template<>`  <br/>`std::pair< typename `[`lanczos](#d1/d82/classietl_1_1lanczos)< MATRIX, VS >::magnitude_type, typename [lanczos`](#d1/d82/classietl_1_1lanczos)`< MATRIX, VS >::magnitude_type > `[`make_first_step`](#d1/d82/classietl_1_1lanczos_1aa7615f98a092227634b34ced92aabf5d)`(GEN gen)` 

#### `typedef `[`vector_type`](#d1/d82/classietl_1_1lanczos_1a491a20a7e965baad6e2ab431b81d24bc) 

#### `typedef `[`scalar_type`](#d1/d82/classietl_1_1lanczos_1a74f3e01ee5a157222af7b3ba4c292229) 

#### `typedef `[`magnitude_type`](#d1/d82/classietl_1_1lanczos_1a7594d77bcb4bee206b17bd28c4b7028a) 

# class `ietl::lanczos_iteration_nhighest` 

```
class ietl::lanczos_iteration_nhighest
  : public ietl::basic_lanczos_iteration< T, lanczos_iteration_nhighest< T > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`lanczos_iteration_nhighest`](#d4/d22/classietl_1_1lanczos__iteration__nhighest_1a2838b489166540ba68d0738e7aa66e45)`(unsigned int max_iter,unsigned int n,T r,T a)` | 
`public template<>`  <br/>`inline bool `[`converged`](#d4/d22/classietl_1_1lanczos__iteration__nhighest_1abcdd8b0c51df991249af5f5445ef3532)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` & tmatrix) const` | 

## Members

#### `public inline  `[`lanczos_iteration_nhighest`](#d4/d22/classietl_1_1lanczos__iteration__nhighest_1a2838b489166540ba68d0738e7aa66e45)`(unsigned int max_iter,unsigned int n,T r,T a)` 

#### `public template<>`  <br/>`inline bool `[`converged`](#d4/d22/classietl_1_1lanczos__iteration__nhighest_1abcdd8b0c51df991249af5f5445ef3532)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` & tmatrix) const` 

# class `ietl::lanczos_iteration_nlowest` 

```
class ietl::lanczos_iteration_nlowest
  : public ietl::basic_lanczos_iteration< T, lanczos_iteration_nlowest< T > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`lanczos_iteration_nlowest`](#d9/d8a/classietl_1_1lanczos__iteration__nlowest_1a12d883d0020c3f9063c32cc2bc773d11)`(unsigned int max_iter,unsigned int n,T r,T a)` | 
`public template<>`  <br/>`inline bool `[`converged`](#d9/d8a/classietl_1_1lanczos__iteration__nlowest_1aa57b4af4788fe90fb90d64ea14d84d8b)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` & tmatrix) const` | 

## Members

#### `public inline  `[`lanczos_iteration_nlowest`](#d9/d8a/classietl_1_1lanczos__iteration__nlowest_1a12d883d0020c3f9063c32cc2bc773d11)`(unsigned int max_iter,unsigned int n,T r,T a)` 

#### `public template<>`  <br/>`inline bool `[`converged`](#d9/d8a/classietl_1_1lanczos__iteration__nlowest_1aa57b4af4788fe90fb90d64ea14d84d8b)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` & tmatrix) const` 

# class `ietl::lanczos_nlowest_better` 

```
class ietl::lanczos_nlowest_better
  : public ietl::basic_lanczos_iteration< T, lanczos_nlowest_better< T > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`lanczos_nlowest_better`](#de/d68/classietl_1_1lanczos__nlowest__better_1a5b79d0e1d694bcee0b9db6d26eb55724)`(unsigned int max_iter,unsigned int n,T r,T a,unsigned int check_each)` | 
`public template<>`  <br/>`inline bool `[`converged`](#de/d68/classietl_1_1lanczos__nlowest__better_1a65c0dbcde718722d9393587cd0793105)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` & tmatrix) const` | 

## Members

#### `public inline  `[`lanczos_nlowest_better`](#de/d68/classietl_1_1lanczos__nlowest__better_1a5b79d0e1d694bcee0b9db6d26eb55724)`(unsigned int max_iter,unsigned int n,T r,T a,unsigned int check_each)` 

#### `public template<>`  <br/>`inline bool `[`converged`](#de/d68/classietl_1_1lanczos__nlowest__better_1a65c0dbcde718722d9393587cd0793105)`(const `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix)` & tmatrix) const` 

# class `ietl::qmr_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`qmr_wrapper`](#d1/d5e/classietl_1_1qmr__wrapper_1ae22addb3f1925cc889f9032a01f5e259)`(const Precond1 M1,const Precond2 M2,Iteration iter)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d1/d5e/classietl_1_1qmr__wrapper_1a5c660d20e57ffd6e3ea6eadf7a576027)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`qmr_wrapper`](#d1/d5e/classietl_1_1qmr__wrapper_1ae22addb3f1925cc889f9032a01f5e259)`(const Precond1 M1,const Precond2 M2,Iteration iter)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d1/d5e/classietl_1_1qmr__wrapper_1a5c660d20e57ffd6e3ea6eadf7a576027)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::richardson_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`richardson_wrapper`](#d6/d46/classietl_1_1richardson__wrapper_1ae8faf06fe1a8bc92d69f21f761735917)`(const Preconditioner M,Iteration iter)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d6/d46/classietl_1_1richardson__wrapper_1a2f834eecfff0837e827ce99970b571a8)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`richardson_wrapper`](#d6/d46/classietl_1_1richardson__wrapper_1ae8faf06fe1a8bc92d69f21f761735917)`(const Preconditioner M,Iteration iter)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d6/d46/classietl_1_1richardson__wrapper_1a2f834eecfff0837e827ce99970b571a8)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::scaled_vector_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper_1aef1c6cd8bfbed040f630e4766abae12c)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & v,S s)` | 
`public inline const V & `[`vector`](#d0/dae/classietl_1_1scaled__vector__wrapper_1afb514933eaa0586c0c7bb96854f73087)`() const` | 
`public inline S `[`scalar`](#d0/dae/classietl_1_1scaled__vector__wrapper_1a96f6041c6be4358178388222e00c18dc)`() const` | 

## Members

#### `public inline  `[`scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper_1aef1c6cd8bfbed040f630e4766abae12c)`(const `[`ietl::vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)`< V > & v,S s)` 

#### `public inline const V & `[`vector`](#d0/dae/classietl_1_1scaled__vector__wrapper_1afb514933eaa0586c0c7bb96854f73087)`() const` 

#### `public inline S `[`scalar`](#d0/dae/classietl_1_1scaled__vector__wrapper_1a96f6041c6be4358178388222e00c18dc)`() const` 

# class `ietl::simple_arnoldi` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`simple_arnoldi`](#d0/df4/classietl_1_1simple__arnoldi_1a561800d17ce4c551282d15a526f7467b)`(Matrix & mat_,VS & vs_,Gen & rng_)` | 
`public template<>`  <br/>`inline void `[`calculate_eigenvalues`](#d0/df4/classietl_1_1simple__arnoldi_1af75e281e533848e51f9cde85d1f01727)`(Iter & iter,bool verbose)` | 
`public inline std::complex< double > `[`get_eigenvalue`](#d0/df4/classietl_1_1simple__arnoldi_1abfb4627f187fd964b0ce5a17022bddb3)`(int i)` | 
`protected Matrix & `[`mat`](#d0/df4/classietl_1_1simple__arnoldi_1ab6e10afffae1d20e7721a39d954a44c7) | 
`protected VS & `[`vs`](#d0/df4/classietl_1_1simple__arnoldi_1a2f1b3e70c16736c058fdcda739d639a8) | 
`protected Gen & `[`rng`](#d0/df4/classietl_1_1simple__arnoldi_1a4e9c3c91b5fa24dba471ccb3d0609f07) | 
`protected std::vector< std::complex< double > > `[`evals`](#d0/df4/classietl_1_1simple__arnoldi_1a8d6d64536f72812809ad223db5f491cc) | 
`typedef `[`vector_type`](#d0/df4/classietl_1_1simple__arnoldi_1ae4614adf25891da6cf1672784ff64cff) | 
`typedef `[`scalar_type`](#d0/df4/classietl_1_1simple__arnoldi_1a8fb4c7526b760b4cc6174a3f807d8139) | 
`typedef `[`magnitude_type`](#d0/df4/classietl_1_1simple__arnoldi_1a94fa718193fd08667c6329676ff60b01) | 

## Members

#### `public inline  `[`simple_arnoldi`](#d0/df4/classietl_1_1simple__arnoldi_1a561800d17ce4c551282d15a526f7467b)`(Matrix & mat_,VS & vs_,Gen & rng_)` 

#### `public template<>`  <br/>`inline void `[`calculate_eigenvalues`](#d0/df4/classietl_1_1simple__arnoldi_1af75e281e533848e51f9cde85d1f01727)`(Iter & iter,bool verbose)` 

#### `public inline std::complex< double > `[`get_eigenvalue`](#d0/df4/classietl_1_1simple__arnoldi_1abfb4627f187fd964b0ce5a17022bddb3)`(int i)` 

#### `protected Matrix & `[`mat`](#d0/df4/classietl_1_1simple__arnoldi_1ab6e10afffae1d20e7721a39d954a44c7) 

#### `protected VS & `[`vs`](#d0/df4/classietl_1_1simple__arnoldi_1a2f1b3e70c16736c058fdcda739d639a8) 

#### `protected Gen & `[`rng`](#d0/df4/classietl_1_1simple__arnoldi_1a4e9c3c91b5fa24dba471ccb3d0609f07) 

#### `protected std::vector< std::complex< double > > `[`evals`](#d0/df4/classietl_1_1simple__arnoldi_1a8d6d64536f72812809ad223db5f491cc) 

#### `typedef `[`vector_type`](#d0/df4/classietl_1_1simple__arnoldi_1ae4614adf25891da6cf1672784ff64cff) 

#### `typedef `[`scalar_type`](#d0/df4/classietl_1_1simple__arnoldi_1a8fb4c7526b760b4cc6174a3f807d8139) 

#### `typedef `[`magnitude_type`](#d0/df4/classietl_1_1simple__arnoldi_1a94fa718193fd08667c6329676ff60b01) 

# class `ietl::tfqmr_wrapper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`tfqmr_wrapper`](#d9/d9d/classietl_1_1tfqmr__wrapper_1aa4fc164303cb5f971155278f5fe400d3)`(const Precond1 M1,const Precond2 M2,Iteration iter)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d9/d9d/classietl_1_1tfqmr__wrapper_1a9ad9fb6c1e7b2e865ba77986133bd207)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` | 

## Members

#### `public inline  `[`tfqmr_wrapper`](#d9/d9d/classietl_1_1tfqmr__wrapper_1aa4fc164303cb5f971155278f5fe400d3)`(const Precond1 M1,const Precond2 M2,Iteration iter)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d9/d9d/classietl_1_1tfqmr__wrapper_1a9ad9fb6c1e7b2e865ba77986133bd207)`(const Matrix & A,scalar_type s,VectorX & x,const VectorB & b)` 

# class `ietl::Tmatrix` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix_1a194580a5cfcdafa35eb4487aab55c6aa)`()` | 
`public inline void `[`push_back`](#db/da5/classietl_1_1_tmatrix_1a324a521408f9f834e57b484984effcf0)`(magnitude_type a,magnitude_type b)` | 
`public inline void `[`push_back`](#db/da5/classietl_1_1_tmatrix_1a71b4b11759805eb13f53a44924075c4d)`(std::pair< magnitude_type, magnitude_type > a_and_b)` | 
`public inline const std::vector< magnitude_type > & `[`eigenvalues`](#db/da5/classietl_1_1_tmatrix_1ae5d8d559ade01e99c71ad5fb6e63edef)`(bool discard_ghosts) const` | 
`public inline const std::vector< magnitude_type > & `[`errors`](#db/da5/classietl_1_1_tmatrix_1a570b59e67929921d2e805134748a661c)`(bool discard_ghosts) const` | 
`public inline const std::vector< int > & `[`multiplicities`](#db/da5/classietl_1_1_tmatrix_1a25b748931d380a2f937c9457b3d794c2)`(bool discard_ghosts) const` | 
`public inline std::vector< magnitude_type > const & `[`diagonal`](#db/da5/classietl_1_1_tmatrix_1a2e5265d363d510673f8f499b9e2b619a)`() const` | 
`public inline std::vector< magnitude_type > const & `[`subdiagonal`](#db/da5/classietl_1_1_tmatrix_1a89a33157e44f43e7c8007713fa6f2612)`() const` | 
`public template<>`  <br/>`inline void `[`save`](#db/da5/classietl_1_1_tmatrix_1a2ba61ac8422d51fc940114d519c8fc89)`(Archive & ar) const` | 
`public template<>`  <br/>`inline void `[`load`](#db/da5/classietl_1_1_tmatrix_1a18d4bb034b63a3064248b0e408140861)`(Archive & ar)` | 
`protected std::vector< magnitude_type > `[`alpha`](#db/da5/classietl_1_1_tmatrix_1a217dbf6d1aa9ab35bf19b3f7bf09d41b) | 
`protected std::vector< magnitude_type > `[`beta`](#db/da5/classietl_1_1_tmatrix_1a03abfbddf34fa0a0ff60eb181c073b0c) | 
`protected magnitude_type `[`error_tol`](#db/da5/classietl_1_1_tmatrix_1a2b4ac214db7d5ef54c6bbb5f38eb1531) | 
`protected mutable magnitude_type `[`thold`](#db/da5/classietl_1_1_tmatrix_1a22ae5dc85d038d8b6e0930fec62c0381) | 
`typedef `[`scalar_type`](#db/da5/classietl_1_1_tmatrix_1a5b053840678044de3952d933bce93f5f) | 
`typedef `[`vector_type`](#db/da5/classietl_1_1_tmatrix_1a0d001101fc0067322c34c43a291ab233) | 
`typedef `[`magnitude_type`](#db/da5/classietl_1_1_tmatrix_1ac90c8ac1307bd138d3621125726b9be9) | 
`typedef `[`size_type`](#db/da5/classietl_1_1_tmatrix_1ac2476f82a65e36198cb8c015679e6536) | 

## Members

#### `public inline  `[`Tmatrix`](#db/da5/classietl_1_1_tmatrix_1a194580a5cfcdafa35eb4487aab55c6aa)`()` 

#### `public inline void `[`push_back`](#db/da5/classietl_1_1_tmatrix_1a324a521408f9f834e57b484984effcf0)`(magnitude_type a,magnitude_type b)` 

#### `public inline void `[`push_back`](#db/da5/classietl_1_1_tmatrix_1a71b4b11759805eb13f53a44924075c4d)`(std::pair< magnitude_type, magnitude_type > a_and_b)` 

#### `public inline const std::vector< magnitude_type > & `[`eigenvalues`](#db/da5/classietl_1_1_tmatrix_1ae5d8d559ade01e99c71ad5fb6e63edef)`(bool discard_ghosts) const` 

#### `public inline const std::vector< magnitude_type > & `[`errors`](#db/da5/classietl_1_1_tmatrix_1a570b59e67929921d2e805134748a661c)`(bool discard_ghosts) const` 

#### `public inline const std::vector< int > & `[`multiplicities`](#db/da5/classietl_1_1_tmatrix_1a25b748931d380a2f937c9457b3d794c2)`(bool discard_ghosts) const` 

#### `public inline std::vector< magnitude_type > const & `[`diagonal`](#db/da5/classietl_1_1_tmatrix_1a2e5265d363d510673f8f499b9e2b619a)`() const` 

#### `public inline std::vector< magnitude_type > const & `[`subdiagonal`](#db/da5/classietl_1_1_tmatrix_1a89a33157e44f43e7c8007713fa6f2612)`() const` 

#### `public template<>`  <br/>`inline void `[`save`](#db/da5/classietl_1_1_tmatrix_1a2ba61ac8422d51fc940114d519c8fc89)`(Archive & ar) const` 

#### `public template<>`  <br/>`inline void `[`load`](#db/da5/classietl_1_1_tmatrix_1a18d4bb034b63a3064248b0e408140861)`(Archive & ar)` 

#### `protected std::vector< magnitude_type > `[`alpha`](#db/da5/classietl_1_1_tmatrix_1a217dbf6d1aa9ab35bf19b3f7bf09d41b) 

#### `protected std::vector< magnitude_type > `[`beta`](#db/da5/classietl_1_1_tmatrix_1a03abfbddf34fa0a0ff60eb181c073b0c) 

#### `protected magnitude_type `[`error_tol`](#db/da5/classietl_1_1_tmatrix_1a2b4ac214db7d5ef54c6bbb5f38eb1531) 

#### `protected mutable magnitude_type `[`thold`](#db/da5/classietl_1_1_tmatrix_1a22ae5dc85d038d8b6e0930fec62c0381) 

#### `typedef `[`scalar_type`](#db/da5/classietl_1_1_tmatrix_1a5b053840678044de3952d933bce93f5f) 

#### `typedef `[`vector_type`](#db/da5/classietl_1_1_tmatrix_1a0d001101fc0067322c34c43a291ab233) 

#### `typedef `[`magnitude_type`](#db/da5/classietl_1_1_tmatrix_1ac90c8ac1307bd138d3621125726b9be9) 

#### `typedef `[`size_type`](#db/da5/classietl_1_1_tmatrix_1ac2476f82a65e36198cb8c015679e6536) 

# class `ietl::vector_wrapper` 

```
class ietl::vector_wrapper
  : public boost::shared_ptr< V >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper_1a608db7d09cbbc33be18a27782b412665)`(V * p)` | 
`public inline  `[`operator V&`](#d0/dba/classietl_1_1vector__wrapper_1a8890c3ef2c06c2daf13b2e59f344c17f)`()` | 
`public inline  `[`operator const V &`](#d0/dba/classietl_1_1vector__wrapper_1a222272464eb67e2517ba47a6a888e76f)`() const` | 
`public inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` `[`operator+=`](#d0/dba/classietl_1_1vector__wrapper_1ad93e2004b7dfec97f51c9897878a7e39)`(const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & x)` | 
`public inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` `[`operator-=`](#d0/dba/classietl_1_1vector__wrapper_1a4ecc9a1fc3af7e3b9f45f3a4136814f3)`(const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & x)` | 
`public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator*=`](#d0/dba/classietl_1_1vector__wrapper_1a654fc060ff90cd2b2648f272f4ed64ac)`(T x)` | 
`public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator/=`](#d0/dba/classietl_1_1vector__wrapper_1a014cb2a334f2f27097b2e49f277568e2)`(T x)` | 
`public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator+=`](#d0/dba/classietl_1_1vector__wrapper_1a5f1bdd1ede941213e3627706284babd3)`(const `[`scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > & x)` | 
`public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator-=`](#d0/dba/classietl_1_1vector__wrapper_1a87efd7970d926369f10f41890cd6f14f)`(const `[`scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > & x)` | 
`public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator=`](#d0/dba/classietl_1_1vector__wrapper_1a50558211648dae38148dbeefc8567f87)`(const `[`scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > & x)` | 

## Members

#### `public inline  `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper_1a608db7d09cbbc33be18a27782b412665)`(V * p)` 

#### `public inline  `[`operator V&`](#d0/dba/classietl_1_1vector__wrapper_1a8890c3ef2c06c2daf13b2e59f344c17f)`()` 

#### `public inline  `[`operator const V &`](#d0/dba/classietl_1_1vector__wrapper_1a222272464eb67e2517ba47a6a888e76f)`() const` 

#### `public inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` `[`operator+=`](#d0/dba/classietl_1_1vector__wrapper_1ad93e2004b7dfec97f51c9897878a7e39)`(const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & x)` 

#### `public inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` `[`operator-=`](#d0/dba/classietl_1_1vector__wrapper_1a4ecc9a1fc3af7e3b9f45f3a4136814f3)`(const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & x)` 

#### `public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator*=`](#d0/dba/classietl_1_1vector__wrapper_1a654fc060ff90cd2b2648f272f4ed64ac)`(T x)` 

#### `public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator/=`](#d0/dba/classietl_1_1vector__wrapper_1a014cb2a334f2f27097b2e49f277568e2)`(T x)` 

#### `public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator+=`](#d0/dba/classietl_1_1vector__wrapper_1a5f1bdd1ede941213e3627706284babd3)`(const `[`scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > & x)` 

#### `public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator-=`](#d0/dba/classietl_1_1vector__wrapper_1a87efd7970d926369f10f41890cd6f14f)`(const `[`scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > & x)` 

#### `public template<>`  <br/>`inline const `[`vector_wrapper`](#d0/dba/classietl_1_1vector__wrapper)` & `[`operator=`](#d0/dba/classietl_1_1vector__wrapper_1a50558211648dae38148dbeefc8567f87)`(const `[`scaled_vector_wrapper`](#d0/dae/classietl_1_1scaled__vector__wrapper)`< V, S > & x)` 

# class `ietl::vectorspace` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`vectorspace`](#d7/d6c/classietl_1_1vectorspace_1a1ad66ed84ca48268a38b05a655cd40a9)`(size_type n)` | 
`public inline size_type `[`vec_dimension`](#d7/d6c/classietl_1_1vectorspace_1ab5cf62c0672e71e201fb398c9d6754c9)`() const` | 
`public inline vector_type `[`new_vector`](#d7/d6c/classietl_1_1vectorspace_1a57f8b2ba0b7144f52f42732015e1707b)`() const` | 
`public inline void `[`project`](#d7/d6c/classietl_1_1vectorspace_1aba16c9c254622b18810348e52ae9be9d)`(vector_type &) const` | 
`typedef `[`vector_type`](#d7/d6c/classietl_1_1vectorspace_1a49aec532d5fb86762dba803fc02df296) | 
`typedef `[`scalar_type`](#d7/d6c/classietl_1_1vectorspace_1ad9f5da50a802270619afa459e6019c19) | 
`typedef `[`size_type`](#d7/d6c/classietl_1_1vectorspace_1abeac0770949b15460f3a0724aedb3705) | 

## Members

#### `public inline  `[`vectorspace`](#d7/d6c/classietl_1_1vectorspace_1a1ad66ed84ca48268a38b05a655cd40a9)`(size_type n)` 

#### `public inline size_type `[`vec_dimension`](#d7/d6c/classietl_1_1vectorspace_1ab5cf62c0672e71e201fb398c9d6754c9)`() const` 

#### `public inline vector_type `[`new_vector`](#d7/d6c/classietl_1_1vectorspace_1a57f8b2ba0b7144f52f42732015e1707b)`() const` 

#### `public inline void `[`project`](#d7/d6c/classietl_1_1vectorspace_1aba16c9c254622b18810348e52ae9be9d)`(vector_type &) const` 

#### `typedef `[`vector_type`](#d7/d6c/classietl_1_1vectorspace_1a49aec532d5fb86762dba803fc02df296) 

#### `typedef `[`scalar_type`](#d7/d6c/classietl_1_1vectorspace_1ad9f5da50a802270619afa459e6019c19) 

#### `typedef `[`size_type`](#d7/d6c/classietl_1_1vectorspace_1abeac0770949b15460f3a0724aedb3705) 

# class `ietl::wrapper_vectorspace` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`wrapper_vectorspace`](#d9/de5/classietl_1_1wrapper__vectorspace_1af01ae1fdf457a5277c4004646f28e7ed)`(size_type n)` | 
`public inline size_type `[`vec_dimension`](#d9/de5/classietl_1_1wrapper__vectorspace_1a689195a54f50576e29135d5100fdb3fc)`() const` | 
`public inline `[`vector_type`](#d0/dba/classietl_1_1vector__wrapper)` `[`new_vector`](#d9/de5/classietl_1_1wrapper__vectorspace_1a6930e289d14ed8f8e60e0ccc1436fbf0)`() const` | 
`public inline void `[`project`](#d9/de5/classietl_1_1wrapper__vectorspace_1a615b06b6372ae6f7331d5d7fc40e32c2)`(`[`vector_type`](#d0/dba/classietl_1_1vector__wrapper)` & src) const` | 
`typedef `[`vector_type`](#d9/de5/classietl_1_1wrapper__vectorspace_1a620704dac9492d1f8c114adece6998c4) | 
`typedef `[`scalar_type`](#d9/de5/classietl_1_1wrapper__vectorspace_1a5b19c7c058455c68e51a91d9d1ba3189) | 
`typedef `[`size_type`](#d9/de5/classietl_1_1wrapper__vectorspace_1ad3d89e099195cd968047f406756cd883) | 

## Members

#### `public inline  `[`wrapper_vectorspace`](#d9/de5/classietl_1_1wrapper__vectorspace_1af01ae1fdf457a5277c4004646f28e7ed)`(size_type n)` 

#### `public inline size_type `[`vec_dimension`](#d9/de5/classietl_1_1wrapper__vectorspace_1a689195a54f50576e29135d5100fdb3fc)`() const` 

#### `public inline `[`vector_type`](#d0/dba/classietl_1_1vector__wrapper)` `[`new_vector`](#d9/de5/classietl_1_1wrapper__vectorspace_1a6930e289d14ed8f8e60e0ccc1436fbf0)`() const` 

#### `public inline void `[`project`](#d9/de5/classietl_1_1wrapper__vectorspace_1a615b06b6372ae6f7331d5d7fc40e32c2)`(`[`vector_type`](#d0/dba/classietl_1_1vector__wrapper)` & src) const` 

#### `typedef `[`vector_type`](#d9/de5/classietl_1_1wrapper__vectorspace_1a620704dac9492d1f8c114adece6998c4) 

#### `typedef `[`scalar_type`](#d9/de5/classietl_1_1wrapper__vectorspace_1a5b19c7c058455c68e51a91d9d1ba3189) 

#### `typedef `[`size_type`](#d9/de5/classietl_1_1wrapper__vectorspace_1ad3d89e099195cd968047f406756cd883) 

# struct `ietl::number_traits` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`magnitude_type`](#db/d49/structietl_1_1number__traits_1a69981e5399baba34647d37b05fc92c47) | 

## Members

#### `typedef `[`magnitude_type`](#db/d49/structietl_1_1number__traits_1a69981e5399baba34647d37b05fc92c47) 

# struct `ietl::number_traits< std::complex< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`magnitude_type`](#df/dd2/structietl_1_1number__traits_3_01std_1_1complex_3_01_t_01_4_01_4_1a8a157ad465dc367fa7ece582335194ac) | 

## Members

#### `typedef `[`magnitude_type`](#df/dd2/structietl_1_1number__traits_3_01std_1_1complex_3_01_t_01_4_01_4_1a8a157ad465dc367fa7ece582335194ac) 

# struct `ietl::real_type` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#d0/d22/structietl_1_1real__type_1aa8ec842628338ea192053c963e0236e8) | 

## Members

#### `typedef `[`type`](#d0/d22/structietl_1_1real__type_1aa8ec842628338ea192053c963e0236e8) 

# struct `ietl::real_type< std::complex< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#dc/d51/structietl_1_1real__type_3_01std_1_1complex_3_01_t_01_4_01_4_1adfb98528385b68acafd42d855cac1d34) | 

## Members

#### `typedef `[`type`](#dc/d51/structietl_1_1real__type_3_01std_1_1complex_3_01_t_01_4_01_4_1adfb98528385b68acafd42d855cac1d34) 

# struct `ietl::vectorspace_traits` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`vector_type`](#d4/d26/structietl_1_1vectorspace__traits_1aff63d6b2b67c5e2d87c07b726477d559) | 
`typedef `[`size_type`](#d4/d26/structietl_1_1vectorspace__traits_1afeb035edbe7ca7815025708870d17977) | 
`typedef `[`scalar_type`](#d4/d26/structietl_1_1vectorspace__traits_1a25005ff64fd04bd64b353ffccb8f9951) | 
`typedef `[`magnitude_type`](#d4/d26/structietl_1_1vectorspace__traits_1a78a708628bb0186e73a2a70a7cb59e45) | 

## Members

#### `typedef `[`vector_type`](#d4/d26/structietl_1_1vectorspace__traits_1aff63d6b2b67c5e2d87c07b726477d559) 

#### `typedef `[`size_type`](#d4/d26/structietl_1_1vectorspace__traits_1afeb035edbe7ca7815025708870d17977) 

#### `typedef `[`scalar_type`](#d4/d26/structietl_1_1vectorspace__traits_1a25005ff64fd04bd64b353ffccb8f9951) 

#### `typedef `[`magnitude_type`](#d4/d26/structietl_1_1vectorspace__traits_1a78a708628bb0186e73a2a70a7cb59e45) 

# namespace `ietl2lapack` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>`fortran_int_t `[`stev`](#de/de9/ietl2lapack_8h_1aac6c63ace381bd21ec47888428ffc397)`(const Vector & alpha,const Vector & beta,Vector & eval,fortran_int_t n)`            | 
`public template<>`  <br/>`int `[`stev`](#de/de9/ietl2lapack_8h_1a093a8e0a1c4a34da5572c15477434777)`(const Vector & alpha,const Vector & beta,Vector & eval,FortranMatrix & z,fortran_int_t n)`            | 

## Members

#### `public template<>`  <br/>`fortran_int_t `[`stev`](#de/de9/ietl2lapack_8h_1aac6c63ace381bd21ec47888428ffc397)`(const Vector & alpha,const Vector & beta,Vector & eval,fortran_int_t n)` 

#### `public template<>`  <br/>`int `[`stev`](#de/de9/ietl2lapack_8h_1a093a8e0a1c4a34da5572c15477434777)`(const Vector & alpha,const Vector & beta,Vector & eval,FortranMatrix & z,fortran_int_t n)` 

# namespace `ietl::detail` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>`void `[`GeneratePlaneRotation`](#d5/d0d/gmres_8h_1a482a0a54abd55e1fc9ecd9d8d4004046)`(T dx,T dy,T & cs,T & sn)`            | 
`public template<>`  <br/>`void `[`ApplyPlaneRotation`](#d5/d0d/gmres_8h_1a58277a8e188ef4ca1e202d7ab202c243)`(T & dx,T & dy,T cs,T sn)`            | 
`public template<>`  <br/>`std::vector< T > `[`Update`](#d5/d0d/gmres_8h_1af61d91807f405339d446baf2c3d0a7d6)`(boost::numeric::ublas::matrix< T > const & H,std::vector< T > const & S,std::size_t k)`            | 
`public template<>`  <br/>`void `[`mult`](#d6/dd6/jd_8h_1a604a08231c2fd0a978f58cbef2116df6)`(const `[`deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix)`< MATRIX, VS > & Adef,const VECTOR & v,VECTOR & r)`            | 
`public template<>`  <br/>`void `[`mult`](#d6/dd6/jd_8h_1a1fdc571a9b99d12f8e2368c16addcdeb)`(std::vector< VECTOR > & vecset,const MATRIX & mat)`            | 
`public template<>`  <br/>`void `[`mult`](#d6/dd6/jd_8h_1a1752a2153933aac73ce65624c3db7927)`(std::vector< ublas::vector< T > > & vecset,const MATRIX & mat)`            | 
`public inline bool `[`cmp`](#d6/d6c/simple__arnoldi_8h_1ae95b5c8d5733a027d33daaf58c3363e6)`(std::complex< double > a,std::complex< double > b)`            | 
`public inline std::complex< double > `[`make_complex`](#d6/d6c/simple__arnoldi_8h_1a491a1a4a66c90b0cc7bf5328628ff7fa)`(double re,double im)`            | 
`public template<>`  <br/>`void `[`arnoldi_geev`](#d6/d6c/simple__arnoldi_8h_1ac33d1fddf3528b4cda91c234f7a72da1)`(MatrixT & mtx,std::vector< std::complex< double > > & evals,MatrixT & evecs,double)`            | 
`public template<>`  <br/>`void `[`arnoldi_geev`](#d6/d6c/simple__arnoldi_8h_1abf117d8cf26c83ca22cfca16713f8399)`(MatrixT & mtx,std::vector< std::complex< double > > & evals,MatrixT & evecs,std::complex< double >)`            | 
`class `[`ietl::detail::deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix) | 

## Members

#### `public template<>`  <br/>`void `[`GeneratePlaneRotation`](#d5/d0d/gmres_8h_1a482a0a54abd55e1fc9ecd9d8d4004046)`(T dx,T dy,T & cs,T & sn)` 

#### `public template<>`  <br/>`void `[`ApplyPlaneRotation`](#d5/d0d/gmres_8h_1a58277a8e188ef4ca1e202d7ab202c243)`(T & dx,T & dy,T cs,T sn)` 

#### `public template<>`  <br/>`std::vector< T > `[`Update`](#d5/d0d/gmres_8h_1af61d91807f405339d446baf2c3d0a7d6)`(boost::numeric::ublas::matrix< T > const & H,std::vector< T > const & S,std::size_t k)` 

#### `public template<>`  <br/>`void `[`mult`](#d6/dd6/jd_8h_1a604a08231c2fd0a978f58cbef2116df6)`(const `[`deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix)`< MATRIX, VS > & Adef,const VECTOR & v,VECTOR & r)` 

#### `public template<>`  <br/>`void `[`mult`](#d6/dd6/jd_8h_1a1fdc571a9b99d12f8e2368c16addcdeb)`(std::vector< VECTOR > & vecset,const MATRIX & mat)` 

#### `public template<>`  <br/>`void `[`mult`](#d6/dd6/jd_8h_1a1752a2153933aac73ce65624c3db7927)`(std::vector< ublas::vector< T > > & vecset,const MATRIX & mat)` 

#### `public inline bool `[`cmp`](#d6/d6c/simple__arnoldi_8h_1ae95b5c8d5733a027d33daaf58c3363e6)`(std::complex< double > a,std::complex< double > b)` 

#### `public inline std::complex< double > `[`make_complex`](#d6/d6c/simple__arnoldi_8h_1a491a1a4a66c90b0cc7bf5328628ff7fa)`(double re,double im)` 

#### `public template<>`  <br/>`void `[`arnoldi_geev`](#d6/d6c/simple__arnoldi_8h_1ac33d1fddf3528b4cda91c234f7a72da1)`(MatrixT & mtx,std::vector< std::complex< double > > & evals,MatrixT & evecs,double)` 

#### `public template<>`  <br/>`void `[`arnoldi_geev`](#d6/d6c/simple__arnoldi_8h_1abf117d8cf26c83ca22cfca16713f8399)`(MatrixT & mtx,std::vector< std::complex< double > > & evals,MatrixT & evecs,std::complex< double >)` 

# class `ietl::detail::deflated_matrix` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1ad390227f2b67f55d7fd15e225d1b7f8b)`(const MATRIX & A,double theta,const std::vector< vector_type > & Q)` | 
`public inline  `[`~deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1a756b02969c1757666d1fe9c13ba87902)`()` | 
`public inline void `[`set_theta`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1a4c77f4be9861f0e33c13ec89e1c026c9)`(real_type theta)` | 
`typedef `[`vector_type`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1ac5a6e7204cbde81b1a85ce28e414fc0f) | 
`typedef `[`scalar_type`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1a7ade10b66d78aa7f918276fcd751fd05) | 
`typedef `[`real_type`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1a80aa3c758281f8ec439e89eac5e7e29c) | 

## Members

#### `public inline  `[`deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1ad390227f2b67f55d7fd15e225d1b7f8b)`(const MATRIX & A,double theta,const std::vector< vector_type > & Q)` 

#### `public inline  `[`~deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1a756b02969c1757666d1fe9c13ba87902)`()` 

#### `public inline void `[`set_theta`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1a4c77f4be9861f0e33c13ec89e1c026c9)`(real_type theta)` 

#### `typedef `[`vector_type`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1ac5a6e7204cbde81b1a85ce28e414fc0f) 

#### `typedef `[`scalar_type`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1a7ade10b66d78aa7f918276fcd751fd05) 

#### `typedef `[`real_type`](#d1/de1/classietl_1_1detail_1_1deflated__matrix_1a80aa3c758281f8ec439e89eac5e7e29c) 

# namespace `ietl::solver` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>`void `[`mult`](#d6/dd6/jd_8h_1aaf2f3f68ae1843b4a2e7128a647fbfdb)`(const `[`left_prec_solver`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver)`< SOLV, MATRIX, VS, PREC > &,const VECTOR &,VECTOR &)`            | 
`class `[`ietl::solver::jd_solver`](#dd/d95/classietl_1_1solver_1_1jd__solver) | 
`class `[`ietl::solver::left_prec_solver`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver) | 

## Members

#### `public template<>`  <br/>`void `[`mult`](#d6/dd6/jd_8h_1aaf2f3f68ae1843b4a2e7128a647fbfdb)`(const `[`left_prec_solver`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver)`< SOLV, MATRIX, VS, PREC > &,const VECTOR &,VECTOR &)` 

# class `ietl::solver::jd_solver` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`jd_solver`](#dd/d95/classietl_1_1solver_1_1jd__solver_1ad1faed3d07e5409224ad4a8daf102a4f)`(SOLV & s,const MATRIX & A,const std::vector< vector_type > & Q,const VS & vspace)` | 
`public template<>`  <br/>`void `[`operator()`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a2009e4476425646d3ca7a2320e87f692)`(real_type theta,vector_type & r,vector_type & t,IT & iter)` | 
`protected `[`detail::deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix)`< MATRIX, VS > `[`Adef_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1ae4ad0c661fd36e1e5b788a65de14ddf2) | 
`protected const VS & `[`vspace_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1adf7c0228ca02379c4fb6889d85ccf613) | 
`protected vector_type `[`x0_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a08838feb5cb893fcaf26d37cc5c685ee) | 
`protected const std::vector< vector_type > & `[`Q_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a9e38bf437fe8526f424e6e0f7aff4f6c) | 
`protected SOLV & `[`solv_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a393d288eafe8ec0cc47abf519e5c2aa4) | 
`typedef `[`vector_type`](#dd/d95/classietl_1_1solver_1_1jd__solver_1acc2b5435604813a87280dfd167e4f647) | 
`typedef `[`scalar_type`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a98df378791a20e0ef1d8c9e46df9d314) | 
`typedef `[`real_type`](#dd/d95/classietl_1_1solver_1_1jd__solver_1af3dfdd4967f22a8b52be1685a80e3864) | 

## Members

#### `public inline  `[`jd_solver`](#dd/d95/classietl_1_1solver_1_1jd__solver_1ad1faed3d07e5409224ad4a8daf102a4f)`(SOLV & s,const MATRIX & A,const std::vector< vector_type > & Q,const VS & vspace)` 

#### `public template<>`  <br/>`void `[`operator()`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a2009e4476425646d3ca7a2320e87f692)`(real_type theta,vector_type & r,vector_type & t,IT & iter)` 

#### `protected `[`detail::deflated_matrix`](#d1/de1/classietl_1_1detail_1_1deflated__matrix)`< MATRIX, VS > `[`Adef_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1ae4ad0c661fd36e1e5b788a65de14ddf2) 

#### `protected const VS & `[`vspace_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1adf7c0228ca02379c4fb6889d85ccf613) 

#### `protected vector_type `[`x0_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a08838feb5cb893fcaf26d37cc5c685ee) 

#### `protected const std::vector< vector_type > & `[`Q_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a9e38bf437fe8526f424e6e0f7aff4f6c) 

#### `protected SOLV & `[`solv_`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a393d288eafe8ec0cc47abf519e5c2aa4) 

#### `typedef `[`vector_type`](#dd/d95/classietl_1_1solver_1_1jd__solver_1acc2b5435604813a87280dfd167e4f647) 

#### `typedef `[`scalar_type`](#dd/d95/classietl_1_1solver_1_1jd__solver_1a98df378791a20e0ef1d8c9e46df9d314) 

#### `typedef `[`real_type`](#dd/d95/classietl_1_1solver_1_1jd__solver_1af3dfdd4967f22a8b52be1685a80e3864) 

# class `ietl::solver::left_prec_solver` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`left_prec_solver`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a9182e36a7b7d32a12e048c018346171d)`(SOLV & s,const MATRIX & A,const std::vector< vector_type > & Q,const VS & vs,PREC & K)` | 
`public template<>`  <br/>`void `[`operator()`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1afd095a78ca7e6e0bbb71a4efb249e71d)`(real_type theta,vector_type & r,vector_type & t,IT & iter)` | 
`protected SOLV & `[`solv_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a0ad15e3ecc5d9046a055d39b9447441f) | 
`protected const MATRIX & `[`A_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1ae91633b83cf18926b72be7594af3c126) | 
`protected const std::vector< vector_type > & `[`Q_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1ad5e74c38b0083aed4dfdbc5d426fe5ba) | 
`protected const VS & `[`vspace_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1ab0e5e5fe9ca5554cf7bbf30b19f3d1f4) | 
`protected std::vector< vector_type > `[`Q_hat_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a1ad5dd9916d78752bbac732afe47297f) | 
`protected PREC & `[`K_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a0ae9d00d2f84d4185b792843b106fae9) | 
`protected vector_type `[`x0_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a5122ba9acf9fc612e75db921a93740b7) | 
`protected real_type `[`theta_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a5dd3af52fc81b02ac3316ce9ffbf765b) | 
`protected mutable ublas::vector< scalar_type > `[`gamma_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a982d9121dce24d0c2f176243606b17a7) | 
`protected std::vector< fortran_int_t > `[`pivot_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1ad140b42c2e361985dfaa6de3df9f23db) | 
`protected matrix_type `[`LU_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a5794a73e5fd6bf6eb8b805f859d5a405) | 
`protected matrix_type `[`M_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1afb8f1a416493d6963b148571f55c62bf) | 
`typedef `[`vector_type`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a000e4011b21f290658e00bcb99d2fb50) | 
`typedef `[`scalar_type`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a1a77f414af24bac616019fb6901440ca) | 
`typedef `[`real_type`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a9bd881b2b576a42a521a5b29b4e161b0) | 
`typedef `[`matrix_type`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a09cd9b99e600077795cf23dfe09f06be) | 

## Members

#### `public inline  `[`left_prec_solver`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a9182e36a7b7d32a12e048c018346171d)`(SOLV & s,const MATRIX & A,const std::vector< vector_type > & Q,const VS & vs,PREC & K)` 

#### `public template<>`  <br/>`void `[`operator()`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1afd095a78ca7e6e0bbb71a4efb249e71d)`(real_type theta,vector_type & r,vector_type & t,IT & iter)` 

#### `protected SOLV & `[`solv_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a0ad15e3ecc5d9046a055d39b9447441f) 

#### `protected const MATRIX & `[`A_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1ae91633b83cf18926b72be7594af3c126) 

#### `protected const std::vector< vector_type > & `[`Q_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1ad5e74c38b0083aed4dfdbc5d426fe5ba) 

#### `protected const VS & `[`vspace_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1ab0e5e5fe9ca5554cf7bbf30b19f3d1f4) 

#### `protected std::vector< vector_type > `[`Q_hat_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a1ad5dd9916d78752bbac732afe47297f) 

#### `protected PREC & `[`K_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a0ae9d00d2f84d4185b792843b106fae9) 

#### `protected vector_type `[`x0_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a5122ba9acf9fc612e75db921a93740b7) 

#### `protected real_type `[`theta_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a5dd3af52fc81b02ac3316ce9ffbf765b) 

#### `protected mutable ublas::vector< scalar_type > `[`gamma_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a982d9121dce24d0c2f176243606b17a7) 

#### `protected std::vector< fortran_int_t > `[`pivot_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1ad140b42c2e361985dfaa6de3df9f23db) 

#### `protected matrix_type `[`LU_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a5794a73e5fd6bf6eb8b805f859d5a405) 

#### `protected matrix_type `[`M_`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1afb8f1a416493d6963b148571f55c62bf) 

#### `typedef `[`vector_type`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a000e4011b21f290658e00bcb99d2fb50) 

#### `typedef `[`scalar_type`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a1a77f414af24bac616019fb6901440ca) 

#### `typedef `[`real_type`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a9bd881b2b576a42a521a5b29b4e161b0) 

#### `typedef `[`matrix_type`](#d6/d8e/classietl_1_1solver_1_1left__prec__solver_1a09cd9b99e600077795cf23dfe09f06be) 

# namespace `ietl_lapack_dispatch` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline void `[`stev`](#de/de9/ietl2lapack_8h_1a9ef8ad5d3fb941c3d9e2a54419936362)`(const char & jobz,fortran_int_t n,double dd,double de,double dz,fortran_int_t ldz,fortran_int_t info)`            | 
`public inline void `[`stev`](#de/de9/ietl2lapack_8h_1a90fb67acb0f95f4e38de468c084dfcf0)`(const char & jobz,fortran_int_t n,double dd,double de,std::complex< double > dz,fortran_int_t ldz,fortran_int_t info)`            | 

## Members

#### `public inline void `[`stev`](#de/de9/ietl2lapack_8h_1a9ef8ad5d3fb941c3d9e2a54419936362)`(const char & jobz,fortran_int_t n,double dd,double de,double dz,fortran_int_t ldz,fortran_int_t info)` 

#### `public inline void `[`stev`](#de/de9/ietl2lapack_8h_1a90fb67acb0f95f4e38de468c084dfcf0)`(const char & jobz,fortran_int_t n,double dd,double de,std::complex< double > dz,fortran_int_t ldz,fortran_int_t info)` 

Generated by [Moxygen](https://sourcey.com/moxygen)
