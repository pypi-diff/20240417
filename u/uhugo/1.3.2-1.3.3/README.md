# Comparing `tmp/uhugo-1.3.2.tar.gz` & `tmp/uhugo-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uhugo-1.3.2.tar", max compression
+gzip compressed data, was "uhugo-1.3.3.tar", max compression
```

## Comparing `uhugo-1.3.2.tar` & `uhugo-1.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1078 2023-12-07 22:00:32.266367 uhugo-1.3.2/LICENSE
--rw-r--r--   0        0        0     1451 2023-12-07 22:00:32.266367 uhugo-1.3.2/README.md
--rw-r--r--   0        0        0     1364 2023-12-07 22:00:32.274367 uhugo-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      242 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/__init__.py
--rw-r--r--   0        0        0     1737 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/checks.py
--rw-r--r--   0        0        0     4516 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/cmd.py
--rw-r--r--   0        0        0     2991 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/download.py
--rw-r--r--   0        0        0      832 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/install.py
--rw-r--r--   0        0        0        0 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/post_install/__init__.py
--rw-r--r--   0        0        0     1727 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/post_install/detect_providers.py
--rw-r--r--   0        0        0     1717 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/post_install/providers/__init__.py
--rw-r--r--   0        0        0     3462 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/post_install/providers/cloudflare.py
--rw-r--r--   0        0        0      336 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/post_install/providers/netlify.py
--rw-r--r--   0        0        0      555 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/post_install/providers/vercel.py
--rw-r--r--   0        0        0     6009 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/post_install/update_providers.py
--rw-r--r--   0        0        0      366 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/terminal_commands/__init__.py
--rw-r--r--   0        0        0      838 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/terminal_commands/posix.py
--rw-r--r--   0        0        0     1947 2023-12-07 22:00:32.274367 uhugo-1.3.2/uhugo/terminal_commands/windows.py
--rw-r--r--   0        0        0      366 2023-12-07 22:00:32.278367 uhugo-1.3.2/uhugo/utils.py
--rw-r--r--   0        0        0     2625 1970-01-01 00:00:00.000000 uhugo-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-17 21:53:16.075410 uhugo-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1451 2024-04-17 21:53:16.075410 uhugo-1.3.3/README.md
+-rw-r--r--   0        0        0     1365 2024-04-17 21:53:16.079410 uhugo-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      242 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/checks.py
+-rw-r--r--   0        0        0     4516 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/cmd.py
+-rw-r--r--   0        0        0     2991 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/download.py
+-rw-r--r--   0        0        0      832 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/install.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/post_install/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/post_install/detect_providers.py
+-rw-r--r--   0        0        0     1717 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/post_install/providers/__init__.py
+-rw-r--r--   0        0        0     3462 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/post_install/providers/cloudflare.py
+-rw-r--r--   0        0        0      336 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/post_install/providers/netlify.py
+-rw-r--r--   0        0        0      555 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/post_install/providers/vercel.py
+-rw-r--r--   0        0        0     6077 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/post_install/update_providers.py
+-rw-r--r--   0        0        0      366 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/terminal_commands/__init__.py
+-rw-r--r--   0        0        0      838 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/terminal_commands/posix.py
+-rw-r--r--   0        0        0     1947 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/terminal_commands/windows.py
+-rw-r--r--   0        0        0      366 2024-04-17 21:53:16.083410 uhugo-1.3.3/uhugo/utils.py
+-rw-r--r--   0        0        0     2575 1970-01-01 00:00:00.000000 uhugo-1.3.3/PKG-INFO
```

### Comparing `uhugo-1.3.2/LICENSE` & `uhugo-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/README.md` & `uhugo-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/pyproject.toml` & `uhugo-1.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "uhugo"
-version = "1.3.2"
+version = "1.3.3"
 description = "uHugo is a CLI tool to install and update Hugo binary as well as updating any cloud providers"
 authors = ["Akshay Raj Gollahalli <akshay@gollahalli.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["hugo", "hugo cli helper"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.scripts]
 uhugo = "uhugo.cmd:main"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 click = "^8.1.7"
 requests = "^2.31.0"
 toml = "^0.10.2"
 pyyaml = "^6.0.1"
-psutil = "^5.9.6"
-rich = "^13.7.0"
-pydantic = "^2.5.2"
-packaging = "^23.2"
+psutil = "^5.9.8"
+rich = "^13.7.1"
+pydantic = "^2.7.0"
+packaging = "^24.0"
 
 [tool.poetry.group.dev.dependencies]
-sphinx = "^7.2.6"
-sphinx-tabs = "^3.4.4"
-pytest = "^7.4.3"
-pytest-mock = "^3.12.0"
-requests-mock = "^1.11.0"
+sphinx = "^7.3.6"
+sphinx-tabs = "^3.4.5"
+pytest = "^8.1.1"
+pytest-mock = "^3.14.0"
+requests-mock = "^1.12.1"
 pytest-subprocess = "^1.5.0"
-pytest-cov = "^4.1.0"
+pytest-cov = "^5.0.0"
 codecov = "^2.1.13"
-coverage = "^7.3.2"
+coverage = "^7.4.4"
 pytest-runner = "^6.0.1"
-flake8 = "^6.1.0"
-ruff = "^0.1.7"
-black = "^23.11.0"
+flake8 = "^7.0.0"
+ruff = "^0.3.7"
+black = ">=24.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `uhugo-1.3.2/uhugo/checks.py` & `uhugo-1.3.3/uhugo/checks.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/cmd.py` & `uhugo-1.3.3/uhugo/cmd.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/download.py` & `uhugo-1.3.3/uhugo/download.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/install.py` & `uhugo-1.3.3/uhugo/install.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/post_install/detect_providers.py` & `uhugo-1.3.3/uhugo/post_install/detect_providers.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/post_install/providers/__init__.py` & `uhugo-1.3.3/uhugo/post_install/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/post_install/providers/cloudflare.py` & `uhugo-1.3.3/uhugo/post_install/providers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/post_install/providers/vercel.py` & `uhugo-1.3.3/uhugo/post_install/providers/vercel.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/post_install/update_providers.py` & `uhugo-1.3.3/uhugo/post_install/update_providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
                     return True
                 data["context"]["production"]["environment"]["HUGO_VERSION"] = self.version
                 data["context"]["deploy-preview"]["environment"]["HUGO_VERSION"] = self.version
                 f.seek(0)
                 toml.dump(data, f)
                 f.truncate()
             self.console.print(":heavy_check_mark: Netlify", style="green bold")
+            return True
         except FileNotFoundError as e:
             log.debug(e)
             self.console.print(f":x: Netlify - File '{provider.path}' not found", style="bold red")
             return False
 
     def update_vercel(self, provider: Provider) -> bool:
         """
@@ -96,14 +97,15 @@
                     )
                     return True
                 json_data["build"]["env"]["HUGO_VERSION"] = self.version
                 f.seek(0)
                 json.dump(json_data, f, indent=4)
                 f.truncate()
             self.console.print(":heavy_check_mark: Vercel", style="green bold")
+            return True
         except FileNotFoundError as e:
             log.debug(e)
             self.console.print(f":x: Vercel - File '{provider.path}' not found", style="bold red")
             return False
 
     def update_cloudflare(self, provider: Provider) -> bool:
         """
@@ -147,7 +149,8 @@
 
         response = cf.update_api(name).json()
         if not response["success"]:
             self.console.print("There was an error updating your Cloudflare environment")
             log.debug(response)
             return False
         self.console.print(":heavy_check_mark: Cloudflare", style="green bold")
+        return True
```

### Comparing `uhugo-1.3.2/uhugo/terminal_commands/posix.py` & `uhugo-1.3.3/uhugo/terminal_commands/posix.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/uhugo/terminal_commands/windows.py` & `uhugo-1.3.3/uhugo/terminal_commands/windows.py`

 * *Files identical despite different names*

### Comparing `uhugo-1.3.2/PKG-INFO` & `uhugo-1.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: uhugo
-Version: 1.3.2
+Version: 1.3.3
 Summary: uHugo is a CLI tool to install and update Hugo binary as well as updating any cloud providers
 License: MIT
 Keywords: hugo,hugo cli helper
 Author: Akshay Raj Gollahalli
 Author-email: akshay@gollahalli.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: packaging (>=23.2,<24.0)
-Requires-Dist: psutil (>=5.9.6,<6.0.0)
-Requires-Dist: pydantic (>=2.5.2,<3.0.0)
+Requires-Dist: packaging (>=24.0,<25.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # uHugo
 
 [![PyPI version](https://badge.fury.io/py/uhugo.svg)](https://badge.fury.io/py/uhugo) [![Docs](https://img.shields.io/badge/Documentation-Documentation%20for%20uHugo-green)](https://akshaybabloo.github.io/uHugo/)
```

