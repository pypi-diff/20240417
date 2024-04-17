# Comparing `tmp/openlane-2.0.0rc2.tar.gz` & `tmp/openlane-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlane-2.0.0rc2.tar", last modified: Sun Apr  7 19:01:48 2024, max compression
+gzip compressed data, was "openlane-2.0.0rc3.tar", last modified: Wed Apr 17 10:11:58 2024, max compression
```

## Comparing `openlane-2.0.0rc2.tar` & `openlane-2.0.0rc3.tar`

### file list

```diff
@@ -1,191 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.501187 openlane-2.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-07 19:01:48.501187 openlane-2.0.0rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.449187 openlane-2.0.0rc2/openlane/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.453187 openlane-2.0.0rc2/openlane/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/drc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/generic_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.453187 openlane-2.0.0rc2/openlane/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/metrics/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/tcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    20900 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/tpe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.457187 openlane-2.0.0rc2/openlane/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32144 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/pdk_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/removals.py
--rw-r--r--   0 runner    (1001) docker     (127)    25394 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/config/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/env_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.445187 openlane-2.0.0rc2/openlane/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.457187 openlane-2.0.0rc2/openlane/examples/spm/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm/config.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm/pin_order.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.461187 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/SPM_example.v
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/config-tut.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/defines.v
--rw-r--r--   0 runner    (1001) docker     (127)   438993 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/template.def
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.465187 openlane-2.0.0rc2/openlane/flows/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/classic.py
--rw-r--r--   0 runner    (1001) docker     (127)    15375 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    33165 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/optimizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/flows/synth_explore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.465187 openlane-2.0.0rc2/openlane/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/open_pdks_rev
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.465187 openlane-2.0.0rc2/openlane/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/base.sdc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.469187 openlane-2.0.0rc2/openlane/scripts/klayout/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/Readme.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2151 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/open_design.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3833 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/render.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5867 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/stream_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/xml_drc_report_to_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3131 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/klayout/xor.drc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.469187 openlane-2.0.0rc2/openlane/scripts/magic/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.469187 openlane-2.0.0rc2/openlane/scripts/magic/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/common/read.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.469187 openlane-2.0.0rc2/openlane/scripts/magic/def/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/def/antenna_check.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/def/mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2137 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/def/mag_gds.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2402 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/drc.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/extract_spice.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.473187 openlane-2.0.0rc2/openlane/scripts/magic/gds/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2198 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/gds/drc_batch.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/gds/erase_box.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/gds/extras_mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/gds/mag_with_pointers.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/get_bbox.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.473187 openlane-2.0.0rc2/openlane/scripts/magic/lef/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/lef/extras_maglef.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/lef/maglef.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/lef.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/magic/wrapper.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.473187 openlane-2.0.0rc2/openlane/scripts/netgen/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/netgen/setup.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.477187 openlane-2.0.0rc2/openlane/scripts/odbpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/apply_def_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/check_antenna_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/contextualize.py
--rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/defutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/diodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/disconnected_pins.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/exception_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/filter_unannotated.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/io_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/label_macro_pins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/lefutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/manual_macro_place.py
--rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/power_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/random_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/remove_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/snap_to_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/odbpy/wire_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.485187 openlane-2.0.0rc2/openlane/scripts/openroad/
--rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/antenna_check.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/antenna_repair.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      788 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/basic_mp.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.489187 openlane-2.0.0rc2/openlane/scripts/openroad/common/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/dpl.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/dpl_cell_pad.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/io.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/pdn_cfg.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/resizer.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_global_connections.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_layer_adjustments.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_power_nets.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_rc.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/common/set_routing_layers.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2658 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/cts.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/cut_rows.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/dpl.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1175 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/drt.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/fill.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     4849 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/floorplan.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2413 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/gpl.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/gui.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/insert_buffer.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1893 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/ioplacer.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/irdrop.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/pdn.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/rcx.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/repair_design.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/repair_design_postgrt.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/rsz_timing_postcts.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/rsz_timing_postgrt.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.489187 openlane-2.0.0rc2/openlane/scripts/openroad/sta/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/sta/check_macro_instances.tcl
--rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/sta/corner.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      935 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/tapcell.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      663 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/openroad/write_views.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.489187 openlane-2.0.0rc2/openlane/scripts/tclsh/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/tclsh/hello.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.489187 openlane-2.0.0rc2/openlane/scripts/yosys/
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/yosys/common.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/yosys/json_header.tcl
--rw-r--r--   0 runner    (1001) docker     (127)    14953 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/scripts/yosys/synthesize.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.493187 openlane-2.0.0rc2/openlane/state/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/state/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/state/design_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.497187 openlane-2.0.0rc2/openlane/steps/
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/common_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/cvc_rv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/klayout.py
--rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/netgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    29790 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/odb.py
--rw-r--r--   0 runner    (1001) docker     (127)    78837 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/openroad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/openroad_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/tclstep.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/verilator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/openlane/steps/yosys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.449187 openlane-2.0.0rc2/openlane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 19:01:48.000000 openlane-2.0.0rc2/openlane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:01:48.501187 openlane-2.0.0rc2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1744 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:01:48.501187 openlane-2.0.0rc2/test/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-07 18:48:52.000000 openlane-2.0.0rc2/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.033450 openlane-2.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-17 10:11:58.033450 openlane-2.0.0rc3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.969449 openlane-2.0.0rc3/openlane/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.973449 openlane-2.0.0rc3/openlane/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/drc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/generic_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.977449 openlane-2.0.0rc3/openlane/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/metrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/metrics/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/metrics/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/tcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20900 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/tpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.981449 openlane-2.0.0rc3/openlane/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32144 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/config/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/config/pdk_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/config/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/config/removals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25394 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/config/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/env_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.965449 openlane-2.0.0rc3/openlane/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.981449 openlane-2.0.0rc3/openlane/examples/spm/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm/pin_order.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.989449 openlane-2.0.0rc3/openlane/examples/spm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm/src/impl.sdc
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm/src/signoff.sdc
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm/src/spm.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.989449 openlane-2.0.0rc3/openlane/examples/spm/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm/verify/spm_tb.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.985449 openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/SPM_example.v
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/config-tut.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/defines.v
+-rw-r--r--   0 runner    (1001) docker     (127)   438993 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/template.def
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.993449 openlane-2.0.0rc3/openlane/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15375 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33165 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/optimizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/flows/synth_explore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.993449 openlane-2.0.0rc3/openlane/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/open_pdks_rev
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.993449 openlane-2.0.0rc3/openlane/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/base.sdc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.997449 openlane-2.0.0rc3/openlane/scripts/klayout/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/klayout/Readme.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2151 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/klayout/open_design.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3833 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/klayout/render.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5867 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/klayout/stream_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/klayout/xml_drc_report_to_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3131 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/klayout/xor.drc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.997449 openlane-2.0.0rc3/openlane/scripts/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.997449 openlane-2.0.0rc3/openlane/scripts/magic/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/common/read.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.997449 openlane-2.0.0rc3/openlane/scripts/magic/def/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/def/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/def/mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2137 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/def/mag_gds.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2402 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/drc.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/extract_spice.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.001449 openlane-2.0.0rc3/openlane/scripts/magic/gds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2198 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/gds/drc_batch.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/gds/erase_box.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/gds/extras_mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/gds/mag_with_pointers.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/get_bbox.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.001449 openlane-2.0.0rc3/openlane/scripts/magic/lef/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/lef/extras_maglef.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/lef/maglef.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/lef.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/magic/wrapper.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.001449 openlane-2.0.0rc3/openlane/scripts/netgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/netgen/setup.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.009449 openlane-2.0.0rc3/openlane/scripts/odbpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/apply_def_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/check_antenna_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/contextualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/defutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/diodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10669 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/disconnected_pins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/exception_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/filter_unannotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/io_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/label_macro_pins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/lefutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/manual_macro_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/power_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/random_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/remove_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/snap_to_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/odbpy/wire_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.017449 openlane-2.0.0rc3/openlane/scripts/openroad/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/antenna_repair.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      788 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/basic_mp.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.021449 openlane-2.0.0rc3/openlane/scripts/openroad/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/dpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/dpl_cell_pad.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/io.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/pdn_cfg.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/resizer.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/set_global_connections.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/set_layer_adjustments.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/set_power_nets.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/set_rc.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/common/set_routing_layers.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2658 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/cts.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/cut_rows.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/dpl.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1175 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/drt.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/fill.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4849 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/floorplan.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2413 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/gpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/gui.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/insert_buffer.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1893 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/ioplacer.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/irdrop.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/pdn.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/rcx.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/repair_design.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/repair_design_postgrt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/rsz_timing_postcts.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/rsz_timing_postgrt.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.021449 openlane-2.0.0rc3/openlane/scripts/openroad/sta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/sta/check_macro_instances.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/sta/corner.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      935 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/tapcell.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      663 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/openroad/write_views.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.025450 openlane-2.0.0rc3/openlane/scripts/tclsh/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/tclsh/hello.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.025450 openlane-2.0.0rc3/openlane/scripts/yosys/
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/yosys/common.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/yosys/construct_abc_script.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/yosys/json_header.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/scripts/yosys/synthesize.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.025450 openlane-2.0.0rc3/openlane/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/state/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/state/design_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.033450 openlane-2.0.0rc3/openlane/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/common_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/cvc_rv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16425 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/klayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/netgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29518 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/odb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81035 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/openroad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/openroad_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53312 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/tclstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/verilator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/openlane/steps/yosys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:57.969449 openlane-2.0.0rc3/openlane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-17 10:11:57.000000 openlane-2.0.0rc3/openlane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-17 10:11:57.000000 openlane-2.0.0rc3/openlane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:11:57.000000 openlane-2.0.0rc3/openlane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-17 10:11:57.000000 openlane-2.0.0rc3/openlane.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 10:11:57.000000 openlane-2.0.0rc3/openlane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 10:11:57.000000 openlane-2.0.0rc3/openlane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:11:58.033450 openlane-2.0.0rc3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1776 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:11:58.033450 openlane-2.0.0rc3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-17 10:01:48.000000 openlane-2.0.0rc3/test/conftest.py
```

### Comparing `openlane-2.0.0rc2/PKG-INFO` & `openlane-2.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized, but some oddities are still to be expected. Proceed with caution.
         >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0rc2 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0rc3 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized,
 but some oddities are still to be expected. Proceed with caution. > > If you
 *don't* know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ************ OOppeennLLaannee ************
