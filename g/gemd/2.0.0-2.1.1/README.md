# Comparing `tmp/gemd-2.0.0.tar.gz` & `tmp/gemd-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemd-2.0.0.tar", last modified: Tue Feb  6 17:45:55 2024, max compression
+gzip compressed data, was "gemd-2.1.1.tar", last modified: Wed Apr 17 18:09:26 2024, max compression
```

## Comparing `gemd-2.0.0.tar` & `gemd-2.1.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.887964 gemd-2.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-02-06 17:44:38.000000 gemd-2.0.0/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)      923 2024-02-06 17:45:55.887964 gemd-2.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      656 2024-02-06 17:44:38.000000 gemd-2.0.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.843961 gemd-2.0.0/gemd/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/__version__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.847962 gemd-2.0.0/gemd/builders/
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/builders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14906 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/builders/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.851962 gemd-2.0.0/gemd/demo/
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38921 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/cake.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4689 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/material_run_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/measurement_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)  1541363 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/strehlow_and_cook.pif
--rw-rw-r--   0 travis    (2000) travis    (2000)    19951 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/strehlow_and_cook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   235566 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/strehlow_and_cook_small.pif
--rw-rw-r--   0 travis    (2000) travis    (2000)      996 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/table_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26784 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/demo/toothpick.jpg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.855962 gemd-2.0.0/gemd/entity/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1591 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.859962 gemd-2.0.0/gemd/entity/attribute/
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/attribute/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4712 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/attribute/base_attribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1342 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/attribute/condition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/attribute/parameter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/attribute/property.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2577 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/attribute/property_and_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8895 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/base_entity.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.863963 gemd-2.0.0/gemd/entity/bounds/
--rw-rw-r--   0 travis    (2000) travis    (2000)      407 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/bounds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2650 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/bounds/base_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5128 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/bounds/categorical_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5247 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/bounds/composition_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5768 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/bounds/integer_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3872 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/bounds/molecular_structure_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7709 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/bounds/real_bounds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1271 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/bounds_validation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6326 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/case_insensitive_dict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7173 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/dict_serializable.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      780 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/file_link.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/has_dependencies.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2598 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/link_by_uid.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.867963 gemd-2.0.0/gemd/entity/object/
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2589 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/base_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1533 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      918 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_material.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1536 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      902 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_process.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_properties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_quantities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      802 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1805 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1582 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4290 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/has_template_check_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7271 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/ingredient_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5967 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/ingredient_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4596 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/material_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5540 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/material_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/measurement_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3082 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/measurement_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4614 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/process_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4730 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/object/process_spec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/setters.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.871963 gemd-2.0.0/gemd/entity/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/source/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/source/performed_source.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.871963 gemd-2.0.0/gemd/entity/template/
--rw-rw-r--   0 travis    (2000) travis    (2000)      495 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/attribute_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3322 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/base_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/condition_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/has_condition_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/has_parameter_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4127 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/has_property_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1932 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/material_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/measurement_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1006 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/parameter_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3887 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/process_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1000 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/template/property_template.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4037 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5686 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/valid_list.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.879964 gemd-2.0.0/gemd/entity/value/
--rw-rw-r--   0 travis    (2000) travis    (2000)      759 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      744 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/base_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      736 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/categorical_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      624 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/composition_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1556 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/continuous_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2263 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/discrete_categorical.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/empirical_formula.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1715 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/inchi_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      642 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/integer_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      664 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/molecular_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1282 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/nominal_categorical.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/nominal_composition.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1485 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/nominal_integer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/nominal_real.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/normal_real.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1360 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/smiles_value.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2907 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/uniform_integer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1712 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/entity/value/uniform_real.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.879964 gemd-2.0.0/gemd/enumeration/
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/enumeration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5108 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/enumeration/base_enumeration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      390 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/enumeration/origin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/enumeration/sample_type.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.879964 gemd-2.0.0/gemd/json/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/json/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      501 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/json/gemd_encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7922 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/json/gemd_json.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.883964 gemd-2.0.0/gemd/units/
--rw-rw-r--   0 travis    (2000) travis    (2000)      346 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/units/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35636 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/units/citrine_en.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6701 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/units/constants_en.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    13542 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/units/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.883964 gemd-2.0.0/gemd/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17810 2024-02-06 17:44:38.000000 gemd-2.0.0/gemd/util/impl.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.883964 gemd-2.0.0/gemd.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      923 2024-02-06 17:45:55.000000 gemd-2.0.0/gemd.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3627 2024-02-06 17:45:55.000000 gemd-2.0.0/gemd.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-02-06 17:45:55.000000 gemd-2.0.0/gemd.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      153 2024-02-06 17:45:55.000000 gemd-2.0.0/gemd.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-02-06 17:45:55.000000 gemd-2.0.0/gemd.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-02-06 17:45:55.887964 gemd-2.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1910 2024-02-06 17:44:38.000000 gemd-2.0.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-02-06 17:45:55.883964 gemd-2.0.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6320 2024-02-06 17:44:38.000000 gemd-2.0.0/tests/test_examples.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.441172 gemd-2.1.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-04-17 18:08:09.000000 gemd-2.1.1/LICENSE
+-rw-r--r--   0 travis    (2000) travis    (2000)     1007 2024-04-17 18:09:26.437172 gemd-2.1.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      656 2024-04-17 18:08:09.000000 gemd-2.1.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.333165 gemd-2.1.1/gemd/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/__version__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.341165 gemd-2.1.1/gemd/builders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      224 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/builders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14906 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/builders/impl.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.357166 gemd-2.1.1/gemd/demo/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38891 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/cake.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4689 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/material_run_example.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2407 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/measurement_example.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1541363 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/strehlow_and_cook.pif
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19946 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/strehlow_and_cook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   235566 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/strehlow_and_cook_small.pif
+-rw-rw-r--   0 travis    (2000) travis    (2000)      996 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/table_example.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26784 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/demo/toothpick.jpg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.365167 gemd-2.1.1/gemd/entity/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1591 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.369167 gemd-2.1.1/gemd/entity/attribute/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      271 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4712 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/base_attribute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1342 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/condition.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1443 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/parameter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/property.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2577 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/attribute/property_and_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8895 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/base_entity.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.377168 gemd-2.1.1/gemd/entity/bounds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      407 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2650 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/base_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5128 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/categorical_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5247 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/composition_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5768 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/integer_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3872 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/molecular_structure_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7709 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds/real_bounds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1271 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/bounds_validation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6326 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/case_insensitive_dict.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7173 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/dict_serializable.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      780 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/file_link.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/has_dependencies.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2598 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/link_by_uid.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.393169 gemd-2.1.1/gemd/entity/object/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2589 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/base_object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1533 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      918 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_material.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1536 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      902 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_process.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_properties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_quantities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      802 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1805 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1582 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4290 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/has_template_check_generator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7271 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/ingredient_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5967 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/ingredient_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4596 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/material_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5540 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/material_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4882 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/measurement_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3082 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/measurement_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4614 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/process_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4730 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/object/process_spec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/setters.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.393169 gemd-2.1.1/gemd/entity/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       92 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/source/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1468 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/source/performed_source.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.401170 gemd-2.1.1/gemd/entity/template/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      495 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/attribute_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3322 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/base_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1004 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/condition_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/has_condition_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/has_parameter_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4127 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/has_property_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1932 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/material_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/measurement_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1006 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/parameter_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3887 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/process_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1000 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/template/property_template.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4037 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5686 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/valid_list.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.417171 gemd-2.1.1/gemd/entity/value/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      759 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      744 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/base_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      736 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/categorical_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      624 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/composition_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1556 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/continuous_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2263 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/discrete_categorical.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/empirical_formula.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1715 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/inchi_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      642 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/integer_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      664 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/molecular_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1282 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/nominal_categorical.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1906 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/nominal_composition.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1485 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/nominal_integer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1306 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/nominal_real.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/normal_real.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1360 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/smiles_value.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2907 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/uniform_integer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1712 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/entity/value/uniform_real.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.421171 gemd-2.1.1/gemd/enumeration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      114 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/enumeration/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5108 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/enumeration/base_enumeration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      390 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/enumeration/origin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      353 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/enumeration/sample_type.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.425171 gemd-2.1.1/gemd/json/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/json/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      501 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/json/gemd_encoder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7922 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/json/gemd_json.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.425171 gemd-2.1.1/gemd/units/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      346 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/units/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35636 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/units/citrine_en.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6701 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/units/constants_en.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15746 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/units/impl.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.429172 gemd-2.1.1/gemd/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      392 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17810 2024-04-17 18:08:09.000000 gemd-2.1.1/gemd/util/impl.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.429172 gemd-2.1.1/gemd.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     1007 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3627 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      207 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-17 18:09:26.000000 gemd-2.1.1/gemd.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-04-17 18:09:26.441172 gemd-2.1.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1990 2024-04-17 18:08:09.000000 gemd-2.1.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-17 18:09:26.429172 gemd-2.1.1/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6320 2024-04-17 18:08:09.000000 gemd-2.1.1/tests/test_examples.py
```

### Comparing `gemd-2.0.0/LICENSE` & `gemd-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/PKG-INFO` & `gemd-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: gemd
-Version: 2.0.0
+Version: 2.1.1
 Summary: Python binding for Citrine's GEMD data model
 Home-page: http://github.com/CitrineInformatics/gemd-python
 Author: Citrine Informatics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pint<0.24,>=0.20
 Requires-Dist: deprecation<3,>=2.1.0
