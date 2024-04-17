# Comparing `tmp/spectrum_fundamentals-0.5.1.tar.gz` & `tmp/spectrum_fundamentals-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.5.1.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.5.2.tar", max compression
```

## Comparing `spectrum_fundamentals-0.5.1.tar` & `spectrum_fundamentals-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1102 2024-04-12 14:21:10.165602 spectrum_fundamentals-0.5.1/LICENSE
--rw-r--r--   0        0        0     2611 2024-04-12 14:21:10.165602 spectrum_fundamentals-0.5.1/README.rst
--rw-r--r--   0        0        0     2464 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      939 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/__init__.py
--rw-r--r--   0        0        0      381 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/__main__.py
--rw-r--r--   0        0        0       29 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/annotation/__init__.py
--rw-r--r--   0        0        0    11644 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/annotation/annotation.py
--rw-r--r--   0        0        0     1377 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/charge.py
--rw-r--r--   0        0        0     8748 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/constants.py
--rw-r--r--   0        0        0    13817 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/fragments.py
--rw-r--r--   0        0        0       26 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/__init__.py
--rw-r--r--   0        0        0    14495 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/fragments_ratio.py
--rw-r--r--   0        0        0     1435 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/metric.py
--rw-r--r--   0        0        0    21687 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/percolator.py
--rw-r--r--   0        0        0    22262 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/similarity.py
--rw-r--r--   0        0        0    15698 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/mod_string.py
--rw-r--r--   0        0        0        0 2024-04-12 14:21:10.169602 spectrum_fundamentals-0.5.1/spectrum_fundamentals/py.typed
--rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2611 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/README.rst
+-rw-r--r--   0        0        0     2464 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    20512 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1377 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0    12541 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    19686 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    34826 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1563 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    23723 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    26034 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0    17026 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:14:48.068504 spectrum_fundamentals-0.5.2/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3700 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.5.2/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.5.1/LICENSE` & `spectrum_fundamentals-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.1/README.rst` & `spectrum_fundamentals-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.1/pyproject.toml` & `spectrum_fundamentals-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.5.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.5.2"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamental functions, annotation pipeline and constants for oktoberfest"
 authors = ["Wilhelmlab at Technical University of Munich"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
@@ -28,15 +28,15 @@
 pandas = "^1.3.0"
 scikit-learn = "^1.0"
 joblib = "^1.0.1"
 moepy = "^1.1.4"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.4"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 coverage = {extras = ["toml"], version = ">=5.3"}
 safety = ">=1.9.0"
 typeguard = ">=2.12.0"
 xdoctest = {extras = ["colors"], version = ">=0.15.0"}
 sphinx = ">=4.0.2"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = ">=2.11.1"
```

### Comparing `spectrum_fundamentals-0.5.1/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.5.2/spectrum_fundamentals/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Initialize fundamentals."""
 
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.5.1/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.5.2/spectrum_fundamentals/charge.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.5.1/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.5.2/spectrum_fundamentals/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 NUM_CHARGES_ONEHOT = 6
 MIN_CHARGE = 1
 MAX_CHARGE = 6
 BATCH_SIZE = 6000
 VEC_LENGTH = (
     (SEQ_LEN - 1) * 2 * 3
 )  # peptide of length 30 has 29 b and y-ions, each with charge 1+, 2+ and 3+, for a total of 174 fragments
-
+VEC_LENGTH_CMS2 = (SEQ_LEN - 1) * 2 * 3 * 2
+# peptide of length 30 can have 29 b, y, b_short, y_short, b_long and y_long ions, each with charge 1+, 2+ and 3+
+# we do not annotate fragments wth charge 3+. All fragmets with charge 3+ convert to -1
 #############
 # ALPHABETS #
 #############
 
 AA_ALPHABET = {
     "A": 1,
     "C": 24,
@@ -47,14 +49,21 @@
 ALPHABET_MODS = {
     "M[UNIMOD:35]": 21,
     "C[UNIMOD:4]": 2,
     "K[UNIMOD:737]": 22,
     "K[UNIMOD:2016]": 22,
     "K[UNIMOD:214]": 22,
     "K[UNIMOD:730]": 22,
+    "K[UNIMOD:1896]": 22,
+    "K[UNIMOD:1898]": 22,
+    "K[UNIMOD:1884]": 23,
+    "K[UNIMOD:1881]": 24,
+    "K[UNIMOD:1882]": 25,
+    "K[UNIMOD:1885]": 26,
+    "K[UNIMOD:1886]": 27,
     "S[UNIMOD:21]": 25,
     "T[UNIMOD:21]": 26,
     "Y[UNIMOD:21]": 27,
     "S[UNIMOD:23]": 16,
     "T[UNIMOD:23]": 17,
     "Y[UNIMOD:23]": 20,
     "[UNIMOD:1]-": 32,
@@ -169,20 +178,65 @@
 MOD_MASSES = {
     "[UNIMOD:737]": 229.162932,  # TMT_6
     "[UNIMOD:2016]": 304.207146,  # TMT_PRO
     "[UNIMOD:214]": 144.102063,  # iTRAQ4
     "[UNIMOD:730]": 304.205360,  # iTRAQ8
     "[UNIMOD:259]": 8.014199,  # SILAC Lysine
     "[UNIMOD:267]": 10.008269,  # SILAC Arginine
-    "[UNIMOD:21]": 79.966331,  # Phospho
-    "[UNIMOD:23]": -18.010565,  # Dehydration after phospho loss
-    "[UNIMOD:4]": 57.02146,  # Carbamidomethyl
-    "[UNIMOD:35]": 15.9949146,  # Oxidation
+    "[]": 0.0,
     "[UNIMOD:1]": 42.010565,  # Acetylation
+    "[UNIMOD:1896]": 158.003765,  # DSSO-crosslinker
+    "[UNIMOD:1881]": 54.010565,  # Alkene short fragment of DSSO-crosslinker
+    "[UNIMOD:1882]": 85.982635,  # Thiol long fragment of DSSO-crosslinker
+    "[UNIMOD:1884]": 196.084792,  # BuUrBu (DSBU)-crosslinker
+    "[UNIMOD:1885]": 111.032028,  # BuUr long fragment of BuUrBu (DSBU)-crosslinker
+    "[UNIMOD:1886]": 85.052764,  # Bu short fragment of BuUrBu (DSBU)-crosslinker
+    "[UNIMOD:1898]": 138.068080,  # DSS and BS3 non-cleavable crosslinker
+    "[UNIMOD:122]": 27.994915,  # Formylation
+    "[UNIMOD:1289]": 70.041865,  # Butyrylation
+    "[UNIMOD:1363]": 68.026215,  # Crotonylation
+    "[UNIMOD:1848]": 114.031694,  # Glutarylation
+    "[UNIMOD:1914]": -32.008456,  # Oxidation and then loss of oxidized M side chain
+    "[UNIMOD:2]": -0.984016,  # Amidation
+    "[UNIMOD:21]": 79.966331,  # Phosphorylation
+    "[UNIMOD:213]": 541.06111,  # ADP-ribosylation
+    "[UNIMOD:23]": -18.010565,  # Water Loss
+    "[UNIMOD:24]": 71.037114,  # Propionamidation
+    "[UNIMOD:354]": 44.985078,  # Nitrosylation
+    "[UNIMOD:28]": -17.026549,  # Glu to PyroGlu
+    "[UNIMOD:280]": 28.0313,  # Ethylation
+    "[UNIMOD:299]": 43.989829,  # Carboxylation
+    "[UNIMOD:3]": 226.077598,  # Biotinylation
+    "[UNIMOD:34]": 14.01565,  # Methylation
+    "[UNIMOD:345]": 47.984744,  # Trioxidation
+    "[UNIMOD:35]": 15.994915,  # Hydroxylation
+    "[UNIMOD:351]": 3.994915,  # Oxidation to Kynurenine
+    "[UNIMOD:36]": 28.0313,  # Dimethylation
+    "[UNIMOD:360]": -30.010565,  # Pyrrolidinone
+    "[UNIMOD:368]": -33.987721,  # Dehydroalanine
+    "[UNIMOD:37]": 42.04695,  # Trimethylation
+    "[UNIMOD:385]": -17.026549,  # Ammonia loss
+    "[UNIMOD:392]": 29.974179,  # Quinone
+    "[UNIMOD:4]": 57.021464,  # Carbamidomethyl
+    "[UNIMOD:40]": 79.956815,  # Sulfonation
+    "[UNIMOD:401]": -2.01565,  # Didehydro
+    "[UNIMOD:425]": 31.989829,  # Dioxidation
+    "[UNIMOD:43]": 203.079373,  # HexNAc
+    "[UNIMOD:44]": 204.187801,  # Farnesylation
+    "[UNIMOD:447]": -15.994915,  # Reduction
+    "[UNIMOD:46]": 229.014009,  # Pyridoxal phosphate
+    "[UNIMOD:47]": 238.229666,  # Palmitoylation
+    "[UNIMOD:5]": 43.005814,  # Carbamyl
+    "[UNIMOD:58]": 56.026215,  # Propionylation
+    "[UNIMOD:6]": 58.005479,  # Carboxymethylation
+    "[UNIMOD:64]": 100.016044,  # Succinylation
+    "[UNIMOD:7]": 0.984016,  # Deamidation
+    "[UNIMOD:747]": 86.000394,  # Malonylation
 }
+
 MOD_MASSES_SAGE = {
     229.1629: "[UNIMOD:737]",
     304.2071: "[UNIMOD:2016]",
     144.1020: "[UNIMOD:214]",
     304.2053: "[UNIMOD:730]",
     8.0141: "[UNIMOD:259]",
     10.0082: "[UNIMOD:267]",
@@ -202,14 +256,21 @@
     "K[UNIMOD:730]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:730]"],
     "S[UNIMOD:21]": AA_MASSES["S"] + MOD_MASSES["[UNIMOD:21]"],
     "T[UNIMOD:21]": AA_MASSES["T"] + MOD_MASSES["[UNIMOD:21]"],
     "Y[UNIMOD:21]": AA_MASSES["Y"] + MOD_MASSES["[UNIMOD:21]"],
     "S[UNIMOD:23]": AA_MASSES["S"],  # + MOD_MASSES['[UNIMOD:23]'],
     "T[UNIMOD:23]": AA_MASSES["T"],  # + MOD_MASSES['[UNIMOD:23]'],
     "Y[UNIMOD:23]": AA_MASSES["Y"],  # + MOD_MASSES['[UNIMOD:23]'],
+    "K[UNIMOD:1896]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:1896]"],
+    "K[UNIMOD:1881]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:1881]"],
+    "K[UNIMOD:1882]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:1882]"],
+    "K[UNIMOD:1884]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:1884]"],
+    "K[UNIMOD:1885]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:1885]"],
+    "K[UNIMOD:1886]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:1886]"],
+    "K[UNIMOD:1898]": AA_MASSES["K"] + MOD_MASSES["[UNIMOD:1898]"],
     "[UNIMOD:1]-": MASSES["N_TERMINUS"] + MOD_MASSES["[UNIMOD:1]"],
     "K[UNIMOD:259]": AA_MASSES[
         "K"
     ],  # + MOD_MASSES['[UNIMOD:259]'],#we need a different way of encoding mods on AA so it wouldn't have same encoding
     # to make vecMZ work
     "R[UNIMOD:267]": AA_MASSES["R"],  # + MOD_MASSES['[UNIMOD:267]']
 }
@@ -231,14 +292,38 @@
 
 B_ION_MASK = np.tile([0, 0, 0, 1, 1, 1], SEQ_LEN - 1)
 Y_ION_MASK = np.tile([1, 1, 1, 0, 0, 0], SEQ_LEN - 1)
 SINGLE_CHARGED_MASK = np.tile([1, 0, 0, 1, 0, 0], SEQ_LEN - 1)
 DOUBLE_CHARGED_MASK = np.tile([0, 1, 0, 0, 1, 0], SEQ_LEN - 1)
 TRIPLE_CHARGED_MASK = np.tile([0, 0, 1, 0, 0, 1], SEQ_LEN - 1)
 
+B_ION_MASK_XL = np.tile([0, 0, 0, 1, 1, 1], (SEQ_LEN - 1) * 2)
+Y_ION_MASK_XL = np.tile([1, 1, 1, 0, 0, 0], (SEQ_LEN - 1) * 2)
+SINGLE_CHARGED_MASK_XL = np.tile([1, 0, 0, 1, 0, 0], (SEQ_LEN - 1) * 2)
+DOUBLE_CHARGED_MASK_XL = np.tile([0, 1, 0, 0, 1, 0], (SEQ_LEN - 1) * 2)
+TRIPLE_CHARGED_MASK_XL = np.tile([0, 0, 1, 0, 0, 1], (SEQ_LEN - 1) * 2)
+
+
+MASK_DICT = {
+    1: SINGLE_CHARGED_MASK,
+    2: DOUBLE_CHARGED_MASK,
+    3: TRIPLE_CHARGED_MASK,
+    4: B_ION_MASK,
+    5: Y_ION_MASK,
+}
+
+
+MASK_DICT_XL = {
+    1: SINGLE_CHARGED_MASK_XL,
+    2: DOUBLE_CHARGED_MASK_XL,
+    3: TRIPLE_CHARGED_MASK_XL,
+    4: B_ION_MASK_XL,
+    5: Y_ION_MASK_XL,
+}
+
 
 SHARED_DATA_COLUMNS = ["RAW_FILE", "SCAN_NUMBER"]
 META_DATA_ONLY_COLUMNS = [
     "MODIFIED_SEQUENCE",
     "PRECURSOR_CHARGE",
     "MASS",
     "SCAN_EVENT_NUMBER",
```

### Comparing `spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,29 @@
     metrics_val: pd.DataFrame
 
     def __init__(
         self,
         pred_intensities: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
         true_intensities: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
         mz: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
+        xl: bool = False,
     ):
         """
         Initialize a Metric object.
 
         :param pred_intensities: predicted intensities
         :param true_intensities: observed intensities
         :param mz: observed mz values
+        :param xl: whether the metric is used for crosslinked or linear peptides
         """
         self.pred_intensities = pred_intensities
         self.true_intensities = true_intensities
         self.mz = mz
         self.metrics_val = pd.DataFrame()
+        self.xl = xl
 
     @abstractmethod
     def calc(self, all_features: bool):
         """Calculate."""
         pass
 
     def write_to_file(self, file_path: str):
```

### Comparing `spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/percolator.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     ):
         """Initialize a Percolator obj."""
         self.metadata = metadata
         self.input_type = input_type
         self.all_features_flag = all_features_flag
         self.regression_method = regression_method
         self.fdr_cutoff = fdr_cutoff
+        self.xl = "CROSSLINKER_TYPE" in self.metadata.columns
+
         super().__init__(pred_intensities, true_intensities, mz)
 
     @staticmethod
     def sample_balanced_over_bins(retention_time_df: pd.DataFrame, sample_size: int = 5000) -> pd.Index:
         """
         Sample balanced over bins.
 
@@ -241,46 +243,65 @@
         :param reverse: if true, return the label for DECOY, otherwise return the label for TARGET
         :return: target/decoy label for percolator
         """
         return TargetDecoyLabel.DECOY if reverse else TargetDecoyLabel.TARGET
 
     def add_common_features(self):
         """Add features used by both Andromeda and Prosit feature scoring sets."""
-        self.metrics_val["missedCleavages"] = self.metadata["SEQUENCE"].apply(Percolator.count_missed_cleavages)
-        self.metrics_val["KR"] = self.metadata["SEQUENCE"].apply(Percolator.count_arginines_and_lysines)
-        self.metrics_val["sequence_length"] = self.metadata["SEQUENCE"].apply(lambda x: len(x))
+        if self.xl:
+            self.metrics_val["missedCleavages_A"] = self.metadata["SEQUENCE_A"].apply(Percolator.count_missed_cleavages)
+            self.metrics_val["missedCleavages_B"] = self.metadata["SEQUENCE_B"].apply(Percolator.count_missed_cleavages)
+            self.metrics_val["KR_A"] = self.metadata["SEQUENCE_A"].apply(Percolator.count_arginines_and_lysines)
+            self.metrics_val["KR_B"] = self.metadata["SEQUENCE_B"].apply(Percolator.count_arginines_and_lysines)
+            self.metrics_val["sequence_length_a"] = self.metadata["SEQUENCE_A"].apply(lambda x: len(x))
+            self.metrics_val["sequence_length_b"] = self.metadata["SEQUENCE_B"].apply(lambda x: len(x))
+            for column_name in self.metadata.columns:
+                self.metrics_val[column_name] = self.metadata[column_name]
+        else:
+            self.metrics_val["missedCleavages"] = self.metadata["SEQUENCE"].apply(Percolator.count_missed_cleavages)
+            self.metrics_val["KR"] = self.metadata["SEQUENCE"].apply(Percolator.count_arginines_and_lysines)
+            self.metrics_val["sequence_length"] = self.metadata["SEQUENCE"].apply(lambda x: len(x))
+            self.metrics_val["Mass"] = self.metadata["CALCULATED_MASS"]  # this is the calculated mass used as a feature
 
-        self.metrics_val["Mass"] = self.metadata["CALCULATED_MASS"]  # this is the calculated mass used as a feature
         self.metrics_val["Charge1"] = (self.metadata["PRECURSOR_CHARGE"] == 1).astype(int)
         self.metrics_val["Charge2"] = (self.metadata["PRECURSOR_CHARGE"] == 2).astype(int)
         self.metrics_val["Charge3"] = (self.metadata["PRECURSOR_CHARGE"] == 3).astype(int)
         self.metrics_val["Charge4"] = (self.metadata["PRECURSOR_CHARGE"] == 4).astype(int)
         self.metrics_val["Charge5"] = (self.metadata["PRECURSOR_CHARGE"] == 5).astype(int)
         self.metrics_val["Charge6"] = (self.metadata["PRECURSOR_CHARGE"] == 6).astype(int)
-
         self.metrics_val["UnknownFragmentationMethod"] = (~self.metadata["FRAGMENTATION"].isin(["HCD", "CID"])).astype(
             int
         )
         self.metrics_val["HCD"] = (self.metadata["FRAGMENTATION"] == "HCD").astype(int)
         self.metrics_val["CID"] = (self.metadata["FRAGMENTATION"] == "CID").astype(int)
 
     def add_percolator_metadata_columns(self):
         """Add metadata columns needed by percolator, e.g. to identify a PSM."""
-        spec_id_cols = ["RAW_FILE", "SCAN_NUMBER", "MODIFIED_SEQUENCE", "PRECURSOR_CHARGE"]
+        if self.xl:
+            spec_id_cols = ["RAW_FILE", "SCAN_NUMBER", "MODIFIED_SEQUENCE_A", "MODIFIED_SEQUENCE_B", "PRECURSOR_CHARGE"]
+            self.metrics_val["Peptide"] = (
+                self.metadata["MODIFIED_SEQUENCE_A"] + "_" + self.metadata["MODIFIED_SEQUENCE_B"]
+            ).apply(lambda x: "_." + x + "._")
+            self.metrics_val["Proteins"] = (
+                self.metadata["MODIFIED_SEQUENCE_A"] + "_" + self.metadata["MODIFIED_SEQUENCE_B"]
+            )
+            self.metrics_val["Label"] = self.target_decoy_labels
+        else:
+            spec_id_cols = ["RAW_FILE", "SCAN_NUMBER", "MODIFIED_SEQUENCE", "PRECURSOR_CHARGE"]
+            self.metrics_val["Peptide"] = self.metadata["MODIFIED_SEQUENCE"].apply(lambda x: "_." + x + "._")
+            self.metrics_val["Proteins"] = self.metadata[
+                "MODIFIED_SEQUENCE"
+            ]  # we don't need the protein ID to get PSM / peptide results, fill with peptide sequence
+
         if "SCAN_EVENT_NUMBER" in self.metadata.columns:
             spec_id_cols.append("SCAN_EVENT_NUMBER")
         self.metrics_val["SpecId"] = self.metadata[spec_id_cols].apply(Percolator.get_specid, axis=1)
         self.metrics_val["Label"] = self.target_decoy_labels
         self.metrics_val["ScanNr"] = self.metadata["SCAN_NUMBER"]
         self.metrics_val["filename"] = self.metadata["RAW_FILE"]
-        self.metrics_val["Peptide"] = self.metadata["MODIFIED_SEQUENCE"].apply(lambda x: "_." + x + "._")
-
-        self.metrics_val["Proteins"] = self.metadata[
-            "MODIFIED_SEQUENCE"
-        ]  # we don't need the protein ID to get PSM / peptide results, fill with peptide sequence
 
     def apply_lda_and_get_indices_below_fdr(
         self, initial_scoring_feature: str = "spectral_angle", fdr_cutoff: float = 0.01
     ):
         """
         Applies a linear discriminant analysis on the features calculated so far (before retention time alignment) \
         to estimate false discovery rates (FDRs).
@@ -318,15 +339,14 @@
         scores_df = self.metrics_val[[feature_name]].copy()
         scores_df["Label"] = self.target_decoy_labels
         # scores_df['Sequence'] = self.metadata['SEQUENCE']
         scores_df = scores_df.sort_values(feature_name, ascending=False)
         logger.debug(scores_df.head(100))
 
         scores_df["fdr"] = Percolator.calculate_fdrs(scores_df["Label"])
-
         # filter for targets only
         scores_df = scores_df[scores_df["Label"] == TargetDecoyLabel.TARGET]
 
         accepted_indices = scores_df.index[scores_df["fdr"] < fdr_cutoff]
         if len(accepted_indices) == 0:
             logger.error(
                 f"Could not find any targets below {fdr_cutoff} out of {len(scores_df.index)} targets in total"
@@ -376,66 +396,71 @@
         mid_columns = list(set(all_columns) - set(first_columns) - set(last_columns))
         new_columns = first_columns + sorted(mid_columns) + last_columns
         self.metrics_val = self.metrics_val[new_columns]
 
     def calc(self):
         """Adds percolator metadata and feature columns to metrics_val based on PSM metadata."""
         self.add_common_features()
-
         self.target_decoy_labels = self.metadata["REVERSE"].apply(Percolator.get_target_decoy_label).to_numpy()
-
         np.random.seed(1)
         # add Prosit or Andromeda features
         if self.input_type == "rescore":
             fragments_ratio = fr.FragmentsRatio(self.pred_intensities, self.true_intensities)
-            fragments_ratio.calc()
-
+            fragments_ratio.calc(xl=self.xl)
             similarity = sim.SimilarityMetrics(self.pred_intensities, self.true_intensities, self.mz)
-            similarity.calc(self.all_features_flag)
+            similarity.calc(self.all_features_flag, xl=self.xl)
 
             self.metrics_val = pd.concat(
                 [self.metrics_val, fragments_ratio.metrics_val, similarity.metrics_val], axis=1
             )
-
-            lda_failed = False
-            idxs_below_lda_fdr = self.apply_lda_and_get_indices_below_fdr(fdr_cutoff=self.fdr_cutoff)
-            current_fdr = self.fdr_cutoff
-            while len(idxs_below_lda_fdr) == 0:
-                current_fdr += 0.01
-                idxs_below_lda_fdr = self.apply_lda_and_get_indices_below_fdr(fdr_cutoff=current_fdr)
-                if current_fdr >= 0.1:
-                    lda_failed = True
-                    break
-
-            if lda_failed:
-                sampled_idxs = Percolator.sample_balanced_over_bins(self.metadata[["RETENTION_TIME", "PREDICTED_IRT"]])
+            if self.xl:
+                self.metrics_val["collision_energy_aligned"] = self.metadata["COLLISION_ENERGY"] / 100.0
             else:
-                sampled_idxs = Percolator.sample_balanced_over_bins(
-                    self.metadata[["RETENTION_TIME", "PREDICTED_IRT"]].iloc[idxs_below_lda_fdr, :]
-                )
-
-            file_sample = self.metadata.iloc[sampled_idxs].sort_values("PREDICTED_IRT")
-            aligned_predicted_rts = Percolator.get_aligned_predicted_retention_times(
-                file_sample["RETENTION_TIME"],
-                file_sample["PREDICTED_IRT"],
-                self.metadata["PREDICTED_IRT"],
-                self.regression_method,
-            )
+                lda_failed = False
+                idxs_below_lda_fdr = self.apply_lda_and_get_indices_below_fdr(fdr_cutoff=self.fdr_cutoff)
+                current_fdr = self.fdr_cutoff
+                while len(idxs_below_lda_fdr) == 0:
+                    current_fdr += 0.01
+                    idxs_below_lda_fdr = self.apply_lda_and_get_indices_below_fdr(fdr_cutoff=current_fdr)
+                    if current_fdr >= 0.1:
+                        lda_failed = True
+                        break
+                else:
+                    if lda_failed:
+                        sampled_idxs = Percolator.sample_balanced_over_bins(
+                            self.metadata[["RETENTION_TIME", "PREDICTED_IRT"]]
+                        )
+                    else:
+                        sampled_idxs = Percolator.sample_balanced_over_bins(
+                            self.metadata[["RETENTION_TIME", "PREDICTED_IRT"]].iloc[idxs_below_lda_fdr, :]
+                        )
+
+                    file_sample = self.metadata.iloc[sampled_idxs].sort_values("PREDICTED_IRT")
+                    aligned_predicted_rts = Percolator.get_aligned_predicted_retention_times(
+                        file_sample["RETENTION_TIME"],
+                        file_sample["PREDICTED_IRT"],
+                        self.metadata["PREDICTED_IRT"],
+                        self.regression_method,
+                    )
+
+                    self.metrics_val["RT"] = self.metadata["RETENTION_TIME"]
+                    self.metrics_val["pred_RT"] = self.metadata["PREDICTED_IRT"]
+                    self.metrics_val["iRT"] = aligned_predicted_rts
+                    self.metrics_val["collision_energy_aligned"] = self.metadata["COLLISION_ENERGY"] / 100.0
+                    self.metrics_val["abs_rt_diff"] = np.abs(self.metadata["RETENTION_TIME"] - aligned_predicted_rts)
+
+                    median_abs_error_lda_targets = np.median(self.metrics_val["abs_rt_diff"].iloc[idxs_below_lda_fdr])
+                    logger.info(
+                        "Median absolute error predicted vs observed retention time on targets < 1% FDR: "
+                        f"{median_abs_error_lda_targets}"
+                    )
+                    logger.debug(
+                        self.metrics_val[["RT", "pred_RT", "abs_rt_diff", "lda_scores"]].iloc[idxs_below_lda_fdr, :]
+                    )
 
-            self.metrics_val["RT"] = self.metadata["RETENTION_TIME"]
-            self.metrics_val["pred_RT"] = self.metadata["PREDICTED_IRT"]
-            self.metrics_val["iRT"] = aligned_predicted_rts
-            self.metrics_val["collision_energy_aligned"] = self.metadata["COLLISION_ENERGY"] / 100.0
-            self.metrics_val["abs_rt_diff"] = np.abs(self.metadata["RETENTION_TIME"] - aligned_predicted_rts)
-
-            median_abs_error_lda_targets = np.median(self.metrics_val["abs_rt_diff"].iloc[idxs_below_lda_fdr])
-            logger.info(
-                f"Median absolute error predicted vs observed retention time on targets < 1% FDR: {median_abs_error_lda_targets}"
-            )
-            logger.debug(self.metrics_val[["RT", "pred_RT", "abs_rt_diff", "lda_scores"]].iloc[idxs_below_lda_fdr, :])
         else:
             self.metrics_val["andromeda"] = self.metadata["SCORE"]
 
         self.add_percolator_metadata_columns()
         if self.input_type == "rescore":
             # TODO: only add this feature if they are not all zero
             # self.metrics_val['spectral_angle_delta_score'] = Percolator.get_delta_score(self.metrics_val[['ScanNr',
```

### Comparing `spectrum_fundamentals-0.5.1/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.5.2/spectrum_fundamentals/metrics/similarity.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 def get_metric_func(metric: str):
     """
     Return a callable function for a given metric shortcut.
 
     :param metric: a shortcut for the desired metric.
-
     :raises ValueError: if the provided metric is not known
 
     :return: callable metric function
 
     """
     if metric == "mean":
         return lambda obs, pred: mean(absolute(obs - mean(pred)))
@@ -43,37 +42,33 @@
     """Class to generate several features than can be used by percoltor for rescoring."""
 
     @staticmethod
     def spectral_angle(
         observed_intensities: Union[scipy.sparse.csr_matrix, np.ndarray],
         predicted_intensities: Union[scipy.sparse.csr_matrix, np.ndarray],
         charge: int = 0,
+        xl: bool = False,
     ) -> np.ndarray:
         """
         Calculate spectral angle.
 
         :param observed_intensities: observed intensities, constants.EPSILON intensity indicates zero intensity peaks, \
                                      0 intensity indicates invalid peaks (charge state > peptide charge state or \
                                      position >= peptide length), array of length 174
         :param predicted_intensities: predicted intensities, see observed_intensities for details, array of length 174
         :param charge: to filter by the peak charges, 0 means everything
+        :param xl: whether operating on cleavable crosslinked or linear peptides
+        :raises ValueError: if charge is smaller than 1 or larger than 5
         :return: SA values
         """
         if charge != 0:
-            if charge == 1:
-                boolean_array = constants.SINGLE_CHARGED_MASK
-            elif charge == 2:
-                boolean_array = constants.DOUBLE_CHARGED_MASK
-            elif charge == 3:
-                boolean_array = constants.TRIPLE_CHARGED_MASK
-            elif charge == 4:
-                boolean_array = constants.B_ION_MASK
-            else:
-                boolean_array = constants.Y_ION_MASK
-
+            if not 1 <= charge <= 5:
+                raise ValueError("Charge must be between 1 to 5.")
+            masks = constants.MASK_DICT_XL if xl else constants.MASK_DICT
+            boolean_array = masks[charge]
             boolean_array = scipy.sparse.csr_matrix(boolean_array)
             observed_intensities = scipy.sparse.csr_matrix(observed_intensities)
             predicted_intensities = scipy.sparse.csr_matrix(predicted_intensities)
             observed_intensities = observed_intensities.multiply(boolean_array).toarray()
             predicted_intensities = predicted_intensities.multiply(boolean_array).toarray()
 
         predicted_non_zero_mask = predicted_intensities > constants.EPSILON
@@ -200,41 +195,38 @@
 
     @staticmethod
     def correlation(
         observed_intensities: scipy.sparse.csr_matrix,
         predicted_intensities: scipy.sparse.csr_matrix,
         charge: int = 0,
         method: str = "pearson",
+        xl: bool = False,
     ) -> List[float]:
         """
         Calculate correlation between observed and predicted.
 
         :param observed_intensities: observed intensities, constants.EPSILON intensity indicates zero intensity peaks, \
                                      0 intensity indicates invalid peaks (charge state > peptide charge state or \
                                      position >= peptide length), array of length 174
         :param predicted_intensities: predicted intensities, see observed_intensities for details, array of length 174
         :param charge: to filter by the peak charges, 0 means everything
         :param method: either pearson or spearman
+        :param xl: wheter or not to use xl mode
+        :raises ValueError: if charge is smaller than 1 or larger than 5
+
         :return: calculated correlations
         """
         observed_intensities_array = observed_intensities.toarray()
         predicted_intensities_array = predicted_intensities.toarray()
 
         if charge != 0:
-            if charge == 1:
-                boolean_array = constants.SINGLE_CHARGED_MASK
-            elif charge == 2:
-                boolean_array = constants.DOUBLE_CHARGED_MASK
-            elif charge == 3:
-                boolean_array = constants.TRIPLE_CHARGED_MASK
-            elif charge == 4:
-                boolean_array = constants.B_ION_MASK
-            else:
-                boolean_array = constants.Y_ION_MASK
-
+            if not 1 <= charge <= 5:
+                raise ValueError("Charge must be between 1 to 5.")
+            masks = constants.MASK_DICT_XL if xl else constants.MASK_DICT
+            boolean_array = masks[charge]
             boolean_array = scipy.sparse.csr_matrix(boolean_array)
             observed_intensities_array = observed_intensities.multiply(boolean_array).toarray()
             predicted_intensities_array = predicted_intensities.multiply(boolean_array).toarray()
 
         pear_corr = []
         for obs, pred in zip(observed_intensities_array, predicted_intensities_array):
             valid_ion_mask = pred > constants.EPSILON
@@ -399,79 +391,151 @@
             cosine = sum_matched / (sqrt_sum_pred * sqrt_sum_obs)
             if np.isnan(cosine):
                 cosine = 0
             cos_values.append(cosine)
 
         return cos_values
 
-    def calc(self, all_features: bool):
+    def calc(self, all_features: bool, xl: bool = False):
         """
         Adds columns with spectral angle feature to metrics_val dataframe.
 
-        :param all_features: if True, calculcate all metrics
+        :param all_features: if True, calculate all metrics
+        :param xl: whether calculating for crosslinked or linear peptides
         """
-        self.metrics_val["spectral_angle"] = SimilarityMetrics.spectral_angle(
-            self.true_intensities, self.pred_intensities, 0
+        if xl:
+            if self.true_intensities is not None and self.pred_intensities is not None:
+                true_intensities_a = (
+                    self.true_intensities[:, :348] if self.true_intensities.shape[1] >= 348 else self.true_intensities
+                )
+                true_intensities_b = self.true_intensities[:, 348:] if self.true_intensities.shape[1] >= 348 else None
+                pred_intensities_a = (
+                    self.pred_intensities[:, :348] if self.pred_intensities.shape[1] >= 348 else self.pred_intensities
+                )
+                pred_intensities_b = self.pred_intensities[:, 348:] if self.pred_intensities.shape[1] >= 348 else None
+
+                if true_intensities_a is not None and pred_intensities_a is not None:
+                    self.metrics_val["spectral_angle_a"] = SimilarityMetrics.spectral_angle(
+                        true_intensities_a, pred_intensities_a, 0
+                    )
+                    self.metrics_val["pearson_corr_a"] = SimilarityMetrics.correlation(
+                        true_intensities_a, pred_intensities_a, 0
+                    )
+                    if all_features:
+                        self._calc_additional_metrics(true_intensities_a, pred_intensities_a, key_suffix="_a")
+
+                if true_intensities_b is not None and pred_intensities_b is not None:
+                    self.metrics_val["spectral_angle_b"] = SimilarityMetrics.spectral_angle(
+                        true_intensities_b, pred_intensities_b, 0
+                    )
+                    self.metrics_val["pearson_corr_b"] = SimilarityMetrics.correlation(
+                        true_intensities_b, pred_intensities_b, 0
+                    )
+                    if all_features:
+                        self._calc_additional_metrics(true_intensities_b, pred_intensities_b, key_suffix="_b")
+
+                if true_intensities_a is not None and true_intensities_b is not None:
+                    self.metrics_val["spectral_angle"] = (
+                        self.metrics_val["spectral_angle_a"] + self.metrics_val["spectral_angle_b"]
+                    ) / 2
+
+        else:
+            if self.true_intensities is not None and self.pred_intensities is not None:
+                self.metrics_val["spectral_angle"] = SimilarityMetrics.spectral_angle(
+                    self.true_intensities, self.pred_intensities, 0
+                )
+                self.metrics_val["pearson_corr"] = SimilarityMetrics.correlation(
+                    self.true_intensities, self.pred_intensities, 0, "pearson"
+                )
+                if all_features:
+                    self._calc_additional_metrics(self.true_intensities, self.pred_intensities)
+
+    def _calc_additional_metrics(
+        self,
+        true_intensities: Union[np.ndarray, scipy.sparse.spmatrix],
+        pred_intensities: Union[np.ndarray, scipy.sparse.spmatrix],
+        key_suffix: str = "",
+    ):
+        self.metrics_val[f"spectral_entropy_similarity{key_suffix}"] = SimilarityMetrics.spectral_entropy_similarity(
+            true_intensities, pred_intensities
         )
-        self.metrics_val["pearson_corr"] = SimilarityMetrics.correlation(
-            self.true_intensities, self.pred_intensities, 0, "pearson"
+        self.metrics_val[f"cos{key_suffix}"] = SimilarityMetrics.cos(true_intensities, pred_intensities)
+        self.metrics_val[f"mean_abs_diff{key_suffix}"] = SimilarityMetrics.abs_diff(
+            true_intensities, pred_intensities, "mean"
         )
-        if all_features:
-            self.metrics_val["modified_cosine"] = SimilarityMetrics.modified_cosine(
-                self.true_intensities, self.pred_intensities, self.mz, self.mz
-            )
-            self.metrics_val["spectral_entropy_similarity"] = SimilarityMetrics.spectral_entropy_similarity(
-                self.true_intensities, self.pred_intensities
-            )
+        self.metrics_val[f"std_abs_diff{key_suffix}"] = SimilarityMetrics.abs_diff(
+            true_intensities, pred_intensities, "std"
+        )
+        self.metrics_val[f"abs_diff_Q3{key_suffix}"] = SimilarityMetrics.abs_diff(
+            true_intensities, pred_intensities, "q3"
+        )
+        self.metrics_val[f"abs_diff_Q2{key_suffix}"] = SimilarityMetrics.abs_diff(
+            true_intensities, pred_intensities, "q2"
+        )
+        self.metrics_val[f"abs_diff_Q1{key_suffix}"] = SimilarityMetrics.abs_diff(
+            true_intensities, pred_intensities, "q1"
+        )
+        self.metrics_val[f"min_abs_diff{key_suffix}"] = SimilarityMetrics.abs_diff(
+            true_intensities, pred_intensities, "min"
+        )
+        self.metrics_val[f"max_abs_diff{key_suffix}"] = SimilarityMetrics.abs_diff(
+            true_intensities, pred_intensities, "max"
+        )
+        self.metrics_val[f"mse{key_suffix}"] = SimilarityMetrics.abs_diff(true_intensities, pred_intensities, "mse")
+        self.metrics_val[f"modified_cosine{key_suffix}"] = SimilarityMetrics.modified_cosine(
+            true_intensities, pred_intensities, self.mz, self.mz
+        )
+
+        col_names_spectral_angle = [
+            f"spectral_angle_{amount}_charge{key_suffix}" for amount in ["single", "double", "triple"]
+        ] + [f"spectral_angle_b_ions{key_suffix}", f"spectral_angle_y_ions{key_suffix}"]
+        col_names_pearson_corr = [
+            f"pearson_corr_{amount}_charge{key_suffix}" for amount in ["single", "double", "triple"]
+        ] + [
+            f"pearson_corr_b_ions{key_suffix}",
+            f"pearson_corr_y_ions{key_suffix}",
+        ]
+        col_names_spearman_corr = [
+            f"spearman_corr_{amount}_charge{key_suffix}" for amount in ["single", "double", "triple"]
+        ] + [f"spearman_corr_b_ions{key_suffix}", f"spearman_corr_y_ions{key_suffix}"]
+
+        if key_suffix != "":
+            # dirty fix, if the key_suffix is not "", that means we have XL mode.
+            # TODO: fix self.mz for XL mode
 
-            col_names_spectral_angle = [
-                f"spectral_angle_{amount}_charge" for amount in ["single", "double", "triple"]
-            ] + ["spectral_angle_b_ions", "spectral_angle_y_ions"]
-            col_names_pearson_corr = [f"pearson_corr_{amount}_charge" for amount in ["single", "double", "triple"]] + [
-                "pearson_corr_b_ions",
-                "pearson_corr_y_ions",
-            ]
-            col_names_spearman_corr = [
-                f"spearman_corr_{amount}_charge" for amount in ["single", "double", "triple"]
-            ] + ["spearman_corr_b_ions", "spearman_corr_y_ions"]
+            self.metrics_val[f"spearman_corr{key_suffix}"] = SimilarityMetrics.correlation(
+                true_intensities, pred_intensities, 0, "spearman", xl=True
+            )
 
             for i, col_name_spectral_angle in enumerate(col_names_spectral_angle):
                 self.metrics_val[col_name_spectral_angle] = SimilarityMetrics.spectral_angle(
-                    self.true_intensities, self.pred_intensities, i + 1
+                    true_intensities, pred_intensities, i + 1, xl=True
                 )
 
             for i, col_name_pearson_corr in enumerate(col_names_pearson_corr):
                 self.metrics_val[col_name_pearson_corr] = SimilarityMetrics.correlation(
-                    self.true_intensities, self.pred_intensities, i + 1, "pearson"
+                    true_intensities, pred_intensities, i + 1, "pearson", xl=True
                 )
 
-            self.metrics_val["cos"] = SimilarityMetrics.cos(self.true_intensities, self.pred_intensities)
-            self.metrics_val["mean_abs_diff"] = SimilarityMetrics.abs_diff(
-                self.true_intensities, self.pred_intensities, "mean"
-            )
-            self.metrics_val["std_abs_diff"] = SimilarityMetrics.abs_diff(
-                self.true_intensities, self.pred_intensities, "std"
-            )
-            self.metrics_val["abs_diff_Q3"] = SimilarityMetrics.abs_diff(
-                self.true_intensities, self.pred_intensities, "q3"
-            )
-            self.metrics_val["abs_diff_Q2"] = SimilarityMetrics.abs_diff(
-                self.true_intensities, self.pred_intensities, "q2"
-            )
-            self.metrics_val["abs_diff_Q1"] = SimilarityMetrics.abs_diff(
-                self.true_intensities, self.pred_intensities, "q1"
-            )
-            self.metrics_val["min_abs_diff"] = SimilarityMetrics.abs_diff(
-                self.true_intensities, self.pred_intensities, "min"
-            )
-            self.metrics_val["max_abs_diff"] = SimilarityMetrics.abs_diff(
-                self.true_intensities, self.pred_intensities, "max"
-            )
-            self.metrics_val["mse"] = SimilarityMetrics.abs_diff(self.true_intensities, self.pred_intensities, "mse")
-            self.metrics_val["spearman_corr"] = SimilarityMetrics.correlation(
-                self.true_intensities, self.pred_intensities, 0, "spearman"
+            for i, col_name_spearman_corr in enumerate(col_names_spearman_corr):
+                self.metrics_val[col_name_spearman_corr] = SimilarityMetrics.correlation(
+                    true_intensities, pred_intensities, i + 1, "spearman", xl=True
+                )
+        else:
+            self.metrics_val[f"spearman_corr{key_suffix}"] = SimilarityMetrics.correlation(
+                true_intensities, pred_intensities, 0, "spearman"
             )
 
+            for i, col_name_spectral_angle in enumerate(col_names_spectral_angle):
+                self.metrics_val[col_name_spectral_angle] = SimilarityMetrics.spectral_angle(
+                    true_intensities, pred_intensities, i + 1
+                )
+
+            for i, col_name_pearson_corr in enumerate(col_names_pearson_corr):
+                self.metrics_val[col_name_pearson_corr] = SimilarityMetrics.correlation(
+                    true_intensities, pred_intensities, i + 1, "pearson"
+                )
+
             for i, col_name_spearman_corr in enumerate(col_names_spearman_corr):
                 self.metrics_val[col_name_spearman_corr] = SimilarityMetrics.correlation(
-                    self.true_intensities, self.pred_intensities, i + 1, "spearman"
+                    true_intensities, pred_intensities, i + 1, "spearman"
                 )
```

### Comparing `spectrum_fundamentals-0.5.1/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.5.2/spectrum_fundamentals/mod_string.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import difflib
 import re
-from itertools import repeat
+from itertools import combinations, repeat
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from .constants import (
     MAXQUANT_VAR_MODS,
@@ -334,14 +334,41 @@
     pattern = sorted(alphabet, key=len, reverse=True)
 
     pattern = [re.escape(i) for i in pattern]
     regex_pattern = re.compile("|".join(pattern))
     return map(split_modstring, sequences, repeat(regex_pattern))
 
 
+def add_permutations(modified_sequence: str, unimod_id: int, residues: List[str]):
+    """
+    Generate different peptide sequences with moving the modification to all possible residues.
+
+    :param modified_sequence: Peptide sequence
+    :param unimod_id: modification unimod id to be used for generating different permutations.
+    :param residues: possible amino acids where this mod can exist
+    :return: list of possible sequence permutations
+    """
+    sequence = modified_sequence.replace("[UNIMOD:" + str(unimod_id) + "]", "")
+    modifications = len(re.findall("UNIMOD:" + str(unimod_id), modified_sequence))
+    if modifications == 0:
+        return modified_sequence
+    possible_positions = [i for i, ltr in enumerate(sequence) if ltr in residues]
+    possible_positions.sort(reverse=True)
+    all_combinations = [list(each_permutation) for each_permutation in combinations(possible_positions, modifications)]
+    modified_sequences_comb = []
+    for comb in all_combinations:
+        modified_sequence = sequence
+        for index in comb:
+            modified_sequence = (
+                modified_sequence[: index + 1] + "[unimod:" + str(unimod_id) + "]" + modified_sequence[index + 1 :]
+            )
+        modified_sequences_comb.append(modified_sequence)
+    return modified_sequences_comb
+
+
 def proteomicsdb_to_internal(sequence: str, mods_variable: str = "", mods_fixed: str = "") -> str:
     """
     Function to create a sequence with UNIMOD modifications from given sequence and it's varaible and fixed modifications.
 
     :param sequence: The sequence to modify
     :param mods_variable: the variable modifacations (e.g. "Oxidation@M45")
     :param mods_fixed: the fixed modifacations (e.g. "Carbamidomethyl@C")
```

### Comparing `spectrum_fundamentals-0.5.1/PKG-INFO` & `spectrum_fundamentals-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_fundamentals
-Version: 0.5.1
+Version: 0.5.2
 Summary: Fundamental functions, annotation pipeline and constants for oktoberfest
 Home-page: https://github.com/wilhelm-lab/spectrum_fundamentals
 License: MIT
 Author: Wilhelmlab at Technical University of Munich
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

