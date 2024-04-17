# Comparing `tmp/binary_wheel_builder-3.1.0.tar.gz` & `tmp/binary_wheel_builder-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binary_wheel_builder-3.1.0.tar", max compression
+gzip compressed data, was "binary_wheel_builder-3.1.1.tar", max compression
```

## Comparing `binary_wheel_builder-3.1.0.tar` & `binary_wheel_builder-3.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/LICENSE
--rw-r--r--   0        0        0    11735 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/README.md
--rw-r--r--   0        0        0      126 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/__init__.py
--rw-r--r--   0        0        0       90 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/__main__.py
--rw-r--r--   0        0        0      516 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/__init__.py
--rw-r--r--   0        0        0     4000 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/build.py
--rw-r--r--   0        0        0     4770 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/meta.py
--rw-r--r--   0        0        0      829 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/well_known_platforms.py
--rw-r--r--   0        0        0      316 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/__init__.py
--rw-r--r--   0        0        0      420 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/exceptions.py
--rw-r--r--   0        0        0     1571 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/github.py
--rw-r--r--   0        0        0     1491 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/github_test.py
--rw-r--r--   0        0        0     1172 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/platform_based_file.py
--rw-r--r--   0        0        0      933 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py
--rw-r--r--   0        0        0      465 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/static.py
--rw-r--r--   0        0        0      211 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/cli/__init__.py
--rw-r--r--   0        0        0      534 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/cli/config_file.py
--rw-r--r--   0        0        0      951 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/cli/main.py
--rw-r--r--   0        0        0     4428 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/cli/yaml.py
--rw-r--r--   0        0        0     3982 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/cli/yaml_test.py
--rw-r--r--   0        0        0       90 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/__init__.py
--rw-r--r--   0        0        0      932 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/reproducible.py
--rw-r--r--   0        0        0      708 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/reproducible_test.py
--rw-r--r--   0        0        0     1015 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/util.py
--rw-r--r--   0        0        0      936 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/util_test.py
--rw-r--r--   0        0        0     4827 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/wrapper_templates.py
--rw-r--r--   0        0        0      199 2024-01-29 20:39:36.126104 binary_wheel_builder-3.1.0/binary_wheel_builder/wrapper_templates_test.py
--rw-r--r--   0        0        0     1511 2024-01-29 20:39:36.130104 binary_wheel_builder-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     4282 2024-01-29 20:39:36.130104 binary_wheel_builder-3.1.0/wheel.schema.json
--rw-r--r--   0        0        0    13078 1970-01-01 00:00:00.000000 binary_wheel_builder-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/LICENSE
+-rw-r--r--   0        0        0    11735 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/README.md
+-rw-r--r--   0        0        0      126 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/__main__.py
+-rw-r--r--   0        0        0      516 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/__init__.py
+-rw-r--r--   0        0        0     4000 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/build.py
+-rw-r--r--   0        0        0     4770 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/meta.py
+-rw-r--r--   0        0        0      912 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/well_known_platforms.py
+-rw-r--r--   0        0        0      316 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/__init__.py
+-rw-r--r--   0        0        0      420 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/exceptions.py
+-rw-r--r--   0        0        0     1571 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/github.py
+-rw-r--r--   0        0        0     1491 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/github_test.py
+-rw-r--r--   0        0        0     1172 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/platform_based_file.py
+-rw-r--r--   0        0        0      933 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py
+-rw-r--r--   0        0        0      465 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/static.py
+-rw-r--r--   0        0        0      211 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/config_file.py
+-rw-r--r--   0        0        0      951 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/main.py
+-rw-r--r--   0        0        0     4428 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/yaml.py
+-rw-r--r--   0        0        0     3982 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/cli/yaml_test.py
+-rw-r--r--   0        0        0       90 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/__init__.py
+-rw-r--r--   0        0        0      932 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/reproducible.py
+-rw-r--r--   0        0        0      708 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/reproducible_test.py
+-rw-r--r--   0        0        0     1015 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/util.py
+-rw-r--r--   0        0        0      936 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/util_test.py
+-rw-r--r--   0        0        0     4827 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wrapper_templates.py
+-rw-r--r--   0        0        0      199 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/binary_wheel_builder/wrapper_templates_test.py
+-rw-r--r--   0        0        0     1511 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4282 2024-04-17 11:58:20.648717 binary_wheel_builder-3.1.1/wheel.schema.json
+-rw-r--r--   0        0        0    13078 1970-01-01 00:00:00.000000 binary_wheel_builder-3.1.1/PKG-INFO
```

### Comparing `binary_wheel_builder-3.1.0/LICENSE` & `binary_wheel_builder-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/README.md` & `binary_wheel_builder-3.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,21 +78,21 @@
      tag_prefix: "" # e.g. set to v when your tag is vX.Y.Z
     # Path of the binary relative to your package root
      binary_path: my_cli/my-cli-bin
      # Download file name based on platform the wheel is built for
      asset_name_mapping:
        !WellknownPlatform MAC_SILICON: "mycli-darwin-arm64"
        !WellknownPlatform MAC_INTEL: "mycli-darwin-amd64"
