# Comparing `tmp/ageml-0.0.1.tar.gz` & `tmp/ageml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ageml-0.0.1.tar", max compression
+gzip compressed data, was "ageml-0.1.0.tar", max compression
```

## Comparing `ageml-0.0.1.tar` & `ageml-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    10173 2023-12-04 15:30:31.571258 ageml-0.0.1/LICENSE
--rw-r--r--   0        0        0     2182 2023-12-04 15:31:39.615445 ageml-0.0.1/README.md
--rw-r--r--   0        0        0     1524 2023-12-04 16:37:56.913789 ageml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      213 2023-11-17 15:45:36.588410 ageml-0.0.1/src/ageml/__init__.py
--rw-r--r--   0        0        0      297 2023-12-04 16:37:12.462906 ageml-0.0.1/src/ageml/__main__.py
--rw-r--r--   0        0        0        0 2023-11-17 11:10:57.200810 ageml-0.0.1/src/ageml/datasets/.gitkeep
--rw-r--r--   0        0        0       47 2023-11-17 11:10:57.200810 ageml-0.0.1/src/ageml/datasets/__init__.py
--rw-r--r--   0        0        0     4005 2023-11-17 15:12:30.998700 ageml-0.0.1/src/ageml/datasets/synthetic_covariates.csv
--rw-r--r--   0        0        0     7529 2023-11-17 15:45:36.588410 ageml-0.0.1/src/ageml/datasets/synthetic_features.csv
--rw-r--r--   0        0        0     5428 2023-12-04 16:37:12.462906 ageml-0.0.1/src/ageml/datasets/synthetic_test_data.py
--rw-r--r--   0        0        0     6259 2023-12-04 16:37:12.462906 ageml-0.0.1/src/ageml/messages.py
--rw-r--r--   0        0        0    12730 2023-12-04 15:51:20.352201 ageml-0.0.1/src/ageml/modelling.py
--rw-r--r--   0        0        0      828 2023-11-28 10:53:38.587631 ageml-0.0.1/src/ageml/processing.py
--rw-r--r--   0        0        0    47471 2023-12-04 16:37:12.462906 ageml-0.0.1/src/ageml/ui.py
--rw-r--r--   0        0        0     2682 2023-11-28 10:53:38.607631 ageml-0.0.1/src/ageml/utils.py
--rw-r--r--   0        0        0    10975 2023-12-04 16:37:12.462906 ageml-0.0.1/src/ageml/visualizer.py
--rw-r--r--   0        0        0     3363 1970-01-01 00:00:00.000000 ageml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-02-01 16:04:14.969912 ageml-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6473 2024-04-10 09:29:39.217248 ageml-0.1.0/README.md
+-rw-r--r--   0        0        0     1818 2024-04-17 15:54:21.277357 ageml-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      213 2024-02-01 16:04:14.969912 ageml-0.1.0/src/ageml/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-17 15:38:20.296650 ageml-0.1.0/src/ageml/__main__.py
+-rw-r--r--   0        0        0    12575 2024-04-17 15:38:22.476232 ageml-0.1.0/src/ageml/commands.py
+-rw-r--r--   0        0        0        0 2024-02-01 16:04:14.969912 ageml-0.1.0/src/ageml/datasets/.gitkeep
+-rw-r--r--   0        0        0       47 2024-02-01 16:04:14.969912 ageml-0.1.0/src/ageml/datasets/__init__.py
+-rw-r--r--   0        0        0     4005 2024-02-01 16:04:14.969912 ageml-0.1.0/src/ageml/datasets/synthetic_covariates.csv
+-rw-r--r--   0        0        0     7529 2024-02-01 16:04:14.969912 ageml-0.1.0/src/ageml/datasets/synthetic_features.csv
+-rw-r--r--   0        0        0     5428 2024-04-17 15:38:20.296650 ageml-0.1.0/src/ageml/datasets/synthetic_test_data.py
+-rw-r--r--   0        0        0     6687 2024-04-17 15:38:20.296650 ageml-0.1.0/src/ageml/messages.py
+-rw-r--r--   0        0        0    22472 2024-04-17 15:38:22.476232 ageml-0.1.0/src/ageml/modelling.py
+-rw-r--r--   0        0        0     1835 2024-04-17 15:38:20.296650 ageml-0.1.0/src/ageml/processing.py
+-rw-r--r--   0        0        0    65573 2024-04-17 15:38:22.476232 ageml-0.1.0/src/ageml/ui.py
+-rw-r--r--   0        0        0     2918 2024-04-17 15:38:22.476232 ageml-0.1.0/src/ageml/utils.py
+-rw-r--r--   0        0        0    12384 2024-04-17 15:38:22.476232 ageml-0.1.0/src/ageml/visualizer.py
+-rw-r--r--   0        0        0     7721 1970-01-01 00:00:00.000000 ageml-0.1.0/PKG-INFO
```

### Comparing `ageml-0.0.1/LICENSE` & `ageml-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ageml-0.0.1/pyproject.toml` & `ageml-0.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ageml"
-version = "0.0.1"
+version = "0.1.0"
 description = "AgeML is a Python package for Age Modelling with Machine Learning made easy."
 authors = [ "Computational Neuroimaging Lab Bilbao, IIS Biobizkaia",
             "jorge.garcia.condado <jorgegarciacondado@gmail.com>",
             "inigo.tellaetxe <inigotellaetxe@gmail.com>",
             "asier.erramuzpe <aerramuzpe@gmail.com>",
             "jesus.cortes <jesus.m.cortes@gmail.com>"
             ]
 maintainers = ["jorge.garcia.condado <jorgegarciacondado@gmail.com>",
                 "inigo.tellaetxe <inigotellaetxe@gmail.com>"
                 ]
 readme = "README.md"
