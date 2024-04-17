# Comparing `tmp/istr_python-0.0.2.tar.gz` & `tmp/istr_python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.0.2.tar", last modified: Sun Apr 14 09:06:41 2024, max compression
+gzip compressed data, was "istr_python-0.0.3.tar", last modified: Wed Apr 17 07:18:05 2024, max compression
```

## Comparing `istr_python-0.0.2.tar` & `istr_python-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 09:06:41.390611 istr_python-0.0.2/
--rw-rw-rw-   0        0        0     2924 2024-04-14 09:06:41.390611 istr_python-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2552 2024-04-14 08:47:05.000000 istr_python-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 09:06:41.363812 istr_python-0.0.2/istr/
--rw-rw-rw-   0        0        0       19 2024-04-13 09:15:49.000000 istr_python-0.0.2/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-13 08:29:51.000000 istr_python-0.0.2/istr/install istr.py
--rw-rw-rw-   0        0        0    10675 2024-04-14 08:57:23.000000 istr_python-0.0.2/istr/istr.py
--rw-rw-rw-   0        0        0      323 2024-04-13 08:58:13.000000 istr_python-0.0.2/istr/sendmoremoney.py
-drwxrwxrwx   0        0        0        0 2024-04-14 09:06:41.389200 istr_python-0.0.2/istr_python.egg-info/
--rw-rw-rw-   0        0        0     2924 2024-04-14 09:06:41.000000 istr_python-0.0.2/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-04-14 09:06:41.000000 istr_python-0.0.2/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 09:06:41.000000 istr_python-0.0.2/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-14 09:06:41.000000 istr_python-0.0.2/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      372 2024-04-14 09:06:31.000000 istr_python-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 09:06:41.390611 istr_python-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 09:06:41.387200 istr_python-0.0.2/tests/
--rw-rw-rw-   0        0        0     8867 2024-04-14 09:00:18.000000 istr_python-0.0.2/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:18:05.735692 istr_python-0.0.3/
+-rw-rw-rw-   0        0        0     4153 2024-04-17 07:18:05.733669 istr_python-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3724 2024-04-17 07:17:19.000000 istr_python-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 07:18:05.709488 istr_python-0.0.3/istr/
+-rw-rw-rw-   0        0        0       19 2024-04-13 09:15:49.000000 istr_python-0.0.3/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.0.3/istr/install istr.py
+-rw-rw-rw-   0        0        0    12638 2024-04-17 07:10:44.000000 istr_python-0.0.3/istr/istr.py
+-rw-rw-rw-   0        0        0      343 2024-04-15 06:46:16.000000 istr_python-0.0.3/istr/sendmoremoney.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:18:05.730674 istr_python-0.0.3/istr_python.egg-info/
+-rw-rw-rw-   0        0        0     4153 2024-04-17 07:18:05.000000 istr_python-0.0.3/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-17 07:18:05.000000 istr_python-0.0.3/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 07:18:05.000000 istr_python-0.0.3/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 07:18:05.000000 istr_python-0.0.3/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      371 2024-04-17 07:17:42.000000 istr_python-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 07:18:05.736685 istr_python-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 07:18:05.726542 istr_python-0.0.3/tests/
+-rw-rw-rw-   0        0        0     9682 2024-04-17 07:00:43.000000 istr_python-0.0.3/tests/test_istr.py
```

### Comparing `istr_python-0.0.2/istr/install istr.py` & `istr_python-0.0.3/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.0.2/tests/test_istr.py` & `istr_python-0.0.3/tests/test_istr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-from __future__ import print_function
-from __future__ import division
-from istr import istr
 import math
 
+if __name__ == "__main__":  # to make the tests run without the pytest cli
+    import sys
+
+    sys.path = ["../istr"] + sys.path
+
 import pytest
 
+from istr import istr
+
+istr.equals = lambda self, other: type(self) == type(other) and (str(self) == str(other))
+# this method tests whether self and other are exactly the same
+
 for i, name in enumerate("minus_one zero one two three four five six seven eight nine ten eleven twelve thirteen".split(), -1):
     globals()[name] = istr(i)
 one_to_twelve = istr.range(1, thirteen)
 
 
 def test_arithmetic():
     assert two + three == "5"
@@ -157,16 +164,16 @@
     assert istr("") == ""
     assert istr("") == 0
     with pytest.raises(ValueError):
         istr(" ")
     assert istr(istr(6)) == "6"
     assert istr(" 12 ") == " 12 "
     with istr.format("03"):
-        assert istr(" 12 ") == "012"
-        assert istr("")==""
+        assert istr("   12  ") == "012"
+        assert istr("") == ""
 
 
 def test_divmod():
     assert divmod(eleven, three) == (istr(3), istr(2))
     assert divmod(11, three) == (istr(3), istr(2))
     assert divmod(eleven, 3) == (istr(3), istr(2))
     assert divmod(11, 3) == (3, 2)
