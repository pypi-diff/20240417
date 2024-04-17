# Comparing `tmp/fractal_tasks_core-1.0.0a1.tar.gz` & `tmp/fractal_tasks_core-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_tasks_core-1.0.0a1.tar", max compression
+gzip compressed data, was "fractal_tasks_core-1.0.0a2.tar", max compression
```

## Comparing `fractal_tasks_core-1.0.0a1.tar` & `fractal_tasks_core-1.0.0a2.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0     1584 2024-04-15 07:06:08.958493 fractal_tasks_core-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     3743 2024-04-15 07:06:08.958493 fractal_tasks_core-1.0.0a1/README.md
--rw-r--r--   0        0        0       32 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/.gitignore
--rw-r--r--   0        0        0    64078 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/__FRACTAL_MANIFEST__.json
--rw-r--r--   0        0        0      200 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/__init__.py
--rw-r--r--   0        0        0       87 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/cellvoyager/__init__.py
--rw-r--r--   0        0        0     4552 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/cellvoyager/filenames.py
--rw-r--r--   0        0        0    12515 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/cellvoyager/metadata.py
--rw-r--r--   0        0        0    16707 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/channels.py
--rw-r--r--   0        0        0      108 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/README.md
--rw-r--r--   0        0        0       98 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/__init__.py
--rw-r--r--   0        0        0     4607 2024-04-15 07:06:08.962493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/check_manifest.py
--rw-r--r--   0        0        0     5368 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/create_manifest.py
--rw-r--r--   0        0        0     8166 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_args_schemas.py
--rw-r--r--   0        0        0     6406 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_descriptions.py
--rw-r--r--   0        0        0     3260 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_signature_constraints.py
--rw-r--r--   0        0        0     2827 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_task_docs.py
--rw-r--r--   0        0        0     2273 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_titles.py
--rw-r--r--   0        0        0     3610 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/task_list.py
--rw-r--r--   0        0        0     2660 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/task_models.py
--rw-r--r--   0        0        0     5189 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/labels.py
--rw-r--r--   0        0        0     9005 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/masked_loading.py
--rw-r--r--   0        0        0      508 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/ngff/__init__.py
--rw-r--r--   0        0        0    13113 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/ngff/specs.py
--rw-r--r--   0        0        0     3974 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/ngff/zarr_utils.py
--rw-r--r--   0        0        0     3788 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/pyramids.py
--rw-r--r--   0        0        0      185 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/__init__.py
--rw-r--r--   0        0        0     4501 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/_overlaps_common.py
--rw-r--r--   0        0        0     1327 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/load_region.py
--rw-r--r--   0        0        0    18609 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/v1.py
--rw-r--r--   0        0        0     4910 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/v1_checks.py
--rw-r--r--   0        0        0    13273 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/v1_overlaps.py
--rw-r--r--   0        0        0     3394 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tables/__init__.py
--rw-r--r--   0        0        0    11579 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tables/v1.py
--rw-r--r--   0        0        0       72 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/__init__.py
--rw-r--r--   0        0        0     8392 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/_registration_utils.py
--rw-r--r--   0        0        0     2407 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/_utils.py
--rw-r--r--   0        0        0    13512 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/apply_registration_to_image.py
--rw-r--r--   0        0        0     9371 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/calculate_registration_image_based.py
--rw-r--r--   0        0        0    27519 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellpose_segmentation.py
--rw-r--r--   0        0        0     8458 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellpose_transforms.py
--rw-r--r--   0        0        0     7728 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
--rw-r--r--   0        0        0    18358 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
--rw-r--r--   0        0        0    21030 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
--rw-r--r--   0        0        0     2567 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/compress_tif.py
--rw-r--r--   0        0        0    11207 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
--rw-r--r--   0        0        0     6384 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/find_registration_consensus.py
--rw-r--r--   0        0        0    10249 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/illumination_correction.py
--rw-r--r--   0        0        0     3603 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
--rw-r--r--   0        0        0    11691 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/import_ome_zarr.py
--rw-r--r--   0        0        0     3039 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
--rw-r--r--   0        0        0     4903 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/io_models.py
--rw-r--r--   0        0        0     6188 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/maximum_intensity_projection.py
--rw-r--r--   0        0        0    24797 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/napari_workflows_wrapper.py
--rw-r--r--   0        0        0     7136 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/upscale_array.py
--rw-r--r--   0        0        0     6101 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/utils.py
--rw-r--r--   0        0        0     3890 2024-04-15 07:06:08.966493 fractal_tasks_core-1.0.0a1/fractal_tasks_core/zarr_utils.py
--rw-r--r--   0        0        0     3431 2024-04-15 07:06:08.970493 fractal_tasks_core-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1584 2024-04-17 14:03:40.647913 fractal_tasks_core-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0     3743 2024-04-17 14:03:40.647913 fractal_tasks_core-1.0.0a2/README.md
+-rw-r--r--   0        0        0       32 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/.gitignore
+-rw-r--r--   0        0        0    64035 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/__FRACTAL_MANIFEST__.json
+-rw-r--r--   0        0        0      200 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/__init__.py
+-rw-r--r--   0        0        0     4552 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/filenames.py
+-rw-r--r--   0        0        0    12515 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/metadata.py
+-rw-r--r--   0        0        0    16707 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/channels.py
+-rw-r--r--   0        0        0      108 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/README.md
+-rw-r--r--   0        0        0       98 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/__init__.py
+-rw-r--r--   0        0        0     4607 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/check_manifest.py
+-rw-r--r--   0        0        0     5368 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/create_manifest.py
+-rw-r--r--   0        0        0     8166 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_args_schemas.py
+-rw-r--r--   0        0        0     6406 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_descriptions.py
+-rw-r--r--   0        0        0     3260 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_signature_constraints.py
+-rw-r--r--   0        0        0     2827 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_task_docs.py
+-rw-r--r--   0        0        0     2273 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_titles.py
+-rw-r--r--   0        0        0     3624 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/task_list.py
+-rw-r--r--   0        0        0     2660 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/task_models.py
+-rw-r--r--   0        0        0     5189 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/labels.py
+-rw-r--r--   0        0        0     9005 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/masked_loading.py
+-rw-r--r--   0        0        0      508 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/__init__.py
+-rw-r--r--   0        0        0    13113 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/specs.py
+-rw-r--r--   0        0        0     3974 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/zarr_utils.py
+-rw-r--r--   0        0        0     3788 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/pyramids.py
+-rw-r--r--   0        0        0      185 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/__init__.py
+-rw-r--r--   0        0        0     4501 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/_overlaps_common.py
+-rw-r--r--   0        0        0     1327 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/load_region.py
+-rw-r--r--   0        0        0    18609 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1.py
+-rw-r--r--   0        0        0     4910 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1_checks.py
+-rw-r--r--   0        0        0    13273 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1_overlaps.py
+-rw-r--r--   0        0        0     3394 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tables/__init__.py
+-rw-r--r--   0        0        0    11579 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tables/v1.py
+-rw-r--r--   0        0        0       72 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/__init__.py
+-rw-r--r--   0        0        0     8392 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/_registration_utils.py
+-rw-r--r--   0        0        0     2407 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/_utils.py
+-rw-r--r--   0        0        0    13827 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/apply_registration_to_image.py
+-rw-r--r--   0        0        0     9363 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/calculate_registration_image_based.py
+-rw-r--r--   0        0        0    27516 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellpose_segmentation.py
+-rw-r--r--   0        0        0     8458 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellpose_transforms.py
+-rw-r--r--   0        0        0     7779 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
+-rw-r--r--   0        0        0    18431 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
+-rw-r--r--   0        0        0    21103 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
+-rw-r--r--   0        0        0    11258 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
+-rw-r--r--   0        0        0     6403 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/find_registration_consensus.py
+-rw-r--r--   0        0        0    10319 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/illumination_correction.py
+-rw-r--r--   0        0        0     3596 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
+-rw-r--r--   0        0        0    11764 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/import_ome_zarr.py
+-rw-r--r--   0        0        0     2998 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
+-rw-r--r--   0        0        0     4903 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/io_models.py
+-rw-r--r--   0        0        0     6239 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/maximum_intensity_projection.py
+-rw-r--r--   0        0        0    24816 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/napari_workflows_wrapper.py
+-rw-r--r--   0        0        0     7136 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/upscale_array.py
+-rw-r--r--   0        0        0     6101 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/utils.py
+-rw-r--r--   0        0        0     3890 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/zarr_utils.py
+-rw-r--r--   0        0        0     3387 2024-04-17 14:03:40.659913 fractal_tasks_core-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.0a2/PKG-INFO
```

### Comparing `fractal_tasks_core-1.0.0a1/LICENSE` & `fractal_tasks_core-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/README.md` & `fractal_tasks_core-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/__FRACTAL_MANIFEST__.json` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/__FRACTAL_MANIFEST__.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981127703631365%*

 * *Differences: {"'task_list'": "{3: {'args_schema_parallel': {'properties': {'background': {'default': 0}, "*

 * *                "'illumination_profiles': OrderedDict([('title', 'Illumination Profiles'), "*

 * *                "('type', 'object'), ('additionalProperties', OrderedDict([('type', 'string')])), "*

 * *                "('description', 'Dictionary where keys match the `wavelength_id` attributes of "*

 * *                'existing channels (e.g. `A01_C01` ) and values are the filenames of the '*

 * *                "corresponding illum […]*

```diff
@@ -620,25 +620,25 @@
             }
         },
         {
             "args_schema_parallel": {
                 "additionalProperties": false,
                 "properties": {
                     "background": {
-                        "default": 110,
+                        "default": 0,
                         "description": "Background value that is subtracted from the image before the illumination correction is applied. Set it to `0` if you don't want any background subtraction.",
                         "title": "Background",
                         "type": "integer"
                     },
-                    "dict_corr": {
+                    "illumination_profiles": {
                         "additionalProperties": {
                             "type": "string"
                         },
                         "description": "Dictionary where keys match the `wavelength_id` attributes of existing channels (e.g. `A01_C01` ) and values are the filenames of the corresponding illumination profiles.",
-                        "title": "Dict Corr",
+                        "title": "Illumination Profiles",
                         "type": "object"
                     },
                     "illumination_profiles_folder": {
                         "description": "Path of folder of illumination profiles.",
                         "title": "Illumination Profiles Folder",
                         "type": "string"
                     },
@@ -665,15 +665,15 @@
                         "title": "Zarr Url",
                         "type": "string"
                     }
                 },
                 "required": [
                     "zarr_url",
                     "illumination_profiles_folder",
-                    "dict_corr"
+                    "illumination_profiles"
                 ],
                 "title": "IlluminationCorrection",
                 "type": "object"
             },
             "docs_info": "## illumination_correction\nApplies illumination correction to the images in the OME-Zarr.\n\nAssumes that the illumination correction profiles were generated before\nseparately and that the same background subtraction was used during\ncalculation of the illumination correction (otherwise, it will not work\nwell & the correction may only be partial).\n",
             "docs_link": "https://fractal-analytics-platform.github.io/fractal-tasks-core",
             "executable_parallel": "tasks/illumination_correction.py",
@@ -1062,15 +1062,15 @@
         },
         {
             "args_schema_non_parallel": {
                 "additionalProperties": false,
                 "properties": {
                     "reference_cycle": {
                         "default": 0,
-                        "description": "Which cycle to register against. Defaults to 0, which is the first OME-Zarr image in the well, usually the first cycle that was provided",
+                        "description": "Which cycle to register against. Uses the OME-NGFF HCS well metadata acquisition keys to find the reference cycle.",
                         "title": "Reference Cycle",
                         "type": "integer"
                     },
                     "zarr_dir": {
                         "description": "path of the directory where the new OME-Zarrs will be created. Not used by this task. (standard argument for Fractal tasks, managed by Fractal server).",
                         "title": "Zarr Dir",
                         "type": "string"
@@ -1163,18 +1163,18 @@
                     "overwrite_input": {
                         "default": true,
                         "description": "Whether the old image data should be replaced with the newly registered image data. Currently only implemented for `overwrite_input=True`.",
                         "title": "Overwrite Input",
                         "type": "boolean"
                     },
                     "reference_cycle": {
-                        "default": "0",
-                        "description": "Which cycle to register against. Defaults to 0, which is the first OME-Zarr image in the well, usually the first cycle that was provided",
+                        "default": 0,
+                        "description": "Which cycle to register against. Uses the OME-NGFF HCS well metadata acquisition keys to find the reference cycle.",
                         "title": "Reference Cycle",
-                        "type": "string"
+                        "type": "integer"
                     },
                     "registered_roi_table": {
                         "description": "Name of the ROI table which has been registered and will be applied to mask and shift the images. Examples: `registered_FOV_ROI_table` => loop over the field of views, `registered_well_ROI_table` => process the whole well as one image.",
                         "title": "Registered Roi Table",
                         "type": "string"
                     },
                     "zarr_url": {
@@ -1186,15 +1186,15 @@
                 "required": [
                     "zarr_url",
                     "registered_roi_table"
                 ],
                 "title": "ApplyRegistrationToImage",
                 "type": "object"
             },
-            "docs_info": "## apply_registration_to_image\nApply registration to images by using a registered ROI table\n\nThis task consists of 4 parts:\n\n1. Mask all regions in images that are not available in the\nregistered ROI table and store each cycle aligned to the\nreference_cycle (by looping over ROIs).\n2. Do the same for all label images.\n3. Copy all tables from the non-aligned image to the aligned image\n(currently only works well if the only tables are well & FOV ROI tables\n(registered and original). Not implemented for measurement tables and\nother ROI tables).\n4. Clean up: Delete the old, non-aligned image and rename the new,\naligned image to take over its place.\n\nParallelization level: image\n",
+            "docs_info": "## apply_registration_to_image\nApply registration to images by using a registered ROI table\n\nThis task consists of 4 parts:\n\n1. Mask all regions in images that are not available in the\nregistered ROI table and store each cycle aligned to the\nreference_cycle (by looping over ROIs).\n2. Do the same for all label images.\n3. Copy all tables from the non-aligned image to the aligned image\n(currently only works well if the only tables are well & FOV ROI tables\n(registered and original). Not implemented for measurement tables and\nother ROI tables).\n4. Clean up: Delete the old, non-aligned image and rename the new,\naligned image to take over its place.\n",
             "docs_link": "https://fractal-analytics-platform.github.io/fractal-tasks-core",
             "executable_parallel": "tasks/apply_registration_to_image.py",
             "input_types": {
                 "registered": false
             },
             "meta_parallel": {
                 "cpus_per_task": 1,
@@ -1428,11 +1428,11 @@
             "docs_info": "## napari_workflows_wrapper\nRun a napari-workflow on the ROIs of a single OME-NGFF image.\n\nThis task takes images and labels and runs a napari-workflow on them that\ncan produce a label and tables as output.\n\nExamples of allowed entries for `input_specs` and `output_specs`:\n\n```\ninput_specs = {\n    \"in_1\": {\"type\": \"image\", \"channel\": {\"wavelength_id\": \"A01_C02\"}},\n    \"in_2\": {\"type\": \"image\", \"channel\": {\"label\": \"DAPI\"}},\n    \"in_3\": {\"type\": \"label\", \"label_name\": \"label_DAPI\"},\n}\n\noutput_specs = {\n    \"out_1\": {\"type\": \"label\", \"label_name\": \"label_DAPI_new\"},\n    \"out_2\": {\"type\": \"dataframe\", \"table_name\": \"measurements\"},\n}\n```\n",
             "docs_link": "https://fractal-analytics-platform.github.io/fractal-tasks-core",
             "executable_parallel": "tasks/napari_workflows_wrapper.py",
             "meta_parallel": {
                 "cpus_per_task": 8,
                 "mem": 32000
             },
-            "name": "Napari workflows wrapper"
+            "name": "Napari Workflows Wrapper"
         }
     ]
 }
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/cellvoyager/filenames.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/filenames.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/cellvoyager/metadata.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/metadata.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/channels.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/channels.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/check_manifest.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/check_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/create_manifest.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/create_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_args_schemas.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_args_schemas.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_descriptions.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_descriptions.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_signature_constraints.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_signature_constraints.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_task_docs.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_task_docs.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/lib_titles.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_titles.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/task_list.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/task_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         name="Illumination Correction",
         input_types=dict(illumination_corrected=False),
         executable="tasks/illumination_correction.py",
         output_types=dict(illumination_corrected=True),
         meta={"cpus_per_task": 1, "mem": 4000},
     ),
     # CompoundTask(
-    #     name="illumination_correction_compound",
+    #     name="Illumination Correction (channel parallelized)",
     #     input_types=dict(illumination_correction=False),
     #     executable_init="illumination_correction_init.py",
     #     executable="illumination_correction_compute.py",
     #     output_types=dict(illumination_correction=True),
     # ),
     ParallelTask(
         name="Cellpose Segmentation",
@@ -80,15 +80,15 @@
         meta={"cpus_per_task": 1, "mem": 4000},
     ),
     NonParallelTask(
         name="Import OME-Zarr",
         executable="tasks/import_ome_zarr.py",
     ),
     ParallelTask(
-        name="Napari workflows wrapper",
+        name="Napari Workflows Wrapper",
         executable="tasks/napari_workflows_wrapper.py",
         meta={
             "cpus_per_task": 8,
             "mem": 32000,
         },
     ),
 ]
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/dev/task_models.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/task_models.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/labels.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/labels.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/masked_loading.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/masked_loading.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/ngff/specs.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/specs.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/ngff/zarr_utils.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/pyramids.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/pyramids.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/_overlaps_common.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/_overlaps_common.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/load_region.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/load_region.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/v1.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/v1_checks.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1_checks.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/roi/v1_overlaps.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1_overlaps.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tables/__init__.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tables/v1.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tables/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/_registration_utils.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/_registration_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/_utils.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/apply_registration_to_image.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/apply_registration_to_image.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,37 +20,41 @@
 import anndata as ad
 import dask.array as da
 import numpy as np
 import zarr
 from pydantic.decorator import validate_arguments
 
 from fractal_tasks_core.ngff import load_NgffImageMeta
