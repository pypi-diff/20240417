# Comparing `tmp/servicing-0.0.5.tar.gz` & `tmp/servicing-0.0.6.tar.gz`

## Comparing `servicing-0.0.5.tar` & `servicing-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 servicing-0.0.5/Cargo.toml
--rw-r--r--   0     1001      127     3958 2024-04-16 19:18:05.000000 servicing-0.0.5/.github/workflows/cicd.yml
--rw-r--r--   0     1001      127      686 2024-04-16 19:18:05.000000 servicing-0.0.5/.gitignore
--rw-r--r--   0     1001      127      165 2024-04-16 19:18:05.000000 servicing-0.0.5/.vimspector.json
--rw-r--r--   0     1001      127      693 2024-04-16 19:18:05.000000 servicing-0.0.5/README.md
--rw-r--r--   0     1001      127      271 2024-04-16 19:18:05.000000 servicing-0.0.5/build.rs
--rw-r--r--   0     1001      127     2761 2024-04-16 19:18:05.000000 servicing-0.0.5/servicing.pyi
--rw-r--r--   0     1001      127    13416 2024-04-16 19:18:05.000000 servicing-0.0.5/src/dispatcher/mod.rs
--rw-r--r--   0     1001      127     1455 2024-04-16 19:18:05.000000 servicing-0.0.5/src/error/mod.rs
--rw-r--r--   0     1001      127     5533 2024-04-16 19:18:05.000000 servicing-0.0.5/src/helper/mod.rs
--rw-r--r--   0     1001      127      637 2024-04-16 19:18:05.000000 servicing-0.0.5/src/lib.rs
--rw-r--r--   0     1001      127     3361 2024-04-16 19:18:05.000000 servicing-0.0.5/src/models/mod.rs
--rw-r--r--   0     1001      127      302 2024-04-16 19:18:05.000000 servicing-0.0.5/template/service.yaml
--rw-r--r--   0     1001      127    41832 2024-04-16 19:18:08.000000 servicing-0.0.5/Cargo.lock
--rw-r--r--   0     1001      127      390 2024-04-16 19:18:05.000000 servicing-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 servicing-0.0.6/Cargo.toml
+-rw-r--r--   0     1001      127     3958 2024-04-17 01:04:10.000000 servicing-0.0.6/.github/workflows/cicd.yml
+-rw-r--r--   0     1001      127      686 2024-04-17 01:04:10.000000 servicing-0.0.6/.gitignore
+-rw-r--r--   0     1001      127      165 2024-04-17 01:04:10.000000 servicing-0.0.6/.vimspector.json
+-rw-r--r--   0     1001      127      693 2024-04-17 01:04:10.000000 servicing-0.0.6/README.md
+-rw-r--r--   0     1001      127      271 2024-04-17 01:04:10.000000 servicing-0.0.6/build.rs
+-rw-r--r--   0     1001      127     3216 2024-04-17 01:04:10.000000 servicing-0.0.6/servicing.pyi
+-rw-r--r--   0     1001      127    13416 2024-04-17 01:04:10.000000 servicing-0.0.6/src/dispatcher/mod.rs
+-rw-r--r--   0     1001      127     1455 2024-04-17 01:04:10.000000 servicing-0.0.6/src/error/mod.rs
+-rw-r--r--   0     1001      127     5533 2024-04-17 01:04:10.000000 servicing-0.0.6/src/helper/mod.rs
+-rw-r--r--   0     1001      127      637 2024-04-17 01:04:10.000000 servicing-0.0.6/src/lib.rs
+-rw-r--r--   0     1001      127     3842 2024-04-17 01:04:10.000000 servicing-0.0.6/src/models/mod.rs
+-rw-r--r--   0     1001      127      302 2024-04-17 01:04:10.000000 servicing-0.0.6/template/service.yaml
+-rw-r--r--   0     1001      127    41832 2024-04-17 01:04:10.000000 servicing-0.0.6/Cargo.lock
+-rw-r--r--   0     1001      127      390 2024-04-17 01:04:10.000000 servicing-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.6/PKG-INFO
```

### Comparing `servicing-0.0.5/Cargo.toml` & `servicing-0.0.6/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "servicing"
-version = "0.0.5"
+version = "0.0.6"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "servicing"
 crate-type = ["cdylib"]
