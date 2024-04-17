# Comparing `tmp/pycups-2.0.1.tar.gz` & `tmp/pycups-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "./pycups-2.0.1.tar", last modified: Thu Apr 23 12:34:49 2020, max compression
+gzip compressed data, was "pycups-2.0.2.tar", last modified: Wed Apr 17 13:07:47 2024, max compression
```

## Comparing `pycups-2.0.1.tar` & `pycups-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)        0 2020-04-23 12:34:49.000000 pycups-2.0.1/
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    18092 2019-08-20 07:58:13.000000 pycups-2.0.1/COPYING
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1171 2020-04-23 10:34:54.000000 pycups-2.0.1/Makefile
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    11132 2020-04-23 12:32:38.000000 pycups-2.0.1/NEWS
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1296 2020-04-23 12:34:49.000000 pycups-2.0.1/PKG-INFO
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1091 2020-04-20 04:37:30.000000 pycups-2.0.1/README
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)      214 2020-04-23 10:42:09.000000 pycups-2.0.1/TODO
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)   172122 2020-04-23 09:29:17.000000 pycups-2.0.1/cupsconnection.c
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     2118 2020-04-23 07:17:21.000000 pycups-2.0.1/cupsconnection.h
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    22243 2020-04-23 08:59:55.000000 pycups-2.0.1/cupsipp.c
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1360 2020-04-23 07:22:50.000000 pycups-2.0.1/cupsipp.h
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    36411 2020-04-23 11:44:12.000000 pycups-2.0.1/cupsmodule.c
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1660 2020-04-23 07:19:09.000000 pycups-2.0.1/cupsmodule.h
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)    46838 2020-04-23 07:19:59.000000 pycups-2.0.1/cupsppd.c
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     1358 2020-04-23 07:23:29.000000 pycups-2.0.1/cupsppd.h
-drwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)        0 2020-04-23 12:34:49.000000 pycups-2.0.1/examples/
--rwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)     1804 2019-08-20 07:58:13.000000 pycups-2.0.1/examples/cupstree.py
--rwxrwxr-x   0 zdohnal  (28720) zdohnal  (28720)     7703 2020-04-23 07:25:04.000000 pycups-2.0.1/postscriptdriver.prov
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)      165 2019-08-20 07:58:13.000000 pycups-2.0.1/psdriver.attr
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)     2565 2020-04-23 12:33:30.000000 pycups-2.0.1/setup.py
--rw-rw-r--   0 zdohnal  (28720) zdohnal  (28720)      886 2019-08-20 07:58:13.000000 pycups-2.0.1/test.py
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 13:07:47.490276 pycups-2.0.2/
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    18092 2022-08-31 12:07:01.000000 pycups-2.0.2/COPYING
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      256 2022-08-31 12:07:01.000000 pycups-2.0.2/MANIFEST.in
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1222 2024-04-17 11:25:39.000000 pycups-2.0.2/Makefile
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    11598 2024-04-17 11:30:11.000000 pycups-2.0.2/NEWS
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1197 2024-04-17 13:07:47.490276 pycups-2.0.2/PKG-INFO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1189 2022-10-25 13:03:09.000000 pycups-2.0.2/README
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      214 2022-08-31 12:07:01.000000 pycups-2.0.2/TODO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)   172355 2024-04-17 11:30:11.000000 pycups-2.0.2/cupsconnection.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2118 2022-08-31 12:07:01.000000 pycups-2.0.2/cupsconnection.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    22247 2024-04-17 11:30:11.000000 pycups-2.0.2/cupsipp.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1386 2022-08-31 12:07:01.000000 pycups-2.0.2/cupsipp.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    36411 2022-10-25 13:03:04.000000 pycups-2.0.2/cupsmodule.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1660 2022-08-31 12:07:01.000000 pycups-2.0.2/cupsmodule.h
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)    46838 2022-10-25 13:03:04.000000 pycups-2.0.2/cupsppd.c
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1358 2022-08-31 12:07:01.000000 pycups-2.0.2/cupsppd.h
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 13:07:47.489276 pycups-2.0.2/examples/
+-rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     2114 2023-04-06 06:01:00.000000 pycups-2.0.2/examples/cupstree.py
+-rwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)     7754 2022-08-31 12:07:01.000000 pycups-2.0.2/postscriptdriver.prov
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      165 2022-08-31 12:07:01.000000 pycups-2.0.2/psdriver.attr
+drwxr-xr-x   0 zdohnal   (1000) zdohnal   (1000)        0 2024-04-17 13:07:47.490276 pycups-2.0.2/pycups.egg-info/
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1197 2024-04-17 13:07:47.000000 pycups-2.0.2/pycups.egg-info/PKG-INFO
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)      339 2024-04-17 13:07:47.000000 pycups-2.0.2/pycups.egg-info/SOURCES.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        1 2024-04-17 13:07:47.000000 pycups-2.0.2/pycups.egg-info/dependency_links.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)        5 2024-04-17 13:07:47.000000 pycups-2.0.2/pycups.egg-info/top_level.txt
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)       38 2024-04-17 13:07:47.490276 pycups-2.0.2/setup.cfg
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     2663 2024-04-17 11:31:11.000000 pycups-2.0.2/setup.py
+-rw-r--r--   0 zdohnal   (1000) zdohnal   (1000)     1401 2023-04-06 08:19:15.000000 pycups-2.0.2/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pycups-2.0.1/COPYING` & `pycups-2.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `pycups-2.0.1/Makefile` & `pycups-2.0.2/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-PYTHON=python
+PYTHON=python3
 NAME=pycups
 VERSION:=$(shell $(PYTHON) setup.py --version)
 SDIST_ARGS=--formats=gztar -d.
 RPMCONFIGDIR:=$(shell rpm -E "%{_rpmconfigdir}" 2>/dev/null || :)
 
 SOURCES=cupsmodule.c cupsconnection.c cupsppd.c cupsipp.c setup.py \
 	cupsppd.h cupsipp.h cupsconnection.h cupsmodule.h \
@@ -14,21 +14,23 @@
 
 cups.so: force
 	$(PYTHON) setup.py build
 	ln -sf build/lib*/$@ .
 
 doc:	cups.so
 	rm -rf html
-	epydoc -o html --html $<
+	$(PYTHON) -m pydoc -w cups
+	mkdir html
+	mv cups.html html
 
 doczip:	doc
 	cd html && zip ../cups-html.zip *
 
 clean:
-	-rm -rf build cups.so *.pyc *~
+	-rm -rf build cups.so html *.pyc *~ __pycache__
 
 dist:
 	$(PYTHON) setup.py sdist $(SDIST_ARGS)
 
 upload:
 	$(PYTHON) setup.py sdist $(SDIST_ARGS) upload -s
```

