---
title: Reference
description: "ALPS Alea Library"
weight: 3
---

# Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`namespace `[`alps`](#d8/d3d/namespacealps) | 
`namespace `[`alps::alea`](#df/d14/namespacealps_1_1alea) | 
`namespace `[`alps::detail`](#d6/d75/namespacealps_1_1detail) | 
`class `[`alps::alea::mcdata::const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator) | 

# namespace `alps` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`enum `[`error_convergence`](#df/d66/convergence_8hpp_1a54a85f12ba2667a7b4da7e563d14e2bc)            | 
`enum `[`Target`](#d6/d1e/observable_8h_1a9a9faee850051d4e990e238c5a7a03e7)            | 
`public template<>`  <br/>`inline bool `[`error_underflow`](#d2/d24/abstractsimpleobservable_8h_1a769d872ca2ea7677d88761d1dd8bf470)`(T mean,T error)`            | 
`public template<>`  <br/>`inline bool `[`error_underflow`](#d2/d24/abstractsimpleobservable_8h_1a6b9b17b0b540f8f06b6df7d39d9abf57)`(std::complex< T > mean,std::complex< T > error)`            | 
`public template<>`  <br/>`inline std::string `[`convergence_to_text`](#df/d66/convergence_8hpp_1ae724277fbd93d10067d7da96c92ac5c1)`(T)`            | 
`public inline std::string `[`convergence_to_text`](#df/d66/convergence_8hpp_1a9800c4c2fbdd25e1d8cb4deb851bdc24)`(int c)`            | 
`public double `[`nan`](#dc/d7c/nan_8_c_1abeaf49c95bb394048ce101340009e3d1)`()`            | 
`public double `[`inf`](#dc/d7c/nan_8_c_1af237b54283d8c970ad6295093e37ca5f)`()`            | 
`public double `[`ninf`](#dc/d7c/nan_8_c_1af51ce066481842c78e67ba0473cd3df5)`()`            | 
`public inline std::ostream & `[`operator<<`](#d6/d1e/observable_8h_1a48576414ff801ef559b7abfa64882c4d)`(std::ostream & out,const `[`alps::Observable`](#df/d26/classalps_1_1_observable)` & m)`            | write an observable to a std::ostream
`public inline std::ostream & `[`operator<<`](#d7/d5e/observableset_8h_1a1c490eb835e15a55082202c8935df864)`(std::ostream & out,const `[`alps::ObservableSet`](#db/da3/classalps_1_1_observable_set)` & obs)`            | output all observables in an [ObservableSet](#db/da3/classalps_1_1_observable_set)
`public template<>`  <br/>`boost::shared_ptr< `[`Observable`](#df/d26/classalps_1_1_observable)` > `[`make_observable`](#d1/d51/signedobservable_8h_1a5a8943843c0a968711b4d9efdc75036e)`(const OBS & obs,bool issigned)`            | 
`public template<>`  <br/>`boost::shared_ptr< `[`Observable`](#df/d26/classalps_1_1_observable)` > `[`make_observable`](#d1/d51/signedobservable_8h_1a59af9accaebef859f998d0000dbad0a6)`(const OBS & obs,const std::string & s,SIGN,bool issigned)`            | 
`public inline double `[`text_to_double`](#d9/d7e/simpleobsdata_8h_1abdf12d170aa2a2afa8c8c06fd9eeb332)`(const std::string & val)`            | 
`public template<>`  <br/>`hdf5::archive & `[`operator<<`](#d6/d72/simpleobservable_8h_1ac07b44afd58c9554147e2d7e95e67c30)`(hdf5::archive & ar,`[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable)`< T, BINNING > const & obs)`            | 
`public template<>`  <br/>`hdf5::archive & `[`operator>>`](#d6/d72/simpleobservable_8h_1a0a2d502415434f4d1dafb44cb63ca0c7)`(hdf5::archive & ar,`[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable)`< T, BINNING > & obs)`            | 
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator+`](#d8/dcf/simpleobseval_8h_1ad165718f4a2d8d5accaf88c00857d83a)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< U > & y)`            | sum of two observables
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator+`](#d8/dcf/simpleobseval_8h_1ab3306ed91e2876a6824c31a50c7837eb)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const Y & y)`            | sum of observable and number
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator+`](#d8/dcf/simpleobseval_8h_1a63b1363e9dbdd1c60ad6c3e32d7fcef7)`(const Y & y,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x)`            | sum of observable and number
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator-`](#d8/dcf/simpleobseval_8h_1ace7acf8cf343b8d2b2e592296fe8a6a1)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< U > & y)`            | difference of two observables (IBM AIX workaround)
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator-`](#d8/dcf/simpleobseval_8h_1a97bb90f4fe9a113e57d12a499fe97370)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const Y & y)`            | difference of observable and number
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator-`](#d8/dcf/simpleobseval_8h_1a98259dc04b7e31d792735cb41d56ad37)`(const Y & y,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x)`            | difference of observable and number
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator*`](#d8/dcf/simpleobseval_8h_1a1c0c37374eeefbcbd28711e4a8a945ba)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< U > & y)`            | product of two observables (IBM AIX workaround)
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator*`](#d8/dcf/simpleobseval_8h_1ac20c602d7e1c8c8398d4f6e9df9da243)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const Y & y)`            | product of observable and number
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator*`](#d8/dcf/simpleobseval_8h_1ac7dc4a20bb172d574988629fdd5c2c52)`(const Y & y,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x)`            | product of observable and number
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< std::valarray< T > > `[`operator*`](#d8/dcf/simpleobseval_8h_1ab3ea34ff7c67ce87df30e34bb7de0a19)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< std::valarray< T > > const & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & y)`            | product of vector and scalar observable
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< std::valarray< T > > `[`operator*`](#d8/dcf/simpleobseval_8h_1a988d5d56a1ba40682cbc4583f9c8076b)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & y,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< std::valarray< T > > const & x)`            | product of vector and scalar observable
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator/`](#d8/dcf/simpleobseval_8h_1a0fbee03ac9cd3a6d36156cca5e615f96)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< U > & y)`            | ratio of two observables (IBM AIX workaround)
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator/`](#d8/dcf/simpleobseval_8h_1a728ac2889190b2099d8c71d693d8ed0d)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const Y & y)`            | ratio of observable and number
`public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator/`](#d8/dcf/simpleobseval_8h_1a3d26195db151fff228c8528abe3ea16c)`(const Y & x,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & y)`            | ratio of number and observable
`public template<>`  <br/>[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`pow`](#d8/dcf/simpleobseval_8h_1a7a8789f5b29a7eb0b1e1b9e1158400f8)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,double p)`            | 
`public template<>`  <br/>[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`pow`](#d8/dcf/simpleobseval_8h_1af9e3e7f6cdc62af12e2c16a1f59c7694)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,int p)`            | 
`class `[`alps::A`](#d1/d2d/classalps_1_1_a) | 
`class `[`alps::AbstractBinning`](#d9/d54/classalps_1_1_abstract_binning) | 
`class `[`alps::AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable) | 
`class `[`alps::AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable) | 
`class `[`alps::BasicDetailedBinning`](#d7/d69/classalps_1_1_basic_detailed_binning) | 
`class `[`alps::DetailedBinning`](#da/dd8/classalps_1_1_detailed_binning) | 
`class `[`alps::FixedBinning`](#df/d7c/classalps_1_1_fixed_binning) | 
`class `[`alps::HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable) | 
`class `[`alps::HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data) | 
`class `[`alps::HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator) | 
`class `[`alps::NoBinning`](#d6/dba/classalps_1_1_no_binning) | 
`class `[`alps::NoMeasurementsError`](#dc/dfe/classalps_1_1_no_measurements_error) | an error class if no measurement was performed
`class `[`alps::Observable`](#df/d26/classalps_1_1_observable) | the base class for all observables
`class `[`alps::ObservableFactory`](#d6/d35/classalps_1_1_observable_factory) | [A](#d1/d2d/classalps_1_1_a) class to collect the various measurements performed in a simulation It is implemented as a map, with std::string as key type
`class `[`alps::ObservableSet`](#db/da3/classalps_1_1_observable_set) | 
`class `[`alps::ObservableSetXMLHandler`](#de/d7b/classalps_1_1_observable_set_x_m_l_handler) | XML parser for the [ObservableSet](#db/da3/classalps_1_1_observable_set) class.
`class `[`alps::ObsValueXMLHandler`](#db/d55/classalps_1_1_obs_value_x_m_l_handler) | 
`class `[`alps::RealHistogramEntryXMLHandler`](#d9/db6/classalps_1_1_real_histogram_entry_x_m_l_handler) | XML parser for the entries for RealHistogramObservable class.
`class `[`alps::RealHistogramObservableXMLHandler`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler) | XML parser for the RealHistogramObservable class.
`class `[`alps::RealObsevaluatorValueXMLHandler`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler) | XML parser for the elements for RealObsevaluator class.
`class `[`alps::RealObsevaluatorXMLHandler`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler) | XML parser for the RealObsevaluator class.
`class `[`alps::RealVectorObsevaluatorXMLHandler`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler) | XML parser for the RealVectorObsevaluator class.
`class `[`alps::RecordableObservable`](#d8/dca/classalps_1_1_recordable_observable) | 
`class `[`alps::SignedObservable`](#dc/d91/classalps_1_1_signed_observable) | 
`class `[`alps::SimpleBinning`](#de/d2e/classalps_1_1_simple_binning) | 
`class `[`alps::SimpleObservable`](#d0/dee/classalps_1_1_simple_observable) | 
`class `[`alps::SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data) | 
`class `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator) | 
`struct `[`alps::ObservableNamingHelper`](#dc/dc5/structalps_1_1_observable_naming_helper) | 
`struct `[`alps::output_helper`](#d4/df9/structalps_1_1output__helper) | 
`struct `[`alps::output_helper< boost::mpl::false_ >`](#d6/db1/structalps_1_1output__helper_3_01boost_1_1mpl_1_1false___01_4) | 
`struct `[`alps::output_helper< boost::mpl::true_ >`](#d1/dbd/structalps_1_1output__helper_3_01boost_1_1mpl_1_1true___01_4) | 
`struct `[`alps::type_tag< std::valarray< T > >`](#da/d0b/structalps_1_1type__tag_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::type_tag< std::vector< T > >`](#d8/d03/structalps_1_1type__tag_3_01std_1_1vector_3_01_t_01_4_01_4) | 

## Members

#### `enum `[`error_convergence`](#df/d66/convergence_8hpp_1a54a85f12ba2667a7b4da7e563d14e2bc) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
CONVERGED            | 
MAYBE_CONVERGED            | 
NOT_CONVERGED            | 

#### `enum `[`Target`](#d6/d1e/observable_8h_1a9a9faee850051d4e990e238c5a7a03e7) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
Mean            | 
Error            | 
Variance            | 
Tau            | 

#### `public template<>`  <br/>`inline bool `[`error_underflow`](#d2/d24/abstractsimpleobservable_8h_1a769d872ca2ea7677d88761d1dd8bf470)`(T mean,T error)` 

#### `public template<>`  <br/>`inline bool `[`error_underflow`](#d2/d24/abstractsimpleobservable_8h_1a6b9b17b0b540f8f06b6df7d39d9abf57)`(std::complex< T > mean,std::complex< T > error)` 

#### `public template<>`  <br/>`inline std::string `[`convergence_to_text`](#df/d66/convergence_8hpp_1ae724277fbd93d10067d7da96c92ac5c1)`(T)` 

#### `public inline std::string `[`convergence_to_text`](#df/d66/convergence_8hpp_1a9800c4c2fbdd25e1d8cb4deb851bdc24)`(int c)` 

#### `public double `[`nan`](#dc/d7c/nan_8_c_1abeaf49c95bb394048ce101340009e3d1)`()` 

#### `public double `[`inf`](#dc/d7c/nan_8_c_1af237b54283d8c970ad6295093e37ca5f)`()` 

#### `public double `[`ninf`](#dc/d7c/nan_8_c_1af51ce066481842c78e67ba0473cd3df5)`()` 

#### `public inline std::ostream & `[`operator<<`](#d6/d1e/observable_8h_1a48576414ff801ef559b7abfa64882c4d)`(std::ostream & out,const `[`alps::Observable`](#df/d26/classalps_1_1_observable)` & m)` 

write an observable to a std::ostream

#### `public inline std::ostream & `[`operator<<`](#d7/d5e/observableset_8h_1a1c490eb835e15a55082202c8935df864)`(std::ostream & out,const `[`alps::ObservableSet`](#db/da3/classalps_1_1_observable_set)` & obs)` 

output all observables in an [ObservableSet](#db/da3/classalps_1_1_observable_set)

#### `public template<>`  <br/>`boost::shared_ptr< `[`Observable`](#df/d26/classalps_1_1_observable)` > `[`make_observable`](#d1/d51/signedobservable_8h_1a5a8943843c0a968711b4d9efdc75036e)`(const OBS & obs,bool issigned)` 

#### `public template<>`  <br/>`boost::shared_ptr< `[`Observable`](#df/d26/classalps_1_1_observable)` > `[`make_observable`](#d1/d51/signedobservable_8h_1a59af9accaebef859f998d0000dbad0a6)`(const OBS & obs,const std::string & s,SIGN,bool issigned)` 

#### `public inline double `[`text_to_double`](#d9/d7e/simpleobsdata_8h_1abdf12d170aa2a2afa8c8c06fd9eeb332)`(const std::string & val)` 

#### `public template<>`  <br/>`hdf5::archive & `[`operator<<`](#d6/d72/simpleobservable_8h_1ac07b44afd58c9554147e2d7e95e67c30)`(hdf5::archive & ar,`[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable)`< T, BINNING > const & obs)` 

#### `public template<>`  <br/>`hdf5::archive & `[`operator>>`](#d6/d72/simpleobservable_8h_1a0a2d502415434f4d1dafb44cb63ca0c7)`(hdf5::archive & ar,`[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable)`< T, BINNING > & obs)` 

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator+`](#d8/dcf/simpleobseval_8h_1ad165718f4a2d8d5accaf88c00857d83a)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< U > & y)` 

sum of two observables

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator+`](#d8/dcf/simpleobseval_8h_1ab3306ed91e2876a6824c31a50c7837eb)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const Y & y)` 

sum of observable and number

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator+`](#d8/dcf/simpleobseval_8h_1a63b1363e9dbdd1c60ad6c3e32d7fcef7)`(const Y & y,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x)` 

sum of observable and number

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator-`](#d8/dcf/simpleobseval_8h_1ace7acf8cf343b8d2b2e592296fe8a6a1)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< U > & y)` 

difference of two observables (IBM AIX workaround)

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator-`](#d8/dcf/simpleobseval_8h_1a97bb90f4fe9a113e57d12a499fe97370)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const Y & y)` 

difference of observable and number

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator-`](#d8/dcf/simpleobseval_8h_1a98259dc04b7e31d792735cb41d56ad37)`(const Y & y,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x)` 

difference of observable and number

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator*`](#d8/dcf/simpleobseval_8h_1a1c0c37374eeefbcbd28711e4a8a945ba)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< U > & y)` 

product of two observables (IBM AIX workaround)

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator*`](#d8/dcf/simpleobseval_8h_1ac20c602d7e1c8c8398d4f6e9df9da243)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const Y & y)` 

product of observable and number

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator*`](#d8/dcf/simpleobseval_8h_1ac7dc4a20bb172d574988629fdd5c2c52)`(const Y & y,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x)` 

product of observable and number

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< std::valarray< T > > `[`operator*`](#d8/dcf/simpleobseval_8h_1ab3ea34ff7c67ce87df30e34bb7de0a19)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< std::valarray< T > > const & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & y)` 

product of vector and scalar observable

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< std::valarray< T > > `[`operator*`](#d8/dcf/simpleobseval_8h_1a988d5d56a1ba40682cbc4583f9c8076b)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & y,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< std::valarray< T > > const & x)` 

product of vector and scalar observable

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator/`](#d8/dcf/simpleobseval_8h_1a0fbee03ac9cd3a6d36156cca5e615f96)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< U > & y)` 

ratio of two observables (IBM AIX workaround)

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator/`](#d8/dcf/simpleobseval_8h_1a728ac2889190b2099d8c71d693d8ed0d)`(`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & x,const Y & y)` 

ratio of observable and number

#### `public template<>`  <br/>`inline `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator/`](#d8/dcf/simpleobseval_8h_1a3d26195db151fff228c8528abe3ea16c)`(const Y & x,`[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > const & y)` 

ratio of number and observable

#### `public template<>`  <br/>[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`pow`](#d8/dcf/simpleobseval_8h_1a7a8789f5b29a7eb0b1e1b9e1158400f8)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,double p)` 

#### `public template<>`  <br/>[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`pow`](#d8/dcf/simpleobseval_8h_1af9e3e7f6cdc62af12e2c16a1f59c7694)`(const `[`alps::SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & x,int p)` 

# class `alps::A` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# class `alps::AbstractBinning` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`AbstractBinning`](#d9/d54/classalps_1_1_abstract_binning_1a4b5dfad25c42722421283ba6860f19fa)`(std::size_t)` | 
`public inline time_type `[`tau`](#d9/d54/classalps_1_1_abstract_binning_1ac437fa3669440fb86d739b61dec8ba29)`() const` | 
`public inline uint32_t `[`max_bin_number`](#d9/d54/classalps_1_1_abstract_binning_1a2292c73f7c0eae76e2883bdbe391cf2a)`() const` | 
`public inline uint32_t `[`bin_number`](#d9/d54/classalps_1_1_abstract_binning_1ace24fc99d6a888bf7806a72a0bfb4c75)`() const` | 
`public inline uint32_t `[`filled_bin_number`](#d9/d54/classalps_1_1_abstract_binning_1a3af1f49a952f5523e723269688df5e48)`() const` | 
`public inline uint32_t `[`filled_bin_number2`](#d9/d54/classalps_1_1_abstract_binning_1a90cd2309e091fb281c2fbc4f73b983fd)`() const` | 
`public inline uint32_t `[`bin_size`](#d9/d54/classalps_1_1_abstract_binning_1af46d5d0edb6afa5c2713b559a4727394)`() const` | 
`public inline const value_type & `[`bin_value`](#d9/d54/classalps_1_1_abstract_binning_1a6d44b3822bfb78694d1e193207afd3c0)`(uint32_t) const` | 
`public inline const value_type & `[`bin_value2`](#d9/d54/classalps_1_1_abstract_binning_1a8f969aabc055e38b713da5a6c1b9efd7)`(uint32_t) const` | 
`public inline const std::vector< value_type > & `[`bins`](#d9/d54/classalps_1_1_abstract_binning_1acc8bcc7de63e937178dbbc8d2df41aac)`() const` | 
`public inline void `[`extract_timeseries`](#d9/d54/classalps_1_1_abstract_binning_1af3a7837fc0e5a68c2b8dae3b32ddcf11)`(ODump & dump) const` | 
`public inline bool `[`has_variance`](#d9/d54/classalps_1_1_abstract_binning_1ac9e2dcc15345e5dd5ca70216c7814c03)`() const` | 
`public inline void `[`write_scalar_xml`](#d9/d54/classalps_1_1_abstract_binning_1a625dc556a2bbce37d38efde696dfcc89)`(oxstream &) const` | 
`public template<>`  <br/>`inline void `[`write_vector_xml`](#d9/d54/classalps_1_1_abstract_binning_1abedab69d87ced296d4b05c3ea276a77a)`(oxstream &,IT) const` | 
`public inline void `[`save`](#d9/d54/classalps_1_1_abstract_binning_1a0745ed466eee6419fdebd520480443fc)`(ODump &) const` | 
`public inline void `[`load`](#d9/d54/classalps_1_1_abstract_binning_1ad751095caf6bdb39c1d4d6174a9e5388)`(IDump & dump)` | 
`public inline void `[`save`](#d9/d54/classalps_1_1_abstract_binning_1a9757301001261e5d1cbf083908d7840f)`(hdf5::archive &) const` | 
`public inline void `[`load`](#d9/d54/classalps_1_1_abstract_binning_1aa642077e1ef2093a2b6d7dd5a3689ad7)`(hdf5::archive &)` | 
`public inline std::string `[`evaluation_method`](#d9/d54/classalps_1_1_abstract_binning_1a2d5f6b8c234c20aa25dbdd5be12a52d2)`() const` | 
`typedef `[`value_type`](#d9/d54/classalps_1_1_abstract_binning_1aec1a1865167eb7b88f3dbf06968178af) | 
`typedef `[`time_type`](#d9/d54/classalps_1_1_abstract_binning_1a8f998b4e8071200966690d84f958af32) | 
`typedef `[`convergence_type`](#d9/d54/classalps_1_1_abstract_binning_1a82d7fe4bcb2914d7406ee259eb3f9664) | 

## Members

#### `public inline  `[`AbstractBinning`](#d9/d54/classalps_1_1_abstract_binning_1a4b5dfad25c42722421283ba6860f19fa)`(std::size_t)` 

#### `public inline time_type `[`tau`](#d9/d54/classalps_1_1_abstract_binning_1ac437fa3669440fb86d739b61dec8ba29)`() const` 

#### `public inline uint32_t `[`max_bin_number`](#d9/d54/classalps_1_1_abstract_binning_1a2292c73f7c0eae76e2883bdbe391cf2a)`() const` 

#### `public inline uint32_t `[`bin_number`](#d9/d54/classalps_1_1_abstract_binning_1ace24fc99d6a888bf7806a72a0bfb4c75)`() const` 

#### `public inline uint32_t `[`filled_bin_number`](#d9/d54/classalps_1_1_abstract_binning_1a3af1f49a952f5523e723269688df5e48)`() const` 

#### `public inline uint32_t `[`filled_bin_number2`](#d9/d54/classalps_1_1_abstract_binning_1a90cd2309e091fb281c2fbc4f73b983fd)`() const` 

#### `public inline uint32_t `[`bin_size`](#d9/d54/classalps_1_1_abstract_binning_1af46d5d0edb6afa5c2713b559a4727394)`() const` 

#### `public inline const value_type & `[`bin_value`](#d9/d54/classalps_1_1_abstract_binning_1a6d44b3822bfb78694d1e193207afd3c0)`(uint32_t) const` 

#### `public inline const value_type & `[`bin_value2`](#d9/d54/classalps_1_1_abstract_binning_1a8f969aabc055e38b713da5a6c1b9efd7)`(uint32_t) const` 

#### `public inline const std::vector< value_type > & `[`bins`](#d9/d54/classalps_1_1_abstract_binning_1acc8bcc7de63e937178dbbc8d2df41aac)`() const` 

#### `public inline void `[`extract_timeseries`](#d9/d54/classalps_1_1_abstract_binning_1af3a7837fc0e5a68c2b8dae3b32ddcf11)`(ODump & dump) const` 

#### `public inline bool `[`has_variance`](#d9/d54/classalps_1_1_abstract_binning_1ac9e2dcc15345e5dd5ca70216c7814c03)`() const` 

#### `public inline void `[`write_scalar_xml`](#d9/d54/classalps_1_1_abstract_binning_1a625dc556a2bbce37d38efde696dfcc89)`(oxstream &) const` 

#### `public template<>`  <br/>`inline void `[`write_vector_xml`](#d9/d54/classalps_1_1_abstract_binning_1abedab69d87ced296d4b05c3ea276a77a)`(oxstream &,IT) const` 

#### `public inline void `[`save`](#d9/d54/classalps_1_1_abstract_binning_1a0745ed466eee6419fdebd520480443fc)`(ODump &) const` 

#### `public inline void `[`load`](#d9/d54/classalps_1_1_abstract_binning_1ad751095caf6bdb39c1d4d6174a9e5388)`(IDump & dump)` 

#### `public inline void `[`save`](#d9/d54/classalps_1_1_abstract_binning_1a9757301001261e5d1cbf083908d7840f)`(hdf5::archive &) const` 

#### `public inline void `[`load`](#d9/d54/classalps_1_1_abstract_binning_1aa642077e1ef2093a2b6d7dd5a3689ad7)`(hdf5::archive &)` 

#### `public inline std::string `[`evaluation_method`](#d9/d54/classalps_1_1_abstract_binning_1a2d5f6b8c234c20aa25dbdd5be12a52d2)`() const` 

#### `typedef `[`value_type`](#d9/d54/classalps_1_1_abstract_binning_1aec1a1865167eb7b88f3dbf06968178af) 

#### `typedef `[`time_type`](#d9/d54/classalps_1_1_abstract_binning_1a8f998b4e8071200966690d84f958af32) 

#### `typedef `[`convergence_type`](#d9/d54/classalps_1_1_abstract_binning_1a82d7fe4bcb2914d7406ee259eb3f9664) 

# class `alps::AbstractSignedObservable` 

```
class alps::AbstractSignedObservable
  : public alps::AbstractSimpleObservable< OBS::value_type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a335f9b1bb546b92803e78cff4eadc9b8)`(int,version)` | 
`public inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ac032a074cdaddaedd1e2238ef682357d)`(const OBS & obs,const std::string & s)` | 
`public inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a22f37e262a0a98b3d9388708ec885107)`(const std::string & name,const std::string & s,const label_type & l)` | 
`public inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a2d5c96871d1f36fc21f36f69fba26e05)`(const std::string & name,const char * s,const label_type & l)` | 
`public template<>`  <br/>`inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a5c4aebedad4bc0ebb189dfea1a7f0cb9)`(const `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable)`< OBS2, SIGN > & o)` | 
`public template<>`  <br/>`inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a441cccf64826e4fb10ef008cbe984a7e)`(const std::string & name,const ARG & arg,const label_type & l)` | 
`public template<>`  <br/>`inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1abd82a405fb37188ae37e5e064373aef4)`(const std::string & name,std::string & s,const ARG & arg,const label_type & l)` | 
`public inline  `[`~AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1aaf40546d4bbcae7a2901cd93c4faa08e)`()` | 
`public inline virtual uint32_t `[`version_id`](#d9/d7a/classalps_1_1_abstract_signed_observable_1afd38b74fa5d2d981243f90a6d840c519)`() const` | return a version ID uniquely identifying the class
`public inline virtual ALPS_DUMMY_VOID `[`reset`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ac41e787483191014923ffaa53fbae292)`(bool equilibrated)` | reset the observable
`public inline virtual ALPS_DUMMY_VOID `[`output`](#d9/d7a/classalps_1_1_abstract_signed_observable_1af8f1b3166ed48e56ecd21e1c4ab981f3)`(std::ostream &) const` | output the result
`public void `[`output_scalar`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a9ab97adde46b21d1a2e41232c6b4f00e)`(std::ostream &) const` | 
`public void `[`output_vector`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a7e0f5510282d9b20f9a0dd08034bee10)`(std::ostream &) const` | 
`public inline virtual void `[`write_xml`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a7fbbfd4d921b6c827f15278b83ca85e4)`(oxstream & oxs,const boost::filesystem::path & fn_hdf5) const` | output the result
`public inline virtual count_type `[`count`](#d9/d7a/classalps_1_1_abstract_signed_observable_1acd53a082e2fd84c9f7bfd5f19da500e5)`() const` | the number of measurements
`public inline virtual result_type `[`mean`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a653a6d71d99998391f7342fe4e595a40)`() const` | the mean value
`public inline virtual result_type `[`error`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a5a11cf1cf2f0f80dec138af1a3e47d78)`() const` | the error
`public inline virtual convergence_type `[`converged_errors`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a2642446db28034013be6301a0d4f1854)`() const` | 
`public inline virtual `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< value_type > `[`make_evaluator`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a3aa77c3a46d02ecde181476d45c00a30)`() const` | 
`public template<>`  <br/>`inline `[`AbstractSignedObservable](#d9/d7a/classalps_1_1_abstract_signed_observable)< [SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< value_type >::type >, SIGN > `[`slice`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a3207fc3b3c9e91ca9f52f6e6ded489de)`(S s,const std::string & newname) const` | 
`public template<>`  <br/>`inline `[`AbstractSignedObservable](#d9/d7a/classalps_1_1_abstract_signed_observable)< [SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< value_type >::type >, SIGN > `[`operator[]`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a50e9814d0db53e5ad8e51add45d8f1b6)`(S s) const` | 
`public virtual void `[`save`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a38ed58d5362fe0dd576c96d0be18645d)`(ODump & dump) const` | 
`public virtual void `[`load`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a00bb8241981888814661e02dfbadc102)`(IDump & dump)` | 
`public virtual void `[`save`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a0b1a2d425d59e5bcdf209097990de77e)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ad9fcfc945af8ef3c76ea6b5f33a4809e)`(hdf5::archive &)` | 
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a556d59cbfaeedf4697e2a86366030b08)`() const` | clones the observable
`public inline virtual bool `[`is_signed`](#d9/d7a/classalps_1_1_abstract_signed_observable_1abc9319cf3604aa5f30de62c715af5b83)`() const` | is the observable signed?
`public inline virtual void `[`set_sign_name`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a03898da80ce8686d98d7ce0ae2bd23e3)`(const std::string & signname)` | set the name of the observable containing the sign for this observable
`public virtual void `[`set_sign`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a8fa6c03fb22972f6e67e02bc27ccf99f)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & sign)` | set the observable containing the sign
`public inline virtual void `[`clear_sign`](#d9/d7a/classalps_1_1_abstract_signed_observable_1aede69c19a60d48f20ccb811497ac4b5e)`()` | clear any previosuly set sign observable
`public virtual const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`sign`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a88aa4b55c17c4a6449df9b199ba72aff)`() const` | get a reference to the sign observable
`public inline virtual const std::string `[`sign_name`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ab79f1c246b21cef463871223862db036)`() const` | get the name of the observable containing the sign
`public inline virtual const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`signed_observable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a73f71e14046fea130247dfe25e022136)`() const` | 
`public inline virtual uint32_t `[`number_of_runs`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a80342d5dc097a0167a4f485fba0182cd)`() const` | get the number of runs which performed measurements for this observable
`public virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`get_run`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a3c132b21b8f0af8e22a5b99a05a9ab5d)`(uint32_t) const` | extract an observable from a specific run only
`protected observable_type `[`obs_`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a42174153c6046a208660f5bb6527de15) | 
`protected std::string `[`sign_name_`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ae2a6016b3a6cefad1bd1a7900c5c4a10) | 
`protected const `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`sign_`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a658aa8cb02608b34c8d108aa2ad7ae13) | 
`protected inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`convert_mergeable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1af9bfa5fa8a4335ba472fb929350797b1)`() const` | create a copy of the observable that can be merged
`protected virtual void `[`write_more_xml`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a7eafa9afddf022037f2214027197fb5f)`(oxstream & oxs,slice_index it) const` | 
`protected inline virtual void `[`merge`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ac7d64db735e082c84d90b555faf811c3)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & o)` | 
`protected inline virtual bool `[`can_merge`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ae84e21c5fa71a62fb2bfadaedac4907a)`() const` | can this observable be merged with one of the same type
`protected inline virtual bool `[`can_merge`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a4d567373646127b689522fc29efbc050)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &) const` | can this observable be merged with one of the given type
`typedef `[`observable_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a32a3b0888f8b4e6e251cf1f2bf412b33) | 
`typedef `[`sign_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ae09913a1d51c3775e4a75e31db9c2c9b) | 
`typedef `[`value_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a929af477fdffda4d94dbfc4d83db8776) | 
`typedef `[`result_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a95521a7cd8094cff6cb12372f8587a9a) | 
`typedef `[`base_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a900ff1f03abd7f118235cfac6c598189) | 
`typedef `[`slice_index`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a5f420fa3a55a00345e9faab84c98cb26) | 
`typedef `[`count_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ade9d71f1d9454c5155f11fd8a10d8368) | 
`typedef `[`time_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ae56c7b82af0d447a9bdcd9c2a6cbc6a8) | 
`typedef `[`convergence_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a737c253b0a5762e75a1110d581e802c6) | 
`typedef `[`label_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a4642a432359bc3605118ac4e76fb51a6) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a335f9b1bb546b92803e78cff4eadc9b8)`(int,version)` 

#### `public inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ac032a074cdaddaedd1e2238ef682357d)`(const OBS & obs,const std::string & s)` 

#### `public inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a22f37e262a0a98b3d9388708ec885107)`(const std::string & name,const std::string & s,const label_type & l)` 

#### `public inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a2d5c96871d1f36fc21f36f69fba26e05)`(const std::string & name,const char * s,const label_type & l)` 

#### `public template<>`  <br/>`inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a5c4aebedad4bc0ebb189dfea1a7f0cb9)`(const `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable)`< OBS2, SIGN > & o)` 

#### `public template<>`  <br/>`inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a441cccf64826e4fb10ef008cbe984a7e)`(const std::string & name,const ARG & arg,const label_type & l)` 

#### `public template<>`  <br/>`inline  `[`AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1abd82a405fb37188ae37e5e064373aef4)`(const std::string & name,std::string & s,const ARG & arg,const label_type & l)` 

#### `public inline  `[`~AbstractSignedObservable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1aaf40546d4bbcae7a2901cd93c4faa08e)`()` 

#### `public inline virtual uint32_t `[`version_id`](#d9/d7a/classalps_1_1_abstract_signed_observable_1afd38b74fa5d2d981243f90a6d840c519)`() const` 

return a version ID uniquely identifying the class

#### `public inline virtual ALPS_DUMMY_VOID `[`reset`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ac41e787483191014923ffaa53fbae292)`(bool equilibrated)` 

reset the observable

#### `public inline virtual ALPS_DUMMY_VOID `[`output`](#d9/d7a/classalps_1_1_abstract_signed_observable_1af8f1b3166ed48e56ecd21e1c4ab981f3)`(std::ostream &) const` 

output the result

#### `public void `[`output_scalar`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a9ab97adde46b21d1a2e41232c6b4f00e)`(std::ostream &) const` 

#### `public void `[`output_vector`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a7e0f5510282d9b20f9a0dd08034bee10)`(std::ostream &) const` 

#### `public inline virtual void `[`write_xml`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a7fbbfd4d921b6c827f15278b83ca85e4)`(oxstream & oxs,const boost::filesystem::path & fn_hdf5) const` 

output the result

#### `public inline virtual count_type `[`count`](#d9/d7a/classalps_1_1_abstract_signed_observable_1acd53a082e2fd84c9f7bfd5f19da500e5)`() const` 

the number of measurements

#### `public inline virtual result_type `[`mean`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a653a6d71d99998391f7342fe4e595a40)`() const` 

the mean value

#### `public inline virtual result_type `[`error`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a5a11cf1cf2f0f80dec138af1a3e47d78)`() const` 

the error

#### `public inline virtual convergence_type `[`converged_errors`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a2642446db28034013be6301a0d4f1854)`() const` 

#### `public inline virtual `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< value_type > `[`make_evaluator`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a3aa77c3a46d02ecde181476d45c00a30)`() const` 

#### `public template<>`  <br/>`inline `[`AbstractSignedObservable](#d9/d7a/classalps_1_1_abstract_signed_observable)< [SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< value_type >::type >, SIGN > `[`slice`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a3207fc3b3c9e91ca9f52f6e6ded489de)`(S s,const std::string & newname) const` 

#### `public template<>`  <br/>`inline `[`AbstractSignedObservable](#d9/d7a/classalps_1_1_abstract_signed_observable)< [SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< value_type >::type >, SIGN > `[`operator[]`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a50e9814d0db53e5ad8e51add45d8f1b6)`(S s) const` 

#### `public virtual void `[`save`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a38ed58d5362fe0dd576c96d0be18645d)`(ODump & dump) const` 

#### `public virtual void `[`load`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a00bb8241981888814661e02dfbadc102)`(IDump & dump)` 

#### `public virtual void `[`save`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a0b1a2d425d59e5bcdf209097990de77e)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ad9fcfc945af8ef3c76ea6b5f33a4809e)`(hdf5::archive &)` 

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a556d59cbfaeedf4697e2a86366030b08)`() const` 

clones the observable

#### `public inline virtual bool `[`is_signed`](#d9/d7a/classalps_1_1_abstract_signed_observable_1abc9319cf3604aa5f30de62c715af5b83)`() const` 

is the observable signed?

#### `public inline virtual void `[`set_sign_name`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a03898da80ce8686d98d7ce0ae2bd23e3)`(const std::string & signname)` 

set the name of the observable containing the sign for this observable

#### `public virtual void `[`set_sign`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a8fa6c03fb22972f6e67e02bc27ccf99f)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & sign)` 

set the observable containing the sign

#### `public inline virtual void `[`clear_sign`](#d9/d7a/classalps_1_1_abstract_signed_observable_1aede69c19a60d48f20ccb811497ac4b5e)`()` 

clear any previosuly set sign observable

#### `public virtual const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`sign`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a88aa4b55c17c4a6449df9b199ba72aff)`() const` 

get a reference to the sign observable

#### `public inline virtual const std::string `[`sign_name`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ab79f1c246b21cef463871223862db036)`() const` 

get the name of the observable containing the sign

#### `public inline virtual const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`signed_observable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a73f71e14046fea130247dfe25e022136)`() const` 

#### `public inline virtual uint32_t `[`number_of_runs`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a80342d5dc097a0167a4f485fba0182cd)`() const` 

get the number of runs which performed measurements for this observable

#### `public virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`get_run`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a3c132b21b8f0af8e22a5b99a05a9ab5d)`(uint32_t) const` 

extract an observable from a specific run only

#### `protected observable_type `[`obs_`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a42174153c6046a208660f5bb6527de15) 

#### `protected std::string `[`sign_name_`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ae2a6016b3a6cefad1bd1a7900c5c4a10) 

#### `protected const `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`sign_`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a658aa8cb02608b34c8d108aa2ad7ae13) 

#### `protected inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`convert_mergeable`](#d9/d7a/classalps_1_1_abstract_signed_observable_1af9bfa5fa8a4335ba472fb929350797b1)`() const` 

create a copy of the observable that can be merged

#### `protected virtual void `[`write_more_xml`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a7eafa9afddf022037f2214027197fb5f)`(oxstream & oxs,slice_index it) const` 

#### `protected inline virtual void `[`merge`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ac7d64db735e082c84d90b555faf811c3)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & o)` 

#### `protected inline virtual bool `[`can_merge`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ae84e21c5fa71a62fb2bfadaedac4907a)`() const` 

can this observable be merged with one of the same type

#### `protected inline virtual bool `[`can_merge`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a4d567373646127b689522fc29efbc050)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &) const` 

can this observable be merged with one of the given type

#### `typedef `[`observable_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a32a3b0888f8b4e6e251cf1f2bf412b33) 

#### `typedef `[`sign_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ae09913a1d51c3775e4a75e31db9c2c9b) 

#### `typedef `[`value_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a929af477fdffda4d94dbfc4d83db8776) 

#### `typedef `[`result_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a95521a7cd8094cff6cb12372f8587a9a) 

#### `typedef `[`base_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a900ff1f03abd7f118235cfac6c598189) 

#### `typedef `[`slice_index`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a5f420fa3a55a00345e9faab84c98cb26) 

#### `typedef `[`count_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ade9d71f1d9454c5155f11fd8a10d8368) 

#### `typedef `[`time_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1ae56c7b82af0d447a9bdcd9c2a6cbc6a8) 

#### `typedef `[`convergence_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a737c253b0a5762e75a1110d581e802c6) 

#### `typedef `[`label_type`](#d9/d7a/classalps_1_1_abstract_signed_observable_1a4642a432359bc3605118ac4e76fb51a6) 

# class `alps::AbstractSimpleObservable` 

```
class alps::AbstractSimpleObservable
  : public alps::Observable
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable_1ae50525d5c6d9d5829658bd23c16dc437)`(const std::string & name,const label_type & l)` | 
`public inline virtual  `[`~AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable_1aa4e535e7e5a93b198e6bb437460ae721)`()` | 
`public `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`count`](#df/d12/classalps_1_1_abstract_simple_observable_1a877742d9f5f60cbb4eb9d7bed2725757)`() const` | the number of measurements
`public `[`result_type`](#df/d12/classalps_1_1_abstract_simple_observable_1af2c2cc7dd0851ff082f2df00a7c72472)` `[`mean`](#df/d12/classalps_1_1_abstract_simple_observable_1a1054808b5647163a28e9759bfb3d87ea)`() const` | the mean value
`public inline virtual `[`result_type`](#df/d12/classalps_1_1_abstract_simple_observable_1af2c2cc7dd0851ff082f2df00a7c72472)` `[`variance`](#df/d12/classalps_1_1_abstract_simple_observable_1a74a2e4eeacd67417472bc4960f0f6e77)`() const` | the variance
`public `[`result_type`](#df/d12/classalps_1_1_abstract_simple_observable_1af2c2cc7dd0851ff082f2df00a7c72472)` `[`error`](#df/d12/classalps_1_1_abstract_simple_observable_1a411d0377714dcba7a7a236c8dfdfd14e)`() const` | the error
`public convergence_type `[`converged_errors`](#df/d12/classalps_1_1_abstract_simple_observable_1abd2d698d55703e6f3a1a32f1904743b7)`() const` | 
`public inline virtual bool `[`has_minmax`](#df/d12/classalps_1_1_abstract_simple_observable_1ad23c1895621d7d50736ba7edab55e6e0)`() const` | is information about the minimum and maximum value available?
`public inline virtual `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b)` min `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#df/d12/classalps_1_1_abstract_simple_observable_1a7c1ef1f4f274415bcf25fd5da86ec345)`() const` | the minimum value
`public inline virtual `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b)` max `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#df/d12/classalps_1_1_abstract_simple_observable_1a132376d3f5cc58df1694fc4fe22357dd)`() const` | the maximum value
`public inline virtual bool `[`has_tau`](#df/d12/classalps_1_1_abstract_simple_observable_1ab972e2b59f52634eafa36ac493e01bed)`() const` | is autocorrelation information available ?
`public inline virtual `[`time_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a6d3d94b68cc857a65d862416ab2a6461)` `[`tau`](#df/d12/classalps_1_1_abstract_simple_observable_1a15bd46b91c6d1717ae1efe070df766aa)`() const` | the autocorrelation time, throws an exception if not available
`public inline virtual bool `[`has_variance`](#df/d12/classalps_1_1_abstract_simple_observable_1aa9020eaaf3c7b0d631d688ac1e3cf30b)`() const` | is variance available ?
`public inline virtual `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`bin_number`](#df/d12/classalps_1_1_abstract_simple_observable_1a450dd42b677bb80017722436a55cd58b)`() const` | the number of bins
`public inline virtual `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`max_bin_number`](#df/d12/classalps_1_1_abstract_simple_observable_1a03251d88922e853b44f6f9a5a67bf224)`() const` | the number of bins
`public inline virtual `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`bin_size`](#df/d12/classalps_1_1_abstract_simple_observable_1a97ca3cbb58b39c7763f10d8aa32e7d34)`() const` | the number of measurements per bin
`public inline virtual const `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b)` & `[`bin_value`](#df/d12/classalps_1_1_abstract_simple_observable_1a297a05238c80387fbe121c58beb381bc)`(`[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)`) const` | the value of a bin
`public inline virtual `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`bin_number2`](#df/d12/classalps_1_1_abstract_simple_observable_1a517ac29377881226e4b8bee344a4216d)`() const` | the number of bins with squared values
`public inline virtual const `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b)` & `[`bin_value2`](#df/d12/classalps_1_1_abstract_simple_observable_1a285089651e962d576f6d567e230ad5d3)`(`[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)`) const` | the squared value of a bin
`public template<>`  <br/>`inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< T >::type > `[`slice`](#df/d12/classalps_1_1_abstract_simple_observable_1aad160035cb67f736960069e8dced15a1)`(S s,const std::string & newname) const` | slice the data type using a single argument. This can easily be extended when needed to more data types. 
`public template<>`  <br/>`inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< T >::type > `[`operator[]`](#df/d12/classalps_1_1_abstract_simple_observable_1a90611b26557c33a4c1fe71763cfdfd7b)`(S s) const` | 
`public void `[`extract_timeseries`](#df/d12/classalps_1_1_abstract_simple_observable_1a490b39fc003baa1015a03b1e4f95cc11)`(ODump & dump) const` | 
`public virtual void `[`write_xml`](#df/d12/classalps_1_1_abstract_simple_observable_1a7ae43014e6ab2f5fcc45aa0b4ec6d925)`(oxstream & oxs,const boost::filesystem::path & fn_hdf5) const` | output the result
`public void `[`write_xml_scalar`](#df/d12/classalps_1_1_abstract_simple_observable_1a79a0966f46d999f091a1d6dd5741c8d2)`(oxstream &,const boost::filesystem::path &) const` | 
`public void `[`write_xml_vector`](#df/d12/classalps_1_1_abstract_simple_observable_1a61ad2aa55a2ae60671e41ab29ee1a899)`(oxstream &,const boost::filesystem::path &) const` | 
`public inline virtual std::string `[`evaluation_method`](#df/d12/classalps_1_1_abstract_simple_observable_1a4fd82c439cfaf8b76e7af47eae1e1054)`(Target) const` | 
`public inline  `[`operator SimpleObservableEvaluator< value_type >`](#df/d12/classalps_1_1_abstract_simple_observable_1ac08e89c201fc28d0b244e34815318164)`() const` | 
`public inline void `[`set_label`](#df/d12/classalps_1_1_abstract_simple_observable_1a6b2c4cf28cb2276508b5621b029e966c)`(const label_type & l)` | 
`public inline const label_type & `[`label`](#df/d12/classalps_1_1_abstract_simple_observable_1a046ed18795334a4a4cee6c87d27ac35c)`() const` | 
`public inline virtual void `[`save`](#df/d12/classalps_1_1_abstract_simple_observable_1a9c45ce922ce97591b83e639c578c6bc0)`(ODump & dump) const` | 
`public inline virtual void `[`load`](#df/d12/classalps_1_1_abstract_simple_observable_1a591f1ebd5f00a0fe5f9d602a434c2018)`(IDump & dump)` | 
`public virtual void `[`save`](#df/d12/classalps_1_1_abstract_simple_observable_1a1ae3dfb20602ecdc480cd3df2ec511cc)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#df/d12/classalps_1_1_abstract_simple_observable_1af8a502b813117d7fc07d8e6a926bda20)`(hdf5::archive &)` | 
`typedef `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b) | the data type of the observable
`typedef `[`result_type`](#df/d12/classalps_1_1_abstract_simple_observable_1af2c2cc7dd0851ff082f2df00a7c72472) | the data type of averages and errors
`typedef `[`slice_index`](#df/d12/classalps_1_1_abstract_simple_observable_1a6086542a2af48468ec781471de2b603d) | 
`typedef `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca) | the count data type: an integral type
`typedef `[`time_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a6d3d94b68cc857a65d862416ab2a6461) | the data type for autocorrelation times
`typedef `[`convergence_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a25d9e4921055c72b49dc8186a3adad61) | 
`typedef `[`label_type`](#df/d12/classalps_1_1_abstract_simple_observable_1aa3df06c47ff0d7e2b65cc6e79f16dca7) | 

## Members

#### `public inline  `[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable_1ae50525d5c6d9d5829658bd23c16dc437)`(const std::string & name,const label_type & l)` 

#### `public inline virtual  `[`~AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable_1aa4e535e7e5a93b198e6bb437460ae721)`()` 

#### `public `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`count`](#df/d12/classalps_1_1_abstract_simple_observable_1a877742d9f5f60cbb4eb9d7bed2725757)`() const` 

the number of measurements

#### `public `[`result_type`](#df/d12/classalps_1_1_abstract_simple_observable_1af2c2cc7dd0851ff082f2df00a7c72472)` `[`mean`](#df/d12/classalps_1_1_abstract_simple_observable_1a1054808b5647163a28e9759bfb3d87ea)`() const` 

the mean value

#### `public inline virtual `[`result_type`](#df/d12/classalps_1_1_abstract_simple_observable_1af2c2cc7dd0851ff082f2df00a7c72472)` `[`variance`](#df/d12/classalps_1_1_abstract_simple_observable_1a74a2e4eeacd67417472bc4960f0f6e77)`() const` 

the variance

#### `public `[`result_type`](#df/d12/classalps_1_1_abstract_simple_observable_1af2c2cc7dd0851ff082f2df00a7c72472)` `[`error`](#df/d12/classalps_1_1_abstract_simple_observable_1a411d0377714dcba7a7a236c8dfdfd14e)`() const` 

the error

#### `public convergence_type `[`converged_errors`](#df/d12/classalps_1_1_abstract_simple_observable_1abd2d698d55703e6f3a1a32f1904743b7)`() const` 

#### `public inline virtual bool `[`has_minmax`](#df/d12/classalps_1_1_abstract_simple_observable_1ad23c1895621d7d50736ba7edab55e6e0)`() const` 

is information about the minimum and maximum value available?

#### `public inline virtual `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b)` min `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#df/d12/classalps_1_1_abstract_simple_observable_1a7c1ef1f4f274415bcf25fd5da86ec345)`() const` 

the minimum value

#### `public inline virtual `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b)` max `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#df/d12/classalps_1_1_abstract_simple_observable_1a132376d3f5cc58df1694fc4fe22357dd)`() const` 

the maximum value

#### `public inline virtual bool `[`has_tau`](#df/d12/classalps_1_1_abstract_simple_observable_1ab972e2b59f52634eafa36ac493e01bed)`() const` 

is autocorrelation information available ?

#### `public inline virtual `[`time_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a6d3d94b68cc857a65d862416ab2a6461)` `[`tau`](#df/d12/classalps_1_1_abstract_simple_observable_1a15bd46b91c6d1717ae1efe070df766aa)`() const` 

the autocorrelation time, throws an exception if not available

#### `public inline virtual bool `[`has_variance`](#df/d12/classalps_1_1_abstract_simple_observable_1aa9020eaaf3c7b0d631d688ac1e3cf30b)`() const` 

is variance available ?

#### `public inline virtual `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`bin_number`](#df/d12/classalps_1_1_abstract_simple_observable_1a450dd42b677bb80017722436a55cd58b)`() const` 

the number of bins

#### `public inline virtual `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`max_bin_number`](#df/d12/classalps_1_1_abstract_simple_observable_1a03251d88922e853b44f6f9a5a67bf224)`() const` 

the number of bins

#### `public inline virtual `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`bin_size`](#df/d12/classalps_1_1_abstract_simple_observable_1a97ca3cbb58b39c7763f10d8aa32e7d34)`() const` 

the number of measurements per bin

#### `public inline virtual const `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b)` & `[`bin_value`](#df/d12/classalps_1_1_abstract_simple_observable_1a297a05238c80387fbe121c58beb381bc)`(`[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)`) const` 

the value of a bin

#### `public inline virtual `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)` `[`bin_number2`](#df/d12/classalps_1_1_abstract_simple_observable_1a517ac29377881226e4b8bee344a4216d)`() const` 

the number of bins with squared values

#### `public inline virtual const `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b)` & `[`bin_value2`](#df/d12/classalps_1_1_abstract_simple_observable_1a285089651e962d576f6d567e230ad5d3)`(`[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca)`) const` 

the squared value of a bin

#### `public template<>`  <br/>`inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< T >::type > `[`slice`](#df/d12/classalps_1_1_abstract_simple_observable_1aad160035cb67f736960069e8dced15a1)`(S s,const std::string & newname) const` 

slice the data type using a single argument. This can easily be extended when needed to more data types. 
#### Parameters
* `s` the slice 

* `newname` optionally a new name for the slice. Default is the same name as the original observable

#### `public template<>`  <br/>`inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< T >::type > `[`operator[]`](#df/d12/classalps_1_1_abstract_simple_observable_1a90611b26557c33a4c1fe71763cfdfd7b)`(S s) const` 

#### `public void `[`extract_timeseries`](#df/d12/classalps_1_1_abstract_simple_observable_1a490b39fc003baa1015a03b1e4f95cc11)`(ODump & dump) const` 

#### `public virtual void `[`write_xml`](#df/d12/classalps_1_1_abstract_simple_observable_1a7ae43014e6ab2f5fcc45aa0b4ec6d925)`(oxstream & oxs,const boost::filesystem::path & fn_hdf5) const` 

output the result

#### `public void `[`write_xml_scalar`](#df/d12/classalps_1_1_abstract_simple_observable_1a79a0966f46d999f091a1d6dd5741c8d2)`(oxstream &,const boost::filesystem::path &) const` 

#### `public void `[`write_xml_vector`](#df/d12/classalps_1_1_abstract_simple_observable_1a61ad2aa55a2ae60671e41ab29ee1a899)`(oxstream &,const boost::filesystem::path &) const` 

#### `public inline virtual std::string `[`evaluation_method`](#df/d12/classalps_1_1_abstract_simple_observable_1a4fd82c439cfaf8b76e7af47eae1e1054)`(Target) const` 

#### `public inline  `[`operator SimpleObservableEvaluator< value_type >`](#df/d12/classalps_1_1_abstract_simple_observable_1ac08e89c201fc28d0b244e34815318164)`() const` 

#### `public inline void `[`set_label`](#df/d12/classalps_1_1_abstract_simple_observable_1a6b2c4cf28cb2276508b5621b029e966c)`(const label_type & l)` 

#### `public inline const label_type & `[`label`](#df/d12/classalps_1_1_abstract_simple_observable_1a046ed18795334a4a4cee6c87d27ac35c)`() const` 

#### `public inline virtual void `[`save`](#df/d12/classalps_1_1_abstract_simple_observable_1a9c45ce922ce97591b83e639c578c6bc0)`(ODump & dump) const` 

#### `public inline virtual void `[`load`](#df/d12/classalps_1_1_abstract_simple_observable_1a591f1ebd5f00a0fe5f9d602a434c2018)`(IDump & dump)` 

#### `public virtual void `[`save`](#df/d12/classalps_1_1_abstract_simple_observable_1a1ae3dfb20602ecdc480cd3df2ec511cc)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#df/d12/classalps_1_1_abstract_simple_observable_1af8a502b813117d7fc07d8e6a926bda20)`(hdf5::archive &)` 

#### `typedef `[`value_type`](#df/d12/classalps_1_1_abstract_simple_observable_1acba19125692db49213f2d282f5b0700b) 

the data type of the observable

#### `typedef `[`result_type`](#df/d12/classalps_1_1_abstract_simple_observable_1af2c2cc7dd0851ff082f2df00a7c72472) 

the data type of averages and errors

#### `typedef `[`slice_index`](#df/d12/classalps_1_1_abstract_simple_observable_1a6086542a2af48468ec781471de2b603d) 

#### `typedef `[`count_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a9e0d8f265c1fc4c738841e86a33b7bca) 

the count data type: an integral type

#### `typedef `[`time_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a6d3d94b68cc857a65d862416ab2a6461) 

the data type for autocorrelation times

#### `typedef `[`convergence_type`](#df/d12/classalps_1_1_abstract_simple_observable_1a25d9e4921055c72b49dc8186a3adad61) 

#### `typedef `[`label_type`](#df/d12/classalps_1_1_abstract_simple_observable_1aa3df06c47ff0d7e2b65cc6e79f16dca7) 

# class `alps::BasicDetailedBinning` 

```
class alps::BasicDetailedBinning
  : public alps::SimpleBinning< double >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d7/d69/classalps_1_1_basic_detailed_binning_1ac8d9ec6a0b107ebd27faeaa3f5f3c141)`(bool,has_tau)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d7/d69/classalps_1_1_basic_detailed_binning_1ad50a3f4187e9a5305ab11c03f884efbb)`(int,magic_id)` | 
`public inline  `[`BasicDetailedBinning`](#d7/d69/classalps_1_1_basic_detailed_binning_1a85a81436e111fcaf2903e75f2fd69532)`(uint32_t binsize,uint32_t binnum)` | 
`public inline void `[`reset`](#d7/d69/classalps_1_1_basic_detailed_binning_1a5a7a83acf0bd2e4b4d7b02bf81f0025d)`(bool)` | 
`public inline void `[`operator<<`](#d7/d69/classalps_1_1_basic_detailed_binning_1ab556442a3f2dbffaa43d7df6d9cc1e70)`(const T & x)` | 
`public inline uint32_t `[`max_bin_number`](#d7/d69/classalps_1_1_basic_detailed_binning_1aebdb0e2ecda8cad2c421a6537e816a83)`() const` | 
`public inline uint32_t `[`bin_number`](#d7/d69/classalps_1_1_basic_detailed_binning_1ac324df99350b7725f62726c3fb8a8fbf)`() const` | 
`public inline uint32_t `[`filled_bin_number`](#d7/d69/classalps_1_1_basic_detailed_binning_1ab84bf8b90b4070da1fc01a9beb601210)`() const` | 
`public inline uint32_t `[`filled_bin_number2`](#d7/d69/classalps_1_1_basic_detailed_binning_1aa53a44ab41bb1b6b1363f337718ec9a6)`() const` | 
`public void `[`set_bin_number`](#d7/d69/classalps_1_1_basic_detailed_binning_1a7cfb3608aa58be48bd82e4fda87bdd58)`(uint32_t binnum)` | 
`public void `[`collect_bins`](#d7/d69/classalps_1_1_basic_detailed_binning_1af7bcf798e153a33cf64edce09ff74d06)`(uint32_t howmany)` | 
`public inline uint32_t `[`bin_size`](#d7/d69/classalps_1_1_basic_detailed_binning_1aec358b6777f791046431efacf9327128)`() const` | 
`public void `[`set_bin_size`](#d7/d69/classalps_1_1_basic_detailed_binning_1a8b4d73dbd51dfbd4a029bbbfb785d872)`(uint32_t binsize)` | 
`public inline const value_type & `[`bin_value`](#d7/d69/classalps_1_1_basic_detailed_binning_1a57a0a16d8643607bb8f88272029cad5f)`(uint32_t i) const` | 
`public inline const value_type & `[`bin_value2`](#d7/d69/classalps_1_1_basic_detailed_binning_1a86e2268a963b2048da0c851d9d291aad)`(uint32_t i) const` | 
`public inline const std::vector< value_type > & `[`bins`](#d7/d69/classalps_1_1_basic_detailed_binning_1af2f65252d62b603616f8d49b5dfc8c4a)`() const` | 
`public inline void `[`compact`](#d7/d69/classalps_1_1_basic_detailed_binning_1a4331be0bb2a3408dee8426e28531bed0)`()` | 
`public inline void `[`save`](#d7/d69/classalps_1_1_basic_detailed_binning_1ab6c690e87a435bca167921303ba347d9)`(ODump & dump) const` | 
`public inline void `[`load`](#d7/d69/classalps_1_1_basic_detailed_binning_1af14b67611ab832baa9c33fdeb0b1c02a)`(IDump & dump)` | 
`public inline void `[`extract_timeseries`](#d7/d69/classalps_1_1_basic_detailed_binning_1aaae74a7807a35d4777241a1e09e40038)`(ODump & dump) const` | 
`public inline void `[`save`](#d7/d69/classalps_1_1_basic_detailed_binning_1a1eacf46416568723d572c8466afc8c6c)`(hdf5::archive &) const` | 
`public inline void `[`load`](#d7/d69/classalps_1_1_basic_detailed_binning_1a1a0680ffeb29c231922bcf8777d97772)`(hdf5::archive &)` | 
`typedef `[`value_type`](#d7/d69/classalps_1_1_basic_detailed_binning_1a065bcc8e57019166538e524c5bb2909c) | 
`typedef `[`time_type`](#d7/d69/classalps_1_1_basic_detailed_binning_1a30f23de30e5c702d554b2899cb4497d7) | 
`typedef `[`size_type`](#d7/d69/classalps_1_1_basic_detailed_binning_1a8605f3c929cb4b37376f5acdaf828cd1) | 
`typedef `[`result_type`](#d7/d69/classalps_1_1_basic_detailed_binning_1a8d57cec1ce34f5c940cf68e72c485fb6) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d7/d69/classalps_1_1_basic_detailed_binning_1ac8d9ec6a0b107ebd27faeaa3f5f3c141)`(bool,has_tau)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d7/d69/classalps_1_1_basic_detailed_binning_1ad50a3f4187e9a5305ab11c03f884efbb)`(int,magic_id)` 

#### `public inline  `[`BasicDetailedBinning`](#d7/d69/classalps_1_1_basic_detailed_binning_1a85a81436e111fcaf2903e75f2fd69532)`(uint32_t binsize,uint32_t binnum)` 

#### `public inline void `[`reset`](#d7/d69/classalps_1_1_basic_detailed_binning_1a5a7a83acf0bd2e4b4d7b02bf81f0025d)`(bool)` 

#### `public inline void `[`operator<<`](#d7/d69/classalps_1_1_basic_detailed_binning_1ab556442a3f2dbffaa43d7df6d9cc1e70)`(const T & x)` 

#### `public inline uint32_t `[`max_bin_number`](#d7/d69/classalps_1_1_basic_detailed_binning_1aebdb0e2ecda8cad2c421a6537e816a83)`() const` 

#### `public inline uint32_t `[`bin_number`](#d7/d69/classalps_1_1_basic_detailed_binning_1ac324df99350b7725f62726c3fb8a8fbf)`() const` 

#### `public inline uint32_t `[`filled_bin_number`](#d7/d69/classalps_1_1_basic_detailed_binning_1ab84bf8b90b4070da1fc01a9beb601210)`() const` 

#### `public inline uint32_t `[`filled_bin_number2`](#d7/d69/classalps_1_1_basic_detailed_binning_1aa53a44ab41bb1b6b1363f337718ec9a6)`() const` 

#### `public void `[`set_bin_number`](#d7/d69/classalps_1_1_basic_detailed_binning_1a7cfb3608aa58be48bd82e4fda87bdd58)`(uint32_t binnum)` 

#### `public void `[`collect_bins`](#d7/d69/classalps_1_1_basic_detailed_binning_1af7bcf798e153a33cf64edce09ff74d06)`(uint32_t howmany)` 

#### `public inline uint32_t `[`bin_size`](#d7/d69/classalps_1_1_basic_detailed_binning_1aec358b6777f791046431efacf9327128)`() const` 

#### `public void `[`set_bin_size`](#d7/d69/classalps_1_1_basic_detailed_binning_1a8b4d73dbd51dfbd4a029bbbfb785d872)`(uint32_t binsize)` 

#### `public inline const value_type & `[`bin_value`](#d7/d69/classalps_1_1_basic_detailed_binning_1a57a0a16d8643607bb8f88272029cad5f)`(uint32_t i) const` 

#### `public inline const value_type & `[`bin_value2`](#d7/d69/classalps_1_1_basic_detailed_binning_1a86e2268a963b2048da0c851d9d291aad)`(uint32_t i) const` 

#### `public inline const std::vector< value_type > & `[`bins`](#d7/d69/classalps_1_1_basic_detailed_binning_1af2f65252d62b603616f8d49b5dfc8c4a)`() const` 

#### `public inline void `[`compact`](#d7/d69/classalps_1_1_basic_detailed_binning_1a4331be0bb2a3408dee8426e28531bed0)`()` 

#### `public inline void `[`save`](#d7/d69/classalps_1_1_basic_detailed_binning_1ab6c690e87a435bca167921303ba347d9)`(ODump & dump) const` 

#### `public inline void `[`load`](#d7/d69/classalps_1_1_basic_detailed_binning_1af14b67611ab832baa9c33fdeb0b1c02a)`(IDump & dump)` 

#### `public inline void `[`extract_timeseries`](#d7/d69/classalps_1_1_basic_detailed_binning_1aaae74a7807a35d4777241a1e09e40038)`(ODump & dump) const` 

#### `public inline void `[`save`](#d7/d69/classalps_1_1_basic_detailed_binning_1a1eacf46416568723d572c8466afc8c6c)`(hdf5::archive &) const` 

#### `public inline void `[`load`](#d7/d69/classalps_1_1_basic_detailed_binning_1a1a0680ffeb29c231922bcf8777d97772)`(hdf5::archive &)` 

#### `typedef `[`value_type`](#d7/d69/classalps_1_1_basic_detailed_binning_1a065bcc8e57019166538e524c5bb2909c) 

#### `typedef `[`time_type`](#d7/d69/classalps_1_1_basic_detailed_binning_1a30f23de30e5c702d554b2899cb4497d7) 

#### `typedef `[`size_type`](#d7/d69/classalps_1_1_basic_detailed_binning_1a8605f3c929cb4b37376f5acdaf828cd1) 

#### `typedef `[`result_type`](#d7/d69/classalps_1_1_basic_detailed_binning_1a8d57cec1ce34f5c940cf68e72c485fb6) 

# class `alps::DetailedBinning` 

```
class alps::DetailedBinning
  : public alps::BasicDetailedBinning< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#da/dd8/classalps_1_1_detailed_binning_1ab88975b9952c0b7d872c4a66f47ed73b)`(int,magic_id)` | 
`public inline  `[`DetailedBinning`](#da/dd8/classalps_1_1_detailed_binning_1af528169f0c4e86d9964939a659e9e4eb)`(uint32_t binnum,uint32_t)` | 
`typedef `[`value_type`](#da/dd8/classalps_1_1_detailed_binning_1acd590ad5eaf5eca1638b77cbbb50b83e) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#da/dd8/classalps_1_1_detailed_binning_1ab88975b9952c0b7d872c4a66f47ed73b)`(int,magic_id)` 

#### `public inline  `[`DetailedBinning`](#da/dd8/classalps_1_1_detailed_binning_1af528169f0c4e86d9964939a659e9e4eb)`(uint32_t binnum,uint32_t)` 

#### `typedef `[`value_type`](#da/dd8/classalps_1_1_detailed_binning_1acd590ad5eaf5eca1638b77cbbb50b83e) 

# class `alps::FixedBinning` 

```
class alps::FixedBinning
  : public alps::BasicDetailedBinning< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#df/d7c/classalps_1_1_fixed_binning_1a1bb2bb67a5b36d273f7d4ea28d679827)`(int,magic_id)` | 
`public inline  `[`FixedBinning`](#df/d7c/classalps_1_1_fixed_binning_1aca5295f5688f97f17041a0279769c173)`(uint32_t binsize,uint32_t)` | 
`typedef `[`value_type`](#df/d7c/classalps_1_1_fixed_binning_1a6b9d9e3b8fae4ee621ab24bf12ae8802) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#df/d7c/classalps_1_1_fixed_binning_1a1bb2bb67a5b36d273f7d4ea28d679827)`(int,magic_id)` 

#### `public inline  `[`FixedBinning`](#df/d7c/classalps_1_1_fixed_binning_1aca5295f5688f97f17041a0279769c173)`(uint32_t binsize,uint32_t)` 

#### `typedef `[`value_type`](#df/d7c/classalps_1_1_fixed_binning_1a6b9d9e3b8fae4ee621ab24bf12ae8802) 

# class `alps::HistogramObservable` 

```
class alps::HistogramObservable
  : public alps::Observable
  : public alps::RecordableObservable< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d5/d10/classalps_1_1_histogram_observable_1a78c67ae3fb1c5d41853a5d95e7b8f12d)`(uint32_t,version)` | 
`public  `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable_1abba800051fe53b920f75caf8c5145d58)`(const std::string & n)` | 
`public inline  `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable_1a6fdea9abfc1289058c297be7db1c0a76)`(const std::string & n,T min,T max,T stepsize)` | 
`public inline void `[`set_range`](#d5/d10/classalps_1_1_histogram_observable_1a421f6e86a2714b1a712690ac5b69724d)`(T min,T max,T stepsize)` | 
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#d5/d10/classalps_1_1_histogram_observable_1a68fd8ccb4db6b078aa00600173a6ddb7)`() const` | clones the observable
`public inline virtual ALPS_DUMMY_VOID `[`reset`](#d5/d10/classalps_1_1_histogram_observable_1a85ded5480c22826ad1d9cc842d628ea9)`(bool equilibrated)` | reset the observable
`public inline virtual ALPS_DUMMY_VOID `[`output`](#d5/d10/classalps_1_1_histogram_observable_1a8a663ee46592aa552d6efd686ef317c8)`(std::ostream &) const` | output the result
`public inline virtual uint32_t `[`version_id`](#d5/d10/classalps_1_1_histogram_observable_1a266aee8b52f17bb525e122181a8301bf)`() const` | return a version ID uniquely identifying the class
`public inline virtual void `[`save`](#d5/d10/classalps_1_1_histogram_observable_1adfd17b5aa3d746b054adf525ac6fb5cf)`(ODump & dump) const` | 
`public inline virtual void `[`load`](#d5/d10/classalps_1_1_histogram_observable_1af334e1ea705fcdce9df252710226dc87)`(IDump & dump)` | 
`public inline virtual void `[`add`](#d5/d10/classalps_1_1_histogram_observable_1a55db64ca8744c1363aad4f86187c6f51)`(const T & x)` | add a simple T-value to the [Observable](#df/d26/classalps_1_1_observable)
`public inline virtual void `[`operator<<`](#d5/d10/classalps_1_1_histogram_observable_1a4c4c02725a20effeb12a3231511e30a8)`(const T & x)` | add a simple T-value to the [Observable](#df/d26/classalps_1_1_observable)
`public inline const_iterator `[`begin`](#d5/d10/classalps_1_1_histogram_observable_1af9401b6aeaa494e93eed928ed1029dbd)`() const` | 
`public inline const_iterator `[`rbegin`](#d5/d10/classalps_1_1_histogram_observable_1a9e5a9c0872a82a864e935037a4d65e38)`() const` | 
`public inline const_iterator `[`end`](#d5/d10/classalps_1_1_histogram_observable_1ab86bf90157d6adabc33f6e4afb401e5e)`() const` | 
`public inline const_iterator `[`rend`](#d5/d10/classalps_1_1_histogram_observable_1ab0a2cd3ef12773f4879c85f88ca948a5)`() const` | 
`public inline size_type `[`size`](#d5/d10/classalps_1_1_histogram_observable_1a68b4eb0321e896269d0a5050ca6ad3c0)`() const` | 
`public inline value_type `[`operator[]`](#d5/d10/classalps_1_1_histogram_observable_1a7d99267b5875fce2bafb20c00d8cc8fc)`(size_type i) const` | 
`public inline value_type `[`at`](#d5/d10/classalps_1_1_histogram_observable_1ab154d9af1f8519662b4123a230d82164)`(size_type i) const` | 
`public inline virtual bool `[`can_merge`](#d5/d10/classalps_1_1_histogram_observable_1aaaba25644ffe7098775e1abbb7f7101f)`() const` | can this observable be merged with one of the same type
`public inline virtual bool `[`can_merge`](#d5/d10/classalps_1_1_histogram_observable_1aa0a43bbf4bd4f14f23e70599c9b4b8be)`(const `[`alps::Observable`](#df/d26/classalps_1_1_observable)` &) const` | can this observable be merged with one of the given type
`public inline value_type & `[`operator[]`](#d5/d10/classalps_1_1_histogram_observable_1a7f369bb936666badaf7997ba9d0d76bf)`(size_type i)` | 
`public virtual void `[`write_xml`](#d5/d10/classalps_1_1_histogram_observable_1a240d3160497591a60afa876453b929e3)`(oxstream & oxs,const boost::filesystem::path & fn_hdf5) const` | output the result
`public inline count_type `[`count`](#d5/d10/classalps_1_1_histogram_observable_1aec95a08073fb4b497add6a272e760537)`() const` | 
`public inline range_type `[`stepsize`](#d5/d10/classalps_1_1_histogram_observable_1ab9d2aeeb57ddecc75e86607483c74aae)`() const` | 
`public inline range_type max `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#d5/d10/classalps_1_1_histogram_observable_1a698359d72ec2370d6ed640449c4cbe66)`() const` | 
`public inline range_type min `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#d5/d10/classalps_1_1_histogram_observable_1a96dc3729b8e018f6d1548e0ddbb6905a)`() const` | 
`public inline  `[`operator HistogramObservableEvaluator< T >`](#d5/d10/classalps_1_1_histogram_observable_1a8a4e4a6577a810a7697ec7179990c644)`() const` | 
`public inline virtual void `[`save`](#d5/d10/classalps_1_1_histogram_observable_1a34916b54770d9a53c10e80e363722640)`(hdf5::archive &) const` | 
`public inline virtual void `[`load`](#d5/d10/classalps_1_1_histogram_observable_1a5a9abaede9ceef0c1a1e11d49f73ed57)`(hdf5::archive &)` | 
`protected mutable std::vector< value_type > `[`histogram_`](#d5/d10/classalps_1_1_histogram_observable_1a703139a91f0899b6167d631a75e218e2) | 
`protected mutable count_type `[`count_`](#d5/d10/classalps_1_1_histogram_observable_1ad2c8edbce09168dd8164ed8cdd4a1123) | 
`typedef `[`value_type`](#d5/d10/classalps_1_1_histogram_observable_1a490eb221ada21258f30294e97fa1ee92) | 
`typedef `[`range_type`](#d5/d10/classalps_1_1_histogram_observable_1af7ff905675ee9dbbcc3466b7125063a1) | 
`typedef `[`count_type`](#d5/d10/classalps_1_1_histogram_observable_1a9652fda53eda77f3236d54a4bee998a0) | 
`typedef `[`const_iterator`](#d5/d10/classalps_1_1_histogram_observable_1a563454fb7449daf6b86e949e632f8e6e) | 
`typedef `[`const_reverse_iterator`](#d5/d10/classalps_1_1_histogram_observable_1af8e98973f0c7a3935d1908e2e1e001bf) | 
`typedef `[`size_type`](#d5/d10/classalps_1_1_histogram_observable_1aa94b93bc0f16e0d5a5e58d1fe6102e6c) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d5/d10/classalps_1_1_histogram_observable_1a78c67ae3fb1c5d41853a5d95e7b8f12d)`(uint32_t,version)` 

#### `public  `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable_1abba800051fe53b920f75caf8c5145d58)`(const std::string & n)` 

#### `public inline  `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable_1a6fdea9abfc1289058c297be7db1c0a76)`(const std::string & n,T min,T max,T stepsize)` 

#### `public inline void `[`set_range`](#d5/d10/classalps_1_1_histogram_observable_1a421f6e86a2714b1a712690ac5b69724d)`(T min,T max,T stepsize)` 

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#d5/d10/classalps_1_1_histogram_observable_1a68fd8ccb4db6b078aa00600173a6ddb7)`() const` 

clones the observable

#### `public inline virtual ALPS_DUMMY_VOID `[`reset`](#d5/d10/classalps_1_1_histogram_observable_1a85ded5480c22826ad1d9cc842d628ea9)`(bool equilibrated)` 

reset the observable

#### `public inline virtual ALPS_DUMMY_VOID `[`output`](#d5/d10/classalps_1_1_histogram_observable_1a8a663ee46592aa552d6efd686ef317c8)`(std::ostream &) const` 

output the result

#### `public inline virtual uint32_t `[`version_id`](#d5/d10/classalps_1_1_histogram_observable_1a266aee8b52f17bb525e122181a8301bf)`() const` 

return a version ID uniquely identifying the class

#### `public inline virtual void `[`save`](#d5/d10/classalps_1_1_histogram_observable_1adfd17b5aa3d746b054adf525ac6fb5cf)`(ODump & dump) const` 

#### `public inline virtual void `[`load`](#d5/d10/classalps_1_1_histogram_observable_1af334e1ea705fcdce9df252710226dc87)`(IDump & dump)` 

#### `public inline virtual void `[`add`](#d5/d10/classalps_1_1_histogram_observable_1a55db64ca8744c1363aad4f86187c6f51)`(const T & x)` 

add a simple T-value to the [Observable](#df/d26/classalps_1_1_observable)

#### `public inline virtual void `[`operator<<`](#d5/d10/classalps_1_1_histogram_observable_1a4c4c02725a20effeb12a3231511e30a8)`(const T & x)` 

add a simple T-value to the [Observable](#df/d26/classalps_1_1_observable)

#### `public inline const_iterator `[`begin`](#d5/d10/classalps_1_1_histogram_observable_1af9401b6aeaa494e93eed928ed1029dbd)`() const` 

#### `public inline const_iterator `[`rbegin`](#d5/d10/classalps_1_1_histogram_observable_1a9e5a9c0872a82a864e935037a4d65e38)`() const` 

#### `public inline const_iterator `[`end`](#d5/d10/classalps_1_1_histogram_observable_1ab86bf90157d6adabc33f6e4afb401e5e)`() const` 

#### `public inline const_iterator `[`rend`](#d5/d10/classalps_1_1_histogram_observable_1ab0a2cd3ef12773f4879c85f88ca948a5)`() const` 

#### `public inline size_type `[`size`](#d5/d10/classalps_1_1_histogram_observable_1a68b4eb0321e896269d0a5050ca6ad3c0)`() const` 

#### `public inline value_type `[`operator[]`](#d5/d10/classalps_1_1_histogram_observable_1a7d99267b5875fce2bafb20c00d8cc8fc)`(size_type i) const` 

#### `public inline value_type `[`at`](#d5/d10/classalps_1_1_histogram_observable_1ab154d9af1f8519662b4123a230d82164)`(size_type i) const` 

#### `public inline virtual bool `[`can_merge`](#d5/d10/classalps_1_1_histogram_observable_1aaaba25644ffe7098775e1abbb7f7101f)`() const` 

can this observable be merged with one of the same type

#### `public inline virtual bool `[`can_merge`](#d5/d10/classalps_1_1_histogram_observable_1aa0a43bbf4bd4f14f23e70599c9b4b8be)`(const `[`alps::Observable`](#df/d26/classalps_1_1_observable)` &) const` 

can this observable be merged with one of the given type

#### `public inline value_type & `[`operator[]`](#d5/d10/classalps_1_1_histogram_observable_1a7f369bb936666badaf7997ba9d0d76bf)`(size_type i)` 

#### `public virtual void `[`write_xml`](#d5/d10/classalps_1_1_histogram_observable_1a240d3160497591a60afa876453b929e3)`(oxstream & oxs,const boost::filesystem::path & fn_hdf5) const` 

output the result

#### `public inline count_type `[`count`](#d5/d10/classalps_1_1_histogram_observable_1aec95a08073fb4b497add6a272e760537)`() const` 

#### `public inline range_type `[`stepsize`](#d5/d10/classalps_1_1_histogram_observable_1ab9d2aeeb57ddecc75e86607483c74aae)`() const` 

#### `public inline range_type max `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#d5/d10/classalps_1_1_histogram_observable_1a698359d72ec2370d6ed640449c4cbe66)`() const` 

#### `public inline range_type min `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#d5/d10/classalps_1_1_histogram_observable_1a96dc3729b8e018f6d1548e0ddbb6905a)`() const` 

#### `public inline  `[`operator HistogramObservableEvaluator< T >`](#d5/d10/classalps_1_1_histogram_observable_1a8a4e4a6577a810a7697ec7179990c644)`() const` 

#### `public inline virtual void `[`save`](#d5/d10/classalps_1_1_histogram_observable_1a34916b54770d9a53c10e80e363722640)`(hdf5::archive &) const` 

#### `public inline virtual void `[`load`](#d5/d10/classalps_1_1_histogram_observable_1a5a9abaede9ceef0c1a1e11d49f73ed57)`(hdf5::archive &)` 

#### `protected mutable std::vector< value_type > `[`histogram_`](#d5/d10/classalps_1_1_histogram_observable_1a703139a91f0899b6167d631a75e218e2) 

#### `protected mutable count_type `[`count_`](#d5/d10/classalps_1_1_histogram_observable_1ad2c8edbce09168dd8164ed8cdd4a1123) 

#### `typedef `[`value_type`](#d5/d10/classalps_1_1_histogram_observable_1a490eb221ada21258f30294e97fa1ee92) 

#### `typedef `[`range_type`](#d5/d10/classalps_1_1_histogram_observable_1af7ff905675ee9dbbcc3466b7125063a1) 

#### `typedef `[`count_type`](#d5/d10/classalps_1_1_histogram_observable_1a9652fda53eda77f3236d54a4bee998a0) 

#### `typedef `[`const_iterator`](#d5/d10/classalps_1_1_histogram_observable_1a563454fb7449daf6b86e949e632f8e6e) 

#### `typedef `[`const_reverse_iterator`](#d5/d10/classalps_1_1_histogram_observable_1af8e98973f0c7a3935d1908e2e1e001bf) 

#### `typedef `[`size_type`](#d5/d10/classalps_1_1_histogram_observable_1aa94b93bc0f16e0d5a5e58d1fe6102e6c) 

# class `alps::HistogramObservableData` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data_1af302b18660873532ce4f3c4f6a84115f)`()` | 
`public inline  `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data_1ab5961142e3ca1632b991dee39de41a75)`(const `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable)`< T > & obs)` | 
`public inline  `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data_1a3f9c3db7d329880a8dc3d84b15090339)`(std::istream & infile,const XMLTag & intag)` | 
`public inline size_type `[`size`](#d2/dae/classalps_1_1_histogram_observable_data_1a193d6dfd798de42ed6759fdeae994ea1)`() const` | 
`public inline void `[`read_xml`](#d2/dae/classalps_1_1_histogram_observable_data_1ac697fbd19d364a207ef4a67df234ef54)`(std::istream & infile,const XMLTag & intag)` | 
`public inline void `[`read_xml_histogram`](#d2/dae/classalps_1_1_histogram_observable_data_1af0e7d593b5d614e8ad10ba43ac796b35)`(std::istream & infile,const XMLTag & intag)` | 
`public inline count_type `[`count`](#d2/dae/classalps_1_1_histogram_observable_data_1a8c7cf764b8520e53a775c13d2193f740)`() const` | 
`public size_type `[`value`](#d2/dae/classalps_1_1_histogram_observable_data_1a5379e07c260cd4822564eea5735e4e4c)`(uint32_t) const` | 
`public inline range_type min `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#d2/dae/classalps_1_1_histogram_observable_data_1ab3450663a9adb97a83eebf7258eab297)`() const` | 
`public inline range_type max `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#d2/dae/classalps_1_1_histogram_observable_data_1a5f2ffccf2dfb2d9f4512f041edba5c12)`() const` | 
`public inline range_type `[`stepsize`](#d2/dae/classalps_1_1_histogram_observable_data_1ab75a2b53b6b7c1f5df2247536bd5c341)`() const` | 
`public inline void `[`save`](#d2/dae/classalps_1_1_histogram_observable_data_1a7c6dd19033c5a6872d7d39857ef4e161)`(ODump & dump) const` | 
`public inline void `[`load`](#d2/dae/classalps_1_1_histogram_observable_data_1a97e80168c72b3a54d03c4e3e1667c618)`(IDump & dump)` | 
`public inline void `[`collect_from`](#d2/dae/classalps_1_1_histogram_observable_data_1a096dfb504cc6342e1c4fcef38b7d855b)`(const std::vector< `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data)`< T > > & runs)` | 
`public inline value_type `[`operator[]`](#d2/dae/classalps_1_1_histogram_observable_data_1a94ff1d41c17669463dad490bcaab99db)`(size_type i) const` | 
`typedef `[`integer_type`](#d2/dae/classalps_1_1_histogram_observable_data_1ab2c4206e3983caf278630899965b4428) | 
`typedef `[`value_type`](#d2/dae/classalps_1_1_histogram_observable_data_1ade4759cd64e268ab573cfd79bd87305d) | 
`typedef `[`size_type`](#d2/dae/classalps_1_1_histogram_observable_data_1afeccca6d004ded012def9b1beb2522f6) | 
`typedef `[`count_type`](#d2/dae/classalps_1_1_histogram_observable_data_1a6a4f941c70acafc15bd6a613fa59d593) | 
`typedef `[`range_type`](#d2/dae/classalps_1_1_histogram_observable_data_1a33d651dd5d808f8276dcaaeb27f4fd76) | 

## Members

#### `public inline  `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data_1af302b18660873532ce4f3c4f6a84115f)`()` 

#### `public inline  `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data_1ab5961142e3ca1632b991dee39de41a75)`(const `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable)`< T > & obs)` 

#### `public inline  `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data_1a3f9c3db7d329880a8dc3d84b15090339)`(std::istream & infile,const XMLTag & intag)` 

#### `public inline size_type `[`size`](#d2/dae/classalps_1_1_histogram_observable_data_1a193d6dfd798de42ed6759fdeae994ea1)`() const` 

#### `public inline void `[`read_xml`](#d2/dae/classalps_1_1_histogram_observable_data_1ac697fbd19d364a207ef4a67df234ef54)`(std::istream & infile,const XMLTag & intag)` 

#### `public inline void `[`read_xml_histogram`](#d2/dae/classalps_1_1_histogram_observable_data_1af0e7d593b5d614e8ad10ba43ac796b35)`(std::istream & infile,const XMLTag & intag)` 

#### `public inline count_type `[`count`](#d2/dae/classalps_1_1_histogram_observable_data_1a8c7cf764b8520e53a775c13d2193f740)`() const` 

#### `public size_type `[`value`](#d2/dae/classalps_1_1_histogram_observable_data_1a5379e07c260cd4822564eea5735e4e4c)`(uint32_t) const` 

#### `public inline range_type min `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#d2/dae/classalps_1_1_histogram_observable_data_1ab3450663a9adb97a83eebf7258eab297)`() const` 

#### `public inline range_type max `[`BOOST_PREVENT_MACRO_SUBSTITUTION`](#d2/dae/classalps_1_1_histogram_observable_data_1a5f2ffccf2dfb2d9f4512f041edba5c12)`() const` 

#### `public inline range_type `[`stepsize`](#d2/dae/classalps_1_1_histogram_observable_data_1ab75a2b53b6b7c1f5df2247536bd5c341)`() const` 

#### `public inline void `[`save`](#d2/dae/classalps_1_1_histogram_observable_data_1a7c6dd19033c5a6872d7d39857ef4e161)`(ODump & dump) const` 

#### `public inline void `[`load`](#d2/dae/classalps_1_1_histogram_observable_data_1a97e80168c72b3a54d03c4e3e1667c618)`(IDump & dump)` 

#### `public inline void `[`collect_from`](#d2/dae/classalps_1_1_histogram_observable_data_1a096dfb504cc6342e1c4fcef38b7d855b)`(const std::vector< `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data)`< T > > & runs)` 

#### `public inline value_type `[`operator[]`](#d2/dae/classalps_1_1_histogram_observable_data_1a94ff1d41c17669463dad490bcaab99db)`(size_type i) const` 

#### `typedef `[`integer_type`](#d2/dae/classalps_1_1_histogram_observable_data_1ab2c4206e3983caf278630899965b4428) 

#### `typedef `[`value_type`](#d2/dae/classalps_1_1_histogram_observable_data_1ade4759cd64e268ab573cfd79bd87305d) 

#### `typedef `[`size_type`](#d2/dae/classalps_1_1_histogram_observable_data_1afeccca6d004ded012def9b1beb2522f6) 

#### `typedef `[`count_type`](#d2/dae/classalps_1_1_histogram_observable_data_1a6a4f941c70acafc15bd6a613fa59d593) 

#### `typedef `[`range_type`](#d2/dae/classalps_1_1_histogram_observable_data_1a33d651dd5d808f8276dcaaeb27f4fd76) 

# class `alps::HistogramObservableEvaluator` 

```
class alps::HistogramObservableEvaluator
  : public alps::HistogramObservable< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a4baf3d5c3580a99d6fe5f3882dce52d3)`(uint32_t,version)` | 
`public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a388cad0af73ebfe9b10f90672dd9f00c)`(const std::string & n)` | 
`public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1af8a7e28220f4cddd7b5f181a672d5c20)`(const char * n)` | 
`public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1ac1affeba4b2aea747aeb40c80ad3e839)`(const `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)` & eval)` | 
`public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1aea58e2292ef25f2814faccc849216346)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs,const std::string &)` | 
`public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a2a8471ae9308496999285d360877d5b8)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &)` | 
`public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a51b365130065200d0f4214eaa4e65feb)`(const std::string & n,std::istream &,const XMLTag &)` | 
`public inline virtual  `[`~HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a7668ab12e2c10af787a1d79b26a11f28)`()` | 
`public inline const `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > & `[`operator=`](#df/dce/classalps_1_1_histogram_observable_evaluator_1ab9feda1523b7931ddfb2afa913c14a9c)`(const `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > & eval)` | 
`public inline const `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > & `[`operator=`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a9e8a3dcfa071a623faf538bd2b998eac)`(const `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable)`< T > & obs)` | 
`public inline `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > & `[`operator<<`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a40e18b6ef9083d66b819d6b6e999f746)`(const `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable)`< T > & obs)` | 
`public inline virtual void `[`rename`](#df/dce/classalps_1_1_histogram_observable_evaluator_1af7f2c91b0ce8783141c111be8a253ec9)`(const std::string &)` | rename the observable
`public inline void `[`rename`](#df/dce/classalps_1_1_histogram_observable_evaluator_1abade5356e5914acb2df3a00630fe2ca5)`(const std::string n,bool a)` | 
`public inline virtual ALPS_DUMMY_VOID `[`reset`](#df/dce/classalps_1_1_histogram_observable_evaluator_1aba6096ff922647097568a2d71a25e028)`(bool equilibrated)` | reset the observable
`public inline value_type `[`operator[]`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a0d04a589c1a1f0acb4f1bd5b36b13cb0)`(int i) const` | 
`public inline count_type `[`count`](#df/dce/classalps_1_1_histogram_observable_evaluator_1af3f1859ae9bf8263811b6a8f5248b449)`() const` | 
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a838031dc68096fe4e1a33d9b9d1c1d4f)`() const` | clones the observable
`public inline virtual uint32_t `[`number_of_runs`](#df/dce/classalps_1_1_histogram_observable_evaluator_1abb71b9536b42056c160145d52bd5fa54)`() const` | get the number of runs which performed measurements for this observable
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`get_run`](#df/dce/classalps_1_1_histogram_observable_evaluator_1aa20f69061bd8f6d078c7ff53dfec9429)`(uint32_t) const` | extract an observable from a specific run only
`public virtual ALPS_DUMMY_VOID `[`output`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a0e2b2e0c580e442575fb8886cafa325c)`(std::ostream &) const` | output the result
`public void `[`output_histogram`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a06b4665f8bbaf102a56a8b6d37d5d625)`(std::ostream &) const` | 
`public inline void `[`operator<<`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a79529d821ee74b771764c538fc576aff)`(const `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data)`< T > & obs)` | 
`public inline virtual uint32_t `[`version_id`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a771d6640d0445a00808d43fd33bccf74)`() const` | return a version ID uniquely identifying the class
`public inline virtual void `[`save`](#df/dce/classalps_1_1_histogram_observable_evaluator_1aef734378f1f4cd3e53ffecef1f92dc2a)`(ODump & dump) const` | 
`public inline virtual void `[`load`](#df/dce/classalps_1_1_histogram_observable_evaluator_1ad52f4699d8323596a790c5e5aa9cdca6)`(IDump & dump)` | 
`public inline virtual void `[`merge`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a2bffec95d794b6c95f79e13e0af5697a)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &)` | 
`public inline virtual bool `[`can_merge`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a7e9e5b0606b3c57e27c0883f3a9c2cf1)`() const` | can this observable be merged with one of the same type
`public inline virtual bool `[`can_merge`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a3b40f2f91292a234a5887747afd28345)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &) const` | can this observable be merged with one of the given type
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`convert_mergeable`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a929280671949d11e1489d2cdc4c6ccd7)`() const` | create a copy of the observable that can be merged
`public inline virtual `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > `[`make_evaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1ad4171254b5af0f76511cdb5024555b2f)`() const` | 
`typedef `[`value_type`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a78e87bf784858c30053def84e926acc5) | 
`typedef `[`range_type`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a2509f184dcccaa8b024281df1c56fa63) | 
`typedef `[`count_type`](#df/dce/classalps_1_1_histogram_observable_evaluator_1af049cddc6894c20fb8100439d31eb728) | 
`typedef `[`iterator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a97e6434190d8b372a3ef57094c65e5d3) | 
`typedef `[`const_iterator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a7f869f2f0ece34fbf8895adbf063c7d2) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a4baf3d5c3580a99d6fe5f3882dce52d3)`(uint32_t,version)` 

#### `public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a388cad0af73ebfe9b10f90672dd9f00c)`(const std::string & n)` 

#### `public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1af8a7e28220f4cddd7b5f181a672d5c20)`(const char * n)` 

#### `public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1ac1affeba4b2aea747aeb40c80ad3e839)`(const `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)` & eval)` 

#### `public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1aea58e2292ef25f2814faccc849216346)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs,const std::string &)` 

#### `public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a2a8471ae9308496999285d360877d5b8)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &)` 

#### `public inline  `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a51b365130065200d0f4214eaa4e65feb)`(const std::string & n,std::istream &,const XMLTag &)` 

#### `public inline virtual  `[`~HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a7668ab12e2c10af787a1d79b26a11f28)`()` 

#### `public inline const `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > & `[`operator=`](#df/dce/classalps_1_1_histogram_observable_evaluator_1ab9feda1523b7931ddfb2afa913c14a9c)`(const `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > & eval)` 

#### `public inline const `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > & `[`operator=`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a9e8a3dcfa071a623faf538bd2b998eac)`(const `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable)`< T > & obs)` 

#### `public inline `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > & `[`operator<<`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a40e18b6ef9083d66b819d6b6e999f746)`(const `[`HistogramObservable`](#d5/d10/classalps_1_1_histogram_observable)`< T > & obs)` 

#### `public inline virtual void `[`rename`](#df/dce/classalps_1_1_histogram_observable_evaluator_1af7f2c91b0ce8783141c111be8a253ec9)`(const std::string &)` 

rename the observable

#### `public inline void `[`rename`](#df/dce/classalps_1_1_histogram_observable_evaluator_1abade5356e5914acb2df3a00630fe2ca5)`(const std::string n,bool a)` 

#### `public inline virtual ALPS_DUMMY_VOID `[`reset`](#df/dce/classalps_1_1_histogram_observable_evaluator_1aba6096ff922647097568a2d71a25e028)`(bool equilibrated)` 

reset the observable

#### `public inline value_type `[`operator[]`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a0d04a589c1a1f0acb4f1bd5b36b13cb0)`(int i) const` 

#### `public inline count_type `[`count`](#df/dce/classalps_1_1_histogram_observable_evaluator_1af3f1859ae9bf8263811b6a8f5248b449)`() const` 

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a838031dc68096fe4e1a33d9b9d1c1d4f)`() const` 

clones the observable

#### `public inline virtual uint32_t `[`number_of_runs`](#df/dce/classalps_1_1_histogram_observable_evaluator_1abb71b9536b42056c160145d52bd5fa54)`() const` 

get the number of runs which performed measurements for this observable

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`get_run`](#df/dce/classalps_1_1_histogram_observable_evaluator_1aa20f69061bd8f6d078c7ff53dfec9429)`(uint32_t) const` 

extract an observable from a specific run only

#### `public virtual ALPS_DUMMY_VOID `[`output`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a0e2b2e0c580e442575fb8886cafa325c)`(std::ostream &) const` 

output the result

#### `public void `[`output_histogram`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a06b4665f8bbaf102a56a8b6d37d5d625)`(std::ostream &) const` 

#### `public inline void `[`operator<<`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a79529d821ee74b771764c538fc576aff)`(const `[`HistogramObservableData`](#d2/dae/classalps_1_1_histogram_observable_data)`< T > & obs)` 

#### `public inline virtual uint32_t `[`version_id`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a771d6640d0445a00808d43fd33bccf74)`() const` 

return a version ID uniquely identifying the class

#### `public inline virtual void `[`save`](#df/dce/classalps_1_1_histogram_observable_evaluator_1aef734378f1f4cd3e53ffecef1f92dc2a)`(ODump & dump) const` 

#### `public inline virtual void `[`load`](#df/dce/classalps_1_1_histogram_observable_evaluator_1ad52f4699d8323596a790c5e5aa9cdca6)`(IDump & dump)` 

#### `public inline virtual void `[`merge`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a2bffec95d794b6c95f79e13e0af5697a)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &)` 

#### `public inline virtual bool `[`can_merge`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a7e9e5b0606b3c57e27c0883f3a9c2cf1)`() const` 

can this observable be merged with one of the same type

#### `public inline virtual bool `[`can_merge`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a3b40f2f91292a234a5887747afd28345)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &) const` 

can this observable be merged with one of the given type

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`convert_mergeable`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a929280671949d11e1489d2cdc4c6ccd7)`() const` 

create a copy of the observable that can be merged

#### `public inline virtual `[`HistogramObservableEvaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator)`< T > `[`make_evaluator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1ad4171254b5af0f76511cdb5024555b2f)`() const` 

#### `typedef `[`value_type`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a78e87bf784858c30053def84e926acc5) 

#### `typedef `[`range_type`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a2509f184dcccaa8b024281df1c56fa63) 

#### `typedef `[`count_type`](#df/dce/classalps_1_1_histogram_observable_evaluator_1af049cddc6894c20fb8100439d31eb728) 

#### `typedef `[`iterator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a97e6434190d8b372a3ef57094c65e5d3) 

#### `typedef `[`const_iterator`](#df/dce/classalps_1_1_histogram_observable_evaluator_1a7f869f2f0ece34fbf8895adbf063c7d2) 

# class `alps::NoBinning` 

```
class alps::NoBinning
  : public alps::AbstractBinning< double >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d6/dba/classalps_1_1_no_binning_1a8ce6e89801af5b34e88eaf098a3697b6)`(bool,has_tau)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d6/dba/classalps_1_1_no_binning_1ae33c0558b2e8482821455fb7b39b8946)`(int,magic_id)` | 
`public inline  `[`NoBinning`](#d6/dba/classalps_1_1_no_binning_1a13bef9b2f1a4426e9c0a1ab0e720774c)`(uint32_t,uint32_t)` | 
`public inline void `[`reset`](#d6/dba/classalps_1_1_no_binning_1a09d6f718dc98cc54909e488b1f5fd323)`(bool)` | 
`public inline void `[`operator<<`](#d6/dba/classalps_1_1_no_binning_1af266005ded8e4d2c3590f5245f64a6d5)`(const value_type & x)` | 
`public inline result_type `[`mean`](#d6/dba/classalps_1_1_no_binning_1a7ae9945fc8c46dcb9876dc1b604ad63d)`() const` | 
`public inline result_type `[`variance`](#d6/dba/classalps_1_1_no_binning_1aa450ec1b944f4fd1a37ac3dd4be3b7d0)`() const` | 
`public inline result_type `[`error`](#d6/dba/classalps_1_1_no_binning_1ad2ceb3fa321d6e0365e09624e3f4dc1e)`(uint32_t) const` | 
`public convergence_type `[`converged_errors`](#d6/dba/classalps_1_1_no_binning_1a9cf24d8a3e70d13ca23fdbd18dd88c71)`() const` | 
`public inline uint32_t `[`count`](#d6/dba/classalps_1_1_no_binning_1a147237bea3d95cce57aef88ff9da6a15)`() const` | 
`public inline void `[`set_bin_size`](#d6/dba/classalps_1_1_no_binning_1a35817be23826fe597450217f1edb713d)`(count_type)` | 
`public inline void `[`set_bin_number`](#d6/dba/classalps_1_1_no_binning_1a3784e2a1ce80ab0e53f317ae810c4a08)`(count_type)` | 
`public inline void `[`output_scalar`](#d6/dba/classalps_1_1_no_binning_1afcd9bb07f20d710e7c4561aab4d8ef16)`(std::ostream & out) const` | 
`public template<>`  <br/>`inline void `[`output_vector`](#d6/dba/classalps_1_1_no_binning_1abf6085f5ff89da7f0f0257828ca0c41a)`(std::ostream & out,const L & l) const` | 
`public inline void `[`save`](#d6/dba/classalps_1_1_no_binning_1ada2d02d19e1637e87eaf2cbf4bec9b99)`(ODump & dump) const` | 
`public inline void `[`load`](#d6/dba/classalps_1_1_no_binning_1a35ad9b5e383ec8f4afc5da7dd3464697)`(IDump & dump)` | 
`public inline void `[`save`](#d6/dba/classalps_1_1_no_binning_1ad93672bb1fd728ed6a32c7add096c266)`(hdf5::archive &) const` | 
`public inline void `[`load`](#d6/dba/classalps_1_1_no_binning_1ade583273cc102cc8103baec431be5dfc)`(hdf5::archive &)` | 
`typedef `[`value_type`](#d6/dba/classalps_1_1_no_binning_1a65a16fd5bbbb8c81fab40c0f82e174f4) | 
`typedef `[`size_type`](#d6/dba/classalps_1_1_no_binning_1aa8ab3681d4da79951269eb0037ddd628) | 
`typedef `[`count_type`](#d6/dba/classalps_1_1_no_binning_1ac5b74d2fd919f59bcde21b89632adf32) | 
`typedef `[`result_type`](#d6/dba/classalps_1_1_no_binning_1a8a82f1527d85408105b5c9043f7b91ac) | 
`typedef `[`convergence_type`](#d6/dba/classalps_1_1_no_binning_1a7b251725914d021439d27cf90e02438d) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d6/dba/classalps_1_1_no_binning_1a8ce6e89801af5b34e88eaf098a3697b6)`(bool,has_tau)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d6/dba/classalps_1_1_no_binning_1ae33c0558b2e8482821455fb7b39b8946)`(int,magic_id)` 

#### `public inline  `[`NoBinning`](#d6/dba/classalps_1_1_no_binning_1a13bef9b2f1a4426e9c0a1ab0e720774c)`(uint32_t,uint32_t)` 

#### `public inline void `[`reset`](#d6/dba/classalps_1_1_no_binning_1a09d6f718dc98cc54909e488b1f5fd323)`(bool)` 

#### `public inline void `[`operator<<`](#d6/dba/classalps_1_1_no_binning_1af266005ded8e4d2c3590f5245f64a6d5)`(const value_type & x)` 

#### `public inline result_type `[`mean`](#d6/dba/classalps_1_1_no_binning_1a7ae9945fc8c46dcb9876dc1b604ad63d)`() const` 

#### `public inline result_type `[`variance`](#d6/dba/classalps_1_1_no_binning_1aa450ec1b944f4fd1a37ac3dd4be3b7d0)`() const` 

#### `public inline result_type `[`error`](#d6/dba/classalps_1_1_no_binning_1ad2ceb3fa321d6e0365e09624e3f4dc1e)`(uint32_t) const` 

#### `public convergence_type `[`converged_errors`](#d6/dba/classalps_1_1_no_binning_1a9cf24d8a3e70d13ca23fdbd18dd88c71)`() const` 

#### `public inline uint32_t `[`count`](#d6/dba/classalps_1_1_no_binning_1a147237bea3d95cce57aef88ff9da6a15)`() const` 

#### `public inline void `[`set_bin_size`](#d6/dba/classalps_1_1_no_binning_1a35817be23826fe597450217f1edb713d)`(count_type)` 

#### `public inline void `[`set_bin_number`](#d6/dba/classalps_1_1_no_binning_1a3784e2a1ce80ab0e53f317ae810c4a08)`(count_type)` 

#### `public inline void `[`output_scalar`](#d6/dba/classalps_1_1_no_binning_1afcd9bb07f20d710e7c4561aab4d8ef16)`(std::ostream & out) const` 

#### `public template<>`  <br/>`inline void `[`output_vector`](#d6/dba/classalps_1_1_no_binning_1abf6085f5ff89da7f0f0257828ca0c41a)`(std::ostream & out,const L & l) const` 

#### `public inline void `[`save`](#d6/dba/classalps_1_1_no_binning_1ada2d02d19e1637e87eaf2cbf4bec9b99)`(ODump & dump) const` 

#### `public inline void `[`load`](#d6/dba/classalps_1_1_no_binning_1a35ad9b5e383ec8f4afc5da7dd3464697)`(IDump & dump)` 

#### `public inline void `[`save`](#d6/dba/classalps_1_1_no_binning_1ad93672bb1fd728ed6a32c7add096c266)`(hdf5::archive &) const` 

#### `public inline void `[`load`](#d6/dba/classalps_1_1_no_binning_1ade583273cc102cc8103baec431be5dfc)`(hdf5::archive &)` 

#### `typedef `[`value_type`](#d6/dba/classalps_1_1_no_binning_1a65a16fd5bbbb8c81fab40c0f82e174f4) 

#### `typedef `[`size_type`](#d6/dba/classalps_1_1_no_binning_1aa8ab3681d4da79951269eb0037ddd628) 

#### `typedef `[`count_type`](#d6/dba/classalps_1_1_no_binning_1ac5b74d2fd919f59bcde21b89632adf32) 

#### `typedef `[`result_type`](#d6/dba/classalps_1_1_no_binning_1a8a82f1527d85408105b5c9043f7b91ac) 

#### `typedef `[`convergence_type`](#d6/dba/classalps_1_1_no_binning_1a7b251725914d021439d27cf90e02438d) 

# class `alps::NoMeasurementsError` 

```
class alps::NoMeasurementsError
  : public std::runtime_error
```  

an error class if no measurement was performed

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`NoMeasurementsError`](#dc/dfe/classalps_1_1_no_measurements_error_1af34c491a2f38d84e993a2ab4f5b54c48)`()` | 

## Members

#### `public inline  `[`NoMeasurementsError`](#dc/dfe/classalps_1_1_no_measurements_error_1af34c491a2f38d84e993a2ab4f5b54c48)`()` 

# class `alps::Observable` 

the base class for all observables

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`Observable`](#df/d26/classalps_1_1_observable_1a3561f5598f54f18f14511fe31a0509ab)`(const std::string & n)` | standard constructors: just assign the name
`public  `[`Observable`](#df/d26/classalps_1_1_observable_1ac419acfe7e31d4b1490310252fa78733)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & o)` | 
`public virtual  `[`~Observable`](#df/d26/classalps_1_1_observable_1a9d62e724e4bc8eca2e456233416a0528)`()` | dtor
`public virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#df/d26/classalps_1_1_observable_1aa74996ccabf6c7755a47c23fb9ade1a3)`() const` | clones the observable
`public const std::string & `[`name`](#df/d26/classalps_1_1_observable_1a6a032aea105aeaa9711ad6adc05f925d)`() const` | returns the name
`public virtual void `[`rename`](#df/d26/classalps_1_1_observable_1a93c386f28983282b12869158d5bf839e)`(const std::string &)` | rename the observable
`public virtual ALPS_DUMMY_VOID `[`reset`](#df/d26/classalps_1_1_observable_1a6f1f1884d64615b573dc608342abc9a6)`(bool equilibrated)` | reset the observable
`public virtual ALPS_DUMMY_VOID `[`output`](#df/d26/classalps_1_1_observable_1afd67c1d98e6662b0f895e662bd6a1baa)`(std::ostream &) const` | output the result
`public virtual void `[`write_xml`](#df/d26/classalps_1_1_observable_1ae8e86fcea8de6d0bb8a84f71583d592c)`(oxstream & oxs,const boost::filesystem::path & fn_hdf5) const` | output the result
`public virtual uint32_t `[`version_id`](#df/d26/classalps_1_1_observable_1ad71e7e40933257bb3a6d74e2035cdb78)`() const` | return a version ID uniquely identifying the class
`public virtual void `[`save`](#df/d26/classalps_1_1_observable_1ae1dcde5b13a43666deae22e6e2e94675)`(ODump & dump) const` | 
`public virtual void `[`load`](#df/d26/classalps_1_1_observable_1ac22850d403beddee13d5c509964b459b)`(IDump & dump)` | 
`public virtual void `[`save`](#df/d26/classalps_1_1_observable_1a02dd4cdabf278c28c5744ea8a69397cc)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#df/d26/classalps_1_1_observable_1a4ddc6a8af88e7544d132882f152b9914)`(hdf5::archive &)` | 
`public virtual bool `[`is_signed`](#df/d26/classalps_1_1_observable_1a80bd2fd5d447542befb55cdab1f91723)`() const` | is the observable signed?
`public virtual void `[`set_sign_name`](#df/d26/classalps_1_1_observable_1adb7d10bec9fa4fa8475afa414e6203f4)`(const std::string & signname)` | set the name of the observable containing the sign for this observable
`public virtual void `[`set_sign`](#df/d26/classalps_1_1_observable_1a37a0fb456b0d23767d182fe01611333d)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & sign)` | set the observable containing the sign
`public virtual void `[`clear_sign`](#df/d26/classalps_1_1_observable_1aa2f5d0524ebf3fad62153c65a90746d5)`()` | clear any previosuly set sign observable
`public virtual const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`sign`](#df/d26/classalps_1_1_observable_1ab979f19d40b7e28f53c6305139b148c1)`() const` | get a reference to the sign observable
`public virtual const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`signed_observable`](#df/d26/classalps_1_1_observable_1a8c991fbbf43785ce54d6dc652c7c7277)`() const` | 
`public virtual const std::string `[`sign_name`](#df/d26/classalps_1_1_observable_1ae412e51383fd8ece6c0899d8c68841fe)`() const` | get the name of the observable containing the sign
`public virtual uint32_t `[`number_of_runs`](#df/d26/classalps_1_1_observable_1a820040b3a895363e5a4741066ea3dc19)`() const` | get the number of runs which performed measurements for this observable
`public virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`get_run`](#df/d26/classalps_1_1_observable_1a398cb54a82894259f87c206c5151029d)`(uint32_t) const` | extract an observable from a specific run only
`public virtual void `[`merge`](#df/d26/classalps_1_1_observable_1afceff88c6ea4384fa16a0c7fafa4a33c)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &)` | 
`public virtual bool `[`can_merge`](#df/d26/classalps_1_1_observable_1a2a58fd110828a90e8972d829a652fbb6)`() const` | can this observable be merged with one of the same type
`public virtual bool `[`can_merge`](#df/d26/classalps_1_1_observable_1aef219e54a1b8bcfd776d0693492b09b1)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &) const` | can this observable be merged with one of the given type
`public virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`convert_mergeable`](#df/d26/classalps_1_1_observable_1aaf22e7d5f7c87ded161ceab73ac722b0)`() const` | create a copy of the observable that can be merged
`public template<>`  <br/>`inline void `[`operator<<`](#df/d26/classalps_1_1_observable_1a2c344681f3d45db4e620d53beeaa9db7)`(const T & x)` | merge this observable with another or add measurement
`public template<>`  <br/>`inline void `[`add`](#df/d26/classalps_1_1_observable_1ad115190f0cf417c40cbc543c9f87fcab)`(const T & x)` | 
`public template<>`  <br/>`inline void `[`add`](#df/d26/classalps_1_1_observable_1a448f50a497423095530f4de5d265c271)`(const T & x,S s)` | 
`typedef `[`version_type`](#df/d26/classalps_1_1_observable_1ab9d98cd14638f94ef8ad84c91f555da5) | 

## Members

#### `public  `[`Observable`](#df/d26/classalps_1_1_observable_1a3561f5598f54f18f14511fe31a0509ab)`(const std::string & n)` 

standard constructors: just assign the name

#### `public  `[`Observable`](#df/d26/classalps_1_1_observable_1ac419acfe7e31d4b1490310252fa78733)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & o)` 

#### `public virtual  `[`~Observable`](#df/d26/classalps_1_1_observable_1a9d62e724e4bc8eca2e456233416a0528)`()` 

dtor

#### `public virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#df/d26/classalps_1_1_observable_1aa74996ccabf6c7755a47c23fb9ade1a3)`() const` 

clones the observable

#### `public const std::string & `[`name`](#df/d26/classalps_1_1_observable_1a6a032aea105aeaa9711ad6adc05f925d)`() const` 

returns the name

#### `public virtual void `[`rename`](#df/d26/classalps_1_1_observable_1a93c386f28983282b12869158d5bf839e)`(const std::string &)` 

rename the observable

#### `public virtual ALPS_DUMMY_VOID `[`reset`](#df/d26/classalps_1_1_observable_1a6f1f1884d64615b573dc608342abc9a6)`(bool equilibrated)` 

reset the observable

#### `public virtual ALPS_DUMMY_VOID `[`output`](#df/d26/classalps_1_1_observable_1afd67c1d98e6662b0f895e662bd6a1baa)`(std::ostream &) const` 

output the result

#### `public virtual void `[`write_xml`](#df/d26/classalps_1_1_observable_1ae8e86fcea8de6d0bb8a84f71583d592c)`(oxstream & oxs,const boost::filesystem::path & fn_hdf5) const` 

output the result

#### `public virtual uint32_t `[`version_id`](#df/d26/classalps_1_1_observable_1ad71e7e40933257bb3a6d74e2035cdb78)`() const` 

return a version ID uniquely identifying the class

#### `public virtual void `[`save`](#df/d26/classalps_1_1_observable_1ae1dcde5b13a43666deae22e6e2e94675)`(ODump & dump) const` 

#### `public virtual void `[`load`](#df/d26/classalps_1_1_observable_1ac22850d403beddee13d5c509964b459b)`(IDump & dump)` 

#### `public virtual void `[`save`](#df/d26/classalps_1_1_observable_1a02dd4cdabf278c28c5744ea8a69397cc)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#df/d26/classalps_1_1_observable_1a4ddc6a8af88e7544d132882f152b9914)`(hdf5::archive &)` 

#### `public virtual bool `[`is_signed`](#df/d26/classalps_1_1_observable_1a80bd2fd5d447542befb55cdab1f91723)`() const` 

is the observable signed?

#### `public virtual void `[`set_sign_name`](#df/d26/classalps_1_1_observable_1adb7d10bec9fa4fa8475afa414e6203f4)`(const std::string & signname)` 

set the name of the observable containing the sign for this observable

#### `public virtual void `[`set_sign`](#df/d26/classalps_1_1_observable_1a37a0fb456b0d23767d182fe01611333d)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & sign)` 

set the observable containing the sign

#### `public virtual void `[`clear_sign`](#df/d26/classalps_1_1_observable_1aa2f5d0524ebf3fad62153c65a90746d5)`()` 

clear any previosuly set sign observable

#### `public virtual const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`sign`](#df/d26/classalps_1_1_observable_1ab979f19d40b7e28f53c6305139b148c1)`() const` 

get a reference to the sign observable

#### `public virtual const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`signed_observable`](#df/d26/classalps_1_1_observable_1a8c991fbbf43785ce54d6dc652c7c7277)`() const` 

#### `public virtual const std::string `[`sign_name`](#df/d26/classalps_1_1_observable_1ae412e51383fd8ece6c0899d8c68841fe)`() const` 

get the name of the observable containing the sign

#### `public virtual uint32_t `[`number_of_runs`](#df/d26/classalps_1_1_observable_1a820040b3a895363e5a4741066ea3dc19)`() const` 

get the number of runs which performed measurements for this observable

#### `public virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`get_run`](#df/d26/classalps_1_1_observable_1a398cb54a82894259f87c206c5151029d)`(uint32_t) const` 

extract an observable from a specific run only

#### `public virtual void `[`merge`](#df/d26/classalps_1_1_observable_1afceff88c6ea4384fa16a0c7fafa4a33c)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &)` 

#### `public virtual bool `[`can_merge`](#df/d26/classalps_1_1_observable_1a2a58fd110828a90e8972d829a652fbb6)`() const` 

can this observable be merged with one of the same type

#### `public virtual bool `[`can_merge`](#df/d26/classalps_1_1_observable_1aef219e54a1b8bcfd776d0693492b09b1)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &) const` 

can this observable be merged with one of the given type

#### `public virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`convert_mergeable`](#df/d26/classalps_1_1_observable_1aaf22e7d5f7c87ded161ceab73ac722b0)`() const` 

create a copy of the observable that can be merged

#### `public template<>`  <br/>`inline void `[`operator<<`](#df/d26/classalps_1_1_observable_1a2c344681f3d45db4e620d53beeaa9db7)`(const T & x)` 

merge this observable with another or add measurement

#### `public template<>`  <br/>`inline void `[`add`](#df/d26/classalps_1_1_observable_1ad115190f0cf417c40cbc543c9f87fcab)`(const T & x)` 

#### `public template<>`  <br/>`inline void `[`add`](#df/d26/classalps_1_1_observable_1a448f50a497423095530f4de5d265c271)`(const T & x,S s)` 

#### `typedef `[`version_type`](#df/d26/classalps_1_1_observable_1ab9d98cd14638f94ef8ad84c91f555da5) 

# class `alps::ObservableFactory` 

```
class alps::ObservableFactory
  : public factory< uint32_t, Observable >
```  

[A](#d1/d2d/classalps_1_1_a) class to collect the various measurements performed in a simulation It is implemented as a map, with std::string as key type

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`ObservableFactory`](#d6/d35/classalps_1_1_observable_factory_1adaf104bf2f4e1b6f1cd59892ff503099)`()` | 
`public template<>`  <br/>`inline void `[`register_observable`](#d6/d35/classalps_1_1_observable_factory_1aa5f7242f3b45950b4b2a6d98a5dfbc59)`()` | 

## Members

#### `public  `[`ObservableFactory`](#d6/d35/classalps_1_1_observable_factory_1adaf104bf2f4e1b6f1cd59892ff503099)`()` 

#### `public template<>`  <br/>`inline void `[`register_observable`](#d6/d35/classalps_1_1_observable_factory_1aa5f7242f3b45950b4b2a6d98a5dfbc59)`()` 

# class `alps::ObservableSet` 

```
class alps::ObservableSet
  : public std::map< std::string, Observable * >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`ObservableSet`](#db/da3/classalps_1_1_observable_set_1a0e5195f9db2afcc8186668162f6ec75d)`()` | the default constructor
`public  `[`ObservableSet`](#db/da3/classalps_1_1_observable_set_1a4e89445c44d492e365f93fad0d3ba28e)`(const `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & m)` | sign problem support requires a non-trivial copy constructor
`public virtual  `[`~ObservableSet`](#db/da3/classalps_1_1_observable_set_1abe3f133824fb40144f9f5d1558277e81)`()` | a non-trivial destructor
`public `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & `[`operator=`](#db/da3/classalps_1_1_observable_set_1a88955a97cad68873232ce6b108693acb)`(const `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & m)` | sign problem support requires non-trivial assignment
`public `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & `[`operator<<`](#db/da3/classalps_1_1_observable_set_1ac19b273b50fe163eb20c6f68d73f3a58)`(const `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & obs)` | merge two observable set. If observables with identical names exist in both sets, a merger of the observables is attempted. In case of failure an exception is thrown. 
`public `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & `[`operator<<`](#db/da3/classalps_1_1_observable_set_1a7faccf8e112f8cec41333659e6528139)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs)` | merge an observable into the set. If an observables with identical names exists, a merger of the observables is attempted. In case of failure an exception is thrown. 
`public inline `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & `[`operator<<`](#db/da3/classalps_1_1_observable_set_1a078617917f3a46ba589400ffac7cd32d)`(const boost::shared_ptr< `[`Observable`](#df/d26/classalps_1_1_observable)` > & obs)` | 
`public void `[`addObservable`](#db/da3/classalps_1_1_observable_set_1af7c35ed676e999c7696d4401b76f9d07)`(`[`Observable`](#df/d26/classalps_1_1_observable)` * obs)` | add an observable to the set. The [ObservableSet](#db/da3/classalps_1_1_observable_set) will delete the object at the end. If an observable with the same name exists, it is replaced. This is different behavior than operator<<.
`public void `[`addObservable`](#db/da3/classalps_1_1_observable_set_1a9f7281e1e7e2998694186ec123f4cacf)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs)` | 
`public void `[`removeObservable`](#db/da3/classalps_1_1_observable_set_1a8418841df3f591b39b62791b76bf6cbc)`(const std::string & name)` | remove an observable with a given name
`public `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`operator[]`](#db/da3/classalps_1_1_observable_set_1ac518f080b975a49632c6ae6cfd9e0091)`(const std::string & name)` | get an observable with the given name 
`public const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`operator[]`](#db/da3/classalps_1_1_observable_set_1a32c10ab0a47a603af3885592bbd9a52c)`(const std::string & name) const` | get an observable with the given name 
`public bool `[`has`](#db/da3/classalps_1_1_observable_set_1a2dda882f39d9ff49c8b165b22c0be9ce)`(const std::string & name) const` | check if an observable with the given name exists
`public void `[`reset`](#db/da3/classalps_1_1_observable_set_1a375ddd2096bee44c0e55aba69eb85026)`(bool)` | reset all observables 
`public template<>`  <br/>`inline void `[`do_for_all`](#db/da3/classalps_1_1_observable_set_1a676af7b78b279864f4a8269b8b42f11f)`(F f) const` | apply a unary function to all observables
`public template<>`  <br/>`inline void `[`do_for_all`](#db/da3/classalps_1_1_observable_set_1a63cf0b51214afbd24268b9063d8e2246)`(F f)` | apply a unary function to all observables
`public template<>`  <br/>`inline T & `[`get`](#db/da3/classalps_1_1_observable_set_1a47d935b07b8b4bfb122d48c706180676)`(const std::string & name)` | get an observable with the given name and type 
`public template<>`  <br/>`inline const T & `[`get`](#db/da3/classalps_1_1_observable_set_1a12a1695d9b0a72358d3e0c677a2d6d09)`(const std::string & name) const` | get an observable with the given name and type 
`public uint32_t `[`number_of_runs`](#db/da3/classalps_1_1_observable_set_1a2f7e02adf60ca513a02baf43b5065ee0)`() const` | the number of runs from which the observables were collected. Care must be taken that if some observables did not occur in all sets the numbering is not consistent and problems can result.
`public `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` `[`get_run`](#db/da3/classalps_1_1_observable_set_1a31a82038afa6a78e9946a44e63b4722b)`(uint32_t) const` | the number of runs from which the observables were collected. Care must be taken that if some observables did not occur in all sets the numbering is not consistent and problems can result.
`public virtual void `[`save`](#db/da3/classalps_1_1_observable_set_1a8c87c7e0b184da38ff777396e08c3053)`(ODump & dump) const` | 
`public virtual void `[`load`](#db/da3/classalps_1_1_observable_set_1a7712c0095bd3a082ff485651e6dc9716)`(IDump & dump)` | 
`public virtual void `[`save`](#db/da3/classalps_1_1_observable_set_1a19f9e4de3872a6f6276d8ef00aa45e7a)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#db/da3/classalps_1_1_observable_set_1aa4ff5f7a7e8fd2fa1cc9e1a3d0e07487)`(hdf5::archive &)` | 
`public template<>`  <br/>`inline void `[`save`](#db/da3/classalps_1_1_observable_set_1ae0e3f114fa289674ec6aafbd4657f787)`(Archive & ar,const unsigned int) const` | support for Boost serialization
`public template<>`  <br/>`inline void `[`load`](#db/da3/classalps_1_1_observable_set_1a1d134e71874e30bc296c093bd0efb6fd)`(Archive & ar,const unsigned int)` | support for Boost serialization
`public void `[`update_signs`](#db/da3/classalps_1_1_observable_set_1a5cdd1bf1405e51a0acee83f36364f8c9)`()` | 
`public void `[`set_sign`](#db/da3/classalps_1_1_observable_set_1a9c29d9335e4414a0d63bcca8ec4d243b)`(const std::string &)` | 
`public inline void `[`compact`](#db/da3/classalps_1_1_observable_set_1a67060108b6b04ddb120b7b8a76dc19e4)`()` | compact the observables to save space, discarding e.g. time series information
`public void `[`write_xml`](#db/da3/classalps_1_1_observable_set_1a34466cd8edcdd00f3405224ea1b7397b)`(oxstream & oxs,const boost::filesystem::path &) const` | 
`public void `[`write_xml_with_id`](#db/da3/classalps_1_1_observable_set_1a8737908c193bf7c4273c4a96ec8a70e4)`(oxstream & oxs,int id,const boost::filesystem::path &) const` | 
`public void `[`read_xml`](#db/da3/classalps_1_1_observable_set_1ac029014f648590077bb46f18664e00bb)`(std::istream & infile,const XMLTag & tag)` | 
`public void `[`write_hdf5`](#db/da3/classalps_1_1_observable_set_1a2c2fe1ff5483a0c37eb958f748ba7419)`(boost::filesystem::path const &,std::size_t realization,std::size_t clone) const` | 
`public void `[`read_hdf5`](#db/da3/classalps_1_1_observable_set_1afec5e44c329f4af5b0f41a79f522e678)`(boost::filesystem::path const &,std::size_t realization,std::size_t clone)` | 
`public void `[`clear`](#db/da3/classalps_1_1_observable_set_1a8989c876d0aa6035b77b3e58f6a76758)`()` | 

## Members

#### `public inline  `[`ObservableSet`](#db/da3/classalps_1_1_observable_set_1a0e5195f9db2afcc8186668162f6ec75d)`()` 

the default constructor

#### `public  `[`ObservableSet`](#db/da3/classalps_1_1_observable_set_1a4e89445c44d492e365f93fad0d3ba28e)`(const `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & m)` 

sign problem support requires a non-trivial copy constructor

#### `public virtual  `[`~ObservableSet`](#db/da3/classalps_1_1_observable_set_1abe3f133824fb40144f9f5d1558277e81)`()` 

a non-trivial destructor

#### `public `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & `[`operator=`](#db/da3/classalps_1_1_observable_set_1a88955a97cad68873232ce6b108693acb)`(const `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & m)` 

sign problem support requires non-trivial assignment

#### `public `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & `[`operator<<`](#db/da3/classalps_1_1_observable_set_1ac19b273b50fe163eb20c6f68d73f3a58)`(const `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & obs)` 

merge two observable set. If observables with identical names exist in both sets, a merger of the observables is attempted. In case of failure an exception is thrown. 
#### Exceptions
* `std::bad_cast` if merging fails

#### `public `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & `[`operator<<`](#db/da3/classalps_1_1_observable_set_1a7faccf8e112f8cec41333659e6528139)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs)` 

merge an observable into the set. If an observables with identical names exists, a merger of the observables is attempted. In case of failure an exception is thrown. 
#### Exceptions
* `std::bad_cast` if merging fails

#### `public inline `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & `[`operator<<`](#db/da3/classalps_1_1_observable_set_1a078617917f3a46ba589400ffac7cd32d)`(const boost::shared_ptr< `[`Observable`](#df/d26/classalps_1_1_observable)` > & obs)` 

#### `public void `[`addObservable`](#db/da3/classalps_1_1_observable_set_1af7c35ed676e999c7696d4401b76f9d07)`(`[`Observable`](#df/d26/classalps_1_1_observable)` * obs)` 

add an observable to the set. The [ObservableSet](#db/da3/classalps_1_1_observable_set) will delete the object at the end. If an observable with the same name exists, it is replaced. This is different behavior than operator<<.

#### `public void `[`addObservable`](#db/da3/classalps_1_1_observable_set_1a9f7281e1e7e2998694186ec123f4cacf)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs)` 

#### `public void `[`removeObservable`](#db/da3/classalps_1_1_observable_set_1a8418841df3f591b39b62791b76bf6cbc)`(const std::string & name)` 

remove an observable with a given name

#### `public `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`operator[]`](#db/da3/classalps_1_1_observable_set_1ac518f080b975a49632c6ae6cfd9e0091)`(const std::string & name)` 

get an observable with the given name 
#### Exceptions
* `throws` a std::runtime_error if no observable exists with the given name

#### `public const `[`Observable`](#df/d26/classalps_1_1_observable)` & `[`operator[]`](#db/da3/classalps_1_1_observable_set_1a32c10ab0a47a603af3885592bbd9a52c)`(const std::string & name) const` 

get an observable with the given name 
#### Exceptions
* `throws` a std::runtime_error if no observable exists with the given name

#### `public bool `[`has`](#db/da3/classalps_1_1_observable_set_1a2dda882f39d9ff49c8b165b22c0be9ce)`(const std::string & name) const` 

check if an observable with the given name exists

#### `public void `[`reset`](#db/da3/classalps_1_1_observable_set_1a375ddd2096bee44c0e55aba69eb85026)`(bool)` 

reset all observables 
#### Parameters
* `flag` a value of true means that reset is called after thermalization and information about thermalization should be kept.

#### `public template<>`  <br/>`inline void `[`do_for_all`](#db/da3/classalps_1_1_observable_set_1a676af7b78b279864f4a8269b8b42f11f)`(F f) const` 

apply a unary function to all observables

#### `public template<>`  <br/>`inline void `[`do_for_all`](#db/da3/classalps_1_1_observable_set_1a63cf0b51214afbd24268b9063d8e2246)`(F f)` 

apply a unary function to all observables

#### `public template<>`  <br/>`inline T & `[`get`](#db/da3/classalps_1_1_observable_set_1a47d935b07b8b4bfb122d48c706180676)`(const std::string & name)` 

get an observable with the given name and type 
#### Exceptions
* `throws` a std::runtime_error if no observable exists with the given name

#### `public template<>`  <br/>`inline const T & `[`get`](#db/da3/classalps_1_1_observable_set_1a12a1695d9b0a72358d3e0c677a2d6d09)`(const std::string & name) const` 

get an observable with the given name and type 
#### Exceptions
* `throws` a std::runtime_error if no observable exists with the given name

#### `public uint32_t `[`number_of_runs`](#db/da3/classalps_1_1_observable_set_1a2f7e02adf60ca513a02baf43b5065ee0)`() const` 

the number of runs from which the observables were collected. Care must be taken that if some observables did not occur in all sets the numbering is not consistent and problems can result.

#### `public `[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` `[`get_run`](#db/da3/classalps_1_1_observable_set_1a31a82038afa6a78e9946a44e63b4722b)`(uint32_t) const` 

the number of runs from which the observables were collected. Care must be taken that if some observables did not occur in all sets the numbering is not consistent and problems can result.

#### `public virtual void `[`save`](#db/da3/classalps_1_1_observable_set_1a8c87c7e0b184da38ff777396e08c3053)`(ODump & dump) const` 

#### `public virtual void `[`load`](#db/da3/classalps_1_1_observable_set_1a7712c0095bd3a082ff485651e6dc9716)`(IDump & dump)` 

#### `public virtual void `[`save`](#db/da3/classalps_1_1_observable_set_1a19f9e4de3872a6f6276d8ef00aa45e7a)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#db/da3/classalps_1_1_observable_set_1aa4ff5f7a7e8fd2fa1cc9e1a3d0e07487)`(hdf5::archive &)` 

#### `public template<>`  <br/>`inline void `[`save`](#db/da3/classalps_1_1_observable_set_1ae0e3f114fa289674ec6aafbd4657f787)`(Archive & ar,const unsigned int) const` 

support for Boost serialization

#### `public template<>`  <br/>`inline void `[`load`](#db/da3/classalps_1_1_observable_set_1a1d134e71874e30bc296c093bd0efb6fd)`(Archive & ar,const unsigned int)` 

support for Boost serialization

#### `public void `[`update_signs`](#db/da3/classalps_1_1_observable_set_1a5cdd1bf1405e51a0acee83f36364f8c9)`()` 

#### `public void `[`set_sign`](#db/da3/classalps_1_1_observable_set_1a9c29d9335e4414a0d63bcca8ec4d243b)`(const std::string &)` 

#### `public inline void `[`compact`](#db/da3/classalps_1_1_observable_set_1a67060108b6b04ddb120b7b8a76dc19e4)`()` 

compact the observables to save space, discarding e.g. time series information

#### `public void `[`write_xml`](#db/da3/classalps_1_1_observable_set_1a34466cd8edcdd00f3405224ea1b7397b)`(oxstream & oxs,const boost::filesystem::path &) const` 

#### `public void `[`write_xml_with_id`](#db/da3/classalps_1_1_observable_set_1a8737908c193bf7c4273c4a96ec8a70e4)`(oxstream & oxs,int id,const boost::filesystem::path &) const` 

#### `public void `[`read_xml`](#db/da3/classalps_1_1_observable_set_1ac029014f648590077bb46f18664e00bb)`(std::istream & infile,const XMLTag & tag)` 

#### `public void `[`write_hdf5`](#db/da3/classalps_1_1_observable_set_1a2c2fe1ff5483a0c37eb958f748ba7419)`(boost::filesystem::path const &,std::size_t realization,std::size_t clone) const` 

#### `public void `[`read_hdf5`](#db/da3/classalps_1_1_observable_set_1afec5e44c329f4af5b0f41a79f522e678)`(boost::filesystem::path const &,std::size_t realization,std::size_t clone)` 

#### `public void `[`clear`](#db/da3/classalps_1_1_observable_set_1a8989c876d0aa6035b77b3e58f6a76758)`()` 

# class `alps::ObservableSetXMLHandler` 

```
class alps::ObservableSetXMLHandler
  : public CompositeXMLHandler
```  

XML parser for the [ObservableSet](#db/da3/classalps_1_1_observable_set) class.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`ObservableSetXMLHandler`](#de/d7b/classalps_1_1_observable_set_x_m_l_handler_1ac837bb5b1d1159c0873463f4df3a6d62)`(`[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & obs)` | 
`protected void `[`end_child`](#de/d7b/classalps_1_1_observable_set_x_m_l_handler_1a2b3347825817f010bfa1756cb5940c17)`(std::string const & name,xml::tag_type type)` | 

## Members

#### `public  `[`ObservableSetXMLHandler`](#de/d7b/classalps_1_1_observable_set_x_m_l_handler_1ac837bb5b1d1159c0873463f4df3a6d62)`(`[`ObservableSet`](#db/da3/classalps_1_1_observable_set)` & obs)` 

#### `protected void `[`end_child`](#de/d7b/classalps_1_1_observable_set_x_m_l_handler_1a2b3347825817f010bfa1756cb5940c17)`(std::string const & name,xml::tag_type type)` 

# class `alps::ObsValueXMLHandler` 

```
class alps::ObsValueXMLHandler
  : public XMLHandlerBase
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`ObsValueXMLHandler`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1a081a50323822de34aa480ab7ad925e84)`(const std::string & basename,double & val,const std::string & attr)` | 
`public inline virtual  `[`~ObsValueXMLHandler`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1a5117719eb97b3c834617cf5a482be48c)`()` | 
`public virtual void `[`start_element`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1acfe14319f86e489728441dc8f41a5618)`(const std::string & name,const XMLAttributes & attributes,xml::tag_type type)` | 
`public virtual void `[`end_element`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1a045f86133551cf9072736ed0f0faeea0)`(const std::string & name,xml::tag_type type)` | 
`public virtual void `[`text`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1ab4cbb25dfe8175d9bd9e77ece8dede24)`(const std::string & text)` | 

## Members

#### `public  `[`ObsValueXMLHandler`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1a081a50323822de34aa480ab7ad925e84)`(const std::string & basename,double & val,const std::string & attr)` 

#### `public inline virtual  `[`~ObsValueXMLHandler`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1a5117719eb97b3c834617cf5a482be48c)`()` 

#### `public virtual void `[`start_element`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1acfe14319f86e489728441dc8f41a5618)`(const std::string & name,const XMLAttributes & attributes,xml::tag_type type)` 

#### `public virtual void `[`end_element`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1a045f86133551cf9072736ed0f0faeea0)`(const std::string & name,xml::tag_type type)` 

#### `public virtual void `[`text`](#db/d55/classalps_1_1_obs_value_x_m_l_handler_1ab4cbb25dfe8175d9bd9e77ece8dede24)`(const std::string & text)` 

# class `alps::RealHistogramEntryXMLHandler` 

```
class alps::RealHistogramEntryXMLHandler
  : public CompositeXMLHandler
```  

XML parser for the entries for RealHistogramObservable class.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`RealHistogramEntryXMLHandler`](#d9/db6/classalps_1_1_real_histogram_entry_x_m_l_handler_1aaa1c361ff46664aafab6d7e558f77c7e)`(uint64_t & count,uint64_t & value)` | 
`public inline virtual  `[`~RealHistogramEntryXMLHandler`](#d9/db6/classalps_1_1_real_histogram_entry_x_m_l_handler_1a1c7db7a496558dd03adedd3f8c5fb055)`()` | 

## Members

#### `public  `[`RealHistogramEntryXMLHandler`](#d9/db6/classalps_1_1_real_histogram_entry_x_m_l_handler_1aaa1c361ff46664aafab6d7e558f77c7e)`(uint64_t & count,uint64_t & value)` 

#### `public inline virtual  `[`~RealHistogramEntryXMLHandler`](#d9/db6/classalps_1_1_real_histogram_entry_x_m_l_handler_1a1c7db7a496558dd03adedd3f8c5fb055)`()` 

# class `alps::RealHistogramObservableXMLHandler` 

```
class alps::RealHistogramObservableXMLHandler
  : public CompositeXMLHandler
```  

XML parser for the RealHistogramObservable class.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`RealHistogramObservableXMLHandler`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler_1aef3ab44d91546bde2b5b68d61772e4a5)`(`[`RealHistogramObservable`](#d5/d10/classalps_1_1_histogram_observable)` & obs)` | 
`public inline virtual  `[`~RealHistogramObservableXMLHandler`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler_1ae31cc84f511c2b69782c7e4aaa330110)`()` | 
`protected void `[`start_top`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler_1a011179bb3d20a19b84adedb8e90a0433)`(const std::string &,const XMLAttributes &,xml::tag_type)` | 
`protected void `[`end_child`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler_1a917bf0f8622423e019cd314a651d5564)`(const std::string & name,xml::tag_type type)` | 

## Members

#### `public  `[`RealHistogramObservableXMLHandler`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler_1aef3ab44d91546bde2b5b68d61772e4a5)`(`[`RealHistogramObservable`](#d5/d10/classalps_1_1_histogram_observable)` & obs)` 

#### `public inline virtual  `[`~RealHistogramObservableXMLHandler`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler_1ae31cc84f511c2b69782c7e4aaa330110)`()` 

#### `protected void `[`start_top`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler_1a011179bb3d20a19b84adedb8e90a0433)`(const std::string &,const XMLAttributes &,xml::tag_type)` 

#### `protected void `[`end_child`](#d7/d36/classalps_1_1_real_histogram_observable_x_m_l_handler_1a917bf0f8622423e019cd314a651d5564)`(const std::string & name,xml::tag_type type)` 

# class `alps::RealObsevaluatorValueXMLHandler` 

```
class alps::RealObsevaluatorValueXMLHandler
  : public XMLHandlerBase
```  

XML parser for the elements for RealObsevaluator class.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`RealObsevaluatorValueXMLHandler`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1ad2db759433d59e8115dcb3091f26fed7)`(std::string const & name,double & value,std::string & method,int & conv)` | 
`public inline virtual  `[`~RealObsevaluatorValueXMLHandler`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1abeab49faaaaaaa931138cd376b2eac09)`()` | 
`public void `[`start_element`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1abf1abe5b42a1876aa55d9b87377b5a10)`(const std::string & name,const XMLAttributes & attributes,xml::tag_type type)` | 
`public void `[`end_element`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1a50902ecc12bd65738c8dd56ac9bf9e72)`(const std::string & name,xml::tag_type type)` | 
`public void `[`text`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1a3374ae4e8e8c9f7173fbb27a06446249)`(const std::string & text)` | 

## Members

#### `public  `[`RealObsevaluatorValueXMLHandler`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1ad2db759433d59e8115dcb3091f26fed7)`(std::string const & name,double & value,std::string & method,int & conv)` 

#### `public inline virtual  `[`~RealObsevaluatorValueXMLHandler`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1abeab49faaaaaaa931138cd376b2eac09)`()` 

#### `public void `[`start_element`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1abf1abe5b42a1876aa55d9b87377b5a10)`(const std::string & name,const XMLAttributes & attributes,xml::tag_type type)` 

#### `public void `[`end_element`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1a50902ecc12bd65738c8dd56ac9bf9e72)`(const std::string & name,xml::tag_type type)` 

#### `public void `[`text`](#d4/de5/classalps_1_1_real_obsevaluator_value_x_m_l_handler_1a3374ae4e8e8c9f7173fbb27a06446249)`(const std::string & text)` 

# class `alps::RealObsevaluatorXMLHandler` 

```
class alps::RealObsevaluatorXMLHandler
  : public CompositeXMLHandler
```  

XML parser for the RealObsevaluator class.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`RealObsevaluatorXMLHandler`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler_1a130eeda6263b382b5c5942540689e6b4)`(`[`RealObsevaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)` & obs,std::string & index)` | 
`public inline virtual  `[`~RealObsevaluatorXMLHandler`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler_1abb3d29dc1880d0e2c0fbd34bcfbd7dc2)`()` | 
`protected void `[`start_top`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler_1ad3fd762b615b4b5ec01505c51db48ace)`(const std::string &,const XMLAttributes &,xml::tag_type)` | 
`protected void `[`end_child`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler_1a728f02a3ea14ec8a7d77e5c8af74f42e)`(const std::string & name,xml::tag_type type)` | 

## Members

#### `public  `[`RealObsevaluatorXMLHandler`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler_1a130eeda6263b382b5c5942540689e6b4)`(`[`RealObsevaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)` & obs,std::string & index)` 

#### `public inline virtual  `[`~RealObsevaluatorXMLHandler`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler_1abb3d29dc1880d0e2c0fbd34bcfbd7dc2)`()` 

#### `protected void `[`start_top`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler_1ad3fd762b615b4b5ec01505c51db48ace)`(const std::string &,const XMLAttributes &,xml::tag_type)` 

#### `protected void `[`end_child`](#d4/d0e/classalps_1_1_real_obsevaluator_x_m_l_handler_1a728f02a3ea14ec8a7d77e5c8af74f42e)`(const std::string & name,xml::tag_type type)` 

# class `alps::RealVectorObsevaluatorXMLHandler` 

```
class alps::RealVectorObsevaluatorXMLHandler
  : public CompositeXMLHandler
```  

XML parser for the RealVectorObsevaluator class.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`RealVectorObsevaluatorXMLHandler`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler_1a13d91dbfeb941041006956baf4751ede)`(`[`RealVectorObsevaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)` & obs)` | 
`public inline virtual  `[`~RealVectorObsevaluatorXMLHandler`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler_1af965a6458875772b8da6038be2ea2f94)`()` | 
`protected void `[`start_top`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler_1aeef5821a24122b421ff780c0dbd6838d)`(const std::string &,const XMLAttributes &,xml::tag_type)` | 
`protected void `[`end_child`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler_1a2a74c6554309c0d3a8f6a79cb1e6089d)`(const std::string & name,xml::tag_type type)` | 

## Members

#### `public  `[`RealVectorObsevaluatorXMLHandler`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler_1a13d91dbfeb941041006956baf4751ede)`(`[`RealVectorObsevaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)` & obs)` 

#### `public inline virtual  `[`~RealVectorObsevaluatorXMLHandler`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler_1af965a6458875772b8da6038be2ea2f94)`()` 

#### `protected void `[`start_top`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler_1aeef5821a24122b421ff780c0dbd6838d)`(const std::string &,const XMLAttributes &,xml::tag_type)` 

#### `protected void `[`end_child`](#dc/d10/classalps_1_1_real_vector_obsevaluator_x_m_l_handler_1a2a74c6554309c0d3a8f6a79cb1e6089d)`(const std::string & name,xml::tag_type type)` 

# class `alps::RecordableObservable` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`RecordableObservable`](#d8/dca/classalps_1_1_recordable_observable_1abb66a11714f0cd25cb786b599e1e7651)`()` | just a default constructor
`public inline virtual  `[`~RecordableObservable`](#d8/dca/classalps_1_1_recordable_observable_1a5c6289f633d80680c172d4fe93fde73d)`()` | 
`public void `[`operator<<`](#d8/dca/classalps_1_1_recordable_observable_1a26f87a17550bbc2787e5abc85973d5d4)`(const value_type & x)` | add another measurement to the observable
`public inline virtual void `[`add`](#d8/dca/classalps_1_1_recordable_observable_1a4af4fba72a92575f728f60526b1c1105)`(const value_type & x)` | add another measurement to the observable
`public inline virtual void `[`add`](#d8/dca/classalps_1_1_recordable_observable_1ac0a95cbceb1dcc33b10f73b48db65cfb)`(const value_type & x,sign_type s)` | add an explcitly signed measurement to the observable
`typedef `[`value_type`](#d8/dca/classalps_1_1_recordable_observable_1acd0da58b4472cbaf1f80c3740030b05a) | 
`typedef `[`sign_type`](#d8/dca/classalps_1_1_recordable_observable_1a8ca7c291f0852724b98ca3c85984dad8) | 

## Members

#### `public inline  `[`RecordableObservable`](#d8/dca/classalps_1_1_recordable_observable_1abb66a11714f0cd25cb786b599e1e7651)`()` 

just a default constructor

#### `public inline virtual  `[`~RecordableObservable`](#d8/dca/classalps_1_1_recordable_observable_1a5c6289f633d80680c172d4fe93fde73d)`()` 

#### `public void `[`operator<<`](#d8/dca/classalps_1_1_recordable_observable_1a26f87a17550bbc2787e5abc85973d5d4)`(const value_type & x)` 

add another measurement to the observable

#### `public inline virtual void `[`add`](#d8/dca/classalps_1_1_recordable_observable_1a4af4fba72a92575f728f60526b1c1105)`(const value_type & x)` 

add another measurement to the observable

#### `public inline virtual void `[`add`](#d8/dca/classalps_1_1_recordable_observable_1ac0a95cbceb1dcc33b10f73b48db65cfb)`(const value_type & x,sign_type s)` 

add an explcitly signed measurement to the observable

#### `typedef `[`value_type`](#d8/dca/classalps_1_1_recordable_observable_1acd0da58b4472cbaf1f80c3740030b05a) 

#### `typedef `[`sign_type`](#d8/dca/classalps_1_1_recordable_observable_1a8ca7c291f0852724b98ca3c85984dad8) 

# class `alps::SignedObservable` 

```
class alps::SignedObservable
  : public alps::AbstractSignedObservable< OBS, double >
  : public alps::RecordableObservable< OBS::value_type, double >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a25c1f07d4ddab9b73d2f570d97cdfd31)`(const OBS & obs,const std::string & s)` | 
`public inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1aab05fd6e41254d3e212edc90bd530edc)`(const std::string & name,const std::string & s,const label_type & l)` | 
`public inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a0e850f8e65309a9aed1a5ff3df5b8e30)`(const std::string & name,const char * s,const label_type & l)` | 
`public template<>`  <br/>`inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a00cb8375084633e3361e20f91d5bb7e6)`(const std::string & name,const ARG & arg,const label_type & l)` | 
`public template<>`  <br/>`inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a37d8e04ce6b8d930de13e9e606d08554)`(const std::string & name,std::string & s,const ARG & arg,const label_type & l)` | 
`public inline  `[`~SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a709b06b5af15ff4ab965c121bc91f13e)`()` | 
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#dc/d91/classalps_1_1_signed_observable_1aa02e1338528d97e2aad954595ace259f)`() const` | clones the observable
`public inline void `[`operator<<`](#dc/d91/classalps_1_1_signed_observable_1a93877aedb21b6e3a6a2faf95e79a2ea6)`(const value_type & x)` | 
`public inline void `[`add`](#dc/d91/classalps_1_1_signed_observable_1a2f917592d0e4652aef2e19e61b45cfbe)`(const value_type & x)` | 
`public inline void `[`add`](#dc/d91/classalps_1_1_signed_observable_1a5aaa14278e1e9e4a7c2795a45719fb63)`(const value_type & x,sign_type s)` | 
`public void `[`write_hdf5`](#dc/d91/classalps_1_1_signed_observable_1aa14904cdb8908574e2c95c4557e86b32)`(const boost::filesystem::path & fn_hdf,std::size_t realization,std::size_t clone) const` | 
`public void `[`read_hdf5`](#dc/d91/classalps_1_1_signed_observable_1a828b8202472884916890810b3a5595e9)`(const boost::filesystem::path & fn_hdf,std::size_t realization,std::size_t clone)` | 
`typedef `[`observable_type`](#dc/d91/classalps_1_1_signed_observable_1a4590cc5be6744dc88ce1636250cef062) | 
`typedef `[`sign_type`](#dc/d91/classalps_1_1_signed_observable_1ac183f8d2fddc665e3b9ff3344ddafeb7) | 
`typedef `[`base_type`](#dc/d91/classalps_1_1_signed_observable_1a6101190ff9919dddca6620d22dff1150) | 
`typedef `[`value_type`](#dc/d91/classalps_1_1_signed_observable_1a937b36689990a3ee5b32f8c28c51dfc3) | 
`typedef `[`result_type`](#dc/d91/classalps_1_1_signed_observable_1a64d1e6eb9ff3c132bd9c010d6f4be93c) | 
`typedef `[`count_type`](#dc/d91/classalps_1_1_signed_observable_1af6a8813c721450fedb0f11fb70f0de0e) | 
`typedef `[`time_type`](#dc/d91/classalps_1_1_signed_observable_1a3ba0d36748413cdfdc754977b78c841a) | 
`typedef `[`label_type`](#dc/d91/classalps_1_1_signed_observable_1a08ba43f0ec5f78018af7383a0bef912a) | 

## Members

#### `public inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a25c1f07d4ddab9b73d2f570d97cdfd31)`(const OBS & obs,const std::string & s)` 

#### `public inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1aab05fd6e41254d3e212edc90bd530edc)`(const std::string & name,const std::string & s,const label_type & l)` 

#### `public inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a0e850f8e65309a9aed1a5ff3df5b8e30)`(const std::string & name,const char * s,const label_type & l)` 

#### `public template<>`  <br/>`inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a00cb8375084633e3361e20f91d5bb7e6)`(const std::string & name,const ARG & arg,const label_type & l)` 

#### `public template<>`  <br/>`inline  `[`SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a37d8e04ce6b8d930de13e9e606d08554)`(const std::string & name,std::string & s,const ARG & arg,const label_type & l)` 

#### `public inline  `[`~SignedObservable`](#dc/d91/classalps_1_1_signed_observable_1a709b06b5af15ff4ab965c121bc91f13e)`()` 

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#dc/d91/classalps_1_1_signed_observable_1aa02e1338528d97e2aad954595ace259f)`() const` 

clones the observable

#### `public inline void `[`operator<<`](#dc/d91/classalps_1_1_signed_observable_1a93877aedb21b6e3a6a2faf95e79a2ea6)`(const value_type & x)` 

#### `public inline void `[`add`](#dc/d91/classalps_1_1_signed_observable_1a2f917592d0e4652aef2e19e61b45cfbe)`(const value_type & x)` 

#### `public inline void `[`add`](#dc/d91/classalps_1_1_signed_observable_1a5aaa14278e1e9e4a7c2795a45719fb63)`(const value_type & x,sign_type s)` 

#### `public void `[`write_hdf5`](#dc/d91/classalps_1_1_signed_observable_1aa14904cdb8908574e2c95c4557e86b32)`(const boost::filesystem::path & fn_hdf,std::size_t realization,std::size_t clone) const` 

#### `public void `[`read_hdf5`](#dc/d91/classalps_1_1_signed_observable_1a828b8202472884916890810b3a5595e9)`(const boost::filesystem::path & fn_hdf,std::size_t realization,std::size_t clone)` 

#### `typedef `[`observable_type`](#dc/d91/classalps_1_1_signed_observable_1a4590cc5be6744dc88ce1636250cef062) 

#### `typedef `[`sign_type`](#dc/d91/classalps_1_1_signed_observable_1ac183f8d2fddc665e3b9ff3344ddafeb7) 

#### `typedef `[`base_type`](#dc/d91/classalps_1_1_signed_observable_1a6101190ff9919dddca6620d22dff1150) 

#### `typedef `[`value_type`](#dc/d91/classalps_1_1_signed_observable_1a937b36689990a3ee5b32f8c28c51dfc3) 

#### `typedef `[`result_type`](#dc/d91/classalps_1_1_signed_observable_1a64d1e6eb9ff3c132bd9c010d6f4be93c) 

#### `typedef `[`count_type`](#dc/d91/classalps_1_1_signed_observable_1af6a8813c721450fedb0f11fb70f0de0e) 

#### `typedef `[`time_type`](#dc/d91/classalps_1_1_signed_observable_1a3ba0d36748413cdfdc754977b78c841a) 

#### `typedef `[`label_type`](#dc/d91/classalps_1_1_signed_observable_1a08ba43f0ec5f78018af7383a0bef912a) 

# class `alps::SimpleBinning` 

```
class alps::SimpleBinning
  : public alps::AbstractBinning< double >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#de/d2e/classalps_1_1_simple_binning_1a4139a0b4a93eadb902d356c0146da2fb)`(bool,has_tau)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#de/d2e/classalps_1_1_simple_binning_1afe16557209d4946dde14af61ebc7c5af)`(int,magic_id)` | 
`public inline  `[`SimpleBinning`](#de/d2e/classalps_1_1_simple_binning_1a21cf96f25e532c38adee90c222d3de28)`(std::size_t)` | 
`public inline void `[`reset`](#de/d2e/classalps_1_1_simple_binning_1ad8f5bde7ca3b8d3640248e7cafd1090f)`(bool)` | 
`public inline void `[`operator<<`](#de/d2e/classalps_1_1_simple_binning_1aa12efabf08080930fc2d90de8ff9ba16)`(const T & x)` | 
`public inline uint64_t `[`count`](#de/d2e/classalps_1_1_simple_binning_1a2bb362fc8dafd21287cd9cddb9567a55)`() const` | 
`public inline result_type `[`mean`](#de/d2e/classalps_1_1_simple_binning_1a7a8c6455ab7e4e1f8bad72e6278d5113)`() const` | 
`public inline result_type `[`variance`](#de/d2e/classalps_1_1_simple_binning_1a64d481b285be24aad9378f14c281fa1f)`() const` | 
`public inline result_type `[`error`](#de/d2e/classalps_1_1_simple_binning_1a46b944b700240276a377a26299067ea0)`(std::size_t bin_used) const` | 
`public inline double `[`error_element`](#de/d2e/classalps_1_1_simple_binning_1ab7541d778475ad20575b56be44eb1dfc)`(std::size_t element,std::size_t bin_used) const` | 
`public inline double `[`binmean_element`](#de/d2e/classalps_1_1_simple_binning_1a3d48fdc9a3c3916d6b00dd903cf5b4ea)`(std::size_t element,std::size_t i) const` | 
`public inline double `[`binvariance_element`](#de/d2e/classalps_1_1_simple_binning_1aef6033f3db7c699bf2e243fea98a4234)`(std::size_t element,std::size_t i) const` | 
`public inline double `[`variance_element`](#de/d2e/classalps_1_1_simple_binning_1a1ce2be1ab85402c37866d84380b5509e)`(std::size_t element) const` | 
`public convergence_type `[`converged_errors`](#de/d2e/classalps_1_1_simple_binning_1a0da6b52b88a6572314e7ffb482828e9c)`() const` | 
`public inline time_type `[`tau`](#de/d2e/classalps_1_1_simple_binning_1ac57191d69f609292ca2c25eb7cd4d4ef)`() const` | 
`public inline uint32_t `[`binning_depth`](#de/d2e/classalps_1_1_simple_binning_1af0a46c7bff19f8f097ceb8adea517fb0)`() const` | 
`public inline std::size_t `[`size`](#de/d2e/classalps_1_1_simple_binning_1a0ff1cf9876b040ba8bc2756a46c09a16)`() const` | 
`public void `[`output_scalar`](#de/d2e/classalps_1_1_simple_binning_1a9c86a6dd5f0917b6fda0420bcd7fb2a0)`(std::ostream & out) const` | 
`public template<>`  <br/>`inline void `[`output_vector`](#de/d2e/classalps_1_1_simple_binning_1a34c86faeda72be0d9ddf0f083122848f)`(std::ostream & out,const L &) const` | 
`public inline void `[`save`](#de/d2e/classalps_1_1_simple_binning_1a59fa048a480a31abf416b73eddc4ddfb)`(ODump & dump) const` | 
`public inline void `[`load`](#de/d2e/classalps_1_1_simple_binning_1ac43620f0ec15b01e1fc2456c2b91cdaf)`(IDump & dump)` | 
`public inline void `[`save`](#de/d2e/classalps_1_1_simple_binning_1af9ee66ffe2450c4cd40ba6fba3718881)`(hdf5::archive &) const` | 
`public inline void `[`load`](#de/d2e/classalps_1_1_simple_binning_1a4aebefb6f42bcd6d45dc8655674a5bf2)`(hdf5::archive &)` | 
`public inline std::string `[`evaluation_method`](#de/d2e/classalps_1_1_simple_binning_1a2562ae1bbf26e448930f733da05336d5)`() const` | 
`public void `[`write_scalar_xml`](#de/d2e/classalps_1_1_simple_binning_1a0afdb9584fda0d57ceef90e19e18b92f)`(oxstream & oxs) const` | 
`public template<>`  <br/>`void `[`write_vector_xml`](#de/d2e/classalps_1_1_simple_binning_1a6a5c4ec36eadcf649b049a07e5e69f27)`(oxstream & oxs,IT) const` | 
`public inline void `[`operator<<`](#de/d2e/classalps_1_1_simple_binning_1a6eba046d7bbd397c16b5857b681cf56b)`(const std::valarray< double > & x)` | 
`public inline double `[`binmean_element`](#de/d2e/classalps_1_1_simple_binning_1adbe0102dd570d8a536fa525503e3b3ea)`(std::size_t element,std::size_t i) const` | 
`public inline double `[`binvariance_element`](#de/d2e/classalps_1_1_simple_binning_1a8b3521de1973ef14ca5039974b53fa3d)`(std::size_t element,std::size_t i) const` | 
`public inline double `[`variance_element`](#de/d2e/classalps_1_1_simple_binning_1a34a5d9670ba7d435a49037ad7597eeff)`(std::size_t element) const` | 
`public inline double `[`error_element`](#de/d2e/classalps_1_1_simple_binning_1a6c6252a0742accada066fc26c048c3cb)`(std::size_t element,std::size_t i) const` | 
`public void `[`write_vector_xml`](#de/d2e/classalps_1_1_simple_binning_1acd1ff1f4e75be4b293596f73fa1cd281)`(oxstream & oxs,IT it) const` | 
`typedef `[`value_type`](#de/d2e/classalps_1_1_simple_binning_1a54484a382fdf9b2157ab5b0f0234105e) | 
`typedef `[`time_type`](#de/d2e/classalps_1_1_simple_binning_1a0d475e36e22383d3de0f71199f17a818) | 
`typedef `[`size_type`](#de/d2e/classalps_1_1_simple_binning_1aaa905fd9668eff1243aa5d0c6650841a) | 
`typedef `[`count_type`](#de/d2e/classalps_1_1_simple_binning_1a2d622a5e632e02d2732eac9f545668af) | 
`typedef `[`result_type`](#de/d2e/classalps_1_1_simple_binning_1ad1d3872906c23048ce65d9d69d763b24) | 
`typedef `[`convergence_type`](#de/d2e/classalps_1_1_simple_binning_1ac9101e89fcf25dd11e79d1bacd2bd975) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#de/d2e/classalps_1_1_simple_binning_1a4139a0b4a93eadb902d356c0146da2fb)`(bool,has_tau)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#de/d2e/classalps_1_1_simple_binning_1afe16557209d4946dde14af61ebc7c5af)`(int,magic_id)` 

#### `public inline  `[`SimpleBinning`](#de/d2e/classalps_1_1_simple_binning_1a21cf96f25e532c38adee90c222d3de28)`(std::size_t)` 

#### `public inline void `[`reset`](#de/d2e/classalps_1_1_simple_binning_1ad8f5bde7ca3b8d3640248e7cafd1090f)`(bool)` 

#### `public inline void `[`operator<<`](#de/d2e/classalps_1_1_simple_binning_1aa12efabf08080930fc2d90de8ff9ba16)`(const T & x)` 

#### `public inline uint64_t `[`count`](#de/d2e/classalps_1_1_simple_binning_1a2bb362fc8dafd21287cd9cddb9567a55)`() const` 

#### `public inline result_type `[`mean`](#de/d2e/classalps_1_1_simple_binning_1a7a8c6455ab7e4e1f8bad72e6278d5113)`() const` 

#### `public inline result_type `[`variance`](#de/d2e/classalps_1_1_simple_binning_1a64d481b285be24aad9378f14c281fa1f)`() const` 

#### `public inline result_type `[`error`](#de/d2e/classalps_1_1_simple_binning_1a46b944b700240276a377a26299067ea0)`(std::size_t bin_used) const` 

#### `public inline double `[`error_element`](#de/d2e/classalps_1_1_simple_binning_1ab7541d778475ad20575b56be44eb1dfc)`(std::size_t element,std::size_t bin_used) const` 

#### `public inline double `[`binmean_element`](#de/d2e/classalps_1_1_simple_binning_1a3d48fdc9a3c3916d6b00dd903cf5b4ea)`(std::size_t element,std::size_t i) const` 

#### `public inline double `[`binvariance_element`](#de/d2e/classalps_1_1_simple_binning_1aef6033f3db7c699bf2e243fea98a4234)`(std::size_t element,std::size_t i) const` 

#### `public inline double `[`variance_element`](#de/d2e/classalps_1_1_simple_binning_1a1ce2be1ab85402c37866d84380b5509e)`(std::size_t element) const` 

#### `public convergence_type `[`converged_errors`](#de/d2e/classalps_1_1_simple_binning_1a0da6b52b88a6572314e7ffb482828e9c)`() const` 

#### `public inline time_type `[`tau`](#de/d2e/classalps_1_1_simple_binning_1ac57191d69f609292ca2c25eb7cd4d4ef)`() const` 

#### `public inline uint32_t `[`binning_depth`](#de/d2e/classalps_1_1_simple_binning_1af0a46c7bff19f8f097ceb8adea517fb0)`() const` 

#### `public inline std::size_t `[`size`](#de/d2e/classalps_1_1_simple_binning_1a0ff1cf9876b040ba8bc2756a46c09a16)`() const` 

#### `public void `[`output_scalar`](#de/d2e/classalps_1_1_simple_binning_1a9c86a6dd5f0917b6fda0420bcd7fb2a0)`(std::ostream & out) const` 

#### `public template<>`  <br/>`inline void `[`output_vector`](#de/d2e/classalps_1_1_simple_binning_1a34c86faeda72be0d9ddf0f083122848f)`(std::ostream & out,const L &) const` 

#### `public inline void `[`save`](#de/d2e/classalps_1_1_simple_binning_1a59fa048a480a31abf416b73eddc4ddfb)`(ODump & dump) const` 

#### `public inline void `[`load`](#de/d2e/classalps_1_1_simple_binning_1ac43620f0ec15b01e1fc2456c2b91cdaf)`(IDump & dump)` 

#### `public inline void `[`save`](#de/d2e/classalps_1_1_simple_binning_1af9ee66ffe2450c4cd40ba6fba3718881)`(hdf5::archive &) const` 

#### `public inline void `[`load`](#de/d2e/classalps_1_1_simple_binning_1a4aebefb6f42bcd6d45dc8655674a5bf2)`(hdf5::archive &)` 

#### `public inline std::string `[`evaluation_method`](#de/d2e/classalps_1_1_simple_binning_1a2562ae1bbf26e448930f733da05336d5)`() const` 

#### `public void `[`write_scalar_xml`](#de/d2e/classalps_1_1_simple_binning_1a0afdb9584fda0d57ceef90e19e18b92f)`(oxstream & oxs) const` 

#### `public template<>`  <br/>`void `[`write_vector_xml`](#de/d2e/classalps_1_1_simple_binning_1a6a5c4ec36eadcf649b049a07e5e69f27)`(oxstream & oxs,IT) const` 

#### `public inline void `[`operator<<`](#de/d2e/classalps_1_1_simple_binning_1a6eba046d7bbd397c16b5857b681cf56b)`(const std::valarray< double > & x)` 

#### `public inline double `[`binmean_element`](#de/d2e/classalps_1_1_simple_binning_1adbe0102dd570d8a536fa525503e3b3ea)`(std::size_t element,std::size_t i) const` 

#### `public inline double `[`binvariance_element`](#de/d2e/classalps_1_1_simple_binning_1a8b3521de1973ef14ca5039974b53fa3d)`(std::size_t element,std::size_t i) const` 

#### `public inline double `[`variance_element`](#de/d2e/classalps_1_1_simple_binning_1a34a5d9670ba7d435a49037ad7597eeff)`(std::size_t element) const` 

#### `public inline double `[`error_element`](#de/d2e/classalps_1_1_simple_binning_1a6c6252a0742accada066fc26c048c3cb)`(std::size_t element,std::size_t i) const` 

#### `public void `[`write_vector_xml`](#de/d2e/classalps_1_1_simple_binning_1acd1ff1f4e75be4b293596f73fa1cd281)`(oxstream & oxs,IT it) const` 

#### `typedef `[`value_type`](#de/d2e/classalps_1_1_simple_binning_1a54484a382fdf9b2157ab5b0f0234105e) 

#### `typedef `[`time_type`](#de/d2e/classalps_1_1_simple_binning_1a0d475e36e22383d3de0f71199f17a818) 

#### `typedef `[`size_type`](#de/d2e/classalps_1_1_simple_binning_1aaa905fd9668eff1243aa5d0c6650841a) 

#### `typedef `[`count_type`](#de/d2e/classalps_1_1_simple_binning_1a2d622a5e632e02d2732eac9f545668af) 

#### `typedef `[`result_type`](#de/d2e/classalps_1_1_simple_binning_1ad1d3872906c23048ce65d9d69d763b24) 

#### `typedef `[`convergence_type`](#de/d2e/classalps_1_1_simple_binning_1ac9101e89fcf25dd11e79d1bacd2bd975) 

# class `alps::SimpleObservable` 

```
class alps::SimpleObservable
  : public alps::AbstractSimpleObservable< T >
  : public alps::RecordableObservable< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d0/dee/classalps_1_1_simple_observable_1a410ce62542eecb79f03be606cbc2e3c0)`(int,version)` | 
`public inline  `[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable_1ab0854352bef4605e280b9fc4f51f8c0a)`(const std::string & name,const label_type & l)` | the constructor needs a name and optionally specifications for the binning strategy
`public inline  `[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable_1a6bf9fe5bfa4beb9703bdc4aabba10086)`(const std::string & name,const binning_type & b,const label_type & l)` | 
`public inline  `[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable_1adfe454b4c2313035e94f028b62eee6d4)`(const std::string & name,uint32_t s,const label_type & l)` | 
`public inline  `[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable_1ad61e13caa8af25cd1ea94731fb15c35f)`(const std::string & name,uint32_t s,uint32_t a,const label_type & l)` | 
`public inline virtual uint32_t `[`version_id`](#d0/dee/classalps_1_1_simple_observable_1a5fcd42c90def189a967097ab22106f5e)`() const` | return a version ID uniquely identifying the class
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#d0/dee/classalps_1_1_simple_observable_1a3de77a826f7aee25690a11871c9b09e6)`() const` | clones the observable
`public virtual void `[`output`](#d0/dee/classalps_1_1_simple_observable_1ae38de068d03e6c17420a451eadd821f2)`(std::ostream &) const` | output the result
`public inline virtual ALPS_DUMMY_VOID `[`reset`](#d0/dee/classalps_1_1_simple_observable_1ac18e04292aeb30f1698c3249f4905bc5)`(bool equilibrated)` | reset the observable
`public inline virtual result_type `[`mean`](#d0/dee/classalps_1_1_simple_observable_1a693b8a4c4cdabef56fcd998df0fdc668)`() const` | the mean value
`public inline virtual bool `[`has_variance`](#d0/dee/classalps_1_1_simple_observable_1a65550fd3ca78eda81a091eb2cb0ee326)`() const` | is variance available ?
`public inline virtual result_type `[`variance`](#d0/dee/classalps_1_1_simple_observable_1a01cea4b0d3e1ee90719809fdc0c07e28)`() const` | the variance
`public inline virtual result_type `[`error`](#d0/dee/classalps_1_1_simple_observable_1a19d67ab06df866a1a4874dd524f25e85)`() const` | the error
`public inline result_type `[`error`](#d0/dee/classalps_1_1_simple_observable_1ad58232a9ee128dc892319838d2a6c2ff)`(unsigned bin_used) const` | 
`public inline virtual convergence_type `[`converged_errors`](#d0/dee/classalps_1_1_simple_observable_1a738e1a756baf599474ca71559900612e)`() const` | 
`public inline virtual count_type `[`count`](#d0/dee/classalps_1_1_simple_observable_1ae10743b14275eae9b92d63e3cb1eb053)`() const` | the number of measurements
`public inline virtual bool `[`has_tau`](#d0/dee/classalps_1_1_simple_observable_1a2058feab0b254f382e91adff65c70962)`() const` | is autocorrelation information available ?
`public inline virtual time_type `[`tau`](#d0/dee/classalps_1_1_simple_observable_1a40597c207b426aee451db1e5a709cd9b)`() const` | the autocorrelation time, throws an exception if not available
`public inline std::string `[`representation`](#d0/dee/classalps_1_1_simple_observable_1acb47a09e828c9650f782cd9138d75680)`() const` | 
`public inline virtual void `[`operator<<`](#d0/dee/classalps_1_1_simple_observable_1a2683b51ebf3d0720688b7efb7f1b6a68)`(const T & x)` | add another measurement to the observable
`public inline virtual count_type `[`bin_size`](#d0/dee/classalps_1_1_simple_observable_1a6d48da2b9cf5300ffad55a193cd9ecba)`() const` | the number of measurements per bin
`public inline void `[`set_bin_size`](#d0/dee/classalps_1_1_simple_observable_1a76de52d6de148f420d7bab55fa5bd73b)`(count_type s)` | resize bins to contain at least the given number of entries
`public inline virtual count_type `[`bin_number`](#d0/dee/classalps_1_1_simple_observable_1ab195703278063ecf6d224f827d41a101)`() const` | the number of bins
`public inline virtual count_type `[`bin_number2`](#d0/dee/classalps_1_1_simple_observable_1a7116b12a258c50e60d523c1671df3fd9)`() const` | the number of bins with squared values
`public inline virtual count_type `[`max_bin_number`](#d0/dee/classalps_1_1_simple_observable_1ac7923b73b080c2d99f05b0bf9fdd954d)`() const` | get the maximum number of bins
`public inline void `[`set_bin_number`](#d0/dee/classalps_1_1_simple_observable_1ac8c28be935d97c730774c3bf7a331792)`(count_type n)` | set the maximum number of bins This will be the maximum number from now on if additional measurements are performed.
`public inline virtual const value_type & `[`bin_value`](#d0/dee/classalps_1_1_simple_observable_1af2149e2ecac935793667d43b0fb659f2)`(count_type) const` | the value of a bin
`public inline virtual const value_type & `[`bin_value2`](#d0/dee/classalps_1_1_simple_observable_1a0be8533ed9c88fed37998750b3211f8a)`(count_type) const` | the squared value of a bin
`public inline const std::vector< value_type > & `[`bins`](#d0/dee/classalps_1_1_simple_observable_1afe6cf14403457f8a76689cdba48efa8a)`() const` | 
`public inline virtual void `[`save`](#d0/dee/classalps_1_1_simple_observable_1a7316162d663db7b67ca05089b44f0b4e)`(ODump & dump) const` | 
`public inline virtual void `[`load`](#d0/dee/classalps_1_1_simple_observable_1ab569bd7940eccdf3f6bf67ddf6818f5c)`(IDump & dump)` | 
`public inline void `[`extract_timeseries`](#d0/dee/classalps_1_1_simple_observable_1a0efabff1656d3d6799a40cc0e0e0d3e8)`(ODump & dump) const` | 
`public virtual void `[`save`](#d0/dee/classalps_1_1_simple_observable_1a7ebcf2f7a19dece2db1fe25fc5116780)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#d0/dee/classalps_1_1_simple_observable_1a8a5ce7643a1a33ad42efe3ba2ccc6faf)`(hdf5::archive &)` | 
`public inline virtual std::string `[`evaluation_method`](#d0/dee/classalps_1_1_simple_observable_1afcd2b8d02e8908a019a04512f2a99f92)`(Target t) const` | 
`typedef `[`value_type`](#d0/dee/classalps_1_1_simple_observable_1a5c0372d83be9c5d04212d78acfb7d395) | 
`typedef `[`time_type`](#d0/dee/classalps_1_1_simple_observable_1a7e2b88943ee17bb6d7509912953ea401) | 
`typedef `[`count_type`](#d0/dee/classalps_1_1_simple_observable_1afd80f98f6819e1c09c0201ec8eb2d889) | 
`typedef `[`result_type`](#d0/dee/classalps_1_1_simple_observable_1aaec8c135711d92653fc0cb9d38824001) | 
`typedef `[`slice_index`](#d0/dee/classalps_1_1_simple_observable_1a7bd603d9bf437f1df8e998fd49ebba4c) | 
`typedef `[`label_type`](#d0/dee/classalps_1_1_simple_observable_1ad06143ba990216cfe6743cf86d438220) | 
`typedef `[`convergence_type`](#d0/dee/classalps_1_1_simple_observable_1a1ff17c4ddf16a0f6a15924585c96a432) | 
`typedef `[`binning_type`](#d0/dee/classalps_1_1_simple_observable_1a803dfb895a81ed8ddb0c40288861936c) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d0/dee/classalps_1_1_simple_observable_1a410ce62542eecb79f03be606cbc2e3c0)`(int,version)` 

#### `public inline  `[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable_1ab0854352bef4605e280b9fc4f51f8c0a)`(const std::string & name,const label_type & l)` 

the constructor needs a name and optionally specifications for the binning strategy

#### `public inline  `[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable_1a6bf9fe5bfa4beb9703bdc4aabba10086)`(const std::string & name,const binning_type & b,const label_type & l)` 

#### `public inline  `[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable_1adfe454b4c2313035e94f028b62eee6d4)`(const std::string & name,uint32_t s,const label_type & l)` 

#### `public inline  `[`SimpleObservable`](#d0/dee/classalps_1_1_simple_observable_1ad61e13caa8af25cd1ea94731fb15c35f)`(const std::string & name,uint32_t s,uint32_t a,const label_type & l)` 

#### `public inline virtual uint32_t `[`version_id`](#d0/dee/classalps_1_1_simple_observable_1a5fcd42c90def189a967097ab22106f5e)`() const` 

return a version ID uniquely identifying the class

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#d0/dee/classalps_1_1_simple_observable_1a3de77a826f7aee25690a11871c9b09e6)`() const` 

clones the observable

#### `public virtual void `[`output`](#d0/dee/classalps_1_1_simple_observable_1ae38de068d03e6c17420a451eadd821f2)`(std::ostream &) const` 

output the result

#### `public inline virtual ALPS_DUMMY_VOID `[`reset`](#d0/dee/classalps_1_1_simple_observable_1ac18e04292aeb30f1698c3249f4905bc5)`(bool equilibrated)` 

reset the observable

#### `public inline virtual result_type `[`mean`](#d0/dee/classalps_1_1_simple_observable_1a693b8a4c4cdabef56fcd998df0fdc668)`() const` 

the mean value

#### `public inline virtual bool `[`has_variance`](#d0/dee/classalps_1_1_simple_observable_1a65550fd3ca78eda81a091eb2cb0ee326)`() const` 

is variance available ?

#### `public inline virtual result_type `[`variance`](#d0/dee/classalps_1_1_simple_observable_1a01cea4b0d3e1ee90719809fdc0c07e28)`() const` 

the variance

#### `public inline virtual result_type `[`error`](#d0/dee/classalps_1_1_simple_observable_1a19d67ab06df866a1a4874dd524f25e85)`() const` 

the error

#### `public inline result_type `[`error`](#d0/dee/classalps_1_1_simple_observable_1ad58232a9ee128dc892319838d2a6c2ff)`(unsigned bin_used) const` 

#### `public inline virtual convergence_type `[`converged_errors`](#d0/dee/classalps_1_1_simple_observable_1a738e1a756baf599474ca71559900612e)`() const` 

#### `public inline virtual count_type `[`count`](#d0/dee/classalps_1_1_simple_observable_1ae10743b14275eae9b92d63e3cb1eb053)`() const` 

the number of measurements

#### `public inline virtual bool `[`has_tau`](#d0/dee/classalps_1_1_simple_observable_1a2058feab0b254f382e91adff65c70962)`() const` 

is autocorrelation information available ?

#### `public inline virtual time_type `[`tau`](#d0/dee/classalps_1_1_simple_observable_1a40597c207b426aee451db1e5a709cd9b)`() const` 

the autocorrelation time, throws an exception if not available

#### `public inline std::string `[`representation`](#d0/dee/classalps_1_1_simple_observable_1acb47a09e828c9650f782cd9138d75680)`() const` 

#### `public inline virtual void `[`operator<<`](#d0/dee/classalps_1_1_simple_observable_1a2683b51ebf3d0720688b7efb7f1b6a68)`(const T & x)` 

add another measurement to the observable

#### `public inline virtual count_type `[`bin_size`](#d0/dee/classalps_1_1_simple_observable_1a6d48da2b9cf5300ffad55a193cd9ecba)`() const` 

the number of measurements per bin

#### `public inline void `[`set_bin_size`](#d0/dee/classalps_1_1_simple_observable_1a76de52d6de148f420d7bab55fa5bd73b)`(count_type s)` 

resize bins to contain at least the given number of entries

#### `public inline virtual count_type `[`bin_number`](#d0/dee/classalps_1_1_simple_observable_1ab195703278063ecf6d224f827d41a101)`() const` 

the number of bins

#### `public inline virtual count_type `[`bin_number2`](#d0/dee/classalps_1_1_simple_observable_1a7116b12a258c50e60d523c1671df3fd9)`() const` 

the number of bins with squared values

#### `public inline virtual count_type `[`max_bin_number`](#d0/dee/classalps_1_1_simple_observable_1ac7923b73b080c2d99f05b0bf9fdd954d)`() const` 

get the maximum number of bins

#### `public inline void `[`set_bin_number`](#d0/dee/classalps_1_1_simple_observable_1ac8c28be935d97c730774c3bf7a331792)`(count_type n)` 

set the maximum number of bins This will be the maximum number from now on if additional measurements are performed.

#### `public inline virtual const value_type & `[`bin_value`](#d0/dee/classalps_1_1_simple_observable_1af2149e2ecac935793667d43b0fb659f2)`(count_type) const` 

the value of a bin

#### `public inline virtual const value_type & `[`bin_value2`](#d0/dee/classalps_1_1_simple_observable_1a0be8533ed9c88fed37998750b3211f8a)`(count_type) const` 

the squared value of a bin

#### `public inline const std::vector< value_type > & `[`bins`](#d0/dee/classalps_1_1_simple_observable_1afe6cf14403457f8a76689cdba48efa8a)`() const` 

#### `public inline virtual void `[`save`](#d0/dee/classalps_1_1_simple_observable_1a7316162d663db7b67ca05089b44f0b4e)`(ODump & dump) const` 

#### `public inline virtual void `[`load`](#d0/dee/classalps_1_1_simple_observable_1ab569bd7940eccdf3f6bf67ddf6818f5c)`(IDump & dump)` 

#### `public inline void `[`extract_timeseries`](#d0/dee/classalps_1_1_simple_observable_1a0efabff1656d3d6799a40cc0e0e0d3e8)`(ODump & dump) const` 

#### `public virtual void `[`save`](#d0/dee/classalps_1_1_simple_observable_1a7ebcf2f7a19dece2db1fe25fc5116780)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#d0/dee/classalps_1_1_simple_observable_1a8a5ce7643a1a33ad42efe3ba2ccc6faf)`(hdf5::archive &)` 

#### `public inline virtual std::string `[`evaluation_method`](#d0/dee/classalps_1_1_simple_observable_1afcd2b8d02e8908a019a04512f2a99f92)`(Target t) const` 

#### `typedef `[`value_type`](#d0/dee/classalps_1_1_simple_observable_1a5c0372d83be9c5d04212d78acfb7d395) 

#### `typedef `[`time_type`](#d0/dee/classalps_1_1_simple_observable_1a7e2b88943ee17bb6d7509912953ea401) 

#### `typedef `[`count_type`](#d0/dee/classalps_1_1_simple_observable_1afd80f98f6819e1c09c0201ec8eb2d889) 

#### `typedef `[`result_type`](#d0/dee/classalps_1_1_simple_observable_1aaec8c135711d92653fc0cb9d38824001) 

#### `typedef `[`slice_index`](#d0/dee/classalps_1_1_simple_observable_1a7bd603d9bf437f1df8e998fd49ebba4c) 

#### `typedef `[`label_type`](#d0/dee/classalps_1_1_simple_observable_1ad06143ba990216cfe6743cf86d438220) 

#### `typedef `[`convergence_type`](#d0/dee/classalps_1_1_simple_observable_1a1ff17c4ddf16a0f6a15924585c96a432) 

#### `typedef `[`binning_type`](#d0/dee/classalps_1_1_simple_observable_1a803dfb895a81ed8ddb0c40288861936c) 

# class `alps::SimpleObservableData` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data_1adb5c54eb227d6e0a33afe1bf3bfdb2e2)`()` | 
`public template<>`  <br/>`inline  `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data_1a016d5ad012dc3b694158e0f240dfc3a4)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< U > & x,S s)` | 
`public  `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data_1a4d2ea4cc104313321ad806e25602b80b)`(const `[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable)`< value_type > & obs)` | 
`public  `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data_1ab31efe34f027d12cb6eba067652d88df)`(std::istream &,const XMLTag &,label_type &)` | 
`public inline `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)` const & `[`operator=`](#d6/df4/classalps_1_1_simple_observable_data_1a34d5f27c5069c94aee423d6617af0d9a)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)` & x)` | 
`public inline void `[`read_xml`](#d6/df4/classalps_1_1_simple_observable_data_1a02a295b53892a9c19ba8f0fee346ca29)`(std::istream &,const XMLTag &,label_type & label)` | 
`public void `[`read_xml_scalar`](#d6/df4/classalps_1_1_simple_observable_data_1a4b8197f9b77a259c68c3586862ce64e6)`(std::istream &,const XMLTag &)` | 
`public void `[`read_xml_vector`](#d6/df4/classalps_1_1_simple_observable_data_1a42e05d7d9578eb3cc358abb80de97935)`(std::istream &,const XMLTag &,label_type & label)` | 
`public inline ALPS_DUMMY_VOID `[`set_thermalization`](#d6/df4/classalps_1_1_simple_observable_data_1aeb00a9fdd6c3224a94281b3083049bc7)`(uint32_t todiscard)` | 
`public inline uint32_t `[`get_thermalization`](#d6/df4/classalps_1_1_simple_observable_data_1a908e2b3a7d38b21f3a93805ac282b4c9)`() const` | 
`public inline bool `[`can_set_thermalization`](#d6/df4/classalps_1_1_simple_observable_data_1a00c74e68f94e327180b85c50938b1dbd)`() const` | 
`public inline uint64_t `[`count`](#d6/df4/classalps_1_1_simple_observable_data_1a3d8ab756776f390a99f6a1d84311aab3)`() const` | 
`public inline const result_type & `[`mean`](#d6/df4/classalps_1_1_simple_observable_data_1a2844e73160f7c90fb3d8a34b31bb05b8)`() const` | 
`public inline const result_type & `[`error`](#d6/df4/classalps_1_1_simple_observable_data_1a9c0d20db9bff4e893a28653822b03ca8)`() const` | 
`public inline const convergence_type & `[`converged_errors`](#d6/df4/classalps_1_1_simple_observable_data_1a9a85d99e03364003d65711da04c8f3d6)`() const` | 
`public inline const convergence_type & `[`any_converged_errors`](#d6/df4/classalps_1_1_simple_observable_data_1a484017268c57377f7d7fdef01292a6bb)`() const` | 
`public inline const result_type & `[`variance`](#d6/df4/classalps_1_1_simple_observable_data_1ae3dc47480b47a9978a60aebcb36383a5)`() const` | 
`public inline const time_type & `[`tau`](#d6/df4/classalps_1_1_simple_observable_data_1ac0fc17e97bdf067b063e9bb7aea59d8f)`() const` | 
`public covariance_type `[`covariance`](#d6/df4/classalps_1_1_simple_observable_data_1abace48efbf31179d97fa464d4d35e127)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T >) const` | 
`public inline bool `[`has_variance`](#d6/df4/classalps_1_1_simple_observable_data_1a13bf209dc8ba8cd26c38cc12624ccad8)`() const` | 
`public inline bool `[`has_tau`](#d6/df4/classalps_1_1_simple_observable_data_1a3f12ac7dfb96917b98e80692712b3053)`() const` | 
`public inline uint64_t `[`bin_size`](#d6/df4/classalps_1_1_simple_observable_data_1af53188d24648b44b805d2aea9e506b5f)`() const` | 
`public inline std::size_t `[`bin_number`](#d6/df4/classalps_1_1_simple_observable_data_1a4509b87696ff8ab5bf7ed4b835e76d6d)`() const` | 
`public inline std::size_t `[`bin_number2`](#d6/df4/classalps_1_1_simple_observable_data_1a61c2b4f51b1574d5fdfb64b270a8d282)`() const` | 
`public inline const value_type & `[`bin_value`](#d6/df4/classalps_1_1_simple_observable_data_1a44ee36681ff7d1cec705974870f196e8)`(std::size_t i) const` | 
`public inline const value_type & `[`bin_value2`](#d6/df4/classalps_1_1_simple_observable_data_1adf586a006977acbe311cf0612eef5595)`(std::size_t i) const` | 
`public inline const std::vector< value_type > & `[`bins`](#d6/df4/classalps_1_1_simple_observable_data_1a370621653defe5d60b92464dc0c21b51)`() const` | 
`public template<>`  <br/>`inline `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< typename element_type< T >::type > `[`slice`](#d6/df4/classalps_1_1_simple_observable_data_1a5b94caf432c6286142c15d348f1590fe)`(S s) const` | 
`public ALPS_DUMMY_VOID `[`compact`](#d6/df4/classalps_1_1_simple_observable_data_1a07298e979d54c1d79e689fff2b1ee28c)`()` | 
`public void `[`extract_timeseries`](#d6/df4/classalps_1_1_simple_observable_data_1ad56949285d91119cbf250d2fb5de9d94)`(ODump & dump) const` | 
`public void `[`save`](#d6/df4/classalps_1_1_simple_observable_data_1a057e9cfbc3a84e534c1bdeafc8397f6b)`(ODump & dump) const` | 
`public void `[`load`](#d6/df4/classalps_1_1_simple_observable_data_1a471a4855e35301079f96006f957b918e)`(IDump & dump)` | 
`public void `[`save`](#d6/df4/classalps_1_1_simple_observable_data_1acdafe8bf06d0358de87cc396ed09bb4e)`(hdf5::archive &) const` | 
`public void `[`load`](#d6/df4/classalps_1_1_simple_observable_data_1ae0c5b948b5bb9e425f9f21359ae55af7)`(hdf5::archive &)` | 
`public inline void `[`set_bin_size`](#d6/df4/classalps_1_1_simple_observable_data_1a055ddf5a40f90d8ccb69363294c170d6)`(uint64_t)` | 
`public inline void `[`set_bin_number`](#d6/df4/classalps_1_1_simple_observable_data_1a01b475a5bfbce715b2d14530df43fa81)`(std::size_t)` | 
`public `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator<<`](#d6/df4/classalps_1_1_simple_observable_data_1aee034c854324cbfc5f876be58d4b0aac)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & b)` | 
`public void `[`negate`](#d6/df4/classalps_1_1_simple_observable_data_1a4bc457cc604a0b3daf27ef683ae456f1)`()` | 
`public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator+=`](#d6/df4/classalps_1_1_simple_observable_data_1a0729e1e75bf803911e9a4f0013cff19d)`(X)` | 
`public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator-=`](#d6/df4/classalps_1_1_simple_observable_data_1ac6861434d3ddc0a0f2a7bcdfed95b5c1)`(X)` | 
`public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator*=`](#d6/df4/classalps_1_1_simple_observable_data_1a76e740a7fe513a17efb3e14426ad317d)`(X)` | 
`public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator/=`](#d6/df4/classalps_1_1_simple_observable_data_1afc7f673a65e6a9f5a44b11f52f2d2ea6)`(X)` | 
`public template<>`  <br/>`void `[`subtract_from`](#d6/df4/classalps_1_1_simple_observable_data_1a29b8630e161873a9b3e9b1ff79aa8b06)`(const X & x)` | 
`public template<>`  <br/>`void `[`divide`](#d6/df4/classalps_1_1_simple_observable_data_1a7294019cd3382ed3065e69fddcdcca27)`(const X & x)` | 
`public `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator+=`](#d6/df4/classalps_1_1_simple_observable_data_1a95ed654f776fcade7bff00b3b72953cb)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > &)` | 
`public `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator-=`](#d6/df4/classalps_1_1_simple_observable_data_1af76451199b66dfa119b7dd44cc30d59d)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > &)` | 
`public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator*=`](#d6/df4/classalps_1_1_simple_observable_data_1a1b708ef4539e60706db4966b04ebcd89)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< X > &)` | 
`public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator/=`](#d6/df4/classalps_1_1_simple_observable_data_1a667f303121b804926c36d7fa0ff6a4d3)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< X > &)` | 
`public template<>`  <br/>`void `[`transform`](#d6/df4/classalps_1_1_simple_observable_data_1a8525bd6c0b617abf14a8942184f72a60)`(OP op)` | 
`public std::string `[`evaluation_method`](#d6/df4/classalps_1_1_simple_observable_data_1a9f0151bce207b1dca776aaec3b1c8dfe)`(Target t) const` | 
`protected void `[`collect_bins`](#d6/df4/classalps_1_1_simple_observable_data_1a7d21af0507749a38ec80e61a0b50c6bc)`(std::size_t howmany)` | 
`protected void `[`analyze`](#d6/df4/classalps_1_1_simple_observable_data_1ac56229af3cf121e6be5eb103092a9ad1)`() const` | 
`protected void `[`jackknife`](#d6/df4/classalps_1_1_simple_observable_data_1afeee5165bcd2553a68818555e5c88036)`() const` | 
`protected void `[`fill_jack`](#d6/df4/classalps_1_1_simple_observable_data_1abaaf25f63fb6c3427dc6abca6af484d4)`() const` | 
`protected template<>`  <br/>`void `[`transform`](#d6/df4/classalps_1_1_simple_observable_data_1a8c7c0d46f7d886a23acef4a2f91329f0)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< X > & x,OP op,double factor)` | 
`protected template<>`  <br/>`void `[`transform_linear`](#d6/df4/classalps_1_1_simple_observable_data_1ab18b1c8e52b77af4c439ecba87882cd3)`(OP op)` | 
`typedef `[`value_type`](#d6/df4/classalps_1_1_simple_observable_data_1a093eee38b709c7fdb471334a07c197ad) | 
`typedef `[`time_type`](#d6/df4/classalps_1_1_simple_observable_data_1afb4e939ce64cfdd1a98cc7d9a450ea8a) | 
`typedef `[`size_type`](#d6/df4/classalps_1_1_simple_observable_data_1a17c5e28b8bf8cab0a5369e0b9c7561bc) | 
`typedef `[`count_type`](#d6/df4/classalps_1_1_simple_observable_data_1a856eed947c8b12be2da80781bfcf825e) | 
`typedef `[`result_type`](#d6/df4/classalps_1_1_simple_observable_data_1a750d957b0e1dac53991ceed33d8302f7) | 
`typedef `[`convergence_type`](#d6/df4/classalps_1_1_simple_observable_data_1a928a8e1eb1697b8c73adde7a64ced31d) | 
`typedef `[`label_type`](#d6/df4/classalps_1_1_simple_observable_data_1a0fea1a10c6f69a82ae3e4e90a8865118) | 
`typedef `[`covariance_type`](#d6/df4/classalps_1_1_simple_observable_data_1a6a3df7b2e948b7d95790d45c812fb7f5) | 

## Members

#### `public  `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data_1adb5c54eb227d6e0a33afe1bf3bfdb2e2)`()` 

#### `public template<>`  <br/>`inline  `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data_1a016d5ad012dc3b694158e0f240dfc3a4)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< U > & x,S s)` 

#### `public  `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data_1a4d2ea4cc104313321ad806e25602b80b)`(const `[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable)`< value_type > & obs)` 

#### `public  `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data_1ab31efe34f027d12cb6eba067652d88df)`(std::istream &,const XMLTag &,label_type &)` 

#### `public inline `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)` const & `[`operator=`](#d6/df4/classalps_1_1_simple_observable_data_1a34d5f27c5069c94aee423d6617af0d9a)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)` & x)` 

#### `public inline void `[`read_xml`](#d6/df4/classalps_1_1_simple_observable_data_1a02a295b53892a9c19ba8f0fee346ca29)`(std::istream &,const XMLTag &,label_type & label)` 

#### `public void `[`read_xml_scalar`](#d6/df4/classalps_1_1_simple_observable_data_1a4b8197f9b77a259c68c3586862ce64e6)`(std::istream &,const XMLTag &)` 

#### `public void `[`read_xml_vector`](#d6/df4/classalps_1_1_simple_observable_data_1a42e05d7d9578eb3cc358abb80de97935)`(std::istream &,const XMLTag &,label_type & label)` 

#### `public inline ALPS_DUMMY_VOID `[`set_thermalization`](#d6/df4/classalps_1_1_simple_observable_data_1aeb00a9fdd6c3224a94281b3083049bc7)`(uint32_t todiscard)` 

#### `public inline uint32_t `[`get_thermalization`](#d6/df4/classalps_1_1_simple_observable_data_1a908e2b3a7d38b21f3a93805ac282b4c9)`() const` 

#### `public inline bool `[`can_set_thermalization`](#d6/df4/classalps_1_1_simple_observable_data_1a00c74e68f94e327180b85c50938b1dbd)`() const` 

#### `public inline uint64_t `[`count`](#d6/df4/classalps_1_1_simple_observable_data_1a3d8ab756776f390a99f6a1d84311aab3)`() const` 

#### `public inline const result_type & `[`mean`](#d6/df4/classalps_1_1_simple_observable_data_1a2844e73160f7c90fb3d8a34b31bb05b8)`() const` 

#### `public inline const result_type & `[`error`](#d6/df4/classalps_1_1_simple_observable_data_1a9c0d20db9bff4e893a28653822b03ca8)`() const` 

#### `public inline const convergence_type & `[`converged_errors`](#d6/df4/classalps_1_1_simple_observable_data_1a9a85d99e03364003d65711da04c8f3d6)`() const` 

#### `public inline const convergence_type & `[`any_converged_errors`](#d6/df4/classalps_1_1_simple_observable_data_1a484017268c57377f7d7fdef01292a6bb)`() const` 

#### `public inline const result_type & `[`variance`](#d6/df4/classalps_1_1_simple_observable_data_1ae3dc47480b47a9978a60aebcb36383a5)`() const` 

#### `public inline const time_type & `[`tau`](#d6/df4/classalps_1_1_simple_observable_data_1ac0fc17e97bdf067b063e9bb7aea59d8f)`() const` 

#### `public covariance_type `[`covariance`](#d6/df4/classalps_1_1_simple_observable_data_1abace48efbf31179d97fa464d4d35e127)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T >) const` 

#### `public inline bool `[`has_variance`](#d6/df4/classalps_1_1_simple_observable_data_1a13bf209dc8ba8cd26c38cc12624ccad8)`() const` 

#### `public inline bool `[`has_tau`](#d6/df4/classalps_1_1_simple_observable_data_1a3f12ac7dfb96917b98e80692712b3053)`() const` 

#### `public inline uint64_t `[`bin_size`](#d6/df4/classalps_1_1_simple_observable_data_1af53188d24648b44b805d2aea9e506b5f)`() const` 

#### `public inline std::size_t `[`bin_number`](#d6/df4/classalps_1_1_simple_observable_data_1a4509b87696ff8ab5bf7ed4b835e76d6d)`() const` 

#### `public inline std::size_t `[`bin_number2`](#d6/df4/classalps_1_1_simple_observable_data_1a61c2b4f51b1574d5fdfb64b270a8d282)`() const` 

#### `public inline const value_type & `[`bin_value`](#d6/df4/classalps_1_1_simple_observable_data_1a44ee36681ff7d1cec705974870f196e8)`(std::size_t i) const` 

#### `public inline const value_type & `[`bin_value2`](#d6/df4/classalps_1_1_simple_observable_data_1adf586a006977acbe311cf0612eef5595)`(std::size_t i) const` 

#### `public inline const std::vector< value_type > & `[`bins`](#d6/df4/classalps_1_1_simple_observable_data_1a370621653defe5d60b92464dc0c21b51)`() const` 

#### `public template<>`  <br/>`inline `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< typename element_type< T >::type > `[`slice`](#d6/df4/classalps_1_1_simple_observable_data_1a5b94caf432c6286142c15d348f1590fe)`(S s) const` 

#### `public ALPS_DUMMY_VOID `[`compact`](#d6/df4/classalps_1_1_simple_observable_data_1a07298e979d54c1d79e689fff2b1ee28c)`()` 

#### `public void `[`extract_timeseries`](#d6/df4/classalps_1_1_simple_observable_data_1ad56949285d91119cbf250d2fb5de9d94)`(ODump & dump) const` 

#### `public void `[`save`](#d6/df4/classalps_1_1_simple_observable_data_1a057e9cfbc3a84e534c1bdeafc8397f6b)`(ODump & dump) const` 

#### `public void `[`load`](#d6/df4/classalps_1_1_simple_observable_data_1a471a4855e35301079f96006f957b918e)`(IDump & dump)` 

#### `public void `[`save`](#d6/df4/classalps_1_1_simple_observable_data_1acdafe8bf06d0358de87cc396ed09bb4e)`(hdf5::archive &) const` 

#### `public void `[`load`](#d6/df4/classalps_1_1_simple_observable_data_1ae0c5b948b5bb9e425f9f21359ae55af7)`(hdf5::archive &)` 

#### `public inline void `[`set_bin_size`](#d6/df4/classalps_1_1_simple_observable_data_1a055ddf5a40f90d8ccb69363294c170d6)`(uint64_t)` 

#### `public inline void `[`set_bin_number`](#d6/df4/classalps_1_1_simple_observable_data_1a01b475a5bfbce715b2d14530df43fa81)`(std::size_t)` 

#### `public `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator<<`](#d6/df4/classalps_1_1_simple_observable_data_1aee034c854324cbfc5f876be58d4b0aac)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & b)` 

#### `public void `[`negate`](#d6/df4/classalps_1_1_simple_observable_data_1a4bc457cc604a0b3daf27ef683ae456f1)`()` 

#### `public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator+=`](#d6/df4/classalps_1_1_simple_observable_data_1a0729e1e75bf803911e9a4f0013cff19d)`(X)` 

#### `public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator-=`](#d6/df4/classalps_1_1_simple_observable_data_1ac6861434d3ddc0a0f2a7bcdfed95b5c1)`(X)` 

#### `public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator*=`](#d6/df4/classalps_1_1_simple_observable_data_1a76e740a7fe513a17efb3e14426ad317d)`(X)` 

#### `public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator/=`](#d6/df4/classalps_1_1_simple_observable_data_1afc7f673a65e6a9f5a44b11f52f2d2ea6)`(X)` 

#### `public template<>`  <br/>`void `[`subtract_from`](#d6/df4/classalps_1_1_simple_observable_data_1a29b8630e161873a9b3e9b1ff79aa8b06)`(const X & x)` 

#### `public template<>`  <br/>`void `[`divide`](#d6/df4/classalps_1_1_simple_observable_data_1a7294019cd3382ed3065e69fddcdcca27)`(const X & x)` 

#### `public `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator+=`](#d6/df4/classalps_1_1_simple_observable_data_1a95ed654f776fcade7bff00b3b72953cb)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > &)` 

#### `public `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator-=`](#d6/df4/classalps_1_1_simple_observable_data_1af76451199b66dfa119b7dd44cc30d59d)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > &)` 

#### `public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator*=`](#d6/df4/classalps_1_1_simple_observable_data_1a1b708ef4539e60706db4966b04ebcd89)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< X > &)` 

#### `public template<>`  <br/>[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & `[`operator/=`](#d6/df4/classalps_1_1_simple_observable_data_1a667f303121b804926c36d7fa0ff6a4d3)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< X > &)` 

#### `public template<>`  <br/>`void `[`transform`](#d6/df4/classalps_1_1_simple_observable_data_1a8525bd6c0b617abf14a8942184f72a60)`(OP op)` 

#### `public std::string `[`evaluation_method`](#d6/df4/classalps_1_1_simple_observable_data_1a9f0151bce207b1dca776aaec3b1c8dfe)`(Target t) const` 

#### `protected void `[`collect_bins`](#d6/df4/classalps_1_1_simple_observable_data_1a7d21af0507749a38ec80e61a0b50c6bc)`(std::size_t howmany)` 

#### `protected void `[`analyze`](#d6/df4/classalps_1_1_simple_observable_data_1ac56229af3cf121e6be5eb103092a9ad1)`() const` 

#### `protected void `[`jackknife`](#d6/df4/classalps_1_1_simple_observable_data_1afeee5165bcd2553a68818555e5c88036)`() const` 

#### `protected void `[`fill_jack`](#d6/df4/classalps_1_1_simple_observable_data_1abaaf25f63fb6c3427dc6abca6af484d4)`() const` 

#### `protected template<>`  <br/>`void `[`transform`](#d6/df4/classalps_1_1_simple_observable_data_1a8c7c0d46f7d886a23acef4a2f91329f0)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< X > & x,OP op,double factor)` 

#### `protected template<>`  <br/>`void `[`transform_linear`](#d6/df4/classalps_1_1_simple_observable_data_1ab18b1c8e52b77af4c439ecba87882cd3)`(OP op)` 

#### `typedef `[`value_type`](#d6/df4/classalps_1_1_simple_observable_data_1a093eee38b709c7fdb471334a07c197ad) 

#### `typedef `[`time_type`](#d6/df4/classalps_1_1_simple_observable_data_1afb4e939ce64cfdd1a98cc7d9a450ea8a) 

#### `typedef `[`size_type`](#d6/df4/classalps_1_1_simple_observable_data_1a17c5e28b8bf8cab0a5369e0b9c7561bc) 

#### `typedef `[`count_type`](#d6/df4/classalps_1_1_simple_observable_data_1a856eed947c8b12be2da80781bfcf825e) 

#### `typedef `[`result_type`](#d6/df4/classalps_1_1_simple_observable_data_1a750d957b0e1dac53991ceed33d8302f7) 

#### `typedef `[`convergence_type`](#d6/df4/classalps_1_1_simple_observable_data_1a928a8e1eb1697b8c73adde7a64ced31d) 

#### `typedef `[`label_type`](#d6/df4/classalps_1_1_simple_observable_data_1a0fea1a10c6f69a82ae3e4e90a8865118) 

#### `typedef `[`covariance_type`](#d6/df4/classalps_1_1_simple_observable_data_1a6a3df7b2e948b7d95790d45c812fb7f5) 

# class `alps::SimpleObservableEvaluator` 

```
class alps::SimpleObservableEvaluator
  : public alps::AbstractSimpleObservable< T >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline virtual uint32_t `[`version_id`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a852cbf03f1d37bd10f40614774b4864b)`() const` | return a version ID uniquely identifying the class
`public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1af974668b196583042a5ef52518dd4827)`(const std::string & n)` | almost default constructor
`public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a2c2c7df34968279467389e798def1e6a)`(const char * n)` | 
`public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a15af751f2896dad4fc5ba853cf958346)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)` & eval)` | copy constructor
`public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6bfb70311682703046d3f86276453fad)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs,const std::string & n)` | constructor from an observable
`public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a99efb77b6d9956f24f42513d911b2dba)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs)` | 
`public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1abceb501a81f041dfd51e4201c2878c5a)`(const std::string & n,std::istream &,const XMLTag &)` | 
`public inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ac813e6cfb71e9f0aec146ed4b83225b0)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & eval)` | needed for silcing: assign an observable, replacing all observables in the class
`public inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a0b5d68de38f02589781d0bb18c546e36)`(const `[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable)`< T > & obs)` | 
`public inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator<<`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ad022fd6dc530c7dce9fc90efc776d261)`(const `[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable)`< T > & obs)` | add an observable to the ones already in the class
`public inline virtual void `[`rename`](#d7/de4/classalps_1_1_simple_observable_evaluator_1af944f3ecdc4c0b672963ce5da473215b)`(const std::string &)` | rename the observable
`public inline void `[`rename`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a05c18f171e2fd1f61f53c6272a39c6ce)`(const std::string & n,bool a)` | 
`public inline virtual ALPS_DUMMY_VOID `[`reset`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ad98a4461a919333c8141a8314093c29b)`(bool equilibrated)` | reset the observable
`public inline virtual bool `[`has_tau`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aa8c151eeb76c34a0cff9c032cb09dbd2)`() const` | is autocorrelation information available ?
`public inline virtual bool `[`has_variance`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a57b8f7848fc82ff98f26821fea88590b)`() const` | is variance available ?
`public inline result_type `[`value`](#d7/de4/classalps_1_1_simple_observable_evaluator_1abeaef05b357a5b8bacd723ff929afd07)`() const` | 
`public inline virtual result_type `[`mean`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a260f2cad341d3223fe7054f8176b366f)`() const` | the mean value
`public inline virtual result_type `[`variance`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1faf0d6f604e5658664782b098a5433c)`() const` | the variance
`public inline virtual result_type `[`error`](#d7/de4/classalps_1_1_simple_observable_evaluator_1abe204d3ef7bb856dbb68870a8a29f6da)`() const` | the error
`public inline virtual convergence_type `[`converged_errors`](#d7/de4/classalps_1_1_simple_observable_evaluator_1adc09ffacc0353a368ed59bbaad3a1850)`() const` | 
`public inline virtual time_type `[`tau`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a9848728886bfd0fc521a44b10a46dd72)`() const` | the autocorrelation time, throws an exception if not available
`public inline covariance_type `[`covariance`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a4a37b0f82e26b5e6c99134aa4fe6aa1d)`(`[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)` & obs2) const` | 
`public inline virtual count_type `[`bin_number`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ae8ba29f3d661fd7c9d06a219721f6d64)`() const` | the number of bins
`public inline virtual const value_type & `[`bin_value`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aba916e10e749d18b7a5929945fd99f8c)`(count_type) const` | the value of a bin
`public inline virtual count_type `[`bin_number2`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ad4fb19b594d0733f4692579aeb82e719)`() const` | the number of bins with squared values
`public inline virtual const value_type & `[`bin_value2`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a3e4e02ec85b9d74033c4e650d30d7207)`(count_type) const` | the squared value of a bin
`public inline virtual count_type `[`bin_size`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6119525407750e184b2d1232c9061046)`() const` | the number of measurements per bin
`public inline virtual count_type `[`count`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6bc099dea8f0f7c9498ef94c828c7b36)`() const` | the number of measurements
`public inline const std::vector< value_type > & `[`bins`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1c0d9cc449c5adbbb68f0f55176f7034)`() const` | 
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#d7/de4/classalps_1_1_simple_observable_evaluator_1adcff4e6ded0b51916284278dea7a72e1)`() const` | clones the observable
`public inline uint32_t `[`get_thermalization`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a4532d11bdc8c1a4416f8e64ba025a390)`() const` | 
`public inline bool `[`can_set_thermalization`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ac3661efe0f32ab2119256d3a7f3821d1)`() const` | 
`public inline ALPS_DUMMY_VOID `[`compact`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aed61dd8b83a930cc7754ce0855dde8ae)`()` | 
`public inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator-`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a0736eba198a8606a9b94004ae6b42180)`() const` | negate
`public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator+=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7a3de3db88b8392bacbfac5037d801fa)`(const X &)` | add a constant
`public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator-=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a8ea6ec51ba0ec1d2992a4eebbfee1063)`(const X &)` | subtract a constant
`public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator*=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a5ce36e317f4d5a7a54efaf9de0a0a797)`(const X &)` | multiply with a constant
`public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator/=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7ae6dfcb6f0ab23db7ae14fc5c644887)`(const X &)` | divide by a constant
`public inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator+=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ae37a1641497ea415b16b5d2dde67d9fc)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > &)` | add another observable
`public inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator-=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a11224f570fece4853c51c86850083806)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > &)` | subtract another observable
`public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator*=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1afdda1c6e2855a698840d32983116a449)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< X > &)` | multiply by another observable
`public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator/=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a652eeea63b0b67b26c77525967168771)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< X > &)` | divide by another observable
`public virtual ALPS_DUMMY_VOID `[`output`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a90fd28716150050cd4c412f28227384d)`(std::ostream &) const` | output the result
`public void `[`output_scalar`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aca8e289aee5580daf689fce31a25fde7)`(std::ostream &) const` | 
`public void `[`output_vector`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1cfd9327c148270dc73db926d750c32c)`(std::ostream &) const` | 
`public template<>`  <br/>`inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< T >::type > `[`slice`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a705593b5d0bc57ca8b3791cbfb51f077)`(const S &,const std::string &) const` | 
`public template<>`  <br/>`inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< T >::type > `[`slice`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ad199bc1c87078361eb8a7ca7ad80981b)`(const S &) const` | 
`public inline void `[`operator<<`](#d7/de4/classalps_1_1_simple_observable_evaluator_1af8111ce515f1eecfa3bab0a06d8524ba)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & obs)` | 
`public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`transform`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a97af81ebff319dc23e5a31837c5e8b07)`(OPV opv,const std::string &)` | 
`public inline void `[`extract_timeseries`](#d7/de4/classalps_1_1_simple_observable_evaluator_1af03c8dc9625f5c1a5b0afdd3138a13e5)`(ODump & dump) const` | 
`public inline virtual void `[`save`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a9e1fbdb1d46457cd4da51f1e7bd9191e)`(ODump & dump) const` | 
`public inline virtual void `[`load`](#d7/de4/classalps_1_1_simple_observable_evaluator_1afeaf413d33b8c7123ca8dac8e69a63a0)`(IDump & dump)` | 
`public inline virtual void `[`save`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a69c5ad4b545ccc1a1343f01b775e592f)`(hdf5::archive &) const` | 
`public inline virtual void `[`load`](#d7/de4/classalps_1_1_simple_observable_evaluator_1afb3aca397519fe3450c44fd576cee4c2)`(hdf5::archive &)` | 
`public template<>`  <br/>`inline void `[`add_to`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1df749b5d6a75fbac88368de35e6b537)`(const X & x)` | 
`public template<>`  <br/>`inline void `[`subtract_from`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7238e113ff61bc8775f7082a8778fd73)`(const X & x)` | 
`public template<>`  <br/>`inline void `[`divide`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6f07d6b7a661d6e2e249ef18130d1836)`(const X & x)` | 
`public template<>`  <br/>`inline void `[`multiply_to`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a9a52c2d76722a796525b6c81b673345e)`(const X & x)` | 
`public inline virtual std::string `[`evaluation_method`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1d1306b22cd1a99ffc8d63b6978b5cc4)`(Target t) const` | 
`public inline virtual void `[`merge`](#d7/de4/classalps_1_1_simple_observable_evaluator_1acb8fc5567aa22b4a05bb3bffe1a17fa9)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &)` | 
`public inline virtual bool `[`can_merge`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a78df84fff4781c0a54ce7ac7595573ce)`() const` | can this observable be merged with one of the same type
`public inline virtual bool `[`can_merge`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1be7470d13a849c76fb0e8b329b606b7)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &) const` | can this observable be merged with one of the given type
`public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`convert_mergeable`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a777ca0779aabeaf5cb6b4305c23d27ad)`() const` | create a copy of the observable that can be merged
`public inline virtual `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< value_type > `[`make_evaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a9a7a43b1f42acaeaf8b3be851afc48df)`() const` | 
`enum `[``](#d7/de4/classalps_1_1_simple_observable_evaluator_1a0fb142ccec33349d7d5dac6d03b7376c) | 
`typedef `[`value_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7afdca9e09c6fba41be48b89a12f6ddb) | 
`typedef `[`time_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1adb9aba35e0aec496e43bbb85b6cc628f) | 
`typedef `[`result_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a007b865176783542eeb9f79b51decd05) | 
`typedef `[`convergence_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aa11cc49463982f77613f0791830f5dcf) | 
`typedef `[`label_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7d76846ea813a9c3ed5cc197585739d3) | 
`typedef `[`count_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6418a3de01b82992a895b416bb3db28f) | 
`typedef `[`covariance_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ab0dffd23383bf31da88ff870cd713ad9) | 

## Members

#### `public inline virtual uint32_t `[`version_id`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a852cbf03f1d37bd10f40614774b4864b)`() const` 

return a version ID uniquely identifying the class

#### `public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1af974668b196583042a5ef52518dd4827)`(const std::string & n)` 

almost default constructor

#### `public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a2c2c7df34968279467389e798def1e6a)`(const char * n)` 

#### `public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a15af751f2896dad4fc5ba853cf958346)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)` & eval)` 

copy constructor

#### `public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6bfb70311682703046d3f86276453fad)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs,const std::string & n)` 

constructor from an observable

#### `public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a99efb77b6d9956f24f42513d911b2dba)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` & obs)` 

#### `public inline  `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1abceb501a81f041dfd51e4201c2878c5a)`(const std::string & n,std::istream &,const XMLTag &)` 

#### `public inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ac813e6cfb71e9f0aec146ed4b83225b0)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & eval)` 

needed for silcing: assign an observable, replacing all observables in the class

#### `public inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a0b5d68de38f02589781d0bb18c546e36)`(const `[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable)`< T > & obs)` 

#### `public inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator<<`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ad022fd6dc530c7dce9fc90efc776d261)`(const `[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable)`< T > & obs)` 

add an observable to the ones already in the class

#### `public inline virtual void `[`rename`](#d7/de4/classalps_1_1_simple_observable_evaluator_1af944f3ecdc4c0b672963ce5da473215b)`(const std::string &)` 

rename the observable

#### `public inline void `[`rename`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a05c18f171e2fd1f61f53c6272a39c6ce)`(const std::string & n,bool a)` 

#### `public inline virtual ALPS_DUMMY_VOID `[`reset`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ad98a4461a919333c8141a8314093c29b)`(bool equilibrated)` 

reset the observable

#### `public inline virtual bool `[`has_tau`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aa8c151eeb76c34a0cff9c032cb09dbd2)`() const` 

is autocorrelation information available ?

#### `public inline virtual bool `[`has_variance`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a57b8f7848fc82ff98f26821fea88590b)`() const` 

is variance available ?

#### `public inline result_type `[`value`](#d7/de4/classalps_1_1_simple_observable_evaluator_1abeaef05b357a5b8bacd723ff929afd07)`() const` 

#### `public inline virtual result_type `[`mean`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a260f2cad341d3223fe7054f8176b366f)`() const` 

the mean value

#### `public inline virtual result_type `[`variance`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1faf0d6f604e5658664782b098a5433c)`() const` 

the variance

#### `public inline virtual result_type `[`error`](#d7/de4/classalps_1_1_simple_observable_evaluator_1abe204d3ef7bb856dbb68870a8a29f6da)`() const` 

the error

#### `public inline virtual convergence_type `[`converged_errors`](#d7/de4/classalps_1_1_simple_observable_evaluator_1adc09ffacc0353a368ed59bbaad3a1850)`() const` 

#### `public inline virtual time_type `[`tau`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a9848728886bfd0fc521a44b10a46dd72)`() const` 

the autocorrelation time, throws an exception if not available

#### `public inline covariance_type `[`covariance`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a4a37b0f82e26b5e6c99134aa4fe6aa1d)`(`[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)` & obs2) const` 

#### `public inline virtual count_type `[`bin_number`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ae8ba29f3d661fd7c9d06a219721f6d64)`() const` 

the number of bins

#### `public inline virtual const value_type & `[`bin_value`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aba916e10e749d18b7a5929945fd99f8c)`(count_type) const` 

the value of a bin

#### `public inline virtual count_type `[`bin_number2`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ad4fb19b594d0733f4692579aeb82e719)`() const` 

the number of bins with squared values

#### `public inline virtual const value_type & `[`bin_value2`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a3e4e02ec85b9d74033c4e650d30d7207)`(count_type) const` 

the squared value of a bin

#### `public inline virtual count_type `[`bin_size`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6119525407750e184b2d1232c9061046)`() const` 

the number of measurements per bin

#### `public inline virtual count_type `[`count`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6bc099dea8f0f7c9498ef94c828c7b36)`() const` 

the number of measurements

#### `public inline const std::vector< value_type > & `[`bins`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1c0d9cc449c5adbbb68f0f55176f7034)`() const` 

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`clone`](#d7/de4/classalps_1_1_simple_observable_evaluator_1adcff4e6ded0b51916284278dea7a72e1)`() const` 

clones the observable

#### `public inline uint32_t `[`get_thermalization`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a4532d11bdc8c1a4416f8e64ba025a390)`() const` 

#### `public inline bool `[`can_set_thermalization`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ac3661efe0f32ab2119256d3a7f3821d1)`() const` 

#### `public inline ALPS_DUMMY_VOID `[`compact`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aed61dd8b83a930cc7754ce0855dde8ae)`()` 

#### `public inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > `[`operator-`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a0736eba198a8606a9b94004ae6b42180)`() const` 

negate

#### `public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator+=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7a3de3db88b8392bacbfac5037d801fa)`(const X &)` 

add a constant

#### `public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator-=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a8ea6ec51ba0ec1d2992a4eebbfee1063)`(const X &)` 

subtract a constant

#### `public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator*=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a5ce36e317f4d5a7a54efaf9de0a0a797)`(const X &)` 

multiply with a constant

#### `public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator/=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7ae6dfcb6f0ab23db7ae14fc5c644887)`(const X &)` 

divide by a constant

#### `public inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator+=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ae37a1641497ea415b16b5d2dde67d9fc)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > &)` 

add another observable

#### `public inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator-=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a11224f570fece4853c51c86850083806)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > &)` 

subtract another observable

#### `public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator*=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1afdda1c6e2855a698840d32983116a449)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< X > &)` 

multiply by another observable

#### `public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`operator/=`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a652eeea63b0b67b26c77525967168771)`(const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< X > &)` 

divide by another observable

#### `public virtual ALPS_DUMMY_VOID `[`output`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a90fd28716150050cd4c412f28227384d)`(std::ostream &) const` 

output the result

#### `public void `[`output_scalar`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aca8e289aee5580daf689fce31a25fde7)`(std::ostream &) const` 

#### `public void `[`output_vector`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1cfd9327c148270dc73db926d750c32c)`(std::ostream &) const` 

#### `public template<>`  <br/>`inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< T >::type > `[`slice`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a705593b5d0bc57ca8b3791cbfb51f077)`(const S &,const std::string &) const` 

#### `public template<>`  <br/>`inline `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< typename element_type< T >::type > `[`slice`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ad199bc1c87078361eb8a7ca7ad80981b)`(const S &) const` 

#### `public inline void `[`operator<<`](#d7/de4/classalps_1_1_simple_observable_evaluator_1af8111ce515f1eecfa3bab0a06d8524ba)`(const `[`SimpleObservableData`](#d6/df4/classalps_1_1_simple_observable_data)`< T > & obs)` 

#### `public template<>`  <br/>`inline const `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< T > & `[`transform`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a97af81ebff319dc23e5a31837c5e8b07)`(OPV opv,const std::string &)` 

#### `public inline void `[`extract_timeseries`](#d7/de4/classalps_1_1_simple_observable_evaluator_1af03c8dc9625f5c1a5b0afdd3138a13e5)`(ODump & dump) const` 

#### `public inline virtual void `[`save`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a9e1fbdb1d46457cd4da51f1e7bd9191e)`(ODump & dump) const` 

#### `public inline virtual void `[`load`](#d7/de4/classalps_1_1_simple_observable_evaluator_1afeaf413d33b8c7123ca8dac8e69a63a0)`(IDump & dump)` 

#### `public inline virtual void `[`save`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a69c5ad4b545ccc1a1343f01b775e592f)`(hdf5::archive &) const` 

#### `public inline virtual void `[`load`](#d7/de4/classalps_1_1_simple_observable_evaluator_1afb3aca397519fe3450c44fd576cee4c2)`(hdf5::archive &)` 

#### `public template<>`  <br/>`inline void `[`add_to`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1df749b5d6a75fbac88368de35e6b537)`(const X & x)` 

#### `public template<>`  <br/>`inline void `[`subtract_from`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7238e113ff61bc8775f7082a8778fd73)`(const X & x)` 

#### `public template<>`  <br/>`inline void `[`divide`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6f07d6b7a661d6e2e249ef18130d1836)`(const X & x)` 

#### `public template<>`  <br/>`inline void `[`multiply_to`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a9a52c2d76722a796525b6c81b673345e)`(const X & x)` 

#### `public inline virtual std::string `[`evaluation_method`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1d1306b22cd1a99ffc8d63b6978b5cc4)`(Target t) const` 

#### `public inline virtual void `[`merge`](#d7/de4/classalps_1_1_simple_observable_evaluator_1acb8fc5567aa22b4a05bb3bffe1a17fa9)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &)` 

#### `public inline virtual bool `[`can_merge`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a78df84fff4781c0a54ce7ac7595573ce)`() const` 

can this observable be merged with one of the same type

#### `public inline virtual bool `[`can_merge`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a1be7470d13a849c76fb0e8b329b606b7)`(const `[`Observable`](#df/d26/classalps_1_1_observable)` &) const` 

can this observable be merged with one of the given type

#### `public inline virtual `[`Observable`](#df/d26/classalps_1_1_observable)` * `[`convert_mergeable`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a777ca0779aabeaf5cb6b4305c23d27ad)`() const` 

create a copy of the observable that can be merged

#### `public inline virtual `[`SimpleObservableEvaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator)`< value_type > `[`make_evaluator`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a9a7a43b1f42acaeaf8b3be851afc48df)`() const` 

#### `enum `[``](#d7/de4/classalps_1_1_simple_observable_evaluator_1a0fb142ccec33349d7d5dac6d03b7376c) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
version            | 

#### `typedef `[`value_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7afdca9e09c6fba41be48b89a12f6ddb) 

#### `typedef `[`time_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1adb9aba35e0aec496e43bbb85b6cc628f) 

#### `typedef `[`result_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a007b865176783542eeb9f79b51decd05) 

#### `typedef `[`convergence_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1aa11cc49463982f77613f0791830f5dcf) 

#### `typedef `[`label_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a7d76846ea813a9c3ed5cc197585739d3) 

#### `typedef `[`count_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1a6418a3de01b82992a895b416bb3db28f) 

#### `typedef `[`covariance_type`](#d7/de4/classalps_1_1_simple_observable_evaluator_1ab0dffd23383bf31da88ff870cd713ad9) 

# struct `alps::ObservableNamingHelper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::output_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::output_helper< boost::mpl::false_ >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::output_helper< boost::mpl::true_ >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::type_tag< std::valarray< T > >` 

```
struct alps::type_tag< std::valarray< T > >
  : public boost::mpl::int_< 256+type_tag< T >::value >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::type_tag< std::vector< T > >` 

```
struct alps::type_tag< std::vector< T > >
  : public boost::mpl::int_< 256+type_tag< T >::value >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# namespace `alps::alea` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>[`const_iterator_type`](#d6/dd3/structalps_1_1alea_1_1const__iterator__type)`< TimeseriesType >::type `[`range_begin`](#df/d51/mcanalyze_8hpp_1a9a1a236f9423fb0b430e2b2ef3c0e87a)`(const TimeseriesType & timeseries)`            | 
`public template<>`  <br/>`std::vector< ValueType >::const_iterator `[`range_begin`](#df/d51/mcanalyze_8hpp_1a447b63a38b841f16b2908a5288078cda)`(const `[`alps::alea::mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< ValueType > & timeseries)`            | 
`public template<>`  <br/>[`const_iterator_type`](#d6/dd3/structalps_1_1alea_1_1const__iterator__type)`< TimeseriesType >::type `[`range_end`](#df/d51/mcanalyze_8hpp_1a97ab74696ed7a3ee0d037e317a38bc43)`(const TimeseriesType & timeseries)`            | 
`public template<>`  <br/>`std::vector< ValueType >::const_iterator `[`range_end`](#df/d51/mcanalyze_8hpp_1ac00249394583311cfd606791eddad4bb)`(const `[`alps::alea::mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< ValueType > & timeseries)`            | 
`public template<>`  <br/>[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< typename TimeseriesType::value_type > `[`cut_head_distance`](#df/d51/mcanalyze_8hpp_1abd691553fcb5ff786da40c07c08e84dc)`(const TimeseriesType & timeseries,int cutoff)`            | 
`public template<>`  <br/>[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< typename TimeseriesType::value_type > `[`cut_tail_distance`](#df/d51/mcanalyze_8hpp_1a39b3b8d12f39e5a45558dc1b4c1d565f)`(const TimeseriesType & timeseries,int cutoff)`            | 
`public template<>`  <br/>[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< typename TimeseriesType::value_type > `[`cut_head_limit`](#df/d51/mcanalyze_8hpp_1a9cb396f162af3de2960020d759deb98b)`(const TimeseriesType & timeseries,double limit)`            | 
`public template<>`  <br/>[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< typename TimeseriesType::value_type > `[`cut_tail_limit`](#df/d51/mcanalyze_8hpp_1ab86261ab4c4b6c9ff1131cf883fc2eb6)`(const TimeseriesType & timeseries,double limit)`            | 
`public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`mean`](#df/d51/mcanalyze_8hpp_1a147856cf8919d2c5e24196d86a6280cf)`(const TimeseriesType & timeseries)`            | 
`public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`variance`](#df/d51/mcanalyze_8hpp_1ab29bc15f9a9168f6df36aedfc72bf287)`(const TimeseriesType & timeseries)`            | 
`public template<>`  <br/>[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< typename average_type< typename TimeseriesType::value_type >::type > `[`autocorrelation_distance`](#df/d51/mcanalyze_8hpp_1aba91006861f71ae72fff7f19f420f003)`(const TimeseriesType & timeseries,int up_to)`            | 
`public template<>`  <br/>[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< typename average_type< typename TimeseriesType::value_type >::type > `[`autocorrelation_limit`](#df/d51/mcanalyze_8hpp_1a67786e8d84cdd70e185e66dc8ef6a5b3)`(const TimeseriesType & timeseries,double limit)`            | 
`public template<>`  <br/>`std::pair< typename average_type< typename TimeseriesType::value_type >::type, typename average_type< typename TimeseriesType::value_type >::type > `[`exponential_autocorrelation_time_distance`](#df/d51/mcanalyze_8hpp_1a1d4692bf22af0eb6e6a578366d13b59e)`(const TimeseriesType & autocorrelation,int from,int to)`            | 
`public template<>`  <br/>`std::pair< typename average_type< typename TimeseriesType::value_type >::type, typename average_type< typename TimeseriesType::value_type >::type > `[`exponential_autocorrelation_time_limit`](#df/d51/mcanalyze_8hpp_1a1b51c7a7ab0c6bc3f767583f5445026a)`(const TimeseriesType & autocorrelation,double max,double min)`            | 
`public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`integrated_autocorrelation_time`](#df/d51/mcanalyze_8hpp_1a93b39244179cbf0a42b97149bb924104)`(const TimeseriesType & autocorrelation,const std::pair< typename average_type< typename TimeseriesType::value_type >::type, typename average_type< typename TimeseriesType::value_type >::type > & tau)`            | 
`public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`error`](#df/d51/mcanalyze_8hpp_1ac84c44931f6df3f8a68a4b6ab32a8f6b)`(const TimeseriesType & timeseries,const `[`uncorrelated_selector`](#d1/db1/structalps_1_1alea_1_1uncorrelated__selector)` & selector)`            | 
`public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`error`](#df/d51/mcanalyze_8hpp_1aaaa701d6e01e269bdf54d0fc11d42ad9)`(const TimeseriesType & timeseries,const `[`binning_selector`](#db/d1d/structalps_1_1alea_1_1binning__selector)` & selector)`            | 
`public template<>`  <br/>`inline average_type< typenameTimeseriesType::value_type >::type `[`uncorrelated_error`](#df/d51/mcanalyze_8hpp_1aff871e63952b8b3696afe83eca2b9096)`(const TimeseriesType & timeseries)`            | 
`public template<>`  <br/>`inline average_type< typenameTimeseriesType::value_type >::type `[`binning_error`](#df/d51/mcanalyze_8hpp_1af3bdb959edd8395d589f2ff9799ceff7)`(const TimeseriesType & timeseries)`            | 
`public template<>`  <br/>[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< typename average_type< typename TimeseriesType::value_type >::type > `[`running_mean`](#df/d51/mcanalyze_8hpp_1a3237d010efb8a46566bc29c48365ec0d)`(const TimeseriesType & timeseries)`            | 
`public template<>`  <br/>[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< typename average_type< typename TimeseriesType::value_type >::type > `[`reverse_running_mean`](#df/d51/mcanalyze_8hpp_1aa774554bb5491f0c7995a04fce02123f)`(const TimeseriesType & timeseries)`            | 
`public template<>`  <br/>`inline std::ostream & `[`operator<<`](#d8/d81/mcdata_8hpp_1a0f4b2305701d014bf4bff0f0674caf9b)`(std::ostream & out,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & obs)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`operator+`](#d8/d81/mcdata_8hpp_1a03dca1afd93bd34a5705e266059de68e)`(T const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`operator-`](#d8/d81/mcdata_8hpp_1adc8992c62941dc928c72e62338b37070)`(T const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`operator*`](#d8/d81/mcdata_8hpp_1acc8b32bf8c54d821c34c568572231a91)`(T const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`operator/`](#d8/d81/mcdata_8hpp_1a3311188edd9a927316a719d045dbb770)`(T const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator+`](#d8/d81/mcdata_8hpp_1a8e7502812529d8260b3fb59e5e6e7445)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator+`](#d8/d81/mcdata_8hpp_1aac9f24ad3531df25f736f37bc0ae9a39)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator-`](#d8/d81/mcdata_8hpp_1aa5052a8472301492645577c17654e6bc)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator-`](#d8/d81/mcdata_8hpp_1a1578d7c90537102a3aabb948a5b32ce8)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator*`](#d8/d81/mcdata_8hpp_1ab2f09e4725cf74fdf0cf6f39cda70007)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator*`](#d8/d81/mcdata_8hpp_1a7f86409880e6c4905a120b1957819941)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator/`](#d8/d81/mcdata_8hpp_1ad5ed9bf1d3196edd1cfdf7374064f63f)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg2)`            | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator/`](#d8/d81/mcdata_8hpp_1a3ea5189c649b3ede76f65bc5beb0cb83)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg2)`            | 
`public template<>`  <br/>[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`pow`](#d8/d81/mcdata_8hpp_1a1a60702d2252b8d65523bc523de5db87)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > rhs,typename `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T >::recursive_element_type exponent)`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a67a6cc083195ce6f2bfc13c0be6fc00c)`(sin,abs(cos(rhs.mean()) *rhs.error()))`            | 
`public  `[`abs`](#d8/d81/mcdata_8hpp_1aab0577c994c1599a36c038a55f276d35)`(- sin)`            | 
`public  `[`abs`](#d8/d81/mcdata_8hpp_1a6c01f91f0088ade9ff5c8aaf58e34419)`(1./)`            | 
`public  `[`abs`](#d8/d81/mcdata_8hpp_1afb4ffb64bebc6171205abfe943bf223f)`(cosh(rhs.mean()) *rhs.error())`            | 
`public  `[`abs`](#d8/d81/mcdata_8hpp_1ad6e72bfb08bcc43fc337bc66acd8e627)`(sinh(rhs.mean()) *rhs.error())`            | 
`public  `[`abs`](#d8/d81/mcdata_8hpp_1acc80dfc9a25fa67eed0aa3b6934bdd75)`(1./)`            | 
`public  `[`abs`](#d8/d81/mcdata_8hpp_1a54294452a36d2acaad81a18808428568)`(1./ sqrt)`            | 
`public  `[`abs`](#d8/d81/mcdata_8hpp_1a51636288901205ed3435fd3058b59fff)`(-1./ sqrt)`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1aaa43dabab611d9b5afdcd6e2fd0c2ea6)`(atan,abs(1./(1.+rhs.mean() *rhs.mean()) *rhs.error()))`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a2f5bdffba76098eb487290f51b910aee)`(abs,rhs. error)`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a5d38d9db2522e8c8d84311c88090eb57)`(sq,abs(2. *rhs.mean() *rhs.error()))`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a1cbb09b9a850c47ff7ad23261e878ba8)`(cb,abs(3. *sq(rhs.mean()) *rhs.error()))`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a65c382422725c25cf8d0fc1f12dc49a1)`(sqrt,abs(rhs.error()/(2. *sqrt(rhs.mean()))))`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a30dd009d0cc551769f416eaa940e5174)`(cbrt,abs(rhs.error()/(3. *sq(pow(rhs.mean(), 1./3)))))`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a4209ad8762c51ee7d2c5726f84ce0a5d)`(exp,exp(rhs.mean()) *rhs.error())`            | 
`public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1ac7eeaaa9d4814ad3c4739a89ac69ab6b)`(log,abs(rhs.error()/rhs.mean()))`            | 
`public template<>`  <br/>`std::ostream & `[`operator<<`](#d0/d14/value__with__error_8hpp_1a4d6be82a61fef36abc696ae08d7216af)`(std::ostream & out,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > const & value)`            | 
`public template<>`  <br/>`std::ostream & `[`operator<<`](#d0/d14/value__with__error_8hpp_1aee7b18daf89d01e308181369a44cfd34)`(std::ostream & out,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< std::vector< T > > const & vec)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > & `[`operator+`](#d0/d14/value__with__error_8hpp_1ac45a13c7d7fdd31c7a35f55d78321aa5)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > & rhs)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator-`](#d0/d14/value__with__error_8hpp_1a2386ea8fd9bdf478ce41e9070622cc4a)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`abs`](#d0/d14/value__with__error_8hpp_1a9393a22b6731c1e06cc78fb7495e6577)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator+`](#d0/d14/value__with__error_8hpp_1aea007cdb662f7a7fd09425f64078b070)`(T const & lhs,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator-`](#d0/d14/value__with__error_8hpp_1a38056f733181c5440d227dd8902d95da)`(T const & lhs,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator*`](#d0/d14/value__with__error_8hpp_1ae72f744e95b2d8af7eead9b09937b99b)`(T const & lhs,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator/`](#d0/d14/value__with__error_8hpp_1aefc61346184d44680bc2c31c5aa6df12)`(T const & lhs,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > const & rhs)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`pow`](#d0/d14/value__with__error_8hpp_1aaed0244f40bdbe3c1c8082c65db6de62)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs,typename `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T >::element_type const & exponent)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`sq`](#d0/d14/value__with__error_8hpp_1af190e116c2b82d01d1cf5b55f33e85dd)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`cb`](#d0/d14/value__with__error_8hpp_1aacbd560c4e79f197c0e0836da4148c71)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`sqrt`](#d0/d14/value__with__error_8hpp_1a1eacc9d21036c3f9769d3f0b56719296)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`cbrt`](#d0/d14/value__with__error_8hpp_1a4b3f7992881085e1ca51d191844bf9aa)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`exp`](#d0/d14/value__with__error_8hpp_1a903529161079ac228b0e6626cb47ec61)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`log`](#d0/d14/value__with__error_8hpp_1ae1c536e373095aff322ef450c039cbe2)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`sin`](#d0/d14/value__with__error_8hpp_1aed5ae88fdb8cd8081c128016d8508d85)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`cos`](#d0/d14/value__with__error_8hpp_1aff6aae2d1d20340703bcd07c2fb58ea5)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`tan`](#d0/d14/value__with__error_8hpp_1aa72a42c481b90893ad0a86c532799a8b)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`sinh`](#d0/d14/value__with__error_8hpp_1addf70f6193821485e6e91b950b10863c)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`cosh`](#d0/d14/value__with__error_8hpp_1a87bf75ab0922449daf54367c5cfc653b)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`tanh`](#d0/d14/value__with__error_8hpp_1ae26d619bc35f080149012c1f813a27ea)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`asin`](#d0/d14/value__with__error_8hpp_1a7e87df1c81fdf4c0188d56d8fc816cf9)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`acos`](#d0/d14/value__with__error_8hpp_1a156a880da66aa3eae587cf2cc0cac5b9)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`atan`](#d0/d14/value__with__error_8hpp_1a29c1eace86c1440b00b9c59c4b19615d)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`asinh`](#d0/d14/value__with__error_8hpp_1a0300b190232b4dd55781ca6138ef2623)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`acosh`](#d0/d14/value__with__error_8hpp_1a7abae77838bea9ae697f9a35c690f3af)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`atanh`](#d0/d14/value__with__error_8hpp_1a08a7a142172e40a23d2c26d484569298)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1adb50c0910ac80a43fbfef12e7cb3c93f)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1a9d39eaa70d028d082edb2c8c836fdf88)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,T const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1adf39cd4c56e79300fdbb4f505cb3b936)`(T const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1abd1a1922df43f9e2dcad0d8291e31877)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< T > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1a8376bd48372f409c0133537cd5f85d30)`(std::vector< T > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a00eaca4f7953d457451ba24a37f0f85d)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a0d8388dbb40aaf89658e45f5390eea51)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,T const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a4434e5a5a842e138e10ba74f520f7a81)`(T const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a46eda068fdacbf3f018865ee798273f9)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< T > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a76b0a4e435d4eefd33d16f60e2ac7fe4)`(std::vector< T > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1a82fa8ac877850eb32daf9ee43a1a3556)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1a3a1d75f0b2d0ff57c60d1698d1af1e88)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,T const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1af009c67d978d84556b378aebb2d93a42)`(T const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1a5c6e179875b2d3be2e79d2513cd43c5b)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< T > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1ad3522eaf950ac95d33d529f972b50d19)`(std::vector< T > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1a4a7f3072e0b80669219072a5cbb300f2)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1ae46db4604e25900b5fac0749ba79dc34)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,T const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1a60d5325ea105b05f7fbc6749a26e4826)`(T const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1a0cdc833bdcb72c126ea36d5189f503e3)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< T > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1a8af52c25dc4f88c5e4e27054aaa93959)`(std::vector< T > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)`            | 
`public template<>`  <br/>`inline std::vector< T > `[`operator-`](#d0/d14/value__with__error_8hpp_1af0c97007088c052947aa2275b4d2e08f)`(std::vector< T > const & rhs)`            | 
`public template<>`  <br/>`inline static std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`vec_pow`](#d0/d14/value__with__error_8hpp_1adb269ffbae6b3c9453a7f923e1c19703)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs,T const & exponent)`            | 
`public template<>`  <br/>`std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`obtain_vector_of_value_with_error_from_vector_with_error`](#d0/d14/value__with__error_8hpp_1a10b5a3485c22f5616d724bb913791209)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< std::vector< T > > vec_with_error)`            | 
`public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< std::vector< T > > `[`obtain_vector_with_error_from_vector_of_value_with_error`](#d0/d14/value__with__error_8hpp_1a6deafb122ff35f74f98277f528f28393)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > vec_of_value_with_error)`            | 
`class `[`alps::alea::mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata) | 
`class `[`alps::alea::mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries) | 
`class `[`alps::alea::mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view) | 
`class `[`alps::alea::None_class`](#d8/de2/classalps_1_1alea_1_1_none__class) | 
`class `[`alps::alea::NotEnoughMeasurementsError`](#df/d48/classalps_1_1alea_1_1_not_enough_measurements_error) | 
`class `[`alps::alea::value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error) | 
`struct `[`alps::alea::binning_selector`](#db/d1d/structalps_1_1alea_1_1binning__selector) | 
`struct `[`alps::alea::const_iterator_type`](#d6/dd3/structalps_1_1alea_1_1const__iterator__type) | 
`struct `[`alps::alea::const_iterator_type< alps::alea::mcdata< ValueType > >`](#db/dfc/structalps_1_1alea_1_1const__iterator__type_3_01alps_1_1alea_1_1mcdata_3_01_value_type_01_4_01_4) | 
`struct `[`alps::alea::iterator_type`](#d3/d45/structalps_1_1alea_1_1iterator__type) | 
`struct `[`alps::alea::iterator_type< alps::alea::mcdata< ValueType > >`](#df/d7e/structalps_1_1alea_1_1iterator__type_3_01alps_1_1alea_1_1mcdata_3_01_value_type_01_4_01_4) | 
`struct `[`alps::alea::uncorrelated_selector`](#d1/db1/structalps_1_1alea_1_1uncorrelated__selector) | 

## Members

#### `public template<>`  <br/>[`const_iterator_type`](#d6/dd3/structalps_1_1alea_1_1const__iterator__type)`< TimeseriesType >::type `[`range_begin`](#df/d51/mcanalyze_8hpp_1a9a1a236f9423fb0b430e2b2ef3c0e87a)`(const TimeseriesType & timeseries)` 

#### `public template<>`  <br/>`std::vector< ValueType >::const_iterator `[`range_begin`](#df/d51/mcanalyze_8hpp_1a447b63a38b841f16b2908a5288078cda)`(const `[`alps::alea::mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< ValueType > & timeseries)` 

#### `public template<>`  <br/>[`const_iterator_type`](#d6/dd3/structalps_1_1alea_1_1const__iterator__type)`< TimeseriesType >::type `[`range_end`](#df/d51/mcanalyze_8hpp_1a97ab74696ed7a3ee0d037e317a38bc43)`(const TimeseriesType & timeseries)` 

#### `public template<>`  <br/>`std::vector< ValueType >::const_iterator `[`range_end`](#df/d51/mcanalyze_8hpp_1ac00249394583311cfd606791eddad4bb)`(const `[`alps::alea::mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< ValueType > & timeseries)` 

#### `public template<>`  <br/>[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< typename TimeseriesType::value_type > `[`cut_head_distance`](#df/d51/mcanalyze_8hpp_1abd691553fcb5ff786da40c07c08e84dc)`(const TimeseriesType & timeseries,int cutoff)` 

#### `public template<>`  <br/>[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< typename TimeseriesType::value_type > `[`cut_tail_distance`](#df/d51/mcanalyze_8hpp_1a39b3b8d12f39e5a45558dc1b4c1d565f)`(const TimeseriesType & timeseries,int cutoff)` 

#### `public template<>`  <br/>[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< typename TimeseriesType::value_type > `[`cut_head_limit`](#df/d51/mcanalyze_8hpp_1a9cb396f162af3de2960020d759deb98b)`(const TimeseriesType & timeseries,double limit)` 

#### `public template<>`  <br/>[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< typename TimeseriesType::value_type > `[`cut_tail_limit`](#df/d51/mcanalyze_8hpp_1ab86261ab4c4b6c9ff1131cf883fc2eb6)`(const TimeseriesType & timeseries,double limit)` 

#### `public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`mean`](#df/d51/mcanalyze_8hpp_1a147856cf8919d2c5e24196d86a6280cf)`(const TimeseriesType & timeseries)` 

#### `public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`variance`](#df/d51/mcanalyze_8hpp_1ab29bc15f9a9168f6df36aedfc72bf287)`(const TimeseriesType & timeseries)` 

#### `public template<>`  <br/>[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< typename average_type< typename TimeseriesType::value_type >::type > `[`autocorrelation_distance`](#df/d51/mcanalyze_8hpp_1aba91006861f71ae72fff7f19f420f003)`(const TimeseriesType & timeseries,int up_to)` 

#### `public template<>`  <br/>[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< typename average_type< typename TimeseriesType::value_type >::type > `[`autocorrelation_limit`](#df/d51/mcanalyze_8hpp_1a67786e8d84cdd70e185e66dc8ef6a5b3)`(const TimeseriesType & timeseries,double limit)` 

#### `public template<>`  <br/>`std::pair< typename average_type< typename TimeseriesType::value_type >::type, typename average_type< typename TimeseriesType::value_type >::type > `[`exponential_autocorrelation_time_distance`](#df/d51/mcanalyze_8hpp_1a1d4692bf22af0eb6e6a578366d13b59e)`(const TimeseriesType & autocorrelation,int from,int to)` 

#### `public template<>`  <br/>`std::pair< typename average_type< typename TimeseriesType::value_type >::type, typename average_type< typename TimeseriesType::value_type >::type > `[`exponential_autocorrelation_time_limit`](#df/d51/mcanalyze_8hpp_1a1b51c7a7ab0c6bc3f767583f5445026a)`(const TimeseriesType & autocorrelation,double max,double min)` 

#### `public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`integrated_autocorrelation_time`](#df/d51/mcanalyze_8hpp_1a93b39244179cbf0a42b97149bb924104)`(const TimeseriesType & autocorrelation,const std::pair< typename average_type< typename TimeseriesType::value_type >::type, typename average_type< typename TimeseriesType::value_type >::type > & tau)` 

#### `public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`error`](#df/d51/mcanalyze_8hpp_1ac84c44931f6df3f8a68a4b6ab32a8f6b)`(const TimeseriesType & timeseries,const `[`uncorrelated_selector`](#d1/db1/structalps_1_1alea_1_1uncorrelated__selector)` & selector)` 

#### `public template<>`  <br/>`average_type< typenameTimeseriesType::value_type >::type `[`error`](#df/d51/mcanalyze_8hpp_1aaaa701d6e01e269bdf54d0fc11d42ad9)`(const TimeseriesType & timeseries,const `[`binning_selector`](#db/d1d/structalps_1_1alea_1_1binning__selector)` & selector)` 

#### `public template<>`  <br/>`inline average_type< typenameTimeseriesType::value_type >::type `[`uncorrelated_error`](#df/d51/mcanalyze_8hpp_1aff871e63952b8b3696afe83eca2b9096)`(const TimeseriesType & timeseries)` 

#### `public template<>`  <br/>`inline average_type< typenameTimeseriesType::value_type >::type `[`binning_error`](#df/d51/mcanalyze_8hpp_1af3bdb959edd8395d589f2ff9799ceff7)`(const TimeseriesType & timeseries)` 

#### `public template<>`  <br/>[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< typename average_type< typename TimeseriesType::value_type >::type > `[`running_mean`](#df/d51/mcanalyze_8hpp_1a3237d010efb8a46566bc29c48365ec0d)`(const TimeseriesType & timeseries)` 

#### `public template<>`  <br/>[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< typename average_type< typename TimeseriesType::value_type >::type > `[`reverse_running_mean`](#df/d51/mcanalyze_8hpp_1aa774554bb5491f0c7995a04fce02123f)`(const TimeseriesType & timeseries)` 

#### `public template<>`  <br/>`inline std::ostream & `[`operator<<`](#d8/d81/mcdata_8hpp_1a0f4b2305701d014bf4bff0f0674caf9b)`(std::ostream & out,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & obs)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`operator+`](#d8/d81/mcdata_8hpp_1a03dca1afd93bd34a5705e266059de68e)`(T const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`operator-`](#d8/d81/mcdata_8hpp_1adc8992c62941dc928c72e62338b37070)`(T const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`operator*`](#d8/d81/mcdata_8hpp_1acc8b32bf8c54d821c34c568572231a91)`(T const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`operator/`](#d8/d81/mcdata_8hpp_1a3311188edd9a927316a719d045dbb770)`(T const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator+`](#d8/d81/mcdata_8hpp_1a8e7502812529d8260b3fb59e5e6e7445)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator+`](#d8/d81/mcdata_8hpp_1aac9f24ad3531df25f736f37bc0ae9a39)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator-`](#d8/d81/mcdata_8hpp_1aa5052a8472301492645577c17654e6bc)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator-`](#d8/d81/mcdata_8hpp_1a1578d7c90537102a3aabb948a5b32ce8)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator*`](#d8/d81/mcdata_8hpp_1ab2f09e4725cf74fdf0cf6f39cda70007)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator*`](#d8/d81/mcdata_8hpp_1a7f86409880e6c4905a120b1957819941)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator/`](#d8/d81/mcdata_8hpp_1ad5ed9bf1d3196edd1cfdf7374064f63f)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg2)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > `[`operator/`](#d8/d81/mcdata_8hpp_1a3ea5189c649b3ede76f65bc5beb0cb83)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & arg1,`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< T > > arg2)` 

#### `public template<>`  <br/>[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > `[`pow`](#d8/d81/mcdata_8hpp_1a1a60702d2252b8d65523bc523de5db87)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > rhs,typename `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T >::recursive_element_type exponent)` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a67a6cc083195ce6f2bfc13c0be6fc00c)`(sin,abs(cos(rhs.mean()) *rhs.error()))` 

#### `public  `[`abs`](#d8/d81/mcdata_8hpp_1aab0577c994c1599a36c038a55f276d35)`(- sin)` 

#### `public  `[`abs`](#d8/d81/mcdata_8hpp_1a6c01f91f0088ade9ff5c8aaf58e34419)`(1./)` 

#### `public  `[`abs`](#d8/d81/mcdata_8hpp_1afb4ffb64bebc6171205abfe943bf223f)`(cosh(rhs.mean()) *rhs.error())` 

#### `public  `[`abs`](#d8/d81/mcdata_8hpp_1ad6e72bfb08bcc43fc337bc66acd8e627)`(sinh(rhs.mean()) *rhs.error())` 

#### `public  `[`abs`](#d8/d81/mcdata_8hpp_1acc80dfc9a25fa67eed0aa3b6934bdd75)`(1./)` 

#### `public  `[`abs`](#d8/d81/mcdata_8hpp_1a54294452a36d2acaad81a18808428568)`(1./ sqrt)` 

#### `public  `[`abs`](#d8/d81/mcdata_8hpp_1a51636288901205ed3435fd3058b59fff)`(-1./ sqrt)` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1aaa43dabab611d9b5afdcd6e2fd0c2ea6)`(atan,abs(1./(1.+rhs.mean() *rhs.mean()) *rhs.error()))` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a2f5bdffba76098eb487290f51b910aee)`(abs,rhs. error)` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a5d38d9db2522e8c8d84311c88090eb57)`(sq,abs(2. *rhs.mean() *rhs.error()))` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a1cbb09b9a850c47ff7ad23261e878ba8)`(cb,abs(3. *sq(rhs.mean()) *rhs.error()))` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a65c382422725c25cf8d0fc1f12dc49a1)`(sqrt,abs(rhs.error()/(2. *sqrt(rhs.mean()))))` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a30dd009d0cc551769f416eaa940e5174)`(cbrt,abs(rhs.error()/(3. *sq(pow(rhs.mean(), 1./3)))))` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1a4209ad8762c51ee7d2c5726f84ce0a5d)`(exp,exp(rhs.mean()) *rhs.error())` 

#### `public  `[`ALPS_ALEA_MCDATA_IMPLEMENT_FUNCTION`](#d8/d81/mcdata_8hpp_1ac7eeaaa9d4814ad3c4739a89ac69ab6b)`(log,abs(rhs.error()/rhs.mean()))` 

#### `public template<>`  <br/>`std::ostream & `[`operator<<`](#d0/d14/value__with__error_8hpp_1a4d6be82a61fef36abc696ae08d7216af)`(std::ostream & out,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > const & value)` 

#### `public template<>`  <br/>`std::ostream & `[`operator<<`](#d0/d14/value__with__error_8hpp_1aee7b18daf89d01e308181369a44cfd34)`(std::ostream & out,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< std::vector< T > > const & vec)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > & `[`operator+`](#d0/d14/value__with__error_8hpp_1ac45a13c7d7fdd31c7a35f55d78321aa5)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > & rhs)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator-`](#d0/d14/value__with__error_8hpp_1a2386ea8fd9bdf478ce41e9070622cc4a)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`abs`](#d0/d14/value__with__error_8hpp_1a9393a22b6731c1e06cc78fb7495e6577)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator+`](#d0/d14/value__with__error_8hpp_1aea007cdb662f7a7fd09425f64078b070)`(T const & lhs,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator-`](#d0/d14/value__with__error_8hpp_1a38056f733181c5440d227dd8902d95da)`(T const & lhs,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator*`](#d0/d14/value__with__error_8hpp_1ae72f744e95b2d8af7eead9b09937b99b)`(T const & lhs,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`operator/`](#d0/d14/value__with__error_8hpp_1aefc61346184d44680bc2c31c5aa6df12)`(T const & lhs,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > const & rhs)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`pow`](#d0/d14/value__with__error_8hpp_1aaed0244f40bdbe3c1c8082c65db6de62)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs,typename `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T >::element_type const & exponent)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`sq`](#d0/d14/value__with__error_8hpp_1af190e116c2b82d01d1cf5b55f33e85dd)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`cb`](#d0/d14/value__with__error_8hpp_1aacbd560c4e79f197c0e0836da4148c71)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`sqrt`](#d0/d14/value__with__error_8hpp_1a1eacc9d21036c3f9769d3f0b56719296)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`cbrt`](#d0/d14/value__with__error_8hpp_1a4b3f7992881085e1ca51d191844bf9aa)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`exp`](#d0/d14/value__with__error_8hpp_1a903529161079ac228b0e6626cb47ec61)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`log`](#d0/d14/value__with__error_8hpp_1ae1c536e373095aff322ef450c039cbe2)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>`inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`sin`](#d0/d14/value__with__error_8hpp_1aed5ae88fdb8cd8081c128016d8508d85)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`cos`](#d0/d14/value__with__error_8hpp_1aff6aae2d1d20340703bcd07c2fb58ea5)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`tan`](#d0/d14/value__with__error_8hpp_1aa72a42c481b90893ad0a86c532799a8b)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`sinh`](#d0/d14/value__with__error_8hpp_1addf70f6193821485e6e91b950b10863c)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`cosh`](#d0/d14/value__with__error_8hpp_1a87bf75ab0922449daf54367c5cfc653b)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`tanh`](#d0/d14/value__with__error_8hpp_1ae26d619bc35f080149012c1f813a27ea)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`asin`](#d0/d14/value__with__error_8hpp_1a7e87df1c81fdf4c0188d56d8fc816cf9)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`acos`](#d0/d14/value__with__error_8hpp_1a156a880da66aa3eae587cf2cc0cac5b9)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`atan`](#d0/d14/value__with__error_8hpp_1a29c1eace86c1440b00b9c59c4b19615d)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`asinh`](#d0/d14/value__with__error_8hpp_1a0300b190232b4dd55781ca6138ef2623)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`acosh`](#d0/d14/value__with__error_8hpp_1a7abae77838bea9ae697f9a35c690f3af)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > `[`atanh`](#d0/d14/value__with__error_8hpp_1a08a7a142172e40a23d2c26d484569298)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1adb50c0910ac80a43fbfef12e7cb3c93f)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1a9d39eaa70d028d082edb2c8c836fdf88)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,T const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1adf39cd4c56e79300fdbb4f505cb3b936)`(T const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1abd1a1922df43f9e2dcad0d8291e31877)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< T > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator+`](#d0/d14/value__with__error_8hpp_1a8376bd48372f409c0133537cd5f85d30)`(std::vector< T > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a00eaca4f7953d457451ba24a37f0f85d)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a0d8388dbb40aaf89658e45f5390eea51)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,T const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a4434e5a5a842e138e10ba74f520f7a81)`(T const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a46eda068fdacbf3f018865ee798273f9)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< T > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator-`](#d0/d14/value__with__error_8hpp_1a76b0a4e435d4eefd33d16f60e2ac7fe4)`(std::vector< T > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1a82fa8ac877850eb32daf9ee43a1a3556)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1a3a1d75f0b2d0ff57c60d1698d1af1e88)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,T const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1af009c67d978d84556b378aebb2d93a42)`(T const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1a5c6e179875b2d3be2e79d2513cd43c5b)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< T > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator*`](#d0/d14/value__with__error_8hpp_1ad3522eaf950ac95d33d529f972b50d19)`(std::vector< T > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1a4a7f3072e0b80669219072a5cbb300f2)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1ae46db4604e25900b5fac0749ba79dc34)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,T const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1a60d5325ea105b05f7fbc6749a26e4826)`(T const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1a0cdc833bdcb72c126ea36d5189f503e3)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & lhs,std::vector< T > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`operator/`](#d0/d14/value__with__error_8hpp_1a8af52c25dc4f88c5e4e27054aaa93959)`(std::vector< T > const & lhs,std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs)` 

#### `public template<>`  <br/>`inline std::vector< T > `[`operator-`](#d0/d14/value__with__error_8hpp_1af0c97007088c052947aa2275b4d2e08f)`(std::vector< T > const & rhs)` 

#### `public template<>`  <br/>`inline static std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`vec_pow`](#d0/d14/value__with__error_8hpp_1adb269ffbae6b3c9453a7f923e1c19703)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > const & rhs,T const & exponent)` 

#### `public template<>`  <br/>`std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > `[`obtain_vector_of_value_with_error_from_vector_with_error`](#d0/d14/value__with__error_8hpp_1a10b5a3485c22f5616d724bb913791209)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< std::vector< T > > vec_with_error)` 

#### `public template<>`  <br/>[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< std::vector< T > > `[`obtain_vector_with_error_from_vector_of_value_with_error`](#d0/d14/value__with__error_8hpp_1a6deafb122ff35f74f98277f528f28393)`(std::vector< `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< T > > vec_of_value_with_error)` 

# class `alps::alea::mcdata` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1ab68db48554787cdd17283af5a26ed3dd)`()` | 
`public inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8a8dbb5f5d88d8e6681c21eba110e402)`(result_type mean,result_type error)` | 
`public inline std::size_t `[`size`](#d9/d76/classalps_1_1alea_1_1mcdata_1a2d42339e979b012ba3f9907dc2a69b93)`() const` | 
`public template<>`  <br/>`inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1ae7f17fbc1c7ca771ebdc9598ab5d8f6f)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs,S s)` | 
`public template<>`  <br/>`inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac9b9066865c5a9d11454bf446c391db6)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs,S from,S to)` | 
`public template<>`  <br/>`inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1aa94d0598e685dd9cecc7a4a2aed8c835)`(`[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable)`< X > const & obs)` | 
`public inline `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` `[`begin`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8dd69d0f3e1858c257e58a3aec419fc4)`() const` | 
`public inline `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` `[`end`](#d9/d76/classalps_1_1alea_1_1mcdata_1aa0648b57198696a41d4d22d41e5713f4)`() const` | 
`public inline bool `[`can_rebin`](#d9/d76/classalps_1_1alea_1_1mcdata_1a67b7802f27e37bcf2025a0527f70ec4c)`() const` | 
`public inline bool `[`jackknife_valid`](#d9/d76/classalps_1_1alea_1_1mcdata_1af2d0262f2ebd92926244f11b4c156f23)`() const` | 
`public inline void `[`swap`](#d9/d76/classalps_1_1alea_1_1mcdata_1a1ed27c7117eb810bb6989ba4fd842fc4)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & rhs)` | 
`public inline uint64_t `[`count`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8dd4cf931cabf9a2406df657ca75e613)`() const` | 
`public inline uint64_t `[`bin_size`](#d9/d76/classalps_1_1alea_1_1mcdata_1a958da526fe62a9387c0895284a6e2586)`() const` | 
`public inline uint64_t `[`max_bin_number`](#d9/d76/classalps_1_1alea_1_1mcdata_1a56e59ce914edf0763e2e038f924ec531)`() const` | 
`public inline std::size_t `[`bin_number`](#d9/d76/classalps_1_1alea_1_1mcdata_1a6721fc1d767198fa9e02e8bb246f0085)`() const` | 
`public inline std::vector< value_type > const & `[`bins`](#d9/d76/classalps_1_1alea_1_1mcdata_1a3bda4aaa08eb58d93654e64f9fd9e268)`() const` | 
`public inline std::vector< result_type > const & `[`jackknife`](#d9/d76/classalps_1_1alea_1_1mcdata_1ab8bc511a7e85173daa68eac57b56d531)`() const` | 
`public inline result_type const & `[`mean`](#d9/d76/classalps_1_1alea_1_1mcdata_1a18a242273eb836aed399cfef62c3cf71)`() const` | 
`public inline result_type const & `[`error`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac15d85ebf6150b68952f901abcac9911)`() const` | 
`public inline bool `[`has_variance`](#d9/d76/classalps_1_1alea_1_1mcdata_1a4fe3cfab1108dbbd1cf6a4aed56dc2d6)`() const` | 
`public inline result_type const & `[`variance`](#d9/d76/classalps_1_1alea_1_1mcdata_1a511435e701b8bd1f9f749143c0af4823)`() const` | 
`public inline bool `[`has_tau`](#d9/d76/classalps_1_1alea_1_1mcdata_1a0337ec97659391af93cf1ffa898472d3)`() const` | 
`public inline time_type const & `[`tau`](#d9/d76/classalps_1_1alea_1_1mcdata_1a549ba5f44450b428b4fef71c436485c2)`() const` | 
`public inline covariance_type `[`covariance`](#d9/d76/classalps_1_1alea_1_1mcdata_1a86edccf255959af487d57421b9a23c20)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & obs) const` | 
`public inline covariance_type `[`accurate_covariance`](#d9/d76/classalps_1_1alea_1_1mcdata_1a368bceb11eaddabee5d1c7d9062fe247)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & obs) const` | 
`public inline void `[`set_bin_size`](#d9/d76/classalps_1_1alea_1_1mcdata_1a6fe53f1d234f189c482b53501aea5c30)`(uint64_t binsize)` | 
`public inline void `[`set_bin_number`](#d9/d76/classalps_1_1alea_1_1mcdata_1a36e28ad570cd3b495779fe7a5e0b860f)`(uint64_t bin_number)` | 
`public inline void `[`discard_bins`](#d9/d76/classalps_1_1alea_1_1mcdata_1a07cf836a63d966e6525ae62ea408da79)`(size_type keep_bins)` | 
`public inline void `[`output`](#d9/d76/classalps_1_1alea_1_1mcdata_1ae0fa97c1aaf9b1581f4af48ec849aa62)`(std::ostream & out) const` | 
`public inline void `[`save`](#d9/d76/classalps_1_1alea_1_1mcdata_1a384a0f66143224fb37bf445f5d29a1a8)`(hdf5::archive & ar) const` | 
`public inline void `[`load`](#d9/d76/classalps_1_1alea_1_1mcdata_1a467e6ef43cc3d967ccdbcdfeae82c01d)`(hdf5::archive & ar)` | 
`public inline void `[`save`](#d9/d76/classalps_1_1alea_1_1mcdata_1a65c85e684a753d9a03f32c8a491afe98)`(std::string const & filename,std::string const & path) const` | 
`public inline void `[`load`](#d9/d76/classalps_1_1alea_1_1mcdata_1a286d9fa410a422040a65117a6677d771)`(std::string const & filename,std::string const & path)` | 
`public inline void `[`merge`](#d9/d76/classalps_1_1alea_1_1mcdata_1af54ea33cccd55bd9bc9ac3a2c6932274)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & rhs)` | 
`public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator<<`](#d9/d76/classalps_1_1alea_1_1mcdata_1a928d4fecc04a04c9bfe206a8b67d2ff2)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & rhs)` | 
`public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator=`](#d9/d76/classalps_1_1alea_1_1mcdata_1af55899c2e32723d6e2adae749da0a3e7)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > rhs)` | 
`public template<>`  <br/>`inline element_type `[`slice`](#d9/d76/classalps_1_1alea_1_1mcdata_1accb9805570b6b8829461052e3d506f25)`(S s) const` | 
`public template<>`  <br/>`inline bool `[`operator==`](#d9/d76/classalps_1_1alea_1_1mcdata_1af9002a048c37dd7fc001e63e35dd792e)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs) const` | 
`public template<>`  <br/>`inline bool `[`operator==`](#d9/d76/classalps_1_1alea_1_1mcdata_1a5b76b7535a91e19f97166905f0fcc757)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< X > > const & rhs) const` | 
`public template<>`  <br/>`inline bool `[`operator!=`](#d9/d76/classalps_1_1alea_1_1mcdata_1abccef1d598cd76e0ca76db514dd5f6fa)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs) const` | 
`public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator+=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a85319efbda55f38c17cc703b32b663ca)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & rhs)` | 
`public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator-=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a9f43f1df948f524ad7a4230ae55f5b14)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & rhs)` | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator*=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a5c989de280e5e1166985c973bbe275a3)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs)` | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator/=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8b0db68ee347124524ec9863c1ec66a2)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs)` | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator+=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a1ddc0b5aa62552df36d1aed7fc6ffded)`(X const & rhs)` | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator-=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a980771be008768dd9f0eec231f44b1fe)`(X const & rhs)` | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator*=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a897ac36575090836132e3991f13fb689)`(X const & rhs)` | 
`public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator/=`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac2ceedc33213b2cc886b814b79b2e2aa)`(X const & rhs)` | 
`public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator+`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8a841c10a98d7a6495098289fc90c739)`()` | 
`public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator-`](#d9/d76/classalps_1_1alea_1_1mcdata_1af6b0bc13b8a057f3453da944ead85418)`()` | 
`public template<>`  <br/>`inline void `[`subtract_from`](#d9/d76/classalps_1_1alea_1_1mcdata_1a5a39a616f0d8d3c745fc759834a7ce9d)`(X const & x)` | 
`public template<>`  <br/>`inline void `[`divide`](#d9/d76/classalps_1_1alea_1_1mcdata_1a7b4c18eea4a5ae03aa1c0693facd7de2)`(X const & x)` | 
`public template<>`  <br/>`inline void `[`transform_linear`](#d9/d76/classalps_1_1alea_1_1mcdata_1a265be05d069f285f4e7dc68273361d64)`(OP op,value_type const & error,boost::optional< result_type > variance_opt)` | 
`public template<>`  <br/>`inline void `[`transform`](#d9/d76/classalps_1_1alea_1_1mcdata_1aeff5d883e59aecc5487832aa1314e095)`(OP op,value_type const & error,boost::optional< result_type > variance_opt)` | 
`public template<>`  <br/>`inline void `[`transform`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac29de8f31a2b176964e3b4c4a001f13c)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs,OP op,value_type const & error,boost::optional< result_type > variance_opt)` | 
`protected inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1a9a52c33a733043ec0b2792cfa935e3ea)`(int64_t count,value_type const & mean,value_type const & error,boost::optional< result_type > const & variance_opt,boost::optional< time_type > const & tau_opt,uint64_t binsize,uint64_t max_bin_number,std::vector< value_type > const & values)` | 
`typedef `[`value_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac391e9aa9fbe39f6d0a265963e34c630) | 
`typedef `[`recursive_element_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a0c6d99ab7ec3193183d84baa2dec3081) | 
`typedef `[`element_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a5f5cdfe34404e55b7ddb3e13806f3604) | 
`typedef `[`time_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a7714fa62c017f35382d72fe996e16335) | 
`typedef `[`size_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a132171539373b6285d265b749d2086cd) | 
`typedef `[`count_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a3fd1ae499f68ea0ca8ac2fd2795c9a76) | 
`typedef `[`result_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a94b85e5eae00808011c7769ad189271a) | 
`typedef `[`convergence_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a26382e87cefb33e266ee4565c9f25a69) | 
`typedef `[`covariance_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a3dcd2411c4b9b035f3e99161914ae172) | 

## Members

#### `public inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1ab68db48554787cdd17283af5a26ed3dd)`()` 

#### `public inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8a8dbb5f5d88d8e6681c21eba110e402)`(result_type mean,result_type error)` 

#### `public inline std::size_t `[`size`](#d9/d76/classalps_1_1alea_1_1mcdata_1a2d42339e979b012ba3f9907dc2a69b93)`() const` 

#### `public template<>`  <br/>`inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1ae7f17fbc1c7ca771ebdc9598ab5d8f6f)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs,S s)` 

#### `public template<>`  <br/>`inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac9b9066865c5a9d11454bf446c391db6)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs,S from,S to)` 

#### `public template<>`  <br/>`inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1aa94d0598e685dd9cecc7a4a2aed8c835)`(`[`AbstractSimpleObservable`](#df/d12/classalps_1_1_abstract_simple_observable)`< X > const & obs)` 

#### `public inline `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` `[`begin`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8dd69d0f3e1858c257e58a3aec419fc4)`() const` 

#### `public inline `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` `[`end`](#d9/d76/classalps_1_1alea_1_1mcdata_1aa0648b57198696a41d4d22d41e5713f4)`() const` 

#### `public inline bool `[`can_rebin`](#d9/d76/classalps_1_1alea_1_1mcdata_1a67b7802f27e37bcf2025a0527f70ec4c)`() const` 

#### `public inline bool `[`jackknife_valid`](#d9/d76/classalps_1_1alea_1_1mcdata_1af2d0262f2ebd92926244f11b4c156f23)`() const` 

#### `public inline void `[`swap`](#d9/d76/classalps_1_1alea_1_1mcdata_1a1ed27c7117eb810bb6989ba4fd842fc4)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & rhs)` 

#### `public inline uint64_t `[`count`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8dd4cf931cabf9a2406df657ca75e613)`() const` 

#### `public inline uint64_t `[`bin_size`](#d9/d76/classalps_1_1alea_1_1mcdata_1a958da526fe62a9387c0895284a6e2586)`() const` 

#### `public inline uint64_t `[`max_bin_number`](#d9/d76/classalps_1_1alea_1_1mcdata_1a56e59ce914edf0763e2e038f924ec531)`() const` 

#### `public inline std::size_t `[`bin_number`](#d9/d76/classalps_1_1alea_1_1mcdata_1a6721fc1d767198fa9e02e8bb246f0085)`() const` 

#### `public inline std::vector< value_type > const & `[`bins`](#d9/d76/classalps_1_1alea_1_1mcdata_1a3bda4aaa08eb58d93654e64f9fd9e268)`() const` 

#### `public inline std::vector< result_type > const & `[`jackknife`](#d9/d76/classalps_1_1alea_1_1mcdata_1ab8bc511a7e85173daa68eac57b56d531)`() const` 

#### `public inline result_type const & `[`mean`](#d9/d76/classalps_1_1alea_1_1mcdata_1a18a242273eb836aed399cfef62c3cf71)`() const` 

#### `public inline result_type const & `[`error`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac15d85ebf6150b68952f901abcac9911)`() const` 

#### `public inline bool `[`has_variance`](#d9/d76/classalps_1_1alea_1_1mcdata_1a4fe3cfab1108dbbd1cf6a4aed56dc2d6)`() const` 

#### `public inline result_type const & `[`variance`](#d9/d76/classalps_1_1alea_1_1mcdata_1a511435e701b8bd1f9f749143c0af4823)`() const` 

#### `public inline bool `[`has_tau`](#d9/d76/classalps_1_1alea_1_1mcdata_1a0337ec97659391af93cf1ffa898472d3)`() const` 

#### `public inline time_type const & `[`tau`](#d9/d76/classalps_1_1alea_1_1mcdata_1a549ba5f44450b428b4fef71c436485c2)`() const` 

#### `public inline covariance_type `[`covariance`](#d9/d76/classalps_1_1alea_1_1mcdata_1a86edccf255959af487d57421b9a23c20)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & obs) const` 

#### `public inline covariance_type `[`accurate_covariance`](#d9/d76/classalps_1_1alea_1_1mcdata_1a368bceb11eaddabee5d1c7d9062fe247)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & obs) const` 

#### `public inline void `[`set_bin_size`](#d9/d76/classalps_1_1alea_1_1mcdata_1a6fe53f1d234f189c482b53501aea5c30)`(uint64_t binsize)` 

#### `public inline void `[`set_bin_number`](#d9/d76/classalps_1_1alea_1_1mcdata_1a36e28ad570cd3b495779fe7a5e0b860f)`(uint64_t bin_number)` 

#### `public inline void `[`discard_bins`](#d9/d76/classalps_1_1alea_1_1mcdata_1a07cf836a63d966e6525ae62ea408da79)`(size_type keep_bins)` 

#### `public inline void `[`output`](#d9/d76/classalps_1_1alea_1_1mcdata_1ae0fa97c1aaf9b1581f4af48ec849aa62)`(std::ostream & out) const` 

#### `public inline void `[`save`](#d9/d76/classalps_1_1alea_1_1mcdata_1a384a0f66143224fb37bf445f5d29a1a8)`(hdf5::archive & ar) const` 

#### `public inline void `[`load`](#d9/d76/classalps_1_1alea_1_1mcdata_1a467e6ef43cc3d967ccdbcdfeae82c01d)`(hdf5::archive & ar)` 

#### `public inline void `[`save`](#d9/d76/classalps_1_1alea_1_1mcdata_1a65c85e684a753d9a03f32c8a491afe98)`(std::string const & filename,std::string const & path) const` 

#### `public inline void `[`load`](#d9/d76/classalps_1_1alea_1_1mcdata_1a286d9fa410a422040a65117a6677d771)`(std::string const & filename,std::string const & path)` 

#### `public inline void `[`merge`](#d9/d76/classalps_1_1alea_1_1mcdata_1af54ea33cccd55bd9bc9ac3a2c6932274)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & rhs)` 

#### `public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator<<`](#d9/d76/classalps_1_1alea_1_1mcdata_1a928d4fecc04a04c9bfe206a8b67d2ff2)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & rhs)` 

#### `public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator=`](#d9/d76/classalps_1_1alea_1_1mcdata_1af55899c2e32723d6e2adae749da0a3e7)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > rhs)` 

#### `public template<>`  <br/>`inline element_type `[`slice`](#d9/d76/classalps_1_1alea_1_1mcdata_1accb9805570b6b8829461052e3d506f25)`(S s) const` 

#### `public template<>`  <br/>`inline bool `[`operator==`](#d9/d76/classalps_1_1alea_1_1mcdata_1af9002a048c37dd7fc001e63e35dd792e)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs) const` 

#### `public template<>`  <br/>`inline bool `[`operator==`](#d9/d76/classalps_1_1alea_1_1mcdata_1a5b76b7535a91e19f97166905f0fcc757)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< std::vector< X > > const & rhs) const` 

#### `public template<>`  <br/>`inline bool `[`operator!=`](#d9/d76/classalps_1_1alea_1_1mcdata_1abccef1d598cd76e0ca76db514dd5f6fa)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs) const` 

#### `public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator+=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a85319efbda55f38c17cc703b32b663ca)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & rhs)` 

#### `public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator-=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a9f43f1df948f524ad7a4230ae55f5b14)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & rhs)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator*=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a5c989de280e5e1166985c973bbe275a3)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator/=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8b0db68ee347124524ec9863c1ec66a2)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator+=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a1ddc0b5aa62552df36d1aed7fc6ffded)`(X const & rhs)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator-=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a980771be008768dd9f0eec231f44b1fe)`(X const & rhs)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator*=`](#d9/d76/classalps_1_1alea_1_1mcdata_1a897ac36575090836132e3991f13fb689)`(X const & rhs)` 

#### `public template<>`  <br/>`inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator/=`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac2ceedc33213b2cc886b814b79b2e2aa)`(X const & rhs)` 

#### `public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator+`](#d9/d76/classalps_1_1alea_1_1mcdata_1a8a841c10a98d7a6495098289fc90c739)`()` 

#### `public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > & `[`operator-`](#d9/d76/classalps_1_1alea_1_1mcdata_1af6b0bc13b8a057f3453da944ead85418)`()` 

#### `public template<>`  <br/>`inline void `[`subtract_from`](#d9/d76/classalps_1_1alea_1_1mcdata_1a5a39a616f0d8d3c745fc759834a7ce9d)`(X const & x)` 

#### `public template<>`  <br/>`inline void `[`divide`](#d9/d76/classalps_1_1alea_1_1mcdata_1a7b4c18eea4a5ae03aa1c0693facd7de2)`(X const & x)` 

#### `public template<>`  <br/>`inline void `[`transform_linear`](#d9/d76/classalps_1_1alea_1_1mcdata_1a265be05d069f285f4e7dc68273361d64)`(OP op,value_type const & error,boost::optional< result_type > variance_opt)` 

#### `public template<>`  <br/>`inline void `[`transform`](#d9/d76/classalps_1_1alea_1_1mcdata_1aeff5d883e59aecc5487832aa1314e095)`(OP op,value_type const & error,boost::optional< result_type > variance_opt)` 

#### `public template<>`  <br/>`inline void `[`transform`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac29de8f31a2b176964e3b4c4a001f13c)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< X > const & rhs,OP op,value_type const & error,boost::optional< result_type > variance_opt)` 

#### `protected inline  `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata_1a9a52c33a733043ec0b2792cfa935e3ea)`(int64_t count,value_type const & mean,value_type const & error,boost::optional< result_type > const & variance_opt,boost::optional< time_type > const & tau_opt,uint64_t binsize,uint64_t max_bin_number,std::vector< value_type > const & values)` 

#### `typedef `[`value_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1ac391e9aa9fbe39f6d0a265963e34c630) 

#### `typedef `[`recursive_element_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a0c6d99ab7ec3193183d84baa2dec3081) 

#### `typedef `[`element_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a5f5cdfe34404e55b7ddb3e13806f3604) 

#### `typedef `[`time_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a7714fa62c017f35382d72fe996e16335) 

#### `typedef `[`size_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a132171539373b6285d265b749d2086cd) 

#### `typedef `[`count_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a3fd1ae499f68ea0ca8ac2fd2795c9a76) 

#### `typedef `[`result_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a94b85e5eae00808011c7769ad189271a) 

#### `typedef `[`convergence_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a26382e87cefb33e266ee4565c9f25a69) 

#### `typedef `[`covariance_type`](#d9/d76/classalps_1_1alea_1_1mcdata_1a3dcd2411c4b9b035f3e99161914ae172) 

# class `alps::alea::mctimeseries` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a88e059316a090ba3e772e6425cfff71a)`()` | 
`public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1ad8cf3350b64820345ccc3ba93e15eac0)`(const `[`alps::alea::mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< ValueType > & IN)` | 
`public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a42f44b0b32e6a1b81cdd93feddb74fa7)`(const `[`alps::alea::mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< ValueType > & IN)` | 
`public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1ae4ab7dd2decfc78fa399dbdbfef11e58)`(const `[`alps::alea::mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< ValueType > & IN)` | 
`public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a321183cad4fd0c0f1ee725e2bedd4feb)`(const std::vector< ValueType > & timeseries)` | 
`public inline void `[`shallow_assign`](#df/dac/classalps_1_1alea_1_1mctimeseries_1abec5550cf0d08417c07e0d970230ecf3)`(const `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< ValueType > & IN)` | 
`public inline const_iterator `[`begin`](#df/dac/classalps_1_1alea_1_1mctimeseries_1ab88df086df1774cdd7e29c1eaceefa62)`() const` | 
`public inline const_iterator `[`end`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a2a8b0fbc12c9d0e4c8cbb1f49bc236c2)`() const` | 
`public inline iterator `[`begin`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a7ce2a5ce3491077481f03d8fd9856a52)`()` | 
`public inline iterator `[`end`](#df/dac/classalps_1_1alea_1_1mctimeseries_1abfbc9e87d301e8e805c94b4abf476c6c)`()` | 
`public inline std::size_t `[`size`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a1cf5265b055555998f1b12ce8dd6e5ad)`() const` | 
`public inline void `[`push_back`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a7a5acd13fe2291aa5a96a01f07a4cab4)`(value_type IN)` | 
`public inline void `[`resize`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a64ef85ecd2aec1f0c56069a13a59429c)`(std::size_t size)` | 
`public inline std::vector< ValueType > `[`timeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a2906be7767e45f08780c809e35030b25)`() const` | 
`public inline void `[`print`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a54ff9df394571545037c5f368e7d2114)`() const` | 
`typedef `[`size_type`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a98a7ab3fb83847a9af875da7fd8dc146) | 
`typedef `[`value_type`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a8038e86e813e77fb69da65b4af872cd2) | 
`typedef `[`average_type`](#df/dac/classalps_1_1alea_1_1mctimeseries_1aac2ad9ac1e2eb88230f64b039c0aeb9e) | 
`typedef `[`iterator`](#df/dac/classalps_1_1alea_1_1mctimeseries_1acf5b0685fde587eecae0c58492bb7e3f) | 
`typedef `[`const_iterator`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a3f39b3e967cc340b961ae669d683eb57) | 

## Members

#### `public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a88e059316a090ba3e772e6425cfff71a)`()` 

#### `public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1ad8cf3350b64820345ccc3ba93e15eac0)`(const `[`alps::alea::mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< ValueType > & IN)` 

#### `public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a42f44b0b32e6a1b81cdd93feddb74fa7)`(const `[`alps::alea::mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< ValueType > & IN)` 

#### `public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1ae4ab7dd2decfc78fa399dbdbfef11e58)`(const `[`alps::alea::mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view)`< ValueType > & IN)` 

#### `public inline  `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a321183cad4fd0c0f1ee725e2bedd4feb)`(const std::vector< ValueType > & timeseries)` 

#### `public inline void `[`shallow_assign`](#df/dac/classalps_1_1alea_1_1mctimeseries_1abec5550cf0d08417c07e0d970230ecf3)`(const `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< ValueType > & IN)` 

#### `public inline const_iterator `[`begin`](#df/dac/classalps_1_1alea_1_1mctimeseries_1ab88df086df1774cdd7e29c1eaceefa62)`() const` 

#### `public inline const_iterator `[`end`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a2a8b0fbc12c9d0e4c8cbb1f49bc236c2)`() const` 

#### `public inline iterator `[`begin`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a7ce2a5ce3491077481f03d8fd9856a52)`()` 

#### `public inline iterator `[`end`](#df/dac/classalps_1_1alea_1_1mctimeseries_1abfbc9e87d301e8e805c94b4abf476c6c)`()` 

#### `public inline std::size_t `[`size`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a1cf5265b055555998f1b12ce8dd6e5ad)`() const` 

#### `public inline void `[`push_back`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a7a5acd13fe2291aa5a96a01f07a4cab4)`(value_type IN)` 

#### `public inline void `[`resize`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a64ef85ecd2aec1f0c56069a13a59429c)`(std::size_t size)` 

#### `public inline std::vector< ValueType > `[`timeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a2906be7767e45f08780c809e35030b25)`() const` 

#### `public inline void `[`print`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a54ff9df394571545037c5f368e7d2114)`() const` 

#### `typedef `[`size_type`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a98a7ab3fb83847a9af875da7fd8dc146) 

#### `typedef `[`value_type`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a8038e86e813e77fb69da65b4af872cd2) 

#### `typedef `[`average_type`](#df/dac/classalps_1_1alea_1_1mctimeseries_1aac2ad9ac1e2eb88230f64b039c0aeb9e) 

#### `typedef `[`iterator`](#df/dac/classalps_1_1alea_1_1mctimeseries_1acf5b0685fde587eecae0c58492bb7e3f) 

#### `typedef `[`const_iterator`](#df/dac/classalps_1_1alea_1_1mctimeseries_1a3f39b3e967cc340b961ae669d683eb57) 

# class `alps::alea::mctimeseries_view` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a564c3f659bf9816e4c7ba68d1ce09271)`(const `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< ValueType > & timeseries)` | 
`public inline void `[`cut_head`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a749ec0638a17618d09f665910c6d84f3)`(int cutoff)` | 
`public inline void `[`cut_tail`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a1849f11ee71470967fc0ac5c6dac5dda)`(int cutoff)` | 
`public inline const_iterator `[`begin`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a9a101f04a35a0c1e80995139d1023431)`() const` | 
`public inline const_iterator `[`end`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a21515a9ab88855e9cd429effda1eb417)`() const` | 
`public inline std::size_t `[`size`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a8eb1f8ce3d27929cc14e969a0464cfd1)`() const` | 
`public inline std::vector< ValueType > `[`timeseries`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1acf99d9bcd0bb4efd4ad6412b03d43411)`() const` | 
`public inline void `[`print`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1ae102d988439b2f88cf3e8f08dee2488d)`() const` | 
`typedef `[`size_type`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a35d210f079691cd3ee2e2cc67161c030) | 
`typedef `[`value_type`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a8e9b62a5df4767e02059b778a56abb5a) | 
`typedef `[`average_type`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a472bf164b23fad0c183e7e6c5ca3b451) | 
`typedef `[`iterator`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a88298e220a0ec3f80d42ca6b24129c7d) | 
`typedef `[`const_iterator`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a5ef8a9b6d6df418b1397cd078c00f9ca) | 

## Members

#### `public inline  `[`mctimeseries_view`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a564c3f659bf9816e4c7ba68d1ce09271)`(const `[`mctimeseries`](#df/dac/classalps_1_1alea_1_1mctimeseries)`< ValueType > & timeseries)` 

#### `public inline void `[`cut_head`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a749ec0638a17618d09f665910c6d84f3)`(int cutoff)` 

#### `public inline void `[`cut_tail`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a1849f11ee71470967fc0ac5c6dac5dda)`(int cutoff)` 

#### `public inline const_iterator `[`begin`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a9a101f04a35a0c1e80995139d1023431)`() const` 

#### `public inline const_iterator `[`end`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a21515a9ab88855e9cd429effda1eb417)`() const` 

#### `public inline std::size_t `[`size`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a8eb1f8ce3d27929cc14e969a0464cfd1)`() const` 

#### `public inline std::vector< ValueType > `[`timeseries`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1acf99d9bcd0bb4efd4ad6412b03d43411)`() const` 

#### `public inline void `[`print`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1ae102d988439b2f88cf3e8f08dee2488d)`() const` 

#### `typedef `[`size_type`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a35d210f079691cd3ee2e2cc67161c030) 

#### `typedef `[`value_type`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a8e9b62a5df4767e02059b778a56abb5a) 

#### `typedef `[`average_type`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a472bf164b23fad0c183e7e6c5ca3b451) 

#### `typedef `[`iterator`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a88298e220a0ec3f80d42ca6b24129c7d) 

#### `typedef `[`const_iterator`](#dc/d0f/classalps_1_1alea_1_1mctimeseries__view_1a5ef8a9b6d6df418b1397cd078c00f9ca) 

# class `alps::alea::None_class` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class_1a19be54f9fcadd6ca0499bcc6519bd1c1)`()` | 
`public inline  `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class_1a25ac125e0593c8369c503344aa5110ec)`(const `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class)` & other)` | 
`public template<>`  <br/>`inline  `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class_1a50449c0ee7d8bb58b24d6f3f467872d9)`(const T &)` | 
`public inline bool `[`operator==`](#d8/de2/classalps_1_1alea_1_1_none__class_1a261afe66edeffbd3004a2d4faba04af8)`(const `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class)` & other) const` | 
`public inline bool `[`operator!=`](#d8/de2/classalps_1_1alea_1_1_none__class_1af82d2dbfdb7a3b83fadcee181a077522)`(const `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class)` & other) const` | 
`public inline  `[`operator int`](#d8/de2/classalps_1_1alea_1_1_none__class_1a55ca7d3fe23ac769bc3341bbfa4a29db)`()` | 

## Members

#### `public inline  `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class_1a19be54f9fcadd6ca0499bcc6519bd1c1)`()` 

#### `public inline  `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class_1a25ac125e0593c8369c503344aa5110ec)`(const `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class)` & other)` 

#### `public template<>`  <br/>`inline  `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class_1a50449c0ee7d8bb58b24d6f3f467872d9)`(const T &)` 

#### `public inline bool `[`operator==`](#d8/de2/classalps_1_1alea_1_1_none__class_1a261afe66edeffbd3004a2d4faba04af8)`(const `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class)` & other) const` 

#### `public inline bool `[`operator!=`](#d8/de2/classalps_1_1alea_1_1_none__class_1af82d2dbfdb7a3b83fadcee181a077522)`(const `[`None_class`](#d8/de2/classalps_1_1alea_1_1_none__class)` & other) const` 

#### `public inline  `[`operator int`](#d8/de2/classalps_1_1alea_1_1_none__class_1a55ca7d3fe23ac769bc3341bbfa4a29db)`()` 

# class `alps::alea::NotEnoughMeasurementsError` 

```
class alps::alea::NotEnoughMeasurementsError
  : public std::runtime_error
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`NotEnoughMeasurementsError`](#df/d48/classalps_1_1alea_1_1_not_enough_measurements_error_1a80f65be3df6e2c9a9dc5e9805d1537aa)`()` | 

## Members

#### `public inline  `[`NotEnoughMeasurementsError`](#df/d48/classalps_1_1alea_1_1_not_enough_measurements_error_1a80f65be3df6e2c9a9dc5e9805d1537aa)`()` 

# class `alps::alea::value_with_error` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error_1afef7ca7753f2564f1f0d209be1d64b93)`(value_type mean,value_type error)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a53d611b18dd97adaaad74bda939a1ec3)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > const rhs)` | 
`public inline value_type `[`mean`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a90743a78f161331eb0707c0df910266f)`() const` | 
`public inline value_type `[`error`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a7d52a8c7f589ac6712a624631bfa8ac1)`() const` | 
`public inline bool `[`operator==`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a37acf675464bed0552d98efbec7092d4)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)` const & rhs)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator+=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ab9738b226557a64d8ecb472f35219c32)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > const & rhs)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator+=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ad2caddbb9cc5e015755b90c2ba14a348)`(value_type const & rhs)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator-=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ae0bcc3bfb818bf3395a7d994f8c6059a)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)` const & rhs)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator-=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a6ebcf83e17e60dddd180993008c3ad87)`(value_type const & rhs)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator*=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ab09ed352db995aac57891b1699fe500a)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > const & rhs)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator*=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a511dbd2bd5e3ea7d3d6b588ea300d600)`(value_type const & rhs)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator/=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a669249d5f6e0d932dcfae0cefb49e528)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > const & rhs)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator/=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ae509a3079cb9691ffb5a10e77ecb7d7e)`(value_type const & rhs)` | 
`public inline size_type `[`size`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ad999cc992786da9d30d00a07ed5dcb5c)`() const` | 
`public inline void `[`push_back`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ad0c93571c2a8d8454b637126347035d7)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< element_type > const & rhs)` | 
`public inline void `[`pop_back`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a364d4e06d38a01a012539e91bce37c0f)`()` | 
`public inline void `[`clear`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a4d0f817b01723a0fb3d70b6327243493)`()` | 
`public inline void `[`insert`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a1a06c49ea511822077d17bd29855ab1e)`(index_type const & index,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< element_type > const & value)` | 
`public inline void `[`erase`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a14a254d759b19042494b9454967c1c44)`(index_type const & index)` | 
`public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< element_type > `[`at`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a50fbdde551498a52adc7b4ac26d0ec4e)`(index_type const & index)` | 
`typedef `[`value_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a566c8023d394853891f41918ae345403) | 
`typedef `[`element_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1af641d3567a697bc5e4f8ced3fab6530e) | 
`typedef `[`size_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a528ac8d7e250b405afe98e14aaa502d3) | 
`typedef `[`index_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a22a046b7c02078e7c9a0693845f96e52) | 
`typedef `[`difference_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a04907cdcc8d8085cc47b42dc37dabe91) | 

## Members

#### `public inline  `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error_1afef7ca7753f2564f1f0d209be1d64b93)`(value_type mean,value_type error)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a53d611b18dd97adaaad74bda939a1ec3)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > const rhs)` 

#### `public inline value_type `[`mean`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a90743a78f161331eb0707c0df910266f)`() const` 

#### `public inline value_type `[`error`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a7d52a8c7f589ac6712a624631bfa8ac1)`() const` 

#### `public inline bool `[`operator==`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a37acf675464bed0552d98efbec7092d4)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)` const & rhs)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator+=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ab9738b226557a64d8ecb472f35219c32)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > const & rhs)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator+=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ad2caddbb9cc5e015755b90c2ba14a348)`(value_type const & rhs)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator-=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ae0bcc3bfb818bf3395a7d994f8c6059a)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)` const & rhs)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator-=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a6ebcf83e17e60dddd180993008c3ad87)`(value_type const & rhs)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator*=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ab09ed352db995aac57891b1699fe500a)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > const & rhs)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator*=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a511dbd2bd5e3ea7d3d6b588ea300d600)`(value_type const & rhs)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator/=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a669249d5f6e0d932dcfae0cefb49e528)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > const & rhs)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< value_type > & `[`operator/=`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ae509a3079cb9691ffb5a10e77ecb7d7e)`(value_type const & rhs)` 

#### `public inline size_type `[`size`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ad999cc992786da9d30d00a07ed5dcb5c)`() const` 

#### `public inline void `[`push_back`](#d5/dab/classalps_1_1alea_1_1value__with__error_1ad0c93571c2a8d8454b637126347035d7)`(`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< element_type > const & rhs)` 

#### `public inline void `[`pop_back`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a364d4e06d38a01a012539e91bce37c0f)`()` 

#### `public inline void `[`clear`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a4d0f817b01723a0fb3d70b6327243493)`()` 

#### `public inline void `[`insert`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a1a06c49ea511822077d17bd29855ab1e)`(index_type const & index,`[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< element_type > const & value)` 

#### `public inline void `[`erase`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a14a254d759b19042494b9454967c1c44)`(index_type const & index)` 

#### `public inline `[`value_with_error`](#d5/dab/classalps_1_1alea_1_1value__with__error)`< element_type > `[`at`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a50fbdde551498a52adc7b4ac26d0ec4e)`(index_type const & index)` 

#### `typedef `[`value_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a566c8023d394853891f41918ae345403) 

#### `typedef `[`element_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1af641d3567a697bc5e4f8ced3fab6530e) 

#### `typedef `[`size_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a528ac8d7e250b405afe98e14aaa502d3) 

#### `typedef `[`index_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a22a046b7c02078e7c9a0693845f96e52) 

#### `typedef `[`difference_type`](#d5/dab/classalps_1_1alea_1_1value__with__error_1a04907cdcc8d8085cc47b42dc37dabe91) 

# struct `alps::alea::binning_selector` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::alea::const_iterator_type` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#d6/dd3/structalps_1_1alea_1_1const__iterator__type_1accc6fe418018e9c8574a20390fbee2aa) | 

## Members

#### `typedef `[`type`](#d6/dd3/structalps_1_1alea_1_1const__iterator__type_1accc6fe418018e9c8574a20390fbee2aa) 

# struct `alps::alea::const_iterator_type< alps::alea::mcdata< ValueType > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#db/dfc/structalps_1_1alea_1_1const__iterator__type_3_01alps_1_1alea_1_1mcdata_3_01_value_type_01_4_01_4_1a59dd26b70e71353fb7b45f90cd8ff8c1) | 

## Members

#### `typedef `[`type`](#db/dfc/structalps_1_1alea_1_1const__iterator__type_3_01alps_1_1alea_1_1mcdata_3_01_value_type_01_4_01_4_1a59dd26b70e71353fb7b45f90cd8ff8c1) 

# struct `alps::alea::iterator_type` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#d3/d45/structalps_1_1alea_1_1iterator__type_1a0a3b71285478426ff0e0e40cf702f9ab) | 

## Members

#### `typedef `[`type`](#d3/d45/structalps_1_1alea_1_1iterator__type_1a0a3b71285478426ff0e0e40cf702f9ab) 

# struct `alps::alea::iterator_type< alps::alea::mcdata< ValueType > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#df/d7e/structalps_1_1alea_1_1iterator__type_3_01alps_1_1alea_1_1mcdata_3_01_value_type_01_4_01_4_1a7c440027a5134273cc30b3dbcbb2b2f6) | 

## Members

#### `typedef `[`type`](#df/d7e/structalps_1_1alea_1_1iterator__type_3_01alps_1_1alea_1_1mcdata_3_01_value_type_01_4_01_4_1a7c440027a5134273cc30b3dbcbb2b2f6) 

# struct `alps::alea::uncorrelated_selector` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# namespace `alps::detail` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline void `[`deleteit`](#d6/d5f/observableset_8_c_1aa6efd17b24a901118fac5dbc86e0c8e1)`(`[`Observable`](#df/d26/classalps_1_1_observable)` & obs)`            | 
`struct `[`alps::detail::function_pow`](#da/d26/structalps_1_1detail_1_1function__pow) | 
`struct `[`alps::detail::input_helper`](#dc/d45/structalps_1_1detail_1_1input__helper) | 
`struct `[`alps::detail::input_helper< boost::mpl::false_ >`](#dc/d4d/structalps_1_1detail_1_1input__helper_3_01boost_1_1mpl_1_1false___01_4) | 
`struct `[`alps::detail::input_helper< boost::mpl::true_ >`](#d1/d26/structalps_1_1detail_1_1input__helper_3_01boost_1_1mpl_1_1true___01_4) | 
`struct `[`alps::detail::pick_add_merge`](#d1/d23/structalps_1_1detail_1_1pick__add__merge) | 
`struct `[`alps::detail::pick_add_merge< false >`](#d3/d35/structalps_1_1detail_1_1pick__add__merge_3_01false_01_4) | 
`struct `[`alps::detail::pick_add_merge< true >`](#da/d42/structalps_1_1detail_1_1pick__add__merge_3_01true_01_4) | 

## Members

#### `public inline void `[`deleteit`](#d6/d5f/observableset_8_c_1aa6efd17b24a901118fac5dbc86e0c8e1)`(`[`Observable`](#df/d26/classalps_1_1_observable)` & obs)` 

# struct `alps::detail::function_pow` 

```
struct alps::detail::function_pow
  : public std::unary_function< T, double >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public double `[`pow_`](#da/d26/structalps_1_1detail_1_1function__pow_1a9e706ca1b8cb4d3390231b244f886107) | 
`public inline  `[`function_pow`](#da/d26/structalps_1_1detail_1_1function__pow_1a4bbb0149e60a7c640c2f836344da6523)`(double p)` | 
`public inline T `[`operator()`](#da/d26/structalps_1_1detail_1_1function__pow_1afecbd8ac219d995c1a9d0c6bd2b7f689)`(T x) const` | 

## Members

#### `public double `[`pow_`](#da/d26/structalps_1_1detail_1_1function__pow_1a9e706ca1b8cb4d3390231b244f886107) 

#### `public inline  `[`function_pow`](#da/d26/structalps_1_1detail_1_1function__pow_1a4bbb0149e60a7c640c2f836344da6523)`(double p)` 

#### `public inline T `[`operator()`](#da/d26/structalps_1_1detail_1_1function__pow_1afecbd8ac219d995c1a9d0c6bd2b7f689)`(T x) const` 

# struct `alps::detail::input_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::input_helper< boost::mpl::false_ >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::input_helper< boost::mpl::true_ >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::pick_add_merge` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::pick_add_merge< false >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::pick_add_merge< true >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# class `alps::alea::mcdata::const_iterator` 

```
class alps::alea::mcdata::const_iterator
  : public boost::random_access_iterator_helper< const_iterator, mcdata< T::value_type >, std::ptrdiff_t, mcdata< T::value_type > *, mcdata< T::value_type > & >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1ac10416c3724b462214eeeb3a6cd6a55e)`()` | 
`public inline  `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1ab36e98a7eec68fbb1f095dc0171a3e87)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & data,std::size_t index)` | 
`public inline  `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1a1359746823a77d69624204086bb5ae42)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & it)` | 
`public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< typename T::value_type > `[`operator*`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1ad66e89a69a4492659e32de0d725f0b23)`() const` | 
`public inline `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` & `[`operator=`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1acd30c82c197d9d49780c8e0c354069ef)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & rhs)` | 
`public inline void `[`operator++`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1a2e8b77cee9e3534a2e050731a4c768ef)`()` | 
`public inline bool `[`operator==`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1ac85b6d2bc923075c6fc53c09bfc29ec1)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & rhs) const` | 
`public inline `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` & `[`operator+=`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1a2e0ad12a0c873d08d260ffdfe67e202c)`(std::ptrdiff_t n)` | 
`public inline bool `[`operator<`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1aa2b204b3084cbb4fc0ebb53d16788881)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & rhs) const` | 
`public inline std::ptrdiff_t `[`operator-`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1a091d5d66a33ec46e3182f3c9f3699923)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & rhs)` | 

## Members

#### `public inline  `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1ac10416c3724b462214eeeb3a6cd6a55e)`()` 

#### `public inline  `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1ab36e98a7eec68fbb1f095dc0171a3e87)`(`[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< T > const & data,std::size_t index)` 

#### `public inline  `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1a1359746823a77d69624204086bb5ae42)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & it)` 

#### `public inline `[`mcdata`](#d9/d76/classalps_1_1alea_1_1mcdata)`< typename T::value_type > `[`operator*`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1ad66e89a69a4492659e32de0d725f0b23)`() const` 

#### `public inline `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` & `[`operator=`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1acd30c82c197d9d49780c8e0c354069ef)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & rhs)` 

#### `public inline void `[`operator++`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1a2e8b77cee9e3534a2e050731a4c768ef)`()` 

#### `public inline bool `[`operator==`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1ac85b6d2bc923075c6fc53c09bfc29ec1)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & rhs) const` 

#### `public inline `[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` & `[`operator+=`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1a2e0ad12a0c873d08d260ffdfe67e202c)`(std::ptrdiff_t n)` 

#### `public inline bool `[`operator<`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1aa2b204b3084cbb4fc0ebb53d16788881)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & rhs) const` 

#### `public inline std::ptrdiff_t `[`operator-`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator_1a091d5d66a33ec46e3182f3c9f3699923)`(`[`const_iterator`](#d4/da3/classalps_1_1alea_1_1mcdata_1_1const__iterator)` const & rhs)` 

Generated by [Moxygen](https://sourcey.com/moxygen)
