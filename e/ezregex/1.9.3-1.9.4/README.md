# Comparing `tmp/ezregex-1.9.3.tar.gz` & `tmp/ezregex-1.9.4.tar.gz`

## Comparing `ezregex-1.9.3.tar` & `ezregex-1.9.4.tar`

### file list

```diff
@@ -1,43 +1,50 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.3/.coveragerc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.3/MANIFEST.in
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-1.9.3/requirements.txt
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-1.9.3/setup.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 ezregex-1.9.3/todo.txt
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.3/tox.ini
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.9.3/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0    18421 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/EZRegex.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/_dialects.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/_docs.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/api.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/api.pyi
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/generate.py
--rw-r--r--   0        0        0    24605 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/invert.py
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/invert_old.py
--rw-r--r--   0        0        0  6825598 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/assets/words.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/base/__init__.py
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/base/elements.py
--rw-r--r--   0        0        0    13333 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/base/interface.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/javascript/__init__.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/javascript/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/javascript/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/javascript/psuedonymns.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/perl/__init__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/perl/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/perl/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/perl/psuedonymns.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/python/__init__.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/python/elements.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/python/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.3/ezregex/python/psuedonymns.py
--rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 ezregex-1.9.3/tests/_groups.py
--rw-r--r--   0        0        0    29505 2020-02-02 00:00:00.000000 ezregex-1.9.3/tests/_regexs.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 ezregex-1.9.3/tests/test_generate.py
--rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.3/tests/testing_color_algorithm.ipynb
--rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 ezregex-1.9.3/tests/tests.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.9.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.3/LICENSE
--rw-r--r--   0        0        0    49171 2020-02-02 00:00:00.000000 ezregex-1.9.3/README.md
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 ezregex-1.9.3/pyproject.toml
--rw-r--r--   0        0        0    50085 2020-02-02 00:00:00.000000 ezregex-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.4/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.4/MANIFEST.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-1.9.4/requirements.txt
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-1.9.4/setup.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.4/tox.ini
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.9.4/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/EZRegex.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/_dialects.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/_docs.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/api.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/api.pyi
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/generate.py
+-rw-r--r--   0        0        0    24543 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/invert.py
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/invert_old.py
+-rw-r--r--   0        0        0  4975177 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/assets/sorted_words.json
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/base/__init__.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/base/elements.py
+-rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/base/interface.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/javascript/__init__.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/javascript/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/javascript/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/javascript/psuedonymns.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/perl/__init__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/perl/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/perl/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/perl/psuedonymns.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/python/__init__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/python/elements.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/python/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.4/ezregex/python/psuedonymns.py
+-rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/groups.py
+-rw-r--r--   0        0        0    17584 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/regexs.jsonc
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/replacements.jsonc
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_EZRegex.py
+-rw-r--r--   0        0        0    17019 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_elements.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_generate.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_invert.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_javascript.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_operators.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_python.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/test_replacement.py
+-rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/testing_color_algorithm.ipynb
+-rw-r--r--   0        0        0    15201 2020-02-02 00:00:00.000000 ezregex-1.9.4/tests/tests.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.9.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.4/LICENSE
+-rw-r--r--   0        0        0    52510 2020-02-02 00:00:00.000000 ezregex-1.9.4/README.md
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 ezregex-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0    53450 2020-02-02 00:00:00.000000 ezregex-1.9.4/PKG-INFO
```

### Comparing `ezregex-1.9.3/setup.py` & `ezregex-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/.github/FUNDING.yml` & `ezregex-1.9.4/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/.github/workflows/unit-tests.yml` & `ezregex-1.9.4/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/EZRegex.py` & `ezregex-1.9.4/ezregex/EZRegex.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .api import api
 from .generate import *
 from .invert import invert
 from ._dialects import dialects
 
 # TODO: consider changing addFlags to "outer" or "end" or something
 # TODO: Seriously consider removing the debug functions
+# TODO: in all the magic functions assert that we're not mixing dialects
 
 class EZRegex:
     """ Represent parts of the Regex syntax. Should not be instantiated by the user directly."""
 
     def __init__(self,
                  definition:List[partial[str]]|str|"EZRegex"|partial[str]|list[str],
                  dialect: str,
@@ -31,58 +32,57 @@
         with other EZRegexs and strings. Ideally, this should only be called internally, but it should
         still work from the user's end
         """
 
         if dialect not in dialects.keys():
             raise ValueError(f'Unsupported dialect `{dialect}` given. Supported dialects are: {list(dialects.keys())}')
 
-        self.flags = flags
+        self.__setattr__('flags', flags, True)
         # Parse params
         # Add flags if it's another EZRegex
         if isinstance(definition, EZRegex):
-            self.flags = definition.flags
-            if definition.dialect != dialect:
+            self.__setattr__('flags', definition.flags, True)
+            if definition._dialect != dialect:
                 raise ValueError('Cannot mix regex dialects')
 
         if isinstance(definition, (str, EZRegex)):
             definition = [str(definition)]
         elif not isinstance(definition, (list, tuple)):
             definition = [definition]
 
-        self.sanatize = sanatize
-        self.replacement = replacement
+        self.__setattr__('_sanatize', sanatize, True)
+        self.__setattr__('replacement', replacement, True)
         # This allows strings in the list now, but they get converted later in this function
-        self.funcList: list[str|partial[str]|Callable] = list(definition)
+        # self._funcList: list[str|partial[str]|Callable] = list(definition)
+        self.__setattr__('_funcList', list(definition), True)
         # Just some psuedonymns
-        self.example = self.invert = self.inverse
-        self.dialect = dialect
+        # self.example = self.invert = self.inverse
+        self.__setattr__('_dialect', dialect, True)
         # The dict that has the values
-        self._dialect = dialects[dialect]
+        self.__setattr__('_dialect_attr', dialects[dialect], True)
 
 
         # The init parameter is not actually required, but it will make it more
         # efficient, so we don't have to check that the whole chain is callable
         if init:
             # Go through the chain (most likely of length 1) and parse any strings
             # This is for simplicity when defining all the members
-            for i in range(len(self.funcList)):
-                if isinstance(self.funcList[i], str):
+            for i in range(len(self._funcList)):
+                if isinstance(self._funcList[i], str):
                     # I *hate* how Python handles lambdas
-                    stringBecauseHatred = deepcopy(self.funcList[i])
-                    self.funcList[i] = lambda cur=...: cur + stringBecauseHatred
-                elif not callable(self.funcList[i]) and self.funcList[i] is not None:
-                    raise ValueError(f"Invalid type {type(self.funcList[i])} passed to EZRegex constructor")
-
+                    stringBecauseHatred = deepcopy(self._funcList[i])
+                    self._funcList[i] = lambda cur=...: cur + stringBecauseHatred
+                elif not callable(self._funcList[i]) and self._funcList[i] is not None:
+                    raise ValueError(f"Invalid type {type(self._funcList[i])} passed to EZRegex constructor")
 
     def _escape(self, pattern:str):
         """ This function was modified from the one in /usr/lib64/python3.12/re/__init__.py line 255 """
-        _special_chars_map = {i: '\\' + chr(i) for i in self._dialect['escape_chars']}
+        _special_chars_map = {i: '\\' + chr(i) for i in self._dialect_attr['escape_chars']}
         return pattern.translate(_special_chars_map)
 
-
     def _sanitizeInput(self, i, addFlags=False):
         """ Instead of rasising an error if passed a strange datatype, it now trys to cast it to a string """
         i = deepcopy(i)
 
         # Don't sanatize anything if this is a replacement string
         if self.replacement:
             return str(i)
@@ -108,32 +108,32 @@
                 raise ValueError(f'Incorrect type {type(i)} given to EZRegex parameter: Must be string or another EZRegex chain.')
 
     def __call__(self, *args, **kwargs):
         """ This should be called by the user to specify the specific parameters of this instance i.e. anyof('a', 'b') """
         # If this is being called without parameters, just compile the chain.
         # If it's being called *with* parameters, then it better be a fundemental
         # member, otherwise that doesn't make any sense.
-        if len(self.funcList) > 1:
+        if len(self._funcList) > 1:
             if not len(args) and not len(kwargs):
                 return self._compile()
             else:
                 raise ValueError("You're trying to pass parameters to a chain of expressions. That doesn't make any sense. Stop that.")
 
         # Sanatize the arguments
-        args = list(map(self._sanitizeInput if self.sanatize else deepcopy, args))
+        args = list(map(self._sanitizeInput if self._sanatize else deepcopy, args))
 
         _kwargs = {}
         for key, val in kwargs.items():
-            _kwargs[key] = self._sanitizeInput(val) if self.sanatize else deepcopy(val)
+            _kwargs[key] = self._sanitizeInput(val) if self._sanatize else deepcopy(val)
 
         return EZRegex(
-            [partial(self.funcList[0], *args, **_kwargs)],
-            dialect=self.dialect,
+            [partial(self._funcList[0], *args, **_kwargs)],
+            dialect=self._dialect,
             init=False,
-            sanatize=self.sanatize,
+            sanatize=self._sanatize,
             replacement=self.replacement,
             flags=self.flags
         )
 
     # Magic Functions
     def __str__(self, addFlags=True):
         return self._compile(addFlags)
@@ -142,15 +142,15 @@
         return 'EZRegex("' + self._compile() + '")'
 
     def __eq__(self, thing):
         return self._sanitizeInput(thing, addFlags=True) == self._compile()
 
     def __mul__(self, amt):
         if amt is Ellipsis:
-            return EZRegex(f'(?{self})*', self.dialect, sanatize=False)
+            return EZRegex(f'(?{self})*', self._dialect, sanatize=False)
         rtn = self
         # This isn't optimal, but it's unlikely anyone will use this with large numbers
         for i in range(amt-1):
             # This doesn't work
             # rtn += self
             # But this does??
             rtn = rtn + self
@@ -159,42 +159,42 @@
     def __rmul__(self, amt):
         return self * amt
 
     def __imul__(self, amt):
         return self * amt
 
     def __add__(self, thing):
-        return EZRegex(self.funcList + [partial(lambda cur=...: cur + self._sanitizeInput(thing))],
-            dialect=self.dialect,
+        return EZRegex(self._funcList + [partial(lambda cur=...: cur + self._sanitizeInput(thing))],
+            dialect=self._dialect,
             init=False,
-            sanatize=self.sanatize or thing.sanatize if isinstance(thing, EZRegex) else self.sanatize,
+            sanatize=self._sanatize or thing._sanatize if isinstance(thing, EZRegex) else self._sanatize,
             replacement=self.replacement or thing.replacement if isinstance(thing, EZRegex) else self.replacement,
             flags=(self.flags + thing.flags) if isinstance(thing, EZRegex) else self.flags
         )
 
     def __radd__(self, thing):
-        return EZRegex([partial(lambda cur=...: self._sanitizeInput(thing) + cur)] + self.funcList,
-            dialect=self.dialect,
+        return EZRegex([partial(lambda cur=...: self._sanitizeInput(thing) + cur)] + self._funcList,
+            dialect=self._dialect,
             init=False,
-            sanatize=self.sanatize or thing.sanatize if isinstance(thing, EZRegex) else self.sanatize,
+            sanatize=self._sanatize or thing._sanatize if isinstance(thing, EZRegex) else self._sanatize,
             replacement=self.replacement or thing.replacement if isinstance(thing, EZRegex) else self.replacement,
             flags=(self.flags + thing.flags) if isinstance(thing, EZRegex) else self.flags
         )
 
     def __iadd__(self, thing):
         # return self + self._sanitizeInput(thing)
         return self + thing
 
     def __and__(self, thing):
         warn('The & operator is unstable still. Use each() instead.')
-        return EZRegex(fr'(?={self}){thing}', self.dialect, sanatize=False)
+        return EZRegex(fr'(?={self}){thing}', self._dialect, sanatize=False)
 
     def __rand__(self, thing):
         warn('The & operator is unstable still. Use each() instead.')
-        return EZRegex(fr'(?={thing}){self}', self.dialect, sanatize=False)
+        return EZRegex(fr'(?={thing}){self}', self._dialect, sanatize=False)
 
     # The shift operators just shadow the add operators
     def __lshift__(self, thing):
         return self.__add__(thing)
 
     def __rlshift__(self, thing):
         return self.__radd__(thing)
@@ -216,23 +216,23 @@
         return self.invert()
 
     def __not__(self):
         raise NotImplementedError('The not operator is not implemented. What you probably want is one of anyExcept(), anyCharExcept(), ifNotProceededBy(), or ifNotPreceededBy()')
 
     def __pos__(self):
         comp = self._compile()
-        return EZRegex(('' if not len(comp) else r'(?:' + comp + r')') + r'+', self.dialect, sanatize=False)
+        return EZRegex(('' if not len(comp) else r'(?:' + comp + r')') + r'+', self._dialect, sanatize=False)
 
     def __ror__(self, thing):
         print('ror called')
-        return EZRegex(f'(?:{self._sanitizeInput(thing)}|{self._compile()})', self.dialect, sanatize=False)
+        return EZRegex(f'(?:{self._sanitizeInput(thing)}|{self._compile()})', self._dialect, sanatize=False)
 
     def __or__(self, thing):
         warn('The or operator is unstable and likely to fail, if used more than twice. Use anyof() instead, for now.')
-        return EZRegex(f'(?:{self._compile()}|{self._sanitizeInput(thing)})', self.dialect, sanatize=False)
+        return EZRegex(f'(?:{self._compile()}|{self._sanitizeInput(thing)})', self._dialect, sanatize=False)
 
     def __xor__(self, thing):
         return NotImplemented
 
     def __rxor__(self, thing):
         return NotImplemented
 
@@ -240,15 +240,15 @@
         """ I would prefer __rmod__(), but it doesn't work on strings, since __mod__() is already specified for string formmating. """
         # I don't need to check this, re will do it for me
         # if not isisntance(other, str):
             # raise TypeError(f"Can't search type {type(other)} ")
         return re.search(other, self._compile())
 
     def __hash__(self):
-        if len(self.funcList) > 1:
+        if len(self._funcList) > 1:
             return hash(self._compile())
         # If we only have 1 function lined up, that means we haven't
         # been called at all. And that means we're one of the basic singletons,
         # because users aren't supposed to instantiate this class directly.
         # THAT means we can use this instance's pointer as a unique identifier.
         else:
             return hash(id(self))
@@ -286,60 +286,60 @@
             # assert digit[...:'foo'] == digit[None:'foo'] == digit[,'foo'] ==
             pass
         elif type(args) is not tuple or len(args) == 1:
             if type(args) is tuple:
                 args = args[0]
             if args is None or args is Ellipsis or args == 0:
                 # at_least_0(self)
-                return EZRegex(fr'(?:{self._compile()})*', self.dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()})*', self._dialect, sanatize=False)
             elif args == 1:
                 # at_least_1(self)
-                return EZRegex(fr'(?:{self._compile()})+', self.dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()})+', self._dialect, sanatize=False)
             else:
                 # match_at_least(args, self)
-                return EZRegex(fr'(?:{self._compile()}){{{args},}}', self.dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{{args},}}', self._dialect, sanatize=False)
         else:
             start, end = args
             if start is None or start is Ellipsis:
                 # match_at_most(2, self)
-                return EZRegex(fr'(?:{self._compile()}){{0,{end}}}', self.dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{0,{end}}}', self._dialect, sanatize=False)
             elif end is None or end is Ellipsis:
                 if start == 0:
                     # at_least_0(self)
-                    return EZRegex(fr'(?:{self._compile()})*', self.dialect, sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()})*', self._dialect, sanatize=False)
                 elif start == 1:
                     # at_least_1(self)
-                    return EZRegex(fr'(?:{self._compile()})+', self.dialect, sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()})+', self._dialect, sanatize=False)
                 else:
                     # match_at_least(start, self)
-                    return EZRegex(fr'(?:{self._compile()}){{{start},}}', self.dialect, sanatize=False)
+                    return EZRegex(fr'(?:{self._compile()}){{{start},}}', self._dialect, sanatize=False)
             else:
                 # match_range(start, end, self)
-                return EZRegex(fr'(?:{self._compile()}){{{start},{end}}}', self.dialect, sanatize=False)
+                return EZRegex(fr'(?:{self._compile()}){{{start},{end}}}', self._dialect, sanatize=False)
 
     def __reversed__(self):
         return self.inverse()
 
     def __rich__(self):
         return self._compile()
 
     def __pretty__(self):
         return self._compile()
 
     # Regular functions
     def _compile(self, addFlags=True):
         regex = ''
-        for func in self.funcList:
+        for func in self._funcList:
             regex = func(cur=regex) # type: ignore
 
         # Add the flags
         if addFlags:
-            regex = self._dialect['beginning'] + regex + self._dialect['end']
+            regex = self._dialect_attr['beginning'] + regex + self._dialect_attr['end']
             if len(self.flags):
-                regex = self._dialect['flag_func'](regex, self.flags)
+                regex = self._dialect_attr['flag_func'](regex, self.flags)
         return regex
 
     def compile(self, addFlags=True):
         return re.compile(self._compile(addFlags))
 
     def str(self):
         return self.__str__()
@@ -438,7 +438,25 @@
 
         return bool(len(json['matches']))
 
     def inverse(self, amt=1, **kwargs):
         """ "Inverts" the current Regex expression to give an example of a string it would match.
             Useful for debugging purposes. """
         return '\n'.join([invert(self._compile(), **kwargs) for _ in range(amt)])
+
+    def invert(self, amt=1, **kwargs):
+        return self.inverse(amt, **kwargs)
+
+
+    @property
+    def dialect(self):
+        return self._dialect
+
+    def __setattr__(self, name, value, ignore=False):
+        if ignore:
+            self.__dict__[name] = value
+        else:
+            raise TypeError('EZRegex objects are immutable')
+
+
+    def __delattr__(self, *args):
+        raise TypeError('EZRegex objects are immutable')
```

### Comparing `ezregex-1.9.3/ezregex/_dialects.py` & `ezregex-1.9.4/ezregex/_dialects.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/_docs.py` & `ezregex-1.9.4/ezregex/_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,16 @@
 }
 
 sdocs = ''
 for dialect, spec in docs.items():
     s = ''
     # Iterate through the groups
     for group, elements in spec.items():
-        s += f'<details style="padding-left: 20px;">\n\t<summary>{group.title()}</summary>\n\n'
+        #  style="padding-left: 20px;"
+        s += f'<details>\n\t<summary>{group.title()}</summary>\n\n'
         # Add the group description, if there is one
         if 'description' in elements:
             s += '#### ' + elements.pop('description') + '\n'
 
         # Iterate through the elements within the groups
         for element, about in elements.items():
             signature, description = about
@@ -113,15 +114,15 @@
             s += '\n'
 
             # Add the additional explanation, if there is one
             if description:
                 s += '\t- ' + description + '\n'
         s += '\n</details>\n\n'
 
-    sdocs += f'<details>\n\t<summary>{dialect}</summary>{s}</details>\n'
+    sdocs += f'<details>\n\t<summary><strong><u>{dialect}</u></strong></summary>{s}</details>\n'
 
 # sdocs += '<details>\n\t<summary>Operators</summary>\n\n'
 # for op, desc in operator_docs.items():
 #     sdocs += '- ' + op + '\n\t- ' + desc + '\n'
 
     # Leave this open, cause we have the additional 2 operators manually added in the README
     # (because they're not relevant to ezregex.org)
```

### Comparing `ezregex-1.9.3/ezregex/api.py` & `ezregex-1.9.4/ezregex/api.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/api.pyi` & `ezregex-1.9.4/ezregex/api.pyi`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/generate.py` & `ezregex-1.9.4/ezregex/generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/invert.py` & `ezregex-1.9.4/ezregex/invert.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,38 @@
 else:
     from re import _parser as sre  # type: ignore
 
 # So I can debug this function directly
 if __name__ != '__main__':
     from .invert_old import invertRegex
 
-with open(Path(__file__).parent / 'assets' / 'words.json') as f:
+with open(Path(__file__).parent / 'assets' / 'sorted_words.json') as f:
     words = json.load(f).keys()
 
 # Don't use string.whitespace, because we don't want to use weird difficult to print characters.
 # We want the replacement to be readable.
 _whitespace   = ' '
 _everything   = string.digits + string.ascii_letters + string.punctuation + _whitespace + '_'
 
 def _randWord(length=None, word='lookup'):
+    if length is None:
+        length = randint(3, 9)
+
     if word == 'random':
-        return ''.join(choices(string.ascii_letters + '_', k=length or randint(3, 9)))
+        return ''.join(choices(string.ascii_letters, k=length))
+
     elif word == 'lookup':
-        options = list(filter((lambda i: len(i) > 2 and len(i) < 10) if length is None else (lambda i: len(i) == length), words))
-        if not len(options):
-            _randWord(length, word='random')
-        return choice(options)
+        try:
+            return choice(words[length])
+        except KeyError:
+            return _randWord(length, word='random')
+
     elif word is None:
         return 'word'
+
     else:
         raise ValueError(f"invalid parameter given for word {word}. Accepted values are either random, lookup, or None")
 
 def _randNumber(length:int, random=False) -> str:
     if random:
         return str(randint(0, 10**length))
     else:
```

### Comparing `ezregex-1.9.3/ezregex/invert_old.py` & `ezregex-1.9.4/ezregex/invert_old.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/base/elements.py` & `ezregex-1.9.4/ezregex/base/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/base/interface.py` & `ezregex-1.9.4/ezregex/base/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,22 +292,14 @@
 plain_float: EZRegex
 "Will match 123.45 and 123."
 full_float: EZRegex
 "Will match plain_float as well as things like 1.23e-10 and 1.23e+10"
 int_or_float: EZRegex
 ow: EZRegex
 "\"Optional Whitechunk\""
-email: EZRegex
-"Matches an email"
-version: EZRegex
-"""The *official* regex for matching version numbers from https://semver.org/. It includes 5 groups that can be
-matched/replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata`
-"""
-version_numbered: EZRegex
-"Same as `version`, but it uses numbered groups for each version number instead of named groups"
 
 
 """ Group: Flags
 These shadow python regex flags, and can just as easily be specified directly to the re library instead. They're provided
 here for compatibility with other regex dialects. See https://docs.python.org/3/library/re.html#flags for details
 """
 ASCII: EZRegex
```

### Comparing `ezregex-1.9.3/ezregex/javascript/elements.py` & `ezregex-1.9.4/ezregex/javascript/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/javascript/psuedonymns.py` & `ezregex-1.9.4/ezregex/javascript/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/perl/elements.py` & `ezregex-1.9.4/ezregex/perl/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/perl/psuedonymns.py` & `ezregex-1.9.4/ezregex/perl/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/ezregex/python/psuedonymns.py` & `ezregex-1.9.4/ezregex/python/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/tests/_groups.py` & `ezregex-1.9.4/tests/groups.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/tests/testing_color_algorithm.ipynb` & `ezregex-1.9.4/tests/testing_color_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/tests/tests.py` & `ezregex-1.9.4/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 from ezregex.python import *
 
 try:
     from Cope import debug
 except ImportError:
     pass
 
-from _groups import *
-from _groups import _losers, _winners
-from _regexs import *
-from _regexs import _regexsLine
+# from tests.groups import *
+# from tests.groups import _losers, _winners
+# from _regexs import *
+# from _regexs import _regexsLine
 
 
 def runTests(singletons=True, _invert=True, replacement=True, _generate=True, testMethod=False, internal=False, operators=True, strictness=20, dontIncludePassed=True, invertBackend='re_parser', invert_tries=1):
     global ow
     if singletons:
         print("Testing EZRegex singletons...")
         # Test the various parameters of anyof()
@@ -246,23 +246,23 @@
         # no idea why this doesnt work.
         # assert (anything + word) * 3 == '.\w+' * 3, f"'{(anything + word) * 3}' != '{'.\w+'*3}'"
 
     print('All Tests Passed!')
 
 # From 1-100, 1 is easy, 100 is hard
 difficulty = 1
