# Comparing `tmp/resqpy-4.7.4.tar.gz` & `tmp/resqpy-4.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resqpy-4.7.4.tar", max compression
+gzip compressed data, was "resqpy-4.7.5.tar", max compression
```

## Comparing `resqpy-4.7.4.tar` & `resqpy-4.7.5.tar`

### file list

```diff
@@ -1,197 +1,197 @@
--rw-r--r--   0        0        0     1059 2023-04-15 11:54:37.774578 resqpy-4.7.4/LICENSE
--rw-r--r--   0        0        0     2893 2023-04-15 11:54:37.774578 resqpy-4.7.4/README.md
--rw-r--r--   0        0        0     3227 2023-04-15 11:54:53.150790 resqpy-4.7.4/pyproject.toml
--rw-r--r--   0        0        0      555 2023-04-15 11:54:53.150790 resqpy-4.7.4/resqpy/__init__.py
--rw-r--r--   0        0        0    24782 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/crs.py
--rw-r--r--   0        0        0     1982 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/__init__.py
--rw-r--r--   0        0        0     6410 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_edges_per_column_property_array.py
--rw-r--r--   0        0        0    20540 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_faults.py
--rw-r--r--   0        0        0     6417 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_one_blocked_well_property.py
--rw-r--r--   0        0        0     8657 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_one_grid_property_array.py
--rw-r--r--   0        0        0     2431 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_single_cell_grid.py
--rw-r--r--   0        0        0     5495 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_wells_from_ascii_file.py
--rw-r--r--   0        0        0     6037 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_zone_by_layer_property.py
--rw-r--r--   0        0        0    11586 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_coarsened_grid.py
--rw-r--r--   0        0        0    10201 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_common.py
--rw-r--r--   0        0        0     3730 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_copy_grid.py
--rw-r--r--   0        0        0    11731 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_drape_to_surface.py
--rw-r--r--   0        0        0    16391 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_extract_box.py
--rw-r--r--   0        0        0    22969 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_extract_box_for_well.py
--rw-r--r--   0        0        0    20325 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_fault_throw_scaling.py
--rw-r--r--   0        0        0     7157 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_gather_ensemble.py
--rw-r--r--   0        0        0    17929 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_interpolated_grid.py
--rw-r--r--   0        0        0     9876 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_local_depth_adjustment.py
--rw-r--r--   0        0        0    20513 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_refined_grid.py
--rw-r--r--   0        0        0     5166 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_tilted_grid.py
--rw-r--r--   0        0        0     4792 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_unsplit_grid.py
--rw-r--r--   0        0        0    18825 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_zonal_grid.py
--rw-r--r--   0        0        0     4358 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_zone_layer_ranges_from_array.py
--rw-r--r--   0        0        0      996 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/fault/__init__.py
--rw-r--r--   0        0        0    29402 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/fault/_gcs_functions.py
--rw-r--r--   0        0        0   109110 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/fault/_grid_connection_set.py
--rw-r--r--   0        0        0      692 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/__init__.py
--rw-r--r--   0        0        0    20689 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_cell_properties.py
--rw-r--r--   0        0        0    10120 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_connection_sets.py
--rw-r--r--   0        0        0    19936 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_create_grid_xml.py
--rw-r--r--   0        0        0    32064 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_defined_geometry.py
--rw-r--r--   0        0        0    28203 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_extract_functions.py
--rw-r--r--   0        0        0    16516 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_face_functions.py
--rw-r--r--   0        0        0    12236 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_faults.py
--rw-r--r--   0        0        0   127766 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_grid.py
--rw-r--r--   0        0        0     3544 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_grid_types.py
--rw-r--r--   0        0        0      338 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_intervals_info.py
--rw-r--r--   0        0        0      604 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_moved_functions.py
--rw-r--r--   0        0        0     7243 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_pillars.py
--rw-r--r--   0        0        0     5386 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_pixel_maps.py
--rw-r--r--   0        0        0    65440 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_points_functions.py
--rw-r--r--   0        0        0    40520 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_regular_grid.py
--rw-r--r--   0        0        0    19413 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_transmissibility.py
--rw-r--r--   0        0        0     7944 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_write_hdf5_from_caches.py
--rw-r--r--   0        0        0     6147 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_write_nexus_corp.py
--rw-r--r--   0        0        0    13087 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_xyz.py
--rw-r--r--   0        0        0     2593 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid_surface/__init__.py
--rw-r--r--   0        0        0    35739 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid_surface/_blocked_well_populate.py
--rw-r--r--   0        0        0    64016 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/_find_faces.py
--rw-r--r--   0        0        0    26056 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/_grid_skin.py
--rw-r--r--   0        0        0    14379 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/_grid_surface.py
--rw-r--r--   0        0        0    22498 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/_trajectory_intersects.py
--rw-r--r--   0        0        0    39760 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/grid_surface_cuda.py
--rw-r--r--   0        0        0      539 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/lines/__init__.py
--rw-r--r--   0        0        0    11960 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/lines/_common.py
--rw-r--r--   0        0        0    41425 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/lines/_polyline.py
--rw-r--r--   0        0        0    26366 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/lines/_polyline_set.py
--rw-r--r--   0        0        0      378 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/__init__.py
--rw-r--r--   0        0        0    30171 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_catalogue.py
--rw-r--r--   0        0        0     2840 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_context.py
--rw-r--r--   0        0        0    34159 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_forestry.py
--rw-r--r--   0        0        0     3371 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_grids.py
--rw-r--r--   0        0        0    14172 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_hdf5.py
--rw-r--r--   0        0        0   103055 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_model.py
--rw-r--r--   0        0        0    23589 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_xml.py
--rw-r--r--   0        0        0      909 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/__init__.py
--rw-r--r--   0        0        0     7017 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/_multiprocessing.py
--rw-r--r--   0        0        0       72 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/wrappers/__init__.py
--rw-r--r--   0        0        0     5952 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/wrappers/blocked_well_mp.py
--rw-r--r--   0        0        0    21156 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/wrappers/grid_surface_mp.py
--rw-r--r--   0        0        0     5793 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/wrappers/mesh_mp.py
--rw-r--r--   0        0        0       84 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/olio/__init__.py
--rw-r--r--   0        0        0     2147 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/olio/ab_toolbox.py
--rw-r--r--   0        0        0     7521 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/olio/base.py
--rw-r--r--   0        0        0    20925 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/box_utilities.py
--rw-r--r--   0        0        0     5935 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/class_dict.py
--rw-r--r--   0        0        0     9285 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/consolidation.py
--rw-r--r--   0        0        0     5177 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/data/build.py
--rw-r--r--   0        0        0   498136 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/data/properties.json
--rw-r--r--   0        0        0    19836 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/dataframe.py
--rw-r--r--   0        0        0      307 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/exceptions.py
--rw-r--r--   0        0        0     1313 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/factors.py
--rw-r--r--   0        0        0    24541 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/fine_coarse.py
--rw-r--r--   0        0        0    27398 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/grid_functions.py
--rw-r--r--   0        0        0    20158 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/intersection.py
--rw-r--r--   0        0        0     8408 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/keyword_files.py
--rw-r--r--   0        0        0    19210 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/load_data.py
--rw-r--r--   0        0        0     6628 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/point_inclusion.py
--rw-r--r--   0        0        0     1103 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/random_seed.py
--rw-r--r--   0        0        0     5441 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/read_nexus_fault.py
--rw-r--r--   0        0        0    17083 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/relperm.py
--rw-r--r--   0        0        0    12189 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/simple_lines.py
--rw-r--r--   0        0        0      760 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/time.py
--rw-r--r--   0        0        0      822 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/trademark.py
--rw-r--r--   0        0        0    61188 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/transmission.py
--rw-r--r--   0        0        0    44288 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/triangulation.py
--rw-r--r--   0        0        0     7324 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/uuid.py
--rw-r--r--   0        0        0    45231 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/vdb.py
--rw-r--r--   0        0        0    46253 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/vector_utilities.py
--rw-r--r--   0        0        0     6185 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/volume.py
--rw-r--r--   0        0        0    26220 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/wellspec_keywords.py
--rw-r--r--   0        0        0     5142 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/write_data.py
--rw-r--r--   0        0        0    19055 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/write_hdf5.py
--rw-r--r--   0        0        0    24925 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/xml_et.py
--rw-r--r--   0        0        0     1824 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/xml_namespaces.py
--rw-r--r--   0        0        0     5709 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/zmap_reader.py
--rw-r--r--   0        0        0     2206 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/__init__.py
--rw-r--r--   0        0        0     2937 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/_utils.py
--rw-r--r--   0        0        0     1685 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/boundary_feature.py
--rw-r--r--   0        0        0     5190 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/boundary_feature_interpretation.py
--rw-r--r--   0        0        0     6186 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/earth_model_interpretation.py
--rw-r--r--   0        0        0    12457 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/fault_interpretation.py
--rw-r--r--   0        0        0     2757 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/fluid_boundary_feature.py
--rw-r--r--   0        0        0     1702 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/frontier_feature.py
--rw-r--r--   0        0        0     4498 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/generic_interpretation.py
--rw-r--r--   0        0        0     3771 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/genetic_boundary_feature.py
--rw-r--r--   0        0        0     8605 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/geobody_boundary_interpretation.py
--rw-r--r--   0        0        0     1836 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/geobody_feature.py
--rw-r--r--   0        0        0     8052 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/geobody_interpretation.py
--rw-r--r--   0        0        0     1739 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/geologic_unit_feature.py
--rw-r--r--   0        0        0     8346 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/horizon_interpretation.py
--rw-r--r--   0        0        0     2697 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/organization_feature.py
--rw-r--r--   0        0        0     5565 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/rock_fluid_unit_feature.py
--rw-r--r--   0        0        0     2675 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/tectonic_boundary_feature.py
--rw-r--r--   0        0        0     1843 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/wellbore_feature.py
--rw-r--r--   0        0        0     6973 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/wellbore_interpretation.py
--rw-r--r--   0        0        0     2155 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/__init__.py
--rw-r--r--   0        0        0    16509 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_collection_add_part.py
--rw-r--r--   0        0        0    13021 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_collection_create_xml.py
--rw-r--r--   0        0        0    30025 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_collection_get_attributes.py
--rw-r--r--   0        0        0     5368 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_collection_support.py
--rw-r--r--   0        0        0    24426 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_property.py
--rw-r--r--   0        0        0    66946 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/grid_property_collection.py
--rw-r--r--   0        0        0   143259 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/property_collection.py
--rw-r--r--   0        0        0    36127 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/property_common.py
--rw-r--r--   0        0        0     5557 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/property_kind.py
--rw-r--r--   0        0        0     7737 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/string_lookup.py
--rw-r--r--   0        0        0     1077 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/well_interval_property.py
--rw-r--r--   0        0        0     1577 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/well_interval_property_collection.py
--rw-r--r--   0        0        0     1205 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/well_log.py
--rw-r--r--   0        0        0     7633 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/well_log_collection.py
--rw-r--r--   0        0        0      713 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/__init__.py
--rw-r--r--   0        0        0     4493 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_add_ab_properties.py
--rw-r--r--   0        0        0     6067 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_add_surfaces.py
--rw-r--r--   0        0        0    32019 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_grid_from_cp.py
--rw-r--r--   0        0        0    34317 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_import_nexus.py
--rw-r--r--   0        0        0     6306 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_import_vdb_all_grids.py
--rw-r--r--   0        0        0    21372 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_import_vdb_ensemble.py
--rw-r--r--   0        0        0     1311 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/__init__.py
--rw-r--r--   0        0        0     8861 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_binary_contact_interpretation.py
--rw-r--r--   0        0        0    10381 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_geologic_unit_interpretation.py
--rw-r--r--   0        0        0     1772 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_strata_common.py
--rw-r--r--   0        0        0     6797 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_stratigraphic_column.py
--rw-r--r--   0        0        0    13322 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_stratigraphic_column_rank.py
--rw-r--r--   0        0        0     7432 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_stratigraphic_unit_feature.py
--rw-r--r--   0        0        0    10167 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_stratigraphic_unit_interpretation.py
--rw-r--r--   0        0        0      696 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/__init__.py
--rw-r--r--   0        0        0     2331 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/_base_surface.py
--rw-r--r--   0        0        0     3082 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/_combined_surface.py
--rw-r--r--   0        0        0    42192 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/_mesh.py
--rw-r--r--   0        0        0    26120 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/_pointset.py
--rw-r--r--   0        0        0    56386 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/surface/_surface.py
--rw-r--r--   0        0        0    24102 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/surface/_tri_mesh.py
--rw-r--r--   0        0        0    25907 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/surface/_triangulated_patch.py
--rw-r--r--   0        0        0     1074 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/__init__.py
--rw-r--r--   0        0        0     8595 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_any_time_series.py
--rw-r--r--   0        0        0     6617 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_from_nexus_summary.py
--rw-r--r--   0        0        0     6366 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_functions.py
--rw-r--r--   0        0        0     3311 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_geologic_time_series.py
--rw-r--r--   0        0        0     2759 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_time_duration.py
--rw-r--r--   0        0        0    10818 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_time_series.py
--rw-r--r--   0        0        0      603 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/__init__.py
--rw-r--r--   0        0        0    15328 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_hexa_grid.py
--rw-r--r--   0        0        0    35856 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_prism_grid.py
--rw-r--r--   0        0        0     7862 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_pyramid_grid.py
--rw-r--r--   0        0        0    10208 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_tetra_grid.py
--rw-r--r--   0        0        0    51550 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_unstructured_grid.py
--rw-r--r--   0        0        0     1135 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/weights_and_measures/__init__.py
--rw-r--r--   0        0        0     4811 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/weights_and_measures/nexus_units.py
--rw-r--r--   0        0        0    16186 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/weights_and_measures/weights_and_measures.py
--rw-r--r--   0        0        0      990 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/__init__.py
--rw-r--r--   0        0        0   186258 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_blocked_well.py
--rw-r--r--   0        0        0    22138 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_deviation_survey.py
--rw-r--r--   0        0        0     7154 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_md_datum.py
--rw-r--r--   0        0        0    48693 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_trajectory.py
--rw-r--r--   0        0        0    15192 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_wellbore_frame.py
--rw-r--r--   0        0        0     8403 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/_wellbore_marker.py
--rw-r--r--   0        0        0    20933 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/_wellbore_marker_frame.py
--rw-r--r--   0        0        0    22555 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/blocked_well_frame.py
--rw-r--r--   0        0        0    24743 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/well_object_funcs.py
--rw-r--r--   0        0        0     5969 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/well_utils.py
--rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 resqpy-4.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-04-20 15:03:15.641749 resqpy-4.7.5/LICENSE
+-rw-r--r--   0        0        0     2893 2023-04-20 15:03:15.641749 resqpy-4.7.5/README.md
+-rw-r--r--   0        0        0     3227 2023-04-20 15:03:32.530127 resqpy-4.7.5/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-04-20 15:03:32.530127 resqpy-4.7.5/resqpy/__init__.py
+-rw-r--r--   0        0        0    24782 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/crs.py
+-rw-r--r--   0        0        0     1982 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/__init__.py
+-rw-r--r--   0        0        0     6410 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_add_edges_per_column_property_array.py
+-rw-r--r--   0        0        0    20540 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_add_faults.py
+-rw-r--r--   0        0        0     6417 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_add_one_blocked_well_property.py
+-rw-r--r--   0        0        0     8657 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_add_one_grid_property_array.py
+-rw-r--r--   0        0        0     2431 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_add_single_cell_grid.py
+-rw-r--r--   0        0        0     5495 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_add_wells_from_ascii_file.py
+-rw-r--r--   0        0        0     6037 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_add_zone_by_layer_property.py
+-rw-r--r--   0        0        0    11586 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_coarsened_grid.py
+-rw-r--r--   0        0        0    10201 2023-04-20 15:03:15.653754 resqpy-4.7.5/resqpy/derived_model/_common.py
+-rw-r--r--   0        0        0     3730 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_copy_grid.py
+-rw-r--r--   0        0        0    11731 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_drape_to_surface.py
+-rw-r--r--   0        0        0    16391 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_extract_box.py
+-rw-r--r--   0        0        0    22969 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_extract_box_for_well.py
+-rw-r--r--   0        0        0    20325 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_fault_throw_scaling.py
+-rw-r--r--   0        0        0     7157 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_gather_ensemble.py
+-rw-r--r--   0        0        0    17929 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_interpolated_grid.py
+-rw-r--r--   0        0        0     9876 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_local_depth_adjustment.py
+-rw-r--r--   0        0        0    20513 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_refined_grid.py
+-rw-r--r--   0        0        0     5166 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_tilted_grid.py
+-rw-r--r--   0        0        0     4792 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_unsplit_grid.py
+-rw-r--r--   0        0        0    18825 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_zonal_grid.py
+-rw-r--r--   0        0        0     4358 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/derived_model/_zone_layer_ranges_from_array.py
+-rw-r--r--   0        0        0      996 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/fault/__init__.py
+-rw-r--r--   0        0        0    29402 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/fault/_gcs_functions.py
+-rw-r--r--   0        0        0   109110 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/fault/_grid_connection_set.py
+-rw-r--r--   0        0        0      692 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/__init__.py
+-rw-r--r--   0        0        0    20689 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_cell_properties.py
+-rw-r--r--   0        0        0    10120 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_connection_sets.py
+-rw-r--r--   0        0        0    19936 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_create_grid_xml.py
+-rw-r--r--   0        0        0    32064 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_defined_geometry.py
+-rw-r--r--   0        0        0    28203 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_extract_functions.py
+-rw-r--r--   0        0        0    16516 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_face_functions.py
+-rw-r--r--   0        0        0    12236 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_faults.py
+-rw-r--r--   0        0        0   127766 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_grid.py
+-rw-r--r--   0        0        0     3544 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_grid_types.py
+-rw-r--r--   0        0        0      338 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_intervals_info.py
+-rw-r--r--   0        0        0      604 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_moved_functions.py
+-rw-r--r--   0        0        0     7243 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_pillars.py
+-rw-r--r--   0        0        0     5386 2023-04-20 15:03:15.657755 resqpy-4.7.5/resqpy/grid/_pixel_maps.py
+-rw-r--r--   0        0        0    65440 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid/_points_functions.py
+-rw-r--r--   0        0        0    40520 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid/_regular_grid.py
+-rw-r--r--   0        0        0    19413 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid/_transmissibility.py
+-rw-r--r--   0        0        0     7944 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid/_write_hdf5_from_caches.py
+-rw-r--r--   0        0        0     6147 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid/_write_nexus_corp.py
+-rw-r--r--   0        0        0    13087 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid/_xyz.py
+-rw-r--r--   0        0        0     2593 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid_surface/__init__.py
+-rw-r--r--   0        0        0    35739 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid_surface/_blocked_well_populate.py
+-rw-r--r--   0        0        0    64016 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid_surface/_find_faces.py
+-rw-r--r--   0        0        0    26056 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid_surface/_grid_skin.py
+-rw-r--r--   0        0        0    14379 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid_surface/_grid_surface.py
+-rw-r--r--   0        0        0    22498 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid_surface/_trajectory_intersects.py
+-rw-r--r--   0        0        0    39760 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/grid_surface/grid_surface_cuda.py
+-rw-r--r--   0        0        0      539 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/lines/__init__.py
+-rw-r--r--   0        0        0    11960 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/lines/_common.py
+-rw-r--r--   0        0        0    41425 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/lines/_polyline.py
+-rw-r--r--   0        0        0    26366 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/lines/_polyline_set.py
+-rw-r--r--   0        0        0      378 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/model/__init__.py
+-rw-r--r--   0        0        0    30171 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/model/_catalogue.py
+-rw-r--r--   0        0        0     2840 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/model/_context.py
+-rw-r--r--   0        0        0    34159 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/model/_forestry.py
+-rw-r--r--   0        0        0     3371 2023-04-20 15:03:15.661757 resqpy-4.7.5/resqpy/model/_grids.py
+-rw-r--r--   0        0        0    14172 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/model/_hdf5.py
+-rw-r--r--   0        0        0   103055 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/model/_model.py
+-rw-r--r--   0        0        0    23589 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/model/_xml.py
+-rw-r--r--   0        0        0      909 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/multi_processing/__init__.py
+-rw-r--r--   0        0        0     7017 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/multi_processing/_multiprocessing.py
+-rw-r--r--   0        0        0       72 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/multi_processing/wrappers/__init__.py
+-rw-r--r--   0        0        0     5952 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/multi_processing/wrappers/blocked_well_mp.py
+-rw-r--r--   0        0        0    21156 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/multi_processing/wrappers/grid_surface_mp.py
+-rw-r--r--   0        0        0     5793 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/multi_processing/wrappers/mesh_mp.py
+-rw-r--r--   0        0        0       84 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/__init__.py
+-rw-r--r--   0        0        0     2147 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/ab_toolbox.py
+-rw-r--r--   0        0        0     7521 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/base.py
+-rw-r--r--   0        0        0    20925 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/box_utilities.py
+-rw-r--r--   0        0        0     5935 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/class_dict.py
+-rw-r--r--   0        0        0     9285 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/consolidation.py
+-rw-r--r--   0        0        0     5177 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/data/build.py
+-rw-r--r--   0        0        0   498136 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/data/properties.json
+-rw-r--r--   0        0        0    19836 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/dataframe.py
+-rw-r--r--   0        0        0      307 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/exceptions.py
+-rw-r--r--   0        0        0     1313 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/factors.py
+-rw-r--r--   0        0        0    24541 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/fine_coarse.py
+-rw-r--r--   0        0        0    27398 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/grid_functions.py
+-rw-r--r--   0        0        0    20158 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/intersection.py
+-rw-r--r--   0        0        0     8408 2023-04-20 15:03:15.665759 resqpy-4.7.5/resqpy/olio/keyword_files.py
+-rw-r--r--   0        0        0    19210 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/load_data.py
+-rw-r--r--   0        0        0     6628 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/point_inclusion.py
+-rw-r--r--   0        0        0     1103 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/random_seed.py
+-rw-r--r--   0        0        0     5441 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/read_nexus_fault.py
+-rw-r--r--   0        0        0    17083 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/relperm.py
+-rw-r--r--   0        0        0    12189 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/simple_lines.py
+-rw-r--r--   0        0        0      760 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/time.py
+-rw-r--r--   0        0        0      822 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/trademark.py
+-rw-r--r--   0        0        0    61188 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/transmission.py
+-rw-r--r--   0        0        0    44288 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/triangulation.py
+-rw-r--r--   0        0        0     7324 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/uuid.py
+-rw-r--r--   0        0        0    45231 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/vdb.py
+-rw-r--r--   0        0        0    46253 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/vector_utilities.py
+-rw-r--r--   0        0        0     6185 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/volume.py
+-rw-r--r--   0        0        0    26220 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/wellspec_keywords.py
+-rw-r--r--   0        0        0     5142 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/write_data.py
+-rw-r--r--   0        0        0    19055 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/write_hdf5.py
+-rw-r--r--   0        0        0    24925 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/xml_et.py
+-rw-r--r--   0        0        0     1824 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/xml_namespaces.py
+-rw-r--r--   0        0        0     5709 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/olio/zmap_reader.py
+-rw-r--r--   0        0        0     2206 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/__init__.py
+-rw-r--r--   0        0        0     2937 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/_utils.py
+-rw-r--r--   0        0        0     1685 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/boundary_feature.py
+-rw-r--r--   0        0        0     5190 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/boundary_feature_interpretation.py
+-rw-r--r--   0        0        0     6186 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/earth_model_interpretation.py
+-rw-r--r--   0        0        0    12457 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/fault_interpretation.py
+-rw-r--r--   0        0        0     2757 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/fluid_boundary_feature.py
+-rw-r--r--   0        0        0     1702 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/frontier_feature.py
+-rw-r--r--   0        0        0     4498 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/generic_interpretation.py
+-rw-r--r--   0        0        0     3771 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/genetic_boundary_feature.py
+-rw-r--r--   0        0        0     8605 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/geobody_boundary_interpretation.py
+-rw-r--r--   0        0        0     1836 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/geobody_feature.py
+-rw-r--r--   0        0        0     8052 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/geobody_interpretation.py
+-rw-r--r--   0        0        0     1739 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/geologic_unit_feature.py
+-rw-r--r--   0        0        0     8346 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/horizon_interpretation.py
+-rw-r--r--   0        0        0     2697 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/organization_feature.py
+-rw-r--r--   0        0        0     5565 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/rock_fluid_unit_feature.py
+-rw-r--r--   0        0        0     2675 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/tectonic_boundary_feature.py
+-rw-r--r--   0        0        0     1843 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/wellbore_feature.py
+-rw-r--r--   0        0        0     6973 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/organize/wellbore_interpretation.py
+-rw-r--r--   0        0        0     2155 2023-04-20 15:03:15.669761 resqpy-4.7.5/resqpy/property/__init__.py
+-rw-r--r--   0        0        0    16697 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/_collection_add_part.py
+-rw-r--r--   0        0        0    13021 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/_collection_create_xml.py
+-rw-r--r--   0        0        0    30025 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/_collection_get_attributes.py
+-rw-r--r--   0        0        0     5368 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/_collection_support.py
+-rw-r--r--   0        0        0    24426 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/_property.py
+-rw-r--r--   0        0        0    66946 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/grid_property_collection.py
+-rw-r--r--   0        0        0   143259 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/property_collection.py
+-rw-r--r--   0        0        0    36127 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/property_common.py
+-rw-r--r--   0        0        0     5557 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/property_kind.py
+-rw-r--r--   0        0        0     7737 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/string_lookup.py
+-rw-r--r--   0        0        0     1077 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/well_interval_property.py
+-rw-r--r--   0        0        0     1577 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/well_interval_property_collection.py
+-rw-r--r--   0        0        0     1205 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/well_log.py
+-rw-r--r--   0        0        0     7633 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/property/well_log_collection.py
+-rw-r--r--   0        0        0      713 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/rq_import/__init__.py
+-rw-r--r--   0        0        0     4493 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/rq_import/_add_ab_properties.py
+-rw-r--r--   0        0        0     6067 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/rq_import/_add_surfaces.py
+-rw-r--r--   0        0        0    32019 2023-04-20 15:03:15.673762 resqpy-4.7.5/resqpy/rq_import/_grid_from_cp.py
+-rw-r--r--   0        0        0    34317 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/rq_import/_import_nexus.py
+-rw-r--r--   0        0        0     6306 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/rq_import/_import_vdb_all_grids.py
+-rw-r--r--   0        0        0    21372 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/rq_import/_import_vdb_ensemble.py
+-rw-r--r--   0        0        0     1311 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/strata/__init__.py
+-rw-r--r--   0        0        0     8861 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/strata/_binary_contact_interpretation.py
+-rw-r--r--   0        0        0    10381 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/strata/_geologic_unit_interpretation.py
+-rw-r--r--   0        0        0     1772 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/strata/_strata_common.py
+-rw-r--r--   0        0        0     6797 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/strata/_stratigraphic_column.py
+-rw-r--r--   0        0        0    13322 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/strata/_stratigraphic_column_rank.py
+-rw-r--r--   0        0        0     7432 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/strata/_stratigraphic_unit_feature.py
+-rw-r--r--   0        0        0    10167 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/strata/_stratigraphic_unit_interpretation.py
+-rw-r--r--   0        0        0      696 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/surface/__init__.py
+-rw-r--r--   0        0        0     2331 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/surface/_base_surface.py
+-rw-r--r--   0        0        0     3082 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/surface/_combined_surface.py
+-rw-r--r--   0        0        0    42192 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/surface/_mesh.py
+-rw-r--r--   0        0        0    26120 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/surface/_pointset.py
+-rw-r--r--   0        0        0    56386 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/surface/_surface.py
+-rw-r--r--   0        0        0    24315 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/surface/_tri_mesh.py
+-rw-r--r--   0        0        0    25907 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/surface/_triangulated_patch.py
+-rw-r--r--   0        0        0     1074 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/time_series/__init__.py
+-rw-r--r--   0        0        0     8595 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/time_series/_any_time_series.py
+-rw-r--r--   0        0        0     6617 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/time_series/_from_nexus_summary.py
+-rw-r--r--   0        0        0     6366 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/time_series/_functions.py
+-rw-r--r--   0        0        0     3311 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/time_series/_geologic_time_series.py
+-rw-r--r--   0        0        0     2759 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/time_series/_time_duration.py
+-rw-r--r--   0        0        0    10818 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/time_series/_time_series.py
+-rw-r--r--   0        0        0      603 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/unstructured/__init__.py
+-rw-r--r--   0        0        0    15328 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/unstructured/_hexa_grid.py
+-rw-r--r--   0        0        0    35856 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/unstructured/_prism_grid.py
+-rw-r--r--   0        0        0     7862 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/unstructured/_pyramid_grid.py
+-rw-r--r--   0        0        0    10208 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/unstructured/_tetra_grid.py
+-rw-r--r--   0        0        0    51550 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/unstructured/_unstructured_grid.py
+-rw-r--r--   0        0        0     1135 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/weights_and_measures/__init__.py
+-rw-r--r--   0        0        0     4811 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/weights_and_measures/nexus_units.py
+-rw-r--r--   0        0        0    16186 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/weights_and_measures/weights_and_measures.py
+-rw-r--r--   0        0        0      990 2023-04-20 15:03:15.677764 resqpy-4.7.5/resqpy/well/__init__.py
+-rw-r--r--   0        0        0   187787 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/_blocked_well.py
+-rw-r--r--   0        0        0    22138 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/_deviation_survey.py
+-rw-r--r--   0        0        0     7154 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/_md_datum.py
+-rw-r--r--   0        0        0    48693 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/_trajectory.py
+-rw-r--r--   0        0        0    15192 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/_wellbore_frame.py
+-rw-r--r--   0        0        0     8403 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/_wellbore_marker.py
+-rw-r--r--   0        0        0    20933 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/_wellbore_marker_frame.py
+-rw-r--r--   0        0        0    22555 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/blocked_well_frame.py
+-rw-r--r--   0        0        0    24743 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/well_object_funcs.py
+-rw-r--r--   0        0        0     5969 2023-04-20 15:03:15.681766 resqpy-4.7.5/resqpy/well/well_utils.py
+-rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 resqpy-4.7.5/PKG-INFO
```

### Comparing `resqpy-4.7.4/LICENSE` & `resqpy-4.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/README.md` & `resqpy-4.7.5/README.md`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/pyproject.toml` & `resqpy-4.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["poetry>=1.0.2", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "resqpy"
-version = "4.7.4" # Set at build time
+version = "4.7.5" # Set at build time
 description = "Python API for working with RESQML models"
 authors = ["BP"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bp/resqpy"
 documentation = "https://resqpy.readthedocs.io/en/latest/"
 keywords = ["RESQML"]
```

