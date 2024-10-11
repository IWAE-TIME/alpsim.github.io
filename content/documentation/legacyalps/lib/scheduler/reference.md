
---
title: Reference
description: "ALPS Scheduler Library"
weight: 2
---

# Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`namespace `[`alps`](#d8/d3d/namespacealps) | 
`namespace `[`alps::scheduler`](#d2/d07/namespacealps_1_1scheduler) | 

# namespace `alps` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public std::string ALPS_DECL `[`convert2xml`](#d3/d82/convert_8h_1aa2928fbce11c8378c4196c9574945f7e)`(std::string const & name)`            | convert a file from XDR format to XML
`public void `[`convert_spectrum`](#dc/d85/convertxdr_8_c_1a7c78adc06705f712adc0c4cfcbeac250)`(const std::string & inname)`            | 
`public void `[`convert_mc`](#dc/d85/convertxdr_8_c_1a43008e40347221c46ad4361a743ffaef)`(const std::string & inname)`            | 
`public void `[`convert_xml`](#dc/d85/convertxdr_8_c_1ae4bf4f31c93214376d5bcf4f3233ba90)`(const std::string & inname)`            | 
`public void `[`convert_params`](#dc/d85/convertxdr_8_c_1a8e15239162ed7b2dfb4cc9766303a369)`(const std::string & inname)`            | 
`public void `[`convert_run`](#dc/d85/convertxdr_8_c_1a78a601f4c667007f0cdec52c8a17b562)`(const std::string & inname)`            | 
`public void `[`convert_simulation`](#dc/d85/convertxdr_8_c_1afc2461a3febd41412926a9ec83e72ee3)`(const std::string & inname)`            | 
`public void `[`convert_scheduler`](#dc/d85/convertxdr_8_c_1a57a6eea5f10e6101e25231efe1651aa6)`(const std::string & inname)`            | 
`class `[`alps::EigenvectorMeasurements`](#d8/de3/classalps_1_1_eigenvector_measurements) | 
`class `[`alps::MeasurementLabels`](#dc/dcc/classalps_1_1_measurement_labels) | 
`class `[`alps::MeasurementOperators`](#dd/db2/classalps_1_1_measurement_operators) | 

## Members

#### `public std::string ALPS_DECL `[`convert2xml`](#d3/d82/convert_8h_1aa2928fbce11c8378c4196c9574945f7e)`(std::string const & name)` 

convert a file from XDR format to XML

#### `public void `[`convert_spectrum`](#dc/d85/convertxdr_8_c_1a7c78adc06705f712adc0c4cfcbeac250)`(const std::string & inname)` 

#### `public void `[`convert_mc`](#dc/d85/convertxdr_8_c_1a43008e40347221c46ad4361a743ffaef)`(const std::string & inname)` 

#### `public void `[`convert_xml`](#dc/d85/convertxdr_8_c_1ae4bf4f31c93214376d5bcf4f3233ba90)`(const std::string & inname)` 

#### `public void `[`convert_params`](#dc/d85/convertxdr_8_c_1a8e15239162ed7b2dfb4cc9766303a369)`(const std::string & inname)` 

#### `public void `[`convert_run`](#dc/d85/convertxdr_8_c_1a78a601f4c667007f0cdec52c8a17b562)`(const std::string & inname)` 

#### `public void `[`convert_simulation`](#dc/d85/convertxdr_8_c_1afc2461a3febd41412926a9ec83e72ee3)`(const std::string & inname)` 

#### `public void `[`convert_scheduler`](#dc/d85/convertxdr_8_c_1a57a6eea5f10e6101e25231efe1651aa6)`(const std::string & inname)` 

# class `alps::EigenvectorMeasurements` 

```
class alps::EigenvectorMeasurements
  : public alps::MeasurementLabels
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public std::map< std::string, std::vector< value_type > > `[`average_values`](#d8/de3/classalps_1_1_eigenvector_measurements_1ae12c5f12bf96064f4da9f943d0996efa) | 
`public std::map< std::string, std::vector< std::vector< value_type > > > `[`local_values`](#d8/de3/classalps_1_1_eigenvector_measurements_1a72abd922e47ee6a8280d55a866f08fe8) | 
`public std::map< std::string, std::vector< std::vector< value_type > > > `[`correlation_values`](#d8/de3/classalps_1_1_eigenvector_measurements_1a481099b99dfdd2b520b7352e5d4eb9ec) | 
`public std::map< std::string, std::vector< std::vector< value_type > > > `[`structurefactor_values`](#d8/de3/classalps_1_1_eigenvector_measurements_1a3474320341da3b3df936123598b88b70) | 
`public template<>`  <br/>` `[`EigenvectorMeasurements`](#d8/de3/classalps_1_1_eigenvector_measurements_1ac0342c406c8180de35dd6c16ed4d1e09)`(LatticeModel const &)` | 
`public void `[`write_xml_one_vector`](#d8/de3/classalps_1_1_eigenvector_measurements_1ad1a37ae31b16bc1ac82f1cca7fe43f2a)`(oxstream & out,const boost::filesystem::path &,std::size_t j) const` | 
`public XMLTag `[`handle_tag`](#d8/de3/classalps_1_1_eigenvector_measurements_1a98070ff04c7eb30ed82a46445b7b80b5)`(std::istream & infile,const XMLTag & intag)` | 
`public virtual void `[`save`](#d8/de3/classalps_1_1_eigenvector_measurements_1a84d3f6f52d108a79031f3c35bab33a49)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#d8/de3/classalps_1_1_eigenvector_measurements_1af1c844ac65d2d58d463a53386ca49cad)`(hdf5::archive &)` | 
`public inline bool `[`empty`](#d8/de3/classalps_1_1_eigenvector_measurements_1aae353fc9127a7df76ed2c815e8646d53)`() const` | 
`typedef `[`value_type`](#d8/de3/classalps_1_1_eigenvector_measurements_1a1028913ca95bedc88dc3fe6e0299af73) | 

## Members

#### `public std::map< std::string, std::vector< value_type > > `[`average_values`](#d8/de3/classalps_1_1_eigenvector_measurements_1ae12c5f12bf96064f4da9f943d0996efa) 

#### `public std::map< std::string, std::vector< std::vector< value_type > > > `[`local_values`](#d8/de3/classalps_1_1_eigenvector_measurements_1a72abd922e47ee6a8280d55a866f08fe8) 

#### `public std::map< std::string, std::vector< std::vector< value_type > > > `[`correlation_values`](#d8/de3/classalps_1_1_eigenvector_measurements_1a481099b99dfdd2b520b7352e5d4eb9ec) 

#### `public std::map< std::string, std::vector< std::vector< value_type > > > `[`structurefactor_values`](#d8/de3/classalps_1_1_eigenvector_measurements_1a3474320341da3b3df936123598b88b70) 

#### `public template<>`  <br/>` `[`EigenvectorMeasurements`](#d8/de3/classalps_1_1_eigenvector_measurements_1ac0342c406c8180de35dd6c16ed4d1e09)`(LatticeModel const &)` 

#### `public void `[`write_xml_one_vector`](#d8/de3/classalps_1_1_eigenvector_measurements_1ad1a37ae31b16bc1ac82f1cca7fe43f2a)`(oxstream & out,const boost::filesystem::path &,std::size_t j) const` 

#### `public XMLTag `[`handle_tag`](#d8/de3/classalps_1_1_eigenvector_measurements_1a98070ff04c7eb30ed82a46445b7b80b5)`(std::istream & infile,const XMLTag & intag)` 

#### `public virtual void `[`save`](#d8/de3/classalps_1_1_eigenvector_measurements_1a84d3f6f52d108a79031f3c35bab33a49)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#d8/de3/classalps_1_1_eigenvector_measurements_1af1c844ac65d2d58d463a53386ca49cad)`(hdf5::archive &)` 

#### `public inline bool `[`empty`](#d8/de3/classalps_1_1_eigenvector_measurements_1aae353fc9127a7df76ed2c815e8646d53)`() const` 

#### `typedef `[`value_type`](#d8/de3/classalps_1_1_eigenvector_measurements_1a1028913ca95bedc88dc3fe6e0299af73) 

# class `alps::MeasurementLabels` 

```
class alps::MeasurementLabels
  : public alps::MeasurementOperators
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>` `[`MeasurementLabels`](#dc/dcc/classalps_1_1_measurement_labels_1a34d4d6c1c312f46b14499d077135b981)`(LatticeModel const &,int)` | 
`protected std::vector< std::string > `[`distlabel_`](#dc/dcc/classalps_1_1_measurement_labels_1a18f6f30c1dfdb6472e054c5fb7a5ec58) | 
`protected std::vector< std::string > `[`momentumlabel_`](#dc/dcc/classalps_1_1_measurement_labels_1a272c5d4cd6ceabc08bb8447517f75d9f) | 
`protected std::vector< std::string > `[`bondlabel_`](#dc/dcc/classalps_1_1_measurement_labels_1a35007e9580980c307023880ac0583fa6) | 
`protected std::vector< std::string > `[`sitelabel_`](#dc/dcc/classalps_1_1_measurement_labels_1a559b9f6155cb8d81962d700d315f522b) | 
`protected mutable std::map< std::string, bool > `[`bond_operator_`](#dc/dcc/classalps_1_1_measurement_labels_1aacf686e2590c352095df4470e9e3e370) | 

## Members

#### `public template<>`  <br/>` `[`MeasurementLabels`](#dc/dcc/classalps_1_1_measurement_labels_1a34d4d6c1c312f46b14499d077135b981)`(LatticeModel const &,int)` 

#### `protected std::vector< std::string > `[`distlabel_`](#dc/dcc/classalps_1_1_measurement_labels_1a18f6f30c1dfdb6472e054c5fb7a5ec58) 

#### `protected std::vector< std::string > `[`momentumlabel_`](#dc/dcc/classalps_1_1_measurement_labels_1a272c5d4cd6ceabc08bb8447517f75d9f) 

#### `protected std::vector< std::string > `[`bondlabel_`](#dc/dcc/classalps_1_1_measurement_labels_1a35007e9580980c307023880ac0583fa6) 

#### `protected std::vector< std::string > `[`sitelabel_`](#dc/dcc/classalps_1_1_measurement_labels_1a559b9f6155cb8d81962d700d315f522b) 

#### `protected mutable std::map< std::string, bool > `[`bond_operator_`](#dc/dcc/classalps_1_1_measurement_labels_1aacf686e2590c352095df4470e9e3e370) 

# class `alps::MeasurementOperators` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`MeasurementOperators`](#dd/db2/classalps_1_1_measurement_operators_1a80aa3b271796a49dce40699d5fc2563d)`(Parameters const & p)` | 
`public inline bool `[`calc_averages`](#dd/db2/classalps_1_1_measurement_operators_1a0f0b71c0c5198da884cde536301b0355)`() const` | 
`protected std::map< std::string, std::string > `[`average_expressions`](#dd/db2/classalps_1_1_measurement_operators_1a8e89f3fb51570e95670f30c07c1c6a00) | 
`protected std::map< std::string, std::string > `[`local_expressions`](#dd/db2/classalps_1_1_measurement_operators_1af6bb48c488697e713e069f29d51d22eb) | 
`protected std::map< std::string, std::pair< std::string, std::string > > `[`correlation_expressions`](#dd/db2/classalps_1_1_measurement_operators_1a7aab32987bf1c60fb4b627a22b44ca6f) | 
`protected std::map< std::string, std::pair< std::string, std::string > > `[`structurefactor_expressions`](#dd/db2/classalps_1_1_measurement_operators_1a7e0d8b9b338b6918155a67ad763551ef) | 
`protected inline bool `[`calc_labels`](#dd/db2/classalps_1_1_measurement_operators_1af407433ecb9290648d1ac0495bd9e343)`() const` | 

## Members

#### `public  `[`MeasurementOperators`](#dd/db2/classalps_1_1_measurement_operators_1a80aa3b271796a49dce40699d5fc2563d)`(Parameters const & p)` 

#### `public inline bool `[`calc_averages`](#dd/db2/classalps_1_1_measurement_operators_1a0f0b71c0c5198da884cde536301b0355)`() const` 

#### `protected std::map< std::string, std::string > `[`average_expressions`](#dd/db2/classalps_1_1_measurement_operators_1a8e89f3fb51570e95670f30c07c1c6a00) 

#### `protected std::map< std::string, std::string > `[`local_expressions`](#dd/db2/classalps_1_1_measurement_operators_1af6bb48c488697e713e069f29d51d22eb) 

#### `protected std::map< std::string, std::pair< std::string, std::string > > `[`correlation_expressions`](#dd/db2/classalps_1_1_measurement_operators_1a7aab32987bf1c60fb4b627a22b44ca6f) 

#### `protected std::map< std::string, std::pair< std::string, std::string > > `[`structurefactor_expressions`](#dd/db2/classalps_1_1_measurement_operators_1a7e0d8b9b338b6918155a67ad763551ef) 

#### `protected inline bool `[`calc_labels`](#dd/db2/classalps_1_1_measurement_operators_1af407433ecb9290648d1ac0495bd9e343)`() const` 

# namespace `alps::scheduler` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`enum `[`MCDumpType`](#d9/d49/types_8h_1ac1f17661c78009cc4bdfad9ecb2a8f9e)            | 
`enum `[`MCMP_Tags`](#d9/d49/types_8h_1a6380a8c791a483bf2e08617b783fbc71)            | 
`public inline alps::oxstream & `[`operator<<`](#d4/d21/info_8h_1a44bc6b5c3e9cd20e11a7b772cc656f95)`(alps::oxstream & o,const `[`alps::scheduler::Info`](#d5/dfa/classalps_1_1scheduler_1_1_info)` & i)`            | 
`public inline alps::oxstream & `[`operator<<`](#d4/d21/info_8h_1a0d392ed07f76623b1898424a4d1a549c)`(alps::oxstream & o,const `[`alps::scheduler::TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info)` & i)`            | 
`public void `[`print_copyright`](#da/d84/scheduler_8_c_1a77bde1298e87c9fc20f8a7afe86cf044)`(std::ostream & out)`            | 
`public void `[`init`](#da/d84/scheduler_8_c_1a5054a214051f716e161d1515d488e3a2)`(const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` & p)`            | 
`public int `[`start`](#da/d84/scheduler_8_c_1afe296223b2450a95f4b7433222ce747a)`(int argc,char ** argv,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` & p)`            | 
`public ALPS_DECL `[`SingleScheduler`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler)` * `[`start_single`](#d2/dd8/scheduler_8h_1ad3dd470c098eaabc7a0cbfde272b94be)`(const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` & p,int argc,char ** argv)`            | 
`public ALPS_DECL void `[`stop_single`](#d2/dd8/scheduler_8h_1ad0a69e1add212044860c59e91f723ed3)`(bool exit_)`            | 
`public inline boost::filesystem::path `[`optional_complete`](#d2/d57/workertask_8_c_1ad954201f1d454208422efadde5aa4c48)`(boost::filesystem::path const & p,boost::filesystem::path const & dir)`            | 
`class `[`alps::scheduler::AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task) | 
`class `[`alps::scheduler::AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker) | 
`class `[`alps::scheduler::BasicFactory`](#d8/d0b/classalps_1_1scheduler_1_1_basic_factory) | 
`class `[`alps::scheduler::DiagTask`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task) | 
`class `[`alps::scheduler::DummyMCRun`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run) | 
`class `[`alps::scheduler::Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory) | 
`class `[`alps::scheduler::Info`](#d5/dfa/classalps_1_1scheduler_1_1_info) | 
`class `[`alps::scheduler::LatticeMCRun`](#df/d74/classalps_1_1scheduler_1_1_lattice_m_c_run) | 
`class `[`alps::scheduler::LatticeModelMCRun`](#d0/d9b/classalps_1_1scheduler_1_1_lattice_model_m_c_run) | 
`class `[`alps::scheduler::MasterScheduler`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler) | 
`class `[`alps::scheduler::MCRun`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run) | 
`class `[`alps::scheduler::MCSimulation`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation) | 
`class `[`alps::scheduler::MPPScheduler`](#de/d2a/classalps_1_1scheduler_1_1_m_p_p_scheduler) | 
`class `[`alps::scheduler::NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options) | 
`class `[`alps::scheduler::Options`](#db/d2f/classalps_1_1scheduler_1_1_options) | 
`class `[`alps::scheduler::RemoteTask`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task) | 
`class `[`alps::scheduler::RemoteWorker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker) | 
`class `[`alps::scheduler::Scheduler`](#db/dd1/classalps_1_1scheduler_1_1_scheduler) | 
`class `[`alps::scheduler::SerialScheduler`](#d9/dce/classalps_1_1scheduler_1_1_serial_scheduler) | 
`class `[`alps::scheduler::SignalHandler`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler) | implements a signal handler. signals are intercepted and can be checked for.
`class `[`alps::scheduler::SimpleFactory`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory) | 
`class `[`alps::scheduler::SimpleMCFactory`](#d3/dda/classalps_1_1scheduler_1_1_simple_m_c_factory) | 
`class `[`alps::scheduler::SingleScheduler`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler) | 
`class `[`alps::scheduler::SlaveTask`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task) | 
`class `[`alps::scheduler::Task`](#d5/de3/classalps_1_1scheduler_1_1_task) | 
`class `[`alps::scheduler::TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info) | 
`class `[`alps::scheduler::Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker) | 
`class `[`alps::scheduler::WorkerTask`](#d9/d91/classalps_1_1scheduler_1_1_worker_task) | 
`struct `[`alps::scheduler::CheckpointFiles`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files) | 
`struct `[`alps::scheduler::rt`](#db/d9e/structalps_1_1scheduler_1_1rt) | 
`struct `[`alps::scheduler::TaskStatus`](#db/d7e/structalps_1_1scheduler_1_1_task_status) | 

## Members

#### `enum `[`MCDumpType`](#d9/d49/types_8h_1ac1f17661c78009cc4bdfad9ecb2a8f9e) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
MCDump_scheduler            | 
MCDump_task            | 
MCDump_run            | 
MCDump_measurements            | 
MCDump_run_master            | 
MCDump_run_slave            | 
MCDump_snapshot            | 
MCDump_worker_version            | 

#### `enum `[`MCMP_Tags`](#d9/d49/types_8h_1a6380a8c791a483bf2e08617b783fbc71) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
MCMP_stop_slave_scheduler            | 
MCMP_make_slave_task            | 
MCMP_make_task            | 
MCMP_dump_name            | 
MCMP_delete_task            | 
MCMP_get_task_finished            | 
MCMP_start_task            | 
MCMP_halt_task            | 
MCMP_add_processes            | 
MCMP_add_process            | 
MCMP_delete_processes            | 
MCMP_delete_process            | 
MCMP_checkpoint            | 
MCMP_get_work            | 
MCMP_nodes            | 
MCMP_ready            | 
MCMP_make_run            | 
MCMP_startRun            | 
MCMP_haltRun            | 
MCMP_delete_run            | 
MCMP_get_run_info            | 
MCMP_get_measurements            | 
MCMP_get_observable            | 
MCMP_save_run_to_file            | 
MCMP_load_run_from_file            | 
MCMP_get_run_work            | 
MCMP_set_parameters            | 
MCMP_get_measurements_and_infos            | 
MCMP_get_summary            | 
MCMP_void            | 
MCMP_run_dump            | 
MCMP_run_info            | 
MCMP_measurements            | 
MCMP_task_finished            | 
MCMP_observable            | 
MCMP_measurements_and_infos            | 
MCMP_work            | 
MCMP_run_work            | 
MCMP_summary            | 
MCMP_do_steps            | 

#### `public inline alps::oxstream & `[`operator<<`](#d4/d21/info_8h_1a44bc6b5c3e9cd20e11a7b772cc656f95)`(alps::oxstream & o,const `[`alps::scheduler::Info`](#d5/dfa/classalps_1_1scheduler_1_1_info)` & i)` 

#### `public inline alps::oxstream & `[`operator<<`](#d4/d21/info_8h_1a0d392ed07f76623b1898424a4d1a549c)`(alps::oxstream & o,const `[`alps::scheduler::TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info)` & i)` 

#### `public void `[`print_copyright`](#da/d84/scheduler_8_c_1a77bde1298e87c9fc20f8a7afe86cf044)`(std::ostream & out)` 

#### `public void `[`init`](#da/d84/scheduler_8_c_1a5054a214051f716e161d1515d488e3a2)`(const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` & p)` 

#### `public int `[`start`](#da/d84/scheduler_8_c_1afe296223b2450a95f4b7433222ce747a)`(int argc,char ** argv,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` & p)` 

#### `public ALPS_DECL `[`SingleScheduler`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler)` * `[`start_single`](#d2/dd8/scheduler_8h_1ad3dd470c098eaabc7a0cbfde272b94be)`(const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` & p,int argc,char ** argv)` 

#### `public ALPS_DECL void `[`stop_single`](#d2/dd8/scheduler_8h_1ad0a69e1add212044860c59e91f723ed3)`(bool exit_)` 

#### `public inline boost::filesystem::path `[`optional_complete`](#d2/d57/workertask_8_c_1ad954201f1d454208422efadde5aa4c48)`(boost::filesystem::path const & p,boost::filesystem::path const & dir)` 

# class `alps::scheduler::AbstractTask` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1ae7a7ad3f5a668913ca1fcd200ff48e0d)`()` | 
`public  `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a0f0e28ee3c93f18e243cac1959860e2d)`(const ProcessList &)` | 
`public virtual  `[`~AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a615411ce744bd7d1e21939c91c5f2201)`()` | 
`public void `[`checkpoint`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a06174423af2d4c29a1496920eb7d5fae)`(const boost::filesystem::path &,bool) const` | 
`public uint32_t `[`cpus`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1acb78cb058b32ff2428d629dfea9aa45d)`() const` | 
`public inline virtual bool `[`local`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a11528c8bdde42f92dcd260a2bccd18c1)`()` | 
`public virtual void `[`add_processes`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a61d2595420fa560ad11b72cbb71fc7f5)`(const ProcessList &)` | 
`public void `[`add_process`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a2ae6f96ba1e0388e5f037cbf816310c5)`(const Process &)` | 
`public void `[`start`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1af00bbd43a55073f5f2137dfc5ab00e64)`()` | 
`public void `[`run`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a8dd2ec85ce6832b52cb563eb9de47edb)`()` | 
`public void `[`halt`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1aadeb2bda1a8fb69c378742b5fc0fa48a)`()` | 
`public `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a2f5d8152dd76a9056de0be6eb1ab2628)`() const` | 
`public inline virtual double `[`work`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1ae7e61100fb9acff1c0b8b62288338d0c)`() const` | 
`public bool `[`finished`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1ae0f6b06ebde5e6e15d20f0ffe35cbd90)`(double &,double &) const` | 
`public virtual bool `[`handle_message`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1ab836ace194320117fab7e59885f51a94)`(const Process & master,int tag)` | 
`public inline int `[`finished_notime`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a8dd86dfc14b29b017d2ab72ce6338374)`() const` | 
`protected `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker)` * `[`theWorker`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1afc45006626bf4faf4846ea200b02a487) | 
`protected ProcessList `[`where`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a4a9782d329ac1dc1b7df56e9812d9887) | 
`protected bool `[`use_error_limit`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a4ddae964e2f9327a9191092a3e18aff4) | 

## Members

#### `public  `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1ae7a7ad3f5a668913ca1fcd200ff48e0d)`()` 

#### `public  `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a0f0e28ee3c93f18e243cac1959860e2d)`(const ProcessList &)` 

#### `public virtual  `[`~AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a615411ce744bd7d1e21939c91c5f2201)`()` 

#### `public void `[`checkpoint`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a06174423af2d4c29a1496920eb7d5fae)`(const boost::filesystem::path &,bool) const` 

#### `public uint32_t `[`cpus`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1acb78cb058b32ff2428d629dfea9aa45d)`() const` 

#### `public inline virtual bool `[`local`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a11528c8bdde42f92dcd260a2bccd18c1)`()` 

#### `public virtual void `[`add_processes`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a61d2595420fa560ad11b72cbb71fc7f5)`(const ProcessList &)` 

#### `public void `[`add_process`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a2ae6f96ba1e0388e5f037cbf816310c5)`(const Process &)` 

#### `public void `[`start`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1af00bbd43a55073f5f2137dfc5ab00e64)`()` 

#### `public void `[`run`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a8dd2ec85ce6832b52cb563eb9de47edb)`()` 

#### `public void `[`halt`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1aadeb2bda1a8fb69c378742b5fc0fa48a)`()` 

#### `public `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a2f5d8152dd76a9056de0be6eb1ab2628)`() const` 

#### `public inline virtual double `[`work`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1ae7e61100fb9acff1c0b8b62288338d0c)`() const` 

#### `public bool `[`finished`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1ae0f6b06ebde5e6e15d20f0ffe35cbd90)`(double &,double &) const` 

#### `public virtual bool `[`handle_message`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1ab836ace194320117fab7e59885f51a94)`(const Process & master,int tag)` 

#### `public inline int `[`finished_notime`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a8dd86dfc14b29b017d2ab72ce6338374)`() const` 

#### `protected `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker)` * `[`theWorker`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1afc45006626bf4faf4846ea200b02a487) 

#### `protected ProcessList `[`where`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a4a9782d329ac1dc1b7df56e9812d9887) 

#### `protected bool `[`use_error_limit`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task_1a4ddae964e2f9327a9191092a3e18aff4) 

# class `alps::scheduler::AbstractWorker` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a18a91c94f5f39b7906f483832bb66101)`()` | 
`public inline virtual  `[`~AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a29044bbf2577b39023fd6cdba65f11b9)`()` | 
`public inline virtual void `[`save`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1adddb968a5c12f3b3934bb4331553a6a9)`(hdf5::archive &) const` | 
`public inline virtual void `[`load`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a8ad9e80b9b5d2469f570b3df267fe745)`(hdf5::archive &)` | 
`public void `[`save_to_file`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1ade69209698534f0951e64e91a6e130e3)`(const boost::filesystem::path &,const boost::filesystem::path &) const` | 
`public void `[`load_from_file`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a29772d6906af83141145b769609caaf5)`(const boost::filesystem::path &,const boost::filesystem::path &)` | 
`public void `[`set_parameters`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1ad7c520a2ec72081b544f06b0b3c1e30a)`(const Parameters & parms)` | 
`public `[`TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info)` `[`get_info`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a96861766c9952962c48913d7c731ecd5)`() const` | 
`public double `[`work_done`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1ad8921cbb08173e0dda44d8494c94c3e1)`() const` | 
`public void `[`start_worker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1ab35c932dc359c1335e38862cb62f5796)`()` | 
`public void `[`halt_worker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a52e04d1ba29ae8f48c08647e83fd4927)`()` | 
`public bool `[`handle_message`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a1c399c9e8b04cde7627a47478a856996)`(const Process & runmaster,int32_t tag)` | 
`public `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a25adf94e337136b773fe88aeaee0e347)`() const` | 

## Members

#### `public inline  `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a18a91c94f5f39b7906f483832bb66101)`()` 

#### `public inline virtual  `[`~AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a29044bbf2577b39023fd6cdba65f11b9)`()` 

#### `public inline virtual void `[`save`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1adddb968a5c12f3b3934bb4331553a6a9)`(hdf5::archive &) const` 

#### `public inline virtual void `[`load`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a8ad9e80b9b5d2469f570b3df267fe745)`(hdf5::archive &)` 

#### `public void `[`save_to_file`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1ade69209698534f0951e64e91a6e130e3)`(const boost::filesystem::path &,const boost::filesystem::path &) const` 

#### `public void `[`load_from_file`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a29772d6906af83141145b769609caaf5)`(const boost::filesystem::path &,const boost::filesystem::path &)` 

#### `public void `[`set_parameters`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1ad7c520a2ec72081b544f06b0b3c1e30a)`(const Parameters & parms)` 

#### `public `[`TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info)` `[`get_info`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a96861766c9952962c48913d7c731ecd5)`() const` 

#### `public double `[`work_done`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1ad8921cbb08173e0dda44d8494c94c3e1)`() const` 

#### `public void `[`start_worker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1ab35c932dc359c1335e38862cb62f5796)`()` 

#### `public void `[`halt_worker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a52e04d1ba29ae8f48c08647e83fd4927)`()` 

#### `public bool `[`handle_message`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a1c399c9e8b04cde7627a47478a856996)`(const Process & runmaster,int32_t tag)` 

#### `public `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker_1a25adf94e337136b773fe88aeaee0e347)`() const` 

# class `alps::scheduler::BasicFactory` 

```
class alps::scheduler::BasicFactory
  : public alps::scheduler::SimpleFactory< TASK >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`BasicFactory`](#d8/d0b/classalps_1_1scheduler_1_1_basic_factory_1a3323022101246fd5b081bfaa616bddd6)`()` | 
`public inline virtual `[`Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker)` * `[`make_worker`](#d8/d0b/classalps_1_1scheduler_1_1_basic_factory_1af065f34c4ed151ec6ab45331f7e32ddc)`(const ProcessList & where,const Parameters & parms,int node) const` | 
`public inline virtual void `[`print_copyright`](#d8/d0b/classalps_1_1scheduler_1_1_basic_factory_1a531967585a40861b0c951133e8cc3e0c)`(std::ostream & out) const` | 

## Members

#### `public inline  `[`BasicFactory`](#d8/d0b/classalps_1_1scheduler_1_1_basic_factory_1a3323022101246fd5b081bfaa616bddd6)`()` 

#### `public inline virtual `[`Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker)` * `[`make_worker`](#d8/d0b/classalps_1_1scheduler_1_1_basic_factory_1af065f34c4ed151ec6ab45331f7e32ddc)`(const ProcessList & where,const Parameters & parms,int node) const` 

#### `public inline virtual void `[`print_copyright`](#d8/d0b/classalps_1_1scheduler_1_1_basic_factory_1a531967585a40861b0c951133e8cc3e0c)`(std::ostream & out) const` 

# class `alps::scheduler::DiagTask` 

```
class alps::scheduler::DiagTask
  : public alps::scheduler::Task
  : public graph_helper< typename graph_helper<>::graph_type >
  : public model_helper<>
  : public alps::MeasurementOperators
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`DiagTask`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a9f8b33dbb1ffe436af5bd4ad51897409)`(const ProcessList & where,const boost::filesystem::path & p,bool delay_construct)` | 
`public inline virtual void `[`dostep`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a75fa05cb8ec43d8129a86e023a888027)`()` | 
`public virtual void `[`save`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a1ec61c19ae4e6da6940df7b126cfda17)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1ac72ad78dd9fca25ddfe2706267a61678)`(hdf5::archive &)` | 
`protected std::vector< mag_vector_type > `[`eigenvalues_`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a87cbe441b890a24dde557c06b10c5d8c) | 
`protected std::vector< `[`EigenvectorMeasurements`](#d8/de3/classalps_1_1_eigenvector_measurements)`< value_type > > `[`measurements_`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1ac72fb1acb75087c37f4ad66b9cd281c1) | 
`protected std::vector< std::vector< std::pair< std::string, std::string > > > `[`quantumnumbervalues_`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a6ad193e5c0eaa453d0c00d6906763802) | 
`protected void `[`write_xml_body`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a031e162204c812d20ea0935cf6a72306)`(oxstream &,const boost::filesystem::path &,bool) const` | 
`protected virtual void `[`handle_tag`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a022d38c7b310c7907d6774e5e2e84a62)`(std::istream & infile,const XMLTag & tag)` | 
`protected inline bool `[`calc_vectors`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a46e04adaa9ab705cc50cfc26904490fb)`() const` | 
`protected inline bool `[`print_vectors`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a310daad9c0094e14bc3cbb62527ee23f)`() const` | 
`typedef `[`value_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a4683f2f0be854abfff8ed6d654e6650e) | 
`typedef `[`magnitude_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a60578fca998175e62be039ed665ff645) | 
`typedef `[`vector_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1aff97a45a72962fd296d42010a6cf8b9b) | 
`typedef `[`mag_vector_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a8d4393d6426e043b01fe05d5f783fddb) | 
`typedef `[`half_integer_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a55049cd0cb530ee8e528615b0f7786a9) | 
`typedef `[`operator_matrix_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a736580a36a1f91a85060a5f0fbc54b90) | 

## Members

#### `public  `[`DiagTask`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a9f8b33dbb1ffe436af5bd4ad51897409)`(const ProcessList & where,const boost::filesystem::path & p,bool delay_construct)` 

#### `public inline virtual void `[`dostep`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a75fa05cb8ec43d8129a86e023a888027)`()` 

#### `public virtual void `[`save`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a1ec61c19ae4e6da6940df7b126cfda17)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1ac72ad78dd9fca25ddfe2706267a61678)`(hdf5::archive &)` 

#### `protected std::vector< mag_vector_type > `[`eigenvalues_`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a87cbe441b890a24dde557c06b10c5d8c) 

#### `protected std::vector< `[`EigenvectorMeasurements`](#d8/de3/classalps_1_1_eigenvector_measurements)`< value_type > > `[`measurements_`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1ac72fb1acb75087c37f4ad66b9cd281c1) 

#### `protected std::vector< std::vector< std::pair< std::string, std::string > > > `[`quantumnumbervalues_`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a6ad193e5c0eaa453d0c00d6906763802) 

#### `protected void `[`write_xml_body`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a031e162204c812d20ea0935cf6a72306)`(oxstream &,const boost::filesystem::path &,bool) const` 

#### `protected virtual void `[`handle_tag`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a022d38c7b310c7907d6774e5e2e84a62)`(std::istream & infile,const XMLTag & tag)` 

#### `protected inline bool `[`calc_vectors`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a46e04adaa9ab705cc50cfc26904490fb)`() const` 

#### `protected inline bool `[`print_vectors`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a310daad9c0094e14bc3cbb62527ee23f)`() const` 

#### `typedef `[`value_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a4683f2f0be854abfff8ed6d654e6650e) 

#### `typedef `[`magnitude_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a60578fca998175e62be039ed665ff645) 

#### `typedef `[`vector_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1aff97a45a72962fd296d42010a6cf8b9b) 

#### `typedef `[`mag_vector_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a8d4393d6426e043b01fe05d5f783fddb) 

#### `typedef `[`half_integer_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a55049cd0cb530ee8e528615b0f7786a9) 

#### `typedef `[`operator_matrix_type`](#d2/d8a/classalps_1_1scheduler_1_1_diag_task_1a736580a36a1f91a85060a5f0fbc54b90) 

# class `alps::scheduler::DummyMCRun` 

```
class alps::scheduler::DummyMCRun
  : public alps::scheduler::MCRun
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`DummyMCRun`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1ad80ea3b5354e6fef2ff0ef67b2ce8aa1)`(const ProcessList & w,const alps::Parameters & p,int n)` | 
`public  `[`DummyMCRun`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1a0981b63013f68c730caf035a15ddde18)`()` | 
`public virtual void `[`dostep`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1ad3b2bf381ac57814bbe0ab0a949a04a1)`()` | 
`public virtual double `[`work_done`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1a24d617afefa126f16e2d71fae48f6abd)`() const` | 
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1a7e977a5dc3e8eda606ba3e5385f87e5c)`() const` | 

## Members

#### `public  `[`DummyMCRun`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1ad80ea3b5354e6fef2ff0ef67b2ce8aa1)`(const ProcessList & w,const alps::Parameters & p,int n)` 

#### `public  `[`DummyMCRun`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1a0981b63013f68c730caf035a15ddde18)`()` 

#### `public virtual void `[`dostep`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1ad3b2bf381ac57814bbe0ab0a949a04a1)`()` 

#### `public virtual double `[`work_done`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1a24d617afefa126f16e2d71fae48f6abd)`() const` 

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d8/d4e/classalps_1_1scheduler_1_1_dummy_m_c_run_1a7e977a5dc3e8eda606ba3e5385f87e5c)`() const` 

# class `alps::scheduler::Factory` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a9db351444555220a5744af345eb79f26)`()` | 
`public inline virtual  `[`~Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a385b920117f4217fdbda7e7f8651d320)`()` | 
`public virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a7fa6b1c0328ef5aefcb0fa15072fcfac)`(const ProcessList &,const boost::filesystem::path &) const` | 
`public virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#db/d7b/classalps_1_1scheduler_1_1_factory_1ae8d69472cc53ca852e246cc8a377071b)`(const ProcessList &,const boost::filesystem::path &,const Parameters &) const` | 
`public virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#db/d7b/classalps_1_1scheduler_1_1_factory_1ae0627a2707d77640a9b5c78da312d1f4)`(const ProcessList &,const Parameters &) const` | 
`public virtual `[`Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker)` * `[`make_worker`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a6fff0d55391888c5a9f18ae195326842)`(const ProcessList &,const Parameters &,int) const` | 
`public void `[`print_copyright`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a69f5b2d0addb74e5582925bd726f195e)`(std::ostream &) const` | 

## Members

#### `public inline  `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a9db351444555220a5744af345eb79f26)`()` 

#### `public inline virtual  `[`~Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a385b920117f4217fdbda7e7f8651d320)`()` 

#### `public virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a7fa6b1c0328ef5aefcb0fa15072fcfac)`(const ProcessList &,const boost::filesystem::path &) const` 

#### `public virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#db/d7b/classalps_1_1scheduler_1_1_factory_1ae8d69472cc53ca852e246cc8a377071b)`(const ProcessList &,const boost::filesystem::path &,const Parameters &) const` 

#### `public virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#db/d7b/classalps_1_1scheduler_1_1_factory_1ae0627a2707d77640a9b5c78da312d1f4)`(const ProcessList &,const Parameters &) const` 

#### `public virtual `[`Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker)` * `[`make_worker`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a6fff0d55391888c5a9f18ae195326842)`(const ProcessList &,const Parameters &,int) const` 

#### `public void `[`print_copyright`](#db/d7b/classalps_1_1scheduler_1_1_factory_1a69f5b2d0addb74e5582925bd726f195e)`(std::ostream &) const` 

# class `alps::scheduler::Info` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`Info`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a191ed71cef5216ffb4115588fd5e8d12)`()` | 
`public void `[`start`](#d5/dfa/classalps_1_1scheduler_1_1_info_1ad963055fb12d1a185af079293cc218f3)`(const std::string &)` | 
`public void `[`halt`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a776ec187bda683ac25f822058eb2441d)`()` | 
`public void `[`checkpoint`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a0f33677f76170d673a8a390c87e739a0)`()` | 
`public void `[`save`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a3b66e1d694f3fa192fdcae8e3f839f0f)`(hdf5::archive &) const` | 
`public void `[`load`](#d5/dfa/classalps_1_1scheduler_1_1_info_1abf00d1c833b8af6f01053fb15d03c76d)`(hdf5::archive &)` | 
`public void `[`save`](#d5/dfa/classalps_1_1scheduler_1_1_info_1abe7148f80bd61f2d439120b154cd7163)`(ODump &) const` | 
`public ALPS_DUMMY_VOID `[`write_xml`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a720f820b3f13a418b1ff804314a9983b)`(alps::oxstream &) const` | 
`public void `[`load`](#d5/dfa/classalps_1_1scheduler_1_1_info_1aa77e9ac5ab651fa25915dff7798fbb4c)`(IDump & dump,int version)` | 
`public const boost::posix_time::ptime & `[`start_time`](#d5/dfa/classalps_1_1scheduler_1_1_info_1acdbd4f1625716609924ccd69e9ed149e)`() const` | 
`public const boost::posix_time::ptime & `[`stop_time`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a83580f0281617a4bbea0f06e68e39aa6)`() const` | 
`public const std::string & `[`phase`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a9b3000df6baaa7af7498dc8fc7f45c67)`() const` | 
`public const std::string & `[`host`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a9c4b1abac6bd842b610e3fc92a6e844b)`() const` | 

## Members

#### `public  `[`Info`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a191ed71cef5216ffb4115588fd5e8d12)`()` 

#### `public void `[`start`](#d5/dfa/classalps_1_1scheduler_1_1_info_1ad963055fb12d1a185af079293cc218f3)`(const std::string &)` 

#### `public void `[`halt`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a776ec187bda683ac25f822058eb2441d)`()` 

#### `public void `[`checkpoint`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a0f33677f76170d673a8a390c87e739a0)`()` 

#### `public void `[`save`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a3b66e1d694f3fa192fdcae8e3f839f0f)`(hdf5::archive &) const` 

#### `public void `[`load`](#d5/dfa/classalps_1_1scheduler_1_1_info_1abf00d1c833b8af6f01053fb15d03c76d)`(hdf5::archive &)` 

#### `public void `[`save`](#d5/dfa/classalps_1_1scheduler_1_1_info_1abe7148f80bd61f2d439120b154cd7163)`(ODump &) const` 

#### `public ALPS_DUMMY_VOID `[`write_xml`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a720f820b3f13a418b1ff804314a9983b)`(alps::oxstream &) const` 

#### `public void `[`load`](#d5/dfa/classalps_1_1scheduler_1_1_info_1aa77e9ac5ab651fa25915dff7798fbb4c)`(IDump & dump,int version)` 

#### `public const boost::posix_time::ptime & `[`start_time`](#d5/dfa/classalps_1_1scheduler_1_1_info_1acdbd4f1625716609924ccd69e9ed149e)`() const` 

#### `public const boost::posix_time::ptime & `[`stop_time`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a83580f0281617a4bbea0f06e68e39aa6)`() const` 

#### `public const std::string & `[`phase`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a9b3000df6baaa7af7498dc8fc7f45c67)`() const` 

#### `public const std::string & `[`host`](#d5/dfa/classalps_1_1scheduler_1_1_info_1a9c4b1abac6bd842b610e3fc92a6e844b)`() const` 

# class `alps::scheduler::LatticeMCRun` 

```
class alps::scheduler::LatticeMCRun
  : public alps::scheduler::MCRun
  : public graph_helper< graph_helper<>::graph_type >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`LatticeMCRun`](#df/d74/classalps_1_1scheduler_1_1_lattice_m_c_run_1ace8f8b06f1dc5f1eaf7c46f0acac6bac)`(const ProcessList & w,const alps::Parameters & p,int n)` | 

## Members

#### `public inline  `[`LatticeMCRun`](#df/d74/classalps_1_1scheduler_1_1_lattice_m_c_run_1ace8f8b06f1dc5f1eaf7c46f0acac6bac)`(const ProcessList & w,const alps::Parameters & p,int n)` 

# class `alps::scheduler::LatticeModelMCRun` 

```
class alps::scheduler::LatticeModelMCRun
  : public alps::scheduler::LatticeMCRun< graph_helper<>::graph_type >
  : public model_helper< short >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`LatticeModelMCRun`](#d0/d9b/classalps_1_1scheduler_1_1_lattice_model_m_c_run_1aa53095d3ee5606e982ed148c6dcb8d29)`(const ProcessList & w,const alps::Parameters & p,int n,bool issymbolic)` | 
`public inline bool `[`has_sign_problem`](#d0/d9b/classalps_1_1scheduler_1_1_lattice_model_m_c_run_1a60548e400e49342e6b584246ad49af0b)`() const` | 

## Members

#### `public inline  `[`LatticeModelMCRun`](#d0/d9b/classalps_1_1scheduler_1_1_lattice_model_m_c_run_1aa53095d3ee5606e982ed148c6dcb8d29)`(const ProcessList & w,const alps::Parameters & p,int n,bool issymbolic)` 

#### `public inline bool `[`has_sign_problem`](#d0/d9b/classalps_1_1scheduler_1_1_lattice_model_m_c_run_1a60548e400e49342e6b584246ad49af0b)`() const` 

# class `alps::scheduler::MasterScheduler` 

```
class alps::scheduler::MasterScheduler
  : public alps::scheduler::Scheduler
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`MasterScheduler`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a544b6295ac6c8ebfb0cfb2d48f9b2518)`(const `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` | 
`public  `[`MasterScheduler`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a1884121704d5614202ab36437218fa5a)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` | 
`public  `[`~MasterScheduler`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1af0056db23de3d5bbd1d26932420906a6)`()` | 
`public virtual void `[`set_new_jobfile`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a4237854d88441b3c9f8caa20901f1921)`(const boost::filesystem::path & jobilename)` | Registers a new job file and updates everything that is related to the job files - namely the task files are parsed and the tasks are created accordingly. This function is used for the fitting and allows to start another simulation based on newly created files. Deleting and re-creating the schedulers yields to problems with syncronisation and integrity of the message space.
`protected std::vector< `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * > `[`tasks`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a5296a29ac7615557136d2e733f527a91) | 
`protected std::vector< int > `[`taskstatus`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a74508a6840923bd900efaa61327c9df7) | 
`protected void `[`remake_task`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1ab77cda7d5559d78c4f84861344ba38e0)`(ProcessList &,const int)` | 
`protected void `[`finish_task`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a99205db868092ee91c1834cbe0a40049)`(int)` | 
`protected virtual void `[`checkpoint`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a264a64b0db7ace14479f7c09cabce83b)`()` | 
`enum `[`TaskStatusFlag`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1acf8617d2804d211ade1484de58d1e84f) | 

## Members

#### `public  `[`MasterScheduler`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a544b6295ac6c8ebfb0cfb2d48f9b2518)`(const `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` 

#### `public  `[`MasterScheduler`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a1884121704d5614202ab36437218fa5a)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` 

#### `public  `[`~MasterScheduler`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1af0056db23de3d5bbd1d26932420906a6)`()` 

#### `public virtual void `[`set_new_jobfile`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a4237854d88441b3c9f8caa20901f1921)`(const boost::filesystem::path & jobilename)` 

Registers a new job file and updates everything that is related to the job files - namely the task files are parsed and the tasks are created accordingly. This function is used for the fitting and allows to start another simulation based on newly created files. Deleting and re-creating the schedulers yields to problems with syncronisation and integrity of the message space.

@params jobfilename The name of the new job file

#### `protected std::vector< `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * > `[`tasks`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a5296a29ac7615557136d2e733f527a91) 

#### `protected std::vector< int > `[`taskstatus`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a74508a6840923bd900efaa61327c9df7) 

#### `protected void `[`remake_task`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1ab77cda7d5559d78c4f84861344ba38e0)`(ProcessList &,const int)` 

#### `protected void `[`finish_task`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a99205db868092ee91c1834cbe0a40049)`(int)` 

#### `protected virtual void `[`checkpoint`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1a264a64b0db7ace14479f7c09cabce83b)`()` 

#### `enum `[`TaskStatusFlag`](#d0/dfd/classalps_1_1scheduler_1_1_master_scheduler_1acf8617d2804d211ade1484de58d1e84f) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
TaskNotExisting            | 
TaskNotStarted            | 
TaskRunning            | 
TaskHalted            | 
TaskFromDump            | 
TaskFinished            | 

# class `alps::scheduler::MCRun` 

```
class alps::scheduler::MCRun
  : public alps::scheduler::Worker
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`MCRun`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a1b0ccbfdf8e96f36da716d68d1d09775)`(const ProcessList &,const alps::Parameters &,int)` | 
`public virtual void `[`save_worker`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a6792939bf4426482303603199032e891)`(ODump &) const` | 
`public virtual void `[`load_worker`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a2b93df6965ca147df02fa76351ebd82f)`(IDump &)` | 
`public virtual void `[`save`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a2919da85a35c18fa025406d834d431dc)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a2ed4de450fe26a98a752f341b46e69db)`(hdf5::archive &)` | 
`public virtual void `[`save`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a1dac6fce5150d361cd11605ed1c12a2b)`(ODump &) const` | 
`public virtual void `[`load`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1ae3503d56265a519658bb9e8401a09f45)`(IDump &)` | 
`public virtual void `[`write_xml`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1abe0a86a9e062473cbbcc98b3f116c918)`(const boost::filesystem::path & name) const` | 
`public inline const ObservableSet & `[`get_measurements`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a3b3b1ebb8426da0cf3a2be4450ae07d0)`() const` | 
`public ObservableSet `[`get_compacted_measurements`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a67a9d183e42ff877d038c142c2d56466)`() const` | 
`public ObservableSet `[`get_and_remove_observable`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1ad2193abc8d150db31b69662709bbfce5)`(const std::string & obsname,bool compact)` | 
`public virtual std::string `[`work_phase`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1af2866b445088f292aafe5b43fb6f3ef8)`()` | 
`public virtual void `[`run`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a5eb950999c3662d81dcbca769e83c6d0)`()` | 
`public virtual bool `[`is_thermalized`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a78e099bad61422c20be0029cbca15361)`() const` | 
`public virtual bool `[`handle_message`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1ad6427e365aabb1bba12c8c7c5b273e2a)`(const Process & runmaster,int32_t tag)` | 
`protected ObservableSet `[`measurements`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a2465b6fbe7baa2e031d8f0498d4f3489) | 

## Members

#### `public  `[`MCRun`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a1b0ccbfdf8e96f36da716d68d1d09775)`(const ProcessList &,const alps::Parameters &,int)` 

#### `public virtual void `[`save_worker`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a6792939bf4426482303603199032e891)`(ODump &) const` 

#### `public virtual void `[`load_worker`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a2b93df6965ca147df02fa76351ebd82f)`(IDump &)` 

#### `public virtual void `[`save`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a2919da85a35c18fa025406d834d431dc)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a2ed4de450fe26a98a752f341b46e69db)`(hdf5::archive &)` 

#### `public virtual void `[`save`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a1dac6fce5150d361cd11605ed1c12a2b)`(ODump &) const` 

#### `public virtual void `[`load`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1ae3503d56265a519658bb9e8401a09f45)`(IDump &)` 

#### `public virtual void `[`write_xml`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1abe0a86a9e062473cbbcc98b3f116c918)`(const boost::filesystem::path & name) const` 

#### `public inline const ObservableSet & `[`get_measurements`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a3b3b1ebb8426da0cf3a2be4450ae07d0)`() const` 

#### `public ObservableSet `[`get_compacted_measurements`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a67a9d183e42ff877d038c142c2d56466)`() const` 

#### `public ObservableSet `[`get_and_remove_observable`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1ad2193abc8d150db31b69662709bbfce5)`(const std::string & obsname,bool compact)` 

#### `public virtual std::string `[`work_phase`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1af2866b445088f292aafe5b43fb6f3ef8)`()` 

#### `public virtual void `[`run`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a5eb950999c3662d81dcbca769e83c6d0)`()` 

#### `public virtual bool `[`is_thermalized`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a78e099bad61422c20be0029cbca15361)`() const` 

#### `public virtual bool `[`handle_message`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1ad6427e365aabb1bba12c8c7c5b273e2a)`(const Process & runmaster,int32_t tag)` 

#### `protected ObservableSet `[`measurements`](#d8/d56/classalps_1_1scheduler_1_1_m_c_run_1a2465b6fbe7baa2e031d8f0498d4f3489) 

# class `alps::scheduler::MCSimulation` 

```
class alps::scheduler::MCSimulation
  : public alps::scheduler::WorkerTask
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`MCSimulation`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a5aa7bb23a5e34e2394197d999fd6239f)`(const ProcessList & w,const boost::filesystem::path & p)` | 
`public inline  `[`MCSimulation`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a5466c41362466d762d82365579d94cf4)`(const ProcessList & w,const Parameters & p)` | 
`public ObservableSet `[`get_measurements`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1ab8f1e45531f5b1524e7fd938e929de42)`(bool compact) const` | 
`public ObservableSet `[`get_and_remove_observable`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1ad82286882afbd231deb69c3e026ee8d2)`(const std::string & obsname,bool compact)` | 
`public `[`MCSimulation`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation)` & `[`operator<<`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a9fff6288bf00ff06df6cce50ffab7609)`(const Observable & obs)` | 
`public void `[`addObservable`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1abff2b862f7917332b825e42e07663b77)`(const Observable & obs)` | 
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a7ac8d8438747d2757066008a6accf125)`() const` | Returns the summary, the name of the Observable is specified in the job file
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a478243b720f874f14f7a5bf1c819478c)`(const std::string) const` | Returns the summary of the [MCSimulation](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation) for the Observable given by the name

## Members

#### `public inline  `[`MCSimulation`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a5aa7bb23a5e34e2394197d999fd6239f)`(const ProcessList & w,const boost::filesystem::path & p)` 

#### `public inline  `[`MCSimulation`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a5466c41362466d762d82365579d94cf4)`(const ProcessList & w,const Parameters & p)` 

#### `public ObservableSet `[`get_measurements`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1ab8f1e45531f5b1524e7fd938e929de42)`(bool compact) const` 

#### `public ObservableSet `[`get_and_remove_observable`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1ad82286882afbd231deb69c3e026ee8d2)`(const std::string & obsname,bool compact)` 

#### `public `[`MCSimulation`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation)` & `[`operator<<`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a9fff6288bf00ff06df6cce50ffab7609)`(const Observable & obs)` 

#### `public void `[`addObservable`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1abff2b862f7917332b825e42e07663b77)`(const Observable & obs)` 

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a7ac8d8438747d2757066008a6accf125)`() const` 

Returns the summary, the name of the Observable is specified in the job file

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation_1a478243b720f874f14f7a5bf1c819478c)`(const std::string) const` 

Returns the summary of the [MCSimulation](#d9/db8/classalps_1_1scheduler_1_1_m_c_simulation) for the Observable given by the name

@params name the name of the observable

# class `alps::scheduler::MPPScheduler` 

```
class alps::scheduler::MPPScheduler
  : public alps::scheduler::MasterScheduler
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`MPPScheduler`](#de/d2a/classalps_1_1scheduler_1_1_m_p_p_scheduler_1ad724acec38574b7b025c3a892776817c)`(const `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` | 
`public  `[`MPPScheduler`](#de/d2a/classalps_1_1scheduler_1_1_m_p_p_scheduler_1a12f85efb72884d6a28b226055c5bf5ff)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` | 
`public virtual int `[`run`](#de/d2a/classalps_1_1scheduler_1_1_m_p_p_scheduler_1af1a6b5313f7b2172502e906e46a4f750)`()` | 

## Members

#### `public  `[`MPPScheduler`](#de/d2a/classalps_1_1scheduler_1_1_m_p_p_scheduler_1ad724acec38574b7b025c3a892776817c)`(const `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` 

#### `public  `[`MPPScheduler`](#de/d2a/classalps_1_1scheduler_1_1_m_p_p_scheduler_1a12f85efb72884d6a28b226055c5bf5ff)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` 

#### `public virtual int `[`run`](#de/d2a/classalps_1_1scheduler_1_1_m_p_p_scheduler_1af1a6b5313f7b2172502e906e46a4f750)`()` 

# class `alps::scheduler::NoJobfileOptions` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public std::string `[`programname`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1acad8005b5361d86b0095dfa1890342b0) | 
`public double `[`min_check_time`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a10c6f3084d15675062ea6c53ff1f3609) | 
`public double `[`max_check_time`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1ad3884a29be73d36731267f406ff9cd9f) | 
`public double `[`checkpoint_time`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a14802f70778503c518ec0f2fdfba0469) | 
`public int `[`min_cpus`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1ae3f8810d3ea965304c482f77183d8f8a) | 
`public int `[`max_cpus`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a8f5977d015a30621294c1b975f7e106b) | 
`public double `[`time_limit`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1ad715ddf4e6394d8a24509dc91e0dce0e) | 
`public bool `[`use_mpi`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1aeaf532b012917bc060cdb368efa86290) | 
`public bool `[`valid`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a1c9112bf7dee3cf18c02f1074c9cfba6) | 
`public bool `[`write_xml`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a5c41a30660d2c3fa68a4b0b32f035b62) | 
`public  `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1ac22ec83a04c3fedda464ff840cf8432b)`(int argc,char ** argv)` | 
`public  `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a9a332c56e2285d2be363dba7d039d640)`()` | 

## Members

#### `public std::string `[`programname`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1acad8005b5361d86b0095dfa1890342b0) 

#### `public double `[`min_check_time`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a10c6f3084d15675062ea6c53ff1f3609) 

#### `public double `[`max_check_time`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1ad3884a29be73d36731267f406ff9cd9f) 

#### `public double `[`checkpoint_time`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a14802f70778503c518ec0f2fdfba0469) 

#### `public int `[`min_cpus`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1ae3f8810d3ea965304c482f77183d8f8a) 

#### `public int `[`max_cpus`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a8f5977d015a30621294c1b975f7e106b) 

#### `public double `[`time_limit`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1ad715ddf4e6394d8a24509dc91e0dce0e) 

#### `public bool `[`use_mpi`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1aeaf532b012917bc060cdb368efa86290) 

#### `public bool `[`valid`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a1c9112bf7dee3cf18c02f1074c9cfba6) 

#### `public bool `[`write_xml`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a5c41a30660d2c3fa68a4b0b32f035b62) 

#### `public  `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1ac22ec83a04c3fedda464ff840cf8432b)`(int argc,char ** argv)` 

#### `public  `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options_1a9a332c56e2285d2be363dba7d039d640)`()` 

# class `alps::scheduler::Options` 

```
class alps::scheduler::Options
  : public alps::scheduler::NoJobfileOptions
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public boost::filesystem::path `[`jobfilename`](#db/d2f/classalps_1_1scheduler_1_1_options_1a8d791d6e51a8af4c5bc0aa14dfcb9c7e) | 
`public  `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options_1a7c7080a098f8752f9797a2d07be930fc)`(int argc,char ** argv)` | 
`public  `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options_1ae3bca6fd4093bf542ef8db70048a3ce1)`()` | 

## Members

#### `public boost::filesystem::path `[`jobfilename`](#db/d2f/classalps_1_1scheduler_1_1_options_1a8d791d6e51a8af4c5bc0aa14dfcb9c7e) 

#### `public  `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options_1a7c7080a098f8752f9797a2d07be930fc)`(int argc,char ** argv)` 

#### `public  `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options_1ae3bca6fd4093bf542ef8db70048a3ce1)`()` 

# class `alps::scheduler::RemoteTask` 

```
class alps::scheduler::RemoteTask
  : public alps::scheduler::AbstractTask
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`RemoteTask`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a868b9812735869a84c59f9208cb3b890)`(const ProcessList &,const boost::filesystem::path &)` | 
`public  `[`~RemoteTask`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a564a50298ea0abc94cccd8ef15c057ef)`()` | 
`public virtual void `[`checkpoint`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1ac456c986ba583697ed72cb4439f2f95a)`(const boost::filesystem::path &,bool) const` | 
`public virtual void `[`add_processes`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a8a3c7f356dd2a8619ff42465d309f009)`(const ProcessList &)` | 
`public virtual void `[`add_process`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a1510614dc7688ebeb852b56b65c926bb)`(const Process &)` | 
`public virtual uint32_t `[`cpus`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a3cda7f9cdd750e2e08fd5f01b99e1a59)`() const` | 
`public inline virtual bool `[`local`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a58d2c3ed3bdfcdb06092851406b1ddb2)`()` | 
`public virtual void `[`start`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a715271e9d2914afa8f02b50f2da11ccb)`()` | 
`public virtual bool `[`finished`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1ad0eb1e9aeac378fe2a1fd92e34045a11)`(double &,double &) const` | 
`public virtual double `[`work`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a3c05ca0bb064f0e0e471be11b84bb7bd)`() const` | 
`public virtual void `[`run`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1ad825748be83ee605ccf8ce834f45c5a2)`()` | 
`public virtual void `[`halt`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1ad71f5531a397eb3b3d932326b877f937)`()` | 
`public virtual bool `[`handle_message`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a1dfc6121db6d971e8919c0924f50fe25)`(const Process & master,int tag)` | 
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1aa400335e795eb99bb7dcd7bd16d0a976)`() const` | Sends the summary for this remote task to the master

## Members

#### `public  `[`RemoteTask`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a868b9812735869a84c59f9208cb3b890)`(const ProcessList &,const boost::filesystem::path &)` 

#### `public  `[`~RemoteTask`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a564a50298ea0abc94cccd8ef15c057ef)`()` 

#### `public virtual void `[`checkpoint`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1ac456c986ba583697ed72cb4439f2f95a)`(const boost::filesystem::path &,bool) const` 

#### `public virtual void `[`add_processes`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a8a3c7f356dd2a8619ff42465d309f009)`(const ProcessList &)` 

#### `public virtual void `[`add_process`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a1510614dc7688ebeb852b56b65c926bb)`(const Process &)` 

#### `public virtual uint32_t `[`cpus`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a3cda7f9cdd750e2e08fd5f01b99e1a59)`() const` 

#### `public inline virtual bool `[`local`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a58d2c3ed3bdfcdb06092851406b1ddb2)`()` 

#### `public virtual void `[`start`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a715271e9d2914afa8f02b50f2da11ccb)`()` 

#### `public virtual bool `[`finished`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1ad0eb1e9aeac378fe2a1fd92e34045a11)`(double &,double &) const` 

#### `public virtual double `[`work`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a3c05ca0bb064f0e0e471be11b84bb7bd)`() const` 

#### `public virtual void `[`run`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1ad825748be83ee605ccf8ce834f45c5a2)`()` 

#### `public virtual void `[`halt`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1ad71f5531a397eb3b3d932326b877f937)`()` 

#### `public virtual bool `[`handle_message`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1a1dfc6121db6d971e8919c0924f50fe25)`(const Process & master,int tag)` 

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d3/dfe/classalps_1_1scheduler_1_1_remote_task_1aa400335e795eb99bb7dcd7bd16d0a976)`() const` 

Sends the summary for this remote task to the master

# class `alps::scheduler::RemoteWorker` 

```
class alps::scheduler::RemoteWorker
  : public alps::scheduler::AbstractWorker
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`RemoteWorker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1aa8ca7ca361e0f146aedd2dd5197c8e73)`(const ProcessList &,const Parameters &,int32_t)` | 
`public virtual  `[`~RemoteWorker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a5d97eae5b4499505d6dc78ac0dbd8cf3)`()` | 
`public virtual void `[`set_parameters`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1aeb07cc81635653586f7095c9ebcf24d2)`(const Parameters & parms)` | 
`public virtual void `[`save_to_file`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a974f70bbde495c943e36830413256775)`(const boost::filesystem::path &,const boost::filesystem::path &) const` | 
`public virtual void `[`load_from_file`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1ae9daae4a1f408b17bcc23a0bfd700969)`(const boost::filesystem::path &,const boost::filesystem::path &)` | 
`public virtual void `[`start_worker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a85088bd9bbc5120b07f4ececa7628157)`()` | 
`public virtual void `[`halt_worker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a2b1658a760cb1331fdb9cb32c0028419)`()` | 
`public virtual `[`TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info)` `[`get_info`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a4f3d713f7c61b537d439fbfe8ca286c7)`() const` | 
`public virtual double `[`work_done`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a0f976457426a9c92720bf14a44427923)`() const` | 
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a499ce21dfc8f47ac55f9f3b7dd635d4e)`() const` | 
`public inline const Process & `[`process`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a3ef96dc6895de37c9aa43e54c10d3b6c)`() const` | 
`public virtual bool `[`handle_message`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a9a518b6da72333c5df85401fe2bca643)`(const Process & runmaster,int32_t tag)` | 

## Members

#### `public  `[`RemoteWorker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1aa8ca7ca361e0f146aedd2dd5197c8e73)`(const ProcessList &,const Parameters &,int32_t)` 

#### `public virtual  `[`~RemoteWorker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a5d97eae5b4499505d6dc78ac0dbd8cf3)`()` 

#### `public virtual void `[`set_parameters`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1aeb07cc81635653586f7095c9ebcf24d2)`(const Parameters & parms)` 

#### `public virtual void `[`save_to_file`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a974f70bbde495c943e36830413256775)`(const boost::filesystem::path &,const boost::filesystem::path &) const` 

#### `public virtual void `[`load_from_file`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1ae9daae4a1f408b17bcc23a0bfd700969)`(const boost::filesystem::path &,const boost::filesystem::path &)` 

#### `public virtual void `[`start_worker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a85088bd9bbc5120b07f4ececa7628157)`()` 

#### `public virtual void `[`halt_worker`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a2b1658a760cb1331fdb9cb32c0028419)`()` 

#### `public virtual `[`TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info)` `[`get_info`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a4f3d713f7c61b537d439fbfe8ca286c7)`() const` 

#### `public virtual double `[`work_done`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a0f976457426a9c92720bf14a44427923)`() const` 

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a499ce21dfc8f47ac55f9f3b7dd635d4e)`() const` 

#### `public inline const Process & `[`process`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a3ef96dc6895de37c9aa43e54c10d3b6c)`() const` 

#### `public virtual bool `[`handle_message`](#df/d55/classalps_1_1scheduler_1_1_remote_worker_1a9a518b6da72333c5df85401fe2bca643)`(const Process & runmaster,int32_t tag)` 

# class `alps::scheduler::Scheduler` 

```
class alps::scheduler::Scheduler
  : public boost::noncopyable
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` & `[`proc`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ac915708540d7b1d55bde8bf349c29f0f) | 
`public `[`SignalHandler`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler)` `[`sig`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a2f97bb8d0fab953094d0fc61e6fd94a1) | 
`public const std::string `[`programname`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a7bab20f0bda19d80cb692b417e035810) | 
`public  `[`Scheduler`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad543a6b646200ca8157724ea8ab87311)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` | 
`public virtual  `[`~Scheduler`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad405d547a4e63d1db2f3e3e236c7a36e)`()` | 
`public inline virtual void `[`set_new_jobfile`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a19b514bc99d411a1dcf710f0844a7838)`(const boost::filesystem::path &)` | 
`public virtual int `[`run`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a5612a21a2b46ff5cb585764057ac5bb0)`()` | 
`public inline void `[`makeSummary`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ac18c9ba027f4e60569e93a8129b66e6f)`()` | 
`public inline ResultsType `[`getSummary`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a0fc96cc3f472e968b5debae2a110328c)`() const` | 
`public `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * `[`make_task`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a2405aa110e6563d18847068397480f0a)`(const ProcessList &,const boost::filesystem::path &)` | 
`public `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * `[`make_task`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad8886505afc31dbf065e1ded348bb2a2)`(const boost::filesystem::path &)` | 
`public `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker)` * `[`make_worker`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a4653cb3ce8689d63bb0552f6fdabf1ec)`(const ProcessList &,const Parameters &,int)` | 
`public `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker)` * `[`make_worker`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ac8677d64c5628ff9973e447211c4629a)`(const Parameters &)` | 
`public virtual void `[`set_time_limit`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a19f0c5043ff481913788c8530fbe5573)`(double limit)` | 
`public virtual void `[`checkpoint`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a72073abd0a28d18e174b654bc0c7a93b)`()` | 
`public int `[`check_signals`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a04f749ef6b85c45a99ab5ee4522f5177)`()` | 
`protected `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * `[`theTask`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a76019eebae92cb24954add517d45fd57) | 
`protected boost::filesystem::path `[`defaultpath`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1aa34f8c21de0f6c71918e00b51296d1fc) | 
`protected bool `[`use_error_limit`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a097c2c6a14cd791ddd69606284d50e77) | 
`protected ResultsType `[`sim_results`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1aab9263af4f3d2c4ff6b8205e48bc46dd) | 
`protected bool `[`make_summary`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad63086cda50b308b7d3633d3cc4fcc23) | 
`protected ProcessList `[`processes`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a2d3264efc9a5886d845ab25151f3cfd9) | 
`protected double `[`min_check_time`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1af45e4d32d1219684f4aedda742310c06) | 
`protected double `[`max_check_time`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad430fb4bd818305211732e3ec4761b95) | 
`protected double `[`checkpoint_time`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a1ad4cd1f88c900e106753fded6522145) | 
`protected std::size_t `[`min_cpus`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a2fa73ded654c320b9856420fdae75298) | 
`protected std::size_t `[`max_cpus`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1aa44824ed68ea14a52e731bb7f9f0f31f) | 
`protected double `[`time_limit`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ab26e818b083010ab80bed791fe335570) | 
`protected bool `[`write_xml`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a4e0d8eb97dd6d6731b2d26d8a9e482b1) | 

## Members

#### `public const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` & `[`proc`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ac915708540d7b1d55bde8bf349c29f0f) 

#### `public `[`SignalHandler`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler)` `[`sig`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a2f97bb8d0fab953094d0fc61e6fd94a1) 

#### `public const std::string `[`programname`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a7bab20f0bda19d80cb692b417e035810) 

#### `public  `[`Scheduler`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad543a6b646200ca8157724ea8ab87311)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` 

#### `public virtual  `[`~Scheduler`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad405d547a4e63d1db2f3e3e236c7a36e)`()` 

#### `public inline virtual void `[`set_new_jobfile`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a19b514bc99d411a1dcf710f0844a7838)`(const boost::filesystem::path &)` 

#### `public virtual int `[`run`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a5612a21a2b46ff5cb585764057ac5bb0)`()` 

#### `public inline void `[`makeSummary`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ac18c9ba027f4e60569e93a8129b66e6f)`()` 

#### `public inline ResultsType `[`getSummary`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a0fc96cc3f472e968b5debae2a110328c)`() const` 

#### `public `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * `[`make_task`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a2405aa110e6563d18847068397480f0a)`(const ProcessList &,const boost::filesystem::path &)` 

#### `public `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * `[`make_task`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad8886505afc31dbf065e1ded348bb2a2)`(const boost::filesystem::path &)` 

#### `public `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker)` * `[`make_worker`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a4653cb3ce8689d63bb0552f6fdabf1ec)`(const ProcessList &,const Parameters &,int)` 

#### `public `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker)` * `[`make_worker`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ac8677d64c5628ff9973e447211c4629a)`(const Parameters &)` 

#### `public virtual void `[`set_time_limit`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a19f0c5043ff481913788c8530fbe5573)`(double limit)` 

#### `public virtual void `[`checkpoint`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a72073abd0a28d18e174b654bc0c7a93b)`()` 

#### `public int `[`check_signals`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a04f749ef6b85c45a99ab5ee4522f5177)`()` 

#### `protected `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * `[`theTask`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a76019eebae92cb24954add517d45fd57) 

#### `protected boost::filesystem::path `[`defaultpath`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1aa34f8c21de0f6c71918e00b51296d1fc) 

#### `protected bool `[`use_error_limit`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a097c2c6a14cd791ddd69606284d50e77) 

#### `protected ResultsType `[`sim_results`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1aab9263af4f3d2c4ff6b8205e48bc46dd) 

#### `protected bool `[`make_summary`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad63086cda50b308b7d3633d3cc4fcc23) 

#### `protected ProcessList `[`processes`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a2d3264efc9a5886d845ab25151f3cfd9) 

#### `protected double `[`min_check_time`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1af45e4d32d1219684f4aedda742310c06) 

#### `protected double `[`max_check_time`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ad430fb4bd818305211732e3ec4761b95) 

#### `protected double `[`checkpoint_time`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a1ad4cd1f88c900e106753fded6522145) 

#### `protected std::size_t `[`min_cpus`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a2fa73ded654c320b9856420fdae75298) 

#### `protected std::size_t `[`max_cpus`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1aa44824ed68ea14a52e731bb7f9f0f31f) 

#### `protected double `[`time_limit`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1ab26e818b083010ab80bed791fe335570) 

#### `protected bool `[`write_xml`](#db/dd1/classalps_1_1scheduler_1_1_scheduler_1a4e0d8eb97dd6d6731b2d26d8a9e482b1) 

# class `alps::scheduler::SerialScheduler` 

```
class alps::scheduler::SerialScheduler
  : public alps::scheduler::MasterScheduler
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`SerialScheduler`](#d9/dce/classalps_1_1scheduler_1_1_serial_scheduler_1ae6763e6371c02caff0f56a4d79bc6909)`(const `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` | 
`public  `[`SerialScheduler`](#d9/dce/classalps_1_1scheduler_1_1_serial_scheduler_1ae978ff85f6bf9e3f121ed4afa99ee655)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` | 
`public virtual int `[`run`](#d9/dce/classalps_1_1scheduler_1_1_serial_scheduler_1a6578c5dec561185b2e36b65d7d53ad71)`()` | 

## Members

#### `public  `[`SerialScheduler`](#d9/dce/classalps_1_1scheduler_1_1_serial_scheduler_1ae6763e6371c02caff0f56a4d79bc6909)`(const `[`Options`](#db/d2f/classalps_1_1scheduler_1_1_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` 

#### `public  `[`SerialScheduler`](#d9/dce/classalps_1_1scheduler_1_1_serial_scheduler_1ae978ff85f6bf9e3f121ed4afa99ee655)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` 

#### `public virtual int `[`run`](#d9/dce/classalps_1_1scheduler_1_1_serial_scheduler_1a6578c5dec561185b2e36b65d7d53ad71)`()` 

# class `alps::scheduler::SignalHandler` 

implements a signal handler. signals are intercepted and can be checked for.

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`SignalHandler`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler_1a232b1b0f1b6243807dd0222b62ad3597)`()` | a default constructor
`public `[`SignalInfo`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler_1ab9e6a1c6006f29871d34079979061fd2)` `[`operator()`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler_1ac10f7b49a94f71463c05dcbb15bab29a)`()` | ask for signals. If more than one signal has been received the signal with the highest priority will be returned. Priorities are: USER1 > USER2 > STOP > TERMINATE.
`enum `[`SignalInfo`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler_1ab9e6a1c6006f29871d34079979061fd2) | symbolic names for signals. SIGINT, SIGQUIT and SIGTERM are mapped to TERMINATE SIGTSTP is mapped to STOP SIGUSR1 is mapped to USER1 SIGUSR2 is mapped to USER2

## Members

#### `public  `[`SignalHandler`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler_1a232b1b0f1b6243807dd0222b62ad3597)`()` 

a default constructor

#### `public `[`SignalInfo`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler_1ab9e6a1c6006f29871d34079979061fd2)` `[`operator()`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler_1ac10f7b49a94f71463c05dcbb15bab29a)`()` 

ask for signals. If more than one signal has been received the signal with the highest priority will be returned. Priorities are: USER1 > USER2 > STOP > TERMINATE.

#### `enum `[`SignalInfo`](#d5/d17/classalps_1_1scheduler_1_1_signal_handler_1ab9e6a1c6006f29871d34079979061fd2) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
NOSIGNAL            | 
USER1            | 
USER2            | 
STOP            | 
TERMINATE            | 

symbolic names for signals. SIGINT, SIGQUIT and SIGTERM are mapped to TERMINATE SIGTSTP is mapped to STOP SIGUSR1 is mapped to USER1 SIGUSR2 is mapped to USER2

# class `alps::scheduler::SimpleFactory` 

```
class alps::scheduler::SimpleFactory
  : public alps::scheduler::Factory
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`SimpleFactory`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory_1ab6653684eefab050b46e637bc18effc3)`()` | 
`public inline virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory_1a63795b9a92bf6083cba629c7aac6e3d0)`(const ProcessList & w,const boost::filesystem::path & fn) const` | 
`public inline virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory_1ade27f97f1252e0f4ad3f82a55634bb0b)`(const ProcessList & w,const Parameters & p) const` | 
`public inline virtual void `[`print_copyright`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory_1afa9e742f92f09f640c9f578c75cfa972)`(std::ostream & out) const` | 

## Members

#### `public inline  `[`SimpleFactory`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory_1ab6653684eefab050b46e637bc18effc3)`()` 

#### `public inline virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory_1a63795b9a92bf6083cba629c7aac6e3d0)`(const ProcessList & w,const boost::filesystem::path & fn) const` 

#### `public inline virtual `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task)` * `[`make_task`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory_1ade27f97f1252e0f4ad3f82a55634bb0b)`(const ProcessList & w,const Parameters & p) const` 

#### `public inline virtual void `[`print_copyright`](#d4/d23/classalps_1_1scheduler_1_1_simple_factory_1afa9e742f92f09f640c9f578c75cfa972)`(std::ostream & out) const` 

# class `alps::scheduler::SimpleMCFactory` 

```
class alps::scheduler::SimpleMCFactory
  : public alps::scheduler::BasicFactory< MCSimulation, WORKER >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`SimpleMCFactory`](#d3/dda/classalps_1_1scheduler_1_1_simple_m_c_factory_1a95aceb4f8c658a63049fd72ae0970fa8)`()` | 

## Members

#### `public inline  `[`SimpleMCFactory`](#d3/dda/classalps_1_1scheduler_1_1_simple_m_c_factory_1a95aceb4f8c658a63049fd72ae0970fa8)`()` 

# class `alps::scheduler::SingleScheduler` 

```
class alps::scheduler::SingleScheduler
  : public alps::scheduler::Scheduler
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`SingleScheduler`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a5d924a86d57470b01a195502c86e24ed)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` | 
`public  `[`~SingleScheduler`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a757887a9f861272f4cf271006ab78c92)`()` | 
`public virtual int `[`run`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a7f75e39dc19f6d159c6510ad86abaac9)`()` | 
`public void `[`create_task`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a8e729db0f6bdb0dcaa21d038f8231aba)`(Parameters const & p)` | 
`public void `[`destroy_task`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1afa8185aa1ef7f9f2a921070bc05e2c5c)`()` | 
`public inline virtual void `[`checkpoint`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a0119a2e04f5df82e8de856cce1cdc0a9)`()` | 
`public inline `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * `[`get_task`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a14ac7a0bde28de688e4ca11ccad064e4)`()` | 

## Members

#### `public  `[`SingleScheduler`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a5d924a86d57470b01a195502c86e24ed)`(const `[`NoJobfileOptions`](#db/dc0/classalps_1_1scheduler_1_1_no_jobfile_options)` &,const `[`Factory`](#db/d7b/classalps_1_1scheduler_1_1_factory)` &)` 

#### `public  `[`~SingleScheduler`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a757887a9f861272f4cf271006ab78c92)`()` 

#### `public virtual int `[`run`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a7f75e39dc19f6d159c6510ad86abaac9)`()` 

#### `public void `[`create_task`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a8e729db0f6bdb0dcaa21d038f8231aba)`(Parameters const & p)` 

#### `public void `[`destroy_task`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1afa8185aa1ef7f9f2a921070bc05e2c5c)`()` 

#### `public inline virtual void `[`checkpoint`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a0119a2e04f5df82e8de856cce1cdc0a9)`()` 

#### `public inline `[`AbstractTask`](#d6/d4f/classalps_1_1scheduler_1_1_abstract_task)` * `[`get_task`](#d7/d7b/classalps_1_1scheduler_1_1_single_scheduler_1a14ac7a0bde28de688e4ca11ccad064e4)`()` 

# class `alps::scheduler::SlaveTask` 

```
class alps::scheduler::SlaveTask
  : public alps::scheduler::AbstractTask
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`SlaveTask`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1ad5c772a9e994844fbeace3c6890799da)`(const Process &)` | 
`public virtual void `[`run`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1adb1e190045ef7fc0feb5f4739ff8f94c)`()` | 
`public virtual void `[`checkpoint`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a14ea0525837b563292ce8b89fe0f944f)`(const boost::filesystem::path & fn,bool) const` | 
`public virtual void `[`add_process`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a8af6a92c5fd167982a81f472b95086bf)`(const Process & p)` | 
`public virtual void `[`start`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a68bd076060e0e1a6a3b480a1879fc783)`()` | 
`public virtual double `[`work`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1ad72c90e4d03e7a86886e5d787dd2030d)`() const` | 
`public virtual bool `[`finished`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a8787d89adce7c2b4f3a94f5145d6cb23)`(double & x,double &) const` | 
`public virtual void `[`halt`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a364a3ae2db10e5ae31efa4fdcbb719c6)`()` | 
`public virtual uint32_t `[`cpus`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a1db66add9313f834948c18234cc27807)`() const` | 
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a225aefbaebdce583050a7153989f52ec)`() const` | 

## Members

#### `public  `[`SlaveTask`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1ad5c772a9e994844fbeace3c6890799da)`(const Process &)` 

#### `public virtual void `[`run`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1adb1e190045ef7fc0feb5f4739ff8f94c)`()` 

#### `public virtual void `[`checkpoint`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a14ea0525837b563292ce8b89fe0f944f)`(const boost::filesystem::path & fn,bool) const` 

#### `public virtual void `[`add_process`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a8af6a92c5fd167982a81f472b95086bf)`(const Process & p)` 

#### `public virtual void `[`start`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a68bd076060e0e1a6a3b480a1879fc783)`()` 

#### `public virtual double `[`work`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1ad72c90e4d03e7a86886e5d787dd2030d)`() const` 

#### `public virtual bool `[`finished`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a8787d89adce7c2b4f3a94f5145d6cb23)`(double & x,double &) const` 

#### `public virtual void `[`halt`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a364a3ae2db10e5ae31efa4fdcbb719c6)`()` 

#### `public virtual uint32_t `[`cpus`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a1db66add9313f834948c18234cc27807)`() const` 

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d7/d2c/classalps_1_1scheduler_1_1_slave_task_1a225aefbaebdce583050a7153989f52ec)`() const` 

# class `alps::scheduler::Task` 

```
class alps::scheduler::Task
  : public alps::scheduler::AbstractTask
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task_1aa6e4412406567f87b603726b64aab8da)`(const ProcessList &,const boost::filesystem::path &)` | 
`public  `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task_1a1a83844d9f80d784b6410baaf12ade56)`(const ProcessList &,const Parameters &)` | 
`public  `[`~Task`](#d5/de3/classalps_1_1scheduler_1_1_task_1aaa7f65007f5f551ae374ea3f3f996433)`()` | 
`public virtual void `[`construct`](#d5/de3/classalps_1_1scheduler_1_1_task_1abde50275d747acd33b82e01f54b5087e)`()` | 
`public virtual void `[`checkpoint`](#d5/de3/classalps_1_1scheduler_1_1_task_1adc6344d42f3aacf9c116560201a793a1)`(const boost::filesystem::path &,bool) const` | 
`public void `[`checkpoint_hdf5`](#d5/de3/classalps_1_1scheduler_1_1_task_1a7f596c4eb8946025f67e3f75dedf57df)`(const boost::filesystem::path &) const` | 
`public void `[`checkpoint_xml`](#d5/de3/classalps_1_1scheduler_1_1_task_1abe5595541fd63db8efe4ef55dcfa7618)`(const boost::filesystem::path &,bool) const` | 
`public virtual void `[`add_process`](#d5/de3/classalps_1_1scheduler_1_1_task_1af6a6e58ab119aad9f71c4f92360ad5b8)`(const Process &)` | 
`public inline virtual uint32_t `[`cpus`](#d5/de3/classalps_1_1scheduler_1_1_task_1a67b4780072fcbf6694f1b9a2e80357d2)`() const` | 
`public inline virtual bool `[`local`](#d5/de3/classalps_1_1scheduler_1_1_task_1a0f5dada03a82430e1904770cbd9b110b)`()` | 
`public const alps::Parameters & `[`get_parameters`](#d5/de3/classalps_1_1scheduler_1_1_task_1a2132fbca72622574d6f5b4aa3e6ccc7c)`() const` | 
`public virtual void `[`start`](#d5/de3/classalps_1_1scheduler_1_1_task_1a30692e570fab69f9504cbbc608dfc47c)`()` | 
`public virtual void `[`run`](#d5/de3/classalps_1_1scheduler_1_1_task_1a83a8142eb13354b33dd2eb601f5eea83)`()` | 
`public void `[`dostep`](#d5/de3/classalps_1_1scheduler_1_1_task_1a9692ee30cb04f518d130034387468d15)`()` | 
`public void `[`finish`](#d5/de3/classalps_1_1scheduler_1_1_task_1aa00a50d59ef4d9496969867aa720bf3b)`()` | 
`public inline bool `[`finished`](#d5/de3/classalps_1_1scheduler_1_1_task_1a28b1d90bc54d1daec6aedceb545f69ca)`() const` | 
`public virtual bool `[`finished`](#d5/de3/classalps_1_1scheduler_1_1_task_1a226bfa85ed5ad922f6a95150e31ce058)`(double &,double &) const` | 
`public inline bool `[`started`](#d5/de3/classalps_1_1scheduler_1_1_task_1ac1c3935d71e4d9e5318adb5893c7141d)`() const` | 
`public virtual void `[`halt`](#d5/de3/classalps_1_1scheduler_1_1_task_1a902cd785afb13d42399a679a8fcb8c58)`()` | 
`public virtual double `[`work`](#d5/de3/classalps_1_1scheduler_1_1_task_1a5213ff4961d3287283da23fe02860eab)`() const` | 
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d5/de3/classalps_1_1scheduler_1_1_task_1addea57d2ba10c147c69d336087765fbe)`() const` | 
`public virtual void `[`load`](#d5/de3/classalps_1_1scheduler_1_1_task_1a12d8180e36298cd927d51bdc323e7734)`(hdf5::archive &)` | 
`public virtual void `[`save`](#d5/de3/classalps_1_1scheduler_1_1_task_1ae420a2e72229eefd91bebd27d08681dd)`(hdf5::archive &) const` | 
`protected alps::Parameters `[`parms`](#d5/de3/classalps_1_1scheduler_1_1_task_1a9280f8ad2a5680ac9d1770ca1b01e3f6) | 
`protected bool `[`finished_`](#d5/de3/classalps_1_1scheduler_1_1_task_1aea5c487fa5c1edd70e414a97bf2cbb8f) | 
`protected boost::filesystem::path `[`infilename`](#d5/de3/classalps_1_1scheduler_1_1_task_1a4f385c8ff2e0d217bfd057fe6f633d10) | 
`protected bool `[`from_file`](#d5/de3/classalps_1_1scheduler_1_1_task_1a77c91355a036a96af2e2f53d692b8754) | 
`protected virtual void `[`write_xml_header`](#d5/de3/classalps_1_1scheduler_1_1_task_1a764d1b458452910adf0a2aaffc7de425)`(alps::oxstream &) const` | 
`protected virtual void `[`write_xml_trailer`](#d5/de3/classalps_1_1scheduler_1_1_task_1a6f71c73fef84e4a324482dab278cc034)`(alps::oxstream &) const` | 
`protected void `[`write_xml_body`](#d5/de3/classalps_1_1scheduler_1_1_task_1a176a6fe4ac9337988466ab76770740ce)`(alps::oxstream &,boost::filesystem::path const & fn,bool writeall) const` | 
`protected virtual void `[`handle_tag`](#d5/de3/classalps_1_1scheduler_1_1_task_1a2d3f675776d5b7ab0fec8b72a9d469c8)`(std::istream &,const XMLTag &)` | 

## Members

#### `public  `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task_1aa6e4412406567f87b603726b64aab8da)`(const ProcessList &,const boost::filesystem::path &)` 

#### `public  `[`Task`](#d5/de3/classalps_1_1scheduler_1_1_task_1a1a83844d9f80d784b6410baaf12ade56)`(const ProcessList &,const Parameters &)` 

#### `public  `[`~Task`](#d5/de3/classalps_1_1scheduler_1_1_task_1aaa7f65007f5f551ae374ea3f3f996433)`()` 

#### `public virtual void `[`construct`](#d5/de3/classalps_1_1scheduler_1_1_task_1abde50275d747acd33b82e01f54b5087e)`()` 

#### `public virtual void `[`checkpoint`](#d5/de3/classalps_1_1scheduler_1_1_task_1adc6344d42f3aacf9c116560201a793a1)`(const boost::filesystem::path &,bool) const` 

#### `public void `[`checkpoint_hdf5`](#d5/de3/classalps_1_1scheduler_1_1_task_1a7f596c4eb8946025f67e3f75dedf57df)`(const boost::filesystem::path &) const` 

#### `public void `[`checkpoint_xml`](#d5/de3/classalps_1_1scheduler_1_1_task_1abe5595541fd63db8efe4ef55dcfa7618)`(const boost::filesystem::path &,bool) const` 

#### `public virtual void `[`add_process`](#d5/de3/classalps_1_1scheduler_1_1_task_1af6a6e58ab119aad9f71c4f92360ad5b8)`(const Process &)` 

#### `public inline virtual uint32_t `[`cpus`](#d5/de3/classalps_1_1scheduler_1_1_task_1a67b4780072fcbf6694f1b9a2e80357d2)`() const` 

#### `public inline virtual bool `[`local`](#d5/de3/classalps_1_1scheduler_1_1_task_1a0f5dada03a82430e1904770cbd9b110b)`()` 

#### `public const alps::Parameters & `[`get_parameters`](#d5/de3/classalps_1_1scheduler_1_1_task_1a2132fbca72622574d6f5b4aa3e6ccc7c)`() const` 

#### `public virtual void `[`start`](#d5/de3/classalps_1_1scheduler_1_1_task_1a30692e570fab69f9504cbbc608dfc47c)`()` 

#### `public virtual void `[`run`](#d5/de3/classalps_1_1scheduler_1_1_task_1a83a8142eb13354b33dd2eb601f5eea83)`()` 

#### `public void `[`dostep`](#d5/de3/classalps_1_1scheduler_1_1_task_1a9692ee30cb04f518d130034387468d15)`()` 

#### `public void `[`finish`](#d5/de3/classalps_1_1scheduler_1_1_task_1aa00a50d59ef4d9496969867aa720bf3b)`()` 

#### `public inline bool `[`finished`](#d5/de3/classalps_1_1scheduler_1_1_task_1a28b1d90bc54d1daec6aedceb545f69ca)`() const` 

#### `public virtual bool `[`finished`](#d5/de3/classalps_1_1scheduler_1_1_task_1a226bfa85ed5ad922f6a95150e31ce058)`(double &,double &) const` 

#### `public inline bool `[`started`](#d5/de3/classalps_1_1scheduler_1_1_task_1ac1c3935d71e4d9e5318adb5893c7141d)`() const` 

#### `public virtual void `[`halt`](#d5/de3/classalps_1_1scheduler_1_1_task_1a902cd785afb13d42399a679a8fcb8c58)`()` 

#### `public virtual double `[`work`](#d5/de3/classalps_1_1scheduler_1_1_task_1a5213ff4961d3287283da23fe02860eab)`() const` 

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d5/de3/classalps_1_1scheduler_1_1_task_1addea57d2ba10c147c69d336087765fbe)`() const` 

#### `public virtual void `[`load`](#d5/de3/classalps_1_1scheduler_1_1_task_1a12d8180e36298cd927d51bdc323e7734)`(hdf5::archive &)` 

#### `public virtual void `[`save`](#d5/de3/classalps_1_1scheduler_1_1_task_1ae420a2e72229eefd91bebd27d08681dd)`(hdf5::archive &) const` 

#### `protected alps::Parameters `[`parms`](#d5/de3/classalps_1_1scheduler_1_1_task_1a9280f8ad2a5680ac9d1770ca1b01e3f6) 

#### `protected bool `[`finished_`](#d5/de3/classalps_1_1scheduler_1_1_task_1aea5c487fa5c1edd70e414a97bf2cbb8f) 

#### `protected boost::filesystem::path `[`infilename`](#d5/de3/classalps_1_1scheduler_1_1_task_1a4f385c8ff2e0d217bfd057fe6f633d10) 

#### `protected bool `[`from_file`](#d5/de3/classalps_1_1scheduler_1_1_task_1a77c91355a036a96af2e2f53d692b8754) 

#### `protected virtual void `[`write_xml_header`](#d5/de3/classalps_1_1scheduler_1_1_task_1a764d1b458452910adf0a2aaffc7de425)`(alps::oxstream &) const` 

#### `protected virtual void `[`write_xml_trailer`](#d5/de3/classalps_1_1scheduler_1_1_task_1a6f71c73fef84e4a324482dab278cc034)`(alps::oxstream &) const` 

#### `protected void `[`write_xml_body`](#d5/de3/classalps_1_1scheduler_1_1_task_1a176a6fe4ac9337988466ab76770740ce)`(alps::oxstream &,boost::filesystem::path const & fn,bool writeall) const` 

#### `protected virtual void `[`handle_tag`](#d5/de3/classalps_1_1scheduler_1_1_task_1a2d3f675776d5b7ab0fec8b72a9d469c8)`(std::istream &,const XMLTag &)` 

# class `alps::scheduler::TaskInfo` 

```
class alps::scheduler::TaskInfo
  : public std::vector< Info >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1a11c791dd448a5508460da1f6f13c4459)`()` | 
`public void `[`start`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1a411c6d45bd483f6c200f372e37ef6fda)`(const std::string &)` | 
`public void `[`halt`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1ae5443c48d21b1c0a5608e26fd833dd7a)`()` | 
`public void `[`save`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1ae35ecd13da4dcde95645232250018a67)`(hdf5::archive &) const` | 
`public void `[`load`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1a01beccfeef3427ff27f80a44470c09bc)`(hdf5::archive &)` | 
`public void `[`save`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1a3ebd93f090fcd4e2dfd5cc0b050a9cfc)`(ODump & dump) const` | 
`public void `[`load`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1abc69602263748787c7afc58cb10a11e3)`(IDump & dump,int version)` | 
`public void `[`write_xml`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1ad4a702ea6c8c85f68b04d2e0aa5abb53)`(alps::oxstream &) const` | 

## Members

#### `public inline  `[`TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1a11c791dd448a5508460da1f6f13c4459)`()` 

#### `public void `[`start`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1a411c6d45bd483f6c200f372e37ef6fda)`(const std::string &)` 

#### `public void `[`halt`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1ae5443c48d21b1c0a5608e26fd833dd7a)`()` 

#### `public void `[`save`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1ae35ecd13da4dcde95645232250018a67)`(hdf5::archive &) const` 

#### `public void `[`load`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1a01beccfeef3427ff27f80a44470c09bc)`(hdf5::archive &)` 

#### `public void `[`save`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1a3ebd93f090fcd4e2dfd5cc0b050a9cfc)`(ODump & dump) const` 

#### `public void `[`load`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1abc69602263748787c7afc58cb10a11e3)`(IDump & dump,int version)` 

#### `public void `[`write_xml`](#d2/dfa/classalps_1_1scheduler_1_1_task_info_1ad4a702ea6c8c85f68b04d2e0aa5abb53)`(alps::oxstream &) const` 

# class `alps::scheduler::Worker` 

```
class alps::scheduler::Worker
  : public alps::scheduler::AbstractWorker
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a91a1fdb40aeff22dab646364e891bc6d)`(const ProcessList &,const Parameters &,int32_t)` | 
`public  `[`Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a601aae9e44e957aa3d8b9fd6e98ef726)`(const Parameters &,int32_t)` | 
`public virtual  `[`~Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a65146a3a85bec3dff9852b26863f0764)`()` | 
`public virtual void `[`set_parameters`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aeb255fe6f3be3919fb39919f0510e601)`(const Parameters & parms)` | 
`public virtual bool `[`change_parameter`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a7b3bddd42d274cfe84d4b8106feaf132)`(const std::string & name,const StringValue & value)` | 
`public virtual void `[`save_worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aef241652aa2706a32f51645b188c0b9f)`(ODump &) const` | 
`public virtual void `[`load_worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a6fff3e8b0af892906109d4a46eb6b95d)`(IDump &)` | 
`public virtual void `[`save`](#d8/d00/classalps_1_1scheduler_1_1_worker_1abf9bdffe7b1f8d924ee763f46cce97be)`(hdf5::archive &) const` | 
`public virtual void `[`load`](#d8/d00/classalps_1_1scheduler_1_1_worker_1ac3bf870b3c6d83838732d73d0096e25c)`(hdf5::archive &)` | 
`public virtual void `[`write_xml`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a2b4658353af6603e53d42dbc37132b1b)`(const boost::filesystem::path & name) const` | 
`public virtual void `[`save_to_file`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a6f86ca2a77f2308b868247fa901d2b75)`(const boost::filesystem::path &,const boost::filesystem::path &) const` | 
`public virtual void `[`load_from_file`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a8d6a885fcd890567bb048399d7cd311b)`(const boost::filesystem::path &,const boost::filesystem::path &)` | 
`public virtual `[`TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info)` `[`get_info`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a9eb6408026396372c2a712f7d8e7b34d)`() const` | 
`public virtual void `[`start_worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aa2ad22302d72754c2baac7644357cef2)`()` | 
`public virtual void `[`halt_worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a25d138bffa09c4920e584a8ec0e74fbb)`()` | 
`public inline virtual void `[`start`](#d8/d00/classalps_1_1scheduler_1_1_worker_1ae00d94ac2fef41d74feb5dbf149d5d70)`()` | 
`public inline virtual void `[`halt`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a5711bfea8bafa0cb726977004b75f0ab)`()` | 
`public virtual std::string `[`work_phase`](#d8/d00/classalps_1_1scheduler_1_1_worker_1afaa40412dcefca97cb8f06dc2f549b7d)`()` | 
`public void `[`change_phase`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aa84008c7afe2efb0e1ec6c0af8ff3a8c)`(const std::string &)` | 
`public virtual void `[`run`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a938024570049a2aad309d050d7b7a52a)`()` | 
`public virtual bool `[`handle_message`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aae303509ab68c4bf39565005bed86cc0)`(const Process & runmaster,int32_t tag)` | 
`public virtual void `[`dostep`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aeaa85c91d4066c8dddd04e94e1a801f9)`()` | 
`public virtual double `[`work_done`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a73616f714b1dca60c112770bac7128f8)`() const` | 
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d8/d00/classalps_1_1scheduler_1_1_worker_1abf107e1f410a80091fbf16e38777681f)`() const` | 
`protected int32_t `[`version`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a0b326ecb40ca12905c347df3860252e3) | 
`protected int32_t `[`user_version`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a4c720213466148084705f588990d6710) | 
`protected int `[`node`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a570789c7b5d1190f426375688763db1d) | 
`protected Parameters `[`parms`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a5d574fb007e693655dea071131c877d8) | 
`protected ProcessList `[`where`](#d8/d00/classalps_1_1scheduler_1_1_worker_1afe65f6bc5fbc961cb3e9cb6652d658a0) | 
`protected mutable boost::shared_ptr< engine_type > `[`engine_ptr`](#d8/d00/classalps_1_1scheduler_1_1_worker_1abc76c93f27766d04ac8adabe27fdee72) | 
`protected mutable boost::variate_generator< engine_type &, boost::uniform_real<> > `[`random`](#d8/d00/classalps_1_1scheduler_1_1_worker_1abc511eb33fb9e72792bbf59dda8deabf) | 
`protected mutable boost::variate_generator< engine_type &, boost::uniform_real<> > `[`random_01`](#d8/d00/classalps_1_1scheduler_1_1_worker_1ac008caaf593042d96390e8b09278553c) | 
`protected inline double `[`random_real`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a9b33c2047d1a61f153d2da646873cc27)`(double a,double b)` | 
`protected inline int `[`random_int`](#d8/d00/classalps_1_1scheduler_1_1_worker_1afdaffb26f8dc08f22f96a3df116c0b44)`(int a,int b)` | 
`protected inline int `[`random_int`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a27d1c414c427c6949bd797039c7be481)`(int n)` | 

## Members

#### `public  `[`Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a91a1fdb40aeff22dab646364e891bc6d)`(const ProcessList &,const Parameters &,int32_t)` 

#### `public  `[`Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a601aae9e44e957aa3d8b9fd6e98ef726)`(const Parameters &,int32_t)` 

#### `public virtual  `[`~Worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a65146a3a85bec3dff9852b26863f0764)`()` 

#### `public virtual void `[`set_parameters`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aeb255fe6f3be3919fb39919f0510e601)`(const Parameters & parms)` 

#### `public virtual bool `[`change_parameter`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a7b3bddd42d274cfe84d4b8106feaf132)`(const std::string & name,const StringValue & value)` 

#### `public virtual void `[`save_worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aef241652aa2706a32f51645b188c0b9f)`(ODump &) const` 

#### `public virtual void `[`load_worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a6fff3e8b0af892906109d4a46eb6b95d)`(IDump &)` 

#### `public virtual void `[`save`](#d8/d00/classalps_1_1scheduler_1_1_worker_1abf9bdffe7b1f8d924ee763f46cce97be)`(hdf5::archive &) const` 

#### `public virtual void `[`load`](#d8/d00/classalps_1_1scheduler_1_1_worker_1ac3bf870b3c6d83838732d73d0096e25c)`(hdf5::archive &)` 

#### `public virtual void `[`write_xml`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a2b4658353af6603e53d42dbc37132b1b)`(const boost::filesystem::path & name) const` 

#### `public virtual void `[`save_to_file`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a6f86ca2a77f2308b868247fa901d2b75)`(const boost::filesystem::path &,const boost::filesystem::path &) const` 

#### `public virtual void `[`load_from_file`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a8d6a885fcd890567bb048399d7cd311b)`(const boost::filesystem::path &,const boost::filesystem::path &)` 

#### `public virtual `[`TaskInfo`](#d2/dfa/classalps_1_1scheduler_1_1_task_info)` `[`get_info`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a9eb6408026396372c2a712f7d8e7b34d)`() const` 

#### `public virtual void `[`start_worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aa2ad22302d72754c2baac7644357cef2)`()` 

#### `public virtual void `[`halt_worker`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a25d138bffa09c4920e584a8ec0e74fbb)`()` 

#### `public inline virtual void `[`start`](#d8/d00/classalps_1_1scheduler_1_1_worker_1ae00d94ac2fef41d74feb5dbf149d5d70)`()` 

#### `public inline virtual void `[`halt`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a5711bfea8bafa0cb726977004b75f0ab)`()` 

#### `public virtual std::string `[`work_phase`](#d8/d00/classalps_1_1scheduler_1_1_worker_1afaa40412dcefca97cb8f06dc2f549b7d)`()` 

#### `public void `[`change_phase`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aa84008c7afe2efb0e1ec6c0af8ff3a8c)`(const std::string &)` 

#### `public virtual void `[`run`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a938024570049a2aad309d050d7b7a52a)`()` 

#### `public virtual bool `[`handle_message`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aae303509ab68c4bf39565005bed86cc0)`(const Process & runmaster,int32_t tag)` 

#### `public virtual void `[`dostep`](#d8/d00/classalps_1_1scheduler_1_1_worker_1aeaa85c91d4066c8dddd04e94e1a801f9)`()` 

#### `public virtual double `[`work_done`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a73616f714b1dca60c112770bac7128f8)`() const` 

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d8/d00/classalps_1_1scheduler_1_1_worker_1abf107e1f410a80091fbf16e38777681f)`() const` 

#### `protected int32_t `[`version`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a0b326ecb40ca12905c347df3860252e3) 

#### `protected int32_t `[`user_version`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a4c720213466148084705f588990d6710) 

#### `protected int `[`node`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a570789c7b5d1190f426375688763db1d) 

#### `protected Parameters `[`parms`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a5d574fb007e693655dea071131c877d8) 

#### `protected ProcessList `[`where`](#d8/d00/classalps_1_1scheduler_1_1_worker_1afe65f6bc5fbc961cb3e9cb6652d658a0) 

#### `protected mutable boost::shared_ptr< engine_type > `[`engine_ptr`](#d8/d00/classalps_1_1scheduler_1_1_worker_1abc76c93f27766d04ac8adabe27fdee72) 

#### `protected mutable boost::variate_generator< engine_type &, boost::uniform_real<> > `[`random`](#d8/d00/classalps_1_1scheduler_1_1_worker_1abc511eb33fb9e72792bbf59dda8deabf) 

#### `protected mutable boost::variate_generator< engine_type &, boost::uniform_real<> > `[`random_01`](#d8/d00/classalps_1_1scheduler_1_1_worker_1ac008caaf593042d96390e8b09278553c) 

#### `protected inline double `[`random_real`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a9b33c2047d1a61f153d2da646873cc27)`(double a,double b)` 

#### `protected inline int `[`random_int`](#d8/d00/classalps_1_1scheduler_1_1_worker_1afdaffb26f8dc08f22f96a3df116c0b44)`(int a,int b)` 

#### `protected inline int `[`random_int`](#d8/d00/classalps_1_1scheduler_1_1_worker_1a27d1c414c427c6949bd797039c7be481)`(int n)` 

# class `alps::scheduler::WorkerTask` 

```
class alps::scheduler::WorkerTask
  : public alps::scheduler::Task
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public std::vector< `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker)` * > `[`runs`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a121af6f8c360e63861f3bad19e89d11d) | 
`public  `[`WorkerTask`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a35c405eaa98071505cb9ca07340ea4fb)`(const ProcessList &,const boost::filesystem::path &)` | 
`public  `[`WorkerTask`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a2c9d69d5826fc0b5562377ff2f988df5)`(const ProcessList &,const Parameters &)` | 
`public  `[`~WorkerTask`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ae7eabbe999038e78114a355fa342b7bf)`()` | 
`public virtual void `[`construct`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a841376b77f0a81bd9697c3c353de71ae)`()` | 
`public virtual void `[`add_process`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a9e73c56eed99999bfac1388abffecc63)`(const Process &)` | 
`public virtual void `[`start`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a771ca36613df6e458a991d657f395bb5)`()` | 
`public virtual void `[`dostep`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ae259142891c4a2c4a57d5cfd4d2445ed)`()` | 
`public virtual bool `[`finished`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ab5ee2714eea5017481bc78b06cf388ee)`(double &,double &) const` | 
`public virtual void `[`halt`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ace26f385d06ab81ce168081d844d6e08)`()` | 
`public virtual double `[`work`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ab6f0901a57813e12b4c655b5a53d958f)`() const` | 
`public double `[`work_done`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1acab551b6b0e01c70626166eba0e5e01f)`() const` | 
`public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a64b7c36a489846a5cd6fbfe95e25654a)`() const` | 
`protected std::vector< RunStatus > `[`workerstatus`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a4593cf6852b93a5601727bca3d676127) | 
`protected std::string `[`worker_tag`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a79c8c69e272385834edf3874fa1fca19)`() const` | 
`protected virtual void `[`write_xml_body`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1af311bbaa8a867fe0b2409a7f6637614e)`(alps::oxstream &,boost::filesystem::path const &,bool writeall) const` | 
`protected virtual void `[`handle_tag`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1adef3e2aa6ac52ee5d33c40a9e594c715)`(std::istream &,const XMLTag &)` | 
`enum `[`RunStatus`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a85e646e9290dc33e1114a07e879e096e) | 

## Members

#### `public std::vector< `[`AbstractWorker`](#db/d77/classalps_1_1scheduler_1_1_abstract_worker)` * > `[`runs`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a121af6f8c360e63861f3bad19e89d11d) 

#### `public  `[`WorkerTask`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a35c405eaa98071505cb9ca07340ea4fb)`(const ProcessList &,const boost::filesystem::path &)` 

#### `public  `[`WorkerTask`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a2c9d69d5826fc0b5562377ff2f988df5)`(const ProcessList &,const Parameters &)` 

#### `public  `[`~WorkerTask`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ae7eabbe999038e78114a355fa342b7bf)`()` 

#### `public virtual void `[`construct`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a841376b77f0a81bd9697c3c353de71ae)`()` 

#### `public virtual void `[`add_process`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a9e73c56eed99999bfac1388abffecc63)`(const Process &)` 

#### `public virtual void `[`start`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a771ca36613df6e458a991d657f395bb5)`()` 

#### `public virtual void `[`dostep`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ae259142891c4a2c4a57d5cfd4d2445ed)`()` 

#### `public virtual bool `[`finished`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ab5ee2714eea5017481bc78b06cf388ee)`(double &,double &) const` 

#### `public virtual void `[`halt`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ace26f385d06ab81ce168081d844d6e08)`()` 

#### `public virtual double `[`work`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1ab6f0901a57813e12b4c655b5a53d958f)`() const` 

#### `public double `[`work_done`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1acab551b6b0e01c70626166eba0e5e01f)`() const` 

#### `public virtual `[`ResultType`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`get_summary`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a64b7c36a489846a5cd6fbfe95e25654a)`() const` 

#### `protected std::vector< RunStatus > `[`workerstatus`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a4593cf6852b93a5601727bca3d676127) 

#### `protected std::string `[`worker_tag`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a79c8c69e272385834edf3874fa1fca19)`() const` 

#### `protected virtual void `[`write_xml_body`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1af311bbaa8a867fe0b2409a7f6637614e)`(alps::oxstream &,boost::filesystem::path const &,bool writeall) const` 

#### `protected virtual void `[`handle_tag`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1adef3e2aa6ac52ee5d33c40a9e594c715)`(std::istream &,const XMLTag &)` 

#### `enum `[`RunStatus`](#d9/d91/classalps_1_1scheduler_1_1_worker_task_1a85e646e9290dc33e1114a07e879e096e) 

 Values                         | Descriptions                                
--------------------------------|---------------------------------------------
RunNotExisting            | 
LocalRun            | 
RemoteRun            | 
RunOnDump            | 

# struct `alps::scheduler::CheckpointFiles` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public boost::filesystem::path `[`in`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files_1a367de30dd105642c25b370133633ba56) | 
`public boost::filesystem::path `[`out`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files_1ac6c9afabd86f865b719ba28e8a11a96d) | 
`public boost::filesystem::path `[`hdf5in`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files_1aad492a0b6e9905471aeea90af71f82a2) | 
`public boost::filesystem::path `[`hdf5out`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files_1a5c867fc8d38efeab1356ce77e0d5df46) | 

## Members

#### `public boost::filesystem::path `[`in`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files_1a367de30dd105642c25b370133633ba56) 

#### `public boost::filesystem::path `[`out`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files_1ac6c9afabd86f865b719ba28e8a11a96d) 

#### `public boost::filesystem::path `[`hdf5in`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files_1aad492a0b6e9905471aeea90af71f82a2) 

#### `public boost::filesystem::path `[`hdf5out`](#d0/d2d/structalps_1_1scheduler_1_1_checkpoint_files_1a5c867fc8d38efeab1356ce77e0d5df46) 

# struct `alps::scheduler::rt` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public double `[`T`](#db/d9e/structalps_1_1scheduler_1_1rt_1a0ce7bf186008278c7059ca11bb4ed11f) | 
`public double `[`mean`](#db/d9e/structalps_1_1scheduler_1_1rt_1a670b7fed3ec2901a282e5527df5d9c14) | 
`public double `[`error`](#db/d9e/structalps_1_1scheduler_1_1rt_1a7900a5469ad3edb65527fdea912158b1) | 
`public double `[`count`](#db/d9e/structalps_1_1scheduler_1_1rt_1aac21cf25f36222abb24d99c9f064efd3) | 
`public inline `[`rt`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`operator+=`](#db/d9e/structalps_1_1scheduler_1_1rt_1ab99144d9a5fe710e5652ad67663ed7f3)`(const `[`rt`](#db/d9e/structalps_1_1scheduler_1_1rt)` c)` | 

## Members

#### `public double `[`T`](#db/d9e/structalps_1_1scheduler_1_1rt_1a0ce7bf186008278c7059ca11bb4ed11f) 

#### `public double `[`mean`](#db/d9e/structalps_1_1scheduler_1_1rt_1a670b7fed3ec2901a282e5527df5d9c14) 

#### `public double `[`error`](#db/d9e/structalps_1_1scheduler_1_1rt_1a7900a5469ad3edb65527fdea912158b1) 

#### `public double `[`count`](#db/d9e/structalps_1_1scheduler_1_1rt_1aac21cf25f36222abb24d99c9f064efd3) 

#### `public inline `[`rt`](#db/d9e/structalps_1_1scheduler_1_1rt)` `[`operator+=`](#db/d9e/structalps_1_1scheduler_1_1rt_1ab99144d9a5fe710e5652ad67663ed7f3)`(const `[`rt`](#db/d9e/structalps_1_1scheduler_1_1rt)` c)` 

# struct `alps::scheduler::TaskStatus` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public int32_t `[`number`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1aa66827e2c0ff51b30b93c7da1da5ffb4) | 
`public uint32_t `[`cpus`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1a649e31d3bd097e552097b92e6fd0c1dd) | 
`public boost::posix_time::ptime `[`next_check`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1ab8521142fac076073d2c96c2d8aabd6e) | 
`public double `[`work`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1a401b54a56b5b4e208f8854b054b0170c) | 
`public ProcessList `[`where`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1a2cd55b18f12f9d0dba905615efa4f87c) | 
`public inline  `[`TaskStatus`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1aac33a5a611b23aab98994c46735e8a10)`()` | 

## Members

#### `public int32_t `[`number`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1aa66827e2c0ff51b30b93c7da1da5ffb4) 

#### `public uint32_t `[`cpus`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1a649e31d3bd097e552097b92e6fd0c1dd) 

#### `public boost::posix_time::ptime `[`next_check`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1ab8521142fac076073d2c96c2d8aabd6e) 

#### `public double `[`work`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1a401b54a56b5b4e208f8854b054b0170c) 

#### `public ProcessList `[`where`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1a2cd55b18f12f9d0dba905615efa4f87c) 

#### `public inline  `[`TaskStatus`](#db/d7e/structalps_1_1scheduler_1_1_task_status_1aac33a5a611b23aab98994c46735e8a10)`()` 

Generated by [Moxygen](https://sourcey.com/moxygen)
