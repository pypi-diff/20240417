# Comparing `tmp/rad-0.19.1.tar.gz` & `tmp/rad-0.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.19.1.tar", last modified: Thu Apr  4 15:39:28 2024, max compression
+gzip compressed data, was "rad-0.19.2.tar", last modified: Wed Apr 17 15:33:51 2024, max compression
```

## Comparing `rad-0.19.1.tar` & `rad-0.19.2.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.827628 rad-0.19.1/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-04 15:39:19.000000 rad-0.19.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.803628 rad-0.19.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-04 15:39:19.000000 rad-0.19.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 15:39:19.000000 rad-0.19.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.803628 rad-0.19.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-04 15:39:19.000000 rad-0.19.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-04 15:39:19.000000 rad-0.19.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 15:39:19.000000 rad-0.19.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-04-04 15:39:19.000000 rad-0.19.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 15:39:19.000000 rad-0.19.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 15:39:19.000000 rad-0.19.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 15:39:19.000000 rad-0.19.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:19.000000 rad-0.19.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-04 15:39:28.827628 rad-0.19.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-04 15:39:19.000000 rad-0.19.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-04 15:39:19.000000 rad-0.19.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.799628 rad-0.19.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-04 15:39:19.000000 rad-0.19.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-04 15:39:19.000000 rad-0.19.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 15:39:19.000000 rad-0.19.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-04-04 15:39:19.000000 rad-0.19.1/docs/creating.rst
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-04 15:39:19.000000 rad-0.19.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-04 15:39:19.000000 rad-0.19.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 15:39:19.000000 rad-0.19.1/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-04 15:39:19.000000 rad-0.19.1/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-04 15:39:19.000000 rad-0.19.1/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-04 15:39:19.000000 rad-0.19.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-04-04 15:39:19.000000 rad-0.19.1/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-04-04 15:39:19.000000 rad-0.19.1/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:39:28.827628 rad-0.19.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.799628 rad-0.19.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/src/rad/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.819628 rad-0.19.1/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/base_exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/base_guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/fps-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ground_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/groundtest-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/msos_stack-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.823628 rad-0.19.1/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/resample-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/source_catalog-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.823628 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/target-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tvac-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.823628 rad-0.19.1/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.823628 rad-0.19.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:19.000000 rad-0.19.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:39:19.000000 rad-0.19.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-04 15:39:19.000000 rad-0.19.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 15:39:19.000000 rad-0.19.1/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-04 15:39:19.000000 rad-0.19.1/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-04 15:39:19.000000 rad-0.19.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.016332 rad-0.19.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-17 15:33:33.000000 rad-0.19.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:50.996333 rad-0.19.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-17 15:33:33.000000 rad-0.19.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-17 15:33:33.000000 rad-0.19.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:50.996333 rad-0.19.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-17 15:33:33.000000 rad-0.19.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-17 15:33:33.000000 rad-0.19.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 15:33:33.000000 rad-0.19.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 15:33:33.000000 rad-0.19.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-17 15:33:33.000000 rad-0.19.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-17 15:33:33.000000 rad-0.19.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-17 15:33:33.000000 rad-0.19.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-17 15:33:33.000000 rad-0.19.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:33.000000 rad-0.19.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-17 15:33:51.016332 rad-0.19.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-17 15:33:33.000000 rad-0.19.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-17 15:33:33.000000 rad-0.19.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:50.992333 rad-0.19.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-17 15:33:33.000000 rad-0.19.2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-17 15:33:33.000000 rad-0.19.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-17 15:33:33.000000 rad-0.19.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 15:33:33.000000 rad-0.19.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-04-17 15:33:33.000000 rad-0.19.2/docs/creating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 15:33:33.000000 rad-0.19.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-17 15:33:33.000000 rad-0.19.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 15:33:33.000000 rad-0.19.2/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-17 15:33:33.000000 rad-0.19.2/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-17 15:33:33.000000 rad-0.19.2/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-17 15:33:33.000000 rad-0.19.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-04-17 15:33:33.000000 rad-0.19.2/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-04-17 15:33:33.000000 rad-0.19.2/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:33:51.016332 rad-0.19.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:50.992333 rad-0.19.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.000332 rad-0.19.2/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.012333 rad-0.19.2/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/base_exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/base_guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/fps-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ground_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/msos_stack-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.012333 rad-0.19.2/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.016332 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/target-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tvac-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-17 15:33:33.000000 rad-0.19.2/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.016332 rad-0.19.2/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 15:33:50.000000 rad-0.19.2/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:51.016332 rad-0.19.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:33:33.000000 rad-0.19.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-17 15:33:33.000000 rad-0.19.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-17 15:33:33.000000 rad-0.19.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-17 15:33:33.000000 rad-0.19.2/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-17 15:33:33.000000 rad-0.19.2/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-17 15:33:33.000000 rad-0.19.2/tox.ini
```

### Comparing `rad-0.19.1/.github/pull_request_template.md` & `rad-0.19.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/.github/workflows/changelog.yml` & `rad-0.19.2/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/.github/workflows/ci_cron.yml` & `rad-0.19.2/.github/workflows/ci_cron.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/.github/workflows/release.yml` & `rad-0.19.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/.gitignore` & `rad-0.19.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/.pre-commit-config.yaml` & `rad-0.19.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/CHANGES.rst` & `rad-0.19.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-0.20.0 (unreleased)
+0.19.3 (unreleased)
 -------------------
 