### Comparing `resqpy-4.7.4/resqpy/__init__.py` & `resqpy-4.7.5/resqpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,10 @@
     weights_and_measures
     well
     olio
 """
 
 import logging
 
-__version__ = "4.7.4"  # Set at build time
+__version__ = "4.7.5"  # Set at build time
 log = logging.getLogger(__name__)
 log.info(f"Imported resqpy version {__version__}")
```

### Comparing `resqpy-4.7.4/resqpy/crs.py` & `resqpy-4.7.5/resqpy/crs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/__init__.py` & `resqpy-4.7.5/resqpy/derived_model/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_add_edges_per_column_property_array.py` & `resqpy-4.7.5/resqpy/derived_model/_add_edges_per_column_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_add_faults.py` & `resqpy-4.7.5/resqpy/derived_model/_add_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_add_one_blocked_well_property.py` & `resqpy-4.7.5/resqpy/derived_model/_add_one_blocked_well_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_add_one_grid_property_array.py` & `resqpy-4.7.5/resqpy/derived_model/_add_one_grid_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_add_single_cell_grid.py` & `resqpy-4.7.5/resqpy/derived_model/_add_single_cell_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_add_wells_from_ascii_file.py` & `resqpy-4.7.5/resqpy/derived_model/_add_wells_from_ascii_file.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_add_zone_by_layer_property.py` & `resqpy-4.7.5/resqpy/derived_model/_add_zone_by_layer_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_coarsened_grid.py` & `resqpy-4.7.5/resqpy/derived_model/_coarsened_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_common.py` & `resqpy-4.7.5/resqpy/derived_model/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_copy_grid.py` & `resqpy-4.7.5/resqpy/derived_model/_copy_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_drape_to_surface.py` & `resqpy-4.7.5/resqpy/derived_model/_drape_to_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_extract_box.py` & `resqpy-4.7.5/resqpy/derived_model/_extract_box.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_extract_box_for_well.py` & `resqpy-4.7.5/resqpy/derived_model/_extract_box_for_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_fault_throw_scaling.py` & `resqpy-4.7.5/resqpy/derived_model/_fault_throw_scaling.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_gather_ensemble.py` & `resqpy-4.7.5/resqpy/derived_model/_gather_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_interpolated_grid.py` & `resqpy-4.7.5/resqpy/derived_model/_interpolated_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_local_depth_adjustment.py` & `resqpy-4.7.5/resqpy/derived_model/_local_depth_adjustment.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_refined_grid.py` & `resqpy-4.7.5/resqpy/derived_model/_refined_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_tilted_grid.py` & `resqpy-4.7.5/resqpy/derived_model/_tilted_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_unsplit_grid.py` & `resqpy-4.7.5/resqpy/derived_model/_unsplit_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_zonal_grid.py` & `resqpy-4.7.5/resqpy/derived_model/_zonal_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/derived_model/_zone_layer_ranges_from_array.py` & `resqpy-4.7.5/resqpy/derived_model/_zone_layer_ranges_from_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/fault/__init__.py` & `resqpy-4.7.5/resqpy/fault/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/fault/_gcs_functions.py` & `resqpy-4.7.5/resqpy/fault/_gcs_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/fault/_grid_connection_set.py` & `resqpy-4.7.5/resqpy/fault/_grid_connection_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/__init__.py` & `resqpy-4.7.5/resqpy/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_cell_properties.py` & `resqpy-4.7.5/resqpy/grid/_cell_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_connection_sets.py` & `resqpy-4.7.5/resqpy/grid/_connection_sets.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_create_grid_xml.py` & `resqpy-4.7.5/resqpy/grid/_create_grid_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_defined_geometry.py` & `resqpy-4.7.5/resqpy/grid/_defined_geometry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_extract_functions.py` & `resqpy-4.7.5/resqpy/grid/_extract_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_face_functions.py` & `resqpy-4.7.5/resqpy/grid/_face_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_faults.py` & `resqpy-4.7.5/resqpy/grid/_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_grid.py` & `resqpy-4.7.5/resqpy/grid/_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_grid_types.py` & `resqpy-4.7.5/resqpy/grid/_grid_types.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_moved_functions.py` & `resqpy-4.7.5/resqpy/grid/_moved_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_pillars.py` & `resqpy-4.7.5/resqpy/grid/_pillars.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_pixel_maps.py` & `resqpy-4.7.5/resqpy/grid/_pixel_maps.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_points_functions.py` & `resqpy-4.7.5/resqpy/grid/_points_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_regular_grid.py` & `resqpy-4.7.5/resqpy/grid/_regular_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_transmissibility.py` & `resqpy-4.7.5/resqpy/grid/_transmissibility.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_write_hdf5_from_caches.py` & `resqpy-4.7.5/resqpy/grid/_write_hdf5_from_caches.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_write_nexus_corp.py` & `resqpy-4.7.5/resqpy/grid/_write_nexus_corp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid/_xyz.py` & `resqpy-4.7.5/resqpy/grid/_xyz.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid_surface/__init__.py` & `resqpy-4.7.5/resqpy/grid_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid_surface/_blocked_well_populate.py` & `resqpy-4.7.5/resqpy/grid_surface/_blocked_well_populate.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid_surface/_find_faces.py` & `resqpy-4.7.5/resqpy/grid_surface/_find_faces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid_surface/_grid_skin.py` & `resqpy-4.7.5/resqpy/grid_surface/_grid_skin.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid_surface/_grid_surface.py` & `resqpy-4.7.5/resqpy/grid_surface/_grid_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid_surface/_trajectory_intersects.py` & `resqpy-4.7.5/resqpy/grid_surface/_trajectory_intersects.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/grid_surface/grid_surface_cuda.py` & `resqpy-4.7.5/resqpy/grid_surface/grid_surface_cuda.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/lines/__init__.py` & `resqpy-4.7.5/resqpy/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/lines/_common.py` & `resqpy-4.7.5/resqpy/lines/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/lines/_polyline.py` & `resqpy-4.7.5/resqpy/lines/_polyline.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/lines/_polyline_set.py` & `resqpy-4.7.5/resqpy/lines/_polyline_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/model/_catalogue.py` & `resqpy-4.7.5/resqpy/model/_catalogue.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/model/_context.py` & `resqpy-4.7.5/resqpy/model/_context.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/model/_forestry.py` & `resqpy-4.7.5/resqpy/model/_forestry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/model/_grids.py` & `resqpy-4.7.5/resqpy/model/_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/model/_hdf5.py` & `resqpy-4.7.5/resqpy/model/_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/model/_model.py` & `resqpy-4.7.5/resqpy/model/_model.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/model/_xml.py` & `resqpy-4.7.5/resqpy/model/_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/multi_processing/__init__.py` & `resqpy-4.7.5/resqpy/multi_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/multi_processing/_multiprocessing.py` & `resqpy-4.7.5/resqpy/multi_processing/_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/multi_processing/wrappers/blocked_well_mp.py` & `resqpy-4.7.5/resqpy/multi_processing/wrappers/blocked_well_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/multi_processing/wrappers/grid_surface_mp.py` & `resqpy-4.7.5/resqpy/multi_processing/wrappers/grid_surface_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/multi_processing/wrappers/mesh_mp.py` & `resqpy-4.7.5/resqpy/multi_processing/wrappers/mesh_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/ab_toolbox.py` & `resqpy-4.7.5/resqpy/olio/ab_toolbox.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/base.py` & `resqpy-4.7.5/resqpy/olio/base.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/box_utilities.py` & `resqpy-4.7.5/resqpy/olio/box_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/class_dict.py` & `resqpy-4.7.5/resqpy/olio/class_dict.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/consolidation.py` & `resqpy-4.7.5/resqpy/olio/consolidation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/data/build.py` & `resqpy-4.7.5/resqpy/olio/data/build.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/data/properties.json` & `resqpy-4.7.5/resqpy/olio/data/properties.json`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/dataframe.py` & `resqpy-4.7.5/resqpy/olio/dataframe.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/factors.py` & `resqpy-4.7.5/resqpy/olio/factors.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/fine_coarse.py` & `resqpy-4.7.5/resqpy/olio/fine_coarse.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/grid_functions.py` & `resqpy-4.7.5/resqpy/olio/grid_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/intersection.py` & `resqpy-4.7.5/resqpy/olio/intersection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/keyword_files.py` & `resqpy-4.7.5/resqpy/olio/keyword_files.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/load_data.py` & `resqpy-4.7.5/resqpy/olio/load_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/point_inclusion.py` & `resqpy-4.7.5/resqpy/olio/point_inclusion.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/random_seed.py` & `resqpy-4.7.5/resqpy/olio/random_seed.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/read_nexus_fault.py` & `resqpy-4.7.5/resqpy/olio/read_nexus_fault.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/relperm.py` & `resqpy-4.7.5/resqpy/olio/relperm.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/simple_lines.py` & `resqpy-4.7.5/resqpy/olio/simple_lines.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/time.py` & `resqpy-4.7.5/resqpy/olio/time.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/trademark.py` & `resqpy-4.7.5/resqpy/olio/trademark.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/transmission.py` & `resqpy-4.7.5/resqpy/olio/transmission.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/triangulation.py` & `resqpy-4.7.5/resqpy/olio/triangulation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/uuid.py` & `resqpy-4.7.5/resqpy/olio/uuid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/vdb.py` & `resqpy-4.7.5/resqpy/olio/vdb.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/vector_utilities.py` & `resqpy-4.7.5/resqpy/olio/vector_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/volume.py` & `resqpy-4.7.5/resqpy/olio/volume.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/wellspec_keywords.py` & `resqpy-4.7.5/resqpy/olio/wellspec_keywords.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/write_data.py` & `resqpy-4.7.5/resqpy/olio/write_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/write_hdf5.py` & `resqpy-4.7.5/resqpy/olio/write_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/xml_et.py` & `resqpy-4.7.5/resqpy/olio/xml_et.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/xml_namespaces.py` & `resqpy-4.7.5/resqpy/olio/xml_namespaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/olio/zmap_reader.py` & `resqpy-4.7.5/resqpy/olio/zmap_reader.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/__init__.py` & `resqpy-4.7.5/resqpy/organize/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/_utils.py` & `resqpy-4.7.5/resqpy/organize/_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/boundary_feature.py` & `resqpy-4.7.5/resqpy/organize/boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/boundary_feature_interpretation.py` & `resqpy-4.7.5/resqpy/organize/boundary_feature_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/earth_model_interpretation.py` & `resqpy-4.7.5/resqpy/organize/earth_model_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/fault_interpretation.py` & `resqpy-4.7.5/resqpy/organize/fault_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/fluid_boundary_feature.py` & `resqpy-4.7.5/resqpy/organize/fluid_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/frontier_feature.py` & `resqpy-4.7.5/resqpy/organize/frontier_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/generic_interpretation.py` & `resqpy-4.7.5/resqpy/organize/generic_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/genetic_boundary_feature.py` & `resqpy-4.7.5/resqpy/organize/genetic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/geobody_boundary_interpretation.py` & `resqpy-4.7.5/resqpy/organize/geobody_boundary_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/geobody_feature.py` & `resqpy-4.7.5/resqpy/organize/geobody_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/geobody_interpretation.py` & `resqpy-4.7.5/resqpy/organize/geobody_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/geologic_unit_feature.py` & `resqpy-4.7.5/resqpy/organize/geologic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/horizon_interpretation.py` & `resqpy-4.7.5/resqpy/organize/horizon_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/organization_feature.py` & `resqpy-4.7.5/resqpy/organize/organization_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/rock_fluid_unit_feature.py` & `resqpy-4.7.5/resqpy/organize/rock_fluid_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/tectonic_boundary_feature.py` & `resqpy-4.7.5/resqpy/organize/tectonic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/wellbore_feature.py` & `resqpy-4.7.5/resqpy/organize/wellbore_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/organize/wellbore_interpretation.py` & `resqpy-4.7.5/resqpy/organize/wellbore_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/__init__.py` & `resqpy-4.7.5/resqpy/property/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/_collection_add_part.py` & `resqpy-4.7.5/resqpy/property/_collection_add_part.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,22 @@
         return method(part) is None
     elif attrib == 'none':
         return method(part) is not None
     return method(part) != attrib
 
 
 def _check_not_none_and_not_uuid_match(uuid, method, part):
-    return uuid is not None and not bu.matching_uuids(uuid, method(part))
+    if uuid is None:
+        return False
+    if isinstance(uuid, str):
+        if uuid == '*':
+            return method(part) is None
+        elif uuid == 'none':
+            return method(part) is not None
+    return not bu.matching_uuids(uuid, method(part))
 
 
 def _check_citation_title(citation_title, citation_title_match_mode, other, part):
     if citation_title is not None:
         if isinstance(citation_title_match_mode, bool):
             citation_title_match_mode = 'starts' if citation_title_match_mode else None
         if citation_title_match_mode is None or citation_title_match_mode == 'is':
```

### Comparing `resqpy-4.7.4/resqpy/property/_collection_create_xml.py` & `resqpy-4.7.5/resqpy/property/_collection_create_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/_collection_get_attributes.py` & `resqpy-4.7.5/resqpy/property/_collection_get_attributes.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/_collection_support.py` & `resqpy-4.7.5/resqpy/property/_collection_support.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/_property.py` & `resqpy-4.7.5/resqpy/property/_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/grid_property_collection.py` & `resqpy-4.7.5/resqpy/property/grid_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/property_collection.py` & `resqpy-4.7.5/resqpy/property/property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/property_common.py` & `resqpy-4.7.5/resqpy/property/property_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/property_kind.py` & `resqpy-4.7.5/resqpy/property/property_kind.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/string_lookup.py` & `resqpy-4.7.5/resqpy/property/string_lookup.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/well_interval_property.py` & `resqpy-4.7.5/resqpy/property/well_interval_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/well_interval_property_collection.py` & `resqpy-4.7.5/resqpy/property/well_interval_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/well_log.py` & `resqpy-4.7.5/resqpy/property/well_log.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/property/well_log_collection.py` & `resqpy-4.7.5/resqpy/property/well_log_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/rq_import/__init__.py` & `resqpy-4.7.5/resqpy/rq_import/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/rq_import/_add_ab_properties.py` & `resqpy-4.7.5/resqpy/rq_import/_add_ab_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/rq_import/_add_surfaces.py` & `resqpy-4.7.5/resqpy/rq_import/_add_surfaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/rq_import/_grid_from_cp.py` & `resqpy-4.7.5/resqpy/rq_import/_grid_from_cp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/rq_import/_import_nexus.py` & `resqpy-4.7.5/resqpy/rq_import/_import_nexus.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/rq_import/_import_vdb_all_grids.py` & `resqpy-4.7.5/resqpy/rq_import/_import_vdb_all_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/rq_import/_import_vdb_ensemble.py` & `resqpy-4.7.5/resqpy/rq_import/_import_vdb_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/strata/__init__.py` & `resqpy-4.7.5/resqpy/strata/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/strata/_binary_contact_interpretation.py` & `resqpy-4.7.5/resqpy/strata/_binary_contact_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/strata/_geologic_unit_interpretation.py` & `resqpy-4.7.5/resqpy/strata/_geologic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/strata/_strata_common.py` & `resqpy-4.7.5/resqpy/strata/_strata_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/strata/_stratigraphic_column.py` & `resqpy-4.7.5/resqpy/strata/_stratigraphic_column.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/strata/_stratigraphic_column_rank.py` & `resqpy-4.7.5/resqpy/strata/_stratigraphic_column_rank.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/strata/_stratigraphic_unit_feature.py` & `resqpy-4.7.5/resqpy/strata/_stratigraphic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/strata/_stratigraphic_unit_interpretation.py` & `resqpy-4.7.5/resqpy/strata/_stratigraphic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/surface/__init__.py` & `resqpy-4.7.5/resqpy/surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/surface/_base_surface.py` & `resqpy-4.7.5/resqpy/surface/_base_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/surface/_combined_surface.py` & `resqpy-4.7.5/resqpy/surface/_combined_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/surface/_mesh.py` & `resqpy-4.7.5/resqpy/surface/_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/surface/_pointset.py` & `resqpy-4.7.5/resqpy/surface/_pointset.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/surface/_surface.py` & `resqpy-4.7.5/resqpy/surface/_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/surface/_tri_mesh.py` & `resqpy-4.7.5/resqpy/surface/_tri_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,18 @@
            originator (str, optional): the name of the person creating the mesh, defaults to login id;
               ignored if uuid is not None
            extra_metadata (dict, optional): string key, value pairs to add as extra metadata for the mesh;
               ignored if uuid is not None
 
         returns:
            the newly created TriMesh object
+
+        note:
+           using the z_uom argument will result in the tri mesh's full_array_ref() method returning data with
+           x and y values in the object's crs, whilst z values will be in the given uom
         """
 
         if uuid is None:
             assert t_side > 0.0
             assert nj > 1 and ni > 1
             assert z_values is None or z_values.shape == (nj, ni)
             assert origin is None or len(origin) == 3