-repository = "https://github.com/compneurobilbao/AgeModelling"
+repository = "https://github.com/compneurobilbao/ageml"
 license = "Apache 2.0"
 keywords = ["Machine Learning", "Age Modelling", "Brain Age"]
 classifiers = ["Topic :: Software Development :: Libraries :: Python Modules"]
 packages = [{include = "ageml", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8, <3.12"
 numpy = "1.24"
 pandas = "2.0"
 scipy = "1.10"
 statsmodels = "0.14.0"
 matplotlib = "3.5"
 scikit-learn = "1.3"
 coverage-conditional-plugin = "^0.7.0"
+xgboost = "^2.0.3"
+pillow = "^10.2.0"
 
 [tool.poetry.dev-dependencies]
 nox-poetry = "*"
 # Testing
 pytest = "*"
 pytest-cov = "*"
 coverage_conditional_plugin = "*"
@@ -43,8 +45,15 @@
 flake8-bugbear = "*"
 flake8-broken-line = "*"
 flake8-comprehensions = "*"
 # Formatting
 black = {version = "^23.1a1", allow-prereleases = true}
 
 [tool.poetry.scripts]
-ageml = "ageml.__main__:main"
+ageml = "ageml.__main__:main"
+model_age = "ageml.commands:model_age"
+factor_correlation = "ageml.commands:factor_correlation"
+clinical_groups = "ageml.commands:clinical_groups"
+clinical_classify = "ageml.commands:clinical_classify"
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.29.0"
+
```

### Comparing `ageml-0.0.1/src/ageml/datasets/synthetic_covariates.csv` & `ageml-0.1.0/src/ageml/datasets/synthetic_covariates.csv`

 * *Files identical despite different names*

### Comparing `ageml-0.0.1/src/ageml/datasets/synthetic_features.csv` & `ageml-0.1.0/src/ageml/datasets/synthetic_features.csv`

 * *Files identical despite different names*

### Comparing `ageml-0.0.1/src/ageml/datasets/synthetic_test_data.py` & `ageml-0.1.0/src/ageml/datasets/synthetic_test_data.py`

 * *Files identical despite different names*

### Comparing `ageml-0.0.1/src/ageml/messages.py` & `ageml-0.1.0/src/ageml/messages.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,113 +1,127 @@
+from ageml.modelling import AgeML
+
 """Messages for the AgeML package."""
 
 # Help command messeages
-cv_command_message = "cv [nº splits] [seed]               - set CV parameters (Default: 5, 0)"
-help_command_message = "h                                   - help (this command)"
-load_command_message = "l --flag [file]                     - load file with the specified flag"
-model_command_message = "m model_type [param1, param2, ...]  - set model type and parameters (Default: linear)"
-output_command_message = "o [directory]                       - set output directory"
-quit_command_message = "q                                   - quit the program"
-run_command_message = "r [command]                         - run different programs (Options: age, lifestyle, clinical, classification)"
-scaler_command_message = "s scaler_type [param1, param2, ...] - set scaler type and parameters (Default: standard)"
+model_age_command_message = "model_age           - run age prediction modelling."
+factor_correlation_command_message = "factor_correlation     - run factor correlation analysis on age deltas."
+clinical_command_message = "clinical            - run analysis on clinical groups based on age deltas."
+classification_command_message = "classification      - run classification based on age deltas."
+quit_command_message = "q                   - quit the program"
 
 # Help long messeages
-run_long_description = (
-    "Run type. Choose between: age, lifestyle, clinical, classification. (Required) \n"
-    "age: Predict age from features. \n"
-    "lifestyle: Calculate associations between lifestyle and age gaps. \n"
-    "clinical: Calculate associations between clinical groups and age gaps. \n"
-    "classification: Classify clinicals groups from age gaps."
-)
-
-output_long_description = "Path to output directory where to save results. (Required)"
+output_long_description = "Path to output directory where to save results."
 
 features_long_description = (
-    "Path to input CSV file containing features. (Required: run age) \n"
+    "Path to input CSV file containing features. \n"
     "In the file the first column should be the ID, the second column should be the AGE, \n"
     "and the following columns the features. The first row should be the header for \n"
     "column names."
+    "\nMore info on the file format in:\n"
+    "https://github.com/compneurobilbao/ageml/blob/main/docs/input_file_specification.md#features-file"
 )
 
 model_long_description = (
     "Model type and model parameters to use. First argument is the type and the following \n"
-    "arguments are input as keyword arguments into the model. They must be seperated by an =.\n"
-    "Example: -m linear fit_intercept=False\n"
-    "Available Types: linear (Default: linear)"
+    "arguments are input as keyword arguments into the model. They must be seperated by an '='.\n"
+    "Example: -m linear_reg fit_intercept=False normalize=True\n"
+    f"Available Types: {list(AgeML.model_dict.keys())} (Default: linear_reg)"
 )
 
 scaler_long_description = (
     "Scaler type and scaler parameters to use. First argument is the type and the following \n"
     "arguments are input as keyword arguments into scaler. They must be seperated by an =.\n"
     "Example: -m standard\n"
-    "Available Types: standard (Default: standard)"
+    f"Available Types:{list(AgeML.scaler_dict.keys())} (Default: standard)"
 )
 
 cv_long_description = (
     "Number of CV splits with which to run the Cross Validation Scheme. Expect 1 or 2 \n"
     "integers. First integer is the number of splits and the second is the seed for \n"
     "randomization. Default: 5 0"
 )
 
 covar_long_description = (
     "Path to input CSV file containing covariates. \n"
     "In the file the first column should be the ID, the followins columns should be the \n"
     "covariates. The first row should be the header for column names."
+    "\nMore info on the file format in:\n"
+    "https://github.com/compneurobilbao/ageml/blob/main/docs/input_file_specification.md#covariates-file"
 )
 
 covar_name_long_description = (
-    "Name of the column (covariate) in the CSV file containing covariates, to make different models for each category of the covariate. \n"
+    "Name of the column (covariate) in the CSV file containing covariates, to make different\n"
+    "models for each category of the covariate. \n"
     "The name must be written exactly as it is in the CSV file. \n"
     "If no covariate name is given, no covariate separation will be done."
 )
 
 factors_long_description = (
-    "Path to input CSV file containing factors (Required: run lifestyle). \n"
+    "Path to input CSV file containing factors. \n"
     "In the file the first column should be the ID, the followins columns should be the \n"
     "factors. The first row should be the header for column names."
+    "\nMore info on the file format in:\n"
+    "https://github.com/compneurobilbao/ageml/blob/main/docs/input_file_specification.md#factors-file"
 )
 
 clinical_long_description = (
-    "Path to input CSV file containing conditions (Required: run clinical or classification).\n"
+    "Path to input CSV file containing conditions.\n"
     "In the file, the first column should be the ID, the second column should be whether the \n"
     "subject is a CONTROL, and the following columns are binary variables for different \n"
     "conditions. The first row should be the header for column names."
+    "\nMore info on the file format in:\n"
+    "https://github.com/compneurobilbao/ageml/blob/main/docs/input_file_specification.md#clinical-file"
 )
 
 systems_long_description = (
     "Path to input .txt file containing the features to use to model each system. \n"
     "Each new line corresponds to a different system. The parser follows a formatting \n"
     "where the first words in the line is the system name followed by a colon and then the \n"
     "names of the features seperated by commas. [SystemName]: [Feature1], [Feature2], ... \n"
     "(e.g. Brain Structure: White Matter Volume, Grey Matter Volume, VCSF Volume)"
+    "\nMore info on the file format in:\n"
+    "https://github.com/compneurobilbao/ageml/blob/main/docs/input_file_specification.md#systems-file"
 )
 
 ages_long_description = (
     "Path to input CSV file containing the ages of the subjects. \n"
     "In the file the first column should be the ID, the second column should be the age, \n"
     "the third column should be the predicted age, fourth age is corrected age and last \n"
     "column is the delta. The first row should be the header for column names."
 )
 
 groups_long_description = (
-    "Clinical groups to do classification on (Required: run classification). \n"
+    "Clinical groups to do classification. \n"
     "Two groups are required. (e.g. --groups cn ad)"
 )
 
-ages_long_description = (
-    "Path to input CSV file containing the ages of the subjects. \n"
-    "In the file the first column should be the ID, the second column should be the age, \n"
-    "the third column should be the predicted age, fourth age is corrected age and last \n"
-    "column is the delta. The first row should be the header for column names."
+
+poly_feature_extension_description = (
+    "Degree of the polynomial to use in Polynomial Feature Extension (from sklearn)\n"
+    "An integer is required. (e.g.   -fext 2    /   --feature_extension 1)"
 )
 
-groups_long_description = (
-    "Clinical groups to do classification on (Required: run classification). \n"
-    "Two groups are required. (e.g. --groups cn ad)"
+hyperparameter_grid_description = (
+    "Number of points for which the hyperparameter optimization Grid Search will train\n"
+    "a model. The parameter ranges are predefined. An integer is required.\n"
+    "(e.g.   -ht 100   /   --hyperparameter_tuning 100)"
+)
+
+thr_long_description = (
+    "Threshold for classification. Default: 0.5 \n"
+    "The threshold is used for assingning hard labels. (e.g. --thr 0.5)"
 )
+
+ci_long_description = ("Confidence interval for classification metrics. Default: 0.95 \n")
+
+read_the_documentation_message = ("\nFor more information, refer to the documentation in the ageml repository:\n"
+                                  "https://github.com/compneurobilbao/ageml/tree/main/docs\n"
+                                  )
+
 # UI information
 
 emblem = """
 ************************************************
 *  █████╗  ██████╗ ███████╗███╗   ███╗██╗      *
 * ██╔══██╗██╔════╝ ██╔════╝████╗ ████║██║      *
 * ███████║██║  ███╗█████╗  ██╔████╔██║██║      *
```

### Comparing `ageml-0.0.1/src/ageml/ui.py` & `ageml-0.1.0/src/ageml/ui.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 """
 
 import argparse
 import numpy as np
 import pandas as pd
 import os
 import warnings
+import copy
 
 from datetime import datetime
 from statsmodels.stats.multitest import multipletests
 import scipy.stats as stats
 
 import ageml.messages as messages
 from ageml.visualizer import Visualizer
-from ageml.utils import create_directory, feature_extractor, significant_markers, convert, log
+from ageml.utils import create_directory, feature_extractor, significant_markers, convert, log, NameTag
 from ageml.modelling import AgeML, Classifier
-from ageml.processing import find_correlations
+from ageml.processing import find_correlations, covariate_correction
 
 
 class Interface:
 
     """Reads, parses and executes user commands.
 
     This class allows the user to enter certain commands.
@@ -39,134 +40,543 @@
     -----------
     args: arguments with which to run the modelling
 
     Public methods:
     ---------------
     setup(self): Creates required directories and files to store results.
 
+    command_setup(self, dir_path): Create required directories and files to store results for command.
+
+    set_flags(self): Set flags.
+
     set_visualizer(self): Set visualizer with output directory.
 
-    set_model(self): Set model with parameters.
+    set_dict(self): Initialise dictionaries for data storage.
+
+    set_features_dataframes(self): Set features dataframes for each subject type, covariate and system.
+
+    generate_model(self): Set model with parameters.
 
     set_classifier(self): Set classifier with parameters.
 
+    update_params(self): Update initial parameters after load.
+
     check_file(self, file): Check that file exists.
 
     load_csv(self, file): Use panda to load csv into dataframe.
 
+    load_features(self, required): Load features from csv file.
+
+    load_covariates(self, required): Load covariates from csv file.
+
+    load_clinical(self, required): Load clinical from csv file.
+
+    load_factors(self, required): Load factors from csv file.
+
+    load_ages(self, required): Load ages from csv file.
+
+    system_parser(self, file): Parse systems file.
+
+    load_systems(self, required): Load systems file.
+
+    remove_missing_data(self): Remove subjects with missing values.
+
     load_data(self, required): Load data from csv files.
 
     age_distribution(self, dfs, labels=None): Use visualizer to show age distribution.
 
     features_vs_age(self, df, significance=0.05): Use visualizer to explore relationship between features and age.
 
     model_age(self, df, model): Use AgeML to fit age model with data.
 
-    predict_age(self, df, model): Use AgeML to predict age with data.
+    model_all(self): Model age for each system and covariate on controls.
+
+    predict_age(self, df, model, model_name): Use AgeML to predict age with data.
+
+    predict_all(self): Predict age for each system and covariate on all subject types excpet cn.
+
+    save_predictions(self): Save age predictions to csv.
 
     factors_vs_deltas(self, dfs_ages, dfs_factors, groups, significance=0.05): Calculate correlations between factors and deltas.
 
     deltas_by_group(self, df, labels): Calculate summary metrics of deltas by group.
 
     classify(self, df1, df2, groups): Classify two groups based on deltas.
 
     run_wrapper(self, run): Wrapper for running modelling with log.
 
-    run_age(self): Run basic age modelling.
+    run_age(self): Run age modelling.
 
-    run_lifestyle(self): Run age modelling with lifestyle factors.
+    run_factor_correlation(self): Factor correlation analysis between deltas and factors.
 
-    run_clinical(self): Run age modelling with clinical factors.
+    run_clinical(self): Analyse differences between deltas in clinical groups.
 
-    run_classification(self): Run classification between two different clinical groups.
+    run_classification(self): Classify groups based on deltas.
     """
 
     def __init__(self, args):
         """Initialise variables."""
 
         # Arguments with which to run modelling
         self.args = args
 
         # Flags
-        self.flags = {"clinical": False, "covariates": False}
+        self.set_flags()
 
         # Set up directory for storage of results
         self.setup()
 
-        # Initialise objects form library
-        self.set_visualizer()
-        self.set_model()
-        self.set_classifier()
-
     def setup(self):
-        """Create required directories and files to store results."""
+        """Create main directory."""
 
-        # Create directories
+        # Create directory
         self.dir_path = os.path.join(self.args.output, "ageml")
         if os.path.exists(self.dir_path):
-            warnings.warn(
-                "Directory %s already exists files may be overwritten." % self.dir_path,
-                category=UserWarning,
-            )
-        create_directory(self.dir_path)
-        create_directory(os.path.join(self.dir_path, "figures"))
+            warnings.warn("Directory %s already exists files may be overwritten." % self.dir_path,
+                          category=UserWarning)
+        else:
+            create_directory(self.dir_path)
 
-        # Create .txt log file and log time
+        # Create .txt log file for which command run
         self.log_path = os.path.join(self.dir_path, "log.txt")
         with open(self.log_path, "a") as f:
             current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             f.write(current_time + "\n")
 
-    def set_visualizer(self):
+    def command_setup(self, dir_path):
+        """Create required directories and files to store results for command.
+        
+        Parameters
+        ----------
+        dir_path: directory path to create"""
+
+        # Create directory
+        self.command_dir = os.path.join(self.dir_path, dir_path)
+        if os.path.exists(self.command_dir):
+            warnings.warn("Directory %s already exists files may be overwritten." % self.command_dir,
+                          category=UserWarning)
+        else:
+            create_directory(self.command_dir)
+
+        # Create .txt log file to save results and log time
+        self.log_path = os.path.join(self.command_dir, "log.txt")
+        with open(self.log_path, "a") as f:
+            current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+            f.write(current_time + "\n")
+        
+        # Set visualizer as command directory
+        self.set_visualizer(self.command_dir)
+
+        # Reset flags
+        self.set_flags()
+
+        # Set initial parameters for model to defaults
+        self.naming = ""
+        self.subject_types = ['cn']
+        self.covars = ['all']
+        self.systems = ['all']
+
+    def set_flags(self):
+        """Set flags."""
+
+        self.flags = {"clinical": False, "covariates": False, "covarname": False,
+                      "systems": False, "ages": False, "features": False}
+
+    def set_visualizer(self, dir):
         """Set visualizer with output directory."""
 
-        self.visualizer = Visualizer(self.dir_path)
+        self.visualizer = Visualizer(dir)
+
+    def set_dict(self):
+        """Initialise dictionaries for data storage."""
+
+        self.dfs = {subject_type: {covar: {system: {} for system in self.systems}
+                    for covar in self.covars} for subject_type in self.subject_types}
+        self.preds = {subject_type: {covar: {system: {} for system in self.systems}
+                      for covar in self.covars} for subject_type in self.subject_types}
+        self.models = {covar: {system: {} for system in self.systems} for covar in self.covars}
+        self.betas = {covar: {system: {} for system in self.systems} for covar in self.covars}
+
+    def set_features_dataframes(self):
+        """Set features dataframes for each subject type, covariate and system."""
+
+        # Obtain dataframes for each subject type, covariate and system
+        for subject_type in self.subject_types:
+            # Keep only the subjects of the specified type
+            df_sub = self.df_features[self.df_clinical[subject_type]]
+            for covar in self.covars:
+                # Keep subjects with the specified covariate
+                if self.flags['covarname']:
+                    covar_index = set(self.df_covariates[self.df_covariates[self.args.covar_name] == covar].index)
+                    df_cov = df_sub[df_sub.index.isin(covar_index)]
+                else:
+                    df_cov = df_sub
+                for system in self.systems:
+                    # Keep only the features of the system
+                    df_sys = df_cov[['age'] + self.dict_systems[system]]
+                    # Save the dataframe
+                    self.dfs[subject_type][covar][system] = df_sys
 
-    def set_model(self):
+    def generate_model(self):
         """Set model with parameters."""
 
-        self.ageml = AgeML(
+        model = AgeML(
             self.args.scaler_type,
             self.args.scaler_params,
             self.args.model_type,
             self.args.model_params,
-            self.args.cv_split,
-            self.args.seed,
+            self.args.model_cv_split,
+            self.args.model_seed,
+            self.args.hyperparameter_tuning,
+            self.args.feature_extension
         )
+        return model
 
-    def set_classifier(self):
+    def generate_classifier(self):
         """Set classifier with parameters."""
 
-        self.classifier = Classifier()
+        classifier = Classifier(
+            self.args.classifier_cv_split,
+            self.args.classifier_seed,
+            self.args.classifier_thr,
+            self.args.classifier_ci)
+        
+        return classifier
+
+    def update_params(self):
+        """Update initial parameters after load."""
+
+        # Check possible flags of interest
+        if self.flags['clinical']:
+            self.subject_types = self.df_clinical.columns.to_list()
+        if self.flags['covarname']:
+            self.covars = pd.unique(self.df_covariates[self.args.covar_name]).tolist()
+            self.naming += f"_{self.args.covar_name}"
+        if self.flags['systems']:
+            self.systems = list(self.dict_systems.keys())
+            self.naming += "_multisystem"
+        elif self.flags['features']:
+            self.dict_systems['all'] = self.df_features.columns.drop('age').to_list()
+        if self.flags['ages']:
+            self.systems = [col[6:] for col in self.df_ages.columns if "delta" in col]
 
     def check_file(self, file):
         """Check that file exists."""
         if not os.path.exists(file):
             return False
         else:
             return True
 
-    def load_csv(self, file):
-        """Use panda to load csv into dataframe.
+    def load_csv(self, file_type):
+        """Use pandas to load csv into dataframe, making all columns lowercase.
 
         Parameters
         ----------
-        file: path to file; must be .csv
+        file_type: type of file to load
         """
 
+        # Obtain file name
+        if hasattr(self.args, file_type):
+            file = getattr(self.args, file_type)
+        else:
+            file = None
+
         if file is not None:
             # Check file exists
             if not self.check_file(file):
                 raise FileNotFoundError("File %s not found." % file)
             df = pd.read_csv(file, header=0, index_col=0)
             df.columns = df.columns.str.lower()  # ensure lower case
             return df
         else:
             return None
 
+    def load_features(self, required=False):
+        """Load features from csv file.
+
+        Parameters
+        ----------
+        required: boolean to check if file is required
+        
+        Returns
+        -------
+        df: dataframe with features"""
+
+        # Load data
+        df = self.load_csv('features')
+
+        # Check that file
+        if required and df is None:
+            raise ValueError("Features file must be provided.")
+        elif df is None:
+            return df
+        
+        # Check that age column is present
+        if "age" not in df:
+            raise KeyError("Features file must contain a column name 'age', or any other case-insensitive variation.")
+
+        # Set features flag
+        self.flags['features'] = True
+
+        return df
+
+    def load_covariates(self, required=False):
+        """Load covariates from csv file.
+
+        Parameters
+        ----------
+        required: boolean to check if file is required
+        
+        Returns
+        -------
+        df: dataframe with covariates"""
+
+        # Load data
+        df = self.load_csv('covariates')
+
+        # Check required
+        if required and df is None:
+            raise ValueError("Covariates file must be provided.")
+        elif df is None:
+            return df
+        
+        # Set covariate flag
+        self.flags['covariates'] = True
+
+        # Set covariate for analysis
+        if hasattr(self.args, 'covar_name') and self.args.covar_name is not None:
+            self.flags['covarname'] = True
+            self.args.covar_name = self.args.covar_name.lower()
+            if self.args.covar_name not in df:
+                raise KeyError("Covariate column %s not found in covariates file." % self.args.covar_name)
+        
+        return df
+
+    def load_clinical(self, required=False):
+        """Load clinical from csv file.
+
+        Parameters
+        ----------
+        required: boolean to check if file is required
+        
+        Returns
+        -------
+        df: dataframe with clinical information"""
+
+        # Load data
+        df = self.load_csv('clinical')
+
+        # Check required
+        if required and df is None:
+            raise ValueError("Clinical file must be provided.")
+        elif df is None:
+            return df
+
+        # Check that CN in columns and boolean type
+        if "cn" not in df:
+            raise KeyError("Clinical file must contain a column name 'CN' or any other case-insensitive variation.")
+        elif [df[col].dtype == bool for col in df.columns].count(False) != 0:
+            raise TypeError("Clinical columns must be boolean type. Check that all values are encoded as 'True' or 'False'.")
+        
+        # Check that all columns have at least two subjects and show which column
+        for col in df.columns:
+            if df[col].sum() == 0:
+                raise ValueError("Clinical column %s has no subjects." % col)
+
+        # Find rows with all False
+        if not df.any(axis=1).all():
+            raise ValueError("Clinical file contains rows with all False values. Please check the file.")
+
+        # Set clinical flag
+        self.flags['clinical'] = True
+
+        return df
+
+    def load_factors(self, required=False):
+        """Load factors from csv file.
+
+        Parameters
+        ----------
+        required: boolean to check if file is required
+
+        Returns
+        -------
+        df: dataframe with factors"""
+        
+        # Load data
+        df = self.load_csv('factors')
+
+        # Check required
+        if required and df is None:
+            raise ValueError("Factors file must be provided.")
+        elif df is None:
+            return df
+        
+        return df
+
+    def load_ages(self, required=False):
+        """Load ages from csv file.
+
+        Parameters
+        ----------
+        required: boolean to check if file is required
+
+        Returns
+        -------
+        df: dataframe with ages"""
+
+        # Load data
+        df = self.load_csv('ages')
+
+        # Check required
+        if required and df is None:
+            raise ValueError("Ages file must be provided.")
+        elif df is None:
+            return df
+
+        # Required columns
+        self.flags['ages'] = True
+        req_cols = ["age", "predicted_age", "corrected_age", "delta"]
+        cols = [col.lower() for col in df.columns.to_list()]
+
+        # Check that columns are present
+        for col in req_cols:
+            if not any(c.startswith(col) for c in cols):
+                raise KeyError("Ages file missing the following column %s, or derived names." % col)
+
+        # Check that columns present are of the correct type
+        for col in cols:
+            if not any(col.startswith(c) for c in req_cols):
+                raise KeyError("Ages file contains unknwon column %s" % col)
+
+        return df
+
+    def system_parser(self, file):
+        """Parse systems file.
+
+        Parameters
+        ----------
+        file: file to parse
+
+        Returns
+        -------
+        dict_systems: dictionary with systems and their features"""
+
+        # Initialise dictionary
+        systems = {}
+
+        # Load feature names
+        features = {f.lower() for f in self.df_features.columns.to_list()}
+
+        # Parse file
+        for line in open(file, 'r'):
+            line = line.split("\n")[0]  # Remove newline character
+            line = line.split(':')  # Split by the separator
+
+            # Must have at exactly two elements (system, features)
+            if len(line) != 2:
+                raise ValueError("Systems file must be in the format 'system_name_1:feature1,feature2,...'")
+            
+            # Obtain system features ignoring trailing white spaces
+            system = line[0].strip()
+            systems_features = [f.lower().strip() for f in line[1].split(',')]
+
+            # Check features exist and not repeated
+            for f in systems_features:
+                if f not in features:
+                    raise ValueError("Feature '%s' not found in features file." % f)
+                elif systems_features.count(f) > 1:
+                    raise ValueError("Feature '%s' is repeated in the system: %s." % (f, system))
+            
+            # Save the system name and its features
+            systems[system] = systems_features
+
+        return systems
+
+    def load_systems(self, required=False):
+        """Load systems file.
+        
+        .txt expected. Format: system_name:feature1,feature2,...
+
+        Parameters
+        ----------
+        required: boolean to check if file is required
+
+        Returns
+        -------
+        systems: dictionary with systems and their features"""
+
+        # Initialise dictionary
+        systems = {}
+
+        # Check if systems file is provided
+        if hasattr(self.args, "systems"):
+            if self.args.systems is not None and not self.check_file(self.args.systems):
+                raise ValueError("Systems file '%s' not found." % self.args.systems)
+            elif required and self.args.systems is None:
+                raise ValueError("Systems file must be provided.")
+            elif self.args.systems is None:
+                return systems
+        else:
+            return systems
+        
+        # Set flag
+        self.flags['systems'] = True
+
+        # Parse file
+        systems = self.system_parser(self.args.systems)
+
+        # Check that the dictionary has at least one entry
+        if len(systems) == 0:
+            raise ValueError("Systems file is probably incorrectly formatted. Check it please.")
+        
+        return systems
+
+    def remove_missing_data(self):
+        """Remove subjects with missing values."""
+
+        # Dataframes
+        dfs = {'features': self.df_features, 'covariates': self.df_covariates,
+               'factors': self.df_factors, 'clinical': self.df_clinical, 'ages': self.df_ages}
+        dfs = {label: df for label, df in dfs.items() if df is not None}
+
+        # Subjects before removing missing data
+        init_count = {label: len(df) for label, df in dfs.items()}
+        for label in dfs.keys():
+            print("Number of subjects in dataframe %s: %d" % (label, init_count[label]))
+
+        # Check for missing data
+        print('Removing subjects with missing data...')
+        for label, df in dfs.items():
+            missing_subjects = df[df.isnull().any(axis=1)].index.to_list()
+            if missing_subjects.__len__() != 0:
+                warn_message = "Subjects with missing data in %s: %s" % (label, missing_subjects)
+                print(warn_message)
+                warnings.warn(warn_message, category=UserWarning)
+                dfs[label] = df.drop(missing_subjects)
+
+        # Check that all dataframes have the same subjects
+        print('Removing subjects not shared among dataframes...')
+        for l1, df1 in dfs.items():
+            for l2, df2 in dfs.items():
+                if l1 != l2:
+                    non_shared_idx = df1.index[~df1.index.isin(set(df2.index.to_list()))]
+                    if non_shared_idx.__len__() != 0:
+                        warn_message = ("Subjects in dataframe %s not in dataframe %s: %s"
+                                        % (l1, l2, non_shared_idx.to_list()))
+                        print(warn_message)
+                        warnings.warn(warn_message, category=UserWarning)
+                        dfs[l1] = df1.drop(non_shared_idx)
+
+        # Set dataframes
+        for label, df in dfs.items():
+            print("Final number of subjects in dataframe %s: %d (%.2f %% of initial)" %
+                  (label, len(df), len(df) / init_count[label] * 100))
+            setattr(self, f'df_{label}', df)
+
     def load_data(self, required=None):
         """Load data from csv files.
 
         Parameters
         ----------
         required: list of required files"""
 
@@ -174,750 +584,602 @@
         print("-----------------------------------")
         print("Loading data...")
 
         # Required files default
         if required is None:
             required = []
 
-        # Load features
-        self.df_features = self.load_csv(self.args.features)
-        if self.df_features is not None:
-            if "age" not in self.df_features.columns:
-                raise KeyError(
-                    "Features file must contain a column name 'age', or any other case-insensitive variation."
-                )
-        elif "features" in required:
-            raise ValueError("Features file must be provided.")
+        # Load Features
+        self.df_features = self.load_features(required="features" in required)
 
         # Load covariates
-        self.df_covariates = self.load_csv(self.args.covariates)
-        if self.df_covariates is not None:
-            # Check that covar name is given
-            if self.args.covar_name:
-                self.flags['covariates'] = True
-
-        # Load factors
-        self.df_factors = self.load_csv(self.args.factors)
-        if self.df_factors is None and "factors" in required:
-            raise ValueError("Factors file must be provided.")
+        self.df_covariates = self.load_covariates(required="covariates" in required)
 
         # Load clinical
-        self.df_clinical = self.load_csv(self.args.clinical)
-        if self.df_clinical is not None:
-            if "cn" not in self.df_clinical.columns:
-                raise KeyError(
-                    "Clinical file must contian a column name 'CN' or any other case-insensitive variation."
-                )
-            # Check datatypes of columns are all boolean
-            elif [
-                self.df_clinical[col].dtype == bool for col in self.df_clinical.columns
-            ].count(False) != 0:
-                raise TypeError("Clinical columns must be boolean type.")
-            else:
-                self.flags['clinical'] = True
-                self.cn_subjects = self.df_clinical[self.df_clinical["cn"]].index
-        elif "clinical" in required:
-            raise ValueError("Clinical file must be provided.")
+        self.df_clinical = self.load_clinical(required="clinical" in required)
+
+        # Load factors
+        self.df_factors = self.load_factors(required='factors' in required)
 
         # Load ages
-        # Check if already has ages loaded
-        if hasattr(self, "df_ages"):
-            if self.df_ages is None:
-                self.df_ages = self.load_csv(self.args.ages)
-            else:
-                # Dont over write if None
-                df = self.load_csv(self.args.ages)
-                if df is not None:
-                    self.df_ages = df
-                    warning_message = (
-                        "Ages file already loaded, overwriting with  %s provided file."
-                        % self.args.ages
-                    )
-                    print(warning_message)
-                    warnings.warn(warning_message, category=UserWarning)
-        else:
-            self.df_ages = self.load_csv(self.args.ages)
-
-        # Check that ages file has required columns
-        if self.df_ages is not None:
-            cols = ["age", "predicted age", "corrected age", "delta"]
-            for col in cols:
-                if col not in self.df_ages.columns:
-                    raise KeyError("Ages file must contain a column name %s" % col)
-
-        # Remove subjects with missing values
-        dfs = [
-            self.df_features,
-            self.df_covariates,
-            self.df_factors,
-            self.df_clinical,
-            self.df_ages,
-        ]
-        labels = ['features', 'covariates', 'factors', 'clinical', 'ages']
-        self.subjects_missing_data = []
-        for label, df in zip(labels, dfs):
-            if df is not None:
-                missing_subjects = df[df.isnull().any(axis=1)].index.to_list()
-                self.subjects_missing_data = (
-                    self.subjects_missing_data + missing_subjects
-                )
-                if missing_subjects.__len__() != 0:
-                    warn_message = "Subjects with missing data in %s: %s" % (label, missing_subjects)
-                    print(warn_message)
-                    warnings.warn(warn_message, category=UserWarning)
+        self.df_ages = self.load_ages(required="ages" in required)
 
-        # Check that all dataframes have the same subjects
-        for i in range(len(dfs)):
-            for j in range(len(dfs)):
-                if i != j:
-                    if dfs[i] is not None and dfs[j] is not None:
-                        # Find subjects in one dataframe but not the other
-                        non_shared_subjects = [s for s in dfs[i].index.to_list()
-                                               if s not in dfs[j].index.to_list()]
-                        if non_shared_subjects.__len__() != 0:
-                            warn_message = ("Subjects in dataframe %s not in dataframe %s: %s"
-                                            % (labels[i], labels[j], non_shared_subjects))
-                            print(warn_message)
-                            warnings.warn(warn_message, category=UserWarning)
-                            self.subjects_missing_data = (
-                                self.subjects_missing_data + non_shared_subjects
-                            )
-
-        # Remove subjects with missing values
-        self.subjects_missing_data = set(self.subjects_missing_data)
-        for df in dfs:
-            if df is not None:
-                df.drop(self.subjects_missing_data, inplace=True, errors="ignore")
+        # Load systems
+        self.dict_systems = self.load_systems(required="systems" in required)
+
+        # Removes subjects with missing values
+        self.remove_missing_data()
+
+        # Show number of subjects per clinical category
+        if self.flags['clinical']:
+            for col in self.df_clinical.columns:
+                print("Number of %s subjects: %d" % (col, self.df_clinical[col].sum()))
+        else:
+            print("No clinical information provided using all subjects as CN.")
+            if self.df_features is not None:
+                index = self.df_features.index
+            elif self.df_ages is not None:
+                index = self.df_ages.index
+            self.df_clinical = pd.DataFrame(index=index, columns=['cn'], data=True)
 
-    def age_distribution(self, dfs: list, labels=None, name=""):
+        # Update initial parameters after load
+        self.update_params()
+
+    def age_distribution(self, ages_dict: dict, name=""):
         """Use visualizer to show age distribution.
 
         Parameters
         ----------
-        dfs: list of dataframes with age information; shape=(n,m)
-        labels: categories of separation criterion
+        ages_dict: dictionary containing ages for each group
         name: name to give to visualizer to save file"""
 
         # Select age information
         print("-----------------------------------")
-        print("Age distribution %s" % name)
-        list_ages = []
-        for i, df in enumerate(dfs):
-            if labels is not None:
-                print(labels[i])
-            ages = df["age"].to_numpy()
-            print("Mean age: %.2f" % np.mean(ages))
-            print("Std age: %.2f" % np.std(ages))
-            print("Age range: [%d,%d]" % (np.min(ages), np.max(ages)))
-            list_ages.append(ages)
-
-        # Check that distributions of ages are similar
-        print("Checking that age distributions are similar...")
-        for i in range(len(list_ages)):
-            for j in range(i + 1, len(list_ages)):
-                _, p_val = stats.ttest_ind(list_ages[i], list_ages[j])
-                if p_val < 0.05:
-                    warn_message = "Age distributions %s and %s are not similar." % (
-                        labels[i],
-                        labels[j],
-                    )
-                    print(warn_message)
-                    warnings.warn(warn_message, category=UserWarning)
+        print("Age distribution of %s" % name)
+        for key, vals in ages_dict.items():
+            print("[Group: %s]" % key)
+            print("Mean age: %.2f" % np.mean(vals))
+            print("Std age: %.2f" % np.std(vals))
+            print("Age range: [%d,%d]" % (np.min(vals), np.max(vals)))
+
+        # Obtain labels and ages
+        labels = list(ages_dict.keys())
+        ages = list(ages_dict.values())
+
+        # Check that distributions of ages are similar if more than one
+        if len(ages_dict) > 1:
+            print("Checking that age distributions are similar using T-test: T-stat (p_value)")
+            print("If p_value > 0.05 distributions are considered simiilar and not displayed...")
+            for i in range(len(labels)):
+                for j in range(i + 1, len(labels)):
+                    t_stat, p_val = stats.ttest_ind(ages[i], ages[j])
+                    if p_val < 0.05:
+                        warn_message = "Age distributions %s and %s are not similar: %.2f (%.2g) " % (
+                            labels[i], labels[j], t_stat, p_val)
+                        print(warn_message)
+                        warnings.warn(warn_message, category=UserWarning)
 
         # Use visualiser
-        self.visualizer.age_distribution(list_ages, labels, name)
+        self.visualizer.age_distribution(ages, labels, name)
 
-    def features_vs_age(self, dfs: list, labels: list = None, significance: float = 0.05, name: str = ""):
+    def features_vs_age(self, features_dict: dict, tag, significance: float = 0.05, ):
         """Use visualizer to explore relationship between features and age.
 
         Parameters
         ----------
-        dfs: list of dataframes with features and age; shape=(n,m+1)
-        labels: # TODO
+        features_dict: dictionary containing features for each group
         significance: significance level for correlation"""
 
         # Select data to visualize
         print("-----------------------------------")
-        print("Features by correlation with Age")
+        print("Features by correlation with Age of Controls [System: %s]" % tag.system)
         print("significance: %.2g * -> FDR, ** -> bonferroni" % significance)
-        if not isinstance(dfs, list):
-            raise TypeError("Input to 'Interface.features_vs_age' must be a list of dataframes.")
-
-        if labels is not None:
-            print(labels)
 
         # Make lists to store covariate info for each dataframe
-        X_list = []
-        y_list = []
-        corr_list = []
-        order_list = []
-        significance_list = []
-        for df, label in zip(dfs, labels):
+        X_list, y_list, corr_list, order_list, significance_list = [], [], [], [], []
+        for label, df in features_dict.items():
+            print('Covariate %s' % label)
             # Extract features
             X, y, feature_names = feature_extractor(df)
+            # Covariate correction
+            if self.flags["covariates"] and not self.flags['covarname']:
+                print("Covariate effects will be subtracted from features.")
+                X, _ = covariate_correction(X, self.df_covariates.loc[df.index].to_numpy())
             # Calculate correlation between features and age
             corr, order, p_values = find_correlations(X, y)
             # Reject null hypothesis of no correlation
             reject_bon, _, _, _ = multipletests(p_values, alpha=significance, method='bonferroni')
             reject_fdr, _, _, _ = multipletests(p_values, alpha=significance, method='fdr_bh')
             significant = significant_markers(reject_bon, reject_fdr)
             # Print results
             for idx, order_element in enumerate(order):
-                print("%d.%s %s %s: %.2f" % (idx + 1, label, significant[order_element],
-                                             feature_names[order_element], corr[order_element]))
+                print("%d.%s %s %s: %.2f (%.2g)" % (idx + 1, label, significant[order_element],
+                                                    feature_names[order_element], corr[order_element],
+                                                    p_values[order_element]))
             # Append all the values
-            X_list.append(X)
-            y_list.append(y)
-            corr_list.append(corr)
-            order_list.append(order)
-            significance_list.append(significant)
+            X_list.append(X), y_list.append(y), corr_list.append(corr), order_list.append(order), significance_list.append(significant)
 
         # Use visualizer to show results
         self.visualizer.features_vs_age(X_list, y_list, corr_list, order_list,
-                                        significance_list, feature_names, labels, name)
+                                        significance_list, feature_names, tag, list(features_dict.keys()))
 
-    def model_age(self, df, model, name: str = ""):
+    def model_age(self, df, model, tag):
         """Use AgeML to fit age model with data.
 
         Parameters
         ----------
         df: dataframe with features and age; shape=(n,m+1)
-        model: AgeML object"""
+        model: AgeML object
+        name: name of the model"""
 
         # Show training pipeline
         print("-----------------------------------")
-        if name == "":
-            print("Training Age Model")
-        else:
-            print("Training Model for covariate %s" % name)
-        print(self.ageml.pipeline)
+        print(f"Training Age Model [Covariate:{tag.covar}, System:{tag.system}]")
+        print(model.pipeline)
 
         # Select data to model
         X, y, _ = feature_extractor(df)
 
+        # Throw error if we do not have enough controls for modelling
+        if X.shape[0] / self.args.model_cv_split < 2:
+            raise ValueError("Not enough controls for modelling for each CV split.")
+
+        # Covariate correction
+        if self.flags["covariates"] and not self.flags['covarname']:
+            print("Covariate effects will be subtracted from features.")
+            X, beta = covariate_correction(X, self.df_covariates.loc[df.index].to_numpy())
+        else:
+            beta = None
+
         # Fit model and plot results
         y_pred, y_corrected = model.fit_age(X, y)
-        self.visualizer.true_vs_pred_age(y, y_pred, name)
-        self.visualizer.age_bias_correction(y, y_pred, y_corrected, name)
+        self.visualizer.true_vs_pred_age(y, y_pred, tag)
+        self.visualizer.age_bias_correction(y, y_pred, y_corrected, tag)
 
         # Calculate deltas
         deltas = y_corrected - y
 
         # Save to dataframe and csv
         data = np.stack((y, y_pred, y_corrected, deltas), axis=1)
-        cols = ["age", "predicted age", "corrected age", "delta"]
+        cols = ["age", "predicted_age", "corrected_age", "delta"]
         df_ages = pd.DataFrame(data, index=df.index, columns=cols)
 
-        return model, df_ages
+        return model, df_ages, beta
+
+    def model_all(self):
+        """Model age for each system and covariate on controls."""
 
-    def predict_age(self, df, model):
+        # Iterate over covariate and system
+        for covar in self.covars:
+            for system in self.systems:
+                tag = NameTag(covar=covar, system=system)
+                # Generate model
+                ageml_model = self.generate_model()
+                self.models[covar][system], df_pred, self.betas[covar][system] = self.model_age(self.dfs['cn'][covar][system],
+                                                                                                ageml_model, tag=tag)
+                # Save predictions
+                df_pred = df_pred.drop(columns=['age'])
+                df_pred.rename(columns=lambda x: f"{x}_{system}", inplace=True)
+                self.preds['cn'][covar][system] = df_pred
+
+    def predict_age(self, df, model, tag: NameTag, beta: np.ndarray = None,):
         """Use AgeML to predict age with data."""
 
         # Show prediction pipeline
         print("-----------------------------------")
-        print("Predicting with Age Model")
-        print(self.ageml.pipeline)
+        print(f"Predicting for {tag.group}")
+        print(f"with Age Model [Covariate:{tag.covar}, System:{tag.system}]")
+        print(model.pipeline)
 
         # Select data to model
         X, y, _ = feature_extractor(df)
 
+        # Covariate correction
+        if self.flags["covariates"] and not self.flags['covarname']:
+            print("Covariate effects will be subtracted from features.")
+            X, _ = covariate_correction(X, self.df_covariates.loc[df.index].to_numpy(), beta)
+
         # Predict age
         y_pred, y_corrected = model.predict_age(X, y)
 
         # Calculate deltas
         deltas = y_corrected - y
 
         # Save to dataframe and csv
         data = np.stack((y, y_pred, y_corrected, deltas), axis=1)
-        cols = ["age", "predicted age", "corrected age", "delta"]
+        cols = ["age", "predicted_age", "corrected_age", "delta"]
         df_ages = pd.DataFrame(data, index=df.index, columns=cols)
 
         return df_ages
 
-    def factors_vs_deltas(self, dfs_ages, dfs_factors, groups, factor_names, significance=0.05):
+    def predict_all(self):
+        """Predict age for each system and covariate on all subject types excpet cn."""
+
+        for subject_type in self.subject_types:
+            # Do not apply to controls
+            if subject_type == 'cn':
+                continue
+            for covar in self.covars:
+                for system in self.systems:
+                    tag = NameTag(group=subject_type, covar=covar, system=system)
+                    df_pred = self.predict_age(self.dfs[subject_type][covar][system], self.models[covar][system],
+                                               tag, self.betas[covar][system])
+                    df_pred = df_pred.drop(columns=['age'])
+                    df_pred.rename(columns=lambda x: f"{x}_{system}", inplace=True)
+                    self.preds[subject_type][covar][system] = df_pred
+
+    def save_predictions(self):
+        """Save age predictions to csv."""
+
+        # Concatenate predictions into a DataFrame
+        stack = []
+        for subject_type in self.subject_types:
+            for covar in self.covars:
+                df_systems = pd.concat([self.preds[subject_type][covar][system] for system in self.systems], axis=1)
+                stack.append(df_systems)
+        df_ages = pd.concat(stack, axis=0)
+
+        # Drop duplicates keep first (some subjects may be in more than one subejct type)
+        df_ages = df_ages[~df_ages.index.duplicated(keep='first')]
+
+        # Add age information
+        df_ages = pd.concat([self.df_features['age'], df_ages], axis=1)
+
+        # Handle NaNs
+        df_ages = df_ages.fillna("")
+
+        # Save dataframe to csv
+        filename = "predicted_age" + self.naming + ".csv"
+        df_ages.to_csv(os.path.join(self.command_dir, filename))
+
+    def factors_vs_deltas(self, dict_ages, df_factors, tag, covars=None, beta=None,
+                          significance=0.05):
         """Calculate correlations between factors and deltas.
 
         Parameters
         ----------
-        dfs_ages: list of dataframes with delta information; shape=(n,m)
-        dfs_factors: list of dataframes with factor information; shape=(n,m)
-        groups: list of labels for each dataframe; shape=(n,),
-        factor_names: list of factor names; shape=(m,)
+        dict_ages: dictionary for each system with deltas; shape=(n,m)
+        df_factors: dataframe with factor information; shape=(n,m)
         significance: significance level for correlation"""
 
         # Select age information
         print("-----------------------------------")
-        print("Correlations between lifestyle factors by group")
+        print("Correlations between lifestyle factors for %s" % tag.group)
         print("significance: %.2g * -> FDR, ** -> bonferroni" % significance)
 
-        # Iterate over groups
+        # Iterate over systems
         corrs, significants = [], []
-        for group, df_ages, df_factors in zip(groups, dfs_ages, dfs_factors):
-            print(group)
+
+        # Facotr information
+        factors = df_factors.to_numpy()
+        factor_names = df_factors.columns.to_list()
+
+        # Applyc covariate correction
+        if self.flags["covariates"]:
+            factors, _ = covariate_correction(factors, covars, beta)
+
+        for system, df in dict_ages.items():
+            print(f"System: {system}")
 
             # Select data to visualize
-            deltas = df_ages["delta"].to_numpy()
-            factors = df_factors.to_numpy()
+            deltas = df['delta_%s' % system].to_numpy()
 
             # Calculate correlation between features and age
             corr, order, p_values = find_correlations(factors, deltas)
             corrs.append(corr)
 
             # Reject null hypothesis of no correlation
             reject_bon, _, _, _ = multipletests(p_values, alpha=significance, method='bonferroni')
             reject_fdr, _, _, _ = multipletests(p_values, alpha=significance, method='fdr_bh')
             significant = significant_markers(reject_bon, reject_fdr)
             significants.append(significant)
 
             # Print results
             for i, o in enumerate(order):
-                print("%d. %s %s: %.2f" % (i + 1, significant[o], factor_names[o], corr[o]))
+                print("%d. %s %s: %.2f (%.2g)" % (i + 1, significant[o], factor_names[o], corr[o], p_values[o]))
 
         # Use visualizer to show bar graph
-        self.visualizer.factors_vs_deltas(corrs, groups, factor_names, significants)
+        self.visualizer.factors_vs_deltas(corrs, list(dict_ages.keys()), factor_names, significants, tag)
 
-    def deltas_by_group(self, df, labels):
+    def deltas_by_group(self, dfs, tag, significance: float = 0.05):
         """Calculate summary metrics of deltas by group.
         
         Parameters
         ----------
         df: list of dataframes with delta information; shape=(n,m)
-        labels: list of labels for each dataframe; shape=(n,)"""
+        labels: list of labels for each dataframe; shape=(n,)
+        system: name of the system from which the variables come from"""
 
         # Select age information
         print("-----------------------------------")
-        print("Delta distribution by group")
+        print("Delta distribution for System:%s" % tag.system)
+
+        # Apply covariate correction
+        if self.flags["covariates"]:
+            df_cn = dfs['cn']
+            cn_idx = df_cn.index
+            covars = self.df_covariates.loc[cn_idx].to_numpy()
+            deltas = df_cn["delta_%s" % tag.system].to_numpy()
+            _, beta = covariate_correction(deltas, covars)
 
         # Obtain deltas means and stds
         deltas = []
-        for i, df_group in enumerate(df):
-            deltas.append(df_group["delta"].to_numpy())
-            print(labels[i])
-            print("Mean delta: %.2f" % np.mean(deltas[i]))
-            print("Std delta: %.2f" % np.std(deltas[i]))
-            print("Delta range: [%d, %d]" % (np.min(deltas[i]), np.max(deltas[i])))
+        for group, df in dfs.items():
+            vals = df["delta_%s" % tag.system].to_numpy()
+            # Apply covariate correction
+            if self.flags["covariates"]:
+                covars = self.df_covariates.loc[df.index].to_numpy()
+                vals, _ = covariate_correction(vals, covars, beta)
+            deltas.append(vals)
+            print(f"[Group: {group}]")
+            print("Mean delta: %.2f" % np.mean(vals))
+            print("Std delta: %.2f" % np.std(vals))
+            print("Delta range: [%d, %d]" % (np.min(vals), np.max(vals)))
 
         # Obtain statistically significant difference between deltas
         print("Checking for statistically significant differences between deltas...")
-        print("*: p-value < 0.01, **: p-value < 0.001")
+        print("significance: %.2g * -> FDR, ** -> bonferroni" % significance)
+
+        # Calculate p-values
+        p_vals_matrix = np.zeros((len(deltas), len(deltas)))
         for i in range(len(deltas)):
             for j in range(i + 1, len(deltas)):
                 _, p_val = stats.ttest_ind(deltas[i], deltas[j])
+                p_vals_matrix[i, j] = p_val
+        
+        # Reject null hypothesis of no correlation
+        reject_bon, _, _, _ = multipletests(p_vals_matrix.flatten(), alpha=significance, method='bonferroni')
+        reject_fdr, _, _, _ = multipletests(p_vals_matrix.flatten(), alpha=significance, method='fdr_bh')
+        reject_bon = reject_bon.reshape((len(deltas), len(deltas)))
+        reject_fdr = reject_fdr.reshape((len(deltas), len(deltas)))
+
+        # Print results
+        labels = list(dfs.keys())
+        for i in range(len(deltas)):
+            significant = significant_markers(reject_bon[i], reject_fdr[i])
+            for j in range(i + 1, len(deltas)):
                 pval_message = "p-value between %s and %s: %.2g" % (
-                    labels[i],
-                    labels[j],
-                    p_val,
-                )
-                if p_val < 0.001:
-                    pval_message = "*" + pval_message
-                elif p_val < 0.01:
-                    pval_message = "**" + pval_message
+                    labels[i], labels[j], p_vals_matrix[i, j])
+                if significant[j] != "":
+                    pval_message = significant[j] + " " + pval_message
                 print(pval_message)
 
         # Use visualizer
-        self.visualizer.deltas_by_groups(deltas, labels)
+        self.visualizer.deltas_by_groups(deltas, labels, tag)
 
-    def classify(self, df1, df2, groups):
+    def classify(self, df1, df2, groups, tag, beta: np.ndarray = None):
         """Classify two groups based on deltas.
 
         Parameters
         ----------
         df1: dataframe with delta information; shape=(n,m)
         df2: dataframe with delta information; shape=(n,m)
-        groups: list of labels for each dataframe; shape=(2,)"""
+        groups: list of labels for each dataframe; shape=(2,)
+        system: name of the system from which the variables come from
+        beta: coefficients for covariate correction"""
 
         # Classification
         print("-----------------------------------")
-        print("Classification between groups %s and %s" % (groups[0], groups[1]))
+        print(f"Classification between groups {groups[0]} and {groups[1]} [System: {tag.system}]")
 
         # Select delta information
-        deltas1 = df1["delta"].to_numpy()
-        deltas2 = df2["delta"].to_numpy()
+        delta_cols = [col for col in df1.columns if "delta" in col]
+        deltas1 = df1[delta_cols].to_numpy()
+        deltas2 = df2[delta_cols].to_numpy()
+
+        # Covariate correction
+        if self.flags["covariates"]:
+            df_cn = self.df_ages[self.df_clinical['cn']]
+            covars = self.df_covariates.loc[df_cn.index].to_numpy()
+            deltas_cn = df_cn[delta_cols].to_numpy()
+            _, beta = covariate_correction(deltas_cn, covars)
+            covars1 = self.df_covariates.loc[df1.index].to_numpy()
+            covars2 = self.df_covariates.loc[df2.index].to_numpy()
+            deltas1, _ = covariate_correction(deltas1, covars1, beta)
+            deltas2, _ = covariate_correction(deltas2, covars2, beta)
 
         # Create X and y for classification
-        X = np.concatenate((deltas1, deltas2)).reshape(-1, 1)
-        y = np.concatenate((np.zeros(deltas1.shape), np.ones(deltas2.shape)))
+        if len(delta_cols) == 1:
+            X = np.concatenate((deltas1, deltas2)).reshape(-1, 1)
+            y = np.concatenate((np.zeros(deltas1.shape), np.ones(deltas2.shape)))
+        else:
+            X = np.concatenate((deltas1, deltas2))
+            y = np.concatenate((np.zeros(deltas1.shape[0]), np.ones(deltas2.shape[0])))
+
+        # Throw error if we do not have enough controls for modelling
+        if X.shape[0] / self.args.classifier_cv_split < 2:
+            raise ValueError("Not enough subjects for classification for each CV split.")
+
+        # Generate classifier
+        self.classifier = self.generate_classifier()
+
+        # Apply covariate correction
+        if self.flags["covariates"]:
+            Z = np.concatenate((self.df_covariates.loc[df1.index].to_numpy(), self.df_covariates.loc[df2.index].to_numpy()))
+            X, _ = covariate_correction(X, Z, beta)
 
         # Calculate classification
         y_pred = self.classifier.fit_model(X, y)
 
+        # Print regressor weights
+        if len(delta_cols) > 1:
+            print("Logistic regressor weigths coef (norm_coef):")
+            coefs = self.classifier.model.coef_[0]
+            max_coef = np.max(np.abs(coefs))
+            for coef, delta in zip(coefs, delta_cols):
+                print(f"{delta} = {coef:.3f} ({np.abs(coef)/max_coef:.3f})")
+
         # Visualize AUC
-        self.visualizer.classification_auc(y, y_pred, groups)
+        self.visualizer.classification_auc(y, y_pred, groups, tag)
 
     @log
     def run_wrapper(self, run):
         """Wrapper for running modelling with log."""
         run()
 
     def run_age(self):
-        """Run basic age modelling."""
+        """Run age modelling."""
 
         # Run age modelling
         print("Running age modelling...")
 
+        # Set up directory
+        self.command_setup('model_age')
+
         # Load data
         self.load_data(required=["features"])
 
-        # Select controls
-        if self.flags["clinical"]:
-            df_cn = self.df_features.loc[self.df_features.index.isin(self.cn_subjects)]
-            df_clinical = self.df_features.loc[~self.df_features.index.isin(self.cn_subjects)]
-        else:
-            df_cn = self.df_features
-            df_clinical = None
-
-        if self.flags["covariates"] and self.args.covar_name is not None:
-            # Check that covariate column exists
-            if self.args.covar_name not in self.df_covariates.columns:
-                raise KeyError("Covariate column %s not found in covariates file." % self.args.covar_name)
+        # Initialized dictionaries
+        self.set_dict()
 
-            # Create dataframe list of controls by covariate
-            labels_covar = pd.unique(self.df_covariates[self.args.covar_name]).tolist()
-            df_covar_cn = self.df_covariates.loc[df_cn.index]
-            dfs_cn = []
-            for label_covar in labels_covar:
-                dfs_cn.append(df_cn[df_covar_cn[self.args.covar_name] == label_covar])
-
-            if self.flags["clinical"]:
-                # Create dataframe list of clinical cases by covariate
-                df_clinical_cov = []
-                for label_covar in labels_covar:
-                    df_covar_clinical = self.df_covar.loc[df_clinical.index]
-                    df_clinical_cov.append(df_clinical[df_covar_clinical[self.args.covar_name] == label_covar])
-
-        else:  # No covariates, so df list of controls is [df_cn] and [df_clinical]
-            dfs_cn = [df_cn]
-            dfs_clinical = [df_clinical]
-            labels_covar = ["all"]
-            self.args.covar_name = "all"
+        # Set dataframes
+        self.set_features_dataframes()
 
-        # Relationship between features and age
-        if self.flags["covariates"]:
-            initial_plots_names = f"controls_{self.args.covar_name}"
-        else:
-            initial_plots_names = "controls"
-            
-        # Use visualizer to show age distribution
-        self.age_distribution(dfs_cn, labels=labels_covar, name=initial_plots_names)
-    
-        self.features_vs_age(dfs_cn, labels=labels_covar, name=initial_plots_names)
-        
-        # Model age
-        self.models = {}
-        dfs_ages = {}
-        for label_covar, df_cn in zip(labels_covar, dfs_cn):
-            model_name = f"{self.args.covar_name}_{label_covar}"
-            self.models[model_name], dfs_ages[model_name] = self.model_age(df_cn, self.ageml, label_covar)
-            df_ages_cn = pd.concat(dfs_ages.values(), axis=0)
-
-        # NOTE: Matching dataframes that cannot be indexed by their name and models could be dangerous and prone to mismatches.
-        # TODO: Discuss about alternatives. Use dicts for all dataframes and models?
-
-        # Apply to clinical data
-        dfs_predicted_ages = {}
-        if self.flags["clinical"]:
-            for df_age_clinical, label_covar in zip(dfs_clinical, labels_covar):
-                model_name = f"{self.args.covar_name}_{label_covar}"
-                dfs_predicted_ages[model_name] = self.predict_age(df_age_clinical, self.models[model_name])
-            # Concatenate all the predicted ages
-            self.df_ages = pd.concat([dfs_predicted_ages.values()])
-        else:
-            self.df_ages = df_ages_cn
+        # Use visualizer to show age distribution of controls per covariate (all systems share the age distribution)
+        cn_ages = {covar: self.dfs['cn'][covar][self.systems[0]]['age'].to_list() for covar in self.covars}
+        self.age_distribution(cn_ages, name="Controls")
 
-        # Save dataframe
-        if self.flags["covariates"]:
-            filename = f"predicted_age_{self.args.covar_name}.csv"
-        else:
-            filename = "predicted_age.csv"
-        self.df_ages.to_csv(os.path.join(self.dir_path, filename))
+        # Show features vs age for controls for each system
+        for system in self.systems:
+            cn_features = {covar: self.dfs['cn'][covar][system] for covar in self.covars}
+            self.features_vs_age(cn_features, tag=NameTag(system=system))
 
-    def run_lifestyle(self):
-        """Run age modelling with lifestyle factors."""
+        # Model age for each system on controls
+        self.model_all()
 
-        print("Running lifestyle factors...")
+        # Predict to all other subject types
+        self.predict_all()
 
-        # Load data
-        self.load_data(required=["factors"])
+        # Save prediction
+        self.save_predictions()
+
+    def run_factor_correlation(self):
+        """Run factor correlation analysis between deltas and factors."""
+
+        print("Running factors correlation analysis...")
 
-        # Run age if not ages found
-        if self.df_ages is None:
-            print("No age data detected...")
-            print("-----------------------------------")
-            self.run_age()
-            print("-----------------------------------")
-            print("Resuming lifestyle factors...")
-
-        if self.flags["clinical"]:
-            groups = self.df_clinical.columns.to_list()
-            dfs_ages, dfs_factors = [], []
-            for g in groups:
-                dfs_ages.append(self.df_ages.loc[self.df_clinical[g]])
-                dfs_factors.append(self.df_factors.loc[self.df_clinical[g]])
-        else:
-            dfs_ages = [self.df_ages]
-            dfs_factors = [self.df_factors]
-            groups = ["all"]
+        # Set up
+        self.command_setup('factor_correlation')
 
-        # Calculate correlations between factors and deltas
-        self.factors_vs_deltas(dfs_ages, dfs_factors, groups, self.df_factors.columns.to_list())
+        # Load data
+        self.load_data(required=["ages", "factors"])
+
+        # Calculate covariate correction for factors
+        if self.flags["covariates"]:
+            print("Applying covariate correction for factors...")
+            factors = self.df_factors.loc[self.df_clinical['cn']].to_numpy()
+            covars = self.df_covariates.loc[self.df_clinical['cn']].to_numpy()
+            _, beta = covariate_correction(factors, covars)
+
+        # For each subject type and system run correlation analysis
+        for subject_type in self.subject_types:
+            tag = NameTag(group=subject_type)
+            dfs_systems = {}
+            df_sub = self.df_ages.loc[self.df_clinical[subject_type]]
+            df_factors = self.df_factors.loc[df_sub.index]
+            for system in self.systems:
+                df_sys = df_sub[[col for col in df_sub.columns if system in col]]
+                dfs_systems[system] = df_sys
+            if self.flags["covariates"]:
+                covars = self.df_covariates.loc[df_sub.index].to_numpy()
+                self.factors_vs_deltas(dfs_systems, df_factors, tag, covars, beta)
+            else:
+                self.factors_vs_deltas(dfs_systems, df_factors, tag)
 
     def run_clinical(self):
-        """Run age modelling with clinical factors."""
+        """Analyse differences between deltas in clinical groups."""
 
         print("Running clinical outcomes...")
 
-        # Load data
-        self.load_data(required=["clinical"])
-
-        # Run age if not ages found
-        if self.df_ages is None:
-            print("No age data detected...")
-            print("-----------------------------------")
-            self.run_age()
-            print("-----------------------------------")
-            print("Resuming clinical outcomes...")
-
-        # Obtain dataframes for each clinical group
-        groups = self.df_clinical.columns.to_list()
-        group_ages = []
-        for g in groups:
-            group_ages.append(self.df_ages.loc[self.df_clinical[g]])
+        # Set up
+        self.command_setup('clinical_groups')
 
-        # Use visualizer to show age distribution
-        self.age_distribution(group_ages, groups, name="clinical_groups")
+        # Load data
+        self.load_data(required=["ages", "clinical"])
 
-        # Use visualizer to show box plots of deltas by group
-        self.deltas_by_group(group_ages, groups)
+        # Obtain dataframes for each group
+        dfs = {g: self.df_ages.loc[self.df_clinical[g]] for g in self.subject_types}
+    
+        # Use visualizer to show age distribution per clinical group
+        ages = {g: dfs[g].iloc[:, 0].to_list() for g in self.subject_types}
+        self.age_distribution(ages, name="Clinical Groups")
+
+        # Show differences in groups per system
+        for system in self.systems:
+            dfs_systems = {g: dfs[g][[col for col in dfs[g].columns if system in col]] for g in self.subject_types}
+            self.deltas_by_group(dfs_systems, tag=NameTag(system=system))
 
     def run_classification(self):
         """Run classification between two different clinical groups."""
 
         print("Running classification...")
 
-        # Load data
-        self.load_data(required=["clinical"])
+        # Set up
+        self.command_setup('clinical_classify')
 
-        # Run age if not ages found
-        if self.df_ages is None:
-            print("No age data detected...")
-            print("-----------------------------------")
-            self.run_age()
-            print("-----------------------------------")
-            print("Resuming clinical outcomes...")
+        # Load data
+        self.load_data(required=["ages", "clinical"])
 
-        # Check that arguments given for each group
+        # Check that arguments given for each group and that they exist
         if self.args.group1 is None or self.args.group2 is None:
             raise ValueError("Must provide two groups to classify.")
-        
-        # Check that those groups exist
-        groups = [self.args.group1.lower(), self.args.group2.lower()]
-        if groups[0] not in self.df_clinical.columns or groups[1] not in self.df_clinical.columns:
+        elif self.args.group1 not in self.df_clinical.columns or self.args.group2 not in self.df_clinical.columns:
             raise ValueError("Classes must be one of the following: %s" % self.df_clinical.columns.to_list())
-
-        # Obtain dataframes for each clinical group
-        df_group1 = self.df_ages.loc[self.df_clinical[groups[0]]]
-        df_group2 = self.df_ages.loc[self.df_clinical[groups[1]]]
-
-        # Classify between groups
-        self.classify(df_group1, df_group2, groups)
-
-
-class CLI(Interface):
-
-    """Read and parses user commands via command line.
-
-    Public methods:
-    ---------------
-    configure_parser(self): Configure parser with required arguments for processing.
-
-    configure_args(self, args): Configure argumens with required fromatting for modelling.
-    """
-
-    def __init__(self):
-        """Initialise variables."""
-        self.parser = argparse.ArgumentParser(
-            description="Age Modelling using python.",
-            formatter_class=argparse.RawTextHelpFormatter,
-        )
-        self.configure_parser()
-        args = self.parser.parse_args()
-        args = self.configure_args(args)
-
-        # Initialise parent class
-        super().__init__(args)
-
-        # Run modelling
-        case = args.run
-        if case == "age":
-            self.run = self.run_age
-        elif case == "lifestyle":
-            self.run = self.run_lifestyle
-        elif case == "clinical":
-            self.run = self.run_clinical
-        elif case == "classification":
-            self.run = self.run_classification
-        else:
-            raise ValueError(
-                "Choose a valid run type: age, lifestyle, clinical, classification"
-            )
-
-        self.run_wrapper(self.run)
-
-    def configure_parser(self):
-        """Configure parser with required arguments for processing."""
-        self.parser.add_argument(
-            "-r",
-            "--run",
-            metavar="RUN",
-            default="age",
-            required=True,
-            help=messages.run_long_description,
-        )
-        self.parser.add_argument(
-            "-o",
-            "--output",
-            metavar="DIR",
-            required=True,
-            help=messages.output_long_description,
-        )
-        self.parser.add_argument(
-            "-f", "--features", metavar="FILE", help=messages.features_long_description
-        )
-        self.parser.add_argument(
-            "-m",
-            "--model",
-            nargs="*",
-            default=["linear"],
-            help=messages.model_long_description,
-        )
-        self.parser.add_argument(
-            "-s",
-            "--scaler",
-            nargs="*",
-            default=["standard"],
-            help=messages.scaler_long_description,
-        )
-        self.parser.add_argument(
-            "--cv",
-            nargs="+",
-            type=int,
-            default=[5, 0],
-            help=messages.cv_long_description,
-        )
-        self.parser.add_argument(
-            "--covariates", metavar="FILE", help=messages.covar_long_description
-        )
-        self.parser.add_argument(
-            "--covar_name", metavar="COVAR_NAME", help=messages.covar_name_long_description
-        )
-        self.parser.add_argument(
-            "--factors", metavar="FILE", help=messages.factors_long_description
-        )
-        self.parser.add_argument(
-            "--clinical", metavar="FILE", help=messages.clinical_long_description
-        )
-        self.parser.add_argument(
-            "--systems", metavar="FILE", help=messages.systems_long_description
-        )
-        self.parser.add_argument(
-            "--ages", metavar="FILE", help=messages.ages_long_description
-        )
-        self.parser.add_argument(
-            "--groups", metavar="GROUP", nargs=2, help=messages.groups_long_description
-        )
-
-    def configure_args(self, args):
-        """Configure argumens with required fromatting for modelling.
-
-        Parameters
-        ----------
-        args: arguments object from parser
-        """
-
-        # Set CV params first item is the number of CV splits
-        if len(args.cv) == 1:
-            args.cv_split = args.cv[0]
-            args.seed = self.parser.get_default("cv")[1]
-        elif len(args.cv) == 2:
-            args.cv_split, args.seed = args.cv
-        else:
-            raise ValueError("Too many values to unpack")
-
-        # Set Scaler parameters first item is the scaler type
-        # The rest of the arguments conform a dictionary for **kwargs
-        args.scaler_type = args.scaler[0]
-        if len(args.scaler) > 1:
-            scaler_params = {}
-            for item in args.scaler[1:]:
-                # Check that item has one = to split
-                if item.count("=") != 1:
-                    raise ValueError(
-                        "Scaler parameters must be in the format param1=value1 param2=value2 ..."
-                    )
-                key, value = item.split("=")
-                value = convert(value)
-                scaler_params[key] = value
-            args.scaler_params = scaler_params
         else:
-            args.scaler_params = {}
+            df_group1 = self.df_ages[self.df_clinical[self.args.group1]]
+            df_group2 = self.df_ages[self.df_clinical[self.args.group2]]
 
-        # Set Model parameters first item is the model type
-        # The rest of the arguments conform a dictionary for **kwargs
-        args.model_type = args.model[0]
-        if len(args.model) > 1:
-            model_params = {}
-            for item in args.model[1:]:
-                # Check that item has one = to split
-                if item.count("=") != 1:
-                    raise ValueError(
-                        "Model parameters must be in the format param1=value1 param2=value2 ..."
-                    )
-                key, value = item.split("=")
-                value = convert(value)
-                model_params[key] = value
-            args.model_params = model_params
-        else:
-            args.model_params = {}
-
-        # Set groups
-        if args.groups is not None:
-            args.group1, args.group2 = args.groups
-        else:
-            args.group1, args.group2 = None, None
-
-        return args
+        # Create a classifier for each system
+        for system in self.systems:
+            df_group1_system = df_group1[[col for col in df_group1.columns if system in col]]
+            df_group2_system = df_group2[[col for col in df_group2.columns if system in col]]
+            self.classify(df_group1_system, df_group2_system, [self.args.group1, self.args.group2], tag=NameTag(system=system))
+        
+        # Create a classifier for all systems
+        if len(self.systems) > 1:
+            self.classify(df_group1, df_group2, [self.args.group1, self.args.group2], tag=NameTag(system="all"))
 
 
-class InteractiveCLI(Interface):
+class CLI(Interface):
 
     """Read and parses user commands via command line via an interactive interface
 
     Public methods:
     ---------------
 
     initial_command(self): Ask for initial inputs for initial setup.
 
     get_line(self): Prints a prompt for the user and updates the user entry.
 
-    force_command(self, func, command = None): Force the user to enter a valid command.
+    force_command(self, flag="", command = None): Force the user to enter a valid command.
 
     command_interface(self): Reads in the commands and calls the corresponding
                              functions.
 
+    classification_command(self): Runs classification.
+
+    clinical_command(self): Runs clinical analysis.
+
+    covar_command(self): Loads covariate group.
+
     cv_command(self): Loads CV parameters.
 
+    factor_correlation_command(self): Runs factor correlation analysis.
+
+    group_command(self): Loads groups.
+
     help_command(self): Prints a list of valid commands.
 
     load_command(self): Loads file paths.
 
     model_command(self): Loads model parameters.
 
-    output_command(self): Loads output directory.
+    model_age_command(self): Runs age modelling.
 
-    run_command(self): Runs the modelling.
+    output_command(self): Loads output directory.
 
     scaler_command(self): Loads scaler parameters.
     """
 
     def __init__(self):
         """Initialise variables."""
 
@@ -951,167 +1213,298 @@
         self.command_interface()
 
     def initial_command(self):
         """Ask for initial inputs for initial setup."""
 
         # Askf for output directory
         print("Output directory path (Required):")
-        self.force_command(self.output_command, "o", required=True)
-        # Ask for input files
-        print("Input features file path (Required for run age):")
-        self.force_command(self.load_command, "l --features")
-        print("Input covariates file path (Optional):")
-        self.force_command(self.load_command, "l --covariates")
-        print("Input factors file path (Reqruired for run lifestyle):")
-        self.force_command(self.load_command, "l --factors")
-        print(
-            "Input clinical file path (Required for run clinical or run classification):"
-        )
-        self.force_command(self.load_command, "l --clinical")
-        print("Input systems file path (Optional):")
-        self.force_command(self.load_command, "l --systems")
-        print("Input ages file path (Optional):")
-        self.force_command(self.load_command, "l --ages")
-
-        # Ask for scaler, model and CV parameters
-        print("Scaler type and parameters (Default:standard):")
-        self.force_command(self.scaler_command, "s")
-        print("Model type and parameters (Default:linear):")
-        self.force_command(self.model_command, "m")
-        print("CV parameters (Default: nº splits=5 and seed=0):")
-        self.force_command(self.cv_command, "cv")
+        self.force_command(self.output_command, required=True)
 
     def get_line(self, required=True):
         """Print prompt for the user and update the user entry."""
         self.line = input("#: ")
         while self.line == "" and required:
             print("Must provide a value.")
             self.line = input("#: ")
 
-    def force_command(self, func, command, required=False):
+    def force_command(self, func, flag="", required=False):
         """Force the user to enter a valid command."""
         while True:
             self.get_line(required=required)
             if self.line == "":
                 self.line = "None"
-            self.line = command + " " + self.line
+            self.line = flag + " " + self.line
             error = func()
             if error is None:
                 return None
             else:
                 print(error)
 
+    def reset_args(self):
+        """Reset arguments to None except output directory."""
+
+        for attr_name in vars(self.args):
+            if attr_name != 'output':
+                setattr(self.args, attr_name, None)
+
     def command_interface(self):
         """Read the command entered and call the corresponding function."""
 
         # Interactive mode after setup
         print("Enter 'h' for help.")
         self.get_line()  # get the user entry
         command = self.line.split()[0]  # read the first item
         while command != "q":
+            # Reset arguments
+            self.reset_args()
+
+            # Run command
             error = None
-            if command == "cv":
-                error = self.cv_command()
+            if command == "classification":
+                error = self.classification_command()
+            elif command == "clinical":
+                error = self.clinical_command()
+            elif command == "factor_correlation":
+                error = self.factor_correlation_command()
+            elif command == "model_age":
+                error = self.model_age_command()
             elif command == "h":
                 self.help_command()
-            elif command == "l":
-                error = self.load_command()
-            elif command == "m":
-                error = self.model_command()
-            elif command == "o":
-                error = self.output_command()
-            elif command == "r":
-                error = self.run_command()
-            elif command == "s":
-                error = self.scaler_command()
             else:
                 print("Invalid command. Enter 'h' for help.")
 
             # Check error and if not make updates
             if error is not None:
                 print(error)
-            elif command == "r":
-                # Capture any error raised and print
-                try:
-                    self.run_wrapper(self.run)
-                except Exception as e:
-                    print(e)
-                    print("Error running modelling.")
-            elif command == "o":
-                try:
-                    self.setup()
-                    self.set_visualizer()
-                except Exception as e:
-                    print(e)
-                    print("Error setting up output directory.")
-            elif command in ["cv", "m", "s"]:
-                try:
-                    self.set_model()
-                except Exception as e:
-                    print(e)
-                    print("Error setting up model.")
 
             # Get next command
             self.get_line()  # get the user entry
             command = self.line.split()[0]  # read the first item
 
+    def classifier_command(self):
+        """Set classifier parameters."""
+
+        # Split into items
+        self.line = self.line.split()
+        error = None
+
+        # Check that at least one argument input
+        if len(self.line) == 0:
+            error = "Must provide two arguments or None."
+            return error
+        
+        # Set defaults
+        if len(self.line) == 1 and self.line[0] == 'None':
+            self.args.classifier_thr = 0.5
+            self.args.classifier_ci = 0.95
+            return error
+        
+        # Check wether items are floats
+        for item in self.line:
+            try:
+                float(item)
+            except ValueError:
+                error = "Parameters must be floats."
+                return error
+            
+        # Set parameters
+        if len(self.line) == 2:
+            self.args.classifier_thr = float(self.line[0])
+            self.args.classifier_ci = float(self.line[1])
+        elif len(self.line) > 2:
+            error = "Too many values to unpack."
+        elif len(self.line) == 1:
+            error = "Must provide two arguments or None."
+        
+        return error
+            
+    def classification_command(self):
+        """Run classification."""
+
+        error = None
+
+        # Ask for input files
+        print("Input ages file path (Required):")
+        self.force_command(self.load_command, "--ages", required=True)
+        print("Input clinical file path (Required):")
+        self.force_command(self.load_command, "--clinical", required=True)
+
+        # Ask for groups
+        print("Input groups (Required):")
+        self.force_command(self.group_command, required=True)
+
+        # Ask for optional
+        print("Input covariates file path (Optional):")
+        self.force_command(self.load_command, "--covariates")
+
+        # Ask for CV parameters adn classifier parameters
+        print("CV parameters (Default: nº splits=5 and seed=0):")
+        self.force_command(self.cv_command, 'classifier')
+        print("Classifier parameters (Default: thr=0.5 and ci=0.95):")
+        self.force_command(self.classifier_command)
+
+        # Run classification capture any error raised and print
+        try:
+            self.run_wrapper(self.run_classification)
+            print("Finished classification.")
+        except Exception as e:
+            print(e)
+            error = "Error running classification."
+        
+        return error
+
+    def clinical_command(self):
+        """Run clinical analysis."""
+
+        error = None
+
+        # Ask for input files
+        print("Input ages file path (Required):")
+        self.force_command(self.load_command, "--ages", required=True)
+        print("Input clinical file path (Required):")
+        self.force_command(self.load_command, "--clinical", required=True)
+
+        # Ask for optional
+        print("Input covariates file path (Optional):")
+        self.force_command(self.load_command, "--covariates")
+
+        # Run clinical analysis capture any error raised and print
+        try:
+            self.run_wrapper(self.run_clinical)
+            print("Finished clinical analysis.")
+        except Exception as e:
+            print(e)
+            error = "Error running clinical analysis."
+        
+        return error
+
+    def covar_command(self):
+        """Load covariate group."""
+
+        # Split into items
+        self.line = self.line.split()
+        error = None
+
+        # Check that one argument given
+        if len(self.line) != 1:
+            error = "Must provide one covariate name."
+            return error
+
+        # Set covariate name
+        if self.line[0] == "None":
+            pass
+        else:
+            self.args.covar_name = self.line[0]
+
+        return error
+
     def cv_command(self):
         """Load CV parameters."""
 
-        # Split into items and remove  command
-        self.line = self.line.split()[1:]
+        # Split into items
+        self.line = self.line.split()
         error = None
 
         # Check that at least one argument input
         if len(self.line) == 0:
-            error = "Must provide at least one argument or None."
+            error = "Must provide at least one argument."
+            return error
+
+        # Check that first argument is model or classifier
+        if self.line[0] not in ['model', 'classifier']:
+            error = "Must provide either model or classifier flag."
             return error
+        elif self.line[0] == 'model':
+            arg_type = 'model'
+        elif self.line[0] == 'classifier':
+            arg_type = 'classifier'
 
         # Set default values
-        if self.line[0] == "None":
-            self.args.cv_split = 5
-            self.args.seed = 0
+        if len(self.line) == 2 and self.line[1] == 'None':
+            setattr(self.args, arg_type + '_cv_split', 5)
+            setattr(self.args, arg_type + '_seed', 0)
             return error
 
         # Check wether items are integers
-        for item in self.line:
+        for item in self.line[1:]:
             if not item.isdigit():
                 error = "CV parameters must be integers"
                 return error
 
         # Set CV parameters
-        if len(self.line) == 1:
-            self.args.cv_split = int(self.line[0])
-            self.args.seed = 0
-        elif len(self.line) == 2:
-            self.args.cv_split, self.args.seed = int(self.line[0]), int(self.line[1])
+        if len(self.line) == 2:
+            setattr(self.args, arg_type + '_cv_split', int(self.line[1]))
+            setattr(self.args, arg_type + '_seed', 0)
+        elif len(self.line) == 3:
+            setattr(self.args, arg_type + '_cv_split', int(self.line[1]))
+            setattr(self.args, arg_type + '_seed', int(self.line[2]))
         else:
             error = "Too many values to unpack."
 
         return error
 
+    def factor_correlation_command(self):
+        """Run factor correlation analysis."""
+
+        error = None
+
+        # Ask for input files
+        print("Input ages file path (Required):")
+        self.force_command(self.load_command, "--ages", required=True)
+        print("Input factors file path (Required):")
+        self.force_command(self.load_command, "--factors", required=True)
+        print("Input clinical file path (Optional):")
+        self.force_command(self.load_command, "--clinical")
+        print("Input covariates file path (Optional):")
+        self.force_command(self.load_command, "--covariates")
+
+        # Run factor correlation analysis capture any error raised and print
+        try:
+            self.run_wrapper(self.run_factor_correlation)
+            print("Finished factor correlation analysis.")
+        except Exception as e:
+            print(e)
+            error = "Error running factor correlation analysis."
+        
+        return error
+
+    def group_command(self):
+        """Load groups."""
+
+        # Split into items
+        self.line = self.line.split()
+        error = None
+
+        # Check that two groups are given
+        if len(self.line) != 2:
+            error = "Must provide two groups."
+            return error
+
+        # Set groups
+        self.args.group1, self.args.group2 = self.line[0], self.line[1]
+
+        return error
+
     def help_command(self):
-        """Print a list of valid commands."""
+        """Print a list of valid commmands."""
 
         # Print possible commands
         print("User commands:")
-        print(messages.cv_command_message)
-        print(messages.help_command_message)
-        print(messages.load_command_message)
-        print(messages.model_command_message)
-        print(messages.output_command_message)
+        print(messages.classification_command_message)
+        print(messages.clinical_command_message)
+        print(messages.factor_correlation_command_message)
+        print(messages.model_age_command_message)
         print(messages.quit_command_message)
-        print(messages.run_command_message)
-        print(messages.scaler_command_message)
+        print(messages.read_the_documentation_message)
 
     def load_command(self):
         """Load file paths."""
 
-        # Split into items and remove  command
-        self.line = self.line.split()[1:]
+        # Split into items
+        self.line = self.line.split()
         error = None
 
         # Determine if correct number of arguments and check file valid
         if len(self.line) > 2:
             error = "Too many arguments only two arguments --file_type and file path."
         elif len(self.line) == 1:
             error = "Must provide a file path or None when using --file_type."
@@ -1157,35 +1550,81 @@
         elif file_type == "--ages":
             self.args.ages = file
         else:
             error = "Choose a valid file type: --features, --covariates, --factors, --clinical, --systems, --ages"
 
         return error
 
+    def model_age_command(self):
+        """Run age modelling."""
+
+        error = None
+        
+        # Ask for input files
+        print("Input features file path (Required):")
+        self.force_command(self.load_command, "--features", required=True)
+        print("Input covariates file path (Optional):")
+        self.force_command(self.load_command, "--covariates")
+        print("Input covariate type to train separate models (Optional):")
+        self.force_command(self.covar_command)
+        print("Input clinical file path (Optional):")
+        self.force_command(self.load_command, "--clinical")
+        print("Input systems file path (Optional):")
+        self.force_command(self.load_command, "--systems")
+
+        # Ask for scaler, model, CV parameters, feature extension, and hyperparameter tuning
+        print("Scaler type and parameters (Default:standard)")
+        print(f"Available: {list(AgeML.scaler_dict.keys())}")
+        print("Example: standard with_mean=True with_std=False")
+        self.force_command(self.scaler_command)
+        print("Model type and parameters (Default:linear_reg)")
+        print(f"Available: {list(AgeML.model_dict.keys())}")
+        print("Example: linear_reg fit_intercept=True normalize=False")
+        self.force_command(self.model_command)
+        print("CV parameters (Default: nº splits=5 and seed=0):")
+        print("Example: 10 0")
+        self.force_command(self.cv_command, 'model')
+        print("Polynomial feature extension degree. Leave blank if not desired (Default: 0, max. 3)")
+        print("Example: 3")
+        self.force_command(self.feature_extension_command)
+        print("Hyperparameter tuning. Number of points in grid search: (Default: 0)")
+        print("Example: 100")
+        self.force_command(self.hyperparameter_grid_command)
+
+        # Run modelling capture any error raised and print
+        try:
+            self.run_wrapper(self.run_age)
+            print("Finished running age modelling.")
+        except Exception as e:
+            print(e)
+            error = "Error running age modelling."
+        
+        return error
+
     def model_command(self):
         """Load model parameters."""
 
-        # Split into items and remove  command
-        self.line = self.line.split()[1:]
-        valid_types = ["linear"]
+        # Split into items
+        self.line = self.line.split()
+        valid_types = list(AgeML.model_dict.keys())
         error = None
 
         # Check that at least one argument input
         if len(self.line) == 0:
             error = "Must provide at least one argument or None."
             return error
         else:
             model_type = self.line[0]
 
         # Set model type or default
         if model_type == "None":
-            self.args.model_type = "linear"
+            self.args.model_type = "linear_reg"
         else:
             if model_type not in valid_types:
-                error = "Choose a valid model type: {}".format(valid_types)
+                error = f"Choose a valid model type: {valid_types}"
             else:
                 self.args.model_type = model_type
 
         # Set model parameters
         if len(self.line) > 1 and model_type != "None":
             model_params = {}
             for item in self.line[1:]:
@@ -1196,21 +1635,27 @@
                 key, value = item.split("=")
                 value = convert(value)
                 model_params[key] = value
             self.args.model_params = model_params
         else:
             self.args.model_params = {}
 
+        # Try to set an instance of the specified scaler with the provided arguments
+        try:
+            AgeML.model_dict[self.args.model_type](**self.args.model_params)
+        except TypeError:  # Raised when invalid parameters are given to sklearn
+            error = f"Model parameters are not valid for {self.args.model_type} model. Check them in the sklearn documentation."
+
         return error
 
     def output_command(self):
         """Load output directory."""
 
-        # Split into items and remove  command
-        self.line = self.line.split()[1:]
+        # Split into items
+        self.line = self.line.split()
         error = None
 
         # Check wether there is a path
         if len(self.line) == 0:
             error = "Must provide a path."
             return error
 
@@ -1221,70 +1666,35 @@
         elif os.path.isdir(path):
             self.args.output = path
         else:
             error = "Directory %s does not exist." % path
 
         return error
 
-    def run_command(self):
-        """Run the modelling."""
-        error = None
-
-        # Split into items and remove  command
-        self.line = self.line.split()[1:]
-
-        # Check that at least one argument given
-        if len(self.line) < 1:
-            error = "Must provide at least one argument."
-            return error
-        elif len(self.line) > 1 and self.line[0] in ['age', 'lifestyle', 'clinical']:
-            error = "Too many arguments given for run type %s" % self.line[0]
-            return error
-        elif len(self.line) != 3 and self.line[0] in ['classification']:
-            error = "For run type %s two arguments should be given" % self.line[0]
-            return error
-
-        # Run specificed modelling
-        case = self.line[0]
-        if case == "age":
-            self.run = self.run_age
-        elif case == "lifestyle":
-            self.run = self.run_lifestyle
-        elif case == "clinical":
-            self.run = self.run_clinical
-        elif case == "classification":
-            self.run = self.run_classification
-            self.args.group1 = self.line[1]
-            self.args.group2 = self.line[2]
-        else:
-            error = "Choose a valid run type: age, lifestyle, clinical, classification"
-
-        return error
-
     def scaler_command(self):
         """Load scaler parameters."""
 
-        # Split into items and remove  command
-        self.line = self.line.split()[1:]
+        # Split into items
+        self.line = self.line.split()
         error = None
-        valid_types = ["standard"]
+        valid_types = list(AgeML.scaler_dict.keys())
 
         # Check that at least one argument input
         if len(self.line) == 0:
             error = "Must provide at least one argument or None."
             return error
         else:
             scaler_type = self.line[0]
 
         # Set scaler type or default
         if scaler_type == "None":
             self.args.scaler_type = "standard"
         else:
             if scaler_type not in valid_types:
-                error = "Choose a valid scaler type: {}".format(valid_types)
+                error = f"Choose a valid scaler type: {valid_types}"
             else:
                 self.args.scaler_type = scaler_type
 
         # Set scaler parameters
         if len(self.line) > 1 and scaler_type != "None":
             scaler_params = {}
             for item in self.line[1:]:
@@ -1294,8 +1704,67 @@
                 key, value = item.split("=")
                 value = convert(value)
                 scaler_params[key] = value
             self.args.scaler_params = scaler_params
         else:
             self.args.scaler_params = {}
 
+        # Try to set an instance of the specified scaler with the provided arguments
+        try:
+            AgeML.scaler_dict[self.args.scaler_type](**self.args.scaler_params)
+        except TypeError:
+            error = f"Scaler parameters are not valid for {self.args.scaler_type} scaler. Check them in the sklearn documentation."
+            return error
+
+        return error
+
+    def feature_extension_command(self):
+        """Load feature extension."""
+
+        # Split into items and remove  command
+        self.line = self.line.split()
+        error = None
+
+        # Check that at least one argument input
+        if len(self.line) > 1:
+            error = "Must provide only one integer, or none."
+            return error
+
+        # Set default values
+        if len(self.line) == 0 or self.line[0] == "None":
+            self.args.feature_extension = 0
+            return error
+        
+        # Check whether items are integers
+        if not self.line[0].isdigit():
+            error = "The polynomial feature extension degree must be an integer (0, 1, 2, or 3)"
+            return error
+
+        # Set CV parameters
+        self.args.feature_extension = int(self.line[0])
+        return error
+
+    def hyperparameter_grid_command(self):
+        """Load hyperparameter search grid."""
+
+        # Split into items and remove command
+        self.line = self.line.split()
+        error = None
+
+        # Check that at least one argument input
+        if len(self.line) > 1:
+            error = "Must provide only one integer, or none."
+            return error
+
+        # Set default values
+        if len(self.line) == 0 or self.line[0] == "None":
+            self.args.hyperparameter_tuning = 0
+            return error
+        
+        # Check whether items are integers
+        if not self.line[0].isdigit():
+            error = "The number of points in the hyperparameter grid must be a positive, nonzero integer."
+            return error
+
+        # Set CV parameters
+        self.args.hyperparameter_tuning = int(self.line[0])
         return error
```

### Comparing `ageml-0.0.1/src/ageml/utils.py` & `ageml-0.1.0/src/ageml/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,33 +65,50 @@
         elif fdr[i]:
             markers.append("*")
         else:
             markers.append("")
     return markers
 
 
+class Logger:
+    """Class to log stdout to log.txt."""
+
+    def __init__(self, instance):
+        self.terminal = sys.stdout
+        self.instance = instance
+
+    def write(self, message):
+        self.terminal.write(message)
+        with open(self.instance.log_path, "a") as f:
+            f.write(message)
+
+    def flush(self):
+        pass
+
+
 def log(func):
     """Decorator function to log stdout to log.txt."""
 
     def wrapper(instance, *args, **kwargs):
         # Redirect the standard output to capture print statements
         original_stdout = sys.stdout
-        captured_output = io.StringIO()
-        sys.stdout = captured_output
+        sys.stdout = Logger(instance)
 
         try:
             # Call the function
             result = func(instance, *args, **kwargs)
         finally:
             # Restore the original standard output
             sys.stdout = original_stdout
 
-        # Log the captured output to the file
-        with open(instance.log_path, "a") as log_file:
-            log_file.write(captured_output.getvalue())
-
-        # Print the captured output to the console
-        print("\n".join(captured_output.getvalue().split("\n")[:-1]))
-
         return result
 
     return wrapper
+
+
+class NameTag:
+    """Class to create unique names for objects."""
+
+    def __init__(self, group="", covar="", system=""):
+        self.group = group
+        self.covar = covar
+        self.system = system
```

### Comparing `ageml-0.0.1/src/ageml/visualizer.py` & `ageml-0.1.0/src/ageml/visualizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 Used in the AgeML project to enable the plotting of modelling results.
 
 Classes:
 --------
 Visualizer - manages the visualization of data and results.
 """
 
+import matplotlib; matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 import math
 import numpy as np
 import os
 
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import roc_curve, roc_auc_score
 
-from .utils import insert_newlines, create_directory
+from .utils import insert_newlines, create_directory, NameTag
 
 plt.rcParams.update({'font.size': 12})
 
 
 class Visualizer:
 
     """Manages the visualization of data and results.
@@ -72,24 +73,28 @@
         ----------
         Ys: list of np.arrays containing ages; shape=(m, n).
         labels: # TODO
         name: # TODO"""
 
         # Plot age distribution
         for Y in Ys:
-            plt.hist(Y, bins=20, alpha=1 / len(Ys))
+            plt.hist(Y, bins=20, alpha=1 / len(Ys), density=True)
         if labels is not None:
             plt.legend(labels)
         plt.xlabel("Age (years)")
         plt.ylabel("Count")
-        plt.savefig(os.path.join(self.path_for_fig, "age_distribution_%s.svg" % name))
+        plt.title("Age distribution")
+
+        # Save fig
+        filename = "age_distribution_" + name.lower().replace(" ", "_") + ".png"
+        plt.savefig(os.path.join(self.path_for_fig, filename))
         plt.close()
 
     def features_vs_age(self, X: list, Y: list, corr: list, order: list, markers,
-                        feature_names, labels: list = None, name: str = ""):
+                        feature_names, tag: NameTag = None, labels: list = None):
         """Plot correlation between features and age.
 
         Parameters
         ----------
         X: 2D-Array with features; shape=(n, m)
         Y: 1D-Array with age; shape=n
         corr: 1D-Array with correlation coefficients; shape=m
@@ -106,111 +111,114 @@
         elif len(Y) > 1:
             color_set = [self.cmap(unique_color) for unique_color in np.arange(len(Y))]
         else:  # If only one covariate, use the same color for all points
             color_set = [self.cmap(0)]
         # Color array for each covariate
         color_list = [len * [color_set[i]] for i, len in enumerate(covar_lens)]
 
-        if labels is None:
-            labels = ['population']
+        if labels == ["all"]:
+            labels = ["population"]
 
         # Show results
         nplots = len(feature_names)
         plt.figure(figsize=(14, 3 * math.ceil(nplots / 4)))
         
         for i, o in enumerate(order[0]):  # Default to order[0] because each covar may have different order
             plt.subplot(math.ceil(nplots / 4), 4, i + 1)
             ax = plt.gca()  # Get current axis
             for i in range(len(color_set)):
                 ax.scatter(Y[i][:], X[i][:, o],
-                           s=15, c=color_list[i], label=labels[i])
+                           s=15, c=color_list[i], label=labels[i], alpha=1 / len(labels))
             # Set axis labels, title, and legend
             ax.set_ylabel(insert_newlines(feature_names[o], 4))
             ax.set_xlabel("age (years)")
             title = "Correlation values:"
             for n, label in enumerate(labels):
                 title += "\n$\\rho_{%s}$: %s%.3f" % (label, markers[n][o], corr[n][o])
             ax.set_title(title)
             ax.legend(labels)
+            plt.suptitle(f"Features vs. Age\n{tag.system}", y=0.99)
         plt.tight_layout()
 
-        if name == "":
-            filename = "features_vs_age.svg"
-        else:
-            filename = f"features_vs_age_{name}.svg"
+        # Save file
+        filename = f"features_vs_age_controls{'_'+tag.system if tag.system != '' else ''}.png"
         plt.savefig(os.path.join(self.path_for_fig, filename))
         plt.close()
 
-    def true_vs_pred_age(self, y_true, y_pred, name: str = ""):
+    def true_vs_pred_age(self, y_true, y_pred, tag: NameTag):
         """Plot true age vs predicted age.
 
         Parameters
         ----------
         y_true: 1D-Array with true age; shape=n
         y_pred: 1D-Array with predicted age; shape=n."""
 
         # Find min and max age range to fit in graph
         age_range = np.arange(np.min([y_true, y_pred]), np.max([y_true, y_pred]))
 
         # Plot true vs predicted age
         plt.scatter(y_true, y_pred)
         plt.plot(age_range, age_range, color="k", linestyle="dashed")
-        plt.title(f"Chronological vs Predicted Age {name}")
+        plt.title(f"Chronological vs Predicted Age \n [Covariate: {tag.covar}, System: {tag.system}]")
         plt.xlabel("Chronological Age")
         plt.ylabel("Predicted Age")
-        if name == "":
-            filename = "chronological_vs_pred_age.svg"
-        else:
-            filename = f"chronological_vs_pred_age_{name}.svg"
+        
+        # Save file
+        filename = (f"chronological_vs_pred_age"
+                    f"{'_' + tag.covar if tag.covar != '' else ''}"
+                    f"{'_' + tag.system if tag.system != '' else ''}.png")
         plt.savefig(os.path.join(self.path_for_fig, filename))
         plt.close()
 
-    def age_bias_correction(self, y_true, y_pred, y_corrected, name: str = ""):
+    def age_bias_correction(self, y_true, y_pred, y_corrected, tag: NameTag):
         """Plot before and after age bias correction procedure.
 
         Parameters
         ----------
         y_true: 1D-Array with true age; shape=n
         y_pred: 1D-Array with predicted age before age bias correction; shape=n.
-        y_corrected: 1D-Array with predicted age after age bias correction; shape=n"""
+        y_corrected: 1D-Array with predicted age after age bias correction; shape=n
+        name: name of the figure"""
 
         # Find min and max age range to fit in graph
         age_range = np.arange(
             np.min([y_true, y_pred, y_corrected]), np.max([y_true, y_pred, y_corrected])
         )
 
         # Before age-bias correction
         LR_age_bias = LinearRegression(fit_intercept=True)
         LR_age_bias.fit(y_true.reshape(-1, 1), y_pred)
         plt.subplot(1, 2, 1)
         plt.plot(age_range, age_range, color="k", linestyle="dashed")
         plt.plot(age_range, LR_age_bias.predict(age_range.reshape(-1, 1)), color="r")
         plt.scatter(y_true, y_pred)
-        plt.title(f"Before age-bias correction {name}")
+        plt.title("Before age-bias correction")
         plt.ylabel("Predicted Age")
         plt.xlabel("Chronological Age")
 
         # After age-bias correction
         LR_age_bias.fit(y_true.reshape(-1, 1), y_corrected)
         plt.subplot(1, 2, 2)
         plt.plot(age_range, age_range, color="k", linestyle="dashed")
         plt.plot(age_range, LR_age_bias.predict(age_range.reshape(-1, 1)), color="r")
         plt.scatter(y_true, y_corrected)
-        plt.title(f"After age-bias correction {name}")
+        plt.title("After age-bias correction")
         plt.ylabel("Predicted Age")
         plt.xlabel("Chronological Age")
         plt.tight_layout()
-        if name == "":
-            filename = "age_bias_correction.svg"
-        else:
-            filename = f"age_bias_correction_{name}.svg"
+        
+        # Save file
+        filename = (f"age_bias_correction"
+                    f"{'_' + tag.covar if tag.covar != '' else ''}"
+                    f"{'_' + tag.system if tag.system != '' else ''}.png")
+        plt.suptitle(f"[Covariate: {tag.covar}, System: {tag.system}]\n", y=1.00)
         plt.savefig(os.path.join(self.path_for_fig, filename))
         plt.close()
 
-    def factors_vs_deltas(self, corrs, groups, labels, markers):
+    def factors_vs_deltas(self, corrs, groups, labels, markers, tag: NameTag):
         """Plot bar graph for correlation between factors and deltas.
         
         Parameters
         ----------
         corr: 2D-Array with correlation coefficients; shape=(n, m)
         labels: list of labels for each factor; shape=m,
         markers: list of list of significance markers; shape=(n, m)"""
@@ -245,51 +253,69 @@
             ax = bargraph(axs, labels, corrs[0], markers[0], groups[0])
         else:
             for i, ax in enumerate(axs):
                 ax = bargraph(ax, labels, corrs[i], markers[i], groups[i])
 
         # Save figure
         fig.set_size_inches(10, 5 * len(corrs))
+        fig.suptitle(f"Correlation of factors with age deltas of {tag.group}", y=0.99)
+        filename = f"factors_vs_deltas{'_' + tag.group if tag.group != '' else ''}.png"
         plt.tight_layout()
-        plt.savefig(os.path.join(self.path_for_fig, "factors_vs_deltas.svg"))
+        plt.savefig(os.path.join(self.path_for_fig, filename))
         plt.close()
 
-    def deltas_by_groups(self, deltas, labels):
+    def deltas_by_groups(self, deltas, labels, tag: NameTag):
         """Plot box plot for deltas in each group.
 
         Parameters
         ----------
         deltas: 2D-Array with deltas; shape=(n, m)
         labels: list of labels for each group; shape=m"""
 
         # Plot boxplots
         plt.figure(figsize=(10, 5))
-        num_groups = len(labels)
-        boxes = plt.boxplot(deltas, labels=labels, patch_artist=True)
-        for i, box in enumerate(boxes["boxes"]):
-            box.set_facecolor(self.cmap(i / num_groups))
+        ngroups = len(labels)
+        clevels = np.linspace(0, 1, ngroups)
+        boxes = plt.boxplot(deltas, labels=labels, patch_artist=True, showfliers=False)
+        # Plot patches
+        for box, clevel in zip(boxes["boxes"], clevels):
+            box.set_facecolor(self.cmap(clevel))
+            box.set_alpha(0.5)
+        # Plot scatter
+        for i, (vals, clevel) in enumerate(zip(deltas, clevels)):
+            x = np.random.normal(i + 1, 0.04, size=len(vals))
+            plt.scatter(x, vals, color=self.cmap(clevel))
         plt.xlabel("Gruop")
         plt.ylabel("Delta")
-        plt.savefig(os.path.join(self.path_for_fig, "clinical_groups_box_plot.svg"))
+
+        # Save file
+        filename = f"clinical_groups_box_plot{'_' + tag.system if tag.system != '' else ''}.png"
+        plt.suptitle(f"Age Delta by clinical group. System: {tag.system}", y=0.99)
+        plt.savefig(os.path.join(self.path_for_fig, filename))
         plt.close()
 
-    def classification_auc(self, y, y_pred, groups):
+    def classification_auc(self, y, y_pred, groups, tag: NameTag):
         """Plot ROC curve.
 
         Parameters
         ----------
         y: 1D-Array with true labels; shape=n
-        y_pred: 1D-Array with predicted labels; shape=n"""
+        y_pred: 1D-Array with predicted labels; shape=n
+        system: system name"""
 
         # Compute ROC curve and AUC
         fpr, tpr, _ = roc_curve(y, y_pred)
         auc = roc_auc_score(y, y_pred)
 
         # Plot ROC curve
         plt.plot(fpr, tpr, color='darkorange', lw=2, label='ROC curve (area = %0.2f)' % auc)
         plt.plot([0, 1], [0, 1], color='navy', lw=2, linestyle='--')
         plt.xlabel('False Positive Rate')
         plt.ylabel('True Positive Rate')
         plt.title('ROC curve %s vs %s' % (groups[0], groups[1]))
         plt.legend(loc="lower right")
-        plt.savefig(os.path.join(self.path_for_fig, "roc_curve_%s_vs_%s.svg" % (groups[0], groups[1])))
+        
+        # Save file
+        filename = f"roc_curve_{groups[0]}_vs_{groups[1]}{'_' + tag.system if tag.system != '' else ''}.png"
+        plt.suptitle(f"System: {tag.system}")
+        plt.savefig(os.path.join(self.path_for_fig, filename))
         plt.close()
```

