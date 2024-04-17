# Comparing `tmp/requests_htmlc-0.0.4.tar.gz` & `tmp/requests_htmlc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_htmlc-0.0.4.tar", last modified: Tue Apr 16 19:29:05 2024, max compression
+gzip compressed data, was "requests_htmlc-0.0.5.tar", last modified: Wed Apr 17 18:56:47 2024, max compression
```

## Comparing `requests_htmlc-0.0.4.tar` & `requests_htmlc-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.236491 requests_htmlc-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.224491 requests_htmlc-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.228491 requests_htmlc-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    20876 2024-04-16 19:29:05.236491 requests_htmlc-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19606 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.228491 requests_htmlc-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.228491 requests_htmlc-0.0.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.228491 requests_htmlc-0.0.4/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   288049 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/docs/source/_static/requests-html-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.228491 requests_htmlc-0.0.4/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/docs/source/_templates/hacks.html
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/docs/source/_templates/sidebarintro.html
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/docs/source/_templates/sidebarlogo.html
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19397 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.232491 requests_htmlc-0.0.4/ext/
--rw-r--r--   0 runner    (1001) docker     (127)  2899712 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/ext/requests-html-logo.ai
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)    30000 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/requests_html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.236491 requests_htmlc-0.0.4/requests_htmlc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20876 2024-04-16 19:29:05.000000 requests_htmlc-0.0.4/requests_htmlc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-16 19:29:05.000000 requests_htmlc-0.0.4/requests_htmlc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:29:05.000000 requests_htmlc-0.0.4/requests_htmlc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-16 19:29:05.000000 requests_htmlc-0.0.4/requests_htmlc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 19:29:05.000000 requests_htmlc-0.0.4/requests_htmlc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:29:05.236491 requests_htmlc-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:29:05.236491 requests_htmlc-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    48883 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/tests/python.html
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/tests/test_internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-16 19:29:00.000000 requests_htmlc-0.0.4/tests/test_requests_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.941187 requests_htmlc-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.929188 requests_htmlc-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.933188 requests_htmlc-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-17 18:56:47.941187 requests_htmlc-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.933188 requests_htmlc-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.933188 requests_htmlc-0.0.5/docs/requests-htmlc/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/docs/requests-htmlc/requests_html.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.933188 requests_htmlc-0.0.5/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)  2899712 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/ext/requests-html-logo.ai
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    32509 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/requests_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.937188 requests_htmlc-0.0.5/requests_htmlc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 18:56:47.000000 requests_htmlc-0.0.5/requests_htmlc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 18:56:47.941187 requests_htmlc-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:56:47.937188 requests_htmlc-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    48883 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/tests/python.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/tests/test_internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-17 18:56:44.000000 requests_htmlc-0.0.5/tests/test_requests_html.py
```

### Comparing `requests_htmlc-0.0.4/.github/workflows/pypi-publish.yaml` & `requests_htmlc-0.0.5/.github/workflows/pypi-publish.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -111,8 +111,8 @@
       uses: actions/download-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution 📦 to TestPyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        repository-url: https://test.pypi.org/legacy/
+        repository-url: https://test.pypi.org/legacy/
```

### Comparing `requests_htmlc-0.0.4/.github/workflows/tests.yaml` & `requests_htmlc-0.0.5/.github/workflows/tests.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: tests
+name: python-tests
 
 on:
   # run tests on all PR's to main
   pull_request:
     branches: [main]
 
 jobs:
```

### Comparing `requests_htmlc-0.0.4/.gitignore` & `requests_htmlc-0.0.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -98,13 +98,14 @@
 .spyproject
 
 # Rope project settings
 .ropeproject
 
 # mkdocs documentation
 /site
+/public
 
 # mypy
 .mypy_cache/
 
 # Visual Studio Code 
 .vscode
```

### Comparing `requests_htmlc-0.0.4/LICENSE` & `requests_htmlc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.4/Makefile` & `requests_htmlc-0.0.5/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -44,12 +44,33 @@
 	pip freeze --exclude-editable > $(APP_NAME)/$(REQUIREMENTS_FILE)
 
 documentation:
 	cd docs && make html
 	cd docs/build/html && git add -A && git commit -m 'updates'
 	cd docs/build/html && git push origin gh-pages
 
+# documentation targets
+.PHONY: docs-lint
+docs-lint:
+	@echo linting files at docs/**/*.md
+	markdownlint docs/**/*.md
+
+.PHONY: docs-serve
+docs-serve:
+	@echo serving the site on http://localhost:8000
+	mkdocs serve
+
+.PHONY: docs-build
+docs-build:
+	@echo building the site
+	mkdocs build --strict --verbose --site-dir public
+
+.PHONY: lint
+lint:
+	black $(APP_NAME)/.
+	black tests
+	
 test:
 	python -m pytest tests -v
 
 test-reports:
 	python -m pytest --doctest-modules --junitxml=junit/test-results.xml --cov=requests-html --cov-report=xml --cov-report=html tests -v
```

### Comparing `requests_htmlc-0.0.4/PKG-INFO` & `requests_htmlc-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: requests-htmlc
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fork of requests-html, powered by playwright
 Author: Christian Boin
 License: MIT License
 Requires-Python: >=3.11
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4==4.12.3
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: cssselect==1.2.0
 Requires-Dist: fake-useragent==1.5.1
 Requires-Dist: greenlet==3.0.3
@@ -28,24 +28,26 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: click; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: requests-file; extra == "dev"
-Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mike; extra == "dev"
+Requires-Dist: mkdocstrings-python; extra == "dev"
 Provides-Extra: package
 Requires-Dist: build; extra == "package"
 Requires-Dist: twine; extra == "package"
 
-Requests-HTMLC: Fork of Requests-HTML, using PlayWright
-=======================================================
+# Requests-HTMLC: Fork of Requests-HTML, using PlayWright
 
