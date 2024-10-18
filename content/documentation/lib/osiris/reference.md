

---
title: Reference
description: "ALPS Osiris Library"
weight: 2
---

# Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`namespace `[`alps`](#d8/d3d/namespacealps) | 
`namespace `[`alps::detail`](#d6/d75/namespacealps_1_1detail) | 
`struct `[`netobj`](#df/d17/structnetobj) | 
`struct `[`XDR`](#da/d72/struct_x_d_r) | 
`struct `[`xdr_discrim`](#da/df0/structxdr__discrim) | 
`struct `[`XDR::xdr_ops`](#d1/d30/struct_x_d_r_1_1xdr__ops) | 

# namespace `alps` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public ALPS_DECL void `[`comm_init`](#d8/db4/comm_8h_1acd549951655b6c7a066927f95c14a51b)`(int & argc,char **& argv,bool)`            | 
`public ALPS_DECL void `[`comm_exit`](#d8/db4/comm_8h_1af69e44eb8272bc9fcf00e9541a21a599)`(bool kill_slaves)`            | 
`public ALPS_DECL bool `[`runs_parallel`](#d8/db4/comm_8h_1a67e4c0dbffb1371041016bea8be62948)`()`            | 
`public ALPS_DECL bool `[`is_master`](#d8/db4/comm_8h_1a9fe7506fd8fcd47a532038b6eebe787b)`()`            | 
`public `[`Process`](#d9/daa/classalps_1_1_process)` `[`local_process`](#d8/db4/comm_8h_1a1016de2f3bc4b54bef48fad97006a93c)`()`            | 
`public ProcessList `[`all_processes`](#d8/db4/comm_8h_1afb9d8e80e8320912dd5b0b25185ed981)`()`            | 
`public `[`Process`](#d9/daa/classalps_1_1_process)` `[`master_process`](#d8/db4/comm_8h_1aca29c9eaf8b3d3bcefe5682ef0e6ee5d)`()`            | 
`public template<>`  <br/>[`ODump`](#d3/db8/classalps_1_1_o_dump)` & `[`operator<<`](#d5/de5/dump_8h_1a4cd77f6e8a83061a79ff1453e2ee6e39)`(`[`ODump`](#d3/db8/classalps_1_1_o_dump)` & d,const T & x)`            | 
`public template<>`  <br/>[`ODump`](#d3/db8/classalps_1_1_o_dump)` & `[`operator<<`](#d5/de5/dump_8h_1acec0a6498df1480027d6b8b72ec4d9f6)`(`[`ODump`](#d3/db8/classalps_1_1_o_dump)` & d,const std::complex< T > & x)`            | 
`public template<>`  <br/>[`IDump`](#d1/d80/classalps_1_1_i_dump)` & `[`operator>>`](#d5/de5/dump_8h_1a5cfff5938a21d828dcd101e1ed27a18e)`(`[`IDump`](#d1/d80/classalps_1_1_i_dump)` & d,T & x)`            | 
`public template<>`  <br/>[`IDump`](#d1/d80/classalps_1_1_i_dump)` & `[`operator>>`](#d5/de5/dump_8h_1aa77ba2818260d2c0e51b854c152c2167)`(`[`IDump`](#d1/d80/classalps_1_1_i_dump)` & d,std::complex< T > & x)`            | 
`public template<>`  <br/>`T `[`get`](#d3/df3/dumparchive_8h_1a84ec516b9e2b9a62c0bcf57ee12a1d40)`(ARCHIVE & ar)`            | 
`public inline std::ostream & `[`operator<<`](#da/d42/process_8h_1a31d7cc4bb4dd8f5638beee21a64123e0)`(std::ostream & out,const `[`alps::Process`](#d9/daa/classalps_1_1_process)` & p)`            | 
`class `[`alps::archive_idump`](#de/de5/classalps_1_1archive__idump) | A class to use a Boost input archive as an Osiris dump
`class `[`alps::archive_odump`](#d8/d6c/classalps_1_1archive__odump) | A class to use a Boost output archive as an Osiris dump
`class `[`alps::IDump`](#d1/d80/classalps_1_1_i_dump) | 
`class `[`alps::idump_archive`](#d0/d5a/classalps_1_1idump__archive) | 
`class `[`alps::IMPDump`](#d1/d8c/classalps_1_1_i_m_p_dump) | 
`class `[`alps::IXDRDump`](#d4/d8e/classalps_1_1_i_x_d_r_dump) | The abstract base class for deserializing an object using the [XDR](#da/d72/struct_x_d_r) stream library to read the architecture indepedent [XDR](#da/d72/struct_x_d_r) format.
`class `[`alps::IXDRFileDump`](#d4/d0a/classalps_1_1_i_x_d_r_file_dump) | a dump for deserializing objects from a file using the [XDR](#da/d72/struct_x_d_r) format.
`class `[`alps::ODump`](#d3/db8/classalps_1_1_o_dump) | 
`class `[`alps::odump_archive`](#d0/d6d/classalps_1_1odump__archive) | 
`class `[`alps::OMPDump`](#dd/dab/classalps_1_1_o_m_p_dump) | 
`class `[`alps::OXDRDump`](#df/de2/classalps_1_1_o_x_d_r_dump) | The abstract base class for serializing an object using the [XDR](#da/d72/struct_x_d_r) stream library to write the architecture indepedent [XDR](#da/d72/struct_x_d_r) format.
`class `[`alps::OXDRFileDump`](#d1/d41/classalps_1_1_o_x_d_r_file_dump) | a dump for serializing objects into a file using the [XDR](#da/d72/struct_x_d_r) format.
`class `[`alps::Process`](#d9/daa/classalps_1_1_process) | a process descriptor.

## Members

#### `public ALPS_DECL void `[`comm_init`](#d8/db4/comm_8h_1acd549951655b6c7a066927f95c14a51b)`(int & argc,char **& argv,bool)` 

#### `public ALPS_DECL void `[`comm_exit`](#d8/db4/comm_8h_1af69e44eb8272bc9fcf00e9541a21a599)`(bool kill_slaves)` 

#### `public ALPS_DECL bool `[`runs_parallel`](#d8/db4/comm_8h_1a67e4c0dbffb1371041016bea8be62948)`()` 

#### `public ALPS_DECL bool `[`is_master`](#d8/db4/comm_8h_1a9fe7506fd8fcd47a532038b6eebe787b)`()` 

#### `public `[`Process`](#d9/daa/classalps_1_1_process)` `[`local_process`](#d8/db4/comm_8h_1a1016de2f3bc4b54bef48fad97006a93c)`()` 

#### `public ProcessList `[`all_processes`](#d8/db4/comm_8h_1afb9d8e80e8320912dd5b0b25185ed981)`()` 

#### `public `[`Process`](#d9/daa/classalps_1_1_process)` `[`master_process`](#d8/db4/comm_8h_1aca29c9eaf8b3d3bcefe5682ef0e6ee5d)`()` 

#### `public template<>`  <br/>[`ODump`](#d3/db8/classalps_1_1_o_dump)` & `[`operator<<`](#d5/de5/dump_8h_1a4cd77f6e8a83061a79ff1453e2ee6e39)`(`[`ODump`](#d3/db8/classalps_1_1_o_dump)` & d,const T & x)` 

#### `public template<>`  <br/>[`ODump`](#d3/db8/classalps_1_1_o_dump)` & `[`operator<<`](#d5/de5/dump_8h_1acec0a6498df1480027d6b8b72ec4d9f6)`(`[`ODump`](#d3/db8/classalps_1_1_o_dump)` & d,const std::complex< T > & x)` 

#### `public template<>`  <br/>[`IDump`](#d1/d80/classalps_1_1_i_dump)` & `[`operator>>`](#d5/de5/dump_8h_1a5cfff5938a21d828dcd101e1ed27a18e)`(`[`IDump`](#d1/d80/classalps_1_1_i_dump)` & d,T & x)` 

#### `public template<>`  <br/>[`IDump`](#d1/d80/classalps_1_1_i_dump)` & `[`operator>>`](#d5/de5/dump_8h_1aa77ba2818260d2c0e51b854c152c2167)`(`[`IDump`](#d1/d80/classalps_1_1_i_dump)` & d,std::complex< T > & x)` 

#### `public template<>`  <br/>`T `[`get`](#d3/df3/dumparchive_8h_1a84ec516b9e2b9a62c0bcf57ee12a1d40)`(ARCHIVE & ar)` 

#### `public inline std::ostream & `[`operator<<`](#da/d42/process_8h_1a31d7cc4bb4dd8f5638beee21a64123e0)`(std::ostream & out,const `[`alps::Process`](#d9/daa/classalps_1_1_process)` & p)` 

# class `alps::archive_idump` 

```
class alps::archive_idump
  : public alps::IDump
```  

A class to use a Boost input archive as an Osiris dump

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`archive_idump`](#de/de5/classalps_1_1archive__idump_1a2ffc338a60bf1fed5ebc954f15845f3d)`(ARCHIVE & a)` | 
`public inline  `[`~archive_idump`](#de/de5/classalps_1_1archive__idump_1a485300c340d495dcf9b2ec603ed38ae4)`()` | 
`public inline virtual void `[`read_string`](#de/de5/classalps_1_1archive__idump_1ac446f931f93ec2f02cb070c9233c4643)`(std::size_t,char * s)` | 
`public inline virtual void `[`read_string`](#de/de5/classalps_1_1archive__idump_1a71e48856cb38a3f995b5c1109770b983)`(std::string & s)` | 

## Members

#### `public inline  `[`archive_idump`](#de/de5/classalps_1_1archive__idump_1a2ffc338a60bf1fed5ebc954f15845f3d)`(ARCHIVE & a)` 

#### `public inline  `[`~archive_idump`](#de/de5/classalps_1_1archive__idump_1a485300c340d495dcf9b2ec603ed38ae4)`()` 

#### `public inline virtual void `[`read_string`](#de/de5/classalps_1_1archive__idump_1ac446f931f93ec2f02cb070c9233c4643)`(std::size_t,char * s)` 

#### `public inline virtual void `[`read_string`](#de/de5/classalps_1_1archive__idump_1a71e48856cb38a3f995b5c1109770b983)`(std::string & s)` 

# class `alps::archive_odump` 

```
class alps::archive_odump
  : public alps::ODump
```  

A class to use a Boost output archive as an Osiris dump

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`archive_odump`](#d8/d6c/classalps_1_1archive__odump_1afee796801291d8d580df122eaf839e77)`(ARCHIVE & a)` | 
`public inline  `[`~archive_odump`](#d8/d6c/classalps_1_1archive__odump_1a47a9243f6f9d1ff04b5e32115d6e3d77)`()` | 
`public inline virtual void `[`write_string`](#d8/d6c/classalps_1_1archive__odump_1ac4ced39ce44137900def0f5f2712b9ed)`(std::size_t,const char * x)` | 
`public inline virtual void `[`write_string`](#d8/d6c/classalps_1_1archive__odump_1a433563567fcac6c72b95708bfd88ad10)`(const std::string & s)` | 

## Members

#### `public inline  `[`archive_odump`](#d8/d6c/classalps_1_1archive__odump_1afee796801291d8d580df122eaf839e77)`(ARCHIVE & a)` 

#### `public inline  `[`~archive_odump`](#d8/d6c/classalps_1_1archive__odump_1a47a9243f6f9d1ff04b5e32115d6e3d77)`()` 

#### `public inline virtual void `[`write_string`](#d8/d6c/classalps_1_1archive__odump_1ac4ced39ce44137900def0f5f2712b9ed)`(std::size_t,const char * x)` 

#### `public inline virtual void `[`write_string`](#d8/d6c/classalps_1_1archive__odump_1a433563567fcac6c72b95708bfd88ad10)`(const std::string & s)` 

# class `alps::IDump` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`IDump`](#d1/d80/classalps_1_1_i_dump_1ac95d375e4c16e1d5a830780b0e3548af)`(uint32_t v)` | 
`public inline virtual  `[`~IDump`](#d1/d80/classalps_1_1_i_dump_1a3f833f65aac5b0780a309470d9b19a3d)`()` | 
`public inline uint32_t `[`version`](#d1/d80/classalps_1_1_i_dump_1ad56d39f8c700e47c78e14c375cc0f576)`() const` | 
`public inline void `[`set_version`](#d1/d80/classalps_1_1_i_dump_1aa52b66b5ff01ce1b8785801be7cebe1d)`(uint32_t v)` | 
`public void `[`read_simple`](#d1/d80/classalps_1_1_i_dump_1a64159cc5b8a7315a67810a473fe36e9d)`(int & x)` | 
`public void `[`read_simple`](#d1/d80/classalps_1_1_i_dump_1afc8fa84ad7a4caab8f884078f36efb75)`(double & x)` | 
`public template<>`  <br/>`inline void `[`read_complex`](#d1/d80/classalps_1_1_i_dump_1a4ba7a64edb0364c5b3786826837c7012)`(std::complex< T > & x)` | 
`public template<>`  <br/>`inline `[`IDump`](#d1/d80/classalps_1_1_i_dump)` & `[`load`](#d1/d80/classalps_1_1_i_dump_1a1e82fc52f8ee6940dbf952fa25ece6e4)`(T & x)` | 
`public template<>`  <br/>`inline `[`IDump`](#d1/d80/classalps_1_1_i_dump)` & `[`load`](#d1/d80/classalps_1_1_i_dump_1a731405efa4fab5950550a07fb6c2b27e)`(std::complex< T > & x)` | 
`public template<>`  <br/>`inline void `[`read_array`](#d1/d80/classalps_1_1_i_dump_1a7a95eb77b18bcd14dc1e93fb77721cf0)`(std::size_t n,std::complex< T > * p)` | 
`public virtual void `[`read_string`](#d1/d80/classalps_1_1_i_dump_1adc0609147381bd15cba2cf2817cf9d28)`(std::size_t n,char * s)` | 
`public virtual void `[`read_string`](#d1/d80/classalps_1_1_i_dump_1af877cb1ec275c4bd3d1d7a1b06fdbbbe)`(std::string &)` | 
`public template<>`  <br/>`inline  `[`operator std::complex< T >`](#d1/d80/classalps_1_1_i_dump_1ab23b01457f1cbd86745e6b9a1bba8654)`()` | 
`public template<>`  <br/>`inline T `[`get`](#d1/d80/classalps_1_1_i_dump_1afb78812cae50e3f0e385ca5638476e9d)`()` | 
`public inline bool `[`test`](#d1/d80/classalps_1_1_i_dump_1a2adca766b47cc879d9de21048248f0fd)`()` | 

## Members

#### `public  `[`IDump`](#d1/d80/classalps_1_1_i_dump_1ac95d375e4c16e1d5a830780b0e3548af)`(uint32_t v)` 

#### `public inline virtual  `[`~IDump`](#d1/d80/classalps_1_1_i_dump_1a3f833f65aac5b0780a309470d9b19a3d)`()` 

#### `public inline uint32_t `[`version`](#d1/d80/classalps_1_1_i_dump_1ad56d39f8c700e47c78e14c375cc0f576)`() const` 

#### `public inline void `[`set_version`](#d1/d80/classalps_1_1_i_dump_1aa52b66b5ff01ce1b8785801be7cebe1d)`(uint32_t v)` 

#### `public void `[`read_simple`](#d1/d80/classalps_1_1_i_dump_1a64159cc5b8a7315a67810a473fe36e9d)`(int & x)` 

#### `public void `[`read_simple`](#d1/d80/classalps_1_1_i_dump_1afc8fa84ad7a4caab8f884078f36efb75)`(double & x)` 

#### `public template<>`  <br/>`inline void `[`read_complex`](#d1/d80/classalps_1_1_i_dump_1a4ba7a64edb0364c5b3786826837c7012)`(std::complex< T > & x)` 

#### `public template<>`  <br/>`inline `[`IDump`](#d1/d80/classalps_1_1_i_dump)` & `[`load`](#d1/d80/classalps_1_1_i_dump_1a1e82fc52f8ee6940dbf952fa25ece6e4)`(T & x)` 

#### `public template<>`  <br/>`inline `[`IDump`](#d1/d80/classalps_1_1_i_dump)` & `[`load`](#d1/d80/classalps_1_1_i_dump_1a731405efa4fab5950550a07fb6c2b27e)`(std::complex< T > & x)` 

#### `public template<>`  <br/>`inline void `[`read_array`](#d1/d80/classalps_1_1_i_dump_1a7a95eb77b18bcd14dc1e93fb77721cf0)`(std::size_t n,std::complex< T > * p)` 

#### `public virtual void `[`read_string`](#d1/d80/classalps_1_1_i_dump_1adc0609147381bd15cba2cf2817cf9d28)`(std::size_t n,char * s)` 

#### `public virtual void `[`read_string`](#d1/d80/classalps_1_1_i_dump_1af877cb1ec275c4bd3d1d7a1b06fdbbbe)`(std::string &)` 

#### `public template<>`  <br/>`inline  `[`operator std::complex< T >`](#d1/d80/classalps_1_1_i_dump_1ab23b01457f1cbd86745e6b9a1bba8654)`()` 

#### `public template<>`  <br/>`inline T `[`get`](#d1/d80/classalps_1_1_i_dump_1afb78812cae50e3f0e385ca5638476e9d)`()` 

#### `public inline bool `[`test`](#d1/d80/classalps_1_1_i_dump_1a2adca766b47cc879d9de21048248f0fd)`()` 

# class `alps::idump_archive` 

```
class alps::idump_archive
  : public boost::archive::detail::common_iarchive< idump_archive >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`idump_archive`](#d0/d5a/classalps_1_1idump__archive_1acb0c1fd6615169fe3701be53759b5be1)`(`[`IDump`](#d1/d80/classalps_1_1_i_dump)` & d,bool c)` | 
`public inline void `[`load_binary`](#d0/d5a/classalps_1_1idump__archive_1a877330ebdf2f1992a4a3e28100af725a)`(void * address,size_t count)` | 
`public template<>`  <br/>`void `[`load`](#d0/d5a/classalps_1_1idump__archive_1a30fe59ba5ce2c7e3a10ac7566e7ffa3b)`(T & t)` | 
`public inline void `[`load`](#d0/d5a/classalps_1_1idump__archive_1a316a1e5c5e215e4171133545889ef930)`(std::string & s)` | 
`public template<>`  <br/>`inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a3007134696bdb399bd44462d9d9c2c4a)`(T & t,BOOST_PFTO int)` | 
`public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1aef0ad08541c38fe3147786a705494802)`(boost::archive::class_id_optional_type &,int)` | 
`public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a0e7d88551aed2fc7bc53a316c14e2150)`(boost::archive::version_type & t,int)` | 
`public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a1f737e0d16f737aee2fe90aac041051e)`(boost::archive::class_id_type & t,int)` | 
`public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a1f858365a2412e11c779b744609fb063)`(boost::archive::class_id_reference_type & t,int)` | 
`public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a89b8a91a34c7808c724ad176e6bfcd31)`(boost::archive::object_id_type & t,int)` | 
`public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a9d575b03c9d2c48b5024d540fa077110)`(boost::archive::object_reference_type & t,int)` | 
`public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1aeff28db7fc88ea878ce99e56a5a8b567)`(boost::archive::tracking_type & t,int)` | 
`public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1ad3203557393b90bd70680efcb45053e9)`(boost::archive::class_name_type & t,int)` | 

## Members

#### `public inline  `[`idump_archive`](#d0/d5a/classalps_1_1idump__archive_1acb0c1fd6615169fe3701be53759b5be1)`(`[`IDump`](#d1/d80/classalps_1_1_i_dump)` & d,bool c)` 

#### `public inline void `[`load_binary`](#d0/d5a/classalps_1_1idump__archive_1a877330ebdf2f1992a4a3e28100af725a)`(void * address,size_t count)` 

#### `public template<>`  <br/>`void `[`load`](#d0/d5a/classalps_1_1idump__archive_1a30fe59ba5ce2c7e3a10ac7566e7ffa3b)`(T & t)` 

#### `public inline void `[`load`](#d0/d5a/classalps_1_1idump__archive_1a316a1e5c5e215e4171133545889ef930)`(std::string & s)` 

#### `public template<>`  <br/>`inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a3007134696bdb399bd44462d9d9c2c4a)`(T & t,BOOST_PFTO int)` 

#### `public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1aef0ad08541c38fe3147786a705494802)`(boost::archive::class_id_optional_type &,int)` 

#### `public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a0e7d88551aed2fc7bc53a316c14e2150)`(boost::archive::version_type & t,int)` 

#### `public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a1f737e0d16f737aee2fe90aac041051e)`(boost::archive::class_id_type & t,int)` 

#### `public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a1f858365a2412e11c779b744609fb063)`(boost::archive::class_id_reference_type & t,int)` 

#### `public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a89b8a91a34c7808c724ad176e6bfcd31)`(boost::archive::object_id_type & t,int)` 

#### `public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1a9d575b03c9d2c48b5024d540fa077110)`(boost::archive::object_reference_type & t,int)` 

#### `public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1aeff28db7fc88ea878ce99e56a5a8b567)`(boost::archive::tracking_type & t,int)` 

#### `public inline void `[`load_override`](#d0/d5a/classalps_1_1idump__archive_1ad3203557393b90bd70680efcb45053e9)`(boost::archive::class_name_type & t,int)` 

# class `alps::IMPDump` 

```
class alps::IMPDump
  : public alps::IDump
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`IMPDump`](#d1/d8c/classalps_1_1_i_m_p_dump_1a00ff2f5909e7f1263fd83341d3c5964f)`()` | 
`public  `[`IMPDump`](#d1/d8c/classalps_1_1_i_m_p_dump_1ac42bcb79640518e6e35fa27c0f3b8dc7)`(int32_t t)` | 
`public  `[`IMPDump`](#d1/d8c/classalps_1_1_i_m_p_dump_1a2df5b35fedd70eacd51c6318fa4240c5)`(const `[`Process`](#d9/daa/classalps_1_1_process)` &,int32_t t)` | 
`public void `[`init`](#d1/d8c/classalps_1_1_i_m_p_dump_1a58da73c3ad16499c6dddb9ccf52ff9f0)`()` | 
`public const `[`Process`](#d9/daa/classalps_1_1_process)` & `[`sender`](#d1/d8c/classalps_1_1_i_m_p_dump_1acdd2fbb37f14df2ebd282b351c32cbf1)`() const` | 
`public void `[`receive`](#d1/d8c/classalps_1_1_i_m_p_dump_1a710525fd8839a90252e11d345020fb6c)`(const `[`Process`](#d9/daa/classalps_1_1_process)` & w,int32_t t)` | 
`public void `[`receive`](#d1/d8c/classalps_1_1_i_m_p_dump_1ad79c8f6e5d431928f20f795282e928c3)`(int32_t t)` | 
`public void `[`broadcast`](#d1/d8c/classalps_1_1_i_m_p_dump_1ade94acd4689c2c57c6bbe997980a80f6)`(const `[`alps::Process`](#d9/daa/classalps_1_1_process)` & sender)` | 
`public virtual void `[`read_string`](#d1/d8c/classalps_1_1_i_m_p_dump_1a1cdb6c25593c4f759ec4348d39f98c80)`(std::size_t,char *)` | 

## Members

#### `public  `[`IMPDump`](#d1/d8c/classalps_1_1_i_m_p_dump_1a00ff2f5909e7f1263fd83341d3c5964f)`()` 

#### `public  `[`IMPDump`](#d1/d8c/classalps_1_1_i_m_p_dump_1ac42bcb79640518e6e35fa27c0f3b8dc7)`(int32_t t)` 

#### `public  `[`IMPDump`](#d1/d8c/classalps_1_1_i_m_p_dump_1a2df5b35fedd70eacd51c6318fa4240c5)`(const `[`Process`](#d9/daa/classalps_1_1_process)` &,int32_t t)` 

#### `public void `[`init`](#d1/d8c/classalps_1_1_i_m_p_dump_1a58da73c3ad16499c6dddb9ccf52ff9f0)`()` 

#### `public const `[`Process`](#d9/daa/classalps_1_1_process)` & `[`sender`](#d1/d8c/classalps_1_1_i_m_p_dump_1acdd2fbb37f14df2ebd282b351c32cbf1)`() const` 

#### `public void `[`receive`](#d1/d8c/classalps_1_1_i_m_p_dump_1a710525fd8839a90252e11d345020fb6c)`(const `[`Process`](#d9/daa/classalps_1_1_process)` & w,int32_t t)` 

#### `public void `[`receive`](#d1/d8c/classalps_1_1_i_m_p_dump_1ad79c8f6e5d431928f20f795282e928c3)`(int32_t t)` 

#### `public void `[`broadcast`](#d1/d8c/classalps_1_1_i_m_p_dump_1ade94acd4689c2c57c6bbe997980a80f6)`(const `[`alps::Process`](#d9/daa/classalps_1_1_process)` & sender)` 

#### `public virtual void `[`read_string`](#d1/d8c/classalps_1_1_i_m_p_dump_1a1cdb6c25593c4f759ec4348d39f98c80)`(std::size_t,char *)` 

# class `alps::IXDRDump` 

```
class alps::IXDRDump
  : public alps::IDump
```  

The abstract base class for deserializing an object using the [XDR](#da/d72/struct_x_d_r) stream library to read the architecture indepedent [XDR](#da/d72/struct_x_d_r) format.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`IXDRDump`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1a2dc1fc0864f2ea92f3829dd16fd41824)`()` | 
`public inline virtual  `[`~IXDRDump`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1aae8e98a6a9396c8470bc8e5fff7ba213)`()` | 
`public virtual void `[`read_string`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1aa94a9569cdf46d78907a5efe364f5802)`(std::size_t n,char * s)` | 
`protected `[`XDR`](#da/d72/struct_x_d_r)` `[`xdr_`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1a389a168095a1e4231178bac9e819d6c2) | 
`protected uint32_t `[`getPosition`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1a25cc4219137f62f09e39c85e365de3a4)`() const` | get the position in the [XDR](#da/d72/struct_x_d_r) stream.
`protected void `[`setPosition`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1af4fdbef4cd92b8891448821f8c881bb0)`(uint32_t pos)` | set the position in the [XDR](#da/d72/struct_x_d_r) stream.

## Members

#### `public inline  `[`IXDRDump`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1a2dc1fc0864f2ea92f3829dd16fd41824)`()` 

#### `public inline virtual  `[`~IXDRDump`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1aae8e98a6a9396c8470bc8e5fff7ba213)`()` 

#### `public virtual void `[`read_string`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1aa94a9569cdf46d78907a5efe364f5802)`(std::size_t n,char * s)` 

#### `protected `[`XDR`](#da/d72/struct_x_d_r)` `[`xdr_`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1a389a168095a1e4231178bac9e819d6c2) 

#### `protected uint32_t `[`getPosition`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1a25cc4219137f62f09e39c85e365de3a4)`() const` 

get the position in the [XDR](#da/d72/struct_x_d_r) stream.

#### `protected void `[`setPosition`](#d4/d8e/classalps_1_1_i_x_d_r_dump_1af4fdbef4cd92b8891448821f8c881bb0)`(uint32_t pos)` 

set the position in the [XDR](#da/d72/struct_x_d_r) stream.

# class `alps::IXDRFileDump` 

```
class alps::IXDRFileDump
  : public alps::IXDRDump
```  

a dump for deserializing objects from a file using the [XDR](#da/d72/struct_x_d_r) format.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`IXDRFileDump`](#d4/d0a/classalps_1_1_i_x_d_r_file_dump_1aa04ae56554cbeb04757a0ad6c981b539)`(const boost::filesystem::path & name)` | open a file. 
`public inline bool `[`couldOpen`](#d4/d0a/classalps_1_1_i_x_d_r_file_dump_1a54483949e4cfab58252980c5014caa3e)`()` | 
`public virtual  `[`~IXDRFileDump`](#d4/d0a/classalps_1_1_i_x_d_r_file_dump_1ae1f9ddcd157761309911064963f0e51f)`()` | 

## Members

#### `public  `[`IXDRFileDump`](#d4/d0a/classalps_1_1_i_x_d_r_file_dump_1aa04ae56554cbeb04757a0ad6c981b539)`(const boost::filesystem::path & name)` 

open a file. 
#### Exceptions
* `std::runtime_error` if the file could not be openend.

#### `public inline bool `[`couldOpen`](#d4/d0a/classalps_1_1_i_x_d_r_file_dump_1a54483949e4cfab58252980c5014caa3e)`()` 

#### `public virtual  `[`~IXDRFileDump`](#d4/d0a/classalps_1_1_i_x_d_r_file_dump_1ae1f9ddcd157761309911064963f0e51f)`()` 

# class `alps::ODump` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`ODump`](#d3/db8/classalps_1_1_o_dump_1a7f6d62758c79fd8859c272b09b05bc4a)`(uint32_t v)` | 
`public inline virtual  `[`~ODump`](#d3/db8/classalps_1_1_o_dump_1a3f6635882af9193c13ecb04768aa79e9)`()` | 
`public inline uint32_t `[`version`](#d3/db8/classalps_1_1_o_dump_1a148aa23a23ee22efec89e23dc7ba85c6)`() const` | 
`public void `[`write_simple`](#d3/db8/classalps_1_1_o_dump_1ab7fdc6b528d0e4c41c5a6eedd19ca790)`(int x)` | 
`public void `[`write_simple`](#d3/db8/classalps_1_1_o_dump_1a78d1eb7d123d6f96b98d2962a17c8654)`(double x)` | 
`public template<>`  <br/>`inline void `[`write_complex`](#d3/db8/classalps_1_1_o_dump_1a56517fb9ec88ed2c807e4a395906b69f)`(const std::complex< T > & x)` | 
`public template<>`  <br/>`inline `[`ODump`](#d3/db8/classalps_1_1_o_dump)` & `[`store`](#d3/db8/classalps_1_1_o_dump_1abbf57f369b10d230382fbc0b8bd97f90)`(const T & x)` | 
`public template<>`  <br/>`inline `[`ODump`](#d3/db8/classalps_1_1_o_dump)` & `[`store`](#d3/db8/classalps_1_1_o_dump_1a5712addee5ff3c24af04d608cdc9bb7f)`(const std::complex< T > & x)` | 
`public template<>`  <br/>`inline void `[`write_array`](#d3/db8/classalps_1_1_o_dump_1a6639a4bbb26ad85d0d885f66e20b1988)`(std::size_t n,const std::complex< T > * p)` | 
`public virtual void `[`write_string`](#d3/db8/classalps_1_1_o_dump_1ac5d05437cb8dd40faa1fa0c605ced022)`(std::size_t n,const char * s)` | 
`public virtual void `[`write_string`](#d3/db8/classalps_1_1_o_dump_1a4763da0632512ad47bdd57f3384e27a1)`(const std::string &)` | 

## Members

#### `public  `[`ODump`](#d3/db8/classalps_1_1_o_dump_1a7f6d62758c79fd8859c272b09b05bc4a)`(uint32_t v)` 

#### `public inline virtual  `[`~ODump`](#d3/db8/classalps_1_1_o_dump_1a3f6635882af9193c13ecb04768aa79e9)`()` 

#### `public inline uint32_t `[`version`](#d3/db8/classalps_1_1_o_dump_1a148aa23a23ee22efec89e23dc7ba85c6)`() const` 

#### `public void `[`write_simple`](#d3/db8/classalps_1_1_o_dump_1ab7fdc6b528d0e4c41c5a6eedd19ca790)`(int x)` 

#### `public void `[`write_simple`](#d3/db8/classalps_1_1_o_dump_1a78d1eb7d123d6f96b98d2962a17c8654)`(double x)` 

#### `public template<>`  <br/>`inline void `[`write_complex`](#d3/db8/classalps_1_1_o_dump_1a56517fb9ec88ed2c807e4a395906b69f)`(const std::complex< T > & x)` 

#### `public template<>`  <br/>`inline `[`ODump`](#d3/db8/classalps_1_1_o_dump)` & `[`store`](#d3/db8/classalps_1_1_o_dump_1abbf57f369b10d230382fbc0b8bd97f90)`(const T & x)` 

#### `public template<>`  <br/>`inline `[`ODump`](#d3/db8/classalps_1_1_o_dump)` & `[`store`](#d3/db8/classalps_1_1_o_dump_1a5712addee5ff3c24af04d608cdc9bb7f)`(const std::complex< T > & x)` 

#### `public template<>`  <br/>`inline void `[`write_array`](#d3/db8/classalps_1_1_o_dump_1a6639a4bbb26ad85d0d885f66e20b1988)`(std::size_t n,const std::complex< T > * p)` 

#### `public virtual void `[`write_string`](#d3/db8/classalps_1_1_o_dump_1ac5d05437cb8dd40faa1fa0c605ced022)`(std::size_t n,const char * s)` 

#### `public virtual void `[`write_string`](#d3/db8/classalps_1_1_o_dump_1a4763da0632512ad47bdd57f3384e27a1)`(const std::string &)` 

# class `alps::odump_archive` 

```
class alps::odump_archive
  : public boost::archive::detail::common_oarchive< odump_archive >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`odump_archive`](#d0/d6d/classalps_1_1odump__archive_1aa8071f4ddabaa8e7c6e143a19adbe39f)`(`[`ODump`](#d3/db8/classalps_1_1_o_dump)` & d,bool c)` | 
`public inline void `[`save_binary`](#d0/d6d/classalps_1_1odump__archive_1a9d1d3a076610d50c4ad22e28ccf7f6be)`(const void * address,size_t count)` | 
`public template<>`  <br/>`void `[`save`](#d0/d6d/classalps_1_1odump__archive_1a7ed30b450a88efda6b63e57ae7fc92dc)`(const T & t)` | 
`public template<>`  <br/>`inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1afbfe2b37ea60fc80e131c59e9efac5bb)`(const T & t,BOOST_PFTO int)` | 
`public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1ae046c81fc1c2feb9258dfb0a001dd37f)`(const boost::archive::class_id_optional_type &,int)` | 
`public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1a7afb174f87af9d3d31439f402996794b)`(const boost::archive::version_type & t,int)` | 
`public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1addd169273a483c4831668ea24d6bb511)`(const boost::archive::class_id_type & t,int)` | 
`public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1ac4d7834643776209c6391a433687000d)`(const boost::archive::class_id_reference_type & t,int)` | 
`public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1adeb928aa40f9a08803b31d5513cdd93e)`(const boost::archive::object_id_type & t,int)` | 
`public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1ae398d09def62c34bda454528af684e94)`(const boost::archive::object_reference_type & t,int)` | 
`public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1adb78a460d3f15082e3439cdeaceeeed2)`(const boost::archive::tracking_type & t,int)` | 
`public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1a3acd7ab1a741e0c0fd1cfad18471c605)`(const boost::archive::class_name_type & t,int)` | 

## Members

#### `public inline  `[`odump_archive`](#d0/d6d/classalps_1_1odump__archive_1aa8071f4ddabaa8e7c6e143a19adbe39f)`(`[`ODump`](#d3/db8/classalps_1_1_o_dump)` & d,bool c)` 

#### `public inline void `[`save_binary`](#d0/d6d/classalps_1_1odump__archive_1a9d1d3a076610d50c4ad22e28ccf7f6be)`(const void * address,size_t count)` 

#### `public template<>`  <br/>`void `[`save`](#d0/d6d/classalps_1_1odump__archive_1a7ed30b450a88efda6b63e57ae7fc92dc)`(const T & t)` 

#### `public template<>`  <br/>`inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1afbfe2b37ea60fc80e131c59e9efac5bb)`(const T & t,BOOST_PFTO int)` 

#### `public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1ae046c81fc1c2feb9258dfb0a001dd37f)`(const boost::archive::class_id_optional_type &,int)` 

#### `public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1a7afb174f87af9d3d31439f402996794b)`(const boost::archive::version_type & t,int)` 

#### `public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1addd169273a483c4831668ea24d6bb511)`(const boost::archive::class_id_type & t,int)` 

#### `public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1ac4d7834643776209c6391a433687000d)`(const boost::archive::class_id_reference_type & t,int)` 

#### `public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1adeb928aa40f9a08803b31d5513cdd93e)`(const boost::archive::object_id_type & t,int)` 

#### `public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1ae398d09def62c34bda454528af684e94)`(const boost::archive::object_reference_type & t,int)` 

#### `public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1adb78a460d3f15082e3439cdeaceeeed2)`(const boost::archive::tracking_type & t,int)` 

#### `public inline void `[`save_override`](#d0/d6d/classalps_1_1odump__archive_1a3acd7ab1a741e0c0fd1cfad18471c605)`(const boost::archive::class_name_type & t,int)` 

# class `alps::OMPDump` 

```
class alps::OMPDump
  : public alps::ODump
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`OMPDump`](#dd/dab/classalps_1_1_o_m_p_dump_1ab5dcc48e17e6477f3286e9c5fe272754)`()` | 
`public  `[`~OMPDump`](#dd/dab/classalps_1_1_o_m_p_dump_1a5c7c052ef5b967f721b1ac1e912ae92e)`()` | 
`public void `[`init`](#dd/dab/classalps_1_1_o_m_p_dump_1a53ba261853d9522313821afe299824c0)`()` | 
`public void `[`send`](#dd/dab/classalps_1_1_o_m_p_dump_1a1ea809d8cfdebd55e00738b2aaba59a4)`(const `[`Process`](#d9/daa/classalps_1_1_process)` &,int32_t tag)` | 
`public void `[`send`](#dd/dab/classalps_1_1_o_m_p_dump_1a7722701e4c2ccb7b2329956763acce3b)`(const ProcessList &,int32_t)` | 
`public void `[`broadcast`](#dd/dab/classalps_1_1_o_m_p_dump_1abbe9aba326dc60a73499e0289267b4b6)`(const `[`alps::Process`](#d9/daa/classalps_1_1_process)` & thisprocess)` | 
`public virtual void `[`write_string`](#dd/dab/classalps_1_1_o_m_p_dump_1a00aff5a115cc1d9fa7642a33ac4c68a2)`(std::size_t,const char *)` | 

## Members

#### `public  `[`OMPDump`](#dd/dab/classalps_1_1_o_m_p_dump_1ab5dcc48e17e6477f3286e9c5fe272754)`()` 

#### `public  `[`~OMPDump`](#dd/dab/classalps_1_1_o_m_p_dump_1a5c7c052ef5b967f721b1ac1e912ae92e)`()` 

#### `public void `[`init`](#dd/dab/classalps_1_1_o_m_p_dump_1a53ba261853d9522313821afe299824c0)`()` 

#### `public void `[`send`](#dd/dab/classalps_1_1_o_m_p_dump_1a1ea809d8cfdebd55e00738b2aaba59a4)`(const `[`Process`](#d9/daa/classalps_1_1_process)` &,int32_t tag)` 

#### `public void `[`send`](#dd/dab/classalps_1_1_o_m_p_dump_1a7722701e4c2ccb7b2329956763acce3b)`(const ProcessList &,int32_t)` 

#### `public void `[`broadcast`](#dd/dab/classalps_1_1_o_m_p_dump_1abbe9aba326dc60a73499e0289267b4b6)`(const `[`alps::Process`](#d9/daa/classalps_1_1_process)` & thisprocess)` 

#### `public virtual void `[`write_string`](#dd/dab/classalps_1_1_o_m_p_dump_1a00aff5a115cc1d9fa7642a33ac4c68a2)`(std::size_t,const char *)` 

# class `alps::OXDRDump` 

```
class alps::OXDRDump
  : public alps::ODump
```  

The abstract base class for serializing an object using the [XDR](#da/d72/struct_x_d_r) stream library to write the architecture indepedent [XDR](#da/d72/struct_x_d_r) format.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`OXDRDump`](#df/de2/classalps_1_1_o_x_d_r_dump_1a179856850ddcbd95902b896644addd58)`()` | 
`public inline virtual  `[`~OXDRDump`](#df/de2/classalps_1_1_o_x_d_r_dump_1a33c7bfa1e4ad83fe08a47c472faf8369)`()` | 
`public virtual void `[`write_string`](#df/de2/classalps_1_1_o_x_d_r_dump_1ac2d63e5711cbde2b3f1fa82e4cd9ca37)`(std::size_t,const char *)` | 
`protected `[`XDR`](#da/d72/struct_x_d_r)` `[`xdr_`](#df/de2/classalps_1_1_o_x_d_r_dump_1a8dfa2116debaac6273add50d147d872c) | 
`protected uint32_t `[`getPosition`](#df/de2/classalps_1_1_o_x_d_r_dump_1a7f465c0c563b60b7c547c0df379cb0e5)`() const` | get the position in the [XDR](#da/d72/struct_x_d_r) stream.
`protected void `[`setPosition`](#df/de2/classalps_1_1_o_x_d_r_dump_1a6a9dd4a2bb0b3bcdcd17a0ed70753410)`(uint32_t pos)` | set the position in the [XDR](#da/d72/struct_x_d_r) stream.

## Members

#### `public inline  `[`OXDRDump`](#df/de2/classalps_1_1_o_x_d_r_dump_1a179856850ddcbd95902b896644addd58)`()` 

#### `public inline virtual  `[`~OXDRDump`](#df/de2/classalps_1_1_o_x_d_r_dump_1a33c7bfa1e4ad83fe08a47c472faf8369)`()` 

#### `public virtual void `[`write_string`](#df/de2/classalps_1_1_o_x_d_r_dump_1ac2d63e5711cbde2b3f1fa82e4cd9ca37)`(std::size_t,const char *)` 

#### `protected `[`XDR`](#da/d72/struct_x_d_r)` `[`xdr_`](#df/de2/classalps_1_1_o_x_d_r_dump_1a8dfa2116debaac6273add50d147d872c) 

#### `protected uint32_t `[`getPosition`](#df/de2/classalps_1_1_o_x_d_r_dump_1a7f465c0c563b60b7c547c0df379cb0e5)`() const` 

get the position in the [XDR](#da/d72/struct_x_d_r) stream.

#### `protected void `[`setPosition`](#df/de2/classalps_1_1_o_x_d_r_dump_1a6a9dd4a2bb0b3bcdcd17a0ed70753410)`(uint32_t pos)` 

set the position in the [XDR](#da/d72/struct_x_d_r) stream.

# class `alps::OXDRFileDump` 

```
class alps::OXDRFileDump
  : public alps::OXDRDump
```  

a dump for serializing objects into a file using the [XDR](#da/d72/struct_x_d_r) format.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`OXDRFileDump`](#d1/d41/classalps_1_1_o_x_d_r_file_dump_1abd30406bb8dfea681df86e45a0e0fbc7)`(const boost::filesystem::path & name,bool append)` | open a new dump file with the given name
`public virtual  `[`~OXDRFileDump`](#d1/d41/classalps_1_1_o_x_d_r_file_dump_1a2521f3927079ee93cfb77fe8512a1f29)`()` | 
`public void `[`flush`](#d1/d41/classalps_1_1_o_x_d_r_file_dump_1aa1cf07fdf3cf491823128e57ed5c0b37)`()` | 

## Members

#### `public  `[`OXDRFileDump`](#d1/d41/classalps_1_1_o_x_d_r_file_dump_1abd30406bb8dfea681df86e45a0e0fbc7)`(const boost::filesystem::path & name,bool append)` 

open a new dump file with the given name

#### `public virtual  `[`~OXDRFileDump`](#d1/d41/classalps_1_1_o_x_d_r_file_dump_1a2521f3927079ee93cfb77fe8512a1f29)`()` 

#### `public void `[`flush`](#d1/d41/classalps_1_1_o_x_d_r_file_dump_1aa1cf07fdf3cf491823128e57ed5c0b37)`()` 

# class `alps::Process` 

a process descriptor.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  explicit `[`Process`](#d9/daa/classalps_1_1_process_1a611f764a490cd089b6c6efc4dbeb6da2)`(int)` | 
`public inline  `[`Process`](#d9/daa/classalps_1_1_process_1a7a4c2933eab25c082cf23b665be414a2)`()` | 
`public void `[`load`](#d9/daa/classalps_1_1_process_1a2202d78e43f8227f90b3d8cc2a5952be)`(`[`IDump`](#d1/d80/classalps_1_1_i_dump)` &)` | 
`public void `[`save`](#d9/daa/classalps_1_1_process_1adee1f9c3c5841e75074dce64e7b53b98)`(`[`ODump`](#d3/db8/classalps_1_1_o_dump)` &) const` | 
`public bool `[`valid`](#d9/daa/classalps_1_1_process_1a5708d077eeff86243b1d01f5f8df7a55)`() const` | 
`public bool `[`local`](#d9/daa/classalps_1_1_process_1a00abffa0c55b644d81da33ee24e58652)`() const` | 
`public inline  `[`operator int`](#d9/daa/classalps_1_1_process_1a2b0e92bcb7a4b1294716a99507982c39)`() const` | 
`public inline bool `[`operator==`](#d9/daa/classalps_1_1_process_1a6e3f588ca10b4cd364e3af4431b1ed57)`(const `[`Process`](#d9/daa/classalps_1_1_process)` & p) const` | 
`public inline bool `[`operator!=`](#d9/daa/classalps_1_1_process_1a6f74ae1bc88ef9573a0d0bf1da97e2f8)`(const `[`Process`](#d9/daa/classalps_1_1_process)` & p) const` | 
`public inline bool `[`operator<`](#d9/daa/classalps_1_1_process_1a4262148f340ec0e1aaf00a4a621f333a)`(const `[`Process`](#d9/daa/classalps_1_1_process)` & p) const` | sorting criterion for two processes?

## Members

#### `public  explicit `[`Process`](#d9/daa/classalps_1_1_process_1a611f764a490cd089b6c6efc4dbeb6da2)`(int)` 

#### `public inline  `[`Process`](#d9/daa/classalps_1_1_process_1a7a4c2933eab25c082cf23b665be414a2)`()` 

#### `public void `[`load`](#d9/daa/classalps_1_1_process_1a2202d78e43f8227f90b3d8cc2a5952be)`(`[`IDump`](#d1/d80/classalps_1_1_i_dump)` &)` 

#### `public void `[`save`](#d9/daa/classalps_1_1_process_1adee1f9c3c5841e75074dce64e7b53b98)`(`[`ODump`](#d3/db8/classalps_1_1_o_dump)` &) const` 

#### `public bool `[`valid`](#d9/daa/classalps_1_1_process_1a5708d077eeff86243b1d01f5f8df7a55)`() const` 

#### `public bool `[`local`](#d9/daa/classalps_1_1_process_1a00abffa0c55b644d81da33ee24e58652)`() const` 

#### `public inline  `[`operator int`](#d9/daa/classalps_1_1_process_1a2b0e92bcb7a4b1294716a99507982c39)`() const` 

#### `public inline bool `[`operator==`](#d9/daa/classalps_1_1_process_1a6e3f588ca10b4cd364e3af4431b1ed57)`(const `[`Process`](#d9/daa/classalps_1_1_process)` & p) const` 

#### `public inline bool `[`operator!=`](#d9/daa/classalps_1_1_process_1a6f74ae1bc88ef9573a0d0bf1da97e2f8)`(const `[`Process`](#d9/daa/classalps_1_1_process)` & p) const` 

#### `public inline bool `[`operator<`](#d9/daa/classalps_1_1_process_1a4262148f340ec0e1aaf00a4a621f333a)`(const `[`Process`](#d9/daa/classalps_1_1_process)` & p) const` 

sorting criterion for two processes?

# namespace `alps::detail` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public int `[`local_id`](#d8/db4/comm_8h_1a967395d3293c3d501e44b8f1554b5cff)`()`            | 
`public int `[`invalid_id`](#d8/db4/comm_8h_1a2a75ceab7ddd1d46304343d04b46ca7e)`()`            | 
`public bool `[`xdr_bool`](#df/d17/xdrdump_8_c_1a397a61eb757e243cca4c6458056e6960)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,bool * bp)`            | 
`public static bool `[`xdr_s_char`](#df/d17/xdrdump_8_c_1a9200d2b9de50a987e9ac19e6beee4bd1)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,signed char * scp)`            | 
`public bool `[`xdr_hyper`](#df/d17/xdrdump_8_c_1af563174489287e49bdcbe864d04c1d98)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,long long * llp)`            | 
`public bool `[`xdr_u_hyper`](#df/d17/xdrdump_8_c_1a2ee23e550a9b5de946aeb50ae6c9adf0)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,unsigned long long * llp)`            | 
`public bool `[`xdr_long_8`](#df/d17/xdrdump_8_c_1afe5f6771b2e5520c08a8053aacc236a6)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,long * lp)`            | 
`public bool `[`xdr_u_long_8`](#df/d17/xdrdump_8_c_1a322d654620f1c5e0c1d8e81b91e08d4b)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,unsigned long * lp)`            | 
`public bool `[`xdr_long_double`](#df/d17/xdrdump_8_c_1aa17d8487a2815e06fbfdaf14317ab0c7)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,long double * ldp)`            | 
`class `[`alps::detail::Buffer`](#d8/d85/classalps_1_1detail_1_1_buffer) | a simple [Buffer](#d8/d85/classalps_1_1detail_1_1_buffer) class. values can be written into it or read from it.
`struct `[`alps::detail::xdr_helper`](#db/d3c/structalps_1_1detail_1_1xdr__helper) | 

## Members

#### `public int `[`local_id`](#d8/db4/comm_8h_1a967395d3293c3d501e44b8f1554b5cff)`()` 

#### `public int `[`invalid_id`](#d8/db4/comm_8h_1a2a75ceab7ddd1d46304343d04b46ca7e)`()` 

#### `public bool `[`xdr_bool`](#df/d17/xdrdump_8_c_1a397a61eb757e243cca4c6458056e6960)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,bool * bp)` 

#### `public static bool `[`xdr_s_char`](#df/d17/xdrdump_8_c_1a9200d2b9de50a987e9ac19e6beee4bd1)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,signed char * scp)` 

#### `public bool `[`xdr_hyper`](#df/d17/xdrdump_8_c_1af563174489287e49bdcbe864d04c1d98)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,long long * llp)` 

#### `public bool `[`xdr_u_hyper`](#df/d17/xdrdump_8_c_1a2ee23e550a9b5de946aeb50ae6c9adf0)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,unsigned long long * llp)` 

#### `public bool `[`xdr_long_8`](#df/d17/xdrdump_8_c_1afe5f6771b2e5520c08a8053aacc236a6)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,long * lp)` 

#### `public bool `[`xdr_u_long_8`](#df/d17/xdrdump_8_c_1a322d654620f1c5e0c1d8e81b91e08d4b)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,unsigned long * lp)` 

#### `public bool `[`xdr_long_double`](#df/d17/xdrdump_8_c_1aa17d8487a2815e06fbfdaf14317ab0c7)`(`[`XDR`](#da/d72/struct_x_d_r)` * xdrs,long double * ldp)` 

# class `alps::detail::Buffer` 

```
class alps::detail::Buffer
  : public std::vector< char >
```  

a simple [Buffer](#d8/d85/classalps_1_1detail_1_1_buffer) class. values can be written into it or read from it.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`Buffer`](#d8/d85/classalps_1_1detail_1_1_buffer_1a6ae0d5c7c88ecfba82eddae78be25794)`()` | create a buffer.
`public inline void `[`clear`](#d8/d85/classalps_1_1detail_1_1_buffer_1ac26ea780afd07d33d200aed2f8b8bd30)`()` | erase the [Buffer](#d8/d85/classalps_1_1detail_1_1_buffer)
`public inline  `[`operator char *`](#d8/d85/classalps_1_1detail_1_1_buffer_1a2c6d0b77703a86897ee2b672ef93d7d0)`()` | get a pointer to the [Buffer](#d8/d85/classalps_1_1detail_1_1_buffer). This pointer might be invalidated by writing to the [Buffer](#d8/d85/classalps_1_1detail_1_1_buffer).
`public template<>`  <br/>`inline void `[`write`](#d8/d85/classalps_1_1detail_1_1_buffer_1a8132c1c92a67c01088c489f9e88ce71c)`(const T * p,size_type n)` | 
`public template<>`  <br/>`inline void `[`write`](#d8/d85/classalps_1_1detail_1_1_buffer_1ae432091edd996a2c04ec8ebb74f8d7de)`(const T x)` | 
`public template<>`  <br/>`inline void `[`read`](#d8/d85/classalps_1_1detail_1_1_buffer_1a6465308319328ef8bf4933a5c25bf463)`(T * p,size_type n)` | 
`public template<>`  <br/>`inline void `[`read`](#d8/d85/classalps_1_1detail_1_1_buffer_1a1d4eadeb1331af6cee6d5813ea28919d)`(T & x)` | 

## Members

#### `public inline  `[`Buffer`](#d8/d85/classalps_1_1detail_1_1_buffer_1a6ae0d5c7c88ecfba82eddae78be25794)`()` 

create a buffer.

#### `public inline void `[`clear`](#d8/d85/classalps_1_1detail_1_1_buffer_1ac26ea780afd07d33d200aed2f8b8bd30)`()` 

erase the [Buffer](#d8/d85/classalps_1_1detail_1_1_buffer)

#### `public inline  `[`operator char *`](#d8/d85/classalps_1_1detail_1_1_buffer_1a2c6d0b77703a86897ee2b672ef93d7d0)`()` 

get a pointer to the [Buffer](#d8/d85/classalps_1_1detail_1_1_buffer). This pointer might be invalidated by writing to the [Buffer](#d8/d85/classalps_1_1detail_1_1_buffer).

#### `public template<>`  <br/>`inline void `[`write`](#d8/d85/classalps_1_1detail_1_1_buffer_1a8132c1c92a67c01088c489f9e88ce71c)`(const T * p,size_type n)` 

#### `public template<>`  <br/>`inline void `[`write`](#d8/d85/classalps_1_1detail_1_1_buffer_1ae432091edd996a2c04ec8ebb74f8d7de)`(const T x)` 

#### `public template<>`  <br/>`inline void `[`read`](#d8/d85/classalps_1_1detail_1_1_buffer_1a6465308319328ef8bf4933a5c25bf463)`(T * p,size_type n)` 

#### `public template<>`  <br/>`inline void `[`read`](#d8/d85/classalps_1_1detail_1_1_buffer_1a1d4eadeb1331af6cee6d5813ea28919d)`(T & x)` 

# struct `alps::detail::xdr_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `netobj` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public u_int `[`n_len`](#df/d17/structnetobj_1a83ba1060952745625b8dcd4f9950a6bc) | 
`public char * `[`n_bytes`](#df/d17/structnetobj_1aee34b7ed11f6e715a101f8f900be3f5c) | 

## Members

#### `public u_int `[`n_len`](#df/d17/structnetobj_1a83ba1060952745625b8dcd4f9950a6bc) 

#### `public char * `[`n_bytes`](#df/d17/structnetobj_1aee34b7ed11f6e715a101f8f900be3f5c) 

# struct `XDR` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public enum xdr_op `[`x_op`](#da/d72/struct_x_d_r_1ac51509abcf1204ea1ef2d7631cec3294) | 
`public struct `[`XDR::xdr_ops`](#d1/d30/struct_x_d_r_1_1xdr__ops)` * `[`x_ops`](#da/d72/struct_x_d_r_1a834111b1d388477ea6914669dc7ff6f5) | 
`public caddr_t `[`x_public`](#da/d72/struct_x_d_r_1a1c8d7ffe7341cdfef4b35f9e112b2bbf) | 
`public caddr_t `[`x_private`](#da/d72/struct_x_d_r_1abd752ae0f84fcc28421986ba6c291b52) | 
`public caddr_t `[`x_base`](#da/d72/struct_x_d_r_1a3ab10557a986d2cec6e5a505c784917f) | 
`public u_int `[`x_handy`](#da/d72/struct_x_d_r_1a452d979b892d36f9b344b5e4ac839d13) | 

## Members

#### `public enum xdr_op `[`x_op`](#da/d72/struct_x_d_r_1ac51509abcf1204ea1ef2d7631cec3294) 

#### `public struct `[`XDR::xdr_ops`](#d1/d30/struct_x_d_r_1_1xdr__ops)` * `[`x_ops`](#da/d72/struct_x_d_r_1a834111b1d388477ea6914669dc7ff6f5) 

#### `public caddr_t `[`x_public`](#da/d72/struct_x_d_r_1a1c8d7ffe7341cdfef4b35f9e112b2bbf) 

#### `public caddr_t `[`x_private`](#da/d72/struct_x_d_r_1abd752ae0f84fcc28421986ba6c291b52) 

#### `public caddr_t `[`x_base`](#da/d72/struct_x_d_r_1a3ab10557a986d2cec6e5a505c784917f) 

#### `public u_int `[`x_handy`](#da/d72/struct_x_d_r_1a452d979b892d36f9b344b5e4ac839d13) 

# struct `xdr_discrim` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public int `[`value`](#da/df0/structxdr__discrim_1a57526f1125df7af463b2556af10916cb) | 
`public xdrproc_t `[`proc`](#da/df0/structxdr__discrim_1ab83aaddb7d00ff4a66497c3024e9d8c9) | 

## Members

#### `public int `[`value`](#da/df0/structxdr__discrim_1a57526f1125df7af463b2556af10916cb) 

#### `public xdrproc_t `[`proc`](#da/df0/structxdr__discrim_1ab83aaddb7d00ff4a66497c3024e9d8c9) 

# struct `XDR::xdr_ops` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public bool_t(* `[`x_getlong`](#d1/d30/struct_x_d_r_1_1xdr__ops_1abcb538b9fa51c53ece7067b179381523) | 
`public bool_t(* `[`x_putlong`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a4773213ccdfa91bc55c46e4d8d7ead0a) | 
`public bool_t(* `[`x_getbytes`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a3d71aaf2a799c3259dba38e8dcbfbc44) | 
`public bool_t(* `[`x_putbytes`](#d1/d30/struct_x_d_r_1_1xdr__ops_1ad990198d634d17d76889240f61c068aa) | 
`public u_int(* `[`x_getpostn`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a31109d548261f421827b598a43424ef2) | 
`public bool_t(* `[`x_setpostn`](#d1/d30/struct_x_d_r_1_1xdr__ops_1ad69f5bf036909413a4208969e9ee035a) | 
`public int32_t *(* `[`x_inline`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a664bb92c593057b4fb3a1b85e98b7b6c) | 
`public void(* `[`x_destroy`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a5b2657f7b099ea38cbeb51612385df3e) | 
`public bool_t(* `[`x_getint32`](#d1/d30/struct_x_d_r_1_1xdr__ops_1aa269b86f98b72a8d2dc18eab54546e6c) | 
`public bool_t(* `[`x_putint32`](#d1/d30/struct_x_d_r_1_1xdr__ops_1aeac725be4279173702e090b34eb1878f) | 

## Members

#### `public bool_t(* `[`x_getlong`](#d1/d30/struct_x_d_r_1_1xdr__ops_1abcb538b9fa51c53ece7067b179381523) 

#### `public bool_t(* `[`x_putlong`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a4773213ccdfa91bc55c46e4d8d7ead0a) 

#### `public bool_t(* `[`x_getbytes`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a3d71aaf2a799c3259dba38e8dcbfbc44) 

#### `public bool_t(* `[`x_putbytes`](#d1/d30/struct_x_d_r_1_1xdr__ops_1ad990198d634d17d76889240f61c068aa) 

#### `public u_int(* `[`x_getpostn`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a31109d548261f421827b598a43424ef2) 

#### `public bool_t(* `[`x_setpostn`](#d1/d30/struct_x_d_r_1_1xdr__ops_1ad69f5bf036909413a4208969e9ee035a) 

#### `public int32_t *(* `[`x_inline`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a664bb92c593057b4fb3a1b85e98b7b6c) 

#### `public void(* `[`x_destroy`](#d1/d30/struct_x_d_r_1_1xdr__ops_1a5b2657f7b099ea38cbeb51612385df3e) 

#### `public bool_t(* `[`x_getint32`](#d1/d30/struct_x_d_r_1_1xdr__ops_1aa269b86f98b72a8d2dc18eab54546e6c) 

#### `public bool_t(* `[`x_putint32`](#d1/d30/struct_x_d_r_1_1xdr__ops_1aeac725be4279173702e090b34eb1878f) 

Generated by [Moxygen](https://sourcey.com/moxygen)