### Comparing `pycups-2.0.1/NEWS` & `pycups-2.0.2/NEWS`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 NEWS
 ----
 
+New in 2.0.2:
+- removed shebang from example/cupstree.py
+- ignore driverless utilities for postscriptdriver tags creation (Fedora bug #1873385)
+- remove epydoc from Makefile (#27)
+- fix invalid delete of pointer (#11)
+- Makefile uses wrong Python (#32)
+- define PY_SSIZE_T_CLEAN in cupsipp.h - fixes traceback during IPPRequest.writeIO
+  with Python 3.10
+- fix the test.py when there is no printer installed (#46)
+- Use PyObject_Call() instead of deprecated PyEval
+
 New in 2.0.1:
 * pypi required .tar.gz
 * cups.require couldn't handle version bigger than 1
 
 New in 2.0.0:
 * dropped macros for older CUPS < 2.0.0
 * dropped Python 2 support and its related macros
```

### Comparing `pycups-2.0.1/README` & `pycups-2.0.2/README`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 CUPS bindings for Python
 ------------------------
 
 These Python bindings are intended to wrap the CUPS API.
 
 Python 3 or later is required since Python 2 is unsupported since 2020-01-01.
 
+CUPS >= 1.7 is required for the latest pycups version. 
+
 Build dependencies
 ------------------
 
 The following packages are needed for compiling PyCUPS. GCC compiler is needed because modules are written
 in C. CUPS development files are needed for providing CUPS API, which are used in modules and Python3
 development files for Python3 functions called in modules.
 
 Packages needed for compilation (default package names are from Fedora, Ubuntu names are in the brackets
 if they differ from Fedora):
 
 - gcc
 - cups-devel (libcups2-dev)
 - python3-devel (python3-dev)
+- (since Python 3.12) python3-setuptools
 
 Please install them before compiling PyCUPS.
 
 Runtime dependencies
 --------------------
 
 CUPS needs to be installed and running for PyCUPS working correctly.
```

### Comparing `pycups-2.0.1/cupsconnection.c` & `pycups-2.0.2/cupsconnection.c`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,22 @@
       args = Py_BuildValue ("(sOssO)", prompt, self, method, resource,
 			    cb_context);
     else
       args = Py_BuildValue ("(sOss)", prompt, self, method, resource);
   } else
     args = Py_BuildValue ("(s)", prompt);
 
-  result = PyEval_CallObject (tls->cups_password_callback, args);
+  if (!args)
+  {
+    debugprintf ("Py_BuildValue failed!");
+    Connection_begin_allow_threads (self);
+    return NULL;
+  }
+
+  result = PyObject_Call (tls->cups_password_callback, args, NULL);
   Py_DECREF (args);
   if (result == NULL)
   {
     debugprintf ("<- password_callback (exception)\n");
     Connection_begin_allow_threads (self);
     return NULL;
   }
@@ -589,15 +596,21 @@
   copy_dest (destobj, dest);
   args = Py_BuildValue ("(OiO)",
 			context->user_data,
 			flags,
 			destobj);
   Py_DECREF ((PyObject *) destobj);
 
-  result = PyEval_CallObject (context->cb, args);
+  if (!args)
+  {
+    debugprintf ("Py_BuildValue() failed!\n");
+    return 0;
+  }
+
+  result = PyObject_Call (context->cb, args, NULL);
   Py_DECREF (args);
   if (result == NULL) {
     debugprintf ("<- cups_dest_cb (exception from cb func)\n");
     ret = 0;
   }
 
 
@@ -3919,14 +3932,15 @@
 		    NULL, format);
 
     Connection_begin_allow_threads (self);
     answer = cupsDoFileRequest (self->http, request, resource, file);
     Connection_end_allow_threads (self);
     if (answer && ippGetStatusCode (answer) == IPP_NOT_POSSIBLE) {
       ippDelete (answer);
+      answer = NULL;
       // Perhaps it's a class, not a printer.
       construct_uri (uri, sizeof (uri),
 		     "ipp://localhost/classes/", printer);
     } else break;
   }
 
   free (printer);
@@ -4709,15 +4723,15 @@
       free_string_list (num_filenames, filenames);
       free (printer);
       PyErr_SetString (PyExc_TypeError, "Keys and values must be strings");
       return NULL;
     }
 
     num_settings = cupsAddOption (UTF8_from_PyObj (&name, key),
-				  UTF8_from_PyObj (&value, key),
+				  UTF8_from_PyObj (&value, val),
 				  num_settings,
 				  &settings);
     free (name);
     free (value);
   }
 
   Connection_begin_allow_threads (self);
