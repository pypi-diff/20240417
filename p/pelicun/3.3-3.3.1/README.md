# Comparing `tmp/pelicun-3.3.tar.gz` & `tmp/pelicun-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelicun-3.3.tar", last modified: Sat Mar 30 00:50:51 2024, max compression
+gzip compressed data, was "pelicun-3.3.1.tar", last modified: Wed Apr 17 00:41:14 2024, max compression
```

## Comparing `pelicun-3.3.tar` & `pelicun-3.3.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-30 00:50:42.000000 pelicun-3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-30 00:50:42.000000 pelicun-3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21819 2024-03-30 00:50:51.431433 pelicun-3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-03-30 00:50:42.000000 pelicun-3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.403432 pelicun-3.3/pelicun/
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/assessment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    38835 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   104242 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.399432 pelicun-3.3/pelicun/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.407432 pelicun-3.3/pelicun/examples/001/
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/001/CMP_QNT.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/001/demands_s4.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/001/input.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.407432 pelicun-3.3/pelicun/examples/002/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/002/CMP_QNT.csv
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/002/input.json
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/002/response.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.407432 pelicun-3.3/pelicun/examples/0_tmp/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/0_tmp/CMP_marginals.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/0_tmp/DMG_process_P58.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/0_tmp/LOSS_map.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/0_tmp/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/0_tmp/demands.csv
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/0_tmp/fragility_Additional.csv
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/examples/0_tmp/repair_Additional.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16427 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/file_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.407432 pelicun-3.3/pelicun/model/
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/model/asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    60323 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/model/damage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    33061 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/model/demand_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    40848 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/model/loss_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/model/pelicun_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.399432 pelicun-3.3/pelicun/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.423432 pelicun-3.3/pelicun/resources/SimCenterDBDL/
--rw-r--r--   0 runner    (1001) docker     (127)    80663 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1167069 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json
--rw-r--r--   0 runner    (1001) docker     (127)    36386 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv
--rw-r--r--   0 runner    (1001) docker     (127)   881431 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv
--rw-r--r--   0 runner    (1001) docker     (127)   183256 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv
--rw-r--r--   0 runner    (1001) docker     (127)    52505 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json
--rw-r--r--   0 runner    (1001) docker     (127)  3714342 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv
--rw-r--r--   0 runner    (1001) docker     (127)   521287 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1132502 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv
--rw-r--r--   0 runner    (1001) docker     (127)   262248 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204054 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json
--rw-r--r--   0 runner    (1001) docker     (127)  2118028 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.423432 pelicun-3.3/pelicun/resources/auto/
--rw-r--r--   0 runner    (1001) docker     (127)    30421 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/auto/Hazus_Earthquake_IM.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/resources/auto/Hazus_Earthquake_Story.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.427432 pelicun-3.3/pelicun/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/settings/default_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/settings/default_units.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.427432 pelicun-3.3/pelicun/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/code_repetition_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.403432 pelicun-3.3/pelicun/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.403432 pelicun-3.3/pelicun/tests/data/assessment/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.427432 pelicun-3.3/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/custom_units.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.403432 pelicun-3.3/pelicun/tests/data/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.427432 pelicun-3.3/pelicun/tests/data/base/test_parse_units/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/base/test_parse_units/additional_units_a.json
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/base/test_parse_units/duplicate.json
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/base/test_parse_units/duplicate2.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/base/test_parse_units/invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/base/test_parse_units/not_dict.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/base/test_parse_units/not_float.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.403432 pelicun-3.3/pelicun/tests/data/file_io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.427432 pelicun-3.3/pelicun/tests/data/file_io/test_load_data/
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/file_io/test_load_data/no_units.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/file_io/test_load_data/orient_1.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      445 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/file_io/test_load_data/orient_1_units.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/file_io/test_load_data/units.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.403432 pelicun-3.3/pelicun/tests/data/model/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tests/data/model/test_AssetModel/
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      317 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals_2.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals_block_weights.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_dir.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_loc.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/demand_sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/demand_sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/damage_model.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/
--rwxr-xr-x   0 runner    (1001) docker     (127)       75 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)      109 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/fragility_DB_test.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_estimate_RID/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_estimate_RID/demand_sample_A.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_load_sample/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_A.csv
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_B.csv
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_C.csv
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_D.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/reset_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/test_assessment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    26202 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    76806 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    46929 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/test_uq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.431433 pelicun-3.3/pelicun/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    70788 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tools/DL_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tools/HDF_to_CSV.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/tools/export_DB.py
--rw-r--r--   0 runner    (1001) docker     (127)    75896 2024-03-30 00:50:42.000000 pelicun-3.3/pelicun/uq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:50:51.407432 pelicun-3.3/pelicun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21819 2024-03-30 00:50:51.000000 pelicun-3.3/pelicun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-03-30 00:50:51.000000 pelicun-3.3/pelicun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 00:50:51.000000 pelicun-3.3/pelicun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-30 00:50:51.000000 pelicun-3.3/pelicun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-30 00:50:51.000000 pelicun-3.3/pelicun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-30 00:50:51.000000 pelicun-3.3/pelicun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 00:50:51.431433 pelicun-3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-30 00:50:42.000000 pelicun-3.3/setup.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.285605 pelicun-3.3.1/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1661 2022-12-05 20:30:08.000000 pelicun-3.3.1/LICENSE
+-rw-r--r--   0 adamzs     (504) staff       (20)      486 2024-04-04 20:31:52.000000 pelicun-3.3.1/MANIFEST.in
+-rw-r--r--   0 adamzs     (504) staff       (20)    21993 2024-04-17 00:41:14.285296 pelicun-3.3.1/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)    20703 2024-04-04 20:38:24.000000 pelicun-3.3.1/README.md
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.229905 pelicun-3.3.1/pelicun/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2012 2024-04-17 00:38:15.000000 pelicun-3.3.1/pelicun/__init__.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     7284 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/assessment.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     3684 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/auto.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    38835 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/base.py
+-rw-r--r--   0 adamzs     (504) staff       (20)   104242 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/db.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.222517 pelicun-3.3.1/pelicun/examples/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.233106 pelicun-3.3.1/pelicun/examples/001/
+-rw-r--r--   0 adamzs     (504) staff       (20)     5011 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/001/CMP_QNT.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    11827 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/001/demands_s4.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     2149 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/001/input.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.234636 pelicun-3.3.1/pelicun/examples/002/
+-rw-r--r--   0 adamzs     (504) staff       (20)      211 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/002/CMP_QNT.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      902 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/002/input.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     4139 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/002/response.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.236681 pelicun-3.3.1/pelicun/examples/0_tmp/
+-rw-r--r--   0 adamzs     (504) staff       (20)      652 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/CMP_marginals.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)       52 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/DMG_process_P58.json
+-rw-r--r--   0 adamzs     (504) staff       (20)      347 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/LOSS_map.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     2782 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/config.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     3892 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/demands.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      890 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/fragility_Additional.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      158 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/examples/0_tmp/repair_Additional.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    16427 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/file_io.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.239279 pelicun-3.3.1/pelicun/model/
+-rw-r--r--   0 adamzs     (504) staff       (20)     2010 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/__init__.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    15084 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/asset_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    60323 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/damage_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    33061 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/demand_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    40848 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/loss_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     8855 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/model/pelicun_model.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.222892 pelicun-3.3.1/pelicun/resources/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.264690 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/
+-rw-r--r--   0 adamzs     (504) staff       (20)    80663 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)  1167069 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json
+-rw-r--r--   0 adamzs     (504) staff       (20)    36386 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   881431 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     9616 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   183256 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     4297 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    52505 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     2203 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     3921 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)    18199 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json
+-rw-r--r--   0 adamzs     (504) staff       (20)  3714342 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   521287 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)  1132502 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     8934 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   262248 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     5912 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)   204054 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json
+-rw-r--r--   0 adamzs     (504) staff       (20)      302 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     3873 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json
+-rw-r--r--   0 adamzs     (504) staff       (20)  2118028 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.269271 pelicun-3.3.1/pelicun/resources/auto/
+-rw-r--r--   0 adamzs     (504) staff       (20)    30421 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/auto/Hazus_Earthquake_IM.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     9084 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/resources/auto/Hazus_Earthquake_Story.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.271753 pelicun-3.3.1/pelicun/settings/
+-rw-r--r--   0 adamzs     (504) staff       (20)      661 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/settings/default_config.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1610 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/settings/default_units.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.275332 pelicun-3.3.1/pelicun/tests/
+-rw-r--r--   0 adamzs     (504) staff       (20)     3113 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/code_repetition_checker.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.223707 pelicun-3.3.1/pelicun/tests/data/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.223307 pelicun-3.3.1/pelicun/tests/data/assessment/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.275686 pelicun-3.3.1/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/
+-rw-r--r--   0 adamzs     (504) staff       (20)       55 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/assessment/test_assessment_calc_unit_scale_factor/custom_units.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.223464 pelicun-3.3.1/pelicun/tests/data/base/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.277291 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/additional_units_a.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1547 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/duplicate.json
+-rw-r--r--   0 adamzs     (504) staff       (20)     1531 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/duplicate2.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       43 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/invalid.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       26 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/not_dict.json
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/not_float.json
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.223618 pelicun-3.3.1/pelicun/tests/data/file_io/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.278427 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/
+-rw-r--r--   0 adamzs     (504) staff       (20)     1537 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/no_units.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      372 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/orient_1.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      445 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/orient_1_units.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     1641 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/units.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.224472 pelicun-3.3.1/pelicun/tests/data/model/
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.279481 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      108 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      317 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals_2.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      125 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals_block_weights.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      116 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_dir.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      111 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_AssetModel/CMP_marginals_invalid_loc.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.279765 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/
+-rw-r--r--   0 adamzs     (504) staff       (20)      229 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel__evaluate_damage_state_and_prepare_dmg_quantities/demand_sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.280000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/
+-rw-r--r--   0 adamzs     (504) staff       (20)      208 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_assemble_required_demand_data/demand_sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.280215 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/
+-rw-r--r--   0 adamzs     (504) staff       (20)      237 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_calculate_multilinear_CDF/damage_model.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.281085 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/
+-rwxr-xr-x   0 adamzs     (504) staff       (20)       75 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals.csv
+-rwxr-xr-x   0 adamzs     (504) staff       (20)      109 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/CMP_marginals_2.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      249 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DamageModel_perform_dmg_task/fragility_DB_test.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.281313 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_estimate_RID/
+-rw-r--r--   0 adamzs     (504) staff       (20)       51 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_estimate_RID/demand_sample_A.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.281559 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/
+-rw-r--r--   0 adamzs     (504) staff       (20)      138 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_generate_sample_with_demand_cloning/sample.csv
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.282509 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/
+-rw-r--r--   0 adamzs     (504) staff       (20)      162 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_A.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_B.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_C.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)      152 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/data/model/test_DemandModel_load_sample/demand_sample_D.csv
+-rw-r--r--   0 adamzs     (504) staff       (20)     5729 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/reset_tests.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     5155 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_assessment.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     4416 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_auto.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    26202 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_base.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     7915 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_file_io.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    76806 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_model.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    46929 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/test_uq.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     3298 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tests/util.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.284158 pelicun-3.3.1/pelicun/tools/
+-rw-r--r--   0 adamzs     (504) staff       (20)    70920 2024-04-10 18:14:45.000000 pelicun-3.3.1/pelicun/tools/DL_calculation.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     2411 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tools/HDF_to_CSV.py
+-rw-r--r--   0 adamzs     (504) staff       (20)     3256 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/tools/export_DB.py
+-rw-r--r--   0 adamzs     (504) staff       (20)    75896 2024-04-04 20:31:52.000000 pelicun-3.3.1/pelicun/uq.py
+drwxr-xr-x   0 adamzs     (504) staff       (20)        0 2024-04-17 00:41:14.284778 pelicun-3.3.1/pelicun.egg-info/
+-rw-r--r--   0 adamzs     (504) staff       (20)    21993 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/PKG-INFO
+-rw-r--r--   0 adamzs     (504) staff       (20)     4829 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/SOURCES.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        1 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/dependency_links.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       62 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/entry_points.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       88 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/requires.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)        8 2024-04-17 00:41:14.000000 pelicun-3.3.1/pelicun.egg-info/top_level.txt
+-rw-r--r--   0 adamzs     (504) staff       (20)       38 2024-04-17 00:41:14.285674 pelicun-3.3.1/setup.cfg
+-rw-r--r--   0 adamzs     (504) staff       (20)     2161 2024-04-04 20:31:52.000000 pelicun-3.3.1/setup.py
```

### Comparing `pelicun-3.3/LICENSE` & `pelicun-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/PKG-INFO` & `pelicun-3.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelicun
-Version: 3.3
+Version: 3.3.1
 Summary: Probabilistic Estimation of Losses, Injuries, and Community resilience Under Natural hazard events
 Home-page: http://nheri-simcenter.github.io/pelicun/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
@@ -20,16 +20,21 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy<2.0,>=1.22.0
+Requires-Dist: scipy<2.0,>=1.7.0
+Requires-Dist: pandas<3.0,>=1.4.0
+Requires-Dist: tables>=3.7.0
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
 
 <p align="center">
 	<img src="https://raw.githubusercontent.com/NHERI-SimCenter/pelicun/gh-pages/doc_src/common/figures/pelicun-Logo-white.png"
 		alt="pelicun" align="middle" height="200"/>
 </p>
 
 <p align="center">
