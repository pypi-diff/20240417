# Comparing `tmp/sphinx-7.2.5.tar.gz` & `tmp/sphinx-7.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-7.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx-7.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx-7.2.5.tar` & `sphinx-7.2.6.tar`

### file list

```diff
@@ -1,1664 +1,1664 @@
--rw-r--r--   0        0        0     3818 2023-08-30 22:09:32.752402 sphinx-7.2.5/AUTHORS
--rw-r--r--   0        0        0   381778 2023-08-30 22:09:32.756402 sphinx-7.2.5/CHANGES
--rw-r--r--   0        0        0     3530 2023-08-30 22:09:32.756402 sphinx-7.2.5/CODE_OF_CONDUCT
--rw-r--r--   0        0        0    26147 2023-08-30 22:09:32.756402 sphinx-7.2.5/EXAMPLES
--rw-r--r--   0        0        0     3135 2023-08-30 22:09:32.756402 sphinx-7.2.5/LICENSE
--rw-r--r--   0        0        0     2323 2023-08-30 22:09:32.756402 sphinx-7.2.5/README.rst
--rw-r--r--   0        0        0      607 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/Makefile
--rw-r--r--   0        0        0      152 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/Makefile
--rw-r--r--   0        0        0    27523 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/bookcover.png
--rw-r--r--   0        0        0     9875 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/conf.py.txt
--rw-r--r--   0        0        0     3307 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/favicon.svg
--rw-r--r--   0        0        0     1351 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/more.png
--rw-r--r--   0        0        0    34213 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/sphinx.png
--rw-r--r--   0        0        0    25792 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/themes/agogo.png
--rw-r--r--   0        0        0    32356 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/themes/alabaster.png
--rw-r--r--   0        0        0    27139 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/themes/bizstyle.png
--rw-r--r--   0        0        0    39927 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/themes/classic.png
--rw-r--r--   0        0        0    56954 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/themes/fullsize/agogo.png
--rw-r--r--   0        0        0    40248 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/themes/fullsize/alabaster.png
--rw-r--r--   0        0        0    75192 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/themes/fullsize/bizstyle.png
--rw-r--r--   0        0        0    72597 2023-08-30 22:09:32.756402 sphinx-7.2.5/doc/_static/themes/fullsize/classic.png
--rw-r--r--   0        0        0    84200 2023-08-30 22:09:32.760402 sphinx-7.2.5/doc/_static/themes/fullsize/haiku.png
--rw-r--r--   0        0        0    32266 2023-08-30 22:09:32.760402 sphinx-7.2.5/doc/_static/themes/fullsize/nature.png
--rw-r--r--   0        0        0   102717 2023-08-30 22:09:32.760402 sphinx-7.2.5/doc/_static/themes/fullsize/pyramid.png
--rw-r--r--   0        0        0    88111 2023-08-30 22:09:32.760402 sphinx-7.2.5/doc/_static/themes/fullsize/scrolls.png
--rw-r--r--   0        0        0    39411 2023-08-30 22:09:32.760402 sphinx-7.2.5/doc/_static/themes/fullsize/sphinx_rtd_theme.png
--rw-r--r--   0        0        0    84439 2023-08-30 22:09:32.760402 sphinx-7.2.5/doc/_static/themes/fullsize/sphinxdoc.png
--rw-r--r--   0        0        0    91744 2023-08-30 22:09:32.760402 sphinx-7.2.5/doc/_static/themes/fullsize/traditional.png
--rw-r--r--   0        0        0    43184 2023-08-30 22:09:32.760402 sphinx-7.2.5/doc/_static/themes/haiku.png
--rw-r--r--   0        0        0    28536 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/themes/nature.png
--rw-r--r--   0        0        0    38805 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/themes/pyramid.png
--rw-r--r--   0        0        0    27800 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/themes/scrolls.png
--rw-r--r--   0        0        0    29138 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/themes/sphinx_rtd_theme.png
--rw-r--r--   0        0        0    30225 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/themes/sphinxdoc.png
--rw-r--r--   0        0        0    32258 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/themes/traditional.png
--rw-r--r--   0        0        0    16371 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/translation.png
--rw-r--r--   0        0        0      342 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/translation.puml
--rw-r--r--   0        0        0     8232 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/translation.svg
--rw-r--r--   0        0        0    26500 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/tutorial/lumache-autosummary.png
--rw-r--r--   0        0        0    52126 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/tutorial/lumache-first-light.png
--rw-r--r--   0        0        0    51223 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/tutorial/lumache-furo.png
--rw-r--r--   0        0        0    71741 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/tutorial/lumache-py-function-full.png
--rw-r--r--   0        0        0    41828 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_static/tutorial/lumache-py-function.png
--rw-r--r--   0        0        0      271 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_templates/contents.html
--rw-r--r--   0        0        0     1860 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_themes/sphinx13/layout.html
--rw-r--r--   0        0        0     6552 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_themes/sphinx13/static/sphinx13.css
--rw-r--r--   0        0        0    11719 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_themes/sphinx13/static/sphinxheader.png
--rw-r--r--   0        0        0       60 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/_themes/sphinx13/theme.conf
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/authors.rst
--rw-r--r--   0        0        0      400 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/changes.rst
--rw-r--r--   0        0        0     9259 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/conf.py
--rw-r--r--   0        0        0     1151 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/builders.rst
--rw-r--r--   0        0        0      649 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/index.rst
--rw-r--r--   0        0        0     1051 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/overview.rst
--rw-r--r--   0        0        0    15049 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/templating.rst
--rw-r--r--   0        0        0    12324 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/theming.rst
--rw-r--r--   0        0        0     4020 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/autodoc_ext.rst
--rw-r--r--   0        0        0      438 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/examples/README.rst
--rw-r--r--   0        0        0     1844 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/examples/autodoc_intenum.py
--rw-r--r--   0        0        0      400 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/examples/helloworld.py
--rw-r--r--   0        0        0     5030 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/examples/recipe.py
--rw-r--r--   0        0        0     3942 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/examples/todo.py
--rw-r--r--   0        0        0     5289 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/helloworld.rst
--rw-r--r--   0        0        0      262 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/index.rst
--rw-r--r--   0        0        0     8216 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/recipe.rst
--rw-r--r--   0        0        0    13435 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/development/tutorials/todo.rst
--rw-r--r--   0        0        0       54 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/examples.rst
--rw-r--r--   0        0        0    14996 2023-08-30 22:09:32.764402 sphinx-7.2.5/doc/extdev/appapi.rst
--rw-r--r--   0        0        0     1103 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/builderapi.rst
--rw-r--r--   0        0        0      165 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/collectorapi.rst
--rw-r--r--   0        0        0    41794 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/deprecated.rst
--rw-r--r--   0        0        0      518 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/domainapi.rst
--rw-r--r--   0        0        0     1043 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/envapi.rst
--rw-r--r--   0        0        0     2817 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/i18n.rst
--rw-r--r--   0        0        0     8597 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/index.rst
--rw-r--r--   0        0        0     2384 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/logging.rst
--rw-r--r--   0        0        0     4787 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/markupapi.rst
--rw-r--r--   0        0        0     2706 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/nodes.rst
--rw-r--r--   0        0        0     1243 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/parserapi.rst
--rw-r--r--   0        0        0      114 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/projectapi.rst
--rw-r--r--   0        0        0      943 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/extdev/utils.rst
--rw-r--r--   0        0        0    13425 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/faq.rst
--rw-r--r--   0        0        0     4173 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/glossary.rst
--rw-r--r--   0        0        0     3539 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/index.rst
--rw-r--r--   0        0        0       71 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/internals/code-of-conduct.rst
--rw-r--r--   0        0        0    11482 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/internals/contributing.rst
--rw-r--r--   0        0        0      353 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/internals/index.rst
--rw-r--r--   0        0        0     1964 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/internals/organization.rst
--rw-r--r--   0        0        0     4395 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/internals/release-process.rst
--rw-r--r--   0        0        0    69427 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/latex.rst
--rw-r--r--   0        0        0      784 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/make.bat
--rw-r--r--   0        0        0      314 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/man/index.rst
--rw-r--r--   0        0        0     4508 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/man/sphinx-apidoc.rst
--rw-r--r--   0        0        0     2122 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/man/sphinx-autogen.rst
--rw-r--r--   0        0        0    10673 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/man/sphinx-build.rst
--rw-r--r--   0        0        0     3692 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/man/sphinx-quickstart.rst
--rw-r--r--   0        0        0      806 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/support.rst
--rw-r--r--   0        0        0     4981 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/automatic-doc-generation.rst
--rw-r--r--   0        0        0    11090 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/deploying.rst
--rw-r--r--   0        0        0     9134 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/describing-code.rst
--rw-r--r--   0        0        0      240 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/end.rst
--rw-r--r--   0        0        0     3450 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/first-steps.rst
--rw-r--r--   0        0        0     3723 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/getting-started.rst
--rw-r--r--   0        0        0     1433 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/index.rst
--rw-r--r--   0        0        0     2528 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/more-sphinx-customization.rst
--rw-r--r--   0        0        0     4177 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/tutorial/narrative-documentation.rst
--rw-r--r--   0        0        0    11831 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/usage/advanced/intl.rst
--rw-r--r--   0        0        0     2670 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/usage/advanced/websupport/api.rst
--rw-r--r--   0        0        0      302 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/usage/advanced/websupport/index.rst
--rw-r--r--   0        0        0     9640 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/usage/advanced/websupport/quickstart.rst
--rw-r--r--   0        0        0     1368 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/usage/advanced/websupport/searchadapters.rst
--rw-r--r--   0        0        0     1231 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/usage/advanced/websupport/storagebackends.rst
--rw-r--r--   0        0        0    17742 2023-08-30 22:09:32.768403 sphinx-7.2.5/doc/usage/builders/index.rst
--rw-r--r--   0        0        0   103770 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/configuration.rst
--rw-r--r--   0        0        0    29866 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/autodoc.rst
--rw-r--r--   0        0        0     1899 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/autosectionlabel.rst
--rw-r--r--   0        0        0    11099 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/autosummary.rst
--rw-r--r--   0        0        0     2832 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/coverage.rst
--rw-r--r--   0        0        0    12084 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/doctest.rst
--rw-r--r--   0        0        0      404 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/duration.rst
--rw-r--r--   0        0        0     9665 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/example_google.py
--rw-r--r--   0        0        0      296 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/example_google.rst
--rw-r--r--   0        0        0     9714 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/example_numpy.py
--rw-r--r--   0        0        0      292 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/example_numpy.rst
--rw-r--r--   0        0        0     2781 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/extlinks.rst
--rw-r--r--   0        0        0      491 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/githubpages.rst
--rw-r--r--   0        0        0     6292 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/graphviz.rst
--rw-r--r--   0        0        0     1329 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/ifconfig.rst
--rw-r--r--   0        0        0     1705 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/imgconverter.rst
--rw-r--r--   0        0        0     2410 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/index.rst
--rw-r--r--   0        0        0     5598 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/inheritance.rst
--rw-r--r--   0        0        0     9934 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/intersphinx.rst
--rw-r--r--   0        0        0     1756 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/linkcode.rst
--rw-r--r--   0        0        0    11756 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/math.rst
--rw-r--r--   0        0        0    15980 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/napoleon.rst
--rw-r--r--   0        0        0     1644 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/todo.rst
--rw-r--r--   0        0        0     3917 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/extensions/viewcode.rst
--rw-r--r--   0        0        0      537 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/index.rst
--rw-r--r--   0        0        0     7146 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/installation.rst
--rw-r--r--   0        0        0     1584 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/markdown.rst
--rw-r--r--   0        0        0    13150 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/quickstart.rst
--rw-r--r--   0        0        0    20508 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/restructuredtext/basics.rst
--rw-r--r--   0        0        0    46040 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/restructuredtext/directives.rst
--rw-r--r--   0        0        0    69567 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/restructuredtext/domains.rst
--rw-r--r--   0        0        0     1967 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/restructuredtext/field-lists.rst
--rw-r--r--   0        0        0      574 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/restructuredtext/index.rst
--rw-r--r--   0        0        0    18409 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/restructuredtext/roles.rst
--rw-r--r--   0        0        0    14326 2023-08-30 22:09:32.772403 sphinx-7.2.5/doc/usage/theming.rst
--rw-r--r--   0        0        0    15097 2023-08-30 22:09:32.772403 sphinx-7.2.5/pyproject.toml
--rw-r--r--   0        0        0     1852 2023-08-30 22:09:32.772403 sphinx-7.2.5/sphinx/__init__.py
--rw-r--r--   0        0        0      127 2023-08-30 22:09:32.772403 sphinx-7.2.5/sphinx/__main__.py
--rw-r--r--   0        0        0    19226 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/addnodes.py
--rw-r--r--   0        0        0    56426 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/application.py
--rw-r--r--   0        0        0    26942 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/__init__.py
--rw-r--r--   0        0        0    28962 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/_epub_base.py
--rw-r--r--   0        0        0     6531 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/changes.py
--rw-r--r--   0        0        0     1542 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/dirhtml.py
--rw-r--r--   0        0        0     1024 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/dummy.py
--rw-r--r--   0        0        0    11439 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/epub3.py
--rw-r--r--   0        0        0    11210 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/gettext.py
--rw-r--r--   0        0        0    59513 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/html/__init__.py
--rw-r--r--   0        0        0     5383 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/html/_assets.py
--rw-r--r--   0        0        0     2563 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/html/transforms.py
--rw-r--r--   0        0        0    24296 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/latex/__init__.py
--rw-r--r--   0        0        0     7365 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/latex/constants.py
--rw-r--r--   0        0        0      866 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/latex/nodes.py
--rw-r--r--   0        0        0     4505 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/latex/theming.py
--rw-r--r--   0        0        0    21041 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/latex/transforms.py
--rw-r--r--   0        0        0     1703 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/latex/util.py
--rw-r--r--   0        0        0    24526 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/linkcheck.py
--rw-r--r--   0        0        0     4567 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/manpage.py
--rw-r--r--   0        0        0     7781 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/singlehtml.py
--rw-r--r--   0        0        0     9769 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/texinfo.py
--rw-r--r--   0        0        0     2945 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/text.py
--rw-r--r--   0        0        0     3848 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/builders/xml.py
--rw-r--r--   0        0        0       44 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/cmd/__init__.py
--rw-r--r--   0        0        0    13942 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/cmd/build.py
--rw-r--r--   0        0        0     6691 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/cmd/make_mode.py
--rw-r--r--   0        0        0    23959 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/cmd/quickstart.py
--rw-r--r--   0        0        0    23017 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/config.py
--rw-r--r--   0        0        0     1859 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/deprecation.py
--rw-r--r--   0        0        0    15095 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/directives/__init__.py
--rw-r--r--   0        0        0    18377 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/directives/code.py
--rw-r--r--   0        0        0    16599 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/directives/other.py
--rw-r--r--   0        0        0     6785 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/directives/patches.py
--rw-r--r--   0        0        0    15376 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/domains/__init__.py
--rw-r--r--   0        0        0   152243 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/domains/c.py
--rw-r--r--   0        0        0     5533 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/domains/changeset.py
--rw-r--r--   0        0        0     5681 2023-08-30 22:09:32.780403 sphinx-7.2.5/sphinx/domains/citation.py
--rw-r--r--   0        0        0   332914 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/domains/cpp.py
--rw-r--r--   0        0        0     4222 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/domains/index.py
--rw-r--r--   0        0        0    19405 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/domains/javascript.py
--rw-r--r--   0        0        0     5499 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/domains/math.py
--rw-r--r--   0        0        0    71297 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/domains/python.py
--rw-r--r--   0        0        0    10651 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/domains/rst.py
--rw-r--r--   0        0        0    46146 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/domains/std.py
--rw-r--r--   0        0        0    31397 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/__init__.py
--rw-r--r--   0        0        0       34 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/adapters/__init__.py
--rw-r--r--   0        0        0      418 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/adapters/asset.py
--rw-r--r--   0        0        0     7589 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/adapters/indexentries.py
--rw-r--r--   0        0        0    18767 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/adapters/toctree.py
--rw-r--r--   0        0        0     2791 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/collectors/__init__.py
--rw-r--r--   0        0        0     6355 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/collectors/asset.py
--rw-r--r--   0        0        0     1934 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/collectors/dependencies.py
--rw-r--r--   0        0        0     2659 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/collectors/metadata.py
--rw-r--r--   0        0        0     2186 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/collectors/title.py
--rw-r--r--   0        0        0    15956 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/environment/collectors/toctree.py
--rw-r--r--   0        0        0     3398 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/errors.py
--rw-r--r--   0        0        0     4296 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/events.py
--rw-r--r--   0        0        0       57 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/__init__.py
--rw-r--r--   0        0        0    20014 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/apidoc.py
--rw-r--r--   0        0        0   116526 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autodoc/__init__.py
--rw-r--r--   0        0        0     6007 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autodoc/directive.py
--rw-r--r--   0        0        0    12149 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autodoc/importer.py
--rw-r--r--   0        0        0     5972 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autodoc/mock.py
--rw-r--r--   0        0        0     7050 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autodoc/preserve_defaults.py
--rw-r--r--   0        0        0     5366 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autodoc/type_comment.py
--rw-r--r--   0        0        0     7859 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autodoc/typehints.py
--rw-r--r--   0        0        0     2335 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autosectionlabel.py
--rw-r--r--   0        0        0    31230 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autosummary/__init__.py
--rw-r--r--   0        0        0    27531 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autosummary/generate.py
--rw-r--r--   0        0        0      106 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autosummary/templates/autosummary/base.rst
--rw-r--r--   0        0        0      553 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autosummary/templates/autosummary/class.rst
--rw-r--r--   0        0        0     1071 2023-08-30 22:09:32.784404 sphinx-7.2.5/sphinx/ext/autosummary/templates/autosummary/module.rst
--rw-r--r--   0        0        0    17527 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/coverage.py
--rw-r--r--   0        0        0    23047 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/doctest.py
--rw-r--r--   0        0        0     2892 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/duration.py
--rw-r--r--   0        0        0     4629 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/extlinks.py
--rw-r--r--   0        0        0     1994 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/githubpages.py
--rw-r--r--   0        0        0    17614 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/graphviz.py
--rw-r--r--   0        0        0     2564 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/ifconfig.py
--rw-r--r--   0        0        0     3620 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/imgconverter.py
--rw-r--r--   0        0        0    15421 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/imgmath.py
--rw-r--r--   0        0        0    17604 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/inheritance_diagram.py
--rw-r--r--   0        0        0    29181 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/intersphinx.py
--rw-r--r--   0        0        0     2301 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/linkcode.py
--rw-r--r--   0        0        0     5323 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/mathjax.py
--rw-r--r--   0        0        0    17950 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/napoleon/__init__.py
--rw-r--r--   0        0        0    48761 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/napoleon/docstring.py
--rw-r--r--   0        0        0     8076 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/todo.py
--rw-r--r--   0        0        0    13765 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/ext/viewcode.py
--rw-r--r--   0        0        0     2999 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/extension.py
--rw-r--r--   0        0        0     7211 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/highlighting.py
--rw-r--r--   0        0        0     6165 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/io.py
--rw-r--r--   0        0        0     7133 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/jinja2glue.py
--rw-r--r--   0        0        0      165 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/locale/.tx/config
--rw-r--r--   0        0        0     7282 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/locale/__init__.py
--rw-r--r--   0        0        0     3494 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/locale/ar/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7494 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/locale/ar/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87441 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/locale/ar/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/locale/bg/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      492 2023-08-30 22:09:32.788404 sphinx-7.2.5/sphinx/locale/bg/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84221 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/bg/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     5977 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/bn/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7591 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/bn/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88102 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/bn/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4029 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/ca/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    84364 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/ca/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   123494 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/ca/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2385 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/cak/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2391 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/cak/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84935 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/cak/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3976 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/cs/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7797 2023-08-30 22:09:32.792404 sphinx-7.2.5/sphinx/locale/cs/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86868 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/cs/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3411 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/cy/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     5686 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/cy/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86117 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/cy/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3578 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/da/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    12266 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/da/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88524 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/da/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3533 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/de/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    10680 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/de/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88190 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/de/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2303 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/de_DE/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      505 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/de_DE/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84234 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/de_DE/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     8758 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/el/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    80411 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/el/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   131575 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/el/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2303 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/en_DE/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      506 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/en_DE/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84235 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/en_DE/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2302 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      462 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/en_FR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84234 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3630 2023-08-30 22:09:32.796404 sphinx-7.2.5/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    75590 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   115380 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2303 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      508 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/en_HK/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84237 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2457 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/eo/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     1864 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/eo/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84717 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/eo/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4155 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/es/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    80907 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/es/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   121834 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/es/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2342 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/es_CO/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      546 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/es_CO/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84275 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/es_CO/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3615 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/et/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    32776 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/et/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    97621 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/et/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3102 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/eu/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6505 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/eu/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86366 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/eu/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     7551 2023-08-30 22:09:32.800404 sphinx-7.2.5/sphinx/locale/fa/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    97001 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fa/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   139238 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fa/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2787 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2912 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85021 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4162 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    83168 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   124747 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2354 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      555 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84284 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/gl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     4716 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/gl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86205 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/gl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4885 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/he/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     4822 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/he/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86002 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/he/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     7427 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/hi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    96953 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/hi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   146384 2023-08-30 22:09:32.804405 sphinx-7.2.5/sphinx/locale/hi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2303 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      502 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84231 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3621 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    16384 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    90403 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3980 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hu/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    10971 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hu/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88513 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/hu/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3465 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/id/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    60268 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/id/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   109906 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/id/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2825 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/is/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2614 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/is/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84925 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/is/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3579 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/it/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    10036 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/it/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87985 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/it/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4957 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/ja/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    85691 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/ja/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   128423 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/ja/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6108 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/ka/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    74059 2023-08-30 22:09:32.808405 sphinx-7.2.5/sphinx/locale/ka/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   131614 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/ka/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4807 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/ko/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    82285 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/ko/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   122848 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/ko/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3473 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/lt/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6832 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/lt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86552 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/lt/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3445 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/lv/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6501 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/lv/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86258 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/lv/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2415 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/mk/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     2011 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/mk/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84911 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/mk/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3108 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6500 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86081 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6223 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/ne/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8520 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/ne/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88266 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/ne/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3489 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/nl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    18611 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/nl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    91729 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/nl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3819 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/pl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    28827 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/pl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    96313 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/pl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2351 2023-08-30 22:09:32.812405 sphinx-7.2.5/sphinx/locale/pt/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      544 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/pt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84273 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/pt/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4219 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    81014 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   121035 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3745 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     7764 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86914 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3700 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/ro/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     8259 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/ro/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87098 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/ro/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     8165 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/ru/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    15343 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/ru/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    91964 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/ru/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3816 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/si/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     3560 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/si/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85703 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/si/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4117 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/sk/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    66206 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/sk/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   112993 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/sk/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3185 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/sl/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     5157 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/sl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    85764 2023-08-30 22:09:32.816405 sphinx-7.2.5/sphinx/locale/sl/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0    84206 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sphinx.pot
--rw-r--r--   0        0        0     4216 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sq/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    79459 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sq/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   120806 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sq/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4100 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     9193 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    88349 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2380 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      584 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84313 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2382 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      579 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84308 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3281 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sv/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6491 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sv/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86103 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/sv/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/ta/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      647 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/ta/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84381 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/ta/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/te/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      489 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/te/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84218 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/te/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3937 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/tr/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    56773 2023-08-30 22:09:32.820405 sphinx-7.2.5/sphinx/locale/tr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   109376 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/tr/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     6283 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     6349 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    87075 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2300 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/ur/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      487 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/ur/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84216 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/ur/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3520 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/vi/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0     5771 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/vi/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    86217 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/vi/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2294 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/yue/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      487 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/yue/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84216 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/yue/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4318 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    75427 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   115775 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2301 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      501 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84230 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     2301 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0      516 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0    84245 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     4451 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js
--rw-r--r--   0        0        0    74037 2023-08-30 22:09:32.824406 sphinx-7.2.5/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo
--rw-r--r--   0        0        0   114591 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0     3121 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/parsers.py
--rw-r--r--   0        0        0     4265 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/project.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/py.typed
--rw-r--r--   0        0        0     5603 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/pycode/__init__.py
--rw-r--r--   0        0        0     6352 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/pycode/ast.py
--rw-r--r--   0        0        0    21521 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/pycode/parser.py
--rw-r--r--   0        0        0     2861 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/pygments_styles.py
--rw-r--r--   0        0        0    22436 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/registry.py
--rw-r--r--   0        0        0    16098 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/roles.py
--rw-r--r--   0        0        0    22113 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/__init__.py
--rw-r--r--   0        0        0     3576 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/da.py
--rw-r--r--   0        0        0     4652 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/de.py
--rw-r--r--   0        0        0     4914 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/en.py
--rw-r--r--   0        0        0     5738 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/es.py
--rw-r--r--   0        0        0     3222 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/fi.py
--rw-r--r--   0        0        0     3453 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/fr.py
--rw-r--r--   0        0        0     1964 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/hu.py
--rw-r--r--   0        0        0     5104 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/it.py
--rw-r--r--   0        0        0    31012 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/ja.py
--rw-r--r--   0        0        0     3594 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/base-stemmer.js
--rw-r--r--   0        0        0     3123 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/danish-stemmer.js
--rw-r--r--   0        0        0     5529 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/dutch-stemmer.js
--rw-r--r--   0        0        0     7529 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/finnish-stemmer.js
--rw-r--r--   0        0        0    11571 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/french-stemmer.js
--rw-r--r--   0        0        0     4669 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/german-stemmer.js
--rw-r--r--   0        0        0     6614 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/hungarian-stemmer.js
--rw-r--r--   0        0        0     9100 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/italian-stemmer.js
--rw-r--r--   0        0        0     2594 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/norwegian-stemmer.js
--rw-r--r--   0        0        0     6439 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/porter-stemmer.js
--rw-r--r--   0        0        0     8373 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/portuguese-stemmer.js
--rw-r--r--   0        0        0     8333 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/romanian-stemmer.js
--rw-r--r--   0        0        0     5735 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/russian-stemmer.js
--rw-r--r--   0        0        0     9121 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/spanish-stemmer.js
--rw-r--r--   0        0        0     2654 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/swedish-stemmer.js
--rw-r--r--   0        0        0    19972 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/minified-js/turkish-stemmer.js
--rw-r--r--   0        0        0     4586 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/nl.py
--rw-r--r--   0        0        0     4908 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/no.py
--rw-r--r--   0        0        0     8133 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/non-minified-js/base-stemmer.js
--rw-r--r--   0        0        0     8134 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/non-minified-js/danish-stemmer.js
--rw-r--r--   0        0        0    19495 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/non-minified-js/dutch-stemmer.js
--rw-r--r--   0        0        0    21286 2023-08-30 22:09:32.828406 sphinx-7.2.5/sphinx/search/non-minified-js/finnish-stemmer.js
--rw-r--r--   0        0        0    42080 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/french-stemmer.js
--rw-r--r--   0        0        0    17647 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/german-stemmer.js
--rw-r--r--   0        0        0    17564 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/hungarian-stemmer.js
--rw-r--r--   0        0        0    29065 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/italian-stemmer.js
--rw-r--r--   0        0        0     6870 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/norwegian-stemmer.js
--rw-r--r--   0        0        0    20391 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/porter-stemmer.js
--rw-r--r--   0        0        0    26718 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/portuguese-stemmer.js
--rw-r--r--   0        0        0    25006 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/romanian-stemmer.js
--rw-r--r--   0        0        0    17996 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/russian-stemmer.js
--rw-r--r--   0        0        0    28534 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/spanish-stemmer.js
--rw-r--r--   0        0        0     6851 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/swedish-stemmer.js
--rw-r--r--   0        0        0    77511 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/non-minified-js/turkish-stemmer.js
--rw-r--r--   0        0        0     4663 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/pt.py
--rw-r--r--   0        0        0      572 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/ro.py
--rw-r--r--   0        0        0     7920 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/ru.py
--rw-r--r--   0        0        0     3451 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/sv.py
--rw-r--r--   0        0        0      566 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/tr.py
--rw-r--r--   0        0        0     6161 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/search/zh.py
--rw-r--r--   0        0        0      196 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/apidoc/module.rst_t
--rw-r--r--   0        0        0     1173 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/apidoc/package.rst_t
--rw-r--r--   0        0        0      128 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/apidoc/toc.rst_t
--rw-r--r--   0        0        0      246 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/epub3/container.xml
--rw-r--r--   0        0        0     2127 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/epub3/content.opf_t
--rw-r--r--   0        0        0       20 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/epub3/mimetype
--rw-r--r--   0        0        0      629 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/epub3/nav.xhtml_t
--rw-r--r--   0        0        0      743 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/epub3/toc.ncx_t
--rw-r--r--   0        0        0      875 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/gettext/message.pot_t
--rw-r--r--   0        0        0      299 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/graphviz/graphviz.css
--rw-r--r--   0        0        0      864 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/htmlhelp/project.hhc
--rw-r--r--   0        0        0      570 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/htmlhelp/project.hhp
--rw-r--r--   0        0        0      165 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/htmlhelp/project.stp
--rw-r--r--   0        0        0      397 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/imgmath/preview.tex_t
--rw-r--r--   0        0        0      321 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/imgmath/template.tex_t
--rw-r--r--   0        0        0     2986 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/latex/latex.tex_t
--rw-r--r--   0        0        0     2156 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/latex/longtable.tex_t
--rw-r--r--   0        0        0      944 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/latex/sphinxmessages.sty_t
--rw-r--r--   0        0        0     1406 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/latex/tabular.tex_t
--rw-r--r--   0        0        0     1420 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/latex/tabulary.tex_t
--rw-r--r--   0        0        0      656 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/quickstart/Makefile.new_t
--rw-r--r--   0        0        0     4031 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/quickstart/Makefile_t
--rw-r--r--   0        0        0     2129 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/quickstart/conf.py_t
--rw-r--r--   0        0        0      787 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/quickstart/make.bat.new_t
--rw-r--r--   0        0        0     3293 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/quickstart/make.bat_t
--rw-r--r--   0        0        0      492 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/quickstart/root_doc.rst_t
--rw-r--r--   0        0        0     1423 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/templates/texinfo/Makefile
--rw-r--r--   0        0        0      171 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/testing/__init__.py
--rw-r--r--   0        0        0     7142 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/testing/fixtures.py
--rw-r--r--   0        0        0     6572 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/testing/path.py
--rw-r--r--   0        0        0     1159 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/testing/restructuredtext.py
--rw-r--r--   0        0        0     6375 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/testing/util.py
--rw-r--r--   0        0        0     4366 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/LICRcyr2utf8.xdy
--rw-r--r--   0        0        0    10188 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/LICRlatin2utf8.xdy
--rw-r--r--   0        0        0    18890 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/LatinRules.xdy
--rw-r--r--   0        0        0     2401 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/Makefile_t
--rw-r--r--   0        0        0      695 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/latexmkjarc_t
--rw-r--r--   0        0        0     1104 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/latexmkrc_t
--rw-r--r--   0        0        0     1041 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/make.bat_t
--rw-r--r--   0        0        0      392 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/python.ist
--rw-r--r--   0        0        0    44560 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/sphinx.sty
--rw-r--r--   0        0        0     9474 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/sphinx.xdy
--rw-r--r--   0        0        0     3256 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/sphinxhowto.cls
--rw-r--r--   0        0        0    10989 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexadmonitions.sty
--rw-r--r--   0        0        0      901 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexcontainers.sty
--rw-r--r--   0        0        0     4840 2023-08-30 22:09:32.832406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexgraphics.sty
--rw-r--r--   0        0        0     2066 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexindbibtoc.sty
--rw-r--r--   0        0        0     5139 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexlists.sty
--rw-r--r--   0        0        0    46048 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexliterals.sty
--rw-r--r--   0        0        0     4532 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexnumfig.sty
--rw-r--r--   0        0        0    14354 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexobjects.sty
--rw-r--r--   0        0        0     5066 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexshadowbox.sty
--rw-r--r--   0        0        0     3445 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexstyleheadings.sty
--rw-r--r--   0        0        0     3064 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexstylepage.sty
--rw-r--r--   0        0        0     8589 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatexstyletext.sty
--rw-r--r--   0        0        0    57830 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxlatextables.sty
--rw-r--r--   0        0        0     4241 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxmanual.cls
--rw-r--r--   0        0        0     2061 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxoptionsgeometry.sty
--rw-r--r--   0        0        0     1094 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxoptionshyperref.sty
--rw-r--r--   0        0        0    36615 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxpackageboxes.sty
--rw-r--r--   0        0        0     2590 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxpackagecyrillic.sty
--rw-r--r--   0        0        0    15254 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs/sphinxpackagefootnote.sty
--rw-r--r--   0        0        0     2503 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/texinputs_win/Makefile_t
--rw-r--r--   0        0        0     3321 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/agogo/layout.html
--rw-r--r--   0        0        0     9236 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/agogo/static/agogo.css_t
--rw-r--r--   0        0        0      276 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/agogo/static/bgfooter.png
--rw-r--r--   0        0        0      266 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/agogo/static/bgtop.png
--rw-r--r--   0        0        0      477 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/agogo/theme.conf
--rw-r--r--   0        0        0      466 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/changes/frameset.html
--rw-r--r--   0        0        0      485 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/changes/rstsource.html
--rw-r--r--   0        0        0     1306 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/changes/versionchanges.html
--rw-r--r--   0        0        0     1636 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/defindex.html
--rw-r--r--   0        0        0     1892 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/domainindex.html
--rw-r--r--   0        0        0     1804 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/genindex-single.html
--rw-r--r--   0        0        0     1210 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/genindex-split.html
--rw-r--r--   0        0        0     2069 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/genindex.html
--rw-r--r--   0        0        0      432 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/globaltoc.html
--rw-r--r--   0        0        0     7673 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/layout.html
--rw-r--r--   0        0        0      370 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/localtoc.html
--rw-r--r--   0        0        0      679 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/opensearch.xml
--rw-r--r--   0        0        0      273 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/page.html
--rw-r--r--   0        0        0      652 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/relations.html
--rw-r--r--   0        0        0     2039 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/search.html
--rw-r--r--   0        0        0      809 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/searchbox.html
--rw-r--r--   0        0        0      947 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/searchfield.html
--rw-r--r--   0        0        0      544 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/sourcelink.html
--rw-r--r--   0        0        0    15174 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/basic.css_t
--rw-r--r--   0        0        0     4472 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/doctools.js
--rw-r--r--   0        0        0      581 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/documentation_options.js_t
--rw-r--r--   0        0        0      286 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/file.png
--rw-r--r--   0        0        0      676 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/language_data.js_t
--rw-r--r--   0        0        0       90 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/minus.png
--rw-r--r--   0        0        0       90 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/plus.png
--rw-r--r--   0        0        0    18732 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/searchtools.js
--rw-r--r--   0        0        0     5123 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/static/sphinx_highlight.js
--rw-r--r--   0        0        0      371 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/basic/theme.conf
--rw-r--r--   0        0        0      664 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/bizstyle/layout.html
--rw-r--r--   0        0        0       78 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/bizstyle/static/background_b01.png
--rw-r--r--   0        0        0    10349 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/bizstyle/static/bizstyle.css_t
--rw-r--r--   0        0        0     1129 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/bizstyle/static/bizstyle.js_t
--rw-r--r--   0        0        0    14940 2023-08-30 22:09:32.836406 sphinx-7.2.5/sphinx/themes/bizstyle/static/css3-mediaqueries.js
--rw-r--r--   0        0        0    28634 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js
--rw-r--r--   0        0        0      148 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/bizstyle/theme.conf
--rw-r--r--   0        0        0      661 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/classic/layout.html
--rw-r--r--   0        0        0     6635 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/classic/static/classic.css_t
--rw-r--r--   0        0        0     2659 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/classic/static/sidebar.js_t
--rw-r--r--   0        0        0      719 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/classic/theme.conf
--rw-r--r--   0        0        0       28 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/default/static/default.css
--rw-r--r--   0        0        0       26 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/default/theme.conf
--rw-r--r--   0        0        0      693 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/epub/epub-cover.html
--rw-r--r--   0        0        0      543 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/epub/layout.html
--rw-r--r--   0        0        0    12435 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/epub/static/epub.css_t
--rw-r--r--   0        0        0      108 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/epub/theme.conf
--rw-r--r--   0        0        0     2012 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/haiku/layout.html
--rw-r--r--   0        0        0     1128 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/haiku/static/alert_info_32.png
--rw-r--r--   0        0        0      944 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/haiku/static/alert_warning_32.png
--rw-r--r--   0        0        0       82 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/haiku/static/bg-page.png
--rw-r--r--   0        0        0      165 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/haiku/static/bullet_orange.png
--rw-r--r--   0        0        0     7059 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/haiku/static/haiku.css_t
--rw-r--r--   0        0        0      298 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/haiku/theme.conf
--rw-r--r--   0        0        0     4269 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/nature/static/nature.css_t
--rw-r--r--   0        0        0       71 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/nature/theme.conf
--rw-r--r--   0        0        0      642 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/nonav/layout.html
--rw-r--r--   0        0        0     9692 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/nonav/static/nonav.css_t
--rw-r--r--   0        0        0      109 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/nonav/theme.conf
--rw-r--r--   0        0        0      875 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/layout.html
--rw-r--r--   0        0        0     1394 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-note.png
--rw-r--r--   0        0        0     1351 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-seealso.png
--rw-r--r--   0        0        0     1186 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-todo.png
--rw-r--r--   0        0        0     1798 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-topic.png
--rw-r--r--   0        0        0     1280 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-warning.png
--rw-r--r--   0        0        0     5629 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/epub.css_t
--rw-r--r--   0        0        0      333 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/footerbg.png
--rw-r--r--   0        0        0      190 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/headerbg.png
--rw-r--r--   0        0        0      726 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/ie6.css
--rw-r--r--   0        0        0      101 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/middlebg.png
--rw-r--r--   0        0        0     6336 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/pyramid.css_t
--rw-r--r--   0        0        0       49 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/static/transparent.gif
--rw-r--r--   0        0        0      102 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/pyramid/theme.conf
--rw-r--r--   0        0        0     5775 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/artwork/logo.svg
--rw-r--r--   0        0        0     1661 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/layout.html
--rw-r--r--   0        0        0    25238 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/darkmetal.png
--rw-r--r--   0        0        0      172 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/headerbg.png
--rw-r--r--   0        0        0     8305 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/logo.png
--rw-r--r--   0        0        0     7547 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/metal.png
--rw-r--r--   0        0        0      124 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/navigation.png
--rw-r--r--   0        0        0      303 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/print.css
--rw-r--r--   0        0        0     8033 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/scrolls.css_t
--rw-r--r--   0        0        0      527 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/theme_extras.js
--rw-r--r--   0        0        0    44483 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/watermark.png
--rw-r--r--   0        0        0     8049 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/static/watermark_blur.png
--rw-r--r--   0        0        0      263 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/scrolls/theme.conf
--rw-r--r--   0        0        0      107 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/sphinxdoc/static/contents.png
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/sphinxdoc/static/navigation.png
--rw-r--r--   0        0        0     6349 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t
--rw-r--r--   0        0        0       77 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/sphinxdoc/theme.conf
--rw-r--r--   0        0        0    12162 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/traditional/static/traditional.css_t
--rw-r--r--   0        0        0      105 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/themes/traditional/theme.conf
--rw-r--r--   0        0        0     7994 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/theming.py
--rw-r--r--   0        0        0    17741 2023-08-30 22:09:32.840407 sphinx-7.2.5/sphinx/transforms/__init__.py
--rw-r--r--   0        0        0     2811 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/transforms/compact_bullet_list.py
--rw-r--r--   0        0        0    26261 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/transforms/i18n.py
--rw-r--r--   0        0        0    12616 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/transforms/post_transforms/__init__.py
--rw-r--r--   0        0        0     4529 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/transforms/post_transforms/code.py
--rw-r--r--   0        0        0    10408 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/transforms/post_transforms/images.py
--rw-r--r--   0        0        0     1361 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/transforms/references.py
--rw-r--r--   0        0        0    10212 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/__init__.py
--rw-r--r--   0        0        0     4255 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/_pathlib.py
--rw-r--r--   0        0        0      240 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/build_phase.py
--rw-r--r--   0        0        0    15450 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/cfamily.py
--rw-r--r--   0        0        0     3223 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/console.py
--rw-r--r--   0        0        0     2710 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/display.py
--rw-r--r--   0        0        0    16843 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/docfields.py
--rw-r--r--   0        0        0     2944 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/docstrings.py
--rw-r--r--   0        0        0    23193 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/docutils.py
--rw-r--r--   0        0        0     1960 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/exceptions.py
--rw-r--r--   0        0        0     3910 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/fileutil.py
--rw-r--r--   0        0        0     1235 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/http_date.py
--rw-r--r--   0        0        0     9580 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/i18n.py
--rw-r--r--   0        0        0     3674 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/images.py
--rw-r--r--   0        0        0      986 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/index_entries.py
--rw-r--r--   0        0        0    29088 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/inspect.py
--rw-r--r--   0        0        0     6347 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/inventory.py
--rw-r--r--   0        0        0    18125 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/logging.py
--rw-r--r--   0        0        0     5363 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/matching.py
--rw-r--r--   0        0        0     1902 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/math.py
--rw-r--r--   0        0        0    24408 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/nodes.py
--rw-r--r--   0        0        0     6532 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/osutil.py
--rw-r--r--   0        0        0     5088 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/parallel.py
--rw-r--r--   0        0        0     1445 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/png.py
--rw-r--r--   0        0        0     2428 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/requests.py
--rw-r--r--   0        0        0     3398 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/rst.py
--rw-r--r--   0        0        0     2770 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/tags.py
--rw-r--r--   0        0        0     4954 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/template.py
--rw-r--r--   0        0        0     5442 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/texescape.py
--rw-r--r--   0        0        0    16646 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/util/typing.py
--rw-r--r--   0        0        0     5849 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/versioning.py
--rw-r--r--   0        0        0       31 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/writers/__init__.py
--rw-r--r--   0        0        0     1603 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/writers/html.py
--rw-r--r--   0        0        0    37346 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/writers/html5.py
--rw-r--r--   0        0        0    90889 2023-08-30 22:09:32.844407 sphinx-7.2.5/sphinx/writers/latex.py
--rw-r--r--   0        0        0    16007 2023-08-30 22:09:32.848407 sphinx-7.2.5/sphinx/writers/manpage.py
--rw-r--r--   0        0        0    53237 2023-08-30 22:09:32.848407 sphinx-7.2.5/sphinx/writers/texinfo.py
--rw-r--r--   0        0        0    43368 2023-08-30 22:09:32.848407 sphinx-7.2.5/sphinx/writers/text.py
--rw-r--r--   0        0        0     1509 2023-08-30 22:09:32.848407 sphinx-7.2.5/sphinx/writers/xml.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/__init__.py
--rw-r--r--   0        0        0     3054 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/certs/cert.pem
--rw-r--r--   0        0        0      975 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/conftest.py
--rw-r--r--   0        0        0      363 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/ext_napoleon_pep526_data_google.py
--rw-r--r--   0        0        0      385 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/ext_napoleon_pep526_data_numpy.py
--rw-r--r--   0        0        0       34 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/js/documentation_options.js
--rw-r--r--   0        0        0     1694 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/js/searchtools.js
--rw-r--r--   0        0        0     1985 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/js/sphinx_highlight.js
--rw-r--r--   0        0        0      111 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-add_enumerable_node/conf.py
--rw-r--r--   0        0        0     1464 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-add_enumerable_node/enumerable_node.py
--rw-r--r--   0        0        0      763 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-add_enumerable_node/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-add_enumerable_node/rimg.png
--rw-r--r--   0        0        0      277 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-add_source_parser-conflicts-with-users-setting/conf.py
--rw-r--r--   0        0        0      201 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-add_source_parser-conflicts-with-users-setting/source_parser.py
--rw-r--r--   0        0        0      121 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-add_source_parser/conf.py
--rw-r--r--   0        0        0      201 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-add_source_parser/source_parser.py
--rw-r--r--   0        0        0     1659 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-api-set-translator/conf.py
--rw-r--r--   0        0        0       72 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-api-set-translator/index.rst
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-api-set-translator/nonext/conf.py
--rw-r--r--   0        0        0      101 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-api-set-translator/translator.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-duplicates/fish_licence/halibut.cpython-38-x86_64-linux-gnu.so
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-duplicates/fish_licence/halibut.pyx
--rw-r--r--   0        0        0       12 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-pep420/a/b/c/__init__.py
--rw-r--r--   0        0        0       11 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-pep420/a/b/c/d.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-pep420/a/b/e/__init__.py
--rw-r--r--   0        0        0       11 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-pep420/a/b/e/f.py
--rw-r--r--   0        0        0       11 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-pep420/a/b/x/y.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-subpackage-in-toc/parent/__init__.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-subpackage-in-toc/parent/child/__init__.py
--rw-r--r--   0        0        0        6 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-subpackage-in-toc/parent/child/foo.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-toc/mypackage/__init__.py
--rwxr-xr-x   0        0        0      404 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-toc/mypackage/main.py
--rw-r--r--   0        0        0       79 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-toc/mypackage/no_init/foo.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-toc/mypackage/resource/__init__.py
--rw-r--r--   0        0        0       96 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-toc/mypackage/resource/resource.txt
--rw-r--r--   0        0        0       23 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-toc/mypackage/something/__init__.py
--rw-r--r--   0        0        0       44 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-trailing-underscore/package_/__init__.py
--rw-r--r--   0        0        0      215 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-apidoc-trailing-underscore/package_/module_.py
--rw-r--r--   0        0        0      221 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-autosummary/conf.py
--rw-r--r--   0        0        0     1335 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-autosummary/dummy_module.py
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-autosummary/index.rst
--rw-r--r--   0        0        0      507 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-autosummary/sphinx.rst
--rw-r--r--   0        0        0      198 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-autosummary/underscore_module_.py
--rw-r--r--   0        0        0      114 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-basic/conf.py
--rw-r--r--   0        0        0     1477 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-basic/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/extra.css
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/mytheme.css
--rw-r--r--   0        0        0       60 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/theme.conf
--rw-r--r--   0        0        0       53 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-html-theme-having-multiple-stylesheets/conf.py
--rw-r--r--   0        0        0      100 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-html-theme-having-multiple-stylesheets/index.rst
--rw-r--r--   0        0        0      372 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-html-translator/conf.py
--rw-r--r--   0        0        0      252 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-html-translator/index.rst
--rw-r--r--   0        0        0       53 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/conf.py
--rw-r--r--   0        0        0       20 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/doc1.txt
--rw-r--r--   0        0        0       51 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/doc2.txt
--rw-r--r--   0        0        0      135 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/index.txt
--rw-r--r--   0        0        0       62 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/lineblock.txt
--rw-r--r--   0        0        0       40 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/listitems.txt
--rw-r--r--   0        0        0      388 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/maxwidth.txt
--rw-r--r--   0        0        0      478 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/nonascii_maxwidth.txt
--rw-r--r--   0        0        0       75 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/nonascii_table.txt
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/nonascii_title.txt
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/table.txt
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/table_colspan.txt
--rw-r--r--   0        0        0      140 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/table_colspan_and_rowspan.txt
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/table_colspan_left.txt
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-build-text/table_rowspan.txt
--rw-r--r--   0        0        0       18 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-dirhtml/bar.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-dirhtml/conf.py
--rw-r--r--   0        0        0       32 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-dirhtml/foo/foo_1.rst
--rw-r--r--   0        0        0       32 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-dirhtml/foo/foo_2.rst
--rw-r--r--   0        0        0       63 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-dirhtml/foo/index.rst
--rw-r--r--   0        0        0       59 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-dirhtml/index.rst
--rw-r--r--   0        0        0       74 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-gettext-dont-rebuild-mo/bom.rst
--rw-r--r--   0        0        0       16 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-gettext-dont-rebuild-mo/conf.py
--rw-r--r--   0        0        0      108 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-gettext-dont-rebuild-mo/index.rst
--rw-r--r--   0        0        0      264 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-builder-gettext-dont-rebuild-mo/xx/LC_MESSAGES/bom.po
--rw-r--r--   0        0        0      330 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-changes/base.rst
--rw-r--r--   0        0        0      371 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-changes/c-api.rst
--rw-r--r--   0        0        0      134 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-changes/conf.py
--rw-r--r--   0        0        0      189 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-changes/contents.rst
--rw-r--r--   0        0        0      443 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-changes/library/utils.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-circular/conf.py
--rw-r--r--   0        0        0       22 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-circular/index.rst
--rw-r--r--   0        0        0       23 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-circular/sub.rst
--rw-r--r--   0        0        0       81 2023-08-30 22:09:32.848407 sphinx-7.2.5/tests/roots/test-config/conf.py
--rw-r--r--   0        0        0      167 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-copyright-multiline/conf.py
--rw-r--r--   0        0        0       75 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-copyright-multiline/index.rst
--rw-r--r--   0        0        0       32 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-correct-year/conf.py
--rw-r--r--   0        0        0       55 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-correct-year/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-default_role/conf.py
--rw-r--r--   0        0        0       29 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-default_role/foo.rst
--rw-r--r--   0        0        0       54 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-default_role/index.rst
--rw-r--r--   0        0        0      762 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/caption.rst
--rw-r--r--   0        0        0      263 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/classes.rst
--rw-r--r--   0        0        0       44 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/conf.py
--rw-r--r--   0        0        0     1434 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/dedent.rst
--rw-r--r--   0        0        0      170 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/emphasize.rst
--rw-r--r--   0        0        0        3 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/empty.inc
--rw-r--r--   0        0        0       21 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/error.inc
--rw-r--r--   0        0        0      203 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/force.rst
--rw-r--r--   0        0        0      345 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/highlight.rst
--rw-r--r--   0        0        0      267 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/index.rst
--rw-r--r--   0        0        0      349 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/linenos.rst
--rw-r--r--   0        0        0      396 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/linenothreshold.rst
--rw-r--r--   0        0        0      206 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/literal-diff.inc
--rw-r--r--   0        0        0       67 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/literal-short.inc
--rw-r--r--   0        0        0      213 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/literal.inc
--rw-r--r--   0        0        0      421 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/namedblocks.rst
--rw-r--r--   0        0        0      263 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/py-decorators.inc
--rw-r--r--   0        0        0      391 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/py-decorators.rst
--rw-r--r--   0        0        0      305 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/python.rst
--rw-r--r--   0        0        0      355 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-code/target.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-csv-table/conf.py
--rw-r--r--   0        0        0       12 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-csv-table/example.csv
--rw-r--r--   0        0        0       12 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-csv-table/subdir/example.csv
--rw-r--r--   0        0        0       27 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-include/bar.txt
--rw-r--r--   0        0        0       45 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-include/baz/baz.rst
--rw-r--r--   0        0        0       65 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-include/conf.py
--rw-r--r--   0        0        0       18 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-include/foo.rst
--rw-r--r--   0        0        0       20 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-include/text.txt
--rw-r--r--   0        0        0       62 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-only/conf.py
--rw-r--r--   0        0        0       63 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-only/index.rst
--rw-r--r--   0        0        0     3063 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directive-only/only.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directives-raw/conf.py
--rw-r--r--   0        0        0      404 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-directives-raw/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-docutilsconf/conf.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-docutilsconf/docutils.conf
--rw-r--r--   0        0        0       89 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-docutilsconf/index.rst
--rw-r--r--   0        0        0       65 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c-c_maximum_signature_line_length/conf.py
--rw-r--r--   0        0        0      119 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c-c_maximum_signature_line_length/index.rst
--rw-r--r--   0        0        0       74 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c-intersphinx/conf.py
--rw-r--r--   0        0        0     1146 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c-intersphinx/index.rst
--rw-r--r--   0        0        0      121 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c/anon-dup-decl.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c/conf.py
--rw-r--r--   0        0        0       70 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c/field-role.rst
--rw-r--r--   0        0        0      101 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c/function_param_target.rst
--rw-r--r--   0        0        0      785 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c/index.rst
--rw-r--r--   0        0        0      261 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c/namespace.rst
--rw-r--r--   0        0        0      163 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-c/ns_lookup.rst
--rw-r--r--   0        0        0       67 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp-cpp_maximum_signature_line_length/conf.py
--rw-r--r--   0        0        0      129 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp-cpp_maximum_signature_line_length/index.rst
--rw-r--r--   0        0        0       74 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp-intersphinx/conf.py
--rw-r--r--   0        0        0     2444 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp-intersphinx/index.rst
--rw-r--r--   0        0        0       92 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/anon-dup-decl.rst
--rw-r--r--   0        0        0      688 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/any-role.rst
--rw-r--r--   0        0        0       27 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/backslash.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/conf.py
--rw-r--r--   0        0        0       59 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/field-role.rst
--rw-r--r--   0        0        0     1136 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/index.rst
--rw-r--r--   0        0        0      133 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/lookup-key-overload.rst
--rw-r--r--   0        0        0      437 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/multi-decl-lookup.rst
--rw-r--r--   0        0        0     2136 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/roles-targets-ok.rst
--rw-r--r--   0        0        0     2406 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/roles-targets-warn.rst
--rw-r--r--   0        0        0      697 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/roles.rst
--rw-r--r--   0        0        0       90 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/roles2.rst
--rw-r--r--   0        0        0      383 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/semicolon.rst
--rw-r--r--   0        0        0      203 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/warn-template-param-qualified-name.rst
--rw-r--r--   0        0        0      249 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-cpp/xref_consistency.rst
--rw-r--r--   0        0        0       45 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-js-javascript_maximum_signature_line_length/conf.py
--rw-r--r--   0        0        0      156 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-js-javascript_maximum_signature_line_length/index.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-js/conf.py
--rw-r--r--   0        0        0       66 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-js/index.rst
--rw-r--r--   0        0        0      527 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-js/module.rst
--rw-r--r--   0        0        0      886 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-js/roles.rst
--rw-r--r--   0        0        0       41 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py-python_maximum_signature_line_length/conf.py
--rw-r--r--   0        0        0      168 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py-python_maximum_signature_line_length/index.rst
--rw-r--r--   0        0        0       41 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py-python_use_unqualified_type_names/conf.py
--rw-r--r--   0        0        0      240 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py-python_use_unqualified_type_names/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py-xref-warning/conf.py
--rw-r--r--   0        0        0      116 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py-xref-warning/index.rst
--rw-r--r--   0        0        0      359 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py/abbr.rst
--rw-r--r--   0        0        0      174 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py/canonical.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py/conf.py
--rw-r--r--   0        0        0      107 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py/index.rst
--rw-r--r--   0        0        0     1040 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py/module.rst
--rw-r--r--   0        0        0      383 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py/module_option.rst
--rw-r--r--   0        0        0      872 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-domain-py/roles.rst
--rw-r--r--   0        0        0       24 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme1/theme.conf
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme2/theme.conf
--rw-r--r--   0        0        0      127 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-double-inheriting-theme/conf.py
--rw-r--r--   0        0        0       87 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-double-inheriting-theme/index.rst
--rw-r--r--   0        0        0       40 2023-08-30 22:09:32.852407 sphinx-7.2.5/tests/roots/test-environment-record-dependencies/api.rst
--rw-r--r--   0        0        0       99 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-environment-record-dependencies/conf.py
--rw-r--r--   0        0        0       38 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-environment-record-dependencies/example_module.py
--rw-r--r--   0        0        0       22 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-environment-record-dependencies/index.rst
--rw-r--r--   0        0        0       87 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-epub-anchor-id/conf.py
--rw-r--r--   0        0        0      191 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-epub-anchor-id/index.rst
--rw-r--r--   0        0        0      111 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/autodoc_dummy_bar.py
--rw-r--r--   0        0        0       94 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/autodoc_dummy_module.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/bug2437/__init__.py
--rw-r--r--   0        0        0       47 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/bug2437/autodoc_dummy_foo.py
--rw-r--r--   0        0        0       40 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/circular_import/__init__.py
--rw-r--r--   0        0        0        7 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/circular_import/a.py
--rw-r--r--   0        0        0       82 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/circular_import/b.py
--rw-r--r--   0        0        0       97 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/circular_import/c.py
--rw-r--r--   0        0        0      215 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/conf.py
--rw-r--r--   0        0        0      282 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/index.rst
--rw-r--r--   0        0        0      301 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/TYPE_CHECKING.py
--rw-r--r--   0        0        0     4363 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/__init__.py
--rw-r--r--   0        0        0      187 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/_functions_to_import.py
--rw-r--r--   0        0        0      428 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/abstractmethods.py
--rw-r--r--   0        0        0      150 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/annotated.py
--rw-r--r--   0        0        0      882 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/autoclass_content.py
--rw-r--r--   0        0        0      665 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py
--rw-r--r--   0        0        0      107 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/bound_method.py
--rw-r--r--   0        0        0      219 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/cached_property.py
--rw-r--r--   0        0        0      279 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/callable.py
--rw-r--r--   0        0        0       47 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/canonical/__init__.py
--rw-r--r--   0        0        0      158 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/canonical/original.py
--rw-r--r--   0        0        0      684 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/classes.py
--rw-r--r--   0        0        0      764 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/coroutine.py
--rw-r--r--   0        0        0      245 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/cython.pyx
--rw-r--r--   0        0        0      766 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/decorator.py
--rw-r--r--   0        0        0      683 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/descriptor.py
--rw-r--r--   0        0        0      643 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/docstring_signature.py
--rw-r--r--   0        0        0      150 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/empty_all.py
--rw-r--r--   0        0        0      384 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/enums.py
--rw-r--r--   0        0        0      227 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/final.py
--rw-r--r--   0        0        0      268 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/functions.py
--rw-r--r--   0        0        0      278 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/generic_class.py
--rw-r--r--   0        0        0      262 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/genericalias.py
--rw-r--r--   0        0        0      260 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/hide_value.py
--rw-r--r--   0        0        0       42 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/imported_members.py
--rw-r--r--   0        0        0      458 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/inheritance.py
--rw-r--r--   0        0        0      279 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/instance_variable.py
--rw-r--r--   0        0        0      344 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/literal.py
--rw-r--r--   0        0        0       52 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/metadata.py
--rw-r--r--   0        0        0      422 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/methods.py
--rw-r--r--   0        0        0      155 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/module.py
--rw-r--r--   0        0        0       93 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/name_conflict/__init__.py
--rw-r--r--   0        0        0       65 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/name_conflict/foo.py
--rw-r--r--   0        0        0      169 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/name_mangling.py
--rw-r--r--   0        0        0      894 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/need_mocks.py
--rw-r--r--   0        0        0     1345 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/overload.py
--rw-r--r--   0        0        0       59 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/overload2.py
--rw-r--r--   0        0        0      207 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/partialfunction.py
--rw-r--r--   0        0        0      420 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/partialmethod.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/pep570.py
--rw-r--r--   0        0        0      292 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/pep604.py
--rw-r--r--   0        0        0     1505 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/preserve_defaults.py
--rw-r--r--   0        0        0      910 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/preserve_defaults_special_constructs.py
--rw-r--r--   0        0        0      556 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/private.py
--rw-r--r--   0        0        0       90 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/process_docstring.py
--rw-r--r--   0        0        0      407 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/properties.py
--rw-r--r--   0        0        0      705 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/singledispatch.py
--rw-r--r--   0        0        0      628 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/singledispatchmethod.py
--rw-r--r--   0        0        0      396 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/slots.py
--rw-r--r--   0        0        0      168 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/sort_by_all.py
--rw-r--r--   0        0        0      551 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/typed_vars.py
--rw-r--r--   0        0        0     2107 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/typehints.py
--rw-r--r--   0        0        0      461 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/typevar.py
--rw-r--r--   0        0        0      123 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/uninitialized_attributes.py
--rw-r--r--   0        0        0      372 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autodoc/target/wrappedfunction.py
--rw-r--r--   0        0        0       85 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosectionlabel-prefix-document/conf.py
--rw-r--r--   0        0        0      591 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst
--rw-r--r--   0        0        0       45 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosectionlabel/conf.py
--rw-r--r--   0        0        0      535 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosectionlabel/index.rst
--rw-r--r--   0        0        0      294 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-filename-map/autosummary_dummy_module.py
--rw-r--r--   0        0        0      255 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-filename-map/conf.py
--rw-r--r--   0        0        0      198 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-filename-map/index.rst
--rw-r--r--   0        0        0       47 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/__init__.py
--rw-r--r--   0        0        0       85 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/autosummary_dummy_module.py
--rw-r--r--   0        0        0      168 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-imported_members/conf.py
--rw-r--r--   0        0        0      147 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-imported_members/index.rst
--rw-r--r--   0        0        0      171 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-mock_imports/conf.py
--rw-r--r--   0        0        0       72 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-mock_imports/foo.py
--rw-r--r--   0        0        0      117 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-mock_imports/index.rst
--rw-r--r--   0        0        0      241 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/__init__.py
--rw-r--r--   0        0        0      201 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/autosummary_dummy_module.py
--rw-r--r--   0        0        0      201 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/extra_dummy_module.py
--rw-r--r--   0        0        0      170 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-module_all/conf.py
--rw-r--r--   0        0        0      154 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-module_all/index.rst
--rw-r--r--   0        0        0      132 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/conf.py
--rw-r--r--   0        0        0      174 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/package/__init__.py
--rw-r--r--   0        0        0      147 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/package/module.py
--rw-r--r--   0        0        0       63 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/package/module_importfail.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/package/package/__init__.py
--rw-r--r--   0        0        0      147 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/package/package/module.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/package2/__init__.py
--rw-r--r--   0        0        0      147 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-recursive/package2/module.py
--rw-r--r--   0        0        0      404 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-skip-member/conf.py
--rw-r--r--   0        0        0       54 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-skip-member/index.rst
--rw-r--r--   0        0        0      264 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-skip-member/target.py
--rw-r--r--   0        0        0        6 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-template/_templates/empty.rst
--rw-r--r--   0        0        0      209 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-template/conf.py
--rw-r--r--   0        0        0       78 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-template/index.rst
--rw-r--r--   0        0        0       39 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary-template/target.py
--rw-r--r--   0        0        0       22 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary/autosummary_class_module.py
--rw-r--r--   0        0        0      232 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary/autosummary_dummy_inherited_module.py
--rw-r--r--   0        0        0      932 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary/autosummary_dummy_module.py
--rw-r--r--   0        0        0       63 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary/autosummary_importfail.py
--rw-r--r--   0        0        0      190 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary/conf.py
--rw-r--r--   0        0        0      499 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-autosummary/index.rst
--rw-r--r--   0        0        0      242 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-coverage/conf.py
--rw-r--r--   0        0        0      254 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-coverage/coverage_ignored.py
--rw-r--r--   0        0        0      254 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-coverage/coverage_not_ignored.py
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-coverage/index.rst
--rw-r--r--   0        0        0      371 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest-skipif/conf.py
--rw-r--r--   0        0        0     2052 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest-skipif/skipif.txt
--rw-r--r--   0        0        0      205 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest-with-autodoc/conf.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest-with-autodoc/dir/__init__.py
--rw-r--r--   0        0        0       28 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest-with-autodoc/dir/bar.py
--rw-r--r--   0        0        0       60 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest-with-autodoc/dir/inner.rst
--rw-r--r--   0        0        0       25 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest-with-autodoc/foo.py
--rw-r--r--   0        0        0       52 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest-with-autodoc/index.rst
--rw-r--r--   0        0        0      148 2023-08-30 22:09:32.856407 sphinx-7.2.5/tests/roots/test-ext-doctest/conf.py
--rw-r--r--   0        0        0     2147 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-doctest/doctest.txt
--rw-r--r--   0        0        0      190 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/conf.py
--rw-r--r--   0        0        0      555 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst
--rw-r--r--   0        0        0      161 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-extlinks-hardcoded-urls/conf.py
--rw-r--r--   0        0        0      703 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst
--rw-r--r--   0        0        0       40 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-githubpages/conf.py
--rw-r--r--   0        0        0       25 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-githubpages/index.rst
--rw-r--r--   0        0        0      187 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-graphviz/_static/images/test.svg
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-graphviz/conf.py
--rw-r--r--   0        0        0       25 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-graphviz/graph.dot
--rw-r--r--   0        0        0       25 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-graphviz/graph.xx.dot
--rw-r--r--   0        0        0      641 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-graphviz/index.rst
--rw-r--r--   0        0        0      256 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-ifconfig/conf.py
--rw-r--r--   0        0        0      274 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-ifconfig/index.rst
--rw-r--r--   0        0        0       41 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgconverter/conf.py
--rw-r--r--   0        0        0   141783 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgconverter/img.pdf
--rw-r--r--   0        0        0       86 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgconverter/index.rst
--rw-r--r--   0        0        0      243 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgconverter/svgimg.svg
--rw-r--r--   0        0        0      106 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgmockconverter/1/svgimg.svg
--rw-r--r--   0        0        0      243 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgmockconverter/2/svgimg.svg
--rw-r--r--   0        0        0       97 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgmockconverter/conf.py
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgmockconverter/index.rst
--rw-r--r--   0        0        0      881 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py
--rw-r--r--   0        0        0      138 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-inheritance_diagram/conf.py
--rw-r--r--   0        0        0       13 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-inheritance_diagram/example/__init__.py
--rw-r--r--   0        0        0       46 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-inheritance_diagram/example/sphinx.py
--rw-r--r--   0        0        0       52 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-inheritance_diagram/external/other.py
--rw-r--r--   0        0        0      354 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-inheritance_diagram/index.rst
--rw-r--r--   0        0        0      264 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-inheritance_diagram/subdir/page1.rst
--rw-r--r--   0        0        0      178 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-inheritance_diagram/subdir/page2.rst
--rw-r--r--   0        0        0      198 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-inheritance_diagram/test.py
--rw-r--r--   0        0        0       40 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-intersphinx-cppdomain/conf.py
--rw-r--r--   0        0        0      150 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-intersphinx-cppdomain/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-intersphinx-role/conf.py
--rw-r--r--   0        0        0     1211 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-intersphinx-role/index.rst
--rw-r--r--   0        0        0      488 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math-compat/conf.py
--rw-r--r--   0        0        0      199 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math-compat/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math-simple/conf.py
--rw-r--r--   0        0        0       43 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math-simple/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math/conf.py
--rw-r--r--   0        0        0      239 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math/index.rst
--rw-r--r--   0        0        0      396 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math/math.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math/nomath.rst
--rw-r--r--   0        0        0      128 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-math/page.rst
--rw-r--r--   0        0        0      100 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-napoleon/conf.py
--rw-r--r--   0        0        0       64 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-napoleon/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-napoleon/mypackage/__init__.py
--rw-r--r--   0        0        0      194 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-napoleon/mypackage/typehints.py
--rw-r--r--   0        0        0       70 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-napoleon/typehints.rst
--rw-r--r--   0        0        0       31 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-todo/bar.rst
--rw-r--r--   0        0        0       33 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-todo/conf.py
--rw-r--r--   0        0        0      125 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-todo/foo.rst
--rw-r--r--   0        0        0      109 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-todo/index.rst
--rw-r--r--   0        0        0      108 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode-find/conf.py
--rw-r--r--   0        0        0      636 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode-find/index.rst
--rw-r--r--   0        0        0       37 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode-find/not_a_package/__init__.py
--rw-r--r--   0        0        0      371 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode-find/not_a_package/submodule.py
--rw-r--r--   0        0        0      745 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode/conf.py
--rw-r--r--   0        0        0      550 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode/index.rst
--rw-r--r--   0        0        0     3112 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode/objects.rst
--rw-r--r--   0        0        0       64 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode/spam/__init__.py
--rw-r--r--   0        0        0      308 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode/spam/mod1.py
--rw-r--r--   0        0        0      188 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode/spam/mod2.py
--rw-r--r--   0        0        0       52 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-ext-viewcode/spam/mod3.py
--rw-r--r--   0        0        0       63 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-extensions/conf.py
--rw-r--r--   0        0        0       70 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-extensions/read_parallel.py
--rw-r--r--   0        0        0       71 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-extensions/read_serial.py
--rw-r--r--   0        0        0       72 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-extensions/write_parallel.py
--rw-r--r--   0        0        0       72 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-extensions/write_serial.py
--rw-r--r--   0        0        0       70 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-footnotes/bar.rst
--rw-r--r--   0        0        0       70 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-footnotes/baz.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-footnotes/conf.py
--rw-r--r--   0        0        0     3386 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-footnotes/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.860407 sphinx-7.2.5/tests/roots/test-footnotes/rimg.png
--rw-r--r--   0        0        0      143 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-gettext-template/_templates/template1.html
--rw-r--r--   0        0        0      143 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-gettext-template/_templates/template2.html
--rw-r--r--   0        0        0       32 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-gettext-template/conf.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-gettext-template/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-glossary/conf.py
--rw-r--r--   0        0        0      260 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-glossary/index.rst
--rw-r--r--   0        0        0      103 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-highlight_options/conf.py
--rw-r--r--   0        0        0      166 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-highlight_options/index.rst
--rw-r--r--   0        0        0      468 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/conf.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/extra/.htaccess
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/extra/.htpasswd
--rw-r--r--   0        0        0       28 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/extra/API.html_t
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/extra/css/style.css
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/extra/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/extra/rimg.png
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/extra/subdir/.htaccess
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/extra/subdir/.htpasswd
--rw-r--r--   0        0        0       65 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/.htaccess
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/.htpasswd
--rw-r--r--   0        0        0       28 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/API.html_t
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/css/style.css
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/js/custom.js
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/rimg.png
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/subdir/.htaccess
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/static/subdir/.htpasswd
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/subdir/_build/index.html
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_assets/subdir/background.png
--rw-r--r--   0        0        0       53 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_entity/conf.py
--rw-r--r--   0        0        0      561 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_entity/index.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_file_checksum/conf.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_file_checksum/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_file_checksum/static/empty.js
--rw-r--r--   0        0        0       13 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_file_checksum/static/script.js
--rw-r--r--   0        0        0       19 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_file_checksum/static/stylesheet-a.css
--rw-r--r--   0        0        0       19 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_file_checksum/static/stylesheet-b.css
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_scaled_image_link/conf.py
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_scaled_image_link/img.png
--rw-r--r--   0        0        0      172 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_scaled_image_link/index.rst
--rw-r--r--   0        0        0       36 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_signaturereturn_icon/conf.py
--rw-r--r--   0        0        0      108 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_signaturereturn_icon/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_style/_static/default.css
--rw-r--r--   0        0        0       58 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_style/conf.py
--rw-r--r--   0        0        0       22 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-html_style/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-escape/conf.py
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-escape/img_#1.png
--rw-r--r--   0        0        0      145 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-escape/index.rst
--rw-r--r--   0        0        0      161 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-in-parsed-literal/conf.py
--rw-r--r--   0        0        0      113 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-in-parsed-literal/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-in-parsed-literal/pic.png
--rw-r--r--   0        0        0      143 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-in-section/conf.py
--rw-r--r--   0        0        0      287 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-in-section/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-image-in-section/pic.png
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/conf.py
--rw-r--r--   0        0        0    24976 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/img.gif
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/img.ja.png
--rw-r--r--   0        0        0   141783 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/img.pdf
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/img.png
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/img.zh.png
--rw-r--r--   0        0        0      466 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/rimg.png
--rw-r--r--   0        0        0      218 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/rimg.png.xx
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/rimg.xx.png
--rw-r--r--   0        0        0      128 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/subdir/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/subdir/rimg.png
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.864408 sphinx-7.2.5/tests/roots/test-images/subdir/rimg.xx.png
--rw-r--r--   0        0        0   141783 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-images/subdir/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-images/subdir/svgimg.svg
--rw-r--r--   0        0        0      243 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-images/subdir/svgimg.xx.svg
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-images/testimäge.png
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-index_on_title/conf.py
--rw-r--r--   0        0        0      117 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-index_on_title/contents.rst
--rw-r--r--   0        0        0       70 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/basic_diagram.rst
--rw-r--r--   0        0        0      135 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/conf.py
--rw-r--r--   0        0        0      166 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/diagram_module_w_2_top_classes.rst
--rw-r--r--   0        0        0      125 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/diagram_w_1_top_class.rst
--rw-r--r--   0        0        0      179 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/diagram_w_2_top_classes.rst
--rw-r--r--   0        0        0      104 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/diagram_w_nested_classes.rst
--rw-r--r--   0        0        0      118 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/diagram_w_parts.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/dummy/__init__.py
--rw-r--r--   0        0        0      267 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/dummy/test.py
--rw-r--r--   0        0        0       95 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/dummy/test_nested.py
--rw-r--r--   0        0        0       31 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-inheritance/index.rst
--rw-r--r--   0        0        0      216 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/_templates/contents.html
--rw-r--r--   0        0        0      599 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/admonitions.txt
--rw-r--r--   0        0        0       74 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/bom.txt
--rw-r--r--   0        0        0      262 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/conf.py
--rw-r--r--   0        0        0      342 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/definition_terms.txt
--rw-r--r--   0        0        0      709 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/docfields.txt
--rw-r--r--   0        0        0      858 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/external_links.txt
--rw-r--r--   0        0        0      747 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/figure.txt
--rw-r--r--   0        0        0      407 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/footnote.txt
--rw-r--r--   0        0        0      378 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/glossary_terms.txt
--rw-r--r--   0        0        0      151 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/glossary_terms_inconsistency.txt
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/i18n.png
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/img.png
--rw-r--r--   0        0        0      563 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/index.txt
--rw-r--r--   0        0        0      384 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/index_entries.txt
--rw-r--r--   0        0        0     1832 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/label_target.txt
--rw-r--r--   0        0        0      943 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/literalblock.txt
--rw-r--r--   0        0        0      278 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/noqa.txt
--rw-r--r--   0        0        0      128 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/only.txt
--rw-r--r--   0        0        0       78 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/raw.txt
--rw-r--r--   0        0        0     1094 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/refs.txt
--rw-r--r--   0        0        0      291 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/refs_inconsistency.txt
--rw-r--r--   0        0        0      252 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/refs_python_domain.txt
--rw-r--r--   0        0        0      738 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/role_xref.txt
--rw-r--r--   0        0        0      152 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/rubric.txt
--rw-r--r--   0        0        0       97 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/section.txt
--rw-r--r--   0        0        0      210 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/seealso.txt
--rw-r--r--   0        0        0       32 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/subdir/index.txt
--rw-r--r--   0        0        0      263 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/table.txt
--rw-r--r--   0        0        0      139 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/toctree.txt
--rw-r--r--   0        0        0      135 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/topic.txt
--rw-r--r--   0        0        0      894 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/translation_progress.txt
--rw-r--r--   0        0        0      337 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/versionchange.txt
--rw-r--r--   0        0        0       79 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/warnings.txt
--rw-r--r--   0        0        0     1513 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po
--rw-r--r--   0        0        0      264 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/bom.po
--rw-r--r--   0        0        0     1198 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po
--rw-r--r--   0        0        0     1086 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po
--rw-r--r--   0        0        0     1691 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po
--rw-r--r--   0        0        0     1307 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/figure.po
--rw-r--r--   0        0        0     1228 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po
--rw-r--r--   0        0        0     1327 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po
--rw-r--r--   0        0        0      754 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po
--rw-r--r--   0        0        0      773 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     1318 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po
--rw-r--r--   0        0        0     2159 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po
--rw-r--r--   0        0        0     2211 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po
--rw-r--r--   0        0        0     1380 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po
--rw-r--r--   0        0        0      723 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/only.po
--rw-r--r--   0        0        0      644 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/raw.po
--rw-r--r--   0        0        0     2771 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/refs.po
--rw-r--r--   0        0        0     1045 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po
--rw-r--r--   0        0        0      675 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po
--rw-r--r--   0        0        0     1707 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po
--rw-r--r--   0        0        0      744 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po
--rw-r--r--   0        0        0      706 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/section.po
--rw-r--r--   0        0        0      792 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po
--rw-r--r--   0        0        0      621 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po
--rw-r--r--   0        0        0      992 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/table.po
--rw-r--r--   0        0        0      767 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po
--rw-r--r--   0        0        0      750 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/topic.po
--rw-r--r--   0        0        0     1744 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/translation_progress.po
--rw-r--r--   0        0        0     1070 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po
--rw-r--r--   0        0        0      710 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po
--rw-r--r--   0        0        0      263 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/conf.py
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/i18n.png
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/img.png
--rw-r--r--   0        0        0      163 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/index.rst
--rw-r--r--   0        0        0      288 2023-08-30 22:09:32.868408 sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/prolog_epilog_substitution.rst
--rw-r--r--   0        0        0      188 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/prolog_epilog_substitution_excluded.rst
--rw-r--r--   0        0        0     1135 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/xx/LC_MESSAGES/prolog_epilog_substitution.po
--rw-r--r--   0        0        0       21 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-keep_warnings/conf.py
--rw-r--r--   0        0        0       20 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-keep_warnings/index.rst
--rw-r--r--   0        0        0       13 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-babel/bar.rst
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-babel/conf.py
--rw-r--r--   0        0        0       13 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-babel/foo.rst
--rw-r--r--   0        0        0       87 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-babel/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-container/conf.py
--rw-r--r--   0        0        0       35 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-container/index.rst
--rw-r--r--   0        0        0       59 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-equations/conf.py
--rw-r--r--   0        0        0      256 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-equations/equations.rst
--rw-r--r--   0        0        0      452 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-equations/expects/latex-equations.tex
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-figure-in-admonition/conf.py
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-figure-in-admonition/img.png
--rw-r--r--   0        0        0      132 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-figure-in-admonition/index.rst
--rw-r--r--   0        0        0     1573 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-includegraphics/conf.py
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-includegraphics/img.png
--rw-r--r--   0        0        0      834 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-includegraphics/index.rst
--rw-r--r--   0        0        0    34213 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-includegraphics/sphinx.png
--rw-r--r--   0        0        0    38192 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-includegraphics/tall.png
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-index/conf.py
--rw-r--r--   0        0        0      215 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-index/index.rst
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels-before-module/automodule1.py
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels-before-module/automodule2a.py
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels-before-module/automodule2b.py
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels-before-module/automodule3.py
--rw-r--r--   0        0        0      117 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels-before-module/conf.py
--rw-r--r--   0        0        0      464 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels-before-module/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels/conf.py
--rw-r--r--   0        0        0      771 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels/index.rst
--rw-r--r--   0        0        0       18 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-labels/otherdoc.rst
--rw-r--r--   0        0        0      250 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-numfig/conf.py
--rw-r--r--   0        0        0      112 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-numfig/index.rst
--rw-r--r--   0        0        0      141 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-numfig/indexhowto.rst
--rw-r--r--   0        0        0      165 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-numfig/indexmanual.rst
--rw-r--r--   0        0        0       18 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/_mytemplates/latex/longtable.tex_t
--rw-r--r--   0        0        0     1661 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/complex.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/conf.py
--rw-r--r--   0        0        0     1933 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/complex_spanning_cell.tex
--rw-r--r--   0        0        0     1752 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/gridtable.tex
--rw-r--r--   0        0        0     1780 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex
--rw-r--r--   0        0        0     1323 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable.tex
--rw-r--r--   0        0        0     1300 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_align.tex
--rw-r--r--   0        0        0     1445 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_caption.tex
--rw-r--r--   0        0        0     1384 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex
--rw-r--r--   0        0        0     1637 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex
--rw-r--r--   0        0        0     1386 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex
--rw-r--r--   0        0        0     1656 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_widths.tex
--rw-r--r--   0        0        0     1409 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex
--rw-r--r--   0        0        0     1341 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex
--rw-r--r--   0        0        0      704 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/simple_table.tex
--rw-r--r--   0        0        0      851 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_caption.tex
--rw-r--r--   0        0        0      777 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex
--rw-r--r--   0        0        0      978 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex
--rw-r--r--   0        0        0      594 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex
--rw-r--r--   0        0        0      779 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_verbatim.tex
--rw-r--r--   0        0        0     1093 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_widths.tex
--rw-r--r--   0        0        0      802 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex
--rw-r--r--   0        0        0      733 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/tabular_having_widths.tex
--rw-r--r--   0        0        0      747 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/tabularcolumn.tex
--rw-r--r--   0        0        0      727 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/expects/tabulary_having_widths.tex
--rw-r--r--   0        0        0       84 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/index.rst
--rw-r--r--   0        0        0     2516 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/longtable.rst
--rw-r--r--   0        0        0     2770 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-table/tabular.rst
--rw-r--r--   0        0        0       52 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-theme/conf.py
--rw-r--r--   0        0        0       24 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-theme/index.rst
--rw-r--r--   0        0        0      117 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-theme/theme/custom/theme.conf
--rw-r--r--   0        0        0      160 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-title/conf.py
--rw-r--r--   0        0        0      165 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-title/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-unicode/conf.py
--rw-r--r--   0        0        0      142 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-latex-unicode/index.rst
--rw-r--r--   0        0        0       80 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-anchors-ignore-for-url/conf.py
--rw-r--r--   0        0        0      532 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-anchors-ignore-for-url/index.rst
--rw-r--r--   0        0        0       80 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-anchors-ignore/conf.py
--rw-r--r--   0        0        0      109 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-anchors-ignore/index.rst
--rw-r--r--   0        0        0      180 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-documents_exclude/br0ken_link.rst
--rw-r--r--   0        0        0      174 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-documents_exclude/broken_link.rst
--rw-r--r--   0        0        0      133 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-documents_exclude/conf.py
--rw-r--r--   0        0        0       40 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-documents_exclude/index.rst
--rw-r--r--   0        0        0       80 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-localserver-anchor/conf.py
--rw-r--r--   0        0        0       48 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-localserver-anchor/index.rst
--rw-r--r--   0        0        0       55 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-localserver-https/conf.py
--rw-r--r--   0        0        0       42 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-localserver-https/index.rst
--rw-r--r--   0        0        0       55 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-localserver-warn-redirects/conf.py
--rw-r--r--   0        0        0       95 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-localserver-warn-redirects/index.rst
--rw-r--r--   0        0        0       55 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-localserver/conf.py
--rw-r--r--   0        0        0       41 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-localserver/index.rst
--rw-r--r--   0        0        0       55 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-raw-node/conf.py
--rw-r--r--   0        0        0       46 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-raw-node/index.rst
--rw-r--r--   0        0        0       80 2023-08-30 22:09:32.872408 sphinx-7.2.5/tests/roots/test-linkcheck-too-many-retries/conf.py
--rw-r--r--   0        0        0       73 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-linkcheck-too-many-retries/index.rst
--rw-r--r--   0        0        0       99 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-linkcheck/conf.py
--rw-r--r--   0        0        0      648 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-linkcheck/links.rst
--rw-r--r--   0        0        0      143 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-local-logo/conf.py
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-local-logo/images/img.png
--rw-r--r--   0        0        0     1477 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-local-logo/index.rst
--rw-r--r--   0        0        0       80 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       41 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       80 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       41 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       82 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.mo
--rw-r--r--   0        0        0       43 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.po
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-manpage_url/conf.py
--rw-r--r--   0        0        0       61 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-manpage_url/index.rst
--rw-r--r--   0        0        0      114 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-markup-citation/conf.py
--rw-r--r--   0        0        0      166 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-markup-citation/index.rst
--rw-r--r--   0        0        0      114 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-markup-rubric/conf.py
--rw-r--r--   0        0        0      112 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-markup-rubric/index.rst
--rw-r--r--   0        0        0       78 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-maxlistdepth/conf.py
--rw-r--r--   0        0        0      687 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-maxlistdepth/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-metadata/conf.py
--rw-r--r--   0        0        0     1436 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-metadata/index.rst
--rw-r--r--   0        0        0        8 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-need-escaped/bar.rst
--rw-r--r--   0        0        0        8 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-need-escaped/baz.rst
--rw-r--r--   0        0        0       62 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-need-escaped/conf.py
--rw-r--r--   0        0        0       82 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-need-escaped/foo.rst
--rw-r--r--   0        0        0      574 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-need-escaped/index.rst
--rw-r--r--   0        0        0       10 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-need-escaped/quux.rst
--rw-r--r--   0        0        0       29 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-need-escaped/qux.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-nested-enumerated-list/conf.py
--rw-r--r--   0        0        0      300 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-nested-enumerated-list/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-nested-tables/conf.py
--rw-r--r--   0        0        0      248 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-nested-tables/index.rst
--rw-r--r--   0        0        0       16 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-nitpicky-warnings/conf.py
--rw-r--r--   0        0        0      176 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-nitpicky-warnings/index.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numbered-circular/conf.py
--rw-r--r--   0        0        0       36 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numbered-circular/index.rst
--rw-r--r--   0        0        0       23 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numbered-circular/sub.rst
--rw-r--r--   0        0        0      710 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numfig/bar.rst
--rw-r--r--   0        0        0      259 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numfig/baz.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numfig/conf.py
--rw-r--r--   0        0        0      912 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numfig/foo.rst
--rw-r--r--   0        0        0     1024 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numfig/index.rst
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-numfig/rimg.png
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-object-description-sections/conf.py
--rw-r--r--   0        0        0       80 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-object-description-sections/index.rst
--rw-r--r--   0        0        0       73 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/Bare.rst
--rw-r--r--   0        0        0       58 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/Dup1.rst
--rw-r--r--   0        0        0       58 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/Dup2.rst
--rw-r--r--   0        0        0       94 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/LineContinuation.rst
--rw-r--r--   0        0        0       72 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/P1.rst
--rw-r--r--   0        0        0       72 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/P2.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/conf.py
--rw-r--r--   0        0        0       97 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/firstLineRule.rst
--rw-r--r--   0        0        0      663 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-productionlist/index.rst
--rw-r--r--   0        0        0      177 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-prolog/conf.py
--rw-r--r--   0        0        0       83 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-prolog/index.rst
--rw-r--r--   0        0        0       57 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-prolog/markdown.md
--rw-r--r--   0        0        0      299 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-prolog/prolog_markdown_parser.py
--rw-r--r--   0        0        0       67 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-prolog/restructuredtext.rst
--rw-r--r--   0        0        0       75 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-pycode/cp_1251_coded.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-reST-code-block/conf.py
--rw-r--r--   0        0        0       97 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-reST-code-block/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-reST-code-role/conf.py
--rw-r--r--   0        0        0      194 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-reST-code-role/index.rst
--rw-r--r--   0        0        0       27 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-refonly_bullet_list/conf.py
--rw-r--r--   0        0        0      147 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-refonly_bullet_list/index.rst
--rw-r--r--   0        0        0      237 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-remote-logo/conf.py
--rw-r--r--   0        0        0     1477 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-remote-logo/index.rst
--rw-r--r--   0        0        0       32 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-roles-download/another/dummy.dat
--rw-r--r--   0        0        0      114 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-roles-download/conf.py
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-roles-download/dummy.dat
--rw-r--r--   0        0        0      214 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-roles-download/index.rst
--rw-r--r--   0        0        0     2111 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/Makefile
--rw-r--r--   0        0        0       67 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/_templates/contentssb.html
--rw-r--r--   0        0        0       99 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/_templates/customsb.html
--rw-r--r--   0        0        0      428 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/_templates/layout.html
--rw-r--r--   0        0        0      578 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/autodoc.txt
--rw-r--r--   0        0        0     4587 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/autodoc_target.py
--rw-r--r--   0        0        0       74 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/bom.txt
--rw-r--r--   0        0        0     4257 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/conf.py
--rw-r--r--   0        0        0       87 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/extapi.txt
--rw-r--r--   0        0        0      365 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/extensions.txt
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/file_with_special_#_chars.xyz
--rw-r--r--   0        0        0      826 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/footnote.txt
--rw-r--r--   0        0        0      575 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/images.txt
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/img.foo.png
--rw-r--r--   0        0        0    24976 2023-08-30 22:09:32.876408 sphinx-7.2.5/tests/roots/test-root/img.gif
--rw-r--r--   0        0        0   141783 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/img.pdf
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/img.png
--rw-r--r--   0        0        0     2108 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/includes.txt
--rw-r--r--   0        0        0     1118 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/index.txt
--rw-r--r--   0        0        0      750 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/lists.txt
--rw-r--r--   0        0        0      200 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/literal.inc
--rw-r--r--   0        0        0      208 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/literal_orig.inc
--rw-r--r--   0        0        0     6902 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/markup.txt
--rw-r--r--   0        0        0      373 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/math.txt
--rw-r--r--   0        0        0     4608 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/objects.txt
--rw-r--r--   0        0        0      110 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/otherext.foo
--rw-r--r--   0        0        0      346 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/parsermod.py
--rw-r--r--   0        0        0       45 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/quotes.inc
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/rimg.png
--rw-r--r--   0        0        0       87 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/special/api.h
--rw-r--r--   0        0        0       32 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/special/code.py
--rw-r--r--   0        0        0       96 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/subdir/excluded.txt
--rw-r--r--   0        0        0      106 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/subdir/images.txt
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/subdir/img.png
--rw-r--r--   0        0        0      143 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/subdir/include.inc
--rw-r--r--   0        0        0      328 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/subdir/includes.txt
--rw-r--r--   0        0        0    66247 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/subdir/simg.png
--rw-r--r--   0        0        0   141783 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/svgimg.svg
--rw-r--r--   0        0        0       78 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/tabs.inc
--rw-r--r--   0        0        0       77 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/test.inc
--rw-r--r--   0        0        0      107 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-root/wrongenc.inc
--rw-r--r--   0        0        0       58 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-search/conf.py
--rw-r--r--   0        0        0      381 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-search/index.rst
--rw-r--r--   0        0        0       41 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-search/nosearch.rst
--rw-r--r--   0        0        0      184 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-search/tocitem.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-smartquotes/conf.py
--rw-r--r--   0        0        0      107 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-smartquotes/index.rst
--rw-r--r--   0        0        0      231 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-smartquotes/literals.rst
--rw-r--r--   0        0        0      453 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-stylesheets/_templates/layout.html
--rw-r--r--   0        0        0      318 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-stylesheets/conf.py
--rw-r--r--   0        0        0       53 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-stylesheets/index.rst
--rw-r--r--   0        0        0      182 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-templating/_templates/autosummary/class.rst
--rw-r--r--   0        0        0      109 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-templating/_templates/layout.html
--rw-r--r--   0        0        0      135 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-templating/autosummary_templating.txt
--rw-r--r--   0        0        0      266 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-templating/conf.py
--rw-r--r--   0        0        0      124 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-templating/index.txt
--rw-r--r--   0        0        0      661 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-theming/child.zip
--rw-r--r--   0        0        0       94 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-theming/conf.py
--rw-r--r--   0        0        0       26 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-theming/index.rst
--rw-r--r--   0        0        0     1039 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-theming/parent.zip
--rw-r--r--   0        0        0       82 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-theming/test_theme/__init__.py
--rw-r--r--   0        0        0      139 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-theming/test_theme/staticfiles/layout.html
--rw-r--r--   0        0        0      120 2023-08-30 22:09:32.880409 sphinx-7.2.5/tests/roots/test-theming/test_theme/staticfiles/static/staticimg.png
--rw-r--r--   0        0        0       82 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-theming/test_theme/staticfiles/static/statictmpl.html_t
--rw-r--r--   0        0        0      104 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-theming/test_theme/staticfiles/theme.conf
--rw-r--r--   0        0        0       98 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-theming/test_theme/test-theme/theme.conf
--rw-r--r--   0        0        0     1039 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-theming/ziptheme.zip
--rw-r--r--   0        0        0      150 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-tocdepth/bar.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-tocdepth/baz.rst
--rw-r--r--   0        0        0       53 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-tocdepth/conf.py
--rw-r--r--   0        0        0      146 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-tocdepth/foo.rst
--rw-r--r--   0        0        0       71 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-tocdepth/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-domain-objects/conf.py
--rw-r--r--   0        0        0      731 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-domain-objects/domains.rst
--rw-r--r--   0        0        0       90 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-domain-objects/index.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-duplicated/conf.py
--rw-r--r--   0        0        0        8 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-duplicated/foo.rst
--rw-r--r--   0        0        0       77 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-duplicated/index.rst
--rw-r--r--   0        0        0      101 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-empty/_templates/localtoc.html
--rw-r--r--   0        0        0       62 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-empty/conf.py
--rw-r--r--   0        0        0       52 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-empty/index.rst
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/bar/bar_1.rst
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/bar/bar_2.rst
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/bar/bar_3.rst
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/bar/bar_4/index.rst
--rw-r--r--   0        0        0       53 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/bar/index.rst
--rw-r--r--   0        0        0       13 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/baz.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/conf.py
--rw-r--r--   0        0        0       13 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/foo.rst
--rw-r--r--   0        0        0      303 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/index.rst
--rw-r--r--   0        0        0       16 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/quux.rst
--rw-r--r--   0        0        0       50 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/qux/index.rst
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/qux/qux_1.rst
--rw-r--r--   0        0        0       17 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-glob/qux/qux_2.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-index/conf.py
--rw-r--r--   0        0        0      105 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-index/foo.rst
--rw-r--r--   0        0        0      132 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-index/index.rst
--rw-r--r--   0        0        0      150 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-maxdepth/bar.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-maxdepth/baz.rst
--rw-r--r--   0        0        0       30 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-maxdepth/conf.py
--rw-r--r--   0        0        0      146 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-maxdepth/foo.rst
--rw-r--r--   0        0        0      105 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-maxdepth/index.rst
--rw-r--r--   0        0        0      105 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree-maxdepth/qux.rst
--rw-r--r--   0        0        0        8 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree/bar.rst
--rw-r--r--   0        0        0        8 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree/baz.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree/conf.py
--rw-r--r--   0        0        0       74 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree/foo.rst
--rw-r--r--   0        0        0      885 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree/index.rst
--rw-r--r--   0        0        0       10 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree/quux.rst
--rw-r--r--   0        0        0       29 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree/qux.rst
--rw-r--r--   0        0        0       97 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-toctree/tocdepth.rst
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-transforms-post_transforms-keyboard/conf.py
--rw-r--r--   0        0        0       94 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-transforms-post_transforms-keyboard/index.rst
--rw-r--r--   0        0        0       16 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-transforms-post_transforms-missing-reference/conf.py
--rw-r--r--   0        0        0      113 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-transforms-post_transforms-missing-reference/index.rst
--rw-r--r--   0        0        0       36 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-trim_doctest_flags/conf.py
--rw-r--r--   0        0        0      784 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-trim_doctest_flags/index.rst
--rw-r--r--   0        0        0     1012 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/added.txt
--rw-r--r--   0        0        0       86 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/conf.py
--rw-r--r--   0        0        0      584 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/deleted.txt
--rw-r--r--   0        0        0      490 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/deleted_end.txt
--rw-r--r--   0        0        0      164 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/index.txt
--rw-r--r--   0        0        0      864 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/insert.txt
--rw-r--r--   0        0        0      850 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/insert_beginning.txt
--rw-r--r--   0        0        0      735 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/insert_similar.txt
--rw-r--r--   0        0        0      867 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/modified.txt
--rw-r--r--   0        0        0      715 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-versioning/original.txt
--rw-r--r--   0        0        0      151 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-warnings/autodoc_fodder.py
--rw-r--r--   0        0        0       97 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-warnings/conf.py
--rw-r--r--   0        0        0      698 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-warnings/index.rst
--rw-r--r--   0        0        0   141783 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-warnings/svgimg.pdf
--rw-r--r--   0        0        0      243 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-warnings/svgimg.svg
--rw-r--r--   0        0        0       18 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-warnings/undecodable.rst
--rw-r--r--   0        0        0      107 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/roots/test-warnings/wrongenc.inc
--rw-r--r--   0        0        0     1918 2023-08-30 22:09:32.884409 sphinx-7.2.5/tests/test_addnodes.py
--rw-r--r--   0        0        0     3309 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_api_translator.py
--rw-r--r--   0        0        0     5494 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_application.py
--rw-r--r--   0        0        0     4719 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build.py
--rw-r--r--   0        0        0     1152 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_changes.py
--rw-r--r--   0        0        0     1407 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_dirhtml.py
--rw-r--r--   0        0        0    16652 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_epub.py
--rw-r--r--   0        0        0     7839 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_gettext.py
--rw-r--r--   0        0        0    82944 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_html.py
--rw-r--r--   0        0        0    76628 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_latex.py
--rw-r--r--   0        0        0    34191 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_linkcheck.py
--rw-r--r--   0        0        0     2785 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_manpage.py
--rw-r--r--   0        0        0     5925 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_texinfo.py
--rw-r--r--   0        0        0     8996 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_build_text.py
--rw-r--r--   0        0        0     1322 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_builder.py
--rw-r--r--   0        0        0     2729 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_catalogs.py
--rw-r--r--   0        0        0    18197 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_config.py
--rw-r--r--   0        0        0      811 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_correct_year.py
--rw-r--r--   0        0        0    22630 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_directive_code.py
--rw-r--r--   0        0        0     2088 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_directive_object_description.py
--rw-r--r--   0        0        0     1655 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_directive_only.py
--rw-r--r--   0        0        0     6912 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_directive_other.py
--rw-r--r--   0        0        0     4362 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_directive_patch.py
--rw-r--r--   0        0        0     5542 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_directives_no_typesetting.py
--rw-r--r--   0        0        0     1084 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_docutilsconf.py
--rw-r--r--   0        0        0    37517 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_domain_c.py
--rw-r--r--   0        0        0    76152 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_domain_cpp.py
--rw-r--r--   0        0        0    20323 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_domain_js.py
--rw-r--r--   0        0        0    99015 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_domain_py.py
--rw-r--r--   0        0        0     5904 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_domain_rst.py
--rw-r--r--   0        0        0    19424 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_domain_std.py
--rw-r--r--   0        0        0     5298 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_environment.py
--rw-r--r--   0        0        0     8068 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_environment_indexentries.py
--rw-r--r--   0        0        0      310 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_environment_record_dependencies.py
--rw-r--r--   0        0        0    20386 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_environment_toctree.py
--rw-r--r--   0        0        0      321 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_errors.py
--rw-r--r--   0        0        0     1826 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_events.py
--rw-r--r--   0        0        0    23586 2023-08-30 22:09:32.888409 sphinx-7.2.5/tests/test_ext_apidoc.py
--rw-r--r--   0        0        0    79428 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc.py
--rw-r--r--   0        0        0     4801 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_autoattribute.py
--rw-r--r--   0        0        0    14302 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_autoclass.py
--rw-r--r--   0        0        0     2631 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_autodata.py
--rw-r--r--   0        0        0     5647 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_autofunction.py
--rw-r--r--   0        0        0     5355 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_automodule.py
--rw-r--r--   0        0        0     2501 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_autoproperty.py
--rw-r--r--   0        0        0    55422 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_configs.py
--rw-r--r--   0        0        0     3335 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_events.py
--rw-r--r--   0        0        0     3979 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_mock.py
--rw-r--r--   0        0        0     6143 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_preserve_defaults.py
--rw-r--r--   0        0        0     4415 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autodoc_private_members.py
--rw-r--r--   0        0        0     3145 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autosectionlabel.py
--rw-r--r--   0        0        0    28028 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_autosummary.py
--rw-r--r--   0        0        0     3575 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_coverage.py
--rw-r--r--   0        0        0     5511 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_doctest.py
--rw-r--r--   0        0        0      378 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_duration.py
--rw-r--r--   0        0        0     2104 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_extlinks.py
--rw-r--r--   0        0        0      958 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_githubpages.py
--rw-r--r--   0        0        0     8462 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_graphviz.py
--rw-r--r--   0        0        0      850 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_ifconfig.py
--rw-r--r--   0        0        0     1038 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_imgconverter.py
--rw-r--r--   0        0        0      609 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_imgmockconverter.py
--rw-r--r--   0        0        0    13984 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_inheritance_diagram.py
--rw-r--r--   0        0        0    21302 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_intersphinx.py
--rw-r--r--   0        0        0    14083 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_math.py
--rw-r--r--   0        0        0     7094 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_napoleon.py
--rw-r--r--   0        0        0    70640 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_napoleon_docstring.py
--rw-r--r--   0        0        0     3878 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_todo.py
--rw-r--r--   0        0        0     5617 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_ext_viewcode.py
--rw-r--r--   0        0        0      857 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_extension.py
--rw-r--r--   0        0        0     3599 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_highlighting.py
--rw-r--r--   0        0        0    53684 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_intl.py
--rw-r--r--   0        0        0     2551 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_locale.py
--rw-r--r--   0        0        0    22386 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_markup.py
--rw-r--r--   0        0        0     1931 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_metadata.py
--rw-r--r--   0        0        0     2459 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_parser.py
--rw-r--r--   0        0        0     2790 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_project.py
--rw-r--r--   0        0        0     6923 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_pycode.py
--rw-r--r--   0        0        0     2840 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_pycode_ast.py
--rw-r--r--   0        0        0    18264 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_pycode_parser.py
--rw-r--r--   0        0        0     7422 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_quickstart.py
--rw-r--r--   0        0        0     2570 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_roles.py
--rw-r--r--   0        0        0    11736 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_search.py
--rw-r--r--   0        0        0     3747 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_smartquotes.py
--rw-r--r--   0        0        0     1435 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_templating.py
--rw-r--r--   0        0        0     4795 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_theming.py
--rw-r--r--   0        0        0     1843 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_toctree.py
--rw-r--r--   0        0        0     2517 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_transforms_move_module_targets.py
--rw-r--r--   0        0        0    11587 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_transforms_post_transforms.py
--rw-r--r--   0        0        0     1324 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_transforms_post_transforms_code.py
--rw-r--r--   0        0        0     4169 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_transforms_reorder_nodes.py
--rw-r--r--   0        0        0     2850 2023-08-30 22:09:32.892409 sphinx-7.2.5/tests/test_util.py
--rw-r--r--   0        0        0     3203 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_display.py
--rw-r--r--   0        0        0     3032 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_docstrings.py
--rw-r--r--   0        0        0     2647 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_docutils.py
--rw-r--r--   0        0        0     4000 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_fileutil.py
--rw-r--r--   0        0        0     8704 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_i18n.py
--rw-r--r--   0        0        0     2713 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_images.py
--rw-r--r--   0        0        0    29622 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_inspect.py
--rw-r--r--   0        0        0     4057 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_inventory.py
--rw-r--r--   0        0        0    13533 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_logging.py
--rw-r--r--   0        0        0     7180 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_matching.py
--rw-r--r--   0        0        0     7482 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_nodes.py
--rw-r--r--   0        0        0     7333 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_rst.py
--rw-r--r--   0        0        0      952 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_template.py
--rw-r--r--   0        0        0    28601 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_util_typing.py
--rw-r--r--   0        0        0     3581 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_versioning.py
--rw-r--r--   0        0        0     1110 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/test_writer_latex.py
--rw-r--r--   0        0        0     1887 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/typing_test_data.py
--rw-r--r--   0        0        0     1663 2023-08-30 22:09:32.896409 sphinx-7.2.5/tests/utils.py
--rw-r--r--   0        0        0      994 2023-08-30 22:09:32.896409 sphinx-7.2.5/tox.ini
--rw-r--r--   0        0        0      226 2023-08-30 22:09:32.896409 sphinx-7.2.5/utils/CHANGES_template
--rw-r--r--   0        0        0        0 2023-08-30 22:09:32.896409 sphinx-7.2.5/utils/__init__.py
--rw-r--r--   0        0        0     8368 2023-08-30 22:09:32.896409 sphinx-7.2.5/utils/babel_runner.py
--rw-r--r--   0        0        0     1646 2023-08-30 22:09:32.896409 sphinx-7.2.5/utils/bump_docker.py
--rwxr-xr-x   0        0        0     5812 2023-08-30 22:09:32.896409 sphinx-7.2.5/utils/bump_version.py
--rw-r--r--   0        0        0     1697 2023-08-30 22:09:32.896409 sphinx-7.2.5/utils/release-checklist
--rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 sphinx-7.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3818 2023-09-13 23:12:58.873780 sphinx-7.2.6/AUTHORS
+-rw-r--r--   0        0        0   382197 2023-09-13 23:12:58.873780 sphinx-7.2.6/CHANGES
+-rw-r--r--   0        0        0     3530 2023-09-13 23:12:58.873780 sphinx-7.2.6/CODE_OF_CONDUCT
+-rw-r--r--   0        0        0    26147 2023-09-13 23:12:58.873780 sphinx-7.2.6/EXAMPLES
+-rw-r--r--   0        0        0     3135 2023-09-13 23:12:58.873780 sphinx-7.2.6/LICENSE
+-rw-r--r--   0        0        0     2323 2023-09-13 23:12:58.881780 sphinx-7.2.6/README.rst
+-rw-r--r--   0        0        0      607 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/Makefile
+-rw-r--r--   0        0        0      152 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/Makefile
+-rw-r--r--   0        0        0    27523 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/bookcover.png
+-rw-r--r--   0        0        0     9875 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/conf.py.txt
+-rw-r--r--   0        0        0     3307 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/favicon.svg
+-rw-r--r--   0        0        0     1351 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/more.png
+-rw-r--r--   0        0        0    34213 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/sphinx.png
+-rw-r--r--   0        0        0    25792 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/agogo.png
+-rw-r--r--   0        0        0    32356 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/alabaster.png
+-rw-r--r--   0        0        0    27139 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/bizstyle.png
+-rw-r--r--   0        0        0    39927 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/classic.png
+-rw-r--r--   0        0        0    56954 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/fullsize/agogo.png
+-rw-r--r--   0        0        0    40248 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/fullsize/alabaster.png
+-rw-r--r--   0        0        0    75192 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/fullsize/bizstyle.png
+-rw-r--r--   0        0        0    72597 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/fullsize/classic.png
+-rw-r--r--   0        0        0    84200 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/fullsize/haiku.png
+-rw-r--r--   0        0        0    32266 2023-09-13 23:12:58.881780 sphinx-7.2.6/doc/_static/themes/fullsize/nature.png
+-rw-r--r--   0        0        0   102717 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/fullsize/pyramid.png
+-rw-r--r--   0        0        0    88111 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/fullsize/scrolls.png
+-rw-r--r--   0        0        0    39411 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/fullsize/sphinx_rtd_theme.png
+-rw-r--r--   0        0        0    84439 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/fullsize/sphinxdoc.png
+-rw-r--r--   0        0        0    91744 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/fullsize/traditional.png
+-rw-r--r--   0        0        0    43184 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/haiku.png
+-rw-r--r--   0        0        0    28536 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/nature.png
+-rw-r--r--   0        0        0    38805 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/pyramid.png
+-rw-r--r--   0        0        0    27800 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/scrolls.png
+-rw-r--r--   0        0        0    29138 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/sphinx_rtd_theme.png
+-rw-r--r--   0        0        0    30225 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/sphinxdoc.png
+-rw-r--r--   0        0        0    32258 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/themes/traditional.png
+-rw-r--r--   0        0        0    16371 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/translation.png
+-rw-r--r--   0        0        0      342 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/translation.puml
+-rw-r--r--   0        0        0     8232 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/translation.svg
+-rw-r--r--   0        0        0    26500 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/tutorial/lumache-autosummary.png
+-rw-r--r--   0        0        0    52126 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/tutorial/lumache-first-light.png
+-rw-r--r--   0        0        0    51223 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/tutorial/lumache-furo.png
+-rw-r--r--   0        0        0    71741 2023-09-13 23:12:58.885780 sphinx-7.2.6/doc/_static/tutorial/lumache-py-function-full.png
+-rw-r--r--   0        0        0    41828 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/_static/tutorial/lumache-py-function.png
+-rw-r--r--   0        0        0      271 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/_templates/contents.html
+-rw-r--r--   0        0        0     1860 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/_themes/sphinx13/layout.html
+-rw-r--r--   0        0        0     6552 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/_themes/sphinx13/static/sphinx13.css
+-rw-r--r--   0        0        0    11719 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/_themes/sphinx13/static/sphinxheader.png
+-rw-r--r--   0        0        0       60 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/_themes/sphinx13/theme.conf
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/authors.rst
+-rw-r--r--   0        0        0      400 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/changes.rst
+-rw-r--r--   0        0        0     9310 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/conf.py
+-rw-r--r--   0        0        0     1151 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/builders.rst
+-rw-r--r--   0        0        0      649 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/index.rst
+-rw-r--r--   0        0        0     1051 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/overview.rst
+-rw-r--r--   0        0        0    15049 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/templating.rst
+-rw-r--r--   0        0        0    12324 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/theming.rst
+-rw-r--r--   0        0        0     4020 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/autodoc_ext.rst
+-rw-r--r--   0        0        0      438 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/examples/README.rst
+-rw-r--r--   0        0        0     1844 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/examples/autodoc_intenum.py
+-rw-r--r--   0        0        0      400 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/examples/helloworld.py
+-rw-r--r--   0        0        0     5030 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/examples/recipe.py
+-rw-r--r--   0        0        0     3942 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/examples/todo.py
+-rw-r--r--   0        0        0     5289 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/helloworld.rst
+-rw-r--r--   0        0        0      262 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/index.rst
+-rw-r--r--   0        0        0     8216 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/recipe.rst
+-rw-r--r--   0        0        0    13435 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/development/tutorials/todo.rst
+-rw-r--r--   0        0        0       54 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/examples.rst
+-rw-r--r--   0        0        0    14996 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/appapi.rst
+-rw-r--r--   0        0        0     1103 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/builderapi.rst
+-rw-r--r--   0        0        0      165 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/collectorapi.rst
+-rw-r--r--   0        0        0    41794 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/deprecated.rst
+-rw-r--r--   0        0        0      518 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/domainapi.rst
+-rw-r--r--   0        0        0     1043 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/envapi.rst
+-rw-r--r--   0        0        0     2817 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/i18n.rst
+-rw-r--r--   0        0        0     8597 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/index.rst
+-rw-r--r--   0        0        0     2384 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/logging.rst
+-rw-r--r--   0        0        0     4787 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/markupapi.rst
+-rw-r--r--   0        0        0     2706 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/nodes.rst
+-rw-r--r--   0        0        0     1243 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/parserapi.rst
+-rw-r--r--   0        0        0      114 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/projectapi.rst
+-rw-r--r--   0        0        0      943 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/extdev/utils.rst
+-rw-r--r--   0        0        0    13425 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/faq.rst
+-rw-r--r--   0        0        0     4173 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/glossary.rst
+-rw-r--r--   0        0        0     3539 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/index.rst
+-rw-r--r--   0        0        0       71 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/internals/code-of-conduct.rst
+-rw-r--r--   0        0        0    11482 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/internals/contributing.rst
+-rw-r--r--   0        0        0      353 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/internals/index.rst
+-rw-r--r--   0        0        0     1964 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/internals/organization.rst
+-rw-r--r--   0        0        0     4395 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/internals/release-process.rst
+-rw-r--r--   0        0        0    69427 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/latex.rst
+-rw-r--r--   0        0        0      784 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/make.bat
+-rw-r--r--   0        0        0      314 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/man/index.rst
+-rw-r--r--   0        0        0     4508 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/man/sphinx-apidoc.rst
+-rw-r--r--   0        0        0     2122 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/man/sphinx-autogen.rst
+-rw-r--r--   0        0        0    10673 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/man/sphinx-build.rst
+-rw-r--r--   0        0        0     3692 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/man/sphinx-quickstart.rst
+-rw-r--r--   0        0        0      806 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/support.rst
+-rw-r--r--   0        0        0     4981 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/tutorial/automatic-doc-generation.rst
+-rw-r--r--   0        0        0    11090 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/tutorial/deploying.rst
+-rw-r--r--   0        0        0     9134 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/tutorial/describing-code.rst
+-rw-r--r--   0        0        0      240 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/tutorial/end.rst
+-rw-r--r--   0        0        0     3450 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/tutorial/first-steps.rst
+-rw-r--r--   0        0        0     3723 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/tutorial/getting-started.rst
+-rw-r--r--   0        0        0     1433 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/tutorial/index.rst
+-rw-r--r--   0        0        0     2528 2023-09-13 23:12:58.889780 sphinx-7.2.6/doc/tutorial/more-sphinx-customization.rst
+-rw-r--r--   0        0        0     4177 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/tutorial/narrative-documentation.rst
+-rw-r--r--   0        0        0    11831 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/advanced/intl.rst
+-rw-r--r--   0        0        0     2670 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/advanced/websupport/api.rst
+-rw-r--r--   0        0        0      302 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/advanced/websupport/index.rst
+-rw-r--r--   0        0        0     9640 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/advanced/websupport/quickstart.rst
+-rw-r--r--   0        0        0     1368 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/advanced/websupport/searchadapters.rst
+-rw-r--r--   0        0        0     1231 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/advanced/websupport/storagebackends.rst
+-rw-r--r--   0        0        0    17742 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/builders/index.rst
+-rw-r--r--   0        0        0   103770 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/configuration.rst
+-rw-r--r--   0        0        0    29866 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/autodoc.rst
+-rw-r--r--   0        0        0     1899 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/autosectionlabel.rst
+-rw-r--r--   0        0        0    11099 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/autosummary.rst
+-rw-r--r--   0        0        0     2832 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/coverage.rst
+-rw-r--r--   0        0        0    12084 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/doctest.rst
+-rw-r--r--   0        0        0      404 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/duration.rst
+-rw-r--r--   0        0        0     9665 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/example_google.py
+-rw-r--r--   0        0        0      296 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/example_google.rst
+-rw-r--r--   0        0        0     9714 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/example_numpy.py
+-rw-r--r--   0        0        0      292 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/example_numpy.rst
+-rw-r--r--   0        0        0     2781 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/extlinks.rst
+-rw-r--r--   0        0        0      491 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/githubpages.rst
+-rw-r--r--   0        0        0     6292 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/graphviz.rst
+-rw-r--r--   0        0        0     1329 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/ifconfig.rst
+-rw-r--r--   0        0        0     1705 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/imgconverter.rst
+-rw-r--r--   0        0        0     2410 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/index.rst
+-rw-r--r--   0        0        0     5598 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/inheritance.rst
+-rw-r--r--   0        0        0     9934 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/intersphinx.rst
+-rw-r--r--   0        0        0     1756 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/linkcode.rst
+-rw-r--r--   0        0        0    11756 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/math.rst
+-rw-r--r--   0        0        0    15980 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/napoleon.rst
+-rw-r--r--   0        0        0     1644 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/todo.rst
+-rw-r--r--   0        0        0     3917 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/extensions/viewcode.rst
+-rw-r--r--   0        0        0      537 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/index.rst
+-rw-r--r--   0        0        0     7146 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/installation.rst
+-rw-r--r--   0        0        0     1584 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/markdown.rst
+-rw-r--r--   0        0        0    13150 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/quickstart.rst
+-rw-r--r--   0        0        0    20508 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/restructuredtext/basics.rst
+-rw-r--r--   0        0        0    46040 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/restructuredtext/directives.rst
+-rw-r--r--   0        0        0    69567 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/restructuredtext/domains.rst
+-rw-r--r--   0        0        0     1967 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/restructuredtext/field-lists.rst
+-rw-r--r--   0        0        0      574 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/restructuredtext/index.rst
+-rw-r--r--   0        0        0    18409 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/restructuredtext/roles.rst
+-rw-r--r--   0        0        0    14326 2023-09-13 23:12:58.893780 sphinx-7.2.6/doc/usage/theming.rst
+-rw-r--r--   0        0        0    15097 2023-09-13 23:12:58.897780 sphinx-7.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1852 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/__init__.py
+-rw-r--r--   0        0        0      127 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/__main__.py
+-rw-r--r--   0        0        0    19226 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/addnodes.py
+-rw-r--r--   0        0        0    56426 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/application.py
+-rw-r--r--   0        0        0    26942 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/__init__.py
+-rw-r--r--   0        0        0    28962 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/_epub_base.py
+-rw-r--r--   0        0        0     6531 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/changes.py
+-rw-r--r--   0        0        0     1542 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/dirhtml.py
+-rw-r--r--   0        0        0     1024 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/dummy.py
+-rw-r--r--   0        0        0    11439 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/epub3.py
+-rw-r--r--   0        0        0    11210 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/gettext.py
+-rw-r--r--   0        0        0    59513 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/html/__init__.py
+-rw-r--r--   0        0        0     5383 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/html/_assets.py
+-rw-r--r--   0        0        0     2563 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/html/transforms.py
+-rw-r--r--   0        0        0    24296 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/latex/__init__.py
+-rw-r--r--   0        0        0     7365 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/latex/constants.py
+-rw-r--r--   0        0        0      866 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/latex/nodes.py
+-rw-r--r--   0        0        0     4505 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/latex/theming.py
+-rw-r--r--   0        0        0    21041 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/latex/transforms.py
+-rw-r--r--   0        0        0     1703 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/latex/util.py
+-rw-r--r--   0        0        0    24526 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/linkcheck.py
+-rw-r--r--   0        0        0     4567 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/manpage.py
+-rw-r--r--   0        0        0     7781 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/singlehtml.py
+-rw-r--r--   0        0        0     9769 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/texinfo.py
+-rw-r--r--   0        0        0     2945 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/text.py
+-rw-r--r--   0        0        0     3848 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/builders/xml.py
+-rw-r--r--   0        0        0       44 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/cmd/__init__.py
+-rw-r--r--   0        0        0    13942 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/cmd/build.py
+-rw-r--r--   0        0        0     7125 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/cmd/make_mode.py
+-rw-r--r--   0        0        0    23959 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/cmd/quickstart.py
+-rw-r--r--   0        0        0    23017 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/config.py
+-rw-r--r--   0        0        0     1859 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/deprecation.py
+-rw-r--r--   0        0        0    15095 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/directives/__init__.py
+-rw-r--r--   0        0        0    18377 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/directives/code.py
+-rw-r--r--   0        0        0    16599 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/directives/other.py
+-rw-r--r--   0        0        0     6785 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/directives/patches.py
+-rw-r--r--   0        0        0    15376 2023-09-13 23:12:58.897780 sphinx-7.2.6/sphinx/domains/__init__.py
+-rw-r--r--   0        0        0   152243 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/c.py
+-rw-r--r--   0        0        0     5533 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/changeset.py
+-rw-r--r--   0        0        0     5681 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/citation.py
+-rw-r--r--   0        0        0   332914 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/cpp.py
+-rw-r--r--   0        0        0     4222 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/index.py
+-rw-r--r--   0        0        0    19405 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/javascript.py
+-rw-r--r--   0        0        0     5499 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/math.py
+-rw-r--r--   0        0        0    71297 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/python.py
+-rw-r--r--   0        0        0    10651 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/rst.py
+-rw-r--r--   0        0        0    46146 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/domains/std.py
+-rw-r--r--   0        0        0    31397 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/__init__.py
+-rw-r--r--   0        0        0       34 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/adapters/__init__.py
+-rw-r--r--   0        0        0      418 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/adapters/asset.py
+-rw-r--r--   0        0        0     7589 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/adapters/indexentries.py
+-rw-r--r--   0        0        0    18767 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/adapters/toctree.py
+-rw-r--r--   0        0        0     2791 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/collectors/__init__.py
+-rw-r--r--   0        0        0     6355 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/collectors/asset.py
+-rw-r--r--   0        0        0     1934 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/collectors/dependencies.py
+-rw-r--r--   0        0        0     2659 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/collectors/metadata.py
+-rw-r--r--   0        0        0     2186 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/collectors/title.py
+-rw-r--r--   0        0        0    15956 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/environment/collectors/toctree.py
+-rw-r--r--   0        0        0     3398 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/errors.py
+-rw-r--r--   0        0        0     4296 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/events.py
+-rw-r--r--   0        0        0       57 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/ext/__init__.py
+-rw-r--r--   0        0        0    20014 2023-09-13 23:12:58.901780 sphinx-7.2.6/sphinx/ext/apidoc.py
+-rw-r--r--   0        0        0   116526 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autodoc/__init__.py
+-rw-r--r--   0        0        0     6007 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autodoc/directive.py
+-rw-r--r--   0        0        0    12655 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autodoc/importer.py
+-rw-r--r--   0        0        0     5972 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autodoc/mock.py
+-rw-r--r--   0        0        0     7050 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autodoc/preserve_defaults.py
+-rw-r--r--   0        0        0     5366 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autodoc/type_comment.py
+-rw-r--r--   0        0        0     7859 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autodoc/typehints.py
+-rw-r--r--   0        0        0     2335 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autosectionlabel.py
+-rw-r--r--   0        0        0    31230 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autosummary/__init__.py
+-rw-r--r--   0        0        0    27531 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autosummary/generate.py
+-rw-r--r--   0        0        0      106 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autosummary/templates/autosummary/base.rst
+-rw-r--r--   0        0        0      553 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autosummary/templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1071 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/autosummary/templates/autosummary/module.rst
+-rw-r--r--   0        0        0    17527 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/coverage.py
+-rw-r--r--   0        0        0    23047 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/doctest.py
+-rw-r--r--   0        0        0     2892 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/duration.py
+-rw-r--r--   0        0        0     4629 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/extlinks.py
+-rw-r--r--   0        0        0     1994 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/githubpages.py
+-rw-r--r--   0        0        0    17614 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/graphviz.py
+-rw-r--r--   0        0        0     2564 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/ifconfig.py
+-rw-r--r--   0        0        0     3620 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/imgconverter.py
+-rw-r--r--   0        0        0    15421 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/imgmath.py
+-rw-r--r--   0        0        0    17604 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/inheritance_diagram.py
+-rw-r--r--   0        0        0    29181 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/intersphinx.py
+-rw-r--r--   0        0        0     2301 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/linkcode.py
+-rw-r--r--   0        0        0     5323 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/mathjax.py
+-rw-r--r--   0        0        0    17950 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/napoleon/__init__.py
+-rw-r--r--   0        0        0    48761 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/napoleon/docstring.py
+-rw-r--r--   0        0        0     8076 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/todo.py
+-rw-r--r--   0        0        0    13765 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/ext/viewcode.py
+-rw-r--r--   0        0        0     2999 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/extension.py
+-rw-r--r--   0        0        0     7211 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/highlighting.py
+-rw-r--r--   0        0        0     6165 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/io.py
+-rw-r--r--   0        0        0     7133 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/jinja2glue.py
+-rw-r--r--   0        0        0      165 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/locale/.tx/config
+-rw-r--r--   0        0        0     7282 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/locale/__init__.py
+-rw-r--r--   0        0        0     3494 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/locale/ar/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7494 2023-09-13 23:12:58.905780 sphinx-7.2.6/sphinx/locale/ar/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87441 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/ar/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/bg/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      492 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/bg/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84221 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/bg/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     5977 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/bn/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7591 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/bn/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88102 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/bn/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4029 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/ca/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    84364 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/ca/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   123494 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/ca/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2385 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/cak/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2391 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/cak/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84935 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/cak/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3976 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/cs/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7797 2023-09-13 23:12:58.909780 sphinx-7.2.6/sphinx/locale/cs/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86868 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/cs/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3411 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/cy/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     5686 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/cy/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86117 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/cy/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3578 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/da/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    12266 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/da/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88524 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/da/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3533 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/de/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    10680 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/de/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88190 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/de/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2303 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/de_DE/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      505 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/de_DE/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84234 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/de_DE/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     8758 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/el/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    80411 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/el/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   131575 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/el/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2303 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/en_DE/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      506 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/en_DE/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84235 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/en_DE/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2302 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      462 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/en_FR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84234 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3630 2023-09-13 23:12:58.913781 sphinx-7.2.6/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    75590 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   115380 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2303 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      508 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/en_HK/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84237 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2457 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/eo/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     1864 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/eo/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84717 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/eo/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4155 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/es/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    80907 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/es/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   121834 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/es/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2342 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/es_CO/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      546 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/es_CO/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84275 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/es_CO/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3615 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/et/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    32776 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/et/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    97621 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/et/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3102 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/eu/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6505 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/eu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86366 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/eu/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     7551 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/fa/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    97001 2023-09-13 23:12:58.917780 sphinx-7.2.6/sphinx/locale/fa/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   139238 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fa/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2787 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2912 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85021 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4162 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    83168 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   124747 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2354 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      555 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84284 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/gl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     4716 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/gl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86205 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/gl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4885 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/he/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     4822 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/he/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86002 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/he/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     7427 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    96953 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   146384 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2303 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      502 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84231 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3621 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    16384 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    90403 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3980 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hu/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    10971 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88513 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/hu/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3465 2023-09-13 23:12:58.921781 sphinx-7.2.6/sphinx/locale/id/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    60268 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/id/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   109906 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/id/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2825 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/is/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2614 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/is/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84925 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/is/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3579 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/it/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    10036 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/it/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87985 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/it/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4957 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ja/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    85691 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ja/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   128423 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ja/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6108 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ka/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    74059 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ka/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   131614 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ka/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4807 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ko/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    82285 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ko/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   122848 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/ko/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3473 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/lt/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6832 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/lt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86552 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/lt/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3445 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/lv/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6501 2023-09-13 23:12:58.925781 sphinx-7.2.6/sphinx/locale/lv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86258 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/lv/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2415 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/mk/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     2011 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/mk/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84911 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/mk/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3108 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6500 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86081 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6223 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ne/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8520 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ne/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88266 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ne/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3489 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/nl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    18611 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/nl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    91729 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/nl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3819 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    28827 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    96313 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2351 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      544 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84273 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4219 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    81014 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   121035 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3745 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     7764 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86914 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3700 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ro/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     8259 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ro/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87098 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ro/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     8165 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ru/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    15343 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ru/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    91964 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/ru/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3816 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/si/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     3560 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/si/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85703 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/si/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4117 2023-09-13 23:12:58.929781 sphinx-7.2.6/sphinx/locale/sk/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    66206 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sk/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   112993 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sk/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3185 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sl/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     5157 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    85764 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sl/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0    84206 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sphinx.pot
+-rw-r--r--   0        0        0     4216 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sq/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    79459 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sq/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   120806 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sq/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4100 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     9193 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    88349 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2380 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      584 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84313 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2382 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      579 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84308 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3281 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sv/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6491 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86103 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/sv/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/ta/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      647 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/ta/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84381 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/ta/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/te/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      489 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/te/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84218 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/te/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3937 2023-09-13 23:12:58.933781 sphinx-7.2.6/sphinx/locale/tr/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    56773 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/tr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   109376 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/tr/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     6283 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     6349 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    87075 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2300 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/ur/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      487 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/ur/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84216 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/ur/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3520 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/vi/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0     5771 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/vi/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    86217 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/vi/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2294 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/yue/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      487 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/yue/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84216 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/yue/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4318 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    75427 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   115775 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2301 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      501 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84230 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     2301 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0      516 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0    84245 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     4451 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js
+-rw-r--r--   0        0        0    74037 2023-09-13 23:12:58.937781 sphinx-7.2.6/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0        0        0   114591 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0     3121 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/parsers.py
+-rw-r--r--   0        0        0     4265 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/project.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/py.typed
+-rw-r--r--   0        0        0     5603 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/pycode/__init__.py
+-rw-r--r--   0        0        0     6352 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/pycode/ast.py
+-rw-r--r--   0        0        0    21521 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/pycode/parser.py
+-rw-r--r--   0        0        0     2861 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/pygments_styles.py
+-rw-r--r--   0        0        0    22436 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/registry.py
+-rw-r--r--   0        0        0    16098 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/roles.py
+-rw-r--r--   0        0        0    22113 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/__init__.py
+-rw-r--r--   0        0        0     3576 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/da.py
+-rw-r--r--   0        0        0     4652 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/de.py
+-rw-r--r--   0        0        0     4914 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/en.py
+-rw-r--r--   0        0        0     5738 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/es.py
+-rw-r--r--   0        0        0     3222 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/fi.py
+-rw-r--r--   0        0        0     3453 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/fr.py
+-rw-r--r--   0        0        0     1964 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/hu.py
+-rw-r--r--   0        0        0     5104 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/it.py
+-rw-r--r--   0        0        0    31012 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/ja.py
+-rw-r--r--   0        0        0     3594 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/base-stemmer.js
+-rw-r--r--   0        0        0     3123 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/danish-stemmer.js
+-rw-r--r--   0        0        0     5529 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/dutch-stemmer.js
+-rw-r--r--   0        0        0     7529 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/finnish-stemmer.js
+-rw-r--r--   0        0        0    11571 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/french-stemmer.js
+-rw-r--r--   0        0        0     4669 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/german-stemmer.js
+-rw-r--r--   0        0        0     6614 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/hungarian-stemmer.js
+-rw-r--r--   0        0        0     9100 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/italian-stemmer.js
+-rw-r--r--   0        0        0     2594 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/norwegian-stemmer.js
+-rw-r--r--   0        0        0     6439 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/porter-stemmer.js
+-rw-r--r--   0        0        0     8373 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/portuguese-stemmer.js
+-rw-r--r--   0        0        0     8333 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/romanian-stemmer.js
+-rw-r--r--   0        0        0     5735 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/russian-stemmer.js
+-rw-r--r--   0        0        0     9121 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/spanish-stemmer.js
+-rw-r--r--   0        0        0     2654 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/swedish-stemmer.js
+-rw-r--r--   0        0        0    19972 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/minified-js/turkish-stemmer.js
+-rw-r--r--   0        0        0     4586 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/nl.py
+-rw-r--r--   0        0        0     4908 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/no.py
+-rw-r--r--   0        0        0     8133 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/base-stemmer.js
+-rw-r--r--   0        0        0     8134 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/danish-stemmer.js
+-rw-r--r--   0        0        0    19495 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/dutch-stemmer.js
+-rw-r--r--   0        0        0    21286 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/finnish-stemmer.js
+-rw-r--r--   0        0        0    42080 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/french-stemmer.js
+-rw-r--r--   0        0        0    17647 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/german-stemmer.js
+-rw-r--r--   0        0        0    17564 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/hungarian-stemmer.js
+-rw-r--r--   0        0        0    29065 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/italian-stemmer.js
+-rw-r--r--   0        0        0     6870 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/norwegian-stemmer.js
+-rw-r--r--   0        0        0    20391 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/porter-stemmer.js
+-rw-r--r--   0        0        0    26718 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/portuguese-stemmer.js
+-rw-r--r--   0        0        0    25006 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/romanian-stemmer.js
+-rw-r--r--   0        0        0    17996 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/russian-stemmer.js
+-rw-r--r--   0        0        0    28534 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/spanish-stemmer.js
+-rw-r--r--   0        0        0     6851 2023-09-13 23:12:58.941781 sphinx-7.2.6/sphinx/search/non-minified-js/swedish-stemmer.js
+-rw-r--r--   0        0        0    77511 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/search/non-minified-js/turkish-stemmer.js
+-rw-r--r--   0        0        0     4663 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/search/pt.py
+-rw-r--r--   0        0        0      572 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/search/ro.py
+-rw-r--r--   0        0        0     7920 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/search/ru.py
+-rw-r--r--   0        0        0     3451 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/search/sv.py
+-rw-r--r--   0        0        0      566 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/search/tr.py
+-rw-r--r--   0        0        0     6161 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/search/zh.py
+-rw-r--r--   0        0        0      196 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/apidoc/module.rst_t
+-rw-r--r--   0        0        0     1173 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/apidoc/package.rst_t
+-rw-r--r--   0        0        0      128 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/apidoc/toc.rst_t
+-rw-r--r--   0        0        0      246 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/epub3/container.xml
+-rw-r--r--   0        0        0     2127 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/epub3/content.opf_t
+-rw-r--r--   0        0        0       20 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/epub3/mimetype
+-rw-r--r--   0        0        0      629 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/epub3/nav.xhtml_t
+-rw-r--r--   0        0        0      743 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/epub3/toc.ncx_t
+-rw-r--r--   0        0        0      875 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/gettext/message.pot_t
+-rw-r--r--   0        0        0      299 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/graphviz/graphviz.css
+-rw-r--r--   0        0        0      864 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/htmlhelp/project.hhc
+-rw-r--r--   0        0        0      570 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/htmlhelp/project.hhp
+-rw-r--r--   0        0        0      165 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/htmlhelp/project.stp
+-rw-r--r--   0        0        0      397 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/imgmath/preview.tex_t
+-rw-r--r--   0        0        0      321 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/imgmath/template.tex_t
+-rw-r--r--   0        0        0     2986 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/latex/latex.tex_t
+-rw-r--r--   0        0        0     2156 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/latex/longtable.tex_t
+-rw-r--r--   0        0        0      944 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/latex/sphinxmessages.sty_t
+-rw-r--r--   0        0        0     1406 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/latex/tabular.tex_t
+-rw-r--r--   0        0        0     1420 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/latex/tabulary.tex_t
+-rw-r--r--   0        0        0      656 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/quickstart/Makefile.new_t
+-rw-r--r--   0        0        0     4031 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/quickstart/Makefile_t
+-rw-r--r--   0        0        0     2129 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/quickstart/conf.py_t
+-rw-r--r--   0        0        0      787 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/quickstart/make.bat.new_t
+-rw-r--r--   0        0        0     3293 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/quickstart/make.bat_t
+-rw-r--r--   0        0        0      492 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/quickstart/root_doc.rst_t
+-rw-r--r--   0        0        0     1423 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/templates/texinfo/Makefile
+-rw-r--r--   0        0        0      171 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/testing/__init__.py
+-rw-r--r--   0        0        0     7142 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/testing/fixtures.py
+-rw-r--r--   0        0        0     6572 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/testing/path.py
+-rw-r--r--   0        0        0     1159 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/testing/restructuredtext.py
+-rw-r--r--   0        0        0     6375 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/testing/util.py
+-rw-r--r--   0        0        0     4366 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/LICRcyr2utf8.xdy
+-rw-r--r--   0        0        0    10188 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/LICRlatin2utf8.xdy
+-rw-r--r--   0        0        0    18890 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/LatinRules.xdy
+-rw-r--r--   0        0        0     2401 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/Makefile_t
+-rw-r--r--   0        0        0      695 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/latexmkjarc_t
+-rw-r--r--   0        0        0     1104 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/latexmkrc_t
+-rw-r--r--   0        0        0     1041 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/make.bat_t
+-rw-r--r--   0        0        0      392 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/python.ist
+-rw-r--r--   0        0        0    44560 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinx.sty
+-rw-r--r--   0        0        0     9474 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinx.xdy
+-rw-r--r--   0        0        0     3256 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxhowto.cls
+-rw-r--r--   0        0        0    10989 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexadmonitions.sty
+-rw-r--r--   0        0        0      901 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexcontainers.sty
+-rw-r--r--   0        0        0     4840 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexgraphics.sty
+-rw-r--r--   0        0        0     2066 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexindbibtoc.sty
+-rw-r--r--   0        0        0     5139 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexlists.sty
+-rw-r--r--   0        0        0    46048 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexliterals.sty
+-rw-r--r--   0        0        0     4532 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexnumfig.sty
+-rw-r--r--   0        0        0    14354 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexobjects.sty
+-rw-r--r--   0        0        0     5066 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexshadowbox.sty
+-rw-r--r--   0        0        0     3445 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexstyleheadings.sty
+-rw-r--r--   0        0        0     3064 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexstylepage.sty
+-rw-r--r--   0        0        0     8589 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatexstyletext.sty
+-rw-r--r--   0        0        0    57830 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxlatextables.sty
+-rw-r--r--   0        0        0     4241 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxmanual.cls
+-rw-r--r--   0        0        0     2061 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxoptionsgeometry.sty
+-rw-r--r--   0        0        0     1094 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxoptionshyperref.sty
+-rw-r--r--   0        0        0    36615 2023-09-13 23:12:58.945781 sphinx-7.2.6/sphinx/texinputs/sphinxpackageboxes.sty
+-rw-r--r--   0        0        0     2590 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/texinputs/sphinxpackagecyrillic.sty
+-rw-r--r--   0        0        0    15254 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/texinputs/sphinxpackagefootnote.sty
+-rw-r--r--   0        0        0     2503 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/texinputs_win/Makefile_t
+-rw-r--r--   0        0        0     3321 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/agogo/layout.html
+-rw-r--r--   0        0        0     9236 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/agogo/static/agogo.css_t
+-rw-r--r--   0        0        0      276 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/agogo/static/bgfooter.png
+-rw-r--r--   0        0        0      266 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/agogo/static/bgtop.png
+-rw-r--r--   0        0        0      477 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/agogo/theme.conf
+-rw-r--r--   0        0        0      466 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/changes/frameset.html
+-rw-r--r--   0        0        0      485 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/changes/rstsource.html
+-rw-r--r--   0        0        0     1306 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/changes/versionchanges.html
+-rw-r--r--   0        0        0     1636 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/defindex.html
+-rw-r--r--   0        0        0     1892 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/domainindex.html
+-rw-r--r--   0        0        0     1804 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/genindex-single.html
+-rw-r--r--   0        0        0     1210 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/genindex-split.html
+-rw-r--r--   0        0        0     2069 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/genindex.html
+-rw-r--r--   0        0        0      432 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/globaltoc.html
+-rw-r--r--   0        0        0     7673 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/layout.html
+-rw-r--r--   0        0        0      370 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/localtoc.html
+-rw-r--r--   0        0        0      679 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/opensearch.xml
+-rw-r--r--   0        0        0      273 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/page.html
+-rw-r--r--   0        0        0      652 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/relations.html
+-rw-r--r--   0        0        0     2039 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/search.html
+-rw-r--r--   0        0        0      809 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/searchbox.html
+-rw-r--r--   0        0        0      947 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/searchfield.html
+-rw-r--r--   0        0        0      544 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/sourcelink.html
+-rw-r--r--   0        0        0    15174 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/basic.css_t
+-rw-r--r--   0        0        0     4472 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/doctools.js
+-rw-r--r--   0        0        0      581 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/documentation_options.js_t
+-rw-r--r--   0        0        0      286 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/file.png
+-rw-r--r--   0        0        0      676 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/language_data.js_t
+-rw-r--r--   0        0        0       90 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/minus.png
+-rw-r--r--   0        0        0       90 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/plus.png
+-rw-r--r--   0        0        0    18732 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/searchtools.js
+-rw-r--r--   0        0        0     5123 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/static/sphinx_highlight.js
+-rw-r--r--   0        0        0      371 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/basic/theme.conf
+-rw-r--r--   0        0        0      664 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/bizstyle/layout.html
+-rw-r--r--   0        0        0       78 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/bizstyle/static/background_b01.png
+-rw-r--r--   0        0        0    10349 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/bizstyle/static/bizstyle.css_t
+-rw-r--r--   0        0        0     1129 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/bizstyle/static/bizstyle.js_t
+-rw-r--r--   0        0        0    14940 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/bizstyle/static/css3-mediaqueries.js
+-rw-r--r--   0        0        0    28634 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js
+-rw-r--r--   0        0        0      148 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/bizstyle/theme.conf
+-rw-r--r--   0        0        0      661 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/classic/layout.html
+-rw-r--r--   0        0        0     6635 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/classic/static/classic.css_t
+-rw-r--r--   0        0        0     2659 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/classic/static/sidebar.js_t
+-rw-r--r--   0        0        0      719 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/classic/theme.conf
+-rw-r--r--   0        0        0       28 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/default/static/default.css
+-rw-r--r--   0        0        0       26 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/default/theme.conf
+-rw-r--r--   0        0        0      693 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/epub/epub-cover.html
+-rw-r--r--   0        0        0      543 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/epub/layout.html
+-rw-r--r--   0        0        0    12435 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/epub/static/epub.css_t
+-rw-r--r--   0        0        0      108 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/epub/theme.conf
+-rw-r--r--   0        0        0     2012 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/haiku/layout.html
+-rw-r--r--   0        0        0     1128 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/haiku/static/alert_info_32.png
+-rw-r--r--   0        0        0      944 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/haiku/static/alert_warning_32.png
+-rw-r--r--   0        0        0       82 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/haiku/static/bg-page.png
+-rw-r--r--   0        0        0      165 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/haiku/static/bullet_orange.png
+-rw-r--r--   0        0        0     7059 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/haiku/static/haiku.css_t
+-rw-r--r--   0        0        0      298 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/haiku/theme.conf
+-rw-r--r--   0        0        0     4269 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/nature/static/nature.css_t
+-rw-r--r--   0        0        0       71 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/nature/theme.conf
+-rw-r--r--   0        0        0      642 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/nonav/layout.html
+-rw-r--r--   0        0        0     9692 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/nonav/static/nonav.css_t
+-rw-r--r--   0        0        0      109 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/nonav/theme.conf
+-rw-r--r--   0        0        0      875 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/layout.html
+-rw-r--r--   0        0        0     1394 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-note.png
+-rw-r--r--   0        0        0     1351 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-seealso.png
+-rw-r--r--   0        0        0     1186 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-todo.png
+-rw-r--r--   0        0        0     1798 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-topic.png
+-rw-r--r--   0        0        0     1280 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-warning.png
+-rw-r--r--   0        0        0     5629 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/epub.css_t
+-rw-r--r--   0        0        0      333 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/footerbg.png
+-rw-r--r--   0        0        0      190 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/headerbg.png
+-rw-r--r--   0        0        0      726 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/ie6.css
+-rw-r--r--   0        0        0      101 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/middlebg.png
+-rw-r--r--   0        0        0     6336 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/pyramid.css_t
+-rw-r--r--   0        0        0       49 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/static/transparent.gif
+-rw-r--r--   0        0        0      102 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/pyramid/theme.conf
+-rw-r--r--   0        0        0     5775 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/scrolls/artwork/logo.svg
+-rw-r--r--   0        0        0     1661 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/scrolls/layout.html
+-rw-r--r--   0        0        0    25238 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/scrolls/static/darkmetal.png
+-rw-r--r--   0        0        0      172 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/scrolls/static/headerbg.png
+-rw-r--r--   0        0        0     8305 2023-09-13 23:12:58.949781 sphinx-7.2.6/sphinx/themes/scrolls/static/logo.png
+-rw-r--r--   0        0        0     7547 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/scrolls/static/metal.png
+-rw-r--r--   0        0        0      124 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/scrolls/static/navigation.png
+-rw-r--r--   0        0        0      303 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/scrolls/static/print.css
+-rw-r--r--   0        0        0     8033 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/scrolls/static/scrolls.css_t
+-rw-r--r--   0        0        0      527 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/scrolls/static/theme_extras.js
+-rw-r--r--   0        0        0    44483 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/scrolls/static/watermark.png
+-rw-r--r--   0        0        0     8049 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/scrolls/static/watermark_blur.png
+-rw-r--r--   0        0        0      263 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/scrolls/theme.conf
+-rw-r--r--   0        0        0      107 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/sphinxdoc/static/contents.png
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/sphinxdoc/static/navigation.png
+-rw-r--r--   0        0        0     6349 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t
+-rw-r--r--   0        0        0       77 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/sphinxdoc/theme.conf
+-rw-r--r--   0        0        0    12162 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/traditional/static/traditional.css_t
+-rw-r--r--   0        0        0      105 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/themes/traditional/theme.conf
+-rw-r--r--   0        0        0     7994 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/theming.py
+-rw-r--r--   0        0        0    17741 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/transforms/__init__.py
+-rw-r--r--   0        0        0     2811 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/transforms/compact_bullet_list.py
+-rw-r--r--   0        0        0    26261 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/transforms/i18n.py
+-rw-r--r--   0        0        0    12616 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/transforms/post_transforms/__init__.py
+-rw-r--r--   0        0        0     4529 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/transforms/post_transforms/code.py
+-rw-r--r--   0        0        0    10408 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/transforms/post_transforms/images.py
+-rw-r--r--   0        0        0     1361 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/transforms/references.py
+-rw-r--r--   0        0        0    10212 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/__init__.py
+-rw-r--r--   0        0        0     4255 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/_pathlib.py
+-rw-r--r--   0        0        0      240 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/build_phase.py
+-rw-r--r--   0        0        0    15450 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/cfamily.py
+-rw-r--r--   0        0        0     3223 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/console.py
+-rw-r--r--   0        0        0     2710 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/display.py
+-rw-r--r--   0        0        0    16843 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/docfields.py
+-rw-r--r--   0        0        0     2944 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/docstrings.py
+-rw-r--r--   0        0        0    23193 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/docutils.py
+-rw-r--r--   0        0        0     1960 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/exceptions.py
+-rw-r--r--   0        0        0     3910 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/fileutil.py
+-rw-r--r--   0        0        0     1235 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/http_date.py
+-rw-r--r--   0        0        0     9580 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/i18n.py
+-rw-r--r--   0        0        0     3674 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/images.py
+-rw-r--r--   0        0        0      986 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/index_entries.py
+-rw-r--r--   0        0        0    29088 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/inspect.py
+-rw-r--r--   0        0        0     6347 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/inventory.py
+-rw-r--r--   0        0        0    18125 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/logging.py
+-rw-r--r--   0        0        0     5363 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/matching.py
+-rw-r--r--   0        0        0     1902 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/math.py
+-rw-r--r--   0        0        0    24408 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/nodes.py
+-rw-r--r--   0        0        0     6532 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/osutil.py
+-rw-r--r--   0        0        0     5088 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/parallel.py
+-rw-r--r--   0        0        0     1445 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/png.py
+-rw-r--r--   0        0        0     2428 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/requests.py
+-rw-r--r--   0        0        0     3398 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/rst.py
+-rw-r--r--   0        0        0     2770 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/tags.py
+-rw-r--r--   0        0        0     4954 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/template.py
+-rw-r--r--   0        0        0     5442 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/texescape.py
+-rw-r--r--   0        0        0    16646 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/util/typing.py
+-rw-r--r--   0        0        0     5849 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/versioning.py
+-rw-r--r--   0        0        0       31 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/writers/__init__.py
+-rw-r--r--   0        0        0     1603 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/writers/html.py
+-rw-r--r--   0        0        0    37346 2023-09-13 23:12:58.953781 sphinx-7.2.6/sphinx/writers/html5.py
+-rw-r--r--   0        0        0    90889 2023-09-13 23:12:58.957781 sphinx-7.2.6/sphinx/writers/latex.py
+-rw-r--r--   0        0        0    16007 2023-09-13 23:12:58.957781 sphinx-7.2.6/sphinx/writers/manpage.py
+-rw-r--r--   0        0        0    53237 2023-09-13 23:12:58.957781 sphinx-7.2.6/sphinx/writers/texinfo.py
+-rw-r--r--   0        0        0    43368 2023-09-13 23:12:58.957781 sphinx-7.2.6/sphinx/writers/text.py
+-rw-r--r--   0        0        0     1509 2023-09-13 23:12:58.957781 sphinx-7.2.6/sphinx/writers/xml.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/__init__.py
+-rw-r--r--   0        0        0     3054 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/certs/cert.pem
+-rw-r--r--   0        0        0     1036 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/conftest.py
+-rw-r--r--   0        0        0      363 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/ext_napoleon_pep526_data_google.py
+-rw-r--r--   0        0        0      385 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/ext_napoleon_pep526_data_numpy.py
+-rw-r--r--   0        0        0       34 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/js/documentation_options.js
+-rw-r--r--   0        0        0     1694 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/js/searchtools.js
+-rw-r--r--   0        0        0     1985 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/js/sphinx_highlight.js
+-rw-r--r--   0        0        0      111 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-add_enumerable_node/conf.py
+-rw-r--r--   0        0        0     1464 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-add_enumerable_node/enumerable_node.py
+-rw-r--r--   0        0        0      763 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-add_enumerable_node/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-add_enumerable_node/rimg.png
+-rw-r--r--   0        0        0      277 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-add_source_parser-conflicts-with-users-setting/conf.py
+-rw-r--r--   0        0        0      201 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-add_source_parser-conflicts-with-users-setting/source_parser.py
+-rw-r--r--   0        0        0      121 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-add_source_parser/conf.py
+-rw-r--r--   0        0        0      201 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-add_source_parser/source_parser.py
+-rw-r--r--   0        0        0     1659 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-api-set-translator/conf.py
+-rw-r--r--   0        0        0       72 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-api-set-translator/index.rst
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-api-set-translator/nonext/conf.py
+-rw-r--r--   0        0        0      101 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-api-set-translator/translator.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-duplicates/fish_licence/halibut.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-duplicates/fish_licence/halibut.pyx
+-rw-r--r--   0        0        0       12 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-pep420/a/b/c/__init__.py
+-rw-r--r--   0        0        0       11 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-pep420/a/b/c/d.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-pep420/a/b/e/__init__.py
+-rw-r--r--   0        0        0       11 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-pep420/a/b/e/f.py
+-rw-r--r--   0        0        0       11 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-pep420/a/b/x/y.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-subpackage-in-toc/parent/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-subpackage-in-toc/parent/child/__init__.py
+-rw-r--r--   0        0        0        6 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-subpackage-in-toc/parent/child/foo.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-toc/mypackage/__init__.py
+-rwxr-xr-x   0        0        0      404 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-toc/mypackage/main.py
+-rw-r--r--   0        0        0       79 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-toc/mypackage/no_init/foo.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-toc/mypackage/resource/__init__.py
+-rw-r--r--   0        0        0       96 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-toc/mypackage/resource/resource.txt
+-rw-r--r--   0        0        0       23 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-toc/mypackage/something/__init__.py
+-rw-r--r--   0        0        0       44 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-trailing-underscore/package_/__init__.py
+-rw-r--r--   0        0        0      215 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-apidoc-trailing-underscore/package_/module_.py
+-rw-r--r--   0        0        0      221 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-autosummary/conf.py
+-rw-r--r--   0        0        0     1335 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-autosummary/dummy_module.py
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-autosummary/index.rst
+-rw-r--r--   0        0        0      507 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-autosummary/sphinx.rst
+-rw-r--r--   0        0        0      198 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-autosummary/underscore_module_.py
+-rw-r--r--   0        0        0      114 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-basic/conf.py
+-rw-r--r--   0        0        0     1477 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-basic/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/extra.css
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/_static/mytheme.css
+-rw-r--r--   0        0        0       60 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-html-theme-having-multiple-stylesheets/_themes/mytheme/theme.conf
+-rw-r--r--   0        0        0       53 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-html-theme-having-multiple-stylesheets/conf.py
+-rw-r--r--   0        0        0      100 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-html-theme-having-multiple-stylesheets/index.rst
+-rw-r--r--   0        0        0      372 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-html-translator/conf.py
+-rw-r--r--   0        0        0      252 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-html-translator/index.rst
+-rw-r--r--   0        0        0       53 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/conf.py
+-rw-r--r--   0        0        0       20 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/doc1.txt
+-rw-r--r--   0        0        0       51 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/doc2.txt
+-rw-r--r--   0        0        0      135 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/index.txt
+-rw-r--r--   0        0        0       62 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/lineblock.txt
+-rw-r--r--   0        0        0       40 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/listitems.txt
+-rw-r--r--   0        0        0      388 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/maxwidth.txt
+-rw-r--r--   0        0        0      478 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/nonascii_maxwidth.txt
+-rw-r--r--   0        0        0       75 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/nonascii_table.txt
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/nonascii_title.txt
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/table.txt
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/table_colspan.txt
+-rw-r--r--   0        0        0      140 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/table_colspan_and_rowspan.txt
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/table_colspan_left.txt
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-build-text/table_rowspan.txt
+-rw-r--r--   0        0        0       18 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-dirhtml/bar.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-dirhtml/conf.py
+-rw-r--r--   0        0        0       32 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-dirhtml/foo/foo_1.rst
+-rw-r--r--   0        0        0       32 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-dirhtml/foo/foo_2.rst
+-rw-r--r--   0        0        0       63 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-dirhtml/foo/index.rst
+-rw-r--r--   0        0        0       59 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-dirhtml/index.rst
+-rw-r--r--   0        0        0       74 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-gettext-dont-rebuild-mo/bom.rst
+-rw-r--r--   0        0        0       16 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-gettext-dont-rebuild-mo/conf.py
+-rw-r--r--   0        0        0      108 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-gettext-dont-rebuild-mo/index.rst
+-rw-r--r--   0        0        0      264 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-builder-gettext-dont-rebuild-mo/xx/LC_MESSAGES/bom.po
+-rw-r--r--   0        0        0      330 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-changes/base.rst
+-rw-r--r--   0        0        0      371 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-changes/c-api.rst
+-rw-r--r--   0        0        0      134 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-changes/conf.py
+-rw-r--r--   0        0        0      189 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-changes/contents.rst
+-rw-r--r--   0        0        0      443 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-changes/library/utils.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-circular/conf.py
+-rw-r--r--   0        0        0       22 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-circular/index.rst
+-rw-r--r--   0        0        0       23 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-circular/sub.rst
+-rw-r--r--   0        0        0       81 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-config/conf.py
+-rw-r--r--   0        0        0      167 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-copyright-multiline/conf.py
+-rw-r--r--   0        0        0       75 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-copyright-multiline/index.rst
+-rw-r--r--   0        0        0       32 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-correct-year/conf.py
+-rw-r--r--   0        0        0       55 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-correct-year/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-default_role/conf.py
+-rw-r--r--   0        0        0       29 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-default_role/foo.rst
+-rw-r--r--   0        0        0       54 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-default_role/index.rst
+-rw-r--r--   0        0        0      762 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-directive-code/caption.rst
+-rw-r--r--   0        0        0      263 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-directive-code/classes.rst
+-rw-r--r--   0        0        0       44 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-directive-code/conf.py
+-rw-r--r--   0        0        0     1434 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-directive-code/dedent.rst
+-rw-r--r--   0        0        0      170 2023-09-13 23:12:58.957781 sphinx-7.2.6/tests/roots/test-directive-code/emphasize.rst
+-rw-r--r--   0        0        0        3 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/empty.inc
+-rw-r--r--   0        0        0       21 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/error.inc
+-rw-r--r--   0        0        0      203 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/force.rst
+-rw-r--r--   0        0        0      345 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/highlight.rst
+-rw-r--r--   0        0        0      267 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/index.rst
+-rw-r--r--   0        0        0      349 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/linenos.rst
+-rw-r--r--   0        0        0      396 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/linenothreshold.rst
+-rw-r--r--   0        0        0      206 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/literal-diff.inc
+-rw-r--r--   0        0        0       67 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/literal-short.inc
+-rw-r--r--   0        0        0      213 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/literal.inc
+-rw-r--r--   0        0        0      421 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/namedblocks.rst
+-rw-r--r--   0        0        0      263 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/py-decorators.inc
+-rw-r--r--   0        0        0      391 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/py-decorators.rst
+-rw-r--r--   0        0        0      305 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/python.rst
+-rw-r--r--   0        0        0      355 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-code/target.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-csv-table/conf.py
+-rw-r--r--   0        0        0       12 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-csv-table/example.csv
+-rw-r--r--   0        0        0       12 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-csv-table/subdir/example.csv
+-rw-r--r--   0        0        0       27 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-include/bar.txt
+-rw-r--r--   0        0        0       45 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-include/baz/baz.rst
+-rw-r--r--   0        0        0       65 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-include/conf.py
+-rw-r--r--   0        0        0       18 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-include/foo.rst
+-rw-r--r--   0        0        0       20 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-include/text.txt
+-rw-r--r--   0        0        0       62 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-only/conf.py
+-rw-r--r--   0        0        0       63 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-only/index.rst
+-rw-r--r--   0        0        0     3063 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directive-only/only.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directives-raw/conf.py
+-rw-r--r--   0        0        0      404 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-directives-raw/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-docutilsconf/conf.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-docutilsconf/docutils.conf
+-rw-r--r--   0        0        0       89 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-docutilsconf/index.rst
+-rw-r--r--   0        0        0       65 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c-c_maximum_signature_line_length/conf.py
+-rw-r--r--   0        0        0      119 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c-c_maximum_signature_line_length/index.rst
+-rw-r--r--   0        0        0       74 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c-intersphinx/conf.py
+-rw-r--r--   0        0        0     1146 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c-intersphinx/index.rst
+-rw-r--r--   0        0        0      121 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c/anon-dup-decl.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c/conf.py
+-rw-r--r--   0        0        0       70 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c/field-role.rst
+-rw-r--r--   0        0        0      101 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c/function_param_target.rst
+-rw-r--r--   0        0        0      785 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c/index.rst
+-rw-r--r--   0        0        0      261 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c/namespace.rst
+-rw-r--r--   0        0        0      163 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-c/ns_lookup.rst
+-rw-r--r--   0        0        0       67 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp-cpp_maximum_signature_line_length/conf.py
+-rw-r--r--   0        0        0      129 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp-cpp_maximum_signature_line_length/index.rst
+-rw-r--r--   0        0        0       74 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp-intersphinx/conf.py
+-rw-r--r--   0        0        0     2444 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp-intersphinx/index.rst
+-rw-r--r--   0        0        0       92 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/anon-dup-decl.rst
+-rw-r--r--   0        0        0      688 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/any-role.rst
+-rw-r--r--   0        0        0       27 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/backslash.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/conf.py
+-rw-r--r--   0        0        0       59 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/field-role.rst
+-rw-r--r--   0        0        0     1136 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/index.rst
+-rw-r--r--   0        0        0      133 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/lookup-key-overload.rst
+-rw-r--r--   0        0        0      437 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/multi-decl-lookup.rst
+-rw-r--r--   0        0        0     2136 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/roles-targets-ok.rst
+-rw-r--r--   0        0        0     2406 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/roles-targets-warn.rst
+-rw-r--r--   0        0        0      697 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/roles.rst
+-rw-r--r--   0        0        0       90 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/roles2.rst
+-rw-r--r--   0        0        0      383 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/semicolon.rst
+-rw-r--r--   0        0        0      203 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/warn-template-param-qualified-name.rst
+-rw-r--r--   0        0        0      249 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-cpp/xref_consistency.rst
+-rw-r--r--   0        0        0       45 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-js-javascript_maximum_signature_line_length/conf.py
+-rw-r--r--   0        0        0      156 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-js-javascript_maximum_signature_line_length/index.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-js/conf.py
+-rw-r--r--   0        0        0       66 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-js/index.rst
+-rw-r--r--   0        0        0      527 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-js/module.rst
+-rw-r--r--   0        0        0      886 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-js/roles.rst
+-rw-r--r--   0        0        0       41 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py-python_maximum_signature_line_length/conf.py
+-rw-r--r--   0        0        0      168 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py-python_maximum_signature_line_length/index.rst
+-rw-r--r--   0        0        0       41 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py-python_use_unqualified_type_names/conf.py
+-rw-r--r--   0        0        0      240 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py-python_use_unqualified_type_names/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py-xref-warning/conf.py
+-rw-r--r--   0        0        0      116 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py-xref-warning/index.rst
+-rw-r--r--   0        0        0      359 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py/abbr.rst
+-rw-r--r--   0        0        0      174 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py/canonical.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py/conf.py
+-rw-r--r--   0        0        0      107 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py/index.rst
+-rw-r--r--   0        0        0     1040 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py/module.rst
+-rw-r--r--   0        0        0      383 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py/module_option.rst
+-rw-r--r--   0        0        0      872 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-domain-py/roles.rst
+-rw-r--r--   0        0        0       24 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme1/theme.conf
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-double-inheriting-theme/base_themes_dir/base_theme2/theme.conf
+-rw-r--r--   0        0        0      127 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-double-inheriting-theme/conf.py
+-rw-r--r--   0        0        0       87 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-double-inheriting-theme/index.rst
+-rw-r--r--   0        0        0       40 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-environment-record-dependencies/api.rst
+-rw-r--r--   0        0        0       99 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-environment-record-dependencies/conf.py
+-rw-r--r--   0        0        0       38 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-environment-record-dependencies/example_module.py
+-rw-r--r--   0        0        0       22 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-environment-record-dependencies/index.rst
+-rw-r--r--   0        0        0       87 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-epub-anchor-id/conf.py
+-rw-r--r--   0        0        0      191 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-epub-anchor-id/index.rst
+-rw-r--r--   0        0        0      111 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/autodoc_dummy_bar.py
+-rw-r--r--   0        0        0       94 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/autodoc_dummy_module.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/bug2437/__init__.py
+-rw-r--r--   0        0        0       47 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/bug2437/autodoc_dummy_foo.py
+-rw-r--r--   0        0        0       40 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/circular_import/__init__.py
+-rw-r--r--   0        0        0        7 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/circular_import/a.py
+-rw-r--r--   0        0        0       82 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/circular_import/b.py
+-rw-r--r--   0        0        0       97 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/circular_import/c.py
+-rw-r--r--   0        0        0      215 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/conf.py
+-rw-r--r--   0        0        0      282 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/index.rst
+-rw-r--r--   0        0        0      301 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/TYPE_CHECKING.py
+-rw-r--r--   0        0        0     4363 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/__init__.py
+-rw-r--r--   0        0        0      187 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/_functions_to_import.py
+-rw-r--r--   0        0        0      428 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/abstractmethods.py
+-rw-r--r--   0        0        0      150 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/annotated.py
+-rw-r--r--   0        0        0      882 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/autoclass_content.py
+-rw-r--r--   0        0        0      665 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py
+-rw-r--r--   0        0        0      107 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/bound_method.py
+-rw-r--r--   0        0        0      219 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/cached_property.py
+-rw-r--r--   0        0        0      279 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/callable.py
+-rw-r--r--   0        0        0       47 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/canonical/__init__.py
+-rw-r--r--   0        0        0      158 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/canonical/original.py
+-rw-r--r--   0        0        0      684 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/classes.py
+-rw-r--r--   0        0        0      764 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/coroutine.py
+-rw-r--r--   0        0        0      245 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/cython.pyx
+-rw-r--r--   0        0        0      766 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/decorator.py
+-rw-r--r--   0        0        0      683 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/descriptor.py
+-rw-r--r--   0        0        0      643 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/docstring_signature.py
+-rw-r--r--   0        0        0      150 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/empty_all.py
+-rw-r--r--   0        0        0      384 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/enums.py
+-rw-r--r--   0        0        0      227 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/final.py
+-rw-r--r--   0        0        0      268 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/functions.py
+-rw-r--r--   0        0        0      278 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/generic_class.py
+-rw-r--r--   0        0        0      262 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/genericalias.py
+-rw-r--r--   0        0        0      260 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/hide_value.py
+-rw-r--r--   0        0        0       42 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/imported_members.py
+-rw-r--r--   0        0        0      458 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/inheritance.py
+-rw-r--r--   0        0        0      279 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/instance_variable.py
+-rw-r--r--   0        0        0      344 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/literal.py
+-rw-r--r--   0        0        0       52 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/metadata.py
+-rw-r--r--   0        0        0      422 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/methods.py
+-rw-r--r--   0        0        0      155 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/module.py
+-rw-r--r--   0        0        0       93 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/name_conflict/__init__.py
+-rw-r--r--   0        0        0       65 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/name_conflict/foo.py
+-rw-r--r--   0        0        0      169 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/name_mangling.py
+-rw-r--r--   0        0        0      894 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/need_mocks.py
+-rw-r--r--   0        0        0     1345 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/overload.py
+-rw-r--r--   0        0        0       59 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/overload2.py
+-rw-r--r--   0        0        0      207 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/partialfunction.py
+-rw-r--r--   0        0        0      420 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/partialmethod.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/pep570.py
+-rw-r--r--   0        0        0      292 2023-09-13 23:12:58.961781 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/pep604.py
+-rw-r--r--   0        0        0     1505 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/preserve_defaults.py
+-rw-r--r--   0        0        0      910 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/preserve_defaults_special_constructs.py
+-rw-r--r--   0        0        0      556 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/private.py
+-rw-r--r--   0        0        0       90 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/process_docstring.py
+-rw-r--r--   0        0        0      407 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/properties.py
+-rw-r--r--   0        0        0      705 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/singledispatch.py
+-rw-r--r--   0        0        0      628 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/singledispatchmethod.py
+-rw-r--r--   0        0        0      396 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/slots.py
+-rw-r--r--   0        0        0      168 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/sort_by_all.py
+-rw-r--r--   0        0        0      551 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/typed_vars.py
+-rw-r--r--   0        0        0     2107 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/typehints.py
+-rw-r--r--   0        0        0      461 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/typevar.py
+-rw-r--r--   0        0        0      123 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/uninitialized_attributes.py
+-rw-r--r--   0        0        0      372 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autodoc/target/wrappedfunction.py
+-rw-r--r--   0        0        0       85 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosectionlabel-prefix-document/conf.py
+-rw-r--r--   0        0        0      591 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst
+-rw-r--r--   0        0        0       45 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosectionlabel/conf.py
+-rw-r--r--   0        0        0      535 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosectionlabel/index.rst
+-rw-r--r--   0        0        0      294 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-filename-map/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      255 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-filename-map/conf.py
+-rw-r--r--   0        0        0      198 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-filename-map/index.rst
+-rw-r--r--   0        0        0       47 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/__init__.py
+-rw-r--r--   0        0        0       85 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-imported_members/autosummary_dummy_package/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      168 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-imported_members/conf.py
+-rw-r--r--   0        0        0      147 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-imported_members/index.rst
+-rw-r--r--   0        0        0      171 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-mock_imports/conf.py
+-rw-r--r--   0        0        0       72 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-mock_imports/foo.py
+-rw-r--r--   0        0        0      117 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-mock_imports/index.rst
+-rw-r--r--   0        0        0      241 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/__init__.py
+-rw-r--r--   0        0        0      201 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/autosummary_dummy_module.py
+-rw-r--r--   0        0        0      201 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-module_all/autosummary_dummy_package_all/extra_dummy_module.py
+-rw-r--r--   0        0        0      170 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-module_all/conf.py
+-rw-r--r--   0        0        0      154 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-module_all/index.rst
+-rw-r--r--   0        0        0      132 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/conf.py
+-rw-r--r--   0        0        0      174 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/package/__init__.py
+-rw-r--r--   0        0        0      147 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/package/module.py
+-rw-r--r--   0        0        0       63 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/package/module_importfail.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/package/package/__init__.py
+-rw-r--r--   0        0        0      147 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/package/package/module.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/package2/__init__.py
+-rw-r--r--   0        0        0      147 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-recursive/package2/module.py
+-rw-r--r--   0        0        0      404 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-skip-member/conf.py
+-rw-r--r--   0        0        0       54 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-skip-member/index.rst
+-rw-r--r--   0        0        0      264 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-skip-member/target.py
+-rw-r--r--   0        0        0        6 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-template/_templates/empty.rst
+-rw-r--r--   0        0        0      209 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-template/conf.py
+-rw-r--r--   0        0        0       78 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-template/index.rst
+-rw-r--r--   0        0        0       39 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary-template/target.py
+-rw-r--r--   0        0        0       22 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary/autosummary_class_module.py
+-rw-r--r--   0        0        0      232 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary/autosummary_dummy_inherited_module.py
+-rw-r--r--   0        0        0      932 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary/autosummary_dummy_module.py
+-rw-r--r--   0        0        0       63 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary/autosummary_importfail.py
+-rw-r--r--   0        0        0      190 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary/conf.py
+-rw-r--r--   0        0        0      499 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-autosummary/index.rst
+-rw-r--r--   0        0        0      242 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-coverage/conf.py
+-rw-r--r--   0        0        0      254 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-coverage/coverage_ignored.py
+-rw-r--r--   0        0        0      254 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-coverage/coverage_not_ignored.py
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-coverage/index.rst
+-rw-r--r--   0        0        0      371 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest-skipif/conf.py
+-rw-r--r--   0        0        0     2052 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest-skipif/skipif.txt
+-rw-r--r--   0        0        0      205 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest-with-autodoc/conf.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest-with-autodoc/dir/__init__.py
+-rw-r--r--   0        0        0       28 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest-with-autodoc/dir/bar.py
+-rw-r--r--   0        0        0       60 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest-with-autodoc/dir/inner.rst
+-rw-r--r--   0        0        0       25 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest-with-autodoc/foo.py
+-rw-r--r--   0        0        0       52 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest-with-autodoc/index.rst
+-rw-r--r--   0        0        0      148 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest/conf.py
+-rw-r--r--   0        0        0     2147 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-doctest/doctest.txt
+-rw-r--r--   0        0        0      190 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/conf.py
+-rw-r--r--   0        0        0      555 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst
+-rw-r--r--   0        0        0      161 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-extlinks-hardcoded-urls/conf.py
+-rw-r--r--   0        0        0      703 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst
+-rw-r--r--   0        0        0       40 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-githubpages/conf.py
+-rw-r--r--   0        0        0       25 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-githubpages/index.rst
+-rw-r--r--   0        0        0      187 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-graphviz/_static/images/test.svg
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-graphviz/conf.py
+-rw-r--r--   0        0        0       25 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-graphviz/graph.dot
+-rw-r--r--   0        0        0       25 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-graphviz/graph.xx.dot
+-rw-r--r--   0        0        0      641 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-graphviz/index.rst
+-rw-r--r--   0        0        0      256 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-ifconfig/conf.py
+-rw-r--r--   0        0        0      274 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-ifconfig/index.rst
+-rw-r--r--   0        0        0       41 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgconverter/conf.py
+-rw-r--r--   0        0        0   141783 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgconverter/img.pdf
+-rw-r--r--   0        0        0       86 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgconverter/index.rst
+-rw-r--r--   0        0        0      243 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgconverter/svgimg.svg
+-rw-r--r--   0        0        0      106 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgmockconverter/1/svgimg.svg
+-rw-r--r--   0        0        0      243 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgmockconverter/2/svgimg.svg
+-rw-r--r--   0        0        0       97 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgmockconverter/conf.py
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgmockconverter/index.rst
+-rw-r--r--   0        0        0      881 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py
+-rw-r--r--   0        0        0      138 2023-09-13 23:12:58.965782 sphinx-7.2.6/tests/roots/test-ext-inheritance_diagram/conf.py
+-rw-r--r--   0        0        0       13 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-inheritance_diagram/example/__init__.py
+-rw-r--r--   0        0        0       46 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-inheritance_diagram/example/sphinx.py
+-rw-r--r--   0        0        0       52 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-inheritance_diagram/external/other.py
+-rw-r--r--   0        0        0      354 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-inheritance_diagram/index.rst
+-rw-r--r--   0        0        0      264 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-inheritance_diagram/subdir/page1.rst
+-rw-r--r--   0        0        0      178 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-inheritance_diagram/subdir/page2.rst
+-rw-r--r--   0        0        0      198 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-inheritance_diagram/test.py
+-rw-r--r--   0        0        0       40 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-intersphinx-cppdomain/conf.py
+-rw-r--r--   0        0        0      150 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-intersphinx-cppdomain/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-intersphinx-role/conf.py
+-rw-r--r--   0        0        0     1211 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-intersphinx-role/index.rst
+-rw-r--r--   0        0        0      488 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math-compat/conf.py
+-rw-r--r--   0        0        0      199 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math-compat/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math-simple/conf.py
+-rw-r--r--   0        0        0       43 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math-simple/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math/conf.py
+-rw-r--r--   0        0        0      239 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math/index.rst
+-rw-r--r--   0        0        0      396 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math/math.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math/nomath.rst
+-rw-r--r--   0        0        0      128 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-math/page.rst
+-rw-r--r--   0        0        0      100 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-napoleon/conf.py
+-rw-r--r--   0        0        0       64 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-napoleon/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-napoleon/mypackage/__init__.py
+-rw-r--r--   0        0        0      194 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-napoleon/mypackage/typehints.py
+-rw-r--r--   0        0        0       70 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-napoleon/typehints.rst
+-rw-r--r--   0        0        0       31 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-todo/bar.rst
+-rw-r--r--   0        0        0       33 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-todo/conf.py
+-rw-r--r--   0        0        0      125 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-todo/foo.rst
+-rw-r--r--   0        0        0      109 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-todo/index.rst
+-rw-r--r--   0        0        0      108 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode-find/conf.py
+-rw-r--r--   0        0        0      636 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode-find/index.rst
+-rw-r--r--   0        0        0       37 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode-find/not_a_package/__init__.py
+-rw-r--r--   0        0        0      371 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode-find/not_a_package/submodule.py
+-rw-r--r--   0        0        0      745 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode/conf.py
+-rw-r--r--   0        0        0      550 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode/index.rst
+-rw-r--r--   0        0        0     3112 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode/objects.rst
+-rw-r--r--   0        0        0       64 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode/spam/__init__.py
+-rw-r--r--   0        0        0      308 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode/spam/mod1.py
+-rw-r--r--   0        0        0      188 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode/spam/mod2.py
+-rw-r--r--   0        0        0       52 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-ext-viewcode/spam/mod3.py
+-rw-r--r--   0        0        0       63 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-extensions/conf.py
+-rw-r--r--   0        0        0       70 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-extensions/read_parallel.py
+-rw-r--r--   0        0        0       71 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-extensions/read_serial.py
+-rw-r--r--   0        0        0       72 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-extensions/write_parallel.py
+-rw-r--r--   0        0        0       72 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-extensions/write_serial.py
+-rw-r--r--   0        0        0       70 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-footnotes/bar.rst
+-rw-r--r--   0        0        0       70 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-footnotes/baz.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-footnotes/conf.py
+-rw-r--r--   0        0        0     3386 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-footnotes/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-footnotes/rimg.png
+-rw-r--r--   0        0        0      143 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-gettext-template/_templates/template1.html
+-rw-r--r--   0        0        0      143 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-gettext-template/_templates/template2.html
+-rw-r--r--   0        0        0       32 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-gettext-template/conf.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-gettext-template/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-glossary/conf.py
+-rw-r--r--   0        0        0      260 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-glossary/index.rst
+-rw-r--r--   0        0        0      103 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-highlight_options/conf.py
+-rw-r--r--   0        0        0      166 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-highlight_options/index.rst
+-rw-r--r--   0        0        0      468 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/conf.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/extra/.htaccess
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/extra/.htpasswd
+-rw-r--r--   0        0        0       28 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/extra/API.html_t
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/extra/css/style.css
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/extra/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/extra/rimg.png
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/extra/subdir/.htaccess
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/extra/subdir/.htpasswd
+-rw-r--r--   0        0        0       65 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/.htaccess
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/.htpasswd
+-rw-r--r--   0        0        0       28 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/API.html_t
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/css/style.css
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/js/custom.js
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/rimg.png
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/subdir/.htaccess
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/static/subdir/.htpasswd
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/subdir/_build/index.html
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_assets/subdir/background.png
+-rw-r--r--   0        0        0       53 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_entity/conf.py
+-rw-r--r--   0        0        0      561 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_entity/index.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_file_checksum/conf.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_file_checksum/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_file_checksum/static/empty.js
+-rw-r--r--   0        0        0       13 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_file_checksum/static/script.js
+-rw-r--r--   0        0        0       19 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_file_checksum/static/stylesheet-a.css
+-rw-r--r--   0        0        0       19 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_file_checksum/static/stylesheet-b.css
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_scaled_image_link/conf.py
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_scaled_image_link/img.png
+-rw-r--r--   0        0        0      172 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_scaled_image_link/index.rst
+-rw-r--r--   0        0        0       36 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_signaturereturn_icon/conf.py
+-rw-r--r--   0        0        0      108 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_signaturereturn_icon/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_style/_static/default.css
+-rw-r--r--   0        0        0       58 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_style/conf.py
+-rw-r--r--   0        0        0       22 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-html_style/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-escape/conf.py
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-escape/img_#1.png
+-rw-r--r--   0        0        0      145 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-escape/index.rst
+-rw-r--r--   0        0        0      161 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-in-parsed-literal/conf.py
+-rw-r--r--   0        0        0      113 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-in-parsed-literal/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-in-parsed-literal/pic.png
+-rw-r--r--   0        0        0      143 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-in-section/conf.py
+-rw-r--r--   0        0        0      287 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-in-section/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-image-in-section/pic.png
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-images/conf.py
+-rw-r--r--   0        0        0    24976 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-images/img.gif
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.969781 sphinx-7.2.6/tests/roots/test-images/img.ja.png
+-rw-r--r--   0        0        0   141783 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/img.pdf
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/img.png
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/img.zh.png
+-rw-r--r--   0        0        0      466 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/rimg.png
+-rw-r--r--   0        0        0      218 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/rimg.png.xx
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/rimg.xx.png
+-rw-r--r--   0        0        0      128 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/subdir/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/subdir/rimg.png
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/subdir/rimg.xx.png
+-rw-r--r--   0        0        0   141783 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/subdir/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/subdir/svgimg.svg
+-rw-r--r--   0        0        0      243 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/subdir/svgimg.xx.svg
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-images/testimäge.png
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-index_on_title/conf.py
+-rw-r--r--   0        0        0      117 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-index_on_title/contents.rst
+-rw-r--r--   0        0        0       70 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/basic_diagram.rst
+-rw-r--r--   0        0        0      135 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/conf.py
+-rw-r--r--   0        0        0      166 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/diagram_module_w_2_top_classes.rst
+-rw-r--r--   0        0        0      125 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/diagram_w_1_top_class.rst
+-rw-r--r--   0        0        0      179 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/diagram_w_2_top_classes.rst
+-rw-r--r--   0        0        0      104 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/diagram_w_nested_classes.rst
+-rw-r--r--   0        0        0      118 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/diagram_w_parts.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/dummy/__init__.py
+-rw-r--r--   0        0        0      267 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/dummy/test.py
+-rw-r--r--   0        0        0       95 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/dummy/test_nested.py
+-rw-r--r--   0        0        0       31 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-inheritance/index.rst
+-rw-r--r--   0        0        0      216 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/_templates/contents.html
+-rw-r--r--   0        0        0      599 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/admonitions.txt
+-rw-r--r--   0        0        0       74 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/bom.txt
+-rw-r--r--   0        0        0      262 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/conf.py
+-rw-r--r--   0        0        0      342 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/definition_terms.txt
+-rw-r--r--   0        0        0      709 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/docfields.txt
+-rw-r--r--   0        0        0      858 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/external_links.txt
+-rw-r--r--   0        0        0      747 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/figure.txt
+-rw-r--r--   0        0        0      407 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/footnote.txt
+-rw-r--r--   0        0        0      378 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/glossary_terms.txt
+-rw-r--r--   0        0        0      151 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/glossary_terms_inconsistency.txt
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/i18n.png
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/img.png
+-rw-r--r--   0        0        0      563 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/index.txt
+-rw-r--r--   0        0        0      384 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/index_entries.txt
+-rw-r--r--   0        0        0     1832 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/label_target.txt
+-rw-r--r--   0        0        0      943 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/literalblock.txt
+-rw-r--r--   0        0        0      278 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/noqa.txt
+-rw-r--r--   0        0        0      128 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/only.txt
+-rw-r--r--   0        0        0       78 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/raw.txt
+-rw-r--r--   0        0        0     1094 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/refs.txt
+-rw-r--r--   0        0        0      291 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/refs_inconsistency.txt
+-rw-r--r--   0        0        0      252 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/refs_python_domain.txt
+-rw-r--r--   0        0        0      738 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/role_xref.txt
+-rw-r--r--   0        0        0      152 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/rubric.txt
+-rw-r--r--   0        0        0       97 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/section.txt
+-rw-r--r--   0        0        0      210 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/seealso.txt
+-rw-r--r--   0        0        0       32 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/subdir/index.txt
+-rw-r--r--   0        0        0      263 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/table.txt
+-rw-r--r--   0        0        0      139 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/toctree.txt
+-rw-r--r--   0        0        0      135 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/topic.txt
+-rw-r--r--   0        0        0      894 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/translation_progress.txt
+-rw-r--r--   0        0        0      337 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/versionchange.txt
+-rw-r--r--   0        0        0       79 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/warnings.txt
+-rw-r--r--   0        0        0     1513 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po
+-rw-r--r--   0        0        0      264 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/bom.po
+-rw-r--r--   0        0        0     1198 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po
+-rw-r--r--   0        0        0     1086 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po
+-rw-r--r--   0        0        0     1691 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po
+-rw-r--r--   0        0        0     1307 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/figure.po
+-rw-r--r--   0        0        0     1228 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po
+-rw-r--r--   0        0        0     1327 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po
+-rw-r--r--   0        0        0      754 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po
+-rw-r--r--   0        0        0      773 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     1318 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po
+-rw-r--r--   0        0        0     2159 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po
+-rw-r--r--   0        0        0     2211 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po
+-rw-r--r--   0        0        0     1380 2023-09-13 23:12:58.973782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po
+-rw-r--r--   0        0        0      723 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/only.po
+-rw-r--r--   0        0        0      644 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/raw.po
+-rw-r--r--   0        0        0     2771 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/refs.po
+-rw-r--r--   0        0        0     1045 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po
+-rw-r--r--   0        0        0      675 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po
+-rw-r--r--   0        0        0     1707 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po
+-rw-r--r--   0        0        0      744 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po
+-rw-r--r--   0        0        0      706 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/section.po
+-rw-r--r--   0        0        0      792 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po
+-rw-r--r--   0        0        0      621 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po
+-rw-r--r--   0        0        0      992 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/table.po
+-rw-r--r--   0        0        0      767 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po
+-rw-r--r--   0        0        0      750 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/topic.po
+-rw-r--r--   0        0        0     1744 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/translation_progress.po
+-rw-r--r--   0        0        0     1070 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po
+-rw-r--r--   0        0        0      710 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po
+-rw-r--r--   0        0        0      263 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/conf.py
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/i18n.png
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/img.png
+-rw-r--r--   0        0        0      163 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/index.rst
+-rw-r--r--   0        0        0      288 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/prolog_epilog_substitution.rst
+-rw-r--r--   0        0        0      188 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/prolog_epilog_substitution_excluded.rst
+-rw-r--r--   0        0        0     1135 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/xx/LC_MESSAGES/prolog_epilog_substitution.po
+-rw-r--r--   0        0        0       21 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-keep_warnings/conf.py
+-rw-r--r--   0        0        0       20 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-keep_warnings/index.rst
+-rw-r--r--   0        0        0       13 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-babel/bar.rst
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-babel/conf.py
+-rw-r--r--   0        0        0       13 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-babel/foo.rst
+-rw-r--r--   0        0        0       87 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-babel/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-container/conf.py
+-rw-r--r--   0        0        0       35 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-container/index.rst
+-rw-r--r--   0        0        0       59 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-equations/conf.py
+-rw-r--r--   0        0        0      256 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-equations/equations.rst
+-rw-r--r--   0        0        0      452 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-equations/expects/latex-equations.tex
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-figure-in-admonition/conf.py
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-figure-in-admonition/img.png
+-rw-r--r--   0        0        0      132 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-figure-in-admonition/index.rst
+-rw-r--r--   0        0        0     1573 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-includegraphics/conf.py
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-includegraphics/img.png
+-rw-r--r--   0        0        0      834 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-includegraphics/index.rst
+-rw-r--r--   0        0        0    34213 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-includegraphics/sphinx.png
+-rw-r--r--   0        0        0    38192 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-includegraphics/tall.png
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-index/conf.py
+-rw-r--r--   0        0        0      215 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-index/index.rst
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels-before-module/automodule1.py
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels-before-module/automodule2a.py
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels-before-module/automodule2b.py
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels-before-module/automodule3.py
+-rw-r--r--   0        0        0      117 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels-before-module/conf.py
+-rw-r--r--   0        0        0      464 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels-before-module/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels/conf.py
+-rw-r--r--   0        0        0      771 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels/index.rst
+-rw-r--r--   0        0        0       18 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-labels/otherdoc.rst
+-rw-r--r--   0        0        0      250 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-numfig/conf.py
+-rw-r--r--   0        0        0      112 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-numfig/index.rst
+-rw-r--r--   0        0        0      141 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-numfig/indexhowto.rst
+-rw-r--r--   0        0        0      165 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-numfig/indexmanual.rst
+-rw-r--r--   0        0        0       18 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/_mytemplates/latex/longtable.tex_t
+-rw-r--r--   0        0        0     1661 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/complex.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/conf.py
+-rw-r--r--   0        0        0     1933 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/complex_spanning_cell.tex
+-rw-r--r--   0        0        0     1752 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/gridtable.tex
+-rw-r--r--   0        0        0     1780 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex
+-rw-r--r--   0        0        0     1323 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable.tex
+-rw-r--r--   0        0        0     1300 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_align.tex
+-rw-r--r--   0        0        0     1445 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_caption.tex
+-rw-r--r--   0        0        0     1384 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex
+-rw-r--r--   0        0        0     1637 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex
+-rw-r--r--   0        0        0     1386 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex
+-rw-r--r--   0        0        0     1656 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_widths.tex
+-rw-r--r--   0        0        0     1409 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex
+-rw-r--r--   0        0        0     1341 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex
+-rw-r--r--   0        0        0      704 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/simple_table.tex
+-rw-r--r--   0        0        0      851 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_caption.tex
+-rw-r--r--   0        0        0      777 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex
+-rw-r--r--   0        0        0      978 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex
+-rw-r--r--   0        0        0      594 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex
+-rw-r--r--   0        0        0      779 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_verbatim.tex
+-rw-r--r--   0        0        0     1093 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_widths.tex
+-rw-r--r--   0        0        0      802 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex
+-rw-r--r--   0        0        0      733 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/tabular_having_widths.tex
+-rw-r--r--   0        0        0      747 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/tabularcolumn.tex
+-rw-r--r--   0        0        0      727 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/expects/tabulary_having_widths.tex
+-rw-r--r--   0        0        0       84 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/index.rst
+-rw-r--r--   0        0        0     2516 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/longtable.rst
+-rw-r--r--   0        0        0     2770 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-table/tabular.rst
+-rw-r--r--   0        0        0       52 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-theme/conf.py
+-rw-r--r--   0        0        0       24 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-theme/index.rst
+-rw-r--r--   0        0        0      117 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-theme/theme/custom/theme.conf
+-rw-r--r--   0        0        0      160 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-title/conf.py
+-rw-r--r--   0        0        0      165 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-title/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-unicode/conf.py
+-rw-r--r--   0        0        0      142 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-latex-unicode/index.rst
+-rw-r--r--   0        0        0       80 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-anchors-ignore-for-url/conf.py
+-rw-r--r--   0        0        0      532 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-anchors-ignore-for-url/index.rst
+-rw-r--r--   0        0        0       80 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-anchors-ignore/conf.py
+-rw-r--r--   0        0        0      109 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-anchors-ignore/index.rst
+-rw-r--r--   0        0        0      180 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-documents_exclude/br0ken_link.rst
+-rw-r--r--   0        0        0      174 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-documents_exclude/broken_link.rst
+-rw-r--r--   0        0        0      133 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-documents_exclude/conf.py
+-rw-r--r--   0        0        0       40 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-documents_exclude/index.rst
+-rw-r--r--   0        0        0       80 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-localserver-anchor/conf.py
+-rw-r--r--   0        0        0       48 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-localserver-anchor/index.rst
+-rw-r--r--   0        0        0       55 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-localserver-https/conf.py
+-rw-r--r--   0        0        0       42 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-localserver-https/index.rst
+-rw-r--r--   0        0        0       55 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-localserver-warn-redirects/conf.py
+-rw-r--r--   0        0        0       95 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-localserver-warn-redirects/index.rst
+-rw-r--r--   0        0        0       55 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-localserver/conf.py
+-rw-r--r--   0        0        0       41 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-localserver/index.rst
+-rw-r--r--   0        0        0       55 2023-09-13 23:12:58.977782 sphinx-7.2.6/tests/roots/test-linkcheck-raw-node/conf.py
+-rw-r--r--   0        0        0       46 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-linkcheck-raw-node/index.rst
+-rw-r--r--   0        0        0       80 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-linkcheck-too-many-retries/conf.py
+-rw-r--r--   0        0        0       73 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-linkcheck-too-many-retries/index.rst
+-rw-r--r--   0        0        0       99 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-linkcheck/conf.py
+-rw-r--r--   0        0        0      648 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-linkcheck/links.rst
+-rw-r--r--   0        0        0      143 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-local-logo/conf.py
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-local-logo/images/img.png
+-rw-r--r--   0        0        0     1477 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-local-logo/index.rst
+-rw-r--r--   0        0        0       80 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       41 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-locale/locale1/en/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       80 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       41 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-locale/locale1/et/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       82 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.mo
+-rw-r--r--   0        0        0       43 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-locale/locale2/en/LC_MESSAGES/myext.po
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-manpage_url/conf.py
+-rw-r--r--   0        0        0       61 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-manpage_url/index.rst
+-rw-r--r--   0        0        0      114 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-markup-citation/conf.py
+-rw-r--r--   0        0        0      166 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-markup-citation/index.rst
+-rw-r--r--   0        0        0      114 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-markup-rubric/conf.py
+-rw-r--r--   0        0        0      112 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-markup-rubric/index.rst
+-rw-r--r--   0        0        0       78 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-maxlistdepth/conf.py
+-rw-r--r--   0        0        0      687 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-maxlistdepth/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-metadata/conf.py
+-rw-r--r--   0        0        0     1436 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-metadata/index.rst
+-rw-r--r--   0        0        0        8 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-need-escaped/bar.rst
+-rw-r--r--   0        0        0        8 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-need-escaped/baz.rst
+-rw-r--r--   0        0        0       62 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-need-escaped/conf.py
+-rw-r--r--   0        0        0       82 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-need-escaped/foo.rst
+-rw-r--r--   0        0        0      574 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-need-escaped/index.rst
+-rw-r--r--   0        0        0       10 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-need-escaped/quux.rst
+-rw-r--r--   0        0        0       29 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-need-escaped/qux.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-nested-enumerated-list/conf.py
+-rw-r--r--   0        0        0      300 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-nested-enumerated-list/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-nested-tables/conf.py
+-rw-r--r--   0        0        0      248 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-nested-tables/index.rst
+-rw-r--r--   0        0        0       16 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-nitpicky-warnings/conf.py
+-rw-r--r--   0        0        0      176 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-nitpicky-warnings/index.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numbered-circular/conf.py
+-rw-r--r--   0        0        0       36 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numbered-circular/index.rst
+-rw-r--r--   0        0        0       23 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numbered-circular/sub.rst
+-rw-r--r--   0        0        0      710 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numfig/bar.rst
+-rw-r--r--   0        0        0      259 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numfig/baz.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numfig/conf.py
+-rw-r--r--   0        0        0      912 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numfig/foo.rst
+-rw-r--r--   0        0        0     1024 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numfig/index.rst
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-numfig/rimg.png
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-object-description-sections/conf.py
+-rw-r--r--   0        0        0       80 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-object-description-sections/index.rst
+-rw-r--r--   0        0        0       73 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/Bare.rst
+-rw-r--r--   0        0        0       58 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/Dup1.rst
+-rw-r--r--   0        0        0       58 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/Dup2.rst
+-rw-r--r--   0        0        0       94 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/LineContinuation.rst
+-rw-r--r--   0        0        0       72 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/P1.rst
+-rw-r--r--   0        0        0       72 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/P2.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/conf.py
+-rw-r--r--   0        0        0       97 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/firstLineRule.rst
+-rw-r--r--   0        0        0      663 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-productionlist/index.rst
+-rw-r--r--   0        0        0      177 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-prolog/conf.py
+-rw-r--r--   0        0        0       83 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-prolog/index.rst
+-rw-r--r--   0        0        0       57 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-prolog/markdown.md
+-rw-r--r--   0        0        0      299 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-prolog/prolog_markdown_parser.py
+-rw-r--r--   0        0        0       67 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-prolog/restructuredtext.rst
+-rw-r--r--   0        0        0       75 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-pycode/cp_1251_coded.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-reST-code-block/conf.py
+-rw-r--r--   0        0        0       97 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-reST-code-block/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-reST-code-role/conf.py
+-rw-r--r--   0        0        0      194 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-reST-code-role/index.rst
+-rw-r--r--   0        0        0       27 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-refonly_bullet_list/conf.py
+-rw-r--r--   0        0        0      147 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-refonly_bullet_list/index.rst
+-rw-r--r--   0        0        0      237 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-remote-logo/conf.py
+-rw-r--r--   0        0        0     1477 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-remote-logo/index.rst
+-rw-r--r--   0        0        0       32 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-roles-download/another/dummy.dat
+-rw-r--r--   0        0        0      114 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-roles-download/conf.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-roles-download/dummy.dat
+-rw-r--r--   0        0        0      214 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-roles-download/index.rst
+-rw-r--r--   0        0        0     2111 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/Makefile
+-rw-r--r--   0        0        0       67 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/_templates/contentssb.html
+-rw-r--r--   0        0        0       99 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/_templates/customsb.html
+-rw-r--r--   0        0        0      428 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/_templates/layout.html
+-rw-r--r--   0        0        0      578 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/autodoc.txt
+-rw-r--r--   0        0        0     4587 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/autodoc_target.py
+-rw-r--r--   0        0        0       74 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/bom.txt
+-rw-r--r--   0        0        0     4257 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/conf.py
+-rw-r--r--   0        0        0       87 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/extapi.txt
+-rw-r--r--   0        0        0      365 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/extensions.txt
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/file_with_special_#_chars.xyz
+-rw-r--r--   0        0        0      826 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/footnote.txt
+-rw-r--r--   0        0        0      575 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/images.txt
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/img.foo.png
+-rw-r--r--   0        0        0    24976 2023-09-13 23:12:58.981782 sphinx-7.2.6/tests/roots/test-root/img.gif
+-rw-r--r--   0        0        0   141783 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/img.pdf
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/img.png
+-rw-r--r--   0        0        0     2108 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/includes.txt
+-rw-r--r--   0        0        0     1118 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/index.txt
+-rw-r--r--   0        0        0      750 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/lists.txt
+-rw-r--r--   0        0        0      200 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/literal.inc
+-rw-r--r--   0        0        0      208 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/literal_orig.inc
+-rw-r--r--   0        0        0     6902 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/markup.txt
+-rw-r--r--   0        0        0      373 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/math.txt
+-rw-r--r--   0        0        0     4608 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/objects.txt
+-rw-r--r--   0        0        0      110 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/otherext.foo
+-rw-r--r--   0        0        0      346 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/parsermod.py
+-rw-r--r--   0        0        0       45 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/quotes.inc
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/rimg.png
+-rw-r--r--   0        0        0       87 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/special/api.h
+-rw-r--r--   0        0        0       32 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/special/code.py
+-rw-r--r--   0        0        0       96 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/subdir/excluded.txt
+-rw-r--r--   0        0        0      106 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/subdir/images.txt
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/subdir/img.png
+-rw-r--r--   0        0        0      143 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/subdir/include.inc
+-rw-r--r--   0        0        0      328 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/subdir/includes.txt
+-rw-r--r--   0        0        0    66247 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/subdir/simg.png
+-rw-r--r--   0        0        0   141783 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/svgimg.svg
+-rw-r--r--   0        0        0       78 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/tabs.inc
+-rw-r--r--   0        0        0       77 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/test.inc
+-rw-r--r--   0        0        0      107 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-root/wrongenc.inc
+-rw-r--r--   0        0        0       58 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-search/conf.py
+-rw-r--r--   0        0        0      381 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-search/index.rst
+-rw-r--r--   0        0        0       41 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-search/nosearch.rst
+-rw-r--r--   0        0        0      184 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-search/tocitem.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-smartquotes/conf.py
+-rw-r--r--   0        0        0      107 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-smartquotes/index.rst
+-rw-r--r--   0        0        0      231 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-smartquotes/literals.rst
+-rw-r--r--   0        0        0      453 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-stylesheets/_templates/layout.html
+-rw-r--r--   0        0        0      318 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-stylesheets/conf.py
+-rw-r--r--   0        0        0       53 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-stylesheets/index.rst
+-rw-r--r--   0        0        0      182 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-templating/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0      109 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-templating/_templates/layout.html
+-rw-r--r--   0        0        0      135 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-templating/autosummary_templating.txt
+-rw-r--r--   0        0        0      266 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-templating/conf.py
+-rw-r--r--   0        0        0      124 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-templating/index.txt
+-rw-r--r--   0        0        0      661 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/child.zip
+-rw-r--r--   0        0        0       94 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/conf.py
+-rw-r--r--   0        0        0       26 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/index.rst
+-rw-r--r--   0        0        0     1039 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/parent.zip
+-rw-r--r--   0        0        0       82 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/test_theme/__init__.py
+-rw-r--r--   0        0        0      139 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/test_theme/staticfiles/layout.html
+-rw-r--r--   0        0        0      120 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/test_theme/staticfiles/static/staticimg.png
+-rw-r--r--   0        0        0       82 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/test_theme/staticfiles/static/statictmpl.html_t
+-rw-r--r--   0        0        0      104 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/test_theme/staticfiles/theme.conf
+-rw-r--r--   0        0        0       98 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/test_theme/test-theme/theme.conf
+-rw-r--r--   0        0        0     1039 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-theming/ziptheme.zip
+-rw-r--r--   0        0        0      150 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-tocdepth/bar.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-tocdepth/baz.rst
+-rw-r--r--   0        0        0       53 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-tocdepth/conf.py
+-rw-r--r--   0        0        0      146 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-tocdepth/foo.rst
+-rw-r--r--   0        0        0       71 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-tocdepth/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-domain-objects/conf.py
+-rw-r--r--   0        0        0      731 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-domain-objects/domains.rst
+-rw-r--r--   0        0        0       90 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-domain-objects/index.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-duplicated/conf.py
+-rw-r--r--   0        0        0        8 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-duplicated/foo.rst
+-rw-r--r--   0        0        0       77 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-duplicated/index.rst
+-rw-r--r--   0        0        0      101 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-empty/_templates/localtoc.html
+-rw-r--r--   0        0        0       62 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-empty/conf.py
+-rw-r--r--   0        0        0       52 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-empty/index.rst
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/bar/bar_1.rst
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/bar/bar_2.rst
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/bar/bar_3.rst
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/bar/bar_4/index.rst
+-rw-r--r--   0        0        0       53 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/bar/index.rst
+-rw-r--r--   0        0        0       13 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/baz.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/conf.py
+-rw-r--r--   0        0        0       13 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/foo.rst
+-rw-r--r--   0        0        0      303 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/index.rst
+-rw-r--r--   0        0        0       16 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/quux.rst
+-rw-r--r--   0        0        0       50 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/qux/index.rst
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/qux/qux_1.rst
+-rw-r--r--   0        0        0       17 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-glob/qux/qux_2.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-index/conf.py
+-rw-r--r--   0        0        0      105 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-index/foo.rst
+-rw-r--r--   0        0        0      132 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-index/index.rst
+-rw-r--r--   0        0        0      150 2023-09-13 23:12:58.985782 sphinx-7.2.6/tests/roots/test-toctree-maxdepth/bar.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree-maxdepth/baz.rst
+-rw-r--r--   0        0        0       30 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree-maxdepth/conf.py
+-rw-r--r--   0        0        0      146 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree-maxdepth/foo.rst
+-rw-r--r--   0        0        0      105 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree-maxdepth/index.rst
+-rw-r--r--   0        0        0      105 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree-maxdepth/qux.rst
+-rw-r--r--   0        0        0        8 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree/bar.rst
+-rw-r--r--   0        0        0        8 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree/baz.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree/conf.py
+-rw-r--r--   0        0        0       74 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree/foo.rst
+-rw-r--r--   0        0        0      885 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree/index.rst
+-rw-r--r--   0        0        0       10 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree/quux.rst
+-rw-r--r--   0        0        0       29 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree/qux.rst
+-rw-r--r--   0        0        0       97 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-toctree/tocdepth.rst
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-transforms-post_transforms-keyboard/conf.py
+-rw-r--r--   0        0        0       94 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-transforms-post_transforms-keyboard/index.rst
+-rw-r--r--   0        0        0       16 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-transforms-post_transforms-missing-reference/conf.py
+-rw-r--r--   0        0        0      113 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-transforms-post_transforms-missing-reference/index.rst
+-rw-r--r--   0        0        0       36 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-trim_doctest_flags/conf.py
+-rw-r--r--   0        0        0      784 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-trim_doctest_flags/index.rst
+-rw-r--r--   0        0        0     1012 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/added.txt
+-rw-r--r--   0        0        0       86 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/conf.py
+-rw-r--r--   0        0        0      584 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/deleted.txt
+-rw-r--r--   0        0        0      490 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/deleted_end.txt
+-rw-r--r--   0        0        0      164 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/index.txt
+-rw-r--r--   0        0        0      864 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/insert.txt
+-rw-r--r--   0        0        0      850 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/insert_beginning.txt
+-rw-r--r--   0        0        0      735 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/insert_similar.txt
+-rw-r--r--   0        0        0      867 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/modified.txt
+-rw-r--r--   0        0        0      715 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-versioning/original.txt
+-rw-r--r--   0        0        0      151 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-warnings/autodoc_fodder.py
+-rw-r--r--   0        0        0       97 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-warnings/conf.py
+-rw-r--r--   0        0        0      698 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-warnings/index.rst
+-rw-r--r--   0        0        0   141783 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-warnings/svgimg.pdf
+-rw-r--r--   0        0        0      243 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-warnings/svgimg.svg
+-rw-r--r--   0        0        0       18 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-warnings/undecodable.rst
+-rw-r--r--   0        0        0      107 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/roots/test-warnings/wrongenc.inc
+-rw-r--r--   0        0        0     1918 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_addnodes.py
+-rw-r--r--   0        0        0     3309 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_api_translator.py
+-rw-r--r--   0        0        0     5494 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_application.py
+-rw-r--r--   0        0        0     4719 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build.py
+-rw-r--r--   0        0        0     1152 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_changes.py
+-rw-r--r--   0        0        0     1407 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_dirhtml.py
+-rw-r--r--   0        0        0    16652 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_epub.py
+-rw-r--r--   0        0        0     7839 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_gettext.py
+-rw-r--r--   0        0        0    82944 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_html.py
+-rw-r--r--   0        0        0    76628 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_latex.py
+-rw-r--r--   0        0        0    34191 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_linkcheck.py
+-rw-r--r--   0        0        0     2785 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_manpage.py
+-rw-r--r--   0        0        0     5925 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_texinfo.py
+-rw-r--r--   0        0        0     8996 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_build_text.py
+-rw-r--r--   0        0        0     1322 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_builder.py
+-rw-r--r--   0        0        0     2729 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_catalogs.py
+-rw-r--r--   0        0        0    18197 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_config.py
+-rw-r--r--   0        0        0      811 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_correct_year.py
+-rw-r--r--   0        0        0    22630 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_directive_code.py
+-rw-r--r--   0        0        0     2088 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_directive_object_description.py
+-rw-r--r--   0        0        0     1655 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_directive_only.py
+-rw-r--r--   0        0        0     6912 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_directive_other.py
+-rw-r--r--   0        0        0     4362 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_directive_patch.py
+-rw-r--r--   0        0        0     5542 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_directives_no_typesetting.py
+-rw-r--r--   0        0        0     1084 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_docutilsconf.py
+-rw-r--r--   0        0        0    37517 2023-09-13 23:12:58.989782 sphinx-7.2.6/tests/test_domain_c.py
+-rw-r--r--   0        0        0    76152 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_domain_cpp.py
+-rw-r--r--   0        0        0    20323 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_domain_js.py
+-rw-r--r--   0        0        0    99015 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_domain_py.py
+-rw-r--r--   0        0        0     5904 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_domain_rst.py
+-rw-r--r--   0        0        0    19424 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_domain_std.py
+-rw-r--r--   0        0        0     5298 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_environment.py
+-rw-r--r--   0        0        0     8068 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_environment_indexentries.py
+-rw-r--r--   0        0        0      310 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_environment_record_dependencies.py
+-rw-r--r--   0        0        0    20386 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_environment_toctree.py
+-rw-r--r--   0        0        0      321 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_errors.py
+-rw-r--r--   0        0        0     1826 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_events.py
+-rw-r--r--   0        0        0    23586 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_apidoc.py
+-rw-r--r--   0        0        0    79346 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc.py
+-rw-r--r--   0        0        0     4801 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_autoattribute.py
+-rw-r--r--   0        0        0    14302 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_autoclass.py
+-rw-r--r--   0        0        0     2631 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_autodata.py
+-rw-r--r--   0        0        0     5647 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_autofunction.py
+-rw-r--r--   0        0        0     5355 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_automodule.py
+-rw-r--r--   0        0        0     2501 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_autoproperty.py
+-rw-r--r--   0        0        0    55422 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_configs.py
+-rw-r--r--   0        0        0     3335 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_events.py
+-rw-r--r--   0        0        0     3979 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_mock.py
+-rw-r--r--   0        0        0     6143 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_preserve_defaults.py
+-rw-r--r--   0        0        0     4415 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autodoc_private_members.py
+-rw-r--r--   0        0        0     3145 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autosectionlabel.py
+-rw-r--r--   0        0        0    28028 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_autosummary.py
+-rw-r--r--   0        0        0     3575 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_coverage.py
+-rw-r--r--   0        0        0     5511 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_doctest.py
+-rw-r--r--   0        0        0      378 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_duration.py
+-rw-r--r--   0        0        0     2104 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_extlinks.py
+-rw-r--r--   0        0        0      958 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_githubpages.py
+-rw-r--r--   0        0        0     8462 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_graphviz.py
+-rw-r--r--   0        0        0      850 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_ifconfig.py
+-rw-r--r--   0        0        0     1038 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_imgconverter.py
+-rw-r--r--   0        0        0      609 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_imgmockconverter.py
+-rw-r--r--   0        0        0    13984 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_inheritance_diagram.py
+-rw-r--r--   0        0        0    21302 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_intersphinx.py
+-rw-r--r--   0        0        0    14083 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_math.py
+-rw-r--r--   0        0        0     7094 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_napoleon.py
+-rw-r--r--   0        0        0    70640 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_napoleon_docstring.py
+-rw-r--r--   0        0        0     3878 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_todo.py
+-rw-r--r--   0        0        0     5617 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_ext_viewcode.py
+-rw-r--r--   0        0        0      857 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_extension.py
+-rw-r--r--   0        0        0     3599 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_highlighting.py
+-rw-r--r--   0        0        0    53684 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_intl.py
+-rw-r--r--   0        0        0     2551 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_locale.py
+-rw-r--r--   0        0        0    22386 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_markup.py
+-rw-r--r--   0        0        0     1931 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_metadata.py
+-rw-r--r--   0        0        0     2459 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_parser.py
+-rw-r--r--   0        0        0     2790 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_project.py
+-rw-r--r--   0        0        0     6923 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_pycode.py
+-rw-r--r--   0        0        0     2840 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_pycode_ast.py
+-rw-r--r--   0        0        0    18264 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_pycode_parser.py
+-rw-r--r--   0        0        0     7422 2023-09-13 23:12:58.993782 sphinx-7.2.6/tests/test_quickstart.py
+-rw-r--r--   0        0        0     2570 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_roles.py
+-rw-r--r--   0        0        0    11736 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_search.py
+-rw-r--r--   0        0        0     3747 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_smartquotes.py
+-rw-r--r--   0        0        0     1435 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_templating.py
+-rw-r--r--   0        0        0     4795 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_theming.py
+-rw-r--r--   0        0        0     1843 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_toctree.py
+-rw-r--r--   0        0        0     2517 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_transforms_move_module_targets.py
+-rw-r--r--   0        0        0    11587 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_transforms_post_transforms.py
+-rw-r--r--   0        0        0     1324 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_transforms_post_transforms_code.py
+-rw-r--r--   0        0        0     4169 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_transforms_reorder_nodes.py
+-rw-r--r--   0        0        0     2850 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util.py
+-rw-r--r--   0        0        0     3203 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_display.py
+-rw-r--r--   0        0        0     3032 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_docstrings.py
+-rw-r--r--   0        0        0     2647 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_docutils.py
+-rw-r--r--   0        0        0     4000 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_fileutil.py
+-rw-r--r--   0        0        0     8704 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_i18n.py
+-rw-r--r--   0        0        0     2713 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_images.py
+-rw-r--r--   0        0        0    29622 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_inspect.py
+-rw-r--r--   0        0        0     4057 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_inventory.py
+-rw-r--r--   0        0        0    13533 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_logging.py
+-rw-r--r--   0        0        0     7180 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_matching.py
+-rw-r--r--   0        0        0     7482 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_nodes.py
+-rw-r--r--   0        0        0     7333 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_rst.py
+-rw-r--r--   0        0        0      952 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_template.py
+-rw-r--r--   0        0        0    28601 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_util_typing.py
+-rw-r--r--   0        0        0     3581 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_versioning.py
+-rw-r--r--   0        0        0     1110 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/test_writer_latex.py
+-rw-r--r--   0        0        0     1887 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/typing_test_data.py
+-rw-r--r--   0        0        0     1663 2023-09-13 23:12:58.997782 sphinx-7.2.6/tests/utils.py
+-rw-r--r--   0        0        0      994 2023-09-13 23:12:58.997782 sphinx-7.2.6/tox.ini
+-rw-r--r--   0        0        0      226 2023-09-13 23:12:58.997782 sphinx-7.2.6/utils/CHANGES_template
+-rw-r--r--   0        0        0        0 2023-09-13 23:12:58.997782 sphinx-7.2.6/utils/__init__.py
+-rw-r--r--   0        0        0     8368 2023-09-13 23:12:58.997782 sphinx-7.2.6/utils/babel_runner.py
+-rw-r--r--   0        0        0     1646 2023-09-13 23:12:58.997782 sphinx-7.2.6/utils/bump_docker.py
+-rwxr-xr-x   0        0        0     5812 2023-09-13 23:12:58.997782 sphinx-7.2.6/utils/bump_version.py
+-rw-r--r--   0        0        0     1697 2023-09-13 23:12:58.997782 sphinx-7.2.6/utils/release-checklist
+-rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 sphinx-7.2.6/PKG-INFO
```