+Requires-Dist: typing_extensions<5,>=4.8
+Requires-Dist: importlib-resources<7,>=5.3
 Provides-Extra: tests
 Requires-Dist: pytest<9,>=8.0.0; extra == "tests"
 Provides-Extra: tests-demo
 Requires-Dist: pandas<3,>=2.0.3; extra == "tests-demo"
 Provides-Extra: tests-entity-bounds
 Requires-Dist: numpy<2,>=1.24.4; extra == "tests-entity-bounds"
 Requires-Dist: pandas<3,>=2.0.3; extra == "tests-entity-bounds"
```

### Comparing `gemd-2.0.0/README.md` & `gemd-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/__init__.py` & `gemd-2.1.1/gemd/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/builders/impl.py` & `gemd-2.1.1/gemd/builders/impl.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/demo/cake.py` & `gemd-2.1.1/gemd/demo/cake.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Bake a cake."""
+from importlib_resources import files
 from io import BytesIO
 import random
 
 from gemd.entity.attribute import Condition, Parameter, Property, PropertyAndConditions
 from gemd.entity.base_entity import BaseEntity
 from gemd.entity.bounds import IntegerBounds, RealBounds, CategoricalBounds, CompositionBounds, \
     MolecularStructureBounds
@@ -63,18 +64,15 @@
 def get_template_scope():
     """Return the value of the DEMO_SCOPE variable."""
     return TEMPLATE_SCOPE
 
 
 def import_toothpick_picture() -> BytesIO:
     """Return the stream of the toothpick picture."""
-    from importlib.resources import read_binary
-    resource = read_binary("gemd.demo", "toothpick.jpg")
-
-    return BytesIO(resource)
+    return files("gemd.demo").joinpath("toothpick.jpg").open("rb")
 
 
 def make_cake_templates():
     """Define all templates independently, as in the wild this will be an independent operation."""
     tmpl = dict()
 
     # Attributes
```

### Comparing `gemd-2.0.0/gemd/demo/material_run_example.py` & `gemd-2.1.1/gemd/demo/material_run_example.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/demo/measurement_example.py` & `gemd-2.1.1/gemd/demo/measurement_example.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/demo/strehlow_and_cook.pif` & `gemd-2.1.1/gemd/demo/strehlow_and_cook.pif`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/demo/strehlow_and_cook.py` & `gemd-2.1.1/gemd/demo/strehlow_and_cook.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,18 @@
     "import_table", "minimal_subset", "make_templates", "make_strehlow_objects",
     "make_strehlow_table", "make_display_table"
 ]
 
 
 def import_table(filename=SMALL_TABLE):
     """Return the deserialized JSON table."""
-    from importlib.resources import read_text
+    from importlib_resources import files
     import json
-    table = json.loads(read_text("gemd.demo", filename))
 
-    return table
+    return json.loads(files("gemd.demo").joinpath(filename).read_text())
 
 
 def _fingerprint(row):
     """Generate a string-based fingerprint to characterize row diversity."""
     return ''.join(map(lambda x: str(type(x)), row))
```

### Comparing `gemd-2.0.0/gemd/demo/strehlow_and_cook_small.pif` & `gemd-2.1.1/gemd/demo/strehlow_and_cook_small.pif`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/demo/table_example.py` & `gemd-2.1.1/gemd/demo/table_example.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/demo/toothpick.jpg` & `gemd-2.1.1/gemd/demo/toothpick.jpg`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/__init__.py` & `gemd-2.1.1/gemd/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/attribute/base_attribute.py` & `gemd-2.1.1/gemd/entity/attribute/base_attribute.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/attribute/condition.py` & `gemd-2.1.1/gemd/entity/attribute/condition.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/attribute/parameter.py` & `gemd-2.1.1/gemd/entity/attribute/parameter.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/attribute/property.py` & `gemd-2.1.1/gemd/entity/attribute/property.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/attribute/property_and_conditions.py` & `gemd-2.1.1/gemd/entity/attribute/property_and_conditions.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/base_entity.py` & `gemd-2.1.1/gemd/entity/base_entity.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/bounds/base_bounds.py` & `gemd-2.1.1/gemd/entity/bounds/base_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/bounds/categorical_bounds.py` & `gemd-2.1.1/gemd/entity/bounds/categorical_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/bounds/composition_bounds.py` & `gemd-2.1.1/gemd/entity/bounds/composition_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/bounds/integer_bounds.py` & `gemd-2.1.1/gemd/entity/bounds/integer_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/bounds/molecular_structure_bounds.py` & `gemd-2.1.1/gemd/entity/bounds/molecular_structure_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/bounds/real_bounds.py` & `gemd-2.1.1/gemd/entity/bounds/real_bounds.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/bounds_validation.py` & `gemd-2.1.1/gemd/entity/bounds_validation.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/case_insensitive_dict.py` & `gemd-2.1.1/gemd/entity/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/dict_serializable.py` & `gemd-2.1.1/gemd/entity/dict_serializable.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/file_link.py` & `gemd-2.1.1/gemd/entity/file_link.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/has_dependencies.py` & `gemd-2.1.1/gemd/entity/has_dependencies.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/link_by_uid.py` & `gemd-2.1.1/gemd/entity/link_by_uid.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/__init__.py` & `gemd-2.1.1/gemd/entity/object/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/base_object.py` & `gemd-2.1.1/gemd/entity/object/base_object.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_conditions.py` & `gemd-2.1.1/gemd/entity/object/has_conditions.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_material.py` & `gemd-2.1.1/gemd/entity/object/has_material.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_parameters.py` & `gemd-2.1.1/gemd/entity/object/has_parameters.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_process.py` & `gemd-2.1.1/gemd/entity/object/has_process.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_properties.py` & `gemd-2.1.1/gemd/entity/object/has_properties.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_quantities.py` & `gemd-2.1.1/gemd/entity/object/has_quantities.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_source.py` & `gemd-2.1.1/gemd/entity/object/has_source.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_spec.py` & `gemd-2.1.1/gemd/entity/object/has_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_template.py` & `gemd-2.1.1/gemd/entity/object/has_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/has_template_check_generator.py` & `gemd-2.1.1/gemd/entity/object/has_template_check_generator.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/ingredient_run.py` & `gemd-2.1.1/gemd/entity/object/ingredient_run.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/ingredient_spec.py` & `gemd-2.1.1/gemd/entity/object/ingredient_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/material_run.py` & `gemd-2.1.1/gemd/entity/object/material_run.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/material_spec.py` & `gemd-2.1.1/gemd/entity/object/material_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/measurement_run.py` & `gemd-2.1.1/gemd/entity/object/measurement_run.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/measurement_spec.py` & `gemd-2.1.1/gemd/entity/object/measurement_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/process_run.py` & `gemd-2.1.1/gemd/entity/object/process_run.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/object/process_spec.py` & `gemd-2.1.1/gemd/entity/object/process_spec.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/setters.py` & `gemd-2.1.1/gemd/entity/setters.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/source/performed_source.py` & `gemd-2.1.1/gemd/entity/source/performed_source.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/attribute_template.py` & `gemd-2.1.1/gemd/entity/template/attribute_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/base_template.py` & `gemd-2.1.1/gemd/entity/template/base_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/condition_template.py` & `gemd-2.1.1/gemd/entity/template/condition_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/has_condition_templates.py` & `gemd-2.1.1/gemd/entity/template/has_condition_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/has_parameter_templates.py` & `gemd-2.1.1/gemd/entity/template/has_parameter_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/has_property_templates.py` & `gemd-2.1.1/gemd/entity/template/has_property_templates.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/material_template.py` & `gemd-2.1.1/gemd/entity/template/material_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/measurement_template.py` & `gemd-2.1.1/gemd/entity/template/measurement_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/parameter_template.py` & `gemd-2.1.1/gemd/entity/template/parameter_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/process_template.py` & `gemd-2.1.1/gemd/entity/template/process_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/template/property_template.py` & `gemd-2.1.1/gemd/entity/template/property_template.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/util.py` & `gemd-2.1.1/gemd/entity/util.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/valid_list.py` & `gemd-2.1.1/gemd/entity/valid_list.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/__init__.py` & `gemd-2.1.1/gemd/entity/value/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/base_value.py` & `gemd-2.1.1/gemd/entity/value/base_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/categorical_value.py` & `gemd-2.1.1/gemd/entity/value/categorical_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/composition_value.py` & `gemd-2.1.1/gemd/entity/value/composition_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/continuous_value.py` & `gemd-2.1.1/gemd/entity/value/continuous_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/discrete_categorical.py` & `gemd-2.1.1/gemd/entity/value/discrete_categorical.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/empirical_formula.py` & `gemd-2.1.1/gemd/entity/value/empirical_formula.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/inchi_value.py` & `gemd-2.1.1/gemd/entity/value/inchi_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/integer_value.py` & `gemd-2.1.1/gemd/entity/value/integer_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/molecular_value.py` & `gemd-2.1.1/gemd/entity/value/molecular_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/nominal_categorical.py` & `gemd-2.1.1/gemd/entity/value/nominal_categorical.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/nominal_composition.py` & `gemd-2.1.1/gemd/entity/value/nominal_composition.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/nominal_integer.py` & `gemd-2.1.1/gemd/entity/value/nominal_integer.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/nominal_real.py` & `gemd-2.1.1/gemd/entity/value/nominal_real.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/normal_real.py` & `gemd-2.1.1/gemd/entity/value/normal_real.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/smiles_value.py` & `gemd-2.1.1/gemd/entity/value/smiles_value.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/uniform_integer.py` & `gemd-2.1.1/gemd/entity/value/uniform_integer.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/entity/value/uniform_real.py` & `gemd-2.1.1/gemd/entity/value/uniform_real.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/enumeration/base_enumeration.py` & `gemd-2.1.1/gemd/enumeration/base_enumeration.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/json/__init__.py` & `gemd-2.1.1/gemd/json/__init__.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/json/gemd_json.py` & `gemd-2.1.1/gemd/json/gemd_json.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/units/citrine_en.txt` & `gemd-2.1.1/gemd/units/citrine_en.txt`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/units/constants_en.txt` & `gemd-2.1.1/gemd/units/constants_en.txt`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd/units/impl.py` & `gemd-2.1.1/gemd/units/impl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Implementation of units."""
+from deprecation import deprecated
 import functools
