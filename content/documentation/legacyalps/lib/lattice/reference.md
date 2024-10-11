
---
title: Reference
description: "ALPS Lattice Library"
weight: 2
---

# Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`namespace `[`alps`](#d8/d3d/namespacealps) | 
`namespace `[`alps::detail`](#d6/d75/namespacealps_1_1detail) | 
`namespace `[`alps::graph`](#dd/d26/namespacealps_1_1graph) | 
`namespace `[`boost`](#d4/da9/namespaceboost) | 
`class `[`alps::hypercubic_lattice::cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator) | 
`class `[`alps::hypercubic_lattice::momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator) | 

# namespace `alps` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>`inline std::pair< typename `[`coordinate_traits](#da/d24/structalps_1_1coordinate__traits)< C >::iterator, typename [coordinate_traits`](#da/d24/structalps_1_1coordinate__traits)`< C >::iterator > `[`coordinates`](#dc/da5/coordinate__traits_8h_1adbcf01b7c48c77e6872841c9751990e3)`(C & c)`            | 
`public template<>`  <br/>`inline std::pair< T *, T * > `[`coordinates`](#dc/da5/coordinate__traits_8h_1a1a7a19aef42281dbff6d72f1c7951f26)`(std::valarray< T > & c)`            | 
`public template<>`  <br/>`inline std::pair< const T *, const T * > `[`coordinates`](#dc/da5/coordinate__traits_8h_1a5818aabec6f4516eb30039b9d2a585e1)`(const std::valarray< T > & c)`            | 
`public template<>`  <br/>`std::string `[`coordinate_to_string`](#dc/da5/coordinate__traits_8h_1a3e63a296549d19faf64db8f82ed0cf3f)`(const C & c,int precision)`            | 
`public template<>`  <br/>`inline `[`dimensional_traits`](#d8/d28/structalps_1_1dimensional__traits)`< std::vector< T, A > >::dimension_type `[`dimension`](#d8/d27/dimensional__traits_8h_1a13c85a33649c811496bc74607f4b897c)`(const std::vector< T, A > & d)`            | 
`public template<>`  <br/>`void `[`disorder_vertices`](#d5/d64/disorder_8h_1a81428a7ee114e5e83c29846cb6726ed4)`(G & g,MAP & type)`            | 
`public template<>`  <br/>`void `[`disorder_edges`](#d5/d64/disorder_8h_1a3a87d6893db5ff915b175f744b8d1a50)`(G & g,MAP & type)`            | 
`public template<>`  <br/>`void `[`disorder_bonds`](#d5/d64/disorder_8h_1a9ec663156c456d4c8c2d9031aeacd80d)`(G & g,MAP & type)`            | 
`public template<>`  <br/>`void `[`disorder_sites`](#d5/d64/disorder_8h_1aca19f6e4d6d53a2ba6e2689b91f69aee)`(G & g,MAP & t)`            | 
`public inline alps::oxstream & `[`operator<<`](#d5/d64/disorder_8h_1a1f9e27b0f8c6a5a59c55598b98c4bb2f)`(alps::oxstream & out,const `[`alps::InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor)` & l)`            | 
`public inline std::ostream & `[`operator<<`](#d5/d64/disorder_8h_1a7baa7b9eb21b369a26a64888b7145b23)`(std::ostream & out,const `[`alps::InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor)` & l)`            | 
`public inline alps::oxstream & `[`operator<<`](#d5/d64/disorder_8h_1aea7c25657f64b3524d663b390154f144)`(alps::oxstream & out,const `[`alps::DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` & l)`            | 
`public inline std::ostream & `[`operator<<`](#d5/d64/disorder_8h_1ab35209ef8573439a2f3a8fbba2b1dbf3)`(std::ostream & out,const `[`alps::DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` & l)`            | 
`public template<>`  <br/>`inline void `[`write_graph_xml`](#d6/df3/graph_8h_1adf1a8d09c4fdf8d1d87f616a390c3d60)`(oxstream & out,const GRAPH & g,const std::string & n)`            | 
`public template<>`  <br/>`inline std::string `[`read_graph_xml`](#d6/df3/graph_8h_1a215fabf7d5f320ffc090001ef244aac3)`(std::istream & in,GRAPH & g)`            | 
`public template<>`  <br/>`inline std::string `[`read_graph_xml`](#d6/df3/graph_8h_1a450b14e91a981d283100a259988f29a4)`(const XMLTag & intag,std::istream & p,GRAPH & g)`            | 
`public template<>`  <br/>`inline void `[`copy_property`](#d6/df3/graph_8h_1aac33d03d4f9c69fd17ceb8a20b157423)`(PROPERTY,const SRC & s,const SRCREF & sr,DST & d,DSTREF & dr)`            | 
`public template<>`  <br/>`inline void `[`copy_property`](#d6/df3/graph_8h_1a4fdd97f36ebc3c52b83ba29d6a32fba6)`(PROPERTY,const SRC & s,DST & d)`            | 
`public template<>`  <br/>`inline void `[`copy_graph`](#d6/df3/graph_8h_1a2e912ff9ed6e9735713dc27daf9d9c30)`(const SRC & src,DST & dst)`            | 
`public template<>`  <br/>`inline int `[`constant_degree`](#d6/df3/graph_8h_1a8e9277e23f7ddbdfc2c9b39a386b3899)`(const G & g)`            | 
`public template<>`  <br/>`inline std::size_t `[`maximum_edge_type`](#d6/df3/graph_8h_1a5b7a71d17d09006f7836f3b1046528a0)`(const G & g)`            | 
`public template<>`  <br/>`inline std::size_t `[`maximum_vertex_type`](#d6/df3/graph_8h_1a073e9743cee7f9cfa7de26d0a9519ace)`(const G & g)`            | 
`public template<>`  <br/>`void `[`throw_if_xyz_defined`](#dd/d08/graph__helper_8h_1a1891aecbee7a0d4e26955f7e1cf944d9)`(const Parameters & p,const G & graph)`            | 
`public template<>`  <br/>`Parameters `[`coordinate_as_parameter`](#dd/d08/graph__helper_8h_1a087a82be1dcbffb98e2fdf022e4fe9e0)`(const G & graph,const typename boost::graph_traits< G >::vertex_descriptor & source,const typename boost::graph_traits< G >::vertex_descriptor & target)`            | 
`public template<>`  <br/>`Parameters `[`coordinate_as_parameter`](#dd/d08/graph__helper_8h_1ac1e85c1838edbc5e28679786fd08e7e5)`(const G & graph,const typename boost::graph_traits< G >::edge_descriptor & edge)`            | 
`public template<>`  <br/>`Parameters `[`coordinate_as_parameter`](#dd/d08/graph__helper_8h_1aa036a63c93c3e09cf31e007eda3b0e09)`(const G & graph,const typename boost::graph_traits< G >::vertex_descriptor & vertex)`            | 
`public template<>`  <br/>`std::string `[`site_label`](#dd/d08/graph__helper_8h_1a99137edd7aa5b4c6348ae802fd274f02)`(G const & g,typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor const & v,int precision)`            | 
`public template<>`  <br/>`std::vector< std::string > `[`site_labels`](#dd/d08/graph__helper_8h_1a3a721cfd39c7ccb52554993a8b981923)`(G const & g,int precision)`            | 
`public template<>`  <br/>`std::string `[`bond_label`](#dd/d08/graph__helper_8h_1a88ddd6a9b0b4419de29477a050d430e1)`(G const & g,typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bond_descriptor const & e,int precision)`            | 
`public template<>`  <br/>`std::vector< std::string > `[`bond_labels`](#dd/d08/graph__helper_8h_1a99a46b4c43f43c2cda6dfa5d3163da10)`(G const & g,int precision)`            | 
`public template<>`  <br/>`inline std::size_t `[`dimension`](#da/d35/hypercubic_8h_1a8423205556b64865fd17a64ee8df4e9b)`(const `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice)`< BASE, EX > & l)`            | 
`public template<>`  <br/>`inline const `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::unit_cell_type & `[`unit_cell`](#da/de0/lattice_8h_1ac014201b0d2a647c8b6597721978307e)`(const Lattice & l)`            | 
`public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor `[`cell`](#da/de0/lattice_8h_1ad811e162551ad41ff098bd23896563c2)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & o,const Lattice & l)`            | 
`public template<>`  <br/>`inline const `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & `[`offset`](#da/de0/lattice_8h_1ad289c470135364d8aa130071893e1695)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor & c,const Lattice &)`            | 
`public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::size_type `[`volume`](#da/de0/lattice_8h_1a6166089abc4ec783f8d7a45c7c8c16e5)`(const Lattice & l)`            | 
`public template<>`  <br/>`inline bool `[`on_lattice`](#da/de0/lattice_8h_1aed582d44d388d50983792cd696ffca28)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & o,const Lattice & l)`            | 
`public template<>`  <br/>`inline std::pair< typename `[`lattice_traits](#d5/d83/structalps_1_1lattice__traits)< Lattice >::cell_iterator, typename [lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_iterator > `[`cells`](#da/de0/lattice_8h_1a552cf28f449bd23fd13d21b6b7ca8380)`(const Lattice & l)`            | 
`public template<>`  <br/>`inline std::pair< bool, typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::boundary_crossing_type > `[`shift`](#da/de0/lattice_8h_1afbdf7c84422d52d236ca31ee15ebdccd)`(typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & o,const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & s,const Lattice & l)`            | 
`public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::size_type `[`index`](#da/de0/lattice_8h_1a990f37cffb92e0d4bc0b4aa9a31171ef)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor & c,const Lattice & l)`            | 
`public template<>`  <br/>`inline std::pair< typename `[`lattice_traits](#d5/d83/structalps_1_1lattice__traits)< Lattice >::basis_vector_iterator, typename [lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::basis_vector_iterator > `[`basis_vectors`](#da/de0/lattice_8h_1a5c9a15dc59e2f27dbb1d7fd696197696)`(const Lattice & l)`            | 
`public template<>`  <br/>`inline std::pair< typename `[`lattice_traits](#d5/d83/structalps_1_1lattice__traits)< Lattice >::basis_vector_iterator, typename [lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::basis_vector_iterator > `[`reciprocal_basis_vectors`](#da/de0/lattice_8h_1a729e47ed9da1599994529f2f538f0b03)`(const Lattice & l)`            | 
`public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type `[`coordinate`](#da/de0/lattice_8h_1a636c3d3c86a74855b7fbf4a441d32655)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor & c,const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type & p,const Lattice & l)`            | 
`public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type `[`origin`](#da/de0/lattice_8h_1aad5587a5e82181bda2fdde35aa003981)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor & c,const Lattice & l)`            | 
`public void ALPS_DECL `[`prevent_optimization`](#da/de0/lattice_8h_1aa0a157499879aeae7c699ce7b211ae88)`()`            | 
`public template<>`  <br/>`inline std::pair< typename `[`lattice_traits](#d5/d83/structalps_1_1lattice__traits)< Lattice >::momentum_iterator, typename [lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::momentum_iterator > `[`momenta`](#da/de0/lattice_8h_1ae6924ef56f802b3b153bbf943de63f71)`(const Lattice & l)`            | 
`public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type `[`momentum`](#da/de0/lattice_8h_1acb05d9a3517fb5681e2da84f99b0a2a2)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type & m,const Lattice & l)`            | 
`public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::extent_type `[`extent`](#da/de0/lattice_8h_1aa615d01301a3a1c705c42016736317f6)`(const Lattice & l)`            | 
`public template<>`  <br/>`inline element_type< typenamelattice_traits< Lattice >::extent_type >::type `[`extent`](#da/de0/lattice_8h_1a854a50386fc75905bcb91cf842cc54ab)`(const Lattice & l,unsigned int d)`            | 
`public inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor)` >::dimension_type `[`dimension`](#d8/d6e/latticedescriptor_8h_1a1e34dab6980274165747548fc9924400)`(const `[`LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor)` & c)`            | 
`public inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor)` >::dimension_type `[`dimension`](#d8/d6e/latticedescriptor_8h_1a7bb2c767f91edca5dd2aca6d46f089bf)`(const `[`FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor)` & c)`            | 
`public inline alps::oxstream & `[`operator<<`](#d8/d6e/latticedescriptor_8h_1a986449cb94ba33dd818d91858d3f7d27)`(alps::oxstream & out,const `[`alps::LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor)` & l)`            | 
`public inline alps::oxstream & `[`operator<<`](#d8/d6e/latticedescriptor_8h_1a07fbf9cb195843559928ccf815af4fb8)`(alps::oxstream & out,const `[`alps::FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor)` & l)`            | 
`public inline std::ostream & `[`operator<<`](#d8/d6e/latticedescriptor_8h_1ae83275caa0a9a377e5af111aca6d6105)`(std::ostream & out,const `[`alps::LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor)` & l)`            | 
`public inline std::ostream & `[`operator<<`](#d8/d6e/latticedescriptor_8h_1ab2e7c51201c06c854c4316c536aca7c9)`(std::ostream & out,const `[`alps::FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor)` & l)`            | 
`public template<>`  <br/>`inline void `[`make_graph_from_lattice`](#d5/df1/latticegraph_8h_1a0ba59efb53070bffe35244ae3ff047f2)`(GRAPH & g,const LATTICE & l,`[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` depl_desc)`            | 
`public template<>`  <br/>`std::size_t `[`dimension`](#d5/df1/latticegraph_8h_1a848e7d52d9553a35ca29a0c5094b74c5)`(const `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G > & l)`            | 
`public inline alps::oxstream & `[`operator<<`](#d7/d5b/latticegraphdescriptor_8h_1a4719c2c799bfe4f662a284373cf5ba44)`(alps::oxstream & out,const `[`alps::LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor)` & l)`            | 
`public inline std::ostream & `[`operator<<`](#d7/d5b/latticegraphdescriptor_8h_1ad80eed18bbd6f804bf8ffab8cd812832)`(std::ostream & out,const `[`alps::LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor)` & l)`            | 
`public inline alps::oxstream & `[`operator<<`](#d5/d97/latticelibrary_8h_1a895e3bff6cb4ad0ed74766a4cdd3213f)`(alps::oxstream & xml,const `[`alps::LatticeLibrary`](#de/da5/classalps_1_1_lattice_library)` & l)`            | 
`public inline std::ostream & `[`operator<<`](#d5/d97/latticelibrary_8h_1a8279dbfe36ed0e5f303438cfd106f1e0)`(std::ostream & os,const `[`alps::LatticeLibrary`](#de/da5/classalps_1_1_lattice_library)` & l)`            | 
`public inline std::istream & `[`operator>>`](#d5/d97/latticelibrary_8h_1ae1db19b6002837375d6e933b504d2bed)`(std::istream & is,`[`alps::LatticeLibrary`](#de/da5/classalps_1_1_lattice_library)` & l)`            | 
`public template<>`  <br/>`bool `[`set_parity`](#dd/d20/parity_8h_1af128b059aab2bfe838f0bebf1b8c3d74)`(Graph & g,alps::Parameters const & p,Parity)`            | 
`public template<>`  <br/>`bool `[`set_parity`](#dd/d20/parity_8h_1a405af18dd4e282b89b31ece2d55246d7)`(Graph & g,alps::Parameters const & p)`            | 
`public template<>`  <br/>`bool `[`set_parity`](#dd/d20/parity_8h_1a3e27ab03ae71c8264a98f5225a04ae98)`(Graph & g)`            | 
`public template<>`  <br/>`inline `[`property_map`](#da/d52/structalps_1_1property__map)`< P, G, V >::type `[`get_or_default`](#d0/d21/propertymap_8h_1a0eefb2f139280ba5924d4e864143dc6a)`(P p,G & g,const V & v)`            | 
`public template<>`  <br/>`inline `[`simple_cell`](#db/d9c/classalps_1_1simple__cell)`< UnitCell, Offset >::dimension_type `[`dimension`](#d4/d7f/simplecell_8h_1aa0261eaf8fc38b53701919b660242617)`(const `[`simple_cell`](#db/d9c/classalps_1_1simple__cell)`< UnitCell, Offset > & c)`            | 
`public template<>`  <br/>`inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< U, C > >::dimension_type `[`dimension`](#d3/d5e/simplelattice_8h_1a2ab0d4d7c9d05309f51f443732e5e6ce)`(const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< U, C > & l)`            | 
`public template<>`  <br/>[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< UnitCell, Cell >::unit_cell_type & `[`unit_cell`](#d3/d5e/simplelattice_8h_1a331565926faf1f10b881ca27a718e6f6)`(`[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< UnitCell, Cell > & l)`            | 
`public template<>`  <br/>`const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< UnitCell, Cell >::unit_cell_type & `[`unit_cell`](#d3/d5e/simplelattice_8h_1a5a530cd60bfd99ba4fec6359800b4451)`(const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< UnitCell, Cell > & l)`            | 
`public inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell)` >::dimension_type `[`dimension`](#d7/db6/unitcell_8h_1a35dd004a29577eaf147fa844c3c1bfe3)`(const `[`EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell)` & c)`            | 
`public inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` >::dimension_type `[`dimension`](#d7/db6/unitcell_8h_1a61e3ec7d83cfec11ad8b879e812aaa22)`(const `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & c)`            | 
`public inline alps::oxstream & `[`operator<<`](#d7/db6/unitcell_8h_1a0f974fc94f8ca9f7b2c2a6caaf7642bb)`(alps::oxstream & out,const `[`alps::GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & u)`            | 
`public inline std::ostream & `[`operator<<`](#d7/db6/unitcell_8h_1aa6828c80ca080dcd264a078f70195045)`(std::ostream & out,const `[`alps::GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & u)`            | 
`class `[`alps::coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice) | 
`class `[`alps::Depletion`](#d9/da1/classalps_1_1_depletion) | 
`class `[`alps::DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor) | 
`class `[`alps::EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell) | 
`class `[`alps::FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor) | 
`class `[`alps::graph_helper`](#da/d9c/classalps_1_1graph__helper) | 
`class `[`alps::GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell) | 
`class `[`alps::hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice) | 
`class `[`alps::InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor) | 
`class `[`alps::lattice_graph`](#db/dc8/classalps_1_1lattice__graph) | 
`class `[`alps::LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor) | 
`class `[`alps::LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor) | 
`class `[`alps::LatticeLibrary`](#de/da5/classalps_1_1_lattice_library) | 
`class `[`alps::simple_cell`](#db/d9c/classalps_1_1simple__cell) | 
`class `[`alps::simple_lattice`](#d2/d41/classalps_1_1simple__lattice) | 
`class `[`alps::singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map) | 
`struct `[`alps::bond_descriptor_compare`](#d3/dc3/structalps_1_1bond__descriptor__compare) | 
`struct `[`alps::bond_descriptor_compare_undirected`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected) | 
`struct `[`alps::boundary_crossing`](#de/df2/structalps_1_1boundary__crossing) | 
`struct `[`alps::boundary_crossing_t`](#d4/ddb/structalps_1_1boundary__crossing__t) | 
`struct `[`alps::cell_traits`](#dc/deb/structalps_1_1cell__traits) | 
`struct `[`alps::coordinate_t`](#d3/d05/structalps_1_1coordinate__t) | 
`struct `[`alps::coordinate_traits`](#da/d24/structalps_1_1coordinate__traits) | 
`struct `[`alps::coordinate_traits< const C >`](#d0/d1f/structalps_1_1coordinate__traits_3_01const_01_c_01_4) | 
`struct `[`alps::coordinate_traits< std::valarray< T > >`](#d4/dd6/structalps_1_1coordinate__traits_3_01std_1_1valarray_3_01_t_01_4_01_4) | 
`struct `[`alps::coordinate_traits< T[sz]>`](#d9/d2a/structalps_1_1coordinate__traits_3_01_t_0fsz_0e_4) | 
`struct `[`alps::copy_property_helper`](#db/d04/structalps_1_1copy__property__helper) | 
`struct `[`alps::copy_property_helper< SRC, DST, PROPERTY, true >`](#d2/d1b/structalps_1_1copy__property__helper_3_01_s_r_c_00_01_d_s_t_00_01_p_r_o_p_e_r_t_y_00_01true_01_4) | 
`struct `[`alps::dimension_t`](#d1/d9f/structalps_1_1dimension__t) | 
`struct `[`alps::dimensional_traits`](#d8/d28/structalps_1_1dimensional__traits) | 
`struct `[`alps::edge_type_t`](#d6/dda/structalps_1_1edge__type__t) | 
`struct `[`alps::edge_vector_relative_t`](#d4/dff/structalps_1_1edge__vector__relative__t) | 
`struct `[`alps::edge_vector_t`](#de/dd9/structalps_1_1edge__vector__t) | 
`struct `[`alps::graph_name_t`](#d4/d34/structalps_1_1graph__name__t) | 
`struct `[`alps::graph_traits`](#d5/d1a/structalps_1_1graph__traits) | 
`struct `[`alps::graph_traits< lattice_graph< L, G > >`](#de/d51/structalps_1_1graph__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4) | 
`struct `[`alps::has_property`](#d4/dcf/structalps_1_1has__property) | 
`struct `[`alps::has_property< P, boost::adjacency_list< s1, s2, s3, VP, EP, GP, s4 >, D >`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59) | 
`struct `[`alps::has_property< P, const boost::adjacency_list< s1, s2, s3, VP, EP, GP, s4 >, D >`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13) | 
`struct `[`alps::lattice_traits`](#d5/d83/structalps_1_1lattice__traits) | 
`struct `[`alps::lattice_traits< coordinate_lattice< B, V > >`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4) | 
`struct `[`alps::lattice_traits< hypercubic_lattice< BASE, EX > >`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4) | 
`struct `[`alps::lattice_traits< lattice_graph< L, G > >`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4) | 
`struct `[`alps::lattice_traits< LatticeGraphDescriptor >`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4) | 
`struct `[`alps::lattice_traits< simple_lattice< U, C > >`](#dd/d42/structalps_1_1lattice__traits_3_01simple__lattice_3_01_u_00_01_c_01_4_01_4) | 
`struct `[`alps::parity_t`](#d7/d70/structalps_1_1parity__t) | 
`struct `[`alps::parity_traits`](#d5/d74/structalps_1_1parity__traits) | 
`struct `[`alps::parity_traits< parity_t, Graph >`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4) | 
`struct `[`alps::point_traits`](#d7/d29/structalps_1_1point__traits) | 
`struct `[`alps::property_map`](#da/d52/structalps_1_1property__map) | 
`struct `[`alps::property_map< P, const G, Default >`](#d4/d4e/structalps_1_1property__map_3_01_p_00_01const_01_g_00_01_default_01_4) | 
`struct `[`alps::source_offset_t`](#d2/dd2/structalps_1_1source__offset__t) | 
`struct `[`alps::target_offset_t`](#dc/da2/structalps_1_1target__offset__t) | 
`struct `[`alps::vertex_type_t`](#d2/d72/structalps_1_1vertex__type__t) | 

## Members

#### `public template<>`  <br/>`inline std::pair< typename `[`coordinate_traits](#da/d24/structalps_1_1coordinate__traits)< C >::iterator, typename [coordinate_traits`](#da/d24/structalps_1_1coordinate__traits)`< C >::iterator > `[`coordinates`](#dc/da5/coordinate__traits_8h_1adbcf01b7c48c77e6872841c9751990e3)`(C & c)` 

#### `public template<>`  <br/>`inline std::pair< T *, T * > `[`coordinates`](#dc/da5/coordinate__traits_8h_1a1a7a19aef42281dbff6d72f1c7951f26)`(std::valarray< T > & c)` 

#### `public template<>`  <br/>`inline std::pair< const T *, const T * > `[`coordinates`](#dc/da5/coordinate__traits_8h_1a5818aabec6f4516eb30039b9d2a585e1)`(const std::valarray< T > & c)` 

#### `public template<>`  <br/>`std::string `[`coordinate_to_string`](#dc/da5/coordinate__traits_8h_1a3e63a296549d19faf64db8f82ed0cf3f)`(const C & c,int precision)` 

#### `public template<>`  <br/>`inline `[`dimensional_traits`](#d8/d28/structalps_1_1dimensional__traits)`< std::vector< T, A > >::dimension_type `[`dimension`](#d8/d27/dimensional__traits_8h_1a13c85a33649c811496bc74607f4b897c)`(const std::vector< T, A > & d)` 

#### `public template<>`  <br/>`void `[`disorder_vertices`](#d5/d64/disorder_8h_1a81428a7ee114e5e83c29846cb6726ed4)`(G & g,MAP & type)` 

#### `public template<>`  <br/>`void `[`disorder_edges`](#d5/d64/disorder_8h_1a3a87d6893db5ff915b175f744b8d1a50)`(G & g,MAP & type)` 

#### `public template<>`  <br/>`void `[`disorder_bonds`](#d5/d64/disorder_8h_1a9ec663156c456d4c8c2d9031aeacd80d)`(G & g,MAP & type)` 

#### `public template<>`  <br/>`void `[`disorder_sites`](#d5/d64/disorder_8h_1aca19f6e4d6d53a2ba6e2689b91f69aee)`(G & g,MAP & t)` 

#### `public inline alps::oxstream & `[`operator<<`](#d5/d64/disorder_8h_1a1f9e27b0f8c6a5a59c55598b98c4bb2f)`(alps::oxstream & out,const `[`alps::InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor)` & l)` 

#### `public inline std::ostream & `[`operator<<`](#d5/d64/disorder_8h_1a7baa7b9eb21b369a26a64888b7145b23)`(std::ostream & out,const `[`alps::InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor)` & l)` 

#### `public inline alps::oxstream & `[`operator<<`](#d5/d64/disorder_8h_1aea7c25657f64b3524d663b390154f144)`(alps::oxstream & out,const `[`alps::DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` & l)` 

#### `public inline std::ostream & `[`operator<<`](#d5/d64/disorder_8h_1ab35209ef8573439a2f3a8fbba2b1dbf3)`(std::ostream & out,const `[`alps::DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` & l)` 

#### `public template<>`  <br/>`inline void `[`write_graph_xml`](#d6/df3/graph_8h_1adf1a8d09c4fdf8d1d87f616a390c3d60)`(oxstream & out,const GRAPH & g,const std::string & n)` 

#### `public template<>`  <br/>`inline std::string `[`read_graph_xml`](#d6/df3/graph_8h_1a215fabf7d5f320ffc090001ef244aac3)`(std::istream & in,GRAPH & g)` 

#### `public template<>`  <br/>`inline std::string `[`read_graph_xml`](#d6/df3/graph_8h_1a450b14e91a981d283100a259988f29a4)`(const XMLTag & intag,std::istream & p,GRAPH & g)` 

#### `public template<>`  <br/>`inline void `[`copy_property`](#d6/df3/graph_8h_1aac33d03d4f9c69fd17ceb8a20b157423)`(PROPERTY,const SRC & s,const SRCREF & sr,DST & d,DSTREF & dr)` 

#### `public template<>`  <br/>`inline void `[`copy_property`](#d6/df3/graph_8h_1a4fdd97f36ebc3c52b83ba29d6a32fba6)`(PROPERTY,const SRC & s,DST & d)` 

#### `public template<>`  <br/>`inline void `[`copy_graph`](#d6/df3/graph_8h_1a2e912ff9ed6e9735713dc27daf9d9c30)`(const SRC & src,DST & dst)` 

#### `public template<>`  <br/>`inline int `[`constant_degree`](#d6/df3/graph_8h_1a8e9277e23f7ddbdfc2c9b39a386b3899)`(const G & g)` 

#### `public template<>`  <br/>`inline std::size_t `[`maximum_edge_type`](#d6/df3/graph_8h_1a5b7a71d17d09006f7836f3b1046528a0)`(const G & g)` 

#### `public template<>`  <br/>`inline std::size_t `[`maximum_vertex_type`](#d6/df3/graph_8h_1a073e9743cee7f9cfa7de26d0a9519ace)`(const G & g)` 

#### `public template<>`  <br/>`void `[`throw_if_xyz_defined`](#dd/d08/graph__helper_8h_1a1891aecbee7a0d4e26955f7e1cf944d9)`(const Parameters & p,const G & graph)` 

#### `public template<>`  <br/>`Parameters `[`coordinate_as_parameter`](#dd/d08/graph__helper_8h_1a087a82be1dcbffb98e2fdf022e4fe9e0)`(const G & graph,const typename boost::graph_traits< G >::vertex_descriptor & source,const typename boost::graph_traits< G >::vertex_descriptor & target)` 

#### `public template<>`  <br/>`Parameters `[`coordinate_as_parameter`](#dd/d08/graph__helper_8h_1ac1e85c1838edbc5e28679786fd08e7e5)`(const G & graph,const typename boost::graph_traits< G >::edge_descriptor & edge)` 

#### `public template<>`  <br/>`Parameters `[`coordinate_as_parameter`](#dd/d08/graph__helper_8h_1aa036a63c93c3e09cf31e007eda3b0e09)`(const G & graph,const typename boost::graph_traits< G >::vertex_descriptor & vertex)` 

#### `public template<>`  <br/>`std::string `[`site_label`](#dd/d08/graph__helper_8h_1a99137edd7aa5b4c6348ae802fd274f02)`(G const & g,typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor const & v,int precision)` 

#### `public template<>`  <br/>`std::vector< std::string > `[`site_labels`](#dd/d08/graph__helper_8h_1a3a721cfd39c7ccb52554993a8b981923)`(G const & g,int precision)` 

#### `public template<>`  <br/>`std::string `[`bond_label`](#dd/d08/graph__helper_8h_1a88ddd6a9b0b4419de29477a050d430e1)`(G const & g,typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bond_descriptor const & e,int precision)` 

#### `public template<>`  <br/>`std::vector< std::string > `[`bond_labels`](#dd/d08/graph__helper_8h_1a99a46b4c43f43c2cda6dfa5d3163da10)`(G const & g,int precision)` 

#### `public template<>`  <br/>`inline std::size_t `[`dimension`](#da/d35/hypercubic_8h_1a8423205556b64865fd17a64ee8df4e9b)`(const `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice)`< BASE, EX > & l)` 

#### `public template<>`  <br/>`inline const `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::unit_cell_type & `[`unit_cell`](#da/de0/lattice_8h_1ac014201b0d2a647c8b6597721978307e)`(const Lattice & l)` 

#### `public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor `[`cell`](#da/de0/lattice_8h_1ad811e162551ad41ff098bd23896563c2)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & o,const Lattice & l)` 

#### `public template<>`  <br/>`inline const `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & `[`offset`](#da/de0/lattice_8h_1ad289c470135364d8aa130071893e1695)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor & c,const Lattice &)` 

#### `public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::size_type `[`volume`](#da/de0/lattice_8h_1a6166089abc4ec783f8d7a45c7c8c16e5)`(const Lattice & l)` 

#### `public template<>`  <br/>`inline bool `[`on_lattice`](#da/de0/lattice_8h_1aed582d44d388d50983792cd696ffca28)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & o,const Lattice & l)` 

#### `public template<>`  <br/>`inline std::pair< typename `[`lattice_traits](#d5/d83/structalps_1_1lattice__traits)< Lattice >::cell_iterator, typename [lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_iterator > `[`cells`](#da/de0/lattice_8h_1a552cf28f449bd23fd13d21b6b7ca8380)`(const Lattice & l)` 

#### `public template<>`  <br/>`inline std::pair< bool, typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::boundary_crossing_type > `[`shift`](#da/de0/lattice_8h_1afbdf7c84422d52d236ca31ee15ebdccd)`(typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & o,const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::offset_type & s,const Lattice & l)` 

#### `public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::size_type `[`index`](#da/de0/lattice_8h_1a990f37cffb92e0d4bc0b4aa9a31171ef)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor & c,const Lattice & l)` 

#### `public template<>`  <br/>`inline std::pair< typename `[`lattice_traits](#d5/d83/structalps_1_1lattice__traits)< Lattice >::basis_vector_iterator, typename [lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::basis_vector_iterator > `[`basis_vectors`](#da/de0/lattice_8h_1a5c9a15dc59e2f27dbb1d7fd696197696)`(const Lattice & l)` 

#### `public template<>`  <br/>`inline std::pair< typename `[`lattice_traits](#d5/d83/structalps_1_1lattice__traits)< Lattice >::basis_vector_iterator, typename [lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::basis_vector_iterator > `[`reciprocal_basis_vectors`](#da/de0/lattice_8h_1a729e47ed9da1599994529f2f538f0b03)`(const Lattice & l)` 

#### `public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type `[`coordinate`](#da/de0/lattice_8h_1a636c3d3c86a74855b7fbf4a441d32655)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor & c,const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type & p,const Lattice & l)` 

#### `public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type `[`origin`](#da/de0/lattice_8h_1aad5587a5e82181bda2fdde35aa003981)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::cell_descriptor & c,const Lattice & l)` 

#### `public void ALPS_DECL `[`prevent_optimization`](#da/de0/lattice_8h_1aa0a157499879aeae7c699ce7b211ae88)`()` 

#### `public template<>`  <br/>`inline std::pair< typename `[`lattice_traits](#d5/d83/structalps_1_1lattice__traits)< Lattice >::momentum_iterator, typename [lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::momentum_iterator > `[`momenta`](#da/de0/lattice_8h_1ae6924ef56f802b3b153bbf943de63f71)`(const Lattice & l)` 

#### `public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type `[`momentum`](#da/de0/lattice_8h_1acb05d9a3517fb5681e2da84f99b0a2a2)`(const typename `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::vector_type & m,const Lattice & l)` 

#### `public template<>`  <br/>`inline `[`lattice_traits`](#d5/d83/structalps_1_1lattice__traits)`< Lattice >::extent_type `[`extent`](#da/de0/lattice_8h_1aa615d01301a3a1c705c42016736317f6)`(const Lattice & l)` 

#### `public template<>`  <br/>`inline element_type< typenamelattice_traits< Lattice >::extent_type >::type `[`extent`](#da/de0/lattice_8h_1a854a50386fc75905bcb91cf842cc54ab)`(const Lattice & l,unsigned int d)` 

#### `public inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor)` >::dimension_type `[`dimension`](#d8/d6e/latticedescriptor_8h_1a1e34dab6980274165747548fc9924400)`(const `[`LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor)` & c)` 

#### `public inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor)` >::dimension_type `[`dimension`](#d8/d6e/latticedescriptor_8h_1a7bb2c767f91edca5dd2aca6d46f089bf)`(const `[`FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor)` & c)` 

#### `public inline alps::oxstream & `[`operator<<`](#d8/d6e/latticedescriptor_8h_1a986449cb94ba33dd818d91858d3f7d27)`(alps::oxstream & out,const `[`alps::LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor)` & l)` 

#### `public inline alps::oxstream & `[`operator<<`](#d8/d6e/latticedescriptor_8h_1a07fbf9cb195843559928ccf815af4fb8)`(alps::oxstream & out,const `[`alps::FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor)` & l)` 

#### `public inline std::ostream & `[`operator<<`](#d8/d6e/latticedescriptor_8h_1ae83275caa0a9a377e5af111aca6d6105)`(std::ostream & out,const `[`alps::LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor)` & l)` 

#### `public inline std::ostream & `[`operator<<`](#d8/d6e/latticedescriptor_8h_1ab2e7c51201c06c854c4316c536aca7c9)`(std::ostream & out,const `[`alps::FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor)` & l)` 

#### `public template<>`  <br/>`inline void `[`make_graph_from_lattice`](#d5/df1/latticegraph_8h_1a0ba59efb53070bffe35244ae3ff047f2)`(GRAPH & g,const LATTICE & l,`[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` depl_desc)` 

#### `public template<>`  <br/>`std::size_t `[`dimension`](#d5/df1/latticegraph_8h_1a848e7d52d9553a35ca29a0c5094b74c5)`(const `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G > & l)` 

#### `public inline alps::oxstream & `[`operator<<`](#d7/d5b/latticegraphdescriptor_8h_1a4719c2c799bfe4f662a284373cf5ba44)`(alps::oxstream & out,const `[`alps::LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor)` & l)` 

#### `public inline std::ostream & `[`operator<<`](#d7/d5b/latticegraphdescriptor_8h_1ad80eed18bbd6f804bf8ffab8cd812832)`(std::ostream & out,const `[`alps::LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor)` & l)` 

#### `public inline alps::oxstream & `[`operator<<`](#d5/d97/latticelibrary_8h_1a895e3bff6cb4ad0ed74766a4cdd3213f)`(alps::oxstream & xml,const `[`alps::LatticeLibrary`](#de/da5/classalps_1_1_lattice_library)` & l)` 

#### `public inline std::ostream & `[`operator<<`](#d5/d97/latticelibrary_8h_1a8279dbfe36ed0e5f303438cfd106f1e0)`(std::ostream & os,const `[`alps::LatticeLibrary`](#de/da5/classalps_1_1_lattice_library)` & l)` 

#### `public inline std::istream & `[`operator>>`](#d5/d97/latticelibrary_8h_1ae1db19b6002837375d6e933b504d2bed)`(std::istream & is,`[`alps::LatticeLibrary`](#de/da5/classalps_1_1_lattice_library)` & l)` 

#### `public template<>`  <br/>`bool `[`set_parity`](#dd/d20/parity_8h_1af128b059aab2bfe838f0bebf1b8c3d74)`(Graph & g,alps::Parameters const & p,Parity)` 

#### `public template<>`  <br/>`bool `[`set_parity`](#dd/d20/parity_8h_1a405af18dd4e282b89b31ece2d55246d7)`(Graph & g,alps::Parameters const & p)` 

#### `public template<>`  <br/>`bool `[`set_parity`](#dd/d20/parity_8h_1a3e27ab03ae71c8264a98f5225a04ae98)`(Graph & g)` 

#### `public template<>`  <br/>`inline `[`property_map`](#da/d52/structalps_1_1property__map)`< P, G, V >::type `[`get_or_default`](#d0/d21/propertymap_8h_1a0eefb2f139280ba5924d4e864143dc6a)`(P p,G & g,const V & v)` 

#### `public template<>`  <br/>`inline `[`simple_cell`](#db/d9c/classalps_1_1simple__cell)`< UnitCell, Offset >::dimension_type `[`dimension`](#d4/d7f/simplecell_8h_1aa0261eaf8fc38b53701919b660242617)`(const `[`simple_cell`](#db/d9c/classalps_1_1simple__cell)`< UnitCell, Offset > & c)` 

#### `public template<>`  <br/>`inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< U, C > >::dimension_type `[`dimension`](#d3/d5e/simplelattice_8h_1a2ab0d4d7c9d05309f51f443732e5e6ce)`(const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< U, C > & l)` 

#### `public template<>`  <br/>[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< UnitCell, Cell >::unit_cell_type & `[`unit_cell`](#d3/d5e/simplelattice_8h_1a331565926faf1f10b881ca27a718e6f6)`(`[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< UnitCell, Cell > & l)` 

#### `public template<>`  <br/>`const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< UnitCell, Cell >::unit_cell_type & `[`unit_cell`](#d3/d5e/simplelattice_8h_1a5a530cd60bfd99ba4fec6359800b4451)`(const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< UnitCell, Cell > & l)` 

#### `public inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell)` >::dimension_type `[`dimension`](#d7/db6/unitcell_8h_1a35dd004a29577eaf147fa844c3c1bfe3)`(const `[`EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell)` & c)` 

#### `public inline `[`dimensional_traits](#d8/d28/structalps_1_1dimensional__traits)< [GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` >::dimension_type `[`dimension`](#d7/db6/unitcell_8h_1a61e3ec7d83cfec11ad8b879e812aaa22)`(const `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & c)` 

#### `public inline alps::oxstream & `[`operator<<`](#d7/db6/unitcell_8h_1a0f974fc94f8ca9f7b2c2a6caaf7642bb)`(alps::oxstream & out,const `[`alps::GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & u)` 

#### `public inline std::ostream & `[`operator<<`](#d7/db6/unitcell_8h_1aa6828c80ca080dcd264a078f70195045)`(std::ostream & out,const `[`alps::GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & u)` 

# class `alps::coordinate_lattice` 

```
class alps::coordinate_lattice
  : public alps::simple_lattice<>
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1ae7e453a8fcdf7630230fc33825b84a8d)`()` | 
`public template<>`  <br/>`inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1a6f0d2f84086babd30b0a4eab29bdbf07)`(const `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice)`< B2, V2 > & l)` | 
`public template<>`  <br/>`inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1acfd953ba9e60e7c5d19d1e83432f7f7a)`(const unit_cell_type & u,InputIterator first,InputIterator last)` | 
`public template<>`  <br/>`inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1a5890fd813b288e804be722301731c2f6)`(const unit_cell_type & u,InputIterator1 first1,InputIterator1 last1,InputIterator2 first2,InputIterator2 last2)` | 
`public inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1ac00d5d5752fc8c4f25492c59689ddd83)`(const unit_cell_type & u)` | 
`public template<>`  <br/>`inline const `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice)` & `[`operator=`](#d6/d8d/classalps_1_1coordinate__lattice_1ac7880d0605e6aaa958e01848043dc566)`(const `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice)`< B2, V2 > & l)` | 
`public inline void `[`set_parameters`](#d6/d8d/classalps_1_1coordinate__lattice_1a6e390dd4efa73fe320c3335272864161)`(const Parameters & p)` | 
`public inline void `[`add_basis_vector`](#d6/d8d/classalps_1_1coordinate__lattice_1a7ea95276957883e64fd688f97459b6fa)`(const vector_type & v)` | 
`public inline std::size_t `[`num_basis_vectors`](#d6/d8d/classalps_1_1coordinate__lattice_1a3db5fddddda65bebcdee7f373b5e5a81)`() const` | 
`public inline std::pair< basis_vector_iterator, basis_vector_iterator > `[`basis_vectors`](#d6/d8d/classalps_1_1coordinate__lattice_1aae2d8c2a4f60c389e26d136db64435ff)`() const` | 
`public inline void `[`add_reciprocal_basis_vector`](#d6/d8d/classalps_1_1coordinate__lattice_1a2217593b81579693c33d9a37c1d6b11a)`(const vector_type & v)` | 
`public inline std::size_t `[`num_reciprocal_basis_vectors`](#d6/d8d/classalps_1_1coordinate__lattice_1ad390c50a8d0c78718be905ff477ef98a)`() const` | 
`public inline std::pair< basis_vector_iterator, basis_vector_iterator > `[`reciprocal_basis_vectors`](#d6/d8d/classalps_1_1coordinate__lattice_1a802d534eec3ec0855ec639d2aca15e49)`() const` | 
`typedef `[`parent_lattice_type`](#d6/d8d/classalps_1_1coordinate__lattice_1ae9cc379bfbf86adba166a35b9b519917) | 
`typedef `[`unit_cell_type`](#d6/d8d/classalps_1_1coordinate__lattice_1aeae1a522845478186169192084d51a04) | 
`typedef `[`offset_type`](#d6/d8d/classalps_1_1coordinate__lattice_1a8f2839e81c5b5424ba87f3677fb74314) | 
`typedef `[`cell_descriptor`](#d6/d8d/classalps_1_1coordinate__lattice_1a3808f9248a102c58a88005efd0a529ff) | 
`typedef `[`vector_type`](#d6/d8d/classalps_1_1coordinate__lattice_1ab6b405e530cfa2a2cd261847469e63bc) | 
`typedef `[`basis_vector_iterator`](#d6/d8d/classalps_1_1coordinate__lattice_1afef5ba53f02cfcd2e04c6d86c610cbea) | 

## Members

#### `public inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1ae7e453a8fcdf7630230fc33825b84a8d)`()` 

#### `public template<>`  <br/>`inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1a6f0d2f84086babd30b0a4eab29bdbf07)`(const `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice)`< B2, V2 > & l)` 

#### `public template<>`  <br/>`inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1acfd953ba9e60e7c5d19d1e83432f7f7a)`(const unit_cell_type & u,InputIterator first,InputIterator last)` 

#### `public template<>`  <br/>`inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1a5890fd813b288e804be722301731c2f6)`(const unit_cell_type & u,InputIterator1 first1,InputIterator1 last1,InputIterator2 first2,InputIterator2 last2)` 

#### `public inline  `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice_1ac00d5d5752fc8c4f25492c59689ddd83)`(const unit_cell_type & u)` 

#### `public template<>`  <br/>`inline const `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice)` & `[`operator=`](#d6/d8d/classalps_1_1coordinate__lattice_1ac7880d0605e6aaa958e01848043dc566)`(const `[`coordinate_lattice`](#d6/d8d/classalps_1_1coordinate__lattice)`< B2, V2 > & l)` 

#### `public inline void `[`set_parameters`](#d6/d8d/classalps_1_1coordinate__lattice_1a6e390dd4efa73fe320c3335272864161)`(const Parameters & p)` 

#### `public inline void `[`add_basis_vector`](#d6/d8d/classalps_1_1coordinate__lattice_1a7ea95276957883e64fd688f97459b6fa)`(const vector_type & v)` 

#### `public inline std::size_t `[`num_basis_vectors`](#d6/d8d/classalps_1_1coordinate__lattice_1a3db5fddddda65bebcdee7f373b5e5a81)`() const` 

#### `public inline std::pair< basis_vector_iterator, basis_vector_iterator > `[`basis_vectors`](#d6/d8d/classalps_1_1coordinate__lattice_1aae2d8c2a4f60c389e26d136db64435ff)`() const` 

#### `public inline void `[`add_reciprocal_basis_vector`](#d6/d8d/classalps_1_1coordinate__lattice_1a2217593b81579693c33d9a37c1d6b11a)`(const vector_type & v)` 

#### `public inline std::size_t `[`num_reciprocal_basis_vectors`](#d6/d8d/classalps_1_1coordinate__lattice_1ad390c50a8d0c78718be905ff477ef98a)`() const` 

#### `public inline std::pair< basis_vector_iterator, basis_vector_iterator > `[`reciprocal_basis_vectors`](#d6/d8d/classalps_1_1coordinate__lattice_1a802d534eec3ec0855ec639d2aca15e49)`() const` 

#### `typedef `[`parent_lattice_type`](#d6/d8d/classalps_1_1coordinate__lattice_1ae9cc379bfbf86adba166a35b9b519917) 

#### `typedef `[`unit_cell_type`](#d6/d8d/classalps_1_1coordinate__lattice_1aeae1a522845478186169192084d51a04) 

#### `typedef `[`offset_type`](#d6/d8d/classalps_1_1coordinate__lattice_1a8f2839e81c5b5424ba87f3677fb74314) 

#### `typedef `[`cell_descriptor`](#d6/d8d/classalps_1_1coordinate__lattice_1a3808f9248a102c58a88005efd0a529ff) 

#### `typedef `[`vector_type`](#d6/d8d/classalps_1_1coordinate__lattice_1ab6b405e530cfa2a2cd261847469e63bc) 

#### `typedef `[`basis_vector_iterator`](#d6/d8d/classalps_1_1coordinate__lattice_1afef5ba53f02cfcd2e04c6d86c610cbea) 

# class `alps::Depletion` 

```
class alps::Depletion
  : public alps::DepletionDescriptor
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`Depletion`](#d9/da1/classalps_1_1_depletion_1aab9598272de3d9c08dc3144fdbda551a)`(`[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` const & depl,std::size_t num_sites)` | 
`public inline bool `[`exists`](#d9/da1/classalps_1_1_depletion_1a39dc4937075ddb2de31a2b748c496085)`(std::size_t site) const` | 
`public inline std::size_t `[`mapped_site`](#d9/da1/classalps_1_1_depletion_1a4731f27c75bf12f641be12992ef85763)`(std::size_t site) const` | 
`public inline std::size_t `[`num_sites`](#d9/da1/classalps_1_1_depletion_1af1c99d64cb7f8b5d261cd686f20eabb4)`()` | 

## Members

#### `public  `[`Depletion`](#d9/da1/classalps_1_1_depletion_1aab9598272de3d9c08dc3144fdbda551a)`(`[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` const & depl,std::size_t num_sites)` 

#### `public inline bool `[`exists`](#d9/da1/classalps_1_1_depletion_1a39dc4937075ddb2de31a2b748c496085)`(std::size_t site) const` 

#### `public inline std::size_t `[`mapped_site`](#d9/da1/classalps_1_1_depletion_1a4731f27c75bf12f641be12992ef85763)`(std::size_t site) const` 

#### `public inline std::size_t `[`num_sites`](#d9/da1/classalps_1_1_depletion_1af1c99d64cb7f8b5d261cd686f20eabb4)`()` 

# class `alps::DepletionDescriptor` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public boost::optional< Expression > `[`prob`](#d9/dd8/classalps_1_1_depletion_descriptor_1ae5b30b444c6ce290525f4f25d3414316) | 
`public std::string `[`seed_name`](#d9/dd8/classalps_1_1_depletion_descriptor_1af9c902ffe2ff6ebf1a3c0a69c3b44bdd) | 
`public int `[`seed_`](#d9/dd8/classalps_1_1_depletion_descriptor_1ad18ba75b4cbb2babcfdd5a84f04d610d) | 
`public inline  `[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor_1a2ddfa5d6179b1441ce074e44773d7052)`()` | 
`public  `[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor_1af36f04352dfbbcf423fed50ea6c6de79)`(XMLTag &,std::istream &)` | 
`public void `[`write_xml`](#d9/dd8/classalps_1_1_depletion_descriptor_1a3bbbfb5f18fabdce9be4820fb5bfe8fb)`(oxstream &) const` | 
`public inline double `[`probability`](#d9/dd8/classalps_1_1_depletion_descriptor_1a65da8c8bce782f50642a439608403798)`() const` | 
`public void `[`set_parameters`](#d9/dd8/classalps_1_1_depletion_descriptor_1ac994321232f11662cfba5ee8a8da914e)`(const Parameters & p)` | 
`public inline int `[`seed`](#d9/dd8/classalps_1_1_depletion_descriptor_1a98411e5fdcc0a06b5419cf4ae40fa0c2)`() const` | 

## Members

#### `public boost::optional< Expression > `[`prob`](#d9/dd8/classalps_1_1_depletion_descriptor_1ae5b30b444c6ce290525f4f25d3414316) 

#### `public std::string `[`seed_name`](#d9/dd8/classalps_1_1_depletion_descriptor_1af9c902ffe2ff6ebf1a3c0a69c3b44bdd) 

#### `public int `[`seed_`](#d9/dd8/classalps_1_1_depletion_descriptor_1ad18ba75b4cbb2babcfdd5a84f04d610d) 

#### `public inline  `[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor_1a2ddfa5d6179b1441ce074e44773d7052)`()` 

#### `public  `[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor_1af36f04352dfbbcf423fed50ea6c6de79)`(XMLTag &,std::istream &)` 

#### `public void `[`write_xml`](#d9/dd8/classalps_1_1_depletion_descriptor_1a3bbbfb5f18fabdce9be4820fb5bfe8fb)`(oxstream &) const` 

#### `public inline double `[`probability`](#d9/dd8/classalps_1_1_depletion_descriptor_1a65da8c8bce782f50642a439608403798)`() const` 

#### `public void `[`set_parameters`](#d9/dd8/classalps_1_1_depletion_descriptor_1ac994321232f11662cfba5ee8a8da914e)`(const Parameters & p)` 

#### `public inline int `[`seed`](#d9/dd8/classalps_1_1_depletion_descriptor_1a98411e5fdcc0a06b5419cf4ae40fa0c2)`() const` 

# class `alps::EmptyUnitCell` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell_1a79527b5432e02212c369040ea9a6b7cf)`(std::size_t d)` | 
`public inline std::size_t `[`dimension`](#de/dd5/classalps_1_1_empty_unit_cell_1a65fa50f11ccdc45fd93575a2cdd82f88)`() const` | 

## Members

#### `public inline  `[`EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell_1a79527b5432e02212c369040ea9a6b7cf)`(std::size_t d)` 

#### `public inline std::size_t `[`dimension`](#de/dd5/classalps_1_1_empty_unit_cell_1a65fa50f11ccdc45fd93575a2cdd82f88)`() const` 

# class `alps::FiniteLatticeDescriptor` 

```
class alps::FiniteLatticeDescriptor
  : public alps::hypercubic_lattice< coordinate_lattice< simple_lattice<>, std::vector< alps::StringValue > >, std::vector< alps::StringValue > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a4ef5ce0f761cd4ec6513437935e97cbe)`()` | 
`public  `[`FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor_1aff86db9f7b499250cb9cd336c848bff4)`(const alps::XMLTag &,std::istream &,const LatticeMap &)` | 
`public void `[`write_xml`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a760e058312a6dcea391c178542cd41ba)`(oxstream &) const` | 
`public inline const std::string & `[`name`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a69e6a2dcb9eca1073b6c7551ae7e926f)`() const` | 
`public void `[`set_parameters`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a47ae961a3ba51b947c481322a0f01159)`(const alps::Parameters &)` | 
`public inline std::size_t `[`dimension`](#da/d60/classalps_1_1_finite_lattice_descriptor_1aa62ad873a052e83f4196416b8d437ebb)`() const` | 
`typedef `[`base_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1ad39788f141229afa6d9cb3be6c0b1ff2) | 
`typedef `[`base_base_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1ac8abae8daa79e9542e5c21471960a1fc) | 
`typedef `[`unit_cell_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a03aab3d0d9b5936375ec0439b31ba49b) | 
`typedef `[`offset_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a51bb926b749c40c2998e44b06181dc24) | 
`typedef `[`cell_descriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a009f4f5db6686644d776610126b1f3cb) | 
`typedef `[`vector_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1ab266ad717440f2fc52eb8d5df58aa42a) | 
`typedef `[`basis_vector_iterator`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a75d312c5ba9c553db360c6c3d4740464) | 
`typedef `[`cell_iterator`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a21abd6de8f1d46bc5fe43b9b3417f252) | 
`typedef `[`size_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1acc57f4800e4cf275e47b04acde5c9b39) | 

## Members

#### `public  `[`FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a4ef5ce0f761cd4ec6513437935e97cbe)`()` 

#### `public  `[`FiniteLatticeDescriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor_1aff86db9f7b499250cb9cd336c848bff4)`(const alps::XMLTag &,std::istream &,const LatticeMap &)` 

#### `public void `[`write_xml`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a760e058312a6dcea391c178542cd41ba)`(oxstream &) const` 

#### `public inline const std::string & `[`name`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a69e6a2dcb9eca1073b6c7551ae7e926f)`() const` 

#### `public void `[`set_parameters`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a47ae961a3ba51b947c481322a0f01159)`(const alps::Parameters &)` 

#### `public inline std::size_t `[`dimension`](#da/d60/classalps_1_1_finite_lattice_descriptor_1aa62ad873a052e83f4196416b8d437ebb)`() const` 

#### `typedef `[`base_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1ad39788f141229afa6d9cb3be6c0b1ff2) 

#### `typedef `[`base_base_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1ac8abae8daa79e9542e5c21471960a1fc) 

#### `typedef `[`unit_cell_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a03aab3d0d9b5936375ec0439b31ba49b) 

#### `typedef `[`offset_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a51bb926b749c40c2998e44b06181dc24) 

#### `typedef `[`cell_descriptor`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a009f4f5db6686644d776610126b1f3cb) 

#### `typedef `[`vector_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1ab266ad717440f2fc52eb8d5df58aa42a) 

#### `typedef `[`basis_vector_iterator`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a75d312c5ba9c553db360c6c3d4740464) 

#### `typedef `[`cell_iterator`](#da/d60/classalps_1_1_finite_lattice_descriptor_1a21abd6de8f1d46bc5fe43b9b3417f252) 

#### `typedef `[`size_type`](#da/d60/classalps_1_1_finite_lattice_descriptor_1acc57f4800e4cf275e47b04acde5c9b39) 

# class `alps::graph_helper` 

```
class alps::graph_helper
  : public alps::LatticeLibrary
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`graph_helper`](#da/d9c/classalps_1_1graph__helper_1adde0193e9b7346ce5aad1a67865ac230)`(std::istream & in,const Parameters & p)` | 
`public inline  `[`graph_helper`](#da/d9c/classalps_1_1graph__helper_1aa1684797abdf9837f9dda8d24d42c4c9)`(const alps::Parameters & p)` | 
`public inline  `[`~graph_helper`](#da/d9c/classalps_1_1graph__helper_1a8b2dc8918994a6da29dc1662460c9e20)`()` | 
`public inline graph_type & `[`graph`](#da/d9c/classalps_1_1graph__helper_1a48bec30b47cbf0ec6eefb8eccea572f7)`()` | 
`public inline const graph_type & `[`graph`](#da/d9c/classalps_1_1graph__helper_1ab4bc73f875a4be9624a649fb33448924)`() const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::graph_type & `[`graph`](#da/d9c/classalps_1_1graph__helper_1a33337b909626756b5e4e882fbe9e30e3)`(H & g) const` | 
`public template<>`  <br/>`inline const `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::graph_type & `[`graph`](#da/d9c/classalps_1_1graph__helper_1aa70d0c41f32af6b69f67cd701452aaaa)`(const H & g) const` | 
`public inline `[`lattice_type`](#db/dc8/classalps_1_1lattice__graph)` & `[`lattice`](#da/d9c/classalps_1_1graph__helper_1a7166c07d787202a823548b15a9711458)`()` | 
`public inline const `[`lattice_type`](#db/dc8/classalps_1_1lattice__graph)` & `[`lattice`](#da/d9c/classalps_1_1graph__helper_1a4ed48ae61643493e36024815161044bf)`() const` | 
`public inline vertices_size_type `[`num_vertices`](#da/d9c/classalps_1_1graph__helper_1a3ab0aa6949be3b8ca87fecb926fd6b61)`() const` | 
`public inline edges_size_type `[`num_edges`](#da/d9c/classalps_1_1graph__helper_1abede5f0a00e7ede0bd9056cb3b99e154)`() const` | 
`public inline std::pair< vertex_iterator, vertex_iterator > `[`vertices`](#da/d9c/classalps_1_1graph__helper_1a26f9658eb64bd38efbbf5204edde4a81)`() const` | 
`public inline std::pair< edge_iterator, edge_iterator > `[`edges`](#da/d9c/classalps_1_1graph__helper_1ae3438cb5ef3cc98af7f2e81f7ac88d74)`() const` | 
`public inline degree_size_type `[`out_degree`](#da/d9c/classalps_1_1graph__helper_1ac8e323b16b0e7ee9555079c735371738)`(const vertex_descriptor & v) const` | 
`public inline degree_size_type `[`in_degree`](#da/d9c/classalps_1_1graph__helper_1a7bbd494c52fa3b2f77fc6755751fa7ee)`(const vertex_descriptor & v) const` | 
`public inline degree_size_type `[`degree`](#da/d9c/classalps_1_1graph__helper_1a222c4d0449b92a9512f574dbc7b999fd)`(const vertex_descriptor & v) const` | 
`public inline std::pair< out_edge_iterator, out_edge_iterator > `[`out_edges`](#da/d9c/classalps_1_1graph__helper_1aab84adbfb1de97669d6846cdb2d30f10)`(const vertex_descriptor & v) const` | 
`public inline std::pair< in_edge_iterator, in_edge_iterator > `[`in_edges`](#da/d9c/classalps_1_1graph__helper_1a5097cca53866b269b00bd975a849fa3d)`(const vertex_descriptor & v) const` | 
`public inline std::pair< adjacency_iterator, adjacency_iterator > `[`adjacent_vertices`](#da/d9c/classalps_1_1graph__helper_1a422f7f3b44d1bd1b17b7e7843b5bff8e)`(const vertex_descriptor & v) const` | 
`public inline vertex_descriptor `[`vertex`](#da/d9c/classalps_1_1graph__helper_1a3a674d6f4523e5077e50f1b6c6cd7e70)`(vertices_size_type i) const` | 
`public inline site_descriptor `[`source`](#da/d9c/classalps_1_1graph__helper_1ade814b397ffece286639f4fb6ee79237)`(const bond_descriptor & b) const` | 
`public inline site_descriptor `[`target`](#da/d9c/classalps_1_1graph__helper_1a0dee76813e338837997391e92e8ff304)`(const bond_descriptor & b) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertices_size_type `[`num_vertices`](#da/d9c/classalps_1_1graph__helper_1a9dddd766f3daf00a7ef1101448859413)`(const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::edges_size_type `[`num_edges`](#da/d9c/classalps_1_1graph__helper_1aee2691f36caa48fe1ba146ee2fee5877)`(const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::vertex_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_iterator > `[`vertices`](#da/d9c/classalps_1_1graph__helper_1a1a72347630b0795c41963786512bd8bd)`(const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::edge_iterator > `[`edges`](#da/d9c/classalps_1_1graph__helper_1a7660e2eafd6c326a2c0379260e5d6690)`(const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::degree_size_type `[`out_degree`](#da/d9c/classalps_1_1graph__helper_1a4e68d505ee0880dabd829a18bff0090f)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::degree_size_type `[`in_degree`](#da/d9c/classalps_1_1graph__helper_1a421b255086354975e4f88c7752ac43a2)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::degree_size_type `[`degree`](#da/d9c/classalps_1_1graph__helper_1ae536cd319060c0cc415a1741571e6417)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::out_edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::out_edge_iterator > `[`out_edges`](#da/d9c/classalps_1_1graph__helper_1a3a04d2ab1ff06353f74aab4524653be3)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::in_edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::in_edge_iterator > `[`in_edges`](#da/d9c/classalps_1_1graph__helper_1a85aa0301888187ab547359005d8b756f)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::adjacency_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::adjacency_iterator > `[`adjacent_vertices`](#da/d9c/classalps_1_1graph__helper_1ac242a3b460da42a12f23def4d09f1961)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor `[`vertex`](#da/d9c/classalps_1_1graph__helper_1a7b496fbf97766d061a5ab12b5412d3bf)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertices_size_type i,const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor `[`source`](#da/d9c/classalps_1_1graph__helper_1a047c30f044757241ccd1a250a5bccbb7)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bond_descriptor & b,const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor `[`target`](#da/d9c/classalps_1_1graph__helper_1aec37d31942a95373ae210e764b3d731d)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bond_descriptor & b,const H & g) const` | 
`public inline sites_size_type `[`num_sites`](#da/d9c/classalps_1_1graph__helper_1aff7313ebbd1820a97b46d694dbbb787d)`() const` | 
`public inline bonds_size_type `[`num_bonds`](#da/d9c/classalps_1_1graph__helper_1a32a85f1c3eeae18c70f120d4fd827232)`() const` | 
`public inline std::pair< site_iterator, site_iterator > `[`sites`](#da/d9c/classalps_1_1graph__helper_1a690a8d6256396acae3bd659a4f95d580)`() const` | 
`public inline site_descriptor `[`site`](#da/d9c/classalps_1_1graph__helper_1ac4c79b2c8eae8d8ef9108458be696d23)`(sites_size_type i) const` | 
`public inline std::pair< bond_iterator, bond_iterator > `[`bonds`](#da/d9c/classalps_1_1graph__helper_1a04c4d663831eb0c4d390b1202ff8016c)`() const` | 
`public inline bond_descriptor `[`bond`](#da/d9c/classalps_1_1graph__helper_1a3856964bd2e23f95ba89a1c14022a037)`(bonds_size_type i) const` | 
`public inline neighbors_size_type `[`num_neighbors`](#da/d9c/classalps_1_1graph__helper_1a9fbb248be2daa346ec120abe7c22ec16)`(const site_descriptor & v) const` | 
`public inline std::pair< neighbor_bond_iterator, neighbor_bond_iterator > `[`neighbor_bonds`](#da/d9c/classalps_1_1graph__helper_1acd95623364649f0bf6e10903c5321040)`(const site_descriptor & v) const` | 
`public inline std::pair< neighbor_iterator, neighbor_iterator > `[`neighbors`](#da/d9c/classalps_1_1graph__helper_1a38e808cd387500955b48d10c00439212)`(const site_descriptor & v) const` | 
`public inline site_descriptor `[`neighbor`](#da/d9c/classalps_1_1graph__helper_1a5998530e42e5a1b888dbe74fcd90a3b8)`(const site_descriptor & v,neighbors_size_type i) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::sites_size_type `[`num_sites`](#da/d9c/classalps_1_1graph__helper_1aa40acd68050e717e992a7c59d8e23337)`(const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bonds_size_type `[`num_bonds`](#da/d9c/classalps_1_1graph__helper_1a63fb1ba1f663d926052c6824edfbd703)`(const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::site_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_iterator > `[`sites`](#da/d9c/classalps_1_1graph__helper_1acaeb570aa88734f9e897ae3c931819ac)`(const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor `[`site`](#da/d9c/classalps_1_1graph__helper_1a99c3df1db758368023cf4c20c5f7c19e)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::sites_size_type i,const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::bond_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bond_iterator > `[`bonds`](#da/d9c/classalps_1_1graph__helper_1a9cbc6b809d57c2a6e2228a31143a0b7e)`(const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bond_descriptor `[`bond`](#da/d9c/classalps_1_1graph__helper_1a79b3ede8f8b3479cacf0b75e0905081a)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bonds_size_type i,const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::neighbors_size_type `[`num_neighbors`](#da/d9c/classalps_1_1graph__helper_1abc5d669034bdae7d0cd4365d3a330cca)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::neighbor_bond_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::neighbor_bond_iterator > `[`neighbor_bonds`](#da/d9c/classalps_1_1graph__helper_1a070bc75e6a0232ba60b83626b34f84f4)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::neighbor_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::neighbor_iterator > `[`neighbors`](#da/d9c/classalps_1_1graph__helper_1abb141953ed2507629bbcd5b3521dfc26)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor & v,const H & g) const` | 
`public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor `[`neighbor`](#da/d9c/classalps_1_1graph__helper_1a62bd08856b20115985f23cd70830aa77)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor & v,typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::neighbors_size_type i,const H & g) const` | 
`public inline double `[`parity`](#da/d9c/classalps_1_1graph__helper_1a9b50cacc36f36ed0da7f08c844bafb5a)`(const site_descriptor & v) const` | 
`public inline bool `[`is_bipartite`](#da/d9c/classalps_1_1graph__helper_1ad7e3180360c5ad741cce68d588241ae7)`() const` | 
`public inline vertex_type_map_type `[`vertex_type_map`](#da/d9c/classalps_1_1graph__helper_1ae911b1dd0edba7c0a5adbb986ef35efa)`() const` | 
`public inline site_type_map_type `[`site_type_map`](#da/d9c/classalps_1_1graph__helper_1adf689be4bbb84b41b205ee94bb355f83)`() const` | 
`public inline edge_type_map_type `[`edge_type_map`](#da/d9c/classalps_1_1graph__helper_1a01b165883a4ec8297560d3a38ad729db)`() const` | 
`public inline bond_type_map_type `[`bond_type_map`](#da/d9c/classalps_1_1graph__helper_1a8601a717dce5236f6d0ce974a44caaf6)`() const` | 
`public inline type_type `[`vertex_type`](#da/d9c/classalps_1_1graph__helper_1a9da3cc1017f93bc27911156cb72d9946)`(const vertex_descriptor & v) const` | 
`public inline type_type `[`site_type`](#da/d9c/classalps_1_1graph__helper_1aacf8df2569142e25a9d130a935f95386)`(const site_descriptor & s) const` | 
`public inline type_type `[`edge_type`](#da/d9c/classalps_1_1graph__helper_1a8a9847a7bf5f2358a42b886a28a01746)`(const edge_descriptor & e) const` | 
`public inline type_type `[`bond_type`](#da/d9c/classalps_1_1graph__helper_1a3e12d6f34f7402f3576d1b9b1cb70414)`(const bond_descriptor & b) const` | 
`public inline bool `[`inhomogeneous`](#da/d9c/classalps_1_1graph__helper_1ae680acd786b7f0ffbdd94d9ec346ea43)`() const` | 
`public inline bool `[`inhomogeneous_vertices`](#da/d9c/classalps_1_1graph__helper_1af1754fa3f5638e83de7c2b1b87ddb6e2)`() const` | 
`public inline bool `[`inhomogeneous_sites`](#da/d9c/classalps_1_1graph__helper_1aa254b754bcad07974fabb83f85e03306)`() const` | 
`public inline bool `[`inhomogeneous_edges`](#da/d9c/classalps_1_1graph__helper_1a45b0971d3122cef662a6fd61f119b591)`() const` | 
`public inline bool `[`inhomogeneous_bonds`](#da/d9c/classalps_1_1graph__helper_1a4224c791e0dc2bbc6148a5085c350a1f)`() const` | 
`public inline inhomogeneous_vertex_type_map_type `[`inhomogeneous_vertex_type_map`](#da/d9c/classalps_1_1graph__helper_1a7509e0501a58ae38aa6809903869f358)`() const` | 
`public inline inhomogeneous_site_type_map_type `[`inhomogeneous_site_type_map`](#da/d9c/classalps_1_1graph__helper_1a0fcb72b4acfe9f4509e52830b1797217)`() const` | 
`public inline inhomogeneous_edge_type_map_type `[`inhomogeneous_edge_type_map`](#da/d9c/classalps_1_1graph__helper_1a801efb9fe2f66e671c328d271d593284)`() const` | 
`public inline inhomogeneous_bond_type_map_type `[`inhomogeneous_bond_type_map`](#da/d9c/classalps_1_1graph__helper_1adebb95bbc578e36c55b2f7243b6e3015)`() const` | 
`public inline type_type `[`inhomogeneous_vertex_type`](#da/d9c/classalps_1_1graph__helper_1a7a4a9497891b40d405c82c98fa1a862a)`(const vertex_descriptor & v) const` | 
`public inline type_type `[`inhomogeneous_site_type`](#da/d9c/classalps_1_1graph__helper_1a853b8463d1250db1a5c8a09d40462ddd)`(const site_descriptor & s) const` | 
`public inline type_type `[`inhomogeneous_edge_type`](#da/d9c/classalps_1_1graph__helper_1a0aa70045c07d6c94dfb503d7da09f2cf)`(const edge_descriptor & e) const` | 
`public inline type_type `[`inhomogeneous_bond_type`](#da/d9c/classalps_1_1graph__helper_1a4226fc1a552ecdf84e854637a924a2e5)`(const bond_descriptor & b) const` | 
`public inline const vector_type & `[`coordinate`](#da/d9c/classalps_1_1graph__helper_1ae414c95e65025212a27e0831764d2669)`(const site_descriptor & s) const` | 
`public inline std::string `[`coordinate_string`](#da/d9c/classalps_1_1graph__helper_1abac50a96e10d34182651a3869c2328e2)`(const site_descriptor & s,int precision) const` | 
`public inline const vector_type & `[`bond_vector`](#da/d9c/classalps_1_1graph__helper_1a23e18357d40568e5f61deb04d877f96c)`(const bond_descriptor & b) const` | 
`public inline const vector_type & `[`bond_vector_relative`](#da/d9c/classalps_1_1graph__helper_1a4f388e74395b42943ce54cf9065c00fa)`(const bond_descriptor & b) const` | 
`public inline std::size_t `[`dimension`](#da/d9c/classalps_1_1graph__helper_1a79e3181ee882eb2236455c4213af1421)`() const` | 
`public inline std::pair< momentum_iterator, momentum_iterator > `[`momenta`](#da/d9c/classalps_1_1graph__helper_1a1d95a3316034859cab4ef760ad203f53)`() const` | 
`public inline void `[`throw_if_xyz_defined`](#da/d9c/classalps_1_1graph__helper_1a4661bb1bcbee258a8f6e720d4f31f3ae)`(const Parameters & p,const vertex_descriptor &) const` | 
`public inline void `[`throw_if_xyz_defined`](#da/d9c/classalps_1_1graph__helper_1a23bb6cd9e9347d1fbd096d2b84379a56)`(const Parameters & p,const edge_descriptor &) const` | 
`public inline Parameters `[`coordinate_as_parameter`](#da/d9c/classalps_1_1graph__helper_1a4e30bb849bb111e607be6d78f2863c71)`(const edge_descriptor & e) const` | 
`public inline Parameters `[`coordinate_as_parameter`](#da/d9c/classalps_1_1graph__helper_1a74ee8246db3a10f0a9b69ddba5572e56)`(const vertex_descriptor & v) const` | 
`public inline size_type `[`volume`](#da/d9c/classalps_1_1graph__helper_1ac7de6175442489278535c9882cdd933a)`() const` | 
`public inline const unit_cell_type & `[`unit_cell`](#da/d9c/classalps_1_1graph__helper_1adc5b55bbd2791484ab952a864851167b)`() const` | 
`public inline cell_descriptor `[`cell`](#da/d9c/classalps_1_1graph__helper_1afd59185485b351736ac1ac89cf744278)`(const offset_type & o) const` | 
`public inline std::pair< cell_iterator, cell_iterator > `[`cells`](#da/d9c/classalps_1_1graph__helper_1af1d01731515a2c7570269359c06f01fe)`() const` | 
`public inline const offset_type & `[`offset`](#da/d9c/classalps_1_1graph__helper_1a40eeb11ed8e26f900f1d854c7402b63e)`(const cell_descriptor & c) const` | 
`public inline bool `[`on_lattice`](#da/d9c/classalps_1_1graph__helper_1ab323cc5ebff9e1b0675c1fe4fefe8ed5)`(const offset_type & o) const` | 
`public inline std::pair< bool, boundary_crossing_type > `[`shift`](#da/d9c/classalps_1_1graph__helper_1a4a778b0f2a874047c3425d17cfeca5fd)`(offset_type & o,const offset_type & s) const` | 
`public inline size_type `[`cell_index`](#da/d9c/classalps_1_1graph__helper_1a7e342aab38e0339ad204f629a96f01f3)`(const cell_descriptor & c) const` | 
`public inline size_type `[`vertex_index`](#da/d9c/classalps_1_1graph__helper_1a5e37f20e5b3614337c57e9e4606ee38d)`(const vertex_descriptor & v) const` | 
`public inline size_type `[`edge_index`](#da/d9c/classalps_1_1graph__helper_1a3d14d962e88213fb4ca98e74d0909ed6)`(const edge_descriptor & e) const` | 
`public inline size_type `[`index`](#da/d9c/classalps_1_1graph__helper_1a463568a85d2fbff688f2e7688e217c1e)`(const cell_descriptor & c) const` | 
`public inline size_type `[`index`](#da/d9c/classalps_1_1graph__helper_1ab1675c0b00a8ef0ab9af42831fd7bfe3)`(const vertex_descriptor & v) const` | 
`public inline size_type `[`index`](#da/d9c/classalps_1_1graph__helper_1a5f042dc93180a6513108551cae281cc9)`(const edge_descriptor & e) const` | 
`public inline std::pair< basis_vector_iterator, basis_vector_iterator > `[`basis_vectors`](#da/d9c/classalps_1_1graph__helper_1a8a99459d520f813545d4ca19e5586001)`() const` | 
`public inline std::pair< basis_vector_iterator, basis_vector_iterator > `[`reciprocal_basis_vectors`](#da/d9c/classalps_1_1graph__helper_1a7e124f402fbde96c6452ca96fdfaf5d1)`() const` | 
`public inline vector_type `[`origin`](#da/d9c/classalps_1_1graph__helper_1a6a0701a6caafbeaf8b67203e77ce333f)`(const cell_descriptor & c) const` | 
`public inline vector_type `[`coordinate`](#da/d9c/classalps_1_1graph__helper_1ab28a81ec04ee9ef4090e6e4314677a4c)`(const cell_descriptor & c,const vector_type & p) const` | 
`public inline vector_type `[`momentum`](#da/d9c/classalps_1_1graph__helper_1a732e14d0258f302c069e8685a3942ddb)`(const vector_type & m) const` | 
`public inline size_type `[`num_distances`](#da/d9c/classalps_1_1graph__helper_1a54ba8fbe1aaa9a0470d4edb4fa70319b)`() const` | 
`public inline std::vector< unsigned int > `[`distance_multiplicities`](#da/d9c/classalps_1_1graph__helper_1a36722c5dc55ff5cf81fbb8c086db4aa4)`() const` | 
`public inline std::vector< std::string > `[`momenta_labels`](#da/d9c/classalps_1_1graph__helper_1a97a8a5764511c614638160a2aa0dc315)`(int precision) const` | 
`public inline std::vector< std::string > `[`distance_labels`](#da/d9c/classalps_1_1graph__helper_1af57f3757d629946c8eceaeba2eb7c6ea)`(int precision) const` | 
`public inline std::string `[`site_label`](#da/d9c/classalps_1_1graph__helper_1ae731d4323fa03d66e8cc2fe4ac8c0283)`(site_descriptor const & s,int precision) const` | 
`public inline std::vector< std::string > `[`site_labels`](#da/d9c/classalps_1_1graph__helper_1aab822076e158438ea7c12802a9d560da)`(int precision) const` | 
`public inline std::string `[`bond_labels`](#da/d9c/classalps_1_1graph__helper_1a14f84a1ddd3ef29f21ecdedb01bbcafc)`(bond_descriptor const & b,int precision) const` | 
`public inline std::vector< std::string > `[`bond_labels`](#da/d9c/classalps_1_1graph__helper_1ac7352512fe1649d6639edba7b5fc2c89)`(int precision) const` | 
`public inline size_type `[`distance`](#da/d9c/classalps_1_1graph__helper_1a3d4adba0f1139f50c1304c53647f7867)`(vertex_descriptor x,vertex_descriptor y) const` | 
`public inline void `[`calculate_distances`](#da/d9c/classalps_1_1graph__helper_1ae836061a9dd719302453a5ce00057a6b)`() const` | 
`public inline std::vector< std::pair< std::complex< double >, std::vector< std::size_t > > > `[`translations`](#da/d9c/classalps_1_1graph__helper_1ae9010abf8a1d417b673003a563360711)`(const vector_type & k) const` | 
`public inline std::vector< int > `[`translation_directions`](#da/d9c/classalps_1_1graph__helper_1a4b4ea6e7a8259c6548c592ac280b7045)`() const` | 
`public inline std::vector< vector_type > `[`translation_momenta`](#da/d9c/classalps_1_1graph__helper_1a5563a0e42214e0968682e3602aba8da3)`() const` | 
`typedef `[`graph_type`](#da/d9c/classalps_1_1graph__helper_1a3a0b40536f2540053a6b3ffd55404714) | 
`typedef `[`lattice_type`](#da/d9c/classalps_1_1graph__helper_1a62bb7492fbcbf46da928c3b524d8a113) | 
`typedef `[`vertex_iterator`](#da/d9c/classalps_1_1graph__helper_1a922ec14a8ad9e17d923e51404f43f8a8) | 
`typedef `[`edge_iterator`](#da/d9c/classalps_1_1graph__helper_1a4bdce9766b8d58392c7bd114d3c4d352) | 
`typedef `[`out_edge_iterator`](#da/d9c/classalps_1_1graph__helper_1a8609c9add1602ce6d00296f640d2dc48) | 
`typedef `[`in_edge_iterator`](#da/d9c/classalps_1_1graph__helper_1acc09759652a8cc07a9b2b3e9f068054e) | 
`typedef `[`edge_descriptor`](#da/d9c/classalps_1_1graph__helper_1a5467f553ecdb7b3e7c6a301dbb3561ab) | 
`typedef `[`vertex_descriptor`](#da/d9c/classalps_1_1graph__helper_1ac615f7addc899f0125e5e6e58fc9a3ca) | 
`typedef `[`vertices_size_type`](#da/d9c/classalps_1_1graph__helper_1a8562ed63bfd75eaca2df00a8e1989ca2) | 
`typedef `[`edges_size_type`](#da/d9c/classalps_1_1graph__helper_1a3ab0a7947f7325c1a776157848e8f7b8) | 
`typedef `[`degree_size_type`](#da/d9c/classalps_1_1graph__helper_1a58d53def8dcce2801c3c7b358dafad46) | 
`typedef `[`adjacency_iterator`](#da/d9c/classalps_1_1graph__helper_1a0d0edbaf1d63ec67084ed5d8d05cf0cf) | 
`typedef `[`site_iterator`](#da/d9c/classalps_1_1graph__helper_1ab84717de779218b982142aec63adcdd4) | 
`typedef `[`bond_iterator`](#da/d9c/classalps_1_1graph__helper_1aa4950864c07d89a7558447ec47ab4fb9) | 
`typedef `[`neighbor_bond_iterator`](#da/d9c/classalps_1_1graph__helper_1aead478f1e25b6e64d53f90042b11018a) | 
`typedef `[`bond_descriptor`](#da/d9c/classalps_1_1graph__helper_1af404572682a9693821fbd3a48ec82ac4) | 
`typedef `[`site_descriptor`](#da/d9c/classalps_1_1graph__helper_1aee230a6575552ff6aadf9bc9498df5b9) | 
`typedef `[`sites_size_type`](#da/d9c/classalps_1_1graph__helper_1acc9b7458e564a11fb8f846e230262dad) | 
`typedef `[`bonds_size_type`](#da/d9c/classalps_1_1graph__helper_1a85609c9fd4a5c5e6dad2b248667be41d) | 
`typedef `[`neighbors_size_type`](#da/d9c/classalps_1_1graph__helper_1a91dede6e95c59c3814e90f8896cb13c3) | 
`typedef `[`neighbor_iterator`](#da/d9c/classalps_1_1graph__helper_1a9c723ccc6e523011297eeab6a5bbebcc) | 
`typedef `[`unit_cell_type`](#da/d9c/classalps_1_1graph__helper_1ad11afcadd96a26d557687826fa1a5e3a) | 
`typedef `[`cell_descriptor`](#da/d9c/classalps_1_1graph__helper_1a03bb56f8da345255c76c3fef9e904f2d) | 
`typedef `[`offset_type`](#da/d9c/classalps_1_1graph__helper_1ae997de4f500f493fad5cd5bd3365dac8) | 
`typedef `[`vector_type`](#da/d9c/classalps_1_1graph__helper_1a4c404bd2bf8d6bc1154ee48c9854b65b) | 
`typedef `[`size_type`](#da/d9c/classalps_1_1graph__helper_1ab88e182235d7e97679b8a55257981a6b) | 
`typedef `[`cell_iterator`](#da/d9c/classalps_1_1graph__helper_1aa1362173e6c651ebc182f21bfc36fd9e) | 
`typedef `[`momentum_iterator`](#da/d9c/classalps_1_1graph__helper_1aaf68e5369f32583f474feff8cd87db80) | 
`typedef `[`basis_vector_iterator`](#da/d9c/classalps_1_1graph__helper_1acdf390f0a6d4fab2d9bc23b907e58d5b) | 
`typedef `[`boundary_crossing_type`](#da/d9c/classalps_1_1graph__helper_1a9a2c6b356148152d8416dfd76edca4de) | 
`typedef `[`edge_type_map_type`](#da/d9c/classalps_1_1graph__helper_1ad203a9f8b566ab546d178ad73f3e09e1) | 
`typedef `[`bond_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a62f05947946410a514b76aec6123e584) | 
`typedef `[`vertex_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a67d2eb97e87370c40abe9e4cf28af230) | 
`typedef `[`site_type_map_type`](#da/d9c/classalps_1_1graph__helper_1af75afadbd64435cff4bafee4ce561d65) | 
`typedef `[`inhomogeneous_vertex_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a5c0be5dca86295afcabfe9d10fe08773) | 
`typedef `[`inhomogeneous_site_type_map_type`](#da/d9c/classalps_1_1graph__helper_1aa6fbeb84872a7cb7acea0c3d7042bedc) | 
`typedef `[`inhomogeneous_edge_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a5e4869b40a3a44fec5a2ae5c0b090ccb) | 
`typedef `[`inhomogeneous_bond_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a21a666a57792e7d73950a33f091fbfd4) | 

## Members

#### `public inline  `[`graph_helper`](#da/d9c/classalps_1_1graph__helper_1adde0193e9b7346ce5aad1a67865ac230)`(std::istream & in,const Parameters & p)` 

#### `public inline  `[`graph_helper`](#da/d9c/classalps_1_1graph__helper_1aa1684797abdf9837f9dda8d24d42c4c9)`(const alps::Parameters & p)` 

#### `public inline  `[`~graph_helper`](#da/d9c/classalps_1_1graph__helper_1a8b2dc8918994a6da29dc1662460c9e20)`()` 

#### `public inline graph_type & `[`graph`](#da/d9c/classalps_1_1graph__helper_1a48bec30b47cbf0ec6eefb8eccea572f7)`()` 

#### `public inline const graph_type & `[`graph`](#da/d9c/classalps_1_1graph__helper_1ab4bc73f875a4be9624a649fb33448924)`() const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::graph_type & `[`graph`](#da/d9c/classalps_1_1graph__helper_1a33337b909626756b5e4e882fbe9e30e3)`(H & g) const` 

#### `public template<>`  <br/>`inline const `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::graph_type & `[`graph`](#da/d9c/classalps_1_1graph__helper_1aa70d0c41f32af6b69f67cd701452aaaa)`(const H & g) const` 

#### `public inline `[`lattice_type`](#db/dc8/classalps_1_1lattice__graph)` & `[`lattice`](#da/d9c/classalps_1_1graph__helper_1a7166c07d787202a823548b15a9711458)`()` 

#### `public inline const `[`lattice_type`](#db/dc8/classalps_1_1lattice__graph)` & `[`lattice`](#da/d9c/classalps_1_1graph__helper_1a4ed48ae61643493e36024815161044bf)`() const` 

#### `public inline vertices_size_type `[`num_vertices`](#da/d9c/classalps_1_1graph__helper_1a3ab0aa6949be3b8ca87fecb926fd6b61)`() const` 

#### `public inline edges_size_type `[`num_edges`](#da/d9c/classalps_1_1graph__helper_1abede5f0a00e7ede0bd9056cb3b99e154)`() const` 

#### `public inline std::pair< vertex_iterator, vertex_iterator > `[`vertices`](#da/d9c/classalps_1_1graph__helper_1a26f9658eb64bd38efbbf5204edde4a81)`() const` 

#### `public inline std::pair< edge_iterator, edge_iterator > `[`edges`](#da/d9c/classalps_1_1graph__helper_1ae3438cb5ef3cc98af7f2e81f7ac88d74)`() const` 

#### `public inline degree_size_type `[`out_degree`](#da/d9c/classalps_1_1graph__helper_1ac8e323b16b0e7ee9555079c735371738)`(const vertex_descriptor & v) const` 

#### `public inline degree_size_type `[`in_degree`](#da/d9c/classalps_1_1graph__helper_1a7bbd494c52fa3b2f77fc6755751fa7ee)`(const vertex_descriptor & v) const` 

#### `public inline degree_size_type `[`degree`](#da/d9c/classalps_1_1graph__helper_1a222c4d0449b92a9512f574dbc7b999fd)`(const vertex_descriptor & v) const` 

#### `public inline std::pair< out_edge_iterator, out_edge_iterator > `[`out_edges`](#da/d9c/classalps_1_1graph__helper_1aab84adbfb1de97669d6846cdb2d30f10)`(const vertex_descriptor & v) const` 

#### `public inline std::pair< in_edge_iterator, in_edge_iterator > `[`in_edges`](#da/d9c/classalps_1_1graph__helper_1a5097cca53866b269b00bd975a849fa3d)`(const vertex_descriptor & v) const` 

#### `public inline std::pair< adjacency_iterator, adjacency_iterator > `[`adjacent_vertices`](#da/d9c/classalps_1_1graph__helper_1a422f7f3b44d1bd1b17b7e7843b5bff8e)`(const vertex_descriptor & v) const` 

#### `public inline vertex_descriptor `[`vertex`](#da/d9c/classalps_1_1graph__helper_1a3a674d6f4523e5077e50f1b6c6cd7e70)`(vertices_size_type i) const` 

#### `public inline site_descriptor `[`source`](#da/d9c/classalps_1_1graph__helper_1ade814b397ffece286639f4fb6ee79237)`(const bond_descriptor & b) const` 

#### `public inline site_descriptor `[`target`](#da/d9c/classalps_1_1graph__helper_1a0dee76813e338837997391e92e8ff304)`(const bond_descriptor & b) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertices_size_type `[`num_vertices`](#da/d9c/classalps_1_1graph__helper_1a9dddd766f3daf00a7ef1101448859413)`(const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::edges_size_type `[`num_edges`](#da/d9c/classalps_1_1graph__helper_1aee2691f36caa48fe1ba146ee2fee5877)`(const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::vertex_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_iterator > `[`vertices`](#da/d9c/classalps_1_1graph__helper_1a1a72347630b0795c41963786512bd8bd)`(const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::edge_iterator > `[`edges`](#da/d9c/classalps_1_1graph__helper_1a7660e2eafd6c326a2c0379260e5d6690)`(const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::degree_size_type `[`out_degree`](#da/d9c/classalps_1_1graph__helper_1a4e68d505ee0880dabd829a18bff0090f)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::degree_size_type `[`in_degree`](#da/d9c/classalps_1_1graph__helper_1a421b255086354975e4f88c7752ac43a2)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::degree_size_type `[`degree`](#da/d9c/classalps_1_1graph__helper_1ae536cd319060c0cc415a1741571e6417)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::out_edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::out_edge_iterator > `[`out_edges`](#da/d9c/classalps_1_1graph__helper_1a3a04d2ab1ff06353f74aab4524653be3)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::in_edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::in_edge_iterator > `[`in_edges`](#da/d9c/classalps_1_1graph__helper_1a85aa0301888187ab547359005d8b756f)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::adjacency_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::adjacency_iterator > `[`adjacent_vertices`](#da/d9c/classalps_1_1graph__helper_1ac242a3b460da42a12f23def4d09f1961)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertex_descriptor `[`vertex`](#da/d9c/classalps_1_1graph__helper_1a7b496fbf97766d061a5ab12b5412d3bf)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::vertices_size_type i,const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor `[`source`](#da/d9c/classalps_1_1graph__helper_1a047c30f044757241ccd1a250a5bccbb7)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bond_descriptor & b,const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor `[`target`](#da/d9c/classalps_1_1graph__helper_1aec37d31942a95373ae210e764b3d731d)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bond_descriptor & b,const H & g) const` 

#### `public inline sites_size_type `[`num_sites`](#da/d9c/classalps_1_1graph__helper_1aff7313ebbd1820a97b46d694dbbb787d)`() const` 

#### `public inline bonds_size_type `[`num_bonds`](#da/d9c/classalps_1_1graph__helper_1a32a85f1c3eeae18c70f120d4fd827232)`() const` 

#### `public inline std::pair< site_iterator, site_iterator > `[`sites`](#da/d9c/classalps_1_1graph__helper_1a690a8d6256396acae3bd659a4f95d580)`() const` 

#### `public inline site_descriptor `[`site`](#da/d9c/classalps_1_1graph__helper_1ac4c79b2c8eae8d8ef9108458be696d23)`(sites_size_type i) const` 

#### `public inline std::pair< bond_iterator, bond_iterator > `[`bonds`](#da/d9c/classalps_1_1graph__helper_1a04c4d663831eb0c4d390b1202ff8016c)`() const` 

#### `public inline bond_descriptor `[`bond`](#da/d9c/classalps_1_1graph__helper_1a3856964bd2e23f95ba89a1c14022a037)`(bonds_size_type i) const` 

#### `public inline neighbors_size_type `[`num_neighbors`](#da/d9c/classalps_1_1graph__helper_1a9fbb248be2daa346ec120abe7c22ec16)`(const site_descriptor & v) const` 

#### `public inline std::pair< neighbor_bond_iterator, neighbor_bond_iterator > `[`neighbor_bonds`](#da/d9c/classalps_1_1graph__helper_1acd95623364649f0bf6e10903c5321040)`(const site_descriptor & v) const` 

#### `public inline std::pair< neighbor_iterator, neighbor_iterator > `[`neighbors`](#da/d9c/classalps_1_1graph__helper_1a38e808cd387500955b48d10c00439212)`(const site_descriptor & v) const` 

#### `public inline site_descriptor `[`neighbor`](#da/d9c/classalps_1_1graph__helper_1a5998530e42e5a1b888dbe74fcd90a3b8)`(const site_descriptor & v,neighbors_size_type i) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::sites_size_type `[`num_sites`](#da/d9c/classalps_1_1graph__helper_1aa40acd68050e717e992a7c59d8e23337)`(const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bonds_size_type `[`num_bonds`](#da/d9c/classalps_1_1graph__helper_1a63fb1ba1f663d926052c6824edfbd703)`(const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::site_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_iterator > `[`sites`](#da/d9c/classalps_1_1graph__helper_1acaeb570aa88734f9e897ae3c931819ac)`(const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor `[`site`](#da/d9c/classalps_1_1graph__helper_1a99c3df1db758368023cf4c20c5f7c19e)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::sites_size_type i,const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::bond_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bond_iterator > `[`bonds`](#da/d9c/classalps_1_1graph__helper_1a9cbc6b809d57c2a6e2228a31143a0b7e)`(const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bond_descriptor `[`bond`](#da/d9c/classalps_1_1graph__helper_1a79b3ede8f8b3479cacf0b75e0905081a)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::bonds_size_type i,const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::neighbors_size_type `[`num_neighbors`](#da/d9c/classalps_1_1graph__helper_1abc5d669034bdae7d0cd4365d3a330cca)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::neighbor_bond_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::neighbor_bond_iterator > `[`neighbor_bonds`](#da/d9c/classalps_1_1graph__helper_1a070bc75e6a0232ba60b83626b34f84f4)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< H >::neighbor_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::neighbor_iterator > `[`neighbors`](#da/d9c/classalps_1_1graph__helper_1abb141953ed2507629bbcd5b3521dfc26)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor & v,const H & g) const` 

#### `public template<>`  <br/>`inline `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor `[`neighbor`](#da/d9c/classalps_1_1graph__helper_1a62bd08856b20115985f23cd70830aa77)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::site_descriptor & v,typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< H >::neighbors_size_type i,const H & g) const` 

#### `public inline double `[`parity`](#da/d9c/classalps_1_1graph__helper_1a9b50cacc36f36ed0da7f08c844bafb5a)`(const site_descriptor & v) const` 

#### `public inline bool `[`is_bipartite`](#da/d9c/classalps_1_1graph__helper_1ad7e3180360c5ad741cce68d588241ae7)`() const` 

#### `public inline vertex_type_map_type `[`vertex_type_map`](#da/d9c/classalps_1_1graph__helper_1ae911b1dd0edba7c0a5adbb986ef35efa)`() const` 

#### `public inline site_type_map_type `[`site_type_map`](#da/d9c/classalps_1_1graph__helper_1adf689be4bbb84b41b205ee94bb355f83)`() const` 

#### `public inline edge_type_map_type `[`edge_type_map`](#da/d9c/classalps_1_1graph__helper_1a01b165883a4ec8297560d3a38ad729db)`() const` 

#### `public inline bond_type_map_type `[`bond_type_map`](#da/d9c/classalps_1_1graph__helper_1a8601a717dce5236f6d0ce974a44caaf6)`() const` 

#### `public inline type_type `[`vertex_type`](#da/d9c/classalps_1_1graph__helper_1a9da3cc1017f93bc27911156cb72d9946)`(const vertex_descriptor & v) const` 

#### `public inline type_type `[`site_type`](#da/d9c/classalps_1_1graph__helper_1aacf8df2569142e25a9d130a935f95386)`(const site_descriptor & s) const` 

#### `public inline type_type `[`edge_type`](#da/d9c/classalps_1_1graph__helper_1a8a9847a7bf5f2358a42b886a28a01746)`(const edge_descriptor & e) const` 

#### `public inline type_type `[`bond_type`](#da/d9c/classalps_1_1graph__helper_1a3e12d6f34f7402f3576d1b9b1cb70414)`(const bond_descriptor & b) const` 

#### `public inline bool `[`inhomogeneous`](#da/d9c/classalps_1_1graph__helper_1ae680acd786b7f0ffbdd94d9ec346ea43)`() const` 

#### `public inline bool `[`inhomogeneous_vertices`](#da/d9c/classalps_1_1graph__helper_1af1754fa3f5638e83de7c2b1b87ddb6e2)`() const` 

#### `public inline bool `[`inhomogeneous_sites`](#da/d9c/classalps_1_1graph__helper_1aa254b754bcad07974fabb83f85e03306)`() const` 

#### `public inline bool `[`inhomogeneous_edges`](#da/d9c/classalps_1_1graph__helper_1a45b0971d3122cef662a6fd61f119b591)`() const` 

#### `public inline bool `[`inhomogeneous_bonds`](#da/d9c/classalps_1_1graph__helper_1a4224c791e0dc2bbc6148a5085c350a1f)`() const` 

#### `public inline inhomogeneous_vertex_type_map_type `[`inhomogeneous_vertex_type_map`](#da/d9c/classalps_1_1graph__helper_1a7509e0501a58ae38aa6809903869f358)`() const` 

#### `public inline inhomogeneous_site_type_map_type `[`inhomogeneous_site_type_map`](#da/d9c/classalps_1_1graph__helper_1a0fcb72b4acfe9f4509e52830b1797217)`() const` 

#### `public inline inhomogeneous_edge_type_map_type `[`inhomogeneous_edge_type_map`](#da/d9c/classalps_1_1graph__helper_1a801efb9fe2f66e671c328d271d593284)`() const` 

#### `public inline inhomogeneous_bond_type_map_type `[`inhomogeneous_bond_type_map`](#da/d9c/classalps_1_1graph__helper_1adebb95bbc578e36c55b2f7243b6e3015)`() const` 

#### `public inline type_type `[`inhomogeneous_vertex_type`](#da/d9c/classalps_1_1graph__helper_1a7a4a9497891b40d405c82c98fa1a862a)`(const vertex_descriptor & v) const` 

#### `public inline type_type `[`inhomogeneous_site_type`](#da/d9c/classalps_1_1graph__helper_1a853b8463d1250db1a5c8a09d40462ddd)`(const site_descriptor & s) const` 

#### `public inline type_type `[`inhomogeneous_edge_type`](#da/d9c/classalps_1_1graph__helper_1a0aa70045c07d6c94dfb503d7da09f2cf)`(const edge_descriptor & e) const` 

#### `public inline type_type `[`inhomogeneous_bond_type`](#da/d9c/classalps_1_1graph__helper_1a4226fc1a552ecdf84e854637a924a2e5)`(const bond_descriptor & b) const` 

#### `public inline const vector_type & `[`coordinate`](#da/d9c/classalps_1_1graph__helper_1ae414c95e65025212a27e0831764d2669)`(const site_descriptor & s) const` 

#### `public inline std::string `[`coordinate_string`](#da/d9c/classalps_1_1graph__helper_1abac50a96e10d34182651a3869c2328e2)`(const site_descriptor & s,int precision) const` 

#### `public inline const vector_type & `[`bond_vector`](#da/d9c/classalps_1_1graph__helper_1a23e18357d40568e5f61deb04d877f96c)`(const bond_descriptor & b) const` 

#### `public inline const vector_type & `[`bond_vector_relative`](#da/d9c/classalps_1_1graph__helper_1a4f388e74395b42943ce54cf9065c00fa)`(const bond_descriptor & b) const` 

#### `public inline std::size_t `[`dimension`](#da/d9c/classalps_1_1graph__helper_1a79e3181ee882eb2236455c4213af1421)`() const` 

#### `public inline std::pair< momentum_iterator, momentum_iterator > `[`momenta`](#da/d9c/classalps_1_1graph__helper_1a1d95a3316034859cab4ef760ad203f53)`() const` 

#### `public inline void `[`throw_if_xyz_defined`](#da/d9c/classalps_1_1graph__helper_1a4661bb1bcbee258a8f6e720d4f31f3ae)`(const Parameters & p,const vertex_descriptor &) const` 

#### `public inline void `[`throw_if_xyz_defined`](#da/d9c/classalps_1_1graph__helper_1a23bb6cd9e9347d1fbd096d2b84379a56)`(const Parameters & p,const edge_descriptor &) const` 

#### `public inline Parameters `[`coordinate_as_parameter`](#da/d9c/classalps_1_1graph__helper_1a4e30bb849bb111e607be6d78f2863c71)`(const edge_descriptor & e) const` 

#### `public inline Parameters `[`coordinate_as_parameter`](#da/d9c/classalps_1_1graph__helper_1a74ee8246db3a10f0a9b69ddba5572e56)`(const vertex_descriptor & v) const` 

#### `public inline size_type `[`volume`](#da/d9c/classalps_1_1graph__helper_1ac7de6175442489278535c9882cdd933a)`() const` 

#### `public inline const unit_cell_type & `[`unit_cell`](#da/d9c/classalps_1_1graph__helper_1adc5b55bbd2791484ab952a864851167b)`() const` 

#### `public inline cell_descriptor `[`cell`](#da/d9c/classalps_1_1graph__helper_1afd59185485b351736ac1ac89cf744278)`(const offset_type & o) const` 

#### `public inline std::pair< cell_iterator, cell_iterator > `[`cells`](#da/d9c/classalps_1_1graph__helper_1af1d01731515a2c7570269359c06f01fe)`() const` 

#### `public inline const offset_type & `[`offset`](#da/d9c/classalps_1_1graph__helper_1a40eeb11ed8e26f900f1d854c7402b63e)`(const cell_descriptor & c) const` 

#### `public inline bool `[`on_lattice`](#da/d9c/classalps_1_1graph__helper_1ab323cc5ebff9e1b0675c1fe4fefe8ed5)`(const offset_type & o) const` 

#### `public inline std::pair< bool, boundary_crossing_type > `[`shift`](#da/d9c/classalps_1_1graph__helper_1a4a778b0f2a874047c3425d17cfeca5fd)`(offset_type & o,const offset_type & s) const` 

#### `public inline size_type `[`cell_index`](#da/d9c/classalps_1_1graph__helper_1a7e342aab38e0339ad204f629a96f01f3)`(const cell_descriptor & c) const` 

#### `public inline size_type `[`vertex_index`](#da/d9c/classalps_1_1graph__helper_1a5e37f20e5b3614337c57e9e4606ee38d)`(const vertex_descriptor & v) const` 

#### `public inline size_type `[`edge_index`](#da/d9c/classalps_1_1graph__helper_1a3d14d962e88213fb4ca98e74d0909ed6)`(const edge_descriptor & e) const` 

#### `public inline size_type `[`index`](#da/d9c/classalps_1_1graph__helper_1a463568a85d2fbff688f2e7688e217c1e)`(const cell_descriptor & c) const` 

#### `public inline size_type `[`index`](#da/d9c/classalps_1_1graph__helper_1ab1675c0b00a8ef0ab9af42831fd7bfe3)`(const vertex_descriptor & v) const` 

#### `public inline size_type `[`index`](#da/d9c/classalps_1_1graph__helper_1a5f042dc93180a6513108551cae281cc9)`(const edge_descriptor & e) const` 

#### `public inline std::pair< basis_vector_iterator, basis_vector_iterator > `[`basis_vectors`](#da/d9c/classalps_1_1graph__helper_1a8a99459d520f813545d4ca19e5586001)`() const` 

#### `public inline std::pair< basis_vector_iterator, basis_vector_iterator > `[`reciprocal_basis_vectors`](#da/d9c/classalps_1_1graph__helper_1a7e124f402fbde96c6452ca96fdfaf5d1)`() const` 

#### `public inline vector_type `[`origin`](#da/d9c/classalps_1_1graph__helper_1a6a0701a6caafbeaf8b67203e77ce333f)`(const cell_descriptor & c) const` 

#### `public inline vector_type `[`coordinate`](#da/d9c/classalps_1_1graph__helper_1ab28a81ec04ee9ef4090e6e4314677a4c)`(const cell_descriptor & c,const vector_type & p) const` 

#### `public inline vector_type `[`momentum`](#da/d9c/classalps_1_1graph__helper_1a732e14d0258f302c069e8685a3942ddb)`(const vector_type & m) const` 

#### `public inline size_type `[`num_distances`](#da/d9c/classalps_1_1graph__helper_1a54ba8fbe1aaa9a0470d4edb4fa70319b)`() const` 

#### `public inline std::vector< unsigned int > `[`distance_multiplicities`](#da/d9c/classalps_1_1graph__helper_1a36722c5dc55ff5cf81fbb8c086db4aa4)`() const` 

#### `public inline std::vector< std::string > `[`momenta_labels`](#da/d9c/classalps_1_1graph__helper_1a97a8a5764511c614638160a2aa0dc315)`(int precision) const` 

#### `public inline std::vector< std::string > `[`distance_labels`](#da/d9c/classalps_1_1graph__helper_1af57f3757d629946c8eceaeba2eb7c6ea)`(int precision) const` 

#### `public inline std::string `[`site_label`](#da/d9c/classalps_1_1graph__helper_1ae731d4323fa03d66e8cc2fe4ac8c0283)`(site_descriptor const & s,int precision) const` 

#### `public inline std::vector< std::string > `[`site_labels`](#da/d9c/classalps_1_1graph__helper_1aab822076e158438ea7c12802a9d560da)`(int precision) const` 

#### `public inline std::string `[`bond_labels`](#da/d9c/classalps_1_1graph__helper_1a14f84a1ddd3ef29f21ecdedb01bbcafc)`(bond_descriptor const & b,int precision) const` 

#### `public inline std::vector< std::string > `[`bond_labels`](#da/d9c/classalps_1_1graph__helper_1ac7352512fe1649d6639edba7b5fc2c89)`(int precision) const` 

#### `public inline size_type `[`distance`](#da/d9c/classalps_1_1graph__helper_1a3d4adba0f1139f50c1304c53647f7867)`(vertex_descriptor x,vertex_descriptor y) const` 

#### `public inline void `[`calculate_distances`](#da/d9c/classalps_1_1graph__helper_1ae836061a9dd719302453a5ce00057a6b)`() const` 

#### `public inline std::vector< std::pair< std::complex< double >, std::vector< std::size_t > > > `[`translations`](#da/d9c/classalps_1_1graph__helper_1ae9010abf8a1d417b673003a563360711)`(const vector_type & k) const` 

#### `public inline std::vector< int > `[`translation_directions`](#da/d9c/classalps_1_1graph__helper_1a4b4ea6e7a8259c6548c592ac280b7045)`() const` 

#### `public inline std::vector< vector_type > `[`translation_momenta`](#da/d9c/classalps_1_1graph__helper_1a5563a0e42214e0968682e3602aba8da3)`() const` 

#### `typedef `[`graph_type`](#da/d9c/classalps_1_1graph__helper_1a3a0b40536f2540053a6b3ffd55404714) 

#### `typedef `[`lattice_type`](#da/d9c/classalps_1_1graph__helper_1a62bb7492fbcbf46da928c3b524d8a113) 

#### `typedef `[`vertex_iterator`](#da/d9c/classalps_1_1graph__helper_1a922ec14a8ad9e17d923e51404f43f8a8) 

#### `typedef `[`edge_iterator`](#da/d9c/classalps_1_1graph__helper_1a4bdce9766b8d58392c7bd114d3c4d352) 

#### `typedef `[`out_edge_iterator`](#da/d9c/classalps_1_1graph__helper_1a8609c9add1602ce6d00296f640d2dc48) 

#### `typedef `[`in_edge_iterator`](#da/d9c/classalps_1_1graph__helper_1acc09759652a8cc07a9b2b3e9f068054e) 

#### `typedef `[`edge_descriptor`](#da/d9c/classalps_1_1graph__helper_1a5467f553ecdb7b3e7c6a301dbb3561ab) 

#### `typedef `[`vertex_descriptor`](#da/d9c/classalps_1_1graph__helper_1ac615f7addc899f0125e5e6e58fc9a3ca) 

#### `typedef `[`vertices_size_type`](#da/d9c/classalps_1_1graph__helper_1a8562ed63bfd75eaca2df00a8e1989ca2) 

#### `typedef `[`edges_size_type`](#da/d9c/classalps_1_1graph__helper_1a3ab0a7947f7325c1a776157848e8f7b8) 

#### `typedef `[`degree_size_type`](#da/d9c/classalps_1_1graph__helper_1a58d53def8dcce2801c3c7b358dafad46) 

#### `typedef `[`adjacency_iterator`](#da/d9c/classalps_1_1graph__helper_1a0d0edbaf1d63ec67084ed5d8d05cf0cf) 

#### `typedef `[`site_iterator`](#da/d9c/classalps_1_1graph__helper_1ab84717de779218b982142aec63adcdd4) 

#### `typedef `[`bond_iterator`](#da/d9c/classalps_1_1graph__helper_1aa4950864c07d89a7558447ec47ab4fb9) 

#### `typedef `[`neighbor_bond_iterator`](#da/d9c/classalps_1_1graph__helper_1aead478f1e25b6e64d53f90042b11018a) 

#### `typedef `[`bond_descriptor`](#da/d9c/classalps_1_1graph__helper_1af404572682a9693821fbd3a48ec82ac4) 

#### `typedef `[`site_descriptor`](#da/d9c/classalps_1_1graph__helper_1aee230a6575552ff6aadf9bc9498df5b9) 

#### `typedef `[`sites_size_type`](#da/d9c/classalps_1_1graph__helper_1acc9b7458e564a11fb8f846e230262dad) 

#### `typedef `[`bonds_size_type`](#da/d9c/classalps_1_1graph__helper_1a85609c9fd4a5c5e6dad2b248667be41d) 

#### `typedef `[`neighbors_size_type`](#da/d9c/classalps_1_1graph__helper_1a91dede6e95c59c3814e90f8896cb13c3) 

#### `typedef `[`neighbor_iterator`](#da/d9c/classalps_1_1graph__helper_1a9c723ccc6e523011297eeab6a5bbebcc) 

#### `typedef `[`unit_cell_type`](#da/d9c/classalps_1_1graph__helper_1ad11afcadd96a26d557687826fa1a5e3a) 

#### `typedef `[`cell_descriptor`](#da/d9c/classalps_1_1graph__helper_1a03bb56f8da345255c76c3fef9e904f2d) 

#### `typedef `[`offset_type`](#da/d9c/classalps_1_1graph__helper_1ae997de4f500f493fad5cd5bd3365dac8) 

#### `typedef `[`vector_type`](#da/d9c/classalps_1_1graph__helper_1a4c404bd2bf8d6bc1154ee48c9854b65b) 

#### `typedef `[`size_type`](#da/d9c/classalps_1_1graph__helper_1ab88e182235d7e97679b8a55257981a6b) 

#### `typedef `[`cell_iterator`](#da/d9c/classalps_1_1graph__helper_1aa1362173e6c651ebc182f21bfc36fd9e) 

#### `typedef `[`momentum_iterator`](#da/d9c/classalps_1_1graph__helper_1aaf68e5369f32583f474feff8cd87db80) 

#### `typedef `[`basis_vector_iterator`](#da/d9c/classalps_1_1graph__helper_1acdf390f0a6d4fab2d9bc23b907e58d5b) 

#### `typedef `[`boundary_crossing_type`](#da/d9c/classalps_1_1graph__helper_1a9a2c6b356148152d8416dfd76edca4de) 

#### `typedef `[`edge_type_map_type`](#da/d9c/classalps_1_1graph__helper_1ad203a9f8b566ab546d178ad73f3e09e1) 

#### `typedef `[`bond_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a62f05947946410a514b76aec6123e584) 

#### `typedef `[`vertex_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a67d2eb97e87370c40abe9e4cf28af230) 

#### `typedef `[`site_type_map_type`](#da/d9c/classalps_1_1graph__helper_1af75afadbd64435cff4bafee4ce561d65) 

#### `typedef `[`inhomogeneous_vertex_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a5c0be5dca86295afcabfe9d10fe08773) 

#### `typedef `[`inhomogeneous_site_type_map_type`](#da/d9c/classalps_1_1graph__helper_1aa6fbeb84872a7cb7acea0c3d7042bedc) 

#### `typedef `[`inhomogeneous_edge_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a5e4869b40a3a44fec5a2ae5c0b090ccb) 

#### `typedef `[`inhomogeneous_bond_type_map_type`](#da/d9c/classalps_1_1graph__helper_1a21a666a57792e7d73950a33f091fbfd4) 

# class `alps::GraphUnitCell` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell_1ac6c70b2a6566ea4f83f7d3f05eb1464e)`()` | 
`public  `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell_1a3db7d720ff6af0e422c6eb4a40d69039)`(const `[`EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell)` & e)` | 
`public  `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell_1a229d161759164a97713a62d5b4a3051f)`(const XMLTag &,std::istream &)` | 
`public  `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell_1a7e128a3a5c6b4ef65d535fc5834f5cc3)`(const std::string & name,std::size_t dim)` | 
`public const `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & `[`operator=`](#d9/d50/classalps_1_1_graph_unit_cell_1a49dd510dd6d430d7a82acf7e6c9c8e7c)`(const `[`EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell)` & e)` | 
`public void `[`write_xml`](#d9/d50/classalps_1_1_graph_unit_cell_1a42f2fd86f55676a28e12ba866651a2c7)`(oxstream &) const` | 
`public inline `[`graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#d9/d50/classalps_1_1_graph_unit_cell_1adbaa3ea8d02da50ceda7b27e22d83b51)`()` | 
`public inline const `[`graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#d9/d50/classalps_1_1_graph_unit_cell_1aca601e52bed15dd84f56221b117c859b)`() const` | 
`public inline std::size_t `[`dimension`](#d9/d50/classalps_1_1_graph_unit_cell_1a1e6f2f8d8f8e76444572c3d85f2f5bd8)`() const` | 
`public inline const std::string & `[`name`](#d9/d50/classalps_1_1_graph_unit_cell_1a73e46d90226f0c9e693152d3bfc245eb)`() const` | 
`public std::size_t `[`add_vertex`](#d9/d50/classalps_1_1_graph_unit_cell_1aa9713493678b6551fa2a9bf3ef5b8124)`(int type,const coordinate_type & coord)` | 
`public std::size_t `[`add_edge`](#d9/d50/classalps_1_1_graph_unit_cell_1a5261873f3fec8fba9fd3ca92b9ec2c8e)`(int type,uint32_t si,const offset_type & so,uint32_t ti,const offset_type & to)` | 
`typedef `[`offset_type`](#d9/d50/classalps_1_1_graph_unit_cell_1a591cb66501cb78a2515590afdcf44b49) | 
`typedef `[`coordinate_type`](#d9/d50/classalps_1_1_graph_unit_cell_1ac3ea9bd32ce1e75abfb74f08c21147b9) | 
`typedef `[`graph_type`](#d9/d50/classalps_1_1_graph_unit_cell_1a1ef2378a356076ffc3d661b7e68311a0) | 

## Members

#### `public  `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell_1ac6c70b2a6566ea4f83f7d3f05eb1464e)`()` 

#### `public  `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell_1a3db7d720ff6af0e422c6eb4a40d69039)`(const `[`EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell)` & e)` 

#### `public  `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell_1a229d161759164a97713a62d5b4a3051f)`(const XMLTag &,std::istream &)` 

#### `public  `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell_1a7e128a3a5c6b4ef65d535fc5834f5cc3)`(const std::string & name,std::size_t dim)` 

#### `public const `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & `[`operator=`](#d9/d50/classalps_1_1_graph_unit_cell_1a49dd510dd6d430d7a82acf7e6c9c8e7c)`(const `[`EmptyUnitCell`](#de/dd5/classalps_1_1_empty_unit_cell)` & e)` 

#### `public void `[`write_xml`](#d9/d50/classalps_1_1_graph_unit_cell_1a42f2fd86f55676a28e12ba866651a2c7)`(oxstream &) const` 

#### `public inline `[`graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#d9/d50/classalps_1_1_graph_unit_cell_1adbaa3ea8d02da50ceda7b27e22d83b51)`()` 

#### `public inline const `[`graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#d9/d50/classalps_1_1_graph_unit_cell_1aca601e52bed15dd84f56221b117c859b)`() const` 

#### `public inline std::size_t `[`dimension`](#d9/d50/classalps_1_1_graph_unit_cell_1a1e6f2f8d8f8e76444572c3d85f2f5bd8)`() const` 

#### `public inline const std::string & `[`name`](#d9/d50/classalps_1_1_graph_unit_cell_1a73e46d90226f0c9e693152d3bfc245eb)`() const` 

#### `public std::size_t `[`add_vertex`](#d9/d50/classalps_1_1_graph_unit_cell_1aa9713493678b6551fa2a9bf3ef5b8124)`(int type,const coordinate_type & coord)` 

#### `public std::size_t `[`add_edge`](#d9/d50/classalps_1_1_graph_unit_cell_1a5261873f3fec8fba9fd3ca92b9ec2c8e)`(int type,uint32_t si,const offset_type & so,uint32_t ti,const offset_type & to)` 

#### `typedef `[`offset_type`](#d9/d50/classalps_1_1_graph_unit_cell_1a591cb66501cb78a2515590afdcf44b49) 

#### `typedef `[`coordinate_type`](#d9/d50/classalps_1_1_graph_unit_cell_1ac3ea9bd32ce1e75abfb74f08c21147b9) 

#### `typedef `[`graph_type`](#d9/d50/classalps_1_1_graph_unit_cell_1a1ef2378a356076ffc3d661b7e68311a0) 

# class `alps::hypercubic_lattice` 

```
class alps::hypercubic_lattice
  : public BASE
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a79975970bec8099c1f553b2e27c3b7fa)`()` | 
`public template<>`  <br/>`inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a1da3e07051bf633af259c88adb2106e1)`(const `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice)`< BASE2, EX2 > & l)` | 
`public inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a3ba539a92c955d096e5b6987c72cc9b1)`(const parent_lattice_type & p,size_type length,const std::string & bc)` | 
`public template<>`  <br/>`inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1ac60cf9a3db55571b58e45ac72e34fa75)`(const parent_lattice_type & p,InputIterator first,InputIterator last,const std::string & bc)` | 
`public template<>`  <br/>`inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1aa3d21d5e454905a60e559e0579d6bfe9)`(const parent_lattice_type & p,size_type length,InputIterator2 first2,InputIterator2 last2)` | 
`public template<>`  <br/>`inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a5eba3ec8a85ce767e2ab5e3e085e21be)`(const parent_lattice_type & p,InputIterator first,InputIterator last,InputIterator2 first2,InputIterator2 last2)` | 
`public template<>`  <br/>`inline const `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice)` & `[`operator=`](#d9/d9f/classalps_1_1hypercubic__lattice_1aaf5144039b10740f038aa398848254fe)`(const `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice)`< BASE2, EX2 > & l)` | 
`public inline std::pair< `[`cell_iterator](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator), [cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` > `[`cells`](#d9/d9f/classalps_1_1hypercubic__lattice_1a0a4cb0d8dc4a8666acc2f8b9e50b558b)`() const` | 
`public inline size_type `[`volume`](#d9/d9f/classalps_1_1hypercubic__lattice_1a3053d864d1cb9ad4ecae67f5e4b8bdb1)`() const` | 
`public inline size_type `[`index`](#d9/d9f/classalps_1_1hypercubic__lattice_1ae50b325334193bb4fce8e7b1e2f2f691)`(const cell_descriptor & c) const` | 
`public inline bool `[`on_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a677c108f876c401654b26d1c0e6c0709)`(const cell_descriptor & c) const` | 
`public inline cell_descriptor `[`cell`](#d9/d9f/classalps_1_1hypercubic__lattice_1a150ed4d0feec1a038963ad23709cd8a1)`(size_type i) const` | 
`public inline cell_descriptor `[`cell`](#d9/d9f/classalps_1_1hypercubic__lattice_1a4a029a3f5dd5bfcc5fc7cf4956f7d0b6)`(offset_type o) const` | 
`public inline std::pair< bool, `[`boundary_crossing_type`](#de/df2/structalps_1_1boundary__crossing)` > `[`shift`](#d9/d9f/classalps_1_1hypercubic__lattice_1a26fa04481b7ddae64f92bd74d7376f6c)`(offset_type & o,const offset_type & s) const` | 
`public inline const std::string & `[`boundary`](#d9/d9f/classalps_1_1hypercubic__lattice_1a164d32286ffb68aa63a87f0811bd74a1)`(unsigned int dim) const` | 
`public inline const std::vector< std::string > & `[`boundary`](#d9/d9f/classalps_1_1hypercubic__lattice_1a304b6416269350bfa5d894e2e53a2cb3)`() const` | 
`public inline extent_type::value_type `[`extent`](#d9/d9f/classalps_1_1hypercubic__lattice_1abdf61e61efc439a848d26a7b0ff2979e)`(unsigned int dim) const` | 
`public inline const extent_type & `[`extent`](#d9/d9f/classalps_1_1hypercubic__lattice_1a782ecc2518abb5523ce6fe8eb6018055)`() const` | 
`public inline std::vector< std::string > `[`distance_labels`](#d9/d9f/classalps_1_1hypercubic__lattice_1a6a9f5fa509bff9711efaafb2f3d7a0a2)`(int precision) const` | 
`public inline std::vector< std::string > `[`momenta_labels`](#d9/d9f/classalps_1_1hypercubic__lattice_1a6f1a952398af5335d5b3fcb0e0924080)`(int precision) const` | 
`public inline std::vector< unsigned int > `[`distance_multiplicities`](#d9/d9f/classalps_1_1hypercubic__lattice_1a0b81c00d0c6e0a81f2c394f422b3e54f)`() const` | 
`public inline std::size_t `[`num_distances`](#d9/d9f/classalps_1_1hypercubic__lattice_1a79a549de89daa6f32275f972d7b4b869)`() const` | 
`public inline std::size_t `[`distance`](#d9/d9f/classalps_1_1hypercubic__lattice_1a0f8f54b2e43f985bf784539580a5d73e)`(const offset_type & x,const offset_type & y) const` | 
`public inline std::pair< `[`momentum_iterator](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator), [momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator)` > `[`momenta`](#d9/d9f/classalps_1_1hypercubic__lattice_1aaa45d5b61254d3a01c403c66ab680046)`() const` | 
`public inline std::vector< int > `[`translation_directions`](#d9/d9f/classalps_1_1hypercubic__lattice_1a1ebb9e27c619ac913f339ee0c4fcc59b)`() const` | 
`public inline std::vector< vector_type > `[`translation_momenta`](#d9/d9f/classalps_1_1hypercubic__lattice_1a7dc2cf5fc1a5ea3a44c491395db69049)`() const` | 
`public inline std::vector< std::pair< std::complex< double >, std::vector< std::size_t > > > `[`translations`](#d9/d9f/classalps_1_1hypercubic__lattice_1aecc8b12ebe75f48055428dcdcc38e456)`(const vector_type & k) const` | 
`protected extent_type `[`extent_`](#d9/d9f/classalps_1_1hypercubic__lattice_1a105fbbff82e8e4049ea01c4a45000a80) | 
`protected std::vector< std::string > `[`bc_`](#d9/d9f/classalps_1_1hypercubic__lattice_1a5ea5c121245bc8fcd0137af558f23f65) | 
`typedef `[`lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1adbc562af254d0e26734cfdfc3a736cee) | 
`typedef `[`parent_lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1ad73e621524483053304f103dada30163) | 
`typedef `[`unit_cell_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1a1c8f2197c0947b3eb74f349ab4b0daab) | 
`typedef `[`cell_descriptor`](#d9/d9f/classalps_1_1hypercubic__lattice_1ac9825eba08b790de5b318751bd7bed4e) | 
`typedef `[`offset_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1ab4c5db22bcdcd75c241bb3409c1bdcf7) | 
`typedef `[`extent_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1ac3746d2fe3cbeb70f978f9cc7e229de9) | 
`typedef `[`basis_vector_iterator`](#d9/d9f/classalps_1_1hypercubic__lattice_1a6f5a54f01962713eb0713150bdda1bc0) | 
`typedef `[`vector_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1ae69079b4fa3a9d90226314e430662c32) | 
`typedef `[`boundary_crossing_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1a6d250aff229bb828e16f12c4c7fe1ebd) | 
`typedef `[`distance_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1a14edd4e4c98ed00b6d080b61b3b2277f) | 
`typedef `[`size_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1a101a2f4e15cecc730c3779d69e92a92e) | 

## Members

#### `public inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a79975970bec8099c1f553b2e27c3b7fa)`()` 

#### `public template<>`  <br/>`inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a1da3e07051bf633af259c88adb2106e1)`(const `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice)`< BASE2, EX2 > & l)` 

#### `public inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a3ba539a92c955d096e5b6987c72cc9b1)`(const parent_lattice_type & p,size_type length,const std::string & bc)` 

#### `public template<>`  <br/>`inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1ac60cf9a3db55571b58e45ac72e34fa75)`(const parent_lattice_type & p,InputIterator first,InputIterator last,const std::string & bc)` 

#### `public template<>`  <br/>`inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1aa3d21d5e454905a60e559e0579d6bfe9)`(const parent_lattice_type & p,size_type length,InputIterator2 first2,InputIterator2 last2)` 

#### `public template<>`  <br/>`inline  `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a5eba3ec8a85ce767e2ab5e3e085e21be)`(const parent_lattice_type & p,InputIterator first,InputIterator last,InputIterator2 first2,InputIterator2 last2)` 

#### `public template<>`  <br/>`inline const `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice)` & `[`operator=`](#d9/d9f/classalps_1_1hypercubic__lattice_1aaf5144039b10740f038aa398848254fe)`(const `[`hypercubic_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice)`< BASE2, EX2 > & l)` 

#### `public inline std::pair< `[`cell_iterator](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator), [cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` > `[`cells`](#d9/d9f/classalps_1_1hypercubic__lattice_1a0a4cb0d8dc4a8666acc2f8b9e50b558b)`() const` 

#### `public inline size_type `[`volume`](#d9/d9f/classalps_1_1hypercubic__lattice_1a3053d864d1cb9ad4ecae67f5e4b8bdb1)`() const` 

#### `public inline size_type `[`index`](#d9/d9f/classalps_1_1hypercubic__lattice_1ae50b325334193bb4fce8e7b1e2f2f691)`(const cell_descriptor & c) const` 

#### `public inline bool `[`on_lattice`](#d9/d9f/classalps_1_1hypercubic__lattice_1a677c108f876c401654b26d1c0e6c0709)`(const cell_descriptor & c) const` 

#### `public inline cell_descriptor `[`cell`](#d9/d9f/classalps_1_1hypercubic__lattice_1a150ed4d0feec1a038963ad23709cd8a1)`(size_type i) const` 

#### `public inline cell_descriptor `[`cell`](#d9/d9f/classalps_1_1hypercubic__lattice_1a4a029a3f5dd5bfcc5fc7cf4956f7d0b6)`(offset_type o) const` 

#### `public inline std::pair< bool, `[`boundary_crossing_type`](#de/df2/structalps_1_1boundary__crossing)` > `[`shift`](#d9/d9f/classalps_1_1hypercubic__lattice_1a26fa04481b7ddae64f92bd74d7376f6c)`(offset_type & o,const offset_type & s) const` 

#### `public inline const std::string & `[`boundary`](#d9/d9f/classalps_1_1hypercubic__lattice_1a164d32286ffb68aa63a87f0811bd74a1)`(unsigned int dim) const` 

#### `public inline const std::vector< std::string > & `[`boundary`](#d9/d9f/classalps_1_1hypercubic__lattice_1a304b6416269350bfa5d894e2e53a2cb3)`() const` 

#### `public inline extent_type::value_type `[`extent`](#d9/d9f/classalps_1_1hypercubic__lattice_1abdf61e61efc439a848d26a7b0ff2979e)`(unsigned int dim) const` 

#### `public inline const extent_type & `[`extent`](#d9/d9f/classalps_1_1hypercubic__lattice_1a782ecc2518abb5523ce6fe8eb6018055)`() const` 

#### `public inline std::vector< std::string > `[`distance_labels`](#d9/d9f/classalps_1_1hypercubic__lattice_1a6a9f5fa509bff9711efaafb2f3d7a0a2)`(int precision) const` 

#### `public inline std::vector< std::string > `[`momenta_labels`](#d9/d9f/classalps_1_1hypercubic__lattice_1a6f1a952398af5335d5b3fcb0e0924080)`(int precision) const` 

#### `public inline std::vector< unsigned int > `[`distance_multiplicities`](#d9/d9f/classalps_1_1hypercubic__lattice_1a0b81c00d0c6e0a81f2c394f422b3e54f)`() const` 

#### `public inline std::size_t `[`num_distances`](#d9/d9f/classalps_1_1hypercubic__lattice_1a79a549de89daa6f32275f972d7b4b869)`() const` 

#### `public inline std::size_t `[`distance`](#d9/d9f/classalps_1_1hypercubic__lattice_1a0f8f54b2e43f985bf784539580a5d73e)`(const offset_type & x,const offset_type & y) const` 

#### `public inline std::pair< `[`momentum_iterator](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator), [momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator)` > `[`momenta`](#d9/d9f/classalps_1_1hypercubic__lattice_1aaa45d5b61254d3a01c403c66ab680046)`() const` 

#### `public inline std::vector< int > `[`translation_directions`](#d9/d9f/classalps_1_1hypercubic__lattice_1a1ebb9e27c619ac913f339ee0c4fcc59b)`() const` 

#### `public inline std::vector< vector_type > `[`translation_momenta`](#d9/d9f/classalps_1_1hypercubic__lattice_1a7dc2cf5fc1a5ea3a44c491395db69049)`() const` 

#### `public inline std::vector< std::pair< std::complex< double >, std::vector< std::size_t > > > `[`translations`](#d9/d9f/classalps_1_1hypercubic__lattice_1aecc8b12ebe75f48055428dcdcc38e456)`(const vector_type & k) const` 

#### `protected extent_type `[`extent_`](#d9/d9f/classalps_1_1hypercubic__lattice_1a105fbbff82e8e4049ea01c4a45000a80) 

#### `protected std::vector< std::string > `[`bc_`](#d9/d9f/classalps_1_1hypercubic__lattice_1a5ea5c121245bc8fcd0137af558f23f65) 

#### `typedef `[`lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1adbc562af254d0e26734cfdfc3a736cee) 

#### `typedef `[`parent_lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1ad73e621524483053304f103dada30163) 

#### `typedef `[`unit_cell_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1a1c8f2197c0947b3eb74f349ab4b0daab) 

#### `typedef `[`cell_descriptor`](#d9/d9f/classalps_1_1hypercubic__lattice_1ac9825eba08b790de5b318751bd7bed4e) 

#### `typedef `[`offset_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1ab4c5db22bcdcd75c241bb3409c1bdcf7) 

#### `typedef `[`extent_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1ac3746d2fe3cbeb70f978f9cc7e229de9) 

#### `typedef `[`basis_vector_iterator`](#d9/d9f/classalps_1_1hypercubic__lattice_1a6f5a54f01962713eb0713150bdda1bc0) 

#### `typedef `[`vector_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1ae69079b4fa3a9d90226314e430662c32) 

#### `typedef `[`boundary_crossing_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1a6d250aff229bb828e16f12c4c7fe1ebd) 

#### `typedef `[`distance_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1a14edd4e4c98ed00b6d080b61b3b2277f) 

#### `typedef `[`size_type`](#d9/d9f/classalps_1_1hypercubic__lattice_1a101a2f4e15cecc730c3779d69e92a92e) 

# class `alps::InhomogeneityDescriptor` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a7baf544064601e80836efc2869e9cf10)`()` | 
`public  `[`InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a0902eb7eed0167ed89e62b5f6ec11919)`(XMLTag &,std::istream &)` | 
`public void `[`write_xml`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1afb5179fd324bc7fe82d8a1dbfa2a1bb1)`(oxstream &) const` | 
`public inline bool `[`inhomogeneous_vertices`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a56ffbcff8de6a4ec71d17d02cc6c0862)`() const` | 
`public inline bool `[`inhomogeneous_edges`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a92f9da2f942a563ed83899a324cabf3c)`() const` | 
`public inline bool `[`inhomogeneous_sites`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1aa6f13dbc5a2f993497fbf58007e6408d)`() const` | 
`public inline bool `[`inhomogeneous_bonds`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1aa2010ecd5191bfb6fc2fd1fb9c8cf2db)`() const` | 
`public inline bool `[`inhomogeneous`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1ab9fcc697124298f00c706a079e4859dd)`() const` | 
`public template<>`  <br/>`inline void `[`disorder_edges`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a16e352d70a0206042645608d39433893)`(G & g,M & m) const` | 
`public template<>`  <br/>`inline void `[`disorder_vertices`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1ac2a123ba1fd35d083051757ecc19d322)`(G & g,M & m) const` | 
`public template<>`  <br/>`inline void `[`disorder_vertices`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a7818c544559deed7e31557084233fa0c)`(G & g) const` | 
`public template<>`  <br/>`inline void `[`disorder_edges`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1ace6730b0ad7cf522b0be635458d2c7f2)`(G & g) const` | 
`public template<>`  <br/>`inline void `[`disorder_sites`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1ae48a029f3f90f1bef74e878998835c03)`(G & g) const` | 
`public template<>`  <br/>`inline void `[`disorder_sites`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a0a1bbdac0991308b2c3b70c7e1cc4dc6)`(G & g,M & m) const` | 
`public template<>`  <br/>`inline void `[`disorder_bonds`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a5d352cc6e90615212e6c8ffeff44c8ee)`(G & g) const` | 
`public template<>`  <br/>`inline void `[`disorder_bonds`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1acd5cfd30442d7fe82ef34f766d898b3c)`(G & g,M & m) const` | 

## Members

#### `public inline  `[`InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a7baf544064601e80836efc2869e9cf10)`()` 

#### `public  `[`InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a0902eb7eed0167ed89e62b5f6ec11919)`(XMLTag &,std::istream &)` 

#### `public void `[`write_xml`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1afb5179fd324bc7fe82d8a1dbfa2a1bb1)`(oxstream &) const` 

#### `public inline bool `[`inhomogeneous_vertices`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a56ffbcff8de6a4ec71d17d02cc6c0862)`() const` 

#### `public inline bool `[`inhomogeneous_edges`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a92f9da2f942a563ed83899a324cabf3c)`() const` 

#### `public inline bool `[`inhomogeneous_sites`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1aa6f13dbc5a2f993497fbf58007e6408d)`() const` 

#### `public inline bool `[`inhomogeneous_bonds`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1aa2010ecd5191bfb6fc2fd1fb9c8cf2db)`() const` 

#### `public inline bool `[`inhomogeneous`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1ab9fcc697124298f00c706a079e4859dd)`() const` 

#### `public template<>`  <br/>`inline void `[`disorder_edges`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a16e352d70a0206042645608d39433893)`(G & g,M & m) const` 

#### `public template<>`  <br/>`inline void `[`disorder_vertices`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1ac2a123ba1fd35d083051757ecc19d322)`(G & g,M & m) const` 

#### `public template<>`  <br/>`inline void `[`disorder_vertices`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a7818c544559deed7e31557084233fa0c)`(G & g) const` 

#### `public template<>`  <br/>`inline void `[`disorder_edges`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1ace6730b0ad7cf522b0be635458d2c7f2)`(G & g) const` 

#### `public template<>`  <br/>`inline void `[`disorder_sites`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1ae48a029f3f90f1bef74e878998835c03)`(G & g) const` 

#### `public template<>`  <br/>`inline void `[`disorder_sites`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a0a1bbdac0991308b2c3b70c7e1cc4dc6)`(G & g,M & m) const` 

#### `public template<>`  <br/>`inline void `[`disorder_bonds`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1a5d352cc6e90615212e6c8ffeff44c8ee)`(G & g) const` 

#### `public template<>`  <br/>`inline void `[`disorder_bonds`](#d1/d80/classalps_1_1_inhomogeneity_descriptor_1acd5cfd30442d7fe82ef34f766d898b3c)`(G & g,M & m) const` 

# class `alps::lattice_graph` 

```
class alps::lattice_graph
  : public LATTICE
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph_1a37c57f759d55b6ddce806b7fafa96b2f)`()` | 
`public template<>`  <br/>`inline  `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph_1adba07453e169dda434ae0aefadf964bf)`(const L2 &)` | 
`public inline const graph_type & `[`graph`](#db/dc8/classalps_1_1lattice__graph_1ac0a36b0c4973a2c063bcb69d8ab319dd)`() const` | 
`public inline graph_type & `[`graph`](#db/dc8/classalps_1_1lattice__graph_1a414ebd1165d27e4a5cd384ca6e872df4)`()` | 
`public template<>`  <br/>`inline H::graph_type & `[`graph`](#db/dc8/classalps_1_1lattice__graph_1a1d174e2eff3cf534f7ca1041b6f6781e)`(H & g) const` | 
`public template<>`  <br/>`inline const H::graph_type & `[`graph`](#db/dc8/classalps_1_1lattice__graph_1a6f3058f3a2c5a02a7d75cf15d168b0da)`(const H & g) const` | 
`public inline std::vector< std::string > `[`distance_labels`](#db/dc8/classalps_1_1lattice__graph_1ab535da929fe2ae6a458db6f091fcd43e)`(int precision) const` | 
`public inline std::vector< unsigned int > `[`distance_multiplicities`](#db/dc8/classalps_1_1lattice__graph_1a5fbb728c7263a87161b85ba407b818ec)`() const` | 
`public inline size_type `[`num_distances`](#db/dc8/classalps_1_1lattice__graph_1ad749f67c67b8575cb19d0c1d14d5eda6)`() const` | 
`public inline size_type `[`distance`](#db/dc8/classalps_1_1lattice__graph_1ac1b722a142b9534b8cb08e4938f6a6df)`(vertex_descriptor x,vertex_descriptor y) const` | 
`public inline std::vector< std::pair< std::complex< double >, std::vector< std::size_t > > > `[`translations`](#db/dc8/classalps_1_1lattice__graph_1a44ee64b6aa85f08765b327f09c19e978)`(const vector_type & k) const` | 
`typedef `[`super_type`](#db/dc8/classalps_1_1lattice__graph_1a88af18f6f61aaca44bde9beedcf9b3a9) | 
`typedef `[`base_type`](#db/dc8/classalps_1_1lattice__graph_1a0db320877848b54b576e9a8ca004ec96) | 
`typedef `[`unit_cell_type`](#db/dc8/classalps_1_1lattice__graph_1a770ce5deef8825e7a320df1b37b1bcec) | 
`typedef `[`offset_type`](#db/dc8/classalps_1_1lattice__graph_1ae04323b2f673659f1be62bf5f81a11c4) | 
`typedef `[`extent_type`](#db/dc8/classalps_1_1lattice__graph_1ad9ad8356b94f482bad159b262bb8d715) | 
`typedef `[`vector_type`](#db/dc8/classalps_1_1lattice__graph_1a244c97f17da6aafce245b139baa3e768) | 
`typedef `[`basis_vector_iterator`](#db/dc8/classalps_1_1lattice__graph_1a93fd1c65d76caeaffad9eb6dddf423b8) | 
`typedef `[`cell_iterator`](#db/dc8/classalps_1_1lattice__graph_1a7bdab60f7646cbde95364e3641ecf589) | 
`typedef `[`boundary_crossing_type`](#db/dc8/classalps_1_1lattice__graph_1aaf63c622bbfb787337e68268405b9064) | 
`typedef `[`size_type`](#db/dc8/classalps_1_1lattice__graph_1a586d9794b1def6f6035fc6f3b3130d9c) | 
`typedef `[`graph_type`](#db/dc8/classalps_1_1lattice__graph_1af42d808e6f8e997b35e3b6b1a101af35) | 
`typedef `[`vertex_iterator`](#db/dc8/classalps_1_1lattice__graph_1a0706668f5cb9c19226bd18663cdad225) | 
`typedef `[`vertex_descriptor`](#db/dc8/classalps_1_1lattice__graph_1a198df4f2a5f731d20ce2f62180fd22e8) | 
`typedef `[`edge_iterator`](#db/dc8/classalps_1_1lattice__graph_1aadd2cd6345fce423cceeb8282b1e669c) | 

## Members

#### `public inline  `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph_1a37c57f759d55b6ddce806b7fafa96b2f)`()` 

#### `public template<>`  <br/>`inline  `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph_1adba07453e169dda434ae0aefadf964bf)`(const L2 &)` 

#### `public inline const graph_type & `[`graph`](#db/dc8/classalps_1_1lattice__graph_1ac0a36b0c4973a2c063bcb69d8ab319dd)`() const` 

#### `public inline graph_type & `[`graph`](#db/dc8/classalps_1_1lattice__graph_1a414ebd1165d27e4a5cd384ca6e872df4)`()` 

#### `public template<>`  <br/>`inline H::graph_type & `[`graph`](#db/dc8/classalps_1_1lattice__graph_1a1d174e2eff3cf534f7ca1041b6f6781e)`(H & g) const` 

#### `public template<>`  <br/>`inline const H::graph_type & `[`graph`](#db/dc8/classalps_1_1lattice__graph_1a6f3058f3a2c5a02a7d75cf15d168b0da)`(const H & g) const` 

#### `public inline std::vector< std::string > `[`distance_labels`](#db/dc8/classalps_1_1lattice__graph_1ab535da929fe2ae6a458db6f091fcd43e)`(int precision) const` 

#### `public inline std::vector< unsigned int > `[`distance_multiplicities`](#db/dc8/classalps_1_1lattice__graph_1a5fbb728c7263a87161b85ba407b818ec)`() const` 

#### `public inline size_type `[`num_distances`](#db/dc8/classalps_1_1lattice__graph_1ad749f67c67b8575cb19d0c1d14d5eda6)`() const` 

#### `public inline size_type `[`distance`](#db/dc8/classalps_1_1lattice__graph_1ac1b722a142b9534b8cb08e4938f6a6df)`(vertex_descriptor x,vertex_descriptor y) const` 

#### `public inline std::vector< std::pair< std::complex< double >, std::vector< std::size_t > > > `[`translations`](#db/dc8/classalps_1_1lattice__graph_1a44ee64b6aa85f08765b327f09c19e978)`(const vector_type & k) const` 

#### `typedef `[`super_type`](#db/dc8/classalps_1_1lattice__graph_1a88af18f6f61aaca44bde9beedcf9b3a9) 

#### `typedef `[`base_type`](#db/dc8/classalps_1_1lattice__graph_1a0db320877848b54b576e9a8ca004ec96) 

#### `typedef `[`unit_cell_type`](#db/dc8/classalps_1_1lattice__graph_1a770ce5deef8825e7a320df1b37b1bcec) 

#### `typedef `[`offset_type`](#db/dc8/classalps_1_1lattice__graph_1ae04323b2f673659f1be62bf5f81a11c4) 

#### `typedef `[`extent_type`](#db/dc8/classalps_1_1lattice__graph_1ad9ad8356b94f482bad159b262bb8d715) 

#### `typedef `[`vector_type`](#db/dc8/classalps_1_1lattice__graph_1a244c97f17da6aafce245b139baa3e768) 

#### `typedef `[`basis_vector_iterator`](#db/dc8/classalps_1_1lattice__graph_1a93fd1c65d76caeaffad9eb6dddf423b8) 

#### `typedef `[`cell_iterator`](#db/dc8/classalps_1_1lattice__graph_1a7bdab60f7646cbde95364e3641ecf589) 

#### `typedef `[`boundary_crossing_type`](#db/dc8/classalps_1_1lattice__graph_1aaf63c622bbfb787337e68268405b9064) 

#### `typedef `[`size_type`](#db/dc8/classalps_1_1lattice__graph_1a586d9794b1def6f6035fc6f3b3130d9c) 

#### `typedef `[`graph_type`](#db/dc8/classalps_1_1lattice__graph_1af42d808e6f8e997b35e3b6b1a101af35) 

#### `typedef `[`vertex_iterator`](#db/dc8/classalps_1_1lattice__graph_1a0706668f5cb9c19226bd18663cdad225) 

#### `typedef `[`vertex_descriptor`](#db/dc8/classalps_1_1lattice__graph_1a198df4f2a5f731d20ce2f62180fd22e8) 

#### `typedef `[`edge_iterator`](#db/dc8/classalps_1_1lattice__graph_1aadd2cd6345fce423cceeb8282b1e669c) 

# class `alps::LatticeDescriptor` 

```
class alps::LatticeDescriptor
  : public alps::coordinate_lattice< simple_lattice<>, std::vector< alps::StringValue > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor_1adfe88660a3eead05ee961ce1c6e59cc3)`()` | 
`public inline  `[`LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor_1a534c577463329d61f67114de66a9c010)`(const std::string & name,std::size_t dim)` | 
`public  `[`LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor_1a12befac41aaf1fe4103a9dc890c44eb4)`(const alps::XMLTag &,std::istream &)` | 
`public void `[`write_xml`](#d0/dc6/classalps_1_1_lattice_descriptor_1aae80e3f5388cc7ebb350bfd76519ec07)`(oxstream &) const` | 
`public inline const std::string & `[`name`](#d0/dc6/classalps_1_1_lattice_descriptor_1a580f0a1e435ec78c7832028e857771ad)`() const` | 
`public inline std::size_t `[`dimension`](#d0/dc6/classalps_1_1_lattice_descriptor_1a7f8ecdc2a959b692c632a6b4c2184a15)`() const` | 
`public void `[`set_parameters`](#d0/dc6/classalps_1_1_lattice_descriptor_1a21c0c8803013bf776e50a8dfef3d8081)`(const alps::Parameters &)` | 
`public template<>`  <br/>`inline void `[`add_default_parameter`](#d0/dc6/classalps_1_1_lattice_descriptor_1a3897eaa6c5d7cee38d4e0cecf9603bdf)`(const std::string & name,const T & value)` | 
`typedef `[`base_type`](#d0/dc6/classalps_1_1_lattice_descriptor_1a2d764491cdc5a7b7db21615420b48821) | 
`typedef `[`unit_cell_type`](#d0/dc6/classalps_1_1_lattice_descriptor_1afa3dbd9290ad1030292e46eaafb240c4) | 
`typedef `[`offset_type`](#d0/dc6/classalps_1_1_lattice_descriptor_1ac5087e9da6ba6b7a5fc520d389c507a0) | 
`typedef `[`cell_descriptor`](#d0/dc6/classalps_1_1_lattice_descriptor_1abfeb2a32ec6fe2ec6f96150c3d4ccb65) | 
`typedef `[`vector_type`](#d0/dc6/classalps_1_1_lattice_descriptor_1af284e04bf64aed180b8bc6bad179f3c5) | 
`typedef `[`basis_vector_iterator`](#d0/dc6/classalps_1_1_lattice_descriptor_1a1947c847e33238206b6e4463dd03ea37) | 

## Members

#### `public inline  `[`LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor_1adfe88660a3eead05ee961ce1c6e59cc3)`()` 

#### `public inline  `[`LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor_1a534c577463329d61f67114de66a9c010)`(const std::string & name,std::size_t dim)` 

#### `public  `[`LatticeDescriptor`](#d0/dc6/classalps_1_1_lattice_descriptor_1a12befac41aaf1fe4103a9dc890c44eb4)`(const alps::XMLTag &,std::istream &)` 

#### `public void `[`write_xml`](#d0/dc6/classalps_1_1_lattice_descriptor_1aae80e3f5388cc7ebb350bfd76519ec07)`(oxstream &) const` 

#### `public inline const std::string & `[`name`](#d0/dc6/classalps_1_1_lattice_descriptor_1a580f0a1e435ec78c7832028e857771ad)`() const` 

#### `public inline std::size_t `[`dimension`](#d0/dc6/classalps_1_1_lattice_descriptor_1a7f8ecdc2a959b692c632a6b4c2184a15)`() const` 

#### `public void `[`set_parameters`](#d0/dc6/classalps_1_1_lattice_descriptor_1a21c0c8803013bf776e50a8dfef3d8081)`(const alps::Parameters &)` 

#### `public template<>`  <br/>`inline void `[`add_default_parameter`](#d0/dc6/classalps_1_1_lattice_descriptor_1a3897eaa6c5d7cee38d4e0cecf9603bdf)`(const std::string & name,const T & value)` 

#### `typedef `[`base_type`](#d0/dc6/classalps_1_1_lattice_descriptor_1a2d764491cdc5a7b7db21615420b48821) 

#### `typedef `[`unit_cell_type`](#d0/dc6/classalps_1_1_lattice_descriptor_1afa3dbd9290ad1030292e46eaafb240c4) 

#### `typedef `[`offset_type`](#d0/dc6/classalps_1_1_lattice_descriptor_1ac5087e9da6ba6b7a5fc520d389c507a0) 

#### `typedef `[`cell_descriptor`](#d0/dc6/classalps_1_1_lattice_descriptor_1abfeb2a32ec6fe2ec6f96150c3d4ccb65) 

#### `typedef `[`vector_type`](#d0/dc6/classalps_1_1_lattice_descriptor_1af284e04bf64aed180b8bc6bad179f3c5) 

#### `typedef `[`basis_vector_iterator`](#d0/dc6/classalps_1_1_lattice_descriptor_1a1947c847e33238206b6e4463dd03ea37) 

# class `alps::LatticeGraphDescriptor` 

```
class alps::LatticeGraphDescriptor
  : public alps::hypercubic_lattice< coordinate_lattice< simple_lattice< GraphUnitCell >, std::vector< StringValue > >, std::vector< StringValue > >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a90984437b095dc643e3f6c7c7e1a0505)`()` | 
`public  `[`LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a5afc4df3a326d4342c218769ac0afa05)`(const std::string & unitcell,const UnitCellMap &)` | 
`public  `[`LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a9529ba7076c1eedccbefa8c3f2094c6a)`(const XMLTag &,std::istream &,const LatticeMap &,const FiniteLatticeMap &,const UnitCellMap &)` | 
`public void `[`write_xml`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1aec70cbc3de1f074776887d29c89d8f09)`(oxstream &) const` | 
`public inline const std::string & `[`name`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a8cdf54ef2790f407517dea4d4653a9c7)`() const` | 
`public void `[`set_parameters`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a2dcc7a3e55542e2c68a3c2c664c1ac8f)`(const Parameters &)` | 
`public inline const `[`InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor)` & `[`inhomogeneity`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1ad86230205ee14c8b761bafb2fa2c208e)`() const` | 
`public inline const `[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` & `[`depletion`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1ad39edb275203dd52544dc5899971f9b7)`() const` | 
`typedef `[`base_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a064d08c66f5dfdac61c0bb9d21e7fb56) | 
`typedef `[`unit_cell_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1ab5a836dea46cbb513283acd49274dc87) | 
`typedef `[`offset_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1af89ec4f6ac664d3698da8ca850d862ca) | 
`typedef `[`extent_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1aeee7f75f7543ae62b9c0bbec9dd249a9) | 
`typedef `[`cell_descriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1ad3c824900ff186a81b8fa6d71e77e21a) | 
`typedef `[`vector_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a52f377d5dacd842d5af27d88d6533d74) | 
`typedef `[`basis_vector_iterator`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1afb57d3599e7e9a194145156fe893d274) | 
`typedef `[`cell_iterator`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a2a8f2327ff190294d1d9d5e22d538873) | 
`typedef `[`size_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a66bac05469422760e35a9cccc67ce7d8) | 
`typedef `[`boundary_crossing_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1afc563fd5f782f6fedb7b535bf409256c) | 

## Members

#### `public inline  `[`LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a90984437b095dc643e3f6c7c7e1a0505)`()` 

#### `public  `[`LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a5afc4df3a326d4342c218769ac0afa05)`(const std::string & unitcell,const UnitCellMap &)` 

#### `public  `[`LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a9529ba7076c1eedccbefa8c3f2094c6a)`(const XMLTag &,std::istream &,const LatticeMap &,const FiniteLatticeMap &,const UnitCellMap &)` 

#### `public void `[`write_xml`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1aec70cbc3de1f074776887d29c89d8f09)`(oxstream &) const` 

#### `public inline const std::string & `[`name`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a8cdf54ef2790f407517dea4d4653a9c7)`() const` 

#### `public void `[`set_parameters`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a2dcc7a3e55542e2c68a3c2c664c1ac8f)`(const Parameters &)` 

#### `public inline const `[`InhomogeneityDescriptor`](#d1/d80/classalps_1_1_inhomogeneity_descriptor)` & `[`inhomogeneity`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1ad86230205ee14c8b761bafb2fa2c208e)`() const` 

#### `public inline const `[`DepletionDescriptor`](#d9/dd8/classalps_1_1_depletion_descriptor)` & `[`depletion`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1ad39edb275203dd52544dc5899971f9b7)`() const` 

#### `typedef `[`base_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a064d08c66f5dfdac61c0bb9d21e7fb56) 

#### `typedef `[`unit_cell_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1ab5a836dea46cbb513283acd49274dc87) 

#### `typedef `[`offset_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1af89ec4f6ac664d3698da8ca850d862ca) 

#### `typedef `[`extent_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1aeee7f75f7543ae62b9c0bbec9dd249a9) 

#### `typedef `[`cell_descriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1ad3c824900ff186a81b8fa6d71e77e21a) 

#### `typedef `[`vector_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a52f377d5dacd842d5af27d88d6533d74) 

#### `typedef `[`basis_vector_iterator`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1afb57d3599e7e9a194145156fe893d274) 

#### `typedef `[`cell_iterator`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a2a8f2327ff190294d1d9d5e22d538873) 

#### `typedef `[`size_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1a66bac05469422760e35a9cccc67ce7d8) 

#### `typedef `[`boundary_crossing_type`](#d5/d81/classalps_1_1_lattice_graph_descriptor_1afc563fd5f782f6fedb7b535bf409256c) 

# class `alps::LatticeLibrary` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`LatticeLibrary`](#de/da5/classalps_1_1_lattice_library_1ac34bfa1abc9512f10ddf304f3a132145)`()` | 
`public inline  `[`LatticeLibrary`](#de/da5/classalps_1_1_lattice_library_1a243900ffa23bb33263d29bfeb7a9d2de)`(std::istream & in)` | 
`public inline  `[`LatticeLibrary`](#de/da5/classalps_1_1_lattice_library_1aebb9274d16fe0067858f09d7850db3e3)`(const XMLTag & tag,std::istream & p)` | 
`public  `[`LatticeLibrary`](#de/da5/classalps_1_1_lattice_library_1aa7d021b01260cf380e5a55b1d88c76c4)`(const Parameters & p)` | 
`public void `[`read_xml`](#de/da5/classalps_1_1_lattice_library_1a797c29a9a399df3f8e5d73e977d38b1b)`(std::istream & in)` | 
`public void `[`read_xml`](#de/da5/classalps_1_1_lattice_library_1a6613d4f19ae66214edee14861db0b095)`(const XMLTag & tag,std::istream & p)` | 
`public void `[`write_xml`](#de/da5/classalps_1_1_lattice_library_1ad1d9affc673346a0662cfd506a4093a0)`(oxstream &) const` | 
`public bool `[`has_graph`](#de/da5/classalps_1_1_lattice_library_1aeacc1e33b5db454aa45c86d02fc118b5)`(const std::string & name) const` | 
`public bool `[`has_lattice`](#de/da5/classalps_1_1_lattice_library_1aff149db03860249cc8a0a9c7171c893e)`(const std::string & name) const` | 
`public bool `[`has_unitcell`](#de/da5/classalps_1_1_lattice_library_1ae96a7c3f1f83a7ab7524773c50c034f1)`(const std::string & name) const` | 
`public const `[`LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor)` & `[`lattice_descriptor`](#de/da5/classalps_1_1_lattice_library_1a1f01683fb9062e06d4123a56efb319db)`(const std::string & name) const` | 
`public `[`lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice)` `[`lattice`](#de/da5/classalps_1_1_lattice_library_1a1bfcfb2b66e928b75aac2ede0ade4e3c)`(const std::string & name) const` | 
`public const `[`coordinate_graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#de/da5/classalps_1_1_lattice_library_1a39a0c139903262e236b3c085521e28eb)`(const std::string & name) const` | 
`public template<>`  <br/>`inline bool `[`get_graph`](#de/da5/classalps_1_1_lattice_library_1ad884fcd9a8e9da7fce22d475d9174437)`(G & graph,const std::string & name) const` | 
`public void `[`make_all_graphs`](#de/da5/classalps_1_1_lattice_library_1a2c3134c3797f11a75056bdadafb5ad4d)`()` | 
`protected LatticeMap `[`lattices_`](#de/da5/classalps_1_1_lattice_library_1ad3b7c8ac3aec732af52d742376796de4) | 
`protected FiniteLatticeMap `[`finitelattices_`](#de/da5/classalps_1_1_lattice_library_1afe3192db11f5752c37d13c0740bf8644) | 
`protected UnitCellMap `[`unitcells_`](#de/da5/classalps_1_1_lattice_library_1a0c949f387243e8739a06ae527153b0f9) | 
`protected LatticeGraphMap `[`latticegraphs_`](#de/da5/classalps_1_1_lattice_library_1ab4a68507151310533b03bf152d24bbe4) | 
`protected GraphMap `[`graphs_`](#de/da5/classalps_1_1_lattice_library_1a68b6cbbc1bfebc3f48bfba3584cd8c5c) | 
`typedef `[`lattice_type`](#de/da5/classalps_1_1_lattice_library_1a73f3971127bd8c2bf73aa6218cb8b183) | 

## Members

#### `public inline  `[`LatticeLibrary`](#de/da5/classalps_1_1_lattice_library_1ac34bfa1abc9512f10ddf304f3a132145)`()` 

#### `public inline  `[`LatticeLibrary`](#de/da5/classalps_1_1_lattice_library_1a243900ffa23bb33263d29bfeb7a9d2de)`(std::istream & in)` 

#### `public inline  `[`LatticeLibrary`](#de/da5/classalps_1_1_lattice_library_1aebb9274d16fe0067858f09d7850db3e3)`(const XMLTag & tag,std::istream & p)` 

#### `public  `[`LatticeLibrary`](#de/da5/classalps_1_1_lattice_library_1aa7d021b01260cf380e5a55b1d88c76c4)`(const Parameters & p)` 

#### `public void `[`read_xml`](#de/da5/classalps_1_1_lattice_library_1a797c29a9a399df3f8e5d73e977d38b1b)`(std::istream & in)` 

#### `public void `[`read_xml`](#de/da5/classalps_1_1_lattice_library_1a6613d4f19ae66214edee14861db0b095)`(const XMLTag & tag,std::istream & p)` 

#### `public void `[`write_xml`](#de/da5/classalps_1_1_lattice_library_1ad1d9affc673346a0662cfd506a4093a0)`(oxstream &) const` 

#### `public bool `[`has_graph`](#de/da5/classalps_1_1_lattice_library_1aeacc1e33b5db454aa45c86d02fc118b5)`(const std::string & name) const` 

#### `public bool `[`has_lattice`](#de/da5/classalps_1_1_lattice_library_1aff149db03860249cc8a0a9c7171c893e)`(const std::string & name) const` 

#### `public bool `[`has_unitcell`](#de/da5/classalps_1_1_lattice_library_1ae96a7c3f1f83a7ab7524773c50c034f1)`(const std::string & name) const` 

#### `public const `[`LatticeGraphDescriptor`](#d5/d81/classalps_1_1_lattice_graph_descriptor)` & `[`lattice_descriptor`](#de/da5/classalps_1_1_lattice_library_1a1f01683fb9062e06d4123a56efb319db)`(const std::string & name) const` 

#### `public `[`lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice)` `[`lattice`](#de/da5/classalps_1_1_lattice_library_1a1bfcfb2b66e928b75aac2ede0ade4e3c)`(const std::string & name) const` 

#### `public const `[`coordinate_graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#de/da5/classalps_1_1_lattice_library_1a39a0c139903262e236b3c085521e28eb)`(const std::string & name) const` 

#### `public template<>`  <br/>`inline bool `[`get_graph`](#de/da5/classalps_1_1_lattice_library_1ad884fcd9a8e9da7fce22d475d9174437)`(G & graph,const std::string & name) const` 

#### `public void `[`make_all_graphs`](#de/da5/classalps_1_1_lattice_library_1a2c3134c3797f11a75056bdadafb5ad4d)`()` 

#### `protected LatticeMap `[`lattices_`](#de/da5/classalps_1_1_lattice_library_1ad3b7c8ac3aec732af52d742376796de4) 

#### `protected FiniteLatticeMap `[`finitelattices_`](#de/da5/classalps_1_1_lattice_library_1afe3192db11f5752c37d13c0740bf8644) 

#### `protected UnitCellMap `[`unitcells_`](#de/da5/classalps_1_1_lattice_library_1a0c949f387243e8739a06ae527153b0f9) 

#### `protected LatticeGraphMap `[`latticegraphs_`](#de/da5/classalps_1_1_lattice_library_1ab4a68507151310533b03bf152d24bbe4) 

#### `protected GraphMap `[`graphs_`](#de/da5/classalps_1_1_lattice_library_1a68b6cbbc1bfebc3f48bfba3584cd8c5c) 

#### `typedef `[`lattice_type`](#de/da5/classalps_1_1_lattice_library_1a73f3971127bd8c2bf73aa6218cb8b183) 

# class `alps::simple_cell` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`simple_cell`](#db/d9c/classalps_1_1simple__cell_1a0aba84ef1ef4a5a1d83d6738ee7ffe1a)`()` | 
`public inline  `[`simple_cell`](#db/d9c/classalps_1_1simple__cell_1a8d07049902f6e6951a87d4c0edc35b17)`(const unit_cell_type & u,const offset_type & o)` | 
`public inline const offset_type & `[`offset`](#db/d9c/classalps_1_1simple__cell_1a941f307a2a4917310da1274738c6cb3b)`() const` | 
`public inline dimension_type `[`dimension`](#db/d9c/classalps_1_1simple__cell_1a1789948e4b219a426d8ced6ac5ca6819)`()` | 
`typedef `[`offset_type`](#db/d9c/classalps_1_1simple__cell_1aa30e094d7899a7c2da0f41cd5dce1e41) | 
`typedef `[`unit_cell_type`](#db/d9c/classalps_1_1simple__cell_1ad6bd98426f91a4e9962f16d57a8d70b8) | 
`typedef `[`dimension_type`](#db/d9c/classalps_1_1simple__cell_1a7375721cf718799727723cf76e112323) | 

## Members

#### `public inline  `[`simple_cell`](#db/d9c/classalps_1_1simple__cell_1a0aba84ef1ef4a5a1d83d6738ee7ffe1a)`()` 

#### `public inline  `[`simple_cell`](#db/d9c/classalps_1_1simple__cell_1a8d07049902f6e6951a87d4c0edc35b17)`(const unit_cell_type & u,const offset_type & o)` 

#### `public inline const offset_type & `[`offset`](#db/d9c/classalps_1_1simple__cell_1a941f307a2a4917310da1274738c6cb3b)`() const` 

#### `public inline dimension_type `[`dimension`](#db/d9c/classalps_1_1simple__cell_1a1789948e4b219a426d8ced6ac5ca6819)`()` 

#### `typedef `[`offset_type`](#db/d9c/classalps_1_1simple__cell_1aa30e094d7899a7c2da0f41cd5dce1e41) 

#### `typedef `[`unit_cell_type`](#db/d9c/classalps_1_1simple__cell_1ad6bd98426f91a4e9962f16d57a8d70b8) 

#### `typedef `[`dimension_type`](#db/d9c/classalps_1_1simple__cell_1a7375721cf718799727723cf76e112323) 

# class `alps::simple_lattice` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice_1a369890b52032fe98f859bb8334b8ba83)`()` | 
`public template<>`  <br/>`inline  `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice_1a0eeb84e462771f1c043a4b579028eba4)`(const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< U2, C2 > & l)` | 
`public inline  `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice_1a919d9484e2f6eca508180389b1f5897a)`(const unit_cell_type & c)` | 
`public template<>`  <br/>`inline const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)` & `[`operator=`](#d2/d41/classalps_1_1simple__lattice_1a5ec4c0ec56b024147429b9deca4aba2e)`(const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< U2, C2 > & l)` | 
`public inline unit_cell_type & `[`unit_cell`](#d2/d41/classalps_1_1simple__lattice_1a3e4dbf276de021f0aca4efe9106d0d7c)`()` | 
`public inline const unit_cell_type & `[`unit_cell`](#d2/d41/classalps_1_1simple__lattice_1ab641d7225d9c4bfb32024bdac018c59b)`() const` | 
`public inline cell_descriptor `[`cell`](#d2/d41/classalps_1_1simple__lattice_1ad4a43e3705e641f05e2d52c999965c03)`(offset_type o) const` | 
`public inline dimension_type `[`dimension`](#d2/d41/classalps_1_1simple__lattice_1acb766a288058116f3ac10acad5c34ea7)`() const` | 
`protected unit_cell_type `[`unit_cell_`](#d2/d41/classalps_1_1simple__lattice_1ae5cad9f36ae8188b0d87b114b05ee858) | 
`typedef `[`unit_cell_type`](#d2/d41/classalps_1_1simple__lattice_1aaea267e5ebc5683eed5803d430466551) | 
`typedef `[`cell_descriptor`](#d2/d41/classalps_1_1simple__lattice_1a81d19dc111fb8c612c28dc2c729d18b8) | 
`typedef `[`dimension_type`](#d2/d41/classalps_1_1simple__lattice_1aacd11801f297dde42d782ca578b90dd0) | 
`typedef `[`offset_type`](#d2/d41/classalps_1_1simple__lattice_1acac761dd17863a9cb57c61064fd93028) | 

## Members

#### `public inline  `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice_1a369890b52032fe98f859bb8334b8ba83)`()` 

#### `public template<>`  <br/>`inline  `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice_1a0eeb84e462771f1c043a4b579028eba4)`(const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< U2, C2 > & l)` 

#### `public inline  `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice_1a919d9484e2f6eca508180389b1f5897a)`(const unit_cell_type & c)` 

#### `public template<>`  <br/>`inline const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)` & `[`operator=`](#d2/d41/classalps_1_1simple__lattice_1a5ec4c0ec56b024147429b9deca4aba2e)`(const `[`simple_lattice`](#d2/d41/classalps_1_1simple__lattice)`< U2, C2 > & l)` 

#### `public inline unit_cell_type & `[`unit_cell`](#d2/d41/classalps_1_1simple__lattice_1a3e4dbf276de021f0aca4efe9106d0d7c)`()` 

#### `public inline const unit_cell_type & `[`unit_cell`](#d2/d41/classalps_1_1simple__lattice_1ab641d7225d9c4bfb32024bdac018c59b)`() const` 

#### `public inline cell_descriptor `[`cell`](#d2/d41/classalps_1_1simple__lattice_1ad4a43e3705e641f05e2d52c999965c03)`(offset_type o) const` 

#### `public inline dimension_type `[`dimension`](#d2/d41/classalps_1_1simple__lattice_1acb766a288058116f3ac10acad5c34ea7)`() const` 

#### `protected unit_cell_type `[`unit_cell_`](#d2/d41/classalps_1_1simple__lattice_1ae5cad9f36ae8188b0d87b114b05ee858) 

#### `typedef `[`unit_cell_type`](#d2/d41/classalps_1_1simple__lattice_1aaea267e5ebc5683eed5803d430466551) 

#### `typedef `[`cell_descriptor`](#d2/d41/classalps_1_1simple__lattice_1a81d19dc111fb8c612c28dc2c729d18b8) 

#### `typedef `[`dimension_type`](#d2/d41/classalps_1_1simple__lattice_1aacd11801f297dde42d782ca578b90dd0) 

#### `typedef `[`offset_type`](#d2/d41/classalps_1_1simple__lattice_1acac761dd17863a9cb57c61064fd93028) 

# class `alps::singleton_property_map` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map_1a67af3b8bc490068fa5acd3fba5d036fb)`(V v)` | 
`public inline  `[`operator V`](#d7/da3/classalps_1_1singleton__property__map_1a8cc1795bf091cf100762fc204297e250)`() const` | 
`public inline V `[`value`](#d7/da3/classalps_1_1singleton__property__map_1ab61879247b0561eb75594fb1098773d7)`() const` | 
`public inline const `[`singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map)`< V, K > & `[`operator=`](#d7/da3/classalps_1_1singleton__property__map_1abb870d4a350f2065b10a92c8d9c00055)`(const V & v)` | 
`public template<>`  <br/>`inline V & `[`operator[]`](#d7/da3/classalps_1_1singleton__property__map_1a1599393a33becb09b07774fa2cb01ebc)`(T)` | 
`public template<>`  <br/>`inline const V & `[`operator[]`](#d7/da3/classalps_1_1singleton__property__map_1a4d58f83eaff1a206f3c0980e292708f4)`(T) const` | 
`typedef `[`key_type`](#d7/da3/classalps_1_1singleton__property__map_1a9a73b50c6576a462ff937e52a935559d) | 
`typedef `[`value_type`](#d7/da3/classalps_1_1singleton__property__map_1a4be0f37899ecb35a767547956f51bb3c) | 
`typedef `[`reference`](#d7/da3/classalps_1_1singleton__property__map_1a221ef0c678bfe1d3bca916abd9c75760) | 
`typedef `[`category`](#d7/da3/classalps_1_1singleton__property__map_1a534786c483c30f2d3a9c7f0a5a3138d1) | 

## Members

#### `public inline  `[`singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map_1a67af3b8bc490068fa5acd3fba5d036fb)`(V v)` 

#### `public inline  `[`operator V`](#d7/da3/classalps_1_1singleton__property__map_1a8cc1795bf091cf100762fc204297e250)`() const` 

#### `public inline V `[`value`](#d7/da3/classalps_1_1singleton__property__map_1ab61879247b0561eb75594fb1098773d7)`() const` 

#### `public inline const `[`singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map)`< V, K > & `[`operator=`](#d7/da3/classalps_1_1singleton__property__map_1abb870d4a350f2065b10a92c8d9c00055)`(const V & v)` 

#### `public template<>`  <br/>`inline V & `[`operator[]`](#d7/da3/classalps_1_1singleton__property__map_1a1599393a33becb09b07774fa2cb01ebc)`(T)` 

#### `public template<>`  <br/>`inline const V & `[`operator[]`](#d7/da3/classalps_1_1singleton__property__map_1a4d58f83eaff1a206f3c0980e292708f4)`(T) const` 

#### `typedef `[`key_type`](#d7/da3/classalps_1_1singleton__property__map_1a9a73b50c6576a462ff937e52a935559d) 

#### `typedef `[`value_type`](#d7/da3/classalps_1_1singleton__property__map_1a4be0f37899ecb35a767547956f51bb3c) 

#### `typedef `[`reference`](#d7/da3/classalps_1_1singleton__property__map_1a221ef0c678bfe1d3bca916abd9c75760) 

#### `typedef `[`category`](#d7/da3/classalps_1_1singleton__property__map_1a534786c483c30f2d3a9c7f0a5a3138d1) 

# struct `alps::bond_descriptor_compare` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public graph_type const  * `[`Graph`](#d3/dc3/structalps_1_1bond__descriptor__compare_1af557c3c330df57735deaba7ea292fbd1) | 
`public inline  `[`bond_descriptor_compare`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a42ac6b21c73898467619c1bf4d512745)`(G const * Gr)` | 
`public inline bool `[`operator()`](#d3/dc3/structalps_1_1bond__descriptor__compare_1ae5e0dc77565a3420870903b42e1ae44b)`(bond_descriptor b1,bond_descriptor b2) const` | 
`typedef `[`graph_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1aab2257f9291c7e65e8e3fc9939810ecb) | 
`typedef `[`traits_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a84aff12cca04712563cf18f0afd18f1b) | 
`typedef `[`bond_descriptor`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a6c4e10ca09a9c8af2db40a6938f9c29f) | 
`typedef `[`site_descriptor`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a1fe0bc8347875b082409ebe725790ccd) | 
`typedef `[`result_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a143f7832817946556e4145515c4627e1) | 
`typedef `[`first_argument_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a204e0321c6e6c3c303fa8b3327349d6c) | 
`typedef `[`second_argument_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a07975d987d8bcca51ad0a70c58691820) | 

## Members

#### `public graph_type const  * `[`Graph`](#d3/dc3/structalps_1_1bond__descriptor__compare_1af557c3c330df57735deaba7ea292fbd1) 

#### `public inline  `[`bond_descriptor_compare`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a42ac6b21c73898467619c1bf4d512745)`(G const * Gr)` 

#### `public inline bool `[`operator()`](#d3/dc3/structalps_1_1bond__descriptor__compare_1ae5e0dc77565a3420870903b42e1ae44b)`(bond_descriptor b1,bond_descriptor b2) const` 

#### `typedef `[`graph_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1aab2257f9291c7e65e8e3fc9939810ecb) 

#### `typedef `[`traits_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a84aff12cca04712563cf18f0afd18f1b) 

#### `typedef `[`bond_descriptor`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a6c4e10ca09a9c8af2db40a6938f9c29f) 

#### `typedef `[`site_descriptor`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a1fe0bc8347875b082409ebe725790ccd) 

#### `typedef `[`result_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a143f7832817946556e4145515c4627e1) 

#### `typedef `[`first_argument_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a204e0321c6e6c3c303fa8b3327349d6c) 

#### `typedef `[`second_argument_type`](#d3/dc3/structalps_1_1bond__descriptor__compare_1a07975d987d8bcca51ad0a70c58691820) 

# struct `alps::bond_descriptor_compare_undirected` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public graph_type const  * `[`Graph`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1af25883404bfc2cfdb7826fb93f13ff8f) | 
`public inline  `[`bond_descriptor_compare_undirected`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a2516392dad442200847d55b0b3d3397c)`(G const * Gr)` | 
`public inline bool `[`operator()`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a6416ba8b5fe404caabf3a4cb7cb1631c)`(bond_descriptor b1,bond_descriptor b2) const` | 
`typedef `[`graph_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a2ddbf5731fa1f31756b7f8caf08e7fa2) | 
`typedef `[`traits_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a016025ce36ad90fe3c7b6e632f95cd47) | 
`typedef `[`bond_descriptor`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a8ce576bb071d707844006681bd9d6d61) | 
`typedef `[`site_descriptor`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1ad30f16a6738ef97ff2d8be1f2d534342) | 
`typedef `[`result_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1ac6193409723894e3262ec15e85a4880b) | 
`typedef `[`first_argument_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a4ed7b79327a20f5d773cf5a86d364c89) | 
`typedef `[`second_argument_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1ab0c63ec30e65820b68e2aa9454820768) | 

## Members

#### `public graph_type const  * `[`Graph`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1af25883404bfc2cfdb7826fb93f13ff8f) 

#### `public inline  `[`bond_descriptor_compare_undirected`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a2516392dad442200847d55b0b3d3397c)`(G const * Gr)` 

#### `public inline bool `[`operator()`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a6416ba8b5fe404caabf3a4cb7cb1631c)`(bond_descriptor b1,bond_descriptor b2) const` 

#### `typedef `[`graph_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a2ddbf5731fa1f31756b7f8caf08e7fa2) 

#### `typedef `[`traits_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a016025ce36ad90fe3c7b6e632f95cd47) 

#### `typedef `[`bond_descriptor`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a8ce576bb071d707844006681bd9d6d61) 

#### `typedef `[`site_descriptor`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1ad30f16a6738ef97ff2d8be1f2d534342) 

#### `typedef `[`result_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1ac6193409723894e3262ec15e85a4880b) 

#### `typedef `[`first_argument_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1a4ed7b79327a20f5d773cf5a86d364c89) 

#### `typedef `[`second_argument_type`](#dd/d2d/structalps_1_1bond__descriptor__compare__undirected_1ab0c63ec30e65820b68e2aa9454820768) 

# struct `alps::boundary_crossing` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`boundary_crossing`](#de/df2/structalps_1_1boundary__crossing_1a8352933b6cfa514e41d92d3cf75a85c2)`()` | 
`public inline  `[`operator bool`](#de/df2/structalps_1_1boundary__crossing_1a62b1b327cb98ade7ddf018e8b3dea6e9)`() const` | 
`public inline direction_type `[`crosses`](#de/df2/structalps_1_1boundary__crossing_1af824fbd7f4298323d0d835cebf3f5055)`(dimension_type d) const` | 
`public inline const `[`boundary_crossing`](#de/df2/structalps_1_1boundary__crossing)` & `[`set_crossing`](#de/df2/structalps_1_1boundary__crossing_1a90f84ba96495d6bce3335dd1900394f5)`(dimension_type d,direction_type dir)` | 
`public inline const `[`boundary_crossing`](#de/df2/structalps_1_1boundary__crossing)` & `[`invert`](#de/df2/structalps_1_1boundary__crossing_1ab6bbf8f5e842a0aa9c331306c82eaab5)`()` | 
`public inline void `[`save`](#de/df2/structalps_1_1boundary__crossing_1a3e5a31dd1543d9dd3b246d59404d9fc6)`(ODump & dump) const` | 
`public inline void `[`load`](#de/df2/structalps_1_1boundary__crossing_1a61b0a8944201b1f79d1f14f5be0db787)`(IDump & dump)` | 
`public template<>`  <br/>`inline void `[`serialize`](#de/df2/structalps_1_1boundary__crossing_1ab26e805608152b68533c02a93efa1d52)`(Archive & ar,const unsigned int version)` | 
`typedef `[`dimension_type`](#de/df2/structalps_1_1boundary__crossing_1a2e8f370839f4463748e35d503b42ed58) | 
`typedef `[`direction_type`](#de/df2/structalps_1_1boundary__crossing_1a45e3cf98863ba4c89b1d3bc99da4d7df) | 

## Members

#### `public inline  `[`boundary_crossing`](#de/df2/structalps_1_1boundary__crossing_1a8352933b6cfa514e41d92d3cf75a85c2)`()` 

#### `public inline  `[`operator bool`](#de/df2/structalps_1_1boundary__crossing_1a62b1b327cb98ade7ddf018e8b3dea6e9)`() const` 

#### `public inline direction_type `[`crosses`](#de/df2/structalps_1_1boundary__crossing_1af824fbd7f4298323d0d835cebf3f5055)`(dimension_type d) const` 

#### `public inline const `[`boundary_crossing`](#de/df2/structalps_1_1boundary__crossing)` & `[`set_crossing`](#de/df2/structalps_1_1boundary__crossing_1a90f84ba96495d6bce3335dd1900394f5)`(dimension_type d,direction_type dir)` 

#### `public inline const `[`boundary_crossing`](#de/df2/structalps_1_1boundary__crossing)` & `[`invert`](#de/df2/structalps_1_1boundary__crossing_1ab6bbf8f5e842a0aa9c331306c82eaab5)`()` 

#### `public inline void `[`save`](#de/df2/structalps_1_1boundary__crossing_1a3e5a31dd1543d9dd3b246d59404d9fc6)`(ODump & dump) const` 

#### `public inline void `[`load`](#de/df2/structalps_1_1boundary__crossing_1a61b0a8944201b1f79d1f14f5be0db787)`(IDump & dump)` 

#### `public template<>`  <br/>`inline void `[`serialize`](#de/df2/structalps_1_1boundary__crossing_1ab26e805608152b68533c02a93efa1d52)`(Archive & ar,const unsigned int version)` 

#### `typedef `[`dimension_type`](#de/df2/structalps_1_1boundary__crossing_1a2e8f370839f4463748e35d503b42ed58) 

#### `typedef `[`direction_type`](#de/df2/structalps_1_1boundary__crossing_1a45e3cf98863ba4c89b1d3bc99da4d7df) 

# struct `alps::boundary_crossing_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d4/ddb/structalps_1_1boundary__crossing__t_1af1b98c3440833682125fe5d472d10349) | 

## Members

#### `typedef `[`kind`](#d4/ddb/structalps_1_1boundary__crossing__t_1af1b98c3440833682125fe5d472d10349) 

# struct `alps::cell_traits` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`offset_type`](#dc/deb/structalps_1_1cell__traits_1a81dbe6526d9f5e635e1dfcc05c0a7b56) | 

## Members

#### `typedef `[`offset_type`](#dc/deb/structalps_1_1cell__traits_1a81dbe6526d9f5e635e1dfcc05c0a7b56) 

# struct `alps::coordinate_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d3/d05/structalps_1_1coordinate__t_1ab0addc109c97b9d306871e63dcb304f7) | 

## Members

#### `typedef `[`kind`](#d3/d05/structalps_1_1coordinate__t_1ab0addc109c97b9d306871e63dcb304f7) 

# struct `alps::coordinate_traits` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`value_type`](#da/d24/structalps_1_1coordinate__traits_1ac87d8e0536a71e4872deb195614aa4a0) | 
`typedef `[`iterator`](#da/d24/structalps_1_1coordinate__traits_1aa961bb554e719aaa2061c404db12656b) | 
`typedef `[`const_iterator`](#da/d24/structalps_1_1coordinate__traits_1a7f967a2d7ba10e98f459b8fbec05e276) | 

## Members

#### `typedef `[`value_type`](#da/d24/structalps_1_1coordinate__traits_1ac87d8e0536a71e4872deb195614aa4a0) 

#### `typedef `[`iterator`](#da/d24/structalps_1_1coordinate__traits_1aa961bb554e719aaa2061c404db12656b) 

#### `typedef `[`const_iterator`](#da/d24/structalps_1_1coordinate__traits_1a7f967a2d7ba10e98f459b8fbec05e276) 

# struct `alps::coordinate_traits< const C >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`value_type`](#d0/d1f/structalps_1_1coordinate__traits_3_01const_01_c_01_4_1a85f944a36adfabfe1651396fc675ec5e) | 
`typedef `[`iterator`](#d0/d1f/structalps_1_1coordinate__traits_3_01const_01_c_01_4_1aaa85fde99e08a0fe121b7d872dd41355) | 
`typedef `[`const_iterator`](#d0/d1f/structalps_1_1coordinate__traits_3_01const_01_c_01_4_1a34272da8c9eb60b60c451b4a539b179a) | 

## Members

#### `typedef `[`value_type`](#d0/d1f/structalps_1_1coordinate__traits_3_01const_01_c_01_4_1a85f944a36adfabfe1651396fc675ec5e) 

#### `typedef `[`iterator`](#d0/d1f/structalps_1_1coordinate__traits_3_01const_01_c_01_4_1aaa85fde99e08a0fe121b7d872dd41355) 

#### `typedef `[`const_iterator`](#d0/d1f/structalps_1_1coordinate__traits_3_01const_01_c_01_4_1a34272da8c9eb60b60c451b4a539b179a) 

# struct `alps::coordinate_traits< std::valarray< T > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`value_type`](#d4/dd6/structalps_1_1coordinate__traits_3_01std_1_1valarray_3_01_t_01_4_01_4_1a6932bd6c963ebdb7227cdb967a58c009) | 
`typedef `[`iterator`](#d4/dd6/structalps_1_1coordinate__traits_3_01std_1_1valarray_3_01_t_01_4_01_4_1a4c368c49d004862f15d5200705c47788) | 
`typedef `[`const_iterator`](#d4/dd6/structalps_1_1coordinate__traits_3_01std_1_1valarray_3_01_t_01_4_01_4_1af5a9699fb0cd4e5dea63a8506698f6c9) | 

## Members

#### `typedef `[`value_type`](#d4/dd6/structalps_1_1coordinate__traits_3_01std_1_1valarray_3_01_t_01_4_01_4_1a6932bd6c963ebdb7227cdb967a58c009) 

#### `typedef `[`iterator`](#d4/dd6/structalps_1_1coordinate__traits_3_01std_1_1valarray_3_01_t_01_4_01_4_1a4c368c49d004862f15d5200705c47788) 

#### `typedef `[`const_iterator`](#d4/dd6/structalps_1_1coordinate__traits_3_01std_1_1valarray_3_01_t_01_4_01_4_1af5a9699fb0cd4e5dea63a8506698f6c9) 

# struct `alps::coordinate_traits< T[sz]>` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`value_type`](#d9/d2a/structalps_1_1coordinate__traits_3_01_t_0fsz_0e_4_1ac2d116c3610cbc3a283e978a473bea7d) | 
`typedef `[`iterator`](#d9/d2a/structalps_1_1coordinate__traits_3_01_t_0fsz_0e_4_1a25df56c175cc62535304b90a65bf316e) | 
`typedef `[`const_iterator`](#d9/d2a/structalps_1_1coordinate__traits_3_01_t_0fsz_0e_4_1a4c44fb0728c7b192e05ad85ca61494a1) | 

## Members

#### `typedef `[`value_type`](#d9/d2a/structalps_1_1coordinate__traits_3_01_t_0fsz_0e_4_1ac2d116c3610cbc3a283e978a473bea7d) 

#### `typedef `[`iterator`](#d9/d2a/structalps_1_1coordinate__traits_3_01_t_0fsz_0e_4_1a25df56c175cc62535304b90a65bf316e) 

#### `typedef `[`const_iterator`](#d9/d2a/structalps_1_1coordinate__traits_3_01_t_0fsz_0e_4_1a4c44fb0728c7b192e05ad85ca61494a1) 

# struct `alps::copy_property_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::copy_property_helper< SRC, DST, PROPERTY, true >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::dimension_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d1/d9f/structalps_1_1dimension__t_1a7aae5598911f3f2edfb6c96610295cf0) | 

## Members

#### `typedef `[`kind`](#d1/d9f/structalps_1_1dimension__t_1a7aae5598911f3f2edfb6c96610295cf0) 

# struct `alps::dimensional_traits` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d8/d28/structalps_1_1dimensional__traits_1ab1d9611f31897d048cee007faa4f347e)`(bool,fixed_dimension)` | 
`typedef `[`dimension_type`](#d8/d28/structalps_1_1dimensional__traits_1a37ad9ff3071ebbcbc40c7743b44c1244) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d8/d28/structalps_1_1dimensional__traits_1ab1d9611f31897d048cee007faa4f347e)`(bool,fixed_dimension)` 

#### `typedef `[`dimension_type`](#d8/d28/structalps_1_1dimensional__traits_1a37ad9ff3071ebbcbc40c7743b44c1244) 

# struct `alps::edge_type_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d6/dda/structalps_1_1edge__type__t_1a6731b1ea13d655d751eb989a649e2f63) | 

## Members

#### `typedef `[`kind`](#d6/dda/structalps_1_1edge__type__t_1a6731b1ea13d655d751eb989a649e2f63) 

# struct `alps::edge_vector_relative_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d4/dff/structalps_1_1edge__vector__relative__t_1adbddac92c741414aec3c755d14528095) | 

## Members

#### `typedef `[`kind`](#d4/dff/structalps_1_1edge__vector__relative__t_1adbddac92c741414aec3c755d14528095) 

# struct `alps::edge_vector_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#de/dd9/structalps_1_1edge__vector__t_1a47767fea07a4d726085256f55571325d) | 

## Members

#### `typedef `[`kind`](#de/dd9/structalps_1_1edge__vector__t_1a47767fea07a4d726085256f55571325d) 

# struct `alps::graph_name_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d4/d34/structalps_1_1graph__name__t_1a936612ce2e4471658df6d9ddf95e3f1a) | 

## Members

#### `typedef `[`kind`](#d4/d34/structalps_1_1graph__name__t_1a936612ce2e4471658df6d9ddf95e3f1a) 

# struct `alps::graph_traits` 

```
struct alps::graph_traits
  : public boost::graph_traits< G >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`graph_type`](#d5/d1a/structalps_1_1graph__traits_1aab978a496c56c50c9d2f9aac9d2bbd32) | 
`typedef `[`site_iterator`](#d5/d1a/structalps_1_1graph__traits_1ab2e2f050cd655d3ae2f6f5d437b9da26) | 
`typedef `[`bond_iterator`](#d5/d1a/structalps_1_1graph__traits_1a4b989e06868f5c717d7109c957bc5821) | 
`typedef `[`neighbor_bond_iterator`](#d5/d1a/structalps_1_1graph__traits_1a500b46fb45dd544480ee0af44795c9be) | 
`typedef `[`site_descriptor`](#d5/d1a/structalps_1_1graph__traits_1a45d906e257c7306cc17a064bd2b6c145) | 
`typedef `[`bond_descriptor`](#d5/d1a/structalps_1_1graph__traits_1a4cd4f43f4109409254f70cb11888db6a) | 
`typedef `[`sites_size_type`](#d5/d1a/structalps_1_1graph__traits_1af2b7ec669347d09ac04714ee7510cc22) | 
`typedef `[`bonds_size_type`](#d5/d1a/structalps_1_1graph__traits_1ac3c40a9ab6dd9a6b996e270df9f27407) | 
`typedef `[`neighbors_size_type`](#d5/d1a/structalps_1_1graph__traits_1ac4f656220de4251a92214ad80cba77e1) | 
`typedef `[`neighbor_iterator`](#d5/d1a/structalps_1_1graph__traits_1aadc568ac5f73b26fac18feaf4907d55f) | 

## Members

#### `typedef `[`graph_type`](#d5/d1a/structalps_1_1graph__traits_1aab978a496c56c50c9d2f9aac9d2bbd32) 

#### `typedef `[`site_iterator`](#d5/d1a/structalps_1_1graph__traits_1ab2e2f050cd655d3ae2f6f5d437b9da26) 

#### `typedef `[`bond_iterator`](#d5/d1a/structalps_1_1graph__traits_1a4b989e06868f5c717d7109c957bc5821) 

#### `typedef `[`neighbor_bond_iterator`](#d5/d1a/structalps_1_1graph__traits_1a500b46fb45dd544480ee0af44795c9be) 

#### `typedef `[`site_descriptor`](#d5/d1a/structalps_1_1graph__traits_1a45d906e257c7306cc17a064bd2b6c145) 

#### `typedef `[`bond_descriptor`](#d5/d1a/structalps_1_1graph__traits_1a4cd4f43f4109409254f70cb11888db6a) 

#### `typedef `[`sites_size_type`](#d5/d1a/structalps_1_1graph__traits_1af2b7ec669347d09ac04714ee7510cc22) 

#### `typedef `[`bonds_size_type`](#d5/d1a/structalps_1_1graph__traits_1ac3c40a9ab6dd9a6b996e270df9f27407) 

#### `typedef `[`neighbors_size_type`](#d5/d1a/structalps_1_1graph__traits_1ac4f656220de4251a92214ad80cba77e1) 

#### `typedef `[`neighbor_iterator`](#d5/d1a/structalps_1_1graph__traits_1aadc568ac5f73b26fac18feaf4907d55f) 

# struct `alps::graph_traits< lattice_graph< L, G > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`graph_type`](#de/d51/structalps_1_1graph__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1a4e0c19b45bbab0d09d946e9b1fe6a913) | 

## Members

#### `typedef `[`graph_type`](#de/d51/structalps_1_1graph__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1a4e0c19b45bbab0d09d946e9b1fe6a913) 

# struct `alps::has_property` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1aea7d91cf5d9e0e30896609c7068c2003)`(bool,vertex_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1a24b5fccbab0c348a88eeab7b86fd3501)`(bool,edge_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1a475c742e6c3bfcf3da66658c43fa55b7)`(bool,graph_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1a5e1974ed447291e704bb86fcdd2e5b3e)`(bool,any_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1a3959b2caaccc04ecadbba9f65fa53af8)`(bool,site_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1ad33dedd9acc77b1af6f52b662625541b)`(bool,bond_property)` | 
`typedef `[`vertex_property_type`](#d4/dcf/structalps_1_1has__property_1a645917d9de6e11e0ee71f4f66b1c9539) | 
`typedef `[`edge_property_type`](#d4/dcf/structalps_1_1has__property_1a8a21d67b7299f36eab0981df756b8074) | 
`typedef `[`graph_property_type`](#d4/dcf/structalps_1_1has__property_1a3d51c46276509b4cfbe18d579979eccc) | 
`typedef `[`property_type`](#d4/dcf/structalps_1_1has__property_1a4c98ea12f8e7cfc390ae977593aaf51e) | 
`typedef `[`type`](#d4/dcf/structalps_1_1has__property_1a94315e0f7dea97212a365be0a8c0a32f) | 
`typedef `[`site_property_type`](#d4/dcf/structalps_1_1has__property_1a000ea0ff222fe59471f857dedb0b86ca) | 
`typedef `[`bond_property_type`](#d4/dcf/structalps_1_1has__property_1af86f74b1cad766c6720d29bcd7aed604) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1aea7d91cf5d9e0e30896609c7068c2003)`(bool,vertex_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1a24b5fccbab0c348a88eeab7b86fd3501)`(bool,edge_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1a475c742e6c3bfcf3da66658c43fa55b7)`(bool,graph_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1a5e1974ed447291e704bb86fcdd2e5b3e)`(bool,any_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1a3959b2caaccc04ecadbba9f65fa53af8)`(bool,site_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/dcf/structalps_1_1has__property_1ad33dedd9acc77b1af6f52b662625541b)`(bool,bond_property)` 

#### `typedef `[`vertex_property_type`](#d4/dcf/structalps_1_1has__property_1a645917d9de6e11e0ee71f4f66b1c9539) 

#### `typedef `[`edge_property_type`](#d4/dcf/structalps_1_1has__property_1a8a21d67b7299f36eab0981df756b8074) 

#### `typedef `[`graph_property_type`](#d4/dcf/structalps_1_1has__property_1a3d51c46276509b4cfbe18d579979eccc) 

#### `typedef `[`property_type`](#d4/dcf/structalps_1_1has__property_1a4c98ea12f8e7cfc390ae977593aaf51e) 

#### `typedef `[`type`](#d4/dcf/structalps_1_1has__property_1a94315e0f7dea97212a365be0a8c0a32f) 

#### `typedef `[`site_property_type`](#d4/dcf/structalps_1_1has__property_1a000ea0ff222fe59471f857dedb0b86ca) 

#### `typedef `[`bond_property_type`](#d4/dcf/structalps_1_1has__property_1af86f74b1cad766c6720d29bcd7aed604) 

# struct `alps::has_property< P, boost::adjacency_list< s1, s2, s3, VP, EP, GP, s4 >, D >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a91320d3e712e4462cdbc8511f77cbf55)`(bool,vertex_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a762eab24f15cfa0c8740e68e925dabe2)`(bool,edge_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1af2d47a35f63adac77a76d263c87206eb)`(bool,graph_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1ac0ae446e0c58bed7280151385d9c22cc)`(bool,any_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a9add1cd02a913a649d51844d9c982077)`(bool,site_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a12b14a42886953fb4c3d138f23797a90)`(bool,bond_property)` | 
`typedef `[`Graph`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1ac2edc8ef7cbd897d28ad705881b38b2d) | 
`typedef `[`vertex_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a06ab870b1833acb576777ce8e5806d11) | 
`typedef `[`edge_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a7ac911c1e2b39ae653cb39d9cf66c020) | 
`typedef `[`graph_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a886485568370860f66ba90ad6b4532d4) | 
`typedef `[`property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a23ec5b66b63117bd35e16b340b5c72b3) | 
`typedef `[`type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a8c85ccdaa8b486509ae15e7f12a9f504) | 
`typedef `[`site_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a0c1644b3ace339036a910cadd9bc0543) | 
`typedef `[`bond_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a2f0da2493691d80f3224805c1d8e9085) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a91320d3e712e4462cdbc8511f77cbf55)`(bool,vertex_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a762eab24f15cfa0c8740e68e925dabe2)`(bool,edge_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1af2d47a35f63adac77a76d263c87206eb)`(bool,graph_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1ac0ae446e0c58bed7280151385d9c22cc)`(bool,any_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a9add1cd02a913a649d51844d9c982077)`(bool,site_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a12b14a42886953fb4c3d138f23797a90)`(bool,bond_property)` 

#### `typedef `[`Graph`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1ac2edc8ef7cbd897d28ad705881b38b2d) 

#### `typedef `[`vertex_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a06ab870b1833acb576777ce8e5806d11) 

#### `typedef `[`edge_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a7ac911c1e2b39ae653cb39d9cf66c020) 

#### `typedef `[`graph_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a886485568370860f66ba90ad6b4532d4) 

#### `typedef `[`property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a23ec5b66b63117bd35e16b340b5c72b3) 

#### `typedef `[`type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a8c85ccdaa8b486509ae15e7f12a9f504) 

#### `typedef `[`site_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a0c1644b3ace339036a910cadd9bc0543) 

#### `typedef `[`bond_property_type`](#d8/dc5/structalps_1_1has__property_3_01_p_00_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_00_01_v_6c9a6a362bb177f99080292335109d59_1a2f0da2493691d80f3224805c1d8e9085) 

# struct `alps::has_property< P, const boost::adjacency_list< s1, s2, s3, VP, EP, GP, s4 >, D >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1ab4c99435468eae055007d67c34daa65a)`(bool,vertex_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1aed3a8d446953966c2fe504705f4f7a11)`(bool,edge_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1ad6eb2e26878336037de5468d423fa844)`(bool,graph_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1af009f8004070ea2703eff50259c49075)`(bool,any_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a93edc421aac3104838435e11ea8364d4)`(bool,site_property)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a39a0061453cd25373eb91383a4075d6d)`(bool,bond_property)` | 
`typedef `[`Graph`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a0e033f078c01f342153e9f795f1b43fe) | 
`typedef `[`vertex_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a9fccfbadf63bf57338dd0e5bae9dd62d) | 
`typedef `[`edge_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a562ebe134290b3dfb01313a43c895c84) | 
`typedef `[`graph_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a0c4854c8f07b8b5afe384a8e416cc4eb) | 
`typedef `[`property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a5202f677d304799259266b63b33e10c3) | 
`typedef `[`type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1ab96f2af4ef3a51ec6ec6fe4d096d879f) | 
`typedef `[`site_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1ab2fecd7a810ddc66667ec16a8b1996a4) | 
`typedef `[`bond_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a60c52b9be4db45bcf74e05ed838969db) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1ab4c99435468eae055007d67c34daa65a)`(bool,vertex_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1aed3a8d446953966c2fe504705f4f7a11)`(bool,edge_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1ad6eb2e26878336037de5468d423fa844)`(bool,graph_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1af009f8004070ea2703eff50259c49075)`(bool,any_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a93edc421aac3104838435e11ea8364d4)`(bool,site_property)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a39a0061453cd25373eb91383a4075d6d)`(bool,bond_property)` 

#### `typedef `[`Graph`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a0e033f078c01f342153e9f795f1b43fe) 

#### `typedef `[`vertex_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a9fccfbadf63bf57338dd0e5bae9dd62d) 

#### `typedef `[`edge_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a562ebe134290b3dfb01313a43c895c84) 

#### `typedef `[`graph_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a0c4854c8f07b8b5afe384a8e416cc4eb) 

#### `typedef `[`property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a5202f677d304799259266b63b33e10c3) 

#### `typedef `[`type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1ab96f2af4ef3a51ec6ec6fe4d096d879f) 

#### `typedef `[`site_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1ab2fecd7a810ddc66667ec16a8b1996a4) 

#### `typedef `[`bond_property_type`](#d4/d70/structalps_1_1has__property_3_01_p_00_01const_01boost_1_1adjacency__list_3_01s1_00_01s2_00_01s3_7740bc30619a05788839d7f1041a7f13_1a60c52b9be4db45bcf74e05ed838969db) 

# struct `alps::lattice_traits` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::lattice_traits< coordinate_lattice< B, V > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`unit_cell_type`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1afa6d877bf3bca7f87d6a0a34922cb418) | 
`typedef `[`cell_descriptor`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1adc7effef67b9acfed62f55375e40f6db) | 
`typedef `[`offset_type`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1ae8cb80d933a16d356c51855c779c32c6) | 
`typedef `[`vector_type`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1a55ff24eb6bebba9099cfc9d2ca1b6f75) | 
`typedef `[`basis_vector_iterator`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1afaff3a9455f5883c2a79c2460f1ca56b) | 

## Members

#### `typedef `[`unit_cell_type`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1afa6d877bf3bca7f87d6a0a34922cb418) 

#### `typedef `[`cell_descriptor`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1adc7effef67b9acfed62f55375e40f6db) 

#### `typedef `[`offset_type`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1ae8cb80d933a16d356c51855c779c32c6) 

#### `typedef `[`vector_type`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1a55ff24eb6bebba9099cfc9d2ca1b6f75) 

#### `typedef `[`basis_vector_iterator`](#d0/de1/structalps_1_1lattice__traits_3_01coordinate__lattice_3_01_b_00_01_v_01_4_01_4_1afaff3a9455f5883c2a79c2460f1ca56b) 

# struct `alps::lattice_traits< hypercubic_lattice< BASE, EX > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`unit_cell_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1ab9c33bd61bc27a92359f511657145f2d) | 
`typedef `[`cell_descriptor`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1aa31f44c41fd5e3a0a3dd7bc9436f67b6) | 
`typedef `[`offset_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a1f36f2ec304dcbe564d4af86955613cb) | 
`typedef `[`extent_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a00c48795f62051fc87152b58e22be093) | 
`typedef `[`basis_vector_iterator`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1aab68c7ad345cf5a8835cba362b5160ce) | 
`typedef `[`momentum_iterator`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a87ee9cefbcfa98b09dc204b88e7d1032) | 
`typedef `[`cell_iterator`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a7b78e69bd0ef989f2314641be9d1d472) | 
`typedef `[`size_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a52108f17d738eaed53e9c47681be6a4b) | 
`typedef `[`vector_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1ae07427bc5a8e6677a73bc07e218f150c) | 
`typedef `[`boundary_crossing_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1af6b204e0b435db4d33fba3e66f2ca11b) | 

## Members

#### `typedef `[`unit_cell_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1ab9c33bd61bc27a92359f511657145f2d) 

#### `typedef `[`cell_descriptor`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1aa31f44c41fd5e3a0a3dd7bc9436f67b6) 

#### `typedef `[`offset_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a1f36f2ec304dcbe564d4af86955613cb) 

#### `typedef `[`extent_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a00c48795f62051fc87152b58e22be093) 

#### `typedef `[`basis_vector_iterator`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1aab68c7ad345cf5a8835cba362b5160ce) 

#### `typedef `[`momentum_iterator`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a87ee9cefbcfa98b09dc204b88e7d1032) 

#### `typedef `[`cell_iterator`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a7b78e69bd0ef989f2314641be9d1d472) 

#### `typedef `[`size_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1a52108f17d738eaed53e9c47681be6a4b) 

#### `typedef `[`vector_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1ae07427bc5a8e6677a73bc07e218f150c) 

#### `typedef `[`boundary_crossing_type`](#d6/d1b/structalps_1_1lattice__traits_3_01hypercubic__lattice_3_01_b_a_s_e_00_01_e_x_01_4_01_4_1af6b204e0b435db4d33fba3e66f2ca11b) 

# struct `alps::lattice_traits< lattice_graph< L, G > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`unit_cell_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1ab324df234da9202dd98179c8efd73c9d) | 
`typedef `[`cell_descriptor`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1a7e3d0c06712cb2eabf68e9a1e6bdf7d1) | 
`typedef `[`offset_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1ab3edeb39e8ce610207d74e1732841424) | 
`typedef `[`extent_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1afd8039bbc3e4d3e6b388e16d8b7cdf5a) | 
`typedef `[`basis_vector_iterator`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1af3f716f3ff86aa5f585ea766fe5d8ea7) | 
`typedef `[`cell_iterator`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1a06a29f4b11e409fa67680cb53532d8de) | 
`typedef `[`momentum_iterator`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1a29f4dae299cb4a499147cded1398af75) | 
`typedef `[`size_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1ad654c21ce3350ced6c9b9944cc40328b) | 
`typedef `[`vector_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1ab861235b91af2e05ddddc73c0665462c) | 
`typedef `[`boundary_crossing_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1aea1cd252598501e18c28c9d9a03d76bb) | 

## Members

#### `typedef `[`unit_cell_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1ab324df234da9202dd98179c8efd73c9d) 

#### `typedef `[`cell_descriptor`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1a7e3d0c06712cb2eabf68e9a1e6bdf7d1) 

#### `typedef `[`offset_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1ab3edeb39e8ce610207d74e1732841424) 

#### `typedef `[`extent_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1afd8039bbc3e4d3e6b388e16d8b7cdf5a) 

#### `typedef `[`basis_vector_iterator`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1af3f716f3ff86aa5f585ea766fe5d8ea7) 

#### `typedef `[`cell_iterator`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1a06a29f4b11e409fa67680cb53532d8de) 

#### `typedef `[`momentum_iterator`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1a29f4dae299cb4a499147cded1398af75) 

#### `typedef `[`size_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1ad654c21ce3350ced6c9b9944cc40328b) 

#### `typedef `[`vector_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1ab861235b91af2e05ddddc73c0665462c) 

#### `typedef `[`boundary_crossing_type`](#d0/d68/structalps_1_1lattice__traits_3_01lattice__graph_3_01_l_00_01_g_01_4_01_4_1aea1cd252598501e18c28c9d9a03d76bb) 

# struct `alps::lattice_traits< LatticeGraphDescriptor >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`unit_cell_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a5793de76f74f3473cdadfbe3b4d25cb9) | 
`typedef `[`cell_descriptor`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a81baee6707b76e8e6d8cc1148f8785fe) | 
`typedef `[`offset_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a865536de4145b43b1c7d1f018beaddfe) | 
`typedef `[`extent_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a8158448800d261599cb5c3b32353026a) | 
`typedef `[`basis_vector_iterator`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a6b705ace73c3dd6349809d41048ed01e) | 
`typedef `[`cell_iterator`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1ada706e4d26209a7018e70a44fde624d6) | 
`typedef `[`momentum_iterator`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1af122429b298c9d4c88bb85a2e7bcd281) | 
`typedef `[`size_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1ad37b84ee0f97ec6b34e61643b97b960d) | 
`typedef `[`vector_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a041dee9c60dc7d71439b35e002f80fc3) | 
`typedef `[`boundary_crossing_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a7eba4bda6e762c1d549053349c7df236) | 

## Members

#### `typedef `[`unit_cell_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a5793de76f74f3473cdadfbe3b4d25cb9) 

#### `typedef `[`cell_descriptor`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a81baee6707b76e8e6d8cc1148f8785fe) 

#### `typedef `[`offset_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a865536de4145b43b1c7d1f018beaddfe) 

#### `typedef `[`extent_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a8158448800d261599cb5c3b32353026a) 

#### `typedef `[`basis_vector_iterator`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a6b705ace73c3dd6349809d41048ed01e) 

#### `typedef `[`cell_iterator`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1ada706e4d26209a7018e70a44fde624d6) 

#### `typedef `[`momentum_iterator`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1af122429b298c9d4c88bb85a2e7bcd281) 

#### `typedef `[`size_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1ad37b84ee0f97ec6b34e61643b97b960d) 

#### `typedef `[`vector_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a041dee9c60dc7d71439b35e002f80fc3) 

#### `typedef `[`boundary_crossing_type`](#da/d56/structalps_1_1lattice__traits_3_01_lattice_graph_descriptor_01_4_1a7eba4bda6e762c1d549053349c7df236) 

# struct `alps::lattice_traits< simple_lattice< U, C > >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`unit_cell_type`](#dd/d42/structalps_1_1lattice__traits_3_01simple__lattice_3_01_u_00_01_c_01_4_01_4_1aab3c403596c33255ffbfc423ee869a50) | 
`typedef `[`cell_descriptor`](#dd/d42/structalps_1_1lattice__traits_3_01simple__lattice_3_01_u_00_01_c_01_4_01_4_1a6a40aa2a9756ae01422dc309b7f99a7e) | 
`typedef `[`offset_type`](#dd/d42/structalps_1_1lattice__traits_3_01simple__lattice_3_01_u_00_01_c_01_4_01_4_1a4e9cca454fd348b31c4d56f361d8e369) | 

## Members

#### `typedef `[`unit_cell_type`](#dd/d42/structalps_1_1lattice__traits_3_01simple__lattice_3_01_u_00_01_c_01_4_01_4_1aab3c403596c33255ffbfc423ee869a50) 

#### `typedef `[`cell_descriptor`](#dd/d42/structalps_1_1lattice__traits_3_01simple__lattice_3_01_u_00_01_c_01_4_01_4_1a6a40aa2a9756ae01422dc309b7f99a7e) 

#### `typedef `[`offset_type`](#dd/d42/structalps_1_1lattice__traits_3_01simple__lattice_3_01_u_00_01_c_01_4_01_4_1a4e9cca454fd348b31c4d56f361d8e369) 

# struct `alps::parity_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d7/d70/structalps_1_1parity__t_1a165e2aade7aa162bd5541df1e3ec6712) | 

## Members

#### `typedef `[`kind`](#d7/d70/structalps_1_1parity__t_1a165e2aade7aa162bd5541df1e3ec6712) 

# struct `alps::parity_traits` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::parity_traits< parity_t, Graph >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4_1a15faa236b7334cdf4047bb832086efac)`(value_type,white)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4_1a6b6a1ad090365177c6f89faaf5f3cb21)`(value_type,black)` | 
`public  `[`BOOST_STATIC_CONSTANT`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4_1adc1e3829740c91327692517598abb0f9)`(value_type,undefined)` | 
`typedef `[`value_type`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4_1a4c5d2e2b16c857c2679a19507e70ba8c) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4_1a15faa236b7334cdf4047bb832086efac)`(value_type,white)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4_1a6b6a1ad090365177c6f89faaf5f3cb21)`(value_type,black)` 

#### `public  `[`BOOST_STATIC_CONSTANT`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4_1adc1e3829740c91327692517598abb0f9)`(value_type,undefined)` 

#### `typedef `[`value_type`](#da/d5a/structalps_1_1parity__traits_3_01parity__t_00_01_graph_01_4_1a4c5d2e2b16c857c2679a19507e70ba8c) 

# struct `alps::point_traits` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`vector_type`](#d7/d29/structalps_1_1point__traits_1a3f2107e2f4ee2bfcb48b6121aa283252) | 

## Members

#### `typedef `[`vector_type`](#d7/d29/structalps_1_1point__traits_1a3f2107e2f4ee2bfcb48b6121aa283252) 

# struct `alps::property_map` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#da/d52/structalps_1_1property__map_1a6b0e0da716125e8bfc0ce4fe418fec9b) | 
`typedef `[`const_type`](#da/d52/structalps_1_1property__map_1a943fd4f17493028ff0582c8586996985) | 

## Members

#### `typedef `[`type`](#da/d52/structalps_1_1property__map_1a6b0e0da716125e8bfc0ce4fe418fec9b) 

#### `typedef `[`const_type`](#da/d52/structalps_1_1property__map_1a943fd4f17493028ff0582c8586996985) 

# struct `alps::property_map< P, const G, Default >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#d4/d4e/structalps_1_1property__map_3_01_p_00_01const_01_g_00_01_default_01_4_1a135c6fd4a04abc83f1b3203e786643eb) | 
`typedef `[`const_type`](#d4/d4e/structalps_1_1property__map_3_01_p_00_01const_01_g_00_01_default_01_4_1a06c048c802afe76c4a8ad7d4e5903898) | 

## Members

#### `typedef `[`type`](#d4/d4e/structalps_1_1property__map_3_01_p_00_01const_01_g_00_01_default_01_4_1a135c6fd4a04abc83f1b3203e786643eb) 

#### `typedef `[`const_type`](#d4/d4e/structalps_1_1property__map_3_01_p_00_01const_01_g_00_01_default_01_4_1a06c048c802afe76c4a8ad7d4e5903898) 

# struct `alps::source_offset_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d2/dd2/structalps_1_1source__offset__t_1ac6e57982617c57a19c7d708141cab65d) | 

## Members

#### `typedef `[`kind`](#d2/dd2/structalps_1_1source__offset__t_1ac6e57982617c57a19c7d708141cab65d) 

# struct `alps::target_offset_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#dc/da2/structalps_1_1target__offset__t_1a149e277c66ad9596020feab55bf439bc) | 

## Members

#### `typedef `[`kind`](#dc/da2/structalps_1_1target__offset__t_1a149e277c66ad9596020feab55bf439bc) 

# struct `alps::vertex_type_t` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`kind`](#d2/d72/structalps_1_1vertex__type__t_1a913140643a99677cedfe07338deac104) | 

## Members

#### `typedef `[`kind`](#d2/d72/structalps_1_1vertex__type__t_1a913140643a99677cedfe07338deac104) 

# namespace `alps::detail` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public alps::oxstream & `[`operator<<`](#db/d9d/disorder_8_c_1a193f3a8bd9269f670b9f41151e238e28)`(alps::oxstream & out,const `[`alps::detail::BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference)` & d)`            | 
`public alps::oxstream & `[`operator<<`](#db/d9d/disorder_8_c_1ac91e010e4f3a57039caae2be4eb1cf03)`(alps::oxstream & out,const `[`alps::detail::VertexReference`](#dc/dc2/classalps_1_1detail_1_1_vertex_reference)` & d)`            | 
`public alps::oxstream & `[`operator<<`](#db/d9d/disorder_8_c_1a61d0b34e7f3ab07e6f1eee98335b7114)`(alps::oxstream & out,const `[`alps::detail::EdgeReference`](#dc/da1/classalps_1_1detail_1_1_edge_reference)` & d)`            | 
`public template<>`  <br/>`T `[`disorder_it`](#d5/d64/disorder_8h_1a8d9e6cf3b8388662c6131a1fba029a12)`(IT start,IT end,MAP & type,T i)`            | 
`public template<>`  <br/>`unsigned int `[`disorder_it`](#d5/d64/disorder_8h_1a0ab4a59b85c07b3ab40b411ea553550f)`(IT start,IT end,MAP & type)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertices_size_type `[`num_vertices_wrap`](#d8/d81/graph__traits_8h_1ae0bf5cd9060acd8dbcfbb03ed8a22435)`(const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::edges_size_type `[`num_edges_wrap`](#d8/d81/graph__traits_8h_1aa9cf2c886865cc69ef127b043ad58e46)`(const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::vertex_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_iterator > `[`vertices_wrap`](#d8/d81/graph__traits_8h_1a5bbc44ce034657e34548920c762b3c2d)`(const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::edge_iterator > `[`edges_wrap`](#d8/d81/graph__traits_8h_1aef059fb0a05f4ac74d98cdd06475a919)`(const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type `[`out_degree_wrap`](#d8/d81/graph__traits_8h_1a18001f259242ffc029788ecb15afa274)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type `[`in_degree_wrap`](#d8/d81/graph__traits_8h_1a2a490368c512fb08eaaeee9b5ff2151a)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type `[`degree_wrap`](#d8/d81/graph__traits_8h_1ad06d371d21330d629674821305a1381b)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::out_edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::out_edge_iterator > `[`out_edges_wrap`](#d8/d81/graph__traits_8h_1ae34dcbafe82524cd2ebb3e4cb3fb6a0a)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::in_edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::in_edge_iterator > `[`in_edges_wrap`](#d8/d81/graph__traits_8h_1a87cf4e411104b62e05126ab8b9cdfa2b)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::adjacency_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::adjacency_iterator > `[`adjacent_vertices_wrap`](#d8/d81/graph__traits_8h_1a4aac488df6c1cfd594f6ddffc409d81d)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor `[`vertex_wrap`](#d8/d81/graph__traits_8h_1ab9dc9ba1d3d707cf5a1e03ae3f78b6e7)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_size_type i,const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor `[`source_wrap`](#d8/d81/graph__traits_8h_1a5125299e86533a682c99c87d98159c75)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::edge_descriptor & e,const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor `[`target_wrap`](#d8/d81/graph__traits_8h_1af6bdeb5c551f17082bf7bdb1d16dec8c)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::edge_descriptor & e,const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::sites_size_type `[`num_sites_wrap`](#d8/d81/graph__traits_8h_1ac4267fcf6ec060452d307a62d91403bf)`(const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bonds_size_type `[`num_bonds_wrap`](#d8/d81/graph__traits_8h_1a3fb4fad1d8bf1ff4eb5bb16ae4b49b6b)`(const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::site_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_iterator > `[`sites_wrap`](#d8/d81/graph__traits_8h_1ad7d5e94f0d4b175c4cccd409184cc421)`(const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor `[`site_wrap`](#d8/d81/graph__traits_8h_1a0eba11bad7dc2a2ae96861f74cdccbe5)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::sites_size_type i,const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::bond_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bond_iterator > `[`bonds_wrap`](#d8/d81/graph__traits_8h_1a4f6b8c5c359500eca07f39f5ce8e145e)`(const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bond_descriptor `[`bond_wrap`](#d8/d81/graph__traits_8h_1a7af10ccc0b29b02bc27ef4460f5c21cb)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bonds_size_type i,const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type `[`num_neighbors_wrap`](#d8/d81/graph__traits_8h_1a3d190613e5ab20ee5b943da1f7b80be3)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor & v,const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::neighbor_bond_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::neighbor_bond_iterator > `[`neighbor_bonds_wrap`](#d8/d81/graph__traits_8h_1ab885dbffe3003bc0927d71a5dfe45dd4)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor & v,const G & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::neighbor_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::neighbor_iterator > `[`neighbors_wrap`](#d8/d81/graph__traits_8h_1aa53f46824fe0288c4badc662061e879e)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor & v,const G & g)`            | 
`public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor `[`neighbor_wrap`](#d8/d81/graph__traits_8h_1ae897d94bf84a6f7860850d44b86e80b0)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor & v,typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type i,const G & g)`            | 
`public template<>`  <br/>`T::graph_type & `[`graph_wrap`](#d8/d81/graph__traits_8h_1a531276d0caf403464a5db00171d2d3e3)`(T & x)`            | 
`public template<>`  <br/>`const T::graph_type & `[`graph_wrap`](#d8/d81/graph__traits_8h_1a75de202520890282ac12effa941b9d41)`(const T & x)`            | 
`class `[`alps::detail::BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference) | 
`class `[`alps::detail::EdgeReference`](#dc/da1/classalps_1_1detail_1_1_edge_reference) | 
`class `[`alps::detail::ParityVisitor`](#d0/d00/classalps_1_1detail_1_1_parity_visitor) | 
`class `[`alps::detail::VertexReference`](#dc/dc2/classalps_1_1detail_1_1_vertex_reference) | 
`struct `[`alps::detail::backbone_edges`](#d4/d37/structalps_1_1detail_1_1backbone__edges) | 
`struct `[`alps::detail::found_property_type_or_default`](#d9/d27/structalps_1_1detail_1_1found__property__type__or__default) | 
`struct `[`alps::detail::found_property_type_or_default_impl`](#d2/d3e/structalps_1_1detail_1_1found__property__type__or__default__impl) | 
`struct `[`alps::detail::found_property_type_or_default_impl< true, PropertyList, Tag, Default >`](#d6/d99/structalps_1_1detail_1_1found__property__type__or__default__impl_3_01true_00_01_property_list_00_01_tag_00_01_default_01_4) | 
`struct `[`alps::detail::get_const_type_member`](#dd/d92/structalps_1_1detail_1_1get__const__type__member) | 
`struct `[`alps::detail::graph_dimension_helper`](#d5/da4/structalps_1_1detail_1_1graph__dimension__helper) | 
`struct `[`alps::detail::graph_dimension_helper< true >`](#de/d75/structalps_1_1detail_1_1graph__dimension__helper_3_01true_01_4) | 
`struct `[`alps::detail::parity_helper`](#dc/d25/structalps_1_1detail_1_1parity__helper) | 
`struct `[`alps::detail::parity_helper< Graph, Parity, true >`](#d3/dac/structalps_1_1detail_1_1parity__helper_3_01_graph_00_01_parity_00_01true_01_4) | 
`struct `[`alps::detail::put_get_helper`](#d3/db2/structalps_1_1detail_1_1put__get__helper) | 
`struct `[`alps::detail::put_get_helper< false >`](#d0/dfb/structalps_1_1detail_1_1put__get__helper_3_01false_01_4) | 
`struct `[`alps::detail::put_get_helper< true >`](#d7/dab/structalps_1_1detail_1_1put__get__helper_3_01true_01_4) | 

## Members

#### `public alps::oxstream & `[`operator<<`](#db/d9d/disorder_8_c_1a193f3a8bd9269f670b9f41151e238e28)`(alps::oxstream & out,const `[`alps::detail::BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference)` & d)` 

#### `public alps::oxstream & `[`operator<<`](#db/d9d/disorder_8_c_1ac91e010e4f3a57039caae2be4eb1cf03)`(alps::oxstream & out,const `[`alps::detail::VertexReference`](#dc/dc2/classalps_1_1detail_1_1_vertex_reference)` & d)` 

#### `public alps::oxstream & `[`operator<<`](#db/d9d/disorder_8_c_1a61d0b34e7f3ab07e6f1eee98335b7114)`(alps::oxstream & out,const `[`alps::detail::EdgeReference`](#dc/da1/classalps_1_1detail_1_1_edge_reference)` & d)` 

#### `public template<>`  <br/>`T `[`disorder_it`](#d5/d64/disorder_8h_1a8d9e6cf3b8388662c6131a1fba029a12)`(IT start,IT end,MAP & type,T i)` 

#### `public template<>`  <br/>`unsigned int `[`disorder_it`](#d5/d64/disorder_8h_1a0ab4a59b85c07b3ab40b411ea553550f)`(IT start,IT end,MAP & type)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertices_size_type `[`num_vertices_wrap`](#d8/d81/graph__traits_8h_1ae0bf5cd9060acd8dbcfbb03ed8a22435)`(const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::edges_size_type `[`num_edges_wrap`](#d8/d81/graph__traits_8h_1aa9cf2c886865cc69ef127b043ad58e46)`(const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::vertex_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_iterator > `[`vertices_wrap`](#d8/d81/graph__traits_8h_1a5bbc44ce034657e34548920c762b3c2d)`(const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::edge_iterator > `[`edges_wrap`](#d8/d81/graph__traits_8h_1aef059fb0a05f4ac74d98cdd06475a919)`(const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type `[`out_degree_wrap`](#d8/d81/graph__traits_8h_1a18001f259242ffc029788ecb15afa274)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type `[`in_degree_wrap`](#d8/d81/graph__traits_8h_1a2a490368c512fb08eaaeee9b5ff2151a)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type `[`degree_wrap`](#d8/d81/graph__traits_8h_1ad06d371d21330d629674821305a1381b)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::out_edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::out_edge_iterator > `[`out_edges_wrap`](#d8/d81/graph__traits_8h_1ae34dcbafe82524cd2ebb3e4cb3fb6a0a)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::in_edge_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::in_edge_iterator > `[`in_edges_wrap`](#d8/d81/graph__traits_8h_1a87cf4e411104b62e05126ab8b9cdfa2b)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::adjacency_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::adjacency_iterator > `[`adjacent_vertices_wrap`](#d8/d81/graph__traits_8h_1a4aac488df6c1cfd594f6ddffc409d81d)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor & v,const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor `[`vertex_wrap`](#d8/d81/graph__traits_8h_1ab9dc9ba1d3d707cf5a1e03ae3f78b6e7)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_size_type i,const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor `[`source_wrap`](#d8/d81/graph__traits_8h_1a5125299e86533a682c99c87d98159c75)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::edge_descriptor & e,const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::vertex_descriptor `[`target_wrap`](#d8/d81/graph__traits_8h_1af6bdeb5c551f17082bf7bdb1d16dec8c)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::edge_descriptor & e,const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::sites_size_type `[`num_sites_wrap`](#d8/d81/graph__traits_8h_1ac4267fcf6ec060452d307a62d91403bf)`(const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bonds_size_type `[`num_bonds_wrap`](#d8/d81/graph__traits_8h_1a3fb4fad1d8bf1ff4eb5bb16ae4b49b6b)`(const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::site_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_iterator > `[`sites_wrap`](#d8/d81/graph__traits_8h_1ad7d5e94f0d4b175c4cccd409184cc421)`(const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor `[`site_wrap`](#d8/d81/graph__traits_8h_1a0eba11bad7dc2a2ae96861f74cdccbe5)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::sites_size_type i,const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::bond_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bond_iterator > `[`bonds_wrap`](#d8/d81/graph__traits_8h_1a4f6b8c5c359500eca07f39f5ce8e145e)`(const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bond_descriptor `[`bond_wrap`](#d8/d81/graph__traits_8h_1a7af10ccc0b29b02bc27ef4460f5c21cb)`(typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::bonds_size_type i,const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type `[`num_neighbors_wrap`](#d8/d81/graph__traits_8h_1a3d190613e5ab20ee5b943da1f7b80be3)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor & v,const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::neighbor_bond_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::neighbor_bond_iterator > `[`neighbor_bonds_wrap`](#d8/d81/graph__traits_8h_1ab885dbffe3003bc0927d71a5dfe45dd4)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor & v,const G & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`graph_traits](#d5/d1a/structalps_1_1graph__traits)< G >::neighbor_iterator, typename [graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::neighbor_iterator > `[`neighbors_wrap`](#d8/d81/graph__traits_8h_1aa53f46824fe0288c4badc662061e879e)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor & v,const G & g)` 

#### `public template<>`  <br/>[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor `[`neighbor_wrap`](#d8/d81/graph__traits_8h_1ae897d94bf84a6f7860850d44b86e80b0)`(const typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::site_descriptor & v,typename `[`graph_traits`](#d5/d1a/structalps_1_1graph__traits)`< G >::degree_size_type i,const G & g)` 

#### `public template<>`  <br/>`T::graph_type & `[`graph_wrap`](#d8/d81/graph__traits_8h_1a531276d0caf403464a5db00171d2d3e3)`(T & x)` 

#### `public template<>`  <br/>`const T::graph_type & `[`graph_wrap`](#d8/d81/graph__traits_8h_1a75de202520890282ac12effa941b9d41)`(const T & x)` 

# class `alps::detail::BasicVertexReference` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1a580fa18342b247933a37cee3f45b77af)`()` | 
`public  `[`BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1aeebcf013850a36cb0b075ac01d72f450)`(XMLTag)` | 
`public inline const offset_type & `[`cell_offset`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1a5bdcd6d306c9ef7b5167ab2f6a4847f0)`() const` | 
`public inline const offset_type & `[`offset`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1af433a4c14a8b569953e70e5381a93c07)`() const` | 
`public inline unsigned int `[`vertex`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1a4f751438097c0e69dcd18a8dcea73cad)`() const` | 
`typedef `[`offset_type`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1a3ffe3b896e34ae3e5ff90f6db3f095f2) | 

## Members

#### `public inline  `[`BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1a580fa18342b247933a37cee3f45b77af)`()` 

#### `public  `[`BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1aeebcf013850a36cb0b075ac01d72f450)`(XMLTag)` 

#### `public inline const offset_type & `[`cell_offset`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1a5bdcd6d306c9ef7b5167ab2f6a4847f0)`() const` 

#### `public inline const offset_type & `[`offset`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1af433a4c14a8b569953e70e5381a93c07)`() const` 

#### `public inline unsigned int `[`vertex`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1a4f751438097c0e69dcd18a8dcea73cad)`() const` 

#### `typedef `[`offset_type`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference_1a3ffe3b896e34ae3e5ff90f6db3f095f2) 

# class `alps::detail::EdgeReference` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`EdgeReference`](#dc/da1/classalps_1_1detail_1_1_edge_reference_1a0e87102236336418d4616bf4cd0448c9)`(XMLTag,std::istream &)` | 
`public inline const `[`BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference)` & `[`source`](#dc/da1/classalps_1_1detail_1_1_edge_reference_1a9a76bdffc0c4caafbe1f10df12fc736a)`() const` | 
`public inline const `[`BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference)` & `[`target`](#dc/da1/classalps_1_1detail_1_1_edge_reference_1aace19b2f40b71053ea87d9134b7cbbac)`() const` | 
`public inline type_type `[`new_type`](#dc/da1/classalps_1_1detail_1_1_edge_reference_1ab7cc2687b92c8f00737694c25fdcdc72)`() const` | 

## Members

#### `public  `[`EdgeReference`](#dc/da1/classalps_1_1detail_1_1_edge_reference_1a0e87102236336418d4616bf4cd0448c9)`(XMLTag,std::istream &)` 

#### `public inline const `[`BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference)` & `[`source`](#dc/da1/classalps_1_1detail_1_1_edge_reference_1a9a76bdffc0c4caafbe1f10df12fc736a)`() const` 

#### `public inline const `[`BasicVertexReference`](#d0/d68/classalps_1_1detail_1_1_basic_vertex_reference)` & `[`target`](#dc/da1/classalps_1_1detail_1_1_edge_reference_1aace19b2f40b71053ea87d9134b7cbbac)`() const` 

#### `public inline type_type `[`new_type`](#dc/da1/classalps_1_1detail_1_1_edge_reference_1ab7cc2687b92c8f00737694c25fdcdc72)`() const` 

# class `alps::detail::ParityVisitor` 

```
class alps::detail::ParityVisitor
  : public boost::dfs_visitor<>
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`ParityVisitor`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1ac8d8618d41fdd7c801f71b94f4db188d)`(PropertyMap & map,bool * bipartite)` | 
`public inline void `[`initialize_vertex`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1aebfb8b03ddf406f6f67310ff24eb7e14)`(vertex_descriptor s,Graph const &)` | 
`public inline void `[`start_vertex`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a5b03194c851c39d90f5a9b0d419ac2a6)`(vertex_descriptor s,Graph const &)` | 
`public inline void `[`tree_edge`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a02ca59256b6fe88ff5b3f83368828c40)`(edge_descriptor e,Graph const & g)` | 
`public inline void `[`back_edge`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a92ccac90dc3d5203d91860faac092ff1)`(edge_descriptor e,const Graph & g) const` | 
`typedef `[`vertex_descriptor`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a8b746220c40e037131857fd2cb1307ba) | 
`typedef `[`edge_descriptor`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a50f25c75736244fb86359c4c50122e74) | 

## Members

#### `public inline  `[`ParityVisitor`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1ac8d8618d41fdd7c801f71b94f4db188d)`(PropertyMap & map,bool * bipartite)` 

#### `public inline void `[`initialize_vertex`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1aebfb8b03ddf406f6f67310ff24eb7e14)`(vertex_descriptor s,Graph const &)` 

#### `public inline void `[`start_vertex`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a5b03194c851c39d90f5a9b0d419ac2a6)`(vertex_descriptor s,Graph const &)` 

#### `public inline void `[`tree_edge`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a02ca59256b6fe88ff5b3f83368828c40)`(edge_descriptor e,Graph const & g)` 

#### `public inline void `[`back_edge`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a92ccac90dc3d5203d91860faac092ff1)`(edge_descriptor e,const Graph & g) const` 

#### `typedef `[`vertex_descriptor`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a8b746220c40e037131857fd2cb1307ba) 

#### `typedef `[`edge_descriptor`](#d0/d00/classalps_1_1detail_1_1_parity_visitor_1a50f25c75736244fb86359c4c50122e74) 

# class `alps::detail::VertexReference` 

```
class alps::detail::VertexReference
  : public alps::detail::BasicVertexReference
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`VertexReference`](#dc/dc2/classalps_1_1detail_1_1_vertex_reference_1afe6a7eb1d41e4992671da7f45000da38)`(XMLTag,std::istream &)` | 
`public inline type_type `[`new_type`](#dc/dc2/classalps_1_1detail_1_1_vertex_reference_1ad188cae969a3935e541d18eb93ec951b)`() const` | 

## Members

#### `public  `[`VertexReference`](#dc/dc2/classalps_1_1detail_1_1_vertex_reference_1afe6a7eb1d41e4992671da7f45000da38)`(XMLTag,std::istream &)` 

#### `public inline type_type `[`new_type`](#dc/dc2/classalps_1_1detail_1_1_vertex_reference_1ad188cae969a3935e541d18eb93ec951b)`() const` 

# struct `alps::detail::backbone_edges` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public const Graph * `[`graph`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1a2cc425f895b2f4c16e95478aac211d12) | 
`public const std::set< int > * `[`backbone`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1af84166aa4bff8883634cac582ac96746) | 
`public inline  `[`backbone_edges`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1a3e34fc20e16cba6356689354ccdf254e)`()` | 
`public inline  `[`backbone_edges`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1a5b87fbabcadd2332c53f0b247f6ea21f)`(Graph const & g,std::set< int > const & bb)` | 
`public inline bool `[`operator()`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1abe80260045ad013cafed34415e5396f2)`(edge_descriptor e) const` | 
`typedef `[`edge_descriptor`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1ade05121432642860d13a055ebb1a227f) | 

## Members

#### `public const Graph * `[`graph`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1a2cc425f895b2f4c16e95478aac211d12) 

#### `public const std::set< int > * `[`backbone`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1af84166aa4bff8883634cac582ac96746) 

#### `public inline  `[`backbone_edges`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1a3e34fc20e16cba6356689354ccdf254e)`()` 

#### `public inline  `[`backbone_edges`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1a5b87fbabcadd2332c53f0b247f6ea21f)`(Graph const & g,std::set< int > const & bb)` 

#### `public inline bool `[`operator()`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1abe80260045ad013cafed34415e5396f2)`(edge_descriptor e) const` 

#### `typedef `[`edge_descriptor`](#d4/d37/structalps_1_1detail_1_1backbone__edges_1ade05121432642860d13a055ebb1a227f) 

# struct `alps::detail::found_property_type_or_default` 

```
struct alps::detail::found_property_type_or_default
  : public alps::detail::found_property_type_or_default_impl< !boost::is_same< boost::property_value< PropertyList, Tag >::type, boost::detail::error_property_not_found >::value, PropertyList, Tag, int >
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::found_property_type_or_default_impl` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d2/d3e/structalps_1_1detail_1_1found__property__type__or__default__impl_1a7a2c0c5adfb41c567cf1997ef9f75c90)`(bool,found)` | 
`typedef `[`type`](#d2/d3e/structalps_1_1detail_1_1found__property__type__or__default__impl_1a14555af99a39f48ba3ee1ee5b311e59a) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d2/d3e/structalps_1_1detail_1_1found__property__type__or__default__impl_1a7a2c0c5adfb41c567cf1997ef9f75c90)`(bool,found)` 

#### `typedef `[`type`](#d2/d3e/structalps_1_1detail_1_1found__property__type__or__default__impl_1a14555af99a39f48ba3ee1ee5b311e59a) 

# struct `alps::detail::found_property_type_or_default_impl< true, PropertyList, Tag, Default >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public  `[`BOOST_STATIC_CONSTANT`](#d6/d99/structalps_1_1detail_1_1found__property__type__or__default__impl_3_01true_00_01_property_list_00_01_tag_00_01_default_01_4_1ab24ff5be239c59d700b8240fd6c642d9)`(bool,found)` | 
`typedef `[`type`](#d6/d99/structalps_1_1detail_1_1found__property__type__or__default__impl_3_01true_00_01_property_list_00_01_tag_00_01_default_01_4_1a603f3758fe1f99337622687f0b2c0d9b) | 

## Members

#### `public  `[`BOOST_STATIC_CONSTANT`](#d6/d99/structalps_1_1detail_1_1found__property__type__or__default__impl_3_01true_00_01_property_list_00_01_tag_00_01_default_01_4_1ab24ff5be239c59d700b8240fd6c642d9)`(bool,found)` 

#### `typedef `[`type`](#d6/d99/structalps_1_1detail_1_1found__property__type__or__default__impl_3_01true_00_01_property_list_00_01_tag_00_01_default_01_4_1a603f3758fe1f99337622687f0b2c0d9b) 

# struct `alps::detail::get_const_type_member` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`type`](#dd/d92/structalps_1_1detail_1_1get__const__type__member_1a4cf5493483439c48b5d4dfc28f6bb39a) | 

## Members

#### `typedef `[`type`](#dd/d92/structalps_1_1detail_1_1get__const__type__member_1a4cf5493483439c48b5d4dfc28f6bb39a) 

# struct `alps::detail::graph_dimension_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::graph_dimension_helper< true >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::parity_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::parity_helper< Graph, Parity, true >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`typedef `[`map_type`](#d3/dac/structalps_1_1detail_1_1parity__helper_3_01_graph_00_01_parity_00_01true_01_4_1a3049ed439f9f07e01c8299dd6a756665) | 

## Members

#### `typedef `[`map_type`](#d3/dac/structalps_1_1detail_1_1parity__helper_3_01_graph_00_01_parity_00_01true_01_4_1a3049ed439f9f07e01c8299dd6a756665) 

# struct `alps::detail::put_get_helper` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::put_get_helper< false >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# struct `alps::detail::put_get_helper< true >` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# namespace `alps::graph` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G >::graph_type & `[`graph`](#d5/df1/latticegraph_8h_1a844f5bdefcd8effeb65caa1911ff9ef1)`(`[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G > & l)`            | 
`public template<>`  <br/>`const `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G >::graph_type & `[`graph`](#d5/df1/latticegraph_8h_1a24b1df61fc50aa7675e7d6a9f5c831d1)`(const `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G > & l)`            | 
`public inline `[`GraphUnitCell::graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#d7/db6/unitcell_8h_1a8c1c2a7b74bdcc34f27f9d36b09c3e78)`(`[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & c)`            | 
`public inline const `[`GraphUnitCell::graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#d7/db6/unitcell_8h_1a608c7c1541d6ae42997d33925a505d75)`(const `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & c)`            | 

## Members

#### `public template<>`  <br/>[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G >::graph_type & `[`graph`](#d5/df1/latticegraph_8h_1a844f5bdefcd8effeb65caa1911ff9ef1)`(`[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G > & l)` 

#### `public template<>`  <br/>`const `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G >::graph_type & `[`graph`](#d5/df1/latticegraph_8h_1a24b1df61fc50aa7675e7d6a9f5c831d1)`(const `[`lattice_graph`](#db/dc8/classalps_1_1lattice__graph)`< L, G > & l)` 

#### `public inline `[`GraphUnitCell::graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#d7/db6/unitcell_8h_1a8c1c2a7b74bdcc34f27f9d36b09c3e78)`(`[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & c)` 

#### `public inline const `[`GraphUnitCell::graph_type`](#de/d7d/classboost_1_1adjacency__list)` & `[`graph`](#d7/db6/unitcell_8h_1a608c7c1541d6ae42997d33925a505d75)`(const `[`GraphUnitCell`](#d9/d50/classalps_1_1_graph_unit_cell)` & c)` 

# namespace `boost` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public template<>`  <br/>`inline std::ostream & `[`operator<<`](#d6/df3/graph_8h_1ae57ea4509c5b3fb43cccbe93bf0ded5d)`(std::ostream & os,const `[`boost::adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>`inline alps::oxstream & `[`operator<<`](#d6/df3/graph_8h_1a262d84d6466531be2a8d8642bf4c6b7b)`(alps::oxstream & oxs,const `[`boost::adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::sites_size_type `[`num_sites`](#d8/d81/graph__traits_8h_1aca574b4f65b02fe07f0bbb3dde387b06)`(const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::bonds_size_type `[`num_bonds`](#d8/d81/graph__traits_8h_1abd5b931e6ced647c8e3af8201063e394)`(const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list](#de/d7d/classboost_1_1adjacency__list)< T0, T1, T2, T3, T4, T5, T6 > >::site_iterator, typename [alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_iterator > `[`sites`](#d8/d81/graph__traits_8h_1a8abd310d0011fd6175ec4593fe7e9f2a)`(const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor `[`site`](#d8/d81/graph__traits_8h_1a594a0a5df7ad5a363958a65221256acd)`(typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::sites_size_type i,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list](#de/d7d/classboost_1_1adjacency__list)< T0, T1, T2, T3, T4, T5, T6 > >::bond_iterator, typename [alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::bond_iterator > `[`bonds`](#d8/d81/graph__traits_8h_1a046eabdfeb03eb961ff28a9c4c8db082)`(const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::bond_descriptor `[`bond`](#d8/d81/graph__traits_8h_1aaa4a24da50ea81eeeb07c2d44351d761)`(typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::bonds_size_type i,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::degree_size_type `[`num_neighbors`](#d8/d81/graph__traits_8h_1a4e80a65e28400c81e53c3200258cdb55)`(const typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor & v,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list](#de/d7d/classboost_1_1adjacency__list)< T0, T1, T2, T3, T4, T5, T6 > >::neighbor_bond_iterator, typename [alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::neighbor_bond_iterator > `[`neighbor_bonds`](#d8/d81/graph__traits_8h_1a2e68b2d2dbfd870e0d6d5e2aade5872b)`(const typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor & v,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>`std::pair< typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list](#de/d7d/classboost_1_1adjacency__list)< T0, T1, T2, T3, T4, T5, T6 > >::neighbor_iterator, typename [alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::neighbor_iterator > `[`neighbors`](#d8/d81/graph__traits_8h_1a15772ef6fb6c65eaf94036ba0b36bad7)`(const typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor & v,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor `[`neighbor`](#d8/d81/graph__traits_8h_1a095d90e91cf0b17c68f27e40b982f825)`(const typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor & v,typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::degree_size_type i,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)`            | 
`public template<>`  <br/>`V `[`get`](#d0/d21/propertymap_8h_1a3701d66e3fe30d025d110f4593cb8966)`(const `[`alps::singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map)`< V, K > & m,const K &)`            | 
`public template<>`  <br/>`void `[`put`](#d0/d21/propertymap_8h_1a85596bc0bad890668a63f4581d69b901)`(`[`alps::singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map)`< V, K > & m,const K & k,const V & v)`            | 
`class `[`boost::adjacency_list`](#de/d7d/classboost_1_1adjacency__list) | 

## Members

#### `public template<>`  <br/>`inline std::ostream & `[`operator<<`](#d6/df3/graph_8h_1ae57ea4509c5b3fb43cccbe93bf0ded5d)`(std::ostream & os,const `[`boost::adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>`inline alps::oxstream & `[`operator<<`](#d6/df3/graph_8h_1a262d84d6466531be2a8d8642bf4c6b7b)`(alps::oxstream & oxs,const `[`boost::adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::sites_size_type `[`num_sites`](#d8/d81/graph__traits_8h_1aca574b4f65b02fe07f0bbb3dde387b06)`(const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::bonds_size_type `[`num_bonds`](#d8/d81/graph__traits_8h_1abd5b931e6ced647c8e3af8201063e394)`(const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list](#de/d7d/classboost_1_1adjacency__list)< T0, T1, T2, T3, T4, T5, T6 > >::site_iterator, typename [alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_iterator > `[`sites`](#d8/d81/graph__traits_8h_1a8abd310d0011fd6175ec4593fe7e9f2a)`(const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor `[`site`](#d8/d81/graph__traits_8h_1a594a0a5df7ad5a363958a65221256acd)`(typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::sites_size_type i,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list](#de/d7d/classboost_1_1adjacency__list)< T0, T1, T2, T3, T4, T5, T6 > >::bond_iterator, typename [alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::bond_iterator > `[`bonds`](#d8/d81/graph__traits_8h_1a046eabdfeb03eb961ff28a9c4c8db082)`(const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::bond_descriptor `[`bond`](#d8/d81/graph__traits_8h_1aaa4a24da50ea81eeeb07c2d44351d761)`(typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::bonds_size_type i,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::degree_size_type `[`num_neighbors`](#d8/d81/graph__traits_8h_1a4e80a65e28400c81e53c3200258cdb55)`(const typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor & v,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list](#de/d7d/classboost_1_1adjacency__list)< T0, T1, T2, T3, T4, T5, T6 > >::neighbor_bond_iterator, typename [alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::neighbor_bond_iterator > `[`neighbor_bonds`](#d8/d81/graph__traits_8h_1a2e68b2d2dbfd870e0d6d5e2aade5872b)`(const typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor & v,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>`std::pair< typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list](#de/d7d/classboost_1_1adjacency__list)< T0, T1, T2, T3, T4, T5, T6 > >::neighbor_iterator, typename [alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::neighbor_iterator > `[`neighbors`](#d8/d81/graph__traits_8h_1a15772ef6fb6c65eaf94036ba0b36bad7)`(const typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor & v,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor `[`neighbor`](#d8/d81/graph__traits_8h_1a095d90e91cf0b17c68f27e40b982f825)`(const typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::site_descriptor & v,typename `[`alps::graph_traits](#d5/d1a/structalps_1_1graph__traits)< [adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > >::degree_size_type i,const `[`adjacency_list`](#de/d7d/classboost_1_1adjacency__list)`< T0, T1, T2, T3, T4, T5, T6 > & g)` 

#### `public template<>`  <br/>`V `[`get`](#d0/d21/propertymap_8h_1a3701d66e3fe30d025d110f4593cb8966)`(const `[`alps::singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map)`< V, K > & m,const K &)` 

#### `public template<>`  <br/>`void `[`put`](#d0/d21/propertymap_8h_1a85596bc0bad890668a63f4581d69b901)`(`[`alps::singleton_property_map`](#d7/da3/classalps_1_1singleton__property__map)`< V, K > & m,const K & k,const V & v)` 

# class `boost::adjacency_list` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------

## Members

# class `alps::hypercubic_lattice::cell_iterator` 

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ab97df561e13dede21c397aaf673233ca)`()` | 
`public inline  `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a597a9f90f301ab384e27ba0c57af0158)`(const `[`lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice)` & l,const offset_type & o)` | 
`public inline const `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` & `[`operator++`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ac5221d9490f0d5fe0193bc30c0b6a884)`()` | 
`public inline `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` `[`operator++`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ac7494dae5f6382cf0b359fcbee388c25)`(int)` | 
`public inline bool `[`operator==`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a3ee1ea0f4aa9a514c01b1308105ca7ff)`(const `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` & it)` | 
`public inline bool `[`operator!=`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a03fb55106ed62a49dbdb8e182394deae)`(const `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` & it)` | 
`public inline cell_descriptor `[`operator*`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1aa00bf1d2e72aea4824b33b807fb10573)`() const` | 
`protected const `[`lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice)` * `[`lattice_`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a00ef8ab9318830c79ad05db712e0427a) | 
`protected offset_type `[`offset_`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ad3be52b47bfc8844e071b058b4668076) | 
`typedef `[`difference_type`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ad44ddff0c94dba21299d09e763462f75) | 
`typedef `[`value_type`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1acd9af09fa2c3b11116f9bc80c9513c44) | 
`typedef `[`pointer`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a80c7291621eda3d1ea867a821b0e9d53) | 
`typedef `[`reference`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a6d04942d4ed89c12b3b7152cf87abf86) | 
`typedef `[`iterator_category`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a50119a61ed973ca5c97bae64f2ddba9a) | 

## Members

#### `public inline  `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ab97df561e13dede21c397aaf673233ca)`()` 

#### `public inline  `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a597a9f90f301ab384e27ba0c57af0158)`(const `[`lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice)` & l,const offset_type & o)` 

#### `public inline const `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` & `[`operator++`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ac5221d9490f0d5fe0193bc30c0b6a884)`()` 

#### `public inline `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` `[`operator++`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ac7494dae5f6382cf0b359fcbee388c25)`(int)` 

#### `public inline bool `[`operator==`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a3ee1ea0f4aa9a514c01b1308105ca7ff)`(const `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` & it)` 

#### `public inline bool `[`operator!=`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a03fb55106ed62a49dbdb8e182394deae)`(const `[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` & it)` 

#### `public inline cell_descriptor `[`operator*`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1aa00bf1d2e72aea4824b33b807fb10573)`() const` 

#### `protected const `[`lattice_type`](#d9/d9f/classalps_1_1hypercubic__lattice)` * `[`lattice_`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a00ef8ab9318830c79ad05db712e0427a) 

#### `protected offset_type `[`offset_`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ad3be52b47bfc8844e071b058b4668076) 

#### `typedef `[`difference_type`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1ad44ddff0c94dba21299d09e763462f75) 

#### `typedef `[`value_type`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1acd9af09fa2c3b11116f9bc80c9513c44) 

#### `typedef `[`pointer`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a80c7291621eda3d1ea867a821b0e9d53) 

#### `typedef `[`reference`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a6d04942d4ed89c12b3b7152cf87abf86) 

#### `typedef `[`iterator_category`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator_1a50119a61ed973ca5c97bae64f2ddba9a) 

# class `alps::hypercubic_lattice::momentum_iterator` 

```
class alps::hypercubic_lattice::momentum_iterator
  : public alps::hypercubic_lattice< BASE, EX >::cell_iterator
```  

## Summary

 Members                        | Descriptions                                
--------------------------------|---------------------------------------------
`public inline  `[`momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1a98ca2b55c4c8f33f6c6c6339fc2048d8)`(`[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` it)` | 
`public inline const vector_type & `[`operator*`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1a125fae6fba14cc1ff510bcf30fd235cf)`() const` | 
`public inline const vector_type * `[`operator->`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1a9db762780de9c7059756bdb452e6e3da)`() const` | 
`public inline const `[`momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator)` & `[`operator++`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1a4674da9642995acb8bb62219e52d634d)`()` | 
`public inline const `[`momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator)` & `[`operator++`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1ab8377d7c8fc07a8a91139ce0e0831e0d)`(int)` | 

## Members

#### `public inline  `[`momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1a98ca2b55c4c8f33f6c6c6339fc2048d8)`(`[`cell_iterator`](#d0/d8d/classalps_1_1hypercubic__lattice_1_1cell__iterator)` it)` 

#### `public inline const vector_type & `[`operator*`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1a125fae6fba14cc1ff510bcf30fd235cf)`() const` 

#### `public inline const vector_type * `[`operator->`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1a9db762780de9c7059756bdb452e6e3da)`() const` 

#### `public inline const `[`momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator)` & `[`operator++`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1a4674da9642995acb8bb62219e52d634d)`()` 

#### `public inline const `[`momentum_iterator`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator)` & `[`operator++`](#d6/d0d/classalps_1_1hypercubic__lattice_1_1momentum__iterator_1ab8377d7c8fc07a8a91139ce0e0831e0d)`(int)` 

Generated by [Moxygen](https://sourcey.com/moxygen)