### Comparing `sphinx-7.2.5/AUTHORS` & `sphinx-7.2.6/AUTHORS`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/CHANGES` & `sphinx-7.2.6/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Release 7.2.6 (released Sep 13, 2023)
+=====================================
+
+Bugs fixed
+----------
+
+* #11679: Add the :envvar:`!SPHINX_AUTODOC_RELOAD_MODULES` environment variable,
+  which if set reloads modules when using autodoc with ``TYPE_CHECKING = True``.
+  Patch by Matt Wozniski and Adam Turner.
+* #11679: Use :py:func:`importlib.reload` to reload modules in autodoc.
+  Patch by Matt Wozniski and Adam Turner.
+
 Release 7.2.5 (released Aug 30, 2023)
 =====================================
 
 Bugs fixed
 ----------
 
 * #11645: Fix a regression preventing autodoc from importing modules within
```

### Comparing `sphinx-7.2.5/CODE_OF_CONDUCT` & `sphinx-7.2.6/CODE_OF_CONDUCT`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/EXAMPLES` & `sphinx-7.2.6/EXAMPLES`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/LICENSE` & `sphinx-7.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/README.rst` & `sphinx-7.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/Makefile` & `sphinx-7.2.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/bookcover.png` & `sphinx-7.2.6/doc/_static/bookcover.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/conf.py.txt` & `sphinx-7.2.6/doc/_static/conf.py.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/favicon.svg` & `sphinx-7.2.6/doc/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/more.png` & `sphinx-7.2.6/doc/_static/more.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/sphinx.png` & `sphinx-7.2.6/doc/_static/sphinx.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/agogo.png` & `sphinx-7.2.6/doc/_static/themes/agogo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/alabaster.png` & `sphinx-7.2.6/doc/_static/themes/alabaster.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/bizstyle.png` & `sphinx-7.2.6/doc/_static/themes/bizstyle.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/classic.png` & `sphinx-7.2.6/doc/_static/themes/classic.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/agogo.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/agogo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/alabaster.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/alabaster.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/bizstyle.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/bizstyle.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/classic.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/classic.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/haiku.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/haiku.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/nature.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/nature.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/pyramid.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/pyramid.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/scrolls.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/scrolls.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/sphinx_rtd_theme.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/sphinx_rtd_theme.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/sphinxdoc.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/sphinxdoc.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/fullsize/traditional.png` & `sphinx-7.2.6/doc/_static/themes/fullsize/traditional.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/haiku.png` & `sphinx-7.2.6/doc/_static/themes/haiku.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/nature.png` & `sphinx-7.2.6/doc/_static/themes/nature.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/pyramid.png` & `sphinx-7.2.6/doc/_static/themes/pyramid.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/scrolls.png` & `sphinx-7.2.6/doc/_static/themes/scrolls.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/sphinx_rtd_theme.png` & `sphinx-7.2.6/doc/_static/themes/sphinx_rtd_theme.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/sphinxdoc.png` & `sphinx-7.2.6/doc/_static/themes/sphinxdoc.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/themes/traditional.png` & `sphinx-7.2.6/doc/_static/themes/traditional.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/translation.png` & `sphinx-7.2.6/doc/_static/translation.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/translation.svg` & `sphinx-7.2.6/doc/_static/translation.svg`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/tutorial/lumache-autosummary.png` & `sphinx-7.2.6/doc/_static/tutorial/lumache-autosummary.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/tutorial/lumache-first-light.png` & `sphinx-7.2.6/doc/_static/tutorial/lumache-first-light.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/tutorial/lumache-furo.png` & `sphinx-7.2.6/doc/_static/tutorial/lumache-furo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/tutorial/lumache-py-function-full.png` & `sphinx-7.2.6/doc/_static/tutorial/lumache-py-function-full.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_static/tutorial/lumache-py-function.png` & `sphinx-7.2.6/doc/_static/tutorial/lumache-py-function.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_themes/sphinx13/layout.html` & `sphinx-7.2.6/doc/_themes/sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_themes/sphinx13/static/sphinx13.css` & `sphinx-7.2.6/doc/_themes/sphinx13/static/sphinx13.css`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/_themes/sphinx13/static/sphinxheader.png` & `sphinx-7.2.6/doc/_themes/sphinx13/static/sphinxheader.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/conf.py` & `sphinx-7.2.6/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import os
 import re
 import time
 
 import sphinx
 
