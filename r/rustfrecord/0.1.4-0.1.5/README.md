# Comparing `tmp/rustfrecord-0.1.4.tar.gz` & `tmp/rustfrecord-0.1.5.tar.gz`

## Comparing `rustfrecord-0.1.4.tar` & `rustfrecord-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 rustfrecord-0.1.4/Cargo.toml
--rw-r--r--   0      502       20     1341 2024-04-11 08:51:17.000000 rustfrecord-0.1.4/.devcontainer/devcontainer.json
--rw-r--r--   0      502       20     5102 2024-04-16 11:33:55.000000 rustfrecord-0.1.4/.github/workflows/CI.yml
--rw-r--r--   0      502       20       85 2024-04-15 12:50:52.000000 rustfrecord-0.1.4/.gitignore
--rw-r--r--   0      502       20      166 2024-04-15 10:44:23.000000 rustfrecord-0.1.4/.vscode/settings.json
--rw-r--r--   0      502       20     1507 2024-04-16 13:52:52.000000 rustfrecord-0.1.4/README.md
--rw-r--r--   0      502       20      634 2024-04-11 18:53:31.000000 rustfrecord-0.1.4/main.py
--rw-r--r--   0      502       20     2536 2024-04-15 13:20:59.000000 rustfrecord-0.1.4/requirements-linux.txt
--rw-r--r--   0      502       20      508 2024-04-15 13:20:18.000000 rustfrecord-0.1.4/requirements-macos.txt
--rw-r--r--   0      502       20     1163 2024-04-15 11:11:32.000000 rustfrecord-0.1.4/src/lib.rs
--rw-r--r--   0      502       20     1571 2024-04-11 10:57:05.000000 rustfrecord-0.1.4/src/pyo3_tch.rs
--rw-r--r--   0      502       20     1951 2024-04-15 10:17:58.000000 rustfrecord-0.1.4/src/tfrecord_reader.rs
--rw-r--r--   0      502       20    45986 2024-04-16 14:00:24.000000 rustfrecord-0.1.4/Cargo.lock
--rw-r--r--   0      502       20      571 2024-04-16 07:56:44.000000 rustfrecord-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 rustfrecord-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 rustfrecord-0.1.5/Cargo.toml
+-rw-r--r--   0      502       20     1341 2024-04-11 08:51:17.000000 rustfrecord-0.1.5/.devcontainer/devcontainer.json
+-rw-r--r--   0      502       20     5102 2024-04-16 11:33:55.000000 rustfrecord-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0      502       20       85 2024-04-15 12:50:52.000000 rustfrecord-0.1.5/.gitignore
+-rw-r--r--   0      502       20      166 2024-04-15 10:44:23.000000 rustfrecord-0.1.5/.vscode/settings.json
+-rw-r--r--   0      502       20     1518 2024-04-17 08:48:24.000000 rustfrecord-0.1.5/README.md
+-rw-r--r--   0      502       20     2536 2024-04-15 13:20:59.000000 rustfrecord-0.1.5/requirements-linux.txt
+-rw-r--r--   0      502       20      508 2024-04-15 13:20:18.000000 rustfrecord-0.1.5/requirements-macos.txt
+-rw-r--r--   0      502       20     1258 2024-04-17 12:52:44.000000 rustfrecord-0.1.5/src/lib.rs
+-rw-r--r--   0      502       20     1571 2024-04-11 10:57:05.000000 rustfrecord-0.1.5/src/pyo3_tch.rs
+-rw-r--r--   0      502       20     2297 2024-04-17 11:38:13.000000 rustfrecord-0.1.5/src/tfrecord_reader.rs
+-rw-r--r--   0      502       20     1758 2024-04-17 12:59:35.000000 rustfrecord-0.1.5/test_rustfrecord.py
+-rw-r--r--   0      502       20    45986 2024-04-17 12:54:10.000000 rustfrecord-0.1.5/Cargo.lock
+-rw-r--r--   0      502       20      571 2024-04-16 07:56:44.000000 rustfrecord-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 rustfrecord-0.1.5/PKG-INFO
```

### Comparing `rustfrecord-0.1.4/Cargo.toml` & `rustfrecord-0.1.5/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rustfrecord"
-version = "0.1.4"
+version = "0.1.5"
 description = "Rust implementation to read TFRecord files into PyTorch tensors"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "rustfrecord"
 crate-type = ["cdylib"]
```

### Comparing `rustfrecord-0.1.4/.devcontainer/devcontainer.json` & `rustfrecord-0.1.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.4/.github/workflows/CI.yml` & `rustfrecord-0.1.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.4/README.md` & `rustfrecord-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,22 @@
     pip3 install rustfrecord
 
 ## Getting Started
 
 The `Reader` class reads TFRecord files and yields `Dict[str, Tensor]` objects.
 
 ```python
+import torch
 from torch import Tensor
 from rustfrecord import Reader
 
 filename = "data/002scattered.training_examples.tfrecord.gz"
 r = Reader(filename, compressed=True)
 
-for (i, features) in enumerate(r):
+for i, features in enumerate(r):
     print(features.keys())
     # ['variant_type', 'image/encoded', 'image/shape',
     #  'variant/encoded', 'label', 'alt_allele_indices/encoded',
     #  'locus', 'sequencing_type']
 
     label: Tensor = features['label']
     shape = torch.Size(tuple(features['image/shape']))
```