-runTests(
-    # These should remain on, for the GitHub automated tests
-    singletons=True,
-    _invert=False,
-    replacement=True,
-    operators=True,
-    _generate=True,
-    # These display for you to check that they look correct
-    testMethod=False,
-    _api=False,
-    # Settings
-    strictness=difficulty,
-    invert_tries=101-difficulty,
-    dontIncludePassed=True,
-    invertBackend='re_parser',
-)
+# runTests(
+#     # These should remain on, for the GitHub automated tests
+#     singletons=True,
+#     _invert=False,
+#     replacement=True,
+#     operators=True,
+#     _generate=True,
+#     # These display for you to check that they look correct
+#     testMethod=False,
+#     _api=False,
+#     # Settings
+#     strictness=difficulty,
+#     invert_tries=101-difficulty,
+#     dontIncludePassed=True,
+#     invertBackend='re_parser',
+# )
```

### Comparing `ezregex-1.9.3/.gitignore` & `ezregex-1.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/LICENSE` & `ezregex-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.3/README.md` & `ezregex-1.9.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 <div align="center">
-    <img src="https://ezregex.org/favicon.png"><br>
-    <p></p>
-
-<a href="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml">
-    <img src="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml/badge.svg" alt="Unit Tests">
-</a>
-<a href="https://pypi.org/project/ezregex/">
-    <img src="https://img.shields.io/pypi/v/ezregex.svg" alt="PyPI Latest Release">
-</a>
-<a href="https://choosealicense.com/licenses/mit/">
-    <img src="https://img.shields.io/github/license/smartycope/ezregex">
-</a>
-<a href="https://www.python.org/">
-    <img src="https://img.shields.io/pypi/implementation/ezregex">
-</a>
-<a href="https://pypi.org/project/ezregex/#files">
-    <img src="https://img.shields.io/pypi/format/ezregex">
-</a>
+    <img src="https://ezregex.org/favicon.png">
+    <br>
+    <br>
+    <a href="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml">
+        <img src="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml/badge.svg" alt="Unit Tests">
+    </a>
+    <a href="https://pypi.org/project/ezregex/">
+        <img src="https://img.shields.io/pypi/v/ezregex.svg" alt="PyPI Latest Release">
+    </a>
+    <a href="https://choosealicense.com/licenses/mit/">
+        <img src="https://img.shields.io/github/license/smartycope/ezregex">
+    </a>
+    <!-- <a href="https://www.python.org/">
+        <img src="https://img.shields.io/pypi/implementation/ezregex">
+    </a> -->
+    <!-- <a href="https://pypi.org/project/ezregex/#files">
+        <img src="https://img.shields.io/pypi/format/ezregex">
+    </a> -->
+    <img src="https://img.shields.io/badge/dependencies-0-blue">
+</div>
+<div align="center">
+    <img src="https://img.shields.io/badge/Supported%20Dialects-3-green">
+    <img src="https://img.shields.io/badge/Python%20Dialect-100%25-blue">
+    <img src="https://img.shields.io/badge/JavaScript%20Dialect-50%25-yellow">
+    <img src="https://img.shields.io/badge/Perl%20Dialect-20%25-red">
 </div>
 
+
 # EZRegex
 A readable and intuitive way to make Regular Expressions without having to know any of the syntax
 