--
+- 
+
+0.19.2 (2024-04-17)
+-------------------
+
+- Duplicated the keywords from base_exposure to exposure and similarly for base_guidestar and guidestar. [#406]
 
 0.19.1 (2024-04-04)
 -------------------
 
 - Add new schemas to documentation. [#386]
 
 - Convert tag keywords to wildcards for external tags. [#370]
```

### Comparing `rad-0.19.1/CODE_OF_CONDUCT.md` & `rad-0.19.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/LICENSE` & `rad-0.19.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/PKG-INFO` & `rad-0.19.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.1
+Version: 0.19.2
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.19.1/README.md` & `rad-0.19.2/README.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/Makefile` & `rad-0.19.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/_static/custom.css` & `rad-0.19.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/_static/stsci_logo.png` & `rad-0.19.2/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/conf.py` & `rad-0.19.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/creating.rst` & `rad-0.19.2/docs/creating.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/index.rst` & `rad-0.19.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/make.bat` & `rad-0.19.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/reference_files.rst` & `rad-0.19.2/docs/reference_files.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/docs/schemas.rst` & `rad-0.19.2/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/pyproject.toml` & `rad-0.19.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/scripts/insert_next_release.py` & `rad-0.19.2/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/scripts/set_release_date.py` & `rad-0.19.2/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/integration.py` & `rad-0.19.2/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.19.2/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/associations-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/associations-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/base_exposure-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/base_exposure-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/base_guidestar-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/base_guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/basic-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/coordinates-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/coordinates-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/ephemeris-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/exposure-1.0.0.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -3,259 +3,430 @@
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/exposure-1.0.0
 
 
 title: |
   Exposure Information
 
-allOf:
-  - $ref: asdf://stsci.edu/datamodels/roman/schemas/base_exposure-1.0.0
-  - type: object
-    properties:
-      id:
-        title: Visit Exposure ID
-        description: |
-          The matching exposure ID for a given visit ID.
+type: object
+properties:
+  type:
+    $ref: asdf://stsci.edu/datamodels/roman/schemas/exposure_type-1.0.0
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(25)
+      destination: [WFIExposure.exposure_type, GuideWindow.exposure_type, WFICommon.exposure_type]
+  start_time:
+    title: Exposure Start Time (UTC)
+    description: |
+      The UTC time at the beginning of the exposure.
+    tag: tag:stsci.edu:asdf/time/time-1.*
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: datetime2
+      destination: [WFIExposure.exposure_start_time, GuideWindow.exposure_start_time, WFICommon.exposure_start_time]
+  ngroups:
+    title: Number of Resultants
+    description: |
+      The number of resultant frames in this exposure that were transmitted to
+      the ground. The number of integrations of WFI data is always 1.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.exposure_ngroups, GuideWindow.exposure_ngroups, WFICommon.exposure_ngroups]
+  nframes:
+    title: Number of Reads
+    description: |
+      This is the number of science frames that are combined to produce a resultant frame.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.exposure_nframes, GuideWindow.exposure_nframes, WFICommon.exposure_nframes]
+  data_problem:
+    title: Data Problem
+    description: |
+      A flag indicating an issue with science telemetry.
+    type: boolean
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nchar(1)
+      destination: [WFIExposure.exposure_data_problem, GuideWindow.exposure_data_problem, WFICommon.exposure_data_problem]
+  frame_divisor:
+    title: Frame Divisor
+    description: |
+      The number of reads averaged to calculate a resultant. Value depends on
+      the readout pattern used from the MultiAccum table.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.exposure_frame_divisor, GuideWindow.exposure_frame_divisor, WFICommon.exposure_frame_divisor]
+  groupgap:
+    title: Number of Frames Dropped Between Resultants
+    description:
+      The number of reads that are dropped, or not used to calculate a
+      resultant.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.exposure_groupgap, GuideWindow.exposure_groupgap, WFICommon.exposure_groupgap]
+  frame_time:
+    title: Time Between Reads (s)
+    description: |
+      The amount of time elapsed between the end of one read and the beginning
+      of the next.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_frame_time, GuideWindow.exposure_frame_time, WFICommon.exposure_frame_time]
+  group_time:
+    title: Time Between Resultants (s)
+    description: |
+      The time that is the sum of the reads that are used to construct a
+      resultant. This will depend on the MA table being used.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_group_time, GuideWindow.exposure_group_time, WFICommon.exposure_group_time]
+  exposure_time:
+    title: Exposure Time (s)
+    description: |
+      The time between the start of the first Reset/Read Science Frame of an
+      Exposure and the completion of the final Read Only Science Frame of that
+      Exposure.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_time, GuideWindow.exposure_time, WFICommon.exposure_time]
+  ma_table_name:
+    title: MA Table Name
+    description: |
+      The name of the MultiAccum table used for this exposure, as defined in the
+      Project Reference Database.
+    type: string
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(50)
+      destination: [WFIExposure.ma_table_name, GuideWindow.ma_table_name, WFICommon.ma_table_name]
+  ma_table_number:
+    title: MA Table Number
+    description: |
+      The number of the MultiAccum table used for this exposure. Used in
+      matching exposures to their corresponding calibration data.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: smallint
+      destination: [WFIExposure.ma_table_number, GuideWindow.ma_table_number, WFICommon.ma_table_number]
+  read_pattern:
+    title: Read Pattern
+    description: |
+      Enumeration of detector reads to resultants making up the L1 data
+      downlinked from the observatory.
+    type: array
+    items:
+      type: array
+      items:
         type: integer
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: int
-          destination: [WFIExposure.exposure_id, GuideWindow.exposure_id,
-                        SourceCatalog.exposure_id]
-      mid_time:
-        title: Exposure Mid Time (UTC)
-        description: |
-          The UTC time at the midpoint of the exposure.
-        tag: tag:stsci.edu:asdf/time/time-1.*
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: datetime2
-          destination: [WFIExposure.exposure_mid_time, GuideWindow.exposure_mid_time,
-                        SourceCatalog.exposure_mid_time]
-      end_time:
-        title: Exposure End Time (UTC)
-        description: |
-          The UTC time at the end of the exposure.
-        tag: tag:stsci.edu:asdf/time/time-1.*
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: datetime2
-          destination: [WFIExposure.exposure_end_time, GuideWindow.exposure_end_time,
-                        SourceCatalog.exposure_end_time]
-      start_time_mjd:
-        title: MJD Start Time (d)
-        description: |
-          The date, in MJD, at the beginning of this exposure. Used in the archive
-          catalog for multi-mission matching.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_start_time_mjd, GuideWindow.exposure_start_time_mjd,
-                        SourceCatalog.exposure_start_time_mjd]
-      mid_time_mjd:
-        title: MJD Mid Time (d)
-        description: |
-          The date, in MJD, at the midpoint of this exposure. Used in the archive
-          catalog for multi-mission matching.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_mid_time_mjd, GuideWindow.exposure_mid_time_mjd,
-                        SourceCatalog.exposure_mid_time_mjd]
-      end_time_mjd:
-        title: MJD End Time (d)
-        description: |
-          The date, in MJD, at the end of this exposure. Used in the archive catalog
-          for multi-mission matching.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_end_time_mjd, GuideWindow.exposure_end_time_mjd,
-                        SourceCatalog.exposure_end_time_mjd]
-      start_time_tdb:
-        title: TDB Start Time (d)
-        description: |
-          The date, in TDB (Barycentric Dynamical Time), at the beginning of this
-          exposure.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_start_time_tdb, GuideWindow.exposure_start_time_tdb,
-                        SourceCatalog.exposure_start_time_tdb]
-      mid_time_tdb:
-        title: TDB Mid Time (d)
-        description: |
-          The date, in TDB (Barycentric Dynamical Time), at the midpoint of this
-          exposure.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_mid_time_tdb, GuideWindow.exposure_mid_time_tdb,
-                        SourceCatalog.exposure_mid_time_tdb]
-      end_time_tdb:
-        title: TDB End Time (d)
-        description: |
-          The date, in TDB (Barycentric Dynamical Time), at the end of this
-          exposure.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_end_time_tdb, GuideWindow.exposure_end_time_tdb,
-                        SourceCatalog.exposure_end_time_tdb]
-      sca_number:
-        title: SCA Number
-        description: |
-          The number of the detector on the Sensor Chip Assembly used for this
-          exposure.
-        type: integer
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: int
-          destination: [WFIExposure.exposure_sca_number, GuideWindow.exposure_sca_number,
-                        SourceCatalog.exposure_sca_number]
-      gain_factor:
-        title: Gain Factor
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_gain_factor, GuideWindow.exposure_gain_factor,
-                        SourceCatalog.exposure_gain_factor]
-      integration_time:
-        title: Effective Integration Time (s)
-        description:
-          The effective amount of time that the sensor was exposed to the sky.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_integration_time, GuideWindow.exposure_integration_time,
-                        SourceCatalog.exposure_integration_time]
-      elapsed_exposure_time:
-        title: Elapsed Exposure Time (s)
-        description: |
-          The amount of time elapsed between an exposure's first and last science
-          reads.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.elapsed_exposure_time, GuideWindow.elapsed_exposure_time,
-                        SourceCatalog.elapsed_exposure_time]
-      effective_exposure_time:
-        title: Effective Exposure Time (s)
-        description: |
-          The amount of time during which the detector actually collected photons
-          during an exposure.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.effective_exposure_time, GuideWindow.effective_exposure_time,
-                        SourceCatalog.effective_exposure_time]
-      duration:
-        title: Exposure Duration (s)
-        description: |
-          The amount of time dedicated to a exposure, including any overhead, time
-          spent on dropped frames, and so on.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.exposure_duration, GuideWindow.exposure_duration,
-                        SourceCatalog.exposure_duration]
-      level0_compressed:
-        title: Level 0 Compression
-        description: |
-          A flag indicating that the exposure has data that was decompressed by the
-          ground system.
-        type: boolean
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: nchar(1)
-          destination: [WFIExposure.exposure_level0_compressed, GuideWindow.exposure_level0_compressed,
-                        SourceCatalog.exposure_level0_compressed]
-      truncated:
-        title: Truncated MA Table
-        description: |
-          A flag indicating whether the MA table was truncated.
-        type: boolean
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: nchar(1)
-          destination: [WFIExposure.exposure_truncated,
-                        SourceCatalog.exposure_truncated]
-    required: [id,
-              mid_time, end_time,
-              start_time_mjd, mid_time_mjd, end_time_mjd,
-              start_time_tdb, mid_time_tdb, end_time_tdb,
-              sca_number,
-              gain_factor, integration_time, elapsed_exposure_time,
-              effective_exposure_time, duration,
-              level0_compressed]
-    propertyOrder: [id,
-              mid_time, end_time,
-              start_time_mjd, mid_time_mjd, end_time_mjd,
-              start_time_tdb, mid_time_tdb, end_time_tdb,
-              sca_number,
-              gain_factor, integration_time, elapsed_exposure_time,
-              effective_exposure_time, duration,
-              level0_compressed, truncated]
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(3500)
+      destination: [WFIExposure.read_pattern, GuideWindow.read_pattern, WFICommon.read_pattern]
+  id:
+    title: Visit Exposure ID
+    description: |
+      The matching exposure ID for a given visit ID.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.exposure_id, GuideWindow.exposure_id,
+                    SourceCatalog.exposure_id]
+  mid_time:
+    title: Exposure Mid Time (UTC)
+    description: |
+      The UTC time at the midpoint of the exposure.
+    tag: tag:stsci.edu:asdf/time/time-1.*
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: datetime2
+      destination: [WFIExposure.exposure_mid_time, GuideWindow.exposure_mid_time,
+                    SourceCatalog.exposure_mid_time]
+  end_time:
+    title: Exposure End Time (UTC)
+    description: |
+      The UTC time at the end of the exposure.
+    tag: tag:stsci.edu:asdf/time/time-1.*
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: datetime2
+      destination: [WFIExposure.exposure_end_time, GuideWindow.exposure_end_time,
+                    SourceCatalog.exposure_end_time]
+  start_time_mjd:
+    title: MJD Start Time (d)
+    description: |
+      The date, in MJD, at the beginning of this exposure. Used in the archive
+      catalog for multi-mission matching.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_start_time_mjd, GuideWindow.exposure_start_time_mjd,
+                    SourceCatalog.exposure_start_time_mjd]
+  mid_time_mjd:
+    title: MJD Mid Time (d)
+    description: |
+      The date, in MJD, at the midpoint of this exposure. Used in the archive
+      catalog for multi-mission matching.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_mid_time_mjd, GuideWindow.exposure_mid_time_mjd,
+                    SourceCatalog.exposure_mid_time_mjd]
+  end_time_mjd:
+    title: MJD End Time (d)
+    description: |
+      The date, in MJD, at the end of this exposure. Used in the archive catalog
+      for multi-mission matching.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_end_time_mjd, GuideWindow.exposure_end_time_mjd,
+                    SourceCatalog.exposure_end_time_mjd]
+  start_time_tdb:
+    title: TDB Start Time (d)
+    description: |
+      The date, in TDB (Barycentric Dynamical Time), at the beginning of this
+      exposure.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_start_time_tdb, GuideWindow.exposure_start_time_tdb,
+                    SourceCatalog.exposure_start_time_tdb]
+  mid_time_tdb:
+    title: TDB Mid Time (d)
+    description: |
+      The date, in TDB (Barycentric Dynamical Time), at the midpoint of this
+      exposure.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_mid_time_tdb, GuideWindow.exposure_mid_time_tdb,
+                    SourceCatalog.exposure_mid_time_tdb]
+  end_time_tdb:
+    title: TDB End Time (d)
+    description: |
+      The date, in TDB (Barycentric Dynamical Time), at the end of this
+      exposure.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_end_time_tdb, GuideWindow.exposure_end_time_tdb,
+                    SourceCatalog.exposure_end_time_tdb]
+  sca_number:
+    title: SCA Number
+    description: |
+      The number of the detector on the Sensor Chip Assembly used for this
+      exposure.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.exposure_sca_number, GuideWindow.exposure_sca_number,
+                    SourceCatalog.exposure_sca_number]
+  gain_factor:
+    title: Gain Factor
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_gain_factor, GuideWindow.exposure_gain_factor,
+                    SourceCatalog.exposure_gain_factor]
+  integration_time:
+    title: Effective Integration Time (s)
+    description:
+      The effective amount of time that the sensor was exposed to the sky.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_integration_time, GuideWindow.exposure_integration_time,
+                    SourceCatalog.exposure_integration_time]
+  elapsed_exposure_time:
+    title: Elapsed Exposure Time (s)
+    description: |
+      The amount of time elapsed between an exposure's first and last science
+      reads.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.elapsed_exposure_time, GuideWindow.elapsed_exposure_time,
+                    SourceCatalog.elapsed_exposure_time]
+  effective_exposure_time:
+    title: Effective Exposure Time (s)
+    description: |
+      The amount of time during which the detector actually collected photons
+      during an exposure.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.effective_exposure_time, GuideWindow.effective_exposure_time,
+                    SourceCatalog.effective_exposure_time]
+  duration:
+    title: Exposure Duration (s)
+    description: |
+      The amount of time dedicated to a exposure, including any overhead, time
+      spent on dropped frames, and so on.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.exposure_duration, GuideWindow.exposure_duration,
+                    SourceCatalog.exposure_duration]
+  level0_compressed:
+    title: Level 0 Compression
+    description: |
+      A flag indicating that the exposure has data that was decompressed by the
+      ground system.
+    type: boolean
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nchar(1)
+      destination: [WFIExposure.exposure_level0_compressed, GuideWindow.exposure_level0_compressed,
+                    SourceCatalog.exposure_level0_compressed]
+  truncated:
+    title: Truncated MA Table
+    description: |
+      A flag indicating whether the MA table was truncated.
+    type: boolean
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nchar(1)
+      destination: [WFIExposure.exposure_truncated,
+                    SourceCatalog.exposure_truncated]
+required: [type, start_time,
+           ngroups, nframes, data_problem,
+           frame_divisor, groupgap, frame_time, group_time, exposure_time,
+           ma_table_name, ma_table_number, read_pattern, id,
+          mid_time, end_time,
+          start_time_mjd, mid_time_mjd, end_time_mjd,
+          start_time_tdb, mid_time_tdb, end_time_tdb,
+          sca_number,
+          gain_factor, integration_time, elapsed_exposure_time,
+          effective_exposure_time, duration,
+          level0_compressed]
+propertyOrder: [type, start_time,
+           ngroups, nframes, data_problem,
+           frame_divisor, groupgap, frame_time, group_time, exposure_time,
+           ma_table_name, ma_table_number, read_pattern, id,
+          mid_time, end_time,
+          start_time_mjd, mid_time_mjd, end_time_mjd,
+          start_time_tdb, mid_time_tdb, end_time_tdb,
+          sca_number,
+          gain_factor, integration_time, elapsed_exposure_time,
+          effective_exposure_time, duration,
+          level0_compressed, truncated]
 flowStyle: block
 ...