```

### Comparing `resqpy-4.7.4/resqpy/surface/_triangulated_patch.py` & `resqpy-4.7.5/resqpy/surface/_triangulated_patch.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/time_series/__init__.py` & `resqpy-4.7.5/resqpy/time_series/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/time_series/_any_time_series.py` & `resqpy-4.7.5/resqpy/time_series/_any_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/time_series/_from_nexus_summary.py` & `resqpy-4.7.5/resqpy/time_series/_from_nexus_summary.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/time_series/_functions.py` & `resqpy-4.7.5/resqpy/time_series/_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/time_series/_geologic_time_series.py` & `resqpy-4.7.5/resqpy/time_series/_geologic_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/time_series/_time_duration.py` & `resqpy-4.7.5/resqpy/time_series/_time_duration.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/time_series/_time_series.py` & `resqpy-4.7.5/resqpy/time_series/_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/unstructured/__init__.py` & `resqpy-4.7.5/resqpy/unstructured/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/unstructured/_hexa_grid.py` & `resqpy-4.7.5/resqpy/unstructured/_hexa_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/unstructured/_prism_grid.py` & `resqpy-4.7.5/resqpy/unstructured/_prism_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/unstructured/_pyramid_grid.py` & `resqpy-4.7.5/resqpy/unstructured/_pyramid_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/unstructured/_tetra_grid.py` & `resqpy-4.7.5/resqpy/unstructured/_tetra_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/unstructured/_unstructured_grid.py` & `resqpy-4.7.5/resqpy/unstructured/_unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/weights_and_measures/__init__.py` & `resqpy-4.7.5/resqpy/weights_and_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/weights_and_measures/nexus_units.py` & `resqpy-4.7.5/resqpy/weights_and_measures/nexus_units.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/weights_and_measures/weights_and_measures.py` & `resqpy-4.7.5/resqpy/weights_and_measures/weights_and_measures.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/__init__.py` & `resqpy-4.7.5/resqpy/well/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/_blocked_well.py` & `resqpy-4.7.5/resqpy/well/_blocked_well.py`

 * *Files 0% similar despite different names*

```diff
@@ -1295,16 +1295,17 @@
 
         arguments:
            i_col (string, default 'IW'): the column name to use for cell I index values
            j_col (string, default 'JW'): the column name to use for cell J index values
            k_col (string, default 'L'): the column name to use for cell K index values
            one_based (boolean, default True): if True, simulator protocol i, j & k values are placed in I, J & K columns;
               if False, resqml zero based values; this does not affect the interpretation of min_k0 & max_k0 arguments