+os.environ['SPHINX_AUTODOC_RELOAD_MODULES'] = '1'
+
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest', 'sphinx.ext.todo',
               'sphinx.ext.autosummary', 'sphinx.ext.extlinks',
               'sphinx.ext.intersphinx',
               'sphinx.ext.viewcode', 'sphinx.ext.inheritance_diagram',
               'sphinx.ext.coverage']
 coverage_statistics_to_report = coverage_statistics_to_stdout = True
 templates_path = ['_templates']
```

### Comparing `sphinx-7.2.5/doc/development/builders.rst` & `sphinx-7.2.6/doc/development/builders.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/index.rst` & `sphinx-7.2.6/doc/development/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/overview.rst` & `sphinx-7.2.6/doc/development/overview.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/templating.rst` & `sphinx-7.2.6/doc/development/templating.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/theming.rst` & `sphinx-7.2.6/doc/development/theming.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/tutorials/autodoc_ext.rst` & `sphinx-7.2.6/doc/development/tutorials/autodoc_ext.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/tutorials/examples/autodoc_intenum.py` & `sphinx-7.2.6/doc/development/tutorials/examples/autodoc_intenum.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/tutorials/examples/recipe.py` & `sphinx-7.2.6/doc/development/tutorials/examples/recipe.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/tutorials/examples/todo.py` & `sphinx-7.2.6/doc/development/tutorials/examples/todo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/tutorials/helloworld.rst` & `sphinx-7.2.6/doc/development/tutorials/helloworld.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/tutorials/recipe.rst` & `sphinx-7.2.6/doc/development/tutorials/recipe.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/development/tutorials/todo.rst` & `sphinx-7.2.6/doc/development/tutorials/todo.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/appapi.rst` & `sphinx-7.2.6/doc/extdev/appapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/builderapi.rst` & `sphinx-7.2.6/doc/extdev/builderapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/deprecated.rst` & `sphinx-7.2.6/doc/extdev/deprecated.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/domainapi.rst` & `sphinx-7.2.6/doc/extdev/domainapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/envapi.rst` & `sphinx-7.2.6/doc/extdev/envapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/i18n.rst` & `sphinx-7.2.6/doc/extdev/i18n.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/index.rst` & `sphinx-7.2.6/doc/extdev/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/logging.rst` & `sphinx-7.2.6/doc/extdev/logging.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/markupapi.rst` & `sphinx-7.2.6/doc/extdev/markupapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/nodes.rst` & `sphinx-7.2.6/doc/extdev/nodes.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/parserapi.rst` & `sphinx-7.2.6/doc/extdev/parserapi.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/extdev/utils.rst` & `sphinx-7.2.6/doc/extdev/utils.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/faq.rst` & `sphinx-7.2.6/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/glossary.rst` & `sphinx-7.2.6/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/index.rst` & `sphinx-7.2.6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/internals/contributing.rst` & `sphinx-7.2.6/doc/internals/contributing.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/internals/organization.rst` & `sphinx-7.2.6/doc/internals/organization.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/internals/release-process.rst` & `sphinx-7.2.6/doc/internals/release-process.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/latex.rst` & `sphinx-7.2.6/doc/latex.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/make.bat` & `sphinx-7.2.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/man/sphinx-apidoc.rst` & `sphinx-7.2.6/doc/man/sphinx-apidoc.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/man/sphinx-autogen.rst` & `sphinx-7.2.6/doc/man/sphinx-autogen.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/man/sphinx-build.rst` & `sphinx-7.2.6/doc/man/sphinx-build.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/man/sphinx-quickstart.rst` & `sphinx-7.2.6/doc/man/sphinx-quickstart.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/support.rst` & `sphinx-7.2.6/doc/support.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/tutorial/automatic-doc-generation.rst` & `sphinx-7.2.6/doc/tutorial/automatic-doc-generation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/tutorial/deploying.rst` & `sphinx-7.2.6/doc/tutorial/deploying.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/tutorial/describing-code.rst` & `sphinx-7.2.6/doc/tutorial/describing-code.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/tutorial/first-steps.rst` & `sphinx-7.2.6/doc/tutorial/first-steps.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/tutorial/getting-started.rst` & `sphinx-7.2.6/doc/tutorial/getting-started.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/tutorial/index.rst` & `sphinx-7.2.6/doc/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/tutorial/more-sphinx-customization.rst` & `sphinx-7.2.6/doc/tutorial/more-sphinx-customization.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/tutorial/narrative-documentation.rst` & `sphinx-7.2.6/doc/tutorial/narrative-documentation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/advanced/intl.rst` & `sphinx-7.2.6/doc/usage/advanced/intl.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/advanced/websupport/api.rst` & `sphinx-7.2.6/doc/usage/advanced/websupport/api.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/advanced/websupport/quickstart.rst` & `sphinx-7.2.6/doc/usage/advanced/websupport/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/advanced/websupport/searchadapters.rst` & `sphinx-7.2.6/doc/usage/advanced/websupport/searchadapters.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/advanced/websupport/storagebackends.rst` & `sphinx-7.2.6/doc/usage/advanced/websupport/storagebackends.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/builders/index.rst` & `sphinx-7.2.6/doc/usage/builders/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/configuration.rst` & `sphinx-7.2.6/doc/usage/configuration.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/autodoc.rst` & `sphinx-7.2.6/doc/usage/extensions/autodoc.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/autosectionlabel.rst` & `sphinx-7.2.6/doc/usage/extensions/autosectionlabel.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/autosummary.rst` & `sphinx-7.2.6/doc/usage/extensions/autosummary.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/coverage.rst` & `sphinx-7.2.6/doc/usage/extensions/coverage.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/doctest.rst` & `sphinx-7.2.6/doc/usage/extensions/doctest.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/example_google.py` & `sphinx-7.2.6/doc/usage/extensions/example_google.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/example_numpy.py` & `sphinx-7.2.6/doc/usage/extensions/example_numpy.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/extlinks.rst` & `sphinx-7.2.6/doc/usage/extensions/extlinks.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/graphviz.rst` & `sphinx-7.2.6/doc/usage/extensions/graphviz.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/ifconfig.rst` & `sphinx-7.2.6/doc/usage/extensions/ifconfig.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/imgconverter.rst` & `sphinx-7.2.6/doc/usage/extensions/imgconverter.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/index.rst` & `sphinx-7.2.6/doc/usage/extensions/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/inheritance.rst` & `sphinx-7.2.6/doc/usage/extensions/inheritance.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/intersphinx.rst` & `sphinx-7.2.6/doc/usage/extensions/intersphinx.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/linkcode.rst` & `sphinx-7.2.6/doc/usage/extensions/linkcode.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/math.rst` & `sphinx-7.2.6/doc/usage/extensions/math.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/napoleon.rst` & `sphinx-7.2.6/doc/usage/extensions/napoleon.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/todo.rst` & `sphinx-7.2.6/doc/usage/extensions/todo.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/extensions/viewcode.rst` & `sphinx-7.2.6/doc/usage/extensions/viewcode.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/index.rst` & `sphinx-7.2.6/doc/usage/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/installation.rst` & `sphinx-7.2.6/doc/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/markdown.rst` & `sphinx-7.2.6/doc/usage/markdown.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/quickstart.rst` & `sphinx-7.2.6/doc/usage/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/restructuredtext/basics.rst` & `sphinx-7.2.6/doc/usage/restructuredtext/basics.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/restructuredtext/directives.rst` & `sphinx-7.2.6/doc/usage/restructuredtext/directives.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/restructuredtext/domains.rst` & `sphinx-7.2.6/doc/usage/restructuredtext/domains.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/restructuredtext/field-lists.rst` & `sphinx-7.2.6/doc/usage/restructuredtext/field-lists.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/restructuredtext/index.rst` & `sphinx-7.2.6/doc/usage/restructuredtext/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/restructuredtext/roles.rst` & `sphinx-7.2.6/doc/usage/restructuredtext/roles.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/doc/usage/theming.rst` & `sphinx-7.2.6/doc/usage/theming.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/pyproject.toml` & `sphinx-7.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/__init__.py` & `sphinx-7.2.6/sphinx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,26 +15,26 @@
     warnings.filterwarnings('default', category=RemovedInNextVersionWarning)
 # docutils.io using mode='rU' for open
 warnings.filterwarnings('ignore', "'U' mode is deprecated",
                         DeprecationWarning, module='docutils.io')
 warnings.filterwarnings('ignore', 'The frontend.Option class .*',
                         DeprecationWarning, module='docutils.frontend')
 
