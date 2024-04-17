# Comparing `tmp/python_package_template_pypi-0.0.3.tar.gz` & `tmp/python_package_template_pypi-0.0.4.tar.gz`

## Comparing `python_package_template_pypi-0.0.3.tar` & `python_package_template_pypi-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/readthedocs.yml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/ruff.toml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/tox.ini
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/CODEOWNERS
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/ISSUE_TEMPLATE/feature.yml
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/docs/add_five.rst
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/docs/conf.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/docs/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/docs/_static/.gitkeep
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/src/python_package_template/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/src/python_package_template/main.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/tests/main_test.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/LICENSE
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/README.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/hatch.toml
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/readthedocs.yml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/ruff.toml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/tox.ini
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.github/ISSUE_TEMPLATE/feature.yml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/docs/add_five.rst
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/docs/conf.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/docs/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/src/python_package_template/__init__.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/src/python_package_template/main.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/tests/main_test.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/README.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/hatch.toml
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8800 2020-02-02 00:00:00.000000 python_package_template_pypi-0.0.4/PKG-INFO
```

### Comparing `python_package_template_pypi-0.0.3/.pre-commit-config.yaml` & `python_package_template_pypi-0.0.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,14 @@
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: name-tests-test
       - id: trailing-whitespace
 
   # ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.3.7
     hooks:
       # Ruff linting
       - id: ruff
         args: [--line-length=120]
       # Ruff formatting
       - id: ruff-format
```

### Comparing `python_package_template_pypi-0.0.3/ruff.toml` & `python_package_template_pypi-0.0.4/ruff.toml`

 * *Files identical despite different names*

### Comparing `python_package_template_pypi-0.0.3/.github/ISSUE_TEMPLATE/bug.yml` & `python_package_template_pypi-0.0.4/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `python_package_template_pypi-0.0.3/docs/conf.py` & `python_package_template_pypi-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_package_template_pypi-0.0.3/LICENSE` & `python_package_template_pypi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_package_template_pypi-0.0.3/README.md` & `python_package_template_pypi-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 - [ReadTheDocs](https://readthedocs.org/) - Documentation hosting
 - [GitHub Pages](https://pages.github.com/) - Documentation hosting
 
 ### Codecov
 Codecov is used to check the code coverage of the tests.\
 It also provides a badge that can be added to the README file.
 
-The way it is set up can be seen in the `.github/workflows/ci.yml` file, but it will probably be moved to my reusable [GitHub Workflows repository](https://github.com/daniel-mizsak/workflows).
+Codecov is set up to be part of the [tox reusable workflow](https://github.com/daniel-mizsak/workflows/blob/main/.github/workflows/tox.yml), but for this action it is important to generate the coverage report using the `--cov-report=xml` flag in the `pyproject.toml` file.
 
 ### Pre-Commit
 Pre-Commit is used to run certain checks on the code before it is committed.\
 These checks are defined in the `.pre-commit-config.yaml` file.\
 To use pre-commit is has to be installed in the virtual environment and also added to the git hooks by running `pre-commit install`.
 
 In this repository pre-commit is set up for a number of general issues and to run formatting and linting checks with `ruff`.
```

#### html2text {}

```diff
@@ -11,25 +11,26 @@
 checking - [Pytest](https://docs.pytest.org/en/latest/) - Testing and code
 coverage - [Ruff](https://docs.astral.sh/ruff/) - Formatting and linting -
 [Tox](https://tox.readthedocs.io/en/latest/) - Orchestration of the above tools
 For documentation: - [Sphinx](https://www.sphinx-doc.org/en/master/) -
 Documentation building - [ReadTheDocs](https://readthedocs.org/) -
 Documentation hosting - [GitHub Pages](https://pages.github.com/) -
 Documentation hosting ### Codecov Codecov is used to check the code coverage of
-the tests.\ It also provides a badge that can be added to the README file. The
-way it is set up can be seen in the `.github/workflows/ci.yml` file, but it
-will probably be moved to my reusable [GitHub Workflows repository](https://
-github.com/daniel-mizsak/workflows). ### Pre-Commit Pre-Commit is used to run
-certain checks on the code before it is committed.\ These checks are defined in
-the `.pre-commit-config.yaml` file.\ To use pre-commit is has to be installed
-in the virtual environment and also added to the git hooks by running `pre-
-commit install`. In this repository pre-commit is set up for a number of
-general issues and to run formatting and linting checks with `ruff`. ### Hatch
-Hatch is primarily used to build the package, but it can also be used to run
-certain tests in isolated environments.\ If the package building is more
+the tests.\ It also provides a badge that can be added to the README file.
+Codecov is set up to be part of the [tox reusable workflow](https://github.com/
+daniel-mizsak/workflows/blob/main/.github/workflows/tox.yml), but for this
+action it is important to generate the coverage report using the `--cov-
+report=xml` flag in the `pyproject.toml` file. ### Pre-Commit Pre-Commit is
+used to run certain checks on the code before it is committed.\ These checks
+are defined in the `.pre-commit-config.yaml` file.\ To use pre-commit is has to
+be installed in the virtual environment and also added to the git hooks by
+running `pre-commit install`. In this repository pre-commit is set up for a
+number of general issues and to run formatting and linting checks with `ruff`.
+### Hatch Hatch is primarily used to build the package, but it can also be used
+to run certain tests in isolated environments.\ If the package building is more
 complex and requires additional settings or files it is recommended to read the
 hatch documentation.\ In this repository hatch is set up with the local path of
 the package as it differs from the one specified in the `pyproject.toml` file
 which is used for publishing to PyPI. The isolated environment settings for
 hatch are defined in the `hatch.toml` file.\ I was thinking about replacing
 `tox` with `hatch`, but for now `tox` fits more into my workflows. ### MyPy
 Python by default is a dynamically typed language, but being explicit about
```

