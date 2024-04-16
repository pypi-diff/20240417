# Comparing `tmp/monacopy-0.0.0.tar.gz` & `tmp/monacopy-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monacopy-0.0.0.tar", last modified: Mon Apr 15 22:12:04 2024, max compression
+gzip compressed data, was "monacopy-0.0.1.tar", last modified: Tue Apr 16 22:18:47 2024, max compression
```

## Comparing `monacopy-0.0.0.tar` & `monacopy-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:12:04.869961 monacopy-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 22:11:56.000000 monacopy-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 22:12:04.869961 monacopy-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 22:11:56.000000 monacopy-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:12:04.869961 monacopy-0.0.0/monacopy/
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-04-15 22:11:56.000000 monacopy-0.0.0/monacopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:12:04.869961 monacopy-0.0.0/monacopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 22:12:04.000000 monacopy-0.0.0/monacopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-15 22:12:04.000000 monacopy-0.0.0/monacopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 22:12:04.000000 monacopy-0.0.0/monacopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 22:12:04.000000 monacopy-0.0.0/monacopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 22:12:04.000000 monacopy-0.0.0/monacopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 22:12:04.869961 monacopy-0.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3540 2024-04-15 22:11:56.000000 monacopy-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:18:47.881712 monacopy-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 22:18:39.000000 monacopy-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-16 22:18:47.881712 monacopy-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 22:18:39.000000 monacopy-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:18:47.877712 monacopy-0.0.1/monacopy/
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-16 22:18:39.000000 monacopy-0.0.1/monacopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:18:47.881712 monacopy-0.0.1/monacopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 22:18:47.000000 monacopy-0.0.1/monacopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:18:47.881712 monacopy-0.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3540 2024-04-16 22:18:39.000000 monacopy-0.0.1/setup.py
```

### Comparing `monacopy-0.0.0/LICENSE` & `monacopy-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monacopy-0.0.0/monacopy/__init__.py` & `monacopy-0.0.1/monacopy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
       source = source.replace(
         /^<svg/,
         '<svg xmlns:xlink="http://www.w3.org/1999/xlink"'
       );
     }
 
     //add xml declaration
-    source = '<?xml version="1.0" standalone="no"?>\r\n' + source;
+    source = '<?xml version="1.0" standalone="no"?>' + source;
 
     //convert svg source to URI data scheme.
     var url = "data:image/svg+xml;charset=utf-8," + encodeURIComponent(source);
 
     var downloadLink = document.createElement("a");
     downloadLink.href = url;
     downloadLink.download = filename + ".svg";
@@ -344,16 +344,17 @@
         //https://microsoft.github.io/monaco-editor/playground.html?source=v0.47.0#example-customizing-the-appearence-scrollbars
         var editor = monaco.editor.create(document.getElementById('container'), {
         value: source_value,
         language: 'javascript',
         minimap: {
             enabled: false
         },
-        lineNumbers: "off",
+        lineNumbers: "on",
         scrollBeyondLastLine: false,
+        wordWrap: "on",
     	scrollbar: {
     		// Subtle shadows to the left & top. Defaults to true.
     		useShadows: false,
     
     		// Render vertical arrows. Defaults to false.
     		verticalHasArrows: false,
     		// Render horizontal arrows. Defaults to false.
@@ -378,15 +379,15 @@
     window.onload = function(){
        setTimeout(loadAfterTime, 10000)
     };
 
     function loadAfterTime(){
                const svg= htmlToSvg(document.getElementById("container"), {
               downloadSvg: true,
-              filename: "htmltosvg",
+              filename: "{{ filename }}",
             });
            console.log(svg);
            var uriContent = "data:image/svg+xml;base64," + encodeURIComponent(svg);
            window.open(uriContent, '{{ filename }}');
     };
     </script>
```

### Comparing `monacopy-0.0.0/setup.py` & `monacopy-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.0"
+VERSION = "0.0.1"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