```

### Comparing `rad-0.19.1/src/rad/resources/schemas/exposure_type-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/fps-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/fps-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/ground_common-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/ground_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/groundtest-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/groundtest-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/guidestar-1.0.0.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,241 +1,371 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/guidestar-1.0.0
 
 title: Guide Star Window Information
 
-allOf:
-  - $ref: asdf://stsci.edu/datamodels/roman/schemas/base_guidestar-1.0.0
-  - type: object
-    properties:
-      gs_id:
-        title: Guide Star Identifier from Guide Star Catalog
-        description: |
-          Identification of the guide star from the guide star catalog.
-        type: string
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: nvarchar(20)
-          destination: [WFIExposure.gs_id, GuideWindow.gs_id]
-      gs_catalog_version:
-        title: Version of the Guide Star Catalog
-        description: |
-          Version identifier of the guide star catalog used for the observation.
-        type: string
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: nvarchar(20)
-          destination: [WFIExposure.gs_catalog_version]
-      gs_ra:
-        title: Guide Star Right Ascension (deg)
-        description: |
-          Right ascension of the guide star from the guide star catalog in units of
-          degrees.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_ra, GuideWindow.gs_ra]
-      gs_dec:
-        title: Guide Star Declination (deg)
-        description: |
-          Declination of the guide star from the guide star catalog in units of
-          degrees.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_dec, GuideWindow.gs_dec]
-      gs_ura:
-        title: Guide Star Right Ascension Uncertainty (deg)
-        description: |
-          Uncertainty in the guide star right ascension from the guide star catalog
-          in units of degrees.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_ura, GuideWindow.gs_ura]
-      gs_udec:
-        title: Guide Star Declination Uncertainty (deg)
-        description: |
-          Uncertainty in the guide star declination from the guide star catalog in
-          units of degrees.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_udec, GuideWindow.gs_udec]
-      gs_mag:
-        title: Guide Star Instrumental Magnitude
-        description: |
-          Predicted instrumental magnitude of the guide star from the guide star
-          catalog.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_mag, GuideWindow.gs_mag]
-      gs_umag:
-        title: Guide Star Instrumental Magnitude Uncertainty
-        description: |
-          Uncertainty in the predicted instrumental magnitude of the guide star from
-          the guide star catalog.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_umag, GuideWindow.gs_umag]
-      gs_ctd_x:
-        title: Guide Star Centroid X Position (arcsec)
-        description: |
-          Centroid of the guide star position longa the X axis of the guider ideal
-          frame measured in units of arcseconds.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_ctd_x, GuideWindow.gs_ctd_x]
-      gs_ctd_y:
-        title: Guide Star Centroid Y Position (arcsec)
-        description: |
-          Centroid of the guide star position along the Y axis of the guider ideal
-          frame measured in units of arcseconds.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_ctd_y, GuideWindow.gs_ctd_y]
-      gs_ctd_ux:
-        title: Guide Star Centroid X Position Uncertainty (arcsec)
-        description: |
-          Uncertainty in the centroid of the guide star position along the X axis of
-          the guider ideal frame measured in units of arcseconds
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_ctd_ux, GuideWindow.gs_ctd_ux]
-      gs_ctd_uy:
-        title: Guide Star Centroid Y Position Uncertainty (arcsec)
-        description: |
-          Uncertainty in the centroid of the guide star position along the Y axis of
-          the guider ideal frame measured in units of arcseconds.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_ctd_uy, GuideWindow.gs_ctd_uy]
-      gs_epoch:
-        title: Guide Star Coordinates Epoch
-        description: |
-          Epoch of the celestial coordinates of the guide star.
-        type: string
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: nvarchar(10)
-          destination: [WFIExposure.gs_epoch, GuideWindow.gs_epoch]
-      gs_mura:
-        title: Proper Motion of the Guide Star Right Ascension (mas / yr)
-        description: |
-          Proper motion of the guide star in right ascension from the guide star
-          catalog measured in units of milli-arcseconds per year.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_mura, GuideWindow.gs_mura]
-      gs_mudec:
-        title: Proper Motion of the Guide Star Declination (mas / yr)
-        description: |
-          Proper motion of the guide star in declination from the guide star catalog
-          measured in units of milli-arcseconds per year.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_mudec, GuideWindow.gs_mudec]
-      gs_para:
-        title: Guide Star Annual Parallax
-        description: |
-          Annual parallax of the guide star from the guide star catalog.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_para, GuideWindow.gs_para]
-      gs_pattern_error:
-        title: Guide Star Centroid RMS
-        description: |
-          RMS of the guide star position in the tracking guide windows from the Fine
-          Attitude Correction Estimate (FACE) information. The FACE information
-          determines the error across the guiding pattern using all centroid
-          measurements.
-        type: number
-        sdf:
-          special_processing: VALUE_REQUIRED
-          source:
-            origin: TBD
-        archive_catalog:
-          datatype: float
-          destination: [WFIExposure.gs_pattern_error, GuideWindow.gs_pattern_error]
-    propertyOrder: [gs_id, gs_catalog_version, gs_ra, gs_dec,
-                  gs_ura, gs_udec, gs_mag, gs_umag,
-                  gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
-                  gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error]
-    required: [gs_id, gs_catalog_version, gs_ra, gs_dec,
+type: object
+properties:
+  gw_id:
+    title: Guide Star Window Identifier
+    description: |
+      Identification of the Guide Star Window.
+    type: string
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(20)
+      destination: [WFIExposure.gw_id, GuideWindow.gw_id, WFICommon.gw_id]
+  gw_fgs_mode:
+    $ref: guidewindow_modes-1.0.0
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(18)
+      destination: [WFIExposure.gw_fgs_mode, GuideWindow.gw_fgs_mode, WFICommon.gw_fgs_mode]
+  data_start:
+    title: Guide Data Start Time (MJD)
+    description: |
+      Start time of the guide window data taken for this exposure as a Modified
+      Julian Date.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.data_start, GuideWindow.data_start, WFICommon.data_start]
+  data_end:
+    title: Guide Data End Time (MJD)
+    description: |
+      End time of the guide window data taken for this exposure as a Modified
+      Julian Date.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.data_end, GuideWindow.data_end, WFICommon.data_end]
+  gw_window_xstart:
+    title: Guide Window X Start Position (pixels)
+    description: |
+      Minimum X position in the science coordinate frame of all tracking guide
+      windows in this exposure measured in pixels.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: Science Data Formatting
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.gw_window_xstart, WFICommon.gw_window_xstart]
+  gw_window_ystart:
+    title: Guide Window Y Start Position (pixels)
+    description: |
+      Minimum Y position in the science coordinate frame of all tracking guide
+      windows in this exposure measured in pixels.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: Science Data Formatting
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.gw_window_ystart, WFICommon.gw_window_ystart]
+  gw_window_xstop:
+    title: Guide Window X Stop Position (pixels)
+    description: |
+      Maximum X position in the science coordinate frame of all tracking guide
+      windows in this exposure measured in pixels.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: Science Data Formatting
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.gw_window_xstop, WFICommon.gw_window_xstop]
+  gw_window_ystop:
+    title: Guide Window Y Stop Position (pixels)
+    description: |
+      Maximum Y position in the science coordinate frame of all tracking guide
+      windows in this exposure measured in pixels
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: Science Data Formatting
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.gw_window_ystop, WFICommon.gw_window_ystop]
+  gw_window_xsize:
+    title: Guide Window Size in the X Direction (pixels)
+    description: |
+      Size of a single tracking guide window in this exposure measured along the
+      X axis in units of pixels.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: Science Data Formatting
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.gw_window_xsize, WFICommon.gw_window_xsize]
+  gw_window_ysize:
+    title: Guide Window Size in the Y Direction (pixels)
+    description: |
+      Size of a single tracking guide window in this exposure measured along the
+      Y axis in units of pixels.
+    type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: Science Data Formatting
+    archive_catalog:
+      datatype: int
+      destination: [WFIExposure.gw_window_ysize, WFICommon.gw_window_ysize]
+  gs_id:
+    title: Guide Star Identifier from Guide Star Catalog
+    description: |
+      Identification of the guide star from the guide star catalog.
+    type: string
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(20)
+      destination: [WFIExposure.gs_id, GuideWindow.gs_id]
+  gs_catalog_version:
+    title: Version of the Guide Star Catalog
+    description: |
+      Version identifier of the guide star catalog used for the observation.
+    type: string
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(20)
+      destination: [WFIExposure.gs_catalog_version]
+  gs_ra:
+    title: Guide Star Right Ascension (deg)
+    description: |
+      Right ascension of the guide star from the guide star catalog in units of
+      degrees.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_ra, GuideWindow.gs_ra]
+  gs_dec:
+    title: Guide Star Declination (deg)
+    description: |
+      Declination of the guide star from the guide star catalog in units of
+      degrees.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_dec, GuideWindow.gs_dec]
+  gs_ura:
+    title: Guide Star Right Ascension Uncertainty (deg)
+    description: |
+      Uncertainty in the guide star right ascension from the guide star catalog
+      in units of degrees.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_ura, GuideWindow.gs_ura]
+  gs_udec:
+    title: Guide Star Declination Uncertainty (deg)
+    description: |
+      Uncertainty in the guide star declination from the guide star catalog in
+      units of degrees.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_udec, GuideWindow.gs_udec]
+  gs_mag:
+    title: Guide Star Instrumental Magnitude
+    description: |
+      Predicted instrumental magnitude of the guide star from the guide star
+      catalog.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_mag, GuideWindow.gs_mag]
+  gs_umag:
+    title: Guide Star Instrumental Magnitude Uncertainty
+    description: |
+      Uncertainty in the predicted instrumental magnitude of the guide star from
+      the guide star catalog.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_umag, GuideWindow.gs_umag]
+  gs_ctd_x:
+    title: Guide Star Centroid X Position (arcsec)
+    description: |
+      Centroid of the guide star position longa the X axis of the guider ideal
+      frame measured in units of arcseconds.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_ctd_x, GuideWindow.gs_ctd_x]
+  gs_ctd_y:
+    title: Guide Star Centroid Y Position (arcsec)
+    description: |
+      Centroid of the guide star position along the Y axis of the guider ideal
+      frame measured in units of arcseconds.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_ctd_y, GuideWindow.gs_ctd_y]
+  gs_ctd_ux:
+    title: Guide Star Centroid X Position Uncertainty (arcsec)
+    description: |
+      Uncertainty in the centroid of the guide star position along the X axis of
+      the guider ideal frame measured in units of arcseconds
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_ctd_ux, GuideWindow.gs_ctd_ux]
+  gs_ctd_uy:
+    title: Guide Star Centroid Y Position Uncertainty (arcsec)
+    description: |
+      Uncertainty in the centroid of the guide star position along the Y axis of
+      the guider ideal frame measured in units of arcseconds.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_ctd_uy, GuideWindow.gs_ctd_uy]
+  gs_epoch:
+    title: Guide Star Coordinates Epoch
+    description: |
+      Epoch of the celestial coordinates of the guide star.
+    type: string
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(10)
+      destination: [WFIExposure.gs_epoch, GuideWindow.gs_epoch]
+  gs_mura:
+    title: Proper Motion of the Guide Star Right Ascension (mas / yr)
+    description: |
+      Proper motion of the guide star in right ascension from the guide star
+      catalog measured in units of milli-arcseconds per year.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_mura, GuideWindow.gs_mura]
+  gs_mudec:
+    title: Proper Motion of the Guide Star Declination (mas / yr)
+    description: |
+      Proper motion of the guide star in declination from the guide star catalog
+      measured in units of milli-arcseconds per year.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_mudec, GuideWindow.gs_mudec]
+  gs_para:
+    title: Guide Star Annual Parallax
+    description: |
+      Annual parallax of the guide star from the guide star catalog.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_para, GuideWindow.gs_para]
+  gs_pattern_error:
+    title: Guide Star Centroid RMS
+    description: |
+      RMS of the guide star position in the tracking guide windows from the Fine
+      Attitude Correction Estimate (FACE) information. The FACE information
+      determines the error across the guiding pattern using all centroid
+      measurements.
+    type: number
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: float
+      destination: [WFIExposure.gs_pattern_error, GuideWindow.gs_pattern_error]
+propertyOrder: [gw_id, gw_fgs_mode,
+           data_start, data_end, gw_window_xstart,
+           gw_window_ystart, gw_window_xstop, gw_window_ystop, gw_window_xsize,
+           gw_window_ysize,
+           gs_id, gs_catalog_version, gs_ra, gs_dec,
               gs_ura, gs_udec, gs_mag, gs_umag,
               gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
               gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error]
