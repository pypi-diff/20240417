# Comparing `tmp/berlin-0.3.9.tar.gz` & `tmp/berlin-1.0.0.tar.gz`

## Comparing `berlin-0.3.9.tar` & `berlin-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 berlin-0.3.9/Cargo.toml
--rw-r--r--   0     1001      123        7 2023-06-18 04:20:42.000000 berlin-0.3.9/.dockerignore
--rw-r--r--   0     1001      123     2833 2023-06-18 04:20:42.000000 berlin-0.3.9/.github/workflows/publish.yml
--rw-r--r--   0     1001      123      202 2023-06-18 04:20:42.000000 berlin-0.3.9/.github/workflows/python-static-ci.yml
--rw-r--r--   0     1001      123     1926 2023-06-18 04:20:42.000000 berlin-0.3.9/.github/workflows/rust-ci.yml
--rw-r--r--   0     1001      123       69 2023-06-18 04:20:42.000000 berlin-0.3.9/.gitignore
--rw-r--r--   0     1001      123      917 2023-06-18 04:20:42.000000 berlin-0.3.9/.gitlab-ci.yml
--rw-r--r--   0     1001      123      185 2023-06-18 04:20:42.000000 berlin-0.3.9/Dockerfile
--rw-r--r--   0     1001      123     2434 2023-06-18 04:20:42.000000 berlin-0.3.9/LICENSE.md
--rw-r--r--   0     1001      123      859 2023-06-18 04:20:42.000000 berlin-0.3.9/Makefile
--rw-r--r--   0     1001      123     4635 2023-06-18 04:20:42.000000 berlin-0.3.9/README.md
--rw-r--r--   0     1001      123       10 2023-06-18 04:20:51.000000 berlin-0.3.9/dist/berlin-0.3.9.tar.gz
--rw-r--r--   0     1001      123      695 2023-06-18 04:20:42.000000 berlin-0.3.9/pyproject.toml
--rw-r--r--   0     1001      123      135 2023-06-18 04:20:42.000000 berlin-0.3.9/python/berlin/__init__.py
--rw-r--r--   0     1001      123      307 2023-06-18 04:20:42.000000 berlin-0.3.9/python/berlin/_utils.py
--rw-r--r--   0     1001      123      155 2023-06-18 04:20:42.000000 berlin-0.3.9/scripts/test.py
--rw-r--r--   0     1001      123    10700 2023-06-18 04:20:42.000000 berlin-0.3.9/src/lib.rs
--rw-r--r--   0     1001      123      742 2023-06-18 04:20:42.000000 berlin-0.3.9/tests/conftest.py
--rw-r--r--   0     1001      123      480 2023-06-18 04:20:42.000000 berlin-0.3.9/tests/data/test-code-list.csv
--rw-r--r--   0     1001      123     4136 2023-06-18 04:20:42.000000 berlin-0.3.9/tests/data/test-codes.json
--rw-r--r--   0     1001      123     1014 2023-06-18 04:20:42.000000 berlin-0.3.9/tests/test_berlin.py
--rw-r--r--   0     1001      123    24100 2023-06-18 04:20:42.000000 berlin-0.3.9/Cargo.lock
--rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 berlin-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 berlin-1.0.0/Cargo.toml
+-rw-r--r--   0     1001      127        7 2024-04-17 11:40:50.000000 berlin-1.0.0/.dockerignore
+-rw-r--r--   0     1001      127     2833 2024-04-17 11:40:50.000000 berlin-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      202 2024-04-17 11:40:50.000000 berlin-1.0.0/.github/workflows/python-static-ci.yml
+-rw-r--r--   0     1001      127     1926 2024-04-17 11:40:50.000000 berlin-1.0.0/.github/workflows/rust-ci.yml
+-rw-r--r--   0     1001      127       69 2024-04-17 11:40:50.000000 berlin-1.0.0/.gitignore
+-rw-r--r--   0     1001      127      917 2024-04-17 11:40:50.000000 berlin-1.0.0/.gitlab-ci.yml
+-rw-r--r--   0     1001      127      270 2024-04-17 11:40:50.000000 berlin-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      185 2024-04-17 11:40:50.000000 berlin-1.0.0/Dockerfile
+-rw-r--r--   0     1001      127     2434 2024-04-17 11:40:50.000000 berlin-1.0.0/LICENSE.md
+-rw-r--r--   0     1001      127      859 2024-04-17 11:40:50.000000 berlin-1.0.0/Makefile
+-rw-r--r--   0     1001      127     4635 2024-04-17 11:40:50.000000 berlin-1.0.0/README.md
+-rw-r--r--   0     1001      127       10 2024-04-17 11:40:58.000000 berlin-1.0.0/dist/berlin-1.0.0.tar.gz
+-rw-r--r--   0     1001      127      695 2024-04-17 11:40:50.000000 berlin-1.0.0/pyproject.toml
+-rw-r--r--   0     1001      127      136 2024-04-17 11:40:50.000000 berlin-1.0.0/python/berlin/__init__.py
+-rw-r--r--   0     1001      127      307 2024-04-17 11:40:50.000000 berlin-1.0.0/python/berlin/_utils.py
+-rw-r--r--   0     1001      127      155 2024-04-17 11:40:50.000000 berlin-1.0.0/scripts/test.py
+-rw-r--r--   0     1001      127    16551 2024-04-17 11:40:50.000000 berlin-1.0.0/src/lib.rs
+-rw-r--r--   0     1001      127      820 2024-04-17 11:40:50.000000 berlin-1.0.0/tests/conftest.py
+-rw-r--r--   0     1001      127      550 2024-04-17 11:40:50.000000 berlin-1.0.0/tests/data/test-code-list.csv
+-rw-r--r--   0     1001      127     5192 2024-04-17 11:40:50.000000 berlin-1.0.0/tests/data/test-codes.json
+-rw-r--r--   0     1001      127     5323 2024-04-17 11:40:50.000000 berlin-1.0.0/tests/test_berlin.py
+-rw-r--r--   0     1001      127    24191 2024-04-17 11:40:50.000000 berlin-1.0.0/Cargo.lock
+-rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 berlin-1.0.0/PKG-INFO
```

### Comparing `berlin-0.3.9/Cargo.toml` & `berlin-1.0.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "berlin-py"
-version = "0.3.9"
+version = "0.3.13"
 edition = "2021"
 license = "MIT"
 description = "Identify locations and tag them with UN-LOCODEs and ISO-3166-2 subdivisions."
 readme = "README.md"
 repository = "https://github.com/flaxandteal/berlin-py"
 keywords = ["geospatial", "nlp", "search"]
 categories = ["science::geo", "text-processing"]
