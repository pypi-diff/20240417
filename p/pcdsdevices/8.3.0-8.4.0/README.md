# Comparing `tmp/pcdsdevices-8.3.0.tar.gz` & `tmp/pcdsdevices-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdsdevices-8.3.0.tar", last modified: Thu Feb 22 18:03:50 2024, max compression
+gzip compressed data, was "pcdsdevices-8.4.0.tar", last modified: Wed Apr 17 00:01:44 2024, max compression
```

## Comparing `pcdsdevices-8.3.0.tar` & `pcdsdevices-8.4.0.tar`

### file list

```diff
@@ -1,291 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.049747 pcdsdevices-8.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.009747 pcdsdevices-8.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.009747 pcdsdevices-8.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-02-22 18:03:50.049747 pcdsdevices-8.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.009747 pcdsdevices-8.3.0/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.009747 pcdsdevices-8.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)      901 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/pre-release-notes.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/release_notes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.013747 pcdsdevices-8.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/README.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.005747 pcdsdevices-8.3.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.013747 pcdsdevices-8.3.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)    31509 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/base_classes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/mv.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/presets.rst
--rw-r--r--   0 runner    (1001) docker     (127)    86538 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/releases.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/signals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/sim_types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/tab.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/ui.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/upcoming_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.013747 pcdsdevices-8.3.0/docs/source/upcoming_release_notes/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/upcoming_release_notes/template-full.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/source/upcoming_release_notes/template-short.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/update_api_list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       43 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs/view-build.sh
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/docs-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/make_ophyd_device
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.025747 pcdsdevices-8.3.0/pcdsdevices/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-22 18:03:49.000000 pcdsdevices-8.3.0/pcdsdevices/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/analog_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.029747 pcdsdevices-8.3.0/pcdsdevices/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/areadetector/cam.py
--rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/areadetector/detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/areadetector/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/atm.py
--rw-r--r--   0 runner    (1001) docker     (127)    64502 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/attenuator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/beam_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    39229 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ccm.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/crix_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/cvmi_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/dc_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/delay_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/digital_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/digitizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/doc_stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    54503 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/epics_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/eps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/evr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    14511 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/fms.py
--rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/gon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.029747 pcdsdevices-8.3.0/pcdsdevices/happi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/happi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29150 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/happi/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/inout.py
--rw-r--r--   0 runner    (1001) docker     (127)    64152 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19459 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ipm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/jet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/keithley.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lamp_motion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.029747 pcdsdevices-8.3.0/pcdsdevices/lasers/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20097 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/btms_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/btps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/counters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/dicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/ek9000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/elliptec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/qmini.py
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/rfof.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/thorlabsWFS.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/tuttifrutti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lasers/zoomtelescope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lic.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/light_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    80467 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lodcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16659 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/lxe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/make_ophyd_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    51424 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/movablestand.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/mpod.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8327 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/mpod_apalis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/mrco_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/mv_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/piezo.py
--rw-r--r--   0 runner    (1001) docker     (127)    21550 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/pim.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/pmps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/positioner.py
--rw-r--r--   0 runner    (1001) docker     (127)    39960 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/pseudopos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/pulsepicker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15336 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/pump.py
--rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/pv_positioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/qadc.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/radiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/rs_powersupply.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/rtds_ebd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/sample_delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11909 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    58193 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/sim.py
--rw-r--r--   0 runner    (1001) docker     (127)    26695 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/slits.py
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/spectrometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/sqr1.py
--rw-r--r--   0 runner    (1001) docker     (127)    32516 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/stopper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/sxr_test_absorber.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    48269 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.037747 pcdsdevices-8.3.0/pcdsdevices/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_analog_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_atm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_attenuator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_beam_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_btms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_ccm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_crix_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_dc_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_disconnected.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    20411 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_epics_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_evr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_gauge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_gon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_inout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_ipm.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_jet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_lens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.037747 pcdsdevices-8.3.0/pcdsdevices/tests/test_lens_sets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_lens_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_lens_sets/original.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_lens_sets/test
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_lens_sets/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_lic.py
--rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_lodcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_lxe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_movablestand.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_mpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_mpod_apalis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_pim.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_positioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_pseudopos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_pulsepicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_pump.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_pv_positioner.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_sample_delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_slits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_spectrometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    17153 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_timetool.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_tpr.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_valve.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_variety.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/test_wfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tests/xcslt8717_wpcalib_opa
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/timetool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/tpr.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/type_hints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.045747 pcdsdevices-8.3.0/pcdsdevices/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AT1K2.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AT1K2.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AT2L0.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AT2L0.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui
--rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (127)    22407 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui
--rw-r--r--   0 runner    (1001) docker     (127)    17847 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
--rw-r--r--   0 runner    (1001) docker     (127)    15571 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffAxisEPSCustom.ui
--rw-r--r--   0 runner    (1001) docker     (127)    41696 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)    25557 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/BtpsState.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/BtpsState.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/IM3L0_K2700.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/IM3L0_K2700.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)    60307 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/JJSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/LCP.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/Leviton1.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/LightControl.ui
--rw-r--r--   0 runner    (1001) docker     (127)    51167 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/PowerSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)    34999 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/PowerSlits.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)    27032 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)    22511 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/Setra5000.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/StatePositioner.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/StatePositioner.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/at2l0_filters.json
--rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-camera-summary.ui
--rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-config.ui
--rw-r--r--   0 runner    (1001) docker     (127)    38523 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-overview.ui
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-range-config.ui
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-range-summary.ui
--rw-r--r--   0 runner    (1001) docker     (127)    46416 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-source-dest.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-source-tabs-config.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-source-tabs.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps-source-valves.ui
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/btps.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/ui/detailed_tree.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/usb_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    27787 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/valve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/variety.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pcdsdevices/wfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:03:50.045747 pcdsdevices-8.3.0/pcdsdevices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-02-22 18:03:49.000000 pcdsdevices-8.3.0/pcdsdevices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-02-22 18:03:50.000000 pcdsdevices-8.3.0/pcdsdevices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 18:03:49.000000 pcdsdevices-8.3.0/pcdsdevices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-22 18:03:49.000000 pcdsdevices-8.3.0/pcdsdevices.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-22 18:03:49.000000 pcdsdevices-8.3.0/pcdsdevices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-22 18:03:49.000000 pcdsdevices-8.3.0/pcdsdevices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-22 18:03:33.000000 pcdsdevices-8.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 18:03:50.049747 pcdsdevices-8.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:44.009401 pcdsdevices-8.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.969401 pcdsdevices-8.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.969401 pcdsdevices-8.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-17 00:01:44.009401 pcdsdevices-8.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.969401 pcdsdevices-8.4.0/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.969401 pcdsdevices-8.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      901 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.973401 pcdsdevices-8.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/README.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.965401 pcdsdevices-8.4.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.973401 pcdsdevices-8.4.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    32006 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/base_classes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/mv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/presets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    89457 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/sim_types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/tab.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/ui.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.973401 pcdsdevices-8.4.0/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/source/upcoming_release_notes/template-short.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/update_api_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       43 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs/view-build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/docs-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/make_ophyd_device
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.985401 pcdsdevices-8.4.0/pcdsdevices/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 00:01:43.000000 pcdsdevices-8.4.0/pcdsdevices/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/analog_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.985401 pcdsdevices-8.4.0/pcdsdevices/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/areadetector/cam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19375 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/areadetector/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/areadetector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/atm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64502 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/beam_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41558 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ccm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/crix_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/cvmi_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/dc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/delay_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/digital_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/doc_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56385 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/eps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/evr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14511 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/fms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/gon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.985401 pcdsdevices-8.4.0/pcdsdevices/happi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/happi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29511 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/happi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/inout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64152 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19459 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ipm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/jet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/keithley.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lamp_motion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.989401 pcdsdevices-8.4.0/pcdsdevices/lasers/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20097 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/btms_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23308 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/btps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/counters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/dicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/ek9000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/elliptec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/qmini.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/rfof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/thorlabsWFS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/tuttifrutti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lasers/zoomtelescope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lic_2d_tmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/light_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80467 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lodcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/lxe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/make_ophyd_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51871 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/movablestand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/mpod.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9365 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/mpod_apalis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/mrco_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/mv_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/piezo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21550 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/pim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/pmps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/positioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39960 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/pulsepicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15336 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/pump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/pv_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/qadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/radiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/rs_powersupply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/rtds_ebd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/sample_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11909 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58193 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26695 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/slits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/smarpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/sqr1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32516 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/stopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/sxr_test_absorber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48269 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.997401 pcdsdevices-8.4.0/pcdsdevices/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_analog_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_atm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_beam_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_btms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_ccm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_crix_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_dc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_disconnected.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20411 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_evr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_gon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_inout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_ipm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_jet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_lens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:43.997401 pcdsdevices-8.4.0/pcdsdevices/tests/test_lens_sets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_lens_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_lens_sets/original.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_lens_sets/test
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_lens_sets/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_lic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19101 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_lodcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9697 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_lxe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_movablestand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_mpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_mpod_apalis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_pim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_pulsepicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_pump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_pv_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_sample_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_slits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12081 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17153 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_timetool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_tpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_variety.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/test_wfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tests/xcslt8717_wpcalib_opa
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/timetool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/tpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/type_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:44.005401 pcdsdevices-8.4.0/pcdsdevices/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AT1K2.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AT1K2.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AT2L0.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AT2L0.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    18911 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    22407 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    17847 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    15571 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffAxisEPSCustom.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffAxisEPSCustom.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    41696 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    25557 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/BtpsState.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/BtpsState.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/IM3L0_K2700.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/IM3L0_K2700.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    60307 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/JJSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/LCP.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/Leviton1.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/LightControl.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    51167 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/PowerSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    34999 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/PowerSlits.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    27032 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    22511 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/Setra5000.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/SmarPod_Pivot.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    21935 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/SmarPod_Poses.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    52536 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/SmarPod_Position.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/SmarPod_Reference.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9580 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/Smarpod.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/StatePositioner.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/StatePositioner.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/at2l0_filters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-camera-summary.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-config.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    38523 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-overview.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-range-config.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-range-summary.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    46416 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-source-dest.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-source-tabs-config.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-source-tabs.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps-source-valves.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/btps.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/ui/detailed_tree.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/usb_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/variety.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pcdsdevices/wfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:01:44.009401 pcdsdevices-8.4.0/pcdsdevices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-17 00:01:43.000000 pcdsdevices-8.4.0/pcdsdevices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8892 2024-04-17 00:01:43.000000 pcdsdevices-8.4.0/pcdsdevices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:01:43.000000 pcdsdevices-8.4.0/pcdsdevices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-17 00:01:43.000000 pcdsdevices-8.4.0/pcdsdevices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-17 00:01:43.000000 pcdsdevices-8.4.0/pcdsdevices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 00:01:43.000000 pcdsdevices-8.4.0/pcdsdevices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-17 00:01:32.000000 pcdsdevices-8.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:01:44.009401 pcdsdevices-8.4.0/setup.cfg
```

### Comparing `pcdsdevices-8.3.0/.github/ISSUE_TEMPLATE.md` & `pcdsdevices-8.4.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/.github/PULL_REQUEST_TEMPLATE.md` & `pcdsdevices-8.4.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/.github/workflows/standard.yml` & `pcdsdevices-8.4.0/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/.pre-commit-config.yaml` & `pcdsdevices-8.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/CONTRIBUTING.rst` & `pcdsdevices-8.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/LICENSE.md` & `pcdsdevices-8.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/PKG-INFO` & `pcdsdevices-8.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsdevices
-Version: 8.3.0
+Version: 8.4.0
 Summary: Ophyd Device definitions for LCLS Beamline components
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `pcdsdevices-8.3.0/README.md` & `pcdsdevices-8.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/conda-recipe/meta.yaml` & `pcdsdevices-8.4.0/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/Makefile` & `pcdsdevices-8.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/pre-release-notes.sh` & `pcdsdevices-8.4.0/docs/pre-release-notes.sh`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/release_notes.py` & `pcdsdevices-8.4.0/docs/release_notes.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/README.inc` & `pcdsdevices-8.4.0/docs/source/README.inc`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/_templates/autosummary/class.rst` & `pcdsdevices-8.4.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/_templates/autosummary/module.rst` & `pcdsdevices-8.4.0/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/api.rst` & `pcdsdevices-8.4.0/docs/source/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 .. autosummary::
     :toctree: generated
 
     pcdsdevices.ccm.CCM
     pcdsdevices.ccm.CCMAlio
     pcdsdevices.ccm.CCMConstantsMixin
     pcdsdevices.ccm.CCMEnergy
+    pcdsdevices.ccm.CCMEnergyWithACRStatus
     pcdsdevices.ccm.CCMEnergyWithVernier
     pcdsdevices.ccm.CCMMotor
     pcdsdevices.ccm.CCMPico
     pcdsdevices.ccm.CCMX
     pcdsdevices.ccm.CCMY
     pcdsdevices.ccm.alio_to_theta
     pcdsdevices.ccm.energy_to_wavelength
@@ -270,14 +271,15 @@
     pcdsdevices.epics_motor.Motor
     pcdsdevices.epics_motor.Newport
     pcdsdevices.epics_motor.OffsetIMSWithPreset
     pcdsdevices.epics_motor.OffsetMotor
     pcdsdevices.epics_motor.PCDSMotorBase
     pcdsdevices.epics_motor.PMC100
     pcdsdevices.epics_motor.SmarAct
+    pcdsdevices.epics_motor.SmarActEncodedTipTilt
     pcdsdevices.epics_motor.SmarActOpenLoop
     pcdsdevices.epics_motor.SmarActOpenLoopPositioner
     pcdsdevices.epics_motor.SmarActTipTilt
 
 pcdsdevices.eps
 ---------------
 
@@ -587,14 +589,22 @@
 
 .. autosummary::
     :toctree: generated
 
     pcdsdevices.lic.LICMirror
     pcdsdevices.lic.LaserInCoupling
 
+pcdsdevices.lic_2d_tmo
+----------------------
+
+.. autosummary::
+    :toctree: generated
+
+    pcdsdevices.lic_2d_tmo.TMOLaserInCouplingTwoDimension
+
 pcdsdevices.light_control
 -------------------------
 
 .. autosummary::
     :toctree: generated
 
     pcdsdevices.light_control.LightControl
@@ -637,14 +647,15 @@
 .. autosummary::
     :toctree: generated
 
     pcdsdevices.lxe.FakeLxtTtc
     pcdsdevices.lxe.LaserEnergyPositioner
     pcdsdevices.lxe.LaserTiming
     pcdsdevices.lxe.LaserTimingCompensation
+    pcdsdevices.lxe.Lcls2LaserTiming
     pcdsdevices.lxe.LxtTtcExample
     pcdsdevices.lxe.TimeToolDelay
     pcdsdevices.lxe._ReversedTimeToolDelay
     pcdsdevices.lxe._ScaledUnitConversionDerivedSignal
     pcdsdevices.lxe.load_calibration_file
 
 pcdsdevices.make_ophyd_device
@@ -1026,14 +1037,24 @@
     pcdsdevices.slits.LusiSlits
     pcdsdevices.slits.PowerSlits
     pcdsdevices.slits.SimLusiSlits
     pcdsdevices.slits.SlitPositioner
     pcdsdevices.slits.Slits
     pcdsdevices.slits.SlitsBase
 
+pcdsdevices.smarpod
+-------------------
+
+.. autosummary::
+    :toctree: generated
+
+    pcdsdevices.smarpod.SmarPod
+    pcdsdevices.smarpod.SmarPodPose
+    pcdsdevices.smarpod.SmarPodStatus
+
 pcdsdevices.spectrometer
 ------------------------
 
 .. autosummary::
     :toctree: generated
 
     pcdsdevices.spectrometer.FZPStates
@@ -1161,14 +1182,15 @@
     pcdsdevices.utils.get_status_float
     pcdsdevices.utils.get_status_value
     pcdsdevices.utils.ipm_screen
     pcdsdevices.utils.is_input
     pcdsdevices.utils.maybe_make_method
     pcdsdevices.utils.move_subdevices_to_start
     pcdsdevices.utils.post_ophyds_to_elog
+    pcdsdevices.utils.re_arg
     pcdsdevices.utils.reorder_components
     pcdsdevices.utils.schedule_task
     pcdsdevices.utils.set_many
     pcdsdevices.utils.set_standard_ordering
     pcdsdevices.utils.sort_components_by_kind
     pcdsdevices.utils.sort_components_by_name
```