-__version__ = '7.2.5'
+__version__ = '7.2.6'
 __display_version__ = __version__  # used for command line version
 
 #: Version info for better programmatic use.
 #:
 #: A tuple of five elements; for Sphinx version 1.2.1 beta 3 this would be
 #: ``(1, 2, 1, 'beta', 3)``. The fourth element can be one of: ``alpha``,
 #: ``beta``, ``rc``, ``final``. ``final`` always has 0 as the last element.
 #:
 #: .. versionadded:: 1.2
 #:    Before version 1.2, check the string ``sphinx.__version__``.
-version_info = (7, 2, 5, 'final', 0)
+version_info = (7, 2, 6, 'final', 0)
 
 package_dir = path.abspath(path.dirname(__file__))
 
 _in_development = False
 if _in_development:
     # Only import subprocess if needed
     import subprocess
```

### Comparing `sphinx-7.2.5/sphinx/addnodes.py` & `sphinx-7.2.6/sphinx/addnodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/application.py` & `sphinx-7.2.6/sphinx/application.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/__init__.py` & `sphinx-7.2.6/sphinx/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/_epub_base.py` & `sphinx-7.2.6/sphinx/builders/_epub_base.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/changes.py` & `sphinx-7.2.6/sphinx/builders/changes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/dirhtml.py` & `sphinx-7.2.6/sphinx/builders/dirhtml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/dummy.py` & `sphinx-7.2.6/sphinx/builders/dummy.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/epub3.py` & `sphinx-7.2.6/sphinx/builders/epub3.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/gettext.py` & `sphinx-7.2.6/sphinx/builders/gettext.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/html/__init__.py` & `sphinx-7.2.6/sphinx/builders/html/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/html/_assets.py` & `sphinx-7.2.6/sphinx/builders/html/_assets.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/html/transforms.py` & `sphinx-7.2.6/sphinx/builders/html/transforms.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/latex/__init__.py` & `sphinx-7.2.6/sphinx/builders/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/latex/constants.py` & `sphinx-7.2.6/sphinx/builders/latex/constants.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/latex/nodes.py` & `sphinx-7.2.6/sphinx/builders/latex/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/latex/theming.py` & `sphinx-7.2.6/sphinx/builders/latex/theming.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/latex/transforms.py` & `sphinx-7.2.6/sphinx/builders/latex/transforms.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/latex/util.py` & `sphinx-7.2.6/sphinx/builders/latex/util.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/linkcheck.py` & `sphinx-7.2.6/sphinx/builders/linkcheck.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/manpage.py` & `sphinx-7.2.6/sphinx/builders/manpage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/singlehtml.py` & `sphinx-7.2.6/sphinx/builders/singlehtml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/texinfo.py` & `sphinx-7.2.6/sphinx/builders/texinfo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/text.py` & `sphinx-7.2.6/sphinx/builders/text.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/builders/xml.py` & `sphinx-7.2.6/sphinx/builders/xml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/cmd/build.py` & `sphinx-7.2.6/sphinx/cmd/build.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/cmd/make_mode.py` & `sphinx-7.2.6/sphinx/cmd/make_mode.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 
 
 class Make:
     def __init__(self, srcdir: str, builddir: str, opts: Sequence[str]) -> None:
         self.srcdir = srcdir
         self.builddir = builddir
         self.opts = [*opts]