-           extra_columns_list (list of string, optional): list of WELLSPEC column names to include in the dataframe, from currently
-              recognised values: 'GRID', 'ANGLA', 'ANGLV', 'LENGTH', 'KH', 'DEPTH', 'MD', 'X', 'Y', 'RADW', 'SKIN', 'PPERF', 'RADB', 'WI', 'WBC'
+           extra_columns_list (list of string, optional): list of WELLSPEC column names to include in the dataframe,
+              from currently recognised values: 'GRID', 'ANGLA', 'ANGLV', 'LENGTH', 'KH', 'DEPTH', 'MD', 'X', 'Y',
+              'RADW', 'SKIN', 'PPERF', 'RADB', 'WI', 'WBC'
            ntg_uuid (uuid.UUID, optional): the uuid of the net to gross ratio property; if present is used to downgrade the i & j
               permeabilities in the calculation of KH; ignored if 'KH' not in the extra column list and min_kh is not specified;
               the argument may also be a dictionary mapping from grid uuid to ntg uuid; if no net to gross data is provided, it
               is effectively assumed to be one (or, equivalently, the I & J permeability data is applicable to the gross rock); see
               also preferential_perforation argument which can cause adjustment of effective ntg in partially perforated cells
            perm_i_uuid (uuid.UUID or dictionary, optional): the uuid of the permeability property in the I direction;
               required if 'KH' is included in the extra columns list and min_kh is not specified; ignored otherwise;
