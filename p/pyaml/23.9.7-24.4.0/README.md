# Comparing `tmp/pyaml-23.9.7.tar.gz` & `tmp/pyaml-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaml-23.9.7.tar", last modified: Fri Sep 29 13:37:30 2023, max compression
+gzip compressed data, was "pyaml-24.4.0.tar", last modified: Wed Apr 17 20:42:55 2024, max compression
```

## Comparing `pyaml-23.9.7.tar` & `pyaml-24.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-09-29 13:37:30.545470 pyaml-23.9.7/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.9.7/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.9.7/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    11255 2023-09-29 13:37:30.545470 pyaml-23.9.7/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    10308 2023-09-29 13:36:01.000000 pyaml-23.9.7/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-09-29 13:37:30.543470 pyaml-23.9.7/pyaml/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    10996 2023-09-29 13:32:12.000000 pyaml-23.9.7/pyaml/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       77 2023-09-09 17:20:36.000000 pyaml-23.9.7/pyaml/__main__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     4202 2023-09-13 04:26:40.000000 pyaml-23.9.7/pyaml/cli.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-09-29 13:37:30.544470 pyaml-23.9.7/pyaml/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.9.7/pyaml/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     5243 2023-09-13 04:45:51.000000 pyaml-23.9.7/pyaml/tests/test_cli.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    21105 2023-09-11 14:34:04.000000 pyaml-23.9.7/pyaml/tests/test_dump.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-09-29 13:37:30.544470 pyaml-23.9.7/pyaml.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    11255 2023-09-29 13:37:30.000000 pyaml-23.9.7/pyaml.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      352 2023-09-29 13:37:30.000000 pyaml-23.9.7/pyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-09-29 13:37:30.000000 pyaml-23.9.7/pyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       46 2023-09-29 13:37:30.000000 pyaml-23.9.7/pyaml.egg-info/entry_points.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-09-29 13:37:30.000000 pyaml-23.9.7/pyaml.egg-info/requires.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-09-29 13:37:30.000000 pyaml-23.9.7/pyaml.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      944 2023-09-29 13:34:57.000000 pyaml-23.9.7/pyproject.toml
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-09-29 13:37:30.545470 pyaml-23.9.7/setup.cfg
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1193 2023-07-06 06:21:28.000000 pyaml-23.9.7/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2024-04-17 20:42:55.818589 pyaml-24.4.0/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-24.4.0/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-24.4.0/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    11422 2024-04-17 20:42:55.818589 pyaml-24.4.0/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    10475 2024-04-17 20:34:35.000000 pyaml-24.4.0/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2024-04-17 20:42:55.816589 pyaml-24.4.0/pyaml/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    11196 2023-12-25 17:40:21.000000 pyaml-24.4.0/pyaml/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      212 2024-04-17 20:41:02.000000 pyaml-24.4.0/pyaml/__main__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     5222 2024-04-17 20:37:55.000000 pyaml-24.4.0/pyaml/cli.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2024-04-17 20:42:55.817589 pyaml-24.4.0/pyaml/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-24.4.0/pyaml/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     7681 2024-04-17 20:32:40.000000 pyaml-24.4.0/pyaml/tests/test_cli.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    21487 2023-12-25 17:35:48.000000 pyaml-24.4.0/pyaml/tests/test_dump.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2024-04-17 20:42:55.817589 pyaml-24.4.0/pyaml.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    11422 2024-04-17 20:42:55.000000 pyaml-24.4.0/pyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      352 2024-04-17 20:42:55.000000 pyaml-24.4.0/pyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2024-04-17 20:42:55.000000 pyaml-24.4.0/pyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       46 2024-04-17 20:42:55.000000 pyaml-24.4.0/pyaml.egg-info/entry_points.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2024-04-17 20:42:55.000000 pyaml-24.4.0/pyaml.egg-info/requires.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2024-04-17 20:42:55.000000 pyaml-24.4.0/pyaml.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      945 2024-04-17 20:41:35.000000 pyaml-24.4.0/pyproject.toml
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2024-04-17 20:42:55.818589 pyaml-24.4.0/setup.cfg
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1193 2023-07-06 06:21:28.000000 pyaml-24.4.0/setup.py
```

### Comparing `pyaml-23.9.7/PKG-INFO` & `pyaml-24.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.9.7
+Version: 24.4.0
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
 Home-page: https://github.com/mk-fg/pretty-yaml
 Author: Mike Kazantsev
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
 Project-URL: Homepage, https://github.com/mk-fg/pretty-yaml
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
@@ -94,15 +94,15 @@
 * Dump "null" values as empty values, if possible, which have the same meaning
   but reduce visual clutter and are easier to edit.
 
 * Dicts, sets, OrderedDicts, defaultdicts, namedtuples, enums, dataclasses, etc
   are represented as their safe YAML-compatible base (like int, list or mapping),
   with mappings key-sorted by default for more diff-friendly output.
 
