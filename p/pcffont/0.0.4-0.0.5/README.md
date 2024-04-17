# Comparing `tmp/pcffont-0.0.4.tar.gz` & `tmp/pcffont-0.0.5.tar.gz`

## Comparing `pcffont-0.0.4.tar` & `pcffont-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.4/requirements.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/artwiz/anorexia.pcf
--rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/artwiz/kates.pcf
--rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/dweep/dweep.pcf
--rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/profont-x11/ProFont_r400-29.pcf
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/raize/raize-normal-19.pcf
--rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/sgi/rock36.pcf
--rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/trisk/trisk.pcf
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/unifont/OFL.txt
--rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/unifont/unifont-15.1.05.pcf
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.4/examples/__init__.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pcffont-0.0.4/examples/create.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pcffont-0.0.4/examples/load.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/error.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/font.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/format.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/header.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/metric.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_accelerators.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_bitmaps.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_encodings.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_glyph_names.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_metrics.py
--rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_properties.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_scalable_widths.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/internal/__init__.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/internal/buffer.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/internal/util.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pcffont-0.0.4/tests/test_dump.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.4/tests/test_example.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pcffont-0.0.4/tests/test_load_save.py
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 pcffont-0.0.4/tests/test_reload.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.4/LICENSE
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 pcffont-0.0.4/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 pcffont-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/artwiz/anorexia.pcf
+-rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/artwiz/kates.pcf
+-rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/dweep/dweep.pcf
+-rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/profont-x11/ProFont_r400-29.pcf
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/raize/raize-normal-19.pcf
+-rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/sgi/rock36.pcf
+-rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/trisk/trisk.pcf
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/unifont/OFL.txt
+-rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.5/assets/unifont/unifont-15.1.05.pcf
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.5/examples/__init__.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pcffont-0.0.5/examples/create.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pcffont-0.0.5/examples/load.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/error.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/font.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/format.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/header.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/metric.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/t_accelerators.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/t_bitmaps.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/t_encodings.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/t_glyph_names.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/t_metrics.py
+-rw-r--r--   0        0        0    11651 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/t_properties.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/t_scalable_widths.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/internal/__init__.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/internal/buffer.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.5/src/pcffont/internal/util.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pcffont-0.0.5/tests/test_dump.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.5/tests/test_example.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pcffont-0.0.5/tests/test_load_save.py
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 pcffont-0.0.5/tests/test_reload.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 pcffont-0.0.5/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 pcffont-0.0.5/PKG-INFO
```

### Comparing `pcffont-0.0.4/.github/workflows/publish.yml` & `pcffont-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/.github/workflows/test.yml` & `pcffont-0.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/artwiz/anorexia.pcf` & `pcffont-0.0.5/assets/artwiz/anorexia.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/artwiz/kates.pcf` & `pcffont-0.0.5/assets/artwiz/kates.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/dweep/dweep.pcf` & `pcffont-0.0.5/assets/dweep/dweep.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/profont-x11/ProFont_r400-29.pcf` & `pcffont-0.0.5/assets/profont-x11/ProFont_r400-29.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/raize/raize-normal-19.pcf` & `pcffont-0.0.5/assets/raize/raize-normal-19.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/sgi/rock36.pcf` & `pcffont-0.0.5/assets/sgi/rock36.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/trisk/trisk.pcf` & `pcffont-0.0.5/assets/trisk/trisk.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/unifont/OFL.txt` & `pcffont-0.0.5/assets/unifont/OFL.txt`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/assets/unifont/unifont-15.1.05.pcf` & `pcffont-0.0.5/assets/unifont/unifont-15.1.05.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/examples/create.py` & `pcffont-0.0.5/examples/create.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/examples/load.py` & `pcffont-0.0.5/examples/load.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/src/pcffont/error.py` & `pcffont-0.0.5/src/pcffont/error.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/src/pcffont/font.py` & `pcffont-0.0.5/src/pcffont/font.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/src/pcffont/format.py` & `pcffont-0.0.5/src/pcffont/format.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/src/pcffont/header.py` & `pcffont-0.0.5/src/pcffont/header.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/src/pcffont/metric.py` & `pcffont-0.0.5/src/pcffont/metric.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pcffont.internal.buffer import Buffer
 
 
 class PcfMetric:
     @staticmethod
     def parse(buffer: Buffer, is_ms_byte: bool, is_compressed: bool) -> 'PcfMetric':
         if is_compressed:
-            left_side_bearing = buffer.read_int8() - 0x80
-            right_side_bearing = buffer.read_int8() - 0x80
-            character_width = buffer.read_int8() - 0x80
-            ascent = buffer.read_int8() - 0x80
-            descent = buffer.read_int8() - 0x80
+            left_side_bearing = buffer.read_uint8() - 0x80
+            right_side_bearing = buffer.read_uint8() - 0x80
+            character_width = buffer.read_uint8() - 0x80
+            ascent = buffer.read_uint8() - 0x80
+            descent = buffer.read_uint8() - 0x80
             attributes = 0
         else:
             left_side_bearing = buffer.read_int16(is_ms_byte)
             right_side_bearing = buffer.read_int16(is_ms_byte)
             character_width = buffer.read_int16(is_ms_byte)
             ascent = buffer.read_int16(is_ms_byte)
             descent = buffer.read_int16(is_ms_byte)
-            attributes = buffer.read_int16(is_ms_byte)
+            attributes = buffer.read_uint16(is_ms_byte)
         return PcfMetric(
             left_side_bearing,
             right_side_bearing,
             character_width,
             ascent,
             descent,
             attributes,
@@ -49,19 +49,19 @@
 
     @property
     def glyph_height(self) -> int:
         return self.ascent + self.descent
 
     def dump(self, buffer: Buffer, is_ms_byte: bool, is_compressed: bool):
         if is_compressed:
-            buffer.write_int8(self.left_side_bearing + 0x80)
-            buffer.write_int8(self.right_side_bearing + 0x80)
-            buffer.write_int8(self.character_width + 0x80)
-            buffer.write_int8(self.ascent + 0x80)
-            buffer.write_int8(self.descent + 0x80)
+            buffer.write_uint8(self.left_side_bearing + 0x80)
+            buffer.write_uint8(self.right_side_bearing + 0x80)
+            buffer.write_uint8(self.character_width + 0x80)
+            buffer.write_uint8(self.ascent + 0x80)
+            buffer.write_uint8(self.descent + 0x80)
         else:
             buffer.write_int16(self.left_side_bearing, is_ms_byte)
             buffer.write_int16(self.right_side_bearing, is_ms_byte)
             buffer.write_int16(self.character_width, is_ms_byte)
             buffer.write_int16(self.ascent, is_ms_byte)
             buffer.write_int16(self.descent, is_ms_byte)
-            buffer.write_int16(self.attributes, is_ms_byte)
+            buffer.write_uint16(self.attributes, is_ms_byte)
```