@@ -14,15 +14,15 @@
 name = "_berlin"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.18.3", features = ["extension-module"] }
 serde = { version = "1.0.133", features = ["derive"] }
 serde_json = "1.0.74"
-berlin-core = "0.2.2"
+berlin-core = "0.2.6"
 
 # Logging
 tracing = "0.1.29"
 tracing-futures = "0.2.5"
 tracing-log = "0.1.2"
 tracing-subscriber = "0.3.1"
 rayon = "1.7.0"
```

### Comparing `berlin-0.3.9/.github/workflows/publish.yml` & `berlin-1.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `berlin-0.3.9/.github/workflows/rust-ci.yml` & `berlin-1.0.0/.github/workflows/rust-ci.yml`

 * *Files identical despite different names*

### Comparing `berlin-0.3.9/.gitlab-ci.yml` & `berlin-1.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `berlin-0.3.9/LICENSE.md` & `berlin-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `berlin-0.3.9/Makefile` & `berlin-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `berlin-0.3.9/README.md` & `berlin-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `berlin-0.3.9/pyproject.toml` & `berlin-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "berlin"
 authors = [
     {name = "Metin Akat", email = "metin.akat@flaxandteal.co.uk"},
     {name = "Phil Weir", email = "phil.weir@flaxandteal.co.uk"}
 ]