-from importlib.resources import read_text
+from importlib_resources import files
 import os
 from pathlib import Path
 import re
 from tempfile import TemporaryDirectory
 from typing import Union, List, Tuple, Generator, Any
 
-from pint import UnitRegistry, Unit, register_unit_format
+from pint import UnitRegistry, register_unit_format
 try:  # Pint 0.23 migrated the location of this method, and augmented it
     from pint.pint_eval import tokenizer
 except ImportError:  # pragma: no cover
     from pint.compat import tokenizer
 from tokenize import NAME, NUMBER, OP, ERRORTOKEN, TokenInfo
 # alias the error that is thrown when units are incompatible
 # this helps to isolate the dependence on pint
@@ -23,26 +24,27 @@
 
 __all__ = [
     "parse_units", "convert_units", "get_base_units", "change_definitions_file",
     "UndefinedUnitError", "IncompatibleUnitsError", "DefinitionSyntaxError"
 ]
 
 
-def _deploy_default_files() -> str:
+def _deploy_default_files() -> Tuple[Path, Path]:
     """Copy the units & constants file into a temporary directory."""
-    units_path = Path(_TEMP_DIRECTORY.name) / "citrine_en.txt"
-    units_path.write_text(read_text("gemd.units", "citrine_en.txt"), encoding="utf-8")
+    resources = files("gemd.units")
+    target_dir = Path(_TEMP_DIRECTORY.name)
+    target_paths = tuple(target_dir / f for f in ("citrine_en.txt", "constants_en.txt"))
+    for target in target_paths:
+        source = resources.joinpath(target.name)
+        target.write_text(source.read_text(), encoding="utf-8")
 
