# Comparing `tmp/django_safe_template_engine-1.0.0.tar.gz` & `tmp/django_safe_template_engine-1.1.0.tar.gz`

## Comparing `django_safe_template_engine-1.0.0.tar` & `django_safe_template_engine-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/.flake8
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/isort.cfg
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/mypy.ini
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/run_tests.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/src/django_safe_template_engine/__init__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/src/django_safe_template_engine/engine.py
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/src/django_safe_template_engine/trusted_filters.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/src/django_safe_template_engine/trusted_tags.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/src/django_safe_template_engine/validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/requirements.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/settings.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/test_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/filters/__init__.py
--rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/filters/test_trusted_filters.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/filters/test_untrusted_filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/loaders/__init__.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/loaders/test_untrusted_loaders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/tags/__init__.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/tags/test_trusted_tags.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/tests/tags/test_untrusted_tags.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/.gitignore
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/LICENSE
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/README.md
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 django_safe_template_engine-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/.flake8
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/isort.cfg
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/mypy.ini
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/run_tests.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/src/django_safe_template_engine/__init__.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/src/django_safe_template_engine/engine.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/src/django_safe_template_engine/trusted_filters.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/src/django_safe_template_engine/trusted_tags.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/src/django_safe_template_engine/validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/requirements.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/settings.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/test_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/filters/__init__.py
+-rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/filters/test_trusted_filters.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/filters/test_untrusted_filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/loaders/__init__.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/loaders/test_untrusted_loaders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/tags/__init__.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/tags/test_trusted_tags.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/tests/tags/test_untrusted_tags.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/README.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10287 2020-02-02 00:00:00.000000 django_safe_template_engine-1.1.0/PKG-INFO
```

### Comparing `django_safe_template_engine-1.0.0/.github/workflows/build.yml` & `django_safe_template_engine-1.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/src/django_safe_template_engine/trusted_filters.py` & `django_safe_template_engine-1.1.0/src/django_safe_template_engine/trusted_filters.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/src/django_safe_template_engine/trusted_tags.py` & `django_safe_template_engine-1.1.0/src/django_safe_template_engine/trusted_tags.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/tests/test_validators.py` & `django_safe_template_engine-1.1.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/tests/filters/test_trusted_filters.py` & `django_safe_template_engine-1.1.0/tests/filters/test_trusted_filters.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/tests/filters/test_untrusted_filters.py` & `django_safe_template_engine-1.1.0/tests/filters/test_untrusted_filters.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/tests/loaders/test_untrusted_loaders.py` & `django_safe_template_engine-1.1.0/tests/loaders/test_untrusted_loaders.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/tests/tags/test_trusted_tags.py` & `django_safe_template_engine-1.1.0/tests/tags/test_trusted_tags.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/tests/tags/test_untrusted_tags.py` & `django_safe_template_engine-1.1.0/tests/tags/test_untrusted_tags.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/.gitignore` & `django_safe_template_engine-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/LICENSE` & `django_safe_template_engine-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.0.0/README.md` & `django_safe_template_engine-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Django Safe Template Engine
 
 Django template engine to render untrusted template code
 
 ## Requirements
 
 - Python 3.8 to 3.11