### Comparing `pcffont-0.0.4/src/pcffont/t_accelerators.py` & `pcffont-0.0.5/src/pcffont/t_accelerators.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/src/pcffont/t_bitmaps.py` & `pcffont-0.0.5/src/pcffont/t_bitmaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
         # FIXME
         bit_scan_mode = PcfTableFormat.bit_scan_mode(table_format)
         if bit_scan_mode != 0:
             raise PcfError(f'Table format not supported: {table_format:b}')
 
         glyphs_count = buffer.read_int32(is_ms_byte)
-        bitmap_offsets = [buffer.read_int32(is_ms_byte) for _ in range(glyphs_count)]
-        size_configs = [buffer.read_int32(is_ms_byte) for _ in range(4)]
+        bitmap_offsets = [buffer.read_uint32(is_ms_byte) for _ in range(glyphs_count)]
+        size_configs = [buffer.read_uint32(is_ms_byte) for _ in range(4)]
         bitmaps_start = buffer.tell()
         bitmaps_size = size_configs[bitmap_pad_mode]
 
         bitmaps = PcfBitmaps(table_format)
         for i in range(glyphs_count):
             bitmap_offset = bitmap_offsets[i]
             if i < glyphs_count - 1:
@@ -107,15 +107,15 @@
                 unit_size_config * 4,
                 unit_size_config * 8,
             ]
 
         buffer.seek(table_offset)
         buffer.write_int32(self.table_format)
         buffer.write_int32(glyphs_count, is_ms_byte)