-* Use shorter and simplier yes/no for booleans.
+* Use shorter and simpler yes/no for booleans.
 
 * List items get indented, as they should be.
 
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
@@ -318,17 +318,20 @@
 ------------
 
 It's a regular Python 3.8+ module/package, published on PyPI (as pyaml_).
 
 Module uses PyYAML_ for processing of the actual YAML files
 and should pull it in as a dependency.
 
-Dependency on unidecode_ module is optional and should only be necessary
-with force_embed=False keyword, and same-id objects or recursion is used
-within serialized data.
+Dependency on unidecode_ module is optional and only be used with
+force_embed=False keyword (defaults to True), and same-id objects
+or recursion within serialized data - i.e. only when generating
+&some_key_id anchors is actually needed.
+If module is unavailable at runtime, anchor ids might be less like their
+keys and maybe not as nice.
 
 Using pip_ is how you generally install it, usually coupled with venv_ usage
 (which will also provide "pip" tool itself)::
 
   % pip install pyaml
 
 Current-git version can be installed like this::
```

### Comparing `pyaml-23.9.7/README.rst` & `pyaml-24.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 * Dump "null" values as empty values, if possible, which have the same meaning
   but reduce visual clutter and are easier to edit.
 
 * Dicts, sets, OrderedDicts, defaultdicts, namedtuples, enums, dataclasses, etc
   are represented as their safe YAML-compatible base (like int, list or mapping),
   with mappings key-sorted by default for more diff-friendly output.
 
-* Use shorter and simplier yes/no for booleans.
+* Use shorter and simpler yes/no for booleans.
 
 * List items get indented, as they should be.
 
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
@@ -293,17 +293,20 @@
 ------------
 
 It's a regular Python 3.8+ module/package, published on PyPI (as pyaml_).
 
 Module uses PyYAML_ for processing of the actual YAML files
 and should pull it in as a dependency.
 
-Dependency on unidecode_ module is optional and should only be necessary
-with force_embed=False keyword, and same-id objects or recursion is used
-within serialized data.
+Dependency on unidecode_ module is optional and only be used with
+force_embed=False keyword (defaults to True), and same-id objects
+or recursion within serialized data - i.e. only when generating
+&some_key_id anchors is actually needed.
+If module is unavailable at runtime, anchor ids might be less like their
+keys and maybe not as nice.
 
 Using pip_ is how you generally install it, usually coupled with venv_ usage
 (which will also provide "pip" tool itself)::
 
   % pip install pyaml
 
 Current-git version can be installed like this::
```

### Comparing `pyaml-23.9.7/pyaml/__init__.py` & `pyaml-24.4.0/pyaml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,30 @@
 			elif sort_dicts is sort_dicts.keys: kws['sort_keys'] = True
 			else: self.pyaml_sort_dicts, kws['sort_keys'] = sort_dicts, False
 		elif sort_dicts is not None: kws['sort_keys'] = sort_dicts # for compatibility
 		return super().__init__(*args, **kws)
 
 	@staticmethod
 	def pyaml_transliterate(s):
