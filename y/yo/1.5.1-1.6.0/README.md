# Comparing `tmp/yo-1.5.1.tar.gz` & `tmp/yo-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yo-1.5.1.tar", last modified: Tue Apr  9 20:41:46 2024, max compression
+gzip compressed data, was "yo-1.6.0.tar", last modified: Wed Apr 17 18:06:51 2024, max compression
```

## Comparing `yo-1.5.1.tar` & `yo-1.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.978702 yo-1.5.1/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-08-25 14:24:53.000000 yo-1.5.1/LICENSE.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3770 2024-04-09 20:41:46.978702 yo-1.5.1/PKG-INFO
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-08-25 14:24:53.000000 yo-1.5.1/README.md
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-08-25 14:24:53.000000 yo-1.5.1/THIRD_PARTY_LICENSES.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)      307 2024-04-09 20:41:46.978702 yo-1.5.1/setup.cfg
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3464 2024-04-09 20:41:38.000000 yo-1.5.1/setup.py
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.977702 yo-1.5.1/tests/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-08-25 14:24:53.000000 yo-1.5.1/tests/test_api.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     7576 2023-12-16 00:08:45.000000 yo-1.5.1/tests/test_cmds.py
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.977702 yo-1.5.1/yo/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)        0 2023-08-25 14:24:53.000000 yo-1.5.1/yo/__init__.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-08-25 14:24:53.000000 yo-1.5.1/yo/__main__.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)    86546 2024-02-05 18:25:03.000000 yo-1.5.1/yo/api.py
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.977702 yo-1.5.1/yo/data/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     9194 2023-12-16 00:08:45.000000 yo-1.5.1/yo/data/sample.yo.ini
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.978702 yo-1.5.1/yo/data/yo-tasks/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/drgn
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/ocid
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/test-deps
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)       23 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/test-existing-task
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/test-run-many
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/test-task
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo_tasklib.sh
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)   135139 2024-04-09 20:41:38.000000 yo-1.5.1/yo/main.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     6384 2023-12-16 00:08:45.000000 yo-1.5.1/yo/oci.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)    10415 2023-09-01 17:04:54.000000 yo-1.5.1/yo/util.py
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.977702 yo-1.5.1/yo.egg-info/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3770 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/PKG-INFO
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)      541 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/SOURCES.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)        1 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/dependency_links.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)       37 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/entry_points.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)       72 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/requires.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)        3 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/top_level.txt
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-17 18:06:51.106844 yo-1.6.0/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-08-25 14:24:53.000000 yo-1.6.0/LICENSE.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3770 2024-04-17 18:06:51.106844 yo-1.6.0/PKG-INFO
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-08-25 14:24:53.000000 yo-1.6.0/README.md
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-08-25 14:24:53.000000 yo-1.6.0/THIRD_PARTY_LICENSES.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)      307 2024-04-17 18:06:51.106844 yo-1.6.0/setup.cfg
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3464 2024-04-17 18:06:45.000000 yo-1.6.0/setup.py
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-17 18:06:51.105844 yo-1.6.0/tests/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-08-25 14:24:53.000000 yo-1.6.0/tests/test_api.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     7670 2024-04-17 18:06:45.000000 yo-1.6.0/tests/test_cmds.py
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-17 18:06:51.106844 yo-1.6.0/yo/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)        0 2023-08-25 14:24:53.000000 yo-1.6.0/yo/__init__.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-08-25 14:24:53.000000 yo-1.6.0/yo/__main__.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)    86637 2024-04-17 18:06:45.000000 yo-1.6.0/yo/api.py
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-17 18:06:51.106844 yo-1.6.0/yo/data/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     9556 2024-04-17 18:06:45.000000 yo-1.6.0/yo/data/sample.yo.ini
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-17 18:06:51.106844 yo-1.6.0/yo/data/yo-tasks/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-08-25 14:24:53.000000 yo-1.6.0/yo/data/yo-tasks/drgn
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-08-25 14:24:53.000000 yo-1.6.0/yo/data/yo-tasks/ocid
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-08-25 14:24:53.000000 yo-1.6.0/yo/data/yo-tasks/test-deps
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)       23 2023-08-25 14:24:53.000000 yo-1.6.0/yo/data/yo-tasks/test-existing-task
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-08-25 14:24:53.000000 yo-1.6.0/yo/data/yo-tasks/test-run-many
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-08-25 14:24:53.000000 yo-1.6.0/yo/data/yo-tasks/test-task
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-08-25 14:24:53.000000 yo-1.6.0/yo/data/yo_tasklib.sh
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)   136778 2024-04-17 18:06:45.000000 yo-1.6.0/yo/main.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     6384 2023-12-16 00:08:45.000000 yo-1.6.0/yo/oci.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)    10474 2024-04-17 18:06:45.000000 yo-1.6.0/yo/util.py
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-17 18:06:51.106844 yo-1.6.0/yo.egg-info/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3770 2024-04-17 18:06:51.000000 yo-1.6.0/yo.egg-info/PKG-INFO
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)      541 2024-04-17 18:06:51.000000 yo-1.6.0/yo.egg-info/SOURCES.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)        1 2024-04-17 18:06:51.000000 yo-1.6.0/yo.egg-info/dependency_links.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)       37 2024-04-17 18:06:51.000000 yo-1.6.0/yo.egg-info/entry_points.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)       72 2024-04-17 18:06:51.000000 yo-1.6.0/yo.egg-info/requires.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)        3 2024-04-17 18:06:51.000000 yo-1.6.0/yo.egg-info/top_level.txt
```

### Comparing `yo-1.5.1/LICENSE.txt` & `yo-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/PKG-INFO` & `yo-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.5.1
+Version: 1.6.0
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Description: # yo - fast and simple OCI client
```

### Comparing `yo-1.5.1/README.md` & `yo-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/THIRD_PARTY_LICENSES.txt` & `yo-1.6.0/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/setup.py` & `yo-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md").read()
 