-        self.makecmd = os.environ.get('MAKE', 'make')  # refer $MAKE to determine make command
 
     def builddir_join(self, *comps: str) -> str:
         return path.join(self.builddir, *comps)
 
     def build_clean(self) -> int:
         srcdir = path.abspath(self.srcdir)
         builddir = path.abspath(self.builddir)
@@ -101,48 +100,55 @@
             if not osname or os.name == osname:
                 print(f'  {blue(bname.ljust(10))}  {description}')
 
     def build_latexpdf(self) -> int:
         if self.run_generic_build('latex') > 0:
             return 1
 
-        if sys.platform == 'win32':
-            makecmd = os.environ.get('MAKE', 'make.bat')
-        else:
-            makecmd = self.makecmd
+        # Use $MAKE to determine the make command
+        make_fallback = 'make.bat' if sys.platform == 'win32' else 'make'
+        makecmd = os.environ.get('MAKE', make_fallback)
+        if not makecmd.lower().startswith('make'):
+            raise RuntimeError('Invalid $MAKE command: %r' % makecmd)
         try:
             with chdir(self.builddir_join('latex')):
                 return subprocess.call([makecmd, 'all-pdf'])
         except OSError:
             print('Error: Failed to run: %s' % makecmd)
             return 1
 
     def build_latexpdfja(self) -> int:
         if self.run_generic_build('latex') > 0:
             return 1
 