### Comparing `pcdsdevices-8.3.0/docs/source/base_classes.rst` & `pcdsdevices-8.4.0/docs/source/base_classes.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/conf.py` & `pcdsdevices-8.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/mv.rst` & `pcdsdevices-8.4.0/docs/source/mv.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/presets.rst` & `pcdsdevices-8.4.0/docs/source/presets.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/releases.rst` & `pcdsdevices-8.4.0/docs/source/releases.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,82 @@
 Release History
 ###############
 
+v8.4.0 (2024-04-16)
+===================
+
+Compatibility Notes
+-------------------
+- If your SmarAct release is < R1.0.20, then the EPICS signals will timeout on the new PVs.
+  Please make sure to update your children IOCs.
+
+Features
+--------
+- Adds `ioc_chan_num` and `ioc_card_num` to the `EnvironmentalMonitor` happi container.
+- Adds the "embedded" file for `BeckhoffAxisEPSCustom` that allows for typhos screens to open using the compact controls.
+- Adds a convenience `re_arg` decorator to redefine and deprecate a function's args in a backwards-compatible way in the `pcdsdevices.utils` submodule.
+
+Device Updates
+--------------
+- `TprTrigger`: Update numerous PVs to "config", add TCMPL PV as the `operation` signal.
+- Adds the following temperature monitoring signals to `SmarAct` and `SmarActOpenLoop`:
+
+  - `channel_temp`
+  - `module_temp`
+- Adds the following hidden config PVs to the (encoded) `SmarAct` device class:
+
+  - `log_scale_offset`
+  - `log_scale_inv`
+  - `def_range_min`
+  - `def_range_max`
+  - `dist_code_inv`
+- Adds the following missing epics signals to `MPODApalisModule`:
+
+  - `supply_status`
+  - `module_status`
+  - `fine_adjustment_status`
+  - `input_status`
+  - `live_insertion_status`
+  - `safety_loop_status`
+  - `kill`
+
+- Adds an `energy_with_acr_status` instance to CCM
+- Updates `BeamEnergyRequest` argument from "bunch" to "pv_index" to better reflect the broader use cases.
+  A backward compatible warning is now returned if the old bunch kwarg is used.
+- Updates "atol" in `BeamEnergyRequestNoWait` to 0.5 (was 5). This is needed for self-seeding.
+- `XOffsetMirrorStateCool` and `XOffsetMirrorNoBend` gets `variable_cool` for controlling 24V solenoid valve.
+
+New Devices
+-----------
+- Adds `li2k4` as `TMOLaserInCouplingTwoDimension`, with the x and y motors supported (no states yet).
+- Adds `Lcls2LaserTiming`: New class supporting control of laser timing for the OPCPA laser locker system.
+- Adds `SmarActEncodedTipTilt` to the `pcdsdevices.epics_motor` submodule.
+- Adds `SmarPod` and related devices in new `pcdsdevices.smarpod` submodule.
+- Adds a `CCMEnergyWithACRStatus` class to the `pcdsdevices.ccm` submodule, a new variant of `CCMEnergy` that waits for ACR status before marking moves as complete.
+
+Bugfixes
+--------
+- Previously, calculate_on_get/put functions used in `MultiDerivedSignal` s in `pcdsdevices.tpr` classes were not accessing their attrs correctly and would throw KeyErrors when called.
+  Specifically, the name of the attr was being used as the key for items dictionary instead of the actual signal object
+- Also added unit tests for these `MultiDerivedSignal` s in the `pcdsdevices.tpr` submodule.
+- Modify `sp1k4` Attenuator RTD class (`TMOSpectrometer`) to match prefix for `sp1k4` group device.
+
+Contributors
+------------
+- aberges-SLAC
+- baljamal
+- jozamudi
+- KaushikMalapati
+- nrwslac
+- patoppermann
+- sainyamn
+- slactjohnson
+- tongju12
+- vespos
+
 
 v8.3.0 (2024-02-21)
 ===================
 
 Features
 --------
 - Enabled the use of custom EPS screens for Beckhoff axes via the
