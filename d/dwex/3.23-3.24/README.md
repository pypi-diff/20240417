# Comparing `tmp/dwex-3.23.tar.gz` & `tmp/dwex-3.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwex-3.23.tar", last modified: Wed Nov 15 18:46:20 2023, max compression
+gzip compressed data, was "dwex-3.24.tar", last modified: Wed Apr 17 17:40:01 2024, max compression
```

## Comparing `dwex-3.23.tar` & `dwex-3.24.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-11-15 18:46:20.684834 dwex-3.23/
--rw-rw-rw-   0        0        0     7190 2023-11-15 18:46:20.684834 dwex-3.23/PKG-INFO
--rw-rw-rw-   0        0        0     5990 2023-09-27 19:20:14.000000 dwex-3.23/README.md
-drwxrwxrwx   0        0        0        0 2023-11-15 18:46:20.665834 dwex-3.23/dwex/
--rw-rw-rw-   0        0        0        0 2020-01-31 01:42:48.000000 dwex-3.23/dwex/__init__.py
--rw-rw-rw-   0        0        0    35969 2023-11-15 18:42:05.000000 dwex-3.23/dwex/__main__.py
--rw-rw-rw-   0        0        0       52 2023-11-15 18:46:19.000000 dwex-3.23/dwex/cookie.py
--rw-rw-rw-   0        0        0     4712 2023-09-15 15:47:53.000000 dwex-3.23/dwex/crash.py
--rw-rw-rw-   0        0        0     1558 2023-09-25 16:37:00.000000 dwex-3.23/dwex/details.py
--rw-rw-rw-   0        0        0    19674 2023-11-14 19:56:05.000000 dwex-3.23/dwex/die.py
--rw-rw-rw-   0        0        0    12055 2023-09-15 16:16:00.000000 dwex-3.23/dwex/dwarfone.py
--rw-rw-rw-   0        0        0    18870 2023-09-09 20:24:09.000000 dwex-3.23/dwex/dwarfutil.py
--rw-rw-rw-   0        0        0     7370 2023-11-15 17:26:47.000000 dwex-3.23/dwex/exprutil.py
--rw-rw-rw-   0        0        0    13559 2023-11-14 19:35:35.000000 dwex-3.23/dwex/formats.py
--rw-rw-rw-   0        0        0    11042 2023-09-15 16:18:19.000000 dwex-3.23/dwex/locals.py
--rw-rw-rw-   0        0        0     7152 2023-11-15 16:16:06.000000 dwex-3.23/dwex/locs.py
--rw-rw-rw-   0        0        0     8056 2023-11-15 17:56:15.000000 dwex-3.23/dwex/patch.py
--rw-rw-rw-   0        0        0     5316 2023-10-07 20:55:27.000000 dwex-3.23/dwex/ranges.py
--rw-rw-rw-   0        0        0     3712 2023-11-14 15:51:57.000000 dwex-3.23/dwex/scriptdlg.py
--rw-rw-rw-   0        0        0    16489 2023-09-13 17:15:24.000000 dwex-3.23/dwex/tree.py
--rw-rw-rw-   0        0        0    13794 2023-10-30 15:26:47.000000 dwex-3.23/dwex/ui.py
-drwxrwxrwx   0        0        0        0 2023-11-15 18:46:20.682832 dwex-3.23/dwex.egg-info/
--rw-rw-rw-   0        0        0     7190 2023-11-15 18:46:20.000000 dwex-3.23/dwex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-11-15 18:46:20.000000 dwex-3.23/dwex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-15 18:46:20.000000 dwex-3.23/dwex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-11-15 18:46:20.000000 dwex-3.23/dwex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-11-15 18:46:20.000000 dwex-3.23/dwex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-11-15 18:46:20.000000 dwex-3.23/dwex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-11-15 18:46:20.685834 dwex-3.23/setup.cfg
--rw-rw-rw-   0        0        0     4655 2023-11-15 18:42:12.000000 dwex-3.23/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-15 18:46:20.683834 dwex-3.23/test/
--rw-rw-rw-   0        0        0     4311 2023-09-23 22:52:34.000000 dwex-3.23/test/testall.py
--rw-rw-rw-   0        0        0     2471 2023-09-28 22:42:37.000000 dwex-3.23/test/testlocal.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:40:01.794530 dwex-3.24/
+-rw-rw-rw-   0        0        0     7190 2024-04-17 17:40:01.794530 dwex-3.24/PKG-INFO
+-rw-rw-rw-   0        0        0     5990 2023-09-27 19:20:14.000000 dwex-3.24/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 17:40:01.764220 dwex-3.24/dwex/
+-rw-rw-rw-   0        0        0        0 2020-01-31 01:42:48.000000 dwex-3.24/dwex/__init__.py
+-rw-rw-rw-   0        0        0    37613 2024-04-17 17:37:41.000000 dwex-3.24/dwex/__main__.py
+-rw-rw-rw-   0        0        0       52 2024-04-17 17:40:00.000000 dwex-3.24/dwex/cookie.py
+-rw-rw-rw-   0        0        0     4712 2023-09-15 15:47:53.000000 dwex-3.24/dwex/crash.py
+-rw-rw-rw-   0        0        0     1558 2023-09-25 16:37:00.000000 dwex-3.24/dwex/details.py
+-rw-rw-rw-   0        0        0    19833 2024-04-17 17:31:33.000000 dwex-3.24/dwex/die.py
+-rw-rw-rw-   0        0        0    12091 2024-04-16 16:48:50.000000 dwex-3.24/dwex/dwarfone.py
+-rw-rw-rw-   0        0        0    18870 2023-09-09 20:24:09.000000 dwex-3.24/dwex/dwarfutil.py
+-rw-rw-rw-   0        0        0     7370 2023-11-15 17:26:47.000000 dwex-3.24/dwex/exprutil.py
+-rw-rw-rw-   0        0        0    13559 2023-11-14 19:35:35.000000 dwex-3.24/dwex/formats.py
+-rw-rw-rw-   0        0        0    11042 2023-09-15 16:18:19.000000 dwex-3.24/dwex/locals.py
+-rw-rw-rw-   0        0        0     7152 2023-11-15 16:16:06.000000 dwex-3.24/dwex/locs.py
+-rw-rw-rw-   0        0        0     8241 2024-04-17 14:58:55.000000 dwex-3.24/dwex/patch.py
+-rw-rw-rw-   0        0        0     5316 2023-10-07 20:55:27.000000 dwex-3.24/dwex/ranges.py
+-rw-rw-rw-   0        0        0     3703 2023-11-23 16:54:02.000000 dwex-3.24/dwex/scriptdlg.py
+-rw-rw-rw-   0        0        0    16489 2023-09-13 17:15:24.000000 dwex-3.24/dwex/tree.py
+-rw-rw-rw-   0        0        0    13925 2024-04-17 12:57:41.000000 dwex-3.24/dwex/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:40:01.786489 dwex-3.24/dwex.egg-info/
+-rw-rw-rw-   0        0        0     7190 2024-04-17 17:40:01.000000 dwex-3.24/dwex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2024-04-17 17:40:01.000000 dwex-3.24/dwex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 17:40:01.000000 dwex-3.24/dwex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-17 17:40:01.000000 dwex-3.24/dwex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2024-04-17 17:40:01.000000 dwex-3.24/dwex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 17:40:01.000000 dwex-3.24/dwex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-17 17:40:01.796548 dwex-3.24/setup.cfg
+-rw-rw-rw-   0        0        0     4655 2024-04-17 17:37:29.000000 dwex-3.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:40:01.794530 dwex-3.24/test/
+-rw-rw-rw-   0        0        0     4311 2023-09-23 22:52:34.000000 dwex-3.24/test/testall.py
+-rw-rw-rw-   0        0        0     2471 2023-09-28 22:42:37.000000 dwex-3.24/test/testlocal.py
```

### Comparing `dwex-3.23/PKG-INFO` & `dwex-3.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwex
-Version: 3.23
+Version: 3.24
 Summary: GUI viewer for DWARF debug information
 Home-page: https://github.com/sevaa/dwex/
 Author: Seva Alekseyev
 Author-email: sevaa@sprynet.com
 License: BSD
 Keywords: dwarf,debug,debugging,symbols,viewer,view,browser,browse,tree
 Platform: any