-		if not all(ord(c) < 128 for c in s):
-			if not (unidecode := PYAMLDumper.pyaml_anchor_decode):
-				from unidecode import unidecode
+		if unidecode_missing := not all(ord(c) < 128 for c in s):
+			if (unidecode := PYAMLDumper.pyaml_anchor_decode) is None:
+				try: from unidecode import unidecode
+				except ImportError: unidecode = False
 				PYAMLDumper.pyaml_anchor_decode = unidecode
-			s = unidecode(s)
-		return re.sub(r'[^-_a-z0-9]+', '_', s.lower())
+			if unidecode: unidecode_missing, s = None, unidecode(s)
+		return re.sub(r'[^-_a-z0-9]+', '_', s.lower()), unidecode_missing
 
 	def anchor_node(self, node, hints=list()):
 		if node in self.anchors:
 			if self.anchors[node] is None and not self.pyaml_force_embed:
 				if hints:
-					nid = self.pyaml_transliterate('_-_'.join(h.value for h in hints))
+					nid, uc = self.pyaml_transliterate('_-_'.join(h.value for h in hints))
 					if len(nid) > (n := self.pyaml_anchor_len_max - 9) + 9:
 						nid = f'{nid[:n//2]}-_-{nid[-n//2:]}_{self.generate_anchor(node)}'
+					elif uc is True: nid = f'{nid}_{self.generate_anchor(node)}'
 				else: nid = self.generate_anchor(node)
 				self.anchors[node] = nid
 		else:
 			self.anchors[node] = None
 			if isinstance(node, yaml.nodes.SequenceNode):
 				for item in node.value: self.anchor_node(item)
 			elif isinstance(node, yaml.nodes.MappingNode):
```

### Comparing `pyaml-23.9.7/pyaml/cli.py` & `pyaml-24.4.0/pyaml/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,14 +25,29 @@
 			try: os.fdatasync(tmp)
 			except AttributeError: pass # MacOS
 			os.rename(tmp.name, path)
 		finally:
 			try: os.unlink(tmp.name)
 			except FileNotFoundError: pass
 