```

### Comparing `openlane-2.0.0rc2/openlane/__init__.py` & `openlane-2.0.0rc3/openlane/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/__main__.py` & `openlane-2.0.0rc3/openlane/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/__version__.py` & `openlane-2.0.0rc3/openlane/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "2.0.0rc2"
+__version__ = "2.0.0rc3"
 
 if __name__ == "__main__":
     print(__version__, end="")
```

### Comparing `openlane-2.0.0rc2/openlane/common/__init__.py` & `openlane-2.0.0rc3/openlane/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/cli.py` & `openlane-2.0.0rc3/openlane/common/cli.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/drc.py` & `openlane-2.0.0rc3/openlane/common/drc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/generic_dict.py` & `openlane-2.0.0rc3/openlane/common/generic_dict.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/metrics/__init__.py` & `openlane-2.0.0rc3/openlane/common/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/metrics/__main__.py` & `openlane-2.0.0rc3/openlane/common/metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/metrics/library.py` & `openlane-2.0.0rc3/openlane/common/metrics/library.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/metrics/metric.py` & `openlane-2.0.0rc3/openlane/common/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/metrics/util.py` & `openlane-2.0.0rc3/openlane/common/metrics/util.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/misc.py` & `openlane-2.0.0rc3/openlane/common/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/ring_buffer.py` & `openlane-2.0.0rc3/openlane/common/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/tcl.py` & `openlane-2.0.0rc3/openlane/common/tcl.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/toolbox.py` & `openlane-2.0.0rc3/openlane/common/toolbox.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/tpe.py` & `openlane-2.0.0rc3/openlane/common/tpe.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/common/types.py` & `openlane-2.0.0rc3/openlane/common/types.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/config/__init__.py` & `openlane-2.0.0rc3/openlane/config/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/config/__main__.py` & `openlane-2.0.0rc3/openlane/config/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/config/config.py` & `openlane-2.0.0rc3/openlane/config/config.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/config/flow.py` & `openlane-2.0.0rc3/openlane/config/flow.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/config/pdk_compat.py` & `openlane-2.0.0rc3/openlane/config/pdk_compat.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/config/preprocessor.py` & `openlane-2.0.0rc3/openlane/config/preprocessor.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/config/removals.py` & `openlane-2.0.0rc3/openlane/config/removals.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/config/variable.py` & `openlane-2.0.0rc3/openlane/config/variable.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/container.py` & `openlane-2.0.0rc3/openlane/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,42 +14,34 @@
 
 ## This file is internal to OpenLane 2 and is not part of the API.
 import os
 import re
 import httpx
 import shlex
 import pathlib
-import getpass
 import tempfile
 import subprocess
 from typing import List, Sequence, Optional, Union, Tuple
 
+from .common import mkdirp
 from .logging import err, info, warn
 from .env_info import OSInfo
 
 CONTAINER_ENGINE = os.getenv("OPENLANE_CONTAINER_ENGINE", "docker")
 
 
 def permission_args(osinfo: OSInfo) -> List[str]:
     if (
         osinfo.kernel == "Linux"
         and osinfo.container_info is not None
         and osinfo.container_info.engine == "docker"
         and not osinfo.container_info.rootless
     ):
-        uid = (
-            subprocess.check_output(["id", "-u", getpass.getuser()])
-            .decode("utf8")
-            .strip()
-        )
-        gid = (
-            subprocess.check_output(["id", "-g", getpass.getuser()])
-            .decode("utf8")
-            .strip()
-        )
+        uid = os.getuid()
+        gid = os.getgid()
 
         return ["--user", f"{uid}:{gid}"]
 
     return []
 
 
 def gui_args(osinfo: OSInfo) -> List[str]:
@@ -189,14 +181,20 @@
 
     mount_args = []
     from_home, to_home = sanitize_path(pathlib.Path.home())
 
     mount_args += ["-v", f"{from_home}:{to_home}"]
 
     from_pdk, to_pdk = sanitize_path(volare.get_volare_home(pdk_root))
+
+    try:
+        mkdirp(from_pdk)
+    except FileExistsError:
+        raise ValueError(f"Invalid PDK root: '{from_pdk}' is a file")
+
     mount_args += [
         "-v",
         f"{from_pdk}:{to_pdk}",
         "-e",
         f"PDK_ROOT={to_pdk}",
     ]
 
@@ -224,14 +222,15 @@
     ]
 
     if other_mounts is not None:
         for mount in other_mounts:
             if os.path.isdir(mount):
                 mount_from, mount_to = sanitize_path(mount)
                 mount_args += ["-v", f"{mount_from}:{mount_to}"]