```

### Comparing `dwex-3.23/README.md` & `dwex-3.24/README.md`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/__main__.py` & `dwex-3.24/dwex/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .dwarfutil import has_code_location, ip_in_range
 from .tree import DWARFTreeModel, cu_sort_key
 from .scriptdlg import ScriptDlg, make_execution_environment
 from .ui import setup_ui
 from .locals import LocalsDlg
 
 # Sync with version in setup.py
-version = (3, 23)
+version = (3, 24)
 
 # TODO:
 # On MacOS, start without a main window, instead show the Open dialog
 
 #-----------------------------------------------------------------
 # The one and only main window class
 # Pretty much DWARF unaware, all the DWARF visualization logic is in tree.py and die.py
@@ -88,82 +88,86 @@
     def open_file(self, filename, arch = None):
         self.start_wait()
         try:
             di = read_dwarf(filename, self.resolve_arch if arch is None else lambda arches: arches.index(arch))
             if not di: # Covers both False and None
                 return di
             
-            # Some degree of graceful handling of wrong format
-            try:
-                # Some cached top level stuff
-                # Notably, iter_CUs doesn't cache
-                di._ranges = None # Loaded on first use
-                di._aranges = None
-                def decorate_cu(cu, i):
-                    cu._i = i
-                    cu._lineprogram = None
-                    cu._exprparser = None
-                    return cu
-                di._unsorted_CUs = [decorate_cu(cu, i) for (i, cu) in enumerate(di.iter_CUs())] # We'll need them first thing, might as well load here
-                if not len(di._unsorted_CUs):
-                    return None # Weird, but saw it once - debug sections present, but no CUs
-                # For quick CU search by offset within the info section, regardless of sorting
-                di._CU_offsets = [cu.cu_offset for cu in di._unsorted_CUs]
-                di._CUs = list(di._unsorted_CUs)
-
-                if self.sortcus:
-                    di._CUs.sort(key = cu_sort_key)
-                    for (i, cu) in enumerate(di._CUs):
-                        cu._i = i
-                di._locparser = None # Created on first use
-
-                self.dwarfinfo = di
-                self.filename = filename
-                self.tree_model = DWARFTreeModel(di, self.prefix, self.sortcus, self.sortdies)
-                self.the_tree.setModel(self.tree_model)
-                self.the_tree.selectionModel().currentChanged.connect(self.on_tree_selection)
-                s = os.path.basename(filename)
-                if arch is not None:
-                    s += ' (' + arch + ')'
-                self.setWindowTitle("DWARF Explorer - " + s)
-                self.savesection_menuitem.setEnabled(True)
-                self.back_menuitem.setEnabled(False)
-                self.back_tbitem.setEnabled(False)
-                self.forward_menuitem.setEnabled(False)
-                self.forward_tbitem.setEnabled(False)
-                self.followref_menuitem.setEnabled(False)
-                self.followref_tbitem.setEnabled(False)
-                self.highlightcode_menuitem.setEnabled(True)
-                self.highlightsubstring_menuitem.setEnabled(True)
-                self.highlightcondition_menuitem.setEnabled(True)
-                self.highlightnothing_menuitem.setEnabled(True)
-                self.copy_menuitem.setEnabled(False)
-                self.copy_tbitem.setEnabled(False)
-                self.copyline_menuitem.setEnabled(False)
-                self.copytable_menuitem.setEnabled(False)
-                self.findbycondition_menuitem.setEnabled(True)
-                self.find_menuitem.setEnabled(True)
-                self.find_tbitem.setEnabled(True)
-                self.findip_menuitem.setEnabled(True)
-                self.byoffset_menuitem.setEnabled(True)
-                self.byoffset_tbitem.setEnabled(True)
-                self.localsat_menuitem.setEnabled(True)
-                self.on_highlight_nothing()
-                # Navigation stack - empty
-                self.navhistory = []
-                self.navpos = -1
-                self.save_filename_in_mru(filename, di._fat_arch if '_fat_arch' in dir(di) and di._fat_arch else None)
-                LocalsDlg.reset(di)
-                from .crash import set_binary_desc
-                set_binary_desc(("ELF", "MachO", "PE", "WASM")[di._format] + " " + di.config.machine_arch)
-                return True
-            except AssertionError as ass: # Covers exeptions during parsing
-                raise DWARFParseError(ass, di)
+            return self.load_dwarfinfo(di, filename, arch)
         finally:
             self.end_wait()
+    
+    # May throw if parsing fails
+    def load_dwarfinfo(self, di, filename, arch):
+        # Some degree of graceful handling of wrong format
+        try:
+            # Some cached top level stuff
+            # Notably, iter_CUs doesn't cache (TODO, check that in the next version)
+            di._ranges = None # Loaded on first use
+            di._aranges = None
+            def decorate_cu(cu, i):
+                cu._i = i
+                cu._lineprogram = None
+                cu._exprparser = None
+                return cu
+            di._unsorted_CUs = [decorate_cu(cu, i) for (i, cu) in enumerate(di.iter_CUs())] # We'll need them first thing, might as well load here
+            if not len(di._unsorted_CUs):
+                return None # Weird, but saw it once - debug sections present, but no CUs
+            # For quick CU search by offset within the info section, regardless of sorting
+            di._CU_offsets = [cu.cu_offset for cu in di._unsorted_CUs]
+            di._CUs = list(di._unsorted_CUs)
+
+            if self.sortcus:
+                di._CUs.sort(key = cu_sort_key)
+                for (i, cu) in enumerate(di._CUs):
+                    cu._i = i
+            di._locparser = None # Created on first use - but see #1683
+
+            self.dwarfinfo = di
+            self.filename = filename
+            self.tree_model = DWARFTreeModel(di, self.prefix, self.sortcus, self.sortdies)
+            self.the_tree.setModel(self.tree_model)
+            self.the_tree.selectionModel().currentChanged.connect(self.on_tree_selection)
+            s = os.path.basename(filename)
+            if arch is not None:
+                s += ' (' + arch + ')'
+            self.setWindowTitle("DWARF Explorer - " + s)
+            self.savesection_menuitem.setEnabled(True)
+            self.back_menuitem.setEnabled(False)
+            self.back_tbitem.setEnabled(False)
+            self.forward_menuitem.setEnabled(False)
+            self.forward_tbitem.setEnabled(False)
+            self.followref_menuitem.setEnabled(False)
+            self.followref_tbitem.setEnabled(False)
+            self.highlightcode_menuitem.setEnabled(True)
+            self.highlightsubstring_menuitem.setEnabled(True)
+            self.highlightcondition_menuitem.setEnabled(True)
+            self.highlightnothing_menuitem.setEnabled(True)
+            self.copy_menuitem.setEnabled(False)
+            self.copy_tbitem.setEnabled(False)
+            self.copyline_menuitem.setEnabled(False)
+            self.copytable_menuitem.setEnabled(False)
+            self.findbycondition_menuitem.setEnabled(True)
+            self.find_menuitem.setEnabled(True)
+            self.find_tbitem.setEnabled(True)
+            self.findip_menuitem.setEnabled(True)
+            self.byoffset_menuitem.setEnabled(True)
+            self.byoffset_tbitem.setEnabled(True)
+            self.localsat_menuitem.setEnabled(True)
+            self.on_highlight_nothing()
+            # Navigation stack - empty
+            self.navhistory = []
+            self.navpos = -1
+            self.save_filename_in_mru(filename, di._fat_arch if '_fat_arch' in dir(di) and di._fat_arch else None)
+            LocalsDlg.reset(di)
+            from .crash import set_binary_desc
+            set_binary_desc(("ELF", "MachO", "PE", "WASM")[di._format] + " " + di.config.machine_arch)
+            return True
+        except AssertionError as ass: # Covers exeptions during parsing
+            raise DWARFParseError(ass, di)        
 
     def save_mru(self):
         for i, fa in enumerate(self.mru):
             self.sett.setValue("General/MRU%d" % i, fa[0])    
             if len(fa) > 1:
                 self.sett.setValue("General/MRUArch%d" % i, fa[1])
             else:
@@ -732,14 +736,54 @@
 
     def on_issue(self):
         QDesktopServices.openUrl(QUrl('https://github.com/sevaa/dwex/issues/new'))
 
     def on_homepage(self):
         QDesktopServices.openUrl(QUrl('https://github.com/sevaa/dwex'))
 
+    # All purpose debug hook
+    def on_debug(self):
+        import io
+        from elftools.dwarf.dwarfinfo import DWARFInfo, DwarfConfig, DebugSectionDescriptor
+        # Read the three saved sections as bytestreams
+        base = os.environ.get("DWEX_ARG")
+        with open(base + '.info.dat', 'rb') as f:
+            info = f.read()
+        with open(base + '.abbrev.dat', 'rb') as f:
+            abbrev = f.read()
+        with open(base + '.str.dat', 'rb') as f:
+            str = f.read()
+
+        # Parse the DWARF info
+        di = DWARFInfo(
+            config = DwarfConfig(little_endian = True, default_address_size = 8, machine_arch = "ARM64"),
+            debug_info_sec = DebugSectionDescriptor(io.BytesIO(info), '__debug_info', None, len(info), 0),
+            debug_aranges_sec = None,
+            debug_abbrev_sec = DebugSectionDescriptor(io.BytesIO(abbrev), '__debug_abbrev', None, len(abbrev), 0),
+            debug_frame_sec = None,
+            eh_frame_sec = None,
+            debug_str_sec = DebugSectionDescriptor(io.BytesIO(str), '__debug_str', None, len(str), 0),
+            debug_loc_sec = None,
+            debug_ranges_sec = None,
+            debug_line_sec = None,
+            debug_pubtypes_sec = None,
+            debug_pubnames_sec = None,
+            debug_addr_sec=None,
+            debug_str_offsets_sec=None,
+            debug_line_str_sec=None,
+            debug_loclists_sec = None,
+            debug_rnglists_sec = None,
+            debug_sup_sec = None,
+            gnu_debugaltlink_sec = None
+        )
+        di._start_address = 0
+        di._format = 1
+
+        self.load_dwarfinfo(di, "", "ARM64")
+
     # Doesn't quite work for the delay on tree expansion :( TODO: timer checks before lighting up this
     def start_wait(self):
         QApplication.setOverrideCursor(Qt.CursorShape.WaitCursor)
 
     def end_wait(self):
         QApplication.restoreOverrideCursor()
```