+from fractal_tasks_core.ngff.zarr_utils import load_NgffWellMeta
 from fractal_tasks_core.pyramids import build_pyramid
 from fractal_tasks_core.roi import (
     convert_indices_to_regions,
 )
 from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
 from fractal_tasks_core.roi import is_standard_roi_table
 from fractal_tasks_core.roi import load_region
 from fractal_tasks_core.tables import write_table
+from fractal_tasks_core.tasks._registration_utils import (
+    _split_well_path_image_path,
+)
 from fractal_tasks_core.utils import _get_table_path_dict
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def apply_registration_to_image(
     *,
-    # Fractal argument
+    # Fractal parameters
     zarr_url: str,
-    # Task-specific arguments
+    # Core parameters
     registered_roi_table: str,
-    reference_cycle: str = "0",
+    reference_cycle: int = 0,
     overwrite_input: bool = True,
 ):
     """
     Apply registration to images by using a registered ROI table
 
     This task consists of 4 parts:
 
@@ -61,45 +65,46 @@
     3. Copy all tables from the non-aligned image to the aligned image
     (currently only works well if the only tables are well & FOV ROI tables
     (registered and original). Not implemented for measurement tables and
     other ROI tables).
     4. Clean up: Delete the old, non-aligned image and rename the new,
     aligned image to take over its place.
 
-    Parallelization level: image
-
     Args:
         zarr_url: Path or url to the individual OME-Zarr image to be processed.
             (standard argument for Fractal tasks, managed by Fractal server).
         registered_roi_table: Name of the ROI table which has been registered
             and will be applied to mask and shift the images.
             Examples: `registered_FOV_ROI_table` => loop over the field of
             views, `registered_well_ROI_table` => process the whole well as
             one image.
-        reference_cycle: Which cycle to register against. Defaults to 0,
-            which is the first OME-Zarr image in the well, usually the first
-            cycle that was provided
+        reference_cycle: Which cycle to register against. Uses the OME-NGFF
+            HCS well metadata acquisition keys to find the reference cycle.
         overwrite_input: Whether the old image data should be replaced with the
             newly registered image data. Currently only implemented for
             `overwrite_input=True`.
 
     """
     logger.info(zarr_url)
     logger.info(
         f"Running `apply_registration_to_image` on {zarr_url=}, "
         f"{registered_roi_table=} and {reference_cycle=}. "
         f"Using {overwrite_input=}"
     )
 