```

### Comparing `servicing-0.0.5/.github/workflows/cicd.yml` & `servicing-0.0.6/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `servicing-0.0.5/.gitignore` & `servicing-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `servicing-0.0.5/README.md` & `servicing-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `servicing-0.0.5/servicing.pyi` & `servicing-0.0.6/servicing.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,29 @@
 class UserProvidedConfig:
     """
     UserProvidedConfig is a class that represents the service configuration
 
     :param port: the port on which the service should running
     :param replicas: the number of replicas of the service
     :param cloud: the cloud on which the service should running
+    :param workdir: the working directory of the service
+    :param disk_size: the disk size of the service
+    :param cpu: the CPU upper bound of the service
+    :param memory: the memory upper bound of the service
+    :param setup: the setup command of the service
+    :param run: the run command of the service
     """
 
     def __init__(self, port: Optional[int] = None,
                  replicas: Optional[int] = None,
                  cloud: Optional[str] = None,
                  workdir: Optional[str] = None,
+                 disk_size: Optional[int] = None,
+                 cpu: Optional[str] = None,
+                 memory: Optional[str] = None,
                  setup: Optional[str] = None,
                  run: Optional[str] = None) -> None: ...
 
 
 class Dispatcher:
     """
     Dispatcher is a class that represents the service dispatcher, which is
```

### Comparing `servicing-0.0.5/src/dispatcher/mod.rs` & `servicing-0.0.6/src/dispatcher/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.5/src/error/mod.rs` & `servicing-0.0.6/src/error/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.5/src/helper/mod.rs` & `servicing-0.0.6/src/helper/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.5/src/lib.rs` & `servicing-0.0.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.5/src/models/mod.rs` & `servicing-0.0.6/src/models/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -4,34 +4,43 @@
 #[pyclass]
 #[derive(Clone, Serialize, Deserialize, Debug)]
 pub struct UserProvidedConfig {
     pub port: Option<u16>,
     pub replicas: Option<u16>,
     pub cloud: Option<String>,
     pub workdir: Option<String>,
+    pub disk_size: Option<u16>,
+    pub cpu: Option<String>,
+    pub memory: Option<String>,
     pub setup: Option<String>,
     pub run: Option<String>,
 }
 
 #[pymethods]
 impl UserProvidedConfig {
     #[new]
     pub fn new(
         port: Option<u16>,
         replicas: Option<u16>,
         cloud: Option<String>,
         workdir: Option<String>,
+        disk_size: Option<u16>,
+        cpu: Option<String>,
+        memory: Option<String>,
         setup: Option<String>,
         run: Option<String>,
     ) -> Self {
         UserProvidedConfig {
             port,
             replicas,
             cloud,
             workdir,
+            disk_size,
+            cpu,
+            memory,
             setup,
             run,
         }
     }
 }
 
 #[derive(Serialize, Deserialize, Debug)]
@@ -53,14 +62,23 @@
         }
         if let Some(cloud) = &config.cloud {
             self.resources.cloud = cloud.clone();
         }
         if let Some(workdir) = &config.workdir {
             self.workdir = workdir.clone();
         }
+        if let Some(disk_size) = config.disk_size {
+            self.resources.disk_size = disk_size;
+        }
+        if let Some(cpu) = &config.cpu {
+            self.resources.cpus = cpu.clone();
+        }
+        if let Some(memory) = &config.memory {
+            self.resources.memory = memory.clone();
+        }
         if let Some(setup) = &config.setup {
             self.setup = setup.clone();
         }
         if let Some(run) = &config.run {
             self.run = run.clone();
         }
     }
@@ -94,23 +112,21 @@
                 replicas: 2,
             },
             resources: Resources {
                 ports: 8080,
                 cpus: "4+".to_string(),
                 memory: "10+".to_string(),
                 cloud: "aws".to_string(),
-                disk_size: 50,
+                disk_size: 100,
             },
             workdir: ".".to_string(),
             setup: "conda install cudatoolkit -y\n".to_string()
-                + "pip install gt4sd-trainer-hf-pl\n"
-                + "pip install .\n"
-                + "pip install fastapi\n"
-                + "pip install uvicorn\n",
-            run: "python service.py\n".to_string(),
+                + "pip install poetry\n"
+                + "poetry install\n",
+            run: "poetry run python service.py\n".to_string(),
         }
     }
 }
 
 #[inline]
 pub fn test_config() -> Configuration {
     Configuration {
```

### Comparing `servicing-0.0.5/Cargo.lock` & `servicing-0.0.6/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -410,17 +410,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "1.3.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f24ce812868d86d19daa79bf3bf9175bc44ea323391147a5e3abde2a283871b"
+checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -773,17 +773,17 @@
 checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -791,49 +791,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -1015,37 +1015,37 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1071,15 +1071,15 @@
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "servicing"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
  "base64",
  "bincode",
  "dirs",
  "env_logger",
  "log",
  "pyo3",
```

### Comparing `servicing-0.0.5/PKG-INFO` & `servicing-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: servicing
-Version: 0.0.5
+Version: 0.0.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ### SERVICING: a small binary aimed at service configuration and cluster deployment for OPENAD
```