### Comparing `dwex-3.23/dwex/crash.py` & `dwex-3.24/dwex/crash.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/details.py` & `dwex-3.24/dwex/details.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/die.py` & `dwex-3.24/dwex/die.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,25 +208,28 @@
                         return ' '.join("%02x" % b for b in val[0:MAX_INLINE_BYTEARRAY_LEN]) + ("...(%s bytes)" % (('0x%x' if self.hex else '%d') % len(val)))
                     else:
                         return ' '.join("%02x" % b for b in val)
                 else: # List of something else
                     return str(val)
             else:
                 return hex(val) if self.hex and isinstance(val, int) else str(val)
+        # except BaseException as exc:
         except ELFParseError as exc:
             from .__main__ import version
             from .crash import report_crash
             from inspect import currentframe
             tb = exc.__traceback__
             di = die.cu.dwarfinfo
+            file_addr_size = di.config.default_address_size
             loc_section = di.debug_loclists_sec if dwarf_version >= 5 else di.debug_loc_sec
             loc_sec_len = len(loc_section.stream.getbuffer()) if loc_section else None
             ctxt = {'attr': attr,
                        'die': die,
                        'cu_header': header,
+                       'file_addr_size': file_addr_size,
                        'dwarf_version': dwarf_version,
                        'sec_size': loc_sec_len}
             report_crash(exc, tb, version, currentframe(), ctxt)
             return "(parse error - please report at github.com/sevaa/dwex)"
 
     def format_form(self, form):
         return form if self.prefix or not str(form).startswith('DW_FORM_') else form[8:]