-    constants_path = Path(_TEMP_DIRECTORY.name) / "constants_en.txt"
-    constants_path.write_text(read_text("gemd.units", "constants_en.txt"), encoding="utf-8")
+    return target_paths
 
-    return str(units_path)
 
-
-DEFAULT_FILE = _deploy_default_files()
+DEFAULT_FILE, DEFAULT_CONSTANTS = _deploy_default_files()
 _ALLOWED_OPERATORS = {".", "+", "-", "*", "/", "//", "^", "**", "(", ")"}
 
 
 def _space_after_minus_preprocessor(input_string: str) -> str:
     """A preprocessor that protects against a pint < 0.21 bug."""
     return re.sub(r"(?<=-)\s+(?=\d)", "", input_string)
 
@@ -127,14 +129,15 @@
     Takes the input_string and the blocks output by _scaling_find_blocks and
     returns a tuple of the substrings that contain scaling factors, the scaling
     factor itself, and the unit string.
 
     """
     todo = []
     for block in blocks:
+        # Note: while Python does not recognize ^ as exponentiation, pint does
         i_exp = next((i for i, t in enumerate(block) if t.string in {"**", "^"}), len(block))
         i_name = next((i for i, t in enumerate(block) if t.type == NAME), None)
         numbers = [(i, t.string) for i, t in enumerate(block) if t.type == NUMBER and i < i_exp]
 
         if len(numbers) == 1:
             position, value = numbers[0]
             if i_exp != len(block):
@@ -164,18 +167,22 @@
 
     Takes the terms to be updated, and actually updates the input_string as well as
     creating an entry for each in the registry.
 
     """
     for scaled_term, number_string, unit_string in todo:
         regex = rf"(?<![-+0-9.]){re.escape(scaled_term)}(?![0-9.])"
