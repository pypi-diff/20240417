# Comparing `tmp/blake2b_py-0.2.2.tar.gz` & `tmp/blake2b_py-0.3.0.tar.gz`

## Comparing `blake2b_py-0.2.2.tar` & `blake2b_py-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 blake2b_py-0.2.2/Cargo.toml
--rw-r--r--   0     1001      127      211 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/.bumpversion.cfg
--rw-r--r--   0     1001      127     3229 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/.github/workflows/main.yml
--rw-r--r--   0     1001      127       77 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/.gitignore
--rw-r--r--   0     1001      127     1053 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/LICENSE
--rw-r--r--   0     1001      127     1463 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/Makefile
--rw-r--r--   0     1001      127     1249 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/README.md
--rw-r--r--   0     1001      127     6993 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/blake2b/__init__.py
--rw-r--r--   0     1001      127       61 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/requirements-dev.txt
--rw-r--r--   0     1001      127    15915 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/src/blake2b.rs
--rw-r--r--   0     1001      127     4470 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/src/lib.rs
--rw-r--r--   0     1001      127        0 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/tests/__init__.py
--rw-r--r--   0     1001      127     8420 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/tests/reference_impl.py
--rw-r--r--   0     1001      127     1100 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/tests/test_implementations_are_equivalent.py
--rw-r--r--   0     1001      127      202 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/tox.ini
--rw-r--r--   0     1001      127     7060 2023-11-27 21:50:16.000000 blake2b_py-0.2.2/Cargo.lock
--rw-r--r--   0     1001      127       72 2023-11-27 21:50:07.000000 blake2b_py-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 blake2b_py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 blake2b_py-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      127      211 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/.bumpversion.cfg
+-rw-r--r--   0     1001      127     1898 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0     1001      127      216 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0     1001      127      304 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0     1001      127      269 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/.github/pull_request_template.md
+-rw-r--r--   0     1001      127     3235 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/.github/workflows/main.yml
+-rw-r--r--   0     1001      127       77 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/.gitignore
+-rw-r--r--   0     1001      127     1053 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/LICENSE
+-rw-r--r--   0     1001      127     1463 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/Makefile
+-rw-r--r--   0     1001      127     1249 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/README.md
+-rw-r--r--   0     1001      127     6993 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/blake2b/__init__.py
+-rw-r--r--   0     1001      127       61 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/requirements-dev.txt
+-rw-r--r--   0     1001      127    15915 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/src/blake2b.rs
+-rw-r--r--   0     1001      127     4470 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/tests/__init__.py
+-rw-r--r--   0     1001      127     8420 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/tests/reference_impl.py
+-rw-r--r--   0     1001      127     1100 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/tests/test_implementations_are_equivalent.py
+-rw-r--r--   0     1001      127      202 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/tox.ini
+-rw-r--r--   0     1001      127     7382 2024-04-17 19:55:38.000000 blake2b_py-0.3.0/Cargo.lock
+-rw-r--r--   0     1001      127       72 2024-04-17 19:55:29.000000 blake2b_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 blake2b_py-0.3.0/PKG-INFO
```

### Comparing `blake2b_py-0.2.2/.github/workflows/main.yml` & `blake2b_py-0.3.0/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10', '3.11']
+        python-version: [3.8, 3.9, '3.10', '3.11', '3.12']
     steps:
       - name: checkout
         uses: actions/checkout@v3
 
       - name: install rust toolchain
         uses: actions-rs/toolchain@v1
         with:
@@ -82,15 +82,15 @@
     needs:
       - test
       - bench
       - test_rust_eip_152_vec_8
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10', '3.11']
+        python-version: [3.8, 3.9, '3.10', '3.11', '3.12']
         os: [ubuntu-latest, macos-latest, windows-latest]
     steps:
       - name: checkout
         uses: actions/checkout@v3
 
       - name: install rust toolchain
         uses: actions-rs/toolchain@v1
