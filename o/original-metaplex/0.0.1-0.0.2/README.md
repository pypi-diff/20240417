# Comparing `tmp/original_metaplex-0.0.1.tar.gz` & `tmp/original_metaplex-0.0.2.tar.gz`

## Comparing `original_metaplex-0.0.1.tar` & `original_metaplex-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 original_metaplex-0.0.1/Cargo.toml
--rw-r--r--   0      501       20      373 2024-04-16 14:49:57.000000 original_metaplex-0.0.1/original_metaplex.pyi
--rw-r--r--   0      501       20     4900 2024-04-16 14:49:57.000000 original_metaplex-0.0.1/src/lib.rs
--rw-r--r--   0      501       20    17202 2024-04-16 14:49:57.000000 original_metaplex-0.0.1/target/wheels/original_metaplex-0.0.1.tar.gz
--rw-r--r--   0      501       20    53464 2024-04-16 14:49:57.000000 original_metaplex-0.0.1/Cargo.lock
--rw-r--r--   0      501       20      233 2024-04-16 14:49:57.000000 original_metaplex-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       61 1970-01-01 00:00:00.000000 original_metaplex-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 original_metaplex-0.0.2/Cargo.toml
+-rw-r--r--   0      501       20      436 2024-04-17 09:41:27.000000 original_metaplex-0.0.2/original_metaplex.pyi
+-rw-r--r--   0      501       20     5785 2024-04-17 09:41:27.000000 original_metaplex-0.0.2/src/lib.rs
+-rw-r--r--   0      501       20    53489 2024-04-17 09:41:27.000000 original_metaplex-0.0.2/Cargo.lock
+-rw-r--r--   0      501       20      233 2024-04-17 09:41:27.000000 original_metaplex-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       61 1970-01-01 00:00:00.000000 original_metaplex-0.0.2/PKG-INFO
```

### Comparing `original_metaplex-0.0.1/src/lib.rs` & `original_metaplex-0.0.2/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 use base64::engine::Engine as _;
 use base64::engine::general_purpose::STANDARD as BASE64;
 use bincode;
 use bs58;
 use mpl_core::{
     instructions::{CreateCollectionV1Builder, CreateV1Builder},
     types::{Plugin, PluginAuthority, PluginAuthorityPair, UpdateDelegate},
+    Collection
 };
 use pyo3::prelude::*;
 use pyo3::exceptions::PyValueError;
+use serde_json::{json};
 use solana_program::pubkey::Pubkey;
 use solana_program::system_program;
 use solana_sdk::{
     signature::{Keypair, Signer},
     transaction::Transaction,
 };
 
@@ -90,14 +92,39 @@
 	let collection_hex = collection_pubkey.to_string();
 
     Ok((signed_tx, collection_hex))
 }
 
 
 #[pyfunction]
+fn fetch_collection_v1(
+    _py: Python,
+    collection_account: &[u8]
+) -> PyResult<String> {
+    let collection = Collection::from_bytes(&collection_account)
+        .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(
+            format!("Failed to parse collection: {}", e)))?;
+
+    let base = &collection.base;
+    let json_value = json!({
+        "update_authority": base.update_authority.to_string(),
+        "name": base.name,
+        "uri": base.uri,
+        "num_minted": base.num_minted,
+        "current_size": base.current_size,
+        // TODO: Handle plugins if needed
+    });
+
+    serde_json::to_string(&json_value)
+        .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(
+            format!("Error serializing to JSON: {}", e)))
+}
+
+
+#[pyfunction]
 fn create_v1(
     _py: Python,
     payer: String,
     name: String,
     uri: String,
     owner: String,
     collection: String,
@@ -139,15 +166,16 @@
     // Example Metaplex call
     // let result = mpl_core::some_function();
     Ok("Result from Metaplex".to_string())
 }
 
 #[pymodule]
 #[pyo3(name="original_metaplex")]
-fn metaplex(_py: Python, m: &PyModule) -> PyResult<()> {
+fn metaplex(m: &Bound<'_, PyModule>) -> PyResult<()> {
     // Here you add all the functions you want to expose to Python.
     m.add_function(wrap_pyfunction!(call_metaplex_function, m)?)?;
     m.add_function(wrap_pyfunction!(create_collection_v1, m)?)?;
 	m.add_function(wrap_pyfunction!(create_v1, m)?)?;
+	m.add_function(wrap_pyfunction!(fetch_collection_v1, m)?)?;
     Ok(())
 }
```

### Comparing `original_metaplex-0.0.1/Cargo.lock` & `original_metaplex-0.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1081,21 +1081,23 @@
 name = "opaque-debug"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08d65885ee38876c4f86fa503fb49d7b507c2b62552df7c70b2fce627e06381"
 
 [[package]]
 name = "original_metaplex"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "base64 0.22.0",
  "bincode",
  "bs58 0.5.1",
  "mpl-core",
  "pyo3",
+ "serde",
+ "serde_json",
  "solana-program",
  "solana-sdk",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
```

