# Comparing `tmp/jbxapi-3.8.0-py2.py3-none-any.whl.zip` & `tmp/jbxapi-3.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 15428 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    55464 b- defN 20-Jun-30 14:41 jbxapi.py
--rw-rw-rw-  2.0 fat     1069 b- defN 20-Jun-30 14:42 jbxapi-3.8.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      835 b- defN 20-Jun-30 14:42 jbxapi-3.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      116 b- defN 20-Jun-30 14:42 jbxapi-3.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       40 b- defN 20-Jun-30 14:42 jbxapi-3.8.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 20-Jun-30 14:42 jbxapi-3.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      541 b- defN 20-Jun-30 14:42 jbxapi-3.8.0.dist-info/RECORD
-7 files, 58072 bytes uncompressed, 14470 bytes compressed:  75.1%
+Zip file size: 15799 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    58989 b- defN 20-Jul-28 19:45 jbxapi.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 20-Jul-28 19:46 jbxapi-3.9.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      835 b- defN 20-Jul-28 19:46 jbxapi-3.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      116 b- defN 20-Jul-28 19:46 jbxapi-3.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       40 b- defN 20-Jul-28 19:46 jbxapi-3.9.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 20-Jul-28 19:46 jbxapi-3.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      541 b- defN 20-Jul-28 19:46 jbxapi-3.9.0.dist-info/RECORD
+7 files, 61597 bytes uncompressed, 14841 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jbxapi.py
 Comment: 
 
-Filename: jbxapi-3.8.0.dist-info/LICENSE
+Filename: jbxapi-3.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: jbxapi-3.8.0.dist-info/METADATA
+Filename: jbxapi-3.9.0.dist-info/METADATA
 Comment: 
 
-Filename: jbxapi-3.8.0.dist-info/WHEEL
+Filename: jbxapi-3.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: jbxapi-3.8.0.dist-info/entry_points.txt
+Filename: jbxapi-3.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: jbxapi-3.8.0.dist-info/top_level.txt
+Filename: jbxapi-3.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jbxapi-3.8.0.dist-info/RECORD
+Filename: jbxapi-3.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jbxapi.py

