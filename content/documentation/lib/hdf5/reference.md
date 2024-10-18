
---
title: Reference
description: "ALPS hdf5 Library"
weight: 3
---

# Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`namespace `[`alps`](#d8/d3d/namespacealps) | 
`namespace `[`alps::hdf5`](#dd/d35/namespacealps_1_1hdf5) | 
`namespace `[`alps::hdf5::detail`](#d3/d2b/namespacealps_1_1hdf5_1_1detail) | 

# namespace `alps` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>`boost::disable_if< typenameboost::mpl::and_< typenameboost::is_same< typenamealps::detail::remove_cvr< typenameboost::remove_all_extents< T >::type >::type, char >::type, typenameboost::is_array< T >::type >::type, `[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T & > >::type `[`make_pvp`](#d9/d50/archive_8hpp_1ab54847109d6768220ad4367001caebfe)`(std::string const & path,T & value)`            | 
`public template<>`  <br/>`boost::disable_if< typenameboost::mpl::and_< typenameboost::is_same< typenamealps::detail::remove_cvr< typenameboost::remove_all_extents< T >::type >::type, char >::type, typenameboost::is_array< T >::type >::type, `[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< Tconst & > >::type `[`make_pvp`](#d9/d50/archive_8hpp_1a37c644928d3b76d1d71a653a68120ef8)`(std::string const & path,T const & value)`            | 
`public template<>`  <br/>`boost::enable_if< typenameboost::mpl::and_< typenameboost::is_same< typenamealps::detail::remove_cvr< typenameboost::remove_all_extents< T >::type >::type, char >::type, typenameboost::is_array< T >::type >::type, `[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< std::stringconst > >::type `[`make_pvp`](#d9/d50/archive_8hpp_1abb5b314a27f828e9c352eda8843eb097)`(std::string const & path,T const & value)`            | 
`public template<>`  <br/>[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< std::pair< T *, std::vector< std::size_t > > > `[`make_pvp`](#d2/d17/pointer_8hpp_1a462cdea6fd429e957abd922c5469fd91)`(std::string const & path,T * value,std::size_t size)`            | 
`public template<>`  <br/>[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< std::pair< T *, std::vector< std::size_t > > > `[`make_pvp`](#d2/d17/pointer_8hpp_1a6e7a772e387784c369eadf57018a6b23)`(std::string const & path,T * value,std::vector< std::size_t > const & size)`            | 

## Members

#### `public template<>`  <br/>`boost::disable_if< typenameboost::mpl::and_< typenameboost::is_same< typenamealps::detail::remove_cvr< typenameboost::remove_all_extents< T >::type >::type, char >::type, typenameboost::is_array< T >::type >::type, `[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T & > >::type `[`make_pvp`](#d9/d50/archive_8hpp_1ab54847109d6768220ad4367001caebfe)`(std::string const & path,T & value)` 

#### `public template<>`  <br/>`boost::disable_if< typenameboost::mpl::and_< typenameboost::is_same< typenamealps::detail::remove_cvr< typenameboost::remove_all_extents< T >::type >::type, char >::type, typenameboost::is_array< T >::type >::type, `[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< Tconst & > >::type `[`make_pvp`](#d9/d50/archive_8hpp_1a37c644928d3b76d1d71a653a68120ef8)`(std::string const & path,T const & value)` 

#### `public template<>`  <br/>`boost::enable_if< typenameboost::mpl::and_< typenameboost::is_same< typenamealps::detail::remove_cvr< typenameboost::remove_all_extents< T >::type >::type, char >::type, typenameboost::is_array< T >::type >::type, `[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< std::stringconst > >::type `[`make_pvp`](#d9/d50/archive_8hpp_1abb5b314a27f828e9c352eda8843eb097)`(std::string const & path,T const & value)` 

#### `public template<>`  <br/>[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< std::pair< T *, std::vector< std::size_t > > > `[`make_pvp`](#d2/d17/pointer_8hpp_1a462cdea6fd429e957abd922c5469fd91)`(std::string const & path,T * value,std::size_t size)` 

#### `public template<>`  <br/>[`hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< std::pair< T *, std::vector< std::size_t > > > `[`make_pvp`](#d2/d17/pointer_8hpp_1a6e7a772e387784c369eadf57018a6b23)`(std::string const & path,T * value,std::vector< std::size_t > const & size)` 

# namespace `alps::hdf5` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>[`scalar_type`](#d1/dbd/structalps_1_1hdf5_1_1scalar__type)`< T >::type * `[`get_pointer`](#d9/d50/archive_8hpp_1acdbe20e090fbbdfbd8aaca2c12ca5ac3)`(T & value)`            | 
`public template<>`  <br/>[`scalar_type`](#d1/dbd/structalps_1_1hdf5_1_1scalar__type)`< T >::type const * `[`get_pointer`](#d9/d50/archive_8hpp_1a1df8fe4743971154b0b9ab3448b2e938)`(T const & value)`            | 
`public template<>`  <br/>`std::vector< std::size_t > `[`get_extent`](#d9/d50/archive_8hpp_1afba1df8d93efd6f4936a40d416a5d14a)`(T const & value)`            | 
`public template<>`  <br/>`void `[`set_extent`](#d9/d50/archive_8hpp_1a3857d31879eef3d15e4a68fe8413a17c)`(T & value,std::vector< std::size_t > const & size)`            | 
`public template<>`  <br/>`bool `[`is_vectorizable`](#d9/d50/archive_8hpp_1a3a5d04c5e5270d9fd933fa593753846a)`(T const & value)`            | 
`public template<>`  <br/>`void `[`save`](#d9/d50/archive_8hpp_1a7601fd066529b2db77d3be662c973c19)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,T const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#d9/d50/archive_8hpp_1a4b580a9a346f143ef99ebf825d9ba9ec)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,T & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`boost::enable_if< `[`has_complex_elements](#d7/d10/structalps_1_1hdf5_1_1has__complex__elements)< typenamealps::detail::remove_cvr< T >::type >, [archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & >::type `[`operator<<`](#d9/d50/archive_8hpp_1ad3b8d87bb62f1ccaa6879764a4fdec88)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,`[`detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T > const & proxy)`            | 
`public template<>`  <br/>`boost::disable_if< `[`has_complex_elements](#d7/d10/structalps_1_1hdf5_1_1has__complex__elements)< typenamealps::detail::remove_cvr< T >::type >, [archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & >::type `[`operator<<`](#d9/d50/archive_8hpp_1afc2ebe85ba4d113f1f4c44ae3c9a78e2)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,`[`detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T > const & proxy)`            | 
`public template<>`  <br/>[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & `[`operator>>`](#d9/d50/archive_8hpp_1a9e1e13ef5366369c139580907b3bbb39)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,`[`detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T > proxy)`            | 
`public template<>`  <br/>`void `[`save`](#d4/db5/array_8hpp_1acbfe54cfd47d6ed999a534bf54bcf3ea)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::array< T, N > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#d4/db5/array_8hpp_1adc03336cebc115fa00a165c914e94381)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::array< T, N > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#db/dd8/complex_8hpp_1ae09776bd99ac0eb67a1ade76a431e254)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::complex< T > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#db/dd8/complex_8hpp_1a0f237d5e1e089f69d5bf846436266b83)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::complex< T > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#df/d7c/map_8hpp_1a038d96be8e5512ac904c708ba87c572a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::map< K, T, C, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#df/d7c/map_8hpp_1a9c8760befbc6725bbb49471511d700b9)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::map< K, T, C, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#df/dce/matrix_8hpp_1a27ce514c439fdd2493e10add285ab04a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::numeric::matrix< T, MemoryBlock > const & m,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#df/dce/matrix_8hpp_1a69ca11a39412c6b0d5ca979656dfac51)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::numeric::matrix< T, MemoryBlock > & m,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#d1/d8a/multi__array_8hpp_1ae4bcdeadb20011392670a727267c5780)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::multi_array< T, N, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#d1/d8a/multi__array_8hpp_1a851af7368b7dcbfa6b9f20dd63d7c6d9)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::multi_array< T, N, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#d1/d8a/multi__array_8hpp_1aff28530a75c2bea6461358d6289f528a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::multi_array< T, N, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#d1/d8a/multi__array_8hpp_1a5dbe942472db20a9486de8d3b5cc2a73)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::multi_array< T, N, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#de/d3d/numeric__vector_8hpp_1a17e26f5df7d3ce60d8f180785436a107)`(`[`alps::hdf5::archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::numeric::vector< T, MemoryBlock > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#de/d3d/numeric__vector_8hpp_1a0f8577ef919a7b21f25c4bba760f0875)`(`[`alps::hdf5::archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::numeric::vector< T, MemoryBlock > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#d3/d9f/pair_8hpp_1a2c5318079392afeef0ab75c3c4ab1ad1)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::pair< T, U > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#d3/d9f/pair_8hpp_1a623b639b1838ac8eda1c81288e95f8d6)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::pair< T, U > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#d3/d9f/pair_8hpp_1a1afb73297cb0c639efa3fafd669704b9)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::pair< T *, std::vector< std::size_t > > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#d3/d9f/pair_8hpp_1a2816fb8c3490b6dd82af6a85976a82cc)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::pair< T *, std::vector< std::size_t > > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save_generic`](#de/db2/python_8cpp_1a17f54861077d10988473e73cb51fb582)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,T const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`save`](#de/db2/python_8cpp_1ac4011bd79e7f8c383946f3107b8fc310)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::list const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`save`](#de/db2/python_8cpp_1a6b38dc3ed378de5534934d5e35173b49)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::tuple const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`load`](#de/db2/python_8cpp_1ab5691bad68403c19f4743cec391c0cc4)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::list & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`save`](#de/db2/python_8cpp_1a0e66fc4a43d8fbceec6592c6ea7d32fc)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::python::numpy::array const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`load`](#de/db2/python_8cpp_1a109cc2902676d54b3dc5eb85a96b8ff6)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::python::numpy::array & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`save`](#de/db2/python_8cpp_1a6326ba75ab7ecf932359e4a1752ae0c1)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::dict const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`load`](#de/db2/python_8cpp_1a060af7d6af982340722e479e1582ee8a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::dict & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`save`](#de/db2/python_8cpp_1a71cde744dd594f8fbda35d053902d190)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::object const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public void `[`load`](#de/db2/python_8cpp_1ace4017eb14295029b7fc1563115125cd)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::object & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#d7/d85/stdarray_8hpp_1ab39cb461f108d449d722bc5658ca3989)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::array< T, N > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#d7/d85/stdarray_8hpp_1ac17a21e73eeac5b8b9d658b44d41887a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::array< T, N > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#d3/d6f/tuple_8hpp_1a4ea0dec0c4c336046280b70333c93256)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::tuple< T0, T1, T2, T3, T4, T5, T6, T7, T8, T9 > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#d3/d6f/tuple_8hpp_1aec7c169181ce47900e6856b2aafe4af9)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::tuple< T0, T1, T2, T3, T4, T5, T6, T7, T8, T9 > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#dc/d69/valarray_8hpp_1a25cea4a2b59c8d5ce1ab1f1c38145cdf)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::valarray< T > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#dc/d69/valarray_8hpp_1a6b1ec38b99161516bc19d40663d783e3)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::valarray< T > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#da/d16/vector_8hpp_1a0652e8d3e0f66b0b30e25ea12b89f921)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< T, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`save`](#da/d16/vector_8hpp_1a5615700c36427d45e14249b6bea943fd)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< bool, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#da/d16/vector_8hpp_1a92769e57872c9da4bb7b2cd44d14cb9b)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< T, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`public template<>`  <br/>`void `[`load`](#da/d16/vector_8hpp_1a0981a3efcda7340c13e5f2b675adea6e)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< bool, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)`            | 
`class `[`alps::hdf5::archive`](#df/d24/classalps_1_1hdf5_1_1archive) | 
`class `[`alps::hdf5::archive_error`](#df/d8a/classalps_1_1hdf5_1_1archive__error) | 
`struct `[`alps::hdf5::has_complex_elements`](#d7/d10/structalps_1_1hdf5_1_1has__complex__elements) | 
`struct `[`alps::hdf5::has_complex_elements< alps::multi_array< T, N, A > >`](#dc/d8e/structalps_1_1hdf5_1_1has__complex__elements_3_01alps_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::has_complex_elements< alps::numeric::matrix< T, MemoryBlock > >`](#d4/d6c/structalps_1_1hdf5_1_1has__complex__elements_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01_4) | 
`struct `[`alps::hdf5::has_complex_elements< boost::array< T, N > >`](#d6/d1a/structalps_1_1hdf5_1_1has__complex__elements_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::has_complex_elements< boost::multi_array< T, N, A > >`](#d5/de1/structalps_1_1hdf5_1_1has__complex__elements_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::has_complex_elements< std::array< T, N > >`](#df/d18/structalps_1_1hdf5_1_1has__complex__elements_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::has_complex_elements< std::complex< T > >`](#d2/de5/structalps_1_1hdf5_1_1has__complex__elements_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::has_complex_elements< std::pair< T *, std::vector< std::size_t > > >`](#d2/dd9/structalps_1_1hdf5_1_1has__complex__elements_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_01std_1_1size__t_01_4_01_4_01_4) | 
`struct `[`alps::hdf5::has_complex_elements< std::valarray< T > >`](#d2/d46/structalps_1_1hdf5_1_1has__complex__elements_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::has_complex_elements< std::vector< T, A > >`](#d4/dde/structalps_1_1hdf5_1_1has__complex__elements_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::is_content_continuous`](#d2/d28/structalps_1_1hdf5_1_1is__content__continuous) | 
`struct `[`alps::hdf5::is_content_continuous< alps::multi_array< T, N, A > >`](#d3/d83/structalps_1_1hdf5_1_1is__content__continuous_3_01alps_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::is_content_continuous< std::pair< T *, std::vector< std::size_t > > >`](#df/d2e/structalps_1_1hdf5_1_1is__content__continuous_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_01std_1_1size__t_01_4_01_4_01_4) | 
`struct `[`alps::hdf5::is_content_continuous< std::valarray< T > >`](#d9/db8/structalps_1_1hdf5_1_1is__content__continuous_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::is_content_continuous< std::vector< bool, A > >`](#d2/d4f/structalps_1_1hdf5_1_1is__content__continuous_3_01std_1_1vector_3_01bool_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::is_content_continuous< std::vector< T, A > >`](#df/d46/structalps_1_1hdf5_1_1is__content__continuous_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::is_continuous`](#d6/d2d/structalps_1_1hdf5_1_1is__continuous) | 
`struct `[`alps::hdf5::is_continuous< boost::array< T, N > >`](#d6/da8/structalps_1_1hdf5_1_1is__continuous_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::is_continuous< boost::array< T, N > const >`](#d7/df9/structalps_1_1hdf5_1_1is__continuous_3_01boost_1_1array_3_01_t_00_01_n_01_4_01const_01_4) | 
`struct `[`alps::hdf5::is_continuous< std::array< T, N > >`](#d9/db8/structalps_1_1hdf5_1_1is__continuous_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::is_continuous< std::array< T, N > const >`](#d0/d0f/structalps_1_1hdf5_1_1is__continuous_3_01std_1_1array_3_01_t_00_01_n_01_4_01const_01_4) | 
`struct `[`alps::hdf5::is_continuous< std::complex< T > >`](#d9/ddc/structalps_1_1hdf5_1_1is__continuous_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::is_continuous< std::complex< T > const >`](#d1/d10/structalps_1_1hdf5_1_1is__continuous_3_01std_1_1complex_3_01_t_01_4_01const_01_4) | 
`struct `[`alps::hdf5::scalar_type`](#d1/dbd/structalps_1_1hdf5_1_1scalar__type) | 
`struct `[`alps::hdf5::scalar_type< alps::multi_array< T, N, A > >`](#d3/dff/structalps_1_1hdf5_1_1scalar__type_3_01alps_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::scalar_type< alps::numeric::matrix< T, MemoryBlock > >`](#df/d79/structalps_1_1hdf5_1_1scalar__type_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01_4) | 
`struct `[`alps::hdf5::scalar_type< boost::array< T, N > >`](#db/dca/structalps_1_1hdf5_1_1scalar__type_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::scalar_type< boost::multi_array< T, N, A > >`](#d7/d05/structalps_1_1hdf5_1_1scalar__type_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::scalar_type< std::array< T, N > >`](#dc/da8/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::scalar_type< std::complex< T > >`](#d7/d48/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::scalar_type< std::pair< T *, std::vector< std::size_t > > >`](#d6/d54/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_01std_1_1size__t_01_4_01_4_01_4) | 
`struct `[`alps::hdf5::scalar_type< std::valarray< T > >`](#de/d44/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::scalar_type< std::vector< T, A > >`](#de/d09/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4) | 

## Members

#### `public template<>`  <br/>[`scalar_type`](#d1/dbd/structalps_1_1hdf5_1_1scalar__type)`< T >::type * `[`get_pointer`](#d9/d50/archive_8hpp_1acdbe20e090fbbdfbd8aaca2c12ca5ac3)`(T & value)` 

#### `public template<>`  <br/>[`scalar_type`](#d1/dbd/structalps_1_1hdf5_1_1scalar__type)`< T >::type const * `[`get_pointer`](#d9/d50/archive_8hpp_1a1df8fe4743971154b0b9ab3448b2e938)`(T const & value)` 

#### `public template<>`  <br/>`std::vector< std::size_t > `[`get_extent`](#d9/d50/archive_8hpp_1afba1df8d93efd6f4936a40d416a5d14a)`(T const & value)` 

#### `public template<>`  <br/>`void `[`set_extent`](#d9/d50/archive_8hpp_1a3857d31879eef3d15e4a68fe8413a17c)`(T & value,std::vector< std::size_t > const & size)` 

#### `public template<>`  <br/>`bool `[`is_vectorizable`](#d9/d50/archive_8hpp_1a3a5d04c5e5270d9fd933fa593753846a)`(T const & value)` 

#### `public template<>`  <br/>`void `[`save`](#d9/d50/archive_8hpp_1a7601fd066529b2db77d3be662c973c19)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,T const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#d9/d50/archive_8hpp_1a4b580a9a346f143ef99ebf825d9ba9ec)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,T & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`boost::enable_if< `[`has_complex_elements](#d7/d10/structalps_1_1hdf5_1_1has__complex__elements)< typenamealps::detail::remove_cvr< T >::type >, [archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & >::type `[`operator<<`](#d9/d50/archive_8hpp_1ad3b8d87bb62f1ccaa6879764a4fdec88)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,`[`detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T > const & proxy)` 

#### `public template<>`  <br/>`boost::disable_if< `[`has_complex_elements](#d7/d10/structalps_1_1hdf5_1_1has__complex__elements)< typenamealps::detail::remove_cvr< T >::type >, [archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & >::type `[`operator<<`](#d9/d50/archive_8hpp_1afc2ebe85ba4d113f1f4c44ae3c9a78e2)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,`[`detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T > const & proxy)` 

#### `public template<>`  <br/>[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & `[`operator>>`](#d9/d50/archive_8hpp_1a9e1e13ef5366369c139580907b3bbb39)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,`[`detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T > proxy)` 

#### `public template<>`  <br/>`void `[`save`](#d4/db5/array_8hpp_1acbfe54cfd47d6ed999a534bf54bcf3ea)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::array< T, N > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#d4/db5/array_8hpp_1adc03336cebc115fa00a165c914e94381)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::array< T, N > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#db/dd8/complex_8hpp_1ae09776bd99ac0eb67a1ade76a431e254)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::complex< T > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#db/dd8/complex_8hpp_1a0f237d5e1e089f69d5bf846436266b83)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::complex< T > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#df/d7c/map_8hpp_1a038d96be8e5512ac904c708ba87c572a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::map< K, T, C, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#df/d7c/map_8hpp_1a9c8760befbc6725bbb49471511d700b9)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::map< K, T, C, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#df/dce/matrix_8hpp_1a27ce514c439fdd2493e10add285ab04a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::numeric::matrix< T, MemoryBlock > const & m,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#df/dce/matrix_8hpp_1a69ca11a39412c6b0d5ca979656dfac51)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::numeric::matrix< T, MemoryBlock > & m,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#d1/d8a/multi__array_8hpp_1ae4bcdeadb20011392670a727267c5780)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::multi_array< T, N, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#d1/d8a/multi__array_8hpp_1a851af7368b7dcbfa6b9f20dd63d7c6d9)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::multi_array< T, N, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#d1/d8a/multi__array_8hpp_1aff28530a75c2bea6461358d6289f528a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::multi_array< T, N, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#d1/d8a/multi__array_8hpp_1a5dbe942472db20a9486de8d3b5cc2a73)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::multi_array< T, N, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#de/d3d/numeric__vector_8hpp_1a17e26f5df7d3ce60d8f180785436a107)`(`[`alps::hdf5::archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::numeric::vector< T, MemoryBlock > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#de/d3d/numeric__vector_8hpp_1a0f8577ef919a7b21f25c4bba760f0875)`(`[`alps::hdf5::archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::numeric::vector< T, MemoryBlock > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#d3/d9f/pair_8hpp_1a2c5318079392afeef0ab75c3c4ab1ad1)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::pair< T, U > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#d3/d9f/pair_8hpp_1a623b639b1838ac8eda1c81288e95f8d6)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::pair< T, U > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#d3/d9f/pair_8hpp_1a1afb73297cb0c639efa3fafd669704b9)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::pair< T *, std::vector< std::size_t > > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#d3/d9f/pair_8hpp_1a2816fb8c3490b6dd82af6a85976a82cc)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::pair< T *, std::vector< std::size_t > > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save_generic`](#de/db2/python_8cpp_1a17f54861077d10988473e73cb51fb582)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,T const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`save`](#de/db2/python_8cpp_1ac4011bd79e7f8c383946f3107b8fc310)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::list const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`save`](#de/db2/python_8cpp_1a6b38dc3ed378de5534934d5e35173b49)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::tuple const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`load`](#de/db2/python_8cpp_1ab5691bad68403c19f4743cec391c0cc4)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::list & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`save`](#de/db2/python_8cpp_1a0e66fc4a43d8fbceec6592c6ea7d32fc)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::python::numpy::array const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`load`](#de/db2/python_8cpp_1a109cc2902676d54b3dc5eb85a96b8ff6)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::python::numpy::array & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`save`](#de/db2/python_8cpp_1a6326ba75ab7ecf932359e4a1752ae0c1)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::dict const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`load`](#de/db2/python_8cpp_1a060af7d6af982340722e479e1582ee8a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::dict & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`save`](#de/db2/python_8cpp_1a71cde744dd594f8fbda35d053902d190)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::object const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public void `[`load`](#de/db2/python_8cpp_1ace4017eb14295029b7fc1563115125cd)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::object & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#d7/d85/stdarray_8hpp_1ab39cb461f108d449d722bc5658ca3989)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::array< T, N > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#d7/d85/stdarray_8hpp_1ac17a21e73eeac5b8b9d658b44d41887a)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::array< T, N > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#d3/d6f/tuple_8hpp_1a4ea0dec0c4c336046280b70333c93256)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::tuple< T0, T1, T2, T3, T4, T5, T6, T7, T8, T9 > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#d3/d6f/tuple_8hpp_1aec7c169181ce47900e6856b2aafe4af9)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::tuple< T0, T1, T2, T3, T4, T5, T6, T7, T8, T9 > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#dc/d69/valarray_8hpp_1a25cea4a2b59c8d5ce1ab1f1c38145cdf)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::valarray< T > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#dc/d69/valarray_8hpp_1a6b1ec38b99161516bc19d40663d783e3)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::valarray< T > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#da/d16/vector_8hpp_1a0652e8d3e0f66b0b30e25ea12b89f921)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< T, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`save`](#da/d16/vector_8hpp_1a5615700c36427d45e14249b6bea943fd)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< bool, A > const & value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#da/d16/vector_8hpp_1a92769e57872c9da4bb7b2cd44d14cb9b)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< T, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`void `[`load`](#da/d16/vector_8hpp_1a0981a3efcda7340c13e5f2b675adea6e)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< bool, A > & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

# class `alps::hdf5::archive` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1ad1230651361f98e08b5ed780f8aebf0e)`(boost::filesystem::path const & filename,std::string mode)` | 
`public  explicit `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1af703e9f3eea0525622ced4f0d6f32629)`(std::string const & filename,int props)` | 
`public  explicit `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1a56d5d4d57c0a675d22a393046ca83714)`(std::string const & filename,char prop)` | 
`public  explicit `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1a0ae443d421dd027027ae787f7c19b84d)`(std::string const & filename,char signed prop)` | 
`public  `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1af84f0cbda1eee5f3ac757a60729de0cb)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` const & arg)` | 
`public virtual  `[`~archive`](#df/d24/classalps_1_1hdf5_1_1archive_1a487b27b9790bfdbd1f005c6fedcdab74)`()` | 
`public std::string const & `[`get_filename`](#df/d24/classalps_1_1hdf5_1_1archive_1a4fdd1370dcb22304f5c2005c3e1f50bb)`() const` | 
`public std::string `[`encode_segment`](#df/d24/classalps_1_1hdf5_1_1archive_1a35ed7fe34299e9bf9bdb555e302511cc)`(std::string segment) const` | 
`public std::string `[`decode_segment`](#df/d24/classalps_1_1hdf5_1_1archive_1acd0e7293f4f3494dadd449327459e4eb)`(std::string segment) const` | 
`public std::string `[`get_context`](#df/d24/classalps_1_1hdf5_1_1archive_1aa5474983515dddb080239dd9384a6e83)`() const` | 
`public void `[`set_context`](#df/d24/classalps_1_1hdf5_1_1archive_1ab13b5600a01d3e8b3eb1ed84a0799ec8)`(std::string const & context)` | 
`public std::string `[`complete_path`](#df/d24/classalps_1_1hdf5_1_1archive_1ad336e3c9ba6ca86fd3d660882d77fb38)`(std::string path) const` | 
`public void `[`close`](#df/d24/classalps_1_1hdf5_1_1archive_1abc6cbb071f730d2a2fa9d0bae0f9077a)`()` | 
`public bool `[`is_open`](#df/d24/classalps_1_1hdf5_1_1archive_1afcfffbee821d312c43834fe7b4959d2e)`()` | 
`public bool `[`is_data`](#df/d24/classalps_1_1hdf5_1_1archive_1a599bb794a3bd17d7a33ba11809060a5d)`(std::string path) const` | 
`public bool `[`is_attribute`](#df/d24/classalps_1_1hdf5_1_1archive_1ad8e3f188026c970715a908f8ebc323a0)`(std::string path) const` | 
`public bool `[`is_group`](#df/d24/classalps_1_1hdf5_1_1archive_1a6d359e22349df7163c17d26bbaf27530)`(std::string path) const` | 
`public bool `[`is_scalar`](#df/d24/classalps_1_1hdf5_1_1archive_1a004a0b58bdb20c6c48c75f97191d33e6)`(std::string path) const` | 
`public bool `[`is_null`](#df/d24/classalps_1_1hdf5_1_1archive_1a8b0391b00662b6493cf490af38ba4407)`(std::string path) const` | 
`public bool `[`is_complex`](#df/d24/classalps_1_1hdf5_1_1archive_1ab79431933eb4b306065550a940e905e1)`(std::string path) const` | 
`public template<>`  <br/>`inline bool `[`is_datatype`](#df/d24/classalps_1_1hdf5_1_1archive_1adf288584f7fabd08bd8846b77610ad99)`(std::string path) const` | 
`public std::vector< std::string > `[`list_children`](#df/d24/classalps_1_1hdf5_1_1archive_1a23ee6a881cd1ee010807e8af7a44279b)`(std::string path) const` | 
`public std::vector< std::string > `[`list_attributes`](#df/d24/classalps_1_1hdf5_1_1archive_1aa8673378a3b72810620ea8d1ffff5748)`(std::string path) const` | 
`public std::vector< std::size_t > `[`extent`](#df/d24/classalps_1_1hdf5_1_1archive_1ab54b27df9f86546938c6cea294077779)`(std::string path) const` | 
`public std::size_t `[`dimensions`](#df/d24/classalps_1_1hdf5_1_1archive_1a1c26d353fc59b1df5bbf07f6d35a5a86)`(std::string path) const` | 
`public void `[`create_group`](#df/d24/classalps_1_1hdf5_1_1archive_1aa25f0db2cf32dab2165d1c414bd56c92)`(std::string path) const` | 
`public void `[`delete_data`](#df/d24/classalps_1_1hdf5_1_1archive_1a565b41cc539fe8b0cfd56f9f7475406d)`(std::string path) const` | 
`public void `[`delete_group`](#df/d24/classalps_1_1hdf5_1_1archive_1aeb8b369b54d16bc5df126a7b5fb18ba1)`(std::string path) const` | 
`public void `[`delete_attribute`](#df/d24/classalps_1_1hdf5_1_1archive_1a8744b96290e31352c54b30d83d8ba5a9)`(std::string path) const` | 
`public void `[`set_complex`](#df/d24/classalps_1_1hdf5_1_1archive_1a37c66adcebb404048b267bf08dd8ad43)`(std::string path)` | 
`public `[`detail::archive_proxy](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)< [archive`](#df/d24/classalps_1_1hdf5_1_1archive)` > `[`operator[]`](#df/d24/classalps_1_1hdf5_1_1archive_1a73316438d407af03a6e07477f32c0eaa)`(std::string const & path)` | 
`public template<>`  <br/>`inline void `[`read`](#df/d24/classalps_1_1hdf5_1_1archive_1a6f761c7eef4af7884ecb3cc609a96d22)`(std::string path,T *,std::vector< std::size_t >,std::vector< std::size_t >) const` | 
`public template<>`  <br/>`inline void `[`write`](#df/d24/classalps_1_1hdf5_1_1archive_1ac359c2dc26ac824c81367a37e36841fe)`(std::string path,T const * value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset) const` | 
`enum `[`properties`](#df/d24/classalps_1_1hdf5_1_1archive_1af0ff0c67be9649fad2099457a33d5db3) | 

## Members

#### `public  `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1ad1230651361f98e08b5ed780f8aebf0e)`(boost::filesystem::path const & filename,std::string mode)` 

#### `public  explicit `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1af703e9f3eea0525622ced4f0d6f32629)`(std::string const & filename,int props)` 

#### `public  explicit `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1a56d5d4d57c0a675d22a393046ca83714)`(std::string const & filename,char prop)` 

#### `public  explicit `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1a0ae443d421dd027027ae787f7c19b84d)`(std::string const & filename,char signed prop)` 

#### `public  `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive_1af84f0cbda1eee5f3ac757a60729de0cb)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` const & arg)` 

#### `public virtual  `[`~archive`](#df/d24/classalps_1_1hdf5_1_1archive_1a487b27b9790bfdbd1f005c6fedcdab74)`()` 

#### `public std::string const & `[`get_filename`](#df/d24/classalps_1_1hdf5_1_1archive_1a4fdd1370dcb22304f5c2005c3e1f50bb)`() const` 

#### `public std::string `[`encode_segment`](#df/d24/classalps_1_1hdf5_1_1archive_1a35ed7fe34299e9bf9bdb555e302511cc)`(std::string segment) const` 

#### `public std::string `[`decode_segment`](#df/d24/classalps_1_1hdf5_1_1archive_1acd0e7293f4f3494dadd449327459e4eb)`(std::string segment) const` 

#### `public std::string `[`get_context`](#df/d24/classalps_1_1hdf5_1_1archive_1aa5474983515dddb080239dd9384a6e83)`() const` 

#### `public void `[`set_context`](#df/d24/classalps_1_1hdf5_1_1archive_1ab13b5600a01d3e8b3eb1ed84a0799ec8)`(std::string const & context)` 

#### `public std::string `[`complete_path`](#df/d24/classalps_1_1hdf5_1_1archive_1ad336e3c9ba6ca86fd3d660882d77fb38)`(std::string path) const` 

#### `public void `[`close`](#df/d24/classalps_1_1hdf5_1_1archive_1abc6cbb071f730d2a2fa9d0bae0f9077a)`()` 

#### `public bool `[`is_open`](#df/d24/classalps_1_1hdf5_1_1archive_1afcfffbee821d312c43834fe7b4959d2e)`()` 

#### `public bool `[`is_data`](#df/d24/classalps_1_1hdf5_1_1archive_1a599bb794a3bd17d7a33ba11809060a5d)`(std::string path) const` 

#### `public bool `[`is_attribute`](#df/d24/classalps_1_1hdf5_1_1archive_1ad8e3f188026c970715a908f8ebc323a0)`(std::string path) const` 

#### `public bool `[`is_group`](#df/d24/classalps_1_1hdf5_1_1archive_1a6d359e22349df7163c17d26bbaf27530)`(std::string path) const` 

#### `public bool `[`is_scalar`](#df/d24/classalps_1_1hdf5_1_1archive_1a004a0b58bdb20c6c48c75f97191d33e6)`(std::string path) const` 

#### `public bool `[`is_null`](#df/d24/classalps_1_1hdf5_1_1archive_1a8b0391b00662b6493cf490af38ba4407)`(std::string path) const` 

#### `public bool `[`is_complex`](#df/d24/classalps_1_1hdf5_1_1archive_1ab79431933eb4b306065550a940e905e1)`(std::string path) const` 

#### `public template<>`  <br/>`inline bool `[`is_datatype`](#df/d24/classalps_1_1hdf5_1_1archive_1adf288584f7fabd08bd8846b77610ad99)`(std::string path) const` 

#### `public std::vector< std::string > `[`list_children`](#df/d24/classalps_1_1hdf5_1_1archive_1a23ee6a881cd1ee010807e8af7a44279b)`(std::string path) const` 

#### `public std::vector< std::string > `[`list_attributes`](#df/d24/classalps_1_1hdf5_1_1archive_1aa8673378a3b72810620ea8d1ffff5748)`(std::string path) const` 

#### `public std::vector< std::size_t > `[`extent`](#df/d24/classalps_1_1hdf5_1_1archive_1ab54b27df9f86546938c6cea294077779)`(std::string path) const` 

#### `public std::size_t `[`dimensions`](#df/d24/classalps_1_1hdf5_1_1archive_1a1c26d353fc59b1df5bbf07f6d35a5a86)`(std::string path) const` 

#### `public void `[`create_group`](#df/d24/classalps_1_1hdf5_1_1archive_1aa25f0db2cf32dab2165d1c414bd56c92)`(std::string path) const` 

#### `public void `[`delete_data`](#df/d24/classalps_1_1hdf5_1_1archive_1a565b41cc539fe8b0cfd56f9f7475406d)`(std::string path) const` 

#### `public void `[`delete_group`](#df/d24/classalps_1_1hdf5_1_1archive_1aeb8b369b54d16bc5df126a7b5fb18ba1)`(std::string path) const` 

#### `public void `[`delete_attribute`](#df/d24/classalps_1_1hdf5_1_1archive_1a8744b96290e31352c54b30d83d8ba5a9)`(std::string path) const` 

#### `public void `[`set_complex`](#df/d24/classalps_1_1hdf5_1_1archive_1a37c66adcebb404048b267bf08dd8ad43)`(std::string path)` 

#### `public `[`detail::archive_proxy](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)< [archive`](#df/d24/classalps_1_1hdf5_1_1archive)` > `[`operator[]`](#df/d24/classalps_1_1hdf5_1_1archive_1a73316438d407af03a6e07477f32c0eaa)`(std::string const & path)` 

#### `public template<>`  <br/>`inline void `[`read`](#df/d24/classalps_1_1hdf5_1_1archive_1a6f761c7eef4af7884ecb3cc609a96d22)`(std::string path,T *,std::vector< std::size_t >,std::vector< std::size_t >) const` 

#### `public template<>`  <br/>`inline void `[`write`](#df/d24/classalps_1_1hdf5_1_1archive_1ac359c2dc26ac824c81367a37e36841fe)`(std::string path,T const * value,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset) const` 

#### `enum `[`properties`](#df/d24/classalps_1_1hdf5_1_1archive_1af0ff0c67be9649fad2099457a33d5db3) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
READ            | 
WRITE            | 
REPLACE            | 
COMPRESS            | 
LARGE            | 
MEMORY            | 

# class `alps::hdf5::archive_error` 

```
class alps::hdf5::archive_error
  : public std::runtime_error
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`archive_error`](#df/d8a/classalps_1_1hdf5_1_1archive__error_1a9f771c484e034bf82699bf102467d4a7)`(std::string const & what)` | 

## Members

#### `public inline  `[`archive_error`](#df/d8a/classalps_1_1hdf5_1_1archive__error_1a9f771c484e034bf82699bf102467d4a7)`(std::string const & what)` 

# struct `alps::hdf5::has_complex_elements` 

```
struct alps::hdf5::has_complex_elements
  : public boost::false_type
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< alps::multi_array< T, N, A > >` 

```
struct alps::hdf5::has_complex_elements< alps::multi_array< T, N, A > >
  : public alps::hdf5::has_complex_elements< boost::multi_array< T, N, A > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< alps::numeric::matrix< T, MemoryBlock > >` 

```
struct alps::hdf5::has_complex_elements< alps::numeric::matrix< T, MemoryBlock > >
  : public alps::hdf5::has_complex_elements< alps::detail::remove_cvr< alps::numeric::matrix< T, MemoryBlock >::value_type >::type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< boost::array< T, N > >` 

```
struct alps::hdf5::has_complex_elements< boost::array< T, N > >
  : public alps::hdf5::has_complex_elements< alps::detail::remove_cvr< boost::array< T, N >::value_type >::type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< boost::multi_array< T, N, A > >` 

```
struct alps::hdf5::has_complex_elements< boost::multi_array< T, N, A > >
  : public alps::hdf5::has_complex_elements< alps::detail::remove_cvr< T >::type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< std::array< T, N > >` 

```
struct alps::hdf5::has_complex_elements< std::array< T, N > >
  : public alps::hdf5::has_complex_elements< alps::detail::remove_cvr< std::array< T, N >::value_type >::type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< std::complex< T > >` 

```
struct alps::hdf5::has_complex_elements< std::complex< T > >
  : public boost::true_type
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< std::pair< T *, std::vector< std::size_t > > >` 

```
struct alps::hdf5::has_complex_elements< std::pair< T *, std::vector< std::size_t > > >
  : public alps::hdf5::has_complex_elements< alps::detail::remove_cvr< T >::type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< std::valarray< T > >` 

```
struct alps::hdf5::has_complex_elements< std::valarray< T > >
  : public alps::hdf5::has_complex_elements< alps::detail::remove_cvr< T >::type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::has_complex_elements< std::vector< T, A > >` 

```
struct alps::hdf5::has_complex_elements< std::vector< T, A > >
  : public alps::hdf5::has_complex_elements< alps::detail::remove_cvr< std::vector< T, A >::value_type >::type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_content_continuous` 

```
struct alps::hdf5::is_content_continuous
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_content_continuous< alps::multi_array< T, N, A > >` 

```
struct alps::hdf5::is_content_continuous< alps::multi_array< T, N, A > >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_content_continuous< std::pair< T *, std::vector< std::size_t > > >` 

```
struct alps::hdf5::is_content_continuous< std::pair< T *, std::vector< std::size_t > > >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_content_continuous< std::valarray< T > >` 

```
struct alps::hdf5::is_content_continuous< std::valarray< T > >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_content_continuous< std::vector< bool, A > >` 

```
struct alps::hdf5::is_content_continuous< std::vector< bool, A > >
  : public boost::false_type
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_content_continuous< std::vector< T, A > >` 

```
struct alps::hdf5::is_content_continuous< std::vector< T, A > >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_continuous` 

```
struct alps::hdf5::is_continuous
  : public boost::false_type
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_continuous< boost::array< T, N > >` 

```
struct alps::hdf5::is_continuous< boost::array< T, N > >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_continuous< boost::array< T, N > const >` 

```
struct alps::hdf5::is_continuous< boost::array< T, N > const >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_continuous< std::array< T, N > >` 

```
struct alps::hdf5::is_continuous< std::array< T, N > >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_continuous< std::array< T, N > const >` 

```
struct alps::hdf5::is_continuous< std::array< T, N > const >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_continuous< std::complex< T > >` 

```
struct alps::hdf5::is_continuous< std::complex< T > >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::is_continuous< std::complex< T > const >` 

```
struct alps::hdf5::is_continuous< std::complex< T > const >
  : public alps::hdf5::is_continuous< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::scalar_type` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#d1/dbd/structalps_1_1hdf5_1_1scalar__type_1a6c171ed89b69a97024d148e7415aeb7f) | 

## Members

#### `typedef `[`type`](#d1/dbd/structalps_1_1hdf5_1_1scalar__type_1a6c171ed89b69a97024d148e7415aeb7f) 

# struct `alps::hdf5::scalar_type< alps::multi_array< T, N, A > >` 

```
struct alps::hdf5::scalar_type< alps::multi_array< T, N, A > >
  : public alps::hdf5::scalar_type< boost::multi_array< T, N, A > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::scalar_type< alps::numeric::matrix< T, MemoryBlock > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#df/d79/structalps_1_1hdf5_1_1scalar__type_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01_4_1ac4168653181930437d79d61ce15c0b22) | 

## Members

#### `typedef `[`type`](#df/d79/structalps_1_1hdf5_1_1scalar__type_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01_4_1ac4168653181930437d79d61ce15c0b22) 

# struct `alps::hdf5::scalar_type< boost::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#db/dca/structalps_1_1hdf5_1_1scalar__type_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4_1a44235a365a062be76ef0aa7097b1b3e5) | 

## Members

#### `typedef `[`type`](#db/dca/structalps_1_1hdf5_1_1scalar__type_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4_1a44235a365a062be76ef0aa7097b1b3e5) 

# struct `alps::hdf5::scalar_type< boost::multi_array< T, N, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#d7/d05/structalps_1_1hdf5_1_1scalar__type_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4_1a0cc1633a01dfefc3c07dd7ae1395107e) | 

## Members

#### `typedef `[`type`](#d7/d05/structalps_1_1hdf5_1_1scalar__type_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4_1a0cc1633a01dfefc3c07dd7ae1395107e) 

# struct `alps::hdf5::scalar_type< std::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#dc/da8/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4_1a10e122d0228cef495b0caa48adf24f44) | 

## Members

#### `typedef `[`type`](#dc/da8/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4_1a10e122d0228cef495b0caa48adf24f44) 

# struct `alps::hdf5::scalar_type< std::complex< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#d7/d48/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1complex_3_01_t_01_4_01_4_1a7b669f544d1538dcf5d0b7ab62c2a407) | 

## Members

#### `typedef `[`type`](#d7/d48/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1complex_3_01_t_01_4_01_4_1a7b669f544d1538dcf5d0b7ab62c2a407) 

# struct `alps::hdf5::scalar_type< std::pair< T *, std::vector< std::size_t > > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#d6/d54/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_01std_1_1size__t_01_4_01_4_01_4_1a644ea70326fa88d14d39e4e85067dcfc) | 

## Members

#### `typedef `[`type`](#d6/d54/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_01std_1_1size__t_01_4_01_4_01_4_1a644ea70326fa88d14d39e4e85067dcfc) 

# struct `alps::hdf5::scalar_type< std::valarray< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#de/d44/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1valarray_3_01_t_01_4_01_4_1af4b85325e9240d9630b747b7c6a5bba8) | 

## Members

#### `typedef `[`type`](#de/d44/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1valarray_3_01_t_01_4_01_4_1af4b85325e9240d9630b747b7c6a5bba8) 

# struct `alps::hdf5::scalar_type< std::vector< T, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#de/d09/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4_1a71f338bd53c5e7bd612e5b7a908f073e) | 

## Members

#### `typedef `[`type`](#de/d09/structalps_1_1hdf5_1_1scalar__type_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4_1a71f338bd53c5e7bd612e5b7a908f073e) 

# namespace `alps::hdf5::detail` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public herr_t `[`noop`](#d7/d05/archive_8cpp_1ae2d250b7653ae45e7e4ac2babc1cbda1)`(hid_t)`            | 
`public hid_t `[`check_group`](#d7/d05/archive_8cpp_1a8b9f2d4d0fe611309ba1501883400e2f)`(hid_t id)`            | 
`public hid_t `[`check_data`](#d7/d05/archive_8cpp_1a654fd4aeaa9cb2451a7e3f51793194cd)`(hid_t id)`            | 
`public hid_t `[`check_attribute`](#d7/d05/archive_8cpp_1ab71316b680e2c262ef72fae1a369febe)`(hid_t id)`            | 
`public hid_t `[`check_space`](#d7/d05/archive_8cpp_1aa9734ba24db1cc39d56558d0a8e60af2)`(hid_t id)`            | 
`public hid_t `[`check_type`](#d7/d05/archive_8cpp_1a356df9c5426c0aeb8bfe31a290ce3935)`(hid_t id)`            | 
`public hid_t `[`check_property`](#d7/d05/archive_8cpp_1ab92ace5e4256a82bbfd08786cee22e30)`(hid_t id)`            | 
`public hid_t `[`check_error`](#d7/d05/archive_8cpp_1a12b74c152a8eda70e09e17f1fe188033)`(hid_t id)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a9fc4695e71227b62d0021c142574d5b2)`(char)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1affa9eaa03a1e68c545361eda41565803)`(signed char)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1afde04d0cd4874eb9d1701f39c148cd14)`(unsigned char)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a5eb3a1f74d68f5381d948a3367a430c4)`(short)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a411bc975371882477fb0bc58b2edc684)`(unsigned short)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a920f385f4bd4312f86e0496212536493)`(int)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ad3fba037afd667dfd3bf27707a7ac196)`(unsigned)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ab515855cafb7a1bae2e24b21fcd32efb)`(long)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ace1eac5ad4b4410baf8b4ce1f4b70d13)`(unsigned long)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a8274e1fae3decc423c6c2d1860153678)`(long long)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a19c76ff98f7adac9e2f89a0e1479caa4)`(unsigned long long)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1aad7f20c52edd7ae8c7f7b437c78c5611)`(float)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a7a8c3042bf068520176c86baa8f2c56c)`(double)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ac975c940c9e0738e18de7fe3cbbaa76c)`(long double)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a8c7e50bd9f7ebe3ea342a2438ae6f2ca)`(bool)`            | 
`public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ab8ea22385d958496452e16efd70cca6a)`(std::string)`            | 
`public hid_t `[`open_attribute`](#d7/d05/archive_8cpp_1affc17b7b88e907316dde1b1bfd69761e)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` const & ar,hid_t file_id,std::string path)`            | 
`public herr_t `[`list_children_visitor`](#d7/d05/archive_8cpp_1a3f50094357f4ec12e48439ad1e701b3b)`(hid_t,char const * n,const H5L_info_t *,void * d)`            | 
`public herr_t `[`list_attributes_visitor`](#d7/d05/archive_8cpp_1a56f6b35ea5d149d98ce11f130361aad4)`(hid_t,char const * n,const H5A_info_t *,void * d)`            | 
`public template<>`  <br/>`bool `[`is_vectorizable_generic`](#de/db2/python_8cpp_1a6531b9f1a6a356a62da2ad4c51f47115)`(T const & value)`            | 
`public template<>`  <br/>`std::vector< std::size_t > `[`get_extent_generic`](#de/db2/python_8cpp_1a33816b97db74f43b60de993cf64b816f)`(T const & value)`            | 
`public template<>`  <br/>`void `[`load_python_numeric`](#de/db2/python_8cpp_1afaf42451d2663c54980d75d2465e74da)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::python::numpy::array & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset,int type)`            | 
`public template<>`  <br/>`void `[`load_python_object`](#de/db2/python_8cpp_1af3ef8f873be574a80997217d300cc8b4)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::object & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset,int type)`            | 
`class `[`alps::hdf5::detail::error`](#d8/dbe/classalps_1_1hdf5_1_1detail_1_1error) | 
`class `[`alps::hdf5::detail::resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource) | 
`struct `[`alps::hdf5::detail::archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy) | 
`struct `[`alps::hdf5::detail::archivecontext`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext) | 
`struct `[`alps::hdf5::detail::get_extent`](#d3/d96/structalps_1_1hdf5_1_1detail_1_1get__extent) | 
`struct `[`alps::hdf5::detail::get_extent< alps::multi_array< T, N, A > >`](#df/d7e/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01alps_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< alps::numeric::matrix< T, MemoryBlock > >`](#d4/dca/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< alps::python::numpy::array >`](#da/de8/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01alps_1_1python_1_1numpy_1_1array_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< boost::array< T, N > >`](#da/d37/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< boost::multi_array< T, N, A > >`](#d8/db0/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< boost::python::list >`](#db/d6c/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01boost_1_1python_1_1list_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< boost::python::object >`](#d0/de6/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01boost_1_1python_1_1object_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< boost::python::tuple >`](#dd/df0/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01boost_1_1python_1_1tuple_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< std::array< T, N > >`](#dd/d18/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< std::complex< T > >`](#d1/d49/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< std::pair< T *, std::vector< std::size_t > > >`](#d7/d3e/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_01std_1_1size__t_01_4_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< std::valarray< T > >`](#db/df6/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_extent< std::vector< T, A > >`](#d0/de0/structalps_1_1hdf5_1_1detail_1_1get__extent_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer`](#da/db5/structalps_1_1hdf5_1_1detail_1_1get__pointer) | 
`struct `[`alps::hdf5::detail::get_pointer< alps::multi_array< T, N, A > >`](#d0/d42/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01alps_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< alps::multi_array< T, N, A > const >`](#dc/d9a/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01alps_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< alps::numeric::matrix< T, MemoryBlock > >`](#db/ddb/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< alps::numeric::matrix< T, MemoryBlock > const >`](#de/d9e/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< boost::array< T, N > >`](#de/df4/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< boost::array< T, N > const >`](#de/dff/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01boost_1_1array_3_01_t_00_01_n_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< boost::multi_array< T, N, A > >`](#d5/d8d/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< boost::multi_array< T, N, A > const >`](#d6/d06/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::array< T, N > >`](#d9/d1f/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::array< T, N > const >`](#da/d05/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1array_3_01_t_00_01_n_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::complex< T > >`](#d9/d6a/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::complex< T > const >`](#d3/d1d/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1complex_3_01_t_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::pair< T *, std::vector< std::size_t > > >`](#d2/d66/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_01std_1_1size__t_01_4_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::pair< T *, std::vector< std::size_t > > const >`](#d1/db2/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_0165f602bbbaf47b3ddeab6121eac01a3b) | 
`struct `[`alps::hdf5::detail::get_pointer< std::valarray< T > >`](#d8/d3a/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::valarray< T > const >`](#d3/d40/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1valarray_3_01_t_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::vector< bool, A > >`](#d4/d9d/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1vector_3_01bool_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::vector< bool, A > const >`](#dc/dee/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1vector_3_01bool_00_01_a_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::vector< T, A > >`](#d1/dd3/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< std::vector< T, A > const >`](#d5/d32/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01std_1_1vector_3_01_t_00_01_a_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::get_pointer< T const >`](#df/da5/structalps_1_1hdf5_1_1detail_1_1get__pointer_3_01_t_01const_01_4) | 
`struct `[`alps::hdf5::detail::is_datatype_caller`](#d8/db6/structalps_1_1hdf5_1_1detail_1_1is__datatype__caller) | 
`struct `[`alps::hdf5::detail::is_datatype_impl_compare`](#d2/df1/structalps_1_1hdf5_1_1detail_1_1is__datatype__impl__compare) | 
`struct `[`alps::hdf5::detail::is_datatype_impl_compare< std::string >`](#d2/da1/structalps_1_1hdf5_1_1detail_1_1is__datatype__impl__compare_3_01std_1_1string_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable`](#d7/daf/structalps_1_1hdf5_1_1detail_1_1is__vectorizable) | 
`struct `[`alps::hdf5::detail::is_vectorizable< alps::multi_array< T, N, A > >`](#df/d8f/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01alps_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< alps::numeric::matrix< T, MemoryBlock > >`](#df/d73/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< alps::python::numpy::array >`](#de/d09/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01alps_1_1python_1_1numpy_1_1array_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< boost::array< T, N > >`](#df/d0f/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< boost::multi_array< T, N, A > >`](#dd/dfc/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< boost::python::list >`](#dd/d28/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01boost_1_1python_1_1list_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< boost::python::object >`](#de/dbf/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01boost_1_1python_1_1object_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< boost::python::tuple >`](#dc/d12/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01boost_1_1python_1_1tuple_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< std::array< T, N > >`](#df/d51/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< std::complex< T > >`](#da/d33/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< std::complex< T > const >`](#dc/db4/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01std_1_1complex_3_01_t_01_4_01const_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< std::pair< T *, std::vector< std::size_t > > >`](#d7/da5/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_944261990554eb324aff5dc16bf8f255) | 
`struct `[`alps::hdf5::detail::is_vectorizable< std::valarray< T > >`](#da/d01/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< std::vector< bool, A > >`](#d2/dcd/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01std_1_1vector_3_01bool_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::is_vectorizable< std::vector< T, A > >`](#da/d62/structalps_1_1hdf5_1_1detail_1_1is__vectorizable_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::load_helper`](#da/d26/structalps_1_1hdf5_1_1detail_1_1load__helper) | 
`struct `[`alps::hdf5::detail::load_helper< N, T, boost::true_type >`](#d5/db7/structalps_1_1hdf5_1_1detail_1_1load__helper_3_01_n_00_01_t_00_01boost_1_1true__type_01_4) | 
`struct `[`alps::hdf5::detail::make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy) | 
`struct `[`alps::hdf5::detail::native_ptr_converter`](#d8/dd2/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter) | 
`struct `[`alps::hdf5::detail::native_ptr_converter< std::string >`](#de/d98/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_3_01std_1_1string_01_4) | 
`struct `[`alps::hdf5::detail::save_helper`](#d0/de6/structalps_1_1hdf5_1_1detail_1_1save__helper) | 
`struct `[`alps::hdf5::detail::save_helper< N, T, boost::true_type >`](#d7/d9d/structalps_1_1hdf5_1_1detail_1_1save__helper_3_01_n_00_01_t_00_01boost_1_1true__type_01_4) | 
`struct `[`alps::hdf5::detail::save_python_object_visitor`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor) | 
`struct `[`alps::hdf5::detail::set_extent`](#d2/d99/structalps_1_1hdf5_1_1detail_1_1set__extent) | 
`struct `[`alps::hdf5::detail::set_extent< alps::multi_array< T, N, A > >`](#da/dcc/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01alps_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< alps::numeric::matrix< T, MemoryBlock > >`](#dd/d2b/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01alps_1_1numeric_1_1matrix_3_01_t_00_01_memory_block_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< alps::python::numpy::array >`](#dd/d04/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01alps_1_1python_1_1numpy_1_1array_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< boost::array< T, N > >`](#d8/d35/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01boost_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< boost::multi_array< T, N, A > >`](#d4/da7/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01boost_1_1multi__array_3_01_t_00_01_n_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< boost::python::list >`](#d1/d91/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01boost_1_1python_1_1list_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< boost::python::object >`](#d6/dc6/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01boost_1_1python_1_1object_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< std::array< T, N > >`](#df/d89/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01std_1_1array_3_01_t_00_01_n_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< std::complex< T > >`](#da/dac/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01std_1_1complex_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< std::pair< T *, std::vector< std::size_t > > >`](#da/d64/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01std_1_1pair_3_01_t_01_5_00_01std_1_1vector_3_01std_1_1size__t_01_4_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< std::valarray< T > >`](#d0/dbb/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< std::vector< bool, A > >`](#d5/d77/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01std_1_1vector_3_01bool_00_01_a_01_4_01_4) | 
`struct `[`alps::hdf5::detail::set_extent< std::vector< T, A > >`](#d1/d2b/structalps_1_1hdf5_1_1detail_1_1set__extent_3_01std_1_1vector_3_01_t_00_01_a_01_4_01_4) | 

## Members

#### `public herr_t `[`noop`](#d7/d05/archive_8cpp_1ae2d250b7653ae45e7e4ac2babc1cbda1)`(hid_t)` 

#### `public hid_t `[`check_group`](#d7/d05/archive_8cpp_1a8b9f2d4d0fe611309ba1501883400e2f)`(hid_t id)` 

#### `public hid_t `[`check_data`](#d7/d05/archive_8cpp_1a654fd4aeaa9cb2451a7e3f51793194cd)`(hid_t id)` 

#### `public hid_t `[`check_attribute`](#d7/d05/archive_8cpp_1ab71316b680e2c262ef72fae1a369febe)`(hid_t id)` 

#### `public hid_t `[`check_space`](#d7/d05/archive_8cpp_1aa9734ba24db1cc39d56558d0a8e60af2)`(hid_t id)` 

#### `public hid_t `[`check_type`](#d7/d05/archive_8cpp_1a356df9c5426c0aeb8bfe31a290ce3935)`(hid_t id)` 

#### `public hid_t `[`check_property`](#d7/d05/archive_8cpp_1ab92ace5e4256a82bbfd08786cee22e30)`(hid_t id)` 

#### `public hid_t `[`check_error`](#d7/d05/archive_8cpp_1a12b74c152a8eda70e09e17f1fe188033)`(hid_t id)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a9fc4695e71227b62d0021c142574d5b2)`(char)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1affa9eaa03a1e68c545361eda41565803)`(signed char)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1afde04d0cd4874eb9d1701f39c148cd14)`(unsigned char)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a5eb3a1f74d68f5381d948a3367a430c4)`(short)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a411bc975371882477fb0bc58b2edc684)`(unsigned short)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a920f385f4bd4312f86e0496212536493)`(int)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ad3fba037afd667dfd3bf27707a7ac196)`(unsigned)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ab515855cafb7a1bae2e24b21fcd32efb)`(long)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ace1eac5ad4b4410baf8b4ce1f4b70d13)`(unsigned long)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a8274e1fae3decc423c6c2d1860153678)`(long long)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a19c76ff98f7adac9e2f89a0e1479caa4)`(unsigned long long)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1aad7f20c52edd7ae8c7f7b437c78c5611)`(float)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a7a8c3042bf068520176c86baa8f2c56c)`(double)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ac975c940c9e0738e18de7fe3cbbaa76c)`(long double)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1a8c7e50bd9f7ebe3ea342a2438ae6f2ca)`(bool)` 

#### `public hid_t `[`get_native_type`](#d7/d05/archive_8cpp_1ab8ea22385d958496452e16efd70cca6a)`(std::string)` 

#### `public hid_t `[`open_attribute`](#d7/d05/archive_8cpp_1affc17b7b88e907316dde1b1bfd69761e)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` const & ar,hid_t file_id,std::string path)` 

#### `public herr_t `[`list_children_visitor`](#d7/d05/archive_8cpp_1a3f50094357f4ec12e48439ad1e701b3b)`(hid_t,char const * n,const H5L_info_t *,void * d)` 

#### `public herr_t `[`list_attributes_visitor`](#d7/d05/archive_8cpp_1a56f6b35ea5d149d98ce11f130361aad4)`(hid_t,char const * n,const H5A_info_t *,void * d)` 

#### `public template<>`  <br/>`bool `[`is_vectorizable_generic`](#de/db2/python_8cpp_1a6531b9f1a6a356a62da2ad4c51f47115)`(T const & value)` 

#### `public template<>`  <br/>`std::vector< std::size_t > `[`get_extent_generic`](#de/db2/python_8cpp_1a33816b97db74f43b60de993cf64b816f)`(T const & value)` 

#### `public template<>`  <br/>`void `[`load_python_numeric`](#de/db2/python_8cpp_1afaf42451d2663c54980d75d2465e74da)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,alps::python::numpy::array & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset,int type)` 

#### `public template<>`  <br/>`void `[`load_python_object`](#de/db2/python_8cpp_1af3ef8f873be574a80997217d300cc8b4)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,boost::python::object & value,std::vector< std::size_t > chunk,std::vector< std::size_t > offset,int type)` 

# class `alps::hdf5::detail::error` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline std::string `[`invoke`](#d8/dbe/classalps_1_1hdf5_1_1detail_1_1error_1a606baba9ff4fece52b2130659196d0ea)`(hid_t id)` | 

## Members

#### `public inline std::string `[`invoke`](#d8/dbe/classalps_1_1hdf5_1_1detail_1_1error_1a606baba9ff4fece52b2130659196d0ea)`(hid_t id)` 

# class `alps::hdf5::detail::resource` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1a94c7588e7b79cedf9ecf2639d731f1b0)`()` | 
`public inline  `[`resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1aaf89e3d999d6e172c66bf42650cf8dac)`(hid_t id)` | 
`public inline  `[`~resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1ad34f4327f9a67190800f31536c7e161e)`()` | 
`public inline  `[`operator hid_t`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1a85a7be5d144e1f2b1033275e81ac3f17)`() const` | 
`public inline `[`resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource)`< F > & `[`operator=`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1a613b0534a3128fc5e85196efd29a19f4)`(hid_t id)` | 

## Members

#### `public inline  `[`resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1a94c7588e7b79cedf9ecf2639d731f1b0)`()` 

#### `public inline  `[`resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1aaf89e3d999d6e172c66bf42650cf8dac)`(hid_t id)` 

#### `public inline  `[`~resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1ad34f4327f9a67190800f31536c7e161e)`()` 

#### `public inline  `[`operator hid_t`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1a85a7be5d144e1f2b1033275e81ac3f17)`() const` 

#### `public inline `[`resource`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource)`< F > & `[`operator=`](#da/db3/classalps_1_1hdf5_1_1detail_1_1resource_1a613b0534a3128fc5e85196efd29a19f4)`(hid_t id)` 

# struct `alps::hdf5::detail::archive_proxy` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public std::string `[`path_`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a37a875c0e2ffa9402ca9bce44d939764) | 
`public A `[`ar_`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a7f2579da78d32042d27c4af70d183a3a) | 
`public inline  explicit `[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a6895d5be7c3ff971849888177c592d4d)`(std::string const & path,A & ar)` | 
`public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)` & `[`operator=`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1abc369075e4ae06a401e68b685376e237)`(T const & value)` | 
`public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)` & `[`operator<<`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a3aba991e0da0cb04a7acaa88d4c9452b)`(T const & value)` | 
`public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)` & `[`operator>>`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a24d2e67eaf8f42c12413b2882fca8287)`(T & value)` | 
`public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)`< A > & `[`operator=`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a445a3b4d2a9ee12b8af858bef258e976)`(T const & value)` | 
`public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)`< A > & `[`operator<<`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a8d61d50fb86c2ddf33438d24a604f484)`(T const & value)` | 
`public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)`< A > & `[`operator>>`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1af2fb6321d532fba45fb3995036386964)`(T & value)` | 

## Members

#### `public std::string `[`path_`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a37a875c0e2ffa9402ca9bce44d939764) 

#### `public A `[`ar_`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a7f2579da78d32042d27c4af70d183a3a) 

#### `public inline  explicit `[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a6895d5be7c3ff971849888177c592d4d)`(std::string const & path,A & ar)` 

#### `public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)` & `[`operator=`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1abc369075e4ae06a401e68b685376e237)`(T const & value)` 

#### `public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)` & `[`operator<<`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a3aba991e0da0cb04a7acaa88d4c9452b)`(T const & value)` 

#### `public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)` & `[`operator>>`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a24d2e67eaf8f42c12413b2882fca8287)`(T & value)` 

#### `public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)`< A > & `[`operator=`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a445a3b4d2a9ee12b8af858bef258e976)`(T const & value)` 

#### `public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)`< A > & `[`operator<<`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1a8d61d50fb86c2ddf33438d24a604f484)`(T const & value)` 

#### `public template<>`  <br/>[`archive_proxy`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy)`< A > & `[`operator>>`](#d3/dbd/structalps_1_1hdf5_1_1detail_1_1archive__proxy_1af2fb6321d532fba45fb3995036386964)`(T & value)` 

# struct `alps::hdf5::detail::archivecontext` 

```
struct alps::hdf5::detail::archivecontext
  : public boost::noncopyable
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public bool `[`compress_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a356630fb283ca4864faf361d640c2980) | 
`public bool `[`write_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a8d7e0f64b46f99114a1d2c47bcb8d7ac) | 
`public bool `[`replace_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a7041fe38b91bdcf42f160ff22b2c8dfd) | 
`public bool `[`large_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a8a6cf30dab9ce06bb93c3bc0c76b7937) | 
`public bool `[`memory_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a6e092a53cf288fbfcfe1c3fa8b9b2135) | 
`public std::string `[`filename_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a4d2f57e97e2e0bbc3785414c2013931a) | 
`public std::string `[`suffix_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1ac3ca21791b45c26e3efc5ed5563cfb9b) | 
`public hid_t `[`file_id_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a7180632cdd9c13097e679680cfc6060c) | 
`public inline  `[`archivecontext`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1ade17892606f40d04eb6a43db7af35a9a)`(std::string const & filename,bool write,bool replace,bool compress,bool large,bool memory)` | 
`public inline  `[`~archivecontext`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a255a0a66ca10090e8be938f6462332d6)`()` | 
`public inline void `[`grant`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a366775383ec8f2e96dd8dc28dd21e8f9)`(bool write,bool replace)` | 

## Members

#### `public bool `[`compress_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a356630fb283ca4864faf361d640c2980) 

#### `public bool `[`write_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a8d7e0f64b46f99114a1d2c47bcb8d7ac) 

#### `public bool `[`replace_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a7041fe38b91bdcf42f160ff22b2c8dfd) 

#### `public bool `[`large_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a8a6cf30dab9ce06bb93c3bc0c76b7937) 

#### `public bool `[`memory_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a6e092a53cf288fbfcfe1c3fa8b9b2135) 

#### `public std::string `[`filename_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a4d2f57e97e2e0bbc3785414c2013931a) 

#### `public std::string `[`suffix_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1ac3ca21791b45c26e3efc5ed5563cfb9b) 

#### `public hid_t `[`file_id_`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a7180632cdd9c13097e679680cfc6060c) 

#### `public inline  `[`archivecontext`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1ade17892606f40d04eb6a43db7af35a9a)`(std::string const & filename,bool write,bool replace,bool compress,bool large,bool memory)` 

#### `public inline  `[`~archivecontext`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a255a0a66ca10090e8be938f6462332d6)`()` 

#### `public inline void `[`grant`](#d9/d7d/structalps_1_1hdf5_1_1detail_1_1archivecontext_1a366775383ec8f2e96dd8dc28dd21e8f9)`(bool write,bool replace)` 

# struct `alps::hdf5::detail::get_extent` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< alps::multi_array< T, N, A > >` 

```
struct alps::hdf5::detail::get_extent< alps::multi_array< T, N, A > >
  : public alps::hdf5::detail::get_extent< boost::multi_array< T, N, A > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< alps::numeric::matrix< T, MemoryBlock > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< alps::python::numpy::array >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< boost::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< boost::multi_array< T, N, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< boost::python::list >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< boost::python::object >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< boost::python::tuple >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< std::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< std::complex< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< std::pair< T *, std::vector< std::size_t > > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< std::valarray< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_extent< std::vector< T, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< alps::multi_array< T, N, A > >` 

```
struct alps::hdf5::detail::get_pointer< alps::multi_array< T, N, A > >
  : public alps::hdf5::detail::get_pointer< boost::multi_array< T, N, A > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< alps::multi_array< T, N, A > const >` 

```
struct alps::hdf5::detail::get_pointer< alps::multi_array< T, N, A > const >
  : public alps::hdf5::detail::get_pointer< boost::multi_array< T, N, A > const >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< alps::numeric::matrix< T, MemoryBlock > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< alps::numeric::matrix< T, MemoryBlock > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< boost::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< boost::array< T, N > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< boost::multi_array< T, N, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< boost::multi_array< T, N, A > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::array< T, N > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::complex< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::complex< T > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::pair< T *, std::vector< std::size_t > > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::pair< T *, std::vector< std::size_t > > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::valarray< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::valarray< T > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::vector< bool, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::vector< bool, A > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::vector< T, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< std::vector< T, A > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::get_pointer< T const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_datatype_caller` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_datatype_impl_compare` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_datatype_impl_compare< std::string >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< alps::multi_array< T, N, A > >` 

```
struct alps::hdf5::detail::is_vectorizable< alps::multi_array< T, N, A > >
  : public alps::hdf5::detail::is_vectorizable< boost::multi_array< T, N, A > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< alps::numeric::matrix< T, MemoryBlock > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< alps::python::numpy::array >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< boost::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< boost::multi_array< T, N, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< boost::python::list >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< boost::python::object >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< boost::python::tuple >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< std::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< std::complex< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< std::complex< T > const >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< std::pair< T *, std::vector< std::size_t > > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< std::valarray< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< std::vector< bool, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::is_vectorizable< std::vector< T, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::load_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::load_helper< N, T, boost::true_type >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::make_pvp_proxy` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public std::string `[`path_`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy_1ac3f0e269ed4152a43979353515453726) | 
`public T `[`value_`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy_1ae690d40c37cf582558687b3f66de5eda) | 
`public inline  explicit `[`make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy_1a3ac9feb58dcd4352854c13571c7b01e6)`(std::string const & path,T value)` | 
`public inline  `[`make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy_1a4456bc16df69e92d7b2d8ae4ad5652e3)`(`[`make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T > const & arg)` | 

## Members

#### `public std::string `[`path_`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy_1ac3f0e269ed4152a43979353515453726) 

#### `public T `[`value_`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy_1ae690d40c37cf582558687b3f66de5eda) 

#### `public inline  explicit `[`make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy_1a3ac9feb58dcd4352854c13571c7b01e6)`(std::string const & path,T value)` 

#### `public inline  `[`make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy_1a4456bc16df69e92d7b2d8ae4ad5652e3)`(`[`make_pvp_proxy`](#de/db3/structalps_1_1hdf5_1_1detail_1_1make__pvp__proxy)`< T > const & arg)` 

# struct `alps::hdf5::detail::native_ptr_converter` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`native_ptr_converter`](#d8/dd2/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_1a607b215ddfb4d29a0cf0ba6ea3872622)`(std::size_t)` | 
`public inline T const * `[`apply`](#d8/dd2/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_1a74e7e964d8e255974f703f27b7311212)`(T const * v)` | 

## Members

#### `public inline  `[`native_ptr_converter`](#d8/dd2/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_1a607b215ddfb4d29a0cf0ba6ea3872622)`(std::size_t)` 

#### `public inline T const * `[`apply`](#d8/dd2/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_1a74e7e964d8e255974f703f27b7311212)`(T const * v)` 

# struct `alps::hdf5::detail::native_ptr_converter< std::string >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public std::vector< char const * > `[`data`](#de/d98/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_3_01std_1_1string_01_4_1a9e8ff13db3372dd1edce95e66b39983c) | 
`public inline  `[`native_ptr_converter`](#de/d98/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_3_01std_1_1string_01_4_1aaa79441bcedf4db2b76f6375df5cc1fe)`(std::size_t size)` | 
`public inline char const *const * `[`apply`](#de/d98/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_3_01std_1_1string_01_4_1ab7c52e6765ca6410244ea4589fb59cc6)`(std::string const * v)` | 

## Members

#### `public std::vector< char const * > `[`data`](#de/d98/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_3_01std_1_1string_01_4_1a9e8ff13db3372dd1edce95e66b39983c) 

#### `public inline  `[`native_ptr_converter`](#de/d98/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_3_01std_1_1string_01_4_1aaa79441bcedf4db2b76f6375df5cc1fe)`(std::size_t size)` 

#### `public inline char const *const * `[`apply`](#de/d98/structalps_1_1hdf5_1_1detail_1_1native__ptr__converter_3_01std_1_1string_01_4_1ab7c52e6765ca6410244ea4589fb59cc6)`(std::string const * v)` 

# struct `alps::hdf5::detail::save_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::save_helper< N, T, boost::true_type >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::save_python_object_visitor` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & `[`_ar`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a4eae157fbcd080f54705f9e8c3e3f7f7) | 
`public std::string const  & `[`_path`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a17c502c78c981c16b2be22a13534efdc) | 
`public std::vector< std::size_t > `[`_size`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a9723afd8a369acdbe53e9796bb052347) | 
`public std::vector< std::size_t > `[`_chunk`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a7414dd4f76b11e4042f17506a12d5fc8) | 
`public std::vector< std::size_t > `[`_offset`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a220f4a1fe911221d307994c365f59df5) | 
`public inline  `[`save_python_object_visitor`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1ac88260a7f953267769b459737ce6a491)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a35212baafef7f19120442bb47d979a81)`(T const & value)` | 
`public template<>`  <br/>`inline void `[`operator()`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a40d70691efd7332653cf477adbfed42d)`(T const *,std::vector< std::size_t >)` | 

## Members

#### `public `[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & `[`_ar`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a4eae157fbcd080f54705f9e8c3e3f7f7) 

#### `public std::string const  & `[`_path`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a17c502c78c981c16b2be22a13534efdc) 

#### `public std::vector< std::size_t > `[`_size`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a9723afd8a369acdbe53e9796bb052347) 

#### `public std::vector< std::size_t > `[`_chunk`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a7414dd4f76b11e4042f17506a12d5fc8) 

#### `public std::vector< std::size_t > `[`_offset`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a220f4a1fe911221d307994c365f59df5) 

#### `public inline  `[`save_python_object_visitor`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1ac88260a7f953267769b459737ce6a491)`(`[`archive`](#df/d24/classalps_1_1hdf5_1_1archive)` & ar,std::string const & path,std::vector< std::size_t > size,std::vector< std::size_t > chunk,std::vector< std::size_t > offset)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a35212baafef7f19120442bb47d979a81)`(T const & value)` 

#### `public template<>`  <br/>`inline void `[`operator()`](#d1/d82/structalps_1_1hdf5_1_1detail_1_1save__python__object__visitor_1a40d70691efd7332653cf477adbfed42d)`(T const *,std::vector< std::size_t >)` 

# struct `alps::hdf5::detail::set_extent` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< alps::multi_array< T, N, A > >` 

```
struct alps::hdf5::detail::set_extent< alps::multi_array< T, N, A > >
  : public alps::hdf5::detail::set_extent< boost::multi_array< T, N, A > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< alps::numeric::matrix< T, MemoryBlock > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< alps::python::numpy::array >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< boost::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< boost::multi_array< T, N, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< boost::python::list >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< boost::python::object >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< std::array< T, N > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< std::complex< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< std::pair< T *, std::vector< std::size_t > > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< std::valarray< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< std::vector< bool, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::hdf5::detail::set_extent< std::vector< T, A > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

Generated by [Moxygen](https://sourcey.com/moxygen)
