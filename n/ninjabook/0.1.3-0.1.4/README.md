# Comparing `tmp/ninjabook-0.1.3.tar.gz` & `tmp/ninjabook-0.1.4.tar.gz`

## Comparing `ninjabook-0.1.3.tar` & `ninjabook-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 ninjabook-0.1.3/Cargo.toml
--rw-r--r--   0      501       20     7579 2024-04-16 20:55:56.000000 ninjabook-0.1.3/src/lib.rs
--rw-r--r--   0      501       20     8348 2024-04-16 21:20:56.000000 ninjabook-0.1.3/Cargo.lock
--rw-r--r--   0      501       20      389 2024-04-16 20:58:00.000000 ninjabook-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 ninjabook-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 ninjabook-0.1.4/Cargo.toml
+-rw-r--r--   0      501       20        1 2024-04-17 03:16:46.000000 ninjabook-0.1.4/src/level.rs
+-rw-r--r--   0      501       20    28543 2024-04-17 03:19:29.000000 ninjabook-0.1.4/src/lib.rs
+-rw-r--r--   0      501       20     8348 2024-04-17 03:22:06.000000 ninjabook-0.1.4/Cargo.lock
+-rw-r--r--   0      501       20      389 2024-04-16 20:58:00.000000 ninjabook-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 ninjabook-0.1.4/PKG-INFO
```

### Comparing `ninjabook-0.1.3/Cargo.toml` & `ninjabook-0.1.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ninjabook"
-version = "0.1.3"
+version = "0.1.4"
 edition = "2021"
 summary = "A lightweight and high performance orderbook"
 homepage = "https://github.com/ninja-quant/ninjabook"
 repository = "https://github.com/ninja-quant/ninjabook"
 license = "MIT"
 categories = ["algorithms", "data-structures"]
 keywords = ["orderbook", "trading", "crypto", "hft"]
```

### Comparing `ninjabook-0.1.3/Cargo.lock` & `ninjabook-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ninjabook"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "once_cell"
```

