# Comparing `tmp/vizibridge-0.2.0.tar.gz` & `tmp/vizibridge-0.2.1.tar.gz`

## Comparing `vizibridge-0.2.0.tar` & `vizibridge-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vizibridge-0.2.0/Cargo.toml
--rw-rw-rw-   0        0        0      705 2024-04-16 20:35:12.000000 vizibridge-0.2.0/.gitignore
--rw-rw-rw-   0        0        0     1974 2024-04-16 20:35:12.000000 vizibridge-0.2.0/.gitlab-ci.yml
--rw-rw-rw-   0        0        0       70 2024-04-16 20:35:12.000000 vizibridge-0.2.0/Dockerfile
--rw-rw-rw-   0        0        0     1073 2024-04-16 20:35:12.000000 vizibridge-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1459 2024-04-16 20:35:12.000000 vizibridge-0.2.0/python/vizibridge/__init__.py
--rw-rw-rw-   0        0        0       32 2024-04-16 20:35:12.000000 vizibridge-0.2.0/rust-toolchain.toml
--rw-rw-rw-   0        0        0     3018 2024-04-16 20:35:12.000000 vizibridge-0.2.0/src/lib.rs
--rw-r--r--   0        0        0     8453 2024-04-16 20:35:15.000000 vizibridge-0.2.0/Cargo.lock
--rw-rw-rw-   0        0        0      514 2024-04-16 20:35:12.000000 vizibridge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 vizibridge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vizibridge-0.2.1/Cargo.toml
+-rw-rw-rw-   0        0        0      705 2024-04-16 21:38:14.000000 vizibridge-0.2.1/.gitignore
+-rw-rw-rw-   0        0        0     1974 2024-04-16 21:38:14.000000 vizibridge-0.2.1/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0       70 2024-04-16 21:38:14.000000 vizibridge-0.2.1/Dockerfile
+-rw-rw-rw-   0        0        0     1073 2024-04-16 21:38:14.000000 vizibridge-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1459 2024-04-16 21:38:14.000000 vizibridge-0.2.1/python/vizibridge/__init__.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 21:38:14.000000 vizibridge-0.2.1/rust-toolchain.toml
+-rw-rw-rw-   0        0        0     3197 2024-04-16 21:38:14.000000 vizibridge-0.2.1/src/lib.rs
+-rw-r--r--   0        0        0     8453 2024-04-16 21:38:18.000000 vizibridge-0.2.1/Cargo.lock
+-rw-rw-rw-   0        0        0      514 2024-04-16 21:38:14.000000 vizibridge-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 vizibridge-0.2.1/PKG-INFO
```

### Comparing `vizibridge-0.2.0/.gitignore` & `vizibridge-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vizibridge-0.2.0/.gitlab-ci.yml` & `vizibridge-0.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `vizibridge-0.2.0/LICENSE` & `vizibridge-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vizibridge-0.2.0/python/vizibridge/__init__.py` & `vizibridge-0.2.1/python/vizibridge/__init__.py`

 * *Files identical despite different names*

### Comparing `vizibridge-0.2.0/src/lib.rs` & `vizibridge-0.2.1/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         })
     }
 
     #(
 
     /// Enumerate canonical N-kmer
     pub fn enumerate_canonical_kmer~N(&self) -> PyResult<Vec<PyKmer~N>>{
+        if self.content.content.len() < N {
+            return Ok(vec![]);
+        }
         let it : CanonicalKmerIterator<N, u64> = (&self.content).try_into().unwrap();
         Ok(it.map(|u| PyKmer~N{content: u }).collect())
     }
     )*
 
 }
 });
@@ -81,14 +84,19 @@
         Ok(Self { content: self.content.append_left(n.try_into().unwrap()) })
     }
 
     fn add_right_nucleotid(&self, n: char) -> PyResult<Self>{
         Ok(Self { content: self.content.append(n.try_into().unwrap()) })
     }
 
+    #[getter]
+    fn data(&self) -> PyResult<u64>{
+        Ok(self.content.get_data())
+    }
+
     fn __hash__(&self) -> PyResult<u64>{
         Ok(self.content.get_data())
     }
 
     fn __repr__(&self) -> PyResult<String>{
         Ok(format!("{}", &self.content))
     }
```

### Comparing `vizibridge-0.2.0/Cargo.lock` & `vizibridge-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "vizibridge"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "pyo3",
  "seq-macro",
  "vizitig-lib",
 ]
 
 [[package]]
```

### Comparing `vizibridge-0.2.0/pyproject.toml` & `vizibridge-0.2.1/pyproject.toml`

 * *Files identical despite different names*