@@ -1318,15 +1319,15 @@
            sato_uuid (uuid.UUID, optional): the uuid of an oil saturation property; required if min_sato is specified; may also
               be a dictionary mapping from grid uuid to sato uuid; ignored if min_sato is None
            satg_uuid (uuid.UUID, optional): the uuid of a gas saturation property; required if max_satg is specified; may also
               be a dictionary mapping from grid uuid to satg uuid; ignored if max_satg is None
            region_uuid (uuid.UUID, optional): the uuid of a discrete or categorical property, required if region_list is not None;
               may also be a dictionary mapping from grid uuid to region uuid; ignored if region_list is None
            radw (float, optional): if present, the wellbore radius used for all perforations; must be in correct units for intended
-              use of the WELLSPEC style dataframe; will default to 0.25 if 'RADW' is included in the extra column list
+              use of the WELLSPEC style dataframe; will default to 0.33 ft or 0.1 m if 'RADW' is included in the extra column list
            skin (float, optional): if present, a skin column is included with values set to this constant
            stat (string, optional): if present, should be 'ON' or 'OFF' and is used for all perforations; will default to 'ON' if
               'STAT' is included in the extra column list
            active_only (boolean, default False): if True, only cells that are flagged in the grid object as active are included;
               if False, cells are included whether active or not
            min_k0 (int, optional): if present, perforations in layers above this are excluded (layer number will be applied
               naively to all grids – not recommended when working with more than one grid with different layering)