-.. image:: https://farm5.staticflickr.com/4695/39152770914_a3ab8af40d_k_d.jpg
+![image](https://farm5.staticflickr.com/4695/39152770914_a3ab8af40d_k_d.jpg)
 
 This library intends to make parsing HTML (e.g. scraping the web) as
 simple and intuitive as possible.
 
 When using this library you automatically get:
 
 - **Full JavaScript support**! (Using Chromium, thanks to playwright)
@@ -53,33 +55,33 @@
 - *XPath Selectors*, for the faint of heart.
 - Mocked user-agent (like a real web browser).
 - Automatic following of redirects.
 - Connection–pooling and cookie persistence.
 - The Requests experience you know and love, with magical parsing abilities.
 - **Async Support**
 
-.. Other nice features include:
+Other nice features include:
+- Markdown export of pages and elements.
 
-    - Markdown export of pages and elements.
+## Tutorial & Usage
 
-
-Tutorial & Usage
-================
+Below is a summary of usage for this package.
+For detailed api documentation, see [here](https://cboin1996.github.io/requests-html)
 
 Make a GET request to 'python.org', using Requests:
 
-.. code-block:: pycon
-
+```python
     >>> from requests_html import HTMLSession
     >>> session = HTMLSession()
     >>> r = session.get('https://python.org/')
+```
 
 Try async and get some sites at the same time:
 
-.. code-block:: pycon
+```python
 
     >>> from requests_html import AsyncHTMLSession
     >>> asession = AsyncHTMLSession()
     >>> async def get_pythonorg():
     ...     r = await asession.get('https://python.org/')
     ...     return r
     ...
@@ -97,132 +99,137 @@
     >>> # Each item in the results list is a response object and can be interacted with as such
     >>> for result in results: 
     ...     print(result.html.url)
     ... 
     https://www.python.org/
     https://www.google.com/
     https://www.reddit.com/
+```
 
-Note that the order of the objects in the results list represents the order they were returned in, not the order that the coroutines are passed to the ``run`` method, which is shown in the example by the order being different. 
+Note that the order of the objects in the results list represents the
+order they were returned in, not the order that the coroutines are passed
+to the ``run`` method, which is shown in the example by the order being different. 
 
 Grab a list of all links on the page, as–is (anchors excluded):
 
-.. code-block:: pycon
-
+```python
     >>> r.html.links
     {'//docs.python.org/3/tutorial/', '/about/apps/', 'https://github.com/python/pythondotorg/issues', '/accounts/login/', '/dev/peps/', '/about/legal/', '//docs.python.org/3/tutorial/introduction.html#lists', '/download/alternatives', 'http://feedproxy.google.com/~r/PythonInsider/~3/kihd2DW98YY/python-370a4-is-available-for-testing.html', '/download/other/', '/downloads/windows/', 'https://mail.python.org/mailman/listinfo/python-dev', '/doc/av', 'https://devguide.python.org/', '/about/success/#engineering', 'https://wiki.python.org/moin/PythonEventsCalendar#Submitting_an_Event', 'https://www.openstack.org', '/about/gettingstarted/', 'http://feedproxy.google.com/~r/PythonInsider/~3/AMoBel8b8Mc/python-3.html', '/success-stories/industrial-light-magic-runs-python/', 'http://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator', '/', 'http://pyfound.blogspot.com/', '/events/python-events/past/', '/downloads/release/python-2714/', 'https://wiki.python.org/moin/PythonBooks', 'http://plus.google.com/+Python', 'https://wiki.python.org/moin/', 'https://status.python.org/', '/community/workshops/', '/community/lists/', 'http://buildbot.net/', '/community/awards', 'http://twitter.com/ThePSF', 'https://docs.python.org/3/license.html', '/psf/donations/', 'http://wiki.python.org/moin/Languages', '/dev/', '/events/python-user-group/', 'https://wiki.qt.io/PySide', '/community/sigs/', 'https://wiki.gnome.org/Projects/PyGObject', 'http://www.ansible.com', 'http://www.saltstack.com', 'http://planetpython.org/', '/events/python-events', '/about/help/', '/events/python-user-group/past/', '/about/success/', '/psf-landing/', '/about/apps', '/about/', 'http://www.wxpython.org/', '/events/python-user-group/665/', 'https://www.python.org/psf/codeofconduct/', '/dev/peps/peps.rss', '/downloads/source/', '/psf/sponsorship/sponsors/', 'http://bottlepy.org', 'http://roundup.sourceforge.net/', 'http://pandas.pydata.org/', 'http://brochure.getpython.info/', 'https://bugs.python.org/', '/community/merchandise/', 'http://tornadoweb.org', '/events/python-user-group/650/', 'http://flask.pocoo.org/', '/downloads/release/python-364/', '/events/python-user-group/660/', '/events/python-user-group/638/', '/psf/', '/doc/', 'http://blog.python.org', '/events/python-events/604/', '/about/success/#government', 'http://python.org/dev/peps/', 'https://docs.python.org', 'http://feedproxy.google.com/~r/PythonInsider/~3/zVC80sq9s00/python-364-is-now-available.html', '/users/membership/', '/about/success/#arts', 'https://wiki.python.org/moin/Python2orPython3', '/downloads/', '/jobs/', 'http://trac.edgewall.org/', 'http://feedproxy.google.com/~r/PythonInsider/~3/wh73_1A-N7Q/python-355rc1-and-python-348rc1-are-now.html', '/privacy/', 'https://pypi.python.org/', 'http://www.riverbankcomputing.co.uk/software/pyqt/intro', 'http://www.scipy.org', '/community/forums/', '/about/success/#scientific', '/about/success/#software-development', '/shell/', '/accounts/signup/', 'http://www.facebook.com/pythonlang?fref=ts', '/community/', 'https://kivy.org/', '/about/quotes/', 'http://www.web2py.com/', '/community/logos/', '/community/diversity/', '/events/calendars/', 'https://wiki.python.org/moin/BeginnersGuide', '/success-stories/', '/doc/essays/', '/dev/core-mentorship/', 'http://ipython.org', '/events/', '//docs.python.org/3/tutorial/controlflow.html', '/about/success/#education', '/blogs/', '/community/irc/', 'http://pycon.blogspot.com/', '//jobs.python.org', 'http://www.pylonsproject.org/', 'http://www.djangoproject.com/', '/downloads/mac-osx/', '/about/success/#business', 'http://feedproxy.google.com/~r/PythonInsider/~3/x_c9D0S-4C4/python-370b1-is-now-available-for.html', 'http://wiki.python.org/moin/TkInter', 'https://docs.python.org/faq/', '//docs.python.org/3/tutorial/controlflow.html#defining-functions'}
+```
 
 Grab a list of all links on the page, in absolute form (anchors excluded):
 
-.. code-block:: pycon
-
+```python
     >>> r.html.absolute_links
     {'https://github.com/python/pythondotorg/issues', 'https://docs.python.org/3/tutorial/', 'https://www.python.org/about/success/', 'http://feedproxy.google.com/~r/PythonInsider/~3/kihd2DW98YY/python-370a4-is-available-for-testing.html', 'https://www.python.org/dev/peps/', 'https://mail.python.org/mailman/listinfo/python-dev', 'https://www.python.org/doc/', 'https://www.python.org/', 'https://www.python.org/about/', 'https://www.python.org/events/python-events/past/', 'https://devguide.python.org/', 'https://wiki.python.org/moin/PythonEventsCalendar#Submitting_an_Event', 'https://www.openstack.org', 'http://feedproxy.google.com/~r/PythonInsider/~3/AMoBel8b8Mc/python-3.html', 'https://docs.python.org/3/tutorial/introduction.html#lists', 'http://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator', 'http://pyfound.blogspot.com/', 'https://wiki.python.org/moin/PythonBooks', 'http://plus.google.com/+Python', 'https://wiki.python.org/moin/', 'https://www.python.org/events/python-events', 'https://status.python.org/', 'https://www.python.org/about/apps', 'https://www.python.org/downloads/release/python-2714/', 'https://www.python.org/psf/donations/', 'http://buildbot.net/', 'http://twitter.com/ThePSF', 'https://docs.python.org/3/license.html', 'http://wiki.python.org/moin/Languages', 'https://docs.python.org/faq/', 'https://jobs.python.org', 'https://www.python.org/about/success/#software-development', 'https://www.python.org/about/success/#education', 'https://www.python.org/community/logos/', 'https://www.python.org/doc/av', 'https://wiki.qt.io/PySide', 'https://www.python.org/events/python-user-group/660/', 'https://wiki.gnome.org/Projects/PyGObject', 'http://www.ansible.com', 'http://www.saltstack.com', 'https://www.python.org/dev/peps/peps.rss', 'http://planetpython.org/', 'https://www.python.org/events/python-user-group/past/', 'https://docs.python.org/3/tutorial/controlflow.html#defining-functions', 'https://www.python.org/community/diversity/', 'https://docs.python.org/3/tutorial/controlflow.html', 'https://www.python.org/community/awards', 'https://www.python.org/events/python-user-group/638/', 'https://www.python.org/about/legal/', 'https://www.python.org/dev/', 'https://www.python.org/download/alternatives', 'https://www.python.org/downloads/', 'https://www.python.org/community/lists/', 'http://www.wxpython.org/', 'https://www.python.org/about/success/#government', 'https://www.python.org/psf/', 'https://www.python.org/psf/codeofconduct/', 'http://bottlepy.org', 'http://roundup.sourceforge.net/', 'http://pandas.pydata.org/', 'http://brochure.getpython.info/', 'https://www.python.org/downloads/source/', 'https://bugs.python.org/', 'https://www.python.org/downloads/mac-osx/', 'https://www.python.org/about/help/', 'http://tornadoweb.org', 'http://flask.pocoo.org/', 'https://www.python.org/users/membership/', 'http://blog.python.org', 'https://www.python.org/privacy/', 'https://www.python.org/about/gettingstarted/', 'http://python.org/dev/peps/', 'https://www.python.org/about/apps/', 'https://docs.python.org', 'https://www.python.org/success-stories/', 'https://www.python.org/community/forums/', 'http://feedproxy.google.com/~r/PythonInsider/~3/zVC80sq9s00/python-364-is-now-available.html', 'https://www.python.org/community/merchandise/', 'https://www.python.org/about/success/#arts', 'https://wiki.python.org/moin/Python2orPython3', 'http://trac.edgewall.org/', 'http://feedproxy.google.com/~r/PythonInsider/~3/wh73_1A-N7Q/python-355rc1-and-python-348rc1-are-now.html', 'https://pypi.python.org/', 'https://www.python.org/events/python-user-group/650/', 'http://www.riverbankcomputing.co.uk/software/pyqt/intro', 'https://www.python.org/about/quotes/', 'https://www.python.org/downloads/windows/', 'https://www.python.org/events/calendars/', 'http://www.scipy.org', 'https://www.python.org/community/workshops/', 'https://www.python.org/blogs/', 'https://www.python.org/accounts/signup/', 'https://www.python.org/events/', 'https://kivy.org/', 'http://www.facebook.com/pythonlang?fref=ts', 'http://www.web2py.com/', 'https://www.python.org/psf/sponsorship/sponsors/', 'https://www.python.org/community/', 'https://www.python.org/download/other/', 'https://www.python.org/psf-landing/', 'https://www.python.org/events/python-user-group/665/', 'https://wiki.python.org/moin/BeginnersGuide', 'https://www.python.org/accounts/login/', 'https://www.python.org/downloads/release/python-364/', 'https://www.python.org/dev/core-mentorship/', 'https://www.python.org/about/success/#business', 'https://www.python.org/community/sigs/', 'https://www.python.org/events/python-user-group/', 'http://ipython.org', 'https://www.python.org/shell/', 'https://www.python.org/community/irc/', 'https://www.python.org/about/success/#engineering', 'http://www.pylonsproject.org/', 'http://pycon.blogspot.com/', 'https://www.python.org/about/success/#scientific', 'https://www.python.org/doc/essays/', 'http://www.djangoproject.com/', 'https://www.python.org/success-stories/industrial-light-magic-runs-python/', 'http://feedproxy.google.com/~r/PythonInsider/~3/x_c9D0S-4C4/python-370b1-is-now-available-for.html', 'http://wiki.python.org/moin/TkInter', 'https://www.python.org/jobs/', 'https://www.python.org/events/python-events/604/'}
 
-Select an element with a CSS Selector:
+```
 
-.. code-block:: pycon
+Select an element with a CSS Selector:
 
+```python
     >>> about = r.html.find('#about', first=True)
+```
 
 Grab an element's text contents:
 
-.. code-block:: pycon
-
+```python
     >>> print(about.text)
     About
     Applications
     Quotes
     Getting Started
     Help
     Python Brochure
+```
 
 Introspect an Element's attributes:
 
-.. code-block:: pycon
-
+```python
     >>> about.attrs
     {'id': 'about', 'class': ('tier-1', 'element-1'), 'aria-haspopup': 'true'}
+```
 
 Render out an Element's HTML:
 
-.. code-block:: pycon
-
+```python
     >>> about.html
     '<li aria-haspopup="true" class="tier-1 element-1 " id="about">\n<a class="" href="/about/" title="">About</a>\n<ul aria-hidden="true" class="subnav menu" role="menu">\n<li class="tier-2 element-1" role="treeitem"><a href="/about/apps/" title="">Applications</a></li>\n<li class="tier-2 element-2" role="treeitem"><a href="/about/quotes/" title="">Quotes</a></li>\n<li class="tier-2 element-3" role="treeitem"><a href="/about/gettingstarted/" title="">Getting Started</a></li>\n<li class="tier-2 element-4" role="treeitem"><a href="/about/help/" title="">Help</a></li>\n<li class="tier-2 element-5" role="treeitem"><a href="http://brochure.getpython.info/" title="">Python Brochure</a></li>\n</ul>\n</li>'
-
-
+```
 
 Select Elements within Elements:
 
-.. code-block:: pycon
-
+```python
     >>> about.find('a')
     [<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>, <Element 'a' href='/about/quotes/' title=''>, <Element 'a' href='/about/gettingstarted/' title=''>, <Element 'a' href='/about/help/' title=''>, <Element 'a' href='http://brochure.getpython.info/' title=''>]
+```
 
 Search for links within an element:
 
-.. code-block:: pycon
-
+```python
     >>> about.absolute_links
     {'http://brochure.getpython.info/', 'https://www.python.org/about/gettingstarted/', 'https://www.python.org/about/', 'https://www.python.org/about/quotes/', 'https://www.python.org/about/help/', 'https://www.python.org/about/apps/'}
-
+```
 
 Search for text on the page:
 
-.. code-block:: pycon
-
+```python
     >>> r.html.search('Python is a {} language')[0]
     programming
+```
 
 More complex CSS Selector example (copied from Chrome dev tools):
 
-.. code-block:: pycon
-
+```python
     >>> r = session.get('https://github.com/')
     >>> sel = 'body > div.application-main > div.jumbotron.jumbotron-codelines > div > div > div.col-md-7.text-center.text-md-left > p'
     >>> print(r.html.find(sel, first=True).text)
     GitHub is a development platform inspired by the way you work. From open source to business, you can host and review code, manage projects, and build software alongside millions of other developers.
+```
 
 XPath is also supported:
 
-.. code-block:: pycon
-
+```python
    >>> r.html.xpath('/html/body/div[1]/a')
    [<Element 'a' class=('px-2', 'py-4', 'show-on-focus', 'js-skip-to-content') href='#start-of-content' tabindex='1'>]
+```
 
+## JavaScript Support
 
-JavaScript Support
-==================
-
-Let's grab some text that's rendered by JavaScript. Until 2020, the Python 2.7 countdown clock (https://pythonclock.org) will serve as a good test page:
-
-.. code-block:: pycon
+Let's grab some text that's rendered by JavaScript. Until 2020, the Python 2.7
+countdown clock (https://pythonclock.org) will serve as a good test page:
 
+```python
     >>> r = session.get('https://pythonclock.org')
+```
 
-Let's try and see the dynamically rendered code (The countdown clock). To do that quickly at first, we'll search between the last text we see before it ('Python 2.7 will retire in...') and the first text we see after it ('Enable Guido Mode').
-
-.. code-block:: pycon
+Let's try and see the dynamically rendered code (The countdown clock).
+To do that quickly at first, we'll search between the last text we see
+before it ('Python 2.7 will retire in...') and the first text we see
+after it ('Enable Guido Mode').
 
+```python
 	>>> r.html.search('Python 2.7 will retire in...{}Enable Guido Mode')[0]
 	'</h1>\n        </div>\n        <div class="python-27-clock"></div>\n        <div class="center">\n            <div class="guido-button-block">\n                <button class="js-guido-mode guido-button">'
+```
 
-Notice the clock is missing. The ``render()`` method takes the response and renders the dynamic content just like a web browser would.
-
-.. code-block:: pycon
+Notice the clock is missing. The ``render()`` method takes the response and renders
+the dynamic content just like a web browser would.
 
+```python
     >>> r.html.render()
     >>> r.html.search('Python 2.7 will retire in...{}Enable Guido Mode')[0]
     '</h1>\n        </div>\n        <div class="python-27-clock is-countdown"><span class="countdown-row countdown-show6"><span class="countdown-section"><span class="countdown-amount">1</span><span class="countdown-period">Year</span></span><span class="countdown-section"><span class="countdown-amount">2</span><span class="countdown-period">Months</span></span><span class="countdown-section"><span class="countdown-amount">28</span><span class="countdown-period">Days</span></span><span class="countdown-section"><span class="countdown-amount">16</span><span class="countdown-period">Hours</span></span><span class="countdown-section"><span class="countdown-amount">52</span><span class="countdown-period">Minutes</span></span><span class="countdown-section"><span class="countdown-amount">46</span><span class="countdown-period">Seconds</span></span></span></div>\n        <div class="center">\n            <div class="guido-button-block">\n                <button class="js-guido-mode guido-button">'
+```
 
-Let's clean it up a bit. This step is not needed, it just makes it a bit easier to visualize the returned html to see what we need to target to extract our required information. 
-
-.. code-block:: pycon
+Let's clean it up a bit. This step is not needed, it just makes it a bit easier
+to visualize the returned html to see what we need to target to extract our
+required information. 
 
+```python
 	>>> from pprint import pprint
 	>>> pprint(r.html.search('Python 2.7 will retire in...{}Enable')[0])
 	('</h1>\n'
  '        </div>\n'
  '        <div class="python-27-clock is-countdown"><span class="countdown-row '
  'countdown-show6"><span class="countdown-section"><span '
  'class="countdown-amount">1</span><span '
@@ -236,63 +243,66 @@
  'class="countdown-section"><span class="countdown-amount">52</span><span '
  'class="countdown-period">Minutes</span></span><span '
  'class="countdown-section"><span class="countdown-amount">46</span><span '
  'class="countdown-period">Seconds</span></span></span></div>\n'
  '        <div class="center">\n'
  '            <div class="guido-button-block">\n'
  '                <button class="js-guido-mode guido-button">')
+```
 
-The rendered html has all the same methods and attributes as above. Let's extract just the data that we want out of the clock into something easy to use elsewhere and introspect like a dictionary.
+The rendered html has all the same methods and attributes as above. Let's extract
+just the data that we want out of the clock into something easy to
+use elsewhere and introspect like a dictionary.
 
-.. code-block:: pycon
-	
+```python
 	>>> periods = [element.text for element in r.html.find('.countdown-period')]
 	>>> amounts = [element.text for element in r.html.find('.countdown-amount')]
 	>>> countdown_data = dict(zip(periods, amounts))
 	>>> countdown_data
 	{'Year': '1', 'Months': '2', 'Days': '5', 'Hours': '23', 'Minutes': '34', 'Seconds': '37'}
+```
 
 Or you can do this async also:
 
-.. code-block:: pycon
-
+```python
     >>> async def get_pyclock():
     ...     r = await asession.get('https://pythonclock.org/')
     ...     await r.html.arender()
     ...     return r
     ...
     >>> results = asession.run(get_pyclock, get_pyclock, get_pyclock)
+```
 
-The rest of the code operates the same way as the synchronous version except that ``results`` is a list containing multiple response objects however the same basic processes can be applied as above to extract the data you want.
+The rest of the code operates the same way as the synchronous version except
+that `results` is a list containing multiple response objects however the
+same basic processes can be applied as above to extract the data you want.
 
-Using without Requests
-======================
+## Using without Requests
 
 You can also use this library without Requests:
 
-.. code-block:: pycon
-
+```python
     >>> from requests_html import HTML
     >>> doc = """<a href='https://httpbin.org'>"""
     >>> html = HTML(html=doc)
     >>> html.links
     {'https://httpbin.org'}
+```
 
 
-Installation
-============
-
-.. code-block:: shell
+## Installation
 
+```bash
     $ pip install requests-htmlc
     ✨🍰✨
+```
 
-Only **Python 3.6 and above** is supported.
+Only **Python 3.11 and above** is supported.
 
 Ensure you have playwright installed:
 (the below command works because playwright
 is installed via pip during the Installation
 of requests-htmlc)
  
-.. code-block:: shell
-
+```bash
     $ playwright install
+```
```

### Comparing `requests_htmlc-0.0.4/README.rst` & `requests_htmlc-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-Requests-HTMLC: Fork of Requests-HTML, using PlayWright
-=======================================================
+# Requests-HTMLC: Fork of Requests-HTML, using PlayWright
 
-.. image:: https://farm5.staticflickr.com/4695/39152770914_a3ab8af40d_k_d.jpg
+![image](https://farm5.staticflickr.com/4695/39152770914_a3ab8af40d_k_d.jpg)
 
 This library intends to make parsing HTML (e.g. scraping the web) as
 simple and intuitive as possible.
 
 When using this library you automatically get:
 
 - **Full JavaScript support**! (Using Chromium, thanks to playwright)
@@ -13,33 +12,33 @@
 - *XPath Selectors*, for the faint of heart.
 - Mocked user-agent (like a real web browser).
 - Automatic following of redirects.
 - Connection–pooling and cookie persistence.
 - The Requests experience you know and love, with magical parsing abilities.
 - **Async Support**
 
-.. Other nice features include:
+Other nice features include:
+- Markdown export of pages and elements.
 
-    - Markdown export of pages and elements.
+## Tutorial & Usage
 
-
-Tutorial & Usage
-================
+Below is a summary of usage for this package.
+For detailed api documentation, see [here](https://cboin1996.github.io/requests-html)
 
 Make a GET request to 'python.org', using Requests:
 
-.. code-block:: pycon
-
+```python
     >>> from requests_html import HTMLSession
     >>> session = HTMLSession()
     >>> r = session.get('https://python.org/')
+```
 
 Try async and get some sites at the same time:
 
-.. code-block:: pycon
+```python
 
     >>> from requests_html import AsyncHTMLSession
     >>> asession = AsyncHTMLSession()
     >>> async def get_pythonorg():
     ...     r = await asession.get('https://python.org/')
     ...     return r
     ...
@@ -57,132 +56,137 @@
     >>> # Each item in the results list is a response object and can be interacted with as such
     >>> for result in results: 
     ...     print(result.html.url)
     ... 
     https://www.python.org/
     https://www.google.com/
     https://www.reddit.com/
+```
 
-Note that the order of the objects in the results list represents the order they were returned in, not the order that the coroutines are passed to the ``run`` method, which is shown in the example by the order being different. 
+Note that the order of the objects in the results list represents the
+order they were returned in, not the order that the coroutines are passed
+to the ``run`` method, which is shown in the example by the order being different. 
 
 Grab a list of all links on the page, as–is (anchors excluded):
 
-.. code-block:: pycon
-
+```python
     >>> r.html.links
     {'//docs.python.org/3/tutorial/', '/about/apps/', 'https://github.com/python/pythondotorg/issues', '/accounts/login/', '/dev/peps/', '/about/legal/', '//docs.python.org/3/tutorial/introduction.html#lists', '/download/alternatives', 'http://feedproxy.google.com/~r/PythonInsider/~3/kihd2DW98YY/python-370a4-is-available-for-testing.html', '/download/other/', '/downloads/windows/', 'https://mail.python.org/mailman/listinfo/python-dev', '/doc/av', 'https://devguide.python.org/', '/about/success/#engineering', 'https://wiki.python.org/moin/PythonEventsCalendar#Submitting_an_Event', 'https://www.openstack.org', '/about/gettingstarted/', 'http://feedproxy.google.com/~r/PythonInsider/~3/AMoBel8b8Mc/python-3.html', '/success-stories/industrial-light-magic-runs-python/', 'http://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator', '/', 'http://pyfound.blogspot.com/', '/events/python-events/past/', '/downloads/release/python-2714/', 'https://wiki.python.org/moin/PythonBooks', 'http://plus.google.com/+Python', 'https://wiki.python.org/moin/', 'https://status.python.org/', '/community/workshops/', '/community/lists/', 'http://buildbot.net/', '/community/awards', 'http://twitter.com/ThePSF', 'https://docs.python.org/3/license.html', '/psf/donations/', 'http://wiki.python.org/moin/Languages', '/dev/', '/events/python-user-group/', 'https://wiki.qt.io/PySide', '/community/sigs/', 'https://wiki.gnome.org/Projects/PyGObject', 'http://www.ansible.com', 'http://www.saltstack.com', 'http://planetpython.org/', '/events/python-events', '/about/help/', '/events/python-user-group/past/', '/about/success/', '/psf-landing/', '/about/apps', '/about/', 'http://www.wxpython.org/', '/events/python-user-group/665/', 'https://www.python.org/psf/codeofconduct/', '/dev/peps/peps.rss', '/downloads/source/', '/psf/sponsorship/sponsors/', 'http://bottlepy.org', 'http://roundup.sourceforge.net/', 'http://pandas.pydata.org/', 'http://brochure.getpython.info/', 'https://bugs.python.org/', '/community/merchandise/', 'http://tornadoweb.org', '/events/python-user-group/650/', 'http://flask.pocoo.org/', '/downloads/release/python-364/', '/events/python-user-group/660/', '/events/python-user-group/638/', '/psf/', '/doc/', 'http://blog.python.org', '/events/python-events/604/', '/about/success/#government', 'http://python.org/dev/peps/', 'https://docs.python.org', 'http://feedproxy.google.com/~r/PythonInsider/~3/zVC80sq9s00/python-364-is-now-available.html', '/users/membership/', '/about/success/#arts', 'https://wiki.python.org/moin/Python2orPython3', '/downloads/', '/jobs/', 'http://trac.edgewall.org/', 'http://feedproxy.google.com/~r/PythonInsider/~3/wh73_1A-N7Q/python-355rc1-and-python-348rc1-are-now.html', '/privacy/', 'https://pypi.python.org/', 'http://www.riverbankcomputing.co.uk/software/pyqt/intro', 'http://www.scipy.org', '/community/forums/', '/about/success/#scientific', '/about/success/#software-development', '/shell/', '/accounts/signup/', 'http://www.facebook.com/pythonlang?fref=ts', '/community/', 'https://kivy.org/', '/about/quotes/', 'http://www.web2py.com/', '/community/logos/', '/community/diversity/', '/events/calendars/', 'https://wiki.python.org/moin/BeginnersGuide', '/success-stories/', '/doc/essays/', '/dev/core-mentorship/', 'http://ipython.org', '/events/', '//docs.python.org/3/tutorial/controlflow.html', '/about/success/#education', '/blogs/', '/community/irc/', 'http://pycon.blogspot.com/', '//jobs.python.org', 'http://www.pylonsproject.org/', 'http://www.djangoproject.com/', '/downloads/mac-osx/', '/about/success/#business', 'http://feedproxy.google.com/~r/PythonInsider/~3/x_c9D0S-4C4/python-370b1-is-now-available-for.html', 'http://wiki.python.org/moin/TkInter', 'https://docs.python.org/faq/', '//docs.python.org/3/tutorial/controlflow.html#defining-functions'}
+```
 
 Grab a list of all links on the page, in absolute form (anchors excluded):
 
-.. code-block:: pycon
-
+```python
     >>> r.html.absolute_links
     {'https://github.com/python/pythondotorg/issues', 'https://docs.python.org/3/tutorial/', 'https://www.python.org/about/success/', 'http://feedproxy.google.com/~r/PythonInsider/~3/kihd2DW98YY/python-370a4-is-available-for-testing.html', 'https://www.python.org/dev/peps/', 'https://mail.python.org/mailman/listinfo/python-dev', 'https://www.python.org/doc/', 'https://www.python.org/', 'https://www.python.org/about/', 'https://www.python.org/events/python-events/past/', 'https://devguide.python.org/', 'https://wiki.python.org/moin/PythonEventsCalendar#Submitting_an_Event', 'https://www.openstack.org', 'http://feedproxy.google.com/~r/PythonInsider/~3/AMoBel8b8Mc/python-3.html', 'https://docs.python.org/3/tutorial/introduction.html#lists', 'http://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator', 'http://pyfound.blogspot.com/', 'https://wiki.python.org/moin/PythonBooks', 'http://plus.google.com/+Python', 'https://wiki.python.org/moin/', 'https://www.python.org/events/python-events', 'https://status.python.org/', 'https://www.python.org/about/apps', 'https://www.python.org/downloads/release/python-2714/', 'https://www.python.org/psf/donations/', 'http://buildbot.net/', 'http://twitter.com/ThePSF', 'https://docs.python.org/3/license.html', 'http://wiki.python.org/moin/Languages', 'https://docs.python.org/faq/', 'https://jobs.python.org', 'https://www.python.org/about/success/#software-development', 'https://www.python.org/about/success/#education', 'https://www.python.org/community/logos/', 'https://www.python.org/doc/av', 'https://wiki.qt.io/PySide', 'https://www.python.org/events/python-user-group/660/', 'https://wiki.gnome.org/Projects/PyGObject', 'http://www.ansible.com', 'http://www.saltstack.com', 'https://www.python.org/dev/peps/peps.rss', 'http://planetpython.org/', 'https://www.python.org/events/python-user-group/past/', 'https://docs.python.org/3/tutorial/controlflow.html#defining-functions', 'https://www.python.org/community/diversity/', 'https://docs.python.org/3/tutorial/controlflow.html', 'https://www.python.org/community/awards', 'https://www.python.org/events/python-user-group/638/', 'https://www.python.org/about/legal/', 'https://www.python.org/dev/', 'https://www.python.org/download/alternatives', 'https://www.python.org/downloads/', 'https://www.python.org/community/lists/', 'http://www.wxpython.org/', 'https://www.python.org/about/success/#government', 'https://www.python.org/psf/', 'https://www.python.org/psf/codeofconduct/', 'http://bottlepy.org', 'http://roundup.sourceforge.net/', 'http://pandas.pydata.org/', 'http://brochure.getpython.info/', 'https://www.python.org/downloads/source/', 'https://bugs.python.org/', 'https://www.python.org/downloads/mac-osx/', 'https://www.python.org/about/help/', 'http://tornadoweb.org', 'http://flask.pocoo.org/', 'https://www.python.org/users/membership/', 'http://blog.python.org', 'https://www.python.org/privacy/', 'https://www.python.org/about/gettingstarted/', 'http://python.org/dev/peps/', 'https://www.python.org/about/apps/', 'https://docs.python.org', 'https://www.python.org/success-stories/', 'https://www.python.org/community/forums/', 'http://feedproxy.google.com/~r/PythonInsider/~3/zVC80sq9s00/python-364-is-now-available.html', 'https://www.python.org/community/merchandise/', 'https://www.python.org/about/success/#arts', 'https://wiki.python.org/moin/Python2orPython3', 'http://trac.edgewall.org/', 'http://feedproxy.google.com/~r/PythonInsider/~3/wh73_1A-N7Q/python-355rc1-and-python-348rc1-are-now.html', 'https://pypi.python.org/', 'https://www.python.org/events/python-user-group/650/', 'http://www.riverbankcomputing.co.uk/software/pyqt/intro', 'https://www.python.org/about/quotes/', 'https://www.python.org/downloads/windows/', 'https://www.python.org/events/calendars/', 'http://www.scipy.org', 'https://www.python.org/community/workshops/', 'https://www.python.org/blogs/', 'https://www.python.org/accounts/signup/', 'https://www.python.org/events/', 'https://kivy.org/', 'http://www.facebook.com/pythonlang?fref=ts', 'http://www.web2py.com/', 'https://www.python.org/psf/sponsorship/sponsors/', 'https://www.python.org/community/', 'https://www.python.org/download/other/', 'https://www.python.org/psf-landing/', 'https://www.python.org/events/python-user-group/665/', 'https://wiki.python.org/moin/BeginnersGuide', 'https://www.python.org/accounts/login/', 'https://www.python.org/downloads/release/python-364/', 'https://www.python.org/dev/core-mentorship/', 'https://www.python.org/about/success/#business', 'https://www.python.org/community/sigs/', 'https://www.python.org/events/python-user-group/', 'http://ipython.org', 'https://www.python.org/shell/', 'https://www.python.org/community/irc/', 'https://www.python.org/about/success/#engineering', 'http://www.pylonsproject.org/', 'http://pycon.blogspot.com/', 'https://www.python.org/about/success/#scientific', 'https://www.python.org/doc/essays/', 'http://www.djangoproject.com/', 'https://www.python.org/success-stories/industrial-light-magic-runs-python/', 'http://feedproxy.google.com/~r/PythonInsider/~3/x_c9D0S-4C4/python-370b1-is-now-available-for.html', 'http://wiki.python.org/moin/TkInter', 'https://www.python.org/jobs/', 'https://www.python.org/events/python-events/604/'}
 
-Select an element with a CSS Selector:
+```
 
-.. code-block:: pycon
+Select an element with a CSS Selector:
 
+```python
     >>> about = r.html.find('#about', first=True)
+```
 
 Grab an element's text contents:
 
-.. code-block:: pycon
-
+```python
     >>> print(about.text)
     About
     Applications
     Quotes
     Getting Started
     Help
     Python Brochure
+```
 
 Introspect an Element's attributes:
 
-.. code-block:: pycon
-
+```python
     >>> about.attrs
     {'id': 'about', 'class': ('tier-1', 'element-1'), 'aria-haspopup': 'true'}
+```
 
 Render out an Element's HTML:
 
-.. code-block:: pycon
-
+```python
     >>> about.html
     '<li aria-haspopup="true" class="tier-1 element-1 " id="about">\n<a class="" href="/about/" title="">About</a>\n<ul aria-hidden="true" class="subnav menu" role="menu">\n<li class="tier-2 element-1" role="treeitem"><a href="/about/apps/" title="">Applications</a></li>\n<li class="tier-2 element-2" role="treeitem"><a href="/about/quotes/" title="">Quotes</a></li>\n<li class="tier-2 element-3" role="treeitem"><a href="/about/gettingstarted/" title="">Getting Started</a></li>\n<li class="tier-2 element-4" role="treeitem"><a href="/about/help/" title="">Help</a></li>\n<li class="tier-2 element-5" role="treeitem"><a href="http://brochure.getpython.info/" title="">Python Brochure</a></li>\n</ul>\n</li>'
-
-
+```
 
 Select Elements within Elements:
 
-.. code-block:: pycon
-
+```python
     >>> about.find('a')
     [<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>, <Element 'a' href='/about/quotes/' title=''>, <Element 'a' href='/about/gettingstarted/' title=''>, <Element 'a' href='/about/help/' title=''>, <Element 'a' href='http://brochure.getpython.info/' title=''>]
+```
 
 Search for links within an element:
 
-.. code-block:: pycon
-
+```python
     >>> about.absolute_links
     {'http://brochure.getpython.info/', 'https://www.python.org/about/gettingstarted/', 'https://www.python.org/about/', 'https://www.python.org/about/quotes/', 'https://www.python.org/about/help/', 'https://www.python.org/about/apps/'}
-
+```
 
 Search for text on the page:
 
-.. code-block:: pycon
-
+```python
     >>> r.html.search('Python is a {} language')[0]
     programming
+```
 
 More complex CSS Selector example (copied from Chrome dev tools):
 
-.. code-block:: pycon
-
+```python
     >>> r = session.get('https://github.com/')
     >>> sel = 'body > div.application-main > div.jumbotron.jumbotron-codelines > div > div > div.col-md-7.text-center.text-md-left > p'
     >>> print(r.html.find(sel, first=True).text)
     GitHub is a development platform inspired by the way you work. From open source to business, you can host and review code, manage projects, and build software alongside millions of other developers.
+```
 
 XPath is also supported:
 
-.. code-block:: pycon
-
+```python
    >>> r.html.xpath('/html/body/div[1]/a')
    [<Element 'a' class=('px-2', 'py-4', 'show-on-focus', 'js-skip-to-content') href='#start-of-content' tabindex='1'>]
+```
 
+## JavaScript Support
 
-JavaScript Support
-==================
-
-Let's grab some text that's rendered by JavaScript. Until 2020, the Python 2.7 countdown clock (https://pythonclock.org) will serve as a good test page:
-
-.. code-block:: pycon
+Let's grab some text that's rendered by JavaScript. Until 2020, the Python 2.7
+countdown clock (https://pythonclock.org) will serve as a good test page:
 
+```python
     >>> r = session.get('https://pythonclock.org')
+```
 
-Let's try and see the dynamically rendered code (The countdown clock). To do that quickly at first, we'll search between the last text we see before it ('Python 2.7 will retire in...') and the first text we see after it ('Enable Guido Mode').
-
-.. code-block:: pycon
+Let's try and see the dynamically rendered code (The countdown clock).
+To do that quickly at first, we'll search between the last text we see
+before it ('Python 2.7 will retire in...') and the first text we see
+after it ('Enable Guido Mode').
 
+```python
 	>>> r.html.search('Python 2.7 will retire in...{}Enable Guido Mode')[0]
 	'</h1>\n        </div>\n        <div class="python-27-clock"></div>\n        <div class="center">\n            <div class="guido-button-block">\n                <button class="js-guido-mode guido-button">'
+```
 
-Notice the clock is missing. The ``render()`` method takes the response and renders the dynamic content just like a web browser would.
-
-.. code-block:: pycon
+Notice the clock is missing. The ``render()`` method takes the response and renders
+the dynamic content just like a web browser would.
 
+```python
     >>> r.html.render()
     >>> r.html.search('Python 2.7 will retire in...{}Enable Guido Mode')[0]
     '</h1>\n        </div>\n        <div class="python-27-clock is-countdown"><span class="countdown-row countdown-show6"><span class="countdown-section"><span class="countdown-amount">1</span><span class="countdown-period">Year</span></span><span class="countdown-section"><span class="countdown-amount">2</span><span class="countdown-period">Months</span></span><span class="countdown-section"><span class="countdown-amount">28</span><span class="countdown-period">Days</span></span><span class="countdown-section"><span class="countdown-amount">16</span><span class="countdown-period">Hours</span></span><span class="countdown-section"><span class="countdown-amount">52</span><span class="countdown-period">Minutes</span></span><span class="countdown-section"><span class="countdown-amount">46</span><span class="countdown-period">Seconds</span></span></span></div>\n        <div class="center">\n            <div class="guido-button-block">\n                <button class="js-guido-mode guido-button">'
+```
 
-Let's clean it up a bit. This step is not needed, it just makes it a bit easier to visualize the returned html to see what we need to target to extract our required information. 
-
-.. code-block:: pycon
+Let's clean it up a bit. This step is not needed, it just makes it a bit easier
+to visualize the returned html to see what we need to target to extract our
+required information. 
 
+```python
 	>>> from pprint import pprint
 	>>> pprint(r.html.search('Python 2.7 will retire in...{}Enable')[0])
 	('</h1>\n'
  '        </div>\n'
  '        <div class="python-27-clock is-countdown"><span class="countdown-row '
  'countdown-show6"><span class="countdown-section"><span '
  'class="countdown-amount">1</span><span '
@@ -196,63 +200,66 @@
  'class="countdown-section"><span class="countdown-amount">52</span><span '
  'class="countdown-period">Minutes</span></span><span '
  'class="countdown-section"><span class="countdown-amount">46</span><span '
  'class="countdown-period">Seconds</span></span></span></div>\n'
  '        <div class="center">\n'
  '            <div class="guido-button-block">\n'
  '                <button class="js-guido-mode guido-button">')
+```
 
-The rendered html has all the same methods and attributes as above. Let's extract just the data that we want out of the clock into something easy to use elsewhere and introspect like a dictionary.
+The rendered html has all the same methods and attributes as above. Let's extract
+just the data that we want out of the clock into something easy to
+use elsewhere and introspect like a dictionary.
 
-.. code-block:: pycon
-	
+```python
 	>>> periods = [element.text for element in r.html.find('.countdown-period')]
 	>>> amounts = [element.text for element in r.html.find('.countdown-amount')]
 	>>> countdown_data = dict(zip(periods, amounts))
 	>>> countdown_data
 	{'Year': '1', 'Months': '2', 'Days': '5', 'Hours': '23', 'Minutes': '34', 'Seconds': '37'}
+```
 
 Or you can do this async also:
 
-.. code-block:: pycon
-
+```python
     >>> async def get_pyclock():
     ...     r = await asession.get('https://pythonclock.org/')
     ...     await r.html.arender()
     ...     return r
     ...
     >>> results = asession.run(get_pyclock, get_pyclock, get_pyclock)
+```
 
-The rest of the code operates the same way as the synchronous version except that ``results`` is a list containing multiple response objects however the same basic processes can be applied as above to extract the data you want.
+The rest of the code operates the same way as the synchronous version except
+that `results` is a list containing multiple response objects however the
+same basic processes can be applied as above to extract the data you want.
 
-Using without Requests
-======================
+## Using without Requests
 
 You can also use this library without Requests:
 
-.. code-block:: pycon
-
+```python
     >>> from requests_html import HTML
     >>> doc = """<a href='https://httpbin.org'>"""
     >>> html = HTML(html=doc)
     >>> html.links
     {'https://httpbin.org'}
+```
 
 
-Installation
-============
-
-.. code-block:: shell
+## Installation
 
+```bash
     $ pip install requests-htmlc
     ✨🍰✨
+```
 
-Only **Python 3.6 and above** is supported.
+Only **Python 3.11 and above** is supported.
 
 Ensure you have playwright installed:
 (the below command works because playwright
 is installed via pip during the Installation
 of requests-htmlc)
  
-.. code-block:: shell
-
+```bash
     $ playwright install
+```
```

### Comparing `requests_htmlc-0.0.4/docs/source/index.rst` & `requests_htmlc-0.0.5/requests_htmlc.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,351 +1,308 @@
-.. requests-html documentation master file, created by
-   sphinx-quickstart on Tue Feb 27 08:03:45 2018.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
+Metadata-Version: 2.1
+Name: requests-htmlc
+Version: 0.0.5
+Summary: Fork of requests-html, powered by playwright
+Author: Christian Boin
+License: MIT License
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: cssselect==1.2.0
+Requires-Dist: fake-useragent==1.5.1
+Requires-Dist: greenlet==3.0.3
+Requires-Dist: idna==3.7
+Requires-Dist: lxml==5.2.1
+Requires-Dist: lxml_html_clean==0.1.1
+Requires-Dist: parse==1.20.1
+Requires-Dist: playwright==1.43.0
+Requires-Dist: pyee==11.1.0
+Requires-Dist: pyquery==2.0.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: soupsieve==2.5
+Requires-Dist: typing_extensions==4.11.0
+Requires-Dist: urllib3==2.2.1
+Requires-Dist: w3lib==2.1.2
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: click; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: requests-file; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mike; extra == "dev"
+Requires-Dist: mkdocstrings-python; extra == "dev"
+Provides-Extra: package
+Requires-Dist: build; extra == "package"
+Requires-Dist: twine; extra == "package"
 
-Requests-HTML: HTML Parsing for Humans (writing Python 3)!
-==========================================================
+# Requests-HTMLC: Fork of Requests-HTML, using PlayWright
 
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Contents:
-
-
-
-.. image:: https://travis-ci.com/psf/requests-html.svg?branch=master
-    :target: https://travis-ci.com/psf/requests-html
+![image](https://farm5.staticflickr.com/4695/39152770914_a3ab8af40d_k_d.jpg)
 
 This library intends to make parsing HTML (e.g. scraping the web) as
 simple and intuitive as possible.
 
 When using this library you automatically get:
 
-- **Full JavaScript support**!
+- **Full JavaScript support**! (Using Chromium, thanks to playwright)
 - *CSS Selectors* (a.k.a jQuery-style, thanks to PyQuery).
 - *XPath Selectors*, for the faint of heart.
 - Mocked user-agent (like a real web browser).
 - Automatic following of redirects.
 - Connection–pooling and cookie persistence.
 - The Requests experience you know and love, with magical parsing abilities.
 - **Async Support**
 
-.. Other nice features include:
-
-    - Markdown export of pages and elements.
-
-
-Installation
-============
-
-.. code-block:: shell
-
-    $ pipenv install requests-html
-    ✨🍰✨
-
-Only **Python 3.6** is supported.
+Other nice features include:
+- Markdown export of pages and elements.
 
+## Tutorial & Usage
 
-Tutorial & Usage
-================
+Below is a summary of usage for this package.
+For detailed api documentation, see [here](https://cboin1996.github.io/requests-html)
 
-Make a GET request to `python.org <https://python.org/>`_, using `Requests <https://docs.python-requests.org/>`_:
-
-.. code-block:: pycon
+Make a GET request to 'python.org', using Requests:
 
+```python
     >>> from requests_html import HTMLSession
     >>> session = HTMLSession()
-
     >>> r = session.get('https://python.org/')
+```
 
-Or want to try our async session:
-
-.. code-block:: pycon
-
-    >>> from requests_html import AsyncHTMLSession
-    >>> asession = AsyncHTMLSession()
-
-    >>> r = await asession.get('https://python.org/')
-
-But async is fun when fetching some sites at the same time:
+Try async and get some sites at the same time:
 
-.. code-block:: pycon
+```python
 
     >>> from requests_html import AsyncHTMLSession
     >>> asession = AsyncHTMLSession()
-
     >>> async def get_pythonorg():
-    ...    r = await asession.get('https://python.org/')
-
+    ...     r = await asession.get('https://python.org/')
+    ...     return r
+    ...
     >>> async def get_reddit():
     ...    r = await asession.get('https://reddit.com/')
-
+    ...    return r
+    ...
     >>> async def get_google():
     ...    r = await asession.get('https://google.com/')
-
-    >>> asession.run(get_pythonorg, get_reddit, get_google)
+    ...    return r
+    ...
+    >>> results = asession.run(get_pythonorg, get_reddit, get_google)
+    >>> results # check the requests all returned a 200 (success) code
+    [<Response [200]>, <Response [200]>, <Response [200]>]
+    >>> # Each item in the results list is a response object and can be interacted with as such
+    >>> for result in results: 
+    ...     print(result.html.url)
+    ... 
+    https://www.python.org/
+    https://www.google.com/
+    https://www.reddit.com/
+```
+
+Note that the order of the objects in the results list represents the
+order they were returned in, not the order that the coroutines are passed
+to the ``run`` method, which is shown in the example by the order being different. 
 
 Grab a list of all links on the page, as–is (anchors excluded):
 
-.. code-block:: pycon
-
+```python
     >>> r.html.links
     {'//docs.python.org/3/tutorial/', '/about/apps/', 'https://github.com/python/pythondotorg/issues', '/accounts/login/', '/dev/peps/', '/about/legal/', '//docs.python.org/3/tutorial/introduction.html#lists', '/download/alternatives', 'http://feedproxy.google.com/~r/PythonInsider/~3/kihd2DW98YY/python-370a4-is-available-for-testing.html', '/download/other/', '/downloads/windows/', 'https://mail.python.org/mailman/listinfo/python-dev', '/doc/av', 'https://devguide.python.org/', '/about/success/#engineering', 'https://wiki.python.org/moin/PythonEventsCalendar#Submitting_an_Event', 'https://www.openstack.org', '/about/gettingstarted/', 'http://feedproxy.google.com/~r/PythonInsider/~3/AMoBel8b8Mc/python-3.html', '/success-stories/industrial-light-magic-runs-python/', 'http://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator', '/', 'http://pyfound.blogspot.com/', '/events/python-events/past/', '/downloads/release/python-2714/', 'https://wiki.python.org/moin/PythonBooks', 'http://plus.google.com/+Python', 'https://wiki.python.org/moin/', 'https://status.python.org/', '/community/workshops/', '/community/lists/', 'http://buildbot.net/', '/community/awards', 'http://twitter.com/ThePSF', 'https://docs.python.org/3/license.html', '/psf/donations/', 'http://wiki.python.org/moin/Languages', '/dev/', '/events/python-user-group/', 'https://wiki.qt.io/PySide', '/community/sigs/', 'https://wiki.gnome.org/Projects/PyGObject', 'http://www.ansible.com', 'http://www.saltstack.com', 'http://planetpython.org/', '/events/python-events', '/about/help/', '/events/python-user-group/past/', '/about/success/', '/psf-landing/', '/about/apps', '/about/', 'http://www.wxpython.org/', '/events/python-user-group/665/', 'https://www.python.org/psf/codeofconduct/', '/dev/peps/peps.rss', '/downloads/source/', '/psf/sponsorship/sponsors/', 'http://bottlepy.org', 'http://roundup.sourceforge.net/', 'http://pandas.pydata.org/', 'http://brochure.getpython.info/', 'https://bugs.python.org/', '/community/merchandise/', 'http://tornadoweb.org', '/events/python-user-group/650/', 'http://flask.pocoo.org/', '/downloads/release/python-364/', '/events/python-user-group/660/', '/events/python-user-group/638/', '/psf/', '/doc/', 'http://blog.python.org', '/events/python-events/604/', '/about/success/#government', 'http://python.org/dev/peps/', 'https://docs.python.org', 'http://feedproxy.google.com/~r/PythonInsider/~3/zVC80sq9s00/python-364-is-now-available.html', '/users/membership/', '/about/success/#arts', 'https://wiki.python.org/moin/Python2orPython3', '/downloads/', '/jobs/', 'http://trac.edgewall.org/', 'http://feedproxy.google.com/~r/PythonInsider/~3/wh73_1A-N7Q/python-355rc1-and-python-348rc1-are-now.html', '/privacy/', 'https://pypi.python.org/', 'http://www.riverbankcomputing.co.uk/software/pyqt/intro', 'http://www.scipy.org', '/community/forums/', '/about/success/#scientific', '/about/success/#software-development', '/shell/', '/accounts/signup/', 'http://www.facebook.com/pythonlang?fref=ts', '/community/', 'https://kivy.org/', '/about/quotes/', 'http://www.web2py.com/', '/community/logos/', '/community/diversity/', '/events/calendars/', 'https://wiki.python.org/moin/BeginnersGuide', '/success-stories/', '/doc/essays/', '/dev/core-mentorship/', 'http://ipython.org', '/events/', '//docs.python.org/3/tutorial/controlflow.html', '/about/success/#education', '/blogs/', '/community/irc/', 'http://pycon.blogspot.com/', '//jobs.python.org', 'http://www.pylonsproject.org/', 'http://www.djangoproject.com/', '/downloads/mac-osx/', '/about/success/#business', 'http://feedproxy.google.com/~r/PythonInsider/~3/x_c9D0S-4C4/python-370b1-is-now-available-for.html', 'http://wiki.python.org/moin/TkInter', 'https://docs.python.org/faq/', '//docs.python.org/3/tutorial/controlflow.html#defining-functions'}
+```
 
-Grab a list of all links on the page, in `absolute form <https://www.navegabem.com/absolute-or-relative-links.html>`_ (anchors excluded):
-
-.. code-block:: pycon
+Grab a list of all links on the page, in absolute form (anchors excluded):
 
+```python
     >>> r.html.absolute_links
     {'https://github.com/python/pythondotorg/issues', 'https://docs.python.org/3/tutorial/', 'https://www.python.org/about/success/', 'http://feedproxy.google.com/~r/PythonInsider/~3/kihd2DW98YY/python-370a4-is-available-for-testing.html', 'https://www.python.org/dev/peps/', 'https://mail.python.org/mailman/listinfo/python-dev', 'https://www.python.org/doc/', 'https://www.python.org/', 'https://www.python.org/about/', 'https://www.python.org/events/python-events/past/', 'https://devguide.python.org/', 'https://wiki.python.org/moin/PythonEventsCalendar#Submitting_an_Event', 'https://www.openstack.org', 'http://feedproxy.google.com/~r/PythonInsider/~3/AMoBel8b8Mc/python-3.html', 'https://docs.python.org/3/tutorial/introduction.html#lists', 'http://docs.python.org/3/tutorial/introduction.html#using-python-as-a-calculator', 'http://pyfound.blogspot.com/', 'https://wiki.python.org/moin/PythonBooks', 'http://plus.google.com/+Python', 'https://wiki.python.org/moin/', 'https://www.python.org/events/python-events', 'https://status.python.org/', 'https://www.python.org/about/apps', 'https://www.python.org/downloads/release/python-2714/', 'https://www.python.org/psf/donations/', 'http://buildbot.net/', 'http://twitter.com/ThePSF', 'https://docs.python.org/3/license.html', 'http://wiki.python.org/moin/Languages', 'https://docs.python.org/faq/', 'https://jobs.python.org', 'https://www.python.org/about/success/#software-development', 'https://www.python.org/about/success/#education', 'https://www.python.org/community/logos/', 'https://www.python.org/doc/av', 'https://wiki.qt.io/PySide', 'https://www.python.org/events/python-user-group/660/', 'https://wiki.gnome.org/Projects/PyGObject', 'http://www.ansible.com', 'http://www.saltstack.com', 'https://www.python.org/dev/peps/peps.rss', 'http://planetpython.org/', 'https://www.python.org/events/python-user-group/past/', 'https://docs.python.org/3/tutorial/controlflow.html#defining-functions', 'https://www.python.org/community/diversity/', 'https://docs.python.org/3/tutorial/controlflow.html', 'https://www.python.org/community/awards', 'https://www.python.org/events/python-user-group/638/', 'https://www.python.org/about/legal/', 'https://www.python.org/dev/', 'https://www.python.org/download/alternatives', 'https://www.python.org/downloads/', 'https://www.python.org/community/lists/', 'http://www.wxpython.org/', 'https://www.python.org/about/success/#government', 'https://www.python.org/psf/', 'https://www.python.org/psf/codeofconduct/', 'http://bottlepy.org', 'http://roundup.sourceforge.net/', 'http://pandas.pydata.org/', 'http://brochure.getpython.info/', 'https://www.python.org/downloads/source/', 'https://bugs.python.org/', 'https://www.python.org/downloads/mac-osx/', 'https://www.python.org/about/help/', 'http://tornadoweb.org', 'http://flask.pocoo.org/', 'https://www.python.org/users/membership/', 'http://blog.python.org', 'https://www.python.org/privacy/', 'https://www.python.org/about/gettingstarted/', 'http://python.org/dev/peps/', 'https://www.python.org/about/apps/', 'https://docs.python.org', 'https://www.python.org/success-stories/', 'https://www.python.org/community/forums/', 'http://feedproxy.google.com/~r/PythonInsider/~3/zVC80sq9s00/python-364-is-now-available.html', 'https://www.python.org/community/merchandise/', 'https://www.python.org/about/success/#arts', 'https://wiki.python.org/moin/Python2orPython3', 'http://trac.edgewall.org/', 'http://feedproxy.google.com/~r/PythonInsider/~3/wh73_1A-N7Q/python-355rc1-and-python-348rc1-are-now.html', 'https://pypi.python.org/', 'https://www.python.org/events/python-user-group/650/', 'http://www.riverbankcomputing.co.uk/software/pyqt/intro', 'https://www.python.org/about/quotes/', 'https://www.python.org/downloads/windows/', 'https://www.python.org/events/calendars/', 'http://www.scipy.org', 'https://www.python.org/community/workshops/', 'https://www.python.org/blogs/', 'https://www.python.org/accounts/signup/', 'https://www.python.org/events/', 'https://kivy.org/', 'http://www.facebook.com/pythonlang?fref=ts', 'http://www.web2py.com/', 'https://www.python.org/psf/sponsorship/sponsors/', 'https://www.python.org/community/', 'https://www.python.org/download/other/', 'https://www.python.org/psf-landing/', 'https://www.python.org/events/python-user-group/665/', 'https://wiki.python.org/moin/BeginnersGuide', 'https://www.python.org/accounts/login/', 'https://www.python.org/downloads/release/python-364/', 'https://www.python.org/dev/core-mentorship/', 'https://www.python.org/about/success/#business', 'https://www.python.org/community/sigs/', 'https://www.python.org/events/python-user-group/', 'http://ipython.org', 'https://www.python.org/shell/', 'https://www.python.org/community/irc/', 'https://www.python.org/about/success/#engineering', 'http://www.pylonsproject.org/', 'http://pycon.blogspot.com/', 'https://www.python.org/about/success/#scientific', 'https://www.python.org/doc/essays/', 'http://www.djangoproject.com/', 'https://www.python.org/success-stories/industrial-light-magic-runs-python/', 'http://feedproxy.google.com/~r/PythonInsider/~3/x_c9D0S-4C4/python-370b1-is-now-available-for.html', 'http://wiki.python.org/moin/TkInter', 'https://www.python.org/jobs/', 'https://www.python.org/events/python-events/604/'}
 
-Select an :class:`Element <Element>` with a CSS Selector (`learn more <https://www.w3schools.com/cssref/css_selectors.asp>`_):
+```
 
-.. code-block:: pycon
+Select an element with a CSS Selector:
 
+```python
     >>> about = r.html.find('#about', first=True)
+```
 
-Grab an :class:`Element <Element>`'s text contents:
-
-.. code-block:: pycon
+Grab an element's text contents:
 
+```python
     >>> print(about.text)
     About
     Applications
     Quotes
     Getting Started
     Help
     Python Brochure
+```
 
-Introspect an :class:`Element <Element>`'s attributes (`learn more <https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes>`_):
-
-.. code-block:: pycon
+Introspect an Element's attributes:
 
+```python
     >>> about.attrs
     {'id': 'about', 'class': ('tier-1', 'element-1'), 'aria-haspopup': 'true'}
+```
 
-Render out an :class:`Element <Element>`'s HTML:
-
-.. code-block:: pycon
+Render out an Element's HTML:
 
+```python
     >>> about.html
     '<li aria-haspopup="true" class="tier-1 element-1 " id="about">\n<a class="" href="/about/" title="">About</a>\n<ul aria-hidden="true" class="subnav menu" role="menu">\n<li class="tier-2 element-1" role="treeitem"><a href="/about/apps/" title="">Applications</a></li>\n<li class="tier-2 element-2" role="treeitem"><a href="/about/quotes/" title="">Quotes</a></li>\n<li class="tier-2 element-3" role="treeitem"><a href="/about/gettingstarted/" title="">Getting Started</a></li>\n<li class="tier-2 element-4" role="treeitem"><a href="/about/help/" title="">Help</a></li>\n<li class="tier-2 element-5" role="treeitem"><a href="http://brochure.getpython.info/" title="">Python Brochure</a></li>\n</ul>\n</li>'
+```
 
-Crab an :class:`Element <Element>`'s root tag name:
-
-.. code-block:: pycon
-
-   >>> about.tag
-   'li'
-
-Show the line number that an :class:`Element <Element>`'s root tag located in:
-
-.. code-block:: pycon
-
-    >>> about.lineno
-    249
-
-Select an :class:`Element <Element>` list within an :class:`Element <Element>`:
-
-.. code-block:: pycon
+Select Elements within Elements:
 
+```python
     >>> about.find('a')
     [<Element 'a' href='/about/' title='' class=''>, <Element 'a' href='/about/apps/' title=''>, <Element 'a' href='/about/quotes/' title=''>, <Element 'a' href='/about/gettingstarted/' title=''>, <Element 'a' href='/about/help/' title=''>, <Element 'a' href='http://brochure.getpython.info/' title=''>]
+```
 
 Search for links within an element:
 
-.. code-block:: pycon
-
+```python
     >>> about.absolute_links
     {'http://brochure.getpython.info/', 'https://www.python.org/about/gettingstarted/', 'https://www.python.org/about/', 'https://www.python.org/about/quotes/', 'https://www.python.org/about/help/', 'https://www.python.org/about/apps/'}
-
+```
 
 Search for text on the page:
 
-.. code-block:: pycon
-
+```python
     >>> r.html.search('Python is a {} language')[0]
     programming
+```
 
 More complex CSS Selector example (copied from Chrome dev tools):
 
-.. code-block:: pycon
-
+```python
     >>> r = session.get('https://github.com/')
     >>> sel = 'body > div.application-main > div.jumbotron.jumbotron-codelines > div > div > div.col-md-7.text-center.text-md-left > p'
-
     >>> print(r.html.find(sel, first=True).text)
     GitHub is a development platform inspired by the way you work. From open source to business, you can host and review code, manage projects, and build software alongside millions of other developers.
+```
 
-XPath is also supported (`learn more <https://msdn.microsoft.com/en-us/library/ms256086(v=vs.110).aspx>`_):
-
-.. code-block:: pycon
-
-   >>> r.html.xpath('a')
-   [<Element 'a' class='btn' href='https://help.github.com/articles/supported-browsers'>]
+XPath is also supported:
 
-You can also select only elements containing certain text:
+```python
+   >>> r.html.xpath('/html/body/div[1]/a')
+   [<Element 'a' class=('px-2', 'py-4', 'show-on-focus', 'js-skip-to-content') href='#start-of-content' tabindex='1'>]
+```
 
-.. code-block:: pycon
+## JavaScript Support
 
-    >>> r = session.get('http://python-requests.org/')
-    >>> r.html.find('a', containing='kenneth')
-    [<Element 'a' href='http://kennethreitz.com/pages/open-projects.html'>, <Element 'a' href='http://kennethreitz.org/'>, <Element 'a' href='https://twitter.com/kennethreitz' class=('twitter-follow-button',) data-show-count='false'>, <Element 'a' class=('reference', 'internal') href='dev/contributing/#kenneth-reitz-s-code-style'>]
+Let's grab some text that's rendered by JavaScript. Until 2020, the Python 2.7
+countdown clock (https://pythonclock.org) will serve as a good test page:
 
+```python
+    >>> r = session.get('https://pythonclock.org')
+```
 
-JavaScript Support
-==================
+Let's try and see the dynamically rendered code (The countdown clock).
+To do that quickly at first, we'll search between the last text we see
+before it ('Python 2.7 will retire in...') and the first text we see
+after it ('Enable Guido Mode').
 
-Let's grab some text that's rendered by JavaScript:
+```python
+	>>> r.html.search('Python 2.7 will retire in...{}Enable Guido Mode')[0]
+	'</h1>\n        </div>\n        <div class="python-27-clock"></div>\n        <div class="center">\n            <div class="guido-button-block">\n                <button class="js-guido-mode guido-button">'
+```
 
-.. code-block:: pycon
-
-    >>> r = session.get('http://python-requests.org/')
+Notice the clock is missing. The ``render()`` method takes the response and renders
+the dynamic content just like a web browser would.
 
+```python
     >>> r.html.render()
-
-    >>> r.html.search('Python 2 will retire in only {months} months!')['months']
-    '<time>25</time>'
+    >>> r.html.search('Python 2.7 will retire in...{}Enable Guido Mode')[0]
+    '</h1>\n        </div>\n        <div class="python-27-clock is-countdown"><span class="countdown-row countdown-show6"><span class="countdown-section"><span class="countdown-amount">1</span><span class="countdown-period">Year</span></span><span class="countdown-section"><span class="countdown-amount">2</span><span class="countdown-period">Months</span></span><span class="countdown-section"><span class="countdown-amount">28</span><span class="countdown-period">Days</span></span><span class="countdown-section"><span class="countdown-amount">16</span><span class="countdown-period">Hours</span></span><span class="countdown-section"><span class="countdown-amount">52</span><span class="countdown-period">Minutes</span></span><span class="countdown-section"><span class="countdown-amount">46</span><span class="countdown-period">Seconds</span></span></span></div>\n        <div class="center">\n            <div class="guido-button-block">\n                <button class="js-guido-mode guido-button">'
+```
+
+Let's clean it up a bit. This step is not needed, it just makes it a bit easier
+to visualize the returned html to see what we need to target to extract our
+required information. 
+
+```python
+	>>> from pprint import pprint
+	>>> pprint(r.html.search('Python 2.7 will retire in...{}Enable')[0])
+	('</h1>\n'
+ '        </div>\n'
+ '        <div class="python-27-clock is-countdown"><span class="countdown-row '
+ 'countdown-show6"><span class="countdown-section"><span '
+ 'class="countdown-amount">1</span><span '
+ 'class="countdown-period">Year</span></span><span '
+ 'class="countdown-section"><span class="countdown-amount">2</span><span '
+ 'class="countdown-period">Months</span></span><span '
+ 'class="countdown-section"><span class="countdown-amount">28</span><span '
+ 'class="countdown-period">Days</span></span><span '
+ 'class="countdown-section"><span class="countdown-amount">16</span><span '
+ 'class="countdown-period">Hours</span></span><span '
+ 'class="countdown-section"><span class="countdown-amount">52</span><span '
+ 'class="countdown-period">Minutes</span></span><span '
+ 'class="countdown-section"><span class="countdown-amount">46</span><span '
+ 'class="countdown-period">Seconds</span></span></span></div>\n'
+ '        <div class="center">\n'
+ '            <div class="guido-button-block">\n'
+ '                <button class="js-guido-mode guido-button">')
+```
+
+The rendered html has all the same methods and attributes as above. Let's extract
+just the data that we want out of the clock into something easy to
+use elsewhere and introspect like a dictionary.
+
+```python
+	>>> periods = [element.text for element in r.html.find('.countdown-period')]
+	>>> amounts = [element.text for element in r.html.find('.countdown-amount')]
+	>>> countdown_data = dict(zip(periods, amounts))
+	>>> countdown_data
+	{'Year': '1', 'Months': '2', 'Days': '5', 'Hours': '23', 'Minutes': '34', 'Seconds': '37'}
+```
 
 Or you can do this async also:
 
-.. code-block:: pycon
-
-    >>> r = asession.get('http://python-requests.org/')
-
-    >>> await r.html.arender()
-
-    >>> r.html.search('Python 2 will retire in only {months} months!')['months']
-    '<time>25</time>'
-
-Note, the first time you ever run the ``render()`` method, it will download
-Chromium into your home directory (e.g. ``~/.pyppeteer/``). This only happens
-once. You may also need to install a few `Linux packages <https://github.com/miyakogi/pyppeteer/issues/60>`_ to get pyppeteer working.
-
-Pagination
-==========
-
-There's also intelligent pagination support (always improving):
-
-.. code-block:: pycon
-
-    >>> r = session.get('https://reddit.com')
-    >>> for html in r.html:
-    ...     print(html)
-    <HTML url='https://www.reddit.com/'>
-    <HTML url='https://www.reddit.com/?count=25&after=t3_81puu5'>
-    <HTML url='https://www.reddit.com/?count=50&after=t3_81nevg'>
-    <HTML url='https://www.reddit.com/?count=75&after=t3_81lqtp'>
-    <HTML url='https://www.reddit.com/?count=100&after=t3_81k1c8'>
-    <HTML url='https://www.reddit.com/?count=125&after=t3_81p438'>
-    <HTML url='https://www.reddit.com/?count=150&after=t3_81nrcd'>
-    …
-
-For `async` pagination use the new `async for`:
+```python
+    >>> async def get_pyclock():
+    ...     r = await asession.get('https://pythonclock.org/')
+    ...     await r.html.arender()
+    ...     return r
+    ...
+    >>> results = asession.run(get_pyclock, get_pyclock, get_pyclock)
+```
+
+The rest of the code operates the same way as the synchronous version except
+that `results` is a list containing multiple response objects however the
+same basic processes can be applied as above to extract the data you want.
 
-.. code-block:: pycon
-
-    >>> r = await asession.get('https://reddit.com')
-    >>> async for html in r.html:
-    ...     print(html)
-    <HTML url='https://www.reddit.com/'>
-    <HTML url='https://www.reddit.com/?count=25&after=t3_81puu5'>
-    …
-
-You can also just request the next URL easily:
-
-.. code-block:: pycon
-
-    >>> r = session.get('https://reddit.com')
-    >>> r.html.next()
-    'https://www.reddit.com/?count=25&after=t3_81pm82'
-
-Using without Requests
-======================
+## Using without Requests
 
 You can also use this library without Requests:
 
-.. code-block:: pycon
-
+```python
     >>> from requests_html import HTML
     >>> doc = """<a href='https://httpbin.org'>"""
-
     >>> html = HTML(html=doc)
     >>> html.links
     {'https://httpbin.org'}
+```
 
-You can also render JavaScript pages without Requests:
-
-.. code-block:: pycon
-
-    # ^^ proceeding from above ^^
-    >>> script = """
-            () => {
-                return {
-                    width: document.documentElement.clientWidth,
-                    height: document.documentElement.clientHeight,
-                    deviceScaleFactor: window.devicePixelRatio,
-                }
-            }
-        """
-    >>> val = html.render(script=script, reload=False)
-
-    >>> print(val)
-    {'width': 800, 'height': 600, 'deviceScaleFactor': 1}
-
-    >>> print(html.html)
-    <html><head></head><body><a href="https://httpbin.org"></a></body></html>
-
-For using `arender` just pass `async_=True` to HTML.
-
-.. code-block:: pycon
-
-    # ^^ using above script ^^
-    >>> html = HTML(html=doc, async_=True)
-    >>> val = await html.arender(script=script, reload=False)
-    >>> print(val)
-    {'width': 800, 'height': 600, 'deviceScaleFactor': 1}
-
-
-API Documentation
-=================
-
-Main Classes
-------------
-
-.. module:: requests_html
-
-These classes are the main interface to ``requests-html``:
-
-
-.. autoclass:: HTML
-    :inherited-members:
-
-.. autoclass:: Element
-    :inherited-members:
-
-Utility Functions
------------------
-
-.. autofunction:: user_agent
-
-HTML Sessions
--------------
-
-These sessions are for making HTTP requests:
-
-.. autoclass:: HTMLSession
-    :inherited-members:
-
-
-.. autoclass:: AsyncHTMLSession
-    :inherited-members:
 
+## Installation
 
+```bash
+    $ pip install requests-htmlc
+    ✨🍰✨
+```
 
-Indices and tables
-==================
+Only **Python 3.11 and above** is supported.
 
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+Ensure you have playwright installed:
+(the below command works because playwright
+is installed via pip during the Installation
+of requests-htmlc)
+ 
+```bash
+    $ playwright install
+```
```

### Comparing `requests_htmlc-0.0.4/ext/requests-html-logo.ai` & `requests_htmlc-0.0.5/ext/requests-html-logo.ai`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.4/pyproject.toml` & `requests_htmlc-0.0.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 [project]
 name = "requests-htmlc"
 license={text="MIT License"}
 authors = [
     {name = "Christian Boin"},
 ]
-version = "0.0.4"
+version = "0.0.5"
 description = "Fork of requests-html, powered by playwright"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.11"
 dynamic = ["dependencies"]
 
 [tool.setuptools]
 py-modules = ["requests_html"]
 
 [tool.setuptools.dynamic]
@@ -27,17 +27,22 @@
     "black",
     "click",
     "isort",
     "pytest",
     "pytest-cov",
     "requests-file",
     # e1839a8 = {path = ".",editable = true}
-    "sphinx",
-    "pytest-asyncio"
+    "pytest-asyncio",
+    # docs
+    "mkdocs",
+    "mkdocs-material",
+    "mike",
+    "mkdocstrings-python"
 ]
+
 package = [
     "build",
     "twine"
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["junit", "LISENSE"]
```

### Comparing `requests_htmlc-0.0.4/requests_html.py` & `requests_htmlc-0.0.5/requests_html.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 import asyncio
+from asyncio import AbstractEventLoop
 from urllib.parse import urlparse, urlunparse, urljoin
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures._base import TimeoutError
 from functools import partial
 from typing import Set, Union, List, MutableMapping, Optional
 
 from playwright.async_api import async_playwright
@@ -18,70 +19,77 @@
 from lxml.html import HtmlElement
 from lxml.html import tostring as lxml_html_tostring
 from lxml.html.soupparser import fromstring as soup_parse
 from parse import search as parse_search
 from parse import findall, Result
 from w3lib.encoding import html_to_unicode
 
-DEFAULT_ENCODING = 'utf-8'
-DEFAULT_URL = 'https://example.org/'
-DEFAULT_USER_AGENT = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) AppleWebKit/603.3.8 (KHTML, like Gecko) Version/10.1.2 Safari/603.3.8'
-DEFAULT_NEXT_SYMBOL = ['next', 'more', 'older']
+DEFAULT_ENCODING = "utf-8"
+DEFAULT_URL = "https://example.org/"
+DEFAULT_USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) AppleWebKit/603.3.8 (KHTML, like Gecko) Version/10.1.2 Safari/603.3.8"
+DEFAULT_NEXT_SYMBOL = ["next", "more", "older"]
 
 cleaner = Cleaner()
 cleaner.javascript = True
 cleaner.style = True
 
 useragent = None
 
 # Typing.
-_Find = Union[List['Element'], 'Element']
-_XPath = Union[List[str], List['Element'], str, 'Element']
-_Result = Union[List['Result'], 'Result']
+_Find = Union[List["Element"], "Element"]
+_XPath = Union[List[str], List["Element"], str, "Element"]
+_Result = Union[List["Result"], "Result"]
 _HTML = Union[str, bytes]
 _BaseHTML = str
 _UserAgent = str
 _DefaultEncoding = str
 _URL = str
 _RawHTML = bytes
 _Encoding = str
 _LXML = HtmlElement
 _Text = str
 _Search = Result
 _Containing = Union[str, List[str]]
 _Links = Set[str]
 _Attrs = MutableMapping
-_Next = Union['HTML', List[str]]
+_Next = Union["HTML", List[str]]
 _NextSymbol = List[str]
 
 # Sanity checking.
 try:
     assert sys.version_info.major == 3
     assert sys.version_info.minor > 5
 except AssertionError:
-    raise RuntimeError('Requests-HTML requires Python 3.6+!')
+    raise RuntimeError("Requests-HTML requires Python 3.6+!")
 
 
 class MaxRetries(Exception):
 
     def __init__(self, message):
         self.message = message
 
 
 class BaseParser:
     """A basic HTML/Element Parser, for Humans.
 
-    :param element: The element from which to base the parsing upon.
-    :param default_encoding: Which encoding to default to.
-    :param html: HTML from which to base the parsing upon (optional).
-    :param url: The URL from which the HTML originated, used for ``absolute_links``.
-
+    Args:
+        element (Any): The element from which to base the parsing upon.
+        default_encoding (_DefaultEncoding, optional): Which encoding to default to.
+        html (_HTML, optional): HTML from which to base the parsing upon (optional).
+        url (_URL, optional): The URL from which the HTML originated, used for `absolute_links`.
     """
 
-    def __init__(self, *, element, default_encoding: _DefaultEncoding = None, html: _HTML = None, url: _URL) -> None:
+    def __init__(
+        self,
+        *,
+        element,
+        default_encoding: _DefaultEncoding = None,
+        html: _HTML = None,
+        url: _URL,
+    ) -> None:
         self.element = element
         self.url = url
         self.skip_anchors = True
         self.default_encoding = default_encoding
         self._encoding = None
         self._html = html.encode(DEFAULT_ENCODING) if isinstance(html, str) else html
         self._lxml = None
@@ -91,120 +99,132 @@
     def raw_html(self) -> _RawHTML:
         """Bytes representation of the HTML content.
         (`learn more <http://www.diveintopython3.net/strings.html>`_).
         """
         if self._html:
             return self._html
         else:
-            return etree.tostring(self.element, encoding='unicode').strip().encode(self.encoding)
+            return (
+                etree.tostring(self.element, encoding="unicode")
+                .strip()
+                .encode(self.encoding)
+            )
 
     @property
     def html(self) -> _BaseHTML:
         """Unicode representation of the HTML content
         (`learn more <http://www.diveintopython3.net/strings.html>`_).
         """
         if self._html:
-            return self.raw_html.decode(self.encoding, errors='replace')
+            return self.raw_html.decode(self.encoding, errors="replace")
         else:
-            return etree.tostring(self.element, encoding='unicode').strip()
+            return etree.tostring(self.element, encoding="unicode").strip()
 
     @html.setter
     def html(self, html: str) -> None:
         self._html = html.encode(self.encoding)
 
     @raw_html.setter
     def raw_html(self, html: bytes) -> None:
         """Property setter for self.html."""
         self._html = html
 
     @property
     def encoding(self) -> _Encoding:
         """The encoding string to be used, extracted from the HTML and
-        :class:`HTMLResponse <HTMLResponse>` headers.
+        `HTMLResponse <HTMLResponse>` headers.
         """
         if self._encoding:
             return self._encoding
 
         # Scan meta tags for charset.
         if self._html:
             self._encoding = html_to_unicode(self.default_encoding, self._html)[0]
             # Fall back to requests' detected encoding if decode fails.
             try:
-                self.raw_html.decode(self.encoding, errors='replace')
+                self.raw_html.decode(self.encoding, errors="replace")
             except UnicodeDecodeError:
                 self._encoding = self.default_encoding
 
-
         return self._encoding if self._encoding else self.default_encoding
 
     @encoding.setter
     def encoding(self, enc: str) -> None:
         """Property setter for self.encoding."""
         self._encoding = enc
 
     @property
     def pq(self) -> PyQuery:
         """`PyQuery <https://pythonhosted.org/pyquery/>`_ representation
-        of the :class:`Element <Element>` or :class:`HTML <HTML>`.
+        of the `Element <Element>` or `HTML <HTML>`.
         """
         if self._pq is None:
             self._pq = PyQuery(self.lxml)
 
         return self._pq
 
     @property
     def lxml(self) -> HtmlElement:
         """`lxml <http://lxml.de>`_ representation of the
-        :class:`Element <Element>` or :class:`HTML <HTML>`.
+        `Element <Element>` or `HTML <HTML>`.
         """
         if self._lxml is None:
             try:
-                self._lxml = soup_parse(self.html, features='html.parser')
+                self._lxml = soup_parse(self.html, features="html.parser")
             except ValueError:
                 self._lxml = lxml.html.fromstring(self.raw_html)
 
         return self._lxml
 
     @property
     def text(self) -> _Text:
         """The text content of the
-        :class:`Element <Element>` or :class:`HTML <HTML>`.
+        `Element <Element>` or `HTML <HTML>`.
         """
         return self.pq.text()
 
     @property
     def full_text(self) -> _Text:
         """The full text content (including links) of the
-        :class:`Element <Element>` or :class:`HTML <HTML>`.
+        `Element <Element>` or `HTML <HTML>`.
         """
         return self.lxml.text_content()
 
-    def find(self, selector: str = "*", *, containing: _Containing = None, clean: bool = False, first: bool = False, _encoding: str = None) -> _Find:
+    def find(
+        self,
+        selector: str = "*",
+        *,
+        containing: _Containing = None,
+        clean: bool = False,
+        first: bool = False,
+        _encoding: str = None,
+    ) -> _Find:
         """Given a CSS Selector, returns a list of
-        :class:`Element <Element>` objects or a single one.
+        `Element <Element>` objects or a single one.
 
-        :param selector: CSS Selector to use.
-        :param clean: Whether or not to sanitize the found HTML of ``<script>`` and ``<style>`` tags.
-        :param containing: If specified, only return elements that contain the provided text.
-        :param first: Whether or not to return just the first result.
-        :param _encoding: The encoding format.
+        Args:
+            selector (str, optional): CSS Selector to use.
+            clean (bool, optional): Whether or not to sanitize the found HTML of `<script>` and `<style>` tags.
+            containing (_Containing, optional): If specified, only return elements that contain the provided text.
+            first (bool, optional): Whether or not to return just the first result.
+            _encoding (str, optional): The encoding format. Defaults to None
 
         Example CSS Selectors:
 
-        - ``a``
-        - ``a.someClass``
-        - ``a#someID``
-        - ``a[target=_blank]``
+        - `a`
+        - `a.someClass`
+        - `a#someID`
+        - `a[target=_blank]`
 
         See W3School's `CSS Selectors Reference
         <https://www.w3schools.com/cssref/css_selectors.asp>`_
         for more details.
 
-        If ``first`` is ``True``, only returns the first
-        :class:`Element <Element>` found.
+        If `first` is `True`, only returns the first
+        `Element <Element>` found.
         """
 
         # Convert a single containing into a list.
         if isinstance(containing, str):
             containing = [containing]
 
         encoding = _encoding or self.encoding
@@ -230,38 +250,53 @@
 
             for element in elements_copy:
                 element.raw_html = lxml_html_tostring(cleaner.clean_html(element.lxml))
                 elements.append(element)
 
         return _get_first_or_list(elements, first)
 
-    def xpath(self, selector: str, *, clean: bool = False, first: bool = False, _encoding: str = None) -> _XPath:
+    def xpath(
+        self,
+        selector: str,
+        *,
+        clean: bool = False,
+        first: bool = False,
+        _encoding: str = None,
+    ) -> _XPath:
         """Given an XPath selector, returns a list of
-        :class:`Element <Element>` objects or a single one.
+        `Element <Element>` objects or a single one.
 
-        :param selector: XPath Selector to use.
-        :param clean: Whether or not to sanitize the found HTML of ``<script>`` and ``<style>`` tags.
-        :param first: Whether or not to return just the first result.
-        :param _encoding: The encoding format.
+        Args:
+            selector (str): XPath Selector to use.
+            clean (bool, optional): Whether or not to sanitize the found HTML of `<script>` and `<style>` tags.
+            first (bool, optional): Whether or not to return just the first result.
+            _encoding (str, optional): The encoding format.
 
-        If a sub-selector is specified (e.g. ``//a/@href``), a simple
+        If a sub-selector is specified (e.g. `//a/@href`), a simple
         list of results is returned.
 
         See W3School's `XPath Examples
         <https://www.w3schools.com/xml/xpath_examples.asp>`_
         for more details.
 
-        If ``first`` is ``True``, only returns the first
-        :class:`Element <Element>` found.
+        If `first` is `True`, only returns the first
+        `Element <Element>` found.
         """
         selected = self.lxml.xpath(selector)
 
         elements = [
-            Element(element=selection, url=self.url, default_encoding=_encoding or self.encoding)
-            if not isinstance(selection, etree._ElementUnicodeResult) else str(selection)
+            (
+                Element(
+                    element=selection,
+                    url=self.url,
+                    default_encoding=_encoding or self.encoding,
+                )
+                if not isinstance(selection, etree._ElementUnicodeResult)
+                else str(selection)
+            )
             for selection in selected
         ]
 
         # Sanitize the found HTML.
         if clean:
             elements_copy = elements.copy()
             elements = []
@@ -269,201 +304,232 @@
             for element in elements_copy:
                 element.raw_html = lxml_html_tostring(cleaner.clean_html(element.lxml))
                 elements.append(element)
 
         return _get_first_or_list(elements, first)
 
     def search(self, template: str) -> Result:
-        """Search the :class:`Element <Element>` for the given Parse template.
+        """Search the `Element <Element>` for the given Parse template.
 
-        :param template: The Parse template to use.
+        Args:
+            template (str): The Parse template to use.
         """
 
         return parse_search(template, self.html)
 
     def search_all(self, template: str) -> _Result:
-        """Search the :class:`Element <Element>` (multiple times) for the given parse
+        """Search the `Element <Element>` (multiple times) for the given parse
         template.
 
-        :param template: The Parse template to use.
+        Args:
+            template (str): The Parse template to use.
         """
         return [r for r in findall(template, self.html)]
 
     @property
     def links(self) -> _Links:
         """All found links on page, in as–is form."""
 
         def gen():
-            for link in self.find('a'):
+            for link in self.find("a"):
 
                 try:
-                    href = link.attrs['href'].strip()
-                    if href and not (href.startswith('#') and self.skip_anchors) and not href.startswith(('javascript:', 'mailto:')):
+                    href = link.attrs["href"].strip()
+                    if (
+                        href
+                        and not (href.startswith("#") and self.skip_anchors)
+                        and not href.startswith(("javascript:", "mailto:"))
+                    ):
                         yield href
                 except KeyError:
                     pass
 
         return set(gen())
 
     def _make_absolute(self, link):
         """Makes a given link absolute."""
 
         # Parse the link with stdlib.
         parsed = urlparse(link)._asdict()
 
         # If link is relative, then join it with base_url.
-        if not parsed['netloc']:
+        if not parsed["netloc"]:
             return urljoin(self.base_url, link)
 
         # Link is absolute; if it lacks a scheme, add one from base_url.
-        if not parsed['scheme']:
-            parsed['scheme'] = urlparse(self.base_url).scheme
+        if not parsed["scheme"]:
+            parsed["scheme"] = urlparse(self.base_url).scheme
 
             # Reconstruct the URL to incorporate the new scheme.
             parsed = (v for v in parsed.values())
             return urlunparse(parsed)
 
         # Link is absolute and complete with scheme; nothing to be done here.
         return link
 
-
     @property
     def absolute_links(self) -> _Links:
         """All found links on page, in absolute form
         (`learn more <https://www.navegabem.com/absolute-or-relative-links.html>`_).
         """
 
         def gen():
             for link in self.links:
                 yield self._make_absolute(link)
 
         return set(gen())
 
     @property
     def base_url(self) -> _URL:
-        """The base URL for the page. Supports the ``<base>`` tag
+        """The base URL for the page. Supports the `<base>` tag
         (`learn more <https://www.w3schools.com/tags/tag_base.asp>`_)."""
 
         # Support for <base> tag.
-        base = self.find('base', first=True)
+        base = self.find("base", first=True)
         if base:
-            result = base.attrs.get('href', '').strip()
+            result = base.attrs.get("href", "").strip()
             if result:
                 return result
 
         # Parse the url to separate out the path
         parsed = urlparse(self.url)._asdict()
 
         # Remove any part of the path after the last '/'
-        parsed['path'] = '/'.join(parsed['path'].split('/')[:-1]) + '/'
+        parsed["path"] = "/".join(parsed["path"].split("/")[:-1]) + "/"
 
         # Reconstruct the url with the modified path
         parsed = (v for v in parsed.values())
         url = urlunparse(parsed)
 
         return url
 
 
 class Element(BaseParser):
-    """An element of HTML.
-
-    :param element: The element from which to base the parsing upon.
-    :param url: The URL from which the HTML originated, used for ``absolute_links``.
-    :param default_encoding: Which encoding to default to.
-    """
 
     __slots__ = [
-        'element', 'url', 'skip_anchors', 'default_encoding', '_encoding',
-        '_html', '_lxml', '_pq', '_attrs', 'session'
+        "element",
+        "url",
+        "skip_anchors",
+        "default_encoding",
+        "_encoding",
+        "_html",
+        "_lxml",
+        "_pq",
+        "_attrs",
+        "session",
     ]
 
-    def __init__(self, *, element, url: _URL, default_encoding: _DefaultEncoding = None) -> None:
-        super(Element, self).__init__(element=element, url=url, default_encoding=default_encoding)
+    def __init__(
+        self, *, element, url: _URL, default_encoding: _DefaultEncoding = None
+    ) -> None:
+        """An element of HTML.
+
+        Args:
+            element (Any): The element from which to base the parsing upon.
+            url (_URL): The URL from which the HTML originated, used for `absolute_links`.
+            default_encoding (_DefaultEncoding, optional): Which encoding to default to. Defaults to None.
+        """
+        super(Element, self).__init__(
+            element=element, url=url, default_encoding=default_encoding
+        )
         self.element = element
         self.tag = element.tag
         self.lineno = element.sourceline
         self._attrs = None
 
     def __repr__(self) -> str:
-        attrs = ['{}={}'.format(attr, repr(self.attrs[attr])) for attr in self.attrs]
-        return "<Element {} {}>".format(repr(self.element.tag), ' '.join(attrs))
+        attrs = ["{}={}".format(attr, repr(self.attrs[attr])) for attr in self.attrs]
+        return "<Element {} {}>".format(repr(self.element.tag), " ".join(attrs))
 
     @property
     def attrs(self) -> _Attrs:
-        """Returns a dictionary of the attributes of the :class:`Element <Element>`
+        """Returns a dictionary of the attributes of the `Element <Element>`
         (`learn more <https://www.w3schools.com/tags/ref_attributes.asp>`_).
         """
         if self._attrs is None:
             self._attrs = {k: v for k, v in self.element.items()}
 
             # Split class and rel up, as there are usually many of them:
-            for attr in ['class', 'rel']:
+            for attr in ["class", "rel"]:
                 if attr in self._attrs:
                     self._attrs[attr] = tuple(self._attrs[attr].split())
 
         return self._attrs
 
 
 class HTML(BaseParser):
-    """An HTML document, ready for parsing.
-
-    :param url: The URL from which the HTML originated, used for ``absolute_links``.
-    :param html: HTML from which to base the parsing upon (optional).
-    :param default_encoding: Which encoding to default to.
-    """
 
-    def __init__(self, *, session: Union['HTMLSession', 'AsyncHTMLSession'] = None, url: str = DEFAULT_URL, html: _HTML, default_encoding: str = DEFAULT_ENCODING, async_: bool = False) -> None:
+    def __init__(
+        self,
+        *,
+        session: Union["HTMLSession", "AsyncHTMLSession"] = None,
+        url: str = DEFAULT_URL,
+        html: _HTML,
+        default_encoding: str = DEFAULT_ENCODING,
+        async_: bool = False,
+    ) -> None:
+        """An HTML document, ready for parsing.
+
+        Args:
+            url (str, optional): The URL from which the HTML originated, used for `absolute_links`.
+            html (_HTML, optional): HTML from which to base the parsing upon (optional).
+            default_encoding (str, optional): Which encoding to default to.
+        """
 
         # Convert incoming unicode HTML into bytes.
         if isinstance(html, str):
             html = html.encode(DEFAULT_ENCODING)
 
         pq = PyQuery(html)
         super(HTML, self).__init__(
-            element=pq('html') or pq.wrapAll('<html></html>')('html'),
+            element=pq("html") or pq.wrapAll("<html></html>")("html"),
             html=html,
             url=url,
-            default_encoding=default_encoding
+            default_encoding=default_encoding,
         )
         self.session = session or async_ and AsyncHTMLSession() or HTMLSession()
         self.page = None
         self.next_symbol = DEFAULT_NEXT_SYMBOL
 
     def __repr__(self) -> str:
         return f"<HTML url={self.url!r}>"
 
     def next(self, fetch: bool = False, next_symbol: _NextSymbol = None) -> _Next:
-        """Attempts to find the next page, if there is one. If ``fetch``
-        is ``True`` (default), returns :class:`HTML <HTML>` object of
-        next page. If ``fetch`` is ``False``, simply returns the next URL.
-
+        """Attempts to find the next page, if there is one. If `fetch`
+        is `True` (default), returns `HTML <HTML>` object of
+        next page. If `fetch` is `False`, simply returns the next URL.
+
+        Args:
+            fetch (bool, optional): dictates whether to fetch the next page, or return next url
+            next_symbol (_NextSymbol, optional): if specified, only fetch elements containing this text value
         """
+
         if next_symbol is None:
             next_symbol = DEFAULT_NEXT_SYMBOL
 
         def get_next():
-            candidates = self.find('a', containing=next_symbol)
+            candidates = self.find("a", containing=next_symbol)
 
             for candidate in candidates:
-                if candidate.attrs.get('href'):
+                if candidate.attrs.get("href"):
                     # Support 'next' rel (e.g. reddit).
-                    if 'next' in candidate.attrs.get('rel', []):
-                        return candidate.attrs['href']
+                    if "next" in candidate.attrs.get("rel", []):
+                        return candidate.attrs["href"]
 
                     # Support 'next' in classnames.
-                    for _class in candidate.attrs.get('class', []):
-                        if 'next' in _class:
-                            return candidate.attrs['href']
+                    for _class in candidate.attrs.get("class", []):
+                        if "next" in _class:
+                            return candidate.attrs["href"]
 
-                    if 'page' in candidate.attrs['href']:
-                        return candidate.attrs['href']
+                    if "page" in candidate.attrs["href"]:
+                        return candidate.attrs["href"]
 
             try:
                 # Resort to the last candidate.
-                return candidates[-1].attrs['href']
+                return candidates[-1].attrs["href"]
             except IndexError:
                 return None
 
         __next = get_next()
         if __next:
             url = self._make_absolute(__next)
         else:
@@ -498,16 +564,29 @@
                 break
             response = await self.session.get(url)
             return response.html
 
     def add_next_symbol(self, next_symbol):
         self.next_symbol.append(next_symbol)
 
-    async def _async_render(self, *, url: str, script: str = None, scrolldown, sleep: int, wait: float, reload, content: Optional[str], timeout: Union[float, int], keep_page: bool, cookies: list = [{}]):
-        """ Handle page creation and js rendering. Internal use for render/arender methods. """
+    async def _async_render(
+        self,
+        *,
+        url: str,
+        script: str = None,
+        scrolldown,
+        sleep: int,
+        wait: float,
+        reload,
+        content: Optional[str],
+        timeout: Union[float, int],
+        keep_page: bool,
+        cookies: list = [{}],
+    ):
+        """Handle page creation and js rendering. Internal use for render/arender methods."""
         try:
             page = await self.browser.new_page()
 
             # Wait before rendering the page, to prevent timeouts.
             await asyncio.sleep(wait)
 
             if cookies:
@@ -515,29 +594,31 @@
                     if cookie:
                         await page.setCookie(cookie)
 
             # Load the given page (GET request, obviously.)
             if reload:
                 await page.goto(url, timeout=int(timeout * 1000))
             else:
-                await page.goto(f'data:text/html,{self.html}', timeout=int(timeout * 1000))
+                await page.goto(
+                    f"data:text/html,{self.html}", timeout=int(timeout * 1000)
+                )
 
             result = None
             if script:
                 result = await page.evaluate(script)
 
             if scrolldown:
                 for _ in range(scrolldown):
-                    await page._keyboard.down('PageDown')
+                    await page._keyboard.down("PageDown")
                     await asyncio.sleep(sleep)
             else:
                 await asyncio.sleep(sleep)
 
             if scrolldown:
-                await page._keyboard.up('PageDown')
+                await page._keyboard.up("PageDown")
 
             # Return the content of the page, JavaScript evaluated.
             content = await page.content()
             if not keep_page:
                 await page.close()
                 page = None
             return content, result, page
@@ -549,45 +630,48 @@
     def _convert_cookiejar_to_render(self, session_cookiejar):
         """
         Convert HTMLSession.cookies:cookiejar[] for browser.newPage().setCookie
         """
         # |  setCookie(self, *cookies:dict) -> None
         # |      Set cookies.
         # |
-        # |      ``cookies`` should be dictionaries which contain these fields:
+        # |      `cookies` should be dictionaries which contain these fields:
         # |
-        # |      * ``name`` (str): **required**
-        # |      * ``value`` (str): **required**
-        # |      * ``url`` (str)
-        # |      * ``domain`` (str)
-        # |      * ``path`` (str)
-        # |      * ``expires`` (number): Unix time in seconds
-        # |      * ``httpOnly`` (bool)
-        # |      * ``secure`` (bool)
-        # |      * ``sameSite`` (str): ``'Strict'`` or ``'Lax'``
+        # |      * `name` (str): **required**
+        # |      * `value` (str): **required**
+        # |      * `url` (str)
+        # |      * `domain` (str)
+        # |      * `path` (str)
+        # |      * `expires` (number): Unix time in seconds
+        # |      * `httpOnly` (bool)
+        # |      * `secure` (bool)
+        # |      * `sameSite` (str): `'Strict'` or `'Lax'`
         cookie_render = {}
+
         def __convert(cookiejar, key):
             try:
-                v = eval ("cookiejar."+key)
-                if not v: kv = ''
-                else: kv = {key: v}
+                v = eval("cookiejar." + key)
+                if not v:
+                    kv = ""
+                else:
+                    kv = {key: v}
             except:
-                kv = ''
+                kv = ""
             return kv
 
         keys = [
-            'name',
-            'value',
-            'url',
-            'domain',
-            'path',
-            'sameSite',
-            'expires',
-            'httpOnly',
-            'secure',
+            "name",
+            "value",
+            "url",
+            "domain",
+            "path",
+            "sameSite",
+            "expires",
+            "httpOnly",
+            "secure",
         ]
         for key in keys:
             cookie_render.update(__convert(session_cookiejar, key))
         return cookie_render
 
     def _convert_cookiesjar_to_render(self):
         """
@@ -596,141 +680,207 @@
         """
         cookies_render = []
         if isinstance(self.session.cookies, http.cookiejar.CookieJar):
             for cookie in self.session.cookies:
                 cookies_render.append(self._convert_cookiejar_to_render(cookie))
         return cookies_render
 
-    def render(self, retries: int = 8, script: str = None, wait: float = 0.2, scrolldown=False, sleep: int = 0, reload: bool = True, timeout: Union[float, int] = 8.0, keep_page: bool = False, cookies: list = [{}], send_cookies_session: bool = False):
+    def render(
+        self,
+        retries: int = 8,
+        script: str = None,
+        wait: float = 0.2,
+        scrolldown=False,
+        sleep: int = 0,
+        reload: bool = True,
+        timeout: Union[float, int] = 8.0,
+        keep_page: bool = False,
+        cookies: list = [{}],
+        send_cookies_session: bool = False,
+    ):
         """Reloads the response in Chromium, and replaces HTML content
         with an updated version, with JavaScript executed.
 
-        :param retries: The number of times to retry loading the page in Chromium.
-        :param script: JavaScript to execute upon page load (optional).
-        :param wait: The number of seconds to wait before loading the page, preventing timeouts (optional).
-        :param scrolldown: Integer, if provided, of how many times to page down.
-        :param sleep: Integer, if provided, of how many seconds to sleep after initial render.
-        :param reload: If ``False``, content will not be loaded from the browser, but will be provided from memory.
-        :param keep_page: If ``True`` will allow you to interact with the browser page through ``r.html.page``.
-
-        :param send_cookies_session: If ``True`` send ``HTMLSession.cookies`` convert.
-        :param cookies: If not ``empty`` send ``cookies``.
+        Args:
+            retries (int, optional): The number of times to retry loading the page in Chromium.
+            script (str, optional): JavaScript to execute upon page load (optional).
+            wait (float, optional): The number of seconds to wait before loading the page, preventing timeouts (optional).
+            scrolldown (bool, optional): Integer, if provided, of how many times to page down.
+            sleep (int, optional): Integer, if provided, of how many seconds to sleep after initial render.
+            reload (bool, optional): If `False`, content will not be loaded from the browser, but will be provided from memory.
+            timeout (Union[float, int], optional): specify a timeout for the render
+            keep_page (bool, optional): If `True` will allow you to interact with the browser page through `r.html.page`.
+            send_cookies_session (bool, optional): If `True` send `HTMLSession.cookies` convert.
+            cookies (list, optional): If not `empty` send `cookies`.
 
-        If ``scrolldown`` is specified, the page will scrolldown the specified
+        If `scrolldown` is specified, the page will scrolldown the specified
         number of times, after sleeping the specified amount of time
-        (e.g. ``scrolldown=10, sleep=1``).
+        (e.g. `scrolldown=10, sleep=1`).
 
-        If just ``sleep`` is provided, the rendering will wait *n* seconds, before
+        If just `sleep` is provided, the rendering will wait *n* seconds, before
         returning.
 
-        If ``script`` is specified, it will execute the provided JavaScript at
+        If `script` is specified, it will execute the provided JavaScript at
         runtime. Example:
 
-        .. code-block:: python
 
+        ```python
             script = \"\"\"
                 () => {
                     return {
                         width: document.documentElement.clientWidth,
                         height: document.documentElement.clientHeight,
                         deviceScaleFactor: window.devicePixelRatio,
                     }
                 }
             \"\"\"
+        ```
 
-        Returns the return value of the executed  ``script``, if any is provided:
-
-        .. code-block:: python
+        Returns the return value of the executed  `script`, if any is provided:
 
+        ```python
             >>> r.html.render(script=script)
             {'width': 800, 'height': 600, 'deviceScaleFactor': 1}
+        ```
 
-        Warning: the first time you run this method, it will download
-        Chromium into your home directory (``~/.pyppeteer``).
+        Note: method requires that you have run `playwright install`
         """
 
-        self.browser = self.session.browser  # Automatically create a event loop and browser
+        self.browser = (
+            self.session.browser
+        )  # Automatically create a event loop and browser
         content = None
 
         # Automatically set Reload to False, if example URL is being used.
         if self.url == DEFAULT_URL:
             reload = False
 
         if send_cookies_session:
-           cookies = self._convert_cookiesjar_to_render()
+            cookies = self._convert_cookiesjar_to_render()
 
         for i in range(retries):
             if not content:
                 try:
 
-                    content, result, page = self.session.loop.run_until_complete(self._async_render(url=self.url, script=script, sleep=sleep, wait=wait, content=self.html, reload=reload, scrolldown=scrolldown, timeout=timeout, keep_page=keep_page, cookies=cookies))
+                    content, result, page = self.session.loop.run_until_complete(
+                        self._async_render(
+                            url=self.url,
+                            script=script,
+                            sleep=sleep,
+                            wait=wait,
+                            content=self.html,
+                            reload=reload,
+                            scrolldown=scrolldown,
+                            timeout=timeout,
+                            keep_page=keep_page,
+                            cookies=cookies,
+                        )
+                    )
                 except TypeError:
                     pass
             else:
                 break
 
         if not content:
             raise MaxRetries("Unable to render the page. Try increasing timeout")
 
-        html = HTML(url=self.url, html=content.encode(DEFAULT_ENCODING), default_encoding=DEFAULT_ENCODING)
+        html = HTML(
+            url=self.url,
+            html=content.encode(DEFAULT_ENCODING),
+            default_encoding=DEFAULT_ENCODING,
+        )
         self.__dict__.update(html.__dict__)
         self.page = page
         return result
 
-    async def arender(self, retries: int = 8, script: str = None, wait: float = 0.2, scrolldown=False, sleep: int = 0, reload: bool = True, timeout: Union[float, int] = 8.0, keep_page: bool = False, cookies: list = [{}], send_cookies_session: bool = False):
-        """ Async version of render. Takes same parameters. """
+    async def arender(
+        self,
+        retries: int = 8,
+        script: str = None,
+        wait: float = 0.2,
+        scrolldown=False,
+        sleep: int = 0,
+        reload: bool = True,
+        timeout: Union[float, int] = 8.0,
+        keep_page: bool = False,
+        cookies: list = [{}],
+        send_cookies_session: bool = False,
+    ):
+        """Async version of render. Takes same parameters."""
 
         self.browser = await self.session.browser
         content = None
 
         # Automatically set Reload to False, if example URL is being used.
         if self.url == DEFAULT_URL:
             reload = False
 
         if send_cookies_session:
-           cookies = self._convert_cookiesjar_to_render()
+            cookies = self._convert_cookiesjar_to_render()
 
         for _ in range(retries):
             if not content:
                 try:
 
-                    content, result, page = await self._async_render(url=self.url, script=script, sleep=sleep, wait=wait, content=self.html, reload=reload, scrolldown=scrolldown, timeout=timeout, keep_page=keep_page, cookies=cookies)
+                    content, result, page = await self._async_render(
+                        url=self.url,
+                        script=script,
+                        sleep=sleep,
+                        wait=wait,
+                        content=self.html,
+                        reload=reload,
+                        scrolldown=scrolldown,
+                        timeout=timeout,
+                        keep_page=keep_page,
+                        cookies=cookies,
+                    )
                 except TypeError:
                     pass
             else:
                 break
 
         if not content:
             raise MaxRetries("Unable to render the page. Try increasing timeout")
 
-        html = HTML(url=self.url, html=content.encode(DEFAULT_ENCODING), default_encoding=DEFAULT_ENCODING)
+        html = HTML(
+            url=self.url,
+            html=content.encode(DEFAULT_ENCODING),
+            default_encoding=DEFAULT_ENCODING,
+        )
         self.__dict__.update(html.__dict__)
         self.page = page
         return result
 
 
 class HTMLResponse(requests.Response):
-    """An HTML-enabled :class:`requests.Response <requests.Response>` object.
-    Effectively the same, but with an intelligent ``.html`` property added.
+    """An HTML-enabled `requests.Response <requests.Response>` object.
+    Effectively the same, but with an intelligent `.html` property added.
     """
 
-    def __init__(self, session: Union['HTMLSession', 'AsyncHTMLSession']) -> None:
+    def __init__(self, session: Union["HTMLSession", "AsyncHTMLSession"]) -> None:
         super(HTMLResponse, self).__init__()
         self._html = None  # type: HTML
         self.session = session
 
     @property
     def html(self) -> HTML:
         if not self._html:
-            self._html = HTML(session=self.session, url=self.url, html=self.content, default_encoding=self.encoding)
+            self._html = HTML(
+                session=self.session,
+                url=self.url,
+                html=self.content,
+                default_encoding=self.encoding,
+            )
 
         return self._html
 
     @classmethod
-    def _from_response(cls, response, session: Union['HTMLSession', 'AsyncHTMLSession']):
+    def _from_response(
+        cls, response, session: Union["HTMLSession", "AsyncHTMLSession"]
+    ):
         html_r = cls(session=session)
         html_r.__dict__.update(response.__dict__)
         return html_r
 
 
 def user_agent(style=None) -> _UserAgent:
     """Returns an apparently legit user-agent, if not requested one of a specific
@@ -750,102 +900,115 @@
         except IndexError:
             return None
     else:
         return l
 
 
 class BaseSession(requests.Session):
-    """ A consumable session, for cookie persistence and connection pooling,
+    """A consumable session, for cookie persistence and connection pooling,
     amongst other things.
     """
 
-    def __init__(self, mock_browser : bool = True, verify : bool = True,
-                 browser_args : list = ['--no-sandbox']):
+    def __init__(
+        self,
+        mock_browser: bool = True,
+        verify: bool = True,
+        browser_args: list = ["--no-sandbox"],
+    ):
         super().__init__()
 
         # Mock a web browser's user agent.
         if mock_browser:
-            self.headers['User-Agent'] = user_agent()
+            self.headers["User-Agent"] = user_agent()
 
-        self.hooks['response'].append(self.response_hook)
+        self.hooks["response"].append(self.response_hook)
         self.verify = verify
 
         self.__browser_args = browser_args
 
-
     def response_hook(self, response, **kwargs) -> HTMLResponse:
-        """ Change response encoding and replace it by a HTMLResponse. """
+        """Change response encoding and replace it by a HTMLResponse."""
         if not response.encoding:
             response.encoding = DEFAULT_ENCODING
         return HTMLResponse._from_response(response, self)
 
     @property
     async def browser(self):
         if not hasattr(self, "_browser"):
             self._playwright = await async_playwright().start()
             self._browser = await self._playwright.chromium.launch(
                 headless=True, args=self.__browser_args
             )
-            # self._browser = await pyppeteer.launch(ignoreHTTPSErrors=not(self.verify), headless=True, args=self.__browser_args)
 
         return self._browser
 
 
 class HTMLSession(BaseSession):
 
     def __init__(self, **kwargs):
         super(HTMLSession, self).__init__(**kwargs)
 
     @property
     def browser(self):
         if not hasattr(self, "_browser"):
             self.loop = asyncio.get_event_loop()
             if self.loop.is_running():
-                raise RuntimeError("Cannot use HTMLSession within an existing event loop. Use AsyncHTMLSession instead.")
+                raise RuntimeError(
+                    "Cannot use HTMLSession within an existing event loop. Use AsyncHTMLSession instead."
+                )
             self._browser = self.loop.run_until_complete(super().browser)
         return self._browser
 
     def close(self):
-        """ If a browser was created close it first. """
+        """If a browser was created close it first."""
         if hasattr(self, "_browser"):
             self.loop.run_until_complete(self._browser.close())
             self.loop.run_until_complete(self._playwright.stop())
         super().close()
 
 
 class AsyncHTMLSession(BaseSession):
-    """ An async consumable session. """
+    """An async consumable session."""
 
-    def __init__(self, loop=None, workers=None,
-                 mock_browser: bool = True, *args, **kwargs):
-        """ Set or create an event loop and a thread pool.
-
-            :param loop: Asyncio loop to use.
-            :param workers: Amount of threads to use for executing async calls.
+    def __init__(
+        self,
+        loop: Optional[AbstractEventLoop] = None,
+        workers: Optional[int] = None,
+        mock_browser: bool = True,
+        *args,
+        **kwargs,
+    ):
+        """Set or create an event loop and a thread pool.
+
+        Args:
+            loop (Optional[AbstractEventLoop], optional): Asyncio loop to use.
+            workers (Optional[int], optional): Amount of threads to use for executing async calls.
                 If not pass it will default to the number of processors on the
-                machine, multiplied by 5. """
+                machine, multiplied by 5.
+
+        """
         super().__init__(*args, **kwargs)
 
         self.loop = loop or asyncio.get_event_loop()
         self.thread_pool = ThreadPoolExecutor(max_workers=workers)
 
     def request(self, *args, **kwargs):
-        """ Partial original request func and run it in a thread. """
+        """Partial original request func and run it in a thread."""
         func = partial(super().request, *args, **kwargs)
         return self.loop.run_in_executor(self.thread_pool, func)
 
     async def close(self):
-        """ If a browser was created close it first. """
+        """If a browser was created close it first."""
         if hasattr(self, "_browser"):
             await self._browser.close()
             await self._playwright.stop()
         super().close()
 
     def run(self, *coros):
-        """ Pass in all the coroutines you want to run, it will wrap each one
-            in a task, run it and wait for the result. Return a list with all
-            results, this is returned in the same order coros are passed in. """
-        tasks = [
-            asyncio.ensure_future(coro()) for coro in coros
-        ]
+        """
+        Pass in all the coroutines you want to run, it will wrap each one
+        in a task, run it and wait for the result. Return a list with all
+        results, this is returned in the same order coros are passed in.
+        """
+        tasks = [asyncio.ensure_future(coro()) for coro in coros]
         done, _ = self.loop.run_until_complete(asyncio.wait(tasks))
         return [t.result() for t in done]
```

### Comparing `requests_htmlc-0.0.4/tests/python.html` & `requests_htmlc-0.0.5/tests/python.html`

 * *Files identical despite different names*

### Comparing `requests_htmlc-0.0.4/tests/test_internet.py` & `requests_htmlc-0.0.5/tests/test_internet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import pytest
 from requests_html import HTMLSession, AsyncHTMLSession, HTMLResponse
 
 
 urls = [
-    'https://xkcd.com/1957/',
+    "https://xkcd.com/1957/",
     # TODO: pagination in github CI not working for reddit
     # 'https://www.reddit.com/',
-    'https://github.com/psf/requests-html/issues',
-    'https://discord.com/category/engineering',
-    'https://stackoverflow.com/',
-    'https://www.frontiersin.org/',
-    'https://azure.microsoft.com/en-us'
+    "https://github.com/psf/requests-html/issues",
+    "https://discord.com/category/engineering",
+    "https://stackoverflow.com/",
+    "https://www.frontiersin.org/",
+    "https://azure.microsoft.com/en-us",
 ]
 
 
-@pytest.mark.parametrize('url', urls)
+@pytest.mark.parametrize("url", urls)
 @pytest.mark.internet
 def test_pagination(url: str):
     session = HTMLSession()
     r = session.get(url)
     assert next(r.html)
 
 
-@pytest.mark.parametrize('url', urls)
+@pytest.mark.parametrize("url", urls)
 @pytest.mark.internet
 @pytest.mark.asyncio
 async def test_async_pagination(event_loop, url):
     asession = AsyncHTMLSession()
 
     r = await asession.get(url)
     assert await r.html.__anext__()
@@ -34,15 +34,17 @@
 
 @pytest.mark.internet
 def test_async_run():
     asession = AsyncHTMLSession()
 
     async_list = []
     for url in urls:
+
         async def _test():
             return await asession.get(url)
+
         async_list.append(_test)
 
     r = asession.run(*async_list)
 
     assert len(r) == len(urls)
     assert isinstance(r[0], HTMLResponse)
```

### Comparing `requests_htmlc-0.0.4/tests/test_requests_html.py` & `requests_htmlc-0.0.5/tests/test_requests_html.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import pytest
 from playwright.async_api import async_playwright
 from playwright.async_api import Browser
 from requests_html import HTMLSession, AsyncHTMLSession, HTML
 from requests_file import FileAdapter
 
 session = HTMLSession()
-session.mount('file://', FileAdapter())
+session.mount("file://", FileAdapter())
 
 
 def get():
-    path = os.path.sep.join((os.path.dirname(os.path.abspath(__file__)), 'python.html'))
-    url = f'file://{path}'
+    path = os.path.sep.join((os.path.dirname(os.path.abspath(__file__)), "python.html"))
+    url = f"file://{path}"
 
     return session.get(url)
 
 
 @pytest.fixture
 def async_get(event_loop):
     """AsyncSession cannot be created global since it will create
-        a different loop from pytest-asyncio. """
+    a different loop from pytest-asyncio."""
     async_session = AsyncHTMLSession()
-    async_session.mount('file://', FileAdapter())
-    path = os.path.sep.join((os.path.dirname(os.path.abspath(__file__)), 'python.html'))
-    url = 'file://{}'.format(path)
+    async_session.mount("file://", FileAdapter())
+    path = os.path.sep.join((os.path.dirname(os.path.abspath(__file__)), "python.html"))
+    url = "file://{}".format(path)
 
     return partial(async_session.get, url)
 
 
 def test_file_get():
     r = get()
     assert r.status_code == 200
@@ -40,127 +40,135 @@
     r = await async_get()
     assert r.status_code == 200
 
 
 def test_class_seperation():
     r = get()
 
-    about = r.html.find('#about', first=True)
-    assert len(about.attrs['class']) == 2
+    about = r.html.find("#about", first=True)
+    assert len(about.attrs["class"]) == 2
 
 
 def test_css_selector():
     r = get()
 
-    about = r.html.find('#about', first=True)
+    about = r.html.find("#about", first=True)
 
     for menu_item in (
-            'About', 'Applications', 'Quotes', 'Getting Started', 'Help',
-            'Python Brochure'
+        "About",
+        "Applications",
+        "Quotes",
+        "Getting Started",
+        "Help",
+        "Python Brochure",
     ):
-        assert menu_item in about.text.split('\n')
-        assert menu_item in about.full_text.split('\n')
+        assert menu_item in about.text.split("\n")
+        assert menu_item in about.full_text.split("\n")
 
 
 def test_containing():
     r = get()
 
-    python = r.html.find(containing='python')
+    python = r.html.find(containing="python")
     assert len(python) == 192
 
     for e in python:
-        assert 'python' in e.full_text.lower()
+        assert "python" in e.full_text.lower()
 
 
 def test_attrs():
     r = get()
-    about = r.html.find('#about', first=True)
+    about = r.html.find("#about", first=True)
 
-    assert 'aria-haspopup' in about.attrs
-    assert len(about.attrs['class']) == 2
+    assert "aria-haspopup" in about.attrs
+    assert len(about.attrs["class"]) == 2
 
 
 def test_links():
     r = get()
-    about = r.html.find('#about', first=True)
+    about = r.html.find("#about", first=True)
 
     assert len(about.links) == 6
     assert len(about.absolute_links) == 6
 
 
 @pytest.mark.asyncio
 async def test_async_links(async_get):
     r = await async_get()
-    about = r.html.find('#about', first=True)
+    about = r.html.find("#about", first=True)
 
     assert len(about.links) == 6
     assert len(about.absolute_links) == 6
 
 
 def test_search():
     r = get()
-    style = r.html.search('Python is a {} language')[0]
-    assert style == 'programming'
+    style = r.html.search("Python is a {} language")[0]
+    assert style == "programming"
 
 
 def test_xpath():
     r = get()
-    html = r.html.xpath('/html', first=True)
-    assert 'no-js' in html.attrs['class']
+    html = r.html.xpath("/html", first=True)
+    assert "no-js" in html.attrs["class"]
 
-    a_hrefs = r.html.xpath('//a/@href')
-    assert '#site-map' in a_hrefs
+    a_hrefs = r.html.xpath("//a/@href")
+    assert "#site-map" in a_hrefs
 
 
 def test_html_loading():
     doc = """<a href='https://httpbin.org'>"""
     html = HTML(html=doc)
 
-    assert 'https://httpbin.org' in html.links
+    assert "https://httpbin.org" in html.links
     assert isinstance(html.raw_html, bytes)
     assert isinstance(html.html, str)
 
 
 def test_anchor_links():
     r = get()
     r.html.skip_anchors = False
 
-    assert '#site-map' in r.html.links
+    assert "#site-map" in r.html.links
 
 
-@pytest.mark.parametrize('url,link,expected', [
-    ('http://example.com/', 'test.html', 'http://example.com/test.html'),
-    ('http://example.com', 'test.html', 'http://example.com/test.html'),
-    ('http://example.com/foo/', 'test.html', 'http://example.com/foo/test.html'),
-    ('http://example.com/foo/bar', 'test.html', 'http://example.com/foo/test.html'),
-    ('http://example.com/foo/', '/test.html', 'http://example.com/test.html'),
-    ('http://example.com/', 'http://xkcd.com/about/', 'http://xkcd.com/about/'),
-    ('http://example.com/', '//xkcd.com/about/', 'http://xkcd.com/about/'),
-])
+@pytest.mark.parametrize(
+    "url,link,expected",
+    [
+        ("http://example.com/", "test.html", "http://example.com/test.html"),
+        ("http://example.com", "test.html", "http://example.com/test.html"),
+        ("http://example.com/foo/", "test.html", "http://example.com/foo/test.html"),
+        ("http://example.com/foo/bar", "test.html", "http://example.com/foo/test.html"),
+        ("http://example.com/foo/", "/test.html", "http://example.com/test.html"),
+        ("http://example.com/", "http://xkcd.com/about/", "http://xkcd.com/about/"),
+        ("http://example.com/", "//xkcd.com/about/", "http://xkcd.com/about/"),
+    ],
+)
 def test_absolute_links(url, link, expected):
     head_template = """<head><base href='{}'></head>"""
     body_template = """<body><a href='{}'>Next</a></body>"""
 
     # Test without `<base>` tag (url is base)
     html = HTML(html=body_template.format(link), url=url)
     assert html.absolute_links.pop() == expected
 
     # Test with `<base>` tag (url is other)
     html = HTML(
         html=head_template.format(url) + body_template.format(link),
-        url='http://example.com/foobar/')
+        url="http://example.com/foobar/",
+    )
     assert html.absolute_links.pop() == expected
 
 
 def test_parser():
     doc = """<a href='https://httpbin.org'>httpbin.org\n</a>"""
     html = HTML(html=doc)
 
-    assert html.find('html')
-    assert html.element('a').text().strip() == 'httpbin.org'
+    assert html.find("html")
+    assert html.element("a").text().strip() == "httpbin.org"
 
 
 @pytest.mark.render
 def test_render():
     r = get()
     script = """
     () => {
@@ -168,18 +176,18 @@
             width: document.documentElement.clientWidth,
             height: document.documentElement.clientHeight,
             deviceScaleFactor: window.devicePixelRatio,
         }
     }
     """
     val = r.html.render(script=script)
-    for value in ('width', 'height', 'deviceScaleFactor'):
+    for value in ("width", "height", "deviceScaleFactor"):
         assert value in val
 
-    about = r.html.find('#about', first=True)
+    about = r.html.find("#about", first=True)
     assert len(about.links) == 6
 
 
 @pytest.mark.render
 @pytest.mark.asyncio
 async def test_async_render(async_get):
     r = await async_get()
@@ -189,18 +197,18 @@
             width: document.documentElement.clientWidth,
             height: document.documentElement.clientHeight,
             deviceScaleFactor: window.devicePixelRatio,
         }
     }
     """
     val = await r.html.arender(script=script)
-    for value in ('width', 'height', 'deviceScaleFactor'):
+    for value in ("width", "height", "deviceScaleFactor"):
         assert value in val
 
-    about = r.html.find('#about', first=True)
+    about = r.html.find("#about", first=True)
     assert len(about.links) == 6
     await r.html.browser.close()
 
 
 @pytest.mark.render
 def test_bare_render():
     doc = """<a href='https://httpbin.org'>"""
@@ -211,19 +219,19 @@
                 width: document.documentElement.clientWidth,
                 height: document.documentElement.clientHeight,
                 deviceScaleFactor: window.devicePixelRatio,
             }
         }
     """
     val = html.render(script=script, reload=False)
-    for value in ('width', 'height', 'deviceScaleFactor'):
+    for value in ("width", "height", "deviceScaleFactor"):
         assert value in val
 
-    assert html.find('html')
-    assert 'https://httpbin.org' in html.links
+    assert html.find("html")
+    assert "https://httpbin.org" in html.links
 
 
 @pytest.mark.render
 @pytest.mark.asyncio
 async def test_bare_arender():
     doc = """<a href='https://httpbin.org'>"""
     html = HTML(html=doc, async_=True)
@@ -233,19 +241,19 @@
                 width: document.documentElement.clientWidth,
                 height: document.documentElement.clientHeight,
                 deviceScaleFactor: window.devicePixelRatio,
             }
         }
     """
     val = await html.arender(script=script, reload=False)
-    for value in ('width', 'height', 'deviceScaleFactor'):
+    for value in ("width", "height", "deviceScaleFactor"):
         assert value in val
 
-    assert html.find('html')
-    assert 'https://httpbin.org' in html.links
+    assert html.find("html")
+    assert "https://httpbin.org" in html.links
     await html.browser.close()
 
 
 @pytest.mark.render
 def test_bare_js_eval():
     doc = """
     <!DOCTYPE html>
@@ -259,15 +267,15 @@
     </body>
     </html>
     """
 
     html = HTML(html=doc)
     html.render()
 
-    assert html.find('#replace', first=True).text == 'yolo'
+    assert html.find("#replace", first=True).text == "yolo"
 
 
 @pytest.mark.render
 @pytest.mark.asyncio
 async def test_bare_js_async_eval():
     doc = """
     <!DOCTYPE html>
@@ -281,41 +289,42 @@
     </body>
     </html>
     """
 
     html = HTML(html=doc, async_=True)
     await html.arender()
 
-    assert html.find('#replace', first=True).text == 'yolo'
+    assert html.find("#replace", first=True).text == "yolo"
     await html.browser.close()
 
 
 def test_browser_session():
-    """ Test browser instances is created and properly close when session is closed.
-        Note: session.close method need to be tested together with browser creation,
-            since not doing that will leave the browser running. """
+    """Test browser instances is created and properly close when session is closed.
+    Note: session.close method need to be tested together with browser creation,
+        since not doing that will leave the browser running."""
     session = HTMLSession()
     assert isinstance(session.browser, Browser)
     assert hasattr(session, "loop")
     session.close()
     # assert count_chromium_process() == 0
 
+
 # TODO: debug this test as it only works if running alone,
 # not amongst all others
 # def test_browser_process():
 #     for _ in range(3):
 #         r = get()
 #         r.html.render()
 
 #         assert r.html.page is None
 
 
 @pytest.mark.asyncio
 async def test_browser_session_fail():
-    """ HTMLSession.browser should not be call within an existing event loop> """
+    """HTMLSession.browser should not be call within an existing event loop>"""
     session = HTMLSession()
     with pytest.raises(RuntimeError):
         session.browser
 
 
 @pytest.mark.asyncio
 async def test_async_browser_session():
```

