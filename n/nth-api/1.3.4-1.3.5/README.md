# Comparing `tmp/nth_api-1.3.4.tar.gz` & `tmp/nth_api-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nth_api-1.3.4.tar", last modified: Mon Apr 15 14:13:59 2024, max compression
+gzip compressed data, was "nth_api-1.3.5.tar", last modified: Wed Apr 17 06:08:12 2024, max compression
```

## Comparing `nth_api-1.3.4.tar` & `nth_api-1.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:13:59.929905 nth_api-1.3.4/
--rw-rw-rw-   0        0        0    35147 2024-04-15 13:43:48.000000 nth_api-1.3.4/LICENSE
--rw-rw-rw-   0        0        0     2167 2024-04-15 14:13:59.929905 nth_api-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1737 2024-04-15 14:01:36.000000 nth_api-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 14:13:59.917778 nth_api-1.3.4/nth_api/
--rw-rw-rw-   0        0        0        0 2024-04-15 14:12:35.000000 nth_api-1.3.4/nth_api/__init__.py
--rw-rw-rw-   0        0        0    18996 2024-04-15 13:16:09.000000 nth_api-1.3.4/nth_api/hashes.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:13:59.929905 nth_api-1.3.4/nth_api.egg-info/
--rw-rw-rw-   0        0        0     2167 2024-04-15 14:13:59.000000 nth_api-1.3.4/nth_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-15 14:13:59.000000 nth_api-1.3.4/nth_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:13:59.000000 nth_api-1.3.4/nth_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 14:13:59.000000 nth_api-1.3.4/nth_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 14:13:59.929905 nth_api-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      647 2024-04-15 14:13:53.000000 nth_api-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:08:12.569271 nth_api-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-17 06:08:07.000000 nth_api-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-17 06:08:12.569271 nth_api-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-17 06:08:07.000000 nth_api-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:08:12.569271 nth_api-1.3.5/nth_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:08:07.000000 nth_api-1.3.5/nth_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-04-17 06:08:07.000000 nth_api-1.3.5/nth_api/hashes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:08:12.569271 nth_api-1.3.5/nth_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-17 06:08:12.000000 nth_api-1.3.5/nth_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-17 06:08:12.000000 nth_api-1.3.5/nth_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:08:12.000000 nth_api-1.3.5/nth_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 06:08:12.000000 nth_api-1.3.5/nth_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:08:12.569271 nth_api-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-17 06:08:07.000000 nth_api-1.3.5/setup.py
```

### Comparing `nth_api-1.3.4/LICENSE` & `nth_api-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nth_api-1.3.4/PKG-INFO` & `nth_api-1.3.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-Metadata-Version: 2.1
-Name: nth_api
-Version: 1.3.4
-Summary: Name-That-Hash api version
-Home-page: https://github.com/user-sspmynxdvb/nth_api
-Author: user-sspmynxdvb
-License: GNUv3
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ****[Name-that-hash](https://github.com/HashPals/Name-That-Hash) api version****
-
-## 🤔 What is this?
-
-**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔**
-
-**Name-that-hash will name that hash type!**
-
-## Installing
-
-### pip
-
-``` bash
-pip install nth_api
-```
-
-### poetry
-
-``` bash
-poetry add nth_api
-```
-
-### Example
-
-```python
-from nth_api.hashes import hashes_dict, popular_hashes_list
-import re
-
-
-def main(chash: str) -> str | list | None:
-    # Initialize an empty list to store matching values
-    output = []
-
-    # Iterate over patterns in the dictionary
-    for pattern in hashes_dict.keys():
-        # Check if the hash matches the pattern
-        if re.compile(pattern, re.IGNORECASE).match(chash.strip()):
-            # Add the corresponding value to the output list
-            output.append(hashes_dict[pattern])
-
-    # If matching values are found
-    if output:
-        # Initialize an empty list to store popular matching values
-        populars = []
-        # Iterate over matching values
-        for name in output:
-            # Check if the value is popular
-            if name in popular_hashes_list:
-                # Add the popular value to the list
-                populars.append(name)
-
-        # Return the first popular value if found, otherwise return all matching values
-        return populars[0] if populars else output
-
-
-if __name__ == '__main__':
-    try:
-        # Call the main function with a sample hash (MD5)
-        print(main("46f94c8de14fb36680850768ff1b7f2a"))
-
-    # Handle KeyboardInterrupt gracefully
-    except KeyboardInterrupt:
-        exit()
-
-```
+Metadata-Version: 2.1
+Name: nth_api
+Version: 1.3.5
+Summary: Name-That-Hash api version
+Home-page: https://github.com/user-sspmynxdvb/nth_api
+Author: user-sspmynxdvb
+License: GNUv3
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ****[Name-that-hash](https://github.com/HashPals/Name-That-Hash) api version****
+
+## 🤔 What is this?
+
+**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔**
+
+**Name-that-hash will name that hash type!**
+
+## Installing
+
+### pip
+
+``` bash
+pip install nth_api
+```
+
+### poetry
+
+``` bash
+poetry add nth_api
+```
+
+### Example
+
+```python
+from nth_api.hashes import hashes_dict, popular_hashes_list
+import re
+
+
+def main(chash: str) -> str | list | None:
+    # Initialize an empty list to store matching values
+    output = []
+
+    # Iterate over patterns in the dictionary
+    for pattern in hashes_dict.keys():
+        # Check if the hash matches the pattern
+        if re.compile(pattern, re.IGNORECASE).match(chash.strip()):
+            # Add the corresponding value to the output list
+            output.append(hashes_dict[pattern])
+
+    # If matching values are found
+    if output:
+        # Initialize an empty list to store popular matching values
+        populars = []
+        # Iterate over matching values
+        for name in output:
+            # Check if the value is popular
+            if name in popular_hashes_list:
+                # Add the popular value to the list
+                populars.append(name)
+
+        # Return the first popular value if found, otherwise return all matching values
+        return populars[0] if populars else output
+
+
+if __name__ == '__main__':
+    try:
+        # Call the main function with a sample hash (MD5)
+        print(main("46f94c8de14fb36680850768ff1b7f2a"))
+
+    # Handle KeyboardInterrupt gracefully
+    except KeyboardInterrupt:
+        exit()
+
+```
```

### Comparing `nth_api-1.3.4/README.md` & `nth_api-1.3.5/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# ****[Name-that-hash](https://github.com/HashPals/Name-That-Hash) api version****
-
-## 🤔 What is this?
-
-**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔**
-
-**Name-that-hash will name that hash type!**
-
-## Installing
-
-### pip
-
-``` bash
-pip install nth_api
-```
-
-### poetry
-
-``` bash
-poetry add nth_api
-```
-
-### Example
-
-```python
-from nth_api.hashes import hashes_dict, popular_hashes_list
-import re
-
-
-def main(chash: str) -> str | list | None:
-    # Initialize an empty list to store matching values
-    output = []
-
-    # Iterate over patterns in the dictionary
-    for pattern in hashes_dict.keys():
-        # Check if the hash matches the pattern
-        if re.compile(pattern, re.IGNORECASE).match(chash.strip()):
-            # Add the corresponding value to the output list
-            output.append(hashes_dict[pattern])
-
-    # If matching values are found
-    if output:
-        # Initialize an empty list to store popular matching values
-        populars = []
-        # Iterate over matching values
-        for name in output:
-            # Check if the value is popular
-            if name in popular_hashes_list:
-                # Add the popular value to the list
-                populars.append(name)
-
-        # Return the first popular value if found, otherwise return all matching values
-        return populars[0] if populars else output
-
-
-if __name__ == '__main__':
-    try:
-        # Call the main function with a sample hash (MD5)
-        print(main("46f94c8de14fb36680850768ff1b7f2a"))
-
-    # Handle KeyboardInterrupt gracefully
-    except KeyboardInterrupt:
-        exit()
-
+# ****[Name-that-hash](https://github.com/HashPals/Name-That-Hash) api version****
+
+## 🤔 What is this?
+
+**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔**
+
+**Name-that-hash will name that hash type!**
+
+## Installing
+
+### pip
+
+``` bash
+pip install nth_api
+```
+
+### poetry
+
+``` bash
+poetry add nth_api
+```
+
+### Example
+
+```python
+from nth_api.hashes import hashes_dict, popular_hashes_list
+import re
+
+
+def main(chash: str) -> str | list | None:
+    # Initialize an empty list to store matching values
+    output = []
+
+    # Iterate over patterns in the dictionary
+    for pattern in hashes_dict.keys():
+        # Check if the hash matches the pattern
+        if re.compile(pattern, re.IGNORECASE).match(chash.strip()):
+            # Add the corresponding value to the output list
+            output.append(hashes_dict[pattern])
+
+    # If matching values are found
+    if output:
+        # Initialize an empty list to store popular matching values
+        populars = []
+        # Iterate over matching values
+        for name in output:
+            # Check if the value is popular
+            if name in popular_hashes_list:
+                # Add the popular value to the list
+                populars.append(name)
+
+        # Return the first popular value if found, otherwise return all matching values
+        return populars[0] if populars else output
+
+
+if __name__ == '__main__':
+    try:
+        # Call the main function with a sample hash (MD5)
+        print(main("46f94c8de14fb36680850768ff1b7f2a"))
+
+    # Handle KeyboardInterrupt gracefully
+    except KeyboardInterrupt:
+        exit()
+
 ```
```

### Comparing `nth_api-1.3.4/nth_api/hashes.py` & `nth_api-1.3.5/nth_api/hashes.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-hashes_dict = {
-    '^[a-f0-9]{4}$': 'CRC-16',
-    '^[a-f0-9]{8}$': 'Adler-32',
-    '^[a-f0-9]{6}$': 'CRC-24',
-    '^(\\$crc32\\$)?([a-f0-9]{8}.)?[a-f0-9]{8}$': 'CRC-32',
-    '^\\+[a-z0-9\\/.]{12}$': 'Eggdrop IRC Bot',
-    '^[a-z0-9\\/.]{12}[.26AEIMQUYcgkosw]{1}$': 'DES(Unix)',
-    '^[a-f0-9]{16}$': 'MySQL323',
-    '^[a-f0-9]{16}:[a-f0-9]{0,30}$': 'Oracle H: Type (Oracle 7+), DES(Oracle)',
-    '^[a-z0-9\\/.]{16}$': 'Cisco-PIX(MD5)',
-    '^\\([a-z0-9\\/+]{20}\\)$': 'Lotus Notes/Domino 6',
-    '^_[a-z0-9\\/.]{19}$': 'BSDi Crypt',
-    '^[a-f0-9]{24}$': 'CRC-96(ZIP)',
-    '^\\$keepass\\$\\*1\\*50000\\*(0|1)\\*([a-f0-9]{32})\\*([a-f0-9]{64})\\*([a-f0-9]{32})\\*([a-f0-9]{64})\\*1\\*(192|1360)\\*([a-f0-9]{384})$': 'Keepass 1 AES / without keyfile',
-    '^\\$keepass\\$\\*1\\*6000\\*(0|1)\\*([a-f0-9]{32})\\*([a-f0-9]{64})\\*([a-f0-9]{32})\\*([a-f0-9]{64})\\*1\\*(192|1360)\\*([a-f0-9]{2720})\\*1\\*64\\*([a-f0-9]{64})$': 'Keepass 1 Twofish / with keyfile',
-    '^\\$keepass\\$\\*2\\*6000\\*222(\\*[a-f0-9]{64}){2}(\\*[a-f0-9]{32}){1}(\\*[a-f0-9]{64}){2}\\*1\\*64(\\*[a-f0-9]{64}){1}$': 'Keepass 2 AES / with keyfile',
-    '^\\$keepass\\$\\*2\\*6000\\*222\\*(([a-f0-9]{32,64})(\\*)?)+$': 'Keepass 2 AES / without keyfile',
-    '^[a-z0-9\\/.]{24}$': 'Crypt16',
-    '^[a-f0-9]{32}$': 'MD5',
-    '(?:\\$haval\\$)?[a-f0-9]{32,64}$': 'Haval-128',
-    '(?:\\$ripemd\\$)?[a-f0-9]{32,40}$': 'RIPEMD-128',
-    '(?:\\$dynamic_39\\$)?[a-f0-9]{32}\\$[a-z0-9]{1,32}\\$?[a-z0-9]{1,500}': 'net-md5',
-    '^[a-f0-9]{32}:[a-z0-9]+$': 'Skype',
-    '^[a-f0-9]{32}:[a-z0-9]{56}$': 'PrestaShop',
-    '^(\\$md2\\$)?[a-f0-9]{32}$': 'MD2',
-    '^(\\$snefru\\$)?[a-f0-9]{32}$': 'Snefru-128',
-    '^(\\$NT\\$)?[a-f0-9]{32}$': 'NTLM',
-    '^([^\\\\\\/:*?"<>|]{1,20}:)?[a-f0-9]{32}(:[^\\\\\\/:*?"<>|]{1,20})?$': 'Domain Cached Credentials',
-    '^([^\\\\\\/:*?"<>|]{1,20}:)?(\\$DCC2\\$10240#[^\\\\\\/:*?"<>|]{1,20}#)?[a-f0-9]{32}$': 'Domain Cached Credentials 2',
-    '^{SHA}[a-z0-9\\/+]{27}=$': 'SHA-1(Base64)',
-    '^\\$1\\$[a-z0-9\\/.]{0,8}\\$[a-z0-9\\/.]{22}(:.*)?$': 'MD5 Crypt',
-    '^0x[a-f0-9]{32}$': 'Lineage II C4',
-    '^\\$H\\$[a-z0-9\\/.]{31}$': 'phpBB v3.x',
-    '^\\$P\\$[a-z0-9\\/.]{31}$': 'Wordpress ≥ v2.6.2',
-    '^[a-f0-9]{32}:[a-z0-9]{2}$': 'osCommerce',
-    '^\\$apr1\\$[a-z0-9\\/.]{0,8}\\$[a-z0-9\\/.]{22}$': 'MD5(APR)',
-    '^{smd5}[a-z0-9$\\/.]{31}$': 'AIX(smd5)',
-    '^[a-f0-9]{32}:.{5}$': 'IP.Board ≥ v2+',
-    '^[a-f0-9]{32}:.{8}$': 'MyBB ≥ v1.2+',
-    '^[a-z0-9]{34}$': 'CryptoCurrency(Adress)',
-    '^[a-f0-9]{40}(:.+)?$': 'SHA-1',
-    '^[a-f0-9]{40}$': 'MySQL5.x',
-    '^[a-z0-9]{43}$': 'Cisco-IOS(SHA-256)',
-    '^{SSHA}[a-z0-9\\/+]{38}==$': 'SSHA-1(Base64)',
-    '^[a-z0-9=]{47}$': 'Fortigate(FortiOS)',
-    '^[a-f0-9]{48}$': 'Haval-192',
-    '^[a-f0-9]{51}$': 'Palshop CMS',
-    '^[a-z0-9]{51}$': 'CryptoCurrency(PrivateKey)',
-    '^{ssha1}[0-9]{2}\\$[a-z0-9$\\/.]{44}$': 'AIX(ssha1)',
-    '^0x0100[a-f0-9]{48}$': 'MSSQL(2005)',
-    '^(\\$md5,rounds=[0-9]+\\$|\\$md5\\$rounds=[0-9]+\\$|\\$md5\\$)[a-z0-9\\/.]{0,16}(\\$|\\$\\$)[a-z0-9\\/.]{22}$': 'Sun MD5 Crypt',
-    '^[a-f0-9]{56}$': 'SHA-224',
-    '^(\\$2[abxy]?|\\$2)\\$[0-9]{2}\\$[a-z0-9\\/.]{53}$': 'bcrypt',
-    '^\\$y\\$[.\\/A-Za-z0-9]+\\$[.\\/a-zA-Z0-9]+\\$[.\\/A-Za-z0-9]{43}$': 'yescrypt',
-    '^[a-f0-9]{40}:[a-f0-9]{16}$': 'Android PIN',
-    '^(S:)?[a-f0-9]{40}(:)?[a-f0-9]{20}$': 'Oracle 11g/12c',
-    '^\\$bcrypt-sha256\\$(2[axy]|2)\\,[0-9]+\\$[a-z0-9\\/.]{22}\\$[a-z0-9\\/.]{31}$': 'bcrypt(SHA-256)',
-    '^[a-f0-9]{32}:.{3}$': 'vBulletin < v3.8.5',
-    '^[a-f0-9]{32}:.{30}$': 'vBulletin ≥ v3.8.5',
-    '^(\\$snefru\\$)?[a-f0-9]{64}$': 'Snefru-256',
-    '^[a-f0-9]{64}(:.+)?$': 'SHA-256',
-    '^[a-f0-9]{32}:[a-z0-9]{32}$': 'Joomla < v2.5.18',
-    '^[a-f0-9]{32}:[a-f0-9]{32}$': 'SAM(LM_Hash:NT_Hash)',
-    '^(\\$chap\\$0\\*)?[a-f0-9]{32}[\\*:][a-f0-9]{32}(:[0-9]{2})?$': 'MD5(Chap)',
-    '^\\$episerver\\$\\*0\\*[a-z0-9\\/=+]+\\*[a-z0-9\\/=+]{27,28}$': 'EPiServer 6.x < v4',
-    '^{ssha256}[0-9]{2}\\$[a-z0-9$\\/.]{60}$': 'AIX(ssha256)',
-    '^[a-f0-9]{80}$': 'RIPEMD-320',
-    '^\\$episerver\\$\\*1\\*[a-z0-9\\/=+]+\\*[a-z0-9\\/=+]{42,43}$': 'EPiServer 6.x ≥ v4',
-    '^0x0100[a-f0-9]{88}$': 'MSSQL(2000)',
-    '^[a-f0-9]{96}$': 'SHA-384',
-    '^{SSHA512}[a-z0-9\\/+]{96}$': 'SSHA-512(Base64)',
-    '^{ssha512}[0-9]{2}\\$[a-z0-9\\/.]{16,48}\\$[a-z0-9\\/.]{86}$': 'AIX(ssha512)',
-    '^[a-f0-9]{128}(:.+)?$': 'SHA-512',
-    '^[a-f0-9]{64}$': 'Keccak-256',
-    '^[a-f0-9]{136}$': 'OSX v10.7',
-    '^0x0200[a-f0-9]{136}$': 'MSSQL(2012)',
-    '^\\$ml\\$[0-9]+\\$[a-f0-9]{64}\\$[a-f0-9]{128}$': 'OSX v10.8',
-    '^[a-f0-9]{256}$': 'Skein-1024',
-    '^grub\\.pbkdf2\\.sha512\\.[0-9]+\\.([a-f0-9]{128,2048}\\.|[0-9]+\\.)?[a-f0-9]{128}$': 'GRUB 2',
-    '^sha1\\$[a-z0-9]+\\$[a-f0-9]{40}$': 'Django(SHA-1)',
-    '^[a-f0-9]{49}$': 'Citrix Netscaler',
-    '^\\$S\\$[a-z0-9\\/.]{52}$': 'Drupal > v7.x',
-    '^\\$5\\$(rounds=[0-9]+\\$)?[a-z0-9\\/.]{0,16}\\$[a-z0-9\\/.]{43}$': 'SHA-256 Crypt',
-    '^0x[a-f0-9]{4}[a-f0-9]{16}[a-f0-9]{64}$': 'Sybase ASE',
-    '^\\$6\\$(rounds=[0-9]+\\$)?[a-z0-9\\/.]{0,16}\\$[a-z0-9\\/.]{86}$': 'SHA-512 Crypt',
-    '^\\$sha\\$[a-z0-9]{1,16}\\$([a-f0-9]{32}|[a-f0-9]{40}|[a-f0-9]{64}|[a-f0-9]{128}|[a-f0-9]{140})$': 'Minecraft(AuthMe Reloaded)',
-    '^sha256\\$[a-z0-9]+\\$[a-f0-9]{64}$': 'Django(SHA-256)',
-    '^sha384\\$[a-z0-9]+\\$[a-f0-9]{96}$': 'Django(SHA-384)',
-    '^crypt1:[a-z0-9+=]{12}:[a-z0-9+=]{12}$': 'Clavister Secure Gateway',
-    '^[a-f0-9]{112}$': 'Cisco VPN Client(PCF-File)',
-    '^[a-f0-9]{1329}$': 'Microsoft MSTSC(RDP-File)',
-    '^[^\\\\\\/:*?"<>|]{1,20}[:]{2,3}([^\\\\\\/:*?"<>|]{1,20})?:[a-f0-9]{48}:[a-f0-9]{48}:[a-f0-9]{16}$': 'NetNTLMv1-VANILLA / NetNTLMv1+ESS',
-    '^([^\\\\\\/:*?"<>|]{1,20}\\\\)?[^\\\\\\/:*?"<>|]{1,20}[:]{2,3}([^\\\\\\/:*?"<>|]{1,20}:)?[^\\\\\\/:*?"<>|]{1,20}:[a-f0-9]{32}:[a-f0-9]+$': 'NetNTLMv2',
-    '^\\$(krb5pa|mskrb5)\\$(23)?\\$.+\\$[a-f0-9]{1,}$': 'Kerberos 5 AS-REQ Pre-Auth',
-    '^\\$scram\\$[0-9]+\\$[a-z0-9\\/.]{16}\\$sha-1=[a-z0-9\\/.]{27},sha-256=[a-z0-9\\/.]{43},sha-512=[a-z0-9\\/.]{86}$': 'SCRAM Hash',
-    '^[a-f0-9]{40}:[a-f0-9]{0,32}$': 'Redmine Project Management Web App',
-    '^([^$]+)?\\$[a-f0-9]{16}$': 'SAP CODVN B (BCODE)',
-    '^(.+)?\\$[a-f0-9]{40}$': 'SAP CODVN F/G (PASSCODE)',
-    '^(.+\\$)?[a-z0-9\\/.+]{30}(:.+)?$': 'Juniper Netscreen/SSG(ScreenOS)',
-    '^0x(?:[a-f0-9]{60}|[a-f0-9]{40})$': 'EPi',
-    '^[a-f0-9]{40}:[^*]{1,25}$': 'SMF ≥ v1.1',
-    '^(\\$wbb3\\$\\*1\\*)?[a-f0-9]{40}[:*][a-f0-9]{40}$': 'Woltlab Burning Board 3.x',
-    '^[a-f0-9]{130}(:[a-f0-9]{40})?$': 'IPMI2 RAKP HMAC-SHA1',
-    '^[a-f0-9]{32}:[0-9]+:[a-z0-9_.+-]+@[a-z0-9-]+\\.[a-z0-9-.]+$': 'Lastpass',
-    '^[a-z0-9\\/.]{16}([:$].{1,})?$': 'Cisco-ASA(MD5)',
-    '^\\$vnc\\$\\*[a-f0-9]{32}\\*[a-f0-9]{32}$': 'VNC',
-    '^[a-z0-9]{32}(:([a-z0-9-]+\\.)?[a-z0-9-.]+\\.[a-z]{2,7}:.+:[0-9]+)?$': 'DNSSEC(NSEC3)',
-    '^(user-.+:)?\\$racf\\$\\*.+\\*[a-f0-9]{16}$': 'RACF',
-    '^\\$3\\$\\$[a-f0-9]{32}$': 'NTHash(FreeBSD Variant)',
-    '^\\$sha1\\$[0-9]+\\$[a-z0-9\\/.]{0,64}\\$[a-z0-9\\/.]{28}$': 'SHA-1 Crypt',
-    '^[a-f0-9]{70}$': 'hMailServer',
-    '^[:\\$][AB][:\\$]([a-f0-9]{1,8}[:\\$])?[a-f0-9]{32}$': 'MediaWiki',
-    '^[a-f0-9]{140}$': 'Minecraft(xAuth)',
-    '^\\$pbkdf2(-sha1)?\\$[0-9]+\\$[a-z0-9\\/.]+\\$[a-z0-9\\/.]{27}$': 'PBKDF2-SHA1(Generic)',
-    '^\\$pbkdf2-sha256\\$[0-9]+\\$[a-z0-9\\/.]+\\$[a-z0-9\\/.]{43}$': 'PBKDF2-SHA256(Generic)',
-    '^\\$pbkdf2-sha512\\$[0-9]+\\$[a-z0-9\\/.]+\\$[a-z0-9\\/.]{86}$': 'PBKDF2-SHA512(Generic)',
-    '^\\$p5k2\\$[0-9]+\\$[a-z0-9\\/+=-]+\\$[a-z0-9\\/+-]{27}=$': 'PBKDF2(Cryptacular)',
-    '^\\$p5k2\\$[0-9]+\\$[a-z0-9\\/.]+\\$[a-z0-9\\/.]{32}$': 'PBKDF2(Dwayne Litzenberger)',
-    '^{FSHP[0123]\\|[0-9]+\\|[0-9]+}[a-z0-9\\/+=]+$': 'Fairly Secure Hashed Password',
-    '^\\$PHPS\\$.+\\$[a-f0-9]{32}$': 'PHPS',
-    '^[0-9]{4}:[a-f0-9]{16}:[a-f0-9]{2080}$': '1Password(Agile Keychain)',
-    '^[a-f0-9]{64}:[a-f0-9]{32}:[0-9]{5}:[a-f0-9]{608}$': '1Password(Cloud Keychain)',
-    '^[a-f0-9]{256}:[a-f0-9]{256}:[a-f0-9]{16}:[a-f0-9]{16}:[a-f0-9]{320}:[a-f0-9]{16}:[a-f0-9]{40}:[a-f0-9]{40}:[a-f0-9]{32}$': 'IKE-PSK MD5',
-    '^[a-f0-9]{256}:[a-f0-9]{256}:[a-f0-9]{16}:[a-f0-9]{16}:[a-f0-9]{320}:[a-f0-9]{16}:[a-f0-9]{40}:[a-f0-9]{40}:[a-f0-9]{40}$': 'IKE-PSK SHA1',
-    '^[a-z0-9\\/+]{27}=$': 'PeopleSoft',
-    '^crypt\\$[a-f0-9]{5}\\$[a-z0-9\\/.]{13}$': 'Django(DES Crypt Wrapper)',
-    '^(\\$django\\$\\*1\\*)?pbkdf2_sha256\\$[0-9]+\\$[a-z0-9]+\\$[a-z0-9\\/+=]{44}$': 'Django(PBKDF2-HMAC-SHA256)',
-    '^pbkdf2_sha1\\$[0-9]+\\$[a-z0-9]+\\$[a-z0-9\\/+=]{28}$': 'Django(PBKDF2-HMAC-SHA1)',
-    '^bcrypt(\\$2[axy]|\\$2)\\$[0-9]{2}\\$[a-z0-9\\/.]{53}$': 'Django(bcrypt)',
-    '^md5\\$[a-f0-9]+\\$[a-f0-9]{32}$': 'Django(MD5)',
-    '^\\{PKCS5S2\\}[a-z0-9\\/+]{64}$': 'PBKDF2(Atlassian)',
-    '^md5[a-f0-9]{32}$': 'PostgreSQL MD5',
-    '^\\([a-z0-9\\/+]{49}\\)$': 'Lotus Notes/Domino 8',
-    '^SCRYPT:[0-9]{1,}:[0-9]{1}:[0-9]{1}:[a-z0-9:\\/+=]{1,}$': 'scrypt',
-    '^\\$8\\$[a-z0-9\\/.]{14}\\$[a-z0-9\\/.]{43}$': 'Cisco Type 8',
-    '^\\$9\\$[a-z0-9\\/.]{14}\\$[a-z0-9\\/.]{43}$': 'Cisco Type 9',
-    '^\\$office\\$\\*2007\\*[0-9]{2}\\*[0-9]{3}\\*[0-9]{2}\\*[a-z0-9]{32}\\*[a-z0-9]{32}\\*[a-z0-9]{40}$': 'Microsoft Office 2007',
-    '^\\$office\\$\\*2010\\*[0-9]{6}\\*[0-9]{3}\\*[0-9]{2}\\*[a-z0-9]{32}\\*[a-z0-9]{32}\\*[a-z0-9]{64}$': 'Microsoft Office 2010',
-    '^\\\\$office\\\\$2016\\\\$[0-9]\\\\$[0-9]{6}\\\\$[^$]{24}\\\\$[^$]{88}$': 'Microsoft Office 2016 - SheetProtection',
-    '^\\$office\\$\\*2013\\*[0-9]{6}\\*[0-9]{3}\\*[0-9]{2}\\*[a-z0-9]{32}\\*[a-z0-9]{32}\\*[a-z0-9]{64}$': 'Microsoft Office 2013',
-    '^\\$fde\\$[0-9]{2}\\$[a-f0-9]{32}\\$[0-9]{2}\\$[a-f0-9]{32}\\$[a-f0-9]{3072}$': 'Android FDE ≤ 4.3',
-    '\\$krb5tgs\\$23\\$\\*[^*]*\\*\\$[a-f0-9]{32}\\$[a-f0-9]{64,40960}': 'Kerberos 5 TGS-REP etype 23',
-    '^\\$oldoffice\\$[01]\\*[a-f0-9]{32}\\*[a-f0-9]{32}\\*[a-f0-9]{32}$': 'Microsoft Office ≤ 2003 (MD5+RC4)',
-    '^\\$oldoffice\\$[34]\\*[a-f0-9]{32}\\*[a-f0-9]{32}\\*[a-f0-9]{40}$': 'Microsoft Office ≤ 2003 (SHA1+RC4)',
-    '^\\$oldoffice\\$[34]\\*[a-f0-9]{32}\\*[a-f0-9]{32}\\*[a-f0-9]{40}:[a-f0-9]{10}': 'MS Office ⇐ 2003 $3, SHA1 + RC4, collider #2',
-    '^(\\$radmin2\\$)?[a-f0-9]{32}$': 'RAdmin v2.x',
-    '^{x-issha,\\s[0-9]{4}}[a-z0-9\\/+=]+$': 'SAP CODVN H (PWDSALTEDHASH) iSSHA-1',
-    '^\\$cram_md5\\$[a-z0-9\\/+=-]+\\$[a-z0-9\\/+=-]{52}$': 'CRAM-MD5',
-    '^[a-f0-9]{16}:2:4:[a-f0-9]{32}$': 'SipHash',
-    '^[a-f0-9]{4,}$': 'Cisco Type 7',
-    '^[a-z0-9\\/.]{13,}$': 'bcrypt',
-    '^(\\$cisco4\\$)?[a-z0-9\\/.]{43}$': 'Cisco Type 4',
-    '^bcrypt_sha256\\$\\$(2[axy]|2)\\$[0-9]+\\$[a-z0-9\\/.]{53}$': 'Django(bcrypt-SHA256)',
-    '^\\$postgres\\$.[^\\*]+[*:][a-f0-9]{1,32}[*:][a-f0-9]{32}$': 'PostgreSQL Challenge-Response Authentication (MD5)',
-    '^\\$siemens-s7\\$[0-9]{1}\\$[a-f0-9]{40}\\$[a-f0-9]{40}$': 'Siemens-S7',
-    '^(\\$pst\\$)?[a-f0-9]{8}$': 'Microsoft Outlook PST',
-    '^sha256[:$][0-9]+[:$][a-z0-9\\/+=]+[:$][a-z0-9\\/+]{32,128}$': 'PBKDF2-HMAC-SHA256(PHP)',
-    '^(\\$dahua\\$)?[a-z0-9]{8}$': 'Dahua',
-    '^\\$mysqlna\\$[a-f0-9]{40}[:*][a-f0-9]{40}$': 'MySQL Challenge-Response Authentication (SHA1)',
-    '\\$pdf\\$1\\*[2|3]\\*[0-9]{2}\\*[-0-9]{1,6}\\*[0-9]\\*[0-9]{2}\\*[a-f0-9]{32,32}\\*[0-9]{2}\\*[a-f0-9]{64}\\*[0-9]{2}\\*[a-f0-9]{64}': 'PDF 1.1 - 1.3 (Acrobat 2 - 4)',
-    '\\$pdf\\$1\\*[2|3]\\*[0-9]{2}\\*[-0-9]{1,6}\\*[0-9]\\*[0-9]{2}\\*[a-f0-9]{32}\\*[0-9]{2}\\*[a-f0-9]{64}\\*[0-9]{2}\\*[a-f0-9]{64}:[a-f0-9]{10}': 'PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2',
-    '^\\$pdf\\$[24]\\*[34]\\*128\\*[0-9-]{1,5}\\*1\\*(16|32)\\*[a-f0-9]{32,64}\\*32\\*[a-f0-9]{64}\\*(8|16|32)\\*[a-f0-9]{16,64}$': 'PDF 1.4 - 1.6 (Acrobat 5 - 8)',
-    '\\$pdf\\$5\\*[5|6]\\*[0-9]{3}\\*[-0-9]{1,6}\\*[0-9]\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}': 'PDF 1.7 Level 3 (Acrobat 9)',
-    '\\$pdf\\$5\\*[5|6]\\*[0-9]{3}\\*[-0-9]{1,6}\\*[0-9]\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}': 'PDF 1.7 Level 8 (Acrobat 10 - 11)',
-    '^\\$krb5asrep\\$23\\$[^:]+:[a-f0-9]{32,32}\\$[a-f0-9]{64,40960}$': 'Kerberos 5 AS-REP etype 23',
-    '^\\$krb5tgs\\$17\\$[^$]{1,512}\\$[^$]{1,512}\\$[^$]{1,4}?\\$?[a-f0-9]{1,32}\\$[a-f0-9]{64,40960}$': 'Kerberos 5 TGS-REP etype 17 (AES128-CTS-HMAC-SHA1-96)',
-    '^\\$krb5tgs\\$18\\$[^$]{1,512}\\$[^$]{1,512}\\$[^$]{1,4}?\\$?[a-f0-9]{1,32}\\$[a-f0-9]{64,40960}': 'Kerberos 5 TGS-REP etype 18 (AES256-CTS-HMAC-SHA1-96)',
-    '^\\$krb5pa\\$17\\$[^$]{1,512}\\$[^$]{1,512}\\$[a-f0-9]{104,112}$': 'Kerberos 5, etype 17, Pre-Auth',
-    '^\\$krb5pa\\$17\\$[^$]{1,512}\\$[^$]{1,512}\\$[^$]{0,512}\\$[a-f0-9]{104,112}$': 'Kerberos 5, etype 17, Pre-Auth (with salt)',
-    '^\\$krb5pa\\$18\\$[^$]{1,512}\\$[^$]{1,512}\\$[^$]{0,512}\\$[a-f0-9]{104,112}$': 'Kerberos 5, etype 18, Pre-Auth (with salt)',
-    '^\\$krb5pa\\$18\\$[^$]{1,512}\\$[^$]{1,512}\\$[a-f0-9]{104,112}$': 'Kerberos 5, etype 18, Pre-Auth',
-    '\\$bitcoin\\$[0-9]{2,4}\\$[a-f0-9$]{250,350}': 'Bitcoin / Litecoin',
-    '\\$ethereum\\$[a-z0-9*]{150,250}': 'Ethereum Wallet, PBKDF2-HMAC-SHA256',
-    '\\$monero\\$(0)\\*[a-f0-9]{32,3196}': 'Monero',
-    '^\\$electrum\\$[1-3]\\*[a-f0-9]{32,32}\\*[a-f0-9]{32,32}$': 'Electrum Wallet (Salt-Type 1-3)',
-    '^\\$electrum\\$4\\*[a-f0-9]{1,66}\\*[a-f0-9]{128,32768}\\*[a-f0-9]{64,64}$': 'Electrum Wallet (Salt-Type 4)',
-    '^\\$electrum\\$5\\*[a-f0-9]{66,66}\\*[a-f0-9]{2048,2048}\\*[a-f0-9]{64,64}$': 'Electrum Wallet (Salt-Type 5)',
-    '\\$ab\\$[0-9]{1}\\*[0-9]{1}\\*[0-9]{1,6}\\*[a-f0-9]{128}\\*[a-f0-9]{128}\\*[a-f0-9]{32}\\*[a-f0-9]{192}': 'Android Backup',
-    '\\$zip2\\$\\*[0-9]{1}\\*[0-9]{1}\\*[0-9]{1}\\*[a-f0-9]{16,32}\\*[a-f0-9]{1,6}\\*[a-f0-9]{1,6}\\*[a-f0-9]+\\*[a-f0-9]{20}\\*\\$\\/zip2\\$': 'WinZip',
-    '\\$itunes_backup\\$\\*[0-9]{1,2}\\*[a-f0-9]{80}\\*[0-9]{1,6}\\*[a-f0-9]{40}\\*[0-9]{0,10}\\*[a-f0-9]{0,40}': 'iTunes backup >= 10.0',
-    '\\$telegram\\$[a-f0-9*]{99}': 'Telegram Mobile App Passcode (SHA256)',
-    '^\\\\$telegram\\\\$1\\\\*4000\\\\*[a-f0-9]{64}\\\\*[a-f0-9]{576}$': 'Telegram Desktop 1.3.9',
-    '^\\\\$telegram\\\\$2\\\\*100000\\\\*[a-f0-9]{64}\\\\*[a-f0-9]{576}$': 'Telegram Desktop >= 2.1.14-beta / 2.2.0',
-    '\\$BLAKE2\\$[a-f0-9]{128}': 'BLAKE2b-512',
-    '\\$oldoffice\\$[a-f0-9*]{100}:[a-f0-9]{10}': 'MS Office ⇐ 2003 $0/$1, MD5 + RC4, collider #2',
-    '\\$office\\$2016\\$[0-9]\\$[0-9]{6}\\$[^$]{24}\\$[^$]{88}': 'MS Office 2016 - SheetProtection',
-    '\\$7z\\$[0-9]\\$[0-9]{1,2}\\$[0-9]{1}\\$[^$]{0,64}\\$[0-9]{1,2}\\$[a-f0-9]{32}\\$[0-9]{1,10}\\$[0-9]{1,6}\\$[0-9]{1,6}\\$[a-f0-9]{2,}': '7-zip',
-    '\\$zip3\\$\\*[0-9]\\*[0-9]\\*256\\*[0-9]\\*[a-f0-9]{0,32}\\*[a-f0-9]{288}\\*[0-9]\\*[0-9]\\*[0-9]\\*[^\\s]{0,64}': 'SecureZIP AES-256',
-    '\\$zip3\\$\\*[0-9]\\*[0-9]\\*192\\*[0-9]\\*[a-f0-9]{0,32}\\*[a-f0-9]{288}\\*[0-9]\\*[0-9]\\*[0-9]\\*[^\\s]{0,64}': 'SecureZIP AES-192',
-    '\\$zip3\\$\\*[0-9]\\*[0-9]\\*128\\*[0-9]\\*[a-f0-9]{0,32}\\*[a-f0-9]{288}\\*[0-9]\\*[0-9]\\*[0-9]\\*[^\\s]{0,64}': 'SecureZIP AES-128',
-    '^\\$pkzip2?\\$(1)\\*[0-9]{1}\\*[0-9]{1}\\*[0-9a-f]{1,3}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,4}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*(8)\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[a-f0-9]+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Compressed)',
-    '^\\$pkzip2?\\$(1)\\*[0-9]{1}\\*[0-9]{1}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*(0)\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[a-f0-9]+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Uncompressed)',
-    '^\\$pkzip2?\\$([2-8])\\*[0-9]{1}(\\*[0-9]{1}\\*[0-9a-f]{1,3}\\*([^0*][0-9a-f]{0,2})\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[0-9a-f]+)+\\*(8)\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[a-f0-9]+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Compressed Multi-File)',
-    '^\\$pkzip2?\\$([2-8])\\*[0-9]{1}(\\*[0-9]{1}\\*[0-9a-f]{1,8}\\*([0-9a-f]{1,8})\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[0-9a-f]+)+\\*([08])\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[a-f0-9]+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Mixed Multi-File)',
-    '^\\$pkzip2?\\$([2-8])\\*[0-9]{1}(\\*[0-9]{1}\\*[0-9a-f]{1,3}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[0-9a-f]+)+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Mixed Multi-File Checksum-Only)',
-    '^\\$argon2i\\$v=19\\$m=[0-9]{1,6},t=[0-9]{1,2},p=[0-9]{1,2}\\$[^$]+\\$[^\\s]{6,134}$': 'Argon2i',
-    '^\\$argon2id\\$v=19\\$m=[0-9]{1,6},t=[0-9]{1,2},p=[0-9]{1,2}\\$[^$]+\\$[^\\s]{6,134}$': 'Argon2id',
-    '^\\$argon2d\\$v=19\\$m=[0-9]{1,6},t=[0-9]{1,2},p=[0-9]{1,2}\\$[^$]+\\$[^\\s]{6,134}$': 'Argon2d',
-    '\\$bitlocker\\$[0-9]\\$[0-9]{2}\\$[a-f0-9]{32}\\$[a-f0-9]{7}\\$[a-f0-9]{2}\\$[a-f0-9]{24}\\$[a-f0-9]{2}\\$[a-f0-9]{120}': 'BitLocker',
-    '\\$racf\\$\\*.{1,}\\*[A-F0-9]{16}': 'RACF',
-    '^\\$sshng\\$4\\$16\\$[0-9]{32}\\$1232\\$[a-f0-9]{2464}$': 'RSA/DSA/EC/OpenSSH Private Keys ($4$)',
-    '^\\$RAR3\\$\\*(1)\\*[0-9a-f]{1,16}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,16}\\*[0-9a-f]{1,16}\\*[01]\\*([0-9a-f]+|[^*]{1,64}\\*[0-9a-f]{1,16})\\*30$': 'RAR3-p (Uncompressed)',
-    '^\\$RAR3\\$\\*(1)\\*[0-9a-f]{1,16}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,16}\\*[0-9a-f]{1,16}\\*[01]\\*([0-9a-f]+|[^*]{1,64}\\*[0-9a-f]{1,16})\\*(31|32|33|34|35)$': 'RAR3-p (Compressed)',
-    '^\\$RAR3\\$\\*0\\*[0-9a-f]{1,16}\\*[0-9a-f]+$': 'RAR3-hp',
-    '^\\$rar5\\$[0-9a-f]{1,2}\\$[0-9a-f]{1,32}\\$[0-9a-f]{1,2}\\$[0-9a-f]{1,32}\\$[0-9a-f]{1,2}\\$[0-9a-f]{1,16}$': 'RAR5',
-    '^\\$keepass\\$\\*1\\*\\d+\\*\\d\\*[0-9a-f]{32}\\*[0-9a-f]{64}\\*[0-9a-f]{32}\\*[0-9a-f]{64}\\*\\d\\*[^*]*(\\*[0-9a-f]+)?$': 'KeePass 1 AES (without keyfile)',
-    '^\\$keepass\\$\\*1\\*\\d+\\*\\d\\*[0-9a-f]{32}\\*[0-9a-f]{64}\\*[0-9a-f]{32}\\*[0-9a-f]{64}\\*\\d\\*[^*]*(\\*[0-9a-f]+)?\\*\\d+\\*\\d+\\*[0-9a-f]{64}$': 'KeePass 1 TwoFish (with keyfile)',
-    '^\\$keepass\\$\\*2\\*\\d+\\*\\d+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+$': 'KeePass 2 AES (without keyfile)',
-    '^\\$keepass\\$\\*2\\*\\d+\\*\\d+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*\\d+\\*\\d+\\*[0-9a-f]+$': 'KeePass 2 AES (with keyfile)',
-    '^\\$odf\\$\\*1\\*1\\*100000\\*32\\*[a-f0-9]{64}\\*16\\*[a-f0-9]{32}\\*16\\*[a-f0-9]{32}\\*0\\*[a-f0-9]{2048}$': 'Open Document Format (ODF) 1.2 (SHA-256, AES)',
-    '^[A-Za-z0-9-_]*\\.[A-Za-z0-9-_]*\\.[A-Za-z0-9-_]*$': 'JWT (JSON Web Token)',
-}
-
-popular_hashes_list = [
-    "MD5",
-    "MD4",
-    "NTLM",
-    "SHA-256",
-    "SHA-512",
-    "Keccak-256",
-    "Keccak-512",
-    "Blake2",
-    "bcrypt",
-    "SHA-1",
-    "HMAC-SHA1 (key = $salt)",
-    "CryptoCurrency(PrivateKey)",
-    "SHA-338",
-    "Domain Cached Credentials",
-    "Domain Cached Credentials 2",
-]
+hashes_dict = {
+    '^[a-f0-9]{4}$': 'CRC-16',
+    '^[a-f0-9]{8}$': 'Adler-32',
+    '^[a-f0-9]{6}$': 'CRC-24',
+    '^(\\$crc32\\$)?([a-f0-9]{8}.)?[a-f0-9]{8}$': 'CRC-32',
+    '^\\+[a-z0-9\\/.]{12}$': 'Eggdrop IRC Bot',
+    '^[a-z0-9\\/.]{12}[.26AEIMQUYcgkosw]{1}$': 'DES(Unix)',
+    '^[a-f0-9]{16}$': 'MySQL323',
+    '^[a-f0-9]{16}:[a-f0-9]{0,30}$': 'Oracle H: Type (Oracle 7+), DES(Oracle)',
+    '^[a-z0-9\\/.]{16}$': 'Cisco-PIX(MD5)',
+    '^\\([a-z0-9\\/+]{20}\\)$': 'Lotus Notes/Domino 6',
+    '^_[a-z0-9\\/.]{19}$': 'BSDi Crypt',
+    '^[a-f0-9]{24}$': 'CRC-96(ZIP)',
+    '^\\$keepass\\$\\*1\\*50000\\*(0|1)\\*([a-f0-9]{32})\\*([a-f0-9]{64})\\*([a-f0-9]{32})\\*([a-f0-9]{64})\\*1\\*(192|1360)\\*([a-f0-9]{384})$': 'Keepass 1 AES / without keyfile',
+    '^\\$keepass\\$\\*1\\*6000\\*(0|1)\\*([a-f0-9]{32})\\*([a-f0-9]{64})\\*([a-f0-9]{32})\\*([a-f0-9]{64})\\*1\\*(192|1360)\\*([a-f0-9]{2720})\\*1\\*64\\*([a-f0-9]{64})$': 'Keepass 1 Twofish / with keyfile',
+    '^\\$keepass\\$\\*2\\*6000\\*222(\\*[a-f0-9]{64}){2}(\\*[a-f0-9]{32}){1}(\\*[a-f0-9]{64}){2}\\*1\\*64(\\*[a-f0-9]{64}){1}$': 'Keepass 2 AES / with keyfile',
+    '^\\$keepass\\$\\*2\\*6000\\*222\\*(([a-f0-9]{32,64})(\\*)?)+$': 'Keepass 2 AES / without keyfile',
+    '^[a-z0-9\\/.]{24}$': 'Crypt16',
+    '^[a-f0-9]{32}$': 'MD5',
+    '(?:\\$haval\\$)?[a-f0-9]{32,64}$': 'Haval-128',
+    '(?:\\$ripemd\\$)?[a-f0-9]{32,40}$': 'RIPEMD-128',
+    '(?:\\$dynamic_39\\$)?[a-f0-9]{32}\\$[a-z0-9]{1,32}\\$?[a-z0-9]{1,500}': 'net-md5',
+    '^[a-f0-9]{32}:[a-z0-9]+$': 'Skype',
+    '^[a-f0-9]{32}:[a-z0-9]{56}$': 'PrestaShop',
+    '^(\\$md2\\$)?[a-f0-9]{32}$': 'MD2',
+    '^(\\$snefru\\$)?[a-f0-9]{32}$': 'Snefru-128',
+    '^(\\$NT\\$)?[a-f0-9]{32}$': 'NTLM',
+    '^([^\\\\\\/:*?"<>|]{1,20}:)?[a-f0-9]{32}(:[^\\\\\\/:*?"<>|]{1,20})?$': 'Domain Cached Credentials',
+    '^([^\\\\\\/:*?"<>|]{1,20}:)?(\\$DCC2\\$10240#[^\\\\\\/:*?"<>|]{1,20}#)?[a-f0-9]{32}$': 'Domain Cached Credentials 2',
+    '^{SHA}[a-z0-9\\/+]{27}=$': 'SHA-1(Base64)',
+    '^\\$1\\$[a-z0-9\\/.]{0,8}\\$[a-z0-9\\/.]{22}(:.*)?$': 'MD5 Crypt',
+    '^0x[a-f0-9]{32}$': 'Lineage II C4',
+    '^\\$H\\$[a-z0-9\\/.]{31}$': 'phpBB v3.x',
+    '^\\$P\\$[a-z0-9\\/.]{31}$': 'Wordpress ≥ v2.6.2',
+    '^[a-f0-9]{32}:[a-z0-9]{2}$': 'osCommerce',
+    '^\\$apr1\\$[a-z0-9\\/.]{0,8}\\$[a-z0-9\\/.]{22}$': 'MD5(APR)',
+    '^{smd5}[a-z0-9$\\/.]{31}$': 'AIX(smd5)',
+    '^[a-f0-9]{32}:.{5}$': 'IP.Board ≥ v2+',
+    '^[a-f0-9]{32}:.{8}$': 'MyBB ≥ v1.2+',
+    '^[a-z0-9]{34}$': 'CryptoCurrency(Adress)',
+    '^[a-f0-9]{40}(:.+)?$': 'SHA-1',
+    '^[a-f0-9]{40}$': 'MySQL5.x',
+    '^[a-z0-9]{43}$': 'Cisco-IOS(SHA-256)',
+    '^{SSHA}[a-z0-9\\/+]{38}==$': 'SSHA-1(Base64)',
+    '^[a-z0-9=]{47}$': 'Fortigate(FortiOS)',
+    '^[a-f0-9]{48}$': 'Haval-192',
+    '^[a-f0-9]{51}$': 'Palshop CMS',
+    '^[a-z0-9]{51}$': 'CryptoCurrency(PrivateKey)',
+    '^{ssha1}[0-9]{2}\\$[a-z0-9$\\/.]{44}$': 'AIX(ssha1)',
+    '^0x0100[a-f0-9]{48}$': 'MSSQL(2005)',
+    '^(\\$md5,rounds=[0-9]+\\$|\\$md5\\$rounds=[0-9]+\\$|\\$md5\\$)[a-z0-9\\/.]{0,16}(\\$|\\$\\$)[a-z0-9\\/.]{22}$': 'Sun MD5 Crypt',
+    '^[a-f0-9]{56}$': 'SHA-224',
+    '^(\\$2[abxy]?|\\$2)\\$[0-9]{2}\\$[a-z0-9\\/.]{53}$': 'bcrypt',
+    '^\\$y\\$[.\\/A-Za-z0-9]+\\$[.\\/a-zA-Z0-9]+\\$[.\\/A-Za-z0-9]{43}$': 'yescrypt',
+    '^[a-f0-9]{40}:[a-f0-9]{16}$': 'Android PIN',
+    '^(S:)?[a-f0-9]{40}(:)?[a-f0-9]{20}$': 'Oracle 11g/12c',
+    '^\\$bcrypt-sha256\\$(2[axy]|2)\\,[0-9]+\\$[a-z0-9\\/.]{22}\\$[a-z0-9\\/.]{31}$': 'bcrypt(SHA-256)',
+    '^[a-f0-9]{32}:.{3}$': 'vBulletin < v3.8.5',
+    '^[a-f0-9]{32}:.{30}$': 'vBulletin ≥ v3.8.5',
+    '^(\\$snefru\\$)?[a-f0-9]{64}$': 'Snefru-256',
+    '^[a-f0-9]{64}(:.+)?$': 'SHA-256',
+    '^[a-f0-9]{32}:[a-z0-9]{32}$': 'Joomla < v2.5.18',
+    '^[a-f0-9]{32}:[a-f0-9]{32}$': 'SAM(LM_Hash:NT_Hash)',
+    '^(\\$chap\\$0\\*)?[a-f0-9]{32}[\\*:][a-f0-9]{32}(:[0-9]{2})?$': 'MD5(Chap)',
+    '^\\$episerver\\$\\*0\\*[a-z0-9\\/=+]+\\*[a-z0-9\\/=+]{27,28}$': 'EPiServer 6.x < v4',
+    '^{ssha256}[0-9]{2}\\$[a-z0-9$\\/.]{60}$': 'AIX(ssha256)',
+    '^[a-f0-9]{80}$': 'RIPEMD-320',
+    '^\\$episerver\\$\\*1\\*[a-z0-9\\/=+]+\\*[a-z0-9\\/=+]{42,43}$': 'EPiServer 6.x ≥ v4',
+    '^0x0100[a-f0-9]{88}$': 'MSSQL(2000)',
+    '^[a-f0-9]{96}$': 'SHA-384',
+    '^{SSHA512}[a-z0-9\\/+]{96}$': 'SSHA-512(Base64)',
+    '^{ssha512}[0-9]{2}\\$[a-z0-9\\/.]{16,48}\\$[a-z0-9\\/.]{86}$': 'AIX(ssha512)',
+    '^[a-f0-9]{128}(:.+)?$': 'SHA-512',
+    '^[a-f0-9]{64}$': 'Keccak-256',
+    '^[a-f0-9]{136}$': 'OSX v10.7',
+    '^0x0200[a-f0-9]{136}$': 'MSSQL(2012)',
+    '^\\$ml\\$[0-9]+\\$[a-f0-9]{64}\\$[a-f0-9]{128}$': 'OSX v10.8',
+    '^[a-f0-9]{256}$': 'Skein-1024',
+    '^grub\\.pbkdf2\\.sha512\\.[0-9]+\\.([a-f0-9]{128,2048}\\.|[0-9]+\\.)?[a-f0-9]{128}$': 'GRUB 2',
+    '^sha1\\$[a-z0-9]+\\$[a-f0-9]{40}$': 'Django(SHA-1)',
+    '^[a-f0-9]{49}$': 'Citrix Netscaler',
+    '^\\$S\\$[a-z0-9\\/.]{52}$': 'Drupal > v7.x',
+    '^\\$5\\$(rounds=[0-9]+\\$)?[a-z0-9\\/.]{0,16}\\$[a-z0-9\\/.]{43}$': 'SHA-256 Crypt',
+    '^0x[a-f0-9]{4}[a-f0-9]{16}[a-f0-9]{64}$': 'Sybase ASE',
+    '^\\$6\\$(rounds=[0-9]+\\$)?[a-z0-9\\/.]{0,16}\\$[a-z0-9\\/.]{86}$': 'SHA-512 Crypt',
+    '^\\$sha\\$[a-z0-9]{1,16}\\$([a-f0-9]{32}|[a-f0-9]{40}|[a-f0-9]{64}|[a-f0-9]{128}|[a-f0-9]{140})$': 'Minecraft(AuthMe Reloaded)',
+    '^sha256\\$[a-z0-9]+\\$[a-f0-9]{64}$': 'Django(SHA-256)',
+    '^sha384\\$[a-z0-9]+\\$[a-f0-9]{96}$': 'Django(SHA-384)',
+    '^crypt1:[a-z0-9+=]{12}:[a-z0-9+=]{12}$': 'Clavister Secure Gateway',
+    '^[a-f0-9]{112}$': 'Cisco VPN Client(PCF-File)',
+    '^[a-f0-9]{1329}$': 'Microsoft MSTSC(RDP-File)',
+    '^[^\\\\\\/:*?"<>|]{1,20}[:]{2,3}([^\\\\\\/:*?"<>|]{1,20})?:[a-f0-9]{48}:[a-f0-9]{48}:[a-f0-9]{16}$': 'NetNTLMv1-VANILLA / NetNTLMv1+ESS',
+    '^([^\\\\\\/:*?"<>|]{1,20}\\\\)?[^\\\\\\/:*?"<>|]{1,20}[:]{2,3}([^\\\\\\/:*?"<>|]{1,20}:)?[^\\\\\\/:*?"<>|]{1,20}:[a-f0-9]{32}:[a-f0-9]+$': 'NetNTLMv2',
+    '^\\$(krb5pa|mskrb5)\\$(23)?\\$.+\\$[a-f0-9]{1,}$': 'Kerberos 5 AS-REQ Pre-Auth',
+    '^\\$scram\\$[0-9]+\\$[a-z0-9\\/.]{16}\\$sha-1=[a-z0-9\\/.]{27},sha-256=[a-z0-9\\/.]{43},sha-512=[a-z0-9\\/.]{86}$': 'SCRAM Hash',
+    '^[a-f0-9]{40}:[a-f0-9]{0,32}$': 'Redmine Project Management Web App',
+    '^([^$]+)?\\$[a-f0-9]{16}$': 'SAP CODVN B (BCODE)',
+    '^(.+)?\\$[a-f0-9]{40}$': 'SAP CODVN F/G (PASSCODE)',
+    '^(.+\\$)?[a-z0-9\\/.+]{30}(:.+)?$': 'Juniper Netscreen/SSG(ScreenOS)',
+    '^0x(?:[a-f0-9]{60}|[a-f0-9]{40})$': 'EPi',
+    '^[a-f0-9]{40}:[^*]{1,25}$': 'SMF ≥ v1.1',
+    '^(\\$wbb3\\$\\*1\\*)?[a-f0-9]{40}[:*][a-f0-9]{40}$': 'Woltlab Burning Board 3.x',
+    '^[a-f0-9]{130}(:[a-f0-9]{40})?$': 'IPMI2 RAKP HMAC-SHA1',
+    '^[a-f0-9]{32}:[0-9]+:[a-z0-9_.+-]+@[a-z0-9-]+\\.[a-z0-9-.]+$': 'Lastpass',
+    '^[a-z0-9\\/.]{16}([:$].{1,})?$': 'Cisco-ASA(MD5)',
+    '^\\$vnc\\$\\*[a-f0-9]{32}\\*[a-f0-9]{32}$': 'VNC',
+    '^[a-z0-9]{32}(:([a-z0-9-]+\\.)?[a-z0-9-.]+\\.[a-z]{2,7}:.+:[0-9]+)?$': 'DNSSEC(NSEC3)',
+    '^(user-.+:)?\\$racf\\$\\*.+\\*[a-f0-9]{16}$': 'RACF',
+    '^\\$3\\$\\$[a-f0-9]{32}$': 'NTHash(FreeBSD Variant)',
+    '^\\$sha1\\$[0-9]+\\$[a-z0-9\\/.]{0,64}\\$[a-z0-9\\/.]{28}$': 'SHA-1 Crypt',
+    '^[a-f0-9]{70}$': 'hMailServer',
+    '^[:\\$][AB][:\\$]([a-f0-9]{1,8}[:\\$])?[a-f0-9]{32}$': 'MediaWiki',
+    '^[a-f0-9]{140}$': 'Minecraft(xAuth)',
+    '^\\$pbkdf2(-sha1)?\\$[0-9]+\\$[a-z0-9\\/.]+\\$[a-z0-9\\/.]{27}$': 'PBKDF2-SHA1(Generic)',
+    '^\\$pbkdf2-sha256\\$[0-9]+\\$[a-z0-9\\/.]+\\$[a-z0-9\\/.]{43}$': 'PBKDF2-SHA256(Generic)',
+    '^\\$pbkdf2-sha512\\$[0-9]+\\$[a-z0-9\\/.]+\\$[a-z0-9\\/.]{86}$': 'PBKDF2-SHA512(Generic)',
+    '^\\$p5k2\\$[0-9]+\\$[a-z0-9\\/+=-]+\\$[a-z0-9\\/+-]{27}=$': 'PBKDF2(Cryptacular)',
+    '^\\$p5k2\\$[0-9]+\\$[a-z0-9\\/.]+\\$[a-z0-9\\/.]{32}$': 'PBKDF2(Dwayne Litzenberger)',
+    '^{FSHP[0123]\\|[0-9]+\\|[0-9]+}[a-z0-9\\/+=]+$': 'Fairly Secure Hashed Password',
+    '^\\$PHPS\\$.+\\$[a-f0-9]{32}$': 'PHPS',
+    '^[0-9]{4}:[a-f0-9]{16}:[a-f0-9]{2080}$': '1Password(Agile Keychain)',
+    '^[a-f0-9]{64}:[a-f0-9]{32}:[0-9]{5}:[a-f0-9]{608}$': '1Password(Cloud Keychain)',
+    '^[a-f0-9]{256}:[a-f0-9]{256}:[a-f0-9]{16}:[a-f0-9]{16}:[a-f0-9]{320}:[a-f0-9]{16}:[a-f0-9]{40}:[a-f0-9]{40}:[a-f0-9]{32}$': 'IKE-PSK MD5',
+    '^[a-f0-9]{256}:[a-f0-9]{256}:[a-f0-9]{16}:[a-f0-9]{16}:[a-f0-9]{320}:[a-f0-9]{16}:[a-f0-9]{40}:[a-f0-9]{40}:[a-f0-9]{40}$': 'IKE-PSK SHA1',
+    '^[a-z0-9\\/+]{27}=$': 'PeopleSoft',
+    '^crypt\\$[a-f0-9]{5}\\$[a-z0-9\\/.]{13}$': 'Django(DES Crypt Wrapper)',
+    '^(\\$django\\$\\*1\\*)?pbkdf2_sha256\\$[0-9]+\\$[a-z0-9]+\\$[a-z0-9\\/+=]{44}$': 'Django(PBKDF2-HMAC-SHA256)',
+    '^pbkdf2_sha1\\$[0-9]+\\$[a-z0-9]+\\$[a-z0-9\\/+=]{28}$': 'Django(PBKDF2-HMAC-SHA1)',
+    '^bcrypt(\\$2[axy]|\\$2)\\$[0-9]{2}\\$[a-z0-9\\/.]{53}$': 'Django(bcrypt)',
+    '^md5\\$[a-f0-9]+\\$[a-f0-9]{32}$': 'Django(MD5)',
+    '^\\{PKCS5S2\\}[a-z0-9\\/+]{64}$': 'PBKDF2(Atlassian)',
+    '^md5[a-f0-9]{32}$': 'PostgreSQL MD5',
+    '^\\([a-z0-9\\/+]{49}\\)$': 'Lotus Notes/Domino 8',
+    '^SCRYPT:[0-9]{1,}:[0-9]{1}:[0-9]{1}:[a-z0-9:\\/+=]{1,}$': 'scrypt',
+    '^\\$8\\$[a-z0-9\\/.]{14}\\$[a-z0-9\\/.]{43}$': 'Cisco Type 8',
+    '^\\$9\\$[a-z0-9\\/.]{14}\\$[a-z0-9\\/.]{43}$': 'Cisco Type 9',
+    '^\\$office\\$\\*2007\\*[0-9]{2}\\*[0-9]{3}\\*[0-9]{2}\\*[a-z0-9]{32}\\*[a-z0-9]{32}\\*[a-z0-9]{40}$': 'Microsoft Office 2007',
+    '^\\$office\\$\\*2010\\*[0-9]{6}\\*[0-9]{3}\\*[0-9]{2}\\*[a-z0-9]{32}\\*[a-z0-9]{32}\\*[a-z0-9]{64}$': 'Microsoft Office 2010',
+    '^\\\\$office\\\\$2016\\\\$[0-9]\\\\$[0-9]{6}\\\\$[^$]{24}\\\\$[^$]{88}$': 'Microsoft Office 2016 - SheetProtection',
+    '^\\$office\\$\\*2013\\*[0-9]{6}\\*[0-9]{3}\\*[0-9]{2}\\*[a-z0-9]{32}\\*[a-z0-9]{32}\\*[a-z0-9]{64}$': 'Microsoft Office 2013',
+    '^\\$fde\\$[0-9]{2}\\$[a-f0-9]{32}\\$[0-9]{2}\\$[a-f0-9]{32}\\$[a-f0-9]{3072}$': 'Android FDE ≤ 4.3',
+    '\\$krb5tgs\\$23\\$\\*[^*]*\\*\\$[a-f0-9]{32}\\$[a-f0-9]{64,40960}': 'Kerberos 5 TGS-REP etype 23',
+    '^\\$oldoffice\\$[01]\\*[a-f0-9]{32}\\*[a-f0-9]{32}\\*[a-f0-9]{32}$': 'Microsoft Office ≤ 2003 (MD5+RC4)',
+    '^\\$oldoffice\\$[34]\\*[a-f0-9]{32}\\*[a-f0-9]{32}\\*[a-f0-9]{40}$': 'Microsoft Office ≤ 2003 (SHA1+RC4)',
+    '^\\$oldoffice\\$[34]\\*[a-f0-9]{32}\\*[a-f0-9]{32}\\*[a-f0-9]{40}:[a-f0-9]{10}': 'MS Office ⇐ 2003 $3, SHA1 + RC4, collider #2',
+    '^(\\$radmin2\\$)?[a-f0-9]{32}$': 'RAdmin v2.x',
+    '^{x-issha,\\s[0-9]{4}}[a-z0-9\\/+=]+$': 'SAP CODVN H (PWDSALTEDHASH) iSSHA-1',
+    '^\\$cram_md5\\$[a-z0-9\\/+=-]+\\$[a-z0-9\\/+=-]{52}$': 'CRAM-MD5',
+    '^[a-f0-9]{16}:2:4:[a-f0-9]{32}$': 'SipHash',
+    '^[a-f0-9]{4,}$': 'Cisco Type 7',
+    '^[a-z0-9\\/.]{13,}$': 'bcrypt',
+    '^(\\$cisco4\\$)?[a-z0-9\\/.]{43}$': 'Cisco Type 4',
+    '^bcrypt_sha256\\$\\$(2[axy]|2)\\$[0-9]+\\$[a-z0-9\\/.]{53}$': 'Django(bcrypt-SHA256)',
+    '^\\$postgres\\$.[^\\*]+[*:][a-f0-9]{1,32}[*:][a-f0-9]{32}$': 'PostgreSQL Challenge-Response Authentication (MD5)',
+    '^\\$siemens-s7\\$[0-9]{1}\\$[a-f0-9]{40}\\$[a-f0-9]{40}$': 'Siemens-S7',
+    '^(\\$pst\\$)?[a-f0-9]{8}$': 'Microsoft Outlook PST',
+    '^sha256[:$][0-9]+[:$][a-z0-9\\/+=]+[:$][a-z0-9\\/+]{32,128}$': 'PBKDF2-HMAC-SHA256(PHP)',
+    '^(\\$dahua\\$)?[a-z0-9]{8}$': 'Dahua',
+    '^\\$mysqlna\\$[a-f0-9]{40}[:*][a-f0-9]{40}$': 'MySQL Challenge-Response Authentication (SHA1)',
+    '\\$pdf\\$1\\*[2|3]\\*[0-9]{2}\\*[-0-9]{1,6}\\*[0-9]\\*[0-9]{2}\\*[a-f0-9]{32,32}\\*[0-9]{2}\\*[a-f0-9]{64}\\*[0-9]{2}\\*[a-f0-9]{64}': 'PDF 1.1 - 1.3 (Acrobat 2 - 4)',
+    '\\$pdf\\$1\\*[2|3]\\*[0-9]{2}\\*[-0-9]{1,6}\\*[0-9]\\*[0-9]{2}\\*[a-f0-9]{32}\\*[0-9]{2}\\*[a-f0-9]{64}\\*[0-9]{2}\\*[a-f0-9]{64}:[a-f0-9]{10}': 'PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2',
+    '^\\$pdf\\$[24]\\*[34]\\*128\\*[0-9-]{1,5}\\*1\\*(16|32)\\*[a-f0-9]{32,64}\\*32\\*[a-f0-9]{64}\\*(8|16|32)\\*[a-f0-9]{16,64}$': 'PDF 1.4 - 1.6 (Acrobat 5 - 8)',
+    '\\$pdf\\$5\\*[5|6]\\*[0-9]{3}\\*[-0-9]{1,6}\\*[0-9]\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}': 'PDF 1.7 Level 3 (Acrobat 9)',
+    '\\$pdf\\$5\\*[5|6]\\*[0-9]{3}\\*[-0-9]{1,6}\\*[0-9]\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}\\*[0-9]{1,4}\\*[a-f0-9]{0,1024}': 'PDF 1.7 Level 8 (Acrobat 10 - 11)',
+    '^\\$krb5asrep\\$23\\$[^:]+:[a-f0-9]{32,32}\\$[a-f0-9]{64,40960}$': 'Kerberos 5 AS-REP etype 23',
+    '^\\$krb5tgs\\$17\\$[^$]{1,512}\\$[^$]{1,512}\\$[^$]{1,4}?\\$?[a-f0-9]{1,32}\\$[a-f0-9]{64,40960}$': 'Kerberos 5 TGS-REP etype 17 (AES128-CTS-HMAC-SHA1-96)',
+    '^\\$krb5tgs\\$18\\$[^$]{1,512}\\$[^$]{1,512}\\$[^$]{1,4}?\\$?[a-f0-9]{1,32}\\$[a-f0-9]{64,40960}': 'Kerberos 5 TGS-REP etype 18 (AES256-CTS-HMAC-SHA1-96)',
+    '^\\$krb5pa\\$17\\$[^$]{1,512}\\$[^$]{1,512}\\$[a-f0-9]{104,112}$': 'Kerberos 5, etype 17, Pre-Auth',
+    '^\\$krb5pa\\$17\\$[^$]{1,512}\\$[^$]{1,512}\\$[^$]{0,512}\\$[a-f0-9]{104,112}$': 'Kerberos 5, etype 17, Pre-Auth (with salt)',
+    '^\\$krb5pa\\$18\\$[^$]{1,512}\\$[^$]{1,512}\\$[^$]{0,512}\\$[a-f0-9]{104,112}$': 'Kerberos 5, etype 18, Pre-Auth (with salt)',
+    '^\\$krb5pa\\$18\\$[^$]{1,512}\\$[^$]{1,512}\\$[a-f0-9]{104,112}$': 'Kerberos 5, etype 18, Pre-Auth',
+    '\\$bitcoin\\$[0-9]{2,4}\\$[a-f0-9$]{250,350}': 'Bitcoin / Litecoin',
+    '\\$ethereum\\$[a-z0-9*]{150,250}': 'Ethereum Wallet, PBKDF2-HMAC-SHA256',
+    '\\$monero\\$(0)\\*[a-f0-9]{32,3196}': 'Monero',
+    '^\\$electrum\\$[1-3]\\*[a-f0-9]{32,32}\\*[a-f0-9]{32,32}$': 'Electrum Wallet (Salt-Type 1-3)',
+    '^\\$electrum\\$4\\*[a-f0-9]{1,66}\\*[a-f0-9]{128,32768}\\*[a-f0-9]{64,64}$': 'Electrum Wallet (Salt-Type 4)',
+    '^\\$electrum\\$5\\*[a-f0-9]{66,66}\\*[a-f0-9]{2048,2048}\\*[a-f0-9]{64,64}$': 'Electrum Wallet (Salt-Type 5)',
+    '\\$ab\\$[0-9]{1}\\*[0-9]{1}\\*[0-9]{1,6}\\*[a-f0-9]{128}\\*[a-f0-9]{128}\\*[a-f0-9]{32}\\*[a-f0-9]{192}': 'Android Backup',
+    '\\$zip2\\$\\*[0-9]{1}\\*[0-9]{1}\\*[0-9]{1}\\*[a-f0-9]{16,32}\\*[a-f0-9]{1,6}\\*[a-f0-9]{1,6}\\*[a-f0-9]+\\*[a-f0-9]{20}\\*\\$\\/zip2\\$': 'WinZip',
+    '\\$itunes_backup\\$\\*[0-9]{1,2}\\*[a-f0-9]{80}\\*[0-9]{1,6}\\*[a-f0-9]{40}\\*[0-9]{0,10}\\*[a-f0-9]{0,40}': 'iTunes backup >= 10.0',
+    '\\$telegram\\$[a-f0-9*]{99}': 'Telegram Mobile App Passcode (SHA256)',
+    '^\\\\$telegram\\\\$1\\\\*4000\\\\*[a-f0-9]{64}\\\\*[a-f0-9]{576}$': 'Telegram Desktop 1.3.9',
+    '^\\\\$telegram\\\\$2\\\\*100000\\\\*[a-f0-9]{64}\\\\*[a-f0-9]{576}$': 'Telegram Desktop >= 2.1.14-beta / 2.2.0',
+    '\\$BLAKE2\\$[a-f0-9]{128}': 'BLAKE2b-512',
+    '\\$oldoffice\\$[a-f0-9*]{100}:[a-f0-9]{10}': 'MS Office ⇐ 2003 $0/$1, MD5 + RC4, collider #2',
+    '\\$office\\$2016\\$[0-9]\\$[0-9]{6}\\$[^$]{24}\\$[^$]{88}': 'MS Office 2016 - SheetProtection',
+    '\\$7z\\$[0-9]\\$[0-9]{1,2}\\$[0-9]{1}\\$[^$]{0,64}\\$[0-9]{1,2}\\$[a-f0-9]{32}\\$[0-9]{1,10}\\$[0-9]{1,6}\\$[0-9]{1,6}\\$[a-f0-9]{2,}': '7-zip',
+    '\\$zip3\\$\\*[0-9]\\*[0-9]\\*256\\*[0-9]\\*[a-f0-9]{0,32}\\*[a-f0-9]{288}\\*[0-9]\\*[0-9]\\*[0-9]\\*[^\\s]{0,64}': 'SecureZIP AES-256',
+    '\\$zip3\\$\\*[0-9]\\*[0-9]\\*192\\*[0-9]\\*[a-f0-9]{0,32}\\*[a-f0-9]{288}\\*[0-9]\\*[0-9]\\*[0-9]\\*[^\\s]{0,64}': 'SecureZIP AES-192',
+    '\\$zip3\\$\\*[0-9]\\*[0-9]\\*128\\*[0-9]\\*[a-f0-9]{0,32}\\*[a-f0-9]{288}\\*[0-9]\\*[0-9]\\*[0-9]\\*[^\\s]{0,64}': 'SecureZIP AES-128',
+    '^\\$pkzip2?\\$(1)\\*[0-9]{1}\\*[0-9]{1}\\*[0-9a-f]{1,3}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,4}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*(8)\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[a-f0-9]+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Compressed)',
+    '^\\$pkzip2?\\$(1)\\*[0-9]{1}\\*[0-9]{1}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}\\*(0)\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[a-f0-9]+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Uncompressed)',
+    '^\\$pkzip2?\\$([2-8])\\*[0-9]{1}(\\*[0-9]{1}\\*[0-9a-f]{1,3}\\*([^0*][0-9a-f]{0,2})\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[0-9a-f]+)+\\*(8)\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[a-f0-9]+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Compressed Multi-File)',
+    '^\\$pkzip2?\\$([2-8])\\*[0-9]{1}(\\*[0-9]{1}\\*[0-9a-f]{1,8}\\*([0-9a-f]{1,8})\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[0-9a-f]+)+\\*([08])\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[a-f0-9]+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Mixed Multi-File)',
+    '^\\$pkzip2?\\$([2-8])\\*[0-9]{1}(\\*[0-9]{1}\\*[0-9a-f]{1,3}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,8}(\\*[0-9a-f]{1,8})?\\*[0-9a-f]{1,8}\\*[0-9a-f]+)+\\*\\$\\/pkzip2?\\$$': 'PKZIP (Mixed Multi-File Checksum-Only)',
+    '^\\$argon2i\\$v=19\\$m=[0-9]{1,6},t=[0-9]{1,2},p=[0-9]{1,2}\\$[^$]+\\$[^\\s]{6,134}$': 'Argon2i',
+    '^\\$argon2id\\$v=19\\$m=[0-9]{1,6},t=[0-9]{1,2},p=[0-9]{1,2}\\$[^$]+\\$[^\\s]{6,134}$': 'Argon2id',
+    '^\\$argon2d\\$v=19\\$m=[0-9]{1,6},t=[0-9]{1,2},p=[0-9]{1,2}\\$[^$]+\\$[^\\s]{6,134}$': 'Argon2d',
+    '\\$bitlocker\\$[0-9]\\$[0-9]{2}\\$[a-f0-9]{32}\\$[a-f0-9]{7}\\$[a-f0-9]{2}\\$[a-f0-9]{24}\\$[a-f0-9]{2}\\$[a-f0-9]{120}': 'BitLocker',
+    '\\$racf\\$\\*.{1,}\\*[A-F0-9]{16}': 'RACF',
+    '^\\$sshng\\$4\\$16\\$[0-9]{32}\\$1232\\$[a-f0-9]{2464}$': 'RSA/DSA/EC/OpenSSH Private Keys ($4$)',
+    '^\\$RAR3\\$\\*(1)\\*[0-9a-f]{1,16}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,16}\\*[0-9a-f]{1,16}\\*[01]\\*([0-9a-f]+|[^*]{1,64}\\*[0-9a-f]{1,16})\\*30$': 'RAR3-p (Uncompressed)',
+    '^\\$RAR3\\$\\*(1)\\*[0-9a-f]{1,16}\\*[0-9a-f]{1,8}\\*[0-9a-f]{1,16}\\*[0-9a-f]{1,16}\\*[01]\\*([0-9a-f]+|[^*]{1,64}\\*[0-9a-f]{1,16})\\*(31|32|33|34|35)$': 'RAR3-p (Compressed)',
+    '^\\$RAR3\\$\\*0\\*[0-9a-f]{1,16}\\*[0-9a-f]+$': 'RAR3-hp',
+    '^\\$rar5\\$[0-9a-f]{1,2}\\$[0-9a-f]{1,32}\\$[0-9a-f]{1,2}\\$[0-9a-f]{1,32}\\$[0-9a-f]{1,2}\\$[0-9a-f]{1,16}$': 'RAR5',
+    '^\\$keepass\\$\\*1\\*\\d+\\*\\d\\*[0-9a-f]{32}\\*[0-9a-f]{64}\\*[0-9a-f]{32}\\*[0-9a-f]{64}\\*\\d\\*[^*]*(\\*[0-9a-f]+)?$': 'KeePass 1 AES (without keyfile)',
+    '^\\$keepass\\$\\*1\\*\\d+\\*\\d\\*[0-9a-f]{32}\\*[0-9a-f]{64}\\*[0-9a-f]{32}\\*[0-9a-f]{64}\\*\\d\\*[^*]*(\\*[0-9a-f]+)?\\*\\d+\\*\\d+\\*[0-9a-f]{64}$': 'KeePass 1 TwoFish (with keyfile)',
+    '^\\$keepass\\$\\*2\\*\\d+\\*\\d+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+$': 'KeePass 2 AES (without keyfile)',
+    '^\\$keepass\\$\\*2\\*\\d+\\*\\d+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*[0-9a-f]+\\*\\d+\\*\\d+\\*[0-9a-f]+$': 'KeePass 2 AES (with keyfile)',
+    '^\\$odf\\$\\*1\\*1\\*100000\\*32\\*[a-f0-9]{64}\\*16\\*[a-f0-9]{32}\\*16\\*[a-f0-9]{32}\\*0\\*[a-f0-9]{2048}$': 'Open Document Format (ODF) 1.2 (SHA-256, AES)',
+    '^[A-Za-z0-9-_]*\\.[A-Za-z0-9-_]*\\.[A-Za-z0-9-_]*$': 'JWT (JSON Web Token)',
+}
+
+popular_hashes_list = [
+    "MD5",
+    "MD4",
+    "NTLM",
+    "SHA-256",
+    "SHA-512",
+    "Keccak-256",
+    "Keccak-512",
+    "Blake2",
+    "bcrypt",
+    "SHA-1",
+    "HMAC-SHA1 (key = $salt)",
+    "CryptoCurrency(PrivateKey)",
+    "SHA-338",
+    "Domain Cached Credentials",
+    "Domain Cached Credentials 2",
+]
```

### Comparing `nth_api-1.3.4/setup.py` & `nth_api-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="nth_api",
     author="user-sspmynxdvb",
-    version="1.3.4",
+    version="1.3.5",
     description="Name-That-Hash api version",
     license="GNUv3",
     url="https://github.com/user-sspmynxdvb/nth_api",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```