### Comparing `python_package_template_pypi-0.0.3/pyproject.toml` & `python_package_template_pypi-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Project Metadata
 [project]
 name = "python-package-template-pypi" # Name has to be unique on pypi.
-version = "0.0.3"
+version = "0.0.4"
 description = "A github template with my python package configurations."
 readme = "README.md"
-requires-python = ">=3.12"
+requires-python = ">=3.11"
 license = { file = "LICENSE" }
 authors = [{ name = "Daniel Mizsak", email = "info@pythonvilag.hu" }]
 keywords = []
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = []
 [project.optional-dependencies]
 dev = ["hatch", "mypy", "pre-commit", "pytest-cov", "pytest", "ruff", "tox"]
 docs = ["furo", "sphinx", "sphinx-copybutton"]
 [project.urls]
@@ -38,9 +39,9 @@
 show_error_context = true
 strict = true
 warn_unreachable = true
 warn_unused_ignores = true
 
 # Pytest
 [tool.pytest.ini_options]
-addopts = "--cov=python_package_template --cov=tests --cov-config=pyproject.toml --cov-report=term-missing --cov-report=html"
+addopts = "--cov=python_package_template --cov=tests --cov-config=pyproject.toml --cov-report=term-missing --cov-report=html --cov-report=xml"
 testpaths = ["tests"]
```

### Comparing `python_package_template_pypi-0.0.3/PKG-INFO` & `python_package_template_pypi-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-package-template-pypi
-Version: 0.0.3
+Version: 0.0.4
 Summary: A github template with my python package configurations.
 Project-URL: Repository, https://github.com/daniel-mizsak/python-package-template
 Author-email: Daniel Mizsak <info@pythonvilag.hu>
 License: MIT License
         
         Copyright (c) Daniel Mizsak
         