-        for offset in bitmap_offsets:
-            buffer.write_int32(offset, is_ms_byte)
+        for bitmap_offset in bitmap_offsets:
+            buffer.write_uint32(bitmap_offset, is_ms_byte)
         for size_config in size_configs:
-            buffer.write_int32(size_config, is_ms_byte)
+            buffer.write_uint32(size_config, is_ms_byte)
         buffer.skip(bitmaps_size)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.4/src/pcffont/t_encodings.py` & `pcffont-0.0.5/src/pcffont/t_encodings.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     """
 
     @staticmethod
     def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfBdfEncodings':
         table_format = PcfTableFormat.read_and_check(buffer, header)
         is_ms_byte = PcfTableFormat.is_ms_byte(table_format)
 
-        min_byte_2 = buffer.read_int16(is_ms_byte)
-        max_byte_2 = buffer.read_int16(is_ms_byte)
-        min_byte_1 = buffer.read_int16(is_ms_byte)
-        max_byte_1 = buffer.read_int16(is_ms_byte)
-        default_char = buffer.read_int16(is_ms_byte)
+        min_byte_2 = buffer.read_uint16(is_ms_byte)
+        max_byte_2 = buffer.read_uint16(is_ms_byte)
+        min_byte_1 = buffer.read_uint16(is_ms_byte)
+        max_byte_1 = buffer.read_uint16(is_ms_byte)
+        default_char = buffer.read_uint16(is_ms_byte)
 
         glyphs_count = (max_byte_2 - min_byte_2 + 1) * (max_byte_1 - min_byte_1 + 1)
-        glyph_indices = [buffer.read_int16(is_ms_byte) for _ in range(glyphs_count)]
+        glyph_indices = [buffer.read_uint16(is_ms_byte) for _ in range(glyphs_count)]
 
         encodings = PcfBdfEncodings(table_format, default_char)
         if min_byte_1 == max_byte_1 == 0:
             for code_point in range(min_byte_2, max_byte_2 + 1):
                 glyph_index = glyph_indices[code_point - min_byte_2]
                 encodings[code_point] = glyph_index
         else:
@@ -81,26 +81,26 @@
             if byte_2 < min_byte_2:
                 min_byte_2 = byte_2
             if byte_2 > max_byte_2:
                 max_byte_2 = byte_2
 
         buffer.seek(table_offset)
         buffer.write_int32(self.table_format)
-        buffer.write_int16(min_byte_2, is_ms_byte)
-        buffer.write_int16(max_byte_2, is_ms_byte)
-        buffer.write_int16(min_byte_1, is_ms_byte)
-        buffer.write_int16(max_byte_1, is_ms_byte)
-        buffer.write_int16(self.default_char, is_ms_byte)
+        buffer.write_uint16(min_byte_2, is_ms_byte)
+        buffer.write_uint16(max_byte_2, is_ms_byte)
+        buffer.write_uint16(min_byte_1, is_ms_byte)
+        buffer.write_uint16(max_byte_1, is_ms_byte)
+        buffer.write_uint16(self.default_char, is_ms_byte)
 
         if min_byte_1 == max_byte_1 == 0:
             for code_point in range(min_byte_2, max_byte_2 + 1):
                 glyph_index = self.get(code_point, _NO_GLYPH_INDEX)
-                buffer.write_int16(glyph_index, is_ms_byte)
+                buffer.write_uint16(glyph_index, is_ms_byte)
         else:
             for byte_1 in range(min_byte_1, max_byte_1 + 1):
                 for byte_2 in range(min_byte_2, max_byte_2 + 1):
                     code_point = int.from_bytes(bytes([byte_1, byte_2]))
                     glyph_index = self.get(code_point, _NO_GLYPH_INDEX)
-                    buffer.write_int16(glyph_index, is_ms_byte)
+                    buffer.write_uint16(glyph_index, is_ms_byte)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.4/src/pcffont/t_glyph_names.py` & `pcffont-0.0.5/src/pcffont/t_glyph_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     @staticmethod
     def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfGlyphNames':
         table_format = PcfTableFormat.read_and_check(buffer, header)
         is_ms_byte = PcfTableFormat.is_ms_byte(table_format)
 
         glyphs_count = buffer.read_int32(is_ms_byte)
         name_offsets = [buffer.read_int32(is_ms_byte) for _ in range(glyphs_count)]
-        buffer.skip_int()  # strings_size
+        buffer.skip(4)  # strings_size
         strings_start = buffer.tell()
 
         names = PcfGlyphNames(table_format)
         for name_offset in name_offsets:
             buffer.seek(strings_start + name_offset)
             name = buffer.read_string()
             names.append(name)
```

### Comparing `pcffont-0.0.4/src/pcffont/t_metrics.py` & `pcffont-0.0.5/src/pcffont/t_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     @staticmethod
     def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfMetrics':
         table_format = PcfTableFormat.read_and_check(buffer, header)
         is_ms_byte = PcfTableFormat.is_ms_byte(table_format)
         is_compressed = PcfTableFormat.is_compressed_metrics(table_format)
 
         if is_compressed:
-            glyphs_count = buffer.read_int16(is_ms_byte)
+            glyphs_count = buffer.read_uint16(is_ms_byte)
         else:
             glyphs_count = buffer.read_int32(is_ms_byte)
 
         metrics = PcfMetrics(table_format)
         for _ in range(glyphs_count):
             metric = PcfMetric.parse(buffer, is_ms_byte, is_compressed)
             metrics.append(metric)
@@ -38,15 +38,15 @@
         is_compressed = PcfTableFormat.is_compressed_metrics(self.table_format)
 
         glyphs_count = len(self)
 
         buffer.seek(table_offset)
         buffer.write_int32(self.table_format)
         if is_compressed:
-            buffer.write_int16(glyphs_count, is_ms_byte)
+            buffer.write_uint16(glyphs_count, is_ms_byte)
         else:
             buffer.write_int32(glyphs_count, is_ms_byte)
         for metric in self:
             metric.dump(buffer, is_ms_byte, is_compressed)
 
         table_size = buffer.tell() - table_offset
         return table_size
```

### Comparing `pcffont-0.0.4/src/pcffont/t_properties.py` & `pcffont-0.0.5/src/pcffont/t_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             value = buffer.read_int32(is_ms_byte)
             prop_infos.append((key_offset, is_string_prop, value))
 
         # Pad to next int32 boundary
         padding = 3 - (((4 + 1 + 4) * props_count + 3) % 4)
         buffer.skip(padding)
 
-        buffer.skip_int()  # strings_size
+        buffer.skip(4)  # strings_size
         strings_start = buffer.tell()
 
         properties = PcfProperties(table_format)
         for key_offset, is_string_prop, value in prop_infos:
             buffer.seek(strings_start + key_offset)
             key = buffer.read_string()
             if is_string_prop:
```

### Comparing `pcffont-0.0.4/src/pcffont/t_scalable_widths.py` & `pcffont-0.0.5/src/pcffont/t_scalable_widths.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/src/pcffont/table.py` & `pcffont-0.0.5/src/pcffont/table.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/src/pcffont/internal/buffer.py` & `pcffont-0.0.5/src/pcffont/internal/buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,45 @@
     def __init__(self, stream: BinaryIO):
         self.stream = stream
 
     def read(self, n: int) -> bytes:
         return self.stream.read(n)
 
     def read_int(self, n: int, is_ms_byte: bool = False) -> int:
-        return int.from_bytes(self.read(n), 'big' if is_ms_byte else 'little')
+        return int.from_bytes(
+            self.read(n),
+            byteorder='big' if is_ms_byte else 'little',
+            signed=True,
+        )
 
     def read_int8(self) -> int:
         return self.read_int(1)
 
     def read_int16(self, is_ms_byte: bool = False) -> int:
         return self.read_int(2, is_ms_byte)
 
     def read_int32(self, is_ms_byte: bool = False) -> int:
         return self.read_int(4, is_ms_byte)
 
+    def read_uint(self, n: int, is_ms_byte: bool = False) -> int:
+        return int.from_bytes(
+            self.read(n),
+            byteorder='big' if is_ms_byte else 'little',
+            signed=False,
+        )
+
+    def read_uint8(self) -> int:
+        return self.read_uint(1)
+
+    def read_uint16(self, is_ms_byte: bool = False) -> int:
+        return self.read_uint(2, is_ms_byte)
+
+    def read_uint32(self, is_ms_byte: bool = False) -> int:
+        return self.read_uint(4, is_ms_byte)
+
     def read_bool(self) -> bool:
         return self.read(1) != b'\x00'
 
     def read_string(self) -> str:
         data = bytearray()
         while True:
             b = self.read(1)
@@ -32,40 +52,57 @@
             data.extend(b)
         return data.decode('utf-8')
 
     def write(self, s: bytes) -> int:
         return self.stream.write(s)
 
     def write_int(self, i: int, n: int, is_ms_byte: bool = False) -> int:
-        return self.write(i.to_bytes(n, 'big' if is_ms_byte else 'little'))
+        return self.write(i.to_bytes(
+            n,
+            byteorder='big' if is_ms_byte else 'little',
+            signed=True,
+        ))
 
     def write_int8(self, i: int) -> int:
         return self.write_int(i, 1)
 
     def write_int16(self, i: int, is_ms_byte: bool = False) -> int:
         return self.write_int(i, 2, is_ms_byte)
 
     def write_int32(self, i: int, is_ms_byte: bool = False) -> int:
         return self.write_int(i, 4, is_ms_byte)
 
+    def write_uint(self, i: int, n: int, is_ms_byte: bool = False) -> int:
+        return self.write(i.to_bytes(
+            n,
+            byteorder='big' if is_ms_byte else 'little',
+            signed=False,
+        ))
+
+    def write_uint8(self, i: int) -> int:
+        return self.write_uint(i, 1)
+
+    def write_uint16(self, i: int, is_ms_byte: bool = False) -> int:
+        return self.write_uint(i, 2, is_ms_byte)
+
+    def write_uint32(self, i: int, is_ms_byte: bool = False) -> int:
+        return self.write_uint(i, 4, is_ms_byte)
+
     def write_bool(self, b: bool) -> int:
         return self.write(b'\x01' if b else b'\x00')
 
     def write_nulls(self, n: int) -> int:
         for _ in range(n):
             self.write(b'\x00')
         return n
 
     def write_string(self, s: str) -> int:
         return self.write(s.encode('utf-8')) + self.write_nulls(1)
 
     def skip(self, n: int):
         self.seek(self.tell() + n)
 
-    def skip_int(self):
-        self.skip(4)
-
     def seek(self, offset: int):
         self.stream.seek(offset)
 
     def tell(self) -> int:
         return self.stream.tell()
```

### Comparing `pcffont-0.0.4/src/pcffont/internal/util.py` & `pcffont-0.0.5/src/pcffont/internal/util.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/tests/test_dump.py` & `pcffont-0.0.5/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/tests/test_load_save.py` & `pcffont-0.0.5/tests/test_load_save.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/tests/test_reload.py` & `pcffont-0.0.5/tests/test_reload.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/.gitignore` & `pcffont-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/LICENSE` & `pcffont-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/README.md` & `pcffont-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.4/pyproject.toml` & `pcffont-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcffont"
-version = "0.0.4"
+version = "0.0.5"
 description = "A library for manipulating Portable Compiled Format (PCF) Fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `pcffont-0.0.4/PKG-INFO` & `pcffont-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pcffont
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for manipulating Portable Compiled Format (PCF) Fonts.
 Project-URL: homepage, https://github.com/TakWolf/pcffont
 Project-URL: source, https://github.com/TakWolf/pcffont
 Project-URL: issues, https://github.com/TakWolf/pcffont/issues
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
```