```

### Comparing `pycups-2.0.1/cupsconnection.h` & `pycups-2.0.2/cupsconnection.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.1/cupsipp.c` & `pycups-2.0.2/cupsipp.c`

 * *Files 1% similar despite different names*

```diff
@@ -567,15 +567,15 @@
   debugprintf ("-> cupsipp_iocb_read\n");
 
   if (!args) {
     debugprintf ("Py_BuildValue failed\n");
     goto out;
   }
 
-  result = PyEval_CallObject (callable, args);
+  result = PyObject_Call (callable, args, NULL);
   Py_DECREF (args);
 
   if (result == NULL) {
     debugprintf ("Exception in read callback\n");
     goto out;
   }
 
@@ -619,15 +619,15 @@
   debugprintf ("-> cupsipp_iocb_write\n");
 
   if (!args) {
     debugprintf ("Py_BuildValue failed\n");
     goto out;
   }
 
-  result = PyEval_CallObject (callable, args);
+  result = PyObject_Call (callable, args, NULL);
   Py_DECREF (args);
 
   if (result == NULL) {
     debugprintf ("Exception in write callback\n");
     goto out;
   }
```

### Comparing `pycups-2.0.1/cupsipp.h` & `pycups-2.0.2/cupsipp.h`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
  * along with this program; if not, write to the Free Software
  * Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
  */
 
 #ifndef HAVE_CUPSIPP_H
 #define HAVE_CUPSIPP_H
 
+#define PY_SSIZE_T_CLEAN
+
 #include <Python.h>
 #include <cups/ipp.h>
 
 extern PyMethodDef IPPRequest_methods[];
 extern PyTypeObject cups_IPPRequestType;
 
 extern PyMethodDef IPPAttribute_methods[];
```