-
+required: [gw_id, gw_fgs_mode,
+           data_start, data_end, gw_window_xstart,
+           gw_window_ystart, gw_window_xstop, gw_window_ystop, gw_window_xsize,
+           gw_window_ysize,
+           gs_id, gs_catalog_version, gs_ra, gs_dec,
+          gs_ura, gs_udec, gs_mag, gs_umag,
+          gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
+          gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error]
 flowStyle: block
 ...
```

### Comparing `rad-0.19.1/src/rad/resources/schemas/guidewindow-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/msos_stack-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/msos_stack-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/observation-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/photometry-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/pointing-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/pointing-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/program-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/program-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/ref_file-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/ref_file-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/resample-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/resample-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/segmentation_map-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/segmentation_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/source_catalog-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/source_catalog-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/target-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/target-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/tvac-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/tvac-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/visit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/wcsinfo-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/wfi_image-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml` & `rad-0.19.2/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/src/rad.egg-info/PKG-INFO` & `rad-0.19.2/src/rad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.1
+Version: 0.19.2
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.19.1/src/rad.egg-info/SOURCES.txt` & `rad-0.19.2/src/rad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/tests/test_integration.py` & `rad-0.19.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/tests/test_manifest.py` & `rad-0.19.2/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/tests/test_schemas.py` & `rad-0.19.2/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.1/tox.ini` & `rad-0.19.2/tox.ini`

 * *Files identical despite different names*