```diff
@@ -29,15 +29,15 @@
 
 try:
     import requests
 except ImportError:
     print("Please install the Python 'requests' package via pip", file=sys.stderr)
     sys.exit(1)
 
-__version__ = "3.8.0"
+__version__ = "3.9.0"
 
 # API URL.
 API_URL = "https://jbxcloud.joesecurity.org/api"
 # for on-premise installations, use the following URL:
 # API_URL = "http://" + webserveraddress + "/joesandbox/index.php/api"
 
 # APIKEY, to generate goto user settings - API key
@@ -537,17 +537,14 @@
 
         return self._raise_or_extract(response)
 
     def joelab_filesystem_download(self, machine, path, file):
         """
         Download a file from a Joe Lab machine.
 
-        When `file` is given, the return value is the filename specified by the server,
-        otherwise it's a tuple of (filename, bytes).
-
         Parameters:
             machine:  The machine id.
             path:     The path of the file on the Joe Lab machine.
             file:     a writable file-like object
 
         Example:
 
@@ -596,14 +593,74 @@
         params['accept-tac'] = "1" if self.accept_tac else "0"
         params['machine'] = machine
 
         response = self._post(self.apiurl + "/v2/joelab/network/update", data=params)
 
         return self._raise_or_extract(response)
 
+    def joelab_pcap_start(self, machine):
+        """
+        Start PCAP recording.
+        """
+
+        params = {
+            'apikey': self.apikey,
+            'accept-tac': "1" if self.accept_tac else "0",
+            'machine': machine,
+        }
+
+        response = self._post(self.apiurl + "/v2/joelab/pcap/start", data=params)
+
+        return self._raise_or_extract(response)
+
+    def joelab_pcap_stop(self, machine):
+        """
+        Stop PCAP recording.
+        """
+
+        params = {
+            'apikey': self.apikey,
+            'accept-tac': "1" if self.accept_tac else "0",
+            'machine': machine,
+        }
+
+        response = self._post(self.apiurl + "/v2/joelab/pcap/stop", data=params)
+
+        return self._raise_or_extract(response)
+
+    def joelab_pcap_download(self, machine, file):
+        """
+        Download the captured PCAP.
+
+        Parameters:
+            machine:  The machine id.
+            file:     a writable file-like object
+
+        Example:
+
+            with open("dump.pcap", "wb") as f:
+                joe.joelab_pcap_download("w7_10", f)
+        """
+
+        data = {'apikey': self.apikey,
+                'machine': machine}
+
+        response = self._post(self.apiurl + "/v2/joelab/pcap/download", data=data, stream=True)
+
+        # do standard error handling when encountering an error (i.e. throw an exception)
+        if not response.ok:
+            self._raise_or_extract(response)
+            raise RuntimeError("Unreachable because statement above should raise.")
+
+        try:
+            for chunk in response.iter_content(1024):
+                file.write(chunk)
+        except requests.exceptions.RequestException as e:
+            raise ConnectionError(e)
+
     def joelab_list_exitpoints(self):
         """
         List the available internet exit points.
         """
         response = self._post(self.apiurl + "/v2/joelab/internet-exitpoints/list", data={'apikey': self.apikey})
 
         return self._raise_or_extract(response)
@@ -880,22 +937,36 @@
     def joelab_images_reset(joe, args):
         print_json(joe.joelab_images_reset(args.machine, args.image))
 
     def joelab_network_info(joe, args):
         print_json(joe.joelab_network_info(args.machine))
 
     def joelab_network_update(joe, args):
-        print(args)
-        return
-
         print_json(joe.joelab_network_update(args.machine, {
             "internet-enabled": args.enable_internet,
             "internet-exitpoint": args.internet_exitpoint,
         }))
 
+    def joelab_pcap_start(joe, args):
+        print_json(joe.joelab_pcap_start(args.machine))
+
+    def joelab_pcap_stop(joe, args):
+        print_json(joe.joelab_pcap_stop(args.machine))
+
+    def joelab_pcap_download(joe, args):
+        output_path = args.destination
+        if os.path.isdir(output_path):
+            filename = "{}.pcap".format(args.machine)
+            output_path = os.path.join(output_path, filename)
+
+        with open(output_path, "wb") as f:
+            joe.joelab_pcap_download(args.machine, f)
+
+        print_json({"path": os.path.abspath(output_path)})
+
     def joelab_exitpoints_list(joe, args):
         print_json(joe.joelab_list_exitpoints())
 
     # common arguments
     common_parser = argparse.ArgumentParser(add_help=False)
     common_group = common_parser.add_argument_group("common arguments")
     common_group.add_argument('--apiurl',
@@ -915,15 +986,15 @@
 
     # add subparsers
     subparsers = parser.add_subparsers(metavar="<command>", title="commands")
     subparsers.required = True
 
     # submit <filepath>
     submit_parser = subparsers.add_parser('submit', parents=[common_parser],
-            usage="%(prog)s [--apiurl APIKEY] [--apikey APIKEY] [--accept-tac]\n" +
+            usage="%(prog)s [--apiurl APIURL] [--apikey APIKEY] [--accept-tac]\n" +
                   24 * " " + "[parameters ...]\n" +
                   24 * " " + "[--url | --sample-url | --cookbook COOKBOOK]\n" +
                   24 * " " + "sample",
             help="Submit a sample to Joe Sandbox.")
     submit_parser.add_argument('sample',
             help="Path or URL to the sample.")
 
@@ -1233,14 +1304,39 @@
     joelab_network_update_parser.add_argument("--machine", required=True, help="Joe Lab machine ID")
     joelab_network_update_parser.add_argument("--enable-internet", dest="enable_internet", action="store_true", default=None,
             help="Enable Internet")
     joelab_network_update_parser.add_argument("--disable-internet", dest="enable_internet", action="store_false", default=None)
     joelab_network_update_parser.add_argument("--internet-exitpoint")
     joelab_network_update_parser.set_defaults(func=joelab_network_update)
 
+    # joelab pcap <command>
+    joelab_pcap_parser = joelab_subparsers.add_parser('pcap',
+            help="PCAP Commands")
+    joelab_pcap_subparsers = joelab_pcap_parser.add_subparsers(metavar="<command>", title="PCAP commands")
+    joelab_pcap_subparsers.required = True
+
+    # joelab pcap download
+    joelab_pcap_download_parser = joelab_pcap_subparsers.add_parser('download', parents=[common_parser],
+            help="Download the most recent PCAP")
+    joelab_pcap_download_parser.add_argument("--machine", required=True, help="Joe Lab machine ID")
+    joelab_pcap_download_parser.add_argument("-d", "--destination", default=".", help="Destination", metavar="PATH")
+    joelab_pcap_download_parser.set_defaults(func=joelab_pcap_download)
+
+    # joelab pcap start
+    joelab_pcap_start_parser = joelab_pcap_subparsers.add_parser('start', parents=[common_parser],
+            help="Start PCAP recodring")
+    joelab_pcap_start_parser.add_argument("--machine", required=True, help="Joe Lab machine ID")
+    joelab_pcap_start_parser.set_defaults(func=joelab_pcap_start)
+
+    # joelab pcap stop
+    joelab_pcap_stop_parser = joelab_pcap_subparsers.add_parser('stop', parents=[common_parser],
+            help="Stop PCAP recording")
+    joelab_pcap_stop_parser.add_argument("--machine", required=True, help="Joe Lab machine ID")
+    joelab_pcap_stop_parser.set_defaults(func=joelab_pcap_stop)
+
     # joelab internet-exitpoints <command>
     joelab_exitpoints_parser = joelab_subparsers.add_parser('internet-exitpoints',
             help="Exitpoints Commands")
     joelab_exitpoints_subparsers = joelab_exitpoints_parser.add_subparsers(metavar="<command>", title="internet exitpoints commands")
     joelab_exitpoints_subparsers.required = True
 
     # joelab internet-exitpoints list
```

## Comparing `jbxapi-3.8.0.dist-info/LICENSE` & `jbxapi-3.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jbxapi-3.8.0.dist-info/METADATA` & `jbxapi-3.9.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jbxapi
-Version: 3.8.0
+Version: 3.9.0
 Summary: API for Joe Sandbox
 Home-page: https://github.com/joesecurity/joesandboxcloudapi
 Author: Joe Security LLC
 Author-email: UNKNOWN
 License: MIT
 Keywords: security sandbox joe
 Platform: UNKNOWN
```