+def file_line_iter(src, sep='\0\n', bs=128 * 2**10):
+	'Generator for src-file chunks, split by any of the separator chars'
+	buff0 = buff = ''
+	while True:
+		eof = len(buff := src.read(bs)) < bs
+		while buff:
+			for n in sorted(buff.find(c) for c in sep):
+				if n >= 0: break
+			else: buff0 += buff; break
+			chunk, buff = buff[:n], buff[n+1:]
+			buff0, chunk = '', buff0 + chunk
+			yield chunk
+		if eof: break
+	if buff0: yield buff0
+
 
 def main(argv=None, stdin=sys.stdin, stdout=sys.stdout, stderr=sys.stderr):
 	import argparse, textwrap
 	dd = lambda text: re.sub( r' \t+', ' ',
 		textwrap.dedent(text).strip('\n') + '\n' ).replace('\t', '  ')
 	parser = argparse.ArgumentParser(
 		formatter_class=argparse.RawTextHelpFormatter,
@@ -49,42 +64,50 @@
 			to visually separate items in overly long YAML lists/mappings.
 		"long" means both >split-lines in line-length and has >split-count items.
 		Value has N[/M][g] format, with default being something like 40/2.
 			N = min number of same-indent lines in a section to split.
 			M = min count of values in a list/mapping to split.
 			"g" can be added to clump single-line values at the top of such lists/maps.
 		Values examples: 20g, 5/1g, 60/4, g, 10.'''))
+	parser.add_argument('-l', '--lines', action='store_true', help=dd('''
+		Read input as a list of \\0 (ascii null char) or newline-separated
+			json/yaml "lines", common with loggers or other incremental data dumps.
+		Each input entry will be exported as a separate YAML document (after "---").
+		Empty or whitespace-only input entries are skipped without errors.'''))
 	parser.add_argument('-q', '--quiet', action='store_true',
 		help='Disable sanity-check on the output and suppress stderr warnings.')
 	opts = parser.parse_args(sys.argv[1:] if argv is None else argv)
 
 	if opts.replace and not opts.path:
 		parser.error('-r/--replace option can only be used with a file path, not stdin')
 
 	src = open(opts.path) if opts.path else stdin
-	try: data = yaml.safe_load(src)
+	try:
+		data = list( yaml.safe_load_all(src) if not opts.lines else
+			(yaml.safe_load(chunk) for chunk in file_line_iter(src) if chunk.strip()) )
 	finally: src.close()
 
 	pyaml_kwargs = dict()
 	if opts.width: pyaml_kwargs['width'] = opts.width
 	if vspacing := opts.vspacing:
 		if vspacing.endswith('g'):
 			pyaml_kwargs['sort_dicts'] = pyaml.PYAMLSort.oneline_group
 			vspacing = vspacing.strip('g')
 		if vspacing:
 			vspacing, (lines, _, count) = dict(), vspacing.strip().strip('/').partition('/')
 			if lines: vspacing['split_lines'] = int(lines.strip())
 			if count: vspacing['split_count'] = int(count.strip())
 			pyaml_kwargs['vspacing'] = vspacing
 
-	ys = pyaml.dump(data, **pyaml_kwargs)
+	if len(data) > 1: ys = pyaml.dump_all(data, **pyaml_kwargs)
+	else: ys = pyaml.dump(data[0], **pyaml_kwargs) # avoids leading "---"
 
 	if not opts.quiet:
 		try:
-			data_chk = yaml.safe_load(ys)
+			data_chk = list(yaml.safe_load_all(ys))
 			try: data_hash = json.dumps(data, sort_keys=True)
 			except: pass # too complex for checking with json
 			else:
 				if json.dumps(data_chk, sort_keys=True) != data_hash:
 					raise AssertionError('Data from before/after pyaml does not match')
 		except Exception as err:
 			p_err = lambda *a,**kw: print(*a, **kw, file=stderr, flush=True)
```

### Comparing `pyaml-23.9.7/pyaml/tests/test_cli.py` & `pyaml-24.4.0/pyaml/tests/test_cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 		yaml.safe_load(out.getvalue())
 		self.assertGreater(len(out.getvalue()), 150)
 		self.assertEqual(err.getvalue(), '')
 
 		d.update(
 			d=test_const.heartbeat,
 			asd=cs.OrderedDict(b=1, a=2) )
-		ys = pyaml.dump(d)
+		ys, out = pyaml.dump(d), io.StringIO()
 		pyaml.cli.main( argv=list(),
 			stdin=io.StringIO(ys), stdout=out, stderr=err )
 		yaml.safe_load(out.getvalue())
 		self.assertGreater(len(out.getvalue()), 150)
 		self.assertEqual(err.getvalue(), '')
 
 	def test_load_fail(self):
@@ -151,9 +151,68 @@
 					stdin=io.StringIO(), stdout=out, stderr=err )
 			self.assertEqual(out.getvalue(), '')
 			self.assertEqual(err.getvalue(), '')
 			with open(tmp.name, 'r') as tmp_new:
 				tmp_new.seek(0); d_new2 = tmp_new.read()
 			self.assertEqual(d_new, d_new2)
 
+	def test_single_doc(self):
+		d, out, err = data.copy(), io.StringIO(), io.StringIO()
+		ys = yaml.safe_dump(d)
+		pyaml.cli.main( argv=list(),
+			stdin=io.StringIO(ys), stdout=out, stderr=err )
+		self.assertNotIn('---', out.getvalue())
+		pyaml.cli.main( argv=list(),
+			stdin=io.StringIO('---\n' + ys), stdout=out, stderr=err )
+		self.assertNotIn('---', out.getvalue())
+		self.assertEqual(len(list(yaml.safe_load_all(out.getvalue()))), 1)
+
+	def test_multi_doc(self):
+		d, out, err = data.copy(), io.StringIO(), io.StringIO()
+		d1, d2 = d, d.copy(); d2['doc2_val'] = 1234
+		ys = yaml.safe_dump_all([d1, d2])
+		pyaml.cli.main( argv=list(),
+			stdin=io.StringIO(ys), stdout=out, stderr=err )
+		self.assertGreater(len(out.getvalue()), 150)
+		self.assertEqual(err.getvalue(), '')
+		self.assertIn('---', out.getvalue())
+		xd1, xd2 = yaml.safe_load_all(out.getvalue())
+		self.assertNotIn('doc2_val', xd1)
+		self.assertEqual(xd2.get('doc2_val'), d2['doc2_val'])
+
+	def test_lines(self):
+		d, out, err = data.copy(), io.StringIO(), io.StringIO()
+		d1, d2, d3 = d, d.copy(), d.copy()
+		d2['doc2_val'], d3['doc3_val'] = 1234, 5678
+		ys = '\n\n   \n \0' + json.dumps(d1)
+		ys += '\0\n   \n\0\0\0\n' + json.dumps(d2)
+		ys += '\n\0' + json.dumps(d3) + '\n \n\0  \t\0\n'
+		ys += '\n' + json.dumps(d3)
+		ys += '\0' + json.dumps(d3)
+		pyaml.cli.main( argv=['-l'],
+			stdin=io.StringIO(ys), stdout=out, stderr=err )
+		with self.assertRaises(yaml.YAMLError):
+			pyaml.cli.main( argv=list(),
+				stdin=io.StringIO(ys), stdout=out, stderr=err )
+		self.assertGreater(len(out.getvalue()), 150)
+		self.assertEqual(err.getvalue(), '')
+		self.assertIn('---', out.getvalue())
+
+		xd1, xd2, xd3, xd3a, xd3b = yaml.safe_load_all(out.getvalue())
+		self.assertNotIn('doc2_val', xd1)
+		self.assertNotIn('doc3_val', xd1)
+		self.assertEqual(xd2.get('doc2_val'), d2['doc2_val'])
+		self.assertNotIn('doc3_val', xd2)
+		self.assertEqual(xd3.get('doc3_val'), d3['doc3_val'])
+		self.assertNotIn('doc2_val', xd3)
+		self.assertEqual(xd3a.get('doc3_val'), d3['doc3_val'])
+		self.assertEqual(xd3b.get('doc3_val'), d3['doc3_val'])
+
+		out, ys = io.StringIO(), '\n\0' + json.dumps(d3) + '\n \n\0\t\0\n'
+		pyaml.cli.main( argv=['--lines'],
+			stdin=io.StringIO(ys), stdout=out, stderr=err )
+		xd3, = yaml.safe_load_all(out.getvalue())
+		self.assertEqual(xd3.get('doc3_val'), d3['doc3_val'])
+		self.assertNotIn('doc2_val', xd3)
+		self.assertNotIn('---', out.getvalue())
 
 if __name__ == '__main__': unittest.main()
```

### Comparing `pyaml-23.9.7/pyaml/tests/test_dump.py` & `pyaml-24.4.0/pyaml/tests/test_dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import yaml
 
 try: import pyaml
 except ImportError:
 	sys.path.insert(1, os.path.join(__file__, *['..']*3))
 	import pyaml
 
+try: import unidecode
+except ImportError: unidecode = None
+
 
 large_yaml = br'''
 ### Default (baseline) configuration parameters.
 ### DO NOT ever change this config, use -c commandline option instead!
 
 # Note that this file is YAML, so YAML types can be used here, see http://yaml.org/type/
 # For instance, large number can be specified as "10_000_000" or "!!float 10e6".
@@ -268,15 +271,24 @@
 		b = pyaml.dump(data, vspacing=False)
 		self.assertNotIn('\n\n', b)
 
 	def test_ids(self):
 		b = pyaml.dump(data, force_embed=False)
 		self.assertNotIn('&id00', b)
 		self.assertIn('query_dump_clone: *query_dump_clone', b)
-		self.assertIn("id в уникоде: &ids_-_id2_v_unikode", b) # kinda bug - should be just "id"
+		self.assertIn('id в уникоде: &ids_-_id2_', b)
+		if not unidecode: self.assertIn('id в уникоде: &ids_-_id2__id00', b)
+
+	def test_ids_unidecode(self):
+		if not unidecode:
+			self.skipTest('No unidecode module to test ids from non-ascii keys')
+		b = pyaml.dump(data, force_embed=False)
+		self.assertNotIn('&id00', b)
+		self.assertNotIn('_id00', b)
+		self.assertIn('id в уникоде: &ids_-_id2_v_unikode', b)
 
 	def test_force_embed(self):
 		for check, fe in (self.assertNotIn, True), (self.assertIn, False):
 			dump = pyaml.dump(data, force_embed=fe)
 			for c in '*&': check(c, dump)
 
 	def test_encoding(self):
@@ -431,15 +443,15 @@
 		self.assertFalse(docs_str2.startswith('---'))
 		self.assertNotEqual(docs_str, docs_str2)
 		docs_str = pyaml.dump(docs, multiple_docs=True, explicit_start=False)
 		self.assertEqual(docs_str, docs_str2)
 
 	def test_ruamel_yaml(self):
 		try: from ruamel.yaml import YAML
-		except ImportError: return unittest.skip('No ruamel.yaml module to test it')
+		except ImportError: self.skipTest('No ruamel.yaml module to test it')
 		data = YAML(typ='safe').load(large_yaml)
 		yaml_str = pyaml.dump(data)
 
 	def test_dump_stream_kws(self):
 		data = [1, 2, 3]
 		buff1, buff2 = io.StringIO(), io.StringIO()
 		pyaml.dump(data, dst=buff1)
```

### Comparing `pyaml-23.9.7/pyaml.egg-info/PKG-INFO` & `pyaml-24.4.0/pyaml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 23.9.7
+Version: 24.4.0
 Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
 Home-page: https://github.com/mk-fg/pretty-yaml
 Author: Mike Kazantsev
 Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
 Project-URL: Homepage, https://github.com/mk-fg/pretty-yaml
 Keywords: yaml,serialization,pretty-print,formatter,human,readability
@@ -94,15 +94,15 @@
 * Dump "null" values as empty values, if possible, which have the same meaning
   but reduce visual clutter and are easier to edit.
 
 * Dicts, sets, OrderedDicts, defaultdicts, namedtuples, enums, dataclasses, etc
   are represented as their safe YAML-compatible base (like int, list or mapping),
   with mappings key-sorted by default for more diff-friendly output.
 
-* Use shorter and simplier yes/no for booleans.
+* Use shorter and simpler yes/no for booleans.
 
 * List items get indented, as they should be.
 
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
@@ -318,17 +318,20 @@
 ------------
 
 It's a regular Python 3.8+ module/package, published on PyPI (as pyaml_).
 
 Module uses PyYAML_ for processing of the actual YAML files
 and should pull it in as a dependency.
 
-Dependency on unidecode_ module is optional and should only be necessary
-with force_embed=False keyword, and same-id objects or recursion is used
-within serialized data.
+Dependency on unidecode_ module is optional and only be used with
+force_embed=False keyword (defaults to True), and same-id objects
+or recursion within serialized data - i.e. only when generating
+&some_key_id anchors is actually needed.
+If module is unavailable at runtime, anchor ids might be less like their
+keys and maybe not as nice.
 
 Using pip_ is how you generally install it, usually coupled with venv_ usage
 (which will also provide "pip" tool itself)::
 
   % pip install pyaml
 
 Current-git version can be installed like this::
```

### Comparing `pyaml-23.9.7/pyproject.toml` & `pyaml-24.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "pyaml"
-version = "23.9.7"
+version = "24.04.0"
 
 description = "PyYAML-based module to produce a bit more pretty and readable YAML-serialized data"
 authors = [{name="Mike Kazantsev", email="mk.fraggod@gmail.com"}]
 license = {text="WTFPL"}
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
```

### Comparing `pyaml-23.9.7/setup.py` & `pyaml-24.4.0/setup.py`

 * *Files identical despite different names*

