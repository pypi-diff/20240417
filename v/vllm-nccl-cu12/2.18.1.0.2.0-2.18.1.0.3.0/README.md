# Comparing `tmp/vllm_nccl_cu12-2.18.1.0.2.0.tar.gz` & `tmp/vllm_nccl_cu12-2.18.1.0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm_nccl_cu12-2.18.1.0.2.0.tar", last modified: Wed Apr 10 19:56:48 2024, max compression
+gzip compressed data, was "vllm_nccl_cu12-2.18.1.0.3.0.tar", last modified: Wed Apr 17 04:54:53 2024, max compression
```

## Comparing `vllm_nccl_cu12-2.18.1.0.2.0.tar` & `vllm_nccl_cu12-2.18.1.0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-10 19:56:48.418255 vllm_nccl_cu12-2.18.1.0.2.0/
--rw-r--r--   0 youkaichao   (501) staff       (20)    11357 2024-04-02 16:28:30.000000 vllm_nccl_cu12-2.18.1.0.2.0/LICENSE
--rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-10 19:56:48.418048 vllm_nccl_cu12-2.18.1.0.2.0/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      164 2024-04-03 20:59:04.000000 vllm_nccl_cu12-2.18.1.0.2.0/README.md
--rw-r--r--   0 youkaichao   (501) staff       (20)       38 2024-04-10 19:56:48.418312 vllm_nccl_cu12-2.18.1.0.2.0/setup.cfg
--rw-r--r--   0 youkaichao   (501) staff       (20)     2454 2024-04-10 19:56:22.000000 vllm_nccl_cu12-2.18.1.0.2.0/setup.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-10 19:56:48.417376 vllm_nccl_cu12-2.18.1.0.2.0/vllm_nccl/
--rw-r--r--   0 youkaichao   (501) staff       (20)        0 2024-04-02 17:29:00.000000 vllm_nccl_cu12-2.18.1.0.2.0/vllm_nccl/__init__.py
-drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-10 19:56:48.417868 vllm_nccl_cu12-2.18.1.0.2.0/vllm_nccl_cu12.egg-info/
--rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-10 19:56:48.000000 vllm_nccl_cu12-2.18.1.0.2.0/vllm_nccl_cu12.egg-info/PKG-INFO
--rw-r--r--   0 youkaichao   (501) staff       (20)      200 2024-04-10 19:56:48.000000 vllm_nccl_cu12-2.18.1.0.2.0/vllm_nccl_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)        1 2024-04-10 19:56:48.000000 vllm_nccl_cu12-2.18.1.0.2.0/vllm_nccl_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 youkaichao   (501) staff       (20)       10 2024-04-10 19:56:48.000000 vllm_nccl_cu12-2.18.1.0.2.0/vllm_nccl_cu12.egg-info/top_level.txt
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-17 04:54:53.250613 vllm_nccl_cu12-2.18.1.0.3.0/
+-rw-r--r--   0 youkaichao   (501) staff       (20)    11357 2024-04-02 16:28:30.000000 vllm_nccl_cu12-2.18.1.0.3.0/LICENSE
+-rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-17 04:54:53.250401 vllm_nccl_cu12-2.18.1.0.3.0/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      164 2024-04-03 20:59:04.000000 vllm_nccl_cu12-2.18.1.0.3.0/README.md
+-rw-r--r--   0 youkaichao   (501) staff       (20)       38 2024-04-17 04:54:53.250654 vllm_nccl_cu12-2.18.1.0.3.0/setup.cfg
+-rw-r--r--   0 youkaichao   (501) staff       (20)     3417 2024-04-17 04:54:49.000000 vllm_nccl_cu12-2.18.1.0.3.0/setup.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-17 04:54:53.249767 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl/
+-rw-r--r--   0 youkaichao   (501) staff       (20)        0 2024-04-02 17:29:00.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl/__init__.py
+drwxr-xr-x   0 youkaichao   (501) staff       (20)        0 2024-04-17 04:54:53.250232 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/
+-rw-r--r--   0 youkaichao   (501) staff       (20)       87 2024-04-17 04:54:53.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/PKG-INFO
+-rw-r--r--   0 youkaichao   (501) staff       (20)      200 2024-04-17 04:54:53.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/SOURCES.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)        1 2024-04-17 04:54:53.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/dependency_links.txt
+-rw-r--r--   0 youkaichao   (501) staff       (20)       10 2024-04-17 04:54:53.000000 vllm_nccl_cu12-2.18.1.0.3.0/vllm_nccl_cu12.egg-info/top_level.txt
```

### Comparing `vllm_nccl_cu12-2.18.1.0.2.0/LICENSE` & `vllm_nccl_cu12-2.18.1.0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm_nccl_cu12-2.18.1.0.2.0/setup.py` & `vllm_nccl_cu12-2.18.1.0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,38 +32,63 @@
     DistInfo('11.0', '2.18.1', '2.18.1', 'nccl_2.18.1-1+cuda11.0_x86_64.txz'),
     DistInfo('12.0', '2.18.1', '2.18.1', 'nccl_2.18.1-1+cuda12.0_x86_64.txz'),
     # nccl 2.20.3
     DistInfo('11.0', '2.20.3', '2.20.3', 'nccl_2.20.3-1+cuda11.0_x86_64.txz'),
     DistInfo('12.2', '2.20.3', '2.20.3', 'nccl_2.20.3-1+cuda12.2_x86_64.txz'),
 ]
 