```

### Comparing `dwex-3.23/dwex/dwarfone.py` & `dwex-3.24/dwex/dwarfone.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,24 +251,23 @@
 
         return parsed
 
 class DWARFInfoV1(object):
     def __init__(self, elffile):
         section = elffile.get_section_by_name(".debug")
         section_data = section.data()
+        # TODO: relocation? Compression?
         self.section_size = len(section_data)
-        self.stm = BytesIO()
-        self.stm.write(section_data)
-        self.stm.seek(0, 0)
+        self.stm = BytesIO(section_data)
 
         lsection = elffile.get_section_by_name(".line")
         if lsection:
-            self.linestream = BytesIO()
-            self.linestream.write(lsection.data())
-            self.linestream.seek(0, 0)
+            self.linestream = BytesIO(lsection.data())
+        # Sections .debug_pubnames, .debug_aranges also in the spec -
+        # those are indices into info, we ignore them
 
         self.config = DwarfConfig(
             little_endian = elffile.little_endian,
             default_address_size = elffile.elfclass // 8,
             machine_arch = elffile.get_machine_arch()
         )
```

### Comparing `dwex-3.23/dwex/dwarfutil.py` & `dwex-3.24/dwex/dwarfutil.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/exprutil.py` & `dwex-3.24/dwex/exprutil.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/formats.py` & `dwex-3.24/dwex/formats.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/locals.py` & `dwex-3.24/dwex/locals.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/locs.py` & `dwex-3.24/dwex/locs.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/patch.py` & `dwex-3.24/dwex/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 from elftools.dwarf.descriptions import _DESCR_DW_CC
 from elftools.dwarf.dwarfinfo import DebugSectionDescriptor
 from elftools.elf.relocation import RelocationHandler
 from elftools.dwarf.locationlists import LocationLists, LocationListsPair
 from types import MethodType
 from io import BytesIO
 
