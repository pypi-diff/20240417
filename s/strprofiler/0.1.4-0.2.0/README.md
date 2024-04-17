# Comparing `tmp/strprofiler-0.1.4.tar.gz` & `tmp/strprofiler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strprofiler-0.1.4.tar", max compression
+gzip compressed data, was "strprofiler-0.2.0.tar", max compression
```

## Comparing `strprofiler-0.1.4.tar` & `strprofiler-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,29 @@
--rwxr-xr-x   0        0        0     1091 2022-08-20 06:50:55.981663 strprofiler-0.1.4/LICENSE
--rwxr-xr-x   0        0        0    15091 2024-01-21 03:16:23.025568 strprofiler-0.1.4/README.md
--rwxr-xr-x   0        0        0      657 2024-01-21 03:55:40.357144 strprofiler-0.1.4/pyproject.toml
--rwxr-xr-x   0        0        0    24147 2024-01-21 03:16:23.034597 strprofiler-0.1.4/strprofiler.py
--rw-r--r--   0        0        0    15797 1970-01-01 00:00:00.000000 strprofiler-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1104 2024-04-05 20:30:55.631155 strprofiler-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0    17476 2024-04-15 13:35:41.805092 strprofiler-0.2.0/README.md
+-rwxr-xr-x   0        0        0      886 2024-04-15 13:35:41.814092 strprofiler-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2024-03-08 15:45:10.361080 strprofiler-0.2.0/strprofiler/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-04-04 17:53:48.533048 strprofiler-0.2.0/strprofiler/shiny_app/__init__.py
+-rwxr-xr-x   0        0        0      173 2024-04-05 20:58:48.036909 strprofiler-0.2.0/strprofiler/shiny_app/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      171 2024-04-17 15:10:19.225291 strprofiler-0.2.0/strprofiler/shiny_app/__pycache__/__init__.cpython-39.pyc
+-rwxr-xr-x   0        0        0     3814 2024-04-05 20:58:48.056909 strprofiler-0.2.0/strprofiler/shiny_app/__pycache__/calc_functions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3808 2024-04-17 15:10:19.278787 strprofiler-0.2.0/strprofiler/shiny_app/__pycache__/calc_functions.cpython-39.pyc
+-rwxr-xr-x   0        0        0    18269 2024-04-05 20:58:48.041909 strprofiler-0.2.0/strprofiler/shiny_app/__pycache__/shiny_app.cpython-310.pyc
+-rwxr-xr-x   0        0        0    18775 2024-04-17 15:52:20.711587 strprofiler-0.2.0/strprofiler/shiny_app/__pycache__/shiny_app.cpython-39.pyc
+-rwxr-xr-x   0        0        0     8617 2024-04-17 19:09:00.483096 strprofiler-0.2.0/strprofiler/shiny_app/calc_functions.py
+-rwxr-xr-x   0        0        0    33476 2024-04-17 19:09:00.485097 strprofiler-0.2.0/strprofiler/shiny_app/shiny_app.py
+-rwxr-xr-x   0        0        0      425 2024-04-04 17:53:48.542048 strprofiler-0.2.0/strprofiler/shiny_app/www/Example_Batch_File.csv
+-rwxr-xr-x   0        0        0   191409 2024-04-15 13:35:41.820101 strprofiler-0.2.0/strprofiler/shiny_app/www/favicon.ico
+-rwxr-xr-x   0        0        0  1117090 2024-04-17 19:09:00.494159 strprofiler-0.2.0/strprofiler/shiny_app/www/help.html
+-rwxr-xr-x   0        0        0     5769 2024-04-17 19:09:00.497168 strprofiler-0.2.0/strprofiler/shiny_app/www/help.md
+-rwxr-xr-x   0        0        0    48304 2024-04-04 17:53:48.556049 strprofiler-0.2.0/strprofiler/shiny_app/www/jax_database.csv
+-rwxr-xr-x   0        0        0    94320 2024-04-13 23:27:28.412191 strprofiler-0.2.0/strprofiler/shiny_app/www/logo.png
+-rwxr-xr-x   0        0        0    11050 2024-04-13 23:27:28.769906 strprofiler-0.2.0/strprofiler/shiny_app/www/logo.svg
+-rwxr-xr-x   0        0        0     1038 2024-04-04 17:53:48.560050 strprofiler-0.2.0/strprofiler/shiny_app/www/masters_query.png
+-rwxr-xr-x   0        0        0     2051 2024-04-04 17:53:48.562048 strprofiler-0.2.0/strprofiler/shiny_app/www/masters_query_inverted.png
+-rwxr-xr-x   0        0        0     1103 2024-04-04 17:53:48.564050 strprofiler-0.2.0/strprofiler/shiny_app/www/masters_ref.png
+-rwxr-xr-x   0        0        0     1949 2024-04-04 17:53:48.567048 strprofiler-0.2.0/strprofiler/shiny_app/www/masters_ref_inverted.png
+-rwxr-xr-x   0        0        0     1499 2024-04-04 17:53:48.569050 strprofiler-0.2.0/strprofiler/shiny_app/www/tanabe.png
+-rwxr-xr-x   0        0        0     3308 2024-04-04 17:53:48.571049 strprofiler-0.2.0/strprofiler/shiny_app/www/tanabe_inverted.png
+-rwxr-xr-x   0        0        0    10343 2024-04-05 21:02:47.758591 strprofiler-0.2.0/strprofiler/strprofiler.py
+-rwxr-xr-x   0        0        0    14555 2024-04-17 19:16:04.437977 strprofiler-0.2.0/strprofiler/utils.py
+-rw-r--r--   0        0        0    18293 1970-01-01 00:00:00.000000 strprofiler-0.2.0/PKG-INFO
```

### Comparing `strprofiler-0.1.4/LICENSE` & `strprofiler-0.2.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Jared Andrews
+Copyright (c) 2024 Jared Andrews & Mike Lloyd
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `strprofiler-0.1.4/README.md` & `strprofiler-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# strprofiler
+<p align="center">
+    <img src="https://raw.githubusercontent.com/j-andrews7/strprofiler/dev/strprofiler/shiny_app/www/logo.png" alt="STRprofiler" height="300">
+</p>
 
 [![Coverage Status](https://coveralls.io/repos/github/j-andrews7/strprofiler/badge.svg?branch=main)](https://coveralls.io/github/j-andrews7/strprofiler?branch=main)
 [![PyPI version](https://badge.fury.io/py/strprofiler.svg)](https://badge.fury.io/py/strprofiler)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/strprofiler.svg)](https://pypi.python.org/pypi/strprofiler/)
 [![PyPI license](https://img.shields.io/pypi/l/strprofiler.svg)](https://pypi.python.org/pypi/strprofiler/)
 [![DOI](https://zenodo.org/badge/523477912.svg)](https://zenodo.org/badge/latestdoi/523477912)
 
+**STRprofiler** is a simple python utility to compare short tandem repeat (STR) profiles. In particular, it is designed to aid research labs in comparing models (e.g. cell lines & xenografts) generated from primary tissue samples to ensure contamination has not occurred. It includes basic checks for sample mixing and contamination.
 
-**strprofiler** is a simple python utility to compare short tandem repeat (STR) profiles. In particular, it is designed to aid research labs in comparing models (e.g. cell lines & xenografts) generated from primary tissue samples to ensure contamination has not occurred. It includes basic checks for sample mixing and contamination.
+**STRprofiler is intended only for research purposes.**
 
-**strprofiler is intended only for research purposes.**
-
-For each STR profile provided, **strprofiler** will generate a sample-specific report that includes the following similarity scores as compared to every other profile:
+For each STR profile provided, **STRprofiler** will generate a sample-specific report that includes the following similarity scores as compared to every other profile:
 
 [Tanabe, AKA the Sørenson-Dice coefficient](https://www.doi.org/10.11418/jtca1981.18.4_329):
 
 $$ score = \frac{2 * no.shared.alleles}{no.query.alleles + no.reference.alleles} $$
 
 [Masters (vs. query)](https://www.ncbi.nlm.nih.gov/pubmed/11416159): 
 
@@ -25,38 +26,39 @@
 
 $$ score = \frac{no.shared.alleles}{no.reference.alleles} $$
 
 Amelogenin is not included in the score computation by default but can be included by passing the `--score_amel` flag.
 
 ## Installation
 
-**strprofiler** is available on PyPI and can be installed with pip:
+**STRprofiler** is available on PyPI and can be installed with pip:
 
 ```bash
 pip install strprofiler
 ```
 
 ## Usage
 
-**strprofiler** can be run directly from the command line. 
+**STRprofiler** can be run directly from the command line. 
 
 `strprofiler -sm "SampleMap_exp.csv" -scol "Sample Name" -o ./strprofiler_output STR1.xlsx STR2.csv STR3.txt`
 
 Full usage information can be found by running `strprofiler --help`.
 
 ```bash
  Usage: strprofiler [OPTIONS] INPUT_FILES...   
 
  STRprofiler compares STR profiles to each other.  
 
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --tan_threshold    -tanth   FLOAT        Minimum Tanabe score to report as potential matches in summary table. [default: 80]                          │
 │ --mas_q_threshold  -masqth  FLOAT        Minimum Masters (vs. query) score to report as potential matches in summary table. [default: 80]             │
 │ --mas_r_threshold  -masrth  FLOAT        Minimum Masters (vs. reference) score to report as potential matches in summary table. [default: 80]         │