@@ -1407,34 +1408,40 @@
 
         assert length_mode in ['MD', 'straight']
         assert length_uom is None or length_uom in ['m', 'ft']
 
         anglv_ref, angla_plane_ref = BlockedWell.__verify_angle_references(anglv_ref, angla_plane_ref)
         column_list = [i_col, j_col, k_col]
 
-        column_list, add_as_properties, use_properties, skin, stat, radw = BlockedWell.__verify_extra_properties_to_be_added_to_dataframe(
-            extra_columns_list = extra_columns_list,
-            column_list = column_list,
-            add_as_properties = add_as_properties,
-            use_properties = use_properties,
-            skin = skin,
-            stat = stat,
-            radw = radw)
-
         pc = None
+        pc_timeless = None
         if use_properties:
             pc = rqp.PropertyCollection(support = self)
+            pc_timeless = rqp.selective_version_of_collection(pc, time_series_uuid = 'none')
+            if pc_timeless is None or pc_timeless.number_of_parts() == 0:
+                pc_timeless = None
             if property_time_index is not None:
+                property_time_index = int(property_time_index)
                 pc = rqp.selective_version_of_collection(pc, time_index = property_time_index)
             if pc is None or pc.number_of_parts() == 0:
                 log.error(
                     f'no blocked well properties found for time index {property_time_index} for well {self.title}')