+# Good reference on DWARF extensions here:
+# https://sourceware.org/elfutils/DwarfExtensions
+
+# ELF reference:
+# https://refspecs.linuxfoundation.org/elf/gabi4+/ch4.sheader.html
+
 def monkeypatch():
     #https://docs.hdoc.io/hdoc/llvm-project/e051F173385B23DEF.html
     elftools.dwarf.enums.ENUM_DW_AT["DW_AT_LLVM_apinotes"] = 0x3e07
     elftools.dwarf.enums.ENUM_DW_AT["DW_AT_APPLE_objc_direct"] = 0x3fee
     elftools.dwarf.enums.ENUM_DW_AT["DW_AT_APPLE_sdk"] = 0x3fef
 
     # Wasmloc: monkeypatch for #1589
```

### Comparing `dwex-3.23/dwex/ranges.py` & `dwex-3.24/dwex/ranges.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/scriptdlg.py` & `dwex-3.24/dwex/scriptdlg.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         from sys import version_info
         QDialog.__init__(self, win, Qt.WindowType.Dialog)
         self.sample_die = sample_die
         ly = QVBoxLayout()
         ly.addWidget(QLabel("Provide a Python %d.%d expression for the \"die\" object:" % (version_info.major, version_info.minor), self))
         self.text = QPlainTextEdit(self)
         ly.addWidget(self.text)