### Comparing `rustfrecord-0.1.4/requirements-linux.txt` & `rustfrecord-0.1.5/requirements-linux.txt`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.4/src/lib.rs` & `rustfrecord-0.1.5/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 struct Reader {
     inner: tfrecord_reader::Reader,
 }
 
 #[pymethods]
 impl Reader {
     #[new]
-    fn new(filename: &str, compressed: bool) -> PyResult<Self> {
-        tfrecord_reader::Reader::new(filename, compressed)
+    fn new(filename: &str, compressed: bool, features: Option<Vec<String>>) -> PyResult<Self> {
+        let features = features.unwrap_or_default();
+        tfrecord_reader::Reader::new(filename, compressed, &features)
             .map(|r| Reader { inner: r })
             .map_err(|e| PyOSError::new_err(format!("{e:?}")))
     }
 
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
```

### Comparing `rustfrecord-0.1.4/src/pyo3_tch.rs` & `rustfrecord-0.1.5/src/pyo3_tch.rs`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.4/src/tfrecord_reader.rs` & `rustfrecord-0.1.5/src/tfrecord_reader.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-use std::{collections::HashMap, fs, io::Read, path::Path};
+use std::{
+    collections::{HashMap, HashSet},
+    fs,
+    io::Read,
+    path::Path,
+};
 
 use anyhow::{Context, Result};
 use flate2::read::GzDecoder;
 use tch::Tensor;
 use tfrecord::{Example, ExampleIter, FeatureKind, RecordReaderConfig};
 
 pub struct Reader {
     example_iter: ExampleIter<Box<dyn Read + Send>>,
+    features: HashSet<String>,
 }
 
 impl Reader {
-    pub fn new(filename: &str, compressed: bool) -> Result<Self> {
+    pub fn new(filename: &str, compressed: bool, features: &[impl AsRef<str>]) -> Result<Self> {
         let path = Path::new(filename);
 
         let conf = RecordReaderConfig {
             check_integrity: false,
         };
 
         let file = fs::File::open(path).with_context(|| format!("failed to open {path:?}"))?;
@@ -23,15 +29,18 @@
             Box::new(GzDecoder::new(file))
         } else {
             Box::new(file)
         };
 
         let example_iter = ExampleIter::from_reader(reader, conf);
 
-        Ok(Self { example_iter })
+        Ok(Self {
+            example_iter,
+            features: features.iter().map(|s| s.as_ref().to_string()).collect(),
+        })
     }
 }
 
 impl Iterator for Reader {
     // Iterate over Examples.
     //
     // Comment from example.proto:
@@ -39,21 +48,24 @@
     // An Example is a mostly-normalized data format for storing data for training and inference.
     // It contains a key-value store (features); where each key (string) maps to a Feature message
     // (which is one of packed BytesList, FloatList, or Int64List).
 
     type Item = tfrecord::Result<HashMap<String, Tensor>>;
 
     fn next(&mut self) -> Option<Self::Item> {
-        self.example_iter.next().map(|e| e.map(example_to_hashmap))
+        self.example_iter
+            .next()
+            .map(|e| e.map(|e| example_to_hashmap(e, &self.features)))
     }
 }
 
-fn example_to_hashmap(example: Example) -> HashMap<String, Tensor> {
+fn example_to_hashmap(example: Example, features: &HashSet<String>) -> HashMap<String, Tensor> {
     example
         .into_iter()
+        .filter(|(name, _)| features.is_empty() || features.contains(name))
         .map(|(name, feature)| {
             let tensor = match feature.into_kinds() {
                 Some(FeatureKind::F32(value)) => Tensor::from_slice(&value),
                 Some(FeatureKind::I64(value)) => Tensor::from_slice(&value),
                 Some(FeatureKind::Bytes(value)) => Tensor::from_slice2(&value),
                 None => Tensor::new(),
             };
```

### Comparing `rustfrecord-0.1.4/Cargo.lock` & `rustfrecord-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1158,15 +1158,15 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustfrecord"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "flate2",
  "pyo3",
  "tch",
  "tfrecord",
  "torch-sys",
```

### Comparing `rustfrecord-0.1.4/pyproject.toml` & `rustfrecord-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.4/PKG-INFO` & `rustfrecord-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rustfrecord
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: setuptools ==69.5.1
 Requires-Dist: torch ==2.2.0
 Requires-Dist: maturin ==1.5.1
 Requires-Dist: pip ==24.0
 Requires-Dist: numpy ==1.24.4
@@ -27,21 +27,22 @@
     pip3 install rustfrecord
 
 ## Getting Started
 
 The `Reader` class reads TFRecord files and yields `Dict[str, Tensor]` objects.
 
 ```python
+import torch
 from torch import Tensor
 from rustfrecord import Reader
 
 filename = "data/002scattered.training_examples.tfrecord.gz"
 r = Reader(filename, compressed=True)
 
-for (i, features) in enumerate(r):
+for i, features in enumerate(r):
     print(features.keys())
     # ['variant_type', 'image/encoded', 'image/shape',
     #  'variant/encoded', 'label', 'alt_allele_indices/encoded',
     #  'locus', 'sequencing_type']
 
     label: Tensor = features['label']
     shape = torch.Size(tuple(features['image/shape']))
```