-- Django 3.0
+- Django 3.2 (officially supported in technical tests, all built-in template tags and filters reviewed)
 
 ## Available tools
 
 Template engine:
 
 ```py
 from django.template import Template
@@ -32,87 +32,87 @@
 
 ## Trusted built-ins
 
 The following tags and filters are allowed by this template engine.
 
 ### Trusted tags
 
-- [`autoescape`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#autoescape)
-- [`comment`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#comment)
-- [`cycle`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#cycle)
-- [`filter`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#filter)
-- [`firstof`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#firstof)
-- [`for`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#for)
-- [`for … empty`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#for-empty)
-- [`if`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#if)
-- [`ifchanged`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#ifchanged)
-- [`lorem`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#lorem)
-- [`now`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#now)
-- [`regroup`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#regroup)
-- [`resetcycle`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#resetcycle)
-- [`spaceless`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#spaceless)
-- [`templatetag`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#templatetag)
-- [`url`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#url)
-- [`verbatim`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#verbatim)
-- [`widthratio`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#widthratio)
-- [`with`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#with)
+- [`autoescape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#autoescape)
+- [`comment`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#comment)
+- [`cycle`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#cycle)
+- [`filter`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#filter)
+- [`firstof`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#firstof)
+- [`for`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#for)
+- [`for … empty`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#for-empty)
+- [`if`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#if)
+- [`ifchanged`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#ifchanged)
+- [`lorem`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#lorem)
+- [`now`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#now)
+- [`regroup`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#regroup)
+- [`resetcycle`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#resetcycle)
+- [`spaceless`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#spaceless)
+- [`templatetag`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#templatetag)
+- [`url`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#url)
+- [`verbatim`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#verbatim)
+- [`widthratio`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#widthratio)
+- [`with`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#with)
 
 ### Trusted filters
 
 <!-- TODO: Check for dead links -->
 <!-- TODO: Re-order? -->
-- [`addslashes`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#addslashes)
-- [`capfirst`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#capfirst)
-- [`escapejs`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#escapejs)
-- [`json_script`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#json_script)
-- [`floatformat`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#floatformat)
-- [`iriencode`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#iriencode)
-- [`linenumbers`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#linenumbers)
-- [`lower`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#lower)
-- [`make_list`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#make_list)
-- [`slugify`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#slugify)
-- [`stringformat`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#stringformat)
-- [`title`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#title)
-- [`truncatechars`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#truncatechars)
-- [`truncatechars_html`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#truncatechars_html)
-- [`truncatewords`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#truncatewords)
-- [`truncatewords_html`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#truncatewords_html)
-- [`upper`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#upper)
-- [`urlencode`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#urlencode)
-- [`urlize`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#urlize)
-- [`urlizetrunc`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#urlizetrunc)
-- [`wordcount`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#wordcount)
-- [`wordwrap`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#wordwrap)
-- [`ljust`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#ljust)
-- [`rjust`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#rjust)
-- [`center`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#center)
-- [`cut`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#cut)
-- [`escape`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#escape)
-- [`force_escape`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#force_escape)
-- [`linebreaks`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#linebreaks)
-- [`linebreaksbr`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#linebreaksbr)
-- [`safe`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#safe)
-- [`safeseq`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#safeseq)
-- [`striptags`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#striptags)
-- [`dictsort`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#dictsort)
-- [`dictsortreversed`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#dictsortreversed)
-- [`first`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#first)
-- [`join`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#join)
-- [`last`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#last)
-- [`length`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#length)
-- [`length_is`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#length_is)
-- [`random`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#random)
-- [`slice`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#slice)
-- [`unordered_list`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#unordered_list)
-- [`add`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#add)
-- [`get_digit`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#get_digit)
-- [`date`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#date)
-- [`time`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#time)
-- [`timesince`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#timesince)
-- [`timeuntil`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#timeuntil)
-- [`default`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#default)
-- [`default_if_none`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#default_if_none)
-- [`divisibleby`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#divisibleby)
-- [`yesno`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#yesno)
-- [`filesizeformat`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#filesizeformat)
-- [`pluralize`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#pluralize)
-- [`phone2numeric`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#phone2numeric)
+- [`addslashes`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#addslashes)
+- [`capfirst`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#capfirst)
+- [`escapejs`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#escapejs)
+- [`json_script`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#json_script)
+- [`floatformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#floatformat)
+- [`iriencode`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#iriencode)
+- [`linenumbers`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linenumbers)
+- [`lower`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#lower)
+- [`make_list`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#make_list)
+- [`slugify`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#slugify)
+- [`stringformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#stringformat)
+- [`title`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#title)
+- [`truncatechars`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatechars)
+- [`truncatechars_html`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatechars_html)
+- [`truncatewords`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatewords)
+- [`truncatewords_html`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatewords_html)
+- [`upper`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#upper)
+- [`urlencode`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlencode)
+- [`urlize`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlize)
+- [`urlizetrunc`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlizetrunc)
+- [`wordcount`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#wordcount)
+- [`wordwrap`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#wordwrap)
+- [`ljust`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#ljust)
+- [`rjust`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#rjust)
+- [`center`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#center)
+- [`cut`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#cut)
+- [`escape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#escape)
+- [`force_escape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#force_escape)
+- [`linebreaks`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linebreaks)
+- [`linebreaksbr`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linebreaksbr)
+- [`safe`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#safe)
+- [`safeseq`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#safeseq)
+- [`striptags`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#striptags)
+- [`dictsort`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#dictsort)
+- [`dictsortreversed`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#dictsortreversed)
+- [`first`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#first)
+- [`join`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#join)
+- [`last`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#last)
+- [`length`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#length)
+- [`length_is`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#length_is)
+- [`random`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#random)
+- [`slice`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#slice)
+- [`unordered_list`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#unordered_list)
+- [`add`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#add)
+- [`get_digit`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#get_digit)
+- [`date`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#date)
+- [`time`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#time)
+- [`timesince`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#timesince)
+- [`timeuntil`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#timeuntil)
+- [`default`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#default)
+- [`default_if_none`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#default_if_none)
+- [`divisibleby`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#divisibleby)
+- [`yesno`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#yesno)
+- [`filesizeformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#filesizeformat)
+- [`pluralize`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#pluralize)
+- [`phone2numeric`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#phone2numeric)
```

### Comparing `django_safe_template_engine-1.0.0/pyproject.toml` & `django_safe_template_engine-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "django_safe_template_engine"
-version = "1.0.0"
-dependencies = ["django >= 3, < 3.1"]
+version = "1.1.0"
+dependencies = ["django >= 3.2, < 4"]
 requires-python = ">=3.8"
 authors = [{ name = "Ronan Boiteau", email = "ronan@boiteau.eu" }]
 maintainers = [{ name = "Ronan Boiteau", email = "ronan@boiteau.eu" }]
 description = "A Django template engine to render untrusted template code"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["django", "safe", "template", "engine"]
```

### Comparing `django_safe_template_engine-1.0.0/PKG-INFO` & `django_safe_template_engine-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django_safe_template_engine
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Django template engine to render untrusted template code
 Project-URL: Homepage, https://github.com/ronanboiteau/django_safe_template_engine
 Project-URL: Documentation, https://github.com/ronanboiteau/django_safe_template_engine/blob/main/README.md
 Project-URL: Repository, https://github.com/ronanboiteau/django_safe_template_engine.git
 Project-URL: Issues, https://github.com/ronanboiteau/django_safe_template_engine/issues
 Project-URL: Changelog, https://github.com/ronanboiteau/django_safe_template_engine/blob/main/CHANGELOG.md
 Author-email: Ronan Boiteau <ronan@boiteau.eu>
@@ -39,27 +39,27 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Keywords: django,engine,safe,template
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: django<3.1,>=3
+Requires-Dist: django<4,>=3.2
 Description-Content-Type: text/markdown
 
 ![GitHub Actions build status](https://github.com/guestready/django_safe_template_engine/actions/workflows/build.yml/badge.svg?branch=main)
 
 # Django Safe Template Engine
 
 Django template engine to render untrusted template code
 
 ## Requirements
 
 - Python 3.8 to 3.11
-- Django 3.0
+- Django 3.2 (officially supported in technical tests, all built-in template tags and filters reviewed)
 
 ## Available tools
 
 Template engine:
 
 ```py
 from django.template import Template
@@ -80,87 +80,87 @@
 
 ## Trusted built-ins
 
 The following tags and filters are allowed by this template engine.
 
 ### Trusted tags
 
-- [`autoescape`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#autoescape)
-- [`comment`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#comment)
-- [`cycle`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#cycle)
-- [`filter`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#filter)
-- [`firstof`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#firstof)
-- [`for`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#for)
-- [`for … empty`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#for-empty)
-- [`if`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#if)
-- [`ifchanged`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#ifchanged)
-- [`lorem`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#lorem)
-- [`now`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#now)
-- [`regroup`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#regroup)
-- [`resetcycle`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#resetcycle)
-- [`spaceless`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#spaceless)
-- [`templatetag`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#templatetag)
-- [`url`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#url)
-- [`verbatim`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#verbatim)
-- [`widthratio`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#widthratio)
-- [`with`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#with)
+- [`autoescape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#autoescape)
+- [`comment`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#comment)
+- [`cycle`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#cycle)
+- [`filter`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#filter)
+- [`firstof`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#firstof)
+- [`for`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#for)
+- [`for … empty`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#for-empty)
+- [`if`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#if)
+- [`ifchanged`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#ifchanged)
+- [`lorem`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#lorem)
+- [`now`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#now)
+- [`regroup`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#regroup)
+- [`resetcycle`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#resetcycle)
+- [`spaceless`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#spaceless)
+- [`templatetag`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#templatetag)
+- [`url`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#url)
+- [`verbatim`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#verbatim)
+- [`widthratio`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#widthratio)
+- [`with`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#with)
 
 ### Trusted filters
 
 <!-- TODO: Check for dead links -->
 <!-- TODO: Re-order? -->
-- [`addslashes`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#addslashes)
-- [`capfirst`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#capfirst)
-- [`escapejs`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#escapejs)
-- [`json_script`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#json_script)
-- [`floatformat`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#floatformat)
-- [`iriencode`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#iriencode)
-- [`linenumbers`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#linenumbers)
-- [`lower`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#lower)
-- [`make_list`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#make_list)
-- [`slugify`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#slugify)
-- [`stringformat`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#stringformat)
-- [`title`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#title)
-- [`truncatechars`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#truncatechars)
-- [`truncatechars_html`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#truncatechars_html)
-- [`truncatewords`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#truncatewords)
-- [`truncatewords_html`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#truncatewords_html)
-- [`upper`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#upper)
-- [`urlencode`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#urlencode)
-- [`urlize`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#urlize)
-- [`urlizetrunc`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#urlizetrunc)
-- [`wordcount`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#wordcount)
-- [`wordwrap`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#wordwrap)
-- [`ljust`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#ljust)
-- [`rjust`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#rjust)
-- [`center`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#center)
-- [`cut`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#cut)
-- [`escape`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#escape)
-- [`force_escape`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#force_escape)
-- [`linebreaks`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#linebreaks)
-- [`linebreaksbr`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#linebreaksbr)
-- [`safe`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#safe)
-- [`safeseq`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#safeseq)
-- [`striptags`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#striptags)
-- [`dictsort`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#dictsort)
-- [`dictsortreversed`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#dictsortreversed)
-- [`first`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#first)
-- [`join`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#join)
-- [`last`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#last)
-- [`length`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#length)
-- [`length_is`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#length_is)
-- [`random`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#random)
-- [`slice`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#slice)
-- [`unordered_list`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#unordered_list)
-- [`add`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#add)
-- [`get_digit`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#get_digit)
-- [`date`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#date)
-- [`time`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#time)
-- [`timesince`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#timesince)
-- [`timeuntil`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#timeuntil)
-- [`default`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#default)
-- [`default_if_none`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#default_if_none)
-- [`divisibleby`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#divisibleby)
-- [`yesno`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#yesno)
-- [`filesizeformat`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#filesizeformat)
-- [`pluralize`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#pluralize)
-- [`phone2numeric`](https://docs.djangoproject.com/en/dev/ref/templates/builtins/#phone2numeric)
+- [`addslashes`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#addslashes)
+- [`capfirst`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#capfirst)
+- [`escapejs`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#escapejs)
+- [`json_script`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#json_script)
+- [`floatformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#floatformat)
+- [`iriencode`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#iriencode)
+- [`linenumbers`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linenumbers)
+- [`lower`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#lower)
+- [`make_list`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#make_list)
+- [`slugify`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#slugify)
+- [`stringformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#stringformat)
+- [`title`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#title)
+- [`truncatechars`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatechars)
+- [`truncatechars_html`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatechars_html)
+- [`truncatewords`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatewords)
+- [`truncatewords_html`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatewords_html)
+- [`upper`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#upper)
+- [`urlencode`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlencode)
+- [`urlize`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlize)
+- [`urlizetrunc`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlizetrunc)
+- [`wordcount`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#wordcount)
+- [`wordwrap`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#wordwrap)
+- [`ljust`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#ljust)
+- [`rjust`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#rjust)
+- [`center`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#center)
+- [`cut`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#cut)
+- [`escape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#escape)
+- [`force_escape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#force_escape)
+- [`linebreaks`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linebreaks)
+- [`linebreaksbr`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linebreaksbr)
+- [`safe`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#safe)
+- [`safeseq`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#safeseq)
+- [`striptags`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#striptags)
+- [`dictsort`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#dictsort)
+- [`dictsortreversed`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#dictsortreversed)
+- [`first`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#first)
+- [`join`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#join)
+- [`last`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#last)
+- [`length`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#length)
+- [`length_is`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#length_is)
+- [`random`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#random)
+- [`slice`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#slice)
+- [`unordered_list`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#unordered_list)
+- [`add`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#add)
+- [`get_digit`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#get_digit)
+- [`date`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#date)
+- [`time`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#time)
+- [`timesince`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#timesince)
+- [`timeuntil`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#timeuntil)
+- [`default`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#default)
+- [`default_if_none`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#default_if_none)
+- [`divisibleby`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#divisibleby)
+- [`yesno`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#yesno)
+- [`filesizeformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#filesizeformat)
+- [`pluralize`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#pluralize)
+- [`phone2numeric`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#phone2numeric)
```

