# Comparing `tmp/seguid-0.0.6.tar.gz` & `tmp/seguid-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seguid-0.0.6.tar", max compression
+gzip compressed data, was "seguid-0.1.0a1.tar", max compression
```

## Comparing `seguid-0.0.6.tar` & `seguid-0.1.0a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1092 2024-04-05 16:04:17.488066 seguid-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1585 2024-04-05 16:04:17.492066 seguid-0.0.6/README.md
--rw-r--r--   0        0        0      683 2024-04-05 16:04:17.492066 seguid-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      649 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/__init__.py
--rw-r--r--   0        0        0     2203 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/__main__.py
--rw-r--r--   0        0        0     3373 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/_asserts.py
--rw-r--r--   0        0        0     3503 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/_manip.py
--rw-r--r--   0        0        0     1398 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/_tables.py
--rw-r--r--   0        0        0     8455 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/chksum.py
--rw-r--r--   0        0        0      765 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/config.py
--rw-r--r--   0        0        0     3001 2024-04-05 16:04:17.492066 seguid-0.0.6/src/seguid/reprutils.py
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 seguid-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-17 17:32:00.313892 seguid-0.1.0a1/LICENSE.txt
+-rw-r--r--   0        0        0     1593 2024-04-17 17:32:00.313892 seguid-0.1.0a1/README.md
+-rw-r--r--   0        0        0      952 2024-04-17 17:32:00.313892 seguid-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      697 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/__init__.py
+-rw-r--r--   0        0        0     2209 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/__main__.py
+-rw-r--r--   0        0        0     3370 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_asserts.py
+-rw-r--r--   0        0        0     9473 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_chksum.py
+-rw-r--r--   0        0        0      765 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_config.py
+-rw-r--r--   0        0        0     3504 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_manip.py
+-rw-r--r--   0        0        0     3001 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_reprutils.py
+-rw-r--r--   0        0        0     1398 2024-04-17 17:32:00.313892 seguid-0.1.0a1/src/seguid/_tables.py
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 seguid-0.1.0a1/PKG-INFO
```

### Comparing `seguid-0.0.6/LICENSE.txt` & `seguid-0.1.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seguid-0.0.6/README.md` & `seguid-0.1.0a1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Python checks](https://github.com/seguid/seguid-python/actions/workflows/check-python.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/check-python.yml)
-[![CLI checks](https://github.com/seguid/seguid-python/actions/workflows/check-cli.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/check-cli.yml)
+[![seguid-tests](https://github.com/seguid/seguid-python/actions/workflows/seguid-tests.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/seguid-tests.yml)
 [![Python Code Coverage](https://codecov.io/gh/seguid/seguid-python/graph/badge.svg)](https://codecov.io/gh/seguid/seguid-python)
 [![Documentation Status](https://github.com/seguid/seguid-python/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/publish-docs.yml)
 
 
 # SEGUID v2: Checksums for Linear, Circular, Single- and Double-Stranded Biological Sequences
 
 This Python package, **seguid**, implements SEGUID v2 together with
```

### Comparing `seguid-0.0.6/pyproject.toml` & `seguid-0.1.0a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "seguid"
-version = "0.0.6"
+version = "0.1.0a01"
 description = "Sequence Globally Unique Identifier (SEGUID) Checksums for Linear, Circular, Single-Stranded and Double-Stranded Biological Sequences"
 authors = [
   "Bjorn Johansson <bjornjobb@gmail.com>",
   "Henrik Bengtsson",
   "Louis Abraham"
 ]
 license = "MIT"
 readme = "README.md"
+documentation = "https://seguid-python.seguid.org"
+homepage = "https://github.com/seguid/seguid-python?tab=readme-ov-file#seguid-v2-checksums-for-linear-circular-single--and-double-stranded-biological-sequences"
+repository = "https://github.com/seguid/seguid-python"
 
 [tool.poetry.dependencies]
 python = ">=3.6, <4.0"
 pydivsufsort = { version = "^0.0.14", optional = true }
 setuptools = [
   {version = "<=69.0.3", python = "<3.8"},
   {version = "<=59.6.0", python = "<3.7"},
 ]
 
 [tool.poetry.extras]
 pydivsufsort =  ["pydivsufsort"]
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `seguid-0.0.6/src/seguid/__init__.py` & `seguid-0.1.0a1/src/seguid/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,14 @@
     except ModuleNotFoundError:
         __version__ = "0.0.0"
     else:
         __version__ = pkg_resources.get_distribution(__package__).version
 else:
     __version__ = _version(__package__)
 
-from seguid.chksum import lsseguid
-from seguid.chksum import csseguid
-from seguid.chksum import ldseguid
-from seguid.chksum import cdseguid
+from seguid._chksum import seguid
+from seguid._chksum import lsseguid
+from seguid._chksum import csseguid
+from seguid._chksum import ldseguid
+from seguid._chksum import cdseguid
 
-__all__ = ["lsseguid", "csseguid", "ldseguid", "cdseguid"]
+__all__ = ["seguid", "lsseguid", "csseguid", "ldseguid", "cdseguid"]
```

### Comparing `seguid-0.0.6/src/seguid/__main__.py` & `seguid-0.1.0a1/src/seguid/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from argparse import ArgumentParser
 from seguid import __version__
 
-from seguid.chksum import seguid
-from seguid.chksum import lsseguid
-from seguid.chksum import csseguid
-from seguid.chksum import ldseguid
-from seguid.chksum import cdseguid
+from seguid._chksum import seguid
+from seguid._chksum import lsseguid
+from seguid._chksum import csseguid
+from seguid._chksum import ldseguid
+from seguid._chksum import cdseguid
 from seguid._manip import reverse
-from seguid.reprutils import parse_sequence_string
+from seguid._reprutils import parse_sequence_string
 
 parser = ArgumentParser(
     prog="python -m seguid",
     description="seguid: Sequence Globally Unique Identifier (SEGUID) Checksums for Linear, Circular, Single-Stranded and Double-Stranded Biological Sequences",
 )
 parser.add_argument("--version", action="store_true", help="Show version")
 parser.add_argument("--alphabet", type=str, nargs="?", help="Type of input sequence")
```

### Comparing `seguid-0.0.6/src/seguid/_asserts.py` & `seguid-0.1.0a1/src/seguid/_asserts.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         return
 
     unknown = set(c for c in seq if c not in (k for k in alphabet))
 
     if unknown:
         missing = " ".join(unknown)
         missing = repr(missing)  ## escape '\n', '\t', ...
-        raise ValueError("Detected symbols " f"{missing} in not in the 'alphabet'")
+        raise ValueError("Detected symbols " f"{missing} not in the 'alphabet'")
 
 
 def assert_alphabet(alphabet: dict):
     assert isinstance(alphabet, dict), "Argument 'alphabet' must be a dict"
     keys = alphabet.keys()
     values = alphabet.values()
     if isinstance(next(iter(values)), str):
```

### Comparing `seguid-0.0.6/src/seguid/_manip.py` & `seguid-0.1.0a1/src/seguid/_manip.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 prev, rep = w, 1
             if len(w) * rep == lens:
                 return old - i
     return 0
 
 
 def rotate_to_min(s: str) -> int:
-    from seguid.config import _min_rotation
+    from seguid._config import _min_rotation
 
     ## Assert upper-case letters are ordered before lower-case letters
     assert _min_rotation("Aa") == 0
 
     amount = _min_rotation(s)
     s = rotate(s, amount=amount)
     return s
```

### Comparing `seguid-0.0.6/src/seguid/_tables.py` & `seguid-0.1.0a1/src/seguid/_tables.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.6/src/seguid/chksum.py` & `seguid-0.1.0a1/src/seguid/_chksum.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 seguid.
 
 The seguid module provides four functions for calculations of SEGUID checksums
-for biological sequences with varying topologies
+for biological sequences with varying topologies:
 
-lsseguid (l)inear   (s)ingle-stranded SEGUID
-csseguid (c)ircular (s)ingle-stranded SEGUID
-ldseguid (l)inear   (d)ouble-stranded SGUID
-cdseguid (c)ircular (d)ouble-stranded SEGUID
+ * lsseguid: (l)inear   (s)ingle-stranded SEGUID
+ * csseguid: (c)ircular (s)ingle-stranded SEGUID
+ * ldseguid: (l)inear   (d)ouble-stranded SEGUID
+ * cdseguid: (c)ircular (d)ouble-stranded SEGUID
 
 Some auxillary functions are also provided.
 
 The functions can be made to work without external dependencies, but
 csseguid and cdseguid are considerably faster with pydivsufsort installed.
 
 """
@@ -62,92 +62,103 @@
         longform = prefix + csum
     if form != "long":
         shortform = csum[:short]
     return " ".join((shortform, longform)).strip()
 
 
 def seguid(seq: str, alphabet: str = "{DNA}", form: str = "long") -> str:
-    """SEGUID checksum for protein or single stranded linear DNA.
+    """SEGUID v1 checksum for linear protein or single-stranded DNA.
 
-    OBSOLETE, use lsseguid instead.
+    'Warning: seguid() (obsolete) is superseded by lsseguid() (recommended).'
 
-    Given a nucleotide or amino-acid sequence `seq`, the function returns
-    a string containing the SEquence Globally Unique IDentifier (SEGUID).
+    Given a nucleotide or amino-acid sequence ``seq`` in uppercase, the function returns
+    a string containing the SEquence Globally Unique IDentifier (SEGUID). The SEGUID is
+    defined as the Base64 encoded SHA1 checksum calculated for the sequence in uppercase
+    with the trailing padding symbol (``=``) removed.
 
-    The optional ´encoding` argument expects a function accepting a
-    byte string an returning another byte string. Several such functions are
-    available from the standard library:
+    The original definition of the SEGUID checksum algorithm (Babnigg & Giometti, 2006)
+    included transformation to uppercase before calculating the checksum.
 
-    https://docs.python.org/3/library/base64.html
+    `seguid()` does *not* coerce the input sequence to upper case. If your input sequence
+    has lower-case symbols, you can use `seq.upper()` to emulate what the original method does.
 
-    The SEGUID is defined as the Base64 encoded sha1 checksum calculated for
-    the sequence in upercase with the trailing "=" character removed. This
-    means that upper or lower case symbols in `seq` do not affect the result.
+    `seguid()` only accepts symbols as specified by the `alphabet` argument.
 
-    The resulting string is not url-safe as the Base64 encoding it potentially
-    produces / and + characters, carrying special meaning in a Uniform Resource
-    Locator (URL). It can also not be used as an identifier or variable name in
-    programming languanges such as Python.
+    Thus, our implementation is more conservative, which has the benefit of
+    lowering the risk of passing the incorrect sequence by mistake.
 
-    This implementation follows the original SEGUID definition by
-    Babnigg et al. 2006. For more information:
+    The resulting checksum string may contain forward slash (``/``) and plus-sign (``+``) symbols.
+    These characters cannot be a part of a Uniform Resource Locator (URL) or a filename on
+    some operating systems. The SEGUID v2 checksum produced by ``lsseguid()`` is similar to the
+    SEGUID v1 checksum by ``seguid()``, but uses the Base64url encoding that do not produce
+    these characters.
 
-    Babnigg, G., & Giometti, C. S. (2006). A database of unique protein
-    sequence identifiers for proteome studies. Proteomics, 6(16), 4514–4522.
-    https://doi.org/10.1002/pmic.200600032
-
-    The checksum is prefixed with "seguid="
+    The checksum is prefixed with ``seguid=``.
 
     Examples
     --------
     >>> seguid("AT")
     'seguid=Ax/RG6hzSrMEEWoCO1IWMGska+4'
+
+    References
+    ----------
+
+    * Babnigg, G., & Giometti, C. S. (2006). A database of unique protein
+      sequence identifiers for proteome studies. Proteomics, 6(16), 4514–4522.
+      https://doi.org/10.1002/pmic.200600032
+
+    * Pereira, Humberto, Paulo César Silva, Wayne M Davis, Louis Abraham, Gyorgy Babnigg,
+      Henrik Bengtsson, and Bjorn Johansson. 2024. “SEGUID v2: Extending SEGUID Checksums
+      for Circular, Linear, Single- and Double-Stranded Biological Sequences.” bioRxiv.
+      https://doi.org/10.1101/2024.02.28.582384.
     """
     return _form(
         seguid_prefix,
         _seguid(seq, alphabet=alphabet, encoding=base64.standard_b64encode),
         form,
     )
 
 
 def lsseguid(seq: str, alphabet: str = "{DNA}", form: str = "long") -> str:
-    """SEGUID checksum for single stranded linear DNA (slSEGUID).
+    """SEGUID checksum for linear single-stranded DNA.
 
-    Identical to the seguid function except for that the '+' and '/' characters
-    of standard Base64 encoding are replaced by '-' and '_', respectively
-    following the standard in RFC 4648 section 5.
+    Identical to the ``seguid()`` function except for that the forward slashes (``/``) and plus signs (``+``)
+    of the standard Base64 encoding are replaced by underscores (``_``) and minus signs (``-``), respectively
+    following the Base64url standard in RFC 4648 section 5.
 
-    The base64.urlsafe_b64encode from the Python standard libary is used.
+    The ``base64.urlsafe_b64encode()`` from the Python standard library is used.
 
-    This checksum is applicable to single stranded linear DNA sequences.
-    Can also be used for protein sequences.
+    This checksum is applicable to linear single-stranded DNA sequences or
+    protein sequences. If protein sequences are analyzed, the alphabet
+    argument should be ``"{protein}"`` or ``"{protein-extended}"``. See _tables
+    module for details.
 
-    The checksum is prefixed with "lsseguid="
+    The checksum is prefixed with ``lsseguid=``.
 
     Examples
     --------
     >>> lsseguid("AT")
     'lsseguid=Ax_RG6hzSrMEEWoCO1IWMGska-4'
     """
     return _form(
         lsseguid_prefix,
         _seguid(seq, alphabet=alphabet, encoding=base64.urlsafe_b64encode),
         form,
     )
 
 
 def csseguid(seq: str, alphabet: str = "{DNA}", form: str = "long") -> str:
-    r"""SEGUID checksum for single stranded circular DNA (csSEGUID).
+    r"""SEGUID checksum for circular single-stranded DNA.
 
-    The csSEGUID is the lsSEGUID checksum calculated for the lexicographically
-    smallest string rotation of a ssDNA sequence.
+    The ``csseguid()`` is the ``lsseguid()`` checksum calculated for the lexicographically
+    smallest string rotation of a sequence.
 
-    Only defined for circular sequences.
+    Only defined for circular single-stranded sequences.
 
-    The checksum is prefixed with "csseguid="
+    The checksum is prefixed with ``csseguid=``.
 
     Examples
     --------
     >>> csseguid("ATTT")
     'csseguid=ot6JPLeAeMmfztW1736Kc6DAqlo'
     >>> lsseguid("ATTT")
     'lsseguid=ot6JPLeAeMmfztW1736Kc6DAqlo'
@@ -164,48 +175,48 @@
         form,
     )
 
 
 def ldseguid(
     watson: str, crick: str, alphabet: str = "{DNA}", form: str = "long"
 ) -> str:
-    r"""SEGUID checksum for double stranded linear DNA (ldSEGUID).
+    r"""SEGUID checksum for linear double-stranded DNA.
 
-    Calculates the ldSEGUID checksum for a dsDNA sequence defined by two
+    Calculates the ``ldseguid()`` checksum for a double-stranded DNA (dsDNA) sequence defined by two
     strings representing the upper (Watson) and the complementary (Crick) DNA strands.
-    Optional ssDNA regions in the ends are indicated by a dash "-" in eather strand.
+    Optional single-stranded DNA regions in the ends are indicated by a dash (``-``) in either strand.
     Watson and Crick strands are always equal in length.
 
     The algorithm first selects the lexicographically smallest of the Watson and Crick strands.
 
-    The two string are joined 5'-3', separated by a semicolon ";" and the lsSEGUID function
+    The two string are joined 5'-3', separated by a semicolon (``;``) and the ``lsseguid()`` function
     is used on the resulting string.
 
     ::
 
-        dsDNA    ldSEGUID
+        dsDNA    SEGUID checksum
 
         -TATGCC  ldseguid=rr65d6AYuP-CdMaVmdw3L9FPt6I
          |||||
         CATACG-
 
         -GCATAC  ldseguid=rr65d6AYuP-CdMaVmdw3L9FPt6I
          |||||
         CCGTAT-
 
-    For the linear dsDNA sequence defined by watson = "-TATGCC", crick ="-GCATAC"
-    (see figures above), The "-GCATAC" strand is selected since lexicographically,
-    "-GCATAC" < "-TATGCC".
+    For the linear dsDNA sequence defined by ``watson="-TATGCC"``, ``crick="-GCATAC"``
+    (see figures above), The ``"-GCATAC"`` strand is selected since lexicographically,
+    ``"-GCATAC"`` < ``"-TATGCC"``.
 
     A string is constructed like so:
     ::
 
         "-GCATAC" + ";" + "-TATGCC"
 
-    The checksum is prefixed with "ldseguid="
+    The checksum is prefixed with ``ldseguid=``.
 
     Examples
     --------
     >>> ldseguid("-TATGCC", "-GCATAC")
     'ldseguid=rr65d6AYuP-CdMaVmdw3L9FPt6I'
     >>> ldseguid("-GCATAC", "-TATGCC")
     'ldseguid=rr65d6AYuP-CdMaVmdw3L9FPt6I'
@@ -231,23 +242,23 @@
         form,
     )
 
 
 def cdseguid(
     watson: str, crick: str, alphabet: str = "{DNA}", form: str = "long"
 ) -> str:
-    """SEGUID checksum for double stranded circular DNA (dcSEGUID).
+    """SEGUID checksum for circular double-stranded DNA.
 
-    The dcSEGUID is the slSEGUID checksum calculated for the lexicographically
-    smallest string rotation of a dsDNA sequence. Only defined for circular
+    The ``cdseguid()`` is the ``lsseguid()`` checksum calculated for the lexicographically
+    smallest string rotation of a double-stranded DNA sequence. Only defined for circular
     sequences.
 
-    The checksum is prefixed with "cdseguid="
+    The checksum is prefixed with ``cdseguid=``.
     """
-    from seguid.config import _min_rotation
+    from seguid._config import _min_rotation
 
     assert watson, "Watson sequence must not be empty"
     assert crick, "Crick sequence must not be empty"
     assert len(watson) == len(crick)
     assert_complementary(watson, crick, alphabet=alphabet)
 
     amount_watson = _min_rotation(watson)
```

### Comparing `seguid-0.0.6/src/seguid/config.py` & `seguid-0.1.0a1/src/seguid/_config.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.6/src/seguid/reprutils.py` & `seguid-0.1.0a1/src/seguid/_reprutils.py`

 * *Files identical despite different names*

### Comparing `seguid-0.0.6/PKG-INFO` & `seguid-0.1.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: seguid
-Version: 0.0.6
+Version: 0.1.0a1
 Summary: Sequence Globally Unique Identifier (SEGUID) Checksums for Linear, Circular, Single-Stranded and Double-Stranded Biological Sequences
+Home-page: https://github.com/seguid/seguid-python?tab=readme-ov-file#seguid-v2-checksums-for-linear-circular-single--and-double-stranded-biological-sequences
 License: MIT
 Author: Bjorn Johansson
 Author-email: bjornjobb@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -15,18 +16,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: pydivsufsort
 Requires-Dist: pydivsufsort (>=0.0.14,<0.0.15) ; extra == "pydivsufsort"
 Requires-Dist: setuptools (<=59.6.0) ; python_version < "3.7"
 Requires-Dist: setuptools (<=69.0.3) ; python_version < "3.8"
+Project-URL: Documentation, https://seguid-python.seguid.org
+Project-URL: Repository, https://github.com/seguid/seguid-python
 Description-Content-Type: text/markdown
 
 [![Python checks](https://github.com/seguid/seguid-python/actions/workflows/check-python.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/check-python.yml)
-[![CLI checks](https://github.com/seguid/seguid-python/actions/workflows/check-cli.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/check-cli.yml)
+[![seguid-tests](https://github.com/seguid/seguid-python/actions/workflows/seguid-tests.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/seguid-tests.yml)
 [![Python Code Coverage](https://codecov.io/gh/seguid/seguid-python/graph/badge.svg)](https://codecov.io/gh/seguid/seguid-python)
 [![Documentation Status](https://github.com/seguid/seguid-python/actions/workflows/publish-docs.yml/badge.svg)](https://github.com/seguid/seguid-python/actions/workflows/publish-docs.yml)
 
 
 # SEGUID v2: Checksums for Linear, Circular, Single- and Double-Stranded Biological Sequences
 
 This Python package, **seguid**, implements SEGUID v2 together with
```