-│ --mix_threshold    -mix     INTEGER      Number of markers with >= 2 alleles allowed before a sample is flagged for potential mixing. [default: 3]    │
+│ --mix_threshold    -mix     INTEGER      Number of markers with >= 2 alleles allowed before a sample is flagged for potential mixing.                 |
+|                                            [default: 3]                                                                                               │
 │ --sample_map       -sm      PATH         Path to sample map in csv format for renaming. First column should be sample names as given                  |
 |                                            in STR file(s),  second should be new names to assign. No header.                                          │
 │ --database         -db      PATH         Path to an STR database file in csv, xlsx, tsv, or txt format.                                               │
 │ --amel_col         -acol    TEXT         Name of Amelogenin column in STR file(s). [default: AMEL]                                                    │
 │ --sample_col       -scol    TEXT         Name of sample column in STR file(s). [default: Sample]                                                      │
 │ --marker_col       -mcol    TEXT         Name of marker column in STR file(s). Only used if format is 'wide'. [default: Marker]                       │
 │ --penta_fix        -pfix                 Whether to try to harmonize PentaE/D allele spelling. [default: True]                                        │
@@ -65,15 +67,15 @@
 │ --version                                Show the version and exit.                                                                                   │
 │ --help                                   Show this message and exit.                                                                                  │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Input Files(s)
 