@@ -24,16 +24,17 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
@@ -73,15 +74,15 @@
 - [ReadTheDocs](https://readthedocs.org/) - Documentation hosting
 - [GitHub Pages](https://pages.github.com/) - Documentation hosting
 
 ### Codecov
 Codecov is used to check the code coverage of the tests.\
 It also provides a badge that can be added to the README file.
 
-The way it is set up can be seen in the `.github/workflows/ci.yml` file, but it will probably be moved to my reusable [GitHub Workflows repository](https://github.com/daniel-mizsak/workflows).
+Codecov is set up to be part of the [tox reusable workflow](https://github.com/daniel-mizsak/workflows/blob/main/.github/workflows/tox.yml), but for this action it is important to generate the coverage report using the `--cov-report=xml` flag in the `pyproject.toml` file.
 
 ### Pre-Commit
 Pre-Commit is used to run certain checks on the code before it is committed.\
 These checks are defined in the `.pre-commit-config.yaml` file.\
 To use pre-commit is has to be installed in the virtual environment and also added to the git hooks by running `pre-commit install`.
 
 In this repository pre-commit is set up for a number of general issues and to run formatting and linting checks with `ruff`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: python-package-template-pypi Version: 0.0.3
+Metadata-Version: 2.3 Name: python-package-template-pypi Version: 0.0.4
 Summary: A github template with my python package configurations. Project-URL:
 Repository, https://github.com/daniel-mizsak/python-package-template Author-
 email: Daniel Mizsak
 pythonvilag.hu> License: MIT License Copyright (c) Daniel Mizsak Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -14,22 +14,22 @@
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. License-File: LICENSE Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.12
-Provides-Extra: dev Requires-Dist: hatch; extra == 'dev' Requires-Dist: mypy;
-extra == 'dev' Requires-Dist: pre-commit; extra == 'dev' Requires-Dist: pytest;
-extra == 'dev' Requires-Dist: pytest-cov; extra == 'dev' Requires-Dist: ruff;
-extra == 'dev' Requires-Dist: tox; extra == 'dev' Provides-Extra: docs
-Requires-Dist: furo; extra == 'docs' Requires-Dist: sphinx; extra == 'docs'
-Requires-Dist: sphinx-copybutton; extra == 'docs' Description-Content-Type:
-text/markdown ##
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Python: >=3.11 Provides-Extra: dev
+Requires-Dist: hatch; extra == 'dev' Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev' Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev' Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: tox; extra == 'dev' Provides-Extra: docs Requires-Dist: furo;
+extra == 'docs' Requires-Dist: sphinx; extra == 'docs' Requires-Dist: sphinx-
+copybutton; extra == 'docs' Description-Content-Type: text/markdown ##
                          ð python-package-template
   _[_b_u_i_l_d_ _s_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_d_a_n_i_e_l_-_m_i_z_s_a_k_/_p_y_t_h_o_n_-_p_a_c_k_a_g_e_-_t_e_m_p_l_a_t_e_/
  _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_S_D_X_G_1_S_8_P_V_M_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]_[_d_o_c_s_ _s_t_a_t_u_s_]_[_l_i_c_e_n_s_e_]
 ## Overview A GitHub template with my python package configurations. ## Package
 tools This template package relies on the synchronized cooperation of several
 exceptional tools.\ These tools include: - [Codecov](https://docs.codecov.com/
 docs/quick-start) - Code coverage - [Pre-Commit](https://pre-commit.com/) - Git
@@ -38,25 +38,26 @@
 checking - [Pytest](https://docs.pytest.org/en/latest/) - Testing and code
 coverage - [Ruff](https://docs.astral.sh/ruff/) - Formatting and linting -
 [Tox](https://tox.readthedocs.io/en/latest/) - Orchestration of the above tools
 For documentation: - [Sphinx](https://www.sphinx-doc.org/en/master/) -
 Documentation building - [ReadTheDocs](https://readthedocs.org/) -
 Documentation hosting - [GitHub Pages](https://pages.github.com/) -
 Documentation hosting ### Codecov Codecov is used to check the code coverage of
-the tests.\ It also provides a badge that can be added to the README file. The
-way it is set up can be seen in the `.github/workflows/ci.yml` file, but it
-will probably be moved to my reusable [GitHub Workflows repository](https://
-github.com/daniel-mizsak/workflows). ### Pre-Commit Pre-Commit is used to run
-certain checks on the code before it is committed.\ These checks are defined in
-the `.pre-commit-config.yaml` file.\ To use pre-commit is has to be installed
-in the virtual environment and also added to the git hooks by running `pre-
-commit install`. In this repository pre-commit is set up for a number of
-general issues and to run formatting and linting checks with `ruff`. ### Hatch
-Hatch is primarily used to build the package, but it can also be used to run
-certain tests in isolated environments.\ If the package building is more
+the tests.\ It also provides a badge that can be added to the README file.
+Codecov is set up to be part of the [tox reusable workflow](https://github.com/
+daniel-mizsak/workflows/blob/main/.github/workflows/tox.yml), but for this
+action it is important to generate the coverage report using the `--cov-
+report=xml` flag in the `pyproject.toml` file. ### Pre-Commit Pre-Commit is
+used to run certain checks on the code before it is committed.\ These checks
+are defined in the `.pre-commit-config.yaml` file.\ To use pre-commit is has to
+be installed in the virtual environment and also added to the git hooks by
+running `pre-commit install`. In this repository pre-commit is set up for a
+number of general issues and to run formatting and linting checks with `ruff`.
+### Hatch Hatch is primarily used to build the package, but it can also be used
+to run certain tests in isolated environments.\ If the package building is more
 complex and requires additional settings or files it is recommended to read the
 hatch documentation.\ In this repository hatch is set up with the local path of
 the package as it differs from the one specified in the `pyproject.toml` file
 which is used for publishing to PyPI. The isolated environment settings for
 hatch are defined in the `hatch.toml` file.\ I was thinking about replacing
 `tox` with `hatch`, but for now `tox` fits more into my workflows. ### MyPy
 Python by default is a dynamically typed language, but being explicit about
```