-        stripped = re.sub(r"[+\s]+", "", scaled_term).replace("--", "")
+        stripped = re.sub(
+            r"(?<=\d)_(?=\d)", "", re.sub(r"[+\s]+", "", scaled_term).replace("--", "")
+        )
 
         if unit_string is not None:
-            stripped_unit = re.sub(r"[+\s]+", "", unit_string).replace("--", "")
+            stripped_unit = re.sub(
+                r"(?<!0)(?=\.)", "0", re.sub(r"[+\s]+", "", unit_string)
+            ).replace("--", "")
             long_unit = f"{_REGISTRY.parse_units(stripped_unit)}"
             short_unit = f"{_REGISTRY.parse_units(stripped_unit):~}"
             long = stripped.replace(stripped_unit, "_" + long_unit)
             short = stripped.replace(stripped_unit, " " + short_unit)
         else:
             long = stripped
             short = stripped
@@ -197,15 +204,66 @@
 
     blocks.pop(0)  # Leading term is not allowed to be a scaling factor
     todo = _scaling_identify_factors(input_string, blocks)
 
     return _scaling_store_and_mangle(input_string, todo)
 
 
-_REGISTRY: UnitRegistry = None  # global requires it be defined in this scope
+def _unmangle_scaling(input_string: str) -> str:
+    """Convert mangled scaling values into a pint-compatible expression."""
+    number_re = r'\b_(_)?(\d+)(_\d+)?([eE]_?\d+)?(_(?=[a-zA-Z]))?'
+    while match := re.search(number_re, input_string):
+        replacement = '' if match.group(1) is None else '-'
+        replacement += match.group(2)
+        replacement += '' if match.group(3) is None else match.group(3).replace('_', '.')
+        replacement += '' if match.group(4) is None else match.group(4).replace('_', '-')
+        replacement += '' if match.group(5) is None else match.group(5).replace('_', ' ')
+        input_string = input_string.replace(match.group(0), replacement)
+    return input_string
+
+
+try:  # pragma: no cover
+    # Pint 0.23 modified the preferred way to derive a custom class
+    # https://pint.readthedocs.io/en/0.23/advanced/custom-registry-class.html
+    from pint.registry import GenericUnitRegistry
+    from typing_extensions import TypeAlias
+
+    class _ScaleFactorUnit(UnitRegistry.Unit):
+        """Child class of Units for generating units w/ clean scaling factors."""
+
+        def __format__(self, format_spec):
+            result = super().__format__(format_spec)
+            return _unmangle_scaling(result)
+
+    class _ScaleFactorQuantity(UnitRegistry.Quantity):
+        """Child class of Quantity for generating units w/ clean scaling factors."""
+
+        pass
+
+    class _ScaleFactorRegistry(GenericUnitRegistry[_ScaleFactorQuantity, _ScaleFactorUnit]):
+        """UnitRegistry class that uses _GemdUnits."""
+
+        Quantity: TypeAlias = _ScaleFactorQuantity
+        Unit: TypeAlias = _ScaleFactorUnit
+
+except ImportError:  # pragma: no cover
+    # https://pint.readthedocs.io/en/0.21/advanced/custom-registry-class.html
+    class _ScaleFactorUnit(UnitRegistry.Unit):
+        """Child class of Units for generating units w/ clean scaling factors."""
+
+        def __format__(self, format_spec):
+            result = super().__format__(format_spec)
+            return _unmangle_scaling(result)
+
+    class _ScaleFactorRegistry(UnitRegistry):
+        """UnitRegistry class that uses _GemdUnits."""
+
+        _unit_class = _ScaleFactorUnit
+
+_REGISTRY: _ScaleFactorRegistry = None  # global requires it be defined in this scope
 
 
 @functools.lru_cache(maxsize=1024 * 1024)
 def convert_units(value: float, starting_unit: str, final_unit: str) -> float:
     """
     Convert the value from the starting_unit to the final_unit.
 
@@ -240,46 +298,31 @@
                 units2=final_unit,
                 dim2=_REGISTRY.get_dimensionality(resolved_final_unit)
             )
         return resolved_value.to(resolved_final_unit).magnitude
 
 
 @register_unit_format("clean")
+@deprecated(deprecated_in="2.1.0", removed_in="3.0.0", details="Scaling factor clean-up ")
 def _format_clean(unit, registry, **options):
-    """Formatter that turns scaling-factor-units into numbers again."""
-    numerator = []
-    denominator = []
-    for u, p in unit.items():
-        if re.match(r"_[\d_]+", u):
-            # Munged scaling factor; grab symbol, which is the prettier
-            u = registry.get_symbol(u)
-
-        if p == 1:
-            numerator.append(u)
-        elif p > 0:
-            numerator.append(f"{u} ** {p}")
-        elif p == -1:
-            denominator.append(u)
-        elif p < 0:
-            denominator.append(f"{u} ** {-p}")
+    """
+    DEPRECATED Formatter that turns scaling-factor-units into numbers again.
 