### Comparing `pycups-2.0.1/cupsmodule.c` & `pycups-2.0.2/cupsmodule.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.1/cupsmodule.h` & `pycups-2.0.2/cupsmodule.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.1/cupsppd.c` & `pycups-2.0.2/cupsppd.c`

 * *Files identical despite different names*

### Comparing `pycups-2.0.1/cupsppd.h` & `pycups-2.0.2/cupsppd.h`

 * *Files identical despite different names*

### Comparing `pycups-2.0.1/examples/cupstree.py` & `pycups-2.0.2/examples/cupstree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,72 @@
-#!/usr/bin/python
 import cups
 
 def do_indent (indent):
-	return "  "*indent
+    return "  "*indent
 
 def getippqueue (dev, queue, depth):
-	name = dev.rfind ('/')
-	name = dev[name + 1:]
-	dev = dev[6:]
-	e = dev.find (':')
-	if e == -1:
-		e = dev.find ('/')
-	host = dev[:e]
-	cups.setServer (host)
-	try:
-		c = cups.Connection ()
-		printers = c.getPrinters ()
-		classes = c.getClasses ()
-	except RuntimeError:
-		# Failed to connect.
-		return
-	except cups.IPPError as e:
-		if e == cups.IPP_OPERATION_NOT_SUPPORTED:
-			# CUPS-Get-Printers not supported so not a CUPS server.
-			printers = {}
-			classes = {}
-		else:
-			return
-
-	queue = c.getPrinterAttributes (name)
-	dev = queue['device-uri']
-	getqueue (name, queue, host, depth + 1, printers, classes)
+    name = dev.rfind ('/')
+    name = dev[name + 1:]
+    dev = dev[6:]
+    e = dev.find (':')
+    if e == -1:
+        e = dev.find ('/')
+    host = dev[:e]
+    cups.setServer (host)
+    try:
+        c = cups.Connection ()
+        printers = c.getPrinters ()
+        classes = c.getClasses ()
+    except RuntimeError:
+        # Failed to connect.
+        return
+    except cups.IPPError as e:
+        if e == cups.IPP_OPERATION_NOT_SUPPORTED:
+            # CUPS-Get-Printers not supported so not a CUPS server.
+            printers = {}
+            classes = {}
+        else:
+            return
+
+    queue = c.getPrinterAttributes (name)
+    dev = queue['device-uri']
+    getqueue (name, queue, host, depth + 1, printers, classes)
 
 def getqueue (name, queue, host, depth, printers, classes):
-	indent = do_indent(depth)
-	if queue['printer-type'] & cups.CUPS_PRINTER_CLASS:
-		print ("%s* Name:\t%s[@%s] (class)" % (indent, name, host))
-		dev = queue['device-uri']
-		if dev.startswith ('ipp:'):
-			getippqueue (dev, queue, depth)
-		else:
-			members = classes[name]
-			depth += 1
-			indent = do_indent(depth)
-			for member in members:
-				getqueue (member, printers[member], host,
-					  depth, printers, classes)
-	else:
-		print ("%s* Name:\t%s[@%s]" % (indent, name, host))
-		dev = queue['device-uri']
-		info = queue['printer-info']
-		print ("%sURI:\t%s" % (indent, dev))
-		print ("%sInfo:\t%s" % (indent, info))
-		if dev.startswith ('ipp:'):
-			getippqueue (dev, name, depth)
+    indent = do_indent(depth)
+    if queue['printer-type'] & cups.CUPS_PRINTER_CLASS:
+        print ("%s* Name:\t%s[@%s] (class)" % (indent, name, host))
+        dev = queue['device-uri']
+        if dev.startswith ('ipp:'):
+            getippqueue (dev, queue, depth)
+        else:
+            members = classes[name]
+            depth += 1
+            indent = do_indent(depth)
+            for member in members:
+                getqueue (member, printers[member], host,
+                          depth, printers, classes)
+    else:
+        print ("%s* Name:\t%s[@%s]" % (indent, name, host))
+        dev = queue['device-uri']
+        info = queue['printer-info']
+        print ("%sURI:\t%s" % (indent, dev))
+        print ("%sInfo:\t%s" % (indent, info))
+        if dev.startswith ('ipp:'):
+            getippqueue (dev, name, depth)
 