-    new_zarr_url = "/".join(
-        zarr_url.split("/")[:-1] + [zarr_url.split("/")[-1] + "_registered"]
-    )
-    # TODO: Make this more robust by actually checking for acquisition
-    # metadata
-    reference_zarr_url = "/".join(zarr_url.split("/")[:-1] + [reference_cycle])
+    well_url, _ = _split_well_path_image_path(zarr_url)
+    new_zarr_url = f"{well_url}/{zarr_url.split('/')[-1]}_registered"
+    # Get the zarr_url for the reference cycle
+    acq_dict = load_NgffWellMeta(well_url).get_acquisition_paths()
+    if reference_cycle not in acq_dict:
+        raise ValueError(
+            f"{reference_cycle=} was not one of the available acquisitions in "
+            f"{acq_dict=} for well {well_url}"
+        )
+    reference_zarr_url = f"{well_url}/{acq_dict[reference_cycle]}"
 
     ROI_table_ref = ad.read_zarr(
         f"{reference_zarr_url}/tables/{registered_roi_table}"
     )
     ROI_table_cycle = ad.read_zarr(f"{zarr_url}/tables/{registered_roi_table}")
 
     ngff_image_meta = load_NgffImageMeta(zarr_url)
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/calculate_registration_image_based.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/calculate_registration_image_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 @validate_arguments
 def calculate_registration_image_based(
     *,
     # Fractal arguments
     zarr_url: str,
     init_args: InitArgsRegistration,
-    # Task-specific arguments
+    # Core parameters
     wavelength_id: str,
     roi_table: str = "FOV_ROI_table",
     level: int = 2,
 ) -> None:
     """
     Calculate registration based on images
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellpose_segmentation.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellpose_segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,30 +190,29 @@
 
     return mask.astype(label_dtype)
 
 
 @validate_arguments
 def cellpose_segmentation(
     *,
-    # Fractal argument
+    # Fractal parameters
     zarr_url: str,
-    # Task-specific arguments
+    # Core parameters
     level: int,
     channel: ChannelInputModel,
     channel2: Optional[ChannelInputModel] = None,
     input_ROI_table: str = "FOV_ROI_table",
     output_ROI_table: Optional[str] = None,
     output_label_name: Optional[str] = None,
-    use_masks: bool = True,
-    relabeling: bool = True,
     # Cellpose-related arguments
     diameter_level0: float = 30.0,
     # https://github.com/fractal-analytics-platform/fractal-tasks-core/issues/401 # noqa E501
     model_type: Literal[tuple(models.MODEL_NAMES)] = "cyto2",
     pretrained_model: Optional[str] = None,
+    # Advanced parameters
     cellprob_threshold: float = 0.0,
     flow_threshold: float = 0.4,
     normalize: CellposeCustomNormalizer = CellposeCustomNormalizer(),
     anisotropy: Optional[float] = None,
     min_size: int = 15,
     augment: bool = False,
     net_avg: bool = False,
@@ -221,15 +220,16 @@
     batch_size: int = 8,
     invert: bool = False,
     tile: bool = True,
     tile_overlap: float = 0.1,
     resample: bool = True,
     interp: bool = True,
     stitch_threshold: float = 0.0,
-    # Overwrite option
+    use_masks: bool = True,
+    relabeling: bool = True,
     overwrite: bool = True,
 ) -> None:
     """
     Run cellpose segmentation on the ROIs of a single OME-Zarr image.
 
     Args:
         zarr_url: Path or url to the individual OME-Zarr image to be processed.
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellpose_transforms.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellpose_transforms.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,18 @@
     z_index = int(filename_metadata["Z"])
     return [site, z_index]
 
 
 @validate_arguments
 def cellvoyager_to_ome_zarr_compute(
     *,
+    # Fractal parameters
     zarr_url: str,
     init_args: InitArgsCellVoyager,
+    # Advanced parameters
     overwrite: bool = False,
 ):
     """
     Convert Yokogawa output (png, tif) to zarr file.
 
     This task is typically run after Create OME-Zarr or
     Create OME-Zarr Multiplexing and populates the empty OME-Zarr files that
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,18 +46,21 @@
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def cellvoyager_to_ome_zarr_init(
     *,
+    # Fractal parameters
     zarr_urls: list[str],
     zarr_dir: str,
+    # Core parameters
     image_dirs: list[str],
     allowed_channels: list[OmeroChannel],
+    # Advanced parameters
     image_glob_patterns: Optional[list[str]] = None,
     num_levels: int = 5,
     coarsening_xy: int = 2,
     image_extension: str = "tif",
     metadata_table_file: Optional[str] = None,
     overwrite: bool = False,
 ) -> dict[str, Any]:
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,20 @@
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def cellvoyager_to_ome_zarr_init_multiplex(
     *,
+    # Fractal parameters
     zarr_urls: list[str],
     zarr_dir: str,
+    # Core parameters
     acquisitions: dict[str, MultiplexingAcquisition],
+    # Advanced parameters
     image_glob_patterns: Optional[list[str]] = None,
     num_levels: int = 5,
     coarsening_xy: int = 2,
     image_extension: str = "tif",
     metadata_table_files: Optional[dict[str, str]] = None,
     overwrite: bool = False,
 ) -> dict[str, Any]:
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,18 @@
 
     return plate_metadata_dicts, new_well_image_attrs, well_image_attrs
 
 
 @validate_arguments
 def copy_ome_zarr_hcs_plate(
     *,
+    # Fractal parameters
     zarr_urls: list[str],
     zarr_dir: str,
+    # Advanced parameters
     suffix: str = "mip",
     overwrite: bool = False,
 ) -> dict[str, Any]:
     """
     Duplicate the OME-Zarr HCS structure for a set of zarr_urls.
 
     This task only processes the zarr images in the zarr_urls, not all the
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/find_registration_consensus.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/find_registration_consensus.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,20 @@
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def find_registration_consensus(
     *,
-    # Fractal arguments
+    # Fractal parameters
     zarr_url: str,
     init_args: InitArgsRegistrationConsensus,
-    # Task-specific arguments
+    # Core parameters
     roi_table: str = "FOV_ROI_table",
+    # Advanced parameters
     new_roi_table: Optional[str] = None,
 ):
     """
     Applies pre-calculated registration to ROI tables.
 
     Apply pre-calculated registration such that resulting ROIs contain
     the consensus align region between all cycles.
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/illumination_correction.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/illumination_correction.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,22 +89,23 @@
     # Cast back to original dtype and return
     return new_img_stack.astype(dtype)
 
 
 @validate_arguments
 def illumination_correction(
     *,
-    # Fractal argument
+    # Fractal parameters
     zarr_url: str,
-    # Task-specific arguments
+    # Core parameters
     illumination_profiles_folder: str,
-    dict_corr: dict[str, str],
-    background: int = 110,
+    illumination_profiles: dict[str, str],
+    background: int = 0,
     input_ROI_table: str = "FOV_ROI_table",
     overwrite_input: bool = True,
+    # Advanced parameters
     suffix: str = "_illum_corr",
 ) -> dict[str, Any]:
 
     """
     Applies illumination correction to the images in the OME-Zarr.
 
     Assumes that the illumination correction profiles were generated before