+                mkdirp(mount_from)
             else:
                 mount_args += ["-v", f"{mount}"]
 
     cmd = (
         [
             CONTAINER_ENGINE,
             "run",
```

### Comparing `openlane-2.0.0rc2/openlane/env_info.py` & `openlane-2.0.0rc3/openlane/env_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 # with ancient versions of Python.
 
 ## This file is internal to OpenLane 2 and is not part of the API.
 import os
 import re
 import sys
 import json
+import tempfile
 import platform
 import subprocess
 
 try:
-    from typing import Optional, Dict, List, Any  # noqa: F401
+    from typing import Optional, Dict, List  # noqa: F401
 except ImportError:
     pass
 
 CONTAINER_ENGINE = os.getenv("OPENLANE_CONTAINER_ENGINE", "docker")
 
 
 class StringRepresentable(object):
@@ -109,61 +110,77 @@
             return cinfo
         except Exception as e:
             print(e, file=sys.stderr)
             return None
 
 
 class NixInfo(StringRepresentable):
-    version = ""  # type: str
-    multi_user = False  # type: bool
-    sandbox = False  # type: bool
-    channels = None  # type: Optional[Dict[str, List[str]]]
-    nixpkgs = ""  # type: str
+    version_string = ""  # type: str
+    channels = None  # type: Optional[Dict[str, str]]
+    nix_command = False  # type: bool
+    flakes = False  # type: bool
 
     def __init__(self) -> None:
-        self.version = ""  # type: str
-        self.multi_user = False  # type: bool
-        self.sandbox = False  # type: bool
-        self.channels = None  # type: Optional[Dict[str, List[str]]]
-        self.nixpkgs = ""  # type: str
+        self.version_string = ""
+        self.channels = None
+        self.nix_command = False
+        self.flakes = False
 
     @staticmethod
     def get():
         # type: () -> Optional['NixInfo']
         ninfo = NixInfo()
-
         try:
             try:
-                info_str = subprocess.check_output(
-                    ["nix-shell", "-p", "nix-info", "--run", "nix-info -m"]
-                ).decode("utf8")
+                version_str = subprocess.check_output(
+                    ["nix", "--version"], encoding="utf8"
+                )
+                ninfo.version_string = version_str.strip()
             except Exception as e:
-                raise Exception("Failed to get Docker info: %s" % str(e)) from None
+                raise Exception("Failed to get Nix info: %s" % str(e)) from None
 
-            for line in info_str.splitlines():
-                if line.strip() == "":
-                    continue
-                line = line[3:]
-                key, value_raw = line.split(": ", maxsplit=1)
-                key = key.strip(" -")
-                value = value_raw.strip(' `"')  # type: Any
-                if value == "yes":
-                    value = True
-                elif value == "no":
-                    value = False
-                if key in ninfo.__dict__:
-                    setattr(ninfo, key, value)
-                elif key.startswith("channels"):
-                    user = key[len("channels") + 1 : -1]
-                    ninfo.channels = ninfo.channels or {}
-                    ninfo.channels[user] = [
-                        el.strip() for el in value.split(",") if el.strip() != ""
-                    ]
-                elif key.startswith("multi-user"):
-                    ninfo.multi_user = value
+            try:
+                channels = {}
+                channels_raw = subprocess.check_output(
+                    ["nix-channel", "--list"], encoding="utf8"
+                )
+                for channel in channels_raw.splitlines():
+                    name, url = channel.split(maxsplit=1)
+                    channels[name] = url
+                ninfo.channels = channels
+            except Exception as e:
+                print(
+                    "Failed to get nix channels: %s" % str(e),
+                    file=sys.stderr,
+                )
+
+            with tempfile.TemporaryDirectory("ol-env-rpt") as d:
+                with open(os.path.join(d, "flake.nix"), "w") as f:
+                    f.write("{}")
+                nix_command = subprocess.run(
+                    ["nix", "eval"],
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.STDOUT,
+                    cwd=d,
+                    encoding="utf8",
+                )
+                nix_command_result = nix_command.stdout
+                if "'nix-command'" in nix_command_result:
+                    pass
+                elif "'flakes'" in nix_command_result:
+                    ninfo.nix_command = True
+                elif "lacks attribute" in nix_command_result:
+                    ninfo.nix_command = True
+                    ninfo.flakes = True
+                else:
+                    print(
+                        "'nix flake' returned unexpected output: %s"
+                        % nix_command_result,
+                        file=sys.stderr,
+                    )
 
             return ninfo
         except Exception as e:
             print(e, file=sys.stderr)
             return None
 
 
@@ -179,15 +196,15 @@
     nix_info = None  # type: Optional[NixInfo]
 
     def __init__(self):
         self.kernel = platform.system()
         self.kernel_version = (
             platform.release()
         )  # Unintuitively enough, it's the kernel's release
-        self.supported = self.kernel in ["Darwin", "Linux", "Windows"]
+        self.supported = self.kernel in ["Darwin", "Linux"]
         self.distro = None
         self.distro_version = None
         self.python_version = platform.python_version()
         self.python_path = sys.path.copy()
         self.tkinter = False
         try:
             import tkinter  # noqa: F401
```

### Comparing `openlane-2.0.0rc2/openlane/examples/spm/config.json` & `openlane-2.0.0rc3/openlane/examples/spm/config.json`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/SPM_example.v` & `openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/SPM_example.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc` & `openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/defines.v` & `openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/defines.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/template.def` & `openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/template.def`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v` & `openlane-2.0.0rc3/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/__init__.py` & `openlane-2.0.0rc3/openlane/flows/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/builtins.py` & `openlane-2.0.0rc3/openlane/flows/builtins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/classic.py` & `openlane-2.0.0rc3/openlane/flows/classic.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/cli.py` & `openlane-2.0.0rc3/openlane/flows/cli.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/flow.py` & `openlane-2.0.0rc3/openlane/flows/flow.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/misc.py` & `openlane-2.0.0rc3/openlane/flows/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/optimizing.py` & `openlane-2.0.0rc3/openlane/flows/optimizing.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/sequential.py` & `openlane-2.0.0rc3/openlane/flows/sequential.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/flows/synth_explore.py` & `openlane-2.0.0rc3/openlane/flows/synth_explore.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/logging/__init__.py` & `openlane-2.0.0rc3/openlane/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/logging/logger.py` & `openlane-2.0.0rc3/openlane/logging/logger.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/plugins.py` & `openlane-2.0.0rc3/openlane/plugins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/base.sdc` & `openlane-2.0.0rc3/openlane/examples/spm/src/impl.sdc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/klayout/open_design.py` & `openlane-2.0.0rc3/openlane/scripts/klayout/open_design.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/klayout/render.py` & `openlane-2.0.0rc3/openlane/scripts/klayout/render.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/klayout/stream_out.py` & `openlane-2.0.0rc3/openlane/scripts/klayout/stream_out.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/klayout/xml_drc_report_to_json.py` & `openlane-2.0.0rc3/openlane/scripts/klayout/xml_drc_report_to_json.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/klayout/xor.drc` & `openlane-2.0.0rc3/openlane/scripts/klayout/xor.drc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/common/read.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/common/read.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/def/antenna_check.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/def/antenna_check.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/def/mag.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/def/mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/def/mag_gds.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/def/mag_gds.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/drc.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/drc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/extract_spice.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/extract_spice.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/gds/drc_batch.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/gds/drc_batch.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/gds/erase_box.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/gds/erase_box.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/gds/extras_mag.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/gds/extras_mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/gds/mag_with_pointers.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/gds/mag_with_pointers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/lef/extras_maglef.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/lef/extras_maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/lef/maglef.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/lef/maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/lef.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/lef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/magic/wrapper.tcl` & `openlane-2.0.0rc3/openlane/scripts/magic/wrapper.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/apply_def_template.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/apply_def_template.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/check_antenna_properties.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/check_antenna_properties.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/contextualize.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/contextualize.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/defutil.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/defutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/diodes.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/diodes.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/disconnected_pins.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/disconnected_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/exception_codes.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/exception_codes.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/filter_unannotated.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/filter_unannotated.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/io_place.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/io_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/label_macro_pins.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/label_macro_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/lefutil.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/lefutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/manual_macro_place.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/manual_macro_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/power_utils.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/power_utils.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/random_place.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/random_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/reader.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/reader.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/remove_buffers.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/remove_buffers.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/snap_to_grid.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/snap_to_grid.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/odbpy/wire_lengths.py` & `openlane-2.0.0rc3/openlane/scripts/odbpy/wire_lengths.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/antenna_check.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/antenna_check.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/antenna_repair.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/antenna_repair.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/basic_mp.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/basic_mp.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/dpl.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/dpl_cell_pad.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/dpl_cell_pad.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/grt.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/io.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/io.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/pdn_cfg.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/pdn_cfg.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/resizer.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/resizer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_global_connections.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/set_global_connections.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_layer_adjustments.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/set_layer_adjustments.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_power_nets.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/set_power_nets.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_rc.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/set_rc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/common/set_routing_layers.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/common/set_routing_layers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/cts.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/cts.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/cut_rows.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/cut_rows.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/dpl.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/drt.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/drt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/fill.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/fill.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/floorplan.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/floorplan.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/gpl.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/gpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/grt.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/gui.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/gui.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/insert_buffer.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/insert_buffer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/ioplacer.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/ioplacer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/irdrop.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/irdrop.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/pdn.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/pdn.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/rcx.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/rcx.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/repair_design.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/repair_design.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/repair_design_postgrt.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/repair_design_postgrt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/rsz_timing_postcts.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/rsz_timing_postcts.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/rsz_timing_postgrt.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/rsz_timing_postgrt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/sta/check_macro_instances.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/sta/check_macro_instances.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/sta/corner.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/sta/corner.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/tapcell.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/tapcell.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/openroad/write_views.tcl` & `openlane-2.0.0rc3/openlane/scripts/openroad/write_views.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/scripts/yosys/json_header.tcl` & `openlane-2.0.0rc3/openlane/scripts/yosys/json_header.tcl`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 yosys -import
 source $::env(SCRIPTS_DIR)/yosys/common.tcl
-set vtop $::env(DESIGN_NAME)
 
 source $::env(_DEPS_SCRIPT)
 
-read_verilog_files $vtop
-hierarchy -check -top $vtop
-yosys rename -top $vtop
+yosys_ol::read_verilog_files $::env(DESIGN_NAME)
+hierarchy -check -top $::env(DESIGN_NAME) -nokeep_prints -nokeep_asserts
+yosys rename -top $::env(DESIGN_NAME)
 yosys proc
 json -o $::env(SAVE_JSON_HEADER)
```

### Comparing `openlane-2.0.0rc2/openlane/state/__init__.py` & `openlane-2.0.0rc3/openlane/state/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/state/__main__.py` & `openlane-2.0.0rc3/openlane/state/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/state/design_format.py` & `openlane-2.0.0rc3/openlane/state/design_format.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/state/state.py` & `openlane-2.0.0rc3/openlane/state/state.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/__init__.py` & `openlane-2.0.0rc3/openlane/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/__main__.py` & `openlane-2.0.0rc3/openlane/steps/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/checker.py` & `openlane-2.0.0rc3/openlane/steps/checker.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/common_variables.py` & `openlane-2.0.0rc3/openlane/steps/common_variables.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/cvc_rv.py` & `openlane-2.0.0rc3/openlane/steps/cvc_rv.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/klayout.py` & `openlane-2.0.0rc3/openlane/steps/klayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
-import shlex
 import sys
 import site
+import shlex
 import shutil
 import subprocess
 from os.path import abspath
 from base64 import b64encode
 from typing import Any, Dict, Optional, List, Sequence, Tuple, Union
 
 from .step import ViewsUpdate, MetricsUpdate, Step, StepError, StepException
@@ -47,25 +47,25 @@
             "KLAYOUT_DEF_LAYER_MAP",
             Path,
             "A path to the KLayout LEF/DEF layer mapping (.map) file.",
             pdk=True,
         ),
     ]
 