-    if len(numerator) == 0:
-        numerator = ["1"]
+    Responsibility for this piece of clean-up has been shifted to a custom class.
 
-    if len(denominator) > 0:
-        return " / ".join((" * ".join(numerator), " / ".join(denominator)))
-    else:
-        return " * ".join(numerator)
+    """
+    from pint.formatting import _FORMATTERS
+    return _FORMATTERS["D"](unit, registry, **options)
 
 
 @functools.lru_cache(maxsize=1024)
-def parse_units(units: Union[str, Unit, None],
+def parse_units(units: Union[str, UnitRegistry.Unit, None],
                 *,
                 return_unit: bool = False
-                ) -> Union[str, Unit, None]:
+                ) -> Union[str, UnitRegistry.Unit, None]:
     """
     Parse a string or Unit into a standard string representation of the unit.
 
     Parameters
     ----------
     units: str, Unit, or None
         The string or Unit representation of the object we wish to display
@@ -294,27 +337,28 @@
     """
     if units is None:
         if return_unit:
             return _REGISTRY.parse_units("")
         else:
             return None
     elif isinstance(units, str):
-        parsed = _REGISTRY.parse_units(units)
+        # SPT-1311 Protect against leaked mangled strings
+        parsed = _REGISTRY.parse_units(_unmangle_scaling(units))
         if return_unit:
             return parsed
         else:
-            return f"{parsed:clean}"
-    elif isinstance(units, Unit):
+            return f"{parsed}"
+    elif isinstance(units, UnitRegistry.Unit):
         return units
     else:
         raise UndefinedUnitError("Units must be given as a recognized unit string or Units object")
 
 
 @functools.lru_cache(maxsize=1024)
-def get_base_units(units: Union[str, Unit]) -> Tuple[Unit, float, float]:
+def get_base_units(units: Union[str, UnitRegistry.Unit]) -> Tuple[UnitRegistry.Unit, float, float]:
     """
     Get the base units and conversion factors for the given unit.
 
     Parameters
     ----------
     units: str, Unit, or None
         The representation of the object we wish to display