@@ -112,17 +113,17 @@
     calculation of the illumination correction (otherwise, it will not work
     well & the correction may only be partial).
 
     Args:
         zarr_url: Path or url to the individual OME-Zarr image to be processed.
             (standard argument for Fractal tasks, managed by Fractal server).
         illumination_profiles_folder: Path of folder of illumination profiles.
-        dict_corr: Dictionary where keys match the `wavelength_id` attributes
-            of existing channels (e.g.  `A01_C01` ) and values are the
-            filenames of the corresponding illumination profiles.
+        illumination_profiles: Dictionary where keys match the `wavelength_id`
+            attributes of existing channels (e.g.  `A01_C01` ) and values are
+            the filenames of the corresponding illumination profiles.
         background: Background value that is subtracted from the image before
             the illumination correction is applied. Set it to `0` if you don't
             want any background subtraction.
         input_ROI_table: Name of the ROI table that contains the information
             about the location of the individual field of views (FOVs) to
             which the illumination correction shall be applied. Defaults to
             "FOV_ROI_table", the default name Fractal converters give the ROI
@@ -196,15 +197,16 @@
 
     # Assemble dictionary of matrices and check their shapes
     corrections = {}
     for channel in channels:
         wavelength_id = channel.wavelength_id
         corrections[wavelength_id] = imread(
             (
-                Path(illumination_profiles_folder) / dict_corr[wavelength_id]
+                Path(illumination_profiles_folder)
+                / illumination_profiles[wavelength_id]
             ).as_posix()
         )
         if corrections[wavelength_id].shape != (img_size_y, img_size_x):
             raise ValueError(
                 "Error in illumination_correction, "
                 "correction matrix has wrong shape."
             )
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/image_based_registration_hcs_init.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/image_based_registration_hcs_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def image_based_registration_hcs_init(
     *,
-    # Fractal arguments
+    # Fractal parameters
     zarr_urls: list[str],
     zarr_dir: str,
-    # Task-specific arguments
+    # Core parameters
     reference_cycle: int = 0,
 ) -> dict[str, list[dict[str, Any]]]:
     """
     Initialized calculate registration task
 
     This task prepares a parallelization list of all zarr_urls that need to be
     used to calculate the registration between cycles (all zarr_urls except
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/import_ome_zarr.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/import_ome_zarr.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,22 +160,25 @@
     types = dict(is_3D=is_3D)
     return types
 
 
 @validate_arguments
 def import_ome_zarr(
     *,
+    # Fractal parameters
     zarr_urls: list[str],
     zarr_dir: str,
+    # Core parameters
     zarr_name: str,
+    update_omero_metadata: bool = True,
     add_image_ROI_table: bool = True,
     add_grid_ROI_table: bool = True,
+    # Advanced parameters
     grid_y_shape: int = 2,
     grid_x_shape: int = 2,
-    update_omero_metadata: bool = True,
     overwrite: bool = False,
 ) -> dict[str, Any]:
     """
     Import a single OME-Zarr into Fractal.
 
     The single OME-Zarr can be a full OME-Zarr HCS plate or an individual
     OME-Zarr image. The image needs to be in the zarr_dir as specified by the
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,35 +22,34 @@
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def init_group_by_well_for_multiplexing(
     *,
-    # Fractal arguments
+    # Fractal parameters
     zarr_urls: list[str],
     zarr_dir: str,
-    # Task-specific arguments
+    # Core parameters
     reference_cycle: int = 0,
 ) -> dict[str, list[str]]:
     """
     Finds images for all acquisitions per well.
 
     Returns the parallelization_list to run `find_registration_consensus`.
 
     Args:
         zarr_urls: List of paths or urls to the individual OME-Zarr image to
             be processed.
             (standard argument for Fractal tasks, managed by Fractal server).
         zarr_dir: path of the directory where the new OME-Zarrs will be
             created. Not used by this task.
             (standard argument for Fractal tasks, managed by Fractal server).
-        reference_cycle: Which cycle to register against. Defaults to 0,
-            which is the first OME-Zarr image in the well, usually the first
-            cycle that was provided
+        reference_cycle: Which cycle to register against. Uses the OME-NGFF
+            HCS well metadata acquisition keys to find the reference cycle.
     """
     logger.info(
         f"Running `init_group_by_well_for_multiplexing` for {zarr_urls=}"
     )
     image_groups = create_well_acquisition_dict(zarr_urls)
 
     # Create the parallelization list
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/io_models.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/io_models.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/maximum_intensity_projection.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/maximum_intensity_projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,18 @@
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def maximum_intensity_projection(
     *,
+    # Fractal parameters
     zarr_url: str,
     init_args: InitArgsMIP,
+    # Advanced parameters
     overwrite: bool = False,
 ) -> dict[str, Any]:
     """
     Perform maximum-intensity projection along Z axis.
 
     Note: this task stores the output in a new zarr file.
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/tasks/napari_workflows_wrapper.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/napari_workflows_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,22 +58,23 @@
 
     pass
 
 
 @validate_arguments
 def napari_workflows_wrapper(
     *,
-    # Fractal argument
+    # Fractal parameters
     zarr_url: str,
-    # Task-specific arguments:
+    # Core parameters
     workflow_file: str,
     input_specs: dict[str, NapariWorkflowsInput],
     output_specs: dict[str, NapariWorkflowsOutput],
     input_ROI_table: str = "FOV_ROI_table",
     level: int = 0,
+    # Advanced parameters
     relabeling: bool = True,
     expected_dimensions: int = 3,
     overwrite: bool = True,
 ):
     """
     Run a napari-workflow on the ROIs of a single OME-NGFF image.
```

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/upscale_array.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/upscale_array.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/utils.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/fractal_tasks_core/zarr_utils.py` & `fractal_tasks_core-1.0.0a2/fractal_tasks_core/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a1/pyproject.toml` & `fractal_tasks_core-1.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-tasks-core"
-version = "1.0.0a1"
+version = "1.0.0a2"
 description = "Core bioimage-analysis library and tasks of the Fractal analytics platform"
 authors = [
     "Joel Lüthi  <joel.luethi@fmi.ch>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
@@ -82,18 +82,18 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 branch = true
 parallel = true
 relative_files = true
 source = ["fractal_tasks_core"]
-omit = ["tests/*", "examples/*", "fractal_tasks_core/dev/*", "fractal_tasks_core/tasks/compress_tif.py"]
+omit = ["tests/*", "examples/*", "fractal_tasks_core/dev/*"]
 
 [tool.bumpver]
-current_version = "1.0.0a1"
+current_version = "1.0.0a2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_tasks_core-1.0.0a1/PKG-INFO` & `fractal_tasks_core-1.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-tasks-core
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Core bioimage-analysis library and tasks of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-tasks-core
 License: BSD-3-Clause
 Author: Joel Lüthi 
 Author-email: joel.luethi@fmi.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