-Try my new frontend for this library at [ezregex.org](https://ezregex.org/)!
+Try the frontend for this library at [ezregex.org](https://ezregex.org/)!
 
 TLDR: This is to regular expressions what CMake is to makefiles
 
-**Table of Contents**
+### **Table of Contents**
 * [Usage](#usage)
-* [Installation](#installation)
 * [Invert](#inverting)
 * [Generate](#generation)
 * [Dialects](#dialects)
 * [Documentation](#documentation)
-* [Explanation](#explanation-of-how-it-works)
+* [Developer Docs](#developer-documentation)
+* [Installation](#installation)
 * [Todo](#todo)
 * [License](#license)
 
 ## Usage
 
 Quickstart
 ```python
@@ -46,23 +54,27 @@
 # Matches `foo123abc` and `foo123 abc`
 # but not `abc123foo` or  `foo bar`
 ```
 
 Importing as a named package is recommended
 ```python
 import ezregex as er
+
 # ow is part of er already as optional whitespace
 params = er.group(er.atLeastNone(er.ow + er.word + er.ow + er.optional(',') + er.ow))
+# Seperate parts as variables for cleaner patterns
 function = er.word + er.ow + '(' + params + ')'
+
 # Automatically calls the re.search() function for you
 function % 'some string containing func( param1 , param2)'
+
 # The test() method is helpful for debugging, and color codes groups for you
 function.test('this should match func(param1,\tparam2 ), foo(), and bar( foo,)')
 ```
-.test() will print all the matches, color coded to match and group (not shown here):
+.test() will print all the matches, color coded to match and group (colors not shown here):
 
 ```
 ╭───────────────────────────── Testing Regex ──────────────────────────────╮
 │ Testing expression:                                                      │
 │         \w+(?:\s+)?\(((?:(?:\s+)?\w+(?:\s+)?,?(?:\s+)?)*)\)              │
 │ for matches in:                                                          │
 │         this should match func(param1,  param2 ), foo(), and bar( foo,)  │
@@ -104,85 +116,75 @@
 │         1: "<span style="color: green;"> foo,</span>" (56:61)                                               │
 │                                                                          │
 │                                                                          │
 ╰───────────────────────────────── <span style="color: blue;">Found</span>  ─────────────────────────────────╯
 </pre>
 -->
 
-## Installation
-EZRegex is distributed on [PyPI](https://pypi.org) as a universal
-wheel and is available on Linux, macOS and Windows and supports
-Python 3.10+ and PyPy.
-
-```bash
-$ pip install ezregex
-```
-
-The import name is the same as the package name:
-```python
-import ezregex as er
-```
 
 ## Inverting
-The `invert` function provided (available as er.invert(`expression`), `expression`.invert(), or ~`expression`) is useful for debugging. You pass it an expression, and it returns an example of a string that is guaranteed to match the provided expression.
+The `invert` function (available as er.invert(`expression`), `expression`.invert(), or ~`expression`) is useful for debugging. You pass it an expression, and it returns an example of a string that is guaranteed to match the provided expression.
 
 
 ## Generation
 In version 1.7.0 we introduced a new function: `generate_regex`. It takes in 2 sets of strings, and returns a regular expression that will match everything in the first set and nothing in the second set. It may be a bit crude, but it can be a good starting point if you don't know where to start. It's also really good at [regex golf](http://regex.alf.nu/).
 
 
 ## Dialects
-As of version 1.6.0, the concepts of *dialects* was introduced. Different languages often have slight variations on the regular expression syntax. As this library is meant to be language independent (even though it's written in Python), you should be able to compile regular expressions to work with other languages as well. To do that, you can simply import a sub-package, and they should work identically (though some languages may have more features than others):
+As of version 1.6.0, the concepts of *dialects* was introduced. Different languages often have slight variations on the regular expression syntax. As this library is meant to be language independent (even though it's written in Python), you should be able to compile regular expressions to work with other languages as well. To do that, you can simply import all the elements as a sub-package, and they should work identically, although some languages may not have the same features as others.
 ```python
 >>> import ezregex as er # The python dialect is the defualt dialect
->>> er.group(digit, 'name') + er.earlierGroup('name')
+>>> er.group(digit, 'name') + er.earlier_group('name')
 EZRegex("(?P<name>\d)(?P=name)")
 >>> import ezregex.perl as er
->>> er.group(digit, 'name') + er.earlierGroup('name')
+>>> er.group(digit, 'name') + er.earlier_group('name')
 EZRegex("?P<name>\d)(\g<name>")
 ```
+
 The currently implemented dialects are:
 - Python
     - Well tested, ~99% implemented
+- JavaScript
+    - Under active development, the basics *should* work, though tests aren't in place yet
 - Perl
-    - Almost identical to the Python dialect because I don't know Perl.
-
-If you know a particular flavor of regex and would like to contribute, feel free to make a pull request, or email me at smartycope@gmail.com
+    - Next on the roadmap, technically importable, but not implemented yet
 
+If you know a particular flavor of regex and would like to contribute, feel free to read the [developer documentation](#developer-documentation) and make a pull request! If you would like one that's not implemented yet, you can also add a [github issue](https://github.com/smartycope/ezregex/issues).
 
 ## Documentation
 ### Notes and Gotchas
-This documentation is for the Python dialect specifically, as it really is the only one currently implemented.
-- When using the re library, functions like search() and sub() don't accept EZRegexs as valid regex patterns. Be sure to call either .str() or .compile(), or cast to a string when passing to those. Also, be careful to call the function on the entire pattern: chunk + whitespace.str() is not the same as (chunk + whitespace).str().
-- In regular Regex, a lot of random things capture groups for no reason. I find this annoying. All regexes in EZRegex intentionally capture passively, so to capture any groups, use group(), with the optional `name` parameter.
+- The different Regular Expression dialects don't all have the same features, and those features don't all work the same way. I've tried to standardize these as best I can and use reasonable names for all the elements. If you're confused by something not working as expected, be sure to understand how your language specifically handles regular expressions.
+- When using the Python `re` library, functions like re.search() and re.sub() don't accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast it to a string) or .compile() (to compile to an re.Pattern) when passing to those. Also, be careful to call the function on the entire pattern: chunk + whitespace.str() is not the same as (chunk + whitespace).str().
+- In regular regex, a lot of random things capture groups for no apparent reason. All regexes in EZRegex intentionally capture passively, so to capture any groups, use group(), with the optional `name` parameter.
 - All EZRegexs (except for `raw`) auto-sanitize strings given to them, so there's no need to escape characters or use r strings. This *does* mean, however, that you cannot pass actual regex strings to any of them, as they'll think you're talking about it literally (unless you want that, of course). To include already written regex strings, use `raw`
 - Note that I have camelCase and snake_case versions of each of the functions, because I waver back and forth between which I like better. Both versions function identically.
-- The `input` parameter can accept strings, other EZRegexs, or entire sequences of EZRegex patterns.
-- A few of these have `greedy` and `possessive` optional parameters. They can be useful, but can get complicated. Refer to [the Python re docs](https://docs.python.org/3/library/re.html) for details.
+- The `InputType` can accept strings, other EZRegexs, or entire sequences of EZRegex patterns. It can also accept things that can be cast to a string, but it will warn you when it does, so it's better to cast to a string yourself.
+- The `invert` function can accept any regular expression, not just EZRegex expressions, if you want to use it independently of the rest of the library.
+
 <!-- Start of generated docs -->
 <details>
-	<summary>perl</summary><details style="padding-left: 20px;">
+	<summary><strong><u>perl</u></strong></summary><details>
 	<summary>Positionals</summary>
 
 #### These differentiate the *string* starting with a sequence, and a *line* starting with a sequence. Do note that the startof the string is also the start of a line. These can also be called without parameters to denote the start/end of astring/line without something specific having to be next to it.
 - string_starts_with
 - string_ends_with
 - line_starts_with
 - line_ends_with
 - word_boundary
 	- Matches the boundary of a word, i.e. the empty space between a word character and not a word character, or the end of a string
 - not_word_boundary
 	- The opposite of `wordBoundary`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Literals</summary>
 
-#### 
+####
 - tab
 - space
 - space_or_tab
 - new_line
 - carriage_return
 - quote
 	- Matches ', ", and `
@@ -190,28 +192,28 @@
 - form_feed
 - comma
 - period
 - underscore
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Not Literals</summary>
 
-#### 
+####
 - not_whitespace
 - not_digit
 - not_word
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Catagories</summary>
 
-#### 
+####
 - whitespace
 - whitechunk
 	- A "chunk" of whitespace. Just any amount of whitespace together
 - digit
 - number
 	- Matches multiple digits next to each other. Does not match negatives or decimals
 - word
@@ -232,130 +234,130 @@
 	- Matches a metadata ASCII characters
 - printable
 	- Matches printable ASCII characters
 - printable_and_space
 - alpha_num
 - unicode
 	- Matches a unicode character by name
-- any_between(char: str, and_char: str) 
+- any_between(char: str, and_char: str)
 	- Match any char between `char` and `and_char`, using the ASCII table for reference
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Amounts</summary>
 
-#### 
-- match_max(input: InputType) 
+####
+- match_max(input: InputType)
 	- Match as many of `input` in the string as you can. This is equivelent to using the unary + operator.
 If `input` is not provided, it works on the previous regex pattern. That's not recommended for
 clarity's sake though
-- match_num(num: int, input: InputType) 
+- match_num(num: int, input: InputType)
 	- Match `num` amount of `input` in the string
-- match_more_than(min: int, input: InputType) 
+- match_more_than(min: int, input: InputType)
 	- Match more than `min` sequences of `input` in the string
-- match_at_least(min: int, input: InputType) 
+- match_at_least(min: int, input: InputType)
 	- Match at least `min` sequences of `input` in the string
-- match_at_most(max: int, input: InputType) 
+- match_at_most(max: int, input: InputType)
 	- Match at most `max` instances of `input` in the string
-- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False) 
+- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match between `min` and `max` sequences of `input` in the string. This also accepts `greedy` and `possessive` parameters
 Max can be an empty string to indicate no maximum
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match at least one of `input` in the string. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match 0 or more sequences of `input`. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Choices</summary>
 
-#### 
-- optional(input: InputType, greedy: bool=True, possessive: bool=False) 
+####
+- optional(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match `input` if it's there. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- either(input: InputType, or_input: InputType) 
-- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None) 
+- either(input: InputType, or_input: InputType)
+- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None)
 	- Match any of the given `inputs`. Note that `inputs` can be multiple parameters,
 or a single string. Can also accept parameters chars and split. If char is set
 to True, then `inputs` must only be a single string, it interprets `inputs`
 as characters, and splits it up to find any of the chars in the string. If
 split is set to true, it forces the ?(...) regex syntax instead of the [...]
 syntax. It should act the same way, but your output regex will look different.
 By default, it just optimizes it for you.
-- any_char_except(*inputs: str) 
+- any_char_except(*inputs: str)
 	- This matches any char that is NOT in `inputs`. `inputs` can be multiple parameters, or a single string of chars to split.
-- any_except(input: InputType, type: InputType='.*') 
+- any_except(input: InputType, type: InputType='.*')
 	- Matches anything other than `input`, which must be a single string or EZRegex chain, **not** a list. Also
 optionally accepts the `type` parameter, which works like this: "Match any `type` other than `input`". For example,
 "match any word which is not foo". Do note that this function is new, and I'm still working out the kinks.
-- each(*inputs: InputType) 
+- each(*inputs: InputType)
 	- Matches if the next part of the string can match all of the given inputs. Like the + operator, but out of order.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Conditionals</summary>
 
 #### These can only be used once in a given expression. They only match a given expression if the expression is/ins'tfollowed/preceeded by a the given pattern
-- if_proceded_by(input: InputType) 
+- if_proceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming after it. Can only be used once in a given pattern,
 as it only applies to the end
-- if_not_proceded_by(input: InputType) 
+- if_not_proceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming after it. Can only be used once in
 a given pattern, as it only applies to the end
-- if_preceded_by(input: InputType) 
+- if_preceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming before it. Can only be used once in a given pattern,
 as it only applies to the beginning
-- if_not_preceded_by(input: InputType) 
+- if_not_preceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming before it. Can only be used once
 in a given pattern, as it only applies to the beginning
-- if_enclosed_with(open: str, stuff: InputType, close: str | None=None) 
+- if_enclosed_with(open: str, stuff: InputType, close: str | None=None)
 	- Matches if the string has `open`, then `stuff`, then `close`, but only "matches"
 stuff. Just a convenience combination of ifProceededBy and ifPreceededBy.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Grouping</summary>
 
-#### 
-- group(input: InputType, name: str | None=None) 
+####
+- group(input: InputType, name: str | None=None)
 	- Causes `input` to be captured as an unnamed group. Only useful when replacing regexs
-- passive_group(input: InputType) 
+- passive_group(input: InputType)
 	- As all regexs in EZRegex capture passively, this is entirely useless. But if you really want to, here it is
-- earlier_group(num_or_name: int | str) 
+- earlier_group(num_or_name: int | str)
 	- Matches whatever the group referenced by `num_or_name` matched earlier. Must be *after* a
 group which would match `num_or_name`
-- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None) 
-	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt` 
+- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None)
+	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Replacement</summary>
 
 #### In the intrest of "I don't want to think about any syntax at all", I have included replace members. Do note that theyare not interoperable with the other EZRegexs, and can only be used with other strings and each other.
-- rgroup(num_or_name: str | int) 
+- rgroup(num_or_name: str | int)
 	- Puts in its place the group specified, either by group number (for unnamed
 groups) or group name (for named groups). Named groups are also counted by
 number, I'm pretty sure. Groups are numbered starting from 1
 - replace_entire
 	- Puts in its place the entire match
 - replace(string: str, rtn_str: bool=True) -> str | EZRegex
 	- Generates a valid regex replacement string, using Python f-string like syntax.
@@ -372,30 +374,30 @@
 There's a few of advantages to using this instead of just the regular regex replacement syntax:
 - It's consistent between dialects
 - It's closer to Python f-string syntax, which is cleaner and more familiar
 - It handles numbered, named, and entire replacement types the same
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Misc</summary>
 
-#### 
-- is_exactly(input: InputType) 
+####
+- is_exactly(input: InputType)
 	- This matches the string if and only if the entire string is exactly equal to `input`
-- literal(input: InputType) 
+- literal(input: InputType)
 	- This is a redundant function. You should always be able to use `... + 'stuff'` just as easily as `... + literal('stuff')`
-- raw(regex: str) 
+- raw(regex: str)
 	- If you already have some regular regex written, and you want to incorperate
 it, this will allow you to include it without sanatizing all the backslaches
 and such, which all the other EZRegexs do automatically
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Premade</summary>
 
 #### These are some useful combinations that may be commonly used. They are not as stable, and may be changed and added to inlater versions to make them more accurate
 - literally_anything
 	- *Any* character, include newline
 - signed
 	- a signed number, including 123, -123, and +123
@@ -413,15 +415,15 @@
 - version
 	- The *official* regex for matching version numbers from https://semver.org/. It includes 5 groups that can bematched/replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata`
 - version_numbered
 	- Same as `version`, but it uses numbered groups for each version number instead of named groups
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Flags</summary>
 
 #### These shadow python regex flags, and can just as easily be specified directly to the re library instead. They're providedhere for compatibility with other regex dialects. See https://docs.python.org/3/library/re.html#flags for details
 - ASCII
 	- Make matching words, word boundaries, digits, and whitespace perform ASCII-only matching instead of full Unicodematching. This is only meaningful for Unicode (str) patterns, and is ignored for bytes patterns
 - IGNORECASE
 	- Perform case-insensitive matching, including expressions that explicitly use uppercase members. Full Unicode matching(such as Ü matching ü) also works unless the ASCII flag is used to disable non-ASCII matches. The current locale does notchange the effect of this flag unless the LOCALE flag is also used
@@ -434,33 +436,33 @@
 - UNICODE
 	- Match using the full unicode standard, instead of just ASCII. Enabled by default, and therefore redundant.
 
 </details>
 
 </details>
 <details>
-	<summary>python</summary><details style="padding-left: 20px;">
+	<summary><strong><u>javascript</u></strong></summary><details>
 	<summary>Positionals</summary>
 
 #### These differentiate the *string* starting with a sequence, and a *line* starting with a sequence. Do note that the startof the string is also the start of a line. These can also be called without parameters to denote the start/end of astring/line without something specific having to be next to it.
 - string_starts_with
 - string_ends_with
 - line_starts_with
 - line_ends_with
 - word_boundary
 	- Matches the boundary of a word, i.e. the empty space between a word character and not a word character, or the end of a string
 - not_word_boundary
 	- The opposite of `wordBoundary`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Literals</summary>
 
-#### 
+####
 - tab
 - space
 - space_or_tab
 - new_line
 - carriage_return
 - quote
 	- Matches ', ", and `
@@ -468,28 +470,28 @@
 - form_feed
 - comma
 - period
 - underscore
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Not Literals</summary>
 
-#### 
+####
 - not_whitespace
 - not_digit
 - not_word
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Catagories</summary>
 
-#### 
+####
 - whitespace
 - whitechunk
 	- A "chunk" of whitespace. Just any amount of whitespace together
 - digit
 - number
 	- Matches multiple digits next to each other. Does not match negatives or decimals
 - word
@@ -510,130 +512,130 @@
 	- Matches a metadata ASCII characters
 - printable
 	- Matches printable ASCII characters
 - printable_and_space
 - alpha_num
 - unicode
 	- Matches a unicode character by name
-- any_between(char: str, and_char: str) 
+- any_between(char: str, and_char: str)
 	- Match any char between `char` and `and_char`, using the ASCII table for reference
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Amounts</summary>
 
-#### 
-- match_max(input: InputType) 
+####
+- match_max(input: InputType)
 	- Match as many of `input` in the string as you can. This is equivelent to using the unary + operator.
 If `input` is not provided, it works on the previous regex pattern. That's not recommended for
 clarity's sake though
-- match_num(num: int, input: InputType) 
+- match_num(num: int, input: InputType)
 	- Match `num` amount of `input` in the string
-- match_more_than(min: int, input: InputType) 
+- match_more_than(min: int, input: InputType)
 	- Match more than `min` sequences of `input` in the string
-- match_at_least(min: int, input: InputType) 
+- match_at_least(min: int, input: InputType)
 	- Match at least `min` sequences of `input` in the string
-- match_at_most(max: int, input: InputType) 
+- match_at_most(max: int, input: InputType)
 	- Match at most `max` instances of `input` in the string
-- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False) 
+- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match between `min` and `max` sequences of `input` in the string. This also accepts `greedy` and `possessive` parameters
 Max can be an empty string to indicate no maximum
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match at least one of `input` in the string. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match 0 or more sequences of `input`. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Choices</summary>
 
-#### 
-- optional(input: InputType, greedy: bool=True, possessive: bool=False) 
+####
+- optional(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match `input` if it's there. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- either(input: InputType, or_input: InputType) 
-- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None) 
+- either(input: InputType, or_input: InputType)
+- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None)
 	- Match any of the given `inputs`. Note that `inputs` can be multiple parameters,
 or a single string. Can also accept parameters chars and split. If char is set
 to True, then `inputs` must only be a single string, it interprets `inputs`
 as characters, and splits it up to find any of the chars in the string. If
 split is set to true, it forces the ?(...) regex syntax instead of the [...]
 syntax. It should act the same way, but your output regex will look different.
 By default, it just optimizes it for you.
-- any_char_except(*inputs: str) 
+- any_char_except(*inputs: str)
 	- This matches any char that is NOT in `inputs`. `inputs` can be multiple parameters, or a single string of chars to split.
-- any_except(input: InputType, type: InputType='.*') 
+- any_except(input: InputType, type: InputType='.*')
 	- Matches anything other than `input`, which must be a single string or EZRegex chain, **not** a list. Also
 optionally accepts the `type` parameter, which works like this: "Match any `type` other than `input`". For example,
 "match any word which is not foo". Do note that this function is new, and I'm still working out the kinks.
-- each(*inputs: InputType) 
+- each(*inputs: InputType)
 	- Matches if the next part of the string can match all of the given inputs. Like the + operator, but out of order.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Conditionals</summary>
 
 #### These can only be used once in a given expression. They only match a given expression if the expression is/ins'tfollowed/preceeded by a the given pattern
-- if_proceded_by(input: InputType) 
+- if_proceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming after it. Can only be used once in a given pattern,
 as it only applies to the end
-- if_not_proceded_by(input: InputType) 
+- if_not_proceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming after it. Can only be used once in
 a given pattern, as it only applies to the end
-- if_preceded_by(input: InputType) 
+- if_preceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming before it. Can only be used once in a given pattern,
 as it only applies to the beginning
-- if_not_preceded_by(input: InputType) 
+- if_not_preceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming before it. Can only be used once
 in a given pattern, as it only applies to the beginning
-- if_enclosed_with(open: str, stuff: InputType, close: str | None=None) 
+- if_enclosed_with(open: str, stuff: InputType, close: str | None=None)
 	- Matches if the string has `open`, then `stuff`, then `close`, but only "matches"
 stuff. Just a convenience combination of ifProceededBy and ifPreceededBy.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Grouping</summary>
 
-#### 
-- group(input: InputType, name: str | None=None) 
+####
+- group(input: InputType, name: str | None=None)
 	- Causes `input` to be captured as an unnamed group. Only useful when replacing regexs
-- passive_group(input: InputType) 
+- passive_group(input: InputType)
 	- As all regexs in EZRegex capture passively, this is entirely useless. But if you really want to, here it is
-- earlier_group(num_or_name: int | str) 
+- earlier_group(num_or_name: int | str)
 	- Matches whatever the group referenced by `num_or_name` matched earlier. Must be *after* a
 group which would match `num_or_name`
-- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None) 
-	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt` 
+- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None)
+	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Replacement</summary>
 
 #### In the intrest of "I don't want to think about any syntax at all", I have included replace members. Do note that theyare not interoperable with the other EZRegexs, and can only be used with other strings and each other.
-- rgroup(num_or_name: str | int) 
+- rgroup(num_or_name: str | int)
 	- Puts in its place the group specified, either by group number (for unnamed
 groups) or group name (for named groups). Named groups are also counted by
 number, I'm pretty sure. Groups are numbered starting from 1
 - replace_entire
 	- Puts in its place the entire match
 - replace(string: str, rtn_str: bool=True) -> str | EZRegex
 	- Generates a valid regex replacement string, using Python f-string like syntax.
@@ -650,30 +652,30 @@
 There's a few of advantages to using this instead of just the regular regex replacement syntax:
 - It's consistent between dialects
 - It's closer to Python f-string syntax, which is cleaner and more familiar
 - It handles numbered, named, and entire replacement types the same
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Misc</summary>
 
-#### 
-- is_exactly(input: InputType) 
+####
+- is_exactly(input: InputType)
 	- This matches the string if and only if the entire string is exactly equal to `input`
-- literal(input: InputType) 
+- literal(input: InputType)
 	- This is a redundant function. You should always be able to use `... + 'stuff'` just as easily as `... + literal('stuff')`
-- raw(regex: str) 
+- raw(regex: str)
 	- If you already have some regular regex written, and you want to incorperate
 it, this will allow you to include it without sanatizing all the backslaches
 and such, which all the other EZRegexs do automatically
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Premade</summary>
 
 #### These are some useful combinations that may be commonly used. They are not as stable, and may be changed and added to inlater versions to make them more accurate
 - literally_anything
 	- *Any* character, include newline
 - signed
 	- a signed number, including 123, -123, and +123
@@ -691,52 +693,54 @@
 - version
 	- The *official* regex for matching version numbers from https://semver.org/. It includes 5 groups that can bematched/replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata`
 - version_numbered
 	- Same as `version`, but it uses numbered groups for each version number instead of named groups
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Flags</summary>
 
 #### These shadow python regex flags, and can just as easily be specified directly to the re library instead. They're providedhere for compatibility with other regex dialects. See https://docs.python.org/3/library/re.html#flags for details
 - ASCII
 	- Make matching words, word boundaries, digits, and whitespace perform ASCII-only matching instead of full Unicodematching. This is only meaningful for Unicode (str) patterns, and is ignored for bytes patterns
 - IGNORECASE
 	- Perform case-insensitive matching, including expressions that explicitly use uppercase members. Full Unicode matching(such as Ü matching ü) also works unless the ASCII flag is used to disable non-ASCII matches. The current locale does notchange the effect of this flag unless the LOCALE flag is also used
 - DOTALL
 	- Make the '.' special character match any character at all, including a newline. It's recommended you simply useliterally_anything instead
 - LOCALE
 	- Try not to use this, and rely on unicode matching instead
 - MULTILINE
 	- This is automatically inserted when using line_start and line_end, you shouldn't need to add it manually
+- UNICODE
+	- Match using the full unicode standard, instead of just ASCII. Enabled by default, and therefore redundant.
 
 </details>
 
 </details>
 <details>
-	<summary>javascript</summary><details style="padding-left: 20px;">
+	<summary><strong><u>python</u></strong></summary><details>
 	<summary>Positionals</summary>
 
 #### These differentiate the *string* starting with a sequence, and a *line* starting with a sequence. Do note that the startof the string is also the start of a line. These can also be called without parameters to denote the start/end of astring/line without something specific having to be next to it.
 - string_starts_with
 - string_ends_with
 - line_starts_with
 - line_ends_with
 - word_boundary
 	- Matches the boundary of a word, i.e. the empty space between a word character and not a word character, or the end of a string
 - not_word_boundary
 	- The opposite of `wordBoundary`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Literals</summary>
 
-#### 
+####
 - tab
 - space
 - space_or_tab
 - new_line
 - carriage_return
 - quote
 	- Matches ', ", and `
@@ -744,28 +748,28 @@
 - form_feed
 - comma
 - period
 - underscore
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Not Literals</summary>
 
-#### 
+####
 - not_whitespace
 - not_digit
 - not_word
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Catagories</summary>
 
-#### 
+####
 - whitespace
 - whitechunk
 	- A "chunk" of whitespace. Just any amount of whitespace together
 - digit
 - number
 	- Matches multiple digits next to each other. Does not match negatives or decimals
 - word
@@ -786,130 +790,130 @@
 	- Matches a metadata ASCII characters
 - printable
 	- Matches printable ASCII characters
 - printable_and_space
 - alpha_num
 - unicode
 	- Matches a unicode character by name
-- any_between(char: str, and_char: str) 
+- any_between(char: str, and_char: str)
 	- Match any char between `char` and `and_char`, using the ASCII table for reference
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Amounts</summary>
 
-#### 
-- match_max(input: InputType) 
+####
+- match_max(input: InputType)
 	- Match as many of `input` in the string as you can. This is equivelent to using the unary + operator.
 If `input` is not provided, it works on the previous regex pattern. That's not recommended for
 clarity's sake though
-- match_num(num: int, input: InputType) 
+- match_num(num: int, input: InputType)
 	- Match `num` amount of `input` in the string
-- match_more_than(min: int, input: InputType) 
+- match_more_than(min: int, input: InputType)
 	- Match more than `min` sequences of `input` in the string
-- match_at_least(min: int, input: InputType) 
+- match_at_least(min: int, input: InputType)
 	- Match at least `min` sequences of `input` in the string
-- match_at_most(max: int, input: InputType) 
+- match_at_most(max: int, input: InputType)
 	- Match at most `max` instances of `input` in the string
-- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False) 
+- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match between `min` and `max` sequences of `input` in the string. This also accepts `greedy` and `possessive` parameters
 Max can be an empty string to indicate no maximum
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match at least one of `input` in the string. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match 0 or more sequences of `input`. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Choices</summary>
 
-#### 
-- optional(input: InputType, greedy: bool=True, possessive: bool=False) 
+####
+- optional(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match `input` if it's there. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- either(input: InputType, or_input: InputType) 
-- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None) 
+- either(input: InputType, or_input: InputType)
+- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None)
 	- Match any of the given `inputs`. Note that `inputs` can be multiple parameters,
 or a single string. Can also accept parameters chars and split. If char is set
 to True, then `inputs` must only be a single string, it interprets `inputs`
 as characters, and splits it up to find any of the chars in the string. If
 split is set to true, it forces the ?(...) regex syntax instead of the [...]
 syntax. It should act the same way, but your output regex will look different.
 By default, it just optimizes it for you.
-- any_char_except(*inputs: str) 
+- any_char_except(*inputs: str)
 	- This matches any char that is NOT in `inputs`. `inputs` can be multiple parameters, or a single string of chars to split.
-- any_except(input: InputType, type: InputType='.*') 
+- any_except(input: InputType, type: InputType='.*')
 	- Matches anything other than `input`, which must be a single string or EZRegex chain, **not** a list. Also
 optionally accepts the `type` parameter, which works like this: "Match any `type` other than `input`". For example,
 "match any word which is not foo". Do note that this function is new, and I'm still working out the kinks.
-- each(*inputs: InputType) 
+- each(*inputs: InputType)
 	- Matches if the next part of the string can match all of the given inputs. Like the + operator, but out of order.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Conditionals</summary>
 
 #### These can only be used once in a given expression. They only match a given expression if the expression is/ins'tfollowed/preceeded by a the given pattern
-- if_proceded_by(input: InputType) 
+- if_proceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming after it. Can only be used once in a given pattern,
 as it only applies to the end
-- if_not_proceded_by(input: InputType) 
+- if_not_proceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming after it. Can only be used once in
 a given pattern, as it only applies to the end
-- if_preceded_by(input: InputType) 
+- if_preceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming before it. Can only be used once in a given pattern,
 as it only applies to the beginning
-- if_not_preceded_by(input: InputType) 
+- if_not_preceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming before it. Can only be used once
 in a given pattern, as it only applies to the beginning
-- if_enclosed_with(open: str, stuff: InputType, close: str | None=None) 
+- if_enclosed_with(open: str, stuff: InputType, close: str | None=None)
 	- Matches if the string has `open`, then `stuff`, then `close`, but only "matches"
 stuff. Just a convenience combination of ifProceededBy and ifPreceededBy.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Grouping</summary>
 
-#### 
-- group(input: InputType, name: str | None=None) 
+####
+- group(input: InputType, name: str | None=None)
 	- Causes `input` to be captured as an unnamed group. Only useful when replacing regexs
-- passive_group(input: InputType) 
+- passive_group(input: InputType)
 	- As all regexs in EZRegex capture passively, this is entirely useless. But if you really want to, here it is
-- earlier_group(num_or_name: int | str) 
+- earlier_group(num_or_name: int | str)
 	- Matches whatever the group referenced by `num_or_name` matched earlier. Must be *after* a
 group which would match `num_or_name`
-- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None) 
-	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt` 
+- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None)
+	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Replacement</summary>
 
 #### In the intrest of "I don't want to think about any syntax at all", I have included replace members. Do note that theyare not interoperable with the other EZRegexs, and can only be used with other strings and each other.
-- rgroup(num_or_name: str | int) 
+- rgroup(num_or_name: str | int)
 	- Puts in its place the group specified, either by group number (for unnamed
 groups) or group name (for named groups). Named groups are also counted by
 number, I'm pretty sure. Groups are numbered starting from 1
 - replace_entire
 	- Puts in its place the entire match
 - replace(string: str, rtn_str: bool=True) -> str | EZRegex
 	- Generates a valid regex replacement string, using Python f-string like syntax.
@@ -926,30 +930,30 @@
 There's a few of advantages to using this instead of just the regular regex replacement syntax:
 - It's consistent between dialects
 - It's closer to Python f-string syntax, which is cleaner and more familiar
 - It handles numbered, named, and entire replacement types the same
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Misc</summary>
 
-#### 
-- is_exactly(input: InputType) 
+####
+- is_exactly(input: InputType)
 	- This matches the string if and only if the entire string is exactly equal to `input`
-- literal(input: InputType) 
+- literal(input: InputType)
 	- This is a redundant function. You should always be able to use `... + 'stuff'` just as easily as `... + literal('stuff')`
-- raw(regex: str) 
+- raw(regex: str)
 	- If you already have some regular regex written, and you want to incorperate
 it, this will allow you to include it without sanatizing all the backslaches
 and such, which all the other EZRegexs do automatically
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Premade</summary>
 
 #### These are some useful combinations that may be commonly used. They are not as stable, and may be changed and added to inlater versions to make them more accurate
 - literally_anything
 	- *Any* character, include newline
 - signed
 	- a signed number, including 123, -123, and +123
@@ -967,64 +971,93 @@
 - version
 	- The *official* regex for matching version numbers from https://semver.org/. It includes 5 groups that can bematched/replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata`
 - version_numbered
 	- Same as `version`, but it uses numbered groups for each version number instead of named groups
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Flags</summary>
 
 #### These shadow python regex flags, and can just as easily be specified directly to the re library instead. They're providedhere for compatibility with other regex dialects. See https://docs.python.org/3/library/re.html#flags for details
 - ASCII
 	- Make matching words, word boundaries, digits, and whitespace perform ASCII-only matching instead of full Unicodematching. This is only meaningful for Unicode (str) patterns, and is ignored for bytes patterns
 - IGNORECASE
 	- Perform case-insensitive matching, including expressions that explicitly use uppercase members. Full Unicode matching(such as Ü matching ü) also works unless the ASCII flag is used to disable non-ASCII matches. The current locale does notchange the effect of this flag unless the LOCALE flag is also used
 - DOTALL
 	- Make the '.' special character match any character at all, including a newline. It's recommended you simply useliterally_anything instead
 - LOCALE
 	- Try not to use this, and rely on unicode matching instead
 - MULTILINE
 	- This is automatically inserted when using line_start and line_end, you shouldn't need to add it manually
-- UNICODE
-	- Match using the full unicode standard, instead of just ASCII. Enabled by default, and therefore redundant.
 
 </details>
 
 </details>
 <!-- End of generated docs -->
 <details>
 <summary>Operators</summary>
 
 - `+`, `<<`, `>>`
 	- These all do the same thing: combine expressions
 - `*`
-	- Multiplies an expression a number of times. `expr * 3` is equivelent to `expr + expr + expr`. Can also be used like `expr * ...` is equivalent to `anyAmt(expr)`
+	- Multiplies an expression a number of times. `expr * 3` is equivelent to `expr + expr + expr`. Can also be used like `expr * ...` is equivalent to `any_amt(expr)`
 - `+`
 	- A unary + operator acts exactly as a match_max() does, or, if you're familiar with regex syntax, the + operator
 - `[]`
 	- expr[2, 3] is equivalent to `match_range(2, 3, expr)`
 	- expr[2, ...] or expr[2,] is equivalent to `at_least(2, expr)`
 	- expr[... , 2] is equivalent to `at_most(2, expr)`
 	- expr[...] or expr[0, ...] is equivelent to `at_least_0(expr)`
 	- expr[1, ...] is equivalent to `at_least_1(expr)`
 - `&`
 	- Coming soon! This will work like the + operator, but they can be out of order. Like an and operation.
 - `|`
-	- Coming soon! This will work like an or operation, which will work just like anyOf()
+	- Coming soon! This will work like an or operation, which will work just like any_of()
 - `%`
     - This automatically calls re.search() for you and returns the match object (or None). Use like this: `(digit * 2) % '99 beers on the wall'`
 - `~`
-    - This inverts the expression. This is equivalent to calling the .invert() method
+    - This inverts the expression, equivalent to calling the .invert() method
 </details>
 
-## Explanation of How it Works
-Everything relies on the EZRegex class. In the elements.py file of each dialect, I have defined a ton of pre-made EZRegexs which mimic all (or at least as many as I can) fundamental parts of the regex syntax, plus a few others which are common combinations (like chunk or optional(whitechunk)). Any of them which have parameters are wrapped in functions to provide proper typing & linting. They all are either EZRegexs or are functions which return EZRegexs. These have operators overloaded so you can combine them in intuitive ways and call them by intuitive names. All the functions passed to EZRegex take a function parameter (or a string which gets converted to a function for convenience), which gets called with the current regex expression and any parameters passed along when the instance gets called with the () operator. That way you can add things to the front or back of an expression for example, and you can change what exactly gets added to the current expression based on other parameters. You can also chain strings together, and pass them as parameters to other EZRegexs, which auto-compiles them and adds them appropriately.
+## Developer Documentation
+### The EZRegex class
+Everything relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as each dialect defines their own EZRegex elements specific to that dialect (more on that later). Each element represents a fundamental part of the Regular Expression syntax for that language, as well as less-fundemental common combinations for convenience (like email and float).
+
+EZRegex can accept a string or a function to define how it's supposed to interact with the current "chain" of elements. If it's a string, it just adds it to the end. If it's a function, it can accept any positional or named parameters, but has to accept `cur=...` as the last parameter (it's complicated). The `cur` parameter is the current regular expression chain, as a string. What's returned becomes the new `cur` parameter of the next element, or, if there is no next element, the final regex. That way you can add to the front or back of an expression, and you can change what exactly gets added to the current expression based on other parameters.
+
+The EZRegex class has operators overloaded so you can combine them in intuitive ways and call them by intuitive names.
+
+### Typing & Linting
+The updated method of doing this is to define all the EZRegex elements of a dialect in `elements.py`, and then add type hints and doc strings in the `elements.pyi` file. EZRegex elements that accept parameters are typed as functions (even though they're not), for both convenience for the user when using linter, and to give documentation in an easier way. EZRegex elements that don't accept parameters should be typed as EZRegex, and given documentation as a string on the line below it. This is *slightly* non-standard, but linters support it, as well as my documentation generator script, which parses the .pyi files. The elements can also be seperated into groups in the .pyi files by using `"Group: \<group name\>\n\<group description\>"`, which also gets parsed by the documentation script. The groups aren't used in the actual library, but are helpful in seperating the documentation, as well as used in [ezregex.org](http://ezregex.org)
+
+### Dialects
+Because most regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but it works a bit differently. It has an `elements.py` file, but it defines all the elements as a dict in the form of {"element_name": {"keyword": "arguements"}}. It then has a `load_dialect()` function, which is the only thing importable from it. The reason it's done this way is because `dialect` is a required parameter of the EZRegex constructor, so `load_dialect()` takes a `dialect` parameter, and constructs the base elements from it's dict and returns a new dict of initialized elements to be dumped into the global scope of the dialect. The `elements.py` file of a specific dialect can then remove any elements that it doesn't support (using the `del` keyword) and add/overwrite any it does support.
 
-I also have everything which could capture a group capture it passively, except for actual group operators, and always have the (?m) (multiline) flag automatically asserted whenever lineStart/lineEnd are used so as to differentiate between capturing at the beginning/end of a string and the beginning/end of a line.
+### Inverting
+There's actually 2 algorithms implemented for "inverting" regexs. The old algorithm regexs the regexs in a specific order to replace parts one at a time. This is just as nasty and horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I actually got it to work decently well.
+
+Later, when I was reading up on abstract syntax trees, and scrolling around on PyPi, I realized that Python has one built in, and that it's available to use. I reimplemented the whole algorithm to instead parse the AST given by the built-in re lexer, and wrote my own parser on top of it, which works *much* better.
+
+Along the way, I also discovered, deep in the corners of the internet, 2 other Python libraries which do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger` technically works, however it tends to include unprintable characters, so it's output isn't very readable. `sre_yeild` is better, but it can be very slow, and is not quite the use case I'm going for. My invert algorithm is meant to be a debugging tool (though it doubles well for a testing tool), so it does things like detecting words (as opposed to seperate word characters) and inserts actual words, and doing the same for numbers and inserting `12345...`, as well as a couple other enhancements.
+
+### Tests
+Tests for a while now have just been in a single `tests.py` file, which was a giant pile of all the tests. I'm currently moving to use pytest. There's a `regexs.json` file (and a `replacements.json` file) that have a bunch of regexs, along with things they're supposed to match, and things they're not supposed to match, for testing.
+
+## Installation
+EZRegex is distributed on [PyPI](https://pypi.org) as a universal wheel and is available on Linux, macOS and Windows and supports Python 3.10+ and PyPy.
+
+```bash
+pip install ezregex
+```
+
+The import name is the same as the package name:
+```python
+import ezregex as er
+```
 
 ## Todo
-See [the todo](todo.txt).
-Eventually, I would like to move the todo to GitHub issues.
+See [the todo](todo.txt). I'm slowly moving these to [GitHub issues](https://github.com/smartycope/ezregex/issues), but for now, they're mostly still there
+
 
 ## License
 EZRegex is distributed under the [MIT License](https://choosealicense.com/licenses/mit)
```

#### html2text {}

```diff
@@ -1,123 +1,132 @@
                        [https://ezregex.org/favicon.png]
+
    _[_U_n_i_t_ _T_e_s_t_s_]_[_P_y_P_I_ _L_a_t_e_s_t_ _R_e_l_e_a_s_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/
-_s_m_a_r_t_y_c_o_p_e_/_e_z_r_e_g_e_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_i_m_p_l_e_m_e_n_t_a_t_i_o_n_/_e_z_r_e_g_e_x_]_[_h_t_t_p_s_:_/
-                     _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_f_o_r_m_a_t_/_e_z_r_e_g_e_x_]
+     _s_m_a_r_t_y_c_o_p_e_/_e_z_r_e_g_e_x_][https://img.shields.io/badge/dependencies-0-blue]
+     [https://img.shields.io/badge/Supported%20Dialects-3-green][https://
+  img.shields.io/badge/Python%20Dialect-100%25-blue][https://img.shields.io/
+    badge/JavaScript%20Dialect-50%25-yellow][https://img.shields.io/badge/
+                           Perl%20Dialect-20%25-red]
 # EZRegex A readable and intuitive way to make Regular Expressions without
-having to know any of the syntax Try my new frontend for this library at
+having to know any of the syntax Try the frontend for this library at
 [ezregex.org](https://ezregex.org/)! TLDR: This is to regular expressions what
-CMake is to makefiles **Table of Contents** * [Usage](#usage) * [Installation]
-(#installation) * [Invert](#inverting) * [Generate](#generation) * [Dialects]
-(#dialects) * [Documentation](#documentation) * [Explanation](#explanation-of-
-how-it-works) * [Todo](#todo) * [License](#license) ## Usage Quickstart
-```python from ezregex import * 'foo' + number + optional(whitespace) + word #
-Matches `foo123abc` and `foo123 abc` # but not `abc123foo` or `foo bar` ```
-Importing as a named package is recommended ```python import ezregex as er # ow
-is part of er already as optional whitespace params = er.group(er.atLeastNone
-(er.ow + er.word + er.ow + er.optional(',') + er.ow)) function = er.word +
-er.ow + '(' + params + ')' # Automatically calls the re.search() function for
-you function % 'some string containing func( param1 , param2)' # The test()
-method is helpful for debugging, and color codes groups for you function.test
-('this should match func(param1,\tparam2 ), foo(), and bar( foo,)') ``` .test()
-will print all the matches, color coded to match and group (not shown here):
-```
+CMake is to makefiles ### **Table of Contents** * [Usage](#usage) * [Invert]
+(#inverting) * [Generate](#generation) * [Dialects](#dialects) *
+[Documentation](#documentation) * [Developer Docs](#developer-documentation) *
+[Installation](#installation) * [Todo](#todo) * [License](#license) ## Usage
+Quickstart ```python from ezregex import * 'foo' + number + optional
+(whitespace) + word # Matches `foo123abc` and `foo123 abc` # but not
+`abc123foo` or `foo bar` ``` Importing as a named package is recommended
+```python import ezregex as er # ow is part of er already as optional
+whitespace params = er.group(er.atLeastNone(er.ow + er.word + er.ow +
+er.optional(',') + er.ow)) # Seperate parts as variables for cleaner patterns
+function = er.word + er.ow + '(' + params + ')' # Automatically calls the
+re.search() function for you function % 'some string containing func( param1 ,
+param2)' # The test() method is helpful for debugging, and color codes groups
+for you function.test('this should match func(param1,\tparam2 ), foo(), and bar
+( foo,)') ``` .test() will print all the matches, color coded to match and
+group (colors not shown here): ```
 â­âââââââââââââââââââââââââââââ
 Testing Regex
 âââââââââââââââââââââââââââââââ®
 â Testing expression: â â \w+(?:\s+)?\(((?:(?:\s+)?\w+(?:\s+)?,?(?:
 \s+)?)*)\) â â for matches in: â â this should match func(param1,
 param2 ), foo(), and bar( foo,) â â â â Match = "func(param1, param2 )"
 (18:39) â â Unnamed Groups: â â 1: "param1, param2 " (23:38) â â
 â â Match = "foo()" (41:46) â â Unnamed Groups: â â 1: "" (45:45)
 â â â â Match = "bar( foo,)" (52:62) â â Unnamed Groups: â â 1:
 " foo," (56:61) â â â â â
 â°âââââââââââââââââââââââââââââââââ
 Found
 ââââââââââââââââââââââââââââââââââ¯
-``` ## Installation EZRegex is distributed on [PyPI](https://pypi.org) as a
-universal wheel and is available on Linux, macOS and Windows and supports
-Python 3.10+ and PyPy. ```bash $ pip install ezregex ``` The import name is the
-same as the package name: ```python import ezregex as er ``` ## Inverting The
-`invert` function provided (available as er.invert(`expression`),
+``` ## Inverting The `invert` function (available as er.invert(`expression`),
 `expression`.invert(), or ~`expression`) is useful for debugging. You pass it
 an expression, and it returns an example of a string that is guaranteed to
 match the provided expression. ## Generation In version 1.7.0 we introduced a
 new function: `generate_regex`. It takes in 2 sets of strings, and returns a
 regular expression that will match everything in the first set and nothing in
 the second set. It may be a bit crude, but it can be a good starting point if
 you don't know where to start. It's also really good at [regex golf](http://
 regex.alf.nu/). ## Dialects As of version 1.6.0, the concepts of *dialects* was
 introduced. Different languages often have slight variations on the regular
 expression syntax. As this library is meant to be language independent (even
 though it's written in Python), you should be able to compile regular
 expressions to work with other languages as well. To do that, you can simply
-import a sub-package, and they should work identically (though some languages
-may have more features than others): ```python >>> import ezregex as er # The
-python dialect is the defualt dialect >>> er.group(digit, 'name') +
-er.earlierGroup('name') EZRegex("(?P\d)(?P=name)") >>> import ezregex.perl as
-er >>> er.group(digit, 'name') + er.earlierGroup('name') EZRegex("?P\d)(\g")
-``` The currently implemented dialects are: - Python - Well tested, ~99%
-implemented - Perl - Almost identical to the Python dialect because I don't
-know Perl. If you know a particular flavor of regex and would like to
-contribute, feel free to make a pull request, or email me at
-smartycope@gmail.com ## Documentation ### Notes and Gotchas This documentation
-is for the Python dialect specifically, as it really is the only one currently
-implemented. - When using the re library, functions like search() and sub()
-don't accept EZRegexs as valid regex patterns. Be sure to call either .str() or
-.compile(), or cast to a string when passing to those. Also, be careful to call
-the function on the entire pattern: chunk + whitespace.str() is not the same as
-(chunk + whitespace).str(). - In regular Regex, a lot of random things capture
-groups for no reason. I find this annoying. All regexes in EZRegex
-intentionally capture passively, so to capture any groups, use group(), with
-the optional `name` parameter. - All EZRegexs (except for `raw`) auto-sanitize
-strings given to them, so there's no need to escape characters or use r
-strings. This *does* mean, however, that you cannot pass actual regex strings
-to any of them, as they'll think you're talking about it literally (unless you
-want that, of course). To include already written regex strings, use `raw` -
-Note that I have camelCase and snake_case versions of each of the functions,
-because I waver back and forth between which I like better. Both versions
-function identically. - The `input` parameter can accept strings, other
-EZRegexs, or entire sequences of EZRegex patterns. - A few of these have
-`greedy` and `possessive` optional parameters. They can be useful, but can get
-complicated. Refer to [the Python re docs](https://docs.python.org/3/library/
-re.html) for details. perl Positionals #### These differentiate the *string*
-starting with a sequence, and a *line* starting with a sequence. Do note that
-the startof the string is also the start of a line. These can also be called
-without parameters to denote the start/end of astring/line without something
-specific having to be next to it. - string_starts_with - string_ends_with -
-line_starts_with - line_ends_with - word_boundary - Matches the boundary of a
-word, i.e. the empty space between a word character and not a word character,
-or the end of a string - not_word_boundary - The opposite of `wordBoundary`
-Literals #### - tab - space - space_or_tab - new_line - carriage_return - quote
-- Matches ', ", and ` - vertical_tab - form_feed - comma - period - underscore
-Not Literals #### - not_whitespace - not_digit - not_word Catagories #### -
-whitespace - whitechunk - A "chunk" of whitespace. Just any amount of
-whitespace together - digit - number - Matches multiple digits next to each
-other. Does not match negatives or decimals - word - word_char - Matches just a
-single "word character", defined as any letter, number, or _ - anything -
-Matches any single character, except a newline. To also match a newline, use
-literally_anything - chunk - A "chunk": Any clump of characters up until the
-next newline - uppercase - lowercase - letter - Matches just a letter -- not
-numbers or _ like word_char - hex_digit - oct_digit - punctuation - controller
-- Matches a metadata ASCII characters - printable - Matches printable ASCII
-characters - printable_and_space - alpha_num - unicode - Matches a unicode
-character by name - any_between(char: str, and_char: str) - Match any char
-between `char` and `and_char`, using the ASCII table for reference Amounts ####
-- match_max(input: InputType) - Match as many of `input` in the string as you
-can. This is equivelent to using the unary + operator. If `input` is not
-provided, it works on the previous regex pattern. That's not recommended for
-clarity's sake though - match_num(num: int, input: InputType) - Match `num`
-amount of `input` in the string - match_more_than(min: int, input: InputType) -
-Match more than `min` sequences of `input` in the string - match_at_least(min:
-int, input: InputType) - Match at least `min` sequences of `input` in the
-string - match_at_most(max: int, input: InputType) - Match at most `max`
-instances of `input` in the string - match_range(min: int, max: int, input:
-InputType, greedy: bool=True, possessive: bool=False) - Match between `min` and
-`max` sequences of `input` in the string. This also accepts `greedy` and
-`possessive` parameters Max can be an empty string to indicate no maximum
+import all the elements as a sub-package, and they should work identically,
+although some languages may not have the same features as others. ```python >>>
+import ezregex as er # The python dialect is the defualt dialect >>> er.group
+(digit, 'name') + er.earlier_group('name') EZRegex("(?P\d)(?P=name)") >>>
+import ezregex.perl as er >>> er.group(digit, 'name') + er.earlier_group
+('name') EZRegex("?P\d)(\g") ``` The currently implemented dialects are: -
+Python - Well tested, ~99% implemented - JavaScript - Under active development,
+the basics *should* work, though tests aren't in place yet - Perl - Next on the
+roadmap, technically importable, but not implemented yet If you know a
+particular flavor of regex and would like to contribute, feel free to read the
+[developer documentation](#developer-documentation) and make a pull request! If
+you would like one that's not implemented yet, you can also add a [github
+issue](https://github.com/smartycope/ezregex/issues). ## Documentation ###
+Notes and Gotchas - The different Regular Expression dialects don't all have
+the same features, and those features don't all work the same way. I've tried
+to standardize these as best I can and use reasonable names for all the
+elements. If you're confused by something not working as expected, be sure to
+understand how your language specifically handles regular expressions. - When
+using the Python `re` library, functions like re.search() and re.sub() don't
+accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast
+it to a string) or .compile() (to compile to an re.Pattern) when passing to
+those. Also, be careful to call the function on the entire pattern: chunk +
+whitespace.str() is not the same as (chunk + whitespace).str(). - In regular
+regex, a lot of random things capture groups for no apparent reason. All
+regexes in EZRegex intentionally capture passively, so to capture any groups,
+use group(), with the optional `name` parameter. - All EZRegexs (except for
+`raw`) auto-sanitize strings given to them, so there's no need to escape
+characters or use r strings. This *does* mean, however, that you cannot pass
+actual regex strings to any of them, as they'll think you're talking about it
+literally (unless you want that, of course). To include already written regex
+strings, use `raw` - Note that I have camelCase and snake_case versions of each
+of the functions, because I waver back and forth between which I like better.
+Both versions function identically. - The `InputType` can accept strings, other
+EZRegexs, or entire sequences of EZRegex patterns. It can also accept things
+that can be cast to a string, but it will warn you when it does, so it's better
+to cast to a string yourself. - The `invert` function can accept any regular
+expression, not just EZRegex expressions, if you want to use it independently
+of the rest of the library. _pp_ee_rr_ll Positionals #### These differentiate the
+*string* starting with a sequence, and a *line* starting with a sequence. Do
+note that the startof the string is also the start of a line. These can also be
+called without parameters to denote the start/end of astring/line without
+something specific having to be next to it. - string_starts_with -
+string_ends_with - line_starts_with - line_ends_with - word_boundary - Matches
+the boundary of a word, i.e. the empty space between a word character and not a
+word character, or the end of a string - not_word_boundary - The opposite of
+`wordBoundary` Literals #### - tab - space - space_or_tab - new_line -
+carriage_return - quote - Matches ', ", and ` - vertical_tab - form_feed -
+comma - period - underscore Not Literals #### - not_whitespace - not_digit -
+not_word Catagories #### - whitespace - whitechunk - A "chunk" of whitespace.
+Just any amount of whitespace together - digit - number - Matches multiple
+digits next to each other. Does not match negatives or decimals - word -
+word_char - Matches just a single "word character", defined as any letter,
+number, or _ - anything - Matches any single character, except a newline. To
+also match a newline, use literally_anything - chunk - A "chunk": Any clump of
+characters up until the next newline - uppercase - lowercase - letter - Matches
+just a letter -- not numbers or _ like word_char - hex_digit - oct_digit -
+punctuation - controller - Matches a metadata ASCII characters - printable -
+Matches printable ASCII characters - printable_and_space - alpha_num - unicode
+- Matches a unicode character by name - any_between(char: str, and_char: str) -
+Match any char between `char` and `and_char`, using the ASCII table for
+reference Amounts #### - match_max(input: InputType) - Match as many of `input`
+in the string as you can. This is equivelent to using the unary + operator. If
+`input` is not provided, it works on the previous regex pattern. That's not
+recommended for clarity's sake though - match_num(num: int, input: InputType) -
+Match `num` amount of `input` in the string - match_more_than(min: int, input:
+InputType) - Match more than `min` sequences of `input` in the string -
+match_at_least(min: int, input: InputType) - Match at least `min` sequences of
+`input` in the string - match_at_most(max: int, input: InputType) - Match at
+most `max` instances of `input` in the string - match_range(min: int, max: int,
+input: InputType, greedy: bool=True, possessive: bool=False) - Match between
+`min` and `max` sequences of `input` in the string. This also accepts `greedy`
+and `possessive` parameters Max can be an empty string to indicate no maximum
 `greedy` means it will try to match as many repititions as possible non-greedy
 will try to match as few repititions as possible `possessive` means it won't
 backtrack to try to find any repitions see https://docs.python.org/3/library/
 re.html for more help - at_least_one(input: InputType, greedy: bool=True,
 possessive: bool=False) - Match at least one of `input` in the string. This
 also accepts `greedy` and `possessive` parameters `greedy` means it will try to
 match as many repititions as possible non-greedy will try to match as few
@@ -219,19 +228,19 @@
 ASCII flag is used to disable non-ASCII matches. The current locale does
 notchange the effect of this flag unless the LOCALE flag is also used - DOTALL
 - Make the '.' special character match any character at all, including a
 newline. It's recommended you simply useliterally_anything instead - LOCALE -
 Try not to use this, and rely on unicode matching instead - MULTILINE - This is
 automatically inserted when using line_start and line_end, you shouldn't need
 to add it manually - UNICODE - Match using the full unicode standard, instead
-of just ASCII. Enabled by default, and therefore redundant. python Positionals
-#### These differentiate the *string* starting with a sequence, and a *line*
-starting with a sequence. Do note that the startof the string is also the start
-of a line. These can also be called without parameters to denote the start/end
-of astring/line without something specific having to be next to it. -
+of just ASCII. Enabled by default, and therefore redundant. _jj_aa_vv_aa_ss_cc_rr_ii_pp_tt
+Positionals #### These differentiate the *string* starting with a sequence, and
+a *line* starting with a sequence. Do note that the startof the string is also
+the start of a line. These can also be called without parameters to denote the
+start/end of astring/line without something specific having to be next to it. -
 string_starts_with - string_ends_with - line_starts_with - line_ends_with -
 word_boundary - Matches the boundary of a word, i.e. the empty space between a
 word character and not a word character, or the end of a string -
 not_word_boundary - The opposite of `wordBoundary` Literals #### - tab - space
 - space_or_tab - new_line - carriage_return - quote - Matches ', ", and ` -
 vertical_tab - form_feed - comma - period - underscore Not Literals #### -
 not_whitespace - not_digit - not_word Catagories #### - whitespace - whitechunk
@@ -362,189 +371,233 @@
 uppercase members. Full Unicode matching(such as Ã matching Ã¼) also works
 unless the ASCII flag is used to disable non-ASCII matches. The current locale
 does notchange the effect of this flag unless the LOCALE flag is also used -
 DOTALL - Make the '.' special character match any character at all, including a
 newline. It's recommended you simply useliterally_anything instead - LOCALE -
 Try not to use this, and rely on unicode matching instead - MULTILINE - This is
 automatically inserted when using line_start and line_end, you shouldn't need
-to add it manually javascript Positionals #### These differentiate the *string*
-starting with a sequence, and a *line* starting with a sequence. Do note that
-the startof the string is also the start of a line. These can also be called
-without parameters to denote the start/end of astring/line without something
-specific having to be next to it. - string_starts_with - string_ends_with -
-line_starts_with - line_ends_with - word_boundary - Matches the boundary of a
-word, i.e. the empty space between a word character and not a word character,
-or the end of a string - not_word_boundary - The opposite of `wordBoundary`
-Literals #### - tab - space - space_or_tab - new_line - carriage_return - quote
-- Matches ', ", and ` - vertical_tab - form_feed - comma - period - underscore
-Not Literals #### - not_whitespace - not_digit - not_word Catagories #### -
-whitespace - whitechunk - A "chunk" of whitespace. Just any amount of
-whitespace together - digit - number - Matches multiple digits next to each
-other. Does not match negatives or decimals - word - word_char - Matches just a
-single "word character", defined as any letter, number, or _ - anything -
-Matches any single character, except a newline. To also match a newline, use
-literally_anything - chunk - A "chunk": Any clump of characters up until the
-next newline - uppercase - lowercase - letter - Matches just a letter -- not
-numbers or _ like word_char - hex_digit - oct_digit - punctuation - controller
-- Matches a metadata ASCII characters - printable - Matches printable ASCII
-characters - printable_and_space - alpha_num - unicode - Matches a unicode
-character by name - any_between(char: str, and_char: str) - Match any char
-between `char` and `and_char`, using the ASCII table for reference Amounts ####
-- match_max(input: InputType) - Match as many of `input` in the string as you
-can. This is equivelent to using the unary + operator. If `input` is not
-provided, it works on the previous regex pattern. That's not recommended for
-clarity's sake though - match_num(num: int, input: InputType) - Match `num`
-amount of `input` in the string - match_more_than(min: int, input: InputType) -
-Match more than `min` sequences of `input` in the string - match_at_least(min:
-int, input: InputType) - Match at least `min` sequences of `input` in the
-string - match_at_most(max: int, input: InputType) - Match at most `max`
-instances of `input` in the string - match_range(min: int, max: int, input:
-InputType, greedy: bool=True, possessive: bool=False) - Match between `min` and
-`max` sequences of `input` in the string. This also accepts `greedy` and
-`possessive` parameters Max can be an empty string to indicate no maximum
+to add it manually - UNICODE - Match using the full unicode standard, instead
+of just ASCII. Enabled by default, and therefore redundant. _pp_yy_tt_hh_oo_nn Positionals
+#### These differentiate the *string* starting with a sequence, and a *line*
+starting with a sequence. Do note that the startof the string is also the start
+of a line. These can also be called without parameters to denote the start/end
+of astring/line without something specific having to be next to it. -
+string_starts_with - string_ends_with - line_starts_with - line_ends_with -
+word_boundary - Matches the boundary of a word, i.e. the empty space between a
+word character and not a word character, or the end of a string -
+not_word_boundary - The opposite of `wordBoundary` Literals #### - tab - space
+- space_or_tab - new_line - carriage_return - quote - Matches ', ", and ` -
+vertical_tab - form_feed - comma - period - underscore Not Literals #### -
+not_whitespace - not_digit - not_word Catagories #### - whitespace - whitechunk
+- A "chunk" of whitespace. Just any amount of whitespace together - digit -
+number - Matches multiple digits next to each other. Does not match negatives
+or decimals - word - word_char - Matches just a single "word character",
+defined as any letter, number, or _ - anything - Matches any single character,
+except a newline. To also match a newline, use literally_anything - chunk - A
+"chunk": Any clump of characters up until the next newline - uppercase -
+lowercase - letter - Matches just a letter -- not numbers or _ like word_char -
+hex_digit - oct_digit - punctuation - controller - Matches a metadata ASCII
+characters - printable - Matches printable ASCII characters -
+printable_and_space - alpha_num - unicode - Matches a unicode character by name
+- any_between(char: str, and_char: str) - Match any char between `char` and
+`and_char`, using the ASCII table for reference Amounts #### - match_max(input:
+InputType) - Match as many of `input` in the string as you can. This is
+equivelent to using the unary + operator. If `input` is not provided, it works
+on the previous regex pattern. That's not recommended for clarity's sake though
+- match_num(num: int, input: InputType) - Match `num` amount of `input` in the
+string - match_more_than(min: int, input: InputType) - Match more than `min`
+sequences of `input` in the string - match_at_least(min: int, input: InputType)
+- Match at least `min` sequences of `input` in the string - match_at_most(max:
+int, input: InputType) - Match at most `max` instances of `input` in the string
+- match_range(min: int, max: int, input: InputType, greedy: bool=True,
+possessive: bool=False) - Match between `min` and `max` sequences of `input` in
+the string. This also accepts `greedy` and `possessive` parameters Max can be
+an empty string to indicate no maximum `greedy` means it will try to match as
+many repititions as possible non-greedy will try to match as few repititions as
+possible `possessive` means it won't backtrack to try to find any repitions see
+https://docs.python.org/3/library/re.html for more help - at_least_one(input:
+InputType, greedy: bool=True, possessive: bool=False) - Match at least one of
+`input` in the string. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible non-greedy
 will try to match as few repititions as possible `possessive` means it won't
 backtrack to try to find any repitions see https://docs.python.org/3/library/
-re.html for more help - at_least_one(input: InputType, greedy: bool=True,
-possessive: bool=False) - Match at least one of `input` in the string. This
-also accepts `greedy` and `possessive` parameters `greedy` means it will try to
+re.html for more help - at_least_none(input: InputType, greedy: bool=True,
+possessive: bool=False) - Match 0 or more sequences of `input`. This also
+accepts `greedy` and `possessive` parameters `greedy` means it will try to
 match as many repititions as possible non-greedy will try to match as few
 repititions as possible `possessive` means it won't backtrack to try to find
-any repitions see https://docs.python.org/3/library/re.html for more help -
-at_least_none(input: InputType, greedy: bool=True, possessive: bool=False) -
-Match 0 or more sequences of `input`. This also accepts `greedy` and
+any repitions see https://docs.python.org/3/library/re.html for more help
+Choices #### - optional(input: InputType, greedy: bool=True, possessive:
+bool=False) - Match `input` if it's there. This also accepts `greedy` and
 `possessive` parameters `greedy` means it will try to match as many repititions
 as possible non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions see https://
-docs.python.org/3/library/re.html for more help Choices #### - optional(input:
-InputType, greedy: bool=True, possessive: bool=False) - Match `input` if it's
-there. This also accepts `greedy` and `possessive` parameters `greedy` means it
-will try to match as many repititions as possible non-greedy will try to match
-as few repititions as possible `possessive` means it won't backtrack to try to
-find any repitions see https://docs.python.org/3/library/re.html for more help
-- either(input: InputType, or_input: InputType) - any_of(*inputs: str, chars:
-bool | None=None, split: bool | None=None) - Match any of the given `inputs`.
-Note that `inputs` can be multiple parameters, or a single string. Can also
-accept parameters chars and split. If char is set to True, then `inputs` must
-only be a single string, it interprets `inputs` as characters, and splits it up
-to find any of the chars in the string. If split is set to true, it forces the
-?(...) regex syntax instead of the [...] syntax. It should act the same way,
-but your output regex will look different. By default, it just optimizes it for
-you. - any_char_except(*inputs: str) - This matches any char that is NOT in
-`inputs`. `inputs` can be multiple parameters, or a single string of chars to
-split. - any_except(input: InputType, type: InputType='.*') - Matches anything
-other than `input`, which must be a single string or EZRegex chain, **not** a
-list. Also optionally accepts the `type` parameter, which works like this:
-"Match any `type` other than `input`". For example, "match any word which is
-not foo". Do note that this function is new, and I'm still working out the
-kinks. - each(*inputs: InputType) - Matches if the next part of the string can
-match all of the given inputs. Like the + operator, but out of order.
-Conditionals #### These can only be used once in a given expression. They only
-match a given expression if the expression is/ins'tfollowed/preceeded by a the
-given pattern - if_proceded_by(input: InputType) - Matches the pattern if it
-has `input` coming after it. Can only be used once in a given pattern, as it
-only applies to the end - if_not_proceded_by(input: InputType) - Matches the
-pattern if it does **not** have `input` coming after it. Can only be used once
-in a given pattern, as it only applies to the end - if_preceded_by(input:
-InputType) - Matches the pattern if it has `input` coming before it. Can only
-be used once in a given pattern, as it only applies to the beginning -
-if_not_preceded_by(input: InputType) - Matches the pattern if it does **not**
-have `input` coming before it. Can only be used once in a given pattern, as it
-only applies to the beginning - if_enclosed_with(open: str, stuff: InputType,
-close: str | None=None) - Matches if the string has `open`, then `stuff`, then
-`close`, but only "matches" stuff. Just a convenience combination of
-ifProceededBy and ifPreceededBy. Grouping #### - group(input: InputType, name:
-str | None=None) - Causes `input` to be captured as an unnamed group. Only
-useful when replacing regexs - passive_group(input: InputType) - As all regexs
-in EZRegex capture passively, this is entirely useless. But if you really want
-to, here it is - earlier_group(num_or_name: int | str) - Matches whatever the
-group referenced by `num_or_name` matched earlier. Must be *after* a group
-which would match `num_or_name` - if_exists(num_or_name: int | str, does:
-InputType, doesnt: InputType | None=None) - Matches `does` if the group
-`num_or_name` exists, otherwise it matches `doesnt` Replacement #### In the
-intrest of "I don't want to think about any syntax at all", I have included
-replace members. Do note that theyare not interoperable with the other
-EZRegexs, and can only be used with other strings and each other. - rgroup
-(num_or_name: str | int) - Puts in its place the group specified, either by
-group number (for unnamed groups) or group name (for named groups). Named
-groups are also counted by number, I'm pretty sure. Groups are numbered
-starting from 1 - replace_entire - Puts in its place the entire match - replace
-(string: str, rtn_str: bool=True) -> str | EZRegex - Generates a valid regex
-replacement string, using Python f-string like syntax. Example: ``` replace
-("named: {group}, numbered: {1}, entire: {0}") ``` Like Python f-strings, use {
-{ and }} to specify { and } Set the `rtn_str` parameter to True to have it
-return an EZRegex type instead of a string Note: Remember that index 0 is the
-entire match There's a few of advantages to using this instead of just the
-regular regex replacement syntax: - It's consistent between dialects - It's
-closer to Python f-string syntax, which is cleaner and more familiar - It
-handles numbered, named, and entire replacement types the same Misc #### -
-is_exactly(input: InputType) - This matches the string if and only if the
-entire string is exactly equal to `input` - literal(input: InputType) - This is
-a redundant function. You should always be able to use `... + 'stuff'` just as
-easily as `... + literal('stuff')` - raw(regex: str) - If you already have some
-regular regex written, and you want to incorperate it, this will allow you to
-include it without sanatizing all the backslaches and such, which all the other
-EZRegexs do automatically Premade #### These are some useful combinations that
-may be commonly used. They are not as stable, and may be changed and added to
-inlater versions to make them more accurate - literally_anything - *Any*
-character, include newline - signed - a signed number, including 123, -123, and
-+123 - unsigned - Same as number. Will not match +123 - plain_float - Will
-match 123.45 and 123. - full_float - Will match plain_float as well as things
-like 1.23e-10 and 1.23e+10 - int_or_float - ow - "Optional Whitechunk" - email
-- Matches an email - version - The *official* regex for matching version
-numbers from https://semver.org/. It includes 5 groups that can bematched/
-replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata` -
-version_numbered - Same as `version`, but it uses numbered groups for each
-version number instead of named groups Flags #### These shadow python regex
-flags, and can just as easily be specified directly to the re library instead.
-They're providedhere for compatibility with other regex dialects. See https://
-docs.python.org/3/library/re.html#flags for details - ASCII - Make matching
-words, word boundaries, digits, and whitespace perform ASCII-only matching
-instead of full Unicodematching. This is only meaningful for Unicode (str)
-patterns, and is ignored for bytes patterns - IGNORECASE - Perform case-
-insensitive matching, including expressions that explicitly use uppercase
-members. Full Unicode matching(such as Ã matching Ã¼) also works unless the
-ASCII flag is used to disable non-ASCII matches. The current locale does
-notchange the effect of this flag unless the LOCALE flag is also used - DOTALL
-- Make the '.' special character match any character at all, including a
+docs.python.org/3/library/re.html for more help - either(input: InputType,
+or_input: InputType) - any_of(*inputs: str, chars: bool | None=None, split:
+bool | None=None) - Match any of the given `inputs`. Note that `inputs` can be
+multiple parameters, or a single string. Can also accept parameters chars and
+split. If char is set to True, then `inputs` must only be a single string, it
+interprets `inputs` as characters, and splits it up to find any of the chars in
+the string. If split is set to true, it forces the ?(...) regex syntax instead
+of the [...] syntax. It should act the same way, but your output regex will
+look different. By default, it just optimizes it for you. - any_char_except
+(*inputs: str) - This matches any char that is NOT in `inputs`. `inputs` can be
+multiple parameters, or a single string of chars to split. - any_except(input:
+InputType, type: InputType='.*') - Matches anything other than `input`, which
+must be a single string or EZRegex chain, **not** a list. Also optionally
+accepts the `type` parameter, which works like this: "Match any `type` other
+than `input`". For example, "match any word which is not foo". Do note that
+this function is new, and I'm still working out the kinks. - each(*inputs:
+InputType) - Matches if the next part of the string can match all of the given
+inputs. Like the + operator, but out of order. Conditionals #### These can only
+be used once in a given expression. They only match a given expression if the
+expression is/ins'tfollowed/preceeded by a the given pattern - if_proceded_by
+(input: InputType) - Matches the pattern if it has `input` coming after it. Can
+only be used once in a given pattern, as it only applies to the end -
+if_not_proceded_by(input: InputType) - Matches the pattern if it does **not**
+have `input` coming after it. Can only be used once in a given pattern, as it
+only applies to the end - if_preceded_by(input: InputType) - Matches the
+pattern if it has `input` coming before it. Can only be used once in a given
+pattern, as it only applies to the beginning - if_not_preceded_by(input:
+InputType) - Matches the pattern if it does **not** have `input` coming before
+it. Can only be used once in a given pattern, as it only applies to the
+beginning - if_enclosed_with(open: str, stuff: InputType, close: str |
+None=None) - Matches if the string has `open`, then `stuff`, then `close`, but
+only "matches" stuff. Just a convenience combination of ifProceededBy and
+ifPreceededBy. Grouping #### - group(input: InputType, name: str | None=None) -
+Causes `input` to be captured as an unnamed group. Only useful when replacing
+regexs - passive_group(input: InputType) - As all regexs in EZRegex capture
+passively, this is entirely useless. But if you really want to, here it is -
+earlier_group(num_or_name: int | str) - Matches whatever the group referenced
+by `num_or_name` matched earlier. Must be *after* a group which would match
+`num_or_name` - if_exists(num_or_name: int | str, does: InputType, doesnt:
+InputType | None=None) - Matches `does` if the group `num_or_name` exists,
+otherwise it matches `doesnt` Replacement #### In the intrest of "I don't want
+to think about any syntax at all", I have included replace members. Do note
+that theyare not interoperable with the other EZRegexs, and can only be used
+with other strings and each other. - rgroup(num_or_name: str | int) - Puts in
+its place the group specified, either by group number (for unnamed groups) or
+group name (for named groups). Named groups are also counted by number, I'm
+pretty sure. Groups are numbered starting from 1 - replace_entire - Puts in its
+place the entire match - replace(string: str, rtn_str: bool=True) -> str |
+EZRegex - Generates a valid regex replacement string, using Python f-string
+like syntax. Example: ``` replace("named: {group}, numbered: {1}, entire: {0}")
+``` Like Python f-strings, use {{ and }} to specify { and } Set the `rtn_str`
+parameter to True to have it return an EZRegex type instead of a string Note:
+Remember that index 0 is the entire match There's a few of advantages to using
+this instead of just the regular regex replacement syntax: - It's consistent
+between dialects - It's closer to Python f-string syntax, which is cleaner and
+more familiar - It handles numbered, named, and entire replacement types the
+same Misc #### - is_exactly(input: InputType) - This matches the string if and
+only if the entire string is exactly equal to `input` - literal(input:
+InputType) - This is a redundant function. You should always be able to use
+`... + 'stuff'` just as easily as `... + literal('stuff')` - raw(regex: str) -
+If you already have some regular regex written, and you want to incorperate it,
+this will allow you to include it without sanatizing all the backslaches and
+such, which all the other EZRegexs do automatically Premade #### These are some
+useful combinations that may be commonly used. They are not as stable, and may
+be changed and added to inlater versions to make them more accurate -
+literally_anything - *Any* character, include newline - signed - a signed
+number, including 123, -123, and +123 - unsigned - Same as number. Will not
+match +123 - plain_float - Will match 123.45 and 123. - full_float - Will match
+plain_float as well as things like 1.23e-10 and 1.23e+10 - int_or_float - ow -
+"Optional Whitechunk" - email - Matches an email - version - The *official*
+regex for matching version numbers from https://semver.org/. It includes 5
+groups that can bematched/replaced: `major`, `minor`, `patch`, `prerelease`,
+and `buildmetadata` - version_numbered - Same as `version`, but it uses
+numbered groups for each version number instead of named groups Flags ####
+These shadow python regex flags, and can just as easily be specified directly
+to the re library instead. They're providedhere for compatibility with other
+regex dialects. See https://docs.python.org/3/library/re.html#flags for details
+- ASCII - Make matching words, word boundaries, digits, and whitespace perform
+ASCII-only matching instead of full Unicodematching. This is only meaningful
+for Unicode (str) patterns, and is ignored for bytes patterns - IGNORECASE -
+Perform case-insensitive matching, including expressions that explicitly use
+uppercase members. Full Unicode matching(such as Ã matching Ã¼) also works
+unless the ASCII flag is used to disable non-ASCII matches. The current locale
+does notchange the effect of this flag unless the LOCALE flag is also used -
+DOTALL - Make the '.' special character match any character at all, including a
 newline. It's recommended you simply useliterally_anything instead - LOCALE -
 Try not to use this, and rely on unicode matching instead - MULTILINE - This is
 automatically inserted when using line_start and line_end, you shouldn't need
-to add it manually - UNICODE - Match using the full unicode standard, instead
-of just ASCII. Enabled by default, and therefore redundant. Operators - `+`,
-`<<`, `>>` - These all do the same thing: combine expressions - `*` -
-Multiplies an expression a number of times. `expr * 3` is equivelent to `expr +
-expr + expr`. Can also be used like `expr * ...` is equivalent to `anyAmt
-(expr)` - `+` - A unary + operator acts exactly as a match_max() does, or, if
-you're familiar with regex syntax, the + operator - `[]` - expr[2, 3] is
-equivalent to `match_range(2, 3, expr)` - expr[2, ...] or expr[2,] is
-equivalent to `at_least(2, expr)` - expr[... , 2] is equivalent to `at_most(2,
-expr)` - expr[...] or expr[0, ...] is equivelent to `at_least_0(expr)` - expr
-[1, ...] is equivalent to `at_least_1(expr)` - `&` - Coming soon! This will
-work like the + operator, but they can be out of order. Like an and operation.
-- `|` - Coming soon! This will work like an or operation, which will work just
-like anyOf() - `%` - This automatically calls re.search() for you and returns
-the match object (or None). Use like this: `(digit * 2) % '99 beers on the
-wall'` - `~` - This inverts the expression. This is equivalent to calling the
-.invert() method ## Explanation of How it Works Everything relies on the
-EZRegex class. In the elements.py file of each dialect, I have defined a ton of
-pre-made EZRegexs which mimic all (or at least as many as I can) fundamental
-parts of the regex syntax, plus a few others which are common combinations
-(like chunk or optional(whitechunk)). Any of them which have parameters are
-wrapped in functions to provide proper typing & linting. They all are either
-EZRegexs or are functions which return EZRegexs. These have operators
-overloaded so you can combine them in intuitive ways and call them by intuitive
-names. All the functions passed to EZRegex take a function parameter (or a
-string which gets converted to a function for convenience), which gets called
-with the current regex expression and any parameters passed along when the
-instance gets called with the () operator. That way you can add things to the
-front or back of an expression for example, and you can change what exactly
-gets added to the current expression based on other parameters. You can also
-chain strings together, and pass them as parameters to other EZRegexs, which
-auto-compiles them and adds them appropriately. I also have everything which
-could capture a group capture it passively, except for actual group operators,
-and always have the (?m) (multiline) flag automatically asserted whenever
-lineStart/lineEnd are used so as to differentiate between capturing at the
-beginning/end of a string and the beginning/end of a line. ## Todo See [the
-todo](todo.txt). Eventually, I would like to move the todo to GitHub issues. ##
-License EZRegex is distributed under the [MIT License](https://
-choosealicense.com/licenses/mit)
+to add it manually Operators - `+`, `<<`, `>>` - These all do the same thing:
+combine expressions - `*` - Multiplies an expression a number of times. `expr *
+3` is equivelent to `expr + expr + expr`. Can also be used like `expr * ...` is
+equivalent to `any_amt(expr)` - `+` - A unary + operator acts exactly as a
+match_max() does, or, if you're familiar with regex syntax, the + operator - `
+[]` - expr[2, 3] is equivalent to `match_range(2, 3, expr)` - expr[2, ...] or
+expr[2,] is equivalent to `at_least(2, expr)` - expr[... , 2] is equivalent to
+`at_most(2, expr)` - expr[...] or expr[0, ...] is equivelent to `at_least_0
+(expr)` - expr[1, ...] is equivalent to `at_least_1(expr)` - `&` - Coming soon!
+This will work like the + operator, but they can be out of order. Like an and
+operation. - `|` - Coming soon! This will work like an or operation, which will
+work just like any_of() - `%` - This automatically calls re.search() for you
+and returns the match object (or None). Use like this: `(digit * 2) % '99 beers
+on the wall'` - `~` - This inverts the expression, equivalent to calling the
+.invert() method ## Developer Documentation ### The EZRegex class Everything
+relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as
+each dialect defines their own EZRegex elements specific to that dialect (more
+on that later). Each element represents a fundamental part of the Regular
+Expression syntax for that language, as well as less-fundemental common
+combinations for convenience (like email and float). EZRegex can accept a
+string or a function to define how it's supposed to interact with the current
+"chain" of elements. If it's a string, it just adds it to the end. If it's a
+function, it can accept any positional or named parameters, but has to accept
+`cur=...` as the last parameter (it's complicated). The `cur` parameter is the
+current regular expression chain, as a string. What's returned becomes the new
+`cur` parameter of the next element, or, if there is no next element, the final
+regex. That way you can add to the front or back of an expression, and you can
+change what exactly gets added to the current expression based on other
+parameters. The EZRegex class has operators overloaded so you can combine them
+in intuitive ways and call them by intuitive names. ### Typing & Linting The
+updated method of doing this is to define all the EZRegex elements of a dialect
+in `elements.py`, and then add type hints and doc strings in the `elements.pyi`
+file. EZRegex elements that accept parameters are typed as functions (even
+though they're not), for both convenience for the user when using linter, and
+to give documentation in an easier way. EZRegex elements that don't accept
+parameters should be typed as EZRegex, and given documentation as a string on
+the line below it. This is *slightly* non-standard, but linters support it, as
+well as my documentation generator script, which parses the .pyi files. The
+elements can also be seperated into groups in the .pyi files by using `"Group:
+\\n\"`, which also gets parsed by the documentation script. The groups aren't
+used in the actual library, but are helpful in seperating the documentation, as
+well as used in [ezregex.org](http://ezregex.org) ### Dialects Because most
+regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but
+it works a bit differently. It has an `elements.py` file, but it defines all
+the elements as a dict in the form of {"element_name": {"keyword":
+"arguements"}}. It then has a `load_dialect()` function, which is the only
+thing importable from it. The reason it's done this way is because `dialect` is
+a required parameter of the EZRegex constructor, so `load_dialect()` takes a
+`dialect` parameter, and constructs the base elements from it's dict and
+returns a new dict of initialized elements to be dumped into the global scope
+of the dialect. The `elements.py` file of a specific dialect can then remove
+any elements that it doesn't support (using the `del` keyword) and add/
+overwrite any it does support. ### Inverting There's actually 2 algorithms
+implemented for "inverting" regexs. The old algorithm regexs the regexs in a
+specific order to replace parts one at a time. This is just as nasty and
+horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I
+actually got it to work decently well. Later, when I was reading up on abstract
+syntax trees, and scrolling around on PyPi, I realized that Python has one
+built in, and that it's available to use. I reimplemented the whole algorithm
+to instead parse the AST given by the built-in re lexer, and wrote my own
+parser on top of it, which works *much* better. Along the way, I also
+discovered, deep in the corners of the internet, 2 other Python libraries which
+do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger`
+technically works, however it tends to include unprintable characters, so it's
+output isn't very readable. `sre_yeild` is better, but it can be very slow, and
+is not quite the use case I'm going for. My invert algorithm is meant to be a
+debugging tool (though it doubles well for a testing tool), so it does things
+like detecting words (as opposed to seperate word characters) and inserts
+actual words, and doing the same for numbers and inserting `12345...`, as well
+as a couple other enhancements. ### Tests Tests for a while now have just been
+in a single `tests.py` file, which was a giant pile of all the tests. I'm
+currently moving to use pytest. There's a `regexs.json` file (and a
+`replacements.json` file) that have a bunch of regexs, along with things
+they're supposed to match, and things they're not supposed to match, for
+testing. ## Installation EZRegex is distributed on [PyPI](https://pypi.org) as
+a universal wheel and is available on Linux, macOS and Windows and supports
+Python 3.10+ and PyPy. ```bash pip install ezregex ``` The import name is the
+same as the package name: ```python import ezregex as er ``` ## Todo See [the
+todo](todo.txt). I'm slowly moving these to [GitHub issues](https://github.com/
+smartycope/ezregex/issues), but for now, they're mostly still there ## License
+EZRegex is distributed under the [MIT License](https://choosealicense.com/
+licenses/mit)
```

### Comparing `ezregex-1.9.3/PKG-INFO` & `ezregex-1.9.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: ezregex
-Version: 1.9.3
+Version: 1.9.4
 Summary: A readable and intuitive way to generate Regular Expressions
-Project-URL: Documentation, https://github.com/smartycope/ezregex#readme
+Project-URL: Documentation, https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation
 Project-URL: Issues, https://github.com/smartycope/ezregex/issues
 Project-URL: Source, https://github.com/smartycope/ezregex
 Project-URL: Official Website, https://ezregex.org
 Author-email: Copeland Carter <smartycope@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -16,49 +16,57 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 <div align="center">
-    <img src="https://ezregex.org/favicon.png"><br>
-    <p></p>
-
-<a href="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml">
-    <img src="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml/badge.svg" alt="Unit Tests">
-</a>
-<a href="https://pypi.org/project/ezregex/">
-    <img src="https://img.shields.io/pypi/v/ezregex.svg" alt="PyPI Latest Release">
-</a>
-<a href="https://choosealicense.com/licenses/mit/">
-    <img src="https://img.shields.io/github/license/smartycope/ezregex">
-</a>
-<a href="https://www.python.org/">
-    <img src="https://img.shields.io/pypi/implementation/ezregex">
-</a>
-<a href="https://pypi.org/project/ezregex/#files">
-    <img src="https://img.shields.io/pypi/format/ezregex">
-</a>
+    <img src="https://ezregex.org/favicon.png">
+    <br>
+    <br>
+    <a href="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml">
+        <img src="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml/badge.svg" alt="Unit Tests">
+    </a>
+    <a href="https://pypi.org/project/ezregex/">
+        <img src="https://img.shields.io/pypi/v/ezregex.svg" alt="PyPI Latest Release">
+    </a>
+    <a href="https://choosealicense.com/licenses/mit/">
+        <img src="https://img.shields.io/github/license/smartycope/ezregex">
+    </a>
+    <!-- <a href="https://www.python.org/">
+        <img src="https://img.shields.io/pypi/implementation/ezregex">
+    </a> -->
+    <!-- <a href="https://pypi.org/project/ezregex/#files">
+        <img src="https://img.shields.io/pypi/format/ezregex">
+    </a> -->
+    <img src="https://img.shields.io/badge/dependencies-0-blue">
+</div>
+<div align="center">
+    <img src="https://img.shields.io/badge/Supported%20Dialects-3-green">
+    <img src="https://img.shields.io/badge/Python%20Dialect-100%25-blue">
+    <img src="https://img.shields.io/badge/JavaScript%20Dialect-50%25-yellow">
+    <img src="https://img.shields.io/badge/Perl%20Dialect-20%25-red">
 </div>
 
+
 # EZRegex
 A readable and intuitive way to make Regular Expressions without having to know any of the syntax
 
-Try my new frontend for this library at [ezregex.org](https://ezregex.org/)!
+Try the frontend for this library at [ezregex.org](https://ezregex.org/)!
 
 TLDR: This is to regular expressions what CMake is to makefiles
 
-**Table of Contents**
+### **Table of Contents**
 * [Usage](#usage)
-* [Installation](#installation)
 * [Invert](#inverting)
 * [Generate](#generation)
 * [Dialects](#dialects)
 * [Documentation](#documentation)
-* [Explanation](#explanation-of-how-it-works)
+* [Developer Docs](#developer-documentation)
+* [Installation](#installation)
 * [Todo](#todo)
 * [License](#license)
 
 ## Usage
 
 Quickstart
 ```python
@@ -67,23 +75,27 @@
 # Matches `foo123abc` and `foo123 abc`
 # but not `abc123foo` or  `foo bar`
 ```
 
 Importing as a named package is recommended
 ```python
 import ezregex as er
+
 # ow is part of er already as optional whitespace
 params = er.group(er.atLeastNone(er.ow + er.word + er.ow + er.optional(',') + er.ow))
+# Seperate parts as variables for cleaner patterns
 function = er.word + er.ow + '(' + params + ')'
+
 # Automatically calls the re.search() function for you
 function % 'some string containing func( param1 , param2)'
+
 # The test() method is helpful for debugging, and color codes groups for you
 function.test('this should match func(param1,\tparam2 ), foo(), and bar( foo,)')
 ```
-.test() will print all the matches, color coded to match and group (not shown here):
+.test() will print all the matches, color coded to match and group (colors not shown here):
 
 ```
 ╭───────────────────────────── Testing Regex ──────────────────────────────╮
 │ Testing expression:                                                      │
 │         \w+(?:\s+)?\(((?:(?:\s+)?\w+(?:\s+)?,?(?:\s+)?)*)\)              │
 │ for matches in:                                                          │
 │         this should match func(param1,  param2 ), foo(), and bar( foo,)  │
@@ -125,85 +137,75 @@
 │         1: "<span style="color: green;"> foo,</span>" (56:61)                                               │
 │                                                                          │
 │                                                                          │
 ╰───────────────────────────────── <span style="color: blue;">Found</span>  ─────────────────────────────────╯
 </pre>
 -->
 
-## Installation
-EZRegex is distributed on [PyPI](https://pypi.org) as a universal
-wheel and is available on Linux, macOS and Windows and supports
-Python 3.10+ and PyPy.
-
-```bash
-$ pip install ezregex
-```
-
-The import name is the same as the package name:
-```python
-import ezregex as er
-```
 
 ## Inverting
-The `invert` function provided (available as er.invert(`expression`), `expression`.invert(), or ~`expression`) is useful for debugging. You pass it an expression, and it returns an example of a string that is guaranteed to match the provided expression.
+The `invert` function (available as er.invert(`expression`), `expression`.invert(), or ~`expression`) is useful for debugging. You pass it an expression, and it returns an example of a string that is guaranteed to match the provided expression.
 
 
 ## Generation
 In version 1.7.0 we introduced a new function: `generate_regex`. It takes in 2 sets of strings, and returns a regular expression that will match everything in the first set and nothing in the second set. It may be a bit crude, but it can be a good starting point if you don't know where to start. It's also really good at [regex golf](http://regex.alf.nu/).
 
 
 ## Dialects
-As of version 1.6.0, the concepts of *dialects* was introduced. Different languages often have slight variations on the regular expression syntax. As this library is meant to be language independent (even though it's written in Python), you should be able to compile regular expressions to work with other languages as well. To do that, you can simply import a sub-package, and they should work identically (though some languages may have more features than others):
+As of version 1.6.0, the concepts of *dialects* was introduced. Different languages often have slight variations on the regular expression syntax. As this library is meant to be language independent (even though it's written in Python), you should be able to compile regular expressions to work with other languages as well. To do that, you can simply import all the elements as a sub-package, and they should work identically, although some languages may not have the same features as others.
 ```python
 >>> import ezregex as er # The python dialect is the defualt dialect
->>> er.group(digit, 'name') + er.earlierGroup('name')
+>>> er.group(digit, 'name') + er.earlier_group('name')
 EZRegex("(?P<name>\d)(?P=name)")
 >>> import ezregex.perl as er
->>> er.group(digit, 'name') + er.earlierGroup('name')
+>>> er.group(digit, 'name') + er.earlier_group('name')
 EZRegex("?P<name>\d)(\g<name>")
 ```
+
 The currently implemented dialects are:
 - Python
     - Well tested, ~99% implemented
+- JavaScript
+    - Under active development, the basics *should* work, though tests aren't in place yet
 - Perl
-    - Almost identical to the Python dialect because I don't know Perl.
-
-If you know a particular flavor of regex and would like to contribute, feel free to make a pull request, or email me at smartycope@gmail.com
+    - Next on the roadmap, technically importable, but not implemented yet
 
+If you know a particular flavor of regex and would like to contribute, feel free to read the [developer documentation](#developer-documentation) and make a pull request! If you would like one that's not implemented yet, you can also add a [github issue](https://github.com/smartycope/ezregex/issues).
 
 ## Documentation
 ### Notes and Gotchas
-This documentation is for the Python dialect specifically, as it really is the only one currently implemented.
-- When using the re library, functions like search() and sub() don't accept EZRegexs as valid regex patterns. Be sure to call either .str() or .compile(), or cast to a string when passing to those. Also, be careful to call the function on the entire pattern: chunk + whitespace.str() is not the same as (chunk + whitespace).str().
-- In regular Regex, a lot of random things capture groups for no reason. I find this annoying. All regexes in EZRegex intentionally capture passively, so to capture any groups, use group(), with the optional `name` parameter.
+- The different Regular Expression dialects don't all have the same features, and those features don't all work the same way. I've tried to standardize these as best I can and use reasonable names for all the elements. If you're confused by something not working as expected, be sure to understand how your language specifically handles regular expressions.
+- When using the Python `re` library, functions like re.search() and re.sub() don't accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast it to a string) or .compile() (to compile to an re.Pattern) when passing to those. Also, be careful to call the function on the entire pattern: chunk + whitespace.str() is not the same as (chunk + whitespace).str().
+- In regular regex, a lot of random things capture groups for no apparent reason. All regexes in EZRegex intentionally capture passively, so to capture any groups, use group(), with the optional `name` parameter.
 - All EZRegexs (except for `raw`) auto-sanitize strings given to them, so there's no need to escape characters or use r strings. This *does* mean, however, that you cannot pass actual regex strings to any of them, as they'll think you're talking about it literally (unless you want that, of course). To include already written regex strings, use `raw`
 - Note that I have camelCase and snake_case versions of each of the functions, because I waver back and forth between which I like better. Both versions function identically.
-- The `input` parameter can accept strings, other EZRegexs, or entire sequences of EZRegex patterns.
-- A few of these have `greedy` and `possessive` optional parameters. They can be useful, but can get complicated. Refer to [the Python re docs](https://docs.python.org/3/library/re.html) for details.
+- The `InputType` can accept strings, other EZRegexs, or entire sequences of EZRegex patterns. It can also accept things that can be cast to a string, but it will warn you when it does, so it's better to cast to a string yourself.
+- The `invert` function can accept any regular expression, not just EZRegex expressions, if you want to use it independently of the rest of the library.
+
 <!-- Start of generated docs -->
 <details>
-	<summary>perl</summary><details style="padding-left: 20px;">
+	<summary><strong><u>perl</u></strong></summary><details>
 	<summary>Positionals</summary>
 
 #### These differentiate the *string* starting with a sequence, and a *line* starting with a sequence. Do note that the startof the string is also the start of a line. These can also be called without parameters to denote the start/end of astring/line without something specific having to be next to it.
 - string_starts_with
 - string_ends_with
 - line_starts_with
 - line_ends_with
 - word_boundary
 	- Matches the boundary of a word, i.e. the empty space between a word character and not a word character, or the end of a string
 - not_word_boundary
 	- The opposite of `wordBoundary`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Literals</summary>
 
-#### 
+####
 - tab
 - space
 - space_or_tab
 - new_line
 - carriage_return
 - quote
 	- Matches ', ", and `
@@ -211,28 +213,28 @@
 - form_feed
 - comma
 - period
 - underscore
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Not Literals</summary>
 
-#### 
+####
 - not_whitespace
 - not_digit
 - not_word
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Catagories</summary>
 
-#### 
+####
 - whitespace
 - whitechunk
 	- A "chunk" of whitespace. Just any amount of whitespace together
 - digit
 - number
 	- Matches multiple digits next to each other. Does not match negatives or decimals
 - word
@@ -253,130 +255,130 @@
 	- Matches a metadata ASCII characters
 - printable
 	- Matches printable ASCII characters
 - printable_and_space
 - alpha_num
 - unicode
 	- Matches a unicode character by name
-- any_between(char: str, and_char: str) 
+- any_between(char: str, and_char: str)
 	- Match any char between `char` and `and_char`, using the ASCII table for reference
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Amounts</summary>
 
-#### 
-- match_max(input: InputType) 
+####
+- match_max(input: InputType)
 	- Match as many of `input` in the string as you can. This is equivelent to using the unary + operator.
 If `input` is not provided, it works on the previous regex pattern. That's not recommended for
 clarity's sake though
-- match_num(num: int, input: InputType) 
+- match_num(num: int, input: InputType)
 	- Match `num` amount of `input` in the string
-- match_more_than(min: int, input: InputType) 
+- match_more_than(min: int, input: InputType)
 	- Match more than `min` sequences of `input` in the string
-- match_at_least(min: int, input: InputType) 
+- match_at_least(min: int, input: InputType)
 	- Match at least `min` sequences of `input` in the string
-- match_at_most(max: int, input: InputType) 
+- match_at_most(max: int, input: InputType)
 	- Match at most `max` instances of `input` in the string
-- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False) 
+- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match between `min` and `max` sequences of `input` in the string. This also accepts `greedy` and `possessive` parameters
 Max can be an empty string to indicate no maximum
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match at least one of `input` in the string. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match 0 or more sequences of `input`. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Choices</summary>
 
-#### 
-- optional(input: InputType, greedy: bool=True, possessive: bool=False) 
+####
+- optional(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match `input` if it's there. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- either(input: InputType, or_input: InputType) 
-- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None) 
+- either(input: InputType, or_input: InputType)
+- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None)
 	- Match any of the given `inputs`. Note that `inputs` can be multiple parameters,
 or a single string. Can also accept parameters chars and split. If char is set
 to True, then `inputs` must only be a single string, it interprets `inputs`
 as characters, and splits it up to find any of the chars in the string. If
 split is set to true, it forces the ?(...) regex syntax instead of the [...]
 syntax. It should act the same way, but your output regex will look different.
 By default, it just optimizes it for you.
-- any_char_except(*inputs: str) 
+- any_char_except(*inputs: str)
 	- This matches any char that is NOT in `inputs`. `inputs` can be multiple parameters, or a single string of chars to split.
-- any_except(input: InputType, type: InputType='.*') 
+- any_except(input: InputType, type: InputType='.*')
 	- Matches anything other than `input`, which must be a single string or EZRegex chain, **not** a list. Also
 optionally accepts the `type` parameter, which works like this: "Match any `type` other than `input`". For example,
 "match any word which is not foo". Do note that this function is new, and I'm still working out the kinks.
-- each(*inputs: InputType) 
+- each(*inputs: InputType)
 	- Matches if the next part of the string can match all of the given inputs. Like the + operator, but out of order.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Conditionals</summary>
 
 #### These can only be used once in a given expression. They only match a given expression if the expression is/ins'tfollowed/preceeded by a the given pattern
-- if_proceded_by(input: InputType) 
+- if_proceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming after it. Can only be used once in a given pattern,
 as it only applies to the end
-- if_not_proceded_by(input: InputType) 
+- if_not_proceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming after it. Can only be used once in
 a given pattern, as it only applies to the end
-- if_preceded_by(input: InputType) 
+- if_preceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming before it. Can only be used once in a given pattern,
 as it only applies to the beginning
-- if_not_preceded_by(input: InputType) 
+- if_not_preceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming before it. Can only be used once
 in a given pattern, as it only applies to the beginning
-- if_enclosed_with(open: str, stuff: InputType, close: str | None=None) 
+- if_enclosed_with(open: str, stuff: InputType, close: str | None=None)
 	- Matches if the string has `open`, then `stuff`, then `close`, but only "matches"
 stuff. Just a convenience combination of ifProceededBy and ifPreceededBy.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Grouping</summary>
 
-#### 
-- group(input: InputType, name: str | None=None) 
+####
+- group(input: InputType, name: str | None=None)
 	- Causes `input` to be captured as an unnamed group. Only useful when replacing regexs
-- passive_group(input: InputType) 
+- passive_group(input: InputType)
 	- As all regexs in EZRegex capture passively, this is entirely useless. But if you really want to, here it is
-- earlier_group(num_or_name: int | str) 
+- earlier_group(num_or_name: int | str)
 	- Matches whatever the group referenced by `num_or_name` matched earlier. Must be *after* a
 group which would match `num_or_name`
-- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None) 
-	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt` 
+- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None)
+	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Replacement</summary>
 
 #### In the intrest of "I don't want to think about any syntax at all", I have included replace members. Do note that theyare not interoperable with the other EZRegexs, and can only be used with other strings and each other.
-- rgroup(num_or_name: str | int) 
+- rgroup(num_or_name: str | int)
 	- Puts in its place the group specified, either by group number (for unnamed
 groups) or group name (for named groups). Named groups are also counted by
 number, I'm pretty sure. Groups are numbered starting from 1
 - replace_entire
 	- Puts in its place the entire match
 - replace(string: str, rtn_str: bool=True) -> str | EZRegex
 	- Generates a valid regex replacement string, using Python f-string like syntax.
@@ -393,30 +395,30 @@
 There's a few of advantages to using this instead of just the regular regex replacement syntax:
 - It's consistent between dialects
 - It's closer to Python f-string syntax, which is cleaner and more familiar
 - It handles numbered, named, and entire replacement types the same
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Misc</summary>
 
-#### 
-- is_exactly(input: InputType) 
+####
+- is_exactly(input: InputType)
 	- This matches the string if and only if the entire string is exactly equal to `input`
-- literal(input: InputType) 
+- literal(input: InputType)
 	- This is a redundant function. You should always be able to use `... + 'stuff'` just as easily as `... + literal('stuff')`
-- raw(regex: str) 
+- raw(regex: str)
 	- If you already have some regular regex written, and you want to incorperate
 it, this will allow you to include it without sanatizing all the backslaches
 and such, which all the other EZRegexs do automatically
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Premade</summary>
 
 #### These are some useful combinations that may be commonly used. They are not as stable, and may be changed and added to inlater versions to make them more accurate
 - literally_anything
 	- *Any* character, include newline
 - signed
 	- a signed number, including 123, -123, and +123
@@ -434,15 +436,15 @@
 - version
 	- The *official* regex for matching version numbers from https://semver.org/. It includes 5 groups that can bematched/replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata`
 - version_numbered
 	- Same as `version`, but it uses numbered groups for each version number instead of named groups
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Flags</summary>
 
 #### These shadow python regex flags, and can just as easily be specified directly to the re library instead. They're providedhere for compatibility with other regex dialects. See https://docs.python.org/3/library/re.html#flags for details
 - ASCII
 	- Make matching words, word boundaries, digits, and whitespace perform ASCII-only matching instead of full Unicodematching. This is only meaningful for Unicode (str) patterns, and is ignored for bytes patterns
 - IGNORECASE
 	- Perform case-insensitive matching, including expressions that explicitly use uppercase members. Full Unicode matching(such as Ü matching ü) also works unless the ASCII flag is used to disable non-ASCII matches. The current locale does notchange the effect of this flag unless the LOCALE flag is also used
@@ -455,33 +457,33 @@
 - UNICODE
 	- Match using the full unicode standard, instead of just ASCII. Enabled by default, and therefore redundant.
 
 </details>
 
 </details>
 <details>
-	<summary>python</summary><details style="padding-left: 20px;">
+	<summary><strong><u>javascript</u></strong></summary><details>
 	<summary>Positionals</summary>
 
 #### These differentiate the *string* starting with a sequence, and a *line* starting with a sequence. Do note that the startof the string is also the start of a line. These can also be called without parameters to denote the start/end of astring/line without something specific having to be next to it.
 - string_starts_with
 - string_ends_with
 - line_starts_with
 - line_ends_with
 - word_boundary
 	- Matches the boundary of a word, i.e. the empty space between a word character and not a word character, or the end of a string
 - not_word_boundary
 	- The opposite of `wordBoundary`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Literals</summary>
 
-#### 
+####
 - tab
 - space
 - space_or_tab
 - new_line
 - carriage_return
 - quote
 	- Matches ', ", and `
@@ -489,28 +491,28 @@
 - form_feed
 - comma
 - period
 - underscore
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Not Literals</summary>
 
-#### 
+####
 - not_whitespace
 - not_digit
 - not_word
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Catagories</summary>
 
-#### 
+####
 - whitespace
 - whitechunk
 	- A "chunk" of whitespace. Just any amount of whitespace together
 - digit
 - number
 	- Matches multiple digits next to each other. Does not match negatives or decimals
 - word
@@ -531,130 +533,130 @@
 	- Matches a metadata ASCII characters
 - printable
 	- Matches printable ASCII characters
 - printable_and_space
 - alpha_num
 - unicode
 	- Matches a unicode character by name
-- any_between(char: str, and_char: str) 
+- any_between(char: str, and_char: str)
 	- Match any char between `char` and `and_char`, using the ASCII table for reference
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Amounts</summary>
 
-#### 
-- match_max(input: InputType) 
+####
+- match_max(input: InputType)
 	- Match as many of `input` in the string as you can. This is equivelent to using the unary + operator.
 If `input` is not provided, it works on the previous regex pattern. That's not recommended for
 clarity's sake though
-- match_num(num: int, input: InputType) 
+- match_num(num: int, input: InputType)
 	- Match `num` amount of `input` in the string
-- match_more_than(min: int, input: InputType) 
+- match_more_than(min: int, input: InputType)
 	- Match more than `min` sequences of `input` in the string
-- match_at_least(min: int, input: InputType) 
+- match_at_least(min: int, input: InputType)
 	- Match at least `min` sequences of `input` in the string
-- match_at_most(max: int, input: InputType) 
+- match_at_most(max: int, input: InputType)
 	- Match at most `max` instances of `input` in the string
-- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False) 
+- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match between `min` and `max` sequences of `input` in the string. This also accepts `greedy` and `possessive` parameters
 Max can be an empty string to indicate no maximum
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match at least one of `input` in the string. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match 0 or more sequences of `input`. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Choices</summary>
 
-#### 
-- optional(input: InputType, greedy: bool=True, possessive: bool=False) 
+####
+- optional(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match `input` if it's there. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- either(input: InputType, or_input: InputType) 
-- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None) 
+- either(input: InputType, or_input: InputType)
+- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None)
 	- Match any of the given `inputs`. Note that `inputs` can be multiple parameters,
 or a single string. Can also accept parameters chars and split. If char is set
 to True, then `inputs` must only be a single string, it interprets `inputs`
 as characters, and splits it up to find any of the chars in the string. If
 split is set to true, it forces the ?(...) regex syntax instead of the [...]
 syntax. It should act the same way, but your output regex will look different.
 By default, it just optimizes it for you.
-- any_char_except(*inputs: str) 
+- any_char_except(*inputs: str)
 	- This matches any char that is NOT in `inputs`. `inputs` can be multiple parameters, or a single string of chars to split.
-- any_except(input: InputType, type: InputType='.*') 
+- any_except(input: InputType, type: InputType='.*')
 	- Matches anything other than `input`, which must be a single string or EZRegex chain, **not** a list. Also
 optionally accepts the `type` parameter, which works like this: "Match any `type` other than `input`". For example,
 "match any word which is not foo". Do note that this function is new, and I'm still working out the kinks.
-- each(*inputs: InputType) 
+- each(*inputs: InputType)
 	- Matches if the next part of the string can match all of the given inputs. Like the + operator, but out of order.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Conditionals</summary>
 
 #### These can only be used once in a given expression. They only match a given expression if the expression is/ins'tfollowed/preceeded by a the given pattern
-- if_proceded_by(input: InputType) 
+- if_proceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming after it. Can only be used once in a given pattern,
 as it only applies to the end
-- if_not_proceded_by(input: InputType) 
+- if_not_proceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming after it. Can only be used once in
 a given pattern, as it only applies to the end
-- if_preceded_by(input: InputType) 
+- if_preceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming before it. Can only be used once in a given pattern,
 as it only applies to the beginning
-- if_not_preceded_by(input: InputType) 
+- if_not_preceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming before it. Can only be used once
 in a given pattern, as it only applies to the beginning
-- if_enclosed_with(open: str, stuff: InputType, close: str | None=None) 
+- if_enclosed_with(open: str, stuff: InputType, close: str | None=None)
 	- Matches if the string has `open`, then `stuff`, then `close`, but only "matches"
 stuff. Just a convenience combination of ifProceededBy and ifPreceededBy.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Grouping</summary>
 
-#### 
-- group(input: InputType, name: str | None=None) 
+####
+- group(input: InputType, name: str | None=None)
 	- Causes `input` to be captured as an unnamed group. Only useful when replacing regexs
-- passive_group(input: InputType) 
+- passive_group(input: InputType)
 	- As all regexs in EZRegex capture passively, this is entirely useless. But if you really want to, here it is
-- earlier_group(num_or_name: int | str) 
+- earlier_group(num_or_name: int | str)
 	- Matches whatever the group referenced by `num_or_name` matched earlier. Must be *after* a
 group which would match `num_or_name`
-- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None) 
-	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt` 
+- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None)
+	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Replacement</summary>
 
 #### In the intrest of "I don't want to think about any syntax at all", I have included replace members. Do note that theyare not interoperable with the other EZRegexs, and can only be used with other strings and each other.
-- rgroup(num_or_name: str | int) 
+- rgroup(num_or_name: str | int)
 	- Puts in its place the group specified, either by group number (for unnamed
 groups) or group name (for named groups). Named groups are also counted by
 number, I'm pretty sure. Groups are numbered starting from 1
 - replace_entire
 	- Puts in its place the entire match
 - replace(string: str, rtn_str: bool=True) -> str | EZRegex
 	- Generates a valid regex replacement string, using Python f-string like syntax.
@@ -671,30 +673,30 @@
 There's a few of advantages to using this instead of just the regular regex replacement syntax:
 - It's consistent between dialects
 - It's closer to Python f-string syntax, which is cleaner and more familiar
 - It handles numbered, named, and entire replacement types the same
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Misc</summary>
 
-#### 
-- is_exactly(input: InputType) 
+####
+- is_exactly(input: InputType)
 	- This matches the string if and only if the entire string is exactly equal to `input`
-- literal(input: InputType) 
+- literal(input: InputType)
 	- This is a redundant function. You should always be able to use `... + 'stuff'` just as easily as `... + literal('stuff')`
-- raw(regex: str) 
+- raw(regex: str)
 	- If you already have some regular regex written, and you want to incorperate
 it, this will allow you to include it without sanatizing all the backslaches
 and such, which all the other EZRegexs do automatically
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Premade</summary>
 
 #### These are some useful combinations that may be commonly used. They are not as stable, and may be changed and added to inlater versions to make them more accurate
 - literally_anything
 	- *Any* character, include newline
 - signed
 	- a signed number, including 123, -123, and +123
@@ -712,52 +714,54 @@
 - version
 	- The *official* regex for matching version numbers from https://semver.org/. It includes 5 groups that can bematched/replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata`
 - version_numbered
 	- Same as `version`, but it uses numbered groups for each version number instead of named groups
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Flags</summary>
 
 #### These shadow python regex flags, and can just as easily be specified directly to the re library instead. They're providedhere for compatibility with other regex dialects. See https://docs.python.org/3/library/re.html#flags for details
 - ASCII
 	- Make matching words, word boundaries, digits, and whitespace perform ASCII-only matching instead of full Unicodematching. This is only meaningful for Unicode (str) patterns, and is ignored for bytes patterns
 - IGNORECASE
 	- Perform case-insensitive matching, including expressions that explicitly use uppercase members. Full Unicode matching(such as Ü matching ü) also works unless the ASCII flag is used to disable non-ASCII matches. The current locale does notchange the effect of this flag unless the LOCALE flag is also used
 - DOTALL
 	- Make the '.' special character match any character at all, including a newline. It's recommended you simply useliterally_anything instead
 - LOCALE
 	- Try not to use this, and rely on unicode matching instead
 - MULTILINE
 	- This is automatically inserted when using line_start and line_end, you shouldn't need to add it manually
+- UNICODE
+	- Match using the full unicode standard, instead of just ASCII. Enabled by default, and therefore redundant.
 
 </details>
 
 </details>
 <details>
-	<summary>javascript</summary><details style="padding-left: 20px;">
+	<summary><strong><u>python</u></strong></summary><details>
 	<summary>Positionals</summary>
 
 #### These differentiate the *string* starting with a sequence, and a *line* starting with a sequence. Do note that the startof the string is also the start of a line. These can also be called without parameters to denote the start/end of astring/line without something specific having to be next to it.
 - string_starts_with
 - string_ends_with
 - line_starts_with
 - line_ends_with
 - word_boundary
 	- Matches the boundary of a word, i.e. the empty space between a word character and not a word character, or the end of a string
 - not_word_boundary
 	- The opposite of `wordBoundary`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Literals</summary>
 
-#### 
+####
 - tab
 - space
 - space_or_tab
 - new_line
 - carriage_return
 - quote
 	- Matches ', ", and `
@@ -765,28 +769,28 @@
 - form_feed
 - comma
 - period
 - underscore
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Not Literals</summary>
 
-#### 
+####
 - not_whitespace
 - not_digit
 - not_word
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Catagories</summary>
 
-#### 
+####
 - whitespace
 - whitechunk
 	- A "chunk" of whitespace. Just any amount of whitespace together
 - digit
 - number
 	- Matches multiple digits next to each other. Does not match negatives or decimals
 - word
@@ -807,130 +811,130 @@
 	- Matches a metadata ASCII characters
 - printable
 	- Matches printable ASCII characters
 - printable_and_space
 - alpha_num
 - unicode
 	- Matches a unicode character by name
-- any_between(char: str, and_char: str) 
+- any_between(char: str, and_char: str)
 	- Match any char between `char` and `and_char`, using the ASCII table for reference
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Amounts</summary>
 
-#### 
-- match_max(input: InputType) 
+####
+- match_max(input: InputType)
 	- Match as many of `input` in the string as you can. This is equivelent to using the unary + operator.
 If `input` is not provided, it works on the previous regex pattern. That's not recommended for
 clarity's sake though
-- match_num(num: int, input: InputType) 
+- match_num(num: int, input: InputType)
 	- Match `num` amount of `input` in the string
-- match_more_than(min: int, input: InputType) 
+- match_more_than(min: int, input: InputType)
 	- Match more than `min` sequences of `input` in the string
-- match_at_least(min: int, input: InputType) 
+- match_at_least(min: int, input: InputType)
 	- Match at least `min` sequences of `input` in the string
-- match_at_most(max: int, input: InputType) 
+- match_at_most(max: int, input: InputType)
 	- Match at most `max` instances of `input` in the string
-- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False) 
+- match_range(min: int, max: int, input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match between `min` and `max` sequences of `input` in the string. This also accepts `greedy` and `possessive` parameters
 Max can be an empty string to indicate no maximum
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_one(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match at least one of `input` in the string. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False) 
+- at_least_none(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match 0 or more sequences of `input`. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Choices</summary>
 
-#### 
-- optional(input: InputType, greedy: bool=True, possessive: bool=False) 
+####
+- optional(input: InputType, greedy: bool=True, possessive: bool=False)
 	- Match `input` if it's there. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible
 non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions
 see https://docs.python.org/3/library/re.html for more help
-- either(input: InputType, or_input: InputType) 
-- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None) 
+- either(input: InputType, or_input: InputType)
+- any_of(*inputs: str, chars: bool | None=None, split: bool | None=None)
 	- Match any of the given `inputs`. Note that `inputs` can be multiple parameters,
 or a single string. Can also accept parameters chars and split. If char is set
 to True, then `inputs` must only be a single string, it interprets `inputs`
 as characters, and splits it up to find any of the chars in the string. If
 split is set to true, it forces the ?(...) regex syntax instead of the [...]
 syntax. It should act the same way, but your output regex will look different.
 By default, it just optimizes it for you.
-- any_char_except(*inputs: str) 
+- any_char_except(*inputs: str)
 	- This matches any char that is NOT in `inputs`. `inputs` can be multiple parameters, or a single string of chars to split.
-- any_except(input: InputType, type: InputType='.*') 
+- any_except(input: InputType, type: InputType='.*')
 	- Matches anything other than `input`, which must be a single string or EZRegex chain, **not** a list. Also
 optionally accepts the `type` parameter, which works like this: "Match any `type` other than `input`". For example,
 "match any word which is not foo". Do note that this function is new, and I'm still working out the kinks.
-- each(*inputs: InputType) 
+- each(*inputs: InputType)
 	- Matches if the next part of the string can match all of the given inputs. Like the + operator, but out of order.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Conditionals</summary>
 
 #### These can only be used once in a given expression. They only match a given expression if the expression is/ins'tfollowed/preceeded by a the given pattern
-- if_proceded_by(input: InputType) 
+- if_proceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming after it. Can only be used once in a given pattern,
 as it only applies to the end
-- if_not_proceded_by(input: InputType) 
+- if_not_proceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming after it. Can only be used once in
 a given pattern, as it only applies to the end
-- if_preceded_by(input: InputType) 
+- if_preceded_by(input: InputType)
 	- Matches the pattern if it has `input` coming before it. Can only be used once in a given pattern,
 as it only applies to the beginning
-- if_not_preceded_by(input: InputType) 
+- if_not_preceded_by(input: InputType)
 	- Matches the pattern if it does **not** have `input` coming before it. Can only be used once
 in a given pattern, as it only applies to the beginning
-- if_enclosed_with(open: str, stuff: InputType, close: str | None=None) 
+- if_enclosed_with(open: str, stuff: InputType, close: str | None=None)
 	- Matches if the string has `open`, then `stuff`, then `close`, but only "matches"
 stuff. Just a convenience combination of ifProceededBy and ifPreceededBy.
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Grouping</summary>
 
-#### 
-- group(input: InputType, name: str | None=None) 
+####
+- group(input: InputType, name: str | None=None)
 	- Causes `input` to be captured as an unnamed group. Only useful when replacing regexs
-- passive_group(input: InputType) 
+- passive_group(input: InputType)
 	- As all regexs in EZRegex capture passively, this is entirely useless. But if you really want to, here it is
-- earlier_group(num_or_name: int | str) 
+- earlier_group(num_or_name: int | str)
 	- Matches whatever the group referenced by `num_or_name` matched earlier. Must be *after* a
 group which would match `num_or_name`
-- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None) 
-	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt` 
+- if_exists(num_or_name: int | str, does: InputType, doesnt: InputType | None=None)
+	- Matches `does` if the group `num_or_name` exists, otherwise it matches `doesnt`
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Replacement</summary>
 
 #### In the intrest of "I don't want to think about any syntax at all", I have included replace members. Do note that theyare not interoperable with the other EZRegexs, and can only be used with other strings and each other.
-- rgroup(num_or_name: str | int) 
+- rgroup(num_or_name: str | int)
 	- Puts in its place the group specified, either by group number (for unnamed
 groups) or group name (for named groups). Named groups are also counted by
 number, I'm pretty sure. Groups are numbered starting from 1
 - replace_entire
 	- Puts in its place the entire match
 - replace(string: str, rtn_str: bool=True) -> str | EZRegex
 	- Generates a valid regex replacement string, using Python f-string like syntax.
@@ -947,30 +951,30 @@
 There's a few of advantages to using this instead of just the regular regex replacement syntax:
 - It's consistent between dialects
 - It's closer to Python f-string syntax, which is cleaner and more familiar
 - It handles numbered, named, and entire replacement types the same
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Misc</summary>
 
-#### 
-- is_exactly(input: InputType) 
+####
+- is_exactly(input: InputType)
 	- This matches the string if and only if the entire string is exactly equal to `input`
-- literal(input: InputType) 
+- literal(input: InputType)
 	- This is a redundant function. You should always be able to use `... + 'stuff'` just as easily as `... + literal('stuff')`
-- raw(regex: str) 
+- raw(regex: str)
 	- If you already have some regular regex written, and you want to incorperate
 it, this will allow you to include it without sanatizing all the backslaches
 and such, which all the other EZRegexs do automatically
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Premade</summary>
 
 #### These are some useful combinations that may be commonly used. They are not as stable, and may be changed and added to inlater versions to make them more accurate
 - literally_anything
 	- *Any* character, include newline
 - signed
 	- a signed number, including 123, -123, and +123
@@ -988,64 +992,93 @@
 - version
 	- The *official* regex for matching version numbers from https://semver.org/. It includes 5 groups that can bematched/replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata`
 - version_numbered
 	- Same as `version`, but it uses numbered groups for each version number instead of named groups
 
 </details>
 
-<details style="padding-left: 20px;">
+<details>
 	<summary>Flags</summary>
 
 #### These shadow python regex flags, and can just as easily be specified directly to the re library instead. They're providedhere for compatibility with other regex dialects. See https://docs.python.org/3/library/re.html#flags for details
 - ASCII
 	- Make matching words, word boundaries, digits, and whitespace perform ASCII-only matching instead of full Unicodematching. This is only meaningful for Unicode (str) patterns, and is ignored for bytes patterns
 - IGNORECASE
 	- Perform case-insensitive matching, including expressions that explicitly use uppercase members. Full Unicode matching(such as Ü matching ü) also works unless the ASCII flag is used to disable non-ASCII matches. The current locale does notchange the effect of this flag unless the LOCALE flag is also used
 - DOTALL
 	- Make the '.' special character match any character at all, including a newline. It's recommended you simply useliterally_anything instead
 - LOCALE
 	- Try not to use this, and rely on unicode matching instead
 - MULTILINE
 	- This is automatically inserted when using line_start and line_end, you shouldn't need to add it manually
-- UNICODE
-	- Match using the full unicode standard, instead of just ASCII. Enabled by default, and therefore redundant.
 
 </details>
 
 </details>
 <!-- End of generated docs -->
 <details>
 <summary>Operators</summary>
 
 - `+`, `<<`, `>>`
 	- These all do the same thing: combine expressions
 - `*`
-	- Multiplies an expression a number of times. `expr * 3` is equivelent to `expr + expr + expr`. Can also be used like `expr * ...` is equivalent to `anyAmt(expr)`
+	- Multiplies an expression a number of times. `expr * 3` is equivelent to `expr + expr + expr`. Can also be used like `expr * ...` is equivalent to `any_amt(expr)`
 - `+`
 	- A unary + operator acts exactly as a match_max() does, or, if you're familiar with regex syntax, the + operator
 - `[]`
 	- expr[2, 3] is equivalent to `match_range(2, 3, expr)`
 	- expr[2, ...] or expr[2,] is equivalent to `at_least(2, expr)`
 	- expr[... , 2] is equivalent to `at_most(2, expr)`
 	- expr[...] or expr[0, ...] is equivelent to `at_least_0(expr)`
 	- expr[1, ...] is equivalent to `at_least_1(expr)`
 - `&`
 	- Coming soon! This will work like the + operator, but they can be out of order. Like an and operation.
 - `|`
-	- Coming soon! This will work like an or operation, which will work just like anyOf()
+	- Coming soon! This will work like an or operation, which will work just like any_of()
 - `%`
     - This automatically calls re.search() for you and returns the match object (or None). Use like this: `(digit * 2) % '99 beers on the wall'`
 - `~`
-    - This inverts the expression. This is equivalent to calling the .invert() method
+    - This inverts the expression, equivalent to calling the .invert() method
 </details>
 
-## Explanation of How it Works
-Everything relies on the EZRegex class. In the elements.py file of each dialect, I have defined a ton of pre-made EZRegexs which mimic all (or at least as many as I can) fundamental parts of the regex syntax, plus a few others which are common combinations (like chunk or optional(whitechunk)). Any of them which have parameters are wrapped in functions to provide proper typing & linting. They all are either EZRegexs or are functions which return EZRegexs. These have operators overloaded so you can combine them in intuitive ways and call them by intuitive names. All the functions passed to EZRegex take a function parameter (or a string which gets converted to a function for convenience), which gets called with the current regex expression and any parameters passed along when the instance gets called with the () operator. That way you can add things to the front or back of an expression for example, and you can change what exactly gets added to the current expression based on other parameters. You can also chain strings together, and pass them as parameters to other EZRegexs, which auto-compiles them and adds them appropriately.
+## Developer Documentation
+### The EZRegex class
+Everything relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as each dialect defines their own EZRegex elements specific to that dialect (more on that later). Each element represents a fundamental part of the Regular Expression syntax for that language, as well as less-fundemental common combinations for convenience (like email and float).
+
+EZRegex can accept a string or a function to define how it's supposed to interact with the current "chain" of elements. If it's a string, it just adds it to the end. If it's a function, it can accept any positional or named parameters, but has to accept `cur=...` as the last parameter (it's complicated). The `cur` parameter is the current regular expression chain, as a string. What's returned becomes the new `cur` parameter of the next element, or, if there is no next element, the final regex. That way you can add to the front or back of an expression, and you can change what exactly gets added to the current expression based on other parameters.
+
+The EZRegex class has operators overloaded so you can combine them in intuitive ways and call them by intuitive names.
+
+### Typing & Linting
+The updated method of doing this is to define all the EZRegex elements of a dialect in `elements.py`, and then add type hints and doc strings in the `elements.pyi` file. EZRegex elements that accept parameters are typed as functions (even though they're not), for both convenience for the user when using linter, and to give documentation in an easier way. EZRegex elements that don't accept parameters should be typed as EZRegex, and given documentation as a string on the line below it. This is *slightly* non-standard, but linters support it, as well as my documentation generator script, which parses the .pyi files. The elements can also be seperated into groups in the .pyi files by using `"Group: \<group name\>\n\<group description\>"`, which also gets parsed by the documentation script. The groups aren't used in the actual library, but are helpful in seperating the documentation, as well as used in [ezregex.org](http://ezregex.org)
+
+### Dialects
+Because most regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but it works a bit differently. It has an `elements.py` file, but it defines all the elements as a dict in the form of {"element_name": {"keyword": "arguements"}}. It then has a `load_dialect()` function, which is the only thing importable from it. The reason it's done this way is because `dialect` is a required parameter of the EZRegex constructor, so `load_dialect()` takes a `dialect` parameter, and constructs the base elements from it's dict and returns a new dict of initialized elements to be dumped into the global scope of the dialect. The `elements.py` file of a specific dialect can then remove any elements that it doesn't support (using the `del` keyword) and add/overwrite any it does support.
 
-I also have everything which could capture a group capture it passively, except for actual group operators, and always have the (?m) (multiline) flag automatically asserted whenever lineStart/lineEnd are used so as to differentiate between capturing at the beginning/end of a string and the beginning/end of a line.
+### Inverting
+There's actually 2 algorithms implemented for "inverting" regexs. The old algorithm regexs the regexs in a specific order to replace parts one at a time. This is just as nasty and horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I actually got it to work decently well.
+
+Later, when I was reading up on abstract syntax trees, and scrolling around on PyPi, I realized that Python has one built in, and that it's available to use. I reimplemented the whole algorithm to instead parse the AST given by the built-in re lexer, and wrote my own parser on top of it, which works *much* better.
+
+Along the way, I also discovered, deep in the corners of the internet, 2 other Python libraries which do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger` technically works, however it tends to include unprintable characters, so it's output isn't very readable. `sre_yeild` is better, but it can be very slow, and is not quite the use case I'm going for. My invert algorithm is meant to be a debugging tool (though it doubles well for a testing tool), so it does things like detecting words (as opposed to seperate word characters) and inserts actual words, and doing the same for numbers and inserting `12345...`, as well as a couple other enhancements.
+
+### Tests
+Tests for a while now have just been in a single `tests.py` file, which was a giant pile of all the tests. I'm currently moving to use pytest. There's a `regexs.json` file (and a `replacements.json` file) that have a bunch of regexs, along with things they're supposed to match, and things they're not supposed to match, for testing.
+
+## Installation
+EZRegex is distributed on [PyPI](https://pypi.org) as a universal wheel and is available on Linux, macOS and Windows and supports Python 3.10+ and PyPy.
+
+```bash
+pip install ezregex
+```
+
+The import name is the same as the package name:
+```python
+import ezregex as er
+```
 
 ## Todo
-See [the todo](todo.txt).
-Eventually, I would like to move the todo to GitHub issues.
+See [the todo](todo.txt). I'm slowly moving these to [GitHub issues](https://github.com/smartycope/ezregex/issues), but for now, they're mostly still there
+
 
 ## License
 EZRegex is distributed under the [MIT License](https://choosealicense.com/licenses/mit)
```

#### html2text {}

```diff
@@ -1,136 +1,145 @@
-Metadata-Version: 2.3 Name: ezregex Version: 1.9.3 Summary: A readable and
+Metadata-Version: 2.3 Name: ezregex Version: 1.9.4 Summary: A readable and
 intuitive way to generate Regular Expressions Project-URL: Documentation,
-https://github.com/smartycope/ezregex#readme Project-URL: Issues, https://
-github.com/smartycope/ezregex/issues Project-URL: Source, https://github.com/
-smartycope/ezregex Project-URL: Official Website, https://ezregex.org Author-
-email: Copeland Carter
+https://github.com/smartycope/ezregex?tab=readme-ov-file#documentation Project-
+URL: Issues, https://github.com/smartycope/ezregex/issues Project-URL: Source,
+https://github.com/smartycope/ezregex Project-URL: Official Website, https://
+ezregex.org Author-email: Copeland Carter
 gmail.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
 Python: >=3.10 Description-Content-Type: text/markdown
                        [https://ezregex.org/favicon.png]
+
    _[_U_n_i_t_ _T_e_s_t_s_]_[_P_y_P_I_ _L_a_t_e_s_t_ _R_e_l_e_a_s_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/
-_s_m_a_r_t_y_c_o_p_e_/_e_z_r_e_g_e_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_i_m_p_l_e_m_e_n_t_a_t_i_o_n_/_e_z_r_e_g_e_x_]_[_h_t_t_p_s_:_/
-                     _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_f_o_r_m_a_t_/_e_z_r_e_g_e_x_]
+     _s_m_a_r_t_y_c_o_p_e_/_e_z_r_e_g_e_x_][https://img.shields.io/badge/dependencies-0-blue]
+     [https://img.shields.io/badge/Supported%20Dialects-3-green][https://
+  img.shields.io/badge/Python%20Dialect-100%25-blue][https://img.shields.io/
+    badge/JavaScript%20Dialect-50%25-yellow][https://img.shields.io/badge/
+                           Perl%20Dialect-20%25-red]
 # EZRegex A readable and intuitive way to make Regular Expressions without
-having to know any of the syntax Try my new frontend for this library at
+having to know any of the syntax Try the frontend for this library at
 [ezregex.org](https://ezregex.org/)! TLDR: This is to regular expressions what
-CMake is to makefiles **Table of Contents** * [Usage](#usage) * [Installation]
-(#installation) * [Invert](#inverting) * [Generate](#generation) * [Dialects]
-(#dialects) * [Documentation](#documentation) * [Explanation](#explanation-of-
-how-it-works) * [Todo](#todo) * [License](#license) ## Usage Quickstart
-```python from ezregex import * 'foo' + number + optional(whitespace) + word #
-Matches `foo123abc` and `foo123 abc` # but not `abc123foo` or `foo bar` ```
-Importing as a named package is recommended ```python import ezregex as er # ow
-is part of er already as optional whitespace params = er.group(er.atLeastNone
-(er.ow + er.word + er.ow + er.optional(',') + er.ow)) function = er.word +
-er.ow + '(' + params + ')' # Automatically calls the re.search() function for
-you function % 'some string containing func( param1 , param2)' # The test()
-method is helpful for debugging, and color codes groups for you function.test
-('this should match func(param1,\tparam2 ), foo(), and bar( foo,)') ``` .test()
-will print all the matches, color coded to match and group (not shown here):
-```
+CMake is to makefiles ### **Table of Contents** * [Usage](#usage) * [Invert]
+(#inverting) * [Generate](#generation) * [Dialects](#dialects) *
+[Documentation](#documentation) * [Developer Docs](#developer-documentation) *
+[Installation](#installation) * [Todo](#todo) * [License](#license) ## Usage
+Quickstart ```python from ezregex import * 'foo' + number + optional
+(whitespace) + word # Matches `foo123abc` and `foo123 abc` # but not
+`abc123foo` or `foo bar` ``` Importing as a named package is recommended
+```python import ezregex as er # ow is part of er already as optional
+whitespace params = er.group(er.atLeastNone(er.ow + er.word + er.ow +
+er.optional(',') + er.ow)) # Seperate parts as variables for cleaner patterns
+function = er.word + er.ow + '(' + params + ')' # Automatically calls the
+re.search() function for you function % 'some string containing func( param1 ,
+param2)' # The test() method is helpful for debugging, and color codes groups
+for you function.test('this should match func(param1,\tparam2 ), foo(), and bar
+( foo,)') ``` .test() will print all the matches, color coded to match and
+group (colors not shown here): ```
 â­âââââââââââââââââââââââââââââ
 Testing Regex
 âââââââââââââââââââââââââââââââ®
 â Testing expression: â â \w+(?:\s+)?\(((?:(?:\s+)?\w+(?:\s+)?,?(?:
 \s+)?)*)\) â â for matches in: â â this should match func(param1,
 param2 ), foo(), and bar( foo,) â â â â Match = "func(param1, param2 )"
 (18:39) â â Unnamed Groups: â â 1: "param1, param2 " (23:38) â â
 â â Match = "foo()" (41:46) â â Unnamed Groups: â â 1: "" (45:45)
 â â â â Match = "bar( foo,)" (52:62) â â Unnamed Groups: â â 1:
 " foo," (56:61) â â â â â
 â°âââââââââââââââââââââââââââââââââ
 Found
 ââââââââââââââââââââââââââââââââââ¯
-``` ## Installation EZRegex is distributed on [PyPI](https://pypi.org) as a
-universal wheel and is available on Linux, macOS and Windows and supports
-Python 3.10+ and PyPy. ```bash $ pip install ezregex ``` The import name is the
-same as the package name: ```python import ezregex as er ``` ## Inverting The
-`invert` function provided (available as er.invert(`expression`),
+``` ## Inverting The `invert` function (available as er.invert(`expression`),
 `expression`.invert(), or ~`expression`) is useful for debugging. You pass it
 an expression, and it returns an example of a string that is guaranteed to
 match the provided expression. ## Generation In version 1.7.0 we introduced a
 new function: `generate_regex`. It takes in 2 sets of strings, and returns a
 regular expression that will match everything in the first set and nothing in
 the second set. It may be a bit crude, but it can be a good starting point if
 you don't know where to start. It's also really good at [regex golf](http://
 regex.alf.nu/). ## Dialects As of version 1.6.0, the concepts of *dialects* was
 introduced. Different languages often have slight variations on the regular
 expression syntax. As this library is meant to be language independent (even
 though it's written in Python), you should be able to compile regular
 expressions to work with other languages as well. To do that, you can simply
-import a sub-package, and they should work identically (though some languages
-may have more features than others): ```python >>> import ezregex as er # The
-python dialect is the defualt dialect >>> er.group(digit, 'name') +
-er.earlierGroup('name') EZRegex("(?P\d)(?P=name)") >>> import ezregex.perl as
-er >>> er.group(digit, 'name') + er.earlierGroup('name') EZRegex("?P\d)(\g")
-``` The currently implemented dialects are: - Python - Well tested, ~99%
-implemented - Perl - Almost identical to the Python dialect because I don't
-know Perl. If you know a particular flavor of regex and would like to
-contribute, feel free to make a pull request, or email me at
-smartycope@gmail.com ## Documentation ### Notes and Gotchas This documentation
-is for the Python dialect specifically, as it really is the only one currently
-implemented. - When using the re library, functions like search() and sub()
-don't accept EZRegexs as valid regex patterns. Be sure to call either .str() or
-.compile(), or cast to a string when passing to those. Also, be careful to call
-the function on the entire pattern: chunk + whitespace.str() is not the same as
-(chunk + whitespace).str(). - In regular Regex, a lot of random things capture
-groups for no reason. I find this annoying. All regexes in EZRegex
-intentionally capture passively, so to capture any groups, use group(), with
-the optional `name` parameter. - All EZRegexs (except for `raw`) auto-sanitize
-strings given to them, so there's no need to escape characters or use r
-strings. This *does* mean, however, that you cannot pass actual regex strings
-to any of them, as they'll think you're talking about it literally (unless you
-want that, of course). To include already written regex strings, use `raw` -
-Note that I have camelCase and snake_case versions of each of the functions,
-because I waver back and forth between which I like better. Both versions
-function identically. - The `input` parameter can accept strings, other
-EZRegexs, or entire sequences of EZRegex patterns. - A few of these have
-`greedy` and `possessive` optional parameters. They can be useful, but can get
-complicated. Refer to [the Python re docs](https://docs.python.org/3/library/
-re.html) for details. perl Positionals #### These differentiate the *string*
-starting with a sequence, and a *line* starting with a sequence. Do note that
-the startof the string is also the start of a line. These can also be called
-without parameters to denote the start/end of astring/line without something
-specific having to be next to it. - string_starts_with - string_ends_with -
-line_starts_with - line_ends_with - word_boundary - Matches the boundary of a
-word, i.e. the empty space between a word character and not a word character,
-or the end of a string - not_word_boundary - The opposite of `wordBoundary`
-Literals #### - tab - space - space_or_tab - new_line - carriage_return - quote
-- Matches ', ", and ` - vertical_tab - form_feed - comma - period - underscore
-Not Literals #### - not_whitespace - not_digit - not_word Catagories #### -
-whitespace - whitechunk - A "chunk" of whitespace. Just any amount of
-whitespace together - digit - number - Matches multiple digits next to each
-other. Does not match negatives or decimals - word - word_char - Matches just a
-single "word character", defined as any letter, number, or _ - anything -
-Matches any single character, except a newline. To also match a newline, use
-literally_anything - chunk - A "chunk": Any clump of characters up until the
-next newline - uppercase - lowercase - letter - Matches just a letter -- not
-numbers or _ like word_char - hex_digit - oct_digit - punctuation - controller
-- Matches a metadata ASCII characters - printable - Matches printable ASCII
-characters - printable_and_space - alpha_num - unicode - Matches a unicode
-character by name - any_between(char: str, and_char: str) - Match any char
-between `char` and `and_char`, using the ASCII table for reference Amounts ####
-- match_max(input: InputType) - Match as many of `input` in the string as you
-can. This is equivelent to using the unary + operator. If `input` is not
-provided, it works on the previous regex pattern. That's not recommended for
-clarity's sake though - match_num(num: int, input: InputType) - Match `num`
-amount of `input` in the string - match_more_than(min: int, input: InputType) -
-Match more than `min` sequences of `input` in the string - match_at_least(min:
-int, input: InputType) - Match at least `min` sequences of `input` in the
-string - match_at_most(max: int, input: InputType) - Match at most `max`
-instances of `input` in the string - match_range(min: int, max: int, input:
-InputType, greedy: bool=True, possessive: bool=False) - Match between `min` and
-`max` sequences of `input` in the string. This also accepts `greedy` and
-`possessive` parameters Max can be an empty string to indicate no maximum
+import all the elements as a sub-package, and they should work identically,
+although some languages may not have the same features as others. ```python >>>
+import ezregex as er # The python dialect is the defualt dialect >>> er.group
+(digit, 'name') + er.earlier_group('name') EZRegex("(?P\d)(?P=name)") >>>
+import ezregex.perl as er >>> er.group(digit, 'name') + er.earlier_group
+('name') EZRegex("?P\d)(\g") ``` The currently implemented dialects are: -
+Python - Well tested, ~99% implemented - JavaScript - Under active development,
+the basics *should* work, though tests aren't in place yet - Perl - Next on the
+roadmap, technically importable, but not implemented yet If you know a
+particular flavor of regex and would like to contribute, feel free to read the
+[developer documentation](#developer-documentation) and make a pull request! If
+you would like one that's not implemented yet, you can also add a [github
+issue](https://github.com/smartycope/ezregex/issues). ## Documentation ###
+Notes and Gotchas - The different Regular Expression dialects don't all have
+the same features, and those features don't all work the same way. I've tried
+to standardize these as best I can and use reasonable names for all the
+elements. If you're confused by something not working as expected, be sure to
+understand how your language specifically handles regular expressions. - When
+using the Python `re` library, functions like re.search() and re.sub() don't
+accept EZRegex patterns as valid regex. Be sure to either call .str() (or cast
+it to a string) or .compile() (to compile to an re.Pattern) when passing to
+those. Also, be careful to call the function on the entire pattern: chunk +
+whitespace.str() is not the same as (chunk + whitespace).str(). - In regular
+regex, a lot of random things capture groups for no apparent reason. All
+regexes in EZRegex intentionally capture passively, so to capture any groups,
+use group(), with the optional `name` parameter. - All EZRegexs (except for
+`raw`) auto-sanitize strings given to them, so there's no need to escape
+characters or use r strings. This *does* mean, however, that you cannot pass
+actual regex strings to any of them, as they'll think you're talking about it
+literally (unless you want that, of course). To include already written regex
+strings, use `raw` - Note that I have camelCase and snake_case versions of each
+of the functions, because I waver back and forth between which I like better.
+Both versions function identically. - The `InputType` can accept strings, other
+EZRegexs, or entire sequences of EZRegex patterns. It can also accept things
+that can be cast to a string, but it will warn you when it does, so it's better
+to cast to a string yourself. - The `invert` function can accept any regular
+expression, not just EZRegex expressions, if you want to use it independently
+of the rest of the library. _pp_ee_rr_ll Positionals #### These differentiate the
+*string* starting with a sequence, and a *line* starting with a sequence. Do
+note that the startof the string is also the start of a line. These can also be
+called without parameters to denote the start/end of astring/line without
+something specific having to be next to it. - string_starts_with -
+string_ends_with - line_starts_with - line_ends_with - word_boundary - Matches
+the boundary of a word, i.e. the empty space between a word character and not a
+word character, or the end of a string - not_word_boundary - The opposite of
+`wordBoundary` Literals #### - tab - space - space_or_tab - new_line -
+carriage_return - quote - Matches ', ", and ` - vertical_tab - form_feed -
+comma - period - underscore Not Literals #### - not_whitespace - not_digit -
+not_word Catagories #### - whitespace - whitechunk - A "chunk" of whitespace.
+Just any amount of whitespace together - digit - number - Matches multiple
+digits next to each other. Does not match negatives or decimals - word -
+word_char - Matches just a single "word character", defined as any letter,
+number, or _ - anything - Matches any single character, except a newline. To
+also match a newline, use literally_anything - chunk - A "chunk": Any clump of
+characters up until the next newline - uppercase - lowercase - letter - Matches
+just a letter -- not numbers or _ like word_char - hex_digit - oct_digit -
+punctuation - controller - Matches a metadata ASCII characters - printable -
+Matches printable ASCII characters - printable_and_space - alpha_num - unicode
+- Matches a unicode character by name - any_between(char: str, and_char: str) -
+Match any char between `char` and `and_char`, using the ASCII table for
+reference Amounts #### - match_max(input: InputType) - Match as many of `input`
+in the string as you can. This is equivelent to using the unary + operator. If
+`input` is not provided, it works on the previous regex pattern. That's not
+recommended for clarity's sake though - match_num(num: int, input: InputType) -
+Match `num` amount of `input` in the string - match_more_than(min: int, input:
+InputType) - Match more than `min` sequences of `input` in the string -
+match_at_least(min: int, input: InputType) - Match at least `min` sequences of
+`input` in the string - match_at_most(max: int, input: InputType) - Match at
+most `max` instances of `input` in the string - match_range(min: int, max: int,
+input: InputType, greedy: bool=True, possessive: bool=False) - Match between
+`min` and `max` sequences of `input` in the string. This also accepts `greedy`
+and `possessive` parameters Max can be an empty string to indicate no maximum
 `greedy` means it will try to match as many repititions as possible non-greedy
 will try to match as few repititions as possible `possessive` means it won't
 backtrack to try to find any repitions see https://docs.python.org/3/library/
 re.html for more help - at_least_one(input: InputType, greedy: bool=True,
 possessive: bool=False) - Match at least one of `input` in the string. This
 also accepts `greedy` and `possessive` parameters `greedy` means it will try to
 match as many repititions as possible non-greedy will try to match as few
@@ -232,19 +241,19 @@
 ASCII flag is used to disable non-ASCII matches. The current locale does
 notchange the effect of this flag unless the LOCALE flag is also used - DOTALL
 - Make the '.' special character match any character at all, including a
 newline. It's recommended you simply useliterally_anything instead - LOCALE -
 Try not to use this, and rely on unicode matching instead - MULTILINE - This is
 automatically inserted when using line_start and line_end, you shouldn't need
 to add it manually - UNICODE - Match using the full unicode standard, instead
-of just ASCII. Enabled by default, and therefore redundant. python Positionals
-#### These differentiate the *string* starting with a sequence, and a *line*
-starting with a sequence. Do note that the startof the string is also the start
-of a line. These can also be called without parameters to denote the start/end
-of astring/line without something specific having to be next to it. -
+of just ASCII. Enabled by default, and therefore redundant. _jj_aa_vv_aa_ss_cc_rr_ii_pp_tt
+Positionals #### These differentiate the *string* starting with a sequence, and
+a *line* starting with a sequence. Do note that the startof the string is also
+the start of a line. These can also be called without parameters to denote the
+start/end of astring/line without something specific having to be next to it. -
 string_starts_with - string_ends_with - line_starts_with - line_ends_with -
 word_boundary - Matches the boundary of a word, i.e. the empty space between a
 word character and not a word character, or the end of a string -
 not_word_boundary - The opposite of `wordBoundary` Literals #### - tab - space
 - space_or_tab - new_line - carriage_return - quote - Matches ', ", and ` -
 vertical_tab - form_feed - comma - period - underscore Not Literals #### -
 not_whitespace - not_digit - not_word Catagories #### - whitespace - whitechunk
@@ -375,189 +384,233 @@
 uppercase members. Full Unicode matching(such as Ã matching Ã¼) also works
 unless the ASCII flag is used to disable non-ASCII matches. The current locale
 does notchange the effect of this flag unless the LOCALE flag is also used -
 DOTALL - Make the '.' special character match any character at all, including a
 newline. It's recommended you simply useliterally_anything instead - LOCALE -
 Try not to use this, and rely on unicode matching instead - MULTILINE - This is
 automatically inserted when using line_start and line_end, you shouldn't need
-to add it manually javascript Positionals #### These differentiate the *string*
-starting with a sequence, and a *line* starting with a sequence. Do note that
-the startof the string is also the start of a line. These can also be called
-without parameters to denote the start/end of astring/line without something
-specific having to be next to it. - string_starts_with - string_ends_with -
-line_starts_with - line_ends_with - word_boundary - Matches the boundary of a
-word, i.e. the empty space between a word character and not a word character,
-or the end of a string - not_word_boundary - The opposite of `wordBoundary`
-Literals #### - tab - space - space_or_tab - new_line - carriage_return - quote
-- Matches ', ", and ` - vertical_tab - form_feed - comma - period - underscore
-Not Literals #### - not_whitespace - not_digit - not_word Catagories #### -
-whitespace - whitechunk - A "chunk" of whitespace. Just any amount of
-whitespace together - digit - number - Matches multiple digits next to each
-other. Does not match negatives or decimals - word - word_char - Matches just a
-single "word character", defined as any letter, number, or _ - anything -
-Matches any single character, except a newline. To also match a newline, use
-literally_anything - chunk - A "chunk": Any clump of characters up until the
-next newline - uppercase - lowercase - letter - Matches just a letter -- not
-numbers or _ like word_char - hex_digit - oct_digit - punctuation - controller
-- Matches a metadata ASCII characters - printable - Matches printable ASCII
-characters - printable_and_space - alpha_num - unicode - Matches a unicode
-character by name - any_between(char: str, and_char: str) - Match any char
-between `char` and `and_char`, using the ASCII table for reference Amounts ####
-- match_max(input: InputType) - Match as many of `input` in the string as you
-can. This is equivelent to using the unary + operator. If `input` is not
-provided, it works on the previous regex pattern. That's not recommended for
-clarity's sake though - match_num(num: int, input: InputType) - Match `num`
-amount of `input` in the string - match_more_than(min: int, input: InputType) -
-Match more than `min` sequences of `input` in the string - match_at_least(min:
-int, input: InputType) - Match at least `min` sequences of `input` in the
-string - match_at_most(max: int, input: InputType) - Match at most `max`
-instances of `input` in the string - match_range(min: int, max: int, input:
-InputType, greedy: bool=True, possessive: bool=False) - Match between `min` and
-`max` sequences of `input` in the string. This also accepts `greedy` and
-`possessive` parameters Max can be an empty string to indicate no maximum
+to add it manually - UNICODE - Match using the full unicode standard, instead
+of just ASCII. Enabled by default, and therefore redundant. _pp_yy_tt_hh_oo_nn Positionals
+#### These differentiate the *string* starting with a sequence, and a *line*
+starting with a sequence. Do note that the startof the string is also the start
+of a line. These can also be called without parameters to denote the start/end
+of astring/line without something specific having to be next to it. -
+string_starts_with - string_ends_with - line_starts_with - line_ends_with -
+word_boundary - Matches the boundary of a word, i.e. the empty space between a
+word character and not a word character, or the end of a string -
+not_word_boundary - The opposite of `wordBoundary` Literals #### - tab - space
+- space_or_tab - new_line - carriage_return - quote - Matches ', ", and ` -
+vertical_tab - form_feed - comma - period - underscore Not Literals #### -
+not_whitespace - not_digit - not_word Catagories #### - whitespace - whitechunk
+- A "chunk" of whitespace. Just any amount of whitespace together - digit -
+number - Matches multiple digits next to each other. Does not match negatives
+or decimals - word - word_char - Matches just a single "word character",
+defined as any letter, number, or _ - anything - Matches any single character,
+except a newline. To also match a newline, use literally_anything - chunk - A
+"chunk": Any clump of characters up until the next newline - uppercase -
+lowercase - letter - Matches just a letter -- not numbers or _ like word_char -
+hex_digit - oct_digit - punctuation - controller - Matches a metadata ASCII
+characters - printable - Matches printable ASCII characters -
+printable_and_space - alpha_num - unicode - Matches a unicode character by name
+- any_between(char: str, and_char: str) - Match any char between `char` and
+`and_char`, using the ASCII table for reference Amounts #### - match_max(input:
+InputType) - Match as many of `input` in the string as you can. This is
+equivelent to using the unary + operator. If `input` is not provided, it works
+on the previous regex pattern. That's not recommended for clarity's sake though
+- match_num(num: int, input: InputType) - Match `num` amount of `input` in the
+string - match_more_than(min: int, input: InputType) - Match more than `min`
+sequences of `input` in the string - match_at_least(min: int, input: InputType)
+- Match at least `min` sequences of `input` in the string - match_at_most(max:
+int, input: InputType) - Match at most `max` instances of `input` in the string
+- match_range(min: int, max: int, input: InputType, greedy: bool=True,
+possessive: bool=False) - Match between `min` and `max` sequences of `input` in
+the string. This also accepts `greedy` and `possessive` parameters Max can be
+an empty string to indicate no maximum `greedy` means it will try to match as
+many repititions as possible non-greedy will try to match as few repititions as
+possible `possessive` means it won't backtrack to try to find any repitions see
+https://docs.python.org/3/library/re.html for more help - at_least_one(input:
+InputType, greedy: bool=True, possessive: bool=False) - Match at least one of
+`input` in the string. This also accepts `greedy` and `possessive` parameters
 `greedy` means it will try to match as many repititions as possible non-greedy
 will try to match as few repititions as possible `possessive` means it won't
 backtrack to try to find any repitions see https://docs.python.org/3/library/
-re.html for more help - at_least_one(input: InputType, greedy: bool=True,
-possessive: bool=False) - Match at least one of `input` in the string. This
-also accepts `greedy` and `possessive` parameters `greedy` means it will try to
+re.html for more help - at_least_none(input: InputType, greedy: bool=True,
+possessive: bool=False) - Match 0 or more sequences of `input`. This also
+accepts `greedy` and `possessive` parameters `greedy` means it will try to
 match as many repititions as possible non-greedy will try to match as few
 repititions as possible `possessive` means it won't backtrack to try to find
-any repitions see https://docs.python.org/3/library/re.html for more help -
-at_least_none(input: InputType, greedy: bool=True, possessive: bool=False) -
-Match 0 or more sequences of `input`. This also accepts `greedy` and
+any repitions see https://docs.python.org/3/library/re.html for more help
+Choices #### - optional(input: InputType, greedy: bool=True, possessive:
+bool=False) - Match `input` if it's there. This also accepts `greedy` and
 `possessive` parameters `greedy` means it will try to match as many repititions
 as possible non-greedy will try to match as few repititions as possible
 `possessive` means it won't backtrack to try to find any repitions see https://
-docs.python.org/3/library/re.html for more help Choices #### - optional(input:
-InputType, greedy: bool=True, possessive: bool=False) - Match `input` if it's
-there. This also accepts `greedy` and `possessive` parameters `greedy` means it
-will try to match as many repititions as possible non-greedy will try to match
-as few repititions as possible `possessive` means it won't backtrack to try to
-find any repitions see https://docs.python.org/3/library/re.html for more help
-- either(input: InputType, or_input: InputType) - any_of(*inputs: str, chars:
-bool | None=None, split: bool | None=None) - Match any of the given `inputs`.
-Note that `inputs` can be multiple parameters, or a single string. Can also
-accept parameters chars and split. If char is set to True, then `inputs` must
-only be a single string, it interprets `inputs` as characters, and splits it up
-to find any of the chars in the string. If split is set to true, it forces the
-?(...) regex syntax instead of the [...] syntax. It should act the same way,
-but your output regex will look different. By default, it just optimizes it for
-you. - any_char_except(*inputs: str) - This matches any char that is NOT in
-`inputs`. `inputs` can be multiple parameters, or a single string of chars to
-split. - any_except(input: InputType, type: InputType='.*') - Matches anything
-other than `input`, which must be a single string or EZRegex chain, **not** a
-list. Also optionally accepts the `type` parameter, which works like this:
-"Match any `type` other than `input`". For example, "match any word which is
-not foo". Do note that this function is new, and I'm still working out the
-kinks. - each(*inputs: InputType) - Matches if the next part of the string can
-match all of the given inputs. Like the + operator, but out of order.
-Conditionals #### These can only be used once in a given expression. They only
-match a given expression if the expression is/ins'tfollowed/preceeded by a the
-given pattern - if_proceded_by(input: InputType) - Matches the pattern if it
-has `input` coming after it. Can only be used once in a given pattern, as it
-only applies to the end - if_not_proceded_by(input: InputType) - Matches the
-pattern if it does **not** have `input` coming after it. Can only be used once
-in a given pattern, as it only applies to the end - if_preceded_by(input:
-InputType) - Matches the pattern if it has `input` coming before it. Can only
-be used once in a given pattern, as it only applies to the beginning -
-if_not_preceded_by(input: InputType) - Matches the pattern if it does **not**
-have `input` coming before it. Can only be used once in a given pattern, as it
-only applies to the beginning - if_enclosed_with(open: str, stuff: InputType,
-close: str | None=None) - Matches if the string has `open`, then `stuff`, then
-`close`, but only "matches" stuff. Just a convenience combination of
-ifProceededBy and ifPreceededBy. Grouping #### - group(input: InputType, name:
-str | None=None) - Causes `input` to be captured as an unnamed group. Only
-useful when replacing regexs - passive_group(input: InputType) - As all regexs
-in EZRegex capture passively, this is entirely useless. But if you really want
-to, here it is - earlier_group(num_or_name: int | str) - Matches whatever the
-group referenced by `num_or_name` matched earlier. Must be *after* a group
-which would match `num_or_name` - if_exists(num_or_name: int | str, does:
-InputType, doesnt: InputType | None=None) - Matches `does` if the group
-`num_or_name` exists, otherwise it matches `doesnt` Replacement #### In the
-intrest of "I don't want to think about any syntax at all", I have included
-replace members. Do note that theyare not interoperable with the other
-EZRegexs, and can only be used with other strings and each other. - rgroup
-(num_or_name: str | int) - Puts in its place the group specified, either by
-group number (for unnamed groups) or group name (for named groups). Named
-groups are also counted by number, I'm pretty sure. Groups are numbered
-starting from 1 - replace_entire - Puts in its place the entire match - replace
-(string: str, rtn_str: bool=True) -> str | EZRegex - Generates a valid regex
-replacement string, using Python f-string like syntax. Example: ``` replace
-("named: {group}, numbered: {1}, entire: {0}") ``` Like Python f-strings, use {
-{ and }} to specify { and } Set the `rtn_str` parameter to True to have it
-return an EZRegex type instead of a string Note: Remember that index 0 is the
-entire match There's a few of advantages to using this instead of just the
-regular regex replacement syntax: - It's consistent between dialects - It's
-closer to Python f-string syntax, which is cleaner and more familiar - It
-handles numbered, named, and entire replacement types the same Misc #### -
-is_exactly(input: InputType) - This matches the string if and only if the
-entire string is exactly equal to `input` - literal(input: InputType) - This is
-a redundant function. You should always be able to use `... + 'stuff'` just as
-easily as `... + literal('stuff')` - raw(regex: str) - If you already have some
-regular regex written, and you want to incorperate it, this will allow you to
-include it without sanatizing all the backslaches and such, which all the other
-EZRegexs do automatically Premade #### These are some useful combinations that
-may be commonly used. They are not as stable, and may be changed and added to
-inlater versions to make them more accurate - literally_anything - *Any*
-character, include newline - signed - a signed number, including 123, -123, and
-+123 - unsigned - Same as number. Will not match +123 - plain_float - Will
-match 123.45 and 123. - full_float - Will match plain_float as well as things
-like 1.23e-10 and 1.23e+10 - int_or_float - ow - "Optional Whitechunk" - email
-- Matches an email - version - The *official* regex for matching version
-numbers from https://semver.org/. It includes 5 groups that can bematched/
-replaced: `major`, `minor`, `patch`, `prerelease`, and `buildmetadata` -
-version_numbered - Same as `version`, but it uses numbered groups for each
-version number instead of named groups Flags #### These shadow python regex
-flags, and can just as easily be specified directly to the re library instead.
-They're providedhere for compatibility with other regex dialects. See https://
-docs.python.org/3/library/re.html#flags for details - ASCII - Make matching
-words, word boundaries, digits, and whitespace perform ASCII-only matching
-instead of full Unicodematching. This is only meaningful for Unicode (str)
-patterns, and is ignored for bytes patterns - IGNORECASE - Perform case-
-insensitive matching, including expressions that explicitly use uppercase
-members. Full Unicode matching(such as Ã matching Ã¼) also works unless the
-ASCII flag is used to disable non-ASCII matches. The current locale does
-notchange the effect of this flag unless the LOCALE flag is also used - DOTALL
-- Make the '.' special character match any character at all, including a
+docs.python.org/3/library/re.html for more help - either(input: InputType,
+or_input: InputType) - any_of(*inputs: str, chars: bool | None=None, split:
+bool | None=None) - Match any of the given `inputs`. Note that `inputs` can be
+multiple parameters, or a single string. Can also accept parameters chars and
+split. If char is set to True, then `inputs` must only be a single string, it
+interprets `inputs` as characters, and splits it up to find any of the chars in
+the string. If split is set to true, it forces the ?(...) regex syntax instead
+of the [...] syntax. It should act the same way, but your output regex will
+look different. By default, it just optimizes it for you. - any_char_except
+(*inputs: str) - This matches any char that is NOT in `inputs`. `inputs` can be
+multiple parameters, or a single string of chars to split. - any_except(input:
+InputType, type: InputType='.*') - Matches anything other than `input`, which
+must be a single string or EZRegex chain, **not** a list. Also optionally
+accepts the `type` parameter, which works like this: "Match any `type` other
+than `input`". For example, "match any word which is not foo". Do note that
+this function is new, and I'm still working out the kinks. - each(*inputs:
+InputType) - Matches if the next part of the string can match all of the given
+inputs. Like the + operator, but out of order. Conditionals #### These can only
+be used once in a given expression. They only match a given expression if the
+expression is/ins'tfollowed/preceeded by a the given pattern - if_proceded_by
+(input: InputType) - Matches the pattern if it has `input` coming after it. Can
+only be used once in a given pattern, as it only applies to the end -
+if_not_proceded_by(input: InputType) - Matches the pattern if it does **not**
+have `input` coming after it. Can only be used once in a given pattern, as it
+only applies to the end - if_preceded_by(input: InputType) - Matches the
+pattern if it has `input` coming before it. Can only be used once in a given
+pattern, as it only applies to the beginning - if_not_preceded_by(input:
+InputType) - Matches the pattern if it does **not** have `input` coming before
+it. Can only be used once in a given pattern, as it only applies to the
+beginning - if_enclosed_with(open: str, stuff: InputType, close: str |
+None=None) - Matches if the string has `open`, then `stuff`, then `close`, but
+only "matches" stuff. Just a convenience combination of ifProceededBy and
+ifPreceededBy. Grouping #### - group(input: InputType, name: str | None=None) -
+Causes `input` to be captured as an unnamed group. Only useful when replacing
+regexs - passive_group(input: InputType) - As all regexs in EZRegex capture
+passively, this is entirely useless. But if you really want to, here it is -
+earlier_group(num_or_name: int | str) - Matches whatever the group referenced
+by `num_or_name` matched earlier. Must be *after* a group which would match
+`num_or_name` - if_exists(num_or_name: int | str, does: InputType, doesnt:
+InputType | None=None) - Matches `does` if the group `num_or_name` exists,
+otherwise it matches `doesnt` Replacement #### In the intrest of "I don't want
+to think about any syntax at all", I have included replace members. Do note
+that theyare not interoperable with the other EZRegexs, and can only be used
+with other strings and each other. - rgroup(num_or_name: str | int) - Puts in
+its place the group specified, either by group number (for unnamed groups) or
+group name (for named groups). Named groups are also counted by number, I'm
+pretty sure. Groups are numbered starting from 1 - replace_entire - Puts in its
+place the entire match - replace(string: str, rtn_str: bool=True) -> str |
+EZRegex - Generates a valid regex replacement string, using Python f-string
+like syntax. Example: ``` replace("named: {group}, numbered: {1}, entire: {0}")
+``` Like Python f-strings, use {{ and }} to specify { and } Set the `rtn_str`
+parameter to True to have it return an EZRegex type instead of a string Note:
+Remember that index 0 is the entire match There's a few of advantages to using
+this instead of just the regular regex replacement syntax: - It's consistent
+between dialects - It's closer to Python f-string syntax, which is cleaner and
+more familiar - It handles numbered, named, and entire replacement types the
+same Misc #### - is_exactly(input: InputType) - This matches the string if and
+only if the entire string is exactly equal to `input` - literal(input:
+InputType) - This is a redundant function. You should always be able to use
+`... + 'stuff'` just as easily as `... + literal('stuff')` - raw(regex: str) -
+If you already have some regular regex written, and you want to incorperate it,
+this will allow you to include it without sanatizing all the backslaches and
+such, which all the other EZRegexs do automatically Premade #### These are some
+useful combinations that may be commonly used. They are not as stable, and may
+be changed and added to inlater versions to make them more accurate -
+literally_anything - *Any* character, include newline - signed - a signed
+number, including 123, -123, and +123 - unsigned - Same as number. Will not
+match +123 - plain_float - Will match 123.45 and 123. - full_float - Will match
+plain_float as well as things like 1.23e-10 and 1.23e+10 - int_or_float - ow -
+"Optional Whitechunk" - email - Matches an email - version - The *official*
+regex for matching version numbers from https://semver.org/. It includes 5
+groups that can bematched/replaced: `major`, `minor`, `patch`, `prerelease`,
+and `buildmetadata` - version_numbered - Same as `version`, but it uses
+numbered groups for each version number instead of named groups Flags ####
+These shadow python regex flags, and can just as easily be specified directly
+to the re library instead. They're providedhere for compatibility with other
+regex dialects. See https://docs.python.org/3/library/re.html#flags for details
+- ASCII - Make matching words, word boundaries, digits, and whitespace perform
+ASCII-only matching instead of full Unicodematching. This is only meaningful
+for Unicode (str) patterns, and is ignored for bytes patterns - IGNORECASE -
+Perform case-insensitive matching, including expressions that explicitly use
+uppercase members. Full Unicode matching(such as Ã matching Ã¼) also works
+unless the ASCII flag is used to disable non-ASCII matches. The current locale
+does notchange the effect of this flag unless the LOCALE flag is also used -
+DOTALL - Make the '.' special character match any character at all, including a
 newline. It's recommended you simply useliterally_anything instead - LOCALE -
 Try not to use this, and rely on unicode matching instead - MULTILINE - This is
 automatically inserted when using line_start and line_end, you shouldn't need
-to add it manually - UNICODE - Match using the full unicode standard, instead
-of just ASCII. Enabled by default, and therefore redundant. Operators - `+`,
-`<<`, `>>` - These all do the same thing: combine expressions - `*` -
-Multiplies an expression a number of times. `expr * 3` is equivelent to `expr +
-expr + expr`. Can also be used like `expr * ...` is equivalent to `anyAmt
-(expr)` - `+` - A unary + operator acts exactly as a match_max() does, or, if
-you're familiar with regex syntax, the + operator - `[]` - expr[2, 3] is
-equivalent to `match_range(2, 3, expr)` - expr[2, ...] or expr[2,] is
-equivalent to `at_least(2, expr)` - expr[... , 2] is equivalent to `at_most(2,
-expr)` - expr[...] or expr[0, ...] is equivelent to `at_least_0(expr)` - expr
-[1, ...] is equivalent to `at_least_1(expr)` - `&` - Coming soon! This will
-work like the + operator, but they can be out of order. Like an and operation.
-- `|` - Coming soon! This will work like an or operation, which will work just
-like anyOf() - `%` - This automatically calls re.search() for you and returns
-the match object (or None). Use like this: `(digit * 2) % '99 beers on the
-wall'` - `~` - This inverts the expression. This is equivalent to calling the
-.invert() method ## Explanation of How it Works Everything relies on the
-EZRegex class. In the elements.py file of each dialect, I have defined a ton of
-pre-made EZRegexs which mimic all (or at least as many as I can) fundamental
-parts of the regex syntax, plus a few others which are common combinations
-(like chunk or optional(whitechunk)). Any of them which have parameters are
-wrapped in functions to provide proper typing & linting. They all are either
-EZRegexs or are functions which return EZRegexs. These have operators
-overloaded so you can combine them in intuitive ways and call them by intuitive
-names. All the functions passed to EZRegex take a function parameter (or a
-string which gets converted to a function for convenience), which gets called
-with the current regex expression and any parameters passed along when the
-instance gets called with the () operator. That way you can add things to the
-front or back of an expression for example, and you can change what exactly
-gets added to the current expression based on other parameters. You can also
-chain strings together, and pass them as parameters to other EZRegexs, which
-auto-compiles them and adds them appropriately. I also have everything which
-could capture a group capture it passively, except for actual group operators,
-and always have the (?m) (multiline) flag automatically asserted whenever
-lineStart/lineEnd are used so as to differentiate between capturing at the
-beginning/end of a string and the beginning/end of a line. ## Todo See [the
-todo](todo.txt). Eventually, I would like to move the todo to GitHub issues. ##
-License EZRegex is distributed under the [MIT License](https://
-choosealicense.com/licenses/mit)
+to add it manually Operators - `+`, `<<`, `>>` - These all do the same thing:
+combine expressions - `*` - Multiplies an expression a number of times. `expr *
+3` is equivelent to `expr + expr + expr`. Can also be used like `expr * ...` is
+equivalent to `any_amt(expr)` - `+` - A unary + operator acts exactly as a
+match_max() does, or, if you're familiar with regex syntax, the + operator - `
+[]` - expr[2, 3] is equivalent to `match_range(2, 3, expr)` - expr[2, ...] or
+expr[2,] is equivalent to `at_least(2, expr)` - expr[... , 2] is equivalent to
+`at_most(2, expr)` - expr[...] or expr[0, ...] is equivelent to `at_least_0
+(expr)` - expr[1, ...] is equivalent to `at_least_1(expr)` - `&` - Coming soon!
+This will work like the + operator, but they can be out of order. Like an and
+operation. - `|` - Coming soon! This will work like an or operation, which will
+work just like any_of() - `%` - This automatically calls re.search() for you
+and returns the match object (or None). Use like this: `(digit * 2) % '99 beers
+on the wall'` - `~` - This inverts the expression, equivalent to calling the
+.invert() method ## Developer Documentation ### The EZRegex class Everything
+relies on the EZRegex class. EZRegex shouldn't be instantiated by the user, as
+each dialect defines their own EZRegex elements specific to that dialect (more
+on that later). Each element represents a fundamental part of the Regular
+Expression syntax for that language, as well as less-fundemental common
+combinations for convenience (like email and float). EZRegex can accept a
+string or a function to define how it's supposed to interact with the current
+"chain" of elements. If it's a string, it just adds it to the end. If it's a
+function, it can accept any positional or named parameters, but has to accept
+`cur=...` as the last parameter (it's complicated). The `cur` parameter is the
+current regular expression chain, as a string. What's returned becomes the new
+`cur` parameter of the next element, or, if there is no next element, the final
+regex. That way you can add to the front or back of an expression, and you can
+change what exactly gets added to the current expression based on other
+parameters. The EZRegex class has operators overloaded so you can combine them
+in intuitive ways and call them by intuitive names. ### Typing & Linting The
+updated method of doing this is to define all the EZRegex elements of a dialect
+in `elements.py`, and then add type hints and doc strings in the `elements.pyi`
+file. EZRegex elements that accept parameters are typed as functions (even
+though they're not), for both convenience for the user when using linter, and
+to give documentation in an easier way. EZRegex elements that don't accept
+parameters should be typed as EZRegex, and given documentation as a string on
+the line below it. This is *slightly* non-standard, but linters support it, as
+well as my documentation generator script, which parses the .pyi files. The
+elements can also be seperated into groups in the .pyi files by using `"Group:
+\\n\"`, which also gets parsed by the documentation script. The groups aren't
+used in the actual library, but are helpful in seperating the documentation, as
+well as used in [ezregex.org](http://ezregex.org) ### Dialects Because most
+regex dialects *are* 90% identical, a hidden "base" dialect is implemented, but
+it works a bit differently. It has an `elements.py` file, but it defines all
+the elements as a dict in the form of {"element_name": {"keyword":
+"arguements"}}. It then has a `load_dialect()` function, which is the only
+thing importable from it. The reason it's done this way is because `dialect` is
+a required parameter of the EZRegex constructor, so `load_dialect()` takes a
+`dialect` parameter, and constructs the base elements from it's dict and
+returns a new dict of initialized elements to be dumped into the global scope
+of the dialect. The `elements.py` file of a specific dialect can then remove
+any elements that it doesn't support (using the `del` keyword) and add/
+overwrite any it does support. ### Inverting There's actually 2 algorithms
+implemented for "inverting" regexs. The old algorithm regexs the regexs in a
+specific order to replace parts one at a time. This is just as nasty and
+horrifying as it sounds. Dispite it being a terrible, *terrible* solution, I
+actually got it to work decently well. Later, when I was reading up on abstract
+syntax trees, and scrolling around on PyPi, I realized that Python has one
+built in, and that it's available to use. I reimplemented the whole algorithm
+to instead parse the AST given by the built-in re lexer, and wrote my own
+parser on top of it, which works *much* better. Along the way, I also
+discovered, deep in the corners of the internet, 2 other Python libraries which
+do almost the same thing: `xeger` (regex backwards), and `sre_yield`. `xeger`
+technically works, however it tends to include unprintable characters, so it's
+output isn't very readable. `sre_yeild` is better, but it can be very slow, and
+is not quite the use case I'm going for. My invert algorithm is meant to be a
+debugging tool (though it doubles well for a testing tool), so it does things
+like detecting words (as opposed to seperate word characters) and inserts
+actual words, and doing the same for numbers and inserting `12345...`, as well
+as a couple other enhancements. ### Tests Tests for a while now have just been
+in a single `tests.py` file, which was a giant pile of all the tests. I'm
+currently moving to use pytest. There's a `regexs.json` file (and a
+`replacements.json` file) that have a bunch of regexs, along with things
+they're supposed to match, and things they're not supposed to match, for
+testing. ## Installation EZRegex is distributed on [PyPI](https://pypi.org) as
+a universal wheel and is available on Linux, macOS and Windows and supports
+Python 3.10+ and PyPy. ```bash pip install ezregex ``` The import name is the
+same as the package name: ```python import ezregex as er ``` ## Todo See [the
+todo](todo.txt). I'm slowly moving these to [GitHub issues](https://github.com/
+smartycope/ezregex/issues), but for now, they're mostly still there ## License
+EZRegex is distributed under the [MIT License](https://choosealicense.com/
+licenses/mit)
```