@@ -189,15 +196,15 @@
     for x in istr(range(10000000000000000000)):
         if x == four:
             break
     assert x == 4
 
 
 def test_str_repr():
-    assert repr(one) == "istr('1')"
+    assert one.equals(istr("1"))
     assert str(one) == "1"
     assert f"{one}" == "1"
     assert repr(one_to_twelve) == "istr.range(1, 13)"
     assert repr(istr.range(10)) == "istr.range(0, 10)"
     assert repr(istr.range(one, two, three)) == "istr.range(1, 2, 3)"
 
     assert str(one_to_twelve) == "istr.range(1, 13)"
@@ -302,61 +309,82 @@
     s = istr("").join(istr(("", "", "6")))
     assert s == "6"
     assert s == 6
     assert type(s) == istr
 
 
 def test_matmul():
-    assert five @ 3 == "555"
-    assert five @ 3 == 555
-
-    assert 3 @ five == "555"
-    assert 3 @ five == 555
+    assert (five @ 3).equals(istr("555"))
+    assert (3 @ five).equals(istr("555"))
 
     with pytest.raises(TypeError):
         three @ five
     with pytest.raises(TypeError):
         three @ "5"
     with pytest.raises(TypeError):
         "3" @ five
 
-
 def test_str():
     assert repr(str(five)) == "'5'"
 
 
 def test_trunc_and_friends():
-    assert repr(math.trunc(one)) == "istr('1')"
-    assert repr(math.ceil(one)) == "istr('1')"
-    assert repr(math.floor(one)) == "istr('1')"
-    assert repr(round(one)) == "istr('1')"
+    assert math.trunc(one).equals(istr("1"))
+    assert math.ceil(one).equals(istr("1"))
+    assert math.floor(one).equals(istr("1"))
+    assert round(one).equals(istr("1"))
 
 
 def test_data_structures():
-    assert istr(list(range(1, 4))) == [1, 2, 3]
-    assert istr(list(range(1, 4))) == ["1", "2", "3"]
-
-    assert istr(tuple(range(1, 4))) == (1, 2, 3)
-    assert istr(tuple(range(1, 4))) == ("1", "2", "3")
+    assert repr(istr(list(range(1, 4)))) == "[istr('1'), istr('2'), istr('3')]"
+    assert repr(istr(tuple(range(1, 4)))) == "(istr('1'), istr('2'), istr('3'))"
     assert istr(set(range(1, 4))) == {istr(1), istr(2), istr(3)}
 
-    assert list(istr(range(1, 4))) == [1, 2, 3]
-    assert list(istr(range(1, 4))) == ["1", "2", "3"]
+    assert repr(list(istr(range(1, 4)))) == "[istr('1'), istr('2'), istr('3')]"
+
+    assert repr(list(istr.enumerate("abc"))) == "[(istr('0'), 'a'), (istr('1'), 'b'), (istr('2'), 'c')]"
+    assert repr(list(istr.enumerate("abc", 1))) == "[(istr('1'), 'a'), (istr('2'), 'b'), (istr('3'), 'c')]"
+
+    assert repr(istr(dict(zero=0, one=1, two=4))) == "{'zero': istr('0'), 'one': istr('1'), 'two': istr('4')}"
 
-    assert list(istr(range(1, 4))) == [1, 2, 3]
-    assert list(istr(range(1, 4))) == ["1", "2", "3"]
 
-    assert list(istr.enumerate("abc")) == [(0, "a"), (1, "b"), (2, "c")]
-    assert list(istr.enumerate("abc")) == [("0", "a"), ("1", "b"), ("2", "c")]
+def test_indexing():
+    a = istr(12345)
+    assert a[0].equals(istr(1))
+    assert a[:2].equals(istr(12))
+    assert a[::-1].equals(istr(54321))
+    assert a[-2:].equals(istr(45))
+
+
+def test_reverse():
+    a = istr(12345)
+    assert a.reversed(), same(istr(54321))
 
 
 def test_edge_cases():
     with pytest.raises(ValueError):
         istr("ab")
-    with pytest.raises(TypeError):
+    with pytest.raises(ValueError):
         istr(istr)
-    assert repr(istr(istr(one))) == "istr('1')"
+    assert istr(istr(one)).equals(istr("1"))
+    with pytest.raises(TypeError):
+        istr()
+
+
+def test_unpacking():
+    a = istr("123")
+    x, y, z = istr(*a)
+    assert x.equals(istr(1))
+    assert y.equals(istr(2))
+    assert z.equals(istr(3))
+
+
+def test_subclassing():
+    class jstr(istr):
+        ...
+
+    assert jstr(5).equals(jstr(5))
+    assert repr(jstr(*range(3))) == "(jstr('0'), jstr('1'), jstr('2'))"
 
 
 if __name__ == "__main__":
     pytest.main(["-vv", "-s", "-x", __file__])
-
```