-	if depth == 0:
-		print ("")
+    if depth == 0:
+        print ("")
 
 def gethost (host=None, depth=0):
-	if host:
-		cups.setServer (host)
-	else:
-		host = "localhost"
-	c = cups.Connection ()
-	printers = c.getPrinters ()
-	classes = c.getClasses ()
-	indent = do_indent(depth)
-	for name, queue in printers.items ():
-		getqueue (name, queue, host, depth, printers, classes)
+    if host:
+        cups.setServer (host)
+    else:
+        host = "localhost"
+    c = cups.Connection ()
+    printers = c.getPrinters ()
+    classes = c.getClasses ()
+    indent = do_indent(depth)
+    for name, queue in printers.items ():
+        getqueue (name, queue, host, depth, printers, classes)
 
 gethost()
```

### Comparing `pycups-2.0.1/postscriptdriver.prov` & `pycups-2.0.2/postscriptdriver.prov`

 * *Files 4% similar despite different names*

```diff
@@ -239,15 +239,16 @@
         if filelist == None:
             filelist = sys.stdin
 
         paths = [x.rstrip () for x in filelist.readlines ()]
         self.ids = DeviceIDs ()
 
         for path in paths:
-            if path.find ("/usr/lib/cups/driver/") != -1:
+            if path.find ("/usr/lib/cups/driver/") != -1 and \
+               path.find("driverless") == -1:
                 try:
                     self.ids += DynamicDriver (path).list ()
                 except TimedOut:
                     pass
                 except OSError as exc:
                     (e, s) = exc.args
                     if e == errno.EACCES or e == errno.ENOENT:
```

### Comparing `pycups-2.0.1/setup.py` & `pycups-2.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,47 +22,47 @@
 CUPS project.
 
 >>> # Example of getting a list of printers
 >>> import cups
 >>> conn = cups.Connection ()
 >>> printers = conn.getPrinters ()
 >>> for printer in printers:
-...     print printer, printers[printer]["device-uri"]
+    ...     print printer, printers[printer]["device-uri"]
 ...
 HP ipp://192.168.1.1:631/printers/HP
 duplex ipp://192.168.1.1:631/printers/duplex
 HP-LaserJet-6MP ipp://192.168.1.1:631/printers/HP-LaserJet-6MP
 EPSON-Stylus-D78 usb://EPSON/Stylus%20D78
 """
 
 from distutils.core import setup, Extension
 import sys
-VERSION="2.0.1"
+VERSION="2.0.2"
 libraries=["cups"]
 
 if sys.platform == "darwin" or sys.platform.startswith("freebsd"):
-	libraries.append ("iconv")
+    libraries.append ("iconv")
 
 setup (name="pycups",
        version=VERSION,
        description="Python bindings for libcups",
        long_description=__doc__,
        maintainer="Zdenek Dohnal",
        maintainer_email="zdohnal@redhat.com",
-       url="https://github.com/zdohnal/pycups",
-       download_url="https://github.com/zdohnal/pycups/releases",
+       url="https://github.com/OpenPrinting/pycups",
+       download_url="https://github.com/OpenPrinting/pycups/releases",
        classifiers=[
-		"Intended Audience :: Developers",
-		"Topic :: Software Development :: Libraries :: Python Modules",
-		"License :: OSI Approved :: GNU General Public License (GPL)",
-		"Development Status :: 5 - Production/Stable",
-		"Operating System :: Unix",
-		"Programming Language :: C",
-		"Programming Language :: Python",
-		"Programming Language :: Python :: 3",
-		],
+           "Intended Audience :: Developers",
+           "Topic :: Software Development :: Libraries :: Python Modules",
+           "License :: OSI Approved :: GNU General Public License (GPL)",
+           "Development Status :: 5 - Production/Stable",
+           "Operating System :: Unix",
+           "Programming Language :: C",
+           "Programming Language :: Python",
+           "Programming Language :: Python :: 3",
+           ],
        license="GPLv2+",
        ext_modules=[Extension("cups",
                               ["cupsmodule.c", "cupsconnection.c",
                                "cupsppd.c", "cupsipp.c"],
                               libraries=libraries,
                               define_macros=[("VERSION", '"%s"' % VERSION)])])
```