-**strprofiler** can take either a single STR file or multiple STR files as input. These files can be csv, tsv, tab-separated text, or xlsx (first sheet used) files. The STR file(s) should be in either 'wide' or 'long' format. The long format expects all columns to map to the markers except for the designated sample name column with each row reflecting a different profile, e.g.:
+**STRprofiler** can take either a single STR file or multiple STR files as input. These files can be csv, tsv, tab-separated text, or xlsx (first sheet used) files. The STR file(s) should be in either 'wide' or 'long' format. The long format expects all columns to map to the markers except for the designated sample name column with each row reflecting a different profile, e.g.:
 
 | Sample | D1S1656 |  DYS391 | D3S1358 | D2S441 | D16S539 | D5S818 | D8S1179 | D22S1045 | D18S51 |
 |:------:|:-------:|:-------:|:-------:|:------:|:-------:|:------:|:-------:|:--------:|:------:|
 | Line1  |   12,14 |      12 |      13 |  12,14 |    17.3 |  16,17 |    18.3 |          |  17,11 |
 | Line2  |   12,14 | 11.3,12 |   13,15 |  12,14 |    17.3 |  16,17 |    18.3 |          |  17,11 |
 | ...    |         |         |         |        |         |        |         |          |        |
 
@@ -114,15 +116,15 @@
 | Sample2      |  DYS391   | 10          | 468.83  | 6722        |             |         |             |             |
 | Sample2      |  FGA      | 21          | 294.67  | 11941       |             |         |             |             |
 
 In this format, the `marker_col` must be specified. Only columns beginning with "Allele" will be used to parse the alleles for each sample/marker. Any other size or height columns will be ignored.
 
 ## Output Files
 