@@ -346,27 +390,26 @@
     global _REGISTRY
     convert_units.cache_clear()  # Units will change
     parse_units.cache_clear()
     get_base_units.cache_clear()
     if filename is None:
         target = DEFAULT_FILE
     else:
-        # TODO: Handle case where user provides a units file but no constants file
         target = Path(filename).expanduser().resolve(strict=True)
 
     current_dir = Path.cwd()
     try:
-        path = Path(target)
-        os.chdir(path.parent)
-        # Need to re-verify path because of some slippiness around tmp on MacOS
-        _REGISTRY = UnitRegistry(filename=Path.cwd() / path.name,
-                                 preprocessors=[_space_after_minus_preprocessor,
-                                                _scientific_notation_preprocessor,
-                                                _scaling_preprocessor
-                                                ],
-                                 autoconvert_offset_to_baseunit=True
-                                 )
+        os.chdir(target.parent)
+        # Need to re-verify path because of some slippiness around tmp on macOS
+        updated = (Path.cwd() / target.name).resolve(strict=True)
+        _REGISTRY = _ScaleFactorRegistry(filename=updated,
+                                         preprocessors=[_space_after_minus_preprocessor,
+                                                        _scientific_notation_preprocessor,
+                                                        _scaling_preprocessor
+                                                        ],
+                                         autoconvert_offset_to_baseunit=True
+                                         )
     finally:
         os.chdir(current_dir)
 
 
 change_definitions_file()  # initialize to default