-        l = QLabel("<a href=\"https://github.com/sevaa/dwex/blob/master/docs/expressions.md\">See the guide</a>", self)
+        l = QLabel("<a href=\"https://github.com/sevaa/dwex/wiki/About-expressions\">See the guide</a>", self)
         l.linkActivated.connect(self.on_see_guide)
         ly.addWidget(l)
         buttons = QDialogButtonBox(QDialogButtonBox.StandardButton.Ok|QDialogButtonBox.StandardButton.Cancel, Qt.Orientation.Horizontal, self)
         buttons.accepted.connect(self.accept)
         buttons.rejected.connect(self.reject)
         ly.addWidget(buttons)
         self.setWindowTitle('Condition')
```

### Comparing `dwex-3.23/dwex/tree.py` & `dwex-3.24/dwex/tree.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/dwex/ui.py` & `dwex-3.24/dwex/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from PyQt6.QtCore import Qt, QRectF, QSizeF, QPointF, QByteArray
 from PyQt6.QtGui import QKeySequence, QAction, QImage, QPixmap, QPainter, QIcon
 from PyQt6.QtWidgets import *
 from PyQt6.QtSvg import QSvgRenderer
 
 def setup_menu(win):
     menu = win.menuBar()
@@ -17,14 +18,16 @@
         win.populate_mru_menu()
     else:
         win.mru_menu.setEnabled(False)
     exit_menuitem = file_menu.addAction("E&xit")
     exit_menuitem.setMenuRole(QAction.MenuRole.QuitRole)
     exit_menuitem.setShortcut(QKeySequence.StandardKey.Quit)
     exit_menuitem.triggered.connect(win.on_exit)
