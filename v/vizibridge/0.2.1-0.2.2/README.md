# Comparing `tmp/vizibridge-0.2.1.tar.gz` & `tmp/vizibridge-0.2.2.tar.gz`

## Comparing `vizibridge-0.2.1.tar` & `vizibridge-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vizibridge-0.2.1/Cargo.toml
--rw-rw-rw-   0        0        0      705 2024-04-16 21:38:14.000000 vizibridge-0.2.1/.gitignore
--rw-rw-rw-   0        0        0     1974 2024-04-16 21:38:14.000000 vizibridge-0.2.1/.gitlab-ci.yml
--rw-rw-rw-   0        0        0       70 2024-04-16 21:38:14.000000 vizibridge-0.2.1/Dockerfile
--rw-rw-rw-   0        0        0     1073 2024-04-16 21:38:14.000000 vizibridge-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1459 2024-04-16 21:38:14.000000 vizibridge-0.2.1/python/vizibridge/__init__.py
--rw-rw-rw-   0        0        0       32 2024-04-16 21:38:14.000000 vizibridge-0.2.1/rust-toolchain.toml
--rw-rw-rw-   0        0        0     3197 2024-04-16 21:38:14.000000 vizibridge-0.2.1/src/lib.rs
--rw-r--r--   0        0        0     8453 2024-04-16 21:38:18.000000 vizibridge-0.2.1/Cargo.lock
--rw-rw-rw-   0        0        0      514 2024-04-16 21:38:14.000000 vizibridge-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 vizibridge-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vizibridge-0.2.2/Cargo.toml
+-rw-rw-rw-   0        0        0      705 2024-04-17 08:21:22.000000 vizibridge-0.2.2/.gitignore
+-rw-rw-rw-   0        0        0     1974 2024-04-17 08:21:22.000000 vizibridge-0.2.2/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0       70 2024-04-17 08:21:22.000000 vizibridge-0.2.2/Dockerfile
+-rw-rw-rw-   0        0        0     1073 2024-04-17 08:21:22.000000 vizibridge-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     1906 2024-04-17 08:21:22.000000 vizibridge-0.2.2/README.md
+-rw-rw-rw-   0        0        0     1559 2024-04-17 08:21:22.000000 vizibridge-0.2.2/python/vizibridge/__init__.py
+-rw-rw-rw-   0        0        0       32 2024-04-17 08:21:22.000000 vizibridge-0.2.2/rust-toolchain.toml
+-rw-rw-rw-   0        0        0     3524 2024-04-17 08:21:22.000000 vizibridge-0.2.2/src/lib.rs
+-rw-r--r--   0        0        0     8453 2024-04-17 08:21:25.000000 vizibridge-0.2.2/Cargo.lock
+-rw-rw-rw-   0        0        0      514 2024-04-17 08:21:22.000000 vizibridge-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 vizibridge-0.2.2/PKG-INFO
```

### Comparing `vizibridge-0.2.1/.gitignore` & `vizibridge-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vizibridge-0.2.1/.gitlab-ci.yml` & `vizibridge-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `vizibridge-0.2.1/LICENSE` & `vizibridge-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vizibridge-0.2.1/python/vizibridge/__init__.py` & `vizibridge-0.2.2/python/vizibridge/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,7 +48,10 @@
         return repr(self.data)
 
     def __len__(self):
         return len(self.data)
 
     def enum_canonical_kmer(self, k: int) -> Kmer:
         return getattr(self.data, f"enumerate_canonical_kmer{k}")()
+
+    def enum_kmer(self, k: int) -> Kmer:
+        return getattr(self.data, f"enumerate_kmer{k}")()
```

### Comparing `vizibridge-0.2.1/src/lib.rs` & `vizibridge-0.2.2/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![allow(non_local_definitions)]
 use pyo3::prelude::*;
 use pyo3::types::{PyString, PyType};
 use seq_macro::seq;
 use vizitig_lib::dna::{Nucleotid, DNA};
-use vizitig_lib::iterators::CanonicalKmerIterator;
+use vizitig_lib::iterators::{CanonicalKmerIterator, KmerIterator};
 use vizitig_lib::kmer::ShortKmer;
 
 
 /// A class wrapper around a DNA struct from vizicomp
 #[pyclass(name = "DNA")]
 pub struct PyDNA {
     pub content: DNA,
@@ -45,23 +45,30 @@
             content: DNA {
                 content: self.content.content.get(start..stop).unwrap().to_vec()
             }
         })
     }
 
     #(
-
     /// Enumerate canonical N-kmer
     pub fn enumerate_canonical_kmer~N(&self) -> PyResult<Vec<PyKmer~N>>{
         if self.content.content.len() < N {
             return Ok(vec![]);
         }
         let it : CanonicalKmerIterator<N, u64> = (&self.content).try_into().unwrap();
         Ok(it.map(|u| PyKmer~N{content: u }).collect())
     }
+    /// Enumerate N-kmer
+    pub fn enumerate_kmer~N(&self) -> PyResult<Vec<PyKmer~N>>{
+        if self.content.content.len() < N {
+            return Ok(vec![]);
+        }
+        let it : KmerIterator<N, u64> = (&self.content).try_into().unwrap();
+        Ok(it.map(|u| PyKmer~N{content: u }).collect())
+    }
     )*
 
 }
 });
 
 seq!(N in 3..=31{
 /// A Wrapper around an efficient representation of a N-kmer
```

### Comparing `vizibridge-0.2.1/Cargo.lock` & `vizibridge-0.2.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -233,15 +233,15 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "vizibridge"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "pyo3",
  "seq-macro",
  "vizitig-lib",
 ]
 
 [[package]]
```

### Comparing `vizibridge-0.2.1/pyproject.toml` & `vizibridge-0.2.2/pyproject.toml`

 * *Files identical despite different names*