```

### Comparing `gemd-2.0.0/gemd/util/impl.py` & `gemd-2.1.1/gemd/util/impl.py`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/gemd.egg-info/PKG-INFO` & `gemd-2.1.1/gemd.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: gemd
-Version: 2.0.0
+Version: 2.1.1
 Summary: Python binding for Citrine's GEMD data model
 Home-page: http://github.com/CitrineInformatics/gemd-python
 Author: Citrine Informatics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pint<0.24,>=0.20
 Requires-Dist: deprecation<3,>=2.1.0
+Requires-Dist: typing_extensions<5,>=4.8
+Requires-Dist: importlib-resources<7,>=5.3
 Provides-Extra: tests
 Requires-Dist: pytest<9,>=8.0.0; extra == "tests"
 Provides-Extra: tests-demo
 Requires-Dist: pandas<3,>=2.0.3; extra == "tests-demo"
 Provides-Extra: tests-entity-bounds
 Requires-Dist: numpy<2,>=1.24.4; extra == "tests-entity-bounds"
 Requires-Dist: pandas<3,>=2.0.3; extra == "tests-entity-bounds"
```

### Comparing `gemd-2.0.0/gemd.egg-info/SOURCES.txt` & `gemd-2.1.1/gemd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemd-2.0.0/setup.py` & `gemd-2.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,17 @@
               'citrine_en.txt',
               'constants_en.txt',
           ],
           'tests.units': ['test_units.txt']
       },
       install_requires=[
           "pint>=0.20,<0.24",
-          "deprecation>=2.1.0,<3"
+          "deprecation>=2.1.0,<3",
+          "typing_extensions>=4.8,<5",
+          "importlib-resources>=5.3,<7"
       ],
       extras_require={
           "tests": [
               "pytest>=8.0.0,<9"
           ],
           "tests.demo": [
               "pandas>=2.0.3,<3"
```

### Comparing `gemd-2.0.0/tests/test_examples.py` & `gemd-2.1.1/tests/test_examples.py`

 * *Files identical despite different names*