-        if sys.platform == 'win32':
-            makecmd = os.environ.get('MAKE', 'make.bat')
-        else:
-            makecmd = self.makecmd
+        # Use $MAKE to determine the make command
+        make_fallback = 'make.bat' if sys.platform == 'win32' else 'make'
+        makecmd = os.environ.get('MAKE', make_fallback)
+        if not makecmd.lower().startswith('make'):
+            raise RuntimeError('Invalid $MAKE command: %r' % makecmd)
         try:
             with chdir(self.builddir_join('latex')):
                 return subprocess.call([makecmd, 'all-pdf'])
         except OSError:
             print('Error: Failed to run: %s' % makecmd)
             return 1
 
     def build_info(self) -> int:
         if self.run_generic_build('texinfo') > 0:
             return 1
+
+        # Use $MAKE to determine the make command
+        makecmd = os.environ.get('MAKE', 'make')
+        if not makecmd.lower().startswith('make'):
+            raise RuntimeError('Invalid $MAKE command: %r' % makecmd)
         try:
             with chdir(self.builddir_join('texinfo')):
-                return subprocess.call([self.makecmd, 'info'])
+                return subprocess.call([makecmd, 'info'])
         except OSError:
-            print('Error: Failed to run: %s' % self.makecmd)
+            print('Error: Failed to run: %s' % makecmd)
             return 1
 
     def build_gettext(self) -> int:
         dtdir = self.builddir_join('gettext', '.doctrees')
         if self.run_generic_build('gettext', doctreedir=dtdir) > 0:
             return 1
         return 0