-    def run_subprocess(
+    def run_pya_script(
         self,
         cmd: Sequence[Union[str, os.PathLike]],
         log_to: Optional[Union[str, os.PathLike]] = None,
         silent: bool = False,
         report_dir: Optional[Union[str, os.PathLike]] = None,
         env: Optional[Dict[str, Any]] = None,
         **kwargs,
     ) -> Dict[str, Any]:
         env = env or os.environ.copy()
-        # Hack for Python subprocesses to get access to installed libraries
+        # Pass site packages
         python_path_elements = site.getsitepackages() + sys.path
         if current_pythonpath := env.get("PYTHONPATH"):
             python_path_elements.append(current_pythonpath)
 
         env["PYTHONPATH"] = ":".join(python_path_elements)
         return super().run_subprocess(cmd, log_to, silent, report_dir, env, **kwargs)
 
@@ -150,15 +150,15 @@
     def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         input_view = state_in[DesignFormat.DEF]
         if gds := state_in[DesignFormat.GDS]:
             input_view = gds
 
         assert isinstance(input_view, Path)
 
-        self.run_subprocess(
+        self.run_pya_script(
             [
                 sys.executable,
                 os.path.join(get_script_dir(), "klayout", "render.py"),
                 abspath(input_view),
                 "--output",
                 abspath(os.path.join(self.step_dir, "out.png")),
             ]
@@ -193,15 +193,15 @@
 
         klayout_gds_out = os.path.join(
             self.step_dir,
             f"{self.config['DESIGN_NAME']}.{DesignFormat.KLAYOUT_GDS.value.extension}",
         )
         kwargs, env = self.extract_env(kwargs)
 
-        self.run_subprocess(
+        self.run_pya_script(
             [
                 sys.executable,
                 os.path.join(
                     get_script_dir(),
                     "klayout",
                     "stream_out.py",
                 ),
@@ -373,14 +373,15 @@
         seal = str(self.config["KLAYOUT_DRC_OPTIONS"]["seal"]).lower()
         threads = self.config["KLAYOUT_DRC_THREADS"] or (str(os.cpu_count()) or "1")
         info(f"Running KLayout DRC with {threads} threads…")
 
         input_view = state_in[DesignFormat.GDS]
         assert isinstance(input_view, Path)
 
+        # Not pya script - DRC script is not part of OpenLane
         self.run_subprocess(
             [
                 "klayout",
                 "-b",
                 "-zz",
                 "-r",
                 drc_script_path,
@@ -402,15 +403,15 @@
                 f"seal={seal}",
                 "-rd",
                 f"threads={threads}",
             ],
             env=env,
         )
 
-        subprocess_result = self.run_subprocess(
+        subprocess_result = self.run_pya_script(
             [
                 "python3",
                 os.path.join(
                     get_script_dir(),
                     "klayout",
                     "xml_drc_report_to_json.py",
                 ),
@@ -492,14 +493,16 @@
                     get_script_dir(),
                     "klayout",
                     "open_design.py",
                 ),
             ]
         )
 
+        # Not run_subprocess- need stdin, stdout, stderr to be accessible to the
+        # user normally
         subprocess.check_call(
             cmd,
             env=env,
             cwd=self.step_dir,
         )
 
         return {}, {}
```

### Comparing `openlane-2.0.0rc2/openlane/steps/magic.py` & `openlane-2.0.0rc3/openlane/steps/magic.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/misc.py` & `openlane-2.0.0rc3/openlane/steps/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/netgen.py` & `openlane-2.0.0rc3/openlane/steps/netgen.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/odb.py` & `openlane-2.0.0rc3/openlane/steps/odb.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
-import sys
 import json
-import site
 import shutil
 from math import inf
 from decimal import Decimal
 from functools import reduce
 from abc import abstractmethod
 from typing import List, Literal, Optional, Tuple
 
@@ -80,19 +78,15 @@
             command.append(file_path)
             views_updates[output] = Path(file_path)
 
         command += [
             str(state_in[DesignFormat.ODB]),
         ]
 
-        python_path_elements = site.getsitepackages() + sys.path
-        if current_pythonpath := env.get("PYTHONPATH"):
-            python_path_elements.append(current_pythonpath)
-        python_path_elements.append(os.path.join(get_script_dir(), "odbpy"))
-        env["PYTHONPATH"] = ":".join(python_path_elements)
+        env["PYTHONPATH"] = os.path.join(get_script_dir(), "odbpy")
 
         subprocess_result = self.run_subprocess(
             command,
             env=env,
             **kwargs,
         )
```

### Comparing `openlane-2.0.0rc2/openlane/steps/openroad.py` & `openlane-2.0.0rc3/openlane/steps/openroad.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import os
 import re
-import sys
 import json
-import site
 import tempfile
 import functools
 import subprocess
 from enum import Enum
 from math import inf
 from glob import glob
 from decimal import Decimal
 from base64 import b64encode
 from abc import abstractmethod
+from dataclasses import dataclass
 from concurrent.futures import Future
 from typing import (
     Any,
     List,
     Dict,
     Literal,
     Set,
@@ -247,20 +246,14 @@
             self.toolbox.get_macro_views(self.config, DesignFormat.LIB)
         )
 
         excluded_cells: Set[str] = set(self.config["EXTRA_EXCLUDED_CELLS"] or [])
         excluded_cells.update(process_list_file(self.config["PNR_EXCLUDED_CELL_FILE"]))
         env["_PNR_EXCLUDED_CELLS"] = TclUtils.join(excluded_cells)
 
-        python_path_elements = site.getsitepackages() + sys.path
-        if current_pythonpath := env.get("PYTHONPATH"):
-            python_path_elements.append(current_pythonpath)
-        python_path_elements.append(os.path.join(get_script_dir(), "odbpy"))
-        env["PYTHONPATH"] = ":".join(python_path_elements)
-
         return env
 
     def run(self, state_in, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         """
         The `run()` override for the OpenROADStep class handles two things:
 
         1. Before the `super()` call: It creates a version of the lib file
@@ -348,172 +341,153 @@
         if image := self.toolbox.render_png(self.config, self.state_out):
             image_encoded = b64encode(image).decode("utf8")
             return f'<img src="data:image/png;base64,{image_encoded}" />'
 
         return None
 
 
-class STAStep(OpenROADStep):
-    """
-    Abstract class for an STA step
-    """
-
-    def layout_preview(self) -> Optional[str]:
-        return None
-
-    def get_script_path(self):
-        return os.path.join(get_script_dir(), "openroad", "sta", "corner.tcl")
-
-
 @Step.factory.register()
-class STAMidPNR(STAStep):
+class STAMidPNR(OpenROADStep):
     """
     Performs `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
-    using OpenROAD on an OpenROAD database, mid-PnR.
+    using OpenROAD on an OpenROAD database, mid-PnR, with estimated values for
+    parasitics.
     """
 
     id = "OpenROAD.STAMidPNR"
     name = "STA (Mid-PnR)"
     long_name = "Static Timing Analysis (Mid-PnR)"
 
     inputs = [DesignFormat.ODB]
     outputs = []
 
-
-def _set_corner_files(
-    step: Step,
-    env: Dict[str, Any],
-    timing_corner: Optional[str] = None,
-    prioritize_nl: bool = False,
-):
-    (
-        timing_corner,
-        libs,
-        netlists,
-        spefs,
-    ) = step.toolbox.get_timing_files_categorized(
-        step.config,
-        prioritize_nl=prioritize_nl,
-        timing_corner=timing_corner,
-    )
-
-    env["_CURRENT_CORNER_NAME"] = timing_corner
-    if extra_spef_list := step.config.get("EXTRA_SPEFS"):
-        extra_spef_pairs = []
-        step.warn(
-            "The configuration variable 'EXTRA_SPEFS' is deprecated. It is recommended to use the new 'MACROS' configuration variable."
-        )
-        if len(extra_spef_list) % 4 != 0:
-            raise StepException(
-                "Invalid value for 'EXTRA_SPEFS': Element count not divisible by four. It is recommended that you migrate your configuration to use the new 'MACROS' configuration variable."
-            )
-        for i in range(len(extra_spef_list) // 4):
-            start = i * 4
-            module, min, nom, max = (
-                extra_spef_list[start],
-                extra_spef_list[start + 1],
-                extra_spef_list[start + 2],
-                extra_spef_list[start + 3],
-            )
-            mapping = {
-                "min_*": [min],
-                "nom_*": [nom],
-                "max_*": [max],
-            }
-            spef = str(
-                step.toolbox.filter_views(
-                    step.config, mapping, timing_corner=timing_corner
-                )[0]
-            )
-            extra_spef_pairs.append((module, spef))
-        env["_CURRENT_CORNER_EXTRA_SPEFS_BACKCOMPAT"] = TclStep.value_to_tcl(
-            extra_spef_pairs
-        )
-
-    env["_CURRENT_CORNER_LIBS"] = TclStep.value_to_tcl(libs)
-    env["_CURRENT_CORNER_NETLISTS"] = TclStep.value_to_tcl(netlists)
-    env["_CURRENT_CORNER_SPEFS"] = TclStep.value_to_tcl(spefs)
+    def get_script_path(self):
+        return os.path.join(get_script_dir(), "openroad", "sta", "corner.tcl")
 
 
-@Step.factory.register()
-class STAPrePNR(STAStep):
-    """
-    Performs hierarchical `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
-    using OpenSTA on the pre-PnR Verilog netlist, with all available timing information
-    for standard cells and macros for the default timing corner as specified in
-    the ``DEFAULT_CORNER`` variable.
-
-    If timing information is not available for macros, the macro in question
-    will be black-boxed.
-    """
+class OpenSTAStep(OpenROADStep):
+    @dataclass(frozen=True)
+    class CornerFileList:
+        libs: Tuple[str, ...]
+        netlists: Tuple[str, ...]
+        spefs: Tuple[Tuple[str, str], ...]
+        extra_spefs_backcompat: Optional[Tuple[Tuple[str, str], ...]] = None
+        current_corner_spef: Optional[str] = None
+
+        def set_env(self, env: Dict[str, Any]):
+            env["_CURRENT_CORNER_LIBS"] = TclStep.value_to_tcl(self.libs)
+            env["_CURRENT_CORNER_NETLISTS"] = TclStep.value_to_tcl(self.netlists)
+            env["_CURRENT_CORNER_SPEFS"] = TclStep.value_to_tcl(self.spefs)
+            if self.extra_spefs_backcompat is not None:
+                env["_CURRENT_CORNER_EXTRA_SPEFS_BACKCOMPAT"] = TclStep.value_to_tcl(
+                    self.extra_spefs_backcompat
+                )
+            if self.current_corner_spef is not None:
+                env["_CURRENT_SPEF_BY_CORNER"] = self.current_corner_spef
 
     inputs = [DesignFormat.NETLIST]
-    outputs = [DesignFormat.SDF, DesignFormat.SDC]
-
-    id = "OpenROAD.STAPrePNR"
-    name = "STA (Pre-PnR)"
-    long_name = "Static Timing Analysis"
-
-    config_vars = STAStep.config_vars + [
-        Variable(
-            "STA_MACRO_PRIORITIZE_NL",
-            bool,
-            "Prioritize the use of Netlists + SPEF files over LIB files if available for Macros. Useful if extraction was done using OpenROAD, where SPEF files are far more accurate.",
-            default=True,
-        ),
-        Variable(
-            "STA_MAX_VIOLATOR_COUNT",
-            Optional[int],
-            "Maximum number of violators to list in violator_list.rpt",
-        ),
-        Variable(
-            "EXTRA_SPEFS",
-            Optional[List[Union[str, Path]]],
-            "A variable that only exists for backwards compatibility with OpenLane <2.0.0 and should not be used by new designs.",
-        ),
-    ]
 
     def get_command(self) -> List[str]:
         return ["sta", "-no_splash", "-exit", self.get_script_path()]
 
-    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
-        kwargs, env = self.extract_env(kwargs)
-
-        prioritize_nl: Optional[bool] = self.config.get("STA_MACRO_PRIORITIZE_NL")
-        if prioritize_nl is None:
-            if "prioritize_nl" in kwargs:
-                prioritize_nl = bool(kwargs.pop("prioritize_nl"))
-            else:
-                prioritize_nl = False
-
-        _set_corner_files(self, env, prioritize_nl=prioritize_nl)
-
+    def prepare_env(self, env: Dict, state: State) -> Dict:
+        env = super().prepare_env(env, state)
         env["_OPENSTA"] = "1"
-        env["_SDF_SAVE_DIR"] = self.step_dir
+        return env
 
-        views_updates, metrics_updates = super().run(state_in, env=env, **kwargs)
+    def layout_preview(self) -> Optional[str]:
+        return None
 
-        sdf_dict = state_in[DesignFormat.SDF] or {}
-        if not isinstance(sdf_dict, dict):
-            raise StepException(
-                "Malformed input state: value for LIB is not a dictionary."
-            )
+    def _get_corner_files(
+        self: Step,
+        timing_corner: Optional[str] = None,
+        prioritize_nl: bool = False,
+    ) -> Tuple[str, CornerFileList]:
+        (
+            timing_corner,
+            libs,
+            netlists,
+            spefs,
+        ) = self.toolbox.get_timing_files_categorized(
+            self.config,
+            prioritize_nl=prioritize_nl,
+            timing_corner=timing_corner,
+        )
+        state_in = self.state_in.result()
 
-        sdfs = sorted(glob(os.path.join(self.step_dir, "*.sdf")))
-        for sdf in sdfs:
-            _, corner = os.path.basename(sdf)[:-4].split("__")
-            sdf_dict[corner] = Path(sdf)
+        name = timing_corner
+        current_corner_spef = None
+        input_spef_dict = state_in[DesignFormat.SPEF]
+        if input_spef_dict is not None:
+            if not isinstance(input_spef_dict, dict):
+                raise StepException(
+                    "Malformed input state: value for 'spef' is not a dictionary"
+                )
 
-        views_updates[DesignFormat.SDF] = sdf_dict
+            current_corner_spefs = self.toolbox.filter_views(
+                self.config, input_spef_dict, timing_corner
+            )
+            if len(current_corner_spefs) < 1:
+                raise StepException(
+                    f"No SPEF file compatible with corner '{timing_corner}' found."
+                )
+            elif len(current_corner_spefs) > 1:
+                self.warn(
+                    f"Multiple SPEF files compatible with corner '{timing_corner}' found. The first one encountered will be used."
+                )
+            current_corner_spef = str(current_corner_spefs[0])
 
-        return views_updates, metrics_updates
+        extra_spefs_backcompat_raw = None
+        if extra_spef_list := self.config.get("EXTRA_SPEFS"):
+            extra_spefs_backcompat_raw = []
+            self.warn(
+                "The configuration variable 'EXTRA_SPEFS' is deprecated. It is recommended to use the new 'MACROS' configuration variable."
+            )
+            if len(extra_spef_list) % 4 != 0:
+                raise StepException(
+                    "Invalid value for 'EXTRA_SPEFS': Element count not divisible by four. It is recommended that you migrate your configuration to use the new 'MACROS' configuration variable."
+                )
+            for i in range(len(extra_spef_list) // 4):
+                start = i * 4
+                module, min, nom, max = (
+                    extra_spef_list[start],
+                    extra_spef_list[start + 1],
+                    extra_spef_list[start + 2],
+                    extra_spef_list[start + 3],
+                )
+                mapping = {
+                    "min_*": [min],
+                    "nom_*": [nom],
+                    "max_*": [max],
+                }
+                spef = str(
+                    self.toolbox.filter_views(
+                        self.config, mapping, timing_corner=timing_corner
+                    )[0]
+                )
+                extra_spefs_backcompat_raw.append((module, spef))
+
+        extra_spefs_backcompat = None
+        if extra_spefs_backcompat_raw is not None:
+            extra_spefs_backcompat = tuple(extra_spefs_backcompat_raw)
+
+        return (
+            name,
+            OpenSTAStep.CornerFileList(
+                libs=tuple([str(lib) for lib in libs]),
+                netlists=tuple([str(netlist) for netlist in netlists]),
+                spefs=tuple([(pair[0], str(pair[1])) for pair in spefs]),
+                extra_spefs_backcompat=extra_spefs_backcompat,
+                current_corner_spef=current_corner_spef,
+            ),
+        )
 
 
 @Step.factory.register()
-class CheckMacroInstances(STAPrePNR):
+class CheckMacroInstances(OpenSTAStep):
     """
     Checks if all macro instances declared in the configuration are, in fact,
     in the design, emitting an error otherwise.
 
     Nested macros (macros within macros) are supported provided netlist views
     are available for the macro.
     """
@@ -540,176 +514,106 @@
         for macro_name, data in macros.items():
             for instance_name in data.instances:
                 macro_instance_pairs.append(instance_name)
                 macro_instance_pairs.append(macro_name)
 
         env["_check_macro_instances"] = TclUtils.join(macro_instance_pairs)
 
-        return super().run(state_in, prioritize_nl=True, env=env, **kwargs)
+        corner_name, file_list = self._get_corner_files(prioritize_nl=True)
+        file_list.set_env(env)
+        env["_CURRENT_CORNER_NAME"] = corner_name
 
+        return super().run(state_in, env=env, **kwargs)
 
-@Step.factory.register()
-class STAPostPNR(STAPrePNR):
-    """
-    Performs multi-corner `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
-    using OpenSTA on the post-PnR Verilog netlist, with extracted parasitics for
-    both the top-level module and any associated macros.
-    """
 
-    id = "OpenROAD.STAPostPNR"
-    name = "STA (Post-PnR)"
-    long_name = "Static Timing Analysis (Post-PnR)"
+class MultiCornerSTA(OpenSTAStep):
+    outputs = [DesignFormat.SDF, DesignFormat.SDC]
 
-    config_vars = STAPrePNR.config_vars + [
+    config_vars = OpenSTAStep.config_vars + [
         Variable(
-            "SIGNOFF_SDC_FILE",
-            Optional[Path],
-            "Specifies the SDC file for STA during signoff",
+            "STA_MACRO_PRIORITIZE_NL",
+            bool,
+            "Prioritize the use of Netlists + SPEF files over LIB files if available for Macros. Useful if extraction was done using OpenROAD, where SPEF files are far more accurate.",
+            default=True,
+        ),
+        Variable(
+            "STA_MAX_VIOLATOR_COUNT",
+            Optional[int],
+            "Maximum number of violators to list in violator_list.rpt",
+        ),
+        Variable(
+            "EXTRA_SPEFS",
+            Optional[List[Union[str, Path]]],
+            "A variable that only exists for backwards compatibility with OpenLane <2.0.0 and should not be used by new designs.",
         ),
     ]
 
-    inputs = STAPrePNR.inputs + [DesignFormat.SPEF, DesignFormat.ODB]
-    outputs = STAPrePNR.outputs + [DesignFormat.LIB]
+    def get_script_path(self):
+        return os.path.join(get_script_dir(), "openroad", "sta", "corner.tcl")
 
-    def filter_unannotated_report(
+    def run_corner(
         self,
+        state_in: State,
+        current_env: Dict[str, Any],
         corner: str,
         corner_dir: str,
-        env: Dict,
-        checks_report: str,
-        odb_design: str,
-    ):
-        tech_lefs = self.toolbox.filter_views(self.config, self.config["TECH_LEFS"])
-        if len(tech_lefs) != 1:
-            raise StepException(
-                "Misconfigured SCL: 'TECH_LEFS' must return exactly one Tech LEF for its default timing corner."
-            )
-
-        lefs = ["--input-lef", tech_lefs[0]]
-        for lef in self.config["CELL_LEFS"]:
-            lefs.append("--input-lef")
-            lefs.append(lef)
-        if extra_lefs := self.config["EXTRA_LEFS"]:
-            for lef in extra_lefs:
-                lefs.append("--input-lef")
-                lefs.append(lef)
-        metrics_path = os.path.join(corner_dir, "filter_unannotated_metrics.json")
-        filter_unannotated_cmd = [
-            "openroad",
-            "-exit",
-            "-no_splash",
-            "-metrics",
-            metrics_path,
-            "-python",
-            os.path.join(get_script_dir(), "odbpy", "filter_unannotated.py"),
-            "--corner",
-            corner,
-            "--checks-report",
-            checks_report,
-            odb_design,
-        ] + lefs
-
-        subprocess_result = self.run_subprocess(
-            filter_unannotated_cmd,
-            log_to=os.path.join(corner_dir, "filter_unannotated.log"),
-            env=env,
-            silent=True,
-            report_dir=corner_dir,
-        )
-
-        generated_metrics = subprocess_result["generated_metrics"]
-
-        if os.path.exists(metrics_path):
-            or_metrics_out = json.loads(open(metrics_path).read())
-            generated_metrics.update(or_metrics_out)
+    ) -> Dict[str, Any]:
+        info(f"Starting STA for the {corner} timing corner…")
+        current_env["_CURRENT_CORNER_NAME"] = corner
+        log_path = os.path.join(corner_dir, "sta.log")
+
+        try:
+            subprocess_result = self.run_subprocess(
+                self.get_command(),
+                log_to=log_path,
+                env=current_env,
+                silent=True,
+                report_dir=corner_dir,
+            )
+
+            generated_metrics = subprocess_result["generated_metrics"]
+
+            info(f"Finished STA for the {corner} timing corner.")
+        except subprocess.CalledProcessError as e:
+            self.err(f"Failed STA for the {corner} timing corner:")
+            raise e
 
         return generated_metrics
 
     def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
         kwargs, env = self.extract_env(kwargs)
-
         env = self.prepare_env(env, state_in)
 
-        env["_OPENSTA"] = "1"
-        env["_SDC_IN"] = (
-            self.config["SIGNOFF_SDC_FILE"] or self.config["FALLBACK_SDC_FILE"]
-        )
-
-        def run_corner(corner: str):
-            nonlocal env
+        futures: Dict[str, Future[MetricsUpdate]] = {}
+        files_so_far: Dict[OpenSTAStep.CornerFileList, str] = {}
+        corners_used: Set[str] = set()
+        for corner in self.config["STA_CORNERS"]:
+            _, file_list = self._get_corner_files(
+                corner, prioritize_nl=self.config["STA_MACRO_PRIORITIZE_NL"]
+            )
+            if previous := files_so_far.get(file_list):
+                info(
+                    f"Skipping corner {corner} for STA (identical to {previous} at this stage)…"
+                )
+                continue
+            files_so_far[file_list] = corner
+            corners_used.add(corner)
 
             current_env = env.copy()
+            file_list.set_env(current_env)
 
             corner_dir = os.path.join(self.step_dir, corner)
             mkdirp(corner_dir)
 
-            current_env["_LIB_SAVE_DIR"] = corner_dir
-            current_env["_SDF_SAVE_DIR"] = corner_dir
-
-            if not isinstance(state_in[DesignFormat.SPEF], dict):
-                raise StepException(
-                    "Malformed input state: value for SPEF is not a dictionary."
-                )
-
-            input_spef_dict = state_in[DesignFormat.SPEF]
-            assert input_spef_dict is not None  # Checked by start
-            if not isinstance(input_spef_dict, dict):
-                raise StepException(
-                    "Malformed input state: value for 'spef' is not a dictionary"
-                )
-
-            spefs = self.toolbox.filter_views(self.config, input_spef_dict, corner)
-            if len(spefs) < 1:
-                raise StepException(
-                    f"No SPEF file compatible with corner '{corner}' found."
-                )
-            elif len(spefs) > 1:
-                self.warn(
-                    f"Multiple SPEF files compatible with corner '{corner}' found. The first one encountered will be used."
-                )
-            current_env["_CURRENT_SPEF_BY_CORNER"] = spefs[0]
-
-            _set_corner_files(
-                self,
-                current_env,
-                timing_corner=corner,
-                prioritize_nl=self.config["STA_MACRO_PRIORITIZE_NL"],
-            )
-
-            log_path = os.path.join(corner_dir, "sta.log")
-
-            try:
-                subprocess_result = self.run_subprocess(
-                    self.get_command(),
-                    log_to=log_path,
-                    env=current_env,
-                    silent=True,
-                    report_dir=corner_dir,
-                )
-                generated_metrics = subprocess_result["generated_metrics"]
-
-                filter_unannotated_metrics = self.filter_unannotated_report(
-                    corner=corner,
-                    checks_report=os.path.join(corner_dir, "checks.rpt"),
-                    corner_dir=corner_dir,
-                    env=env,
-                    odb_design=str(state_in[DesignFormat.ODB]),
-                )
-                info(f"Finished STA for the {corner} timing corner.")
-            except subprocess.CalledProcessError as e:
-                self.err(f"Failed STA for the {corner} timing corner:")
-                raise e
-
-            return {**generated_metrics, **filter_unannotated_metrics}
-
-        futures: Dict[str, Future[MetricsUpdate]] = {}
-        for corner in self.config["STA_CORNERS"]:
             futures[corner] = get_tpe().submit(
-                run_corner,
+                self.run_corner,
+                state_in,
+                current_env,
                 corner,
+                corner_dir,
             )
 
         metrics_updates: MetricsUpdate = {}
         for corner, updates_future in futures.items():
             metrics_updates.update(updates_future.result())
 
         metric_updates_with_aggregates = aggregate_metrics(metrics_updates)
@@ -737,25 +641,27 @@
 
         table = rich.table.Table()
         table.add_column("Corner/Group", width=20)
         table.add_column("Hold Worst Slack")
         table.add_column("Reg to Reg Paths")
         table.add_column("Hold TNS")
         table.add_column("Hold Vio Count")
-        table.add_column("⊃ reg to reg")
+        table.add_column("of which reg to reg")
         table.add_column("Setup Worst Slack")
         table.add_column("Reg to Reg Paths")
         table.add_column("Setup TNS")
         table.add_column("Setup Vio Count")
-        table.add_column("⊃ reg to reg")
+        table.add_column("of which reg to reg")
         table.add_column("Max Cap Violations")
         table.add_column("Max Slew Violations")
         for corner in ["Overall"] + self.config["STA_CORNERS"]:
             modifier = ""
             if corner != "Overall":
+                if corner not in corners_used:
+                    continue
                 modifier = f"__corner:{corner}"
             row = [corner]
             for metric in [
                 "timing__hold__ws",
                 "timing__hold_r2r__ws",
                 "timing__hold__tns",
                 "timing__hold_vio__count",
@@ -776,46 +682,186 @@
 
         if not options.get_condensed_mode():
             console.print(table)
         with open(os.path.join(self.step_dir, "summary.rpt"), "w") as f:
             table.width = 160
             rich.print(table, file=f)
 
-        views_updates: ViewsUpdate = {}
-        lib_dict = state_in[DesignFormat.LIB] or {}
-        if not isinstance(lib_dict, dict):
+        return {}, metric_updates_with_aggregates
+
+
+@Step.factory.register()
+class STAPrePNR(MultiCornerSTA):
+    """
+    Performs hierarchical `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
+    using OpenSTA on the pre-PnR Verilog netlist, with all available timing information
+    for standard cells and macros for multiple corners.
+
+    If timing information is not available for a Macro, the macro in question
+    will be black-boxed.
+    """
+
+    id = "OpenROAD.STAPrePNR"
+    name = "STA (Pre-PnR)"
+    long_name = "Static Timing Analysis (Pre-PnR)"
+
+    def run_corner(
+        self, state_in: State, current_env: Dict[str, Any], corner: str, corner_dir: str
+    ) -> Dict[str, Any]:
+        current_env["_SDF_SAVE_DIR"] = corner_dir
+        return super().run_corner(state_in, current_env, corner, corner_dir)
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        views_updates, metrics_updates = super().run(state_in, **kwargs)
+
+        sdf_dict = state_in[DesignFormat.SDF] or {}
+        if not isinstance(sdf_dict, dict):
             raise StepException(
-                "Malformed input state: value for LIB is not a dictionary."
+                "Malformed input state: incoming value for SDF is not a dictionary."
             )
 
+        sdf_dict = sdf_dict.copy()
+
         for corner in self.config["STA_CORNERS"]:
-            lib_dict[corner] = Path(
-                os.path.join(
-                    self.step_dir, corner, f"{self.config['DESIGN_NAME']}__{corner}.lib"
-                )
+            sdf = os.path.join(
+                self.step_dir, corner, f"{self.config['DESIGN_NAME']}__{corner}.sdf"
             )
+            if os.path.isfile(sdf):
+                sdf_dict[corner] = Path(sdf)
 
-        views_updates[DesignFormat.LIB] = lib_dict
+        views_updates[DesignFormat.SDF] = sdf_dict
 
-        sdf_dict = state_in[DesignFormat.SDF] or {}
-        if not isinstance(sdf_dict, dict):
+        return views_updates, metrics_updates
+
+
+@Step.factory.register()
+class STAPostPNR(STAPrePNR):
+    """
+    Performs multi-corner `Static Timing Analysis <https://en.wikipedia.org/wiki/Static_timing_analysis>`_
+    using OpenSTA on the post-PnR Verilog netlist, with extracted parasitics for
+    both the top-level module and any associated macros.
+    """
+
+    id = "OpenROAD.STAPostPNR"
+    name = "STA (Post-PnR)"
+    long_name = "Static Timing Analysis (Post-PnR)"
+
+    config_vars = STAPrePNR.config_vars + [
+        Variable(
+            "SIGNOFF_SDC_FILE",
+            Optional[Path],
+            "Specifies the SDC file for STA during signoff",
+        ),
+    ]
+
+    inputs = STAPrePNR.inputs + [DesignFormat.SPEF, DesignFormat.ODB]
+    outputs = STAPrePNR.outputs + [DesignFormat.LIB]
+
+    def prepare_env(self, env: dict, state: State) -> dict:
+        env = super().prepare_env(env, state)
+        if signoff_sdc_file := self.config["SIGNOFF_SDC_FILE"]:
+            env["_SDC_IN"] = signoff_sdc_file
+        return env
+
+    def filter_unannotated_report(
+        self,
+        corner: str,
+        corner_dir: str,
+        env: Dict,
+        checks_report: str,
+        odb_design: str,
+    ):
+        tech_lefs = self.toolbox.filter_views(self.config, self.config["TECH_LEFS"])
+        if len(tech_lefs) != 1:
+            raise StepException(
+                "Misconfigured SCL: 'TECH_LEFS' must return exactly one Tech LEF for its default timing corner."
+            )
+
+        lefs = ["--input-lef", tech_lefs[0]]
+        for lef in self.config["CELL_LEFS"]:
+            lefs.append("--input-lef")
+            lefs.append(lef)
+        if extra_lefs := self.config["EXTRA_LEFS"]:
+            for lef in extra_lefs:
+                lefs.append("--input-lef")
+                lefs.append(lef)
+        metrics_path = os.path.join(corner_dir, "filter_unannotated_metrics.json")
+        filter_unannotated_cmd = [
+            "openroad",
+            "-exit",
+            "-no_splash",
+            "-metrics",
+            metrics_path,
+            "-python",
+            os.path.join(get_script_dir(), "odbpy", "filter_unannotated.py"),
+            "--corner",
+            corner,
+            "--checks-report",
+            checks_report,
+            odb_design,
+        ] + lefs
+
+        subprocess_result = self.run_subprocess(
+            filter_unannotated_cmd,
+            log_to=os.path.join(corner_dir, "filter_unannotated.log"),
+            env=env,
+            silent=True,
+            report_dir=corner_dir,
+        )
+
+        generated_metrics = subprocess_result["generated_metrics"]
+
+        if os.path.exists(metrics_path):
+            or_metrics_out = json.loads(open(metrics_path).read())
+            generated_metrics.update(or_metrics_out)
+
+        return generated_metrics
+
+    def run_corner(
+        self,
+        state_in: State,
+        current_env: Dict[str, Any],
+        corner: str,
+        corner_dir: str,
+    ) -> MetricsUpdate:
+        current_env["_LIB_SAVE_DIR"] = corner_dir
+        metrics_updates = super().run_corner(state_in, current_env, corner, corner_dir)
+        try:
+            filter_unannotated_metrics = self.filter_unannotated_report(
+                corner=corner,
+                checks_report=os.path.join(corner_dir, "checks.rpt"),
+                corner_dir=corner_dir,
+                env=current_env,
+                odb_design=str(state_in[DesignFormat.ODB]),
+            )
+        except subprocess.CalledProcessError as e:
+            self.err(
+                f"Failed filtering unannotated nets for the {corner} timing corner."
+            )
+            raise e
+        return {**metrics_updates, **filter_unannotated_metrics}
+
+    def run(self, state_in: State, **kwargs) -> Tuple[ViewsUpdate, MetricsUpdate]:
+        views_updates, metrics_updates = super().run(state_in, **kwargs)
+        lib_dict = state_in[DesignFormat.LIB] or {}
+        if not isinstance(lib_dict, dict):
             raise StepException(
                 "Malformed input state: value for LIB is not a dictionary."
             )
 
+        lib_dict.copy()
+
         for corner in self.config["STA_CORNERS"]:
-            sdf_dict[corner] = Path(
-                os.path.join(
-                    self.step_dir, corner, f"{self.config['DESIGN_NAME']}__{corner}.sdf"
-                )
+            lib = os.path.join(
+                self.step_dir, corner, f"{self.config['DESIGN_NAME']}__{corner}.lib"
             )
+            lib_dict[corner] = Path(lib)
 
-        views_updates[DesignFormat.SDF] = sdf_dict
-
-        return views_updates, metric_updates_with_aggregates
+        views_updates[DesignFormat.LIB] = lib_dict
+        return views_updates, metrics_updates
 
 
 @Step.factory.register()
 class Floorplan(OpenROADStep):
     """
     Creates DEF and ODB files with the initial floorplan based on the Yosys netlist.
     """
```

### Comparing `openlane-2.0.0rc2/openlane/steps/openroad_alerts.py` & `openlane-2.0.0rc3/openlane/steps/openroad_alerts.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/step.py` & `openlane-2.0.0rc3/openlane/steps/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -1074,21 +1074,16 @@
         else:
             self.toolbox = toolbox
 
         state_in_result = self.state_in.result()
 
         if not logging.options.get_condensed_mode():
             rule(f"{self.long_name}")
-        log_path = Path(self.get_log_path()).rel_if_child(
-            relative_prefix=f".{os.path.sep}"
-        )
 
-        verbose(
-            f"Running '{self.id}'… (Log: [link=file://{os.path.abspath(log_path)}]{log_path}[/link])"
-        )
+        verbose(f"Running '{self.id}'…")
 
         mkdirp(self.step_dir)
         with open(os.path.join(self.step_dir, "state_in.json"), "w") as f:
             f.write(state_in_result.dumps())
 
         with open(os.path.join(self.step_dir, "config.json"), "w") as f:
             config_mut = self.config.to_raw_dict()
@@ -1260,14 +1255,17 @@
 
         if output_processing is None:
             output_processing = self.output_processors
         output_processors = []
         for cls in output_processing:
             output_processors.append(cls(self, report_dir, silent))
 
+        verbose(
+            f"Logging subprocess to [repr.filename][link=file://{os.path.abspath(log_path)}]{os.path.relpath(log_path)}[/link][/repr.filename]…"
+        )
         process = _popen_callable(
             cmd_str,
             encoding="utf8",
             env=env,
             **kwargs,
         )
```

### Comparing `openlane-2.0.0rc2/openlane/steps/tclstep.py` & `openlane-2.0.0rc3/openlane/steps/tclstep.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/verilator.py` & `openlane-2.0.0rc3/openlane/steps/verilator.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane/steps/yosys.py` & `openlane-2.0.0rc3/openlane/steps/yosys.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0rc2/openlane.egg-info/PKG-INFO` & `openlane-2.0.0rc3/openlane.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized, but some oddities are still to be expected. Proceed with caution.
         >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0rc2 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0rc3 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > OpenLane 2.0.0 is in beta. APIs have mostly stabilized,
 but some oddities are still to be expected. Proceed with caution. > > If you
 *don't* know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ************ OOppeennLLaannee ************
```

### Comparing `openlane-2.0.0rc2/openlane.egg-info/SOURCES.txt` & `openlane-2.0.0rc3/openlane.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 openlane/examples/spm-user_project_wrapper/SPM_example.v
 openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc
 openlane/examples/spm-user_project_wrapper/config-tut.json
 openlane/examples/spm-user_project_wrapper/config.json
 openlane/examples/spm-user_project_wrapper/defines.v
 openlane/examples/spm-user_project_wrapper/template.def
 openlane/examples/spm-user_project_wrapper/user_project_wrapper.v
+openlane/examples/spm/src/impl.sdc
+openlane/examples/spm/src/signoff.sdc
+openlane/examples/spm/src/spm.v
+openlane/examples/spm/verify/spm_tb.v
 openlane/flows/__init__.py
 openlane/flows/builtins.py
 openlane/flows/classic.py
 openlane/flows/cli.py
 openlane/flows/flow.py
 openlane/flows/misc.py
 openlane/flows/optimizing.py
@@ -131,14 +135,15 @@
 openlane/scripts/openroad/common/set_power_nets.tcl
 openlane/scripts/openroad/common/set_rc.tcl
 openlane/scripts/openroad/common/set_routing_layers.tcl
 openlane/scripts/openroad/sta/check_macro_instances.tcl
 openlane/scripts/openroad/sta/corner.tcl
 openlane/scripts/tclsh/hello.tcl
 openlane/scripts/yosys/common.tcl
+openlane/scripts/yosys/construct_abc_script.tcl
 openlane/scripts/yosys/json_header.tcl
 openlane/scripts/yosys/synthesize.tcl
 openlane/state/__init__.py
 openlane/state/__main__.py
 openlane/state/design_format.py
 openlane/state/state.py
 openlane/steps/__init__.py
```

### Comparing `openlane-2.0.0rc2/setup.py` & `openlane-2.0.0rc3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             "py.typed",
             "open_pdks_rev",
             "scripts/*",
             "scripts/**/*",
             "scripts/**/**/*",
             "examples/*",
             "examples/**/*",
+            "examples/**/**/*",
         ]
     },
     version=version,
     description="An infrastructure for implementing chip design flows",
     long_description=open(os.path.join(__dir__, "Readme.md")).read(),
     long_description_content_type="text/markdown",
     author="Efabless Corporation and Contributors",
```

### Comparing `openlane-2.0.0rc2/test/conftest.py` & `openlane-2.0.0rc3/test/conftest.py`

 * *Files identical despite different names*