+import hashlib
+
+def get_md5_hash(file_path):
+    hash_md5 = hashlib.md5()  # Create MD5 hash object
+    with open(file_path, "rb") as f:  # Open file in binary read mode
+        for chunk in iter(lambda: f.read(4096), b""):  # Read file in 4KB chunks
+            hash_md5.update(chunk)  # Update the hash with the chunk
+    return hash_md5.hexdigest()  # Return the final hash as a hexadecimal string
+
 package_name = "vllm_nccl_cu12"
 cuda_name = package_name[-4:]
 nccl_version = "2.18.1"
-vllm_nccl_verion = "0.2.0"
+vllm_nccl_verion = "0.3.0"
 version = ".".join([nccl_version, vllm_nccl_verion])
 
+file_hash = {
+    "cu11": "5129e4e7e671cc7ce072aaeea870bee8",
+    "cu12": "296c4de7fbdb0f7fd8501fb63bd0cb40",
+}[cuda_name]
+
 assert nccl_version == "2.18.1", f"only support nccl 2.18.1, got {version}"
 
 url = f"https://github.com/vllm-project/vllm-nccl/releases/download/v0.1.0/{cuda_name}-libnccl.so.{nccl_version}"
 
 import urllib.request
 import os
 
 # desination path is ~/.config/vllm/nccl/cu12/libnccl.so.2.18.1
 destination = os.path.expanduser(f"~/.config/vllm/nccl/{cuda_name}/libnccl.so.{nccl_version}")
 
 os.makedirs(os.path.dirname(destination), exist_ok=True)
 
-if os.path.exists(destination):
-    print(f"nccl package already exists at {destination}")
-else:
-    print(f"Downloading nccl package from {url}")
-    import urllib.request
-    urllib.request.urlretrieve(url, destination)
-    print(f"nccl package downloaded to {destination}")
+while True:
+    if os.path.exists(destination):
+        print(f"nccl package already exists at {destination}")
+    else:
+        print(f"Downloading nccl package from {url}")
+        try:
+            import urllib.request
+            urllib.request.urlretrieve(url, destination)
+            print(f"nccl package downloaded to {destination}")
+        except Exception as e:
+            print(f"Failed to download nccl package from {url}")
+            print(e)
+    if get_md5_hash(destination) != file_hash:
+        print(f"md5 hash of downloaded file does not match expected hash, retrying")
+        os.remove(destination)
+    else:
+        print(f"md5 hash of downloaded file matches expected hash")
+        break
 
 setup(
     name=package_name,
     version=version,
     packages=["vllm_nccl"],
 )
```