+    if os.environ.get("DWEX_DEBUG") is not None:
+        file_menu.addAction("Debug").triggered.connect(win.on_debug)
     #########
     view_menu = menu.addMenu("View")
     win.prefix_menuitem = view_menu.addAction("DWARF prefix")
     win.prefix_menuitem.setCheckable(True)
     win.prefix_menuitem.setChecked(win.prefix)
     win.prefix_menuitem.triggered.connect(win.on_view_prefix)
     win.lowlevel_menuitem = view_menu.addAction("Low level")
```

### Comparing `dwex-3.23/dwex.egg-info/PKG-INFO` & `dwex-3.24/dwex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwex
-Version: 3.23
+Version: 3.24
 Summary: GUI viewer for DWARF debug information
 Home-page: https://github.com/sevaa/dwex/
 Author: Seva Alekseyev
 Author-email: sevaa@sprynet.com
 License: BSD
 Keywords: dwarf,debug,debugging,symbols,viewer,view,browser,browse,tree
 Platform: any
```

### Comparing `dwex-3.23/setup.py` & `dwex-3.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     with open(path.join(path.abspath(path.dirname(__file__)), 'README.md')) as f:
         long_desc = f.read()          
 except:
     long_desc = "GUI viewer for DWARF debug information"
 
 setup(
     name='dwex',
-    version='3.23',  # Sync with version in __main__
+    version='3.24',  # Sync with version in __main__
     packages=['dwex'],
     url="https://github.com/sevaa/dwex/",
     entry_points={"gui_scripts": ["dwex = dwex.__main__:main"]},
     cmdclass={'install': my_install},
     keywords = ['dwarf', 'debug', 'debugging', 'symbols', 'viewer', 'view', 'browser', 'browse', 'tree'],
     license="BSD",
     author="Seva Alekseyev",
```

### Comparing `dwex-3.23/test/testall.py` & `dwex-3.24/test/testall.py`

 * *Files identical despite different names*

### Comparing `dwex-3.23/test/testlocal.py` & `dwex-3.24/test/testlocal.py`

 * *Files identical despite different names*