```

### Comparing `pcdsdevices-8.3.0/docs/source/signals.rst` & `pcdsdevices-8.4.0/docs/source/signals.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/tab.rst` & `pcdsdevices-8.4.0/docs/source/tab.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/source/upcoming_release_notes/template-full.rst` & `pcdsdevices-8.4.0/docs/source/upcoming_release_notes/template-full.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/docs/update_api_list.py` & `pcdsdevices-8.4.0/docs/update_api_list.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/__init__.py` & `pcdsdevices-8.4.0/pcdsdevices/__init__.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/_html.py` & `pcdsdevices-8.4.0/pcdsdevices/_html.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/analog_signals.py` & `pcdsdevices-8.4.0/pcdsdevices/analog_signals.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/areadetector/cam.py` & `pcdsdevices-8.4.0/pcdsdevices/areadetector/cam.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/areadetector/detectors.py` & `pcdsdevices-8.4.0/pcdsdevices/areadetector/detectors.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/areadetector/plugins.py` & `pcdsdevices-8.4.0/pcdsdevices/areadetector/plugins.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/atm.py` & `pcdsdevices-8.4.0/pcdsdevices/atm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/attenuator.py` & `pcdsdevices-8.4.0/pcdsdevices/attenuator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/beam_stats.py` & `pcdsdevices-8.4.0/pcdsdevices/beam_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ophyd.pv_positioner import PVPositioner
 from ophyd.signal import AttributeSignal, EpicsSignal, EpicsSignalRO
 from ophyd.sim import fake_device_cache, make_fake_device
 
 from .interface import BaseInterface, FltMvInterface
 from .pv_positioner import PVPositionerDone
 from .signal import AvgSignal
+from .utils import re_arg
 
 logger = logging.getLogger(__name__)
 
 
 class BeamStats(BaseInterface, Device):
     mj = Cpt(EpicsSignalRO, 'GDET:FEE1:241:ENRC', kind='hinted',
              doc='Pulse energy [mJ]')
@@ -85,36 +86,38 @@
 
     line : str, optional
         Whether to use the K line or L line PV. If provided this should be a
         string with a single character. The K line PVs have "EPHOTK"
         in them, the L line PVs just have "EPHOT". This will default to the
         line associated with the prefix hutch name, or to L line failing that.
 
-    bunch : int, optional
-        Whether to move the first bunch (1) or the second bunch (2). This is
-        only relevant for 2-color mode. Defaults to bunch 1.
+    pv_index : int, optional
+        Whether to move the first PV (1) or the second PV (2). This is relevant
+        2-color mode or when scanning combined K and Vernier. Defaults to 1.
 
     acr_status_suffix : str, optional
         If provided, we'll wait on the ACR PV specified by
         SIOC:SYS0:ML07:{suffix}. The selected PV should be 0 while the device
         is moving and 1 when it is done.
     """
     setpoint = FCpt(
         EpicsSignal,
-        '{prefix}:USER:MCC:EPHOT{line_text}:SET{bunch}',
+        '{prefix}:USER:MCC:EPHOT{line_text}:SET{pv_index}',
         kind='hinted',
+        add_prefix=('suffix', 'write_pv', 'line_text', 'pv_index'),
         doc=(
             'The setpoint PV that acr listens on to update the '
             'vernier or undulator PVs as appropriate.'
         ),
     )
     ref = FCpt(
         EpicsSignal,
-        '{prefix}:USER:MCC:EPHOT{line_text}:REF{bunch}',
+        '{prefix}:USER:MCC:EPHOT{line_text}:REF{pv_index}',
         kind='normal',
+        add_prefix=('suffix', 'write_pv', 'line_text', 'pv_index'),
         doc=(
             'A reference PV for the photon energy at the nominal '
             'position of the vernier or undulator.'
         ),
     )
 
     line_text_dict = {
@@ -134,38 +137,39 @@
     ):
         if cls is not BeamEnergyRequest:
             return super().__new__(cls)
         if acr_status_suffix is None:
             return super().__new__(BeamEnergyRequestNoWait)
         return super().__new__(BeamEnergyRequestACRWait)
 
+    @re_arg({"bunch": "pv_index"})
     def __init__(
         self,
         prefix: str,
         *,
         name: str,
         line: Optional[str] = None,
-        bunch: int = 1,
+        pv_index: int = 1,
         acr_status_suffix: Optional[str] = None,
         **kwargs
     ):
         self.line_text = self.line_text_dict.get(line or prefix, '')
-        self.bunch = bunch
+        self.pv_index = pv_index
         self.acr_status_suffix = acr_status_suffix
         super().__init__(prefix, name=name, **kwargs)
 
 
 class BeamEnergyRequestNoWait(BeamEnergyRequest, PVPositionerDone):
     """
     BeamEnergyRequest variant that does not wait on a PV.
 
     It will report done immediately and ignore moves that are smaller than
     atol.
     """
-    atol = 5
+    atol = 0.5
 
     # All done-related functionality is inherited from PVPositionerDone
     # Just implement skip_small_moves's default
     def __init__(self, *args, skip_small_moves: bool = True, **kwargs):
         super().__init__(*args, skip_small_moves=skip_small_moves, **kwargs)
 
 
@@ -177,14 +181,15 @@
     not use the atol parameter.
     """
     # All the logic is implemented in parent classes, just pick the PV
     done = FCpt(
         EpicsSignal,
         'SIOC:SYS0:ML07:{acr_status_suffix}',
         kind='normal',
+        add_prefix=('suffix', 'write_pv', 'acr_status_suffix'),
         doc=(
             'PV that is 0 while the motors are moving and 1 when ACR is '
             'ready for a new request. ACR can pick which of these PVs '
             'to use to report status.'
         )
     )
     done_value = 1
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ccm.py` & `pcdsdevices-8.4.0/pcdsdevices/ccm.py`

 * *Files 4% similar despite different names*

```diff
@@ -718,16 +718,16 @@
     prefix : str
         The PV prefix of the Alio motor, e.g. XPP:MON:MPZ:07A
     hutch : str, optional
         The hutch we're in. This informs us as to which vernier
         PVs to write to. If omitted, we can guess this from the
         prefix.
     """
-    vernier = FCpt(BeamEnergyRequest, '{hutch}', kind='normal',
-                   doc='Requests ACR to move the Vernier.')
+    acr_energy = FCpt(BeamEnergyRequest, '{hutch}', kind='normal',
+                      doc='Requests ACR to move the Vernier.')
 
     # These are duplicate warnings with main energy motor
     _enable_warn_constants: bool = False
     hutch: str
 
     def __init__(
         self,
@@ -755,28 +755,68 @@
         and also converts that energy to eV and passes it along to
         the vernier.
         """
         pseudo_pos = self.PseudoPosition(*pseudo_pos)
         energy = pseudo_pos.energy
         alio = self.energy_to_alio(energy)
         vernier = energy * 1000