-**strprofiler** generates two types of output files. The first is a summary file, which contains the top hits for each sample above the specified scoring thresholds. This file provides a useful overview in addition to a flag to identify samples with potential mixing for closer inspection. In the output directory, this file will be named `full_summary.strprofiler.YYYYMMDD.HH_MM_SS.csv` where the date and time are the time the program was run.
+**STRprofiler** generates two types of output files. The first is a summary file, which contains the top hits for each sample above the specified scoring thresholds. This file provides a useful overview in addition to a flag to identify samples with potential mixing for closer inspection. In the output directory, this file will be named `full_summary.strprofiler.YYYYMMDD.HH_MM_SS.csv` where the date and time are the time the program was run.
 
 In addition to the marker columns, the summary file contains the following columns:
 
 | **Column Name**           | **Description**                                                                      |
 |---------------------------|--------------------------------------------------------------------------------------|
 | **mixed**                 | Flag to indicate sample mixing.                                                      |
 | **top_hit**               | Name and Tanabe score of top match to sample.                                        |
@@ -145,25 +147,63 @@
 | **n_reference_alleles** | Total number of alleles in reference sample.                 |
 | **tanabe_score**        | Tanabe similarity score.                                     |
 | **masters_query_score** | Masters (vs query) similarity score.                         |
 | **masters_ref_score**   | Masters (vs reference) similarity score.                     |
 
 ## Database Comparison
 
-**strprofiler** can be also used to compare batches of samples against a larger database of samples. 
+**STRprofiler** can be also used to compare batches of samples against a larger database of samples. 
 
 `strprofiler -db ExampleSTR_database.csv -o ./strprofiler_output STR1.xlsx`
 