@@ -175,124 +180,124 @@
 
 - Dependencies
 
   - Ceiling raised for `pandas`, supporting version 2.0 and above up until 3.0.
 
 ### Changes in v3.2
 
-* Changes that might affect backwards compatibility:
+- Changes that might affect backwards compatibility:
 
-  * Unit information is included in every output file. If you parse Pelicun outputs and did not anticipate a Unit entry, your parser might need an update.
+  - Unit information is included in every output file. If you parse Pelicun outputs and did not anticipate a Unit entry, your parser might need an update.
   
-  * Decision variable types in the repair consequence outputs are named using CamelCase rather than all capitals to be consistent with other parts of the codebase. For example, we use "Cost" instead of "COST". This might affect post-processing scripts. 
+  - Decision variable types in the repair consequence outputs are named using CamelCase rather than all capitals to be consistent with other parts of the codebase. For example, we use "Cost" instead of "COST". This might affect post-processing scripts. 
   
-  * For clarity, "ea" units were replaced with "unitless" where appropriate. There should be no practical difference between the calculations due to this change. Interstory drift ratio demand types are one example.
+  - For clarity, "ea" units were replaced with "unitless" where appropriate. There should be no practical difference between the calculations due to this change. Interstory drift ratio demand types are one example.
     
-  * Weighted component block assignment is no longer supported. We recommend using more versatile multiple component definitions (see new feature below) to achieve the same effect.
+  - Weighted component block assignment is no longer supported. We recommend using more versatile multiple component definitions (see new feature below) to achieve the same effect.
     
-  * Damage functions (i.e., assign quantity of damage as a function of demand) are no longer supported. We recommend using the new multilinear CDF feature to develop theoretically equivalent, but more efficient models.
+  - Damage functions (i.e., assign quantity of damage as a function of demand) are no longer supported. We recommend using the new multilinear CDF feature to develop theoretically equivalent, but more efficient models.
 
-* New multilinear CDF Random Variable allows using the multilinear approximation of any CDF in the tool.
+- New multilinear CDF Random Variable allows using the multilinear approximation of any CDF in the tool.
 
-* Capacity adjustment allows adjusting (scaling or shifting) default capacities (i.e., fragility curves) with factors specific to each Performance Group.
+- Capacity adjustment allows adjusting (scaling or shifting) default capacities (i.e., fragility curves) with factors specific to each Performance Group.
 
-* Support for multiple definitions of the same component at the same location-direction. This feature facilitates adding components with different block sizes to the same floor or defining multiple tenants on the same floor, each with their own set of components.
+- Support for multiple definitions of the same component at the same location-direction. This feature facilitates adding components with different block sizes to the same floor or defining multiple tenants on the same floor, each with their own set of components.
 
-* Support for cloning demands, that is, taking a provided demand dataset, creating a copy and considering it as another demand. For example, you can provide results of seismic response in the X direction and automatically prepare a copy of them to represent results in the Y direction. 
+- Support for cloning demands, that is, taking a provided demand dataset, creating a copy and considering it as another demand. For example, you can provide results of seismic response in the X direction and automatically prepare a copy of them to represent results in the Y direction. 
 
-* Added a comprehensive suite of more than 140 unit tests that cover more than 93% of the codebase. Tests are automatically executed after every commit using GitHub Actions and coverage is monitored through `Codecov.io`. Badges at the top of the Readme show the status of tests and coverage. We hope this continuous integration facilitates editing and extending the existing codebase for interested members of the community.
+- Added a comprehensive suite of more than 140 unit tests that cover more than 93% of the codebase. Tests are automatically executed after every commit using GitHub Actions and coverage is monitored through `Codecov.io`. Badges at the top of the Readme show the status of tests and coverage. We hope this continuous integration facilitates editing and extending the existing codebase for interested members of the community.
 
-* Completed a review of the entire codebase using `flake8` and `pylint` to ensure PEP8 compliance. The corresponding changes yielded code that is easier to read and use. See guidance in Readme on linting and how to ensure newly added code is compliant.
+- Completed a review of the entire codebase using `flake8` and `pylint` to ensure PEP8 compliance. The corresponding changes yielded code that is easier to read and use. See guidance in Readme on linting and how to ensure newly added code is compliant.
 