-                pc = None
+                pc = pc_timeless
         pc_titles = [] if pc is None else pc.titles()
 
+        column_list, add_as_properties, use_properties, skin, stat, radw =  \
+            BlockedWell.__verify_extra_properties_to_be_added_to_dataframe(
+                extra_columns_list = extra_columns_list,
+                column_list = column_list,
+                add_as_properties = add_as_properties,
+                use_properties = use_properties,
+                skin = skin,
+                stat = stat,
+                radw = radw)
+
         max_satw, min_sato, max_satg = BlockedWell.__verify_saturation_ranges_and_property_uuids(
             max_satw, min_sato, max_satg, satw_uuid, sato_uuid, satg_uuid)
 
         min_kh, doing_kh = BlockedWell.__verify_perm_i_uuid_for_kh(min_kh = min_kh,
                                                                    column_list = column_list,
                                                                    perm_i_uuid = perm_i_uuid,
                                                                    pc_titles = pc_titles)
@@ -1600,38 +1607,43 @@
                                                                                 pc = pc,
                                                                                 pc_titles = pc_titles,
                                                                                 ci = ci)
 
             if skip_interval_due_to_min_kh:
                 continue
 
-            length, radw, skin, radb, wi, wbc = BlockedWell.__get_pc_arrays_for_interval(pc = pc,
-                                                                                         pc_titles = pc_titles,
-                                                                                         ci = ci,
-                                                                                         length = length,
-                                                                                         radw = radw,
-                                                                                         skin = skin)
+            length, radw_i, skin_i, radb, wi, wbc = BlockedWell.__get_pc_arrays_for_interval(pc = pc,
+                                                                                             pc_timeless = pc_timeless,
+                                                                                             pc_titles = pc_titles,
+                                                                                             ci = ci,
+                                                                                             length = length,
+                                                                                             radw = radw,
+                                                                                             skin = skin)
+            if skin_i is None:
+                skin_i = 0.0
+            if radw_i is None:
+                radw_i = (0.33 if length_uom == 'ft' else 0.1)
 
             radb, wi, wbc = BlockedWell.__get_well_inflow_parameters_for_interval(do_well_inflow = do_well_inflow,
                                                                                   isotropic_perm = isotropic_perm,
                                                                                   ntg_is_one = ntg_is_one,
                                                                                   k_i = k_i,
                                                                                   k_j = k_j,
                                                                                   k_k = k_k,
                                                                                   sine_anglv = sine_anglv,
                                                                                   cosine_anglv = cosine_anglv,
                                                                                   sine_angla = sine_angla,
                                                                                   cosine_angla = cosine_angla,
                                                                                   grid = grid,
                                                                                   cell_kji0 = cell_kji0,
-                                                                                  radw = radw,
+                                                                                  radw = radw_i,
                                                                                   radb = radb,
                                                                                   wi = wi,
                                                                                   wbc = wbc,
-                                                                                  skin = skin,
+                                                                                  skin = skin_i,
                                                                                   kh = kh,
                                                                                   length_uom = length_uom,
                                                                                   column_list = column_list)
 
             xyz = self.__get_xyz_for_interval(doing_xyz = doing_xyz,
                                               length_mode = length_mode,
                                               length_uom = length_uom,
@@ -1650,16 +1662,16 @@
                                                                    length_uom = length_uom,
                                                                    pc = pc,
                                                                    pc_titles = pc_titles,
                                                                    ci = ci)
 
             df = BlockedWell.__append_interval_data_to_dataframe(df = df,
                                                                  grid_name = grid_name,
-                                                                 radw = radw,
-                                                                 skin = skin,
+                                                                 radw = radw_i,
+                                                                 skin = skin_i,
                                                                  angla = angla,
                                                                  anglv = anglv,
                                                                  length = length,
                                                                  kh = kh,
                                                                  xyz = xyz,
                                                                  md = md,
                                                                  stat = stat,
@@ -1914,29 +1926,25 @@
 
     @staticmethod
     def __check_skin_stat_radw_to_be_added_as_properties(skin, stat, radw, column_list):
         """Verify whether skin should be added as a property in the dataframe."""
 
         if skin is not None and 'SKIN' not in column_list:
             column_list.append('SKIN')
-        if skin is None:
-            skin = 0.0
 
         if stat is not None:
             assert str(stat).upper() in ['ON', 'OFF']
             stat = str(stat).upper()
             if 'STAT' not in column_list:
                 column_list.append('STAT')
         else:
             stat = 'ON'
 
         if radw is not None and 'RADW' not in column_list:
             column_list.append('RADW')
-        if radw is None:
-            radw = 0.25
 
         return column_list, skin, stat, radw
 
     @staticmethod
     def __verify_perm_i_uuid_for_well_inflow(column_list, perm_i_uuid, pc_titles):
         # Verify that the I direction permeability has been specified if well inflow properties are to be added
         # to the dataframe.
@@ -2370,31 +2378,46 @@
                     l_j = length * maths.sqrt(k_e / k_j) * sine_anglv * sine_angla
                     l_k = length * maths.sqrt(k_e / k_k) * cosine_anglv
                     l_p = maths.sqrt(l_i * l_i + l_j * l_j + l_k * l_k)
                     kh = k_e * l_p
         return kh
 
     @staticmethod
-    def __get_pc_arrays_for_interval(pc, pc_titles, ci, length, radw, skin):
+    def __get_pc_arrays_for_interval(pc, pc_timeless, pc_titles, ci, length, radw, skin):
         """Get the property collection arrays for the interval."""
 
-        if 'LENGTH' in pc_titles:
-            length = pc.single_array_ref(citation_title = 'LENGTH')[ci]
-        if 'RADW' in pc_titles:
-            radw = pc.single_array_ref(citation_title = 'RADW')[ci]
-        assert radw > 0.0  # todo: allow zero for inactive intervals?
-        if 'SKIN' in pc_titles:
-            skin = pc.single_array_ref(citation_title = 'SKIN')[ci]
-        radb = wi = wbc = None
-        if 'RADB' in pc_titles:
-            radb = pc.single_array_ref(citation_title = 'RADB')[ci]
-        if 'WI' in pc_titles:
-            wi = pc.single_array_ref(citation_title = 'WI')[ci]
-        if 'WBC' in pc_titles:
-            wbc = pc.single_array_ref(citation_title = 'WBC')[ci]
+        def get_item(v, title, pc_titles, pc, pc_timeless, ci):
+
+            def pk_for_title(title):
+                d = {'RADW': 'wellbore radius', 'RADB': 'block equivalent radius', 'SKIN': 'skin'}
+                return d.get(title)
+
+            if title in pc_titles:
+                v = pc.single_array_ref(citation_title = title)[ci]
+            elif pc_timeless is not None:
+                a = pc_timeless.single_array_ref(citation_title = title)
+                if a is None:
+                    pk = pk_for_title(title)
+                    if pk is not None:
+                        a = pc_timeless.single_array_ref(property_kind = pk)
+                if a is not None:
+                    v = a[ci]
+            return v
+
+        length = get_item(length, 'LENGTH', pc_titles, pc, pc_timeless, ci)
+        radw = get_item(radw, 'RADW', pc_titles, pc, pc_timeless, ci)
+        assert radw is None or radw > 0.0  # todo: allow zero for inactive intervals?
+        skin = get_item(skin, 'SKIN', pc_titles, pc, pc_timeless, ci)
+        if skin is None:
+            skin = get_item(None, 'skin', pc_titles, pc, pc_timeless, ci)
+        radb = get_item(None, 'RADB', pc_titles, pc, pc_timeless, ci)
+        if radb is None:
+            radb = get_item(None, 'block equivalent radius', pc_titles, pc, pc_timeless, ci)
+        wi = get_item(None, 'WI', pc_titles, pc, pc_timeless, ci)
+        wbc = get_item(None, 'WBC', pc_titles, pc, pc_timeless, ci)
 
         return length, radw, skin, radb, wi, wbc
 
     @staticmethod
     def __get_well_inflow_parameters_for_interval(do_well_inflow, isotropic_perm, ntg_is_one, k_i, k_j, k_k, sine_anglv,
                                                   cosine_anglv, sine_angla, cosine_angla, grid, cell_kji0, radw, radb,
                                                   wi, wbc, skin, kh, length_uom, column_list):
@@ -2415,28 +2438,28 @@
 
             cell_axial_vectors = grid.interface_vectors_kji(cell_kji0)
             wam.convert_lengths(cell_axial_vectors[..., :2], grid.crs.xy_units, length_uom)
             wam.convert_lengths(cell_axial_vectors[..., 2], grid.crs.z_units, length_uom)
             d2 = np.empty(3)
             for axis in range(3):
                 d2[axis] = np.sum(cell_axial_vectors[axis] * cell_axial_vectors[axis])
-            radb_e = BlockedWell.__calculate_radb_e(k_ei = k_ei,
-                                                    k_ej = k_ej,
-                                                    k_ek = k_ek,
-                                                    k_i = k_i,
-                                                    k_j = k_j,
-                                                    k_k = k_k,
-                                                    d2 = d2,
-                                                    sine_anglv = sine_anglv,
-                                                    cosine_anglv = cosine_anglv,
-                                                    sine_angla = sine_angla,
-                                                    cosine_angla = cosine_angla)
-
             if radb is None:
+                radb_e = BlockedWell.__calculate_radb_e(k_ei = k_ei,
+                                                        k_ej = k_ej,
+                                                        k_ek = k_ek,
+                                                        k_i = k_i,
+                                                        k_j = k_j,
+                                                        k_k = k_k,
+                                                        d2 = d2,
+                                                        sine_anglv = sine_anglv,
+                                                        cosine_anglv = cosine_anglv,
+                                                        sine_angla = sine_angla,
+                                                        cosine_angla = cosine_angla)
                 radb = radw * radb_e / radw_e
+                log.debug(f'RADB value calculated in BlockedWell dataframe method as: {radb}')
             if wi is None:
                 wi = 0.0 if radb <= 0.0 else 2.0 * maths.pi / (maths.log(radb / radw) + skin)
             if 'WBC' in column_list and wbc is None:
                 assert length_uom == 'm' or length_uom.startswith('ft'),  \
                     'WBC only calculable for length uom of m or ft*'
                 conversion_constant = 8.5270171e-5 if length_uom == 'm' else 0.006328286
                 wbc = conversion_constant * kh * wi  # note: pperf aleady accounted for in kh
@@ -3344,15 +3367,14 @@
         # add the newly created BlockedWell object's root node as a part in the model and add reciprocal relationships
 
         if add_as_part:
             self.model.add_part('obj_BlockedWellboreRepresentation', self.uuid, bw_node)
             if add_relationships:
                 self.model.create_reciprocal_relationship(bw_node, 'destinationObject', self.trajectory.root,
                                                           'sourceObject')
-
                 for grid in self.grid_list:
                     self.model.create_reciprocal_relationship(bw_node, 'destinationObject', grid.root, 'sourceObject')
                 if interp_root is not None:
                     self.model.create_reciprocal_relationship(bw_node, 'destinationObject', interp_root, 'sourceObject')
                 ext_part = rqet.part_name_for_object('obj_EpcExternalPartReference', ext_uuid, prefixed = False)
                 ext_node = self.model.root_for_part(ext_part)
                 self.model.create_reciprocal_relationship(bw_node, 'mlToExternalPartProxy', ext_node,
@@ -3397,31 +3419,33 @@
         part_list = [self.model.part_for_uuid(uuid) for uuid in uuid_list]
 
         assert len(self.grid_list) == 1, "only blocked wells with a single grid can be handled currently"
         grid = self.grid_list[0]
         # filter to only those properties on the grid
         parts = self.model.parts_list_filtered_by_supporting_uuid(part_list, grid.uuid)
         if len(parts) < len(uuid_list):
-            log.warning(f"{len(uuid_list)-len(parts)} uuids ignored as they do not belong to the same grid as the gcs")
+            log.warning(
+                f"{len(uuid_list)-len(parts)} uuids ignored as they do not belong to the same grid as the blocked well")
 
         gridpc = grid.extract_property_collection()
         # only 'cell' properties are handled
         cell_parts = [part for part in parts if gridpc.indexable_for_part(part) == 'cells']
         if len(cell_parts) < len(parts):
-            log.warning(f"{len(parts)-len(cell_parts)} uuids ignored as they do not have indexableelement of cells")
+            log.warning(f"{len(parts)-len(cell_parts)} uuids ignored as they do not have indexable element of cells")
 
         if len(cell_parts) > 0:
             bwpc = rqp.PropertyCollection(support = self)
             if len(gridpc.time_series_uuid_list()) > 0:
-                time_dict = {
-                }  # Dictionary with keys for time_series uuids and None for static properties. Values for each key are a list of property parts associated with that time_series_uuid, or None
+                # dictionary with keys for time_series uuids and None for static properties
+                # values for each key are a list of property parts associated with that time_series_uuid, or None
+                time_dict = {}
                 for part in cell_parts:
                     if gridpc.time_series_uuid_for_part(part) in time_dict.keys():
-                        time_dict[gridpc.time_series_uuid_for_part(
-                            part)] = time_dict[gridpc.time_series_uuid_for_part(part)] + [part]
+                        time_dict[gridpc.time_series_uuid_for_part(part)] =  \
+                            time_dict[gridpc.time_series_uuid_for_part(part)] + [part]
                     else:
                         time_dict[gridpc.time_series_uuid_for_part(part)] = [part]
             else:
                 time_dict = {None: cell_parts}
 
             for time_uuid in time_dict.keys():
                 parts = time_dict[time_uuid]
```

### Comparing `resqpy-4.7.4/resqpy/well/_deviation_survey.py` & `resqpy-4.7.5/resqpy/well/_deviation_survey.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/_md_datum.py` & `resqpy-4.7.5/resqpy/well/_md_datum.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/_trajectory.py` & `resqpy-4.7.5/resqpy/well/_trajectory.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/_wellbore_frame.py` & `resqpy-4.7.5/resqpy/well/_wellbore_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/_wellbore_marker.py` & `resqpy-4.7.5/resqpy/well/_wellbore_marker.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/_wellbore_marker_frame.py` & `resqpy-4.7.5/resqpy/well/_wellbore_marker_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/blocked_well_frame.py` & `resqpy-4.7.5/resqpy/well/blocked_well_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/well_object_funcs.py` & `resqpy-4.7.5/resqpy/well/well_object_funcs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/resqpy/well/well_utils.py` & `resqpy-4.7.5/resqpy/well/well_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.4/PKG-INFO` & `resqpy-4.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resqpy
-Version: 4.7.4
+Version: 4.7.5
 Summary: Python API for working with RESQML models
 Home-page: https://github.com/bp/resqpy
 License: MIT
 Keywords: RESQML
 Author: BP
 Requires-Python: >=3.8.1,<3.11
 Classifier: Development Status :: 5 - Production/Stable
```