-In this mode, inputs are compared against the database samples only, and not among themselves. Outputs will be as described above for sample input(s). 
+In this mode, inputs are compared against the database samples only, and not among themselves. Outputs will be as described above for sample input(s).
+
+## The STRprofiler App
+
+New in v0.2.0 is `strprofiler-app`, a command that launches a Shiny application that allows for user queries against an uploaded or pre-defined database (provided with the `-db` parameter) of STR profiles.
+
+This application can provide a convenient portal to a group's STR database and can be hosted on standard Shiny servers, Posit Connect instances, or ShinyApps.io. 
+
+An example of the application can be seen [here](https://hg99x7-jared0andrews.shinyapps.io/strprofiler/).
+
+### Deploying an `strprofiler` App
+
+Building an app for deployment to any of the above options is simple.
+
+First, make your app.py file:
+
+```python
+from strprofiler.shiny_app.shiny_app import create_app
+
+database = "./tester_db.csv"
+app = create_app(db=database)
+```
+
+If no database is provided, an example database included with the package will be used. 
+This app can then be deployed to any of the above endpoints as [one would with any other Shiny app](https://shiny.posit.co/py/docs/deploy.html).
+
+Alternatively, one could export it as a shinylive app and host it on Github pages or similar.
+
+#### Database Format
+
+The database should be formatted as a samples by markers matrix and saved as a csv, tsv, tab-delimited txt, or xlsx file, the same format as for the standard `strprofiler` command, e.g:
+
+|Sample       |Amelogenin|CSF1PO|D13S317|D16S539|D18S51|D19S433|D21S11 |D2S1338|D3S1358|D5S818|D7S820|D8S1179|FGA|TH01 |TPOX|vWA|PentaE |PentaD |
+|-------------|----------|------|-------|-------|------|-------|-------|-------|-------|------|------|-------|---|-----|----|---|-------|-------|
+|sample1      |X,Y       |12    |8      |13     |14    |14     |31,31.2|17,19  |15     |11,12 |11,12 |12,15  |23 |7,9.3|8   |18 |       |       |
+|sample2      |X         |10    |9      |13     |16    |12,14  |29     |20,23  |15,16  |12,13 |9,12  |14,15  |18 |7    |8,9 |15 |       |       |
+
+Optionally, one may provide two metadata columns - "Center" and "Passage", which will be recognized as non-marker columns.
 
 ## Contributing
-You can contribute by creating [issues](https://github.com/j-andrews7/strprofiler/issues) to highlight bugs and make suggestions for additional features. [Pull requests](https://github.com/j-andrews7/strprofiler/pulls) are also very welcome.
+You can contribute by creating [issues](https://github.com/j-andrews7/strprofiler/issues) to highlight bugs and make suggestions for additional features.
+[Pull requests](https://github.com/j-andrews7/strprofiler/pulls) are also very welcome.
 
 ## License
 
-**strprofiler** is released on the MIT license. You are free to use, modify, or redistribute it in almost any way, provided you state changes to the code, disclose the source, and use the same license. It is released with zero warranty for any purpose and I retain no liability for its use. [Read the full license](https://github.com/j-andrews7/strprofiler/blob/master/LICENSE) for additional details.
+**STRprofiler** is released on the MIT license. You are free to use, modify, or redistribute it in almost any way, provided you state changes to the code, disclose the source, and use the same license. It is released with zero warranty for any purpose and the authors retain no liability for its use. [Read the full license](https://github.com/j-andrews7/strprofiler/blob/master/LICENSE) for additional details.
 
 ## Reference
 
 If you use **strprofiler** in your research, please cite the DOI:
 
-Jared Andrews, & Sam Culley. (2022). j-andrews7/strprofiler: v0.1.1 (v0.1.1). Zenodo. https://doi.org/10.5281/zenodo.7348387
+Jared Andrews, Mike Lloyd, & Sam Culley. (2024). j-andrews7/strprofiler: v0.2.0 (v0.2.0). Zenodo. https://doi.org/10.5281/zenodo.7348386
```

### Comparing `strprofiler-0.1.4/pyproject.toml` & `strprofiler-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 [tool.poetry]
 name = "strprofiler"
-version = "0.1.4"
+version = "0.2.0"
 description = "A simple python utility to compare short tandem repeat (STR) profiles."
-authors = ["Jared Andrews"]
+authors = ["Jared Andrews <jared.andrews07@gmail.com>",
+           "Mike Lloyd <mike.lloyd@jax.org>"]
 license = "MIT"
 repository = "https://github.com/j-andrews7/strprofiler"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 pandas = "^1.4.3"
 rich-click = "^1.5.2"
-numpy = "^1.23.3"
+numpy = "^1.26.3"
 openpyxl = "^3.0.10"
+shiny = "^0.8.0"
+shinyswatch = "^0.4.2"
+Jinja2 = "^3.1.3"
+faicons = "^0.2.2"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
-strprofiler = 'strprofiler:strprofiler'
+strprofiler = 'strprofiler.strprofiler:strprofiler'
+strprofiler-app = 'strprofiler.strprofiler:local_shiny_app'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = [
```

### Comparing `strprofiler-0.1.4/PKG-INFO` & `strprofiler-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 Metadata-Version: 2.1
 Name: strprofiler
-Version: 0.1.4
+Version: 0.2.0
 Summary: A simple python utility to compare short tandem repeat (STR) profiles.
 Home-page: https://github.com/j-andrews7/strprofiler
 License: MIT
 Author: Jared Andrews
-Requires-Python: >=3.8,<4.0
+Author-email: jared.andrews07@gmail.com
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: numpy (>=1.23.3,<2.0.0)
+Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: faicons (>=0.2.2,<0.3.0)
+Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: rich-click (>=1.5.2,<2.0.0)
+Requires-Dist: shiny (>=0.8.0,<0.9.0)
+Requires-Dist: shinyswatch (>=0.4.2,<0.5.0)
 Project-URL: Repository, https://github.com/j-andrews7/strprofiler
 Description-Content-Type: text/markdown
 
-# strprofiler
+<p align="center">
+    <img src="https://raw.githubusercontent.com/j-andrews7/strprofiler/dev/strprofiler/shiny_app/www/logo.png" alt="STRprofiler" height="300">
+</p>
 
 [![Coverage Status](https://coveralls.io/repos/github/j-andrews7/strprofiler/badge.svg?branch=main)](https://coveralls.io/github/j-andrews7/strprofiler?branch=main)
 [![PyPI version](https://badge.fury.io/py/strprofiler.svg)](https://badge.fury.io/py/strprofiler)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/strprofiler.svg)](https://pypi.python.org/pypi/strprofiler/)
 [![PyPI license](https://img.shields.io/pypi/l/strprofiler.svg)](https://pypi.python.org/pypi/strprofiler/)
 [![DOI](https://zenodo.org/badge/523477912.svg)](https://zenodo.org/badge/latestdoi/523477912)
 
+**STRprofiler** is a simple python utility to compare short tandem repeat (STR) profiles. In particular, it is designed to aid research labs in comparing models (e.g. cell lines & xenografts) generated from primary tissue samples to ensure contamination has not occurred. It includes basic checks for sample mixing and contamination.
 
-**strprofiler** is a simple python utility to compare short tandem repeat (STR) profiles. In particular, it is designed to aid research labs in comparing models (e.g. cell lines & xenografts) generated from primary tissue samples to ensure contamination has not occurred. It includes basic checks for sample mixing and contamination.
+**STRprofiler is intended only for research purposes.**
 
-**strprofiler is intended only for research purposes.**
-
-For each STR profile provided, **strprofiler** will generate a sample-specific report that includes the following similarity scores as compared to every other profile:
+For each STR profile provided, **STRprofiler** will generate a sample-specific report that includes the following similarity scores as compared to every other profile:
 
 [Tanabe, AKA the Sørenson-Dice coefficient](https://www.doi.org/10.11418/jtca1981.18.4_329):
 
 $$ score = \frac{2 * no.shared.alleles}{no.query.alleles + no.reference.alleles} $$
 
 [Masters (vs. query)](https://www.ncbi.nlm.nih.gov/pubmed/11416159): 
 
@@ -47,38 +52,39 @@
 
 $$ score = \frac{no.shared.alleles}{no.reference.alleles} $$
 
 Amelogenin is not included in the score computation by default but can be included by passing the `--score_amel` flag.
 
 ## Installation
 
-**strprofiler** is available on PyPI and can be installed with pip:
+**STRprofiler** is available on PyPI and can be installed with pip:
 
 ```bash
 pip install strprofiler
 ```
 
 ## Usage
 
-**strprofiler** can be run directly from the command line. 
+**STRprofiler** can be run directly from the command line. 
 
 `strprofiler -sm "SampleMap_exp.csv" -scol "Sample Name" -o ./strprofiler_output STR1.xlsx STR2.csv STR3.txt`
 
 Full usage information can be found by running `strprofiler --help`.
 
 ```bash
  Usage: strprofiler [OPTIONS] INPUT_FILES...   
 
  STRprofiler compares STR profiles to each other.  
 
 ╭─ Options ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --tan_threshold    -tanth   FLOAT        Minimum Tanabe score to report as potential matches in summary table. [default: 80]                          │
 │ --mas_q_threshold  -masqth  FLOAT        Minimum Masters (vs. query) score to report as potential matches in summary table. [default: 80]             │
 │ --mas_r_threshold  -masrth  FLOAT        Minimum Masters (vs. reference) score to report as potential matches in summary table. [default: 80]         │
-│ --mix_threshold    -mix     INTEGER      Number of markers with >= 2 alleles allowed before a sample is flagged for potential mixing. [default: 3]    │
+│ --mix_threshold    -mix     INTEGER      Number of markers with >= 2 alleles allowed before a sample is flagged for potential mixing.                 |
+|                                            [default: 3]                                                                                               │
 │ --sample_map       -sm      PATH         Path to sample map in csv format for renaming. First column should be sample names as given                  |
 |                                            in STR file(s),  second should be new names to assign. No header.                                          │
 │ --database         -db      PATH         Path to an STR database file in csv, xlsx, tsv, or txt format.                                               │
 │ --amel_col         -acol    TEXT         Name of Amelogenin column in STR file(s). [default: AMEL]                                                    │
 │ --sample_col       -scol    TEXT         Name of sample column in STR file(s). [default: Sample]                                                      │
 │ --marker_col       -mcol    TEXT         Name of marker column in STR file(s). Only used if format is 'wide'. [default: Marker]                       │
 │ --penta_fix        -pfix                 Whether to try to harmonize PentaE/D allele spelling. [default: True]                                        │
@@ -87,15 +93,15 @@
 │ --version                                Show the version and exit.                                                                                   │
 │ --help                                   Show this message and exit.                                                                                  │
 ╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## Input Files(s)
 
-**strprofiler** can take either a single STR file or multiple STR files as input. These files can be csv, tsv, tab-separated text, or xlsx (first sheet used) files. The STR file(s) should be in either 'wide' or 'long' format. The long format expects all columns to map to the markers except for the designated sample name column with each row reflecting a different profile, e.g.:
+**STRprofiler** can take either a single STR file or multiple STR files as input. These files can be csv, tsv, tab-separated text, or xlsx (first sheet used) files. The STR file(s) should be in either 'wide' or 'long' format. The long format expects all columns to map to the markers except for the designated sample name column with each row reflecting a different profile, e.g.:
 
 | Sample | D1S1656 |  DYS391 | D3S1358 | D2S441 | D16S539 | D5S818 | D8S1179 | D22S1045 | D18S51 |
 |:------:|:-------:|:-------:|:-------:|:------:|:-------:|:------:|:-------:|:--------:|:------:|
 | Line1  |   12,14 |      12 |      13 |  12,14 |    17.3 |  16,17 |    18.3 |          |  17,11 |
 | Line2  |   12,14 | 11.3,12 |   13,15 |  12,14 |    17.3 |  16,17 |    18.3 |          |  17,11 |
 | ...    |         |         |         |        |         |        |         |          |        |
 
@@ -136,15 +142,15 @@
 | Sample2      |  DYS391   | 10          | 468.83  | 6722        |             |         |             |             |
 | Sample2      |  FGA      | 21          | 294.67  | 11941       |             |         |             |             |
 
 In this format, the `marker_col` must be specified. Only columns beginning with "Allele" will be used to parse the alleles for each sample/marker. Any other size or height columns will be ignored.
 
 ## Output Files
 
-**strprofiler** generates two types of output files. The first is a summary file, which contains the top hits for each sample above the specified scoring thresholds. This file provides a useful overview in addition to a flag to identify samples with potential mixing for closer inspection. In the output directory, this file will be named `full_summary.strprofiler.YYYYMMDD.HH_MM_SS.csv` where the date and time are the time the program was run.
+**STRprofiler** generates two types of output files. The first is a summary file, which contains the top hits for each sample above the specified scoring thresholds. This file provides a useful overview in addition to a flag to identify samples with potential mixing for closer inspection. In the output directory, this file will be named `full_summary.strprofiler.YYYYMMDD.HH_MM_SS.csv` where the date and time are the time the program was run.
 
 In addition to the marker columns, the summary file contains the following columns:
 
 | **Column Name**           | **Description**                                                                      |
 |---------------------------|--------------------------------------------------------------------------------------|
 | **mixed**                 | Flag to indicate sample mixing.                                                      |
 | **top_hit**               | Name and Tanabe score of top match to sample.                                        |
@@ -167,26 +173,64 @@
 | **n_reference_alleles** | Total number of alleles in reference sample.                 |
 | **tanabe_score**        | Tanabe similarity score.                                     |
 | **masters_query_score** | Masters (vs query) similarity score.                         |
 | **masters_ref_score**   | Masters (vs reference) similarity score.                     |
 
 ## Database Comparison
 
-**strprofiler** can be also used to compare batches of samples against a larger database of samples. 
+**STRprofiler** can be also used to compare batches of samples against a larger database of samples. 
 
 `strprofiler -db ExampleSTR_database.csv -o ./strprofiler_output STR1.xlsx`
 
-In this mode, inputs are compared against the database samples only, and not among themselves. Outputs will be as described above for sample input(s). 
+In this mode, inputs are compared against the database samples only, and not among themselves. Outputs will be as described above for sample input(s).
+
+## The STRprofiler App
+
+New in v0.2.0 is `strprofiler-app`, a command that launches a Shiny application that allows for user queries against an uploaded or pre-defined database (provided with the `-db` parameter) of STR profiles.
+
+This application can provide a convenient portal to a group's STR database and can be hosted on standard Shiny servers, Posit Connect instances, or ShinyApps.io. 
+
+An example of the application can be seen [here](https://hg99x7-jared0andrews.shinyapps.io/strprofiler/).
+
+### Deploying an `strprofiler` App
+
+Building an app for deployment to any of the above options is simple.
+
+First, make your app.py file:
+
+```python
+from strprofiler.shiny_app.shiny_app import create_app
+
+database = "./tester_db.csv"
+app = create_app(db=database)
+```
+
+If no database is provided, an example database included with the package will be used. 
+This app can then be deployed to any of the above endpoints as [one would with any other Shiny app](https://shiny.posit.co/py/docs/deploy.html).
+
+Alternatively, one could export it as a shinylive app and host it on Github pages or similar.
+
+#### Database Format
+
+The database should be formatted as a samples by markers matrix and saved as a csv, tsv, tab-delimited txt, or xlsx file, the same format as for the standard `strprofiler` command, e.g:
+
+|Sample       |Amelogenin|CSF1PO|D13S317|D16S539|D18S51|D19S433|D21S11 |D2S1338|D3S1358|D5S818|D7S820|D8S1179|FGA|TH01 |TPOX|vWA|PentaE |PentaD |
+|-------------|----------|------|-------|-------|------|-------|-------|-------|-------|------|------|-------|---|-----|----|---|-------|-------|
+|sample1      |X,Y       |12    |8      |13     |14    |14     |31,31.2|17,19  |15     |11,12 |11,12 |12,15  |23 |7,9.3|8   |18 |       |       |
+|sample2      |X         |10    |9      |13     |16    |12,14  |29     |20,23  |15,16  |12,13 |9,12  |14,15  |18 |7    |8,9 |15 |       |       |
+
+Optionally, one may provide two metadata columns - "Center" and "Passage", which will be recognized as non-marker columns.
 
 ## Contributing
-You can contribute by creating [issues](https://github.com/j-andrews7/strprofiler/issues) to highlight bugs and make suggestions for additional features. [Pull requests](https://github.com/j-andrews7/strprofiler/pulls) are also very welcome.
+You can contribute by creating [issues](https://github.com/j-andrews7/strprofiler/issues) to highlight bugs and make suggestions for additional features.
+[Pull requests](https://github.com/j-andrews7/strprofiler/pulls) are also very welcome.
 
 ## License
 
-**strprofiler** is released on the MIT license. You are free to use, modify, or redistribute it in almost any way, provided you state changes to the code, disclose the source, and use the same license. It is released with zero warranty for any purpose and I retain no liability for its use. [Read the full license](https://github.com/j-andrews7/strprofiler/blob/master/LICENSE) for additional details.
+**STRprofiler** is released on the MIT license. You are free to use, modify, or redistribute it in almost any way, provided you state changes to the code, disclose the source, and use the same license. It is released with zero warranty for any purpose and the authors retain no liability for its use. [Read the full license](https://github.com/j-andrews7/strprofiler/blob/master/LICENSE) for additional details.
 
 ## Reference
 
 If you use **strprofiler** in your research, please cite the DOI:
 
-Jared Andrews, & Sam Culley. (2022). j-andrews7/strprofiler: v0.1.1 (v0.1.1). Zenodo. https://doi.org/10.5281/zenodo.7348387
+Jared Andrews, Mike Lloyd, & Sam Culley. (2024). j-andrews7/strprofiler: v0.2.0 (v0.2.0). Zenodo. https://doi.org/10.5281/zenodo.7348386
```

