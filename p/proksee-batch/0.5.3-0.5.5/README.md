# Comparing `tmp/proksee_batch-0.5.3.tar.gz` & `tmp/proksee_batch-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proksee_batch-0.5.3.tar", max compression
+gzip compressed data, was "proksee_batch-0.5.5.tar", max compression
```

## Comparing `proksee_batch-0.5.3.tar` & `proksee_batch-0.5.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1089 2024-03-18 15:19:34.862723 proksee_batch-0.5.3/LICENSE
--rw-r--r--   0        0        0     3861 2024-03-18 15:19:34.862723 proksee_batch-0.5.3/README.md
--rw-r--r--   0        0        0     1797 2024-03-18 15:19:43.918751 proksee_batch-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       21 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/__init__.py
--rw-r--r--   0        0        0    15177 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/__main__.py
--rw-r--r--   0        0        0     2330 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png
--rw-r--r--   0        0        0    22591 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/batch.js
--rw-r--r--   0        0        0   208923 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/cgview.min.js
--rw-r--r--   0        0        0     1843 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/controls.js
--rw-r--r--   0        0        0   274269 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/d3.min.js
--rw-r--r--   0        0        0    61938 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js
--rw-r--r--   0        0        0    14980 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/styles/cgview.css
--rw-r--r--   0        0        0     5696 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/styles/controls.css
--rw-r--r--   0        0        0    12170 2024-03-18 15:19:34.866723 proksee_batch-0.5.3/src/proksee_batch/data/assets/styles/style.css
--rw-r--r--   0        0        0  5809583 2024-03-18 15:19:34.898723 proksee_batch-0.5.3/src/proksee_batch/data/data.example/genome_maps/genome_1.js
--rw-r--r--   0        0        0  5469891 2024-03-18 15:19:34.906723 proksee_batch-0.5.3/src/proksee_batch/data/data.example/genome_maps/genome_2.js
--rw-r--r--   0        0        0  6164597 2024-03-18 15:19:34.926723 proksee_batch-0.5.3/src/proksee_batch/data/data.example/genome_maps/genome_3.js
--rw-r--r--   0        0        0  7518134 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/data.example/genome_maps/genome_4.js
--rw-r--r--   0        0        0     3605 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/data.example/table_data.js
--rw-r--r--   0        0        0   221376 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/default_proksee_template.json
--rw-r--r--   0        0        0      158 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/bed/e_coli_features.bed
--rw-r--r--   0        0        0      269 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/blast/blast_against_e_coli.txt
--rw-r--r--   0        0        0      180 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/vcf/e_coli_variants.vcf
--rw-r--r--   0        0        0       79 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/bed/k_aerogenes_features.bed
--rw-r--r--   0        0        0      134 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/blast/blast_against_k_aerogenes.txt
--rw-r--r--   0        0        0       75 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/bed/s_enterica_features.bed
--rw-r--r--   0        0        0      130 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/blast/blast_against_s_enterica.txt
--rw-r--r--   0        0        0       75 2024-03-18 15:19:34.950723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/bed/s_flexneri_features.bed
--rw-r--r--   0        0        0      130 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/blast/blast_against_s_flexneri.txt
--rw-r--r--   0        0        0     5127 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/data/report.html
--rw-r--r--   0        0        0     6474 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/download_example_input.py
--rw-r--r--   0        0        0      895 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/generate_proksee_link.py
--rw-r--r--   0        0        0     5311 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/generate_report_html.py
--rw-r--r--   0        0        0     1037 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/get_stats_from_seq_file.py
--rw-r--r--   0        0        0     1952 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/merge_cgview_json_with_template.py
--rw-r--r--   0        0        0    21297 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/parse_additional_features.py
--rw-r--r--   0        0        0        0 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/py.typed
--rw-r--r--   0        0        0     1163 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/remove_covered_features.py
--rw-r--r--   0        0        0     2658 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/scrape_proksee_image.py
--rw-r--r--   0        0        0    10839 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/seq_file_to_cgview_json.py
--rw-r--r--   0        0        0    23912 2024-03-18 15:19:34.954723 proksee_batch-0.5.3/src/proksee_batch/validate_input_data.py
--rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 proksee_batch-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-17 19:31:20.557570 proksee_batch-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3861 2024-04-17 19:31:20.557570 proksee_batch-0.5.5/README.md
+-rw-r--r--   0        0        0     1797 2024-04-17 19:31:31.937689 proksee_batch-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/__init__.py
+-rw-r--r--   0        0        0    15177 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/__main__.py
+-rw-r--r--   0        0        0     2330 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png
+-rw-r--r--   0        0        0    22591 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/batch.js
+-rw-r--r--   0        0        0   208923 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/cgview.min.js
+-rw-r--r--   0        0        0     1843 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/controls.js
+-rw-r--r--   0        0        0   274269 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/d3.min.js
+-rw-r--r--   0        0        0    61938 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js
+-rw-r--r--   0        0        0    14980 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/styles/cgview.css
+-rw-r--r--   0        0        0     5696 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/styles/controls.css
+-rw-r--r--   0        0        0    12170 2024-04-17 19:31:20.561570 proksee_batch-0.5.5/src/proksee_batch/data/assets/styles/style.css
+-rw-r--r--   0        0        0  5809583 2024-04-17 19:31:20.593570 proksee_batch-0.5.5/src/proksee_batch/data/data.example/genome_maps/genome_1.js
+-rw-r--r--   0        0        0  5469891 2024-04-17 19:31:20.601570 proksee_batch-0.5.5/src/proksee_batch/data/data.example/genome_maps/genome_2.js
+-rw-r--r--   0        0        0  6164597 2024-04-17 19:31:20.621571 proksee_batch-0.5.5/src/proksee_batch/data/data.example/genome_maps/genome_3.js
+-rw-r--r--   0        0        0  7518134 2024-04-17 19:31:20.645571 proksee_batch-0.5.5/src/proksee_batch/data/data.example/genome_maps/genome_4.js
+-rw-r--r--   0        0        0     3605 2024-04-17 19:31:20.645571 proksee_batch-0.5.5/src/proksee_batch/data/data.example/table_data.js
+-rw-r--r--   0        0        0   221376 2024-04-17 19:31:20.645571 proksee_batch-0.5.5/src/proksee_batch/data/default_proksee_template.json
+-rw-r--r--   0        0        0      158 2024-04-17 19:31:20.645571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/bed/e_coli_features.bed
+-rw-r--r--   0        0        0      269 2024-04-17 19:31:20.645571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/blast/blast_against_e_coli.txt
+-rw-r--r--   0        0        0      180 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/vcf/e_coli_variants.vcf
+-rw-r--r--   0        0        0       79 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/bed/k_aerogenes_features.bed
+-rw-r--r--   0        0        0      134 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/blast/blast_against_k_aerogenes.txt
+-rw-r--r--   0        0        0       75 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/bed/s_enterica_features.bed
+-rw-r--r--   0        0        0      130 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/blast/blast_against_s_enterica.txt
+-rw-r--r--   0        0        0       75 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/bed/s_flexneri_features.bed
+-rw-r--r--   0        0        0      130 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/blast/blast_against_s_flexneri.txt
+-rw-r--r--   0        0        0     5127 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/data/report.html
+-rw-r--r--   0        0        0     6474 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/download_example_input.py
+-rw-r--r--   0        0        0      895 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/generate_proksee_link.py
+-rw-r--r--   0        0        0     5311 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/generate_report_html.py
+-rw-r--r--   0        0        0     1037 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/get_stats_from_seq_file.py
+-rw-r--r--   0        0        0     1952 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/merge_cgview_json_with_template.py
+-rw-r--r--   0        0        0    21297 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/parse_additional_features.py
+-rw-r--r--   0        0        0        0 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/py.typed
+-rw-r--r--   0        0        0     1163 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/remove_covered_features.py
+-rw-r--r--   0        0        0     2658 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/scrape_proksee_image.py
+-rw-r--r--   0        0        0    10839 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/seq_file_to_cgview_json.py
+-rw-r--r--   0        0        0    23940 2024-04-17 19:31:20.649571 proksee_batch-0.5.5/src/proksee_batch/validate_input_data.py
+-rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 proksee_batch-0.5.5/PKG-INFO
```

### Comparing `proksee_batch-0.5.3/LICENSE` & `proksee_batch-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/README.md` & `proksee_batch-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/pyproject.toml` & `proksee_batch-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proksee-batch"
-version = "0.5.3"
+version = "0.5.5"
 description = "Proksee Batch"
 authors = ["Lael D. Barlow"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/stothard-group/proksee-batch"
 repository = "https://github.com/stothard-group/proksee-batch"
 documentation = "https://proksee-batch.readthedocs.io"
```

### Comparing `proksee_batch-0.5.3/src/proksee_batch/__main__.py` & `proksee_batch-0.5.5/src/proksee_batch/__main__.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/batch.js` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/batch.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/cgview.min.js` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/cgview.min.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/controls.js` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/controls.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/d3.min.js` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/d3.min.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/styles/cgview.css` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/styles/cgview.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/styles/controls.css` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/styles/controls.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/assets/styles/style.css` & `proksee_batch-0.5.5/src/proksee_batch/data/assets/styles/style.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/data.example/genome_maps/genome_1.js` & `proksee_batch-0.5.5/src/proksee_batch/data/data.example/genome_maps/genome_1.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/data.example/genome_maps/genome_2.js` & `proksee_batch-0.5.5/src/proksee_batch/data/data.example/genome_maps/genome_2.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/data.example/genome_maps/genome_3.js` & `proksee_batch-0.5.5/src/proksee_batch/data/data.example/genome_maps/genome_3.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/data.example/genome_maps/genome_4.js` & `proksee_batch-0.5.5/src/proksee_batch/data/data.example/genome_maps/genome_4.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/data.example/table_data.js` & `proksee_batch-0.5.5/src/proksee_batch/data/data.example/table_data.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/default_proksee_template.json` & `proksee_batch-0.5.5/src/proksee_batch/data/default_proksee_template.json`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/data/report.html` & `proksee_batch-0.5.5/src/proksee_batch/data/report.html`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/download_example_input.py` & `proksee_batch-0.5.5/src/proksee_batch/download_example_input.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/generate_proksee_link.py` & `proksee_batch-0.5.5/src/proksee_batch/generate_proksee_link.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/generate_report_html.py` & `proksee_batch-0.5.5/src/proksee_batch/generate_report_html.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/get_stats_from_seq_file.py` & `proksee_batch-0.5.5/src/proksee_batch/get_stats_from_seq_file.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/merge_cgview_json_with_template.py` & `proksee_batch-0.5.5/src/proksee_batch/merge_cgview_json_with_template.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/parse_additional_features.py` & `proksee_batch-0.5.5/src/proksee_batch/parse_additional_features.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/remove_covered_features.py` & `proksee_batch-0.5.5/src/proksee_batch/remove_covered_features.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/scrape_proksee_image.py` & `proksee_batch-0.5.5/src/proksee_batch/scrape_proksee_image.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/seq_file_to_cgview_json.py` & `proksee_batch-0.5.5/src/proksee_batch/seq_file_to_cgview_json.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.3/src/proksee_batch/validate_input_data.py` & `proksee_batch-0.5.5/src/proksee_batch/validate_input_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         # Check that the subdirectory contains a genbank subdirectory, a fasta subdirectory, or both.
         required_subdirectories = ["genbank", "fasta"]
         if not any(
             os.path.isdir(os.path.join(input, genome_dir, subdirectory))
             for subdirectory in required_subdirectories
         ):
             handle_error_exit(
-                f"The input directory {input} does not contain any of the required subdirectories: {required_subdirectories}"
+                f"The input directory {os.path.join(input, genome_dir)} is missing one or both of the required subdirectories: {required_subdirectories}"
             )
 
         # Check that all subdirectories have valid names.
         valid_subdirectories = [
             "genbank",
             "fasta",
             "blast",
```

### Comparing `proksee_batch-0.5.3/PKG-INFO` & `proksee_batch-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proksee-batch
-Version: 0.5.3
+Version: 0.5.5
 Summary: Proksee Batch
 Home-page: https://github.com/stothard-group/proksee-batch
 License: MIT
 Author: Lael D. Barlow
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