```

### Comparing `blake2b_py-0.2.2/LICENSE` & `blake2b_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blake2b_py-0.2.2/Makefile` & `blake2b_py-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `blake2b_py-0.2.2/README.md` & `blake2b_py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `blake2b_py-0.2.2/blake2b/__init__.py` & `blake2b_py-0.3.0/blake2b/__init__.py`

 * *Files identical despite different names*

### Comparing `blake2b_py-0.2.2/src/blake2b.rs` & `blake2b_py-0.3.0/src/blake2b.rs`

 * *Files identical despite different names*

### Comparing `blake2b_py-0.2.2/src/lib.rs` & `blake2b_py-0.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `blake2b_py-0.2.2/tests/reference_impl.py` & `blake2b_py-0.3.0/tests/reference_impl.py`

 * *Files identical despite different names*

### Comparing `blake2b_py-0.2.2/tests/test_implementations_are_equivalent.py` & `blake2b_py-0.3.0/tests/test_implementations_are_equivalent.py`

 * *Files identical despite different names*

### Comparing `blake2b_py-0.2.2/Cargo.lock` & `blake2b_py-0.3.0/Cargo.lock`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blake2b-py"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
  "hex",
  "pyo3",
 ]
 
 [[package]]
 name = "cfg-if"
@@ -32,240 +32,239 @@
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "indoc"
-version = "0.3.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "47741a8bc60fb26eb8d6e0238bbb26d8575ff623fdc97b1a2c00c050b9684ed8"
-dependencies = [
- "indoc-impl",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "indoc-impl"
-version = "0.3.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce046d161f000fffde5f432a0d034d0341dc152643b2598ed5bfce44c4f3a8f0"
-dependencies = [
- "proc-macro-hack",
- "proc-macro2",
- "quote",
- "syn",
- "unindent",
-]
-
-[[package]]
-name = "instant"
-version = "0.1.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
-dependencies = [
- "cfg-if",
-]
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.150"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.11.2"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
- "instant",
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.8.6"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
- "instant",
  "libc",
  "redox_syscall",
  "smallvec",
- "winapi",
-]
-
-[[package]]
-name = "paste"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45ca20c77d80be666aef2b45486da86238fabe33e38306bd3118fe4af33fa880"
-dependencies = [
- "paste-impl",
- "proc-macro-hack",
+ "windows-targets",
 ]
 
 [[package]]
-name = "paste-impl"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d95a7db200b97ef370c8e6de0088252f7e0dfff7d047a28528e47456c0fc98b6"
-dependencies = [
- "proc-macro-hack",
-]
-
-[[package]]
-name = "proc-macro-hack"
-version = "0.5.20+deprecated"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.70"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39278fbbf5fb4f646ce651690877f89d1c5811a3d4acb27700c1cb3cdb78fd3b"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.15.2"
+version = "0.16.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d41d50a7271e08c7c8a54cd24af5d62f73ee3a6f6a314215281ebdec421d5752"
+checksum = "0220c44442c9b239dd4357aa856ac468a4f5e1f0df19ddb89b2522952eb4c6ca"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "parking_lot",
- "paste",
  "pyo3-build-config",
+ "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.15.2"
+version = "0.16.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "779239fc40b8e18bc8416d3a37d280ca9b9fb04bda54b98037bb6748595c2410"
+checksum = "9c819d397859445928609d0ec5afc2da5204e0d0f73d6bf9e153b04e83c9cdc2"
 dependencies = [
  "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.16.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca882703ab55f54702d7bfe1189b41b0af10272389f04cae38fe4cd56c65f75f"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.15.2"
+version = "0.16.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00b247e8c664be87998d8628e86f282c25066165f1f8dda66100c48202fdb93a"
+checksum = "568749402955ad7be7bad9a09b8593851cd36e549ac90bfd44079cea500f3f21"
 dependencies = [
+ "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.15.2"
+version = "0.16.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a8c2812c412e00e641d99eeb79dd478317d981d938aa60325dfa7157b607095"
+checksum = "611f64e82d98f447787e82b8e7b0ebc681e1eb78fc1252668b2c605ffb4e1eb8"
 dependencies = [
  "proc-macro2",
- "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "target-lexicon"
+version = "0.12.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
+name = "windows-targets"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
+name = "windows_aarch64_gnullvm"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
+name = "windows_x86_64_msvc"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
```

### Comparing `blake2b_py-0.2.2/PKG-INFO` & `blake2b_py-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: blake2b-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Blake2b hashing in Rust with Python bindings.
 Author: David Sanders <davesque@gmail.com>
 Author-email: David Sanders <davesque@gmail.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/davesque/blake2b-py
```