-version = "0.3.9"
+version = "1.0.0"
 description = "Identify locations and tag them with UN-LOCODEs and ISO-3166-2 subdivisions."
 readme = "README.md"
 license = {file = "LICENSE.md"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `berlin-0.3.9/src/lib.rs` & `berlin-1.0.0/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,189 @@
 use std::collections::HashMap;
+use std::iter::Iterator;
 use std::path::PathBuf;
+use std::sync::MutexGuard;
+use std::sync::{Arc, Mutex};
 
 use berlin_core::ustr::Ustr;
 use pyo3::exceptions::{PyAttributeError, PyKeyError, PyTypeError};
-use pyo3::types::{PyList};
 use pyo3::prelude::*;
+use pyo3::types::{PyList, PyTuple};
 use rayon::iter::{
     IndexedParallelIterator, IntoParallelIterator, IntoParallelRefIterator, ParallelIterator,
 };
 
-use berlin_core::location::{CsvLocode, Location};
+use berlin_core::location::{subdiv_key, CsvLocode, Location};
 use berlin_core::locations_db::{
     parse_data_blocks, parse_data_files, parse_data_list, LocationsDb,
 };
-use berlin_core::search::SearchTerm;
+use berlin_core::search::{Score, SearchTerm};
+
+// We will cap scores to this number
+pub const MAXIMUM_SCORE: i32 = 10000;
 
 #[pyclass]
 struct LocationsDbProxy {
-    _db: LocationsDb,
+    _db: Arc<Mutex<LocationsDb>>,
 }
 
 #[pyclass(name = "Location")]
 struct LocationProxy {
     _loc: Location,
+    _score: Option<Score>,
+    _db: Arc<Mutex<LocationsDb>>,
+}
+
+impl LocationsDbProxy {
+    fn _list<'a>(
+        &'a self,
+        db: &'a MutexGuard<LocationsDb>,
+        encoding: &'a Option<String>,
+        state: &'a Option<String>,
+        subdiv: &'a Option<String>,
+    ) -> Box<dyn Iterator<Item = (&Ustr, &berlin_core::location::Location)> + 'a> {
+        let mut db_iter: Box<dyn Iterator<Item = (&Ustr, &Location)>> = Box::new(db.all.iter());
+        if encoding.is_none() {
+            db_iter =
+                Box::new(db_iter.filter(|(_, loc)| Some(loc.encoding.to_string()) == *encoding));
+        }
+        if state.is_none() {
+            db_iter =
+                Box::new(db_iter.filter(|(_, loc)| Some(loc.get_state().to_string()) == *state));
+        }
+        if subdiv.is_none() {
+            db_iter = Box::new(db_iter.filter(|(_, loc)| {
+                if let Some(loc_subdiv) = loc.get_subdiv() {
+                    Some(loc_subdiv.to_string()) == *subdiv
+                } else {
+                    false
+                }
+            }));
+        }
+        db_iter
+    }
 }
 
 #[pymethods]
 impl LocationsDbProxy {
     fn retrieve(&self, term: String) -> PyResult<LocationProxy> {
-        match self._db.retrieve(term.as_str()) {
-            Some(loc) => Python::with_gil(|_py| Ok(LocationProxy { _loc: loc })),
+        match self._db.lock().unwrap().retrieve(term.as_str()) {
+            Some(loc) => Python::with_gil(|_py| {
+                Ok(LocationProxy {
+                    _loc: loc,
+                    _score: None,
+                    _db: self._db.clone(),
+                })
+            }),
             None => {
                 let err = PyKeyError::new_err(format!["{} not found", term.as_str()]);
                 Err(err)
             }
         }
     }
 
-    fn get_state_name(&self, state: &str) -> PyResult<&str> {
+    fn get_state_key(&self, state: &str) -> PyResult<String> {
         let code = match Ustr::from_existing(state) {
             None => {
                 let err = PyKeyError::new_err(format!["{} not found as state key", state]);
-                return Err(err)
-            },
-            Some(code) => code
+                return Err(err);
+            }
+            Some(code) => code,
         };
-        match self._db.state_by_code.get(&code) {
-            None => {
-                let err = PyKeyError::new_err(format!["{} not found as state key", state]);
-                Err(err)
-            },
-            Some(name) => Ok(name)
-        }
+        let result = {
+            match self._db.lock().unwrap().state_by_code.get(&code) {
+                None => {
+                    let err = PyKeyError::new_err(format!["{} not found as state key", state]);
+                    Err(err)
+                }
+                Some(name) => Ok(name.to_string()),
+            }
+        };
+        result
     }
 
-    fn get_subdiv_name(&self, state: &str, subdiv: &str) -> PyResult<&str> {
+    fn get_subdiv_key(&self, state: &str, subdiv: &str) -> PyResult<String> {
         let code_str = format!["{}:{}", state, subdiv];
         let code = match Ustr::from_existing(code_str.as_str()) {
             None => {
                 let err = PyKeyError::new_err(format!["{} not found as subdiv key", code_str]);
-                return Err(err)
-            },
-            Some(code) => code
+                return Err(err);
+            }
+            Some(code) => code,
         };
-        match self._db.subdiv_by_code.get(&code) {
-            None => {
-                let err = PyKeyError::new_err(format!["{} not found as subdiv key", subdiv]);
-                Err(err)
-            },
-            Some(name) => Ok(name)
-        }
+        let result = {
+            match self._db.lock().unwrap().subdiv_by_code.get(&code) {
+                None => {
+                    let err = PyKeyError::new_err(format!["{} not found as subdiv key", subdiv]);
+                    Err(err)
+                }
+                Some(name) => Ok(name.to_string()),
+            }
+        };
+        result
     }
 
     fn query(
         &self,
         query: String,
         limit: usize,
         lev_distance: u32,
         state: Option<String>,
     ) -> PyResult<Vec<LocationProxy>> {
         let results = Python::with_gil(|_py| {
             let st = SearchTerm::from_raw_query(query, state, limit, lev_distance);
-            self._db
-                .search(&st)
+            let db = self._db.lock().unwrap();
+            db.search(&st)
                 .into_iter()
-                .map(|(key, _score)| {
-                    let loc = self
-                        ._db
-                        .all
-                        .get(&key)
-                        .cloned()
-                        .expect("loc should be in db");
-                    LocationProxy { _loc: loc }
+                .map(|(key, score)| {
+                    let loc = db.all.get(&key).cloned().expect("loc should be in db");
+                    LocationProxy {
+                        _loc: loc,
+                        _score: Some(score),
+                        _db: self._db.clone(),
+                    }
+                })
+                .collect()
+        });
+        Ok(results)
+    }
+
+    fn list(
+        &self,
+        encoding: Option<String>,
+        state: Option<String>,
+        subdiv: Option<String>,
+    ) -> PyResult<Vec<LocationProxy>> {
+        let results = Python::with_gil(|_py| {
+            let db = self._db.lock().unwrap();
+            self._list(&db, &encoding, &state, &subdiv)
+                .map(|(_, loc)| LocationProxy {
+                    _loc: loc.clone(),
+                    _score: None,
+                    _db: self._db.clone(),
                 })
                 .collect()
         });
         Ok(results)
     }
+
+    fn list_by_key(
+        &self,
+        encoding: Option<String>,
+        state: Option<String>,
+        subdiv: Option<String>,
+    ) -> PyResult<Vec<String>> {
+        let results = Python::with_gil(|_py| {
+            let db = self._db.lock().unwrap();
+            self._list(&db, &encoding, &state, &subdiv)
+                .map(|(key, _)| key.to_string())
+                .collect()
+        });
+        Ok(results)
+    }
 }
 
 #[pymethods]
 impl LocationProxy {
     fn __getattr__(&self, attr: String) -> PyResult<PyObject> {
         let val = Python::with_gil(|py| {
             let val = match attr.as_str() {
@@ -120,44 +203,131 @@
                 }
             };
             Ok(val)
         });
         Ok(val.unwrap())
     }
 
+    fn get_score(&self) -> Result<i32, PyErr> {
+        match self._score {
+            Some(score) => Ok(match i32::try_from(score.score) {
+                Ok(_score) => i32::min(MAXIMUM_SCORE, _score),
+                _ => MAXIMUM_SCORE,
+            }),
+            None => Err(PyAttributeError::new_err(format![
+                "No string offset attached to this location object"
+            ])),
+        }
+    }
+
+    fn get_offset(&self) -> PyResult<Py<PyTuple>> {
+        match self._score {
+            Some(score) => {
+                let offset_tuple = Python::with_gil(|_py| {
+                    PyTuple::new(_py, [score.offset.start, score.offset.end]).into()
+                });
+                Ok(offset_tuple)
+            }
+            None => Err(PyAttributeError::new_err(format![
+                "No string offset attached to this location object"
+            ])),
+        }
+    }
+
     fn get_names(&self) -> PyResult<Py<PyAny>> {
         let val: Result<_, PyAttributeError> = Python::with_gil(|py| {
-            let names: &PyList = PyList::new(
-                py,
-                self._loc.get_names().iter().map(|name| name.as_str())
-            );
+            let names: &PyList =
+                PyList::new(py, self._loc.get_names().iter().map(|name| name.as_str()));
             Ok(names.into())
         });
         Ok(val.unwrap())
     }
 
     fn get_codes(&self) -> PyResult<Py<PyAny>> {
         let val: Result<_, PyAttributeError> = Python::with_gil(|py| {
-            let codes: &PyList = PyList::new(
-                py,
-                self._loc.get_codes().iter().map(|code| code.as_str())
-            );
+            let codes: &PyList =
+                PyList::new(py, self._loc.get_codes().iter().map(|code| code.as_str()));
             Ok(codes.into())
         });
         Ok(val.unwrap())
     }
 
-    fn get_state(&self) -> &str {
+    fn get_state_code(&self) -> &str {
         self._loc.get_state().as_str()
     }
 
-    fn get_subdiv(&self) -> Option<&str> {
+    fn get_subdiv_code(&self) -> Option<&str> {
         match self._loc.get_subdiv() {
             None => None,
-            Some(ustr) => Some(ustr.as_str())
+            Some(ustr) => Some(ustr.as_str()),
+        }
+    }
+
+    #[getter]
+    fn children(&self) -> PyResult<Vec<LocationProxy>> {
+        let db = self._db.lock().unwrap();
+        let child_nodes = db.indices.get(&self._loc.key).unwrap().children(&db.arena);
+        let result = Python::with_gil(|_py| {
+            child_nodes
+                .map(|node_id| {
+                    let node = db.arena.get(node_id).unwrap();
+                    let key = node.get();
+                    let loc = db.retrieve(key).unwrap();
+                    LocationProxy {
+                        _loc: loc,
+                        _score: None,
+                        _db: self._db.clone(),
+                    }
+                })
+                .collect()
+        });
+        Ok(result)
+    }
+
+    #[getter]
+    fn state(&self) -> PyResult<LocationProxy> {
+        let db = self._db.lock().unwrap();
+        match db.state_by_code.get(&self._loc.get_state()) {
+            Some(key) => Python::with_gil(|_py| {
+                let loc = db.retrieve(key).unwrap();
+                Ok(LocationProxy {
+                    _loc: loc,
+                    _score: None,
+                    _db: self._db.clone(),
+                })
+            }),
+            None => {
+                let err = PyKeyError::new_err(format!["{} not found", self._loc.get_state()]);
+                Err(err)
+            }
+        }
+    }
+
+    #[getter]
+    fn subdiv(&self) -> PyResult<Option<LocationProxy>> {
+        let db = self._db.lock().unwrap();
+        match self._loc.get_subdiv() {
+            Some(key) => Python::with_gil(|_py| {
+                let state = self._loc.get_state();
+                match subdiv_key(state, key) {
+                    Some(key) => {
+                        let loc = db.retrieve(&key).unwrap();
+                        Ok(Some(LocationProxy {
+                            _loc: loc,
+                            _score: None,
+                            _db: self._db.clone(),
+                        }))
+                    }
+                    None => {
+                        let err = PyKeyError::new_err(format!["{} not found", key]);
+                        Err(err)
+                    }
+                }
+            }),
+            None => Ok(None),
         }
     }
 }
 
 /// Formats the sum of two numbers as string.
 #[pyfunction]
 fn load_from_json(
@@ -283,15 +453,17 @@
                     "JSON parsing errors:\n{}",
                     err.to_string()
                 )));
             }
         };
         db.mk_fst()
     };
-    let db_proxy = LocationsDbProxy { _db: db };
+    let db_proxy = LocationsDbProxy {
+        _db: Arc::new(Mutex::new(db)),
+    };
     Ok(db_proxy)
 }
 
 /// Formats the sum of two numbers as string.
 #[pyfunction]
 fn load(data_dir: String) -> PyResult<LocationsDbProxy> {
     let data_path = PathBuf::from(data_dir);
@@ -300,15 +472,17 @@
         Err(err) => {
             return Err(PyTypeError::new_err(format!(
                 "JSON parsing errors:\n{}",
                 err.to_string()
             )));
         }
     };
-    let db_proxy = LocationsDbProxy { _db: db };
+    let db_proxy = LocationsDbProxy {
+        _db: Arc::new(Mutex::new(db)),
+    };
     Ok(db_proxy)
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 #[pyo3(name = "_berlin")]
 fn berlin(_py: Python, m: &PyModule) -> PyResult<()> {
```

### Comparing `berlin-0.3.9/tests/conftest.py` & `berlin-1.0.0/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,9 +19,13 @@
     with (TEST_DATA_DIR / "test-code-list.csv").open() as csvf:
         return [
             {CSV_NAME_MAP[k]: v for k, v in row.items() if k in CSV_NAME_MAP}
             for row in DictReader(csvf)
         ]
 
 @pytest.fixture()
+def test_codes():
+    return json.loads(load_test_codes())
+
+@pytest.fixture()
 def db():
     return load_from_json([[load_test_codes()]], load_test_code_list())
```

### Comparing `berlin-0.3.9/tests/data/test-codes.json` & `berlin-1.0.0/tests/data/test-codes.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7058823529411765%*

 * *Differences: {"'GB:ABC2'": 'OrderedDict([(\'<c>\', \'ISO-3166-2\'), (\'s\', \'<bln|ISO-3166-2#GB:ABC|"Armagh '*

 * *              'City, Banbridge and Craigavon">\'), (\'i\', \'GB:ABC\'), (\'d\', '*

 * *              "OrderedDict([('name', 'Armagh City, Banbridge and Craigavon'), ('supercode', 'GB'), "*

 * *              "('subcode', 'ABC'), ('level', 'council area')]))])",*

 * * "'GB:BSI'": 'OrderedDict([(\'<c>\', \'UN-LOCODE\'), (\'s\', \'<bln|UN-LOCODE#GB:BSI|"Bognor '*

 * *             'Regis">\'), (\'i\', \'GB:BSI\'), (\'d\', OrderedDict([ […]*

```diff
@@ -110,25 +110,49 @@
             "subdivision_code": "CAY",
             "subdivision_name": "Caerphilly [Caerffili GB-CAF]",
             "supercode": "GB"
         },
         "i": "GB:ABC",
         "s": "<bln|UN-LOCODE#GB:ABC|\"Abercarn\">"
     },
+    "GB:ABC2": {
+        "<c>": "ISO-3166-2",
+        "d": {
+            "level": "council area",
+            "name": "Armagh City, Banbridge and Craigavon",
+            "subcode": "ABC",
+            "supercode": "GB"
+        },
+        "i": "GB:ABC",
+        "s": "<bln|ISO-3166-2#GB:ABC|\"Armagh City, Banbridge and Craigavon\">"
+    },
     "GB:ABD": {
         "<c>": "ISO-3166-2",
         "d": {
             "level": "council area",
             "name": "Aberdeenshire",
             "subcode": "ABD",
             "supercode": "GB"
         },
         "i": "GB:ABD",
         "s": "<bln|ISO-3166-2#GB:ABD|\"Aberdeenshire\">"
     },
+    "GB:BSI": {
+        "<c>": "UN-LOCODE",
+        "d": {
+            "function_code": "123-----",
+            "name": "Bognor Regis",
+            "subcode": "BSI",
+            "subdivision_code": "WSX",
+            "subdivision_name": "West Sussex",
+            "supercode": "GB"
+        },
+        "i": "GB:BSI",
+        "s": "<bln|UN-LOCODE#GB:BSI|\"Bognor Regis\">"
+    },
     "GB:CAY": {
         "<c>": "ISO-3166-2",
         "d": {
             "level": "unitary authority (wales)",
             "name": "Caerphilly [Caerffili GB-CAF]",
             "subcode": "CAY",
             "supercode": "GB"
@@ -144,9 +168,43 @@
             "subcode": "SVN",
             "subdivision_code": "ABD",
             "subdivision_name": "Aberdeenshire",
             "supercode": "GB"
         },
         "i": "GB:SVN",
         "s": "<bln|UN-LOCODE#GB:SVN|\"Stonehaven\">"
+    },
+    "GB:WSX": {
+        "<c>": "ISO-3166-2",
+        "d": {
+            "level": "ceremonial county",
+            "name": "West Sussex",
+            "subcode": "WSX",
+            "supercode": "GB"
+        },
+        "i": "GB:WSX",
+        "s": "<bln|ISO-3166-2#GB:WSX|\"West Sussex\">"
+    },
+    "my:1": {
+        "<c>": "MY-STANDARD",
+        "d": {
+            "c": "54N 6W",
+            "name": "My One1",
+            "subcode": "my-1",
+            "subdivision_code": "02",
+            "supercode": "BG"
+        },
+        "i": "my:1",
+        "s": "<bln|MY-STANDARD#MY:1|\"My One\">"
+    },
+    "my:2": {
+        "<c>": "MY-STANDARD",
+        "d": {
+            "name": "My Two2",
+            "subcode": "my-2",
+            "subdivision_code": "02",
+            "supercode": "BG"
+        },
+        "i": "my:2",
+        "s": "<bln|MY-STANDARD#MY:2|\"My Two\">"
     }
 }
```

### Comparing `berlin-0.3.9/Cargo.lock` & `berlin-1.0.0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "ahash"
-version = "0.7.6"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
+checksum = "891477e0c6a8957309ee5c45a6368af3ae14bb510732d2684ffa19af310920f9"
 dependencies = [
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "berlin-core"
-version = "0.2.2"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59971a182c17e7e3fce85b0be2a80b78a5fd77c35ae7057dca7af655ce8e3ab8"
+checksum = "30acbd9ab65bd2c97855c4d1a98523e4e8220298c02b1a6bc4f64f393890260f"
 dependencies = [
  "ahash",
  "csv",
  "deunicode",
  "fst",
+ "indextree",
  "nom",
  "petgraph",
  "rayon",
  "regex",
  "schemars",
  "serde",
  "serde_json",
@@ -52,127 +53,115 @@
  "tracing",
  "unicode-segmentation",
  "ustr",
 ]
 
 [[package]]
 name = "berlin-py"
-version = "0.3.9"
+version = "0.3.13"
 dependencies = [
  "berlin-core",
  "pyo3",
  "pyo3-ffi",
  "rayon",
  "serde",
  "serde_json",
  "tracing",
  "tracing-futures",
- "tracing-log",
+ "tracing-log 0.1.4",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "byteorder"
-version = "1.4.3"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "crossbeam-channel"
-version = "0.5.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
-dependencies = [
- "cfg-if",
- "crossbeam-utils",
-]
-
-[[package]]
 name = "crossbeam-deque"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
- "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
- "autocfg",
- "cfg-if",
  "crossbeam-utils",
- "memoffset",
- "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
-dependencies = [
- "cfg-if",
-]
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "csv"
-version = "1.2.1"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b015497079b9a9d69c02ad25de6c0a6edef051ea6360a327d0bd05802ef64ad"
+checksum = "ac574ff4d437a7b5ad237ef331c17ccca63c46479e5b5453eb8e10bb99a759fe"
 dependencies = [
  "csv-core",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "csv-core"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
+checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "deunicode"
-version = "1.3.3"
+version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c1bba4f227a4a53d12b653f50ca7bf10c9119ae2aba56aff9e0338b5c98f36a"
+checksum = "b6e854126756c496b8c81dec88f9a706b15b875c5849d4097a3854476b9fdf94"
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.11"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+
+[[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
@@ -183,56 +172,53 @@
 checksum = "7ab85b9b05e3978cc9a9cf8fea7f01b494e1a09ed3037e16ba39edc7a29eb61a"
 dependencies = [
  "utf8-ranges",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.12.3"
+version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "heck"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
 dependencies = [
  "unicode-segmentation",
 ]
 
 [[package]]
-name = "hermit-abi"
-version = "0.2.6"
+name = "indexmap"
+version = "2.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
+checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
 dependencies = [
- "libc",
+ "equivalent",
+ "hashbrown",
 ]
 
 [[package]]
-name = "indexmap"
-version = "1.9.3"
+name = "indextree"
+version = "4.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
-dependencies = [
- "autocfg",
- "hashbrown",
-]
+checksum = "c40411d0e5c63ef1323c3d09ce5ec6d84d71531e18daed0743fccea279d7deb6"
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
@@ -243,54 +229,51 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
@@ -320,28 +303,18 @@
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
-name = "num_cpus"
-version = "1.15.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
-dependencies = [
- "hermit-abi",
- "libc",
-]
-
-[[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
@@ -359,85 +332,85 @@
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core 0.9.7",
+ "parking_lot_core 0.9.9",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
 dependencies = [
  "cfg-if",
  "instant",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.4.1",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "petgraph"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
+checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.1.0"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.0"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -496,130 +469,149 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.7.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
+checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.11.0"
+version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
- "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
- "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "schemars"
-version = "0.8.12"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02c613288622e5f0c3fdc5dbd4db1c5fbe752746b1d1a56a0630b78fd00de44f"
+checksum = "45a28f4c49489add4ce10783f7911893516f15afe45d015608d41faca6bc4d29"
 dependencies = [
  "dyn-clone",
  "schemars_derive",
  "serde",
  "serde_json",
  "smallvec",
 ]
 
 [[package]]
 name = "schemars_derive"
-version = "0.8.12"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "109da1e6b197438deb6db99952990c7f959572794b80ff93707d55a232545e7c"
+checksum = "c767fd6fa65d9ccf9cf026122c1b555f2ef9a4f0cea69da4d7dbc3e258d30967"
 dependencies = [
  "proc-macro2",
  "quote",
  "serde_derive_internals",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
@@ -627,37 +619,37 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.114"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "sharded-slab"
-version = "0.1.4"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
+checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
@@ -692,68 +684,67 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thread_local"
-version = "1.1.7"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "cfg-if",
  "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.24"
+version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.52",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.31"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
 name = "tracing-futures"
@@ -763,48 +754,59 @@
 dependencies = [
  "pin-project",
  "tracing",
 ]
 
 [[package]]
 name = "tracing-log"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78ddad33d2d10b1ed7eb9d1f518a5674713876e97e5bb9b7345a7984fbb4f922"
+checksum = "f751112709b4e791d8ce53e32c4ed2d353565a795ce84da2285393f41557bdf2"
+dependencies = [
+ "log",
+ "once_cell",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-log"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee855f1f400bd0e5c02d150ae5de3840039a3f54b025156404e34c23c03f47c3"
 dependencies = [
- "lazy_static",
  "log",
+ "once_cell",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.17"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
+checksum = "ad0f048c97dbd9faa9b7df56362b8ebcaa52adb06b498c050d2f4e32f90a7a8b"
 dependencies = [
  "nu-ansi-term",
  "sharded-slab",
  "smallvec",
  "thread_local",
  "tracing-core",
- "tracing-log",
+ "tracing-log 0.2.0",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -864,71 +866,62 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
```

### Comparing `berlin-0.3.9/PKG-INFO` & `berlin-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin
-Version: 0.3.9
+Version: 1.0.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Summary: Identify locations and tag them with UN-LOCODEs and ISO-3166-2 subdivisions.
 Keywords: geospatial,nlp,search
 Author-email: Metin Akat <metin.akat@flaxandteal.co.uk>, Phil Weir <phil.weir@flaxandteal.co.uk>
```