-VERSION = "1.5.1"
+VERSION = "1.6.0"
 
 setup(
     name="yo",
     version=VERSION,
     description="A fast and simple CLI client for managing OCI instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `yo-1.5.1/tests/test_api.py` & `yo-1.6.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/tests/test_cmds.py` & `yo-1.6.0/tests/test_cmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,30 @@
 # SOFTWARE.
 import contextlib
 import dataclasses
 from unittest import mock
 
 import pytest
 
+from tests.testing.factories import config_factory
 from tests.testing.factories import image_factory
 from tests.testing.factories import instance_factory
 from tests.testing.rich import FakeTable
 from yo.main import YoCmd
 from yo.util import strftime
 
 
 @pytest.fixture
 def mock_ctx():
     es = contextlib.ExitStack()
     with es:
         mock_ctx = es.enter_context(
             mock.patch("yo.main.YoCtx"),
         ).return_value
+        mock_ctx.config = config_factory()
         mock_con = es.enter_context(
             mock.patch(
                 "rich.console.Console",
                 autospec=True,
             )
         ).return_value
         mock_ctx.con = mock_con
```

### Comparing `yo-1.5.1/yo/__main__.py` & `yo-1.6.0/yo/__main__.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/yo/api.py` & `yo-1.6.0/yo/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,14 +285,15 @@
     shape: str
     memory_gb: int
     ocpu: int
     time_created: datetime.datetime
     image_id: str
     termination_protected: bool
     freeform_tags: t.Dict[str, str]
+    defined_tags: t.Dict[str, t.Dict[str, str]]
     username: t.Optional[str]  # from tag
 
     @classmethod
     def from_oci(cls, oci: "Instance") -> "YoInstance":
         term_protect = oci.freeform_tags.get(TERMPROTECT, "false") == "true"
         return cls(
             id=oci.id,
@@ -302,14 +303,15 @@
             shape=oci.shape,
             memory_gb=oci.shape_config.memory_in_gbs,
             ocpu=oci.shape_config.ocpus,
             time_created=oci.time_created,
             image_id=oci.image_id,
             termination_protected=term_protect,
             freeform_tags=oci.freeform_tags,
+            defined_tags=oci.defined_tags,
             username=oci.freeform_tags.get(USERNAME),
         )
 
 
 @dataclasses.dataclass
 class YoVnic(YoCachedWithId):
     ad: str
@@ -966,15 +968,15 @@
     con: rich.console.Console
     config: YoConfig
     instance_profiles: t.Mapping[str, InstanceProfile]
 
     cache_version = 1
     last_checked_for_update: datetime.datetime
 
-    _instances: YoCache[YoInstance] = YoCache(YoInstance, "instances", 4)
+    _instances: YoCache[YoInstance] = YoCache(YoInstance, "instances", 5)
     _vnics: YoCache[YoVnic] = YoCache(YoVnic, "vnics", 2)
     _images: YoCache[YoImage] = YoCache(YoImage, "images", 6)
     _consoles: YoCache[YoConsole] = YoCache(YoConsole, "consoles", 2)
     _shapes: YoCache[YoShape] = YoCache(YoShape, "shapes", 5)
     _vols: YoCache[YoVolume] = YoCache(YoVolume, "bootvols", 5)
     _vas: YoCache[YoVolumeAttachment] = YoCache(YoVolumeAttachment, "vas", 3)
```

### Comparing `yo-1.5.1/yo/data/sample.yo.ini` & `yo-1.6.0/yo/data/sample.yo.ini`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,24 @@
 # operation which typically takes a few seconds, there's virtually no
 # performance impact.
 #
 # However, you can set this to 0 in order to disable these checks.
 #
 # check_for_update_every = 6
 
+# OPTIONAL: list_columns
+#
+# (String, default: Name,Shape,Mem,CPU,State,Created)
+#
+# A comma-separated list of column names to include in the table for the `yo
+# list` command. You can override this on the command line with the `-C`
+# argument. You can add to this on the command line with the `-x` argument.
+#
+# list_columns = Name,Shape,Mem,CPU,State,Created
+
 # Any section prefixed with "instances." declares an instance profile. The
 # instance profile DEFAULT is required, but you can make additional ones as
 # well.
 [instances.DEFAULT]
 
 # REQUIRED: set the availability domain for this instance.
 availability_domain = VkEH:US-ASHBURN-AD-3
```

### Comparing `yo-1.5.1/yo/data/yo-tasks/drgn` & `yo-1.6.0/yo/data/yo-tasks/drgn`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/yo/data/yo-tasks/ocid` & `yo-1.6.0/yo/data/yo-tasks/ocid`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/yo/data/yo-tasks/test-deps` & `yo-1.6.0/yo/data/yo-tasks/test-deps`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/yo/data/yo-tasks/test-run-many` & `yo-1.6.0/yo/data/yo-tasks/test-run-many`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/yo/data/yo-tasks/test-task` & `yo-1.6.0/yo/data/yo-tasks/test-task`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/yo/data/yo_tasklib.sh` & `yo-1.6.0/yo/data/yo_tasklib.sh`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/yo/main.py` & `yo-1.6.0/yo/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 from rich.prompt import Confirm
 
 import yo.util
 from yo.api import AttachmentType
 from yo.api import ImageLoad
 from yo.api import InstanceProfile
 from yo.api import OS_TO_USER
+from yo.api import SavedInstanceMetadata
 from yo.api import VolumeKind
 from yo.api import YoCtx
 from yo.api import YoImage
 from yo.api import YoInstance
 from yo.api import YoShape
 from yo.api import YoVolume
 from yo.api import YoVolumeAttachment
@@ -841,40 +842,110 @@
     please see the documentation for the config "yo.resource_filtering"). You
     can use the "--all" argument to see all of the instances in your
     compartment, regardless of whether Yo believes you created them. Please keep
     in mind that you won't be able to manage those instances (e.g. yo ssh, yo
     terminate, etc) unless you change your "yo.resource_filtering" configuration.
     """
 
+    def _ip_column(self, i: YoInstance) -> str:
+        # It's more efficient to bulk lookup the IPs.
+        if not getattr(self, "_fetched_ips", False):
+            self.c.get_all_instance_ips(self.instances)
+            self._fetched_ips = True
+        return self.c.get_instance_ip(i, quiet=True)
+
+    def _name_column(self, i: YoInstance) -> str:
+        if i.termination_protected:
+            return f":lock: {i.name}"
+        else:
+            return i.name
+
+    Column = t.Tuple[
+        t.Callable[[YoInstance], str],
+        t.Optional[t.Callable[[YoVolume, SavedInstanceMetadata], str]],
+    ]
+
+    def columns(self) -> t.Dict[str, Column]:
+        return {
+            "Name": (self._name_column, lambda v, m: f":warning: {m.name}"),
+            "Shape": (lambda i: i.shape, lambda v, m: m.shape),
+            "CPU": (lambda i: str(int(i.ocpu)), lambda v, m: str(m.ocpu)),
+            "Mem": (
+                lambda i: str(int(i.memory_gb)),
+                lambda v, m: str(m.memory_gb),
+            ),
+            "State": (lambda i: i.state, lambda v, m: "[red]SAVED[/red]"),
+            "AD": (lambda i: i.ad, lambda v, m: v.ad),
+            "Created": (lambda i: strftime(i.time_created), None),
+            "IP": (self._ip_column, None),
+            "ResourceType": (
+                lambda i: i.defined_tags.get("Oracle-Recommended-Tags", {}).get(
+                    "ResourceType", ""
+                ),
+                None,
+            ),
+        }
+
     def add_args(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--cached",
             "-c",
             action="store_true",
             help="avoid loading and calling OCI if possible (list may be"
             "out of date)",
         )
         parser.add_argument(
+            "--columns",
+            "-C",
+            type=str,
+            help="specify all columns in the table",
+        )
+        parser.add_argument(
+            "--extra-column",
+            "-x",
+            action="append",
+            choices=list(self.columns().keys()),
+            default=[],
+            help="add a column to the table",
+        )
+        parser.add_argument(
             "--ip",
             "-i",
             action="store_true",
-            help="include IP addresses (this may require calling the API)",
+            help="include IP addresses column (alias for: -x IP)",
         )
         parser.add_argument(
             "--ad",
             action="store_true",
-            help="display the availability domain column",
+            help="display the availability domain column (alias for: -x AD)",
         )
         parser.add_argument(
             "--all",
             "-a",
             action="store_true",
             help="display all instances in the compartment (not just yours)",
         )
 
+    def get_columns(self) -> t.List[t.Tuple[str, Column]]:
+        names_str = self.args.columns or self.c.config.list_columns
+        names = list(s.strip() for s in names_str.split(","))
+        if self.args.ip:
+            self.args.extra_column.append("IP")
+        if self.args.ad:
+            self.args.extra_column.append("AD")
+        names += self.args.extra_column
+
+        col_defs = self.columns()
+        ret = []
+        for name in names:
+            if name not in col_defs:
+                raise YoExc(f"column {name} has no implementation!")
+            ret.append((name, col_defs[name]))
+        return ret
+
     def run(self) -> None:
         verbose = not self.c.config.silence_automatic_tag_warning
         # We do not cache other people's instances. If --all is provided, we
         # must not call list_instances_cached()
         if self.args.all:
             self.args.cached = False
         if self.args.cached:
@@ -886,66 +957,38 @@
             )
 
         instances = [
             x for x in instances if x.state not in ("TERMINATED", "TERMINATING")
         ]
         instances.sort(key=lambda i: i.time_created)
 
-        # It's more efficient to bulk lookup the IPs. This will cache them so
-        # that below, we don't do individual calls.
-        if self.args.ip:
-            self.c.get_all_instance_ips(instances)
+        # Store instances to as a class variable so column functions could
+        # access them as necessary.
+        self.instances = instances
 
+        columns = self.get_columns()
         table = rich.table.Table()
-        table.add_column("Name")
-        table.add_column("Shape")
-        table.add_column("Mem")
-        table.add_column("CPU")
-        table.add_column("State")
-        if self.args.ad:
-            table.add_column("AD")
-        table.add_column("Created")
-        if self.args.ip:
-            table.add_column("IP")
+        for name, _ in columns:
+            table.add_column(name)
         for instance in instances:
-            name = instance.name
-            if instance.termination_protected:
-                name = ":lock:" + name
-            values = [
-                name,
-                instance.shape,
-                str(int(instance.memory_gb)),
-                str(int(instance.ocpu)),
-                instance.state,
-            ]
-            if self.args.ad:
-                values.append(instance.ad)
-            values += [
-                strftime(instance.time_created),
-            ]
-            if self.args.ip:
-                values.append(self.c.get_instance_ip(instance, quiet=True))
+            values = []
+            for name, (inst_fn, _) in columns:
+                values.append(inst_fn(instance))
             table.add_row(*values)
 
         for volume in self.c.list_volumes():
             md = volume.saved_instance_metadata
             if not md:
                 continue
-            values = [
-                f":warning: {md.name}",
-                md.shape,
-                str(md.memory_gb),
-                str(md.ocpu),
-                "[red]SAVED[/red]",
-            ]
-            if self.args.ad:
-                values.append(volume.ad)
-            values.append("---")
-            if self.args.ip:
-                values.append("---")
+            values = []
+            for _, (_, saved_fn) in columns:
+                if saved_fn:
+                    values.append(saved_fn(volume, md))
+                else:
+                    values.append("---")
             table.add_row(*values)
         self.c.con.print(table)
 
 
 class SingleInstanceCommand(YoCmd):
     positional_name: bool = True
     states_allowlist: t.Collection[str] = ("RUNNING",)
```

### Comparing `yo-1.5.1/yo/oci.py` & `yo-1.6.0/yo/oci.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.1/yo/util.py` & `yo-1.6.0/yo/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     task_dir: str = "/tmp/tasks"
     image_compartment_ids: t.List[str] = dataclasses.field(default_factory=list)
     silence_automatic_tag_warning: t.Optional[bool] = None
     exact_name: t.Optional[bool] = None
     resource_filtering: bool = True
     check_for_update_every: t.Optional[int] = 6
     creator_tags: t.List[str] = dataclasses.field(default_factory=list)
+    list_columns: str = "Name,Shape,Mem,CPU,State,Created"
 
     @property
     def ssh_public_key_full(self) -> str:
         path = os.path.expanduser(self.ssh_public_key)
         return open(path).read()
 
     @property
```

### Comparing `yo-1.5.1/yo.egg-info/PKG-INFO` & `yo-1.6.0/yo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.5.1
+Version: 1.6.0
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Description: # yo - fast and simple OCI client
```

### Comparing `yo-1.5.1/yo.egg-info/SOURCES.txt` & `yo-1.6.0/yo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