```

### Comparing `sphinx-7.2.5/sphinx/cmd/quickstart.py` & `sphinx-7.2.6/sphinx/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/config.py` & `sphinx-7.2.6/sphinx/config.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/deprecation.py` & `sphinx-7.2.6/sphinx/deprecation.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/directives/__init__.py` & `sphinx-7.2.6/sphinx/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/directives/code.py` & `sphinx-7.2.6/sphinx/directives/code.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/directives/other.py` & `sphinx-7.2.6/sphinx/directives/other.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/directives/patches.py` & `sphinx-7.2.6/sphinx/directives/patches.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/__init__.py` & `sphinx-7.2.6/sphinx/domains/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/c.py` & `sphinx-7.2.6/sphinx/domains/c.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/changeset.py` & `sphinx-7.2.6/sphinx/domains/changeset.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/citation.py` & `sphinx-7.2.6/sphinx/domains/citation.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/cpp.py` & `sphinx-7.2.6/sphinx/domains/cpp.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/index.py` & `sphinx-7.2.6/sphinx/domains/index.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/javascript.py` & `sphinx-7.2.6/sphinx/domains/javascript.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/math.py` & `sphinx-7.2.6/sphinx/domains/math.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/python.py` & `sphinx-7.2.6/sphinx/domains/python.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/rst.py` & `sphinx-7.2.6/sphinx/domains/rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/domains/std.py` & `sphinx-7.2.6/sphinx/domains/std.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/__init__.py` & `sphinx-7.2.6/sphinx/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/adapters/indexentries.py` & `sphinx-7.2.6/sphinx/environment/adapters/indexentries.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/adapters/toctree.py` & `sphinx-7.2.6/sphinx/environment/adapters/toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/collectors/__init__.py` & `sphinx-7.2.6/sphinx/environment/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/collectors/asset.py` & `sphinx-7.2.6/sphinx/environment/collectors/asset.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/collectors/dependencies.py` & `sphinx-7.2.6/sphinx/environment/collectors/dependencies.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/collectors/metadata.py` & `sphinx-7.2.6/sphinx/environment/collectors/metadata.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/collectors/title.py` & `sphinx-7.2.6/sphinx/environment/collectors/title.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/environment/collectors/toctree.py` & `sphinx-7.2.6/sphinx/environment/collectors/toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/errors.py` & `sphinx-7.2.6/sphinx/errors.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/events.py` & `sphinx-7.2.6/sphinx/events.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/apidoc.py` & `sphinx-7.2.6/sphinx/ext/apidoc.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autodoc/__init__.py` & `sphinx-7.2.6/sphinx/ext/autodoc/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autodoc/directive.py` & `sphinx-7.2.6/sphinx/ext/autodoc/directive.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autodoc/importer.py` & `sphinx-7.2.6/sphinx/ext/autodoc/importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Importer utilities for autodoc"""
 
 from __future__ import annotations
 
+import contextlib
 import importlib
+import os
 import sys
 import traceback
 import typing
 from typing import TYPE_CHECKING, Any, Callable, NamedTuple
 
 from sphinx.ext.autodoc.mock import ismock, undecorate
 from sphinx.pycode import ModuleAnalyzer, PycodeError
@@ -17,14 +19,16 @@
     getslots,
     isclass,
     isenumclass,
     safe_getattr,
 )
 
 if TYPE_CHECKING:
+    from types import ModuleType
+
     from sphinx.ext.autodoc import ObjectMember
 
 logger = logging.getLogger(__name__)
 
 
 def mangle(subject: Any, name: str) -> str:
     """Mangle the given name."""
@@ -65,45 +69,55 @@
             return importlib.import_module(modname)
     except BaseException as exc:
         # Importing modules may cause any side effects, including
         # SystemExit, so we need to catch all errors.
         raise ImportError(exc, traceback.format_exc()) from exc
 
 
+def _reload_module(module: ModuleType, warningiserror: bool = False) -> Any:
+    """
+    Call importlib.reload(module), convert exceptions to ImportError
+    """
+    try:
+        with logging.skip_warningiserror(not warningiserror):
+            return importlib.reload(module)
+    except BaseException as exc:
+        # Importing modules may cause any side effects, including
+        # SystemExit, so we need to catch all errors.
+        raise ImportError(exc, traceback.format_exc()) from exc
+
+
 def import_object(modname: str, objpath: list[str], objtype: str = '',
                   attrgetter: Callable[[Any, str], Any] = safe_getattr,
                   warningiserror: bool = False) -> Any:
     if objpath:
         logger.debug('[autodoc] from %s import %s', modname, '.'.join(objpath))
     else:
         logger.debug('[autodoc] import %s', modname)
 
     try:
         module = None
         exc_on_importing = None
         objpath = list(objpath)
         while module is None:
             try:
-                orig_modules = frozenset(sys.modules)
-                try:
-                    # try importing with ``typing.TYPE_CHECKING == True``
-                    typing.TYPE_CHECKING = True
-                    module = import_module(modname, warningiserror=warningiserror)
-                except ImportError:
-                    # if that fails (e.g. circular import), retry with
-                    # ``typing.TYPE_CHECKING == False`` after reverting
-                    # changes made to ``sys.modules`` by the failed try
-                    for m in [m for m in sys.modules if m not in orig_modules]:
-                        sys.modules.pop(m)
-
-                    typing.TYPE_CHECKING = False
-                    module = import_module(modname, warningiserror=warningiserror)
-                finally:
-                    # ensure ``typing.TYPE_CHECKING == False``
-                    typing.TYPE_CHECKING = False
+                original_module_names = frozenset(sys.modules)
+                module = import_module(modname, warningiserror=warningiserror)
+                if os.environ.get('SPHINX_AUTODOC_RELOAD_MODULES'):
+                    new_modules = [m for m in sys.modules if m not in original_module_names]
+                    # Try reloading modules with ``typing.TYPE_CHECKING == True``.
+                    try:
+                        typing.TYPE_CHECKING = True
+                        # Ignore failures; we've already successfully loaded these modules
+                        with contextlib.suppress(ImportError, KeyError):
+                            for m in new_modules:
+                                _reload_module(sys.modules[m])
+                    finally:
+                        typing.TYPE_CHECKING = False
+                    module = sys.modules[modname]
                 logger.debug('[autodoc] import %s => %r', modname, module)
             except ImportError as exc:
                 logger.debug('[autodoc] import %s => failed', modname)
                 exc_on_importing = exc
                 if '.' in modname:
                     # retry with parent module
                     modname, name = modname.rsplit('.', 1)
```

### Comparing `sphinx-7.2.5/sphinx/ext/autodoc/mock.py` & `sphinx-7.2.6/sphinx/ext/autodoc/mock.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autodoc/preserve_defaults.py` & `sphinx-7.2.6/sphinx/ext/autodoc/preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autodoc/type_comment.py` & `sphinx-7.2.6/sphinx/ext/autodoc/type_comment.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autodoc/typehints.py` & `sphinx-7.2.6/sphinx/ext/autodoc/typehints.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autosectionlabel.py` & `sphinx-7.2.6/sphinx/ext/autosectionlabel.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autosummary/__init__.py` & `sphinx-7.2.6/sphinx/ext/autosummary/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autosummary/generate.py` & `sphinx-7.2.6/sphinx/ext/autosummary/generate.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autosummary/templates/autosummary/class.rst` & `sphinx-7.2.6/sphinx/ext/autosummary/templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/autosummary/templates/autosummary/module.rst` & `sphinx-7.2.6/sphinx/ext/autosummary/templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/coverage.py` & `sphinx-7.2.6/sphinx/ext/coverage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/doctest.py` & `sphinx-7.2.6/sphinx/ext/doctest.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/duration.py` & `sphinx-7.2.6/sphinx/ext/duration.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/extlinks.py` & `sphinx-7.2.6/sphinx/ext/extlinks.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/githubpages.py` & `sphinx-7.2.6/sphinx/ext/githubpages.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/graphviz.py` & `sphinx-7.2.6/sphinx/ext/graphviz.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/ifconfig.py` & `sphinx-7.2.6/sphinx/ext/ifconfig.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/imgconverter.py` & `sphinx-7.2.6/sphinx/ext/imgconverter.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/imgmath.py` & `sphinx-7.2.6/sphinx/ext/imgmath.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/inheritance_diagram.py` & `sphinx-7.2.6/sphinx/ext/inheritance_diagram.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/intersphinx.py` & `sphinx-7.2.6/sphinx/ext/intersphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/linkcode.py` & `sphinx-7.2.6/sphinx/ext/linkcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/mathjax.py` & `sphinx-7.2.6/sphinx/ext/mathjax.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/napoleon/__init__.py` & `sphinx-7.2.6/sphinx/ext/napoleon/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/napoleon/docstring.py` & `sphinx-7.2.6/sphinx/ext/napoleon/docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/todo.py` & `sphinx-7.2.6/sphinx/ext/todo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/ext/viewcode.py` & `sphinx-7.2.6/sphinx/ext/viewcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/extension.py` & `sphinx-7.2.6/sphinx/extension.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/highlighting.py` & `sphinx-7.2.6/sphinx/highlighting.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/io.py` & `sphinx-7.2.6/sphinx/io.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/jinja2glue.py` & `sphinx-7.2.6/sphinx/jinja2glue.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/__init__.py` & `sphinx-7.2.6/sphinx/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ar/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ar/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ar/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ar/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ar/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ar/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/bg/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/bg/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/bg/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/bg/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/bn/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/bn/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/bn/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/bn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/bn/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/bn/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ca/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ca/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ca/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ca/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ca/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ca/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cak/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/cak/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cak/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/cak/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cak/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/cak/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cs/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/cs/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cs/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/cs/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cs/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/cs/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cy/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/cy/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cy/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/cy/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/cy/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/cy/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/da/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/da/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/da/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/da/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/da/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/da/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/de/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/de/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/de/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/de/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/de/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/de_DE/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/de_DE/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/de_DE/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/de_DE/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/el/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/el/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/el/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/el/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/el/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/el/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_DE/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/en_DE/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_DE/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/en_DE/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/en_FR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/en_FR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/en_GB/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/en_GB/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/en_GB/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/en_HK/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/en_HK/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/eo/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/eo/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/eo/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/eo/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/eo/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/eo/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/es/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/es/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/es/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/es/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/es/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/es_CO/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/es_CO/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/es_CO/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/es_CO/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/es_CO/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/es_CO/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/et/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/et/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/et/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/et/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/et/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/et/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/eu/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/eu/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/eu/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/eu/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/eu/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/eu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fa/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/fa/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fa/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/fa/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fa/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/fa/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fi/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/fi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fi/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/fi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fi/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/fi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fr/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/fr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fr/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/fr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fr/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/fr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/fr_FR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/gl/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/gl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/gl/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/gl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/gl/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/gl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/he/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/he/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/he/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/he/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/he/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/he/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hi/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/hi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hi/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/hi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hi/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/hi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/hi_IN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hr/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/hr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hr/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/hr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hr/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/hr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hu/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/hu/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hu/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/hu/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/hu/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/hu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/id/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/id/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/id/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/id/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/id/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/id/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/is/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/is/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/is/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/is/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/is/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/is/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/it/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/it/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/it/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/it/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/it/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/it/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ja/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ja/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ja/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ja/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ja/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ja/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ka/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ka/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ka/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ka/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ka/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ka/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ko/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ko/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ko/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ko/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ko/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ko/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/lt/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/lt/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/lt/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/lt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/lt/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/lt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/lv/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/lv/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/lv/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/lv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/lv/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/lv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/mk/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/mk/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/mk/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/mk/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/mk/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/mk/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/nb_NO/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ne/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ne/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ne/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ne/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ne/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ne/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/nl/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/nl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/nl/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/nl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/nl/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/nl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pl/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/pl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pl/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/pl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pl/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/pl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/pt/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/pt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/pt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/pt_BR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/pt_PT/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ro/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ro/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ro/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ro/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ro/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ro/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ru/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ru/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ru/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ru/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ru/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ru/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/si/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/si/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/si/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/si/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/si/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/si/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sk/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/sk/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sk/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/sk/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sk/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/sk/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sl/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/sl/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sl/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/sl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sl/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/sl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sphinx.pot` & `sphinx-7.2.6/sphinx/locale/sphinx.pot`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sq/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/sq/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sq/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/sq/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sq/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/sq/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/sr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/sr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/sr@latin/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/sr_RS/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sv/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/sv/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sv/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/sv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/sv/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/sv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ta/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ta/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ta/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/ta/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ta/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ta/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/te/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/te/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/te/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/te/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/tr/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/tr/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/tr/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/tr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/tr/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/tr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/uk_UA/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ur/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/ur/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/ur/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/ur/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/vi/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/vi/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/vi/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/vi/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/vi/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/vi/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/yue/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/yue/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/yue/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/yue/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/zh_CN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/zh_HK/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/zh_TW.Big5/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js` & `sphinx-7.2.6/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo` & `sphinx-7.2.6/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/sphinx/locale/zh_TW/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/parsers.py` & `sphinx-7.2.6/sphinx/parsers.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/project.py` & `sphinx-7.2.6/sphinx/project.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/pycode/__init__.py` & `sphinx-7.2.6/sphinx/pycode/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/pycode/ast.py` & `sphinx-7.2.6/sphinx/pycode/ast.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/pycode/parser.py` & `sphinx-7.2.6/sphinx/pycode/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/pygments_styles.py` & `sphinx-7.2.6/sphinx/pygments_styles.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/registry.py` & `sphinx-7.2.6/sphinx/registry.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/roles.py` & `sphinx-7.2.6/sphinx/roles.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/__init__.py` & `sphinx-7.2.6/sphinx/search/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/da.py` & `sphinx-7.2.6/sphinx/search/da.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/de.py` & `sphinx-7.2.6/sphinx/search/de.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/en.py` & `sphinx-7.2.6/sphinx/search/en.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/es.py` & `sphinx-7.2.6/sphinx/search/es.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/fi.py` & `sphinx-7.2.6/sphinx/search/fi.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/fr.py` & `sphinx-7.2.6/sphinx/search/fr.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/hu.py` & `sphinx-7.2.6/sphinx/search/hu.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/it.py` & `sphinx-7.2.6/sphinx/search/it.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/ja.py` & `sphinx-7.2.6/sphinx/search/ja.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/base-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/base-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/danish-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/danish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/dutch-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/dutch-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/finnish-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/finnish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/french-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/french-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/german-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/german-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/hungarian-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/hungarian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/italian-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/italian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/norwegian-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/norwegian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/porter-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/porter-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/portuguese-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/portuguese-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/romanian-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/romanian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/russian-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/russian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/spanish-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/spanish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/swedish-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/swedish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/minified-js/turkish-stemmer.js` & `sphinx-7.2.6/sphinx/search/minified-js/turkish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/nl.py` & `sphinx-7.2.6/sphinx/search/nl.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/no.py` & `sphinx-7.2.6/sphinx/search/no.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/base-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/base-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/danish-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/danish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/dutch-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/dutch-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/finnish-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/finnish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/french-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/french-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/german-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/german-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/hungarian-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/hungarian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/italian-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/italian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/norwegian-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/norwegian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/porter-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/porter-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/portuguese-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/portuguese-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/romanian-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/romanian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/russian-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/russian-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/spanish-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/spanish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/swedish-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/swedish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/non-minified-js/turkish-stemmer.js` & `sphinx-7.2.6/sphinx/search/non-minified-js/turkish-stemmer.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/pt.py` & `sphinx-7.2.6/sphinx/search/pt.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/ro.py` & `sphinx-7.2.6/sphinx/search/ro.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/ru.py` & `sphinx-7.2.6/sphinx/search/ru.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/sv.py` & `sphinx-7.2.6/sphinx/search/sv.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/tr.py` & `sphinx-7.2.6/sphinx/search/tr.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/search/zh.py` & `sphinx-7.2.6/sphinx/search/zh.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/apidoc/package.rst_t` & `sphinx-7.2.6/sphinx/templates/apidoc/package.rst_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/epub3/content.opf_t` & `sphinx-7.2.6/sphinx/templates/epub3/content.opf_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/epub3/nav.xhtml_t` & `sphinx-7.2.6/sphinx/templates/epub3/nav.xhtml_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/epub3/toc.ncx_t` & `sphinx-7.2.6/sphinx/templates/epub3/toc.ncx_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/gettext/message.pot_t` & `sphinx-7.2.6/sphinx/templates/gettext/message.pot_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/htmlhelp/project.hhc` & `sphinx-7.2.6/sphinx/templates/htmlhelp/project.hhc`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/htmlhelp/project.hhp` & `sphinx-7.2.6/sphinx/templates/htmlhelp/project.hhp`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/latex/latex.tex_t` & `sphinx-7.2.6/sphinx/templates/latex/latex.tex_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/latex/longtable.tex_t` & `sphinx-7.2.6/sphinx/templates/latex/longtable.tex_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/latex/sphinxmessages.sty_t` & `sphinx-7.2.6/sphinx/templates/latex/sphinxmessages.sty_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/latex/tabular.tex_t` & `sphinx-7.2.6/sphinx/templates/latex/tabular.tex_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/latex/tabulary.tex_t` & `sphinx-7.2.6/sphinx/templates/latex/tabulary.tex_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/quickstart/Makefile.new_t` & `sphinx-7.2.6/sphinx/templates/quickstart/Makefile.new_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/quickstart/Makefile_t` & `sphinx-7.2.6/sphinx/templates/quickstart/Makefile_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/quickstart/conf.py_t` & `sphinx-7.2.6/sphinx/templates/quickstart/conf.py_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/quickstart/make.bat.new_t` & `sphinx-7.2.6/sphinx/templates/quickstart/make.bat.new_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/quickstart/make.bat_t` & `sphinx-7.2.6/sphinx/templates/quickstart/make.bat_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/templates/texinfo/Makefile` & `sphinx-7.2.6/sphinx/templates/texinfo/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/testing/fixtures.py` & `sphinx-7.2.6/sphinx/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/testing/path.py` & `sphinx-7.2.6/sphinx/testing/path.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/testing/restructuredtext.py` & `sphinx-7.2.6/sphinx/testing/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/testing/util.py` & `sphinx-7.2.6/sphinx/testing/util.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/LICRcyr2utf8.xdy` & `sphinx-7.2.6/sphinx/texinputs/LICRcyr2utf8.xdy`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/LICRlatin2utf8.xdy` & `sphinx-7.2.6/sphinx/texinputs/LICRlatin2utf8.xdy`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/LatinRules.xdy` & `sphinx-7.2.6/sphinx/texinputs/LatinRules.xdy`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/Makefile_t` & `sphinx-7.2.6/sphinx/texinputs/Makefile_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/latexmkjarc_t` & `sphinx-7.2.6/sphinx/texinputs/latexmkjarc_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/latexmkrc_t` & `sphinx-7.2.6/sphinx/texinputs/latexmkrc_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/make.bat_t` & `sphinx-7.2.6/sphinx/texinputs/make.bat_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinx.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinx.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinx.xdy` & `sphinx-7.2.6/sphinx/texinputs/sphinx.xdy`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxhowto.cls` & `sphinx-7.2.6/sphinx/texinputs/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexadmonitions.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexadmonitions.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexcontainers.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexcontainers.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexgraphics.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexgraphics.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexindbibtoc.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexindbibtoc.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexlists.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexlists.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexliterals.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexliterals.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexnumfig.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexnumfig.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexobjects.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexobjects.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexshadowbox.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexshadowbox.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexstyleheadings.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexstyleheadings.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexstylepage.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexstylepage.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatexstyletext.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatexstyletext.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxlatextables.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxlatextables.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxmanual.cls` & `sphinx-7.2.6/sphinx/texinputs/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxoptionsgeometry.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxoptionsgeometry.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxoptionshyperref.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxoptionshyperref.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxpackageboxes.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxpackageboxes.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxpackagecyrillic.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxpackagecyrillic.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs/sphinxpackagefootnote.sty` & `sphinx-7.2.6/sphinx/texinputs/sphinxpackagefootnote.sty`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/texinputs_win/Makefile_t` & `sphinx-7.2.6/sphinx/texinputs_win/Makefile_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/agogo/layout.html` & `sphinx-7.2.6/sphinx/themes/agogo/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/agogo/static/agogo.css_t` & `sphinx-7.2.6/sphinx/themes/agogo/static/agogo.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/changes/versionchanges.html` & `sphinx-7.2.6/sphinx/themes/basic/changes/versionchanges.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/defindex.html` & `sphinx-7.2.6/sphinx/themes/basic/defindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/domainindex.html` & `sphinx-7.2.6/sphinx/themes/basic/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/genindex-single.html` & `sphinx-7.2.6/sphinx/themes/basic/genindex-single.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/genindex-split.html` & `sphinx-7.2.6/sphinx/themes/basic/genindex-split.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/genindex.html` & `sphinx-7.2.6/sphinx/themes/basic/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/layout.html` & `sphinx-7.2.6/sphinx/themes/basic/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/opensearch.xml` & `sphinx-7.2.6/sphinx/themes/basic/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/relations.html` & `sphinx-7.2.6/sphinx/themes/basic/relations.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/search.html` & `sphinx-7.2.6/sphinx/themes/basic/search.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/searchbox.html` & `sphinx-7.2.6/sphinx/themes/basic/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/searchfield.html` & `sphinx-7.2.6/sphinx/themes/basic/searchfield.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/sourcelink.html` & `sphinx-7.2.6/sphinx/themes/basic/sourcelink.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/static/basic.css_t` & `sphinx-7.2.6/sphinx/themes/basic/static/basic.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/static/doctools.js` & `sphinx-7.2.6/sphinx/themes/basic/static/doctools.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/static/documentation_options.js_t` & `sphinx-7.2.6/sphinx/themes/basic/static/documentation_options.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/static/language_data.js_t` & `sphinx-7.2.6/sphinx/themes/basic/static/language_data.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/static/searchtools.js` & `sphinx-7.2.6/sphinx/themes/basic/static/searchtools.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/basic/static/sphinx_highlight.js` & `sphinx-7.2.6/sphinx/themes/basic/static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/bizstyle/layout.html` & `sphinx-7.2.6/sphinx/themes/bizstyle/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/bizstyle/static/bizstyle.css_t` & `sphinx-7.2.6/sphinx/themes/bizstyle/static/bizstyle.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/bizstyle/static/bizstyle.js_t` & `sphinx-7.2.6/sphinx/themes/bizstyle/static/bizstyle.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/bizstyle/static/css3-mediaqueries.js` & `sphinx-7.2.6/sphinx/themes/bizstyle/static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js` & `sphinx-7.2.6/sphinx/themes/bizstyle/static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/classic/layout.html` & `sphinx-7.2.6/sphinx/themes/classic/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/classic/static/classic.css_t` & `sphinx-7.2.6/sphinx/themes/classic/static/classic.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/classic/static/sidebar.js_t` & `sphinx-7.2.6/sphinx/themes/classic/static/sidebar.js_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/classic/theme.conf` & `sphinx-7.2.6/sphinx/themes/classic/theme.conf`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/epub/epub-cover.html` & `sphinx-7.2.6/sphinx/themes/epub/epub-cover.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/epub/layout.html` & `sphinx-7.2.6/sphinx/themes/epub/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/epub/static/epub.css_t` & `sphinx-7.2.6/sphinx/themes/epub/static/epub.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/haiku/layout.html` & `sphinx-7.2.6/sphinx/themes/haiku/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/haiku/static/alert_info_32.png` & `sphinx-7.2.6/sphinx/themes/haiku/static/alert_info_32.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/haiku/static/alert_warning_32.png` & `sphinx-7.2.6/sphinx/themes/haiku/static/alert_warning_32.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/haiku/static/haiku.css_t` & `sphinx-7.2.6/sphinx/themes/haiku/static/haiku.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/nature/static/nature.css_t` & `sphinx-7.2.6/sphinx/themes/nature/static/nature.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/nonav/layout.html` & `sphinx-7.2.6/sphinx/themes/nonav/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/nonav/static/nonav.css_t` & `sphinx-7.2.6/sphinx/themes/nonav/static/nonav.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/layout.html` & `sphinx-7.2.6/sphinx/themes/pyramid/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-note.png` & `sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-note.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-seealso.png` & `sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-seealso.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-todo.png` & `sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-todo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-topic.png` & `sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-topic.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/static/dialog-warning.png` & `sphinx-7.2.6/sphinx/themes/pyramid/static/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/static/epub.css_t` & `sphinx-7.2.6/sphinx/themes/pyramid/static/epub.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/static/ie6.css` & `sphinx-7.2.6/sphinx/themes/pyramid/static/ie6.css`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/pyramid/static/pyramid.css_t` & `sphinx-7.2.6/sphinx/themes/pyramid/static/pyramid.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/artwork/logo.svg` & `sphinx-7.2.6/sphinx/themes/scrolls/artwork/logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/layout.html` & `sphinx-7.2.6/sphinx/themes/scrolls/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/static/darkmetal.png` & `sphinx-7.2.6/sphinx/themes/scrolls/static/darkmetal.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/static/logo.png` & `sphinx-7.2.6/sphinx/themes/scrolls/static/logo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/static/metal.png` & `sphinx-7.2.6/sphinx/themes/scrolls/static/metal.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/static/scrolls.css_t` & `sphinx-7.2.6/sphinx/themes/scrolls/static/scrolls.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/static/theme_extras.js` & `sphinx-7.2.6/sphinx/themes/scrolls/static/theme_extras.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/static/watermark.png` & `sphinx-7.2.6/sphinx/themes/scrolls/static/watermark.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/scrolls/static/watermark_blur.png` & `sphinx-7.2.6/sphinx/themes/scrolls/static/watermark_blur.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t` & `sphinx-7.2.6/sphinx/themes/sphinxdoc/static/sphinxdoc.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/themes/traditional/static/traditional.css_t` & `sphinx-7.2.6/sphinx/themes/traditional/static/traditional.css_t`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/theming.py` & `sphinx-7.2.6/sphinx/theming.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/transforms/__init__.py` & `sphinx-7.2.6/sphinx/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/transforms/compact_bullet_list.py` & `sphinx-7.2.6/sphinx/transforms/compact_bullet_list.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/transforms/i18n.py` & `sphinx-7.2.6/sphinx/transforms/i18n.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/transforms/post_transforms/__init__.py` & `sphinx-7.2.6/sphinx/transforms/post_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/transforms/post_transforms/code.py` & `sphinx-7.2.6/sphinx/transforms/post_transforms/code.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/transforms/post_transforms/images.py` & `sphinx-7.2.6/sphinx/transforms/post_transforms/images.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/transforms/references.py` & `sphinx-7.2.6/sphinx/transforms/references.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/__init__.py` & `sphinx-7.2.6/sphinx/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/_pathlib.py` & `sphinx-7.2.6/sphinx/util/_pathlib.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/cfamily.py` & `sphinx-7.2.6/sphinx/util/cfamily.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/console.py` & `sphinx-7.2.6/sphinx/util/console.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/display.py` & `sphinx-7.2.6/sphinx/util/display.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/docfields.py` & `sphinx-7.2.6/sphinx/util/docfields.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/docstrings.py` & `sphinx-7.2.6/sphinx/util/docstrings.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/docutils.py` & `sphinx-7.2.6/sphinx/util/docutils.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/exceptions.py` & `sphinx-7.2.6/sphinx/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/fileutil.py` & `sphinx-7.2.6/sphinx/util/fileutil.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/http_date.py` & `sphinx-7.2.6/sphinx/util/http_date.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/i18n.py` & `sphinx-7.2.6/sphinx/util/i18n.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/images.py` & `sphinx-7.2.6/sphinx/util/images.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/index_entries.py` & `sphinx-7.2.6/sphinx/util/index_entries.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/inspect.py` & `sphinx-7.2.6/sphinx/util/inspect.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/inventory.py` & `sphinx-7.2.6/sphinx/util/inventory.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/logging.py` & `sphinx-7.2.6/sphinx/util/logging.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/matching.py` & `sphinx-7.2.6/sphinx/util/matching.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/math.py` & `sphinx-7.2.6/sphinx/util/math.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/nodes.py` & `sphinx-7.2.6/sphinx/util/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/osutil.py` & `sphinx-7.2.6/sphinx/util/osutil.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/parallel.py` & `sphinx-7.2.6/sphinx/util/parallel.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/png.py` & `sphinx-7.2.6/sphinx/util/png.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/requests.py` & `sphinx-7.2.6/sphinx/util/requests.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/rst.py` & `sphinx-7.2.6/sphinx/util/rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/tags.py` & `sphinx-7.2.6/sphinx/util/tags.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/template.py` & `sphinx-7.2.6/sphinx/util/template.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/texescape.py` & `sphinx-7.2.6/sphinx/util/texescape.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/util/typing.py` & `sphinx-7.2.6/sphinx/util/typing.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/versioning.py` & `sphinx-7.2.6/sphinx/versioning.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/writers/html.py` & `sphinx-7.2.6/sphinx/writers/html.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/writers/html5.py` & `sphinx-7.2.6/sphinx/writers/html5.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/writers/latex.py` & `sphinx-7.2.6/sphinx/writers/latex.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/writers/manpage.py` & `sphinx-7.2.6/sphinx/writers/manpage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/writers/texinfo.py` & `sphinx-7.2.6/sphinx/writers/texinfo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/writers/text.py` & `sphinx-7.2.6/sphinx/writers/text.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/sphinx/writers/xml.py` & `sphinx-7.2.6/sphinx/writers/xml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/certs/cert.pem` & `sphinx-7.2.6/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/conftest.py` & `sphinx-7.2.6/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from pathlib import Path
 
 import docutils
 import pytest
 
 import sphinx
 import sphinx.locale
@@ -20,14 +21,16 @@
 sphinx.locale.init_console = _init_console
 
 pytest_plugins = 'sphinx.testing.fixtures'
 
 # Exclude 'roots' dirs for pytest test collector
 collect_ignore = ['roots']
 
+os.environ['SPHINX_AUTODOC_RELOAD_MODULES'] = '1'
+
 
 @pytest.fixture(scope='session')
 def rootdir():
     return Path(__file__).parent.absolute() / 'roots'
 
 
 def pytest_report_header(config):
```

### Comparing `sphinx-7.2.5/tests/js/searchtools.js` & `sphinx-7.2.6/tests/js/searchtools.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/js/sphinx_highlight.js` & `sphinx-7.2.6/tests/js/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-add_enumerable_node/enumerable_node.py` & `sphinx-7.2.6/tests/roots/test-add_enumerable_node/enumerable_node.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-add_enumerable_node/index.rst` & `sphinx-7.2.6/tests/roots/test-add_enumerable_node/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-api-set-translator/conf.py` & `sphinx-7.2.6/tests/roots/test-api-set-translator/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-autosummary/dummy_module.py` & `sphinx-7.2.6/tests/roots/test-autosummary/dummy_module.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-basic/index.rst` & `sphinx-7.2.6/tests/roots/test-basic/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-directive-code/caption.rst` & `sphinx-7.2.6/tests/roots/test-directive-code/caption.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-directive-code/dedent.rst` & `sphinx-7.2.6/tests/roots/test-directive-code/dedent.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-directive-only/only.rst` & `sphinx-7.2.6/tests/roots/test-directive-only/only.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-c-intersphinx/index.rst` & `sphinx-7.2.6/tests/roots/test-domain-c-intersphinx/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-c/index.rst` & `sphinx-7.2.6/tests/roots/test-domain-c/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-cpp-intersphinx/index.rst` & `sphinx-7.2.6/tests/roots/test-domain-cpp-intersphinx/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-cpp/any-role.rst` & `sphinx-7.2.6/tests/roots/test-domain-cpp/any-role.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-cpp/index.rst` & `sphinx-7.2.6/tests/roots/test-domain-cpp/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-cpp/roles-targets-ok.rst` & `sphinx-7.2.6/tests/roots/test-domain-cpp/roles-targets-ok.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-cpp/roles-targets-warn.rst` & `sphinx-7.2.6/tests/roots/test-domain-cpp/roles-targets-warn.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-cpp/roles.rst` & `sphinx-7.2.6/tests/roots/test-domain-cpp/roles.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-js/module.rst` & `sphinx-7.2.6/tests/roots/test-domain-js/module.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-js/roles.rst` & `sphinx-7.2.6/tests/roots/test-domain-js/roles.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-py/module.rst` & `sphinx-7.2.6/tests/roots/test-domain-py/module.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-domain-py/roles.rst` & `sphinx-7.2.6/tests/roots/test-domain-py/roles.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/__init__.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/autoclass_content.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/autoclass_content.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/autodoc_type_aliases.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/classes.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/classes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/coroutine.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/coroutine.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/decorator.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/decorator.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/descriptor.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/descriptor.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/docstring_signature.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/docstring_signature.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/need_mocks.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/need_mocks.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/overload.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/overload.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/preserve_defaults.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/preserve_defaults_special_constructs.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/preserve_defaults_special_constructs.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/private.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/private.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/singledispatch.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/singledispatch.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/singledispatchmethod.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/singledispatchmethod.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/typed_vars.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/typed_vars.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autodoc/target/typehints.py` & `sphinx-7.2.6/tests/roots/test-ext-autodoc/target/typehints.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst` & `sphinx-7.2.6/tests/roots/test-ext-autosectionlabel-prefix-document/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autosectionlabel/index.rst` & `sphinx-7.2.6/tests/roots/test-ext-autosectionlabel/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-autosummary/autosummary_dummy_module.py` & `sphinx-7.2.6/tests/roots/test-ext-autosummary/autosummary_dummy_module.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-doctest-skipif/skipif.txt` & `sphinx-7.2.6/tests/roots/test-ext-doctest-skipif/skipif.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-doctest/doctest.txt` & `sphinx-7.2.6/tests/roots/test-ext-doctest/doctest.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst` & `sphinx-7.2.6/tests/roots/test-ext-extlinks-hardcoded-urls-multiple-replacements/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst` & `sphinx-7.2.6/tests/roots/test-ext-extlinks-hardcoded-urls/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-graphviz/index.rst` & `sphinx-7.2.6/tests/roots/test-ext-graphviz/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-imgconverter/img.pdf` & `sphinx-7.2.6/tests/roots/test-ext-imgconverter/img.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py` & `sphinx-7.2.6/tests/roots/test-ext-imgmockconverter/mocksvgconverter.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-intersphinx-role/index.rst` & `sphinx-7.2.6/tests/roots/test-ext-intersphinx-role/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-viewcode-find/index.rst` & `sphinx-7.2.6/tests/roots/test-ext-viewcode-find/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-viewcode/conf.py` & `sphinx-7.2.6/tests/roots/test-ext-viewcode/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-viewcode/index.rst` & `sphinx-7.2.6/tests/roots/test-ext-viewcode/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-ext-viewcode/objects.rst` & `sphinx-7.2.6/tests/roots/test-ext-viewcode/objects.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-footnotes/index.rst` & `sphinx-7.2.6/tests/roots/test-footnotes/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-html_entity/index.rst` & `sphinx-7.2.6/tests/roots/test-html_entity/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-html_scaled_image_link/img.png` & `sphinx-7.2.6/tests/roots/test-html_scaled_image_link/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-image-escape/img_#1.png` & `sphinx-7.2.6/tests/roots/test-image-escape/img_#1.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-images/img.gif` & `sphinx-7.2.6/tests/roots/test-images/img.gif`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-images/img.ja.png` & `sphinx-7.2.6/tests/roots/test-images/img.ja.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-images/img.pdf` & `sphinx-7.2.6/tests/roots/test-images/img.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-images/img.png` & `sphinx-7.2.6/tests/roots/test-images/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-images/img.zh.png` & `sphinx-7.2.6/tests/roots/test-images/img.zh.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-images/subdir/svgimg.pdf` & `sphinx-7.2.6/tests/roots/test-images/subdir/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-images/testimäge.png` & `sphinx-7.2.6/tests/roots/test-images/testimäge.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/admonitions.txt` & `sphinx-7.2.6/tests/roots/test-intl/admonitions.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/docfields.txt` & `sphinx-7.2.6/tests/roots/test-intl/docfields.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/external_links.txt` & `sphinx-7.2.6/tests/roots/test-intl/external_links.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/figure.txt` & `sphinx-7.2.6/tests/roots/test-intl/figure.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/i18n.png` & `sphinx-7.2.6/tests/roots/test-intl/i18n.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/img.png` & `sphinx-7.2.6/tests/roots/test-intl/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/index.txt` & `sphinx-7.2.6/tests/roots/test-intl/index.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/label_target.txt` & `sphinx-7.2.6/tests/roots/test-intl/label_target.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/literalblock.txt` & `sphinx-7.2.6/tests/roots/test-intl/literalblock.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/refs.txt` & `sphinx-7.2.6/tests/roots/test-intl/refs.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/role_xref.txt` & `sphinx-7.2.6/tests/roots/test-intl/role_xref.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/translation_progress.txt` & `sphinx-7.2.6/tests/roots/test-intl/translation_progress.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/admonitions.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/definition_terms.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/docfields.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/external_links.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/figure.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/figure.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/footnote.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/glossary_terms_inconsistency.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/index.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/index_entries.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/label_target.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/literalblock.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/noqa.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/only.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/only.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/raw.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/raw.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/refs.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/refs.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/refs_inconsistency.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/refs_python_domain.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/role_xref.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/rubric.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/section.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/section.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/seealso.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/table.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/table.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/toctree.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/topic.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/topic.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/translation_progress.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/translation_progress.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/versionchange.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po` & `sphinx-7.2.6/tests/roots/test-intl/xx/LC_MESSAGES/warnings.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/i18n.png` & `sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/i18n.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/img.png` & `sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-intl_substitution_definitions/xx/LC_MESSAGES/prolog_epilog_substitution.po` & `sphinx-7.2.6/tests/roots/test-intl_substitution_definitions/xx/LC_MESSAGES/prolog_epilog_substitution.po`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-figure-in-admonition/img.png` & `sphinx-7.2.6/tests/roots/test-latex-figure-in-admonition/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-includegraphics/conf.py` & `sphinx-7.2.6/tests/roots/test-latex-includegraphics/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-includegraphics/img.png` & `sphinx-7.2.6/tests/roots/test-latex-includegraphics/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-includegraphics/index.rst` & `sphinx-7.2.6/tests/roots/test-latex-includegraphics/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-includegraphics/sphinx.png` & `sphinx-7.2.6/tests/roots/test-latex-includegraphics/sphinx.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-includegraphics/tall.png` & `sphinx-7.2.6/tests/roots/test-latex-includegraphics/tall.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-labels/index.rst` & `sphinx-7.2.6/tests/roots/test-latex-labels/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/complex.rst` & `sphinx-7.2.6/tests/roots/test-latex-table/complex.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/complex_spanning_cell.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/complex_spanning_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/gridtable.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/gridtable.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/gridtable_with_tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_align.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_align.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_caption.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_caption.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_stub_columns_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_verbatim.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_widths.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_widths.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_having_widths_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/longtable_with_tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/simple_table.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/simple_table.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_caption.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_caption.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_stub_columns_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_threeparagraphs_cell_in_first_col.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_verbatim.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_verbatim.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_widths.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_widths.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/table_having_widths_and_problematic_cell.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/tabular_having_widths.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/tabular_having_widths.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/tabularcolumn.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/tabularcolumn.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/expects/tabulary_having_widths.tex` & `sphinx-7.2.6/tests/roots/test-latex-table/expects/tabulary_having_widths.tex`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/longtable.rst` & `sphinx-7.2.6/tests/roots/test-latex-table/longtable.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-latex-table/tabular.rst` & `sphinx-7.2.6/tests/roots/test-latex-table/tabular.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-linkcheck-anchors-ignore-for-url/index.rst` & `sphinx-7.2.6/tests/roots/test-linkcheck-anchors-ignore-for-url/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-linkcheck/links.rst` & `sphinx-7.2.6/tests/roots/test-linkcheck/links.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-local-logo/images/img.png` & `sphinx-7.2.6/tests/roots/test-local-logo/images/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-local-logo/index.rst` & `sphinx-7.2.6/tests/roots/test-local-logo/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-maxlistdepth/index.rst` & `sphinx-7.2.6/tests/roots/test-maxlistdepth/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-metadata/index.rst` & `sphinx-7.2.6/tests/roots/test-metadata/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-need-escaped/index.rst` & `sphinx-7.2.6/tests/roots/test-need-escaped/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-numfig/bar.rst` & `sphinx-7.2.6/tests/roots/test-numfig/bar.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-numfig/foo.rst` & `sphinx-7.2.6/tests/roots/test-numfig/foo.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-numfig/index.rst` & `sphinx-7.2.6/tests/roots/test-numfig/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-productionlist/index.rst` & `sphinx-7.2.6/tests/roots/test-productionlist/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-remote-logo/index.rst` & `sphinx-7.2.6/tests/roots/test-remote-logo/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/Makefile` & `sphinx-7.2.6/tests/roots/test-root/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/autodoc.txt` & `sphinx-7.2.6/tests/roots/test-root/autodoc.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/autodoc_target.py` & `sphinx-7.2.6/tests/roots/test-root/autodoc_target.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/conf.py` & `sphinx-7.2.6/tests/roots/test-root/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/footnote.txt` & `sphinx-7.2.6/tests/roots/test-root/footnote.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/images.txt` & `sphinx-7.2.6/tests/roots/test-root/images.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/img.foo.png` & `sphinx-7.2.6/tests/roots/test-root/img.foo.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/img.gif` & `sphinx-7.2.6/tests/roots/test-root/img.gif`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/img.pdf` & `sphinx-7.2.6/tests/roots/test-root/img.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/img.png` & `sphinx-7.2.6/tests/roots/test-root/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/includes.txt` & `sphinx-7.2.6/tests/roots/test-root/includes.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/index.txt` & `sphinx-7.2.6/tests/roots/test-root/index.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/lists.txt` & `sphinx-7.2.6/tests/roots/test-root/lists.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/markup.txt` & `sphinx-7.2.6/tests/roots/test-root/markup.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/objects.txt` & `sphinx-7.2.6/tests/roots/test-root/objects.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/subdir/img.png` & `sphinx-7.2.6/tests/roots/test-root/subdir/img.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/subdir/simg.png` & `sphinx-7.2.6/tests/roots/test-root/subdir/simg.png`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-root/svgimg.pdf` & `sphinx-7.2.6/tests/roots/test-root/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-theming/child.zip` & `sphinx-7.2.6/tests/roots/test-theming/child.zip`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-theming/parent.zip` & `sphinx-7.2.6/tests/roots/test-theming/parent.zip`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-theming/ziptheme.zip` & `sphinx-7.2.6/tests/roots/test-theming/ziptheme.zip`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-toctree-domain-objects/domains.rst` & `sphinx-7.2.6/tests/roots/test-toctree-domain-objects/domains.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-toctree/index.rst` & `sphinx-7.2.6/tests/roots/test-toctree/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-trim_doctest_flags/index.rst` & `sphinx-7.2.6/tests/roots/test-trim_doctest_flags/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-versioning/added.txt` & `sphinx-7.2.6/tests/roots/test-versioning/added.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-versioning/deleted.txt` & `sphinx-7.2.6/tests/roots/test-versioning/deleted.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-versioning/insert.txt` & `sphinx-7.2.6/tests/roots/test-versioning/insert.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-versioning/insert_beginning.txt` & `sphinx-7.2.6/tests/roots/test-versioning/insert_beginning.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-versioning/insert_similar.txt` & `sphinx-7.2.6/tests/roots/test-versioning/insert_similar.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-versioning/modified.txt` & `sphinx-7.2.6/tests/roots/test-versioning/modified.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-versioning/original.txt` & `sphinx-7.2.6/tests/roots/test-versioning/original.txt`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-warnings/index.rst` & `sphinx-7.2.6/tests/roots/test-warnings/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/roots/test-warnings/svgimg.pdf` & `sphinx-7.2.6/tests/roots/test-warnings/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_addnodes.py` & `sphinx-7.2.6/tests/test_addnodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_api_translator.py` & `sphinx-7.2.6/tests/test_api_translator.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_application.py` & `sphinx-7.2.6/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build.py` & `sphinx-7.2.6/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_changes.py` & `sphinx-7.2.6/tests/test_build_changes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_dirhtml.py` & `sphinx-7.2.6/tests/test_build_dirhtml.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_epub.py` & `sphinx-7.2.6/tests/test_build_epub.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_gettext.py` & `sphinx-7.2.6/tests/test_build_gettext.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_html.py` & `sphinx-7.2.6/tests/test_build_html.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_latex.py` & `sphinx-7.2.6/tests/test_build_latex.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_linkcheck.py` & `sphinx-7.2.6/tests/test_build_linkcheck.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_manpage.py` & `sphinx-7.2.6/tests/test_build_manpage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_texinfo.py` & `sphinx-7.2.6/tests/test_build_texinfo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_build_text.py` & `sphinx-7.2.6/tests/test_build_text.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_builder.py` & `sphinx-7.2.6/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_catalogs.py` & `sphinx-7.2.6/tests/test_catalogs.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_config.py` & `sphinx-7.2.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_correct_year.py` & `sphinx-7.2.6/tests/test_correct_year.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_directive_code.py` & `sphinx-7.2.6/tests/test_directive_code.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_directive_object_description.py` & `sphinx-7.2.6/tests/test_directive_object_description.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_directive_only.py` & `sphinx-7.2.6/tests/test_directive_only.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_directive_other.py` & `sphinx-7.2.6/tests/test_directive_other.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_directive_patch.py` & `sphinx-7.2.6/tests/test_directive_patch.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_directives_no_typesetting.py` & `sphinx-7.2.6/tests/test_directives_no_typesetting.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_docutilsconf.py` & `sphinx-7.2.6/tests/test_docutilsconf.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_domain_c.py` & `sphinx-7.2.6/tests/test_domain_c.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_domain_cpp.py` & `sphinx-7.2.6/tests/test_domain_cpp.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_domain_js.py` & `sphinx-7.2.6/tests/test_domain_js.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_domain_py.py` & `sphinx-7.2.6/tests/test_domain_py.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_domain_rst.py` & `sphinx-7.2.6/tests/test_domain_rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_domain_std.py` & `sphinx-7.2.6/tests/test_domain_std.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_environment.py` & `sphinx-7.2.6/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_environment_indexentries.py` & `sphinx-7.2.6/tests/test_environment_indexentries.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_environment_toctree.py` & `sphinx-7.2.6/tests/test_environment_toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_events.py` & `sphinx-7.2.6/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_apidoc.py` & `sphinx-7.2.6/tests/test_ext_apidoc.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc.py` & `sphinx-7.2.6/tests/test_ext_autodoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -2099,17 +2099,16 @@
         '   :module: target.singledispatchmethod',
         '',
         '   A method for general use.',
         '',
     ]
 
 
-@pytest.mark.skipif(sys.version_info[:2] >= (3, 11),
-                    reason=('cython does not support python-3.11 yet. '
-                            'see https://github.com/cython/cython/issues/4365'))
+@pytest.mark.skipif(sys.version_info[:2] >= (3, 13),
+                    reason='Cython does not support Python 3.13 yet.')
 @pytest.mark.skipif(pyximport is None, reason='cython is not installed')
 @pytest.mark.sphinx('html', testroot='ext-autodoc')
 def test_cython(app):
     options = {"members": None,
                "undoc-members": None}
     actual = do_autodoc(app, 'module', 'target.cython', options)
     assert list(actual) == [
```

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_autoattribute.py` & `sphinx-7.2.6/tests/test_ext_autodoc_autoattribute.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_autoclass.py` & `sphinx-7.2.6/tests/test_ext_autodoc_autoclass.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_autodata.py` & `sphinx-7.2.6/tests/test_ext_autodoc_autodata.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_autofunction.py` & `sphinx-7.2.6/tests/test_ext_autodoc_autofunction.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_automodule.py` & `sphinx-7.2.6/tests/test_ext_autodoc_automodule.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_autoproperty.py` & `sphinx-7.2.6/tests/test_ext_autodoc_autoproperty.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_configs.py` & `sphinx-7.2.6/tests/test_ext_autodoc_configs.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_events.py` & `sphinx-7.2.6/tests/test_ext_autodoc_events.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_mock.py` & `sphinx-7.2.6/tests/test_ext_autodoc_mock.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_preserve_defaults.py` & `sphinx-7.2.6/tests/test_ext_autodoc_preserve_defaults.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autodoc_private_members.py` & `sphinx-7.2.6/tests/test_ext_autodoc_private_members.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autosectionlabel.py` & `sphinx-7.2.6/tests/test_ext_autosectionlabel.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_autosummary.py` & `sphinx-7.2.6/tests/test_ext_autosummary.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_coverage.py` & `sphinx-7.2.6/tests/test_ext_coverage.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_doctest.py` & `sphinx-7.2.6/tests/test_ext_doctest.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_extlinks.py` & `sphinx-7.2.6/tests/test_ext_extlinks.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_githubpages.py` & `sphinx-7.2.6/tests/test_ext_githubpages.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_graphviz.py` & `sphinx-7.2.6/tests/test_ext_graphviz.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_ifconfig.py` & `sphinx-7.2.6/tests/test_ext_ifconfig.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_imgconverter.py` & `sphinx-7.2.6/tests/test_ext_imgconverter.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_imgmockconverter.py` & `sphinx-7.2.6/tests/test_ext_imgmockconverter.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_inheritance_diagram.py` & `sphinx-7.2.6/tests/test_ext_inheritance_diagram.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_intersphinx.py` & `sphinx-7.2.6/tests/test_ext_intersphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_math.py` & `sphinx-7.2.6/tests/test_ext_math.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_napoleon.py` & `sphinx-7.2.6/tests/test_ext_napoleon.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_napoleon_docstring.py` & `sphinx-7.2.6/tests/test_ext_napoleon_docstring.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_todo.py` & `sphinx-7.2.6/tests/test_ext_todo.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_ext_viewcode.py` & `sphinx-7.2.6/tests/test_ext_viewcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_extension.py` & `sphinx-7.2.6/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_highlighting.py` & `sphinx-7.2.6/tests/test_highlighting.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_intl.py` & `sphinx-7.2.6/tests/test_intl.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_locale.py` & `sphinx-7.2.6/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_markup.py` & `sphinx-7.2.6/tests/test_markup.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_metadata.py` & `sphinx-7.2.6/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_parser.py` & `sphinx-7.2.6/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_project.py` & `sphinx-7.2.6/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_pycode.py` & `sphinx-7.2.6/tests/test_pycode.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_pycode_ast.py` & `sphinx-7.2.6/tests/test_pycode_ast.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_pycode_parser.py` & `sphinx-7.2.6/tests/test_pycode_parser.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_quickstart.py` & `sphinx-7.2.6/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_roles.py` & `sphinx-7.2.6/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_search.py` & `sphinx-7.2.6/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_smartquotes.py` & `sphinx-7.2.6/tests/test_smartquotes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_templating.py` & `sphinx-7.2.6/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_theming.py` & `sphinx-7.2.6/tests/test_theming.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_toctree.py` & `sphinx-7.2.6/tests/test_toctree.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_transforms_move_module_targets.py` & `sphinx-7.2.6/tests/test_transforms_move_module_targets.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_transforms_post_transforms.py` & `sphinx-7.2.6/tests/test_transforms_post_transforms.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_transforms_post_transforms_code.py` & `sphinx-7.2.6/tests/test_transforms_post_transforms_code.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_transforms_reorder_nodes.py` & `sphinx-7.2.6/tests/test_transforms_reorder_nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util.py` & `sphinx-7.2.6/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_display.py` & `sphinx-7.2.6/tests/test_util_display.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_docstrings.py` & `sphinx-7.2.6/tests/test_util_docstrings.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_docutils.py` & `sphinx-7.2.6/tests/test_util_docutils.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_fileutil.py` & `sphinx-7.2.6/tests/test_util_fileutil.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_i18n.py` & `sphinx-7.2.6/tests/test_util_i18n.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_images.py` & `sphinx-7.2.6/tests/test_util_images.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_inspect.py` & `sphinx-7.2.6/tests/test_util_inspect.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_inventory.py` & `sphinx-7.2.6/tests/test_util_inventory.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_logging.py` & `sphinx-7.2.6/tests/test_util_logging.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_matching.py` & `sphinx-7.2.6/tests/test_util_matching.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_nodes.py` & `sphinx-7.2.6/tests/test_util_nodes.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_rst.py` & `sphinx-7.2.6/tests/test_util_rst.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_template.py` & `sphinx-7.2.6/tests/test_util_template.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_util_typing.py` & `sphinx-7.2.6/tests/test_util_typing.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_versioning.py` & `sphinx-7.2.6/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/test_writer_latex.py` & `sphinx-7.2.6/tests/test_writer_latex.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/typing_test_data.py` & `sphinx-7.2.6/tests/typing_test_data.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tests/utils.py` & `sphinx-7.2.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/tox.ini` & `sphinx-7.2.6/tox.ini`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/utils/babel_runner.py` & `sphinx-7.2.6/utils/babel_runner.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/utils/bump_docker.py` & `sphinx-7.2.6/utils/bump_docker.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/utils/bump_version.py` & `sphinx-7.2.6/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/utils/release-checklist` & `sphinx-7.2.6/utils/release-checklist`

 * *Files identical despite different names*

### Comparing `sphinx-7.2.5/PKG-INFO` & `sphinx-7.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sphinx
-Version: 7.2.5
+Version: 7.2.6
 Summary: Python documentation generator
 Author-email: Georg Brandl <georg@python.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

