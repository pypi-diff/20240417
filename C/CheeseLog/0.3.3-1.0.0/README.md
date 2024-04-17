# Comparing `tmp/cheeselog-0.3.3.tar.gz` & `tmp/cheeselog-1.0.0.tar.gz`

## Comparing `cheeselog-0.3.3.tar` & `cheeselog-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cheeselog-0.3.3/CheeseLog/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 cheeselog-0.3.3/CheeseLog/level.py
--rw-r--r--   0        0        0     9908 2020-02-02 00:00:00.000000 cheeselog-0.3.3/CheeseLog/logger.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 cheeselog-0.3.3/CheeseLog/progressBar.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cheeselog-0.3.3/CheeseLog/style.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cheeselog-0.3.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeselog-0.3.3/LICENSE
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 cheeselog-0.3.3/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cheeselog-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 cheeselog-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/level.py
+-rw-r--r--   0        0        0     9882 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/logger.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/progressBar.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cheeselog-1.0.0/CheeseLog/style.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 cheeselog-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeselog-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 cheeselog-1.0.0/README.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cheeselog-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 cheeselog-1.0.0/PKG-INFO
```

### Comparing `cheeselog-0.3.3/CheeseLog/logger.py` & `cheeselog-1.0.0/CheeseLog/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,29 +52,27 @@
                 if self.fileExpire.total_seconds():
                     try:
                         fileExpire = (datetime.datetime.now() - self.fileExpire).strftime(self.filePath)
                         os.remove(fileExpire)
                     except:
                         ...
 
-                data = self._queue.get(timeout = 0.016)
+                data = self._queue.get()
                 message = data[2].strftime(data[3].replace('%l', data[0]).replace('%c', data[1]).replace('%t', data[4])).replace('\n', '\n    ').replace('&lt;', '<').replace('&gt;', '>') + '\n'
 
                 try:
                     filePath = time.strftime(self.filePath)
                 except:
                     filePath = self.filePath
 
                 os.makedirs(os.path.dirname(filePath), exist_ok = True)
                 with open(filePath, 'a', encoding = 'utf-8') as f:
                     f.write(message)
             except KeyboardInterrupt:
                 ...
-            except queue.Empty:
-                ...
 
     def default(self, level: str, message: str, styledMessage: str | None = None, *, end: str = '\n', refreshed: bool = False):
         if level not in self.levels:
             raise KeyError('No level with this key')
 
         if self.levels[level].weight < self.weightFilter:
             return
@@ -181,14 +179,15 @@
         self.default('LOADING', message, styledMessage, end = end, refreshed = refreshed)
 
     def encode(self, message: str) -> str:
         return message.replace('<', '&lt;').replace('>', '&gt;').replace('%', '%%')
 
     def destroy(self):
         self._event.set()
+        self._processHandler.terminate()
         self._processHandler.join()
         self._event.clear()
         self._processHandler = None
 
     @property
     def filePath(self) -> str:
         return self._filePath
```

### Comparing `cheeselog-0.3.3/CheeseLog/progressBar.py` & `cheeselog-1.0.0/CheeseLog/progressBar.py`

 * *Files identical despite different names*

### Comparing `cheeselog-0.3.3/CheeseLog/style.py` & `cheeselog-1.0.0/CheeseLog/style.py`

 * *Files identical despite different names*

### Comparing `cheeselog-0.3.3/LICENSE` & `cheeselog-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeselog-0.3.3/README.md` & `cheeselog-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cheeselog-0.3.3/pyproject.toml` & `cheeselog-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseLog"
-version = "0.3.3"
+version = "1.0.0"
 description = "日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'log', 'logger' ]
```

### Comparing `cheeselog-0.3.3/PKG-INFO` & `cheeselog-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseLog
-Version: 0.3.3
+Version: 1.0.0
 Summary: 日志系统。可在控制台输出一定格式的、可选颜色的内容，并支持写入指定的日志文件。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseLog
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: log,logger
 Requires-Dist: setproctitle
 Description-Content-Type: text/markdown
```