-* Models for estimating Environmental Impact (i.e., embodied carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL Model Library and available in this release.
+- Models for estimating Environmental Impact (i.e., embodied carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL Model Library and available in this release.
 
-* "ListAllDamageStates" option allows you to print a comprehensive list of all possible damage states for all components in the columns of the DMG output file. This can make parsing the output easier but increases file size. By default, this option is turned off and only damage states that affect at least one block are printed.
+- "ListAllDamageStates" option allows you to print a comprehensive list of all possible damage states for all components in the columns of the DMG output file. This can make parsing the output easier but increases file size. By default, this option is turned off and only damage states that affect at least one block are printed.
 
-* Damage and Loss Model Library
+- Damage and Loss Model Library
 
-  * A collection of parameters and metadata for damage and loss models for performance based engineering. The library is available and updated regularly in the DB_DamageAndLoss GitHub Repository.
+  - A collection of parameters and metadata for damage and loss models for performance based engineering. The library is available and updated regularly in the DB_DamageAndLoss GitHub Repository.
   
-  * This and future releases of Pelicun have the latest version of the library at the time of their release bundled with them.
+  - This and future releases of Pelicun have the latest version of the library at the time of their release bundled with them.
 
-* DL_calculation tool
+- DL_calculation tool
 
-  * Support for combination of built-in and user-defined databases for damage and loss models.
+  - Support for combination of built-in and user-defined databases for damage and loss models.
   
-  * Results are now also provided in standard SimCenter `JSON` format besides the existing `CSV` tables. You can specify the preferred format in the configuration file under Output/Format. The default file format is still CSV.
+  - Results are now also provided in standard SimCenter `JSON` format besides the existing `CSV` tables. You can specify the preferred format in the configuration file under Output/Format. The default file format is still CSV.
     
-  * Support running calculations for only a subset of available consequence types.
+  - Support running calculations for only a subset of available consequence types.
 
-* Several error and warning messages added to provide more meaningful information in the log file when something goes wrong in a simulation.
+- Several error and warning messages added to provide more meaningful information in the log file when something goes wrong in a simulation.
 
-* Update dependencies to more recent versions. 
+- Update dependencies to more recent versions. 
 
-* The online documentation is significantly out of date. While we are working on an update, we recommend using the documentation of the [DL panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
+- The online documentation is significantly out of date. While we are working on an update, we recommend using the documentation of the [DL panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
 
 ### Changes in v3.1
 
-* Calculation settings are now assessment-specific. This allows you to use more than one assessments in an interactive calculation and each will have its own set of options, including log files.
+- Calculation settings are now assessment-specific. This allows you to use more than one assessments in an interactive calculation and each will have its own set of options, including log files.
 
-* The uq module was decoupled from the others to enable standalone uq calculations that work without having an active assessment.
+- The uq module was decoupled from the others to enable standalone uq calculations that work without having an active assessment.
 
-* A completely redesigned DL_calculation.py script that provides decoupled demand, damage, and loss assessment and more flexibility when setting up each of those when pelicun is used with a configuration file in a larger workflow.
+- A completely redesigned DL_calculation.py script that provides decoupled demand, damage, and loss assessment and more flexibility when setting up each of those when pelicun is used with a configuration file in a larger workflow.
 
-* Two new examples that use the DL_calculation.py script and a json configuration file were added to the example folder.
+- Two new examples that use the DL_calculation.py script and a json configuration file were added to the example folder.
 
-* A new example that demonstrates a detailed interactive calculation in a Jupyter notebook was added to the following DesignSafe project: https://www.designsafe-ci.org/data/browser/public/designsafe.storage.published/PRJ-3411v5 This project will be extended with additional examples in the future.
+- A new example that demonstrates a detailed interactive calculation in a Jupyter notebook was added to the following DesignSafe project: https://www.designsafe-ci.org/data/browser/public/designsafe.storage.published/PRJ-3411v5 This project will be extended with additional examples in the future.
 
-* Unit conversion factors moved to an external file (settings/default_units) to make it easier to add new units to the list. This also allows redefining the internal units through a complete replacement of the factors. The internal units continue to follow the SI system.
+- Unit conversion factors moved to an external file (settings/default_units) to make it easier to add new units to the list. This also allows redefining the internal units through a complete replacement of the factors. The internal units continue to follow the SI system.
 
-* Substantial improvements in coding style using flake8 and pylint to monitor and help enforce PEP8.
+- Substantial improvements in coding style using flake8 and pylint to monitor and help enforce PEP8.
 
-* Several performance improvements made calculations more efficient, especially for large problems, such as regional assessments or tall buildings investigated using the FEMA P-58 methodology.
+- Several performance improvements made calculations more efficient, especially for large problems, such as regional assessments or tall buildings investigated using the FEMA P-58 methodology.
 
-* Several bugfixes and a large number of minor changes that make the engine more robust and easier to use.
+- Several bugfixes and a large number of minor changes that make the engine more robust and easier to use.
 
-* Update recommended Python version to 3.10 and other dependencies to more recent versions. 
+- Update recommended Python version to 3.10 and other dependencies to more recent versions. 
 
 ### Changes in v3.0
 
-* The architecture was redesigned to better support interactive calculation and provide a low-level integration across all supported methods. This is the first release with the new architecture. Frequent updates are planned to provide additional examples, tests, and bugfixes in the next few months.  
+- The architecture was redesigned to better support interactive calculation and provide a low-level integration across all supported methods. This is the first release with the new architecture. Frequent updates are planned to provide additional examples, tests, and bugfixes in the next few months.  
 
-* New `assessment` module introduced to replace `control` module:
-  * Provides a high-level access to models and their methods
-  * Integrates all types of assessments into a uniform approach
-  * Most of the methods from the earlier `control` module were moved to the `model` module
+- New `assessment` module introduced to replace `control` module:
+  - Provides a high-level access to models and their methods
+  - Integrates all types of assessments into a uniform approach
+  - Most of the methods from the earlier `control` module were moved to the `model` module
   
-* Decoupled demand, damage, and loss calculations:
-  * Fragility functions and consequence functions are stored in separate files. Added new methods to the `db` module to prepare the corresponding data files and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus hurricane data will be added in a future release.
-  * Decoupling removed a large amount of redundant data from supporting databases and made the use of HDF and json files for such data unnecessary. All data are stored in easy-to-read csv files.
-  * Assessment workflows can include all three steps (i.e., demand, damage, and loss) or only one or two steps. For example, damage estimates from one analysis can drive loss calculations in another one.
+- Decoupled demand, damage, and loss calculations:
+  - Fragility functions and consequence functions are stored in separate files. Added new methods to the `db` module to prepare the corresponding data files and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus hurricane data will be added in a future release.
+  - Decoupling removed a large amount of redundant data from supporting databases and made the use of HDF and json files for such data unnecessary. All data are stored in easy-to-read csv files.
+  - Assessment workflows can include all three steps (i.e., demand, damage, and loss) or only one or two steps. For example, damage estimates from one analysis can drive loss calculations in another one.
   
-* Integrated damage and loss calculation across all methods and components:
-  * This includes phenomena such as collapse, including various collapse modes, and irreparable damage.
-  * Cascading damages and other interdependencies between various components can be introduced using a damage process file.
-  * Losses can be driven by damages or demands. The former supports the conventional damage->consequence function approach, while the latter supports the use of vulnerability functions. These can be combined within the same analysis, if needed.
-  * The same loss component can be driven by multiple types of damages. For example, replacement can be triggered by either collapse or irreparable damage.
+- Integrated damage and loss calculation across all methods and components:
+  - This includes phenomena such as collapse, including various collapse modes, and irreparable damage.
+  - Cascading damages and other interdependencies between various components can be introduced using a damage process file.
+  - Losses can be driven by damages or demands. The former supports the conventional damage->consequence function approach, while the latter supports the use of vulnerability functions. These can be combined within the same analysis, if needed.
+  - The same loss component can be driven by multiple types of damages. For example, replacement can be triggered by either collapse or irreparable damage.
 
-* Introduced *Options* in the configuration file and in the `base` module:
-  * These options handle settings that concern pelicun behavior;
-  * general preferences that might affect multiple assessment models;
-  * and settings that users would not want to change frequently.
-  * Default settings are provided in a `default_config.json` file. These can be overridden by providing any of the prescribed keys with a user-defined value assigned to them in the configuration file for an analysis.
+- Introduced *Options* in the configuration file and in the `base` module:
+  - These options handle settings that concern pelicun behavior;
+  - general preferences that might affect multiple assessment models;
+  - and settings that users would not want to change frequently.
+  - Default settings are provided in a `default_config.json` file. These can be overridden by providing any of the prescribed keys with a user-defined value assigned to them in the configuration file for an analysis.
 
-* Introduced consistent handling of units. Each csv table has a standard column to describe units of the data in it. If the standard column is missing, the table is assumed to use SI units.
+- Introduced consistent handling of units. Each csv table has a standard column to describe units of the data in it. If the standard column is missing, the table is assumed to use SI units.
 
-* Introduced consistent handling of pandas MultiIndex objects in headers and indexes. When tabular data is stored in csv files, MultiIndex objects are converted to simple indexes by concatenating the strings at each level and separating them with a `-`. This facilitates post-processing csv files in pandas without impeding post-processing those files in non-Python environments.
+- Introduced consistent handling of pandas MultiIndex objects in headers and indexes. When tabular data is stored in csv files, MultiIndex objects are converted to simple indexes by concatenating the strings at each level and separating them with a `-`. This facilitates post-processing csv files in pandas without impeding post-processing those files in non-Python environments.
 
-* Updated the DL_calculation script to support the new architecture. Currently, only the config file input is used. Other arguments were kept in the script for backwards compatibility; future updates will remove some of those arguments and introduce new ones.
+- Updated the DL_calculation script to support the new architecture. Currently, only the config file input is used. Other arguments were kept in the script for backwards compatibility; future updates will remove some of those arguments and introduce new ones.
 
-* The log files were redesigned to provide more legible and easy-to-read information about the assessment.
+- The log files were redesigned to provide more legible and easy-to-read information about the assessment.
 
 ### Changes in v2.6
 
-* Support EDPs with more than 3 characters and/or a variable in their name. For example, SA_1.0 or SA_T1
-* Support fitting normal distribution to raw EDP data (lognormal was already available)
-* Extract key settings to base.py to make them more accessible for users.
-* Minor bugfixes mostly related to hurricane storm surge assessment
+- Support EDPs with more than 3 characters and/or a variable in their name. For example, SA_1.0 or SA_T1
+- Support fitting normal distribution to raw EDP data (lognormal was already available)
+- Extract key settings to base.py to make them more accessible for users.
+- Minor bugfixes mostly related to hurricane storm surge assessment
 
 ## License
 
 `pelicun` is distributed under the BSD 3-Clause license, see LICENSE.
 
 ## Acknowledgment
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: pelicun Version: 3.3 Summary: Probabilistic
+Metadata-Version: 2.1 Name: pelicun Version: 3.3.1 Summary: Probabilistic
 Estimation of Losses, Injuries, and Community resilience Under Natural hazard
 events Home-page: http://nheri-simcenter.github.io/pelicun/ Author: Adam
 ZsarnÃ³czay Author-email: adamzs@stanford.edu License: BSD License Platform:
 any Classifier: Programming Language :: Python Classifier: Development Status
 :: 5 - Production/Stable Classifier: Natural Language :: English Classifier:
 Environment :: Console Classifier: Framework :: Jupyter Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
 :: English Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
-markdown Provides-Extra: testing License-File: LICENSE
+markdown License-File: LICENSE Requires-Dist: numpy<2.0,>=1.22.0 Requires-Dist:
+scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Requires-Dist:
+tables>=3.7.0 Provides-Extra: testing Requires-Dist: pytest; extra == "testing"
                                    [pelicun]
       alt="DOI">[https://zenodo.org/badge/DOI/10.5281/zenodo.2558558.svg]
  PPrroobbaabbiilliissttiicc EEssttiimmaattiioonn ooff LLoosssseess,, IInnjjuurriieess,, aanndd CCoommmmuunniittyy rreessiilliieennccee UUnnddeerr
                              NNaattuurraall hhaazzaarrdd eevveennttss
 ![Tests](https://github.com/NHERI-SimCenter/pelicun/actions/workflows/
 tests.yml/badge.svg) [![codecov](https://codecov.io/github/NHERI-SimCenter/
 pelicun/branch/master/graph/badge.svg?token=W79M5FGOCG)](https://codecov.io/
@@ -139,143 +141,143 @@
 needed. - **Remove `bldg` from variable and class names**: Following the
 changes mentioned earlier, we dropped `bldg` from lables where the
 functionality is no longer limited to buildings. - **Introduce `calibrated`
 attribute for demand model**: This new attribute will allow users to check if a
 model has already been calibrated to the provided empirical data. - Several
 other minor improvements; see commit messages for details. - Dependencies -
 Ceiling raised for `pandas`, supporting version 2.0 and above up until 3.0. ###
-Changes in v3.2 * Changes that might affect backwards compatibility: * Unit
+Changes in v3.2 - Changes that might affect backwards compatibility: - Unit
 information is included in every output file. If you parse Pelicun outputs and
-did not anticipate a Unit entry, your parser might need an update. * Decision
+did not anticipate a Unit entry, your parser might need an update. - Decision
 variable types in the repair consequence outputs are named using CamelCase
 rather than all capitals to be consistent with other parts of the codebase. For
 example, we use "Cost" instead of "COST". This might affect post-processing
-scripts. * For clarity, "ea" units were replaced with "unitless" where
+scripts. - For clarity, "ea" units were replaced with "unitless" where
 appropriate. There should be no practical difference between the calculations
-due to this change. Interstory drift ratio demand types are one example. *
+due to this change. Interstory drift ratio demand types are one example. -
 Weighted component block assignment is no longer supported. We recommend using
 more versatile multiple component definitions (see new feature below) to
-achieve the same effect. * Damage functions (i.e., assign quantity of damage as
+achieve the same effect. - Damage functions (i.e., assign quantity of damage as
 a function of demand) are no longer supported. We recommend using the new
 multilinear CDF feature to develop theoretically equivalent, but more efficient
-models. * New multilinear CDF Random Variable allows using the multilinear
-approximation of any CDF in the tool. * Capacity adjustment allows adjusting
+models. - New multilinear CDF Random Variable allows using the multilinear
+approximation of any CDF in the tool. - Capacity adjustment allows adjusting
 (scaling or shifting) default capacities (i.e., fragility curves) with factors
-specific to each Performance Group. * Support for multiple definitions of the
+specific to each Performance Group. - Support for multiple definitions of the
 same component at the same location-direction. This feature facilitates adding
 components with different block sizes to the same floor or defining multiple
-tenants on the same floor, each with their own set of components. * Support for
+tenants on the same floor, each with their own set of components. - Support for
 cloning demands, that is, taking a provided demand dataset, creating a copy and
 considering it as another demand. For example, you can provide results of
 seismic response in the X direction and automatically prepare a copy of them to
-represent results in the Y direction. * Added a comprehensive suite of more
+represent results in the Y direction. - Added a comprehensive suite of more
 than 140 unit tests that cover more than 93% of the codebase. Tests are
 automatically executed after every commit using GitHub Actions and coverage is
 monitored through `Codecov.io`. Badges at the top of the Readme show the status
 of tests and coverage. We hope this continuous integration facilitates editing
-and extending the existing codebase for interested members of the community. *
+and extending the existing codebase for interested members of the community. -
 Completed a review of the entire codebase using `flake8` and `pylint` to ensure
 PEP8 compliance. The corresponding changes yielded code that is easier to read
 and use. See guidance in Readme on linting and how to ensure newly added code
-is compliant. * Models for estimating Environmental Impact (i.e., embodied
+is compliant. - Models for estimating Environmental Impact (i.e., embodied
 carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL
-Model Library and available in this release. * "ListAllDamageStates" option
+Model Library and available in this release. - "ListAllDamageStates" option
 allows you to print a comprehensive list of all possible damage states for all
 components in the columns of the DMG output file. This can make parsing the
 output easier but increases file size. By default, this option is turned off
-and only damage states that affect at least one block are printed. * Damage and
-Loss Model Library * A collection of parameters and metadata for damage and
+and only damage states that affect at least one block are printed. - Damage and
+Loss Model Library - A collection of parameters and metadata for damage and
 loss models for performance based engineering. The library is available and
-updated regularly in the DB_DamageAndLoss GitHub Repository. * This and future
+updated regularly in the DB_DamageAndLoss GitHub Repository. - This and future
 releases of Pelicun have the latest version of the library at the time of their
-release bundled with them. * DL_calculation tool * Support for combination of
-built-in and user-defined databases for damage and loss models. * Results are
+release bundled with them. - DL_calculation tool - Support for combination of
+built-in and user-defined databases for damage and loss models. - Results are
 now also provided in standard SimCenter `JSON` format besides the existing
 `CSV` tables. You can specify the preferred format in the configuration file
-under Output/Format. The default file format is still CSV. * Support running
-calculations for only a subset of available consequence types. * Several error
+under Output/Format. The default file format is still CSV. - Support running
+calculations for only a subset of available consequence types. - Several error
 and warning messages added to provide more meaningful information in the log
-file when something goes wrong in a simulation. * Update dependencies to more
-recent versions. * The online documentation is significantly out of date. While
+file when something goes wrong in a simulation. - Update dependencies to more
+recent versions. - The online documentation is significantly out of date. While
 we are working on an update, we recommend using the documentation of the [DL
 panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-
 Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
-### Changes in v3.1 * Calculation settings are now assessment-specific. This
+### Changes in v3.1 - Calculation settings are now assessment-specific. This
 allows you to use more than one assessments in an interactive calculation and
-each will have its own set of options, including log files. * The uq module was
+each will have its own set of options, including log files. - The uq module was
 decoupled from the others to enable standalone uq calculations that work
-without having an active assessment. * A completely redesigned
+without having an active assessment. - A completely redesigned
 DL_calculation.py script that provides decoupled demand, damage, and loss
 assessment and more flexibility when setting up each of those when pelicun is
-used with a configuration file in a larger workflow. * Two new examples that
+used with a configuration file in a larger workflow. - Two new examples that
 use the DL_calculation.py script and a json configuration file were added to
-the example folder. * A new example that demonstrates a detailed interactive
+the example folder. - A new example that demonstrates a detailed interactive
 calculation in a Jupyter notebook was added to the following DesignSafe
 project: https://www.designsafe-ci.org/data/browser/public/
 designsafe.storage.published/PRJ-3411v5 This project will be extended with
-additional examples in the future. * Unit conversion factors moved to an
+additional examples in the future. - Unit conversion factors moved to an
 external file (settings/default_units) to make it easier to add new units to
 the list. This also allows redefining the internal units through a complete
 replacement of the factors. The internal units continue to follow the SI
-system. * Substantial improvements in coding style using flake8 and pylint to
-monitor and help enforce PEP8. * Several performance improvements made
+system. - Substantial improvements in coding style using flake8 and pylint to
+monitor and help enforce PEP8. - Several performance improvements made
 calculations more efficient, especially for large problems, such as regional
-assessments or tall buildings investigated using the FEMA P-58 methodology. *
+assessments or tall buildings investigated using the FEMA P-58 methodology. -
 Several bugfixes and a large number of minor changes that make the engine more
-robust and easier to use. * Update recommended Python version to 3.10 and other
-dependencies to more recent versions. ### Changes in v3.0 * The architecture
+robust and easier to use. - Update recommended Python version to 3.10 and other
+dependencies to more recent versions. ### Changes in v3.0 - The architecture
 was redesigned to better support interactive calculation and provide a low-
 level integration across all supported methods. This is the first release with
 the new architecture. Frequent updates are planned to provide additional
-examples, tests, and bugfixes in the next few months. * New `assessment` module
-introduced to replace `control` module: * Provides a high-level access to
-models and their methods * Integrates all types of assessments into a uniform
-approach * Most of the methods from the earlier `control` module were moved to
-the `model` module * Decoupled demand, damage, and loss calculations: *
+examples, tests, and bugfixes in the next few months. - New `assessment` module
+introduced to replace `control` module: - Provides a high-level access to
+models and their methods - Integrates all types of assessments into a uniform
+approach - Most of the methods from the earlier `control` module were moved to
+the `model` module - Decoupled demand, damage, and loss calculations: -
 Fragility functions and consequence functions are stored in separate files.
 Added new methods to the `db` module to prepare the corresponding data files
 and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus
-hurricane data will be added in a future release. * Decoupling removed a large
+hurricane data will be added in a future release. - Decoupling removed a large
 amount of redundant data from supporting databases and made the use of HDF and
 json files for such data unnecessary. All data are stored in easy-to-read csv
-files. * Assessment workflows can include all three steps (i.e., demand,
+files. - Assessment workflows can include all three steps (i.e., demand,
 damage, and loss) or only one or two steps. For example, damage estimates from
-one analysis can drive loss calculations in another one. * Integrated damage
-and loss calculation across all methods and components: * This includes
+one analysis can drive loss calculations in another one. - Integrated damage
+and loss calculation across all methods and components: - This includes
 phenomena such as collapse, including various collapse modes, and irreparable
-damage. * Cascading damages and other interdependencies between various
-components can be introduced using a damage process file. * Losses can be
+damage. - Cascading damages and other interdependencies between various
+components can be introduced using a damage process file. - Losses can be
 driven by damages or demands. The former supports the conventional damage-
 >consequence function approach, while the latter supports the use of
 vulnerability functions. These can be combined within the same analysis, if
-needed. * The same loss component can be driven by multiple types of damages.
+needed. - The same loss component can be driven by multiple types of damages.
 For example, replacement can be triggered by either collapse or irreparable
-damage. * Introduced *Options* in the configuration file and in the `base`
-module: * These options handle settings that concern pelicun behavior; *
-general preferences that might affect multiple assessment models; * and
-settings that users would not want to change frequently. * Default settings are
+damage. - Introduced *Options* in the configuration file and in the `base`
+module: - These options handle settings that concern pelicun behavior; -
+general preferences that might affect multiple assessment models; - and
+settings that users would not want to change frequently. - Default settings are
 provided in a `default_config.json` file. These can be overridden by providing
 any of the prescribed keys with a user-defined value assigned to them in the
-configuration file for an analysis. * Introduced consistent handling of units.
+configuration file for an analysis. - Introduced consistent handling of units.
 Each csv table has a standard column to describe units of the data in it. If
-the standard column is missing, the table is assumed to use SI units. *
+the standard column is missing, the table is assumed to use SI units. -
 Introduced consistent handling of pandas MultiIndex objects in headers and
 indexes. When tabular data is stored in csv files, MultiIndex objects are
 converted to simple indexes by concatenating the strings at each level and
 separating them with a `-`. This facilitates post-processing csv files in
 pandas without impeding post-processing those files in non-Python environments.
-* Updated the DL_calculation script to support the new architecture. Currently,
+- Updated the DL_calculation script to support the new architecture. Currently,
 only the config file input is used. Other arguments were kept in the script for
 backwards compatibility; future updates will remove some of those arguments and
-introduce new ones. * The log files were redesigned to provide more legible and
-easy-to-read information about the assessment. ### Changes in v2.6 * Support
+introduce new ones. - The log files were redesigned to provide more legible and
+easy-to-read information about the assessment. ### Changes in v2.6 - Support
 EDPs with more than 3 characters and/or a variable in their name. For example,
-SA_1.0 or SA_T1 * Support fitting normal distribution to raw EDP data
-(lognormal was already available) * Extract key settings to base.py to make
-them more accessible for users. * Minor bugfixes mostly related to hurricane
+SA_1.0 or SA_T1 - Support fitting normal distribution to raw EDP data
+(lognormal was already available) - Extract key settings to base.py to make
+them more accessible for users. - Minor bugfixes mostly related to hurricane
 storm surge assessment ## License `pelicun` is distributed under the BSD 3-
 Clause license, see LICENSE. ## Acknowledgment This material is based upon work
 supported by the National Science Foundation under Grants No. 1612843 2131111.
 Any opinions, findings, and conclusions or recommendations expressed in this
 material are those of the authors and do not necessarily reflect the views of
 the National Science Foundation. ## Contact Adam ZsarnÃ³czay, NHERI SimCenter,
 Stanford University, adamzs@stanford.edu
```

### Comparing `pelicun-3.3/README.md` & `pelicun-3.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -146,124 +146,124 @@
 
 - Dependencies
 
   - Ceiling raised for `pandas`, supporting version 2.0 and above up until 3.0.
 
 ### Changes in v3.2
 
-* Changes that might affect backwards compatibility:
+- Changes that might affect backwards compatibility:
 
-  * Unit information is included in every output file. If you parse Pelicun outputs and did not anticipate a Unit entry, your parser might need an update.
+  - Unit information is included in every output file. If you parse Pelicun outputs and did not anticipate a Unit entry, your parser might need an update.
   
-  * Decision variable types in the repair consequence outputs are named using CamelCase rather than all capitals to be consistent with other parts of the codebase. For example, we use "Cost" instead of "COST". This might affect post-processing scripts. 
+  - Decision variable types in the repair consequence outputs are named using CamelCase rather than all capitals to be consistent with other parts of the codebase. For example, we use "Cost" instead of "COST". This might affect post-processing scripts. 
   
-  * For clarity, "ea" units were replaced with "unitless" where appropriate. There should be no practical difference between the calculations due to this change. Interstory drift ratio demand types are one example.
+  - For clarity, "ea" units were replaced with "unitless" where appropriate. There should be no practical difference between the calculations due to this change. Interstory drift ratio demand types are one example.
     
-  * Weighted component block assignment is no longer supported. We recommend using more versatile multiple component definitions (see new feature below) to achieve the same effect.
+  - Weighted component block assignment is no longer supported. We recommend using more versatile multiple component definitions (see new feature below) to achieve the same effect.
     
-  * Damage functions (i.e., assign quantity of damage as a function of demand) are no longer supported. We recommend using the new multilinear CDF feature to develop theoretically equivalent, but more efficient models.
+  - Damage functions (i.e., assign quantity of damage as a function of demand) are no longer supported. We recommend using the new multilinear CDF feature to develop theoretically equivalent, but more efficient models.
 
-* New multilinear CDF Random Variable allows using the multilinear approximation of any CDF in the tool.
+- New multilinear CDF Random Variable allows using the multilinear approximation of any CDF in the tool.
 
-* Capacity adjustment allows adjusting (scaling or shifting) default capacities (i.e., fragility curves) with factors specific to each Performance Group.
+- Capacity adjustment allows adjusting (scaling or shifting) default capacities (i.e., fragility curves) with factors specific to each Performance Group.
 
-* Support for multiple definitions of the same component at the same location-direction. This feature facilitates adding components with different block sizes to the same floor or defining multiple tenants on the same floor, each with their own set of components.
+- Support for multiple definitions of the same component at the same location-direction. This feature facilitates adding components with different block sizes to the same floor or defining multiple tenants on the same floor, each with their own set of components.
 
-* Support for cloning demands, that is, taking a provided demand dataset, creating a copy and considering it as another demand. For example, you can provide results of seismic response in the X direction and automatically prepare a copy of them to represent results in the Y direction. 
+- Support for cloning demands, that is, taking a provided demand dataset, creating a copy and considering it as another demand. For example, you can provide results of seismic response in the X direction and automatically prepare a copy of them to represent results in the Y direction. 
 
-* Added a comprehensive suite of more than 140 unit tests that cover more than 93% of the codebase. Tests are automatically executed after every commit using GitHub Actions and coverage is monitored through `Codecov.io`. Badges at the top of the Readme show the status of tests and coverage. We hope this continuous integration facilitates editing and extending the existing codebase for interested members of the community.
+- Added a comprehensive suite of more than 140 unit tests that cover more than 93% of the codebase. Tests are automatically executed after every commit using GitHub Actions and coverage is monitored through `Codecov.io`. Badges at the top of the Readme show the status of tests and coverage. We hope this continuous integration facilitates editing and extending the existing codebase for interested members of the community.
 
-* Completed a review of the entire codebase using `flake8` and `pylint` to ensure PEP8 compliance. The corresponding changes yielded code that is easier to read and use. See guidance in Readme on linting and how to ensure newly added code is compliant.
+- Completed a review of the entire codebase using `flake8` and `pylint` to ensure PEP8 compliance. The corresponding changes yielded code that is easier to read and use. See guidance in Readme on linting and how to ensure newly added code is compliant.
 
-* Models for estimating Environmental Impact (i.e., embodied carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL Model Library and available in this release.
+- Models for estimating Environmental Impact (i.e., embodied carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL Model Library and available in this release.
 
-* "ListAllDamageStates" option allows you to print a comprehensive list of all possible damage states for all components in the columns of the DMG output file. This can make parsing the output easier but increases file size. By default, this option is turned off and only damage states that affect at least one block are printed.
+- "ListAllDamageStates" option allows you to print a comprehensive list of all possible damage states for all components in the columns of the DMG output file. This can make parsing the output easier but increases file size. By default, this option is turned off and only damage states that affect at least one block are printed.
 
-* Damage and Loss Model Library
+- Damage and Loss Model Library
 
-  * A collection of parameters and metadata for damage and loss models for performance based engineering. The library is available and updated regularly in the DB_DamageAndLoss GitHub Repository.
+  - A collection of parameters and metadata for damage and loss models for performance based engineering. The library is available and updated regularly in the DB_DamageAndLoss GitHub Repository.
   
-  * This and future releases of Pelicun have the latest version of the library at the time of their release bundled with them.
+  - This and future releases of Pelicun have the latest version of the library at the time of their release bundled with them.
 
-* DL_calculation tool
+- DL_calculation tool
 
-  * Support for combination of built-in and user-defined databases for damage and loss models.
+  - Support for combination of built-in and user-defined databases for damage and loss models.
   
-  * Results are now also provided in standard SimCenter `JSON` format besides the existing `CSV` tables. You can specify the preferred format in the configuration file under Output/Format. The default file format is still CSV.
+  - Results are now also provided in standard SimCenter `JSON` format besides the existing `CSV` tables. You can specify the preferred format in the configuration file under Output/Format. The default file format is still CSV.
     
-  * Support running calculations for only a subset of available consequence types.
+  - Support running calculations for only a subset of available consequence types.
 
-* Several error and warning messages added to provide more meaningful information in the log file when something goes wrong in a simulation.
+- Several error and warning messages added to provide more meaningful information in the log file when something goes wrong in a simulation.
 
-* Update dependencies to more recent versions. 
+- Update dependencies to more recent versions. 
 
-* The online documentation is significantly out of date. While we are working on an update, we recommend using the documentation of the [DL panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
+- The online documentation is significantly out of date. While we are working on an update, we recommend using the documentation of the [DL panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
 
 ### Changes in v3.1
 
-* Calculation settings are now assessment-specific. This allows you to use more than one assessments in an interactive calculation and each will have its own set of options, including log files.
+- Calculation settings are now assessment-specific. This allows you to use more than one assessments in an interactive calculation and each will have its own set of options, including log files.
 
-* The uq module was decoupled from the others to enable standalone uq calculations that work without having an active assessment.
+- The uq module was decoupled from the others to enable standalone uq calculations that work without having an active assessment.
 
-* A completely redesigned DL_calculation.py script that provides decoupled demand, damage, and loss assessment and more flexibility when setting up each of those when pelicun is used with a configuration file in a larger workflow.
+- A completely redesigned DL_calculation.py script that provides decoupled demand, damage, and loss assessment and more flexibility when setting up each of those when pelicun is used with a configuration file in a larger workflow.
 
-* Two new examples that use the DL_calculation.py script and a json configuration file were added to the example folder.
+- Two new examples that use the DL_calculation.py script and a json configuration file were added to the example folder.
 
-* A new example that demonstrates a detailed interactive calculation in a Jupyter notebook was added to the following DesignSafe project: https://www.designsafe-ci.org/data/browser/public/designsafe.storage.published/PRJ-3411v5 This project will be extended with additional examples in the future.
+- A new example that demonstrates a detailed interactive calculation in a Jupyter notebook was added to the following DesignSafe project: https://www.designsafe-ci.org/data/browser/public/designsafe.storage.published/PRJ-3411v5 This project will be extended with additional examples in the future.
 
-* Unit conversion factors moved to an external file (settings/default_units) to make it easier to add new units to the list. This also allows redefining the internal units through a complete replacement of the factors. The internal units continue to follow the SI system.
+- Unit conversion factors moved to an external file (settings/default_units) to make it easier to add new units to the list. This also allows redefining the internal units through a complete replacement of the factors. The internal units continue to follow the SI system.
 
-* Substantial improvements in coding style using flake8 and pylint to monitor and help enforce PEP8.
+- Substantial improvements in coding style using flake8 and pylint to monitor and help enforce PEP8.
 
-* Several performance improvements made calculations more efficient, especially for large problems, such as regional assessments or tall buildings investigated using the FEMA P-58 methodology.
+- Several performance improvements made calculations more efficient, especially for large problems, such as regional assessments or tall buildings investigated using the FEMA P-58 methodology.
 
-* Several bugfixes and a large number of minor changes that make the engine more robust and easier to use.
+- Several bugfixes and a large number of minor changes that make the engine more robust and easier to use.
 
-* Update recommended Python version to 3.10 and other dependencies to more recent versions. 
+- Update recommended Python version to 3.10 and other dependencies to more recent versions. 
 
 ### Changes in v3.0
 
-* The architecture was redesigned to better support interactive calculation and provide a low-level integration across all supported methods. This is the first release with the new architecture. Frequent updates are planned to provide additional examples, tests, and bugfixes in the next few months.  
+- The architecture was redesigned to better support interactive calculation and provide a low-level integration across all supported methods. This is the first release with the new architecture. Frequent updates are planned to provide additional examples, tests, and bugfixes in the next few months.  
 
-* New `assessment` module introduced to replace `control` module:
-  * Provides a high-level access to models and their methods
-  * Integrates all types of assessments into a uniform approach
-  * Most of the methods from the earlier `control` module were moved to the `model` module
+- New `assessment` module introduced to replace `control` module:
+  - Provides a high-level access to models and their methods
+  - Integrates all types of assessments into a uniform approach
+  - Most of the methods from the earlier `control` module were moved to the `model` module
   
-* Decoupled demand, damage, and loss calculations:
-  * Fragility functions and consequence functions are stored in separate files. Added new methods to the `db` module to prepare the corresponding data files and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus hurricane data will be added in a future release.
-  * Decoupling removed a large amount of redundant data from supporting databases and made the use of HDF and json files for such data unnecessary. All data are stored in easy-to-read csv files.
-  * Assessment workflows can include all three steps (i.e., demand, damage, and loss) or only one or two steps. For example, damage estimates from one analysis can drive loss calculations in another one.
+- Decoupled demand, damage, and loss calculations:
+  - Fragility functions and consequence functions are stored in separate files. Added new methods to the `db` module to prepare the corresponding data files and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus hurricane data will be added in a future release.
+  - Decoupling removed a large amount of redundant data from supporting databases and made the use of HDF and json files for such data unnecessary. All data are stored in easy-to-read csv files.
+  - Assessment workflows can include all three steps (i.e., demand, damage, and loss) or only one or two steps. For example, damage estimates from one analysis can drive loss calculations in another one.
   
-* Integrated damage and loss calculation across all methods and components:
-  * This includes phenomena such as collapse, including various collapse modes, and irreparable damage.
-  * Cascading damages and other interdependencies between various components can be introduced using a damage process file.
-  * Losses can be driven by damages or demands. The former supports the conventional damage->consequence function approach, while the latter supports the use of vulnerability functions. These can be combined within the same analysis, if needed.
-  * The same loss component can be driven by multiple types of damages. For example, replacement can be triggered by either collapse or irreparable damage.
+- Integrated damage and loss calculation across all methods and components:
+  - This includes phenomena such as collapse, including various collapse modes, and irreparable damage.
+  - Cascading damages and other interdependencies between various components can be introduced using a damage process file.
+  - Losses can be driven by damages or demands. The former supports the conventional damage->consequence function approach, while the latter supports the use of vulnerability functions. These can be combined within the same analysis, if needed.
+  - The same loss component can be driven by multiple types of damages. For example, replacement can be triggered by either collapse or irreparable damage.
 
-* Introduced *Options* in the configuration file and in the `base` module:
-  * These options handle settings that concern pelicun behavior;
-  * general preferences that might affect multiple assessment models;
-  * and settings that users would not want to change frequently.
-  * Default settings are provided in a `default_config.json` file. These can be overridden by providing any of the prescribed keys with a user-defined value assigned to them in the configuration file for an analysis.
+- Introduced *Options* in the configuration file and in the `base` module:
+  - These options handle settings that concern pelicun behavior;
+  - general preferences that might affect multiple assessment models;
+  - and settings that users would not want to change frequently.
+  - Default settings are provided in a `default_config.json` file. These can be overridden by providing any of the prescribed keys with a user-defined value assigned to them in the configuration file for an analysis.
 
-* Introduced consistent handling of units. Each csv table has a standard column to describe units of the data in it. If the standard column is missing, the table is assumed to use SI units.
+- Introduced consistent handling of units. Each csv table has a standard column to describe units of the data in it. If the standard column is missing, the table is assumed to use SI units.
 
-* Introduced consistent handling of pandas MultiIndex objects in headers and indexes. When tabular data is stored in csv files, MultiIndex objects are converted to simple indexes by concatenating the strings at each level and separating them with a `-`. This facilitates post-processing csv files in pandas without impeding post-processing those files in non-Python environments.
+- Introduced consistent handling of pandas MultiIndex objects in headers and indexes. When tabular data is stored in csv files, MultiIndex objects are converted to simple indexes by concatenating the strings at each level and separating them with a `-`. This facilitates post-processing csv files in pandas without impeding post-processing those files in non-Python environments.
 
-* Updated the DL_calculation script to support the new architecture. Currently, only the config file input is used. Other arguments were kept in the script for backwards compatibility; future updates will remove some of those arguments and introduce new ones.
+- Updated the DL_calculation script to support the new architecture. Currently, only the config file input is used. Other arguments were kept in the script for backwards compatibility; future updates will remove some of those arguments and introduce new ones.
 
-* The log files were redesigned to provide more legible and easy-to-read information about the assessment.
+- The log files were redesigned to provide more legible and easy-to-read information about the assessment.
 
 ### Changes in v2.6
 
-* Support EDPs with more than 3 characters and/or a variable in their name. For example, SA_1.0 or SA_T1
-* Support fitting normal distribution to raw EDP data (lognormal was already available)
-* Extract key settings to base.py to make them more accessible for users.
-* Minor bugfixes mostly related to hurricane storm surge assessment
+- Support EDPs with more than 3 characters and/or a variable in their name. For example, SA_1.0 or SA_T1
+- Support fitting normal distribution to raw EDP data (lognormal was already available)
+- Extract key settings to base.py to make them more accessible for users.
+- Minor bugfixes mostly related to hurricane storm surge assessment
 
 ## License
 
 `pelicun` is distributed under the BSD 3-Clause license, see LICENSE.
 
 ## Acknowledgment
```

#### html2text {}

```diff
@@ -124,143 +124,143 @@
 needed. - **Remove `bldg` from variable and class names**: Following the
 changes mentioned earlier, we dropped `bldg` from lables where the
 functionality is no longer limited to buildings. - **Introduce `calibrated`
 attribute for demand model**: This new attribute will allow users to check if a
 model has already been calibrated to the provided empirical data. - Several
 other minor improvements; see commit messages for details. - Dependencies -
 Ceiling raised for `pandas`, supporting version 2.0 and above up until 3.0. ###
-Changes in v3.2 * Changes that might affect backwards compatibility: * Unit
+Changes in v3.2 - Changes that might affect backwards compatibility: - Unit
 information is included in every output file. If you parse Pelicun outputs and
-did not anticipate a Unit entry, your parser might need an update. * Decision
+did not anticipate a Unit entry, your parser might need an update. - Decision
 variable types in the repair consequence outputs are named using CamelCase
 rather than all capitals to be consistent with other parts of the codebase. For
 example, we use "Cost" instead of "COST". This might affect post-processing
-scripts. * For clarity, "ea" units were replaced with "unitless" where
+scripts. - For clarity, "ea" units were replaced with "unitless" where
 appropriate. There should be no practical difference between the calculations
-due to this change. Interstory drift ratio demand types are one example. *
+due to this change. Interstory drift ratio demand types are one example. -
 Weighted component block assignment is no longer supported. We recommend using
 more versatile multiple component definitions (see new feature below) to
-achieve the same effect. * Damage functions (i.e., assign quantity of damage as
+achieve the same effect. - Damage functions (i.e., assign quantity of damage as
 a function of demand) are no longer supported. We recommend using the new
 multilinear CDF feature to develop theoretically equivalent, but more efficient
-models. * New multilinear CDF Random Variable allows using the multilinear
-approximation of any CDF in the tool. * Capacity adjustment allows adjusting
+models. - New multilinear CDF Random Variable allows using the multilinear
+approximation of any CDF in the tool. - Capacity adjustment allows adjusting
 (scaling or shifting) default capacities (i.e., fragility curves) with factors
-specific to each Performance Group. * Support for multiple definitions of the
+specific to each Performance Group. - Support for multiple definitions of the
 same component at the same location-direction. This feature facilitates adding
 components with different block sizes to the same floor or defining multiple
-tenants on the same floor, each with their own set of components. * Support for
+tenants on the same floor, each with their own set of components. - Support for
 cloning demands, that is, taking a provided demand dataset, creating a copy and
 considering it as another demand. For example, you can provide results of
 seismic response in the X direction and automatically prepare a copy of them to
-represent results in the Y direction. * Added a comprehensive suite of more
+represent results in the Y direction. - Added a comprehensive suite of more
 than 140 unit tests that cover more than 93% of the codebase. Tests are
 automatically executed after every commit using GitHub Actions and coverage is
 monitored through `Codecov.io`. Badges at the top of the Readme show the status
 of tests and coverage. We hope this continuous integration facilitates editing
-and extending the existing codebase for interested members of the community. *
+and extending the existing codebase for interested members of the community. -
 Completed a review of the entire codebase using `flake8` and `pylint` to ensure
 PEP8 compliance. The corresponding changes yielded code that is easier to read
 and use. See guidance in Readme on linting and how to ensure newly added code
-is compliant. * Models for estimating Environmental Impact (i.e., embodied
+is compliant. - Models for estimating Environmental Impact (i.e., embodied
 carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL
-Model Library and available in this release. * "ListAllDamageStates" option
+Model Library and available in this release. - "ListAllDamageStates" option
 allows you to print a comprehensive list of all possible damage states for all
 components in the columns of the DMG output file. This can make parsing the
 output easier but increases file size. By default, this option is turned off
-and only damage states that affect at least one block are printed. * Damage and
-Loss Model Library * A collection of parameters and metadata for damage and
+and only damage states that affect at least one block are printed. - Damage and
+Loss Model Library - A collection of parameters and metadata for damage and
 loss models for performance based engineering. The library is available and
-updated regularly in the DB_DamageAndLoss GitHub Repository. * This and future
+updated regularly in the DB_DamageAndLoss GitHub Repository. - This and future
 releases of Pelicun have the latest version of the library at the time of their
-release bundled with them. * DL_calculation tool * Support for combination of
-built-in and user-defined databases for damage and loss models. * Results are
+release bundled with them. - DL_calculation tool - Support for combination of
+built-in and user-defined databases for damage and loss models. - Results are
 now also provided in standard SimCenter `JSON` format besides the existing
 `CSV` tables. You can specify the preferred format in the configuration file
-under Output/Format. The default file format is still CSV. * Support running
-calculations for only a subset of available consequence types. * Several error
+under Output/Format. The default file format is still CSV. - Support running
+calculations for only a subset of available consequence types. - Several error
 and warning messages added to provide more meaningful information in the log
-file when something goes wrong in a simulation. * Update dependencies to more
-recent versions. * The online documentation is significantly out of date. While
+file when something goes wrong in a simulation. - Update dependencies to more
+recent versions. - The online documentation is significantly out of date. While
 we are working on an update, we recommend using the documentation of the [DL
 panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-
 Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
-### Changes in v3.1 * Calculation settings are now assessment-specific. This
+### Changes in v3.1 - Calculation settings are now assessment-specific. This
 allows you to use more than one assessments in an interactive calculation and
-each will have its own set of options, including log files. * The uq module was
+each will have its own set of options, including log files. - The uq module was
 decoupled from the others to enable standalone uq calculations that work
-without having an active assessment. * A completely redesigned
+without having an active assessment. - A completely redesigned
 DL_calculation.py script that provides decoupled demand, damage, and loss
 assessment and more flexibility when setting up each of those when pelicun is
-used with a configuration file in a larger workflow. * Two new examples that
+used with a configuration file in a larger workflow. - Two new examples that
 use the DL_calculation.py script and a json configuration file were added to
-the example folder. * A new example that demonstrates a detailed interactive
+the example folder. - A new example that demonstrates a detailed interactive
 calculation in a Jupyter notebook was added to the following DesignSafe
 project: https://www.designsafe-ci.org/data/browser/public/
 designsafe.storage.published/PRJ-3411v5 This project will be extended with
-additional examples in the future. * Unit conversion factors moved to an
+additional examples in the future. - Unit conversion factors moved to an
 external file (settings/default_units) to make it easier to add new units to
 the list. This also allows redefining the internal units through a complete
 replacement of the factors. The internal units continue to follow the SI
-system. * Substantial improvements in coding style using flake8 and pylint to
-monitor and help enforce PEP8. * Several performance improvements made
+system. - Substantial improvements in coding style using flake8 and pylint to
+monitor and help enforce PEP8. - Several performance improvements made
 calculations more efficient, especially for large problems, such as regional
-assessments or tall buildings investigated using the FEMA P-58 methodology. *
+assessments or tall buildings investigated using the FEMA P-58 methodology. -
 Several bugfixes and a large number of minor changes that make the engine more
-robust and easier to use. * Update recommended Python version to 3.10 and other
-dependencies to more recent versions. ### Changes in v3.0 * The architecture
+robust and easier to use. - Update recommended Python version to 3.10 and other
+dependencies to more recent versions. ### Changes in v3.0 - The architecture
 was redesigned to better support interactive calculation and provide a low-
 level integration across all supported methods. This is the first release with
 the new architecture. Frequent updates are planned to provide additional
-examples, tests, and bugfixes in the next few months. * New `assessment` module
-introduced to replace `control` module: * Provides a high-level access to
-models and their methods * Integrates all types of assessments into a uniform
-approach * Most of the methods from the earlier `control` module were moved to
-the `model` module * Decoupled demand, damage, and loss calculations: *
+examples, tests, and bugfixes in the next few months. - New `assessment` module
+introduced to replace `control` module: - Provides a high-level access to
+models and their methods - Integrates all types of assessments into a uniform
+approach - Most of the methods from the earlier `control` module were moved to
+the `model` module - Decoupled demand, damage, and loss calculations: -
 Fragility functions and consequence functions are stored in separate files.
 Added new methods to the `db` module to prepare the corresponding data files
 and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus
-hurricane data will be added in a future release. * Decoupling removed a large
+hurricane data will be added in a future release. - Decoupling removed a large
 amount of redundant data from supporting databases and made the use of HDF and
 json files for such data unnecessary. All data are stored in easy-to-read csv
-files. * Assessment workflows can include all three steps (i.e., demand,
+files. - Assessment workflows can include all three steps (i.e., demand,
 damage, and loss) or only one or two steps. For example, damage estimates from
-one analysis can drive loss calculations in another one. * Integrated damage
-and loss calculation across all methods and components: * This includes
+one analysis can drive loss calculations in another one. - Integrated damage
+and loss calculation across all methods and components: - This includes
 phenomena such as collapse, including various collapse modes, and irreparable
-damage. * Cascading damages and other interdependencies between various
-components can be introduced using a damage process file. * Losses can be
+damage. - Cascading damages and other interdependencies between various
+components can be introduced using a damage process file. - Losses can be
 driven by damages or demands. The former supports the conventional damage-
 >consequence function approach, while the latter supports the use of
 vulnerability functions. These can be combined within the same analysis, if
-needed. * The same loss component can be driven by multiple types of damages.
+needed. - The same loss component can be driven by multiple types of damages.
 For example, replacement can be triggered by either collapse or irreparable
-damage. * Introduced *Options* in the configuration file and in the `base`
-module: * These options handle settings that concern pelicun behavior; *
-general preferences that might affect multiple assessment models; * and
-settings that users would not want to change frequently. * Default settings are
+damage. - Introduced *Options* in the configuration file and in the `base`
+module: - These options handle settings that concern pelicun behavior; -
+general preferences that might affect multiple assessment models; - and
+settings that users would not want to change frequently. - Default settings are
 provided in a `default_config.json` file. These can be overridden by providing
 any of the prescribed keys with a user-defined value assigned to them in the
-configuration file for an analysis. * Introduced consistent handling of units.
+configuration file for an analysis. - Introduced consistent handling of units.
 Each csv table has a standard column to describe units of the data in it. If
-the standard column is missing, the table is assumed to use SI units. *
+the standard column is missing, the table is assumed to use SI units. -
 Introduced consistent handling of pandas MultiIndex objects in headers and
 indexes. When tabular data is stored in csv files, MultiIndex objects are
 converted to simple indexes by concatenating the strings at each level and
 separating them with a `-`. This facilitates post-processing csv files in
 pandas without impeding post-processing those files in non-Python environments.
-* Updated the DL_calculation script to support the new architecture. Currently,
+- Updated the DL_calculation script to support the new architecture. Currently,
 only the config file input is used. Other arguments were kept in the script for
 backwards compatibility; future updates will remove some of those arguments and
-introduce new ones. * The log files were redesigned to provide more legible and
-easy-to-read information about the assessment. ### Changes in v2.6 * Support
+introduce new ones. - The log files were redesigned to provide more legible and
+easy-to-read information about the assessment. ### Changes in v2.6 - Support
 EDPs with more than 3 characters and/or a variable in their name. For example,
-SA_1.0 or SA_T1 * Support fitting normal distribution to raw EDP data
-(lognormal was already available) * Extract key settings to base.py to make
-them more accessible for users. * Minor bugfixes mostly related to hurricane
+SA_1.0 or SA_T1 - Support fitting normal distribution to raw EDP data
+(lognormal was already available) - Extract key settings to base.py to make
+them more accessible for users. - Minor bugfixes mostly related to hurricane
 storm surge assessment ## License `pelicun` is distributed under the BSD 3-
 Clause license, see LICENSE. ## Acknowledgment This material is based upon work
 supported by the National Science Foundation under Grants No. 1612843 2131111.
 Any opinions, findings, and conclusions or recommendations expressed in this
 material are those of the authors and do not necessarily reflect the views of
 the National Science Foundation. ## Contact Adam ZsarnÃ³czay, NHERI SimCenter,
 Stanford University, adamzs@stanford.edu
```

### Comparing `pelicun-3.3/pelicun/__init__.py` & `pelicun-3.3.1/pelicun/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,14 @@
 
 Contributors:
 Adam Zsarnóczay
 """
 
 name = "pelicun"
 
-__version__ = '3.3'
+__version__ = '3.3.1'
 
 __copyright__ = ("Copyright (c) 2018 Leland Stanford "
                  "Junior University and The Regents "
                  "of the University of California")
 
 __license__ = "BSD 3-Clause License"
```

### Comparing `pelicun-3.3/pelicun/assessment.py` & `pelicun-3.3.1/pelicun/assessment.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/auto.py` & `pelicun-3.3.1/pelicun/auto.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/base.py` & `pelicun-3.3.1/pelicun/base.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/db.py` & `pelicun-3.3.1/pelicun/db.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/001/CMP_QNT.csv` & `pelicun-3.3.1/pelicun/examples/001/CMP_QNT.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/001/demands_s4.csv` & `pelicun-3.3.1/pelicun/examples/001/demands_s4.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/001/input.json` & `pelicun-3.3.1/pelicun/examples/001/input.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/002/input.json` & `pelicun-3.3.1/pelicun/examples/002/input.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/002/response.csv` & `pelicun-3.3.1/pelicun/examples/002/response.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/0_tmp/CMP_marginals.csv` & `pelicun-3.3.1/pelicun/examples/0_tmp/CMP_marginals.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/0_tmp/config.json` & `pelicun-3.3.1/pelicun/examples/0_tmp/config.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/0_tmp/demands.csv` & `pelicun-3.3.1/pelicun/examples/0_tmp/demands.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/examples/0_tmp/fragility_Additional.csv` & `pelicun-3.3.1/pelicun/examples/0_tmp/fragility_Additional.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/file_io.py` & `pelicun-3.3.1/pelicun/file_io.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/model/__init__.py` & `pelicun-3.3.1/pelicun/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/model/asset_model.py` & `pelicun-3.3.1/pelicun/model/asset_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/model/damage_model.py` & `pelicun-3.3.1/pelicun/model/damage_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/model/demand_model.py` & `pelicun-3.3.1/pelicun/model/demand_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/model/loss_model.py` & `pelicun-3.3.1/pelicun/model/loss_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/model/pelicun_model.py` & `pelicun-3.3.1/pelicun/model/pelicun_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_FEMA_P58_2nd.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_bldg.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_story.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_trnsp.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_Hazus_EQ_water.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_HU.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/damage_DB_SimCenter_Hazus_HU_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_FEMA_P58_2nd.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_bldg.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_story.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_Hazus_EQ_trnsp.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv` & `pelicun-3.3.1/pelicun/resources/SimCenterDBDL/loss_repair_DB_SimCenter_Hazus_HU_bldg.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/auto/Hazus_Earthquake_IM.py` & `pelicun-3.3.1/pelicun/resources/auto/Hazus_Earthquake_IM.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/resources/auto/Hazus_Earthquake_Story.py` & `pelicun-3.3.1/pelicun/resources/auto/Hazus_Earthquake_Story.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/settings/default_config.json` & `pelicun-3.3.1/pelicun/settings/default_config.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/settings/default_units.json` & `pelicun-3.3.1/pelicun/settings/default_units.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/code_repetition_checker.py` & `pelicun-3.3.1/pelicun/tests/code_repetition_checker.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/data/base/test_parse_units/duplicate.json` & `pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/duplicate.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/data/base/test_parse_units/duplicate2.json` & `pelicun-3.3.1/pelicun/tests/data/base/test_parse_units/duplicate2.json`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/data/file_io/test_load_data/no_units.csv` & `pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/no_units.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/data/file_io/test_load_data/units.csv` & `pelicun-3.3.1/pelicun/tests/data/file_io/test_load_data/units.csv`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/reset_tests.py` & `pelicun-3.3.1/pelicun/tests/reset_tests.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/test_assessment.py` & `pelicun-3.3.1/pelicun/tests/test_assessment.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/test_auto.py` & `pelicun-3.3.1/pelicun/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/test_base.py` & `pelicun-3.3.1/pelicun/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/test_file_io.py` & `pelicun-3.3.1/pelicun/tests/test_file_io.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/test_model.py` & `pelicun-3.3.1/pelicun/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/test_uq.py` & `pelicun-3.3.1/pelicun/tests/test_uq.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tests/util.py` & `pelicun-3.3.1/pelicun/tests/util.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tools/DL_calculation.py` & `pelicun-3.3.1/pelicun/tools/DL_calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -860,17 +860,18 @@
             ]
         else:
             component_db = []
 
         if asset_config.get('ComponentDatabasePath', False) is not False:
             extra_comps = asset_config['ComponentDatabasePath']
 
-            extra_comps = extra_comps.replace(
-                'CustomDLDataFolder', custom_dl_file_path
-            )
+            if 'CustomDLDataFolder' in extra_comps:
+                extra_comps = extra_comps.replace(
+                    'CustomDLDataFolder', custom_dl_file_path
+                )
 
             component_db += [
                 extra_comps,
             ]
         component_db = component_db[::-1]
 
         # prepare additional fragility data
@@ -1313,17 +1314,18 @@
                 consequence_db = []
 
                 conseq_df = pd.DataFrame()
 
             if repair_config.get('ConsequenceDatabasePath', False) is not False:
                 extra_comps = repair_config['ConsequenceDatabasePath']
 
-                extra_comps = extra_comps.replace(
-                    'CustomDLDataFolder', custom_dl_file_path
-                )
+                if 'CustomDLDataFolder' in extra_comps:
+                    extra_comps = extra_comps.replace(
+                        'CustomDLDataFolder', custom_dl_file_path
+                    )
 
                 consequence_db += [
                     extra_comps,
                 ]
 
                 extra_conseq_df = load_data(
                     extra_comps,
```

### Comparing `pelicun-3.3/pelicun/tools/HDF_to_CSV.py` & `pelicun-3.3.1/pelicun/tools/HDF_to_CSV.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/tools/export_DB.py` & `pelicun-3.3.1/pelicun/tools/export_DB.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun/uq.py` & `pelicun-3.3.1/pelicun/uq.py`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/pelicun.egg-info/PKG-INFO` & `pelicun-3.3.1/pelicun.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelicun
-Version: 3.3
+Version: 3.3.1
 Summary: Probabilistic Estimation of Losses, Injuries, and Community resilience Under Natural hazard events
 Home-page: http://nheri-simcenter.github.io/pelicun/
 Author: Adam Zsarnóczay
 Author-email: adamzs@stanford.edu
 License: BSD License
 Platform: any
 Classifier: Programming Language :: Python
@@ -20,16 +20,21 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy<2.0,>=1.22.0
+Requires-Dist: scipy<2.0,>=1.7.0
+Requires-Dist: pandas<3.0,>=1.4.0
+Requires-Dist: tables>=3.7.0
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
 
 <p align="center">
 	<img src="https://raw.githubusercontent.com/NHERI-SimCenter/pelicun/gh-pages/doc_src/common/figures/pelicun-Logo-white.png"
 		alt="pelicun" align="middle" height="200"/>
 </p>
 
 <p align="center">
@@ -175,124 +180,124 @@
 
 - Dependencies
 
   - Ceiling raised for `pandas`, supporting version 2.0 and above up until 3.0.
 
 ### Changes in v3.2
 
-* Changes that might affect backwards compatibility:
+- Changes that might affect backwards compatibility:
 
-  * Unit information is included in every output file. If you parse Pelicun outputs and did not anticipate a Unit entry, your parser might need an update.
+  - Unit information is included in every output file. If you parse Pelicun outputs and did not anticipate a Unit entry, your parser might need an update.
   
-  * Decision variable types in the repair consequence outputs are named using CamelCase rather than all capitals to be consistent with other parts of the codebase. For example, we use "Cost" instead of "COST". This might affect post-processing scripts. 
+  - Decision variable types in the repair consequence outputs are named using CamelCase rather than all capitals to be consistent with other parts of the codebase. For example, we use "Cost" instead of "COST". This might affect post-processing scripts. 
   
-  * For clarity, "ea" units were replaced with "unitless" where appropriate. There should be no practical difference between the calculations due to this change. Interstory drift ratio demand types are one example.
+  - For clarity, "ea" units were replaced with "unitless" where appropriate. There should be no practical difference between the calculations due to this change. Interstory drift ratio demand types are one example.
     
-  * Weighted component block assignment is no longer supported. We recommend using more versatile multiple component definitions (see new feature below) to achieve the same effect.
+  - Weighted component block assignment is no longer supported. We recommend using more versatile multiple component definitions (see new feature below) to achieve the same effect.
     
-  * Damage functions (i.e., assign quantity of damage as a function of demand) are no longer supported. We recommend using the new multilinear CDF feature to develop theoretically equivalent, but more efficient models.
+  - Damage functions (i.e., assign quantity of damage as a function of demand) are no longer supported. We recommend using the new multilinear CDF feature to develop theoretically equivalent, but more efficient models.
 
-* New multilinear CDF Random Variable allows using the multilinear approximation of any CDF in the tool.
+- New multilinear CDF Random Variable allows using the multilinear approximation of any CDF in the tool.
 
-* Capacity adjustment allows adjusting (scaling or shifting) default capacities (i.e., fragility curves) with factors specific to each Performance Group.
+- Capacity adjustment allows adjusting (scaling or shifting) default capacities (i.e., fragility curves) with factors specific to each Performance Group.
 
-* Support for multiple definitions of the same component at the same location-direction. This feature facilitates adding components with different block sizes to the same floor or defining multiple tenants on the same floor, each with their own set of components.
+- Support for multiple definitions of the same component at the same location-direction. This feature facilitates adding components with different block sizes to the same floor or defining multiple tenants on the same floor, each with their own set of components.
 
-* Support for cloning demands, that is, taking a provided demand dataset, creating a copy and considering it as another demand. For example, you can provide results of seismic response in the X direction and automatically prepare a copy of them to represent results in the Y direction. 
+- Support for cloning demands, that is, taking a provided demand dataset, creating a copy and considering it as another demand. For example, you can provide results of seismic response in the X direction and automatically prepare a copy of them to represent results in the Y direction. 
 
-* Added a comprehensive suite of more than 140 unit tests that cover more than 93% of the codebase. Tests are automatically executed after every commit using GitHub Actions and coverage is monitored through `Codecov.io`. Badges at the top of the Readme show the status of tests and coverage. We hope this continuous integration facilitates editing and extending the existing codebase for interested members of the community.
+- Added a comprehensive suite of more than 140 unit tests that cover more than 93% of the codebase. Tests are automatically executed after every commit using GitHub Actions and coverage is monitored through `Codecov.io`. Badges at the top of the Readme show the status of tests and coverage. We hope this continuous integration facilitates editing and extending the existing codebase for interested members of the community.
 
-* Completed a review of the entire codebase using `flake8` and `pylint` to ensure PEP8 compliance. The corresponding changes yielded code that is easier to read and use. See guidance in Readme on linting and how to ensure newly added code is compliant.
+- Completed a review of the entire codebase using `flake8` and `pylint` to ensure PEP8 compliance. The corresponding changes yielded code that is easier to read and use. See guidance in Readme on linting and how to ensure newly added code is compliant.
 
-* Models for estimating Environmental Impact (i.e., embodied carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL Model Library and available in this release.
+- Models for estimating Environmental Impact (i.e., embodied carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL Model Library and available in this release.
 
-* "ListAllDamageStates" option allows you to print a comprehensive list of all possible damage states for all components in the columns of the DMG output file. This can make parsing the output easier but increases file size. By default, this option is turned off and only damage states that affect at least one block are printed.
+- "ListAllDamageStates" option allows you to print a comprehensive list of all possible damage states for all components in the columns of the DMG output file. This can make parsing the output easier but increases file size. By default, this option is turned off and only damage states that affect at least one block are printed.
 
-* Damage and Loss Model Library
+- Damage and Loss Model Library
 
-  * A collection of parameters and metadata for damage and loss models for performance based engineering. The library is available and updated regularly in the DB_DamageAndLoss GitHub Repository.
+  - A collection of parameters and metadata for damage and loss models for performance based engineering. The library is available and updated regularly in the DB_DamageAndLoss GitHub Repository.
   
-  * This and future releases of Pelicun have the latest version of the library at the time of their release bundled with them.
+  - This and future releases of Pelicun have the latest version of the library at the time of their release bundled with them.
 
-* DL_calculation tool
+- DL_calculation tool
 
-  * Support for combination of built-in and user-defined databases for damage and loss models.
+  - Support for combination of built-in and user-defined databases for damage and loss models.
   
-  * Results are now also provided in standard SimCenter `JSON` format besides the existing `CSV` tables. You can specify the preferred format in the configuration file under Output/Format. The default file format is still CSV.
+  - Results are now also provided in standard SimCenter `JSON` format besides the existing `CSV` tables. You can specify the preferred format in the configuration file under Output/Format. The default file format is still CSV.
     
-  * Support running calculations for only a subset of available consequence types.
+  - Support running calculations for only a subset of available consequence types.
 
-* Several error and warning messages added to provide more meaningful information in the log file when something goes wrong in a simulation.
+- Several error and warning messages added to provide more meaningful information in the log file when something goes wrong in a simulation.
 
-* Update dependencies to more recent versions. 
+- Update dependencies to more recent versions. 
 
-* The online documentation is significantly out of date. While we are working on an update, we recommend using the documentation of the [DL panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
+- The online documentation is significantly out of date. While we are working on an update, we recommend using the documentation of the [DL panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
 
 ### Changes in v3.1
 
-* Calculation settings are now assessment-specific. This allows you to use more than one assessments in an interactive calculation and each will have its own set of options, including log files.
+- Calculation settings are now assessment-specific. This allows you to use more than one assessments in an interactive calculation and each will have its own set of options, including log files.
 
-* The uq module was decoupled from the others to enable standalone uq calculations that work without having an active assessment.
+- The uq module was decoupled from the others to enable standalone uq calculations that work without having an active assessment.
 
-* A completely redesigned DL_calculation.py script that provides decoupled demand, damage, and loss assessment and more flexibility when setting up each of those when pelicun is used with a configuration file in a larger workflow.
+- A completely redesigned DL_calculation.py script that provides decoupled demand, damage, and loss assessment and more flexibility when setting up each of those when pelicun is used with a configuration file in a larger workflow.
 
-* Two new examples that use the DL_calculation.py script and a json configuration file were added to the example folder.
+- Two new examples that use the DL_calculation.py script and a json configuration file were added to the example folder.
 
-* A new example that demonstrates a detailed interactive calculation in a Jupyter notebook was added to the following DesignSafe project: https://www.designsafe-ci.org/data/browser/public/designsafe.storage.published/PRJ-3411v5 This project will be extended with additional examples in the future.
+- A new example that demonstrates a detailed interactive calculation in a Jupyter notebook was added to the following DesignSafe project: https://www.designsafe-ci.org/data/browser/public/designsafe.storage.published/PRJ-3411v5 This project will be extended with additional examples in the future.
 
-* Unit conversion factors moved to an external file (settings/default_units) to make it easier to add new units to the list. This also allows redefining the internal units through a complete replacement of the factors. The internal units continue to follow the SI system.
+- Unit conversion factors moved to an external file (settings/default_units) to make it easier to add new units to the list. This also allows redefining the internal units through a complete replacement of the factors. The internal units continue to follow the SI system.
 
-* Substantial improvements in coding style using flake8 and pylint to monitor and help enforce PEP8.
+- Substantial improvements in coding style using flake8 and pylint to monitor and help enforce PEP8.
 
-* Several performance improvements made calculations more efficient, especially for large problems, such as regional assessments or tall buildings investigated using the FEMA P-58 methodology.
+- Several performance improvements made calculations more efficient, especially for large problems, such as regional assessments or tall buildings investigated using the FEMA P-58 methodology.
 
-* Several bugfixes and a large number of minor changes that make the engine more robust and easier to use.
+- Several bugfixes and a large number of minor changes that make the engine more robust and easier to use.
 
-* Update recommended Python version to 3.10 and other dependencies to more recent versions. 
+- Update recommended Python version to 3.10 and other dependencies to more recent versions. 
 
 ### Changes in v3.0
 
-* The architecture was redesigned to better support interactive calculation and provide a low-level integration across all supported methods. This is the first release with the new architecture. Frequent updates are planned to provide additional examples, tests, and bugfixes in the next few months.  
+- The architecture was redesigned to better support interactive calculation and provide a low-level integration across all supported methods. This is the first release with the new architecture. Frequent updates are planned to provide additional examples, tests, and bugfixes in the next few months.  
 
-* New `assessment` module introduced to replace `control` module:
-  * Provides a high-level access to models and their methods
-  * Integrates all types of assessments into a uniform approach
-  * Most of the methods from the earlier `control` module were moved to the `model` module
+- New `assessment` module introduced to replace `control` module:
+  - Provides a high-level access to models and their methods
+  - Integrates all types of assessments into a uniform approach
+  - Most of the methods from the earlier `control` module were moved to the `model` module
   
-* Decoupled demand, damage, and loss calculations:
-  * Fragility functions and consequence functions are stored in separate files. Added new methods to the `db` module to prepare the corresponding data files and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus hurricane data will be added in a future release.
-  * Decoupling removed a large amount of redundant data from supporting databases and made the use of HDF and json files for such data unnecessary. All data are stored in easy-to-read csv files.
-  * Assessment workflows can include all three steps (i.e., demand, damage, and loss) or only one or two steps. For example, damage estimates from one analysis can drive loss calculations in another one.
+- Decoupled demand, damage, and loss calculations:
+  - Fragility functions and consequence functions are stored in separate files. Added new methods to the `db` module to prepare the corresponding data files and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus hurricane data will be added in a future release.
+  - Decoupling removed a large amount of redundant data from supporting databases and made the use of HDF and json files for such data unnecessary. All data are stored in easy-to-read csv files.
+  - Assessment workflows can include all three steps (i.e., demand, damage, and loss) or only one or two steps. For example, damage estimates from one analysis can drive loss calculations in another one.
   
-* Integrated damage and loss calculation across all methods and components:
-  * This includes phenomena such as collapse, including various collapse modes, and irreparable damage.
-  * Cascading damages and other interdependencies between various components can be introduced using a damage process file.
-  * Losses can be driven by damages or demands. The former supports the conventional damage->consequence function approach, while the latter supports the use of vulnerability functions. These can be combined within the same analysis, if needed.
-  * The same loss component can be driven by multiple types of damages. For example, replacement can be triggered by either collapse or irreparable damage.
+- Integrated damage and loss calculation across all methods and components:
+  - This includes phenomena such as collapse, including various collapse modes, and irreparable damage.
+  - Cascading damages and other interdependencies between various components can be introduced using a damage process file.
+  - Losses can be driven by damages or demands. The former supports the conventional damage->consequence function approach, while the latter supports the use of vulnerability functions. These can be combined within the same analysis, if needed.
+  - The same loss component can be driven by multiple types of damages. For example, replacement can be triggered by either collapse or irreparable damage.
 
-* Introduced *Options* in the configuration file and in the `base` module:
-  * These options handle settings that concern pelicun behavior;
-  * general preferences that might affect multiple assessment models;
-  * and settings that users would not want to change frequently.
-  * Default settings are provided in a `default_config.json` file. These can be overridden by providing any of the prescribed keys with a user-defined value assigned to them in the configuration file for an analysis.
+- Introduced *Options* in the configuration file and in the `base` module:
+  - These options handle settings that concern pelicun behavior;
+  - general preferences that might affect multiple assessment models;
+  - and settings that users would not want to change frequently.
+  - Default settings are provided in a `default_config.json` file. These can be overridden by providing any of the prescribed keys with a user-defined value assigned to them in the configuration file for an analysis.
 
-* Introduced consistent handling of units. Each csv table has a standard column to describe units of the data in it. If the standard column is missing, the table is assumed to use SI units.
+- Introduced consistent handling of units. Each csv table has a standard column to describe units of the data in it. If the standard column is missing, the table is assumed to use SI units.
 
-* Introduced consistent handling of pandas MultiIndex objects in headers and indexes. When tabular data is stored in csv files, MultiIndex objects are converted to simple indexes by concatenating the strings at each level and separating them with a `-`. This facilitates post-processing csv files in pandas without impeding post-processing those files in non-Python environments.
+- Introduced consistent handling of pandas MultiIndex objects in headers and indexes. When tabular data is stored in csv files, MultiIndex objects are converted to simple indexes by concatenating the strings at each level and separating them with a `-`. This facilitates post-processing csv files in pandas without impeding post-processing those files in non-Python environments.
 
-* Updated the DL_calculation script to support the new architecture. Currently, only the config file input is used. Other arguments were kept in the script for backwards compatibility; future updates will remove some of those arguments and introduce new ones.
+- Updated the DL_calculation script to support the new architecture. Currently, only the config file input is used. Other arguments were kept in the script for backwards compatibility; future updates will remove some of those arguments and introduce new ones.
 
-* The log files were redesigned to provide more legible and easy-to-read information about the assessment.
+- The log files were redesigned to provide more legible and easy-to-read information about the assessment.
 
 ### Changes in v2.6
 
-* Support EDPs with more than 3 characters and/or a variable in their name. For example, SA_1.0 or SA_T1
-* Support fitting normal distribution to raw EDP data (lognormal was already available)
-* Extract key settings to base.py to make them more accessible for users.
-* Minor bugfixes mostly related to hurricane storm surge assessment
+- Support EDPs with more than 3 characters and/or a variable in their name. For example, SA_1.0 or SA_T1
+- Support fitting normal distribution to raw EDP data (lognormal was already available)
+- Extract key settings to base.py to make them more accessible for users.
+- Minor bugfixes mostly related to hurricane storm surge assessment
 
 ## License
 
 `pelicun` is distributed under the BSD 3-Clause license, see LICENSE.
 
 ## Acknowledgment
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: pelicun Version: 3.3 Summary: Probabilistic
+Metadata-Version: 2.1 Name: pelicun Version: 3.3.1 Summary: Probabilistic
 Estimation of Losses, Injuries, and Community resilience Under Natural hazard
 events Home-page: http://nheri-simcenter.github.io/pelicun/ Author: Adam
 ZsarnÃ³czay Author-email: adamzs@stanford.edu License: BSD License Platform:
 any Classifier: Programming Language :: Python Classifier: Development Status
 :: 5 - Production/Stable Classifier: Natural Language :: English Classifier:
 Environment :: Console Classifier: Framework :: Jupyter Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License Classifier: Natural Language
 :: English Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
-markdown Provides-Extra: testing License-File: LICENSE
+markdown License-File: LICENSE Requires-Dist: numpy<2.0,>=1.22.0 Requires-Dist:
+scipy<2.0,>=1.7.0 Requires-Dist: pandas<3.0,>=1.4.0 Requires-Dist:
+tables>=3.7.0 Provides-Extra: testing Requires-Dist: pytest; extra == "testing"
                                    [pelicun]
       alt="DOI">[https://zenodo.org/badge/DOI/10.5281/zenodo.2558558.svg]
  PPrroobbaabbiilliissttiicc EEssttiimmaattiioonn ooff LLoosssseess,, IInnjjuurriieess,, aanndd CCoommmmuunniittyy rreessiilliieennccee UUnnddeerr
                              NNaattuurraall hhaazzaarrdd eevveennttss
 ![Tests](https://github.com/NHERI-SimCenter/pelicun/actions/workflows/
 tests.yml/badge.svg) [![codecov](https://codecov.io/github/NHERI-SimCenter/
 pelicun/branch/master/graph/badge.svg?token=W79M5FGOCG)](https://codecov.io/
@@ -139,143 +141,143 @@
 needed. - **Remove `bldg` from variable and class names**: Following the
 changes mentioned earlier, we dropped `bldg` from lables where the
 functionality is no longer limited to buildings. - **Introduce `calibrated`
 attribute for demand model**: This new attribute will allow users to check if a
 model has already been calibrated to the provided empirical data. - Several
 other minor improvements; see commit messages for details. - Dependencies -
 Ceiling raised for `pandas`, supporting version 2.0 and above up until 3.0. ###
-Changes in v3.2 * Changes that might affect backwards compatibility: * Unit
+Changes in v3.2 - Changes that might affect backwards compatibility: - Unit
 information is included in every output file. If you parse Pelicun outputs and
-did not anticipate a Unit entry, your parser might need an update. * Decision
+did not anticipate a Unit entry, your parser might need an update. - Decision
 variable types in the repair consequence outputs are named using CamelCase
 rather than all capitals to be consistent with other parts of the codebase. For
 example, we use "Cost" instead of "COST". This might affect post-processing
-scripts. * For clarity, "ea" units were replaced with "unitless" where
+scripts. - For clarity, "ea" units were replaced with "unitless" where
 appropriate. There should be no practical difference between the calculations
-due to this change. Interstory drift ratio demand types are one example. *
+due to this change. Interstory drift ratio demand types are one example. -
 Weighted component block assignment is no longer supported. We recommend using
 more versatile multiple component definitions (see new feature below) to
-achieve the same effect. * Damage functions (i.e., assign quantity of damage as
+achieve the same effect. - Damage functions (i.e., assign quantity of damage as
 a function of demand) are no longer supported. We recommend using the new
 multilinear CDF feature to develop theoretically equivalent, but more efficient
-models. * New multilinear CDF Random Variable allows using the multilinear
-approximation of any CDF in the tool. * Capacity adjustment allows adjusting
+models. - New multilinear CDF Random Variable allows using the multilinear
+approximation of any CDF in the tool. - Capacity adjustment allows adjusting
 (scaling or shifting) default capacities (i.e., fragility curves) with factors
-specific to each Performance Group. * Support for multiple definitions of the
+specific to each Performance Group. - Support for multiple definitions of the
 same component at the same location-direction. This feature facilitates adding
 components with different block sizes to the same floor or defining multiple
-tenants on the same floor, each with their own set of components. * Support for
+tenants on the same floor, each with their own set of components. - Support for
 cloning demands, that is, taking a provided demand dataset, creating a copy and
 considering it as another demand. For example, you can provide results of
 seismic response in the X direction and automatically prepare a copy of them to
-represent results in the Y direction. * Added a comprehensive suite of more
+represent results in the Y direction. - Added a comprehensive suite of more
 than 140 unit tests that cover more than 93% of the codebase. Tests are
 automatically executed after every commit using GitHub Actions and coverage is
 monitored through `Codecov.io`. Badges at the top of the Readme show the status
 of tests and coverage. We hope this continuous integration facilitates editing
-and extending the existing codebase for interested members of the community. *
+and extending the existing codebase for interested members of the community. -
 Completed a review of the entire codebase using `flake8` and `pylint` to ensure
 PEP8 compliance. The corresponding changes yielded code that is easier to read
 and use. See guidance in Readme on linting and how to ensure newly added code
-is compliant. * Models for estimating Environmental Impact (i.e., embodied
+is compliant. - Models for estimating Environmental Impact (i.e., embodied
 carbon and energy) of earthquake damage as per FEMA P-58 are included in the DL
-Model Library and available in this release. * "ListAllDamageStates" option
+Model Library and available in this release. - "ListAllDamageStates" option
 allows you to print a comprehensive list of all possible damage states for all
 components in the columns of the DMG output file. This can make parsing the
 output easier but increases file size. By default, this option is turned off
-and only damage states that affect at least one block are printed. * Damage and
-Loss Model Library * A collection of parameters and metadata for damage and
+and only damage states that affect at least one block are printed. - Damage and
+Loss Model Library - A collection of parameters and metadata for damage and
 loss models for performance based engineering. The library is available and
-updated regularly in the DB_DamageAndLoss GitHub Repository. * This and future
+updated regularly in the DB_DamageAndLoss GitHub Repository. - This and future
 releases of Pelicun have the latest version of the library at the time of their
-release bundled with them. * DL_calculation tool * Support for combination of
-built-in and user-defined databases for damage and loss models. * Results are
+release bundled with them. - DL_calculation tool - Support for combination of
+built-in and user-defined databases for damage and loss models. - Results are
 now also provided in standard SimCenter `JSON` format besides the existing
 `CSV` tables. You can specify the preferred format in the configuration file
-under Output/Format. The default file format is still CSV. * Support running
-calculations for only a subset of available consequence types. * Several error
+under Output/Format. The default file format is still CSV. - Support running
+calculations for only a subset of available consequence types. - Several error
 and warning messages added to provide more meaningful information in the log
-file when something goes wrong in a simulation. * Update dependencies to more
-recent versions. * The online documentation is significantly out of date. While
+file when something goes wrong in a simulation. - Update dependencies to more
+recent versions. - The online documentation is significantly out of date. While
 we are working on an update, we recommend using the documentation of the [DL
 panel in SimCenter's PBE Tool](https://nheri-simcenter.github.io/PBE-
 Documentation/common/user_manual/usage/desktop/PBE/Pelicun.html) as a resource.
-### Changes in v3.1 * Calculation settings are now assessment-specific. This
+### Changes in v3.1 - Calculation settings are now assessment-specific. This
 allows you to use more than one assessments in an interactive calculation and
-each will have its own set of options, including log files. * The uq module was
+each will have its own set of options, including log files. - The uq module was
 decoupled from the others to enable standalone uq calculations that work
-without having an active assessment. * A completely redesigned
+without having an active assessment. - A completely redesigned
 DL_calculation.py script that provides decoupled demand, damage, and loss
 assessment and more flexibility when setting up each of those when pelicun is
-used with a configuration file in a larger workflow. * Two new examples that
+used with a configuration file in a larger workflow. - Two new examples that
 use the DL_calculation.py script and a json configuration file were added to
-the example folder. * A new example that demonstrates a detailed interactive
+the example folder. - A new example that demonstrates a detailed interactive
 calculation in a Jupyter notebook was added to the following DesignSafe
 project: https://www.designsafe-ci.org/data/browser/public/
 designsafe.storage.published/PRJ-3411v5 This project will be extended with
-additional examples in the future. * Unit conversion factors moved to an
+additional examples in the future. - Unit conversion factors moved to an
 external file (settings/default_units) to make it easier to add new units to
 the list. This also allows redefining the internal units through a complete
 replacement of the factors. The internal units continue to follow the SI
-system. * Substantial improvements in coding style using flake8 and pylint to
-monitor and help enforce PEP8. * Several performance improvements made
+system. - Substantial improvements in coding style using flake8 and pylint to
+monitor and help enforce PEP8. - Several performance improvements made
 calculations more efficient, especially for large problems, such as regional
-assessments or tall buildings investigated using the FEMA P-58 methodology. *
+assessments or tall buildings investigated using the FEMA P-58 methodology. -
 Several bugfixes and a large number of minor changes that make the engine more
-robust and easier to use. * Update recommended Python version to 3.10 and other
-dependencies to more recent versions. ### Changes in v3.0 * The architecture
+robust and easier to use. - Update recommended Python version to 3.10 and other
+dependencies to more recent versions. ### Changes in v3.0 - The architecture
 was redesigned to better support interactive calculation and provide a low-
 level integration across all supported methods. This is the first release with
 the new architecture. Frequent updates are planned to provide additional
-examples, tests, and bugfixes in the next few months. * New `assessment` module
-introduced to replace `control` module: * Provides a high-level access to
-models and their methods * Integrates all types of assessments into a uniform
-approach * Most of the methods from the earlier `control` module were moved to
-the `model` module * Decoupled demand, damage, and loss calculations: *
+examples, tests, and bugfixes in the next few months. - New `assessment` module
+introduced to replace `control` module: - Provides a high-level access to
+models and their methods - Integrates all types of assessments into a uniform
+approach - Most of the methods from the earlier `control` module were moved to
+the `model` module - Decoupled demand, damage, and loss calculations: -
 Fragility functions and consequence functions are stored in separate files.
 Added new methods to the `db` module to prepare the corresponding data files
 and re-generated such data for FEMA P58 and Hazus earthquake assessments. Hazus
-hurricane data will be added in a future release. * Decoupling removed a large
+hurricane data will be added in a future release. - Decoupling removed a large
 amount of redundant data from supporting databases and made the use of HDF and
 json files for such data unnecessary. All data are stored in easy-to-read csv
-files. * Assessment workflows can include all three steps (i.e., demand,
+files. - Assessment workflows can include all three steps (i.e., demand,
 damage, and loss) or only one or two steps. For example, damage estimates from
-one analysis can drive loss calculations in another one. * Integrated damage
-and loss calculation across all methods and components: * This includes
+one analysis can drive loss calculations in another one. - Integrated damage
+and loss calculation across all methods and components: - This includes
 phenomena such as collapse, including various collapse modes, and irreparable
-damage. * Cascading damages and other interdependencies between various
-components can be introduced using a damage process file. * Losses can be
+damage. - Cascading damages and other interdependencies between various
+components can be introduced using a damage process file. - Losses can be
 driven by damages or demands. The former supports the conventional damage-
 >consequence function approach, while the latter supports the use of
 vulnerability functions. These can be combined within the same analysis, if
-needed. * The same loss component can be driven by multiple types of damages.
+needed. - The same loss component can be driven by multiple types of damages.
 For example, replacement can be triggered by either collapse or irreparable
-damage. * Introduced *Options* in the configuration file and in the `base`
-module: * These options handle settings that concern pelicun behavior; *
-general preferences that might affect multiple assessment models; * and
-settings that users would not want to change frequently. * Default settings are
+damage. - Introduced *Options* in the configuration file and in the `base`
+module: - These options handle settings that concern pelicun behavior; -
+general preferences that might affect multiple assessment models; - and
+settings that users would not want to change frequently. - Default settings are
 provided in a `default_config.json` file. These can be overridden by providing
 any of the prescribed keys with a user-defined value assigned to them in the
-configuration file for an analysis. * Introduced consistent handling of units.
+configuration file for an analysis. - Introduced consistent handling of units.
 Each csv table has a standard column to describe units of the data in it. If
-the standard column is missing, the table is assumed to use SI units. *
+the standard column is missing, the table is assumed to use SI units. -
 Introduced consistent handling of pandas MultiIndex objects in headers and
 indexes. When tabular data is stored in csv files, MultiIndex objects are
 converted to simple indexes by concatenating the strings at each level and
 separating them with a `-`. This facilitates post-processing csv files in
 pandas without impeding post-processing those files in non-Python environments.
-* Updated the DL_calculation script to support the new architecture. Currently,
+- Updated the DL_calculation script to support the new architecture. Currently,
 only the config file input is used. Other arguments were kept in the script for
 backwards compatibility; future updates will remove some of those arguments and
-introduce new ones. * The log files were redesigned to provide more legible and
-easy-to-read information about the assessment. ### Changes in v2.6 * Support
+introduce new ones. - The log files were redesigned to provide more legible and
+easy-to-read information about the assessment. ### Changes in v2.6 - Support
 EDPs with more than 3 characters and/or a variable in their name. For example,
-SA_1.0 or SA_T1 * Support fitting normal distribution to raw EDP data
-(lognormal was already available) * Extract key settings to base.py to make
-them more accessible for users. * Minor bugfixes mostly related to hurricane
+SA_1.0 or SA_T1 - Support fitting normal distribution to raw EDP data
+(lognormal was already available) - Extract key settings to base.py to make
+them more accessible for users. - Minor bugfixes mostly related to hurricane
 storm surge assessment ## License `pelicun` is distributed under the BSD 3-
 Clause license, see LICENSE. ## Acknowledgment This material is based upon work
 supported by the National Science Foundation under Grants No. 1612843 2131111.
 Any opinions, findings, and conclusions or recommendations expressed in this
 material are those of the authors and do not necessarily reflect the views of
 the National Science Foundation. ## Contact Adam ZsarnÃ³czay, NHERI SimCenter,
 Stanford University, adamzs@stanford.edu
```

### Comparing `pelicun-3.3/pelicun.egg-info/SOURCES.txt` & `pelicun-3.3.1/pelicun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pelicun-3.3/setup.py` & `pelicun-3.3.1/setup.py`

 * *Files identical despite different names*