-        return self.RealPosition(alio=alio, vernier=vernier)
+        return self.RealPosition(alio=alio, acr_energy=vernier)
 
     def inverse(self, real_pos: namedtuple) -> namedtuple:
         """
         PseudoPositioner interface function for calculating the readback.
 
         Converts the real position of the alio to the calculated energy
         """
         real_pos = self.RealPosition(*real_pos)
         alio = real_pos.alio
         energy = self.alio_to_energy(alio)
         return self.PseudoPosition(energy=energy)
 
 
+class CCMEnergyWithACRStatus(CCMEnergyWithVernier):
+    """
+    CCM energy motor and ACR beam energy request with status.
+    Note that in this case vernier indicates any ways that ACR will act on the
+    photon energy request. This includes the Vernier, but can also lead to
+    motion of the undulators or the K.
+
+    Parameters
+    ----------
+    prefix : str
+        The PV prefix of the Alio motor, e.g. XPP:MON:MPZ:07A
+    hutch : str, optional
+        The hutch we're in. This informs us as to which vernier
+        PVs to write to. If omitted, we can guess this from the
+        prefix.
+    acr_status_sufix : str
+        Prefix to the SIOC PV that ACR uses to report the move status.
+        For HXR this usually is 'AO805'.
+    """
+    acr_energy = FCpt(BeamEnergyRequest, '{hutch}',
+                      pv_index='{pv_index}',
+                      acr_status_suffix='{acr_status_suffix}',
+                      add_prefix=('suffix', 'write_pv', 'pv_index',
+                                  'acr_status_suffix'),
+                      kind='normal',
+                      doc='Requests ACR to move the energy.')
+
+    def __init__(
+        self,
+        prefix: str,
+        hutch: typing.Optional[str] = None,
+        acr_status_suffix='AO805',
+        pv_index=2,
+        **kwargs
+    ):
+        self.acr_status_suffix = acr_status_suffix
+        self.pv_index = pv_index
+        super().__init__(prefix, **kwargs)
+
+
 class CCMX(SyncAxis):
     """
     Combined motion of the CCM X motors.
 
     You can use this device like a motor, and the position setpoint will be
     forwarded to both x motors.
 
@@ -888,30 +928,46 @@
         The prefix for the upstream ccm x translation motor (x2).
     y_down_prefix : str, required keyword
         The prefix for the downstream ccm y translation motor (y1).
     y_up_north_prefix : str, required keyword
         The prefix for the north upstream ccm y translation motor (y2).
     y_up_south_prefix : str, required keyword
         The prefix for the south upstream ccm y translation motor (y3).
+    acr_status_pv_index : int
+        The index for the energy request PV in the case of the acr status
+        wait. Default: 2.
+    acr_status_suffix : str
+        The suffix for the ACR status energy change move. Default to 'AO805'
     """
     energy = Cpt(
         CCMEnergy, '', kind='hinted',
         doc=(
             'PseudoPositioner that moves the alio in '
             'terms of the calculated CCM energy.'
         ),
     )
     energy_with_vernier = Cpt(
         CCMEnergyWithVernier, '', kind='normal',
         doc=(
-            'PsuedoPositioner that moves the alio in '
+            'PseudoPositioner that moves the alio in '
             'terms of the calculated CCM energy while '
             'also requesting a vernier move.'
         ),
     )