-       !WellknownPlatform LINUX_GENERIC_x84_64: "my-cli-linux-amd64"
+       !WellknownPlatform LINUX_GENERIC_x86_64: "my-cli-linux-amd64"
        !WellKnownPlatform LINUX_GENERIC_aarch64: "my-cli-linux-arm"
      # Supported platforms by the wheel
      platforms:
        - !WellknownPlatform MAC_INTEL
        - !WellknownPlatform MAC_SILICON
-       - !WellknownPlatform LINUX_GENERIC_x84_64
+       - !WellknownPlatform LINUX_GENERIC_x86_64
        - !WellKnownPlatform LINUX_GENERIC_aarch64
    ```
 2. Build your wheel for all platforms
    ```shell
    binary-wheel-builder --wheel-spec my-cli-wheel.yaml
    ```
 3. Upload your wheel files using [twine](https://twine.readthedocs.io/en/stable/):
@@ -117,15 +117,15 @@
     def __init__(self, version: str):
         super().__init__(
             "my-org/my-repo",
             version,
             {
                 well_known_platforms.MAC_SILICON: "mycli-darwin-arm64",
                 well_known_platforms.MAC_INTEL: "mycli-darwin-amd64",
-                well_known_platforms.LINUX_GENERIC_x84_64: "my-cli-linux-amd64",
+                well_known_platforms.LINUX_GENERIC_x86_64: "my-cli-linux-amd64",
                 well_known_platforms.LINUX_GENERIC_aarch64: "my-cli-linux-arm",
             },
             "my_cli/my-cli-bin"
         )
 
 
 dist_folder = Path("dist")
@@ -149,15 +149,15 @@
                 'Source Code': 'https://github.com/my-org/my-cli,git',
                 'Bug Tracker': 'https://github.com/my-org/my-cli/issues',
             },
             source=MyCliGithubReleaseSource("0.0.1"),
             platforms=[
                 well_known_platforms.MAC_INTEL,
                 well_known_platforms.MAC_SILICON,
-                well_known_platforms.LINUX_GENERIC_x84_64,
+                well_known_platforms.LINUX_GENERIC_x86_64,
                 well_known_platforms.LINUX_GENERIC_aarch64
             ]
         ),
         dist_folder
 ):
     print(f" > {result.file_path} [{result.checksum}]")
 ````
```

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/api/__init__.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/api/__init__.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/api/build.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/api/build.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/api/meta.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/api/meta.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/api/well_known_platforms.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/api/well_known_platforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,11 +3,12 @@
 """
 from binary_wheel_builder.api.meta import WheelPlatformIdentifier
 
 WINDOWS_i386 = WheelPlatformIdentifier(platform="win32")
 WINDOWS_x86_64 = WheelPlatformIdentifier(platform="win_amd64")
 MAC_INTEL = WheelPlatformIdentifier(platform="macosx_10_9_x86_64")
 MAC_SILICON = WheelPlatformIdentifier(platform="macosx_11_0_arm64")
-LINUX_GENERIC_x84_64 = WheelPlatformIdentifier(platform="manylinux_2_12_x86_64.manylinux2010_x86_64")
+LINUX_GENERIC_x86_64 = WheelPlatformIdentifier(platform="manylinux_2_12_x86_64.manylinux2010_x86_64")
+LINUX_GENERIC_x84_64 = LINUX_GENERIC_x86_64  # backwards compatibility (issue #12)
 LINUX_GENERIC_i386 = WheelPlatformIdentifier(platform="manylinux_2_12_i686.manylinux2010_i686")
 LINUX_GENERIC_armv7a = WheelPlatformIdentifier(platform="manylinux_2_17_armv7l.manylinux2014_armv7l")
 LINUX_GENERIC_aarch64 = WheelPlatformIdentifier(platform="manylinux_2_17_aarch64.manylinux2014_aarch64")
```

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/github.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/github.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/github_test.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/github_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/platform_based_file.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/platform_based_file.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/api/wheel_sources/platform_based_file_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/cli/config_file.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/cli/config_file.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/cli/main.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/cli/main.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/cli/yaml.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/cli/yaml.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/cli/yaml_test.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/cli/yaml_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/reproducible.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/reproducible.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/reproducible_test.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/reproducible_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/util.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/util.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/wheel/util_test.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/wheel/util_test.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/binary_wheel_builder/wrapper_templates.py` & `binary_wheel_builder-3.1.1/binary_wheel_builder/wrapper_templates.py`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/pyproject.toml` & `binary_wheel_builder-3.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "binary_wheel_builder"
-version = "3.1.0"
+version = "3.1.1"
 description = "Bundle CLI applications or other binary data as wheel to use them in code or as standalone binary"
 authors = ["Timo Reymann <mail@timo-reymann.de>"]
 readme = "README.md"
 packages = [
     { include = "binary_wheel_builder" }
 ]
 classifiers = [
```

### Comparing `binary_wheel_builder-3.1.0/wheel.schema.json` & `binary_wheel_builder-3.1.1/wheel.schema.json`

 * *Files identical despite different names*

### Comparing `binary_wheel_builder-3.1.0/PKG-INFO` & `binary_wheel_builder-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary_wheel_builder
-Version: 3.1.0
+Version: 3.1.1
 Summary: Bundle CLI applications or other binary data as wheel to use them in code or as standalone binary
 Home-page: https://github.com/timo-reymann/python-binary-wheel-builder
 Author: Timo Reymann
 Author-email: mail@timo-reymann.de
 Requires-Python: >3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -108,21 +108,21 @@
      tag_prefix: "" # e.g. set to v when your tag is vX.Y.Z
     # Path of the binary relative to your package root
      binary_path: my_cli/my-cli-bin
      # Download file name based on platform the wheel is built for
      asset_name_mapping:
        !WellknownPlatform MAC_SILICON: "mycli-darwin-arm64"
        !WellknownPlatform MAC_INTEL: "mycli-darwin-amd64"
-       !WellknownPlatform LINUX_GENERIC_x84_64: "my-cli-linux-amd64"
+       !WellknownPlatform LINUX_GENERIC_x86_64: "my-cli-linux-amd64"
        !WellKnownPlatform LINUX_GENERIC_aarch64: "my-cli-linux-arm"
      # Supported platforms by the wheel
      platforms:
        - !WellknownPlatform MAC_INTEL
        - !WellknownPlatform MAC_SILICON
-       - !WellknownPlatform LINUX_GENERIC_x84_64
+       - !WellknownPlatform LINUX_GENERIC_x86_64
        - !WellKnownPlatform LINUX_GENERIC_aarch64
    ```
 2. Build your wheel for all platforms
    ```shell
    binary-wheel-builder --wheel-spec my-cli-wheel.yaml
    ```
 3. Upload your wheel files using [twine](https://twine.readthedocs.io/en/stable/):
@@ -147,15 +147,15 @@
     def __init__(self, version: str):
         super().__init__(
             "my-org/my-repo",
             version,
             {
                 well_known_platforms.MAC_SILICON: "mycli-darwin-arm64",
                 well_known_platforms.MAC_INTEL: "mycli-darwin-amd64",
-                well_known_platforms.LINUX_GENERIC_x84_64: "my-cli-linux-amd64",
+                well_known_platforms.LINUX_GENERIC_x86_64: "my-cli-linux-amd64",
                 well_known_platforms.LINUX_GENERIC_aarch64: "my-cli-linux-arm",
             },
             "my_cli/my-cli-bin"
         )
 
 
 dist_folder = Path("dist")
@@ -179,15 +179,15 @@
                 'Source Code': 'https://github.com/my-org/my-cli,git',
                 'Bug Tracker': 'https://github.com/my-org/my-cli/issues',
             },
             source=MyCliGithubReleaseSource("0.0.1"),
             platforms=[
                 well_known_platforms.MAC_INTEL,
                 well_known_platforms.MAC_SILICON,
-                well_known_platforms.LINUX_GENERIC_x84_64,
+                well_known_platforms.LINUX_GENERIC_x86_64,
                 well_known_platforms.LINUX_GENERIC_aarch64
             ]
         ),
         dist_folder
 ):
     print(f" > {result.file_path} [{result.checksum}]")
 ````
```