+    energy_with_acr_status = FCpt(
+        CCMEnergyWithACRStatus, '{prefix}', kind='normal',
+        acr_status_suffix='{acr_status_suffix}',
+        add_prefix=('suffix', 'write_pv', 'acr_status_suffix'),
+        doc=(
+            'PseudoPositioner that moves the alio in '
+            'terms of the calculated CCM energy while '
+            'also requesting an energy change to ACR. '
+            'This will wait on ACR to complete the move.'
+        ),
+    )
 
     alio = UCpt(CCMAlio, kind='normal',
                 doc='The motor that rotates the CCM crystal.')
     theta2fine = UCpt(
         CCMMotor, atol=0.01, kind='normal',
         doc=(
             'The motor that controls the fine adjustment '
@@ -935,16 +991,17 @@
     x = UCpt(CCMX, add_prefix=[], kind='normal',
              doc='Combined motion of the CCM X motors.')
     y = UCpt(CCMY, add_prefix=[], kind='normal',
              doc='Combined motion of the CCM Y motors.')
 
     lightpath_cpts = ['x.up.user_readback']
     tab_whitelist = ['x1', 'x2', 'y1', 'y2', 'y3', 'E', 'E_Vernier',
-                     'th2fine', 'alio2E', 'E2alio', 'alio', 'home',
-                     'kill', 'insert', 'remove', 'inserted', 'removed']
+                     'energy_with_acr_status', 'th2fine', 'alio2E', 'E2alio',
+                     'alio', 'home', 'kill', 'insert', 'remove', 'inserted',
+                     'removed']
 
     _in_pos: float
     _out_pos: float
 
     def __init__(
         self,
         *,
@@ -953,14 +1010,16 @@
         out_pos: float,
         **kwargs
     ):
         UCpt.collect_prefixes(self, kwargs)
         self._in_pos = in_pos
         self._out_pos = out_pos
         prefix = prefix or self.unrelated_prefixes['alio_prefix']
+        self.acr_status_suffix = kwargs.get('acr_status_suffix', 'AO805')
+        self.acr_status_pv_index = kwargs.get('acr_status_suffix', 2)
         super().__init__(prefix, **kwargs)
 
         # Aliases: defined by the scientists
         self.x1 = self.x.down
         self.x2 = self.x.up
         self.y1 = self.y.down
         self.y2 = self.y.up_north
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/crix_motion.py` & `pcdsdevices-8.4.0/pcdsdevices/crix_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/cvmi_motion.py` & `pcdsdevices-8.4.0/pcdsdevices/cvmi_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/dc_devices.py` & `pcdsdevices-8.4.0/pcdsdevices/dc_devices.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/delay_generator.py` & `pcdsdevices-8.4.0/pcdsdevices/delay_generator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/device.py` & `pcdsdevices-8.4.0/pcdsdevices/device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/device_types.py` & `pcdsdevices-8.4.0/pcdsdevices/device_types.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/digitizers.py` & `pcdsdevices-8.4.0/pcdsdevices/digitizers.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/doc_stubs.py` & `pcdsdevices-8.4.0/pcdsdevices/doc_stubs.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/energy_monitor.py` & `pcdsdevices-8.4.0/pcdsdevices/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/epics_motor.py` & `pcdsdevices-8.4.0/pcdsdevices/epics_motor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1365,15 +1365,15 @@
 
 
 class SmarActOpenLoop(Device):
     """
     Class containing the open loop PVs used to control an un-encoded SmarAct
     stage.
 
-    Can be used for sub-classing, or creating a simple  device without the
+    Can be used for sub-classing, or creating a simple device without the
     motor record PVs.
     """
 
     # Voltage for sawtooth ramp
     step_voltage = Cpt(EpicsSignal, ':STEP_VOLTAGE', kind='omitted',
                        doc='Voltage for sawtooth (0-100V)')
     # Frequency of steps
@@ -1397,19 +1397,24 @@
     step_clear_cmd = Cpt(EpicsSignal, ':CLEAR_COUNT', kind='config',
                          doc='Clear the current step count')
     set_metadata(step_clear_cmd, dict(variety='command-proc', value=1))
     # Scan move
     scan_move = Cpt(EpicsSignal, ':SCAN_POS', write_pv=':SCAN_MOVE',
                     kind='config',
                     doc='Set current piezo voltage (in 16 bit ADC steps)')
+    # Diagnostic read only PVs
+    channel_temp = Cpt(EpicsSignalRO, ':CHANTEMP', kind='normal',
+                       doc="Temperature at the channel's amplifier")
+    module_temp = Cpt(EpicsSignalRO, ':MODTEMP', kind='normal',
+                      doc='Temperature of the MCS2 Module in the rack')
 
 
 class SmarActTipTilt(Device):
     """
-    Class for bundling two SmarActOpenLoop axes arranged in a tip-tilt mirro
+    Class for bundling two SmarActOpenLoop axes arranged in a tip-tilt mirror
     positioning configuration into a single device.
 
     Parameters:
     -----------
     prefix : str <optional, default=''>
         The base PV of the stages. Can be omitted, but then tip_pv and
         tilt_pv must specify the full stage PV.
@@ -1466,19 +1471,52 @@
 
     # Calibration - only works for encoded stages
     needs_calib = Cpt(EpicsSignalRO, ':NEED_CALIB', kind='config')
 
     do_calib = Cpt(EpicsSignal, ':DO_CALIB.PROC', kind='config')
     set_metadata(do_calib, dict(variety='command-proc', value=1))
 
+    # Configuration for settings in NVRAM
+    log_scale_offset = Cpt(EpicsSignal, ':LSCO', write_pv=':SET_LSCO',
+                           kind='omitted', doc='Logical Scale Offset')
+    def_range_min = Cpt(EpicsSignal, ':DRMIN', write_pv=':SET_DRMIN',
+                        kind='omitted', doc='Default Range Minimum')
+    def_range_max = Cpt(EpicsSignal, ':DRMAX', write_pv=':SET_DRMAX',
+                        kind='omitted', doc='Default Range Maximum')
+    log_scale_inv = Cpt(EpicsSignal, ':LSCI_RBV', write_pv=':SET_LSCI',
+                        kind='omitted', doc='Default Range Minimum')
+    dist_code_inv = Cpt(EpicsSignal, ':DCIN_RBV', write_pv=':SET_DCIN',
+                        kind='omitted', doc='Distance Code Inversion')
+
+    # Diagnostic read only PVs
+    channel_temp = Cpt(EpicsSignalRO, ':CHANTEMP', kind='normal',
+                       doc="Temperature at the channel's amplifier")
+    module_temp = Cpt(EpicsSignalRO, ':MODTEMP', kind='normal',
+                      doc='Temperature of the MCS2 Module in the rack')
+
     # These PVs will probably not be needed for most encoded motors, but can be
     # useful
     open_loop = Cpt(SmarActOpenLoop, '', kind='omitted')
 
 
+class SmarActEncodedTipTilt(Device):
+    """
+    Class for bundling two SmarAct encoded axes arranged in a tip-tilt mirror
+    positioning configuration into a single device.
+    Refer to SmarActTipTilt for more info.
+    """
+    tip = FCpt(SmarAct, '{prefix}{self._tip_pv}', kind='normal')
+    tilt = FCpt(SmarAct, '{prefix}{self._tip_pv}', kind='normal')
+
+    def __init__(self, prefix='', *, tip_pv, tilt_pv, **kwargs):
+        self._tip_pv = tip_pv
+        self._tilt_pv = tilt_pv
+        super().__init__(prefix, **kwargs)
+
+
 def _GetMotorClass(basepv):
     """
     Function to determine the appropriate motor class based on the PV.
     """
     # Available motor types
     motor_types = (('MMS', IMS),
                    ('CLZ', IMS),
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/eps.py` & `pcdsdevices-8.4.0/pcdsdevices/eps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/evr.py` & `pcdsdevices-8.4.0/pcdsdevices/evr.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/example.py` & `pcdsdevices-8.4.0/pcdsdevices/example.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/fms.py` & `pcdsdevices-8.4.0/pcdsdevices/fms.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/gauge.py` & `pcdsdevices-8.4.0/pcdsdevices/gauge.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/gon.py` & `pcdsdevices-8.4.0/pcdsdevices/gon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/happi/containers.py` & `pcdsdevices-8.4.0/pcdsdevices/happi/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -535,14 +535,16 @@
     ioc_alias = EntryInfo('Optional PV alias to give this axis.',
                           optional=True, enforce=str)
 
 
 class SmarActTipTiltMotor(LCLSItem):
     """
     Container for SmarAct tip-tilt motor pairs.
+    Use pcdsdevices.epics_motor.SmarActEncodedTipTilt device_class for
+    encoded tip-tilts.
     """
     device_class = copy(LCLSItem.device_class)
     device_class.default = 'pcdsdevices.epics_motor.SmarActTipTilt'
     ioc_type = copy(LCLSItem.ioc_type)
     ioc_type.default = 'SmarAct'
     kwargs = deepcopy(LegacyItem.kwargs)
     args = deepcopy(LegacyItem.args)
@@ -662,14 +664,18 @@
     ioc_type = copy(LCLSItem.ioc_type)
     ioc_type.default = 'EK9000'
     ioc_ip = EntryInfo(('Netconfig name of the EK9000 the sensors are '
                         'connected to. Used to build IOC configs.'),
                        optional=True, enforce=str)
     ioc_base = EntryInfo('Base PV of the EK9000 IOC', optional=True,
                          enforce=str)
+    ioc_chan_num = EntryInfo('Channel number for the environmental monitor.',
+                             optional=True, enforce=str)
+    ioc_card_num = EntryInfo('Card number for the environmental monitor.',
+                             optional=True, enforce=str)
 
 
 class Leviton(LCLSItem):
     kwargs = deepcopy(LCLSItem.kwargs)
     kwargs.default['elevations'] = "{{elevations}}"
     elevations = EntryInfo(doc='List of elevation numbers for rack',
                            optional=False, enforce=list)
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/inout.py` & `pcdsdevices-8.4.0/pcdsdevices/inout.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/interface.py` & `pcdsdevices-8.4.0/pcdsdevices/interface.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ipm.py` & `pcdsdevices-8.4.0/pcdsdevices/ipm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/jet.py` & `pcdsdevices-8.4.0/pcdsdevices/jet.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/keithley.py` & `pcdsdevices-8.4.0/pcdsdevices/keithley.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lamp_motion.py` & `pcdsdevices-8.4.0/pcdsdevices/lamp_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/btms_config.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/btms_config.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/btps.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/btps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/counters.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/counters.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/dicon.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/dicon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/ek9000.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/ek9000.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/elliptec.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/elliptec.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/qmini.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/qmini.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/rfof.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/rfof.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/thorlabsWFS.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/thorlabsWFS.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/tuttifrutti.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/tuttifrutti.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lasers/zoomtelescope.py` & `pcdsdevices-8.4.0/pcdsdevices/lasers/zoomtelescope.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lens.py` & `pcdsdevices-8.4.0/pcdsdevices/lens.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lic.py` & `pcdsdevices-8.4.0/pcdsdevices/lic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/light_control.py` & `pcdsdevices-8.4.0/pcdsdevices/light_control.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lodcm.py` & `pcdsdevices-8.4.0/pcdsdevices/lodcm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/lxe.py` & `pcdsdevices-8.4.0/pcdsdevices/lxe.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """
 'lxe' position / pulse energy pseudopositioner support.
-
 Notes
 -----
 OPA::
 
     An optical parametric amplifier, abbreviated OPA, is a laser light source
     that emits light of variable wavelengths by an optical parametric
     amplification process. It is essentially the same as an optical parametric
@@ -384,14 +383,173 @@
             # convert from ns to s
             return f'{(dial_pos * 1e-9):.3e}'
         except Exception:
             return 'N/A'
 
     def format_status_info(self, status_info):
         """
+        Override status info handler to render the LXT motor.
+
+        Display lxt motor status info in the ipython terminal.
+
+        Parameters
+        ----------
+        status_info: dict
+            Nested dictionary. Each level has keys name, kind, and is_device.
+            If is_device is True, subdevice dictionaries may follow. Otherwise,
+            the only other key in the dictionary will be value.
+
+        Returns
+        -------
+        status: str
+            Formatted string with all relevant status information.
+        """
+        dial_pos = self.dial_pos
+        position = get_status_float(
+            status_info, 'position', precision=3, format='e')
+        units = get_status_value(status_info, 'setpoint', 'units')
+        return f"""\
+Virtual Motor {self.verbose_name} {self.prefix}
+Current position (user, dial): {position} [{units}] {dial_pos} [s]
+"""
+
+
+class Lcls2LaserTiming(FltMvInterface, PVPositioner):
+    """
+    A "lxt" motor for the LCLS-II laser locker, AKA the OPCPA laser locker.
+    """
+
+    tab_component_names = True
+
+    verbose_name = 'Laser X-ray Timing'
+
+    _tgt_time = Cpt(EpicsSignal, ':PHASCTL:DELAY_SET', auto_monitor=True,
+                    kind='omitted',
+                    doc='The internal nanosecond-expecting signal.'
+                    )
+    setpoint = Cpt(_ScaledUnitConversionDerivedSignal,
+                   derived_from='_tgt_time',
+                   derived_units='s',
+                   original_units='ns',
+                   kind='hinted',
+                   doc='Setpoint which handles the timing conversion.',
+                   limits=(-100e-6, 100e-6),
+                   )
+    notepad_setpoint = Cpt(NotepadLinkedSignal, ':lxt:OphydSetpoint',
+                           notepad_metadata={'record': 'ao',
+                                             'default_value': 0.0},
+                           kind='omitted'
+                           )
+    notepad_readback = Cpt(NotepadLinkedSignal, ':lxt:OphydReadback',
+                           notepad_metadata={'record': 'ao',
+                                             'default_value': 0.0},
+                           kind='omitted'
+                           )
+    user_offset = Cpt(NotepadLinkedSignal, ':lxt:OphydOffset',
+                      notepad_metadata={'record': 'ao', 'default_value': 0.0},
+                      kind='normal',
+                      doc='A Python-level user offset.'
+                      )
+
+    # The phase shifter will be moved after the above record is touched, so
+    # use its done status:
+    done = Cpt(EpicsSignal, ':PHASCTL:DELAY_MOVING', auto_monitor=True, kind='omitted')
+    done_value = 0
+
+    def __init__(self, prefix='', *, egu=None, **kwargs):
+        if egu not in (None, 's'):
+            raise ValueError(
+                f'{self.__class__.__name__} is pre-configured to work in units'
+                f' of seconds.'
+            )
+        super().__init__(prefix, egu='s', **kwargs)
+
+    @user_offset.sub_value
+    def _offset_changed(self, value, **kwargs):
+        """
+        The user offset was changed.  Update the setpoint attribute.
+        """
+        self.setpoint.user_offset = value
+
+    def _setup_move(self, position):
+        """Update the notepad setpoint, move, and do not wait."""
+        try:
+            signal = self.notepad_setpoint
+            if signal.connected and signal.write_access:
+                if signal.get(use_monitor=True) != position:
+                    signal.put(position, wait=False)
+        except Exception as ex:
+            self.log.debug('Failed to update notepad setpoint to position %s',
+                           position, exc_info=ex)
+        super()._setup_move(position)
+
+    @done.sub_value
+    def _update_position(self, old_value=None, value=None, **kwargs):
+        """The move was completed. Update the notepad readback."""
+        if value == self.done_value and old_value == 0:
+            try:
+                signal = self.notepad_readback
+                position = self.setpoint.get()
+                if signal.connected and signal.write_access:
+                    if signal.get(use_monitor=True) != position:
+                        signal.put(position, wait=False)
+            except Exception as ex:
+                self.log.debug('Failed to update notepad readback to position'
+                               ' %s', position, exc_info=ex)
+
+    @property
+    def limits(self):
+        """
+        Limits as (low_limit, high_limit).
+
+        These Python-only user limits are mirrored from `setpoint`.
+        """
+        return self.setpoint.limits
+
+    @limits.setter
+    def limits(self, limits):
+        # Update the setpoint limits
+        self.setpoint.limits = limits
+
+    def set_current_position(self, position):
+        '''
+        Calculate and configure the user_offset value, indicating the provided
+        ``position`` as the new current position.
+
+        Parameters
+        ----------
+        position
+            The new current position.
+        '''
+        self.user_offset.put(0.0)
+        new_offset = position - self.setpoint.get()
+        self.user_offset.put(new_offset)
+
+    @property
+    def dial_pos(self):
+        """
+        Calculate the dial position.
+
+        The _tgt_time is the actual dial_position in ns.
+
+        Returns
+        -------
+        dial_pos : number
+            The dial position in [s] seconds, or 'N/A' if the dial position is
+            0 or None.
+        """
+        try:
+            dial_pos = self._tgt_time.get()
+            # convert from ns to s
+            return f'{(dial_pos * 1e-9):.3e}'
+        except Exception:
+            return 'N/A'
+
+    def format_status_info(self, status_info):
+        """
         Override status info handler to render the LXT motor.
 
         Display lxt motor status info in the ipython terminal.
 
         Parameters
         ----------
         status_info: dict
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/make_ophyd_device.py` & `pcdsdevices-8.4.0/pcdsdevices/make_ophyd_device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/mirror.py` & `pcdsdevices-8.4.0/pcdsdevices/mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -739,27 +739,31 @@
 
 class XOffsetMirrorNoBend(XOffsetMirror):
     """
     X-ray Offset Mirror with no bender.
 
     2nd gen Axilon designs with LCLS-II Beckhoff motion architecture.
 
+    With variable cooling valve installed.
+
     Parameters
     ----------
     prefix : str
         Base PV for the mirror.
 
     name : str
 
     Currently (10/11/2023) services: mr1l1
 
     """
     bender = None
     bender_enc_rms = None
 
+    variable_cool = Cpt(PytmcSignal, ':VCV', kind='normal', io='io', doc='Activates variable cooling valve')
+
 
 class XOffsetMirrorBend(XOffsetMirror):
     """
     X-ray Offset Mirror with 2 bender acutators.
 
     1st and 2nd gen Axilon designs with LCLS-II Beckhoff motion architecture.
 
@@ -1406,26 +1410,30 @@
 
     1st and 2nd gen Axilon designs with LCLS-II Beckhoff motion architecture.
 
     With Coating State selection implemented.
 
     With cooling and pressure meters installed.
 
+    With variable cooling valve installed.
+
     Parameters
     ----------
     prefix : str
         Base PV for the mirror.
 
     name : str
         Alias for the device.
     """
     # Cooling
-    cool_flow1 = Cpt(EpicsSignalRO, ':FWM:1_RBV', kind='normal')
-    cool_flow2 = Cpt(EpicsSignalRO, ':FWM:2_RBV', kind='normal')
-    cool_press = Cpt(EpicsSignalRO, ':PRSM:1_RBV', kind='normal')
+    cool_flow1 = Cpt(EpicsSignalRO, ':FWM:1_RBV', kind='normal', doc='Mirror cooling panel loop flow sensor')
+    cool_flow2 = Cpt(EpicsSignalRO, ':FWM:2_RBV', kind='normal', doc='Mirror cooling panel loop flow sensor')
+    cool_press = Cpt(EpicsSignalRO, ':PRSM:1_RBV', kind='normal', doc='Mirror cooling panel loop pressure sensor')
+
+    variable_cool = Cpt(PytmcSignal, ':VCV', kind='normal', io='io', doc='Activates variable cooling valve')
 
 
 class MirrorInsertState(TwinCATStatePMPS):
     """
     A state positioner with two states (3 including Unknown) representing
     insertion state of mirror
     """
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/movablestand.py` & `pcdsdevices-8.4.0/pcdsdevices/movablestand.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/mpod.py` & `pcdsdevices-8.4.0/pcdsdevices/mpod.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/mpod_apalis.py` & `pcdsdevices-8.4.0/pcdsdevices/mpod_apalis.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,37 @@
 
     current_ramp_speed = Cpt(EpicsSignal, ':CurrentRampSpeed', kind='normal',
                              doc='MPOD module current Ramp  Rate [%/sec*Inom]')
 
     temperature = Cpt(EpicsSignalRO, ':Temperature', kind='normal',
                       doc='MPOD Temperature [C]')
 
+    supply_status = Cpt(EpicsSignalRO, ':isSupplyGood', kind='normal',
+                        doc='Supply voltages are within range')
+
+    module_status = Cpt(EpicsSignalRO, ':isModuleGood', kind='normal',
+                        doc='Module health status')
+
+    fine_adjustment_status = Cpt(EpicsSignalRO, ':isFineAdjustment',
+                                 kind='normal', doc='Fine adjustment mode status')
+
+    input_status = Cpt(EpicsSignalRO, ':isInputError', kind='normal',
+                       doc='Input error in connection with a module access')
+
+    live_insertion_status = Cpt(EpicsSignalRO, ':isLiveInsertion',
+                                kind='normal', doc='Live insertion mode status')
+
+    saftey_loop_status = Cpt(EpicsSignalRO, ':isSafetyLoopGood',
+                             kind='normal', doc='Saftey loop status')
+
+    kill = Cpt(EpicsSignal, ':isKillEnable',
+               write_pv=':Control:setKillEnable',
+               kind='normal', string=True,
+               doc='Module-wide kill functionality')
+
     faults = Cpt(EpicsSignal, ':isEventActive',
                  write_pv=':Control:doClear',
                  kind='normal', string=True,
                  doc='Clears all MPOD module faults')
 
     tab_component_names = True
     tab_whitelist = ['clear_faults', 'set_voltage_ramp_speed',
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/mps.py` & `pcdsdevices-8.4.0/pcdsdevices/mps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/mrco_motion.py` & `pcdsdevices-8.4.0/pcdsdevices/mrco_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/piezo.py` & `pcdsdevices-8.4.0/pcdsdevices/piezo.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/pim.py` & `pcdsdevices-8.4.0/pcdsdevices/pim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/pmps.py` & `pcdsdevices-8.4.0/pcdsdevices/pmps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/pneumatic.py` & `pcdsdevices-8.4.0/pcdsdevices/pneumatic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/positioner.py` & `pcdsdevices-8.4.0/pcdsdevices/positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/pseudopos.py` & `pcdsdevices-8.4.0/pcdsdevices/pseudopos.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/pulsepicker.py` & `pcdsdevices-8.4.0/pcdsdevices/pulsepicker.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/pump.py` & `pcdsdevices-8.4.0/pcdsdevices/pump.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/pv_positioner.py` & `pcdsdevices-8.4.0/pcdsdevices/pv_positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/qadc.py` & `pcdsdevices-8.4.0/pcdsdevices/qadc.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/radiation.py` & `pcdsdevices-8.4.0/pcdsdevices/radiation.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ref.py` & `pcdsdevices-8.4.0/pcdsdevices/ref.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/rs_powersupply.py` & `pcdsdevices-8.4.0/pcdsdevices/rs_powersupply.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/rtds_ebd.py` & `pcdsdevices-8.4.0/pcdsdevices/rtds_ebd.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/sample_delivery.py` & `pcdsdevices-8.4.0/pcdsdevices/sample_delivery.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/sensors.py` & `pcdsdevices-8.4.0/pcdsdevices/sensors.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/sequencer.py` & `pcdsdevices-8.4.0/pcdsdevices/sequencer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/signal.py` & `pcdsdevices-8.4.0/pcdsdevices/signal.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/sim.py` & `pcdsdevices-8.4.0/pcdsdevices/sim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/slits.py` & `pcdsdevices-8.4.0/pcdsdevices/slits.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/spectrometer.py` & `pcdsdevices-8.4.0/pcdsdevices/spectrometer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/sqr1.py` & `pcdsdevices-8.4.0/pcdsdevices/sqr1.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/state.py` & `pcdsdevices-8.4.0/pcdsdevices/state.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/stopper.py` & `pcdsdevices-8.4.0/pcdsdevices/stopper.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/sxr_test_absorber.py` & `pcdsdevices-8.4.0/pcdsdevices/sxr_test_absorber.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/targets.py` & `pcdsdevices-8.4.0/pcdsdevices/targets.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/conftest.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_analog_signals.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_analog_signals.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_attenuator.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_attenuator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_beam_stats.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_beam_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,22 +103,22 @@
     tmo_request = BeamEnergyRequest('TMO', name='tmo_request', atol=4)
     assert tmo_request.setpoint.pvname == 'TMO:USER:MCC:EPHOTK:SET1'
     # Future TXI and multi-bunch specific options
     tst_k1_request = BeamEnergyRequest(
         'TST',
         name='tst_k1_request',
         line='k',
-        bunch=1,
+        pv_index=1,
     )
     assert tst_k1_request.setpoint.pvname == 'TST:USER:MCC:EPHOTK:SET1'
     tst_l2_request = BeamEnergyRequest(
         'TST',
         name='tst_l2_request',
         line='L',
-        bunch=2,
+        pv_index=2,
     )
     assert tst_l2_request.setpoint.pvname == 'TST:USER:MCC:EPHOT:SET2'
     # let's test the class splitting here too
     for obj in (
         xpp_request,
         tmo_request,
         tst_k1_request,
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_btms.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_btms.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_ccm.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_ccm.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     init_pos(fake_ccm.y.down)
     init_pos(fake_ccm.y.up_north)
     init_pos(fake_ccm.y.up_south)
 
     fake_ccm.alio.set(SAMPLE_ALIO)
     fake_ccm.energy.alio.set(SAMPLE_ALIO)
     fake_ccm.energy_with_vernier.alio.set(SAMPLE_ALIO)
-    fake_ccm.energy_with_vernier.vernier.setpoint.sim_put(0)
+    fake_ccm.energy_with_vernier.acr_energy.setpoint.sim_put(0)
 
     return fake_ccm
 
 
 def test_fake_ccm(fake_ccm):
     logger.debug('test_fake_ccm')
     fake_ccm.get()
@@ -161,34 +161,34 @@
     logger.debug('test_vernier')
 
     pseudopos = fake_ccm.energy_with_vernier
 
     # Moving with vernier should move the energy request motor too
     pseudopos.move(7, wait=False)
     assert np.isclose(pseudopos.energy.position, 7)
-    assert pseudopos.vernier.position == 7000
+    assert pseudopos.acr_energy.position == 7000
 
     pseudopos.move(8, wait=False)
     assert np.isclose(pseudopos.energy.position, 8)
-    assert pseudopos.vernier.position == 8000
+    assert pseudopos.acr_energy.position == 8000
 
     pseudopos.move(9, wait=False)
     assert np.isclose(pseudopos.energy.position, 9)
-    assert pseudopos.vernier.position == 9000
+    assert pseudopos.acr_energy.position == 9000
 
     # Small moves (less than 30eV) should be skipped on the energy request
-    pseudopos.move(9.001, wait=False)
-    assert np.isclose(pseudopos.energy.position, 9.001)
-    assert pseudopos.vernier.position == 9000
+    pseudopos.move(9.0001, wait=False)
+    assert np.isclose(pseudopos.energy.position, 9.0001)
+    assert pseudopos.acr_energy.position == 9000
 
     # Unless we set the option for not skipping them
-    pseudopos.vernier.skip_small_moves = False
+    pseudopos.acr_energy.skip_small_moves = False
     pseudopos.move(9.002, wait=False)
     assert np.isclose(pseudopos.energy.position, 9.002)
-    assert pseudopos.vernier.position == 9002
+    assert pseudopos.acr_energy.position == 9002
 
 
 @pytest.mark.timeout(5)
 def test_set_current_position(fake_ccm):
     logger.debug('test_set_current_position')
     mot = fake_ccm.energy.energy
     for energy in range(6, 14):
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_crix_motion.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_crix_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_dc_devices.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_dc_devices.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_device.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_disconnected.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_disconnected.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_entrypoints.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_epics_motor.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_epics_motor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_gauge.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_gauge.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_gon.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_gon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_inout.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_inout.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_interface.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_ipm.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_ipm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_jet.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_jet.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_lens.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_lens.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_lodcm.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_lodcm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_lxe.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_lxe.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_movablestand.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_movablestand.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_mpod.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_mpod.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_mpod_apalis.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_mpod_apalis.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_mps.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_mps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_pim.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_pim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_pneumatic.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_pneumatic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_positioner.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_pseudopos.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_pseudopos.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_pulsepicker.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_pulsepicker.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_pump.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_pump.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_pv_positioner.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_pv_positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_sample_delivery.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_sample_delivery.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_sequencer.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_sequencer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_signal.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_slits.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_slits.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_spectrometer.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_spectrometer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_state.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_targets.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_targets.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_timetool.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_timetool.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_utils.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_valve.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/test_variety.py` & `pcdsdevices-8.4.0/pcdsdevices/tests/test_variety.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tests/xcslt8717_wpcalib_opa` & `pcdsdevices-8.4.0/pcdsdevices/tests/xcslt8717_wpcalib_opa`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/timetool.py` & `pcdsdevices-8.4.0/pcdsdevices/timetool.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/tpr.py` & `pcdsdevices-8.4.0/pcdsdevices/tpr.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 class TimingMode(Enum):
     LCLS1 = 1
     LCLS2 = 2
 
 
 def _get_delay(mds: MultiDerivedSignal, items: SignalToValue) -> float:
     """Calculates delay in ns from ticks and taps"""
-    return items[mds.attrs[0]] * TPR_TICK_NS + items[mds.attrs[1] * TPR_TAP_NS]
+    return items[mds.signals[0]] * TPR_TICK_NS + items[mds.signals[1]] * TPR_TAP_NS
 
 
 def _get_width(mds: MultiDerivedSignal, items: SignalToValue) -> float:
     """Calculates width in ns from ticks"""
-    return items[mds.attrs[0]] * TPR_TICK_NS
+    return items[mds.signals[0]] * TPR_TICK_NS
 
 
 def _put_last(mds: MultiDerivedSignal, value: float) -> SignalToValue:
     """Only writes value to last attr"""
-    return {mds.attrs[-1]: value}
+    return {mds.signals[-1]: value}
 
 
 class TprMotor(PVPositionerIsClose):
     """
     PV Positioner for adjusting an TPR channel.
 
     Moves that are less than one tick
@@ -57,24 +57,24 @@
         self.sys = sys
         super().__init__(prefix, name=name, **kwargs)
 
 
 class TprTrigger(BaseInterface, Device):
     """Class for an individual TprTrigger."""
     ratemode = FCpt(EpicsSignal, '{self.prefix}{self.ch}RATEMODE', kind="config", doc="Channel rate mode selector")
-    group = FCpt(EpicsSignal, '{self.prefix}{self.ch}GROUP', kind="omitted", doc="Channel group Bit")
-    seqcode = FCpt(EpicsSignal, '{self.prefix}{self.ch}SEQCODE', kind="omitted", doc="Channel sequence code")
-    fixedrate = FCpt(EpicsSignal, '{self.prefix}{self.ch}FIXEDRATE', kind="omitted", doc="Channel Fxed rate selector")
+    group = FCpt(EpicsSignal, '{self.prefix}{self.ch}GROUP', kind="config", doc="Channel group Bit")
+    seqcode = FCpt(EpicsSignal, '{self.prefix}{self.ch}SEQCODE', kind="config", doc="Channel sequence code")
+    fixedrate = FCpt(EpicsSignal, '{self.prefix}{self.ch}FIXEDRATE', kind="config", doc="Channel Fxed rate selector")
     count = FCpt(EpicsSignal, '{self.prefix}{self.ch}CNT', kind="omitted", doc="Channel counter")
-    destmask = FCpt(EpicsSignal, '{self.prefix}{self.ch}DESTMASK', kind="omitted", doc="Channel destination mask")
-    destmode = FCpt(EpicsSignal, '{self.prefix}{self.ch}DESTMODE', kind="omitted", doc="Channel destination mode selector")
-    src = FCpt(EpicsSignal, '{self.prefix}{self.trg}SOURCE', kind="omitted", doc="Trigger source")
+    destmask = FCpt(EpicsSignal, '{self.prefix}{self.ch}DESTMASK', kind="config", doc="Channel destination mask")
+    destmode = FCpt(EpicsSignal, '{self.prefix}{self.ch}DESTMODE', kind="config", doc="Channel destination mode selector")
+    src = FCpt(EpicsSignal, '{self.prefix}{self.trg}SOURCE', kind="config", doc="Trigger source")
     eventcode = FCpt(EpicsSignal, '{self.prefix}{self.ch}EVCODE', kind="config", doc="Channel LCLS1 event code")
     eventrate = FCpt(EpicsSignalRO, '{self.prefix}{self.ch}RATE', kind="normal", doc="Channel event rates")
-    label = FCpt(EpicsSignal, '{self.prefix}{self.ch}{self.sys}TCTL.DESC', kind="omitted", doc="Enable/disable")
+    label = FCpt(EpicsSignal, '{self.prefix}{self.ch}{self.sys}TCTL.DESC', kind="normal", doc="Channel description")
     delay_ticks = FCpt(EpicsSignal, '{self.prefix}{self.trg}TDESTICKS', kind="omitted", doc="Trigger delay in clock ticks")
     delay_taps = FCpt(EpicsSignal, '{self.prefix}{self.trg}TDESTAPS', kind="omitted", doc="Trigger delay in delay taps")
     delay_setpoint = FCpt(EpicsSignal, '{self.prefix}{self.trg}{self.sys}TDES', kind="omitted", doc="Trigger delay setpoint in nsec")
     ns_delay = Cpt(
         MultiDerivedSignal,
         attrs=['delay_ticks', 'delay_taps', 'delay_setpoint'],
         calculate_on_get=_get_delay,
@@ -88,18 +88,19 @@
     width = Cpt(
         MultiDerivedSignal,
         attrs=['width_ticks', 'width_setpoint'],
         calculate_on_get=_get_width,
         calculate_on_put=_put_last,
         doc="Get/set trigger width in nsec",
     )
-    enable_ch_cmd = FCpt(EpicsSignal, '{self.prefix}{self.ch}{self.sys}TCTL', kind="omitted", doc="Channel enable/disable")
+    enable_ch_cmd = FCpt(EpicsSignal, '{self.prefix}{self.ch}{self.sys}TCTL', kind="config", doc="Channel enable/disable")
     set_metadata(enable_ch_cmd, dict(variety='command-proc', value=1))
-    enable_trg_cmd = FCpt(EpicsSignal, '{self.prefix}{self.trg}{self.sys}TCTL', kind="omitted", doc="Trigger enable/disable")
+    enable_trg_cmd = FCpt(EpicsSignal, '{self.prefix}{self.trg}{self.sys}TCTL', kind="config", doc="Trigger enable/disable")
     set_metadata(enable_trg_cmd, dict(variety='command-proc', value=1))
+    operation = FCpt(EpicsSignal, '{self.prefix}{self.trg}TCMPL', kind="config", doc="Trigger complementary logic")
 
     tab_whitelist = ['enable', 'disable']
     tab_component_names = True
 
     def __init__(self, prefix, *, channel, timing_mode, name, **kwargs):
         if timing_mode == TimingMode.LCLS1:
             self.sys = 'SYS0_'
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/type_hints.py` & `pcdsdevices-8.4.0/pcdsdevices/type_hints.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AT1K2.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AT1K2.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AT1K2.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AT1K2.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AT2L0.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AT2L0.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AT2L0.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AT2L0.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffAxisEPSCustom.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffAxisEPSCustom.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/BtpsState.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/BtpsState.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/BtpsState.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/BtpsState.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/IM3L0_K2700.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/IM3L0_K2700.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/IM3L0_K2700.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/IM3L0_K2700.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/JJSlits.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/JJSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/LCP.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/LCP.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/Leviton1.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/Leviton1.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/LightControl.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/LightControl.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/PowerSlits.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/PowerSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/PowerSlits.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/PowerSlits.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/Setra5000.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/Setra5000.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/StatePositioner.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/StatePositioner.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/StatePositioner.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/StatePositioner.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-camera-summary.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-camera-summary.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-config.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-overview.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-range-config.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-range-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-range-summary.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-range-summary.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-source-dest.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-source-dest.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-source-tabs-config.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-source-tabs-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-source-tabs.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-source-tabs.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps-source-valves.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps-source-valves.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/btps.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/btps.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/ui/detailed_tree.ui` & `pcdsdevices-8.4.0/pcdsdevices/ui/detailed_tree.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/usb_encoder.py` & `pcdsdevices-8.4.0/pcdsdevices/usb_encoder.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/utils.py` & `pcdsdevices-8.4.0/pcdsdevices/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,35 @@
 ctrl_arrow_down = '\x1b[1;5B'
 ctrl_arrow_right = '\x1b[1;5C'
 ctrl_arrow_left = '\x1b[1;5D'
 plus = '+'
 minus = '-'
 
 
+def re_arg(kwarg_map):
+    """
+    Decorator to redefine a kwarg to a function, while still supporting the old kwarg, and warning the end user.
+
+    Usage:
+    @re_arg({"new_kwarg": "old_kwarg"})
+    def myfunc(*args, new_kwarg=<a_value>, **kwargs):
+        ...
+    """
+    def decorator(func):
+        def wrapped(*args, **kwargs):
+            new_kwargs = {}
+            for k, v in kwargs.items():
+                if k in kwarg_map:
+                    print(f"DEPRECATION WARNING: keyword argument '{k}' is no longer valid. Use '{kwarg_map[k]}' instead.")
+                new_kwargs[kwarg_map.get(k, k)] = v
+            return func(*args, **new_kwargs)
+        return wrapped
+    return decorator
+
+
 def is_input():
     """
     Utility to check if there is input available.
 
     Returns
     -------
     is_input : bool
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices/valve.py` & `pcdsdevices-8.4.0/pcdsdevices/valve.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/variety.py` & `pcdsdevices-8.4.0/pcdsdevices/variety.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/version.py` & `pcdsdevices-8.4.0/pcdsdevices/version.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices/wfs.py` & `pcdsdevices-8.4.0/pcdsdevices/wfs.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-8.3.0/pcdsdevices.egg-info/PKG-INFO` & `pcdsdevices-8.4.0/pcdsdevices.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsdevices
-Version: 8.3.0
+Version: 8.4.0
 Summary: Ophyd Device definitions for LCLS Beamline components
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `pcdsdevices-8.3.0/pcdsdevices.egg-info/SOURCES.txt` & `pcdsdevices-8.4.0/pcdsdevices.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 pcdsdevices/interface.py
 pcdsdevices/ipm.py
 pcdsdevices/jet.py
 pcdsdevices/keithley.py
 pcdsdevices/lamp_motion.py
 pcdsdevices/lens.py
 pcdsdevices/lic.py
+pcdsdevices/lic_2d_tmo.py
 pcdsdevices/light_control.py
 pcdsdevices/lodcm.py
 pcdsdevices/lxe.py
 pcdsdevices/make_ophyd_device.py
 pcdsdevices/mirror.py
 pcdsdevices/movablestand.py
 pcdsdevices/mpod.py
@@ -104,14 +105,15 @@
 pcdsdevices/rtds_ebd.py
 pcdsdevices/sample_delivery.py
 pcdsdevices/sensors.py
 pcdsdevices/sequencer.py
 pcdsdevices/signal.py
 pcdsdevices/sim.py
 pcdsdevices/slits.py
+pcdsdevices/smarpod.py
 pcdsdevices/spectrometer.py
 pcdsdevices/sqr1.py
 pcdsdevices/state.py
 pcdsdevices/stopper.py
 pcdsdevices/sxr_test_absorber.py
 pcdsdevices/tags.py
 pcdsdevices/targets.py
@@ -232,14 +234,15 @@
 pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
 pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
 pcdsdevices/ui/AttenuatorCalculator_filter.ui
 pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
 pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
 pcdsdevices/ui/BeckhoffAxis.detailed.ui
 pcdsdevices/ui/BeckhoffAxis.embedded.ui
+pcdsdevices/ui/BeckhoffAxisEPSCustom.embedded.ui
 pcdsdevices/ui/BeckhoffAxisEPSCustom.ui
 pcdsdevices/ui/BeckhoffSlits.detailed.ui
 pcdsdevices/ui/BeckhoffSlits.embedded.ui
 pcdsdevices/ui/BtpsState.detailed.ui
 pcdsdevices/ui/BtpsState.embedded.ui
 pcdsdevices/ui/IM3L0_K2700.detailed.ui
 pcdsdevices/ui/IM3L0_K2700.embedded.ui
@@ -249,14 +252,19 @@
 pcdsdevices/ui/LightControl.ui
 pcdsdevices/ui/PowerSlits.detailed.ui
 pcdsdevices/ui/PowerSlits.embedded.ui
 pcdsdevices/ui/QminiSpectrometer.embedded.ui
 pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
 pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
 pcdsdevices/ui/Setra5000.detailed.ui
+pcdsdevices/ui/SmarPod_Pivot.ui
+pcdsdevices/ui/SmarPod_Poses.ui
+pcdsdevices/ui/SmarPod_Position.ui
+pcdsdevices/ui/SmarPod_Reference.ui
+pcdsdevices/ui/Smarpod.detailed.ui
 pcdsdevices/ui/StatePositioner.detailed.ui
 pcdsdevices/ui/StatePositioner.embedded.ui
 pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
 pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
 pcdsdevices/ui/__init__.py
 pcdsdevices/ui/at2l0_filters.json
 pcdsdevices/ui/btps-camera-summary.ui
```

### Comparing `pcdsdevices-8.3.0/pyproject.toml` & `pcdsdevices-8.4.0/pyproject.toml`

 * *Files identical despite different names*

