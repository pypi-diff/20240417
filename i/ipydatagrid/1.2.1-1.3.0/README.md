# Comparing `tmp/ipydatagrid-1.2.1.tar.gz` & `tmp/ipydatagrid-1.3.0.tar.gz`

## Comparing `ipydatagrid-1.2.1.tar` & `ipydatagrid-1.3.0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/RELEASE.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/babel.config.js
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid.json
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/package.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/tsconfig.json
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/webpack.lab.config.js
--rw-r--r--   0        0        0   403047 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/yarn.lock
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/_version.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/cellrenderer.py
--rw-r--r--   0        0        0    31053 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/datagrid.py
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/package.json
--rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/14ad542071f6e259fbe2.png
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/296.60cde3fcac5bac525295.js
--rw-r--r--   0        0        0    32396 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/3546b939aba74f121f34.png
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js
--rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js
--rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/481.911a23288443c8041987.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/5b5469a81198fb5e6aa1.png
--rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/642.730227a42292c5f89120.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js
--rw-r--r--   0        0        0   136897 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js
--rw-r--r--   0        0        0    12508 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/733684aa1ae47c885305.png
--rw-r--r--   0        0        0   292706 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js.LICENSE.txt
--rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js
--rw-r--r--   0        0        0    96423 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/787.0a00e3d5d9b736236907.js
--rw-r--r--   0        0        0    22076 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js
--rw-r--r--   0        0        0    10377 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js
--rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js
--rw-r--r--   0        0        0    13250 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/remoteEntry.55f84c86e55d5446e7ec.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/style.js
--rw-r--r--   0        0        0    40475 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/nbextension/extension.js
--rw-r--r--   0        0        0  1049949 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/nbextension/index.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/ipydatagrid/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/cellrenderer.ts
--rw-r--r--   0        0        0    24623 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/datagrid.ts
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/extension.ts
--rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/feathergrid.ts
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/index.ts
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/keyhandler.ts
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/mousehandler.ts
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/plugin.ts
--rw-r--r--   0        0        0     8137 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/utils.ts
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/vegaexpr.ts
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/version.ts
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/barrenderer.ts
--rw-r--r--   0        0        0    45646 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/filterMenu.ts
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/gridContextMenu.ts
--rw-r--r--   0        0        0    15136 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/headerRenderer.ts
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/transform.ts
--rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/transformExecutors.ts
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/transformStateManager.ts
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/valueRenderer.ts
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/view.ts
--rw-r--r--   0        0        0    22709 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/js/core/viewbasedjsonmodel.ts
--rw-r--r--   0        0        0  1526055 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/static/ipydatagrid_1.gif
--rw-r--r--   0        0        0  1526560 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/static/ipydatagrid_2.gif
--rw-r--r--   0        0        0  2696451 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/static/ipydatagrid_3.gif
--rw-r--r--   0        0        0   203865 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/static/ipydatagrid_4.gif
--rw-r--r--   0        0        0    52546 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/static/ipydatagrid_5.gif
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/style/feathergrid.css
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/style/jupyter-widget.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/style/icons/filter.svg
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/LICENSE.txt
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/README.md
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 ipydatagrid-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/RELEASE.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/babel.config.js
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid.json
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/package.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/tsconfig.json
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/webpack.lab.config.js
+-rw-r--r--   0        0        0   403706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/yarn.lock
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/_version.py
+-rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/cellrenderer.py
+-rw-r--r--   0        0        0    34516 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/datagrid.py
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/package.json
+-rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/14ad542071f6e259fbe2.png
+-rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/296.d2eeaa2e543e597ac586.js
+-rw-r--r--   0        0        0    32396 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/3546b939aba74f121f34.png
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js
+-rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js
+-rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/481.911a23288443c8041987.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/5b5469a81198fb5e6aa1.png
+-rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/642.730227a42292c5f89120.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js
+-rw-r--r--   0        0        0   136897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js
+-rw-r--r--   0        0        0    12508 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/733684aa1ae47c885305.png
+-rw-r--r--   0        0        0   292706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/762.42901b906691b1301214.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/762.42901b906691b1301214.js.LICENSE.txt
+-rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js
+-rw-r--r--   0        0        0   105436 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/787.f307b1ca46997f4a9051.js
+-rw-r--r--   0        0        0    22076 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js
+-rw-r--r--   0        0        0    10377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js
+-rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js
+-rw-r--r--   0        0        0    13315 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/remoteEntry.e416f171876299bb6885.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/style.js
+-rw-r--r--   0        0        0    40475 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/nbextension/extension.js
+-rw-r--r--   0        0        0  2612931 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/nbextension/index.js
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/ipydatagrid/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/cellrenderer.ts
+-rw-r--r--   0        0        0    24043 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/datagrid.ts
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/datasource.ts
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/extension.ts
+-rw-r--r--   0        0        0    31969 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/feathergrid.ts
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/index.ts
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/keyhandler.ts
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/mousehandler.ts
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/plugin.ts
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/utils.ts
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/vegaexpr.ts
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/version.ts
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/barrenderer.ts
+-rw-r--r--   0        0        0    45377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/filterMenu.ts
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/gridContextMenu.ts
+-rw-r--r--   0        0        0    15136 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/headerRenderer.ts
+-rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/htmlRenderer.ts
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/transform.ts
+-rw-r--r--   0        0        0    11413 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/transformExecutors.ts
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/transformStateManager.ts
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/valueRenderer.ts
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/view.ts
+-rw-r--r--   0        0        0    19073 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/js/core/viewbasedjsonmodel.ts
+-rw-r--r--   0        0        0  1526055 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_1.gif
+-rw-r--r--   0        0        0  1526560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_2.gif
+-rw-r--r--   0        0        0  2696451 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_3.gif
+-rw-r--r--   0        0        0   203865 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_4.gif
+-rw-r--r--   0        0        0    52546 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/static/ipydatagrid_5.gif
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/feathergrid.css
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/jupyter-widget.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/style/icons/filter.svg
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/README.md
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 ipydatagrid-1.3.0/PKG-INFO
```

### Comparing `ipydatagrid-1.2.1/RELEASE.md` & `ipydatagrid-1.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/package.json` & `ipydatagrid-1.3.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9678460299590329%*

 * *Differences: {"'devDependencies'": "{'jest-raw-loader': '^1.0.1', 'raw-loader': '^4.0.2'}",*

 * * "'jupyterlab'": "{'sharedPackages': {'bqplot': OrderedDict([('bundled', False), ('singleton', "*

 * *                 'True)])}}',*

 * * "'scripts'": "{'watch': 'npm-run-all -p watch:lib watch:labextension watch:nbextension'}",*

 * * "'version'": "'1.3.0'"}*

```diff
@@ -52,18 +52,20 @@
         "babel-plugin-transform-es2015-modules-commonjs": "^6.26.2",
         "css-loader": "^6.8.1",
         "eslint": "^7.3.1",
         "eslint-config-prettier": "^6.11.0",
         "eslint-plugin-prettier": "^3.1.4",
         "fs-extra": "^7.0.0",
         "jest": "^28.1.3",
+        "jest-raw-loader": "^1.0.1",
         "lint-staged": "^10.2.11",
         "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
         "prettier": "^2.0.5",
+        "raw-loader": "^4.0.2",
         "rimraf": "^2.6.2",
         "source-map-loader": "^0.2.4",
         "style-loader": "^3.3.3",
         "svg-url-loader": "~3.0.3",
         "ts-jest": "^28.0.8",
         "ts-loader": "^6.0.4",
         "typescript": "~4.2.4",
@@ -120,14 +122,18 @@
             "@lumino/virtualdom": {
                 "bundled": false,
                 "singleton": true
             },
             "@lumino/widgets": {
                 "bundled": false,
                 "singleton": true
+            },
+            "bqplot": {
+                "bundled": false,
+                "singleton": true
             }
         },
         "webpackConfig": "webpack.lab.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -154,15 +160,15 @@
         "clean": "rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension",
         "clean:labextension": "rimraf ipydatagrid/labextension",
         "clean:lib": "rimraf lib",
         "clean:nbextension": "rimraf ipydatagrid/nbextension/index.*",
         "lint": "eslint 'js/**/*.{js,ts}' --quiet --fix",
         "prepack": "jlpm run build:labextension && jlpm run build:nbextension",
         "test": "jest --verbose",
-        "watch": "npm-run-all -p watch:*",
+        "watch": "npm-run-all -p watch:lib watch:labextension watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.2.1"
+    "version": "1.3.0"
 }
```

### Comparing `ipydatagrid-1.2.1/tsconfig.json` & `ipydatagrid-1.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/webpack.config.js` & `ipydatagrid-1.3.0/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/yarn.lock` & `ipydatagrid-1.3.0/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -6313,19 +6313,21 @@
     d3-time-format: ^2.1.3
     eslint: ^7.3.1
     eslint-config-prettier: ^6.11.0
     eslint-plugin-prettier: ^3.1.4
     fs-extra: ^7.0.0
     jest: ^28.1.3
     jest-environment-jsdom: ^28.1.3
+    jest-raw-loader: ^1.0.1
     lint-staged: ^10.2.11
     mkdirp: ^0.5.1
     moment: ^2.24.0
     npm-run-all: ^4.1.3
     prettier: ^2.0.5
+    raw-loader: ^4.0.2
     rimraf: ^2.6.2
     source-map-loader: ^0.2.4
     style-loader: ^3.3.3
     svg-url-loader: ~3.0.3
     ts-jest: ^28.0.8
     ts-loader: ^6.0.4
     typescript: ~4.2.4
@@ -6974,14 +6976,21 @@
   peerDependenciesMeta:
     jest-resolve:
       optional: true
   checksum: db1a8ab2cb97ca19c01b1cfa9a9c8c69a143fde833c14df1fab0766f411b1148ff0df878adea09007ac6a2085ec116ba9a996a6ad104b1e58c20adbf88eed9b2
   languageName: node
   linkType: hard
 
+"jest-raw-loader@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "jest-raw-loader@npm:1.0.1"
+  checksum: 0f1e2c650a0dd46cdb6c7b678b384170d41737cc17fca2f776a57af57827bf73bd37e6d0f6625d7912f126ea0dce09b1db2b26424cc1468f08e10e59c7ba1a70
+  languageName: node
+  linkType: hard
+
 "jest-regex-util@npm:^28.0.2":
   version: 28.0.2
   resolution: "jest-regex-util@npm:28.0.2"
   checksum: 0ea8c5c82ec88bc85e273c0ec82e0c0f35f7a1e2d055070e50f0cc2a2177f848eec55f73e37ae0d045c3db5014c42b2f90ac62c1ab3fdb354d2abd66a9e08add
   languageName: node
   linkType: hard
 
@@ -8703,14 +8712,26 @@
   resolution: "randombytes@npm:2.1.0"
   dependencies:
     safe-buffer: "npm:^5.1.0"
   checksum: d779499376bd4cbb435ef3ab9a957006c8682f343f14089ed5f27764e4645114196e75b7f6abf1cbd84fd247c0cb0651698444df8c9bf30e62120fbbc52269d6
   languageName: node
   linkType: hard
 
+"raw-loader@npm:^4.0.2":
+  version: 4.0.2
+  resolution: "raw-loader@npm:4.0.2"
+  dependencies:
+    loader-utils: ^2.0.0
+    schema-utils: ^3.0.0
+  peerDependencies:
+    webpack: ^4.0.0 || ^5.0.0
+  checksum: 51cc1b0d0e8c37c4336b5318f3b2c9c51d6998ad6f56ea09612afcfefc9c1f596341309e934a744ae907177f28efc9f1654eacd62151e82853fcc6d37450e795
+  languageName: node
+  linkType: hard
+
 "react-dom@npm:^18.2.0":
   version: 18.2.0
   resolution: "react-dom@npm:18.2.0"
   dependencies:
     loose-envify: "npm:^1.1.0"
     scheduler: "npm:^0.23.0"
   peerDependencies:
@@ -9789,24 +9810,24 @@
   version: 2.2.1
   resolution: "tapable@npm:2.2.1"
   checksum: 3b7a1b4d86fa940aad46d9e73d1e8739335efd4c48322cb37d073eb6f80f5281889bf0320c6d8ffcfa1a0dd5bfdbd0f9d037e252ef972aca595330538aac4d51
   languageName: node
   linkType: hard
 
 "tar@npm:^6.1.11, tar@npm:^6.1.2":
-  version: 6.2.0
-  resolution: "tar@npm:6.2.0"
+  version: 6.2.1
+  resolution: "tar@npm:6.2.1"
   dependencies:
-    chownr: "npm:^2.0.0"
-    fs-minipass: "npm:^2.0.0"
-    minipass: "npm:^5.0.0"
-    minizlib: "npm:^2.1.1"
-    mkdirp: "npm:^1.0.3"
-    yallist: "npm:^4.0.0"
-  checksum: db4d9fe74a2082c3a5016630092c54c8375ff3b280186938cfd104f2e089c4fd9bad58688ef6be9cf186a889671bf355c7cda38f09bbf60604b281715ca57f5c
+    chownr: ^2.0.0
+    fs-minipass: ^2.0.0
+    minipass: ^5.0.0
+    minizlib: ^2.1.1
+    mkdirp: ^1.0.3
+    yallist: ^4.0.0
+  checksum: f1322768c9741a25356c11373bce918483f40fa9a25c69c59410c8a1247632487edef5fe76c5f12ac51a6356d2f1829e96d2bc34098668a2fc34d76050ac2b6c
   languageName: node
   linkType: hard
 
 "terminal-link@npm:^2.0.0":
   version: 2.1.1
   resolution: "terminal-link@npm:2.1.1"
   dependencies:
```

### Comparing `ipydatagrid-1.2.1/ipydatagrid/datagrid.py` & `ipydatagrid-1.3.0/ipydatagrid/datagrid.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 import decimal
 from collections.abc import Iterator
 from copy import deepcopy
 from math import floor
 
 import numpy as np
 import pandas as pd
+from bqplot.traits import array_from_json, array_to_json
 from ipywidgets import CallbackDispatcher, DOMWidget, widget_serialization
 from traitlets import (
     Bool,
     Dict,
     Enum,
     Instance,
     Int,
     List,
     Unicode,
     default,
     validate,
 )
 
 from ._frontend import module_name, module_version
-from .cellrenderer import CellRenderer, TextRenderer
+from .cellrenderer import BarRenderer, CellRenderer, TextRenderer
 
 
 class SelectionIterator(Iterator):
     def __init__(self, selections):
         self._rect_index = 0
         self._cell_index = 0
         self._selections = selections
@@ -72,15 +73,14 @@
         return (
             rect["r1"] <= cell["r"] <= rect["r2"]
             and rect["c1"] <= cell["c"] <= rect["c2"]
         )
 
 
 class SelectionHelper:
-
     """A Helper Class for processing selections. Provides an iterator
     to traverse selected cells.
     """
 
     def __init__(self, data, selections, selection_mode, **kwargs):
         super().__init__(**kwargs)
         self._data = data
@@ -160,22 +160,21 @@
             return self._num_rows
 
         data = self._data
         self._num_rows = 0 if "data" not in data else len(data["data"])
         return self._num_rows
 
 
-# modified from ipywidgets original
-def _data_to_json(x):
+def _data_to_json(x, _):
     if isinstance(x, dict):
-        return {str(k): _data_to_json(v) for k, v in x.items()}
+        return {str(k): _data_to_json(v, _) for k, v in x.items()}
     if isinstance(x, np.ndarray):
-        return _data_to_json(x.tolist())
+        return _data_to_json(x.tolist(), _)
     if isinstance(x, (list, tuple)):
-        return [_data_to_json(v) for v in x]
+        return [_data_to_json(v, _) for v in x]
     if isinstance(x, int):
         return x
     if isinstance(x, float):
         if np.isnan(x):
             return "$NaN$"
         if np.isposinf(x):
             return "$Infinity$"
@@ -189,17 +188,63 @@
     if x is pd.NaT:
         return "$NaT$"
     if pd.isna(x):
         return "$NaN$"
     return str(x)
 
 
+def _data_serialization_impl(data, _):
+    if not data:
+        return {}
+
+    serialized_data = {}
+    for column, value in data["data"].items():
+        arr = value.to_numpy()
+        if arr.size == 0:
+            serialized_data[str(column)] = {
+                "value": [],
+                "dtype": str(arr.dtype),
+                "shape": arr.shape,
+                "type": None,
+            }
+            continue
+        try:
+            serialized_data[str(column)] = array_to_json(arr)
+        except ValueError:
+            # Column is most likely heterogeneous, sending the column raw
+            serialized_data[str(column)] = {
+                "value": _data_to_json(arr, _),
+                "type": "raw",
+            }
+
+    return {
+        "data": serialized_data,
+        "schema": data["schema"],
+        "fields": _data_to_json(data["fields"], _),
+    }
+
+
+def _data_deserialization_impl(data, _):  # noqa: U101
+    if not data:
+        return {}
+
+    deserialized_data = {}
+    for column, value in data["data"].items():
+        deserialized_data[column] = array_from_json(value.to_numpy())
+
+    return {
+        "data": deserialized_data,
+        "schema": data["schema"],
+        "fields": data["fields"],
+    }
+
+
 _data_serialization = {
-    "from_json": widget_serialization["from_json"],
-    "to_json": lambda x, _: _data_to_json(x),  # noqa: U101
+    "from_json": _data_deserialization_impl,
+    "to_json": _data_serialization_impl,
 }
 
 
 def _widgets_dict_to_json(x, obj):
     return {
         str(k): widget_serialization["to_json"](v, obj) for k, v in x.items()
     }
@@ -208,15 +253,14 @@
 _widgets_dict_serialization = {
     "from_json": widget_serialization["from_json"],
     "to_json": _widgets_dict_to_json,
 }
 
 
 class DataGrid(DOMWidget):
-
     """A Grid Widget with filter, sort and selection capabilities.
 
     Attributes
     ----------
     base_row_size : int (default: 20)
         Default row height
     base_column_size : int (default: 64)
@@ -273,14 +317,18 @@
         Dict to specify global grid styles.
         The keys (strings) indicate the styling property
         The values (css color properties or Vega Expression) indicate the values
         See below for all supported styling properties
     index_name : str (default: "key")
         String to specify the index column name. **Only set when the grid
         is constructed and is not an observable traitlet**
+    horizontal_stripes : bool (default: False)
+        Enable themed coloring of alternate grid rows
+    vertical_stripes : bool (default: False)
+        Enable themed coloring of alternate grid columns
 
     Accessors (not observable traitlets)
     ---------
     selected_cells : list of dict
         List of selected cells. Each cell is represented as a dictionary
         with keys 'r': row and 'c': column
     selected_cell_values : list
@@ -312,15 +360,15 @@
         header_selection_fill_color : fill color of headers intersecting with
             selected area at column or row
         header_selection_border_color : border color of headers
             intersecting with selected area at column or row
         cursor_fill_color : fill color of cursor
         cursor_border_color : border color of cursor
         scroll_shadow : Dict of color parameters for scroll shadow (vertical and
-            horizontal). Takes three paramaters:
+            horizontal). Takes three parameters:
             size : size of shadow in pixels
             color1 : gradient color 1
             color2 : gradient color 2
             color3 : gradient color 3
     """
 
     _model_name = Unicode("DataGridModel").tag(sync=True)
@@ -356,47 +404,48 @@
         sync=True, **widget_serialization
     )
     selection_mode = Enum(
         default_value="none", values=["row", "column", "cell", "none"]
     ).tag(sync=True)
     selections = List(Dict()).tag(sync=True)
     editable = Bool(False).tag(sync=True)
-    column_widths = Dict({}).tag(sync=True, **_data_serialization)
+    column_widths = Dict({}).tag(sync=True, to_json=_data_to_json)
     grid_style = Dict(allow_none=True).tag(
         sync=True, **_widgets_dict_serialization
     )
     auto_fit_columns = Bool(False).tag(sync=True)
     auto_fit_params = Dict(
         {"area": "all", "padding": 30, "numCols": None}, allow_none=False
     ).tag(sync=True)
+    horizontal_stripes = Bool(False).tag(sync=True)
+    vertical_stripes = Bool(False).tag(sync=True)
 
     def __init__(self, dataframe, index_name=None, **kwargs):
         # Setting default index name if not explicitly
         # set by the user.
         self._index_name = index_name
         self.data = dataframe
         super().__init__(**kwargs)
         self._cell_click_handlers = CallbackDispatcher()
         self._cell_change_handlers = CallbackDispatcher()
         self.on_msg(self.__handle_custom_msg)
+        self._set_renderer_defaults()
 
     def __handle_custom_msg(self, _, content, buffers):  # noqa: U101,U100
         if content["event_type"] == "cell-changed":
             row = content["row"]
-            column = self._column_index_to_name(
-                self._data, content["column_index"]
-            )
+            column = content["column"]
             value = content["value"]
             # update data on kernel
-            self._data["data"][row][column] = value
+            self._data["data"].loc[row, column] = value
             # notify python listeners
             self._cell_change_handlers(
                 {
                     "row": row,
-                    "column": column,
+                    "column": content["column"],
                     "column_index": content["column_index"],
                     "value": value,
                 }
             )
         elif content["event_type"] == "cell-click":
             # notify python listeners
             self._cell_click_handlers(
@@ -409,15 +458,15 @@
                     "cell_value": content["cell_value"],
                 }
             )
 
     @property
     def data(self):
         trimmed_primary_key = self._data["schema"]["primaryKey"][:-1]
-        if self._data["data"]:
+        if "data" in self._data:
             df = pd.DataFrame(self._data["data"])
         else:
             df = pd.DataFrame(
                 {value["name"]: [] for value in self._data["schema"]["fields"]}
             )
         final_df = df.set_index(trimmed_primary_key)
         final_df = final_df[final_df.columns[:-1]]
@@ -455,15 +504,15 @@
                     new_index_name = f"{index_name}_{index}"
                 dataframe = dataframe.rename_axis(new_index_name)
             else:
                 dataframe = dataframe.rename_axis(index_name)
 
         schema = pd.io.json.build_table_schema(dataframe)
         reset_index_dataframe = dataframe.reset_index()
-        data = reset_index_dataframe.to_dict(orient="records")
+        data = reset_index_dataframe
 
         # Check for multiple primary keys
         key = reset_index_dataframe.columns[: dataframe.index.nlevels].tolist()
 
         num_index_levels = len(key) if isinstance(key, list) else 1
 
         # Check for nested columns in schema, if so, we need to update the
@@ -517,15 +566,15 @@
 
         Tuples should be used to index into multi-index columns."""
         row_indices = self._get_row_index_of_primary_key(primary_key_value)
 
         if isinstance(column_name, list):
             column_name = tuple(column_name)
 
-        return [self._data["data"][row][column_name] for row in row_indices]
+        return [self._data["data"][column_name][row] for row in row_indices]
 
     def set_cell_value(self, column_name, primary_key_value, new_value):
         """Sets the value for a single cell by column name and primary key.
 
         Note: This method returns a boolean to indicate if the operation
         was successful.
         """
@@ -536,17 +585,17 @@
 
         if isinstance(column_name, list):
             column_name = tuple(column_name)
 
         # Iterate over all indices
         outcome = True
         for row_index in row_indices:
-            has_column = column_name in self._data["data"][row_index]
+            has_column = column_name in self._data["data"]
             if has_column and row_index is not None:
-                self._data["data"][row_index][column_name] = new_value
+                self._data["data"].loc[row_index, column_name] = new_value
                 self._notify_cell_change(row_index, column_name, new_value)
             else:
                 outcome = False
         return outcome
 
     def set_row_value(self, primary_key_value, new_value):
         """Sets the value for a row by and primary key.
@@ -560,37 +609,39 @@
             return False
 
         # Iterate over all indices
         for row_index in row_indices:
             column_index = 0
             column = DataGrid._column_index_to_name(self._data, column_index)
             while column is not None:
-                self._data["data"][row_index][column] = new_value[column_index]
+                self._data["data"].loc[row_index, column] = new_value[
+                    column_index
+                ]
 
                 column_index = column_index + 1
                 column = DataGrid._column_index_to_name(
                     self._data, column_index
                 )
 
             self._notify_row_change(row_index, new_value)
         return True
 
     def get_cell_value_by_index(self, column_name, row_index):
         """Gets the value for a single cell by column name and row index."""
-        return self._data["data"][row_index][column_name]
+        return self._data["data"][column_name][row_index]
 
     def set_cell_value_by_index(self, column_name, row_index, new_value):
         """Sets the value for a single cell by column name and row index.
 
         Note: This method returns a boolean to indicate if the operation
         was successful.
         """
-        has_column = column_name in self._data["data"][row_index]
-        if has_column and 0 <= row_index < len(self._data["data"]):
-            self._data["data"][row_index][column_name] = new_value
+        has_column = column_name in self._data["data"]
+        if has_column and 0 <= row_index < len(self._data["data"][column_name]):
+            self._data["data"].loc[row_index, column_name] = new_value
             self._notify_cell_change(row_index, column_name, new_value)
             return True
         return False
 
     def _notify_cell_change(self, row, column, value):
         column_index = self._column_name_to_index(column)
         # notify python listeners
@@ -629,15 +680,15 @@
             }
         )
 
     def get_visible_data(self):
         """Returns a dataframe of the current View."""
         data = deepcopy(self._data)
         if self._visible_rows:
-            data["data"] = [data["data"][i] for i in self._visible_rows]
+            data["data"] = data["data"].reindex(self._visible_rows)
 
         at = self._data["schema"]["primaryKey"]
         return_df = pd.DataFrame(data["data"]).set_index(at)
         return_df.index = return_df.index.droplevel(return_df.index.nlevels - 1)
         return_df.index.names = self.__dataframe_reference_index_names
         return_df.columns = self.__dataframe_reference_columns
         return return_df
@@ -847,21 +898,63 @@
         key = schema["primaryKey"][:-1]  # Omitting ipydguuid
         if len(value) != len(key):
             raise ValueError(
                 "The provided primary key value must be the same length "
                 "as the primary key."
             )
 
-        row_indices = [
-            at
-            for at, row in enumerate(self._data["data"])
-            if all(row[key[j]] == value[j] for j in range(len(key)))
-        ]
-        return row_indices
+        df = self._data["data"]
+        return pd.RangeIndex(len(df))[
+            (df[key] == value).all(axis="columns")
+        ].to_list()
 
     @staticmethod
     def _get_cell_value_by_numerical_index(data, column_index, row_index):
         """Gets the value for a single cell by column index and row index."""
         column = DataGrid._column_index_to_name(data, column_index)
         if column is None:
             return None
-        return data["data"][row_index][column]
+        return data["data"].loc[row_index, column]
+
+    def _set_renderer_defaults(self):
+        # Set sensible default values for renderers that are not completely
+        # specified, such as missing a min or max value.
+
+        data = None  # Only read data once, and only if necessary.
+
+        for name, renderer in self.renderers.items():
+            if isinstance(renderer, BarRenderer):
+                from bqplot import DateScale, LinearScale, Scale
+
+                if renderer.bar_value is None:
+                    # If BarRenderer.bar_value is not specified, create an
+                    # appropriate Scale based on the column data type.
+                    col_schema = next(
+                        filter(
+                            lambda x: x["name"] == name,
+                            self._data["schema"]["fields"],
+                        )
+                    )
+                    is_date = col_schema["type"] in ("date", "time", "datetime")
+                    if is_date:
+                        renderer.bar_value = DateScale()
+                    else:
+                        renderer.bar_value = LinearScale()
+
+                scale = renderer.bar_value
+                if (
+                    isinstance(scale, Scale)
+                    and scale.has_trait("min")
+                    and scale.has_trait("max")
+                    and (scale.min is None or scale.max is None)
+                ):
+                    # Set min and/or max from column data.
+                    if data is None:
+                        data = self.data  # Only want to get the data once
+                    column_data = data[name]
+                    is_date = isinstance(scale, DateScale)
+                    if scale.min is None:
+                        min = column_data.min()
+                        scale.min = min if is_date else float(min)
+                    if scale.max is None:
+                        max = column_data.max()
+                        scale.max = max if is_date else float(max)
```

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/package.json` & `ipydatagrid-1.3.0/ipydatagrid/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9671775807611721%*

 * *Differences: {"'devDependencies'": "{'jest-raw-loader': '^1.0.1', 'raw-loader': '^4.0.2'}",*

 * * "'jupyterlab'": "{'sharedPackages': {'bqplot': OrderedDict([('bundled', False), ('singleton', "*

 * *                 "True)])}, '_build': {'load': 'static/remoteEntry.e416f171876299bb6885.js'}}",*

 * * "'scripts'": "{'watch': 'npm-run-all -p watch:lib watch:labextension watch:nbextension'}",*

 * * "'version'": "'1.3.0'"}*

```diff
@@ -52,18 +52,20 @@
         "babel-plugin-transform-es2015-modules-commonjs": "^6.26.2",
         "css-loader": "^6.8.1",
         "eslint": "^7.3.1",
         "eslint-config-prettier": "^6.11.0",
         "eslint-plugin-prettier": "^3.1.4",
         "fs-extra": "^7.0.0",
         "jest": "^28.1.3",
+        "jest-raw-loader": "^1.0.1",
         "lint-staged": "^10.2.11",
         "mkdirp": "^0.5.1",
         "npm-run-all": "^4.1.3",
         "prettier": "^2.0.5",
+        "raw-loader": "^4.0.2",
         "rimraf": "^2.6.2",
         "source-map-loader": "^0.2.4",
         "style-loader": "^3.3.3",
         "svg-url-loader": "~3.0.3",
         "ts-jest": "^28.0.8",
         "ts-loader": "^6.0.4",
         "typescript": "~4.2.4",
@@ -80,15 +82,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/Bloomberg/ipydatagrid",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.55f84c86e55d5446e7ec.js"
+            "load": "static/remoteEntry.e416f171876299bb6885.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./ipydatagrid/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -124,14 +126,18 @@
             "@lumino/virtualdom": {
                 "bundled": false,
                 "singleton": true
             },
             "@lumino/widgets": {
                 "bundled": false,
                 "singleton": true
+            },
+            "bqplot": {
+                "bundled": false,
+                "singleton": true
             }
         },
         "webpackConfig": "webpack.lab.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -158,15 +164,15 @@
         "clean": "rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension",
         "clean:labextension": "rimraf ipydatagrid/labextension",
         "clean:lib": "rimraf lib",
         "clean:nbextension": "rimraf ipydatagrid/nbextension/index.*",
         "lint": "eslint 'js/**/*.{js,ts}' --quiet --fix",
         "prepack": "jlpm run build:labextension && jlpm run build:nbextension",
         "test": "jest --verbose",
-        "watch": "npm-run-all -p watch:*",
+        "watch": "npm-run-all -p watch:lib watch:labextension watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.2.1"
+    "version": "1.3.0"
 }
```

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/296.60cde3fcac5bac525295.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/296.d2eeaa2e543e597ac586.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
                         for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && r(n, e, t);
                     return i(n, e), n
                 };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             });
             const a = t(6664),
-                s = t(5123),
+                s = t(1464),
                 d = o(t(5787)),
                 c = t(8657),
                 l = {
                     id: "ipydatagrid:plugin",
                     requires: [a.IJupyterWidgetRegistry],
                     optional: [s.IThemeManager],
                     activate: function(e, n, t) {
```

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/481.911a23288443c8041987.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/481.911a23288443c8041987.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/642.730227a42292c5f89120.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/642.730227a42292c5f89120.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/762.42901b906691b1301214.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/787.0a00e3d5d9b736236907.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/787.f307b1ca46997f4a9051.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,83 +1,78 @@
 "use strict";
 (self.webpackChunkipydatagrid = self.webpackChunkipydatagrid || []).push([
     [787], {
         2509: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
-            }), t.HyperlinkRendererView = t.HyperlinkRendererModel = t.BarRendererView = t.BarRendererModel = t.TextRendererView = t.TextRendererModel = t.CellRendererView = t.CellRendererModel = void 0;
+            }), t.HtmlRendererView = t.HtmlRendererModel = t.ImageRendererView = t.ImageRendererModel = t.HyperlinkRendererView = t.HyperlinkRendererModel = t.BarRendererView = t.BarRendererModel = t.TextRendererView = t.TextRendererModel = t.CellRendererView = t.CellRendererModel = void 0;
             const r = i(5058),
                 n = i(7831),
-                o = i(6092),
-                a = i(6664),
+                a = i(6479),
+                o = i(6664),
                 s = i(8657),
                 l = i(26),
                 d = i(2584),
-                h = i(6988);
-            class c extends a.WidgetModel {
+                h = i(2355),
+                c = i(6988);
+            class u extends o.WidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: c.model_name,
-                        _model_module: c.model_module,
-                        _model_module_version: c.model_module_version,
-                        _view_name: c.view_name,
-                        _view_module: c.view_module,
-                        _view_module_version: c.view_module_version
+                        _model_name: u.model_name,
+                        _model_module: u.model_module,
+                        _model_module_version: u.model_module_version,
+                        _view_name: u.view_name,
+                        _view_module: u.view_module,
+                        _view_module_version: u.view_module_version
                     })
                 }
             }
-            t.CellRendererModel = c, c.model_name = "CellRendererModel", c.model_module = s.MODULE_NAME, c.model_module_version = s.MODULE_VERSION, c.view_name = "CellRendererView", c.view_module = s.MODULE_NAME, c.view_module_version = s.MODULE_VERSION;
-            class u extends a.WidgetView {
+            t.CellRendererModel = u, u.model_name = "CellRendererModel", u.model_module = s.MODULE_NAME, u.model_module_version = s.MODULE_VERSION, u.view_name = "CellRendererView", u.view_module = s.MODULE_NAME, u.view_module_version = s.MODULE_VERSION;
+            class m extends o.WidgetView {
                 constructor() {
                     super(...arguments), this.processors = {}
                 }
-                render() {
-                    return this.initializeRenderer().then((() => {
-                        this.updateRenderer(), this.on("renderer-needs-update", this.updateRenderer.bind(this))
-                    }))
+                async render() {
+                    await this.initializeRenderer(), this.updateRenderer(), this.on("renderer-needs-update", this.updateRenderer.bind(this))
                 }
-                onThemeChanged() {
-                    return this.initializeRenderer().then((() => {
-                        this.updateRenderer()
-                    }))
+                async onThemeChanged() {
+                    return await this.initializeRenderer(), this.updateRenderer()
                 }
-                initializeRenderer() {
+                async initializeRenderer() {
                     const e = {},
                         t = this.model.get_attrs().map((e => e.name));
                     this.model.on_some_change(t, this._on_some_processors_change, this);
                     for (const i of t) e[i] = this.updateProcessor(i);
-                    return a.resolvePromisesDict(e).then((e => {
-                        this.processors = e
-                    }))
+                    this.processors = await o.resolvePromisesDict(e)
                 }
                 _on_some_processors_change(e) {
                     const t = {};
                     for (const i in e.changed) t[i] = this.updateProcessor(i);
-                    a.resolvePromisesDict(t).then((e => {
+                    o.resolvePromisesDict(t).then((e => {
                         this.processors = Object.assign(Object.assign({}, this.processors), e), this.trigger("renderer-needs-update")
                     }))
                 }
                 updateRenderer() {
                     const e = {};
                     for (const t of this.model.get_attrs()) t.phosphorName && (e[t.phosphorName] = e => this.process(t.name, e, t.defaultValue));
                     this.renderer = this.createRenderer(e), this.trigger("renderer-changed")
                 }
                 updateProcessor(e) {
                     const t = this.model.get(e);
-                    return h.Scalar.isScalar(t) ? t : (this.listenTo(t, "change", (() => {
+                    return c.Scalar.isScalar(t) ? t : (this.listenTo(t, "change", (() => {
                         this.trigger("renderer-needs-update")
                     })), this.create_child_view(t))
                 }
                 process(e, t, i) {
                     const r = this.processors[e];
-                    return h.Scalar.isScalar(r) ? "font" === e && "string" == typeof r && ("number" == typeof t.value && !Number.isFinite(t.value) || t.value instanceof Date && Number.isNaN(t.value.getTime())) ? `italic ${r}` : r : r instanceof d.VegaExprView ? r.process(t, i) : "date" == r.model.type || "date_color_linear" == r.model.type ? r.scale(new Date(t.value)) : r.scale(t.value)
+                    return c.Scalar.isScalar(r) ? "font" === e && "string" == typeof r && ("number" == typeof t.value && !Number.isFinite(t.value) || t.value instanceof Date && Number.isNaN(t.value.getTime())) ? `italic ${r}` : r : r instanceof d.VegaExprView ? r.process(t, i) : "date" == r.model.type || "date_color_linear" == r.model.type ? r.scale(new Date(t.value)) : r.scale(t.value)
                 }
             }
-            t.CellRendererView = u;
-            class g extends c {
+            t.CellRendererView = m;
+            class g extends u {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: g.model_name,
                         _view_name: g.view_name,
                         font: "12px sans-serif",
                         text_color: null,
                         text_wrap: !1,
@@ -103,23 +98,23 @@
                     }, {
                         name: "text_elide_direction",
                         phosphorName: "elideDirection",
                         defaultValue: "right"
                     }, {
                         name: "text_color",
                         phosphorName: "textColor",
-                        defaultValue: h.Theme.getFontColor()
+                        defaultValue: c.Theme.getFontColor()
                     }, {
                         name: "text_value",
                         phosphorName: null,
                         defaultValue: null
                     }, {
                         name: "background_color",
                         phosphorName: "backgroundColor",
-                        defaultValue: h.Theme.getBackgroundColor()
+                        defaultValue: c.Theme.getBackgroundColor()
                     }, {
                         name: "vertical_alignment",
                         phosphorName: "verticalAlignment",
                         defaultValue: "center"
                     }, {
                         name: "horizontal_alignment",
                         phosphorName: "horizontalAlignment",
@@ -127,53 +122,53 @@
                     }, {
                         name: "format",
                         phosphorName: null,
                         defaultValue: null
                     }]
                 }
             }
-            t.TextRendererModel = g, g.serializers = Object.assign(Object.assign({}, c.serializers), {
+            t.TextRendererModel = g, g.serializers = Object.assign(Object.assign({}, u.serializers), {
                 font: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 text_color: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 text_wrap: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 text_elide_direction: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 text_value: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 background_color: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 vertical_alignment: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 horizontal_alignment: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 format: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 }
             }), g.model_name = "TextRendererModel", g.view_name = "TextRendererView";
-            class m extends u {
+            class p extends m {
                 render() {
                     return super.render().then((() => {
                         this.model.on_some_change(["missing", "format_type"], (() => {
                             this.trigger("renderer-needs-update")
                         }), this)
                     }))
                 }
                 createRenderer(e) {
-                    return new o.TextRenderer(Object.assign(Object.assign({}, e), {
+                    return new a.TextRenderer(Object.assign(Object.assign({}, e), {
                         format: this.getFormatter()
                     }))
                 }
                 getFormatter(e = {}) {
                     return e => {
                         let t;
                         if (null === e.value) t = this.model.get("missing");
@@ -181,20 +176,20 @@
                             const i = this.process("format", e, null);
                             t = null === i ? String(e.value) : "time" == this.model.get("format_type") ? String(n.timeFormat(i)(new Date(e.value))) : String(r.format(i)(e.value))
                         }
                         return this.process("text_value", e, t) || t
                     }
                 }
             }
-            t.TextRendererView = m;
-            class p extends g {
+            t.TextRendererView = p;
+            class _ extends g {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: p.model_name,
-                        _view_name: p.view_name,
+                        _model_name: _.model_name,
+                        _view_name: _.view_name,
                         bar_color: "#4682b4",
                         bar_value: 0,
                         orientation: "horizontal",
                         bar_vertical_alignment: "bottom",
                         bar_horizontal_alignment: "left",
                         show_text: !0
                     })
@@ -223,45 +218,45 @@
                     }, {
                         name: "show_text",
                         phosphorName: "showText",
                         defaultValue: !0
                     }])
                 }
             }
-            t.BarRendererModel = p, p.serializers = Object.assign(Object.assign({}, g.serializers), {
+            t.BarRendererModel = _, _.serializers = Object.assign(Object.assign({}, g.serializers), {
                 bar_color: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 bar_value: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 orientation: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 bar_vertical_alignment: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 bar_horizontal_alignment: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 show_text: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 }
-            }), p.model_name = "BarRendererModel", p.view_name = "BarRendererView", t.BarRendererView = class extends m {
+            }), _.model_name = "BarRendererModel", _.view_name = "BarRendererView", t.BarRendererView = class extends p {
                 createRenderer(e) {
                     return new l.BarRenderer(Object.assign(Object.assign({}, e), {
                         format: this.getFormatter()
                     }))
                 }
             };
-            class _ extends g {
+            class f extends g {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: p.model_name,
-                        _view_name: p.view_name,
+                        _model_name: _.model_name,
+                        _view_name: _.view_name,
                         url: {},
                         url_name: {}
                     })
                 }
                 get_attrs() {
                     return super.get_attrs().concat([{
                         name: "url",
@@ -270,99 +265,233 @@
                     }, {
                         name: "url_name",
                         phosphorName: "urlName",
                         defaultValue: null
                     }])
                 }
             }
-            t.HyperlinkRendererModel = _, _.serializers = Object.assign(Object.assign({}, g.serializers), {
+            t.HyperlinkRendererModel = f, f.serializers = Object.assign(Object.assign({}, g.serializers), {
                 url: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 },
                 url_name: {
-                    deserialize: a.unpack_models
+                    deserialize: o.unpack_models
                 }
-            }), _.model_name = "HyperlinkRendererModel", _.view_name = "HyperlinkRendererView", t.HyperlinkRendererView = class extends m {
+            }), f.model_name = "HyperlinkRendererModel", f.view_name = "HyperlinkRendererView", t.HyperlinkRendererView = class extends p {
                 createRenderer(e) {
-                    return new o.HyperlinkRenderer(Object.assign(Object.assign({}, e), {
+                    return new a.HyperlinkRenderer(Object.assign(Object.assign({}, e), {
                         format: this.getFormatter()
                     }))
                 }
+            };
+            class b extends u {
+                defaults() {
+                    return Object.assign(Object.assign({}, super.defaults()), {
+                        _model_name: b.model_name,
+                        _view_name: b.view_name,
+                        background_color: {},
+                        placeholder: {},
+                        text_color: {},
+                        width: {},
+                        height: {}
+                    })
+                }
+                get_attrs() {
+                    return [{
+                        name: "background_color",
+                        phosphorName: "backgroundColor",
+                        defaultValue: ""
+                    }, {
+                        name: "placeholder",
+                        phosphorName: "placeholder",
+                        defaultValue: "..."
+                    }, {
+                        name: "text_color",
+                        phosphorName: "textColor",
+                        defaultValue: "#000000"
+                    }, {
+                        name: "width",
+                        phosphorName: "width",
+                        defaultValue: ""
+                    }, {
+                        name: "height",
+                        phosphorName: "height",
+                        defaultValue: "100%"
+                    }]
+                }
+            }
+            t.ImageRendererModel = b, b.serializers = Object.assign(Object.assign({}, g.serializers), {
+                background_color: {
+                    deserialize: o.unpack_models
+                },
+                placeholder: {
+                    deserialize: o.unpack_models
+                },
+                text_color: {
+                    deserialize: o.unpack_models
+                },
+                width: {
+                    deserialize: o.unpack_models
+                },
+                height: {
+                    deserialize: o.unpack_models
+                }
+            }), b.model_name = "ImageRendererModel", b.view_name = "ImageRendererView", t.ImageRendererView = class extends m {
+                createRenderer(e) {
+                    return a.ImageRenderer ? new a.ImageRenderer(Object.assign({}, e)) : new a.TextRenderer({
+                        format: e => "ImageRenderer not available. Check that you are using JupyterLab>=4.1.",
+                        wrapText: !0
+                    })
+                }
+            };
+            class y extends u {
+                defaults() {
+                    return Object.assign(Object.assign({}, super.defaults()), {
+                        _model_name: y.model_name,
+                        _view_name: y.view_name,
+                        font: "12px sans-serif",
+                        placeholder: "...",
+                        text_color: null,
+                        background_color: null,
+                        vertical_alignment: "center",
+                        horizontal_alignment: "left"
+                    })
+                }
+                get_attrs() {
+                    return [{
+                        name: "font",
+                        phosphorName: "font",
+                        defaultValue: "12px sans-serif"
+                    }, {
+                        name: "placeholder",
+                        phosphorName: "placeholder",
+                        defaultValue: "..."
+                    }, {
+                        name: "text_color",
+                        phosphorName: "textColor",
+                        defaultValue: c.Theme.getFontColor()
+                    }, {
+                        name: "background_color",
+                        phosphorName: "backgroundColor",
+                        defaultValue: c.Theme.getBackgroundColor()
+                    }, {
+                        name: "vertical_alignment",
+                        phosphorName: "verticalAlignment",
+                        defaultValue: "center"
+                    }, {
+                        name: "horizontal_alignment",
+                        phosphorName: "horizontalAlignment",
+                        defaultValue: "left"
+                    }]
+                }
+            }
+            t.HtmlRendererModel = y, y.serializers = Object.assign(Object.assign({}, u.serializers), {
+                font: {
+                    deserialize: o.unpack_models
+                },
+                placeholder: {
+                    deserialize: o.unpack_models
+                },
+                text_color: {
+                    deserialize: o.unpack_models
+                },
+                background_color: {
+                    deserialize: o.unpack_models
+                },
+                vertical_alignment: {
+                    deserialize: o.unpack_models
+                },
+                horizontal_alignment: {
+                    deserialize: o.unpack_models
+                }
+            }), y.model_name = "HtmlRendererModel", y.view_name = "HtmlRendererView", t.HtmlRendererView = class extends m {
+                createRenderer(e) {
+                    let t;
+                    return a.AsyncCellRenderer ? (t = new h.exportedClass(Object.assign({}, e)), t.imageLoaded.connect((() => {
+                        setTimeout((() => {
+                            this.trigger("renderer-needs-update")
+                        }), 0)
+                    }))) : t = new a.TextRenderer({
+                        format: e => "AsyncCellRenderer not available. Check that you are using JupyterLab>=4.1.",
+                        wrapText: !0
+                    }), t
+                }
             }
         },
         26: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.BarRenderer = void 0;
-            const r = i(6092);
+            const r = i(6479);
             class n extends r.TextRenderer {
                 constructor(e = {}) {
                     super(e), this.barColor = e.barColor || "#4682b4", this.barValue = e.barValue || 0, this.orientation = e.orientation || "horizontal", this.barVerticalAlignment = e.barVerticalAlignment || "bottom", this.barHorizontalAlignment = e.barHorizontalAlignment || "left", this.showText = e.showText || !0
                 }
                 paint(e, t) {
                     const i = r.CellRenderer.resolveOption(this.showText, t);
                     this.drawBackground(e, t), this.drawBar(e, t), i && this.drawText(e, t)
                 }
                 prepare(e, t) {
                     const {
                         font: i,
                         textColor: r,
                         barColor: n,
-                        backgroundColor: o,
-                        horizontalAlignment: a
+                        backgroundColor: a,
+                        horizontalAlignment: o
                     } = this;
-                    i && "string" == typeof i && (e.font = i), o && "string" == typeof o ? e.fillStyle = o : n && "string" == typeof n ? e.fillStyle = n : r && "string" == typeof r && (e.fillStyle = r), e.textAlign = "string" == typeof a ? a : "left", e.textBaseline = "bottom"
+                    i && "string" == typeof i && (e.font = i), a && "string" == typeof a ? e.fillStyle = a : n && "string" == typeof n ? e.fillStyle = n : r && "string" == typeof r && (e.fillStyle = r), e.textAlign = "string" == typeof o ? o : "left", e.textBaseline = "bottom"
                 }
                 drawBar(e, t) {
                     const i = r.CellRenderer.resolveOption(this.barColor, t);
                     let n = r.CellRenderer.resolveOption(this.barValue, t);
-                    const o = r.CellRenderer.resolveOption(this.barVerticalAlignment, t),
-                        a = r.CellRenderer.resolveOption(this.barHorizontalAlignment, t),
+                    const a = r.CellRenderer.resolveOption(this.barVerticalAlignment, t),
+                        o = r.CellRenderer.resolveOption(this.barHorizontalAlignment, t),
                         s = r.CellRenderer.resolveOption(this.orientation, t);
                     if (!i) return;
                     n > 1 && (n = 1), n < 0 && (n = 0);
                     let l = t.x,
                         d = t.y;
                     if (e.fillStyle = i, "horizontal" === s) {
                         const i = n * t.width;
-                        "center" === a && (l += (t.width - i) / 2), "right" === a && (l += t.width - i), e.fillRect(l, d, i, t.height)
+                        "center" === o && (l += (t.width - i) / 2), "right" === o && (l += t.width - i), e.fillRect(l, d, i, t.height)
                     } else {
                         const i = n * t.height;
-                        "center" === o ? d += (t.height - i) / 2 : "bottom" === o && (d += t.height - i), e.fillRect(l, d, t.width, i)
+                        "center" === a ? d += (t.height - i) / 2 : "bottom" === a && (d += t.height - i), e.fillRect(l, d, t.width, i)
                     }
                 }
             }
             t.BarRenderer = n
         },
         8126: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.UniqueValueStateManager = t.InteractiveFilterDialog = void 0;
             const r = i(8785),
-                n = i(6092),
-                o = i(4901),
-                a = i(5633),
-                s = i(6092),
-                l = i(8778),
+                n = i(6479),
+                a = i(4901),
+                o = i(5633),
+                s = i(6479),
+                l = i(4882),
                 d = i(4059),
                 h = i(4080),
-                c = i(6988);
-            class u extends l.BoxPanel {
+                c = i(6988),
+                u = i(4373);
+            class m extends l.BoxPanel {
                 constructor(e) {
                     super(), this._columnDType = "number", this._columnIndex = 0, this._region = "column-header", this._mode = "value", this._filterOperator = "<", this.hasFilter = !1, this.userInteractedWithDialog = !1, this.addClass("ipydatagrid-filterMenu"), this.node.style.position = "absolute", this._model = e.model, this._filterByConditionWidget = new l.Widget, this._filterByConditionWidget.addClass("ipydatagrid-filter-condition-select"), this._uniqueValueGrid = new n.DataGrid({
                         headerVisibility: "none",
                         stretchLastColumn: !0
-                    }), this._uniqueValueGrid.addClass("ipydatagrid-unique-value-grid"), this._uniqueValueStateManager = new p({
+                    }), this._uniqueValueGrid.addClass("ipydatagrid-unique-value-grid"), this._uniqueValueStateManager = new _({
                         grid: this._uniqueValueGrid
                     });
-                    const t = new _({
+                    const t = new f({
                         stateManager: this._uniqueValueStateManager,
                         dialog: this
                     });
-                    this._uniqueValueGrid.mouseHandler = t, this._titleWidget = new l.Widget, this._titleWidget.addClass("ipydatagrid-filter-title"), this._applyWidget = new l.Widget, this._applyWidget.addClass("ipydatagrid-filter-apply"), this._textInputWidget = new g, this._selectAllCheckbox = new m, this._connectToCheckbox(), this.addWidget(this._titleWidget), this.addWidget(this._textInputWidget), this.addWidget(this._selectAllCheckbox), this.addWidget(this._filterByConditionWidget), this.addWidget(this._uniqueValueGrid), this.addWidget(this._applyWidget)
+                    this._uniqueValueGrid.mouseHandler = t, this._titleWidget = new l.Widget, this._titleWidget.addClass("ipydatagrid-filter-title"), this._applyWidget = new l.Widget, this._applyWidget.addClass("ipydatagrid-filter-apply"), this._textInputWidget = new g, this._selectAllCheckbox = new p, this._connectToCheckbox(), this.addWidget(this._titleWidget), this.addWidget(this._textInputWidget), this.addWidget(this._selectAllCheckbox), this.addWidget(this._filterByConditionWidget), this.addWidget(this._uniqueValueGrid), this.addWidget(this._applyWidget)
                 }
                 _connectToCheckbox() {
                     this._selectAllCheckbox.checkChanged.connect(((e, t) => {
                         this.userInteractedWithDialog = !0, this.addRemoveAllUniqueValuesToState(t)
                     }))
                 }
                 hasValidFilterValue() {
@@ -388,53 +517,53 @@
                 _render() {
                     if ("condition" === this._mode) this._applyWidget.node.style.minHeight = "65px", this._selectAllCheckbox.setHidden(!0), this._uniqueValueGrid.setHidden(!0), this._textInputWidget.setHidden(!0), this._filterByConditionWidget.setHidden(!1), d.VirtualDOM.render([this.createOperatorList()], this._filterByConditionWidget.node), d.VirtualDOM.render([this.createTitleNode()], this._titleWidget.node), d.VirtualDOM.render(["between" === this._filterOperator ? this.createDualValueNode() : this.createSingleValueNode()], this._applyWidget.node);
                     else {
                         if ("value" !== this._mode) throw "unreachable";
                         this._applyWidget.node.style.minHeight = "30px", this._selectAllCheckbox.setHidden(!1), this._uniqueValueGrid.setHidden(!1), this._textInputWidget.setHidden(!1), this._filterByConditionWidget.setHidden(!0), d.VirtualDOM.render([this.createTitleNode()], this._titleWidget.node), d.VirtualDOM.render([this.createTextInputDialog()], this._textInputWidget.node), d.VirtualDOM.render([this.createApplyButtonNode()], this._applyWidget.node), this._renderUniqueVals()
                     }
                 }
-                async _renderUniqueVals() {
-                    this._model.uniqueValues(this._region, this._columnIndex).then((e => {
-                        const t = {
-                            schema: {
-                                fields: [{
-                                    name: "index",
-                                    type: "integer",
-                                    rows: []
-                                }, {
-                                    name: "uniqueVals",
-                                    type: "number",
-                                    rows: []
-                                }],
-                                primaryKey: ["index"],
-                                primaryKeyUuid: "index"
-                            },
-                            data: e.map(((e, t) => ({
-                                index: t,
-                                uniqueVals: e
-                            })))
-                        };
-                        this._uniqueValueGrid.dataModel = new r.ViewBasedJSONModel(t);
-                        const i = {
-                            type: "sort",
-                            columnIndex: this.model.getSchemaIndex(this._region, 0),
-                            desc: !1
-                        };
-                        this._uniqueValueGrid.dataModel.addTransform(i)
-                    }))
+                _renderUniqueVals() {
+                    const e = this._model.uniqueValues(this._region, this._columnIndex),
+                        t = new u.DataSource({
+                            index: [...e.keys()],
+                            uniqueVals: e
+                        }, [{
+                            index: null
+                        }, {
+                            uniqueVals: null
+                        }], {
+                            fields: [{
+                                name: "index",
+                                type: "integer",
+                                rows: []
+                            }, {
+                                name: "uniqueVals",
+                                type: "number",
+                                rows: []
+                            }],
+                            primaryKey: ["index"],
+                            primaryKeyUuid: "index"
+                        });
+                    this._uniqueValueGrid.dataModel = new r.ViewBasedJSONModel(t);
+                    const i = {
+                        type: "sort",
+                        columnIndex: this.model.getSchemaIndex(this._region, 0),
+                        desc: !1
+                    };
+                    this._uniqueValueGrid.dataModel.addTransform(i)
                 }
                 updateSelectAllCheckboxState() {
-                    this.userInteractedWithDialog || this.hasFilter ? this._model.uniqueValues(this._region, this._columnIndex).then((e => {
-                        let t = !0;
-                        for (const i of e)
-                            if (!this._uniqueValueStateManager.has(this._region, this._columnIndex, i)) {
-                                t = !1;
-                                break
-                            } this._selectAllCheckbox.checked = t
-                    })) : this._selectAllCheckbox.checked = !0
+                    if (!this.userInteractedWithDialog && !this.hasFilter) return void(this._selectAllCheckbox.checked = !0);
+                    const e = this._model.uniqueValues(this._region, this._columnIndex);
+                    let t = !0;
+                    for (const i of e)
+                        if (!this._uniqueValueStateManager.has(this._region, this._columnIndex, i)) {
+                            t = !1;
+                            break
+                        } this._selectAllCheckbox.checked = t
                 }
                 open(e) {
                     this._columnIndex = e.columnIndex, this._columnDType = this._model.metadata(e.region, 0, e.columnIndex).type, this._region = e.region, this._mode = e.mode, this.hasFilter = void 0 !== this._model.getFilterTransform(this.model.getSchemaIndex(this._region, this._columnIndex)), this.userInteractedWithDialog = !1, this.updateSelectAllCheckboxState(), this._uniqueValueGrid.style = {
                         voidColor: c.Theme.getBackgroundColor(),
                         backgroundColor: c.Theme.getBackgroundColor(),
                         gridLineColor: c.Theme.getBackgroundColor(),
                         headerGridLineColor: c.Theme.getBorderColor(1),
@@ -452,22 +581,22 @@
                             backgroundColor: c.Theme.getBackgroundColor()
                         })
                     }), this.updateDialog();
                     const t = window.pageXOffset,
                         i = window.pageYOffset,
                         r = document.documentElement.clientWidth,
                         n = document.documentElement.clientHeight,
-                        o = n - (e.forceY ? e.y : 0),
-                        a = this.node,
-                        s = a.style;
-                    s.top = "", s.left = "", s.width = "", s.height = "", s.visibility = "hidden", s.maxHeight = `${o}px`, l.Widget.attach(this, document.body);
+                        a = n - (e.forceY ? e.y : 0),
+                        o = this.node,
+                        s = o.style;
+                    s.top = "", s.left = "", s.width = "", s.height = "", s.visibility = "hidden", s.maxHeight = `${a}px`, l.Widget.attach(this, document.body);
                     const {
                         width: d,
                         height: u
-                    } = a.getBoundingClientRect();
+                    } = o.getBoundingClientRect();
                     !e.forceX && e.x + d > t + r && (e.x = t + r - d), !e.forceY && e.y + u > i + n && (e.y > i + n ? e.y = i + n - u : e.y = e.y - u), s.top = `${Math.max(0,e.y)}px`, s.left = `${Math.max(0,e.x)}px`, s.visibility = ""
                 }
                 handleEvent(e) {
                     switch (e.type) {
                         case "mousedown":
                             this._evtMouseDown(e);
                             break;
@@ -621,15 +750,15 @@
                         className: "p-Menu-itemLabel widget-text",
                         style: {
                             paddingLeft: "5px"
                         }
                     }, "Loading unique values...")
                 }
                 async createUniqueValueNodes() {
-                    const e = (await this._model.uniqueValues(this._region, this._columnIndex)).map((e => d.h.option({
+                    const e = this._model.uniqueValues(this._region, this._columnIndex).map((e => d.h.option({
                         value: e
                     }, String(e))));
                     return d.h.li({
                         className: "p-Menu-item"
                     }, d.h.div({
                         className: "widget-select widget-select-multiple",
                         style: {
@@ -842,18 +971,17 @@
                         selected: ""
                     }), "Is after"), d.h.option(Object.assign({
                         value: "between"
                     }, "between" === e && {
                         selected: ""
                     }), "Is in between")]
                 }
-                async addRemoveAllUniqueValuesToState(e) {
-                    return this.model.uniqueValues(this._region, this._columnIndex).then((t => {
-                        for (const i of t) e ? this._uniqueValueStateManager.add(this._region, this._columnIndex, i) : this._uniqueValueStateManager.remove(this._region, this._columnIndex, i)
-                    }))
+                addRemoveAllUniqueValuesToState(e) {
+                    const t = this.model.uniqueValues(this._region, this._columnIndex);
+                    for (const i of t) e ? this._uniqueValueStateManager.add(this._region, this._columnIndex, i) : this._uniqueValueStateManager.remove(this._region, this._columnIndex, i)
                 }
                 get model() {
                     return this._model
                 }
                 set model(e) {
                     this._model = e
                 }
@@ -869,25 +997,25 @@
                 get columnIndex() {
                     return this._columnIndex
                 }
                 get columnDType() {
                     return this._columnDType
                 }
             }
-            t.InteractiveFilterDialog = u;
+            t.InteractiveFilterDialog = m;
             class g extends l.Widget {
                 constructor() {
                     super(), this.node.style.minHeight = "16px", this.node.style.overflow = "visible"
                 }
             }
-            class m extends l.Widget {
+            class p extends l.Widget {
                 constructor() {
                     super(), this.toggleCheckMark = () => {
                         this._checked = !this._checked, this.renderCheckbox(), this._checkedChanged.emit(this._checked)
-                    }, this._checked = !1, this._checkedChanged = new o.Signal(this), this.canvas = document.createElement("canvas"), this.node.style.minHeight = "16px", this.node.style.overflow = "visible", this.node.appendChild(this.canvas)
+                    }, this._checked = !1, this._checkedChanged = new a.Signal(this), this.canvas = document.createElement("canvas"), this.node.style.minHeight = "16px", this.node.style.overflow = "visible", this.node.appendChild(this.canvas)
                 }
                 get checked() {
                     return this._checked
                 }
                 set checked(e) {
                     this._checked = e, this.renderCheckbox()
                 }
@@ -908,63 +1036,60 @@
                 onAfterAttach() {
                     this.renderCheckbox(), this.canvas.addEventListener("click", this.toggleCheckMark, !0)
                 }
                 onAfterDetach(e) {
                     this.canvas.removeEventListener("click", this.toggleCheckMark, !0)
                 }
             }
-            class p {
+            class _ {
                 constructor(e) {
                     this._state = {}, this._grid = e.grid
                 }
                 has(e, t, i) {
                     const r = this.getKeyName(e, t);
                     return this._state.hasOwnProperty(r) && this._state[r].has(i)
                 }
                 getKeyName(e, t) {
                     return `${e}:${t}`
                 }
                 add(e, t, i) {
                     const r = this.getKeyName(e, t);
                     this._state.hasOwnProperty(r) || (this._state[r] = new Set), this._state[r].add(i);
-                    const n = new f("all", 0, 0, 0, 0);
-                    a.MessageLoop.postMessage(this._grid.viewport, n)
+                    const n = new b("all", 0, 0, 0, 0);
+                    o.MessageLoop.postMessage(this._grid.viewport, n)
                 }
                 remove(e, t, i) {
                     const r = this.getKeyName(e, t);
                     this._state.hasOwnProperty(r) && this._state[r].delete(i);
-                    const n = new f("all", 0, 0, 0, 0);
-                    a.MessageLoop.postMessage(this._grid.viewport, n)
+                    const n = new b("all", 0, 0, 0, 0);
+                    o.MessageLoop.postMessage(this._grid.viewport, n)
                 }
                 getValues(e, t) {
                     const i = this.getKeyName(e, t);
                     return this._state.hasOwnProperty(i) ? Array.from(this._state[i]) : []
                 }
             }
-            t.UniqueValueStateManager = p;
-            class _ extends s.BasicMouseHandler {
+            t.UniqueValueStateManager = _;
+            class f extends s.BasicMouseHandler {
                 constructor(e) {
                     super(), this._uniqueValuesSelectionState = e.stateManager, this._filterDialog = e.dialog
                 }
                 onMouseDown(e, t) {
                     const i = e.hitTest(t.clientX, t.clientY);
                     if ("void" === i.region) return;
                     const r = i.row,
                         n = this._filterDialog.columnIndex,
-                        o = this._filterDialog.region,
-                        a = e.dataModel.data("body", r, 0),
-                        s = () => {
-                            this._uniqueValuesSelectionState.has(o, n, a) ? this._uniqueValuesSelectionState.remove(o, n, a) : this._uniqueValuesSelectionState.add(o, n, a), this._filterDialog.updateSelectAllCheckboxState()
-                        };
-                    this._filterDialog.hasFilter || this._filterDialog.userInteractedWithDialog ? s() : this._filterDialog.addRemoveAllUniqueValuesToState(!0).then((() => {
-                        this._filterDialog.userInteractedWithDialog = !0, s()
-                    }))
+                        a = this._filterDialog.region,
+                        o = e.dataModel.data("body", r, 0);
+                    this._filterDialog.hasFilter || this._filterDialog.userInteractedWithDialog || (this._filterDialog.addRemoveAllUniqueValuesToState(!0), this._filterDialog.userInteractedWithDialog = !0), (() => {
+                        this._uniqueValuesSelectionState.has(a, n, o) ? this._uniqueValuesSelectionState.remove(a, n, o) : this._uniqueValuesSelectionState.add(a, n, o), this._filterDialog.updateSelectAllCheckboxState()
+                    })()
                 }
             }
-            class f extends a.ConflatableMessage {
+            class b extends o.ConflatableMessage {
                 constructor(e, t, i, r, n) {
                     super("paint-request"), this._region = e, this._r1 = t, this._c1 = i, this._r2 = r, this._c2 = n
                 }
                 get region() {
                     return this._region
                 }
                 get r1() {
@@ -984,191 +1109,316 @@
                 }
             }
         },
         6175: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.FeatherGridContextMenu = t.GridContextMenu = void 0;
-            const r = i(8778);
+            const r = i(4882);
             class n {
                 constructor(e) {
                     this._menu = new r.Menu({
                         commands: e.commands
                     }), this._menu.addClass("ipydatagrid-context-menu")
                 }
             }
             t.GridContextMenu = n;
-            class o extends n {
+            class a extends n {
                 open(e, t) {
                     this._menu.clearItems();
                     const i = {
                         region: t.region,
                         rowIndex: t.row,
                         columnIndex: t.column,
                         clientX: t.x,
                         clientY: t.y
                     };
                     switch (t.region) {
                         case "column-header":
+                            this._menu.addItem({
+                                command: a.CommandID.SortAscending,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.SortDescending,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.SortClear,
+                                args: i
+                            }), this._menu.addItem({
+                                type: "separator"
+                            }), this._menu.addItem({
+                                command: a.CommandID.OpenFilterByConditionDialog,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.OpenFilterByValueDialog,
+                                args: i
+                            }), this._menu.addItem({
+                                type: "separator"
+                            }), this._menu.addItem({
+                                command: a.CommandID.ClearSelection,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.ClearThisFilter,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.ClearFiltersInAllColumns,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.CopyToClipboard,
+                                args: i
+                            });
+                            break;
                         case "corner-header":
                             this._menu.addItem({
-                                command: o.CommandID.SortAscending,
+                                command: a.CommandID.SortAscending,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.SortDescending,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.SortClear,
+                                args: i
+                            }), this._menu.addItem({
+                                type: "separator"
+                            }), this._menu.addItem({
+                                command: a.CommandID.OpenFilterByConditionDialog,
+                                args: i
+                            }), this._menu.addItem({
+                                command: a.CommandID.OpenFilterByValueDialog,
+                                args: i
+                            }), this._menu.addItem({
+                                type: "separator"
+                            }), this._menu.addItem({
+                                command: a.CommandID.CopySelectionToClipboard,
                                 args: i
                             }), this._menu.addItem({
-                                command: o.CommandID.SortDescending,
+                                command: a.CommandID.SaveSelectionAsCsv,
                                 args: i
                             }), this._menu.addItem({
-                                command: o.CommandID.OpenFilterByConditionDialog,
+                                command: a.CommandID.SaveAllAsCsv,
                                 args: i
                             }), this._menu.addItem({
-                                command: o.CommandID.OpenFilterByValueDialog,
+                                type: "separator"
+                            }), this._menu.addItem({
+                                command: a.CommandID.ClearSelection,
                                 args: i
                             }), this._menu.addItem({
-                                command: o.CommandID.ClearThisFilter,
+                                command: a.CommandID.ClearThisFilter,
                                 args: i
                             }), this._menu.addItem({
-                                command: o.CommandID.ClearFiltersInAllColumns,
+                                command: a.CommandID.ClearFiltersInAllColumns,
                                 args: i
                             });
                             break;
                         case "body":
                             this._menu.addItem({
-                                command: o.CommandID.RevertGrid,
+                                command: a.CommandID.RevertGrid,
                                 args: i
                             });
                             break;
                         default:
                             throw "unreachable"
                     }
                     this._menu.open(t.x, t.y)
                 }
             }
-            t.FeatherGridContextMenu = o,
+            t.FeatherGridContextMenu = a,
                 function(e) {
                     let t;
                     ! function(e) {
-                        e.SortAscending = "sort:Asc", e.SortDescending = "sort:Desc", e.OpenFilterByConditionDialog = "filterCondition:openDialog", e.OpenFilterByValueDialog = "filterValue:openDialog", e.RevertGrid = "grid:reset", e.ClearThisFilter = "filter:clearCurrentColumn", e.ClearFiltersInAllColumns = "filter:clearAllColumns"
+                        e.SortAscending = "sort:Asc", e.SortDescending = "sort:Desc", e.SortClear = "sort:Clear", e.OpenFilterByConditionDialog = "filterCondition:openDialog", e.OpenFilterByValueDialog = "filterValue:openDialog", e.RevertGrid = "grid:reset", e.ClearThisFilter = "filter:clearCurrentColumn", e.ClearFiltersInAllColumns = "filter:clearAllColumns", e.CopyToClipboard = "copyToClipboard", e.CopySelectionToClipboard = "copySelectionToClipboard", e.SaveSelectionAsCsv = "saveSelectionAsCsv", e.SaveAllAsCsv = "saveAllAsCsv", e.ClearSelection = "clearSelection"
                     }(t = e.CommandID || (e.CommandID = {}))
-                }(o = t.FeatherGridContextMenu || (t.FeatherGridContextMenu = {}))
+                }(a = t.FeatherGridContextMenu || (t.FeatherGridContextMenu = {}))
         },
         2320: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.HeaderRenderer = void 0;
-            const r = i(6092),
+            const r = i(6479),
                 n = i(6988);
-            class o extends r.TextRenderer {
+            class a extends r.TextRenderer {
                 constructor(e) {
                     super(e.textOptions), this._isLightTheme = e.isLightTheme, this._grid = e.grid
                 }
                 get model() {
                     return this._grid.dataModel
                 }
                 drawText(e, t) {
                     const i = r.CellRenderer.resolveOption(this.font, t);
                     if (!i) return;
-                    const a = r.CellRenderer.resolveOption(this.textColor, t);
-                    if (!a) return;
+                    const o = r.CellRenderer.resolveOption(this.textColor, t);
+                    if (!o) return;
                     let s = (0, this.format)(t);
                     if (!s) return;
                     const l = r.CellRenderer.resolveOption(this.verticalAlignment, t),
                         d = r.CellRenderer.resolveOption(this.horizontalAlignment, t),
                         h = r.CellRenderer.resolveOption(this.elideDirection, t),
                         c = r.CellRenderer.resolveOption(this.wrapText, t),
                         u = t.height - ("center" === l ? 1 : 2);
                     if (u <= 0) return;
-                    const g = r.TextRenderer.measureFontHeight(i);
-                    let m, p, _;
+                    const m = r.TextRenderer.measureFontHeight(i);
+                    let g, p, _;
                     switch (l) {
                         case "top":
-                            p = t.y + 2 + g;
+                            p = t.y + 2 + m;
                             break;
                         case "center":
-                            p = t.y + t.height / 2 + g / 2;
+                            p = t.y + t.height / 2 + m / 2;
                             break;
                         case "bottom":
                             p = t.y + t.height - 2;
                             break;
                         default:
                             throw "unreachable"
                     }
                     switch (d) {
                         case "left":
-                            m = t.x + 8, _ = t.width - 14;
+                            g = t.x + 8, _ = t.width - 14;
                             break;
                         case "center":
-                            m = t.x + t.width / 2, _ = t.width;
+                            g = t.x + t.width / 2, _ = t.width;
                             break;
                         case "right":
-                            m = t.x + t.width - 8, _ = t.width - 14;
+                            g = t.x + t.width - 8, _ = t.width - 14;
                             break;
                         default:
                             throw "unreachable"
                     }
-                    g > u && (e.beginPath(), e.rect(t.x, t.y, t.width, t.height - 1), e.clip()), e.font = i, e.fillStyle = a, e.textAlign = d, e.textBaseline = "bottom";
+                    m > u && (e.beginPath(), e.rect(t.x, t.y, t.width, t.height - 1), e.clip()), e.font = i, e.fillStyle = o, e.textAlign = d, e.textBaseline = "bottom";
                     let f = e.measureText(s).width;
                     if (c && f > _) {
                         e.beginPath(), e.rect(t.x, t.y, t.width, t.height - 1), e.clip();
                         const i = s.split(/\s(?=\b)/);
                         let r = p,
                             n = i.shift();
                         if (0 === i.length) {
                             let t = e.measureText(n).width;
                             for (; t > _ && "" !== n;)
                                 for (let i = n.length; i > 0; i--) {
-                                    const o = n.substring(0, i);
-                                    if (e.measureText(o).width < _ || 1 === o.length) {
-                                        const a = n.substring(i, n.length);
-                                        n = a, t = e.measureText(n).width, e.fillText(o, m, r), r += g;
+                                    const a = n.substring(0, i);
+                                    if (e.measureText(a).width < _ || 1 === a.length) {
+                                        const o = n.substring(i, n.length);
+                                        n = o, t = e.measureText(n).width, e.fillText(a, g, r), r += m;
                                         break
                                     }
                                 }
                         } else
                             for (; 0 !== i.length;) {
                                 const t = i.shift(),
-                                    o = [n, t].join(" ");
-                                e.measureText(o).width > _ ? (e.fillText(n, m, r), r += g, n = t) : n = o
+                                    a = [n, t].join(" ");
+                                e.measureText(a).width > _ ? (e.fillText(n, g, r), r += m, n = t) : n = a
                             }
-                        return void e.fillText(n, m, r)
+                        return void e.fillText(n, g, r)
                     }
-                    const y = "…";
+                    const b = "…";
                     if ("right" === h)
-                        for (; f > _ && s.length > 1;) s = s.length > 4 && f >= 2 * _ ? s.substring(0, s.length / 2 + 1) + y : s.substring(0, s.length - 2) + y, f = e.measureText(s).width;
+                        for (; f > _ && s.length > 1;) s = s.length > 4 && f >= 2 * _ ? s.substring(0, s.length / 2 + 1) + b : s.substring(0, s.length - 2) + b, f = e.measureText(s).width;
                     else
-                        for (; f > _ && s.length > 1;) s = s.length > 4 && f >= 2 * _ ? y + s.substring(s.length / 2) : y + s.substring(2), f = e.measureText(s).width;
-                    if (e.fillText(s, m, p), "column-header" === t.region && t.row !== this._grid.dataModel.rowCount("column-header") - 1) return;
-                    const b = o.iconWidth + o.iconWidth + o.iconSpacing + 2 * o.buttonPadding;
-                    e.fillStyle = r.CellRenderer.resolveOption(this.backgroundColor, t), e.fillRect(t.x + t.width - b, t.y + t.height - b, b, b);
-                    const w = t.x + t.width - o.iconWidth - o.buttonPadding;
+                        for (; f > _ && s.length > 1;) s = s.length > 4 && f >= 2 * _ ? b + s.substring(s.length / 2) : b + s.substring(2), f = e.measureText(s).width;
+                    if (e.fillText(s, g, p), "column-header" === t.region && t.row !== this._grid.dataModel.rowCount("column-header") - 1) return;
+                    const y = a.iconWidth + a.iconWidth + a.iconSpacing + 2 * a.buttonPadding;
+                    e.fillStyle = r.CellRenderer.resolveOption(this.backgroundColor, t), e.fillRect(t.x + t.width - y, t.y + t.height - y, y, y);
+                    const w = t.x + t.width - a.iconWidth - a.buttonPadding;
                     if (this.drawFilterIcon(e, t), e.fillStyle = n.Theme.getBorderColor(1), e.fill(), this.model) {
                         const i = this.model.getSchemaIndex(t.region, t.column),
                             r = this.model.transformMetadata(i);
                         r && r.filter && (e.fillStyle = n.Theme.getBrandColor(this._isLightTheme ? 8 : 6), e.fill()), r && r.sort && (r.sort.desc ? this.drawSortArrow(e, t, w, !1) : this.drawSortArrow(e, t, w, !0), e.fillStyle = n.Theme.getBrandColor(this._isLightTheme ? 7 : 5), e.fill())
                     }
                 }
                 drawFilterIcon(e, t) {
-                    const i = t.x + t.width - o.iconWidth - o.buttonPadding,
-                        r = o.iconWidth / 2 + 1,
-                        n = o.iconWidth / 2 - 1,
-                        a = t.height - o.iconHeight - 1 + t.y;
-                    e.beginPath(), e.moveTo(i, a), e.lineTo(i + o.iconWidth, a), e.lineTo(i + r, t.y + t.height - o.iconHeight + 2), e.lineTo(i + r, t.y + t.height - 1.5 * o.buttonPadding), e.lineTo(i + n, t.y + t.height - 2 * o.buttonPadding), e.lineTo(i + n, t.y + t.height - o.iconHeight + 2), e.closePath()
+                    const i = t.x + t.width - a.iconWidth - a.buttonPadding,
+                        r = a.iconWidth / 2 + 1,
+                        n = a.iconWidth / 2 - 1,
+                        o = t.height - a.iconHeight - 1 + t.y;
+                    e.beginPath(), e.moveTo(i, o), e.lineTo(i + a.iconWidth, o), e.lineTo(i + r, t.y + t.height - a.iconHeight + 2), e.lineTo(i + r, t.y + t.height - 1.5 * a.buttonPadding), e.lineTo(i + n, t.y + t.height - 2 * a.buttonPadding), e.lineTo(i + n, t.y + t.height - a.iconHeight + 2), e.closePath()
                 }
                 drawSortArrow(e, t, i, r) {
-                    const n = o.iconWidth - 2,
-                        a = i - o.iconSpacing,
-                        s = a - n / 2 + .5,
-                        l = a - n / 2 - .5,
-                        d = t.height + t.y - o.buttonPadding - o.iconHeight + 4,
-                        h = a - n / 2,
-                        c = t.height + t.y - o.iconHeight - 1,
-                        u = t.height - 8 + t.y + o.buttonPadding;
-                    e.beginPath(), r ? (e.moveTo(h, c), e.lineTo(a, d), e.lineTo(a, d + 1), e.lineTo(s, d + 1), e.lineTo(h + .5, u), e.lineTo(h - .5, u), e.lineTo(h - .5, d + 1), e.lineTo(a - n, d + 1), e.lineTo(a - n, d)) : (e.moveTo(h, u), e.lineTo(a - n, d + 4.5), e.lineTo(a - n, d + 3.5), e.lineTo(l, d + 3.5), e.lineTo(l, c), e.lineTo(h + .5, c), e.lineTo(h + .5, d + 3.5), e.lineTo(a, d + 3.5), e.lineTo(a, d + 4.5)), e.closePath()
+                    const n = a.iconWidth - 2,
+                        o = i - a.iconSpacing,
+                        s = o - n / 2 + .5,
+                        l = o - n / 2 - .5,
+                        d = t.height + t.y - a.buttonPadding - a.iconHeight + 4,
+                        h = o - n / 2,
+                        c = t.height + t.y - a.iconHeight - 1,
+                        u = t.height - 8 + t.y + a.buttonPadding;
+                    e.beginPath(), r ? (e.moveTo(h, c), e.lineTo(o, d), e.lineTo(o, d + 1), e.lineTo(s, d + 1), e.lineTo(h + .5, u), e.lineTo(h - .5, u), e.lineTo(h - .5, d + 1), e.lineTo(o - n, d + 1), e.lineTo(o - n, d)) : (e.moveTo(h, u), e.lineTo(o - n, d + 4.5), e.lineTo(o - n, d + 3.5), e.lineTo(l, d + 3.5), e.lineTo(l, c), e.lineTo(h + .5, c), e.lineTo(h + .5, d + 3.5), e.lineTo(o, d + 3.5), e.lineTo(o, d + 4.5)), e.closePath()
                 }
             }
-            t.HeaderRenderer = o, o.buttonSize = 11, o.iconHeight = 12, o.iconWidth = 7, o.buttonPadding = 3, o.iconSpacing = 1.5
+            t.HeaderRenderer = a, a.buttonSize = 11, a.iconHeight = 12, a.iconWidth = 7, a.buttonPadding = 3, a.iconSpacing = 1.5
+        },
+        2355: (e, t, i) => {
+            var r;
+            Object.defineProperty(t, "__esModule", {
+                value: !0
+            }), t.exportedClass = void 0;
+            const n = i(7930),
+                a = i(6479),
+                o = i(4901),
+                s = i(6988);
+            let l;
+            t.exportedClass = l, a.AsyncCellRenderer && (t.exportedClass = ((r = class e extends a.AsyncCellRenderer {
+                constructor(e = {}) {
+                    super(), this._imgLoaded = new o.Signal(this), this.font = e.font || "12px", this.placeholder = e.placeholder || "...", this.textColor = e.textColor || s.Theme.getFontColor(), this.backgroundColor = e.backgroundColor || s.Theme.getBackgroundColor(), this.verticalAlignment = e.verticalAlignment || "bottom", this.horizontalAlignment = e.horizontalAlignment || "left"
+                }
+                isReady(t) {
+                    return !t.value || void 0 !== e.dataCache.get(t.value)
+                }
+                get imageLoaded() {
+                    return this._imgLoaded
+                }
+                async load(t) {
+                    if (!t.value) return;
+                    const i = t.value,
+                        r = new n.PromiseDelegate;
+                    e.dataCache.set(i, void 0);
+                    const a = new Image;
+                    return a.src = this.htmlToSvg(t), a.width = t.width, a.height = t.height, a.onload = () => {
+                        e.dataCache.set(i, a), r.resolve(), this._imgLoaded.emit()
+                    }, r.promise
+                }
+                paintPlaceholder(e, t) {
+                    this.drawBackground(e, t), this.drawPlaceholder(e, t)
+                }
+                paint(e, t) {
+                    this.drawBackground(e, t), this.drawImage(e, t)
+                }
+                drawBackground(e, t) {
+                    const i = a.CellRenderer.resolveOption(this.backgroundColor, t);
+                    i && (e.fillStyle = i, e.fillRect(t.x, t.y, t.width, t.height))
+                }
+                drawPlaceholder(e, t) {
+                    const i = a.CellRenderer.resolveOption(this.placeholder, t),
+                        r = a.CellRenderer.resolveOption(this.textColor, t),
+                        n = t.x + t.width / 2,
+                        o = t.y + t.height / 2;
+                    e.fillStyle = r, e.fillText(i, n, o)
+                }
+                drawImage(t, i) {
+                    if (!i.value) return;
+                    const r = e.dataCache.get(i.value);
+                    if (!r) return this.drawPlaceholder(t, i);
+                    const n = a.CellRenderer.resolveOption(this.font, i),
+                        o = a.CellRenderer.resolveOption(this.textColor, i),
+                        s = a.TextRenderer.measureFontHeight(n),
+                        l = a.CellRenderer.resolveOption(this.verticalAlignment, i),
+                        d = a.CellRenderer.resolveOption(this.horizontalAlignment, i),
+                        h = i.height - ("center" === l ? 1 : 2);
+                    h <= 0 || (t.textBaseline = "bottom", t.textAlign = d, t.font = n, t.fillStyle = o, s > h && (t.beginPath(), t.rect(i.x, i.y, i.width, i.height - 1), t.clip()), t.drawImage(r, i.x, i.y))
+                }
+                htmlToSvg(e) {
+                    const t = a.CellRenderer.resolveOption(this.font, e),
+                        i = a.CellRenderer.resolveOption(this.textColor, e),
+                        r = a.CellRenderer.resolveOption(this.verticalAlignment, e),
+                        n = a.CellRenderer.resolveOption(this.horizontalAlignment, e),
+                        o = a.CellRenderer.resolveOption(e.width, e),
+                        s = a.CellRenderer.resolveOption(e.height, e),
+                        l = a.CellRenderer.resolveOption(e.value, e);
+                    return "data:image/svg+xml," + encodeURIComponent(`<svg xmlns="http://www.w3.org/2000/svg" width="${o}px" height="${s}px">\n      <foreignObject width="${o}px" height="${s}px">\n        <div\n          xmlns="http://www.w3.org/1999/xhtml"\n          style="display: table-cell; font: ${t}; width: ${o}px; height: ${s}px; color: ${i}; vertical-align: ${"center"===r?"middle":r}; text-align: ${n}"\n        >\n          <div style="display: inline-block; padding: 0 2px">${l}</div>\n        </div>\n      </foreignObject>\n    </svg>`)
+                }
+            }).dataCache = new Map, l = r))
         },
         5091: function(e, t, i) {
             var r = this && this.__createBinding || (Object.create ? function(e, t, i, r) {
                     void 0 === r && (r = i), Object.defineProperty(e, r, {
                         enumerable: !0,
                         get: function() {
                             return t[i]
@@ -1181,176 +1431,183 @@
                     Object.defineProperty(e, "default", {
                         enumerable: !0,
                         value: t
                     })
                 } : function(e, t) {
                     e.default = t
                 }),
-                o = this && this.__importStar || function(e) {
+                a = this && this.__importStar || function(e) {
                     if (e && e.__esModule) return e;
                     var t = {};
                     if (null != e)
                         for (var i in e) "default" !== i && Object.prototype.hasOwnProperty.call(e, i) && r(t, e, i);
                     return n(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.SortExecutor = t.FilterExecutor = t.TransformExecutor = void 0;
-            const a = i(6697),
-                s = o(i(4031));
+            const o = i(4373),
+                s = a(i(4031));
             class l {}
             t.TransformExecutor = l, t.FilterExecutor = class extends l {
                 constructor(e) {
                     super(), this._options = e
                 }
                 apply(e) {
                     let t;
+                    const i = this._options.field;
                     switch (this._options.operator) {
                         case ">":
-                            t = e => {
+                            t = t => {
                                 if (["date", "datetime", "time"].includes(this._options.dType)) {
-                                    const t = s.default.utc(e[this._options.field]),
-                                        i = s.default.utc(this._options.value);
-                                    return t.isAfter(i, "day")
+                                    const r = s.default.utc(e.data[i][t]),
+                                        n = s.default.utc(this._options.value);
+                                    return r.isAfter(n, "day")
                                 }
-                                return e[this._options.field] > this._options.value
+                                return e.data[i][t] > this._options.value
                             };
                             break;
                         case "<":
-                            t = e => {
+                            t = t => {
                                 if (["date", "datetime", "time"].includes(this._options.dType)) {
-                                    const t = s.default.utc(e[this._options.field]),
-                                        i = s.default.utc(this._options.value);
-                                    return t.isBefore(i, "day")
+                                    const r = s.default.utc(e.data[i][t]),
+                                        n = s.default.utc(this._options.value);
+                                    return r.isBefore(n, "day")
                                 }
-                                return e[this._options.field] < this._options.value
+                                return e.data[i][t] < this._options.value
                             };
                             break;
                         case "<=":
-                            t = e => {
+                            t = t => {
                                 if (["date", "datetime", "time"].includes(this._options.dType)) {
-                                    const t = s.default.utc(e[this._options.field]),
-                                        i = s.default.utc(this._options.value);
-                                    return t.isSameOrBefore(i, "day")
+                                    const r = s.default.utc(e.data[i][t]),
+                                        n = s.default.utc(this._options.value);
+                                    return r.isSameOrBefore(n, "day")
                                 }
-                                return e[this._options.field] <= this._options.value
+                                return e.data[i][t] <= this._options.value
                             };
                             break;
                         case ">=":
-                            t = e => {
+                            t = t => {
                                 if (["date", "datetime", "time"].includes(this._options.dType)) {
-                                    const t = s.default.utc(e[this._options.field]),
-                                        i = s.default.utc(this._options.value);
-                                    return t.isSameOrAfter(i, "day")
+                                    const r = s.default.utc(e.data[i][t]),
+                                        n = s.default.utc(this._options.value);
+                                    return r.isSameOrAfter(n, "day")
                                 }
-                                return e[this._options.field] >= this._options.value
+                                return e.data[i][t] >= this._options.value
                             };
                             break;
                         case "=":
-                            t = e => {
+                            t = t => {
                                 if (["date", "datetime", "time"].includes(this._options.dType)) {
-                                    const t = s.default.utc(e[this._options.field]),
-                                        i = s.default.utc(this._options.value);
-                                    return t.isSame(i)
+                                    const r = s.default.utc(e.data[i][t]),
+                                        n = s.default.utc(this._options.value);
+                                    return r.isSame(n)
                                 }
-                                return e[this._options.field] == this._options.value
+                                return e.data[i][t] == this._options.value
                             };
                             break;
                         case "!=":
-                            t = e => {
+                            t = t => {
                                 if (["date", "datetime", "time"].includes(this._options.dType)) {
-                                    const t = s.default.utc(e[this._options.field]),
-                                        i = s.default.utc(this._options.value);
-                                    return !t.isSame(i)
+                                    const r = s.default.utc(e.data[i][t]),
+                                        n = s.default.utc(this._options.value);
+                                    return !r.isSame(n)
                                 }
-                                return e[this._options.field] !== this._options.value
+                                return e.data[i][t] !== this._options.value
                             };
                             break;
                         case "empty":
-                            t = e => null === e[this._options.field];
+                            t = t => null === e.data[i][t];
                             break;
                         case "notempty":
-                            t = e => null !== e[this._options.field];
+                            t = t => null !== e.data[i][t];
                             break;
                         case "in":
-                            t = e => this._options.value.includes(e[this._options.field]);
+                            t = t => this._options.value.includes(e.data[i][t]);
                             break;
                         case "between":
-                            t = e => {
-                                const t = this._options.value;
+                            t = t => {
+                                const r = this._options.value;
                                 if (["date", "datetime", "time"].includes(this._options.dType)) {
-                                    const i = s.default.utc(e[this._options.field]),
-                                        r = s.default.utc(t[0]),
-                                        n = s.default.utc(t[1]);
-                                    return i.isBetween(r, n, "day")
+                                    const n = s.default.utc(e.data[i][t]),
+                                        a = s.default.utc(r[0]),
+                                        o = s.default.utc(r[1]);
+                                    return n.isBetween(a, o, "day")
                                 }
-                                return e[this._options.field] > t[0] && e[this._options.field] < t[1]
+                                return e.data[i][t] > r[0] && e.data[i][t] < r[1]
                             };
                             break;
                         case "startswith":
-                            t = e => e[this._options.field].startsWith(this._options.value);
+                            t = t => e.data[i][t].startsWith(this._options.value);
                             break;
                         case "endswith":
-                            t = e => e[this._options.field].endsWith(this._options.value);
+                            t = t => e.data[i][t].endsWith(this._options.value);
                             break;
                         case "stringContains":
-                            t = e => String(e[this._options.field]).toLowerCase().includes(String(this._options.value).toLowerCase());
+                            t = t => String(e.data[i][t]).toLowerCase().includes(String(this._options.value).toLowerCase());
                             break;
                         case "contains":
-                            t = e => e[this._options.field].includes(this._options.value);
+                            t = t => e.data[i][t].includes(this._options.value);
                             break;
                         case "!contains":
-                            t = e => !e[this._options.field].includes(this._options.value);
+                            t = t => !e.data[i][t].includes(this._options.value);
                             break;
                         case "isOnSameDay":
-                            t = e => {
-                                const t = s.default.utc(e[this._options.field]),
-                                    i = s.default.utc(this._options.value);
-                                return t.isSame(i, "day")
+                            t = t => {
+                                const r = s.default.utc(e.data[i][t]),
+                                    n = s.default.utc(this._options.value);
+                                return r.isSame(n, "day")
                             };
                             break;
                         default:
                             throw "unreachable"
                     }
-                    return {
-                        schema: e.schema,
-                        data: a.toArray(a.filter(e.data, t))
+                    const r = {},
+                        n = Array.from(Array(e.length).keys()).filter(t);
+                    for (const t of Object.keys(e.data)) {
+                        let i = 0;
+                        r[t] = [];
+                        for (const a of n) r[t][i++] = e.data[t][a]
                     }
+                    return new o.DataSource(r, e.fields, e.schema)
                 }
             }, t.SortExecutor = class extends l {
                 constructor(e) {
                     super(), this._options = e
                 }
                 apply(e) {
                     let t;
                     const i = this._options.field,
                         r = this._options.dType,
-                        n = e => "string" != typeof e ? String(e) : e;
-                    t = "string" == r ? this._options.desc ? (e, t) => n(e[i]) < n(t[i]) ? 1 : -1 : (e, t) => n(e[i]) > n(t[i]) ? 1 : -1 : this._options.desc ? (e, t) => e[i] < t[i] ? 1 : -1 : (e, t) => e[i] > t[i] ? 1 : -1;
-                    const o = e.data.slice(0),
-                        a = [],
-                        s = [];
-                    return o.forEach((e => {
-                        const t = e[i];
-                        null === t || "number" == typeof t && Number.isNaN(t) || t instanceof Date && Number.isNaN(t.getTime()) ? s.push(e) : a.push(e)
-                    })), {
-                        schema: e.schema,
-                        data: a.sort(t).concat(s)
+                        n = e => "string" != typeof e ? String(e) : e,
+                        a = e => null === e || "number" == typeof e && Number.isNaN(e) || e instanceof Date && Number.isNaN(e.getTime()),
+                        s = Array.from(Array(e.length).keys()).filter((t => a(e.data[i][t]))),
+                        l = Array.from(Array(e.length).keys()).filter((t => !a(e.data[i][t])));
+                    t = "string" == r ? this._options.desc ? (t, r) => n(e.data[i][t]) < n(e.data[i][r]) ? 1 : -1 : (t, r) => n(e.data[i][t]) > n(e.data[i][r]) ? 1 : -1 : this._options.desc ? (t, r) => e.data[i][t] < e.data[i][r] ? 1 : -1 : (t, r) => e.data[i][t] > e.data[i][r] ? 1 : -1;
+                    const d = {};
+                    let h = l.sort(t);
+                    h = h.concat(s);
+                    for (const t of Object.keys(e.data)) {
+                        let i = 0;
+                        d[t] = [];
+                        for (const r of h) d[t][i++] = e.data[t][r]
                     }
+                    return new o.DataSource(d, e.fields, e.schema)
                 }
             }
         },
         8405: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.TransformStateManager = void 0;
             const r = i(2679),
                 n = i(5091),
-                o = i(6697),
-                a = i(7930),
+                a = i(6697),
+                o = i(7930),
                 s = i(4901);
             t.TransformStateManager = class {
                 constructor() {
                     this._state = {}, this._changed = new s.Signal(this)
                 }
                 _add(e) {
                     switch (this._state.hasOwnProperty(e.columnIndex) || (this._state[e.columnIndex] = {
@@ -1375,51 +1632,51 @@
                             transforms: this.activeTransforms
                         })
                     } catch (e) {
                         this.clear()
                     }
                 }
                 replace(e) {
-                    if (!a.JSONExt.deepEqual(e, this.activeTransforms)) try {
-                        this._state = {}, o.each(e, (e => {
+                    if (!o.JSONExt.deepEqual(e, this.activeTransforms)) try {
+                        this._state = {}, a.each(e, (e => {
                             this._add(e)
                         })), this._changed.emit({
                             type: "transforms-updated",
                             transforms: this.activeTransforms
                         })
                     } catch (e) {
                         this.clear()
                     }
                 }
                 createView(e) {
                     const t = this._createExecutors(e);
                     let i = e;
-                    return o.each(t, (e => {
+                    return a.each(t, (e => {
                         i = e.apply(i)
                     })), new r.View(i)
                 }
                 _createExecutors(e) {
                     const t = [],
                         i = [];
                     return Object.keys(this._state).forEach((r => {
-                        const o = this._state[r];
-                        if (o.sort) {
+                        const a = this._state[r];
+                        if (a.sort) {
                             const i = new n.SortExecutor({
-                                field: e.schema.fields[o.sort.columnIndex].name,
-                                dType: e.schema.fields[o.sort.columnIndex].type,
-                                desc: o.sort.desc
+                                field: e.schema.fields[a.sort.columnIndex].name,
+                                dType: e.schema.fields[a.sort.columnIndex].type,
+                                desc: a.sort.desc
                             });
                             t.push(i)
                         }
-                        if (o.filter) {
+                        if (a.filter) {
                             const t = new n.FilterExecutor({
-                                field: e.schema.fields[o.filter.columnIndex].name,
-                                dType: e.schema.fields[o.filter.columnIndex].type,
-                                operator: o.filter.operator,
-                                value: o.filter.value
+                                field: e.schema.fields[a.filter.columnIndex].name,
+                                dType: e.schema.fields[a.filter.columnIndex].type,
+                                operator: a.filter.operator,
+                                value: a.filter.value
                             });
                             i.push(t)
                         }
                     })), [...i, ...t]
                 }
                 remove(e, t) {
                     if (this._state.hasOwnProperty(e)) try {
@@ -1447,43 +1704,43 @@
                     })
                 }
                 get changed() {
                     return this._changed
                 }
                 get activeTransforms() {
                     const e = [];
-                    return o.each(Object.keys(this._state), (t => {
+                    return a.each(Object.keys(this._state), (t => {
                         this._state[t].sort && e.push(this._state[t].sort), this._state[t].filter && e.push(this._state[t].filter)
                     })), e
                 }
                 getFilterTransform(e) {
                     if (this._state.hasOwnProperty(e)) return this._state[e].filter
                 }
             }
         },
         4080: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.FilterValueRenderer = void 0;
-            const r = i(6092),
+            const r = i(6479),
                 n = i(6988);
-            class o extends r.TextRenderer {
+            class a extends r.TextRenderer {
                 constructor(e) {
                     super({
                         textColor: e.textColor,
                         backgroundColor: e.backgroundColor
                     }), this._stateManager = e.stateManager, this._dialog = e.dialog
                 }
                 drawText(e, t) {
                     const i = r.CellRenderer.resolveOption(this.font, t);
                     if (!i) return;
-                    const o = r.CellRenderer.resolveOption(this.textColor, t);
-                    if (!o) return;
-                    const a = (0, this.format)(t);
+                    const a = r.CellRenderer.resolveOption(this.textColor, t);
                     if (!a) return;
+                    const o = (0, this.format)(t);
+                    if (!o) return;
                     const s = r.CellRenderer.resolveOption(this.verticalAlignment, t),
                         l = r.CellRenderer.resolveOption(this.horizontalAlignment, t),
                         d = t.height - ("center" === s ? 1 : 2);
                     if (d <= 0) return;
                     const h = r.TextRenderer.measureFontHeight(i);
                     let c, u;
                     switch (s) {
@@ -1508,33 +1765,34 @@
                             break;
                         case "right":
                             c = t.x + t.width - 3;
                             break;
                         default:
                             throw "unreachable"
                     }
-                    h > d && (e.beginPath(), e.rect(t.x, t.y, t.width, t.height - 1), e.clip()), e.font = i, e.fillStyle = o, e.textAlign = l, e.textBaseline = "bottom", e.fillText(a, c + 25, u), e.fillStyle = n.Theme.getBorderColor(1), e.fillStyle = "#ffffff", e.fillRect(t.x + 5, t.y + 5, 10, 10), e.fillStyle = "#000000", e.strokeRect(t.x + 5, t.y + 5, 10, 10), this._getCheckedState(t) && (e.beginPath(), e.strokeStyle = "#000000", e.moveTo(t.x + 5 + 3, t.y + 5 + 5), e.lineTo(t.x + 5 + 4, t.y + 5 + 8), e.lineTo(t.x + 5 + 8, t.y + 5 + 2), e.lineWidth = 2, e.stroke())
+                    h > d && (e.beginPath(), e.rect(t.x, t.y, t.width, t.height - 1), e.clip()), e.font = i, e.fillStyle = a, e.textAlign = l, e.textBaseline = "bottom", e.fillText(o, c + 25, u), e.fillStyle = n.Theme.getBorderColor(1), e.fillStyle = "#ffffff", e.fillRect(t.x + 5, t.y + 5, 10, 10), e.fillStyle = "#000000", e.strokeRect(t.x + 5, t.y + 5, 10, 10), this._getCheckedState(t) && (e.beginPath(), e.strokeStyle = "#000000", e.moveTo(t.x + 5 + 3, t.y + 5 + 5), e.lineTo(t.x + 5 + 4, t.y + 5 + 8), e.lineTo(t.x + 5 + 8, t.y + 5 + 2), e.lineWidth = 2, e.stroke())
                 }
                 _getCheckedState(e) {
                     return this._stateManager.has(this._dialog.region, this._dialog.columnIndex, e.value) || !this._dialog.hasFilter && !this._dialog.userInteractedWithDialog
                 }
             }
-            t.FilterValueRenderer = o
+            t.FilterValueRenderer = a
         },
         2679: (e, t) => {
             var i;
             Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.View = void 0, t.View = class {
                     constructor(e) {
                         const t = i.splitFields(e.schema);
-                        this._data = e.data, this._bodyFields = t.bodyFields, this._headerFields = t.headerFields, this._missingValues = i.createMissingMap(e.schema)
+                        this._data = e, this._bodyFields = t.bodyFields, this._headerFields = t.headerFields, this._missingValues = i.createMissingMap(e.schema)
                     }
                     rowCount(e) {
-                        return "body" === e ? this._data.length : this._bodyFields[0].rows.length
+                        var t, i;
+                        return "body" === e ? this._data.length : null !== (i = null === (t = this._bodyFields[0]) || void 0 === t ? void 0 : t.rows.length) && void 0 !== i ? i : 1
                     }
                     columnCount(e) {
                         return "body" === e ? this._bodyFields.length : this._headerFields.length
                     }
                     metadata(e, t, i) {
                         return "body" === e || "column-header" === e ? Object.assign({
                             row: t,
@@ -1544,21 +1802,21 @@
                             column: i
                         }, this._headerFields[i])
                     }
                     data(e, t, i) {
                         let r, n;
                         switch (e) {
                             case "body":
-                                r = this._bodyFields[i], n = this._data[t][r.name];
+                                r = this._bodyFields[i], n = this._data.data[r.name][t];
                                 break;
                             case "column-header":
                                 r = this._bodyFields[i], n = r.rows[t];
                                 break;
                             case "row-header":
-                                r = this._headerFields[i], n = this._data[t][r.name];
+                                r = this._headerFields[i], n = this._data.data[r.name][t];
                                 break;
                             case "corner-header":
                                 r = this._headerFields[i], n = r.rows[t];
                                 break;
                             default:
                                 throw "unreachable"
                         }
@@ -1566,21 +1824,17 @@
                     }
                     get dataset() {
                         return this._data
                     }
                     getSchemaIndex(e, t) {
                         return "corner-header" === e ? t : this._headerFields.length + t
                     }
-                    async uniqueValues(e, t) {
-                        return new Promise(((i, r) => {
-                            const n = this.metadata(e, 0, t).name,
-                                o = new Set;
-                            for (const e of this.dataset) o.add(e[n]);
-                            i(Array.from(o))
-                        }))
+                    uniqueValues(e, t) {
+                        const i = this.metadata(e, 0, t).name;
+                        return Array.from(new Set(this.dataset.data[i]))
                     }
                 },
                 function(e) {
                     e.splitFields = function(e) {
                         let t;
                         t = void 0 === e.primaryKey ? [] : "string" == typeof e.primaryKey ? [e.primaryKey] : e.primaryKey;
                         const i = [],
@@ -1598,58 +1852,56 @@
                     }
                 }(i || (i = {}))
         },
         8785: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.ViewBasedJSONModel = void 0;
-            const r = i(6092),
-                n = i(6697),
-                o = i(7930),
-                a = i(4901),
-                s = i(2679),
-                l = i(8405),
-                d = i(6988);
-            class h extends r.MutableDataModel {
+            const r = i(6479),
+                n = i(4901),
+                a = i(2679),
+                o = i(8405),
+                s = i(6988);
+            class l extends r.MutableDataModel {
                 constructor(e) {
-                    super(), this._transformSignal = new a.Signal(this), this._dataSyncSignal = new a.Signal(this), this._primaryKeyMap = new Map, this.updateDataset(e), this._transformState = new l.TransformStateManager, this._transformState.changed.connect(((e, t) => {
+                    super(), this._transformSignal = new n.Signal(this), this._dataSyncSignal = new n.Signal(this), this._primaryKeyMap = new Map, this.updateDataset(e), this._transformState = new o.TransformStateManager, this._transformState.changed.connect(((e, t) => {
                         this.currentView = this._transformState.createView(this._dataset), this._transformSignal.emit(t)
                     }));
-                    const t = d.ArrayUtils.generateMultiIndexArrayLocations(this);
-                    let i = d.ArrayUtils.generateColMergedCellLocations(this, t);
-                    d.ArrayUtils.validateMergingHierarchy(i) || (i = []), this._mergedColumnCellLocations = i, this._columnCellGroups = d.ArrayUtils.generateColumnCellGroups(this._mergedColumnCellLocations);
-                    let r = d.ArrayUtils.generateRowMergedCellLocations(this);
-                    d.ArrayUtils.validateMergingHierarchy(i) || (r = []), this._rowCellGroups = d.ArrayUtils.generateRowCellGroups(r)
+                    const t = s.ArrayUtils.generateMultiIndexArrayLocations(this);
+                    let i = s.ArrayUtils.generateColMergedCellLocations(this, t);
+                    s.ArrayUtils.validateMergingHierarchy(i) || (i = []), this._mergedColumnCellLocations = i, this._columnCellGroups = s.ArrayUtils.generateColumnCellGroups(this._mergedColumnCellLocations);
+                    let r = s.ArrayUtils.generateRowMergedCellLocations(this);
+                    s.ArrayUtils.validateMergingHierarchy(r) || (r = []), this._mergedRowCellLocations = r, this._rowCellGroups = s.ArrayUtils.generateRowCellGroups(this._mergedRowCellLocations)
                 }
                 updateDataset(e) {
                     this._dataset = e, this._updatePrimaryKeyMap();
-                    const t = new s.View(this._dataset);
+                    const t = new a.View(this._dataset);
                     this.currentView = t
                 }
                 _updatePrimaryKeyMap() {
                     this._primaryKeyMap.clear();
                     const e = this._dataset.schema.primaryKey;
-                    n.each(this._dataset.data, ((t, i) => {
-                        const r = e.map((e => t[e]));
-                        this._primaryKeyMap.set(JSON.stringify(r), i)
-                    }))
+                    for (let t = 0; t < this._dataset.length; t++) {
+                        const i = e.map((e => this._dataset.data[e][t]));
+                        this._primaryKeyMap.set(JSON.stringify(i), t)
+                    }
                 }
                 areCellsMerged(e, t) {
                     const [i, r] = t, n = this.getMergedSiblingCells(e);
                     for (const e of n)
                         if (i === e[0] && r === e[1]) return !0;
                     return !1
                 }
                 getMergedSiblingCells(e) {
                     const [t, i] = e;
                     if (t < 0 || i < 0 || t >= this._mergedColumnCellLocations.length) return [];
                     for (const e of this._mergedColumnCellLocations[t])
                         for (const r of e) {
-                            const [n, o] = r;
-                            if (t === n && i == o) return e
+                            const [n, a] = r;
+                            if (t === n && i == a) return e
                         }
                     return []
                 }
                 rowCount(e) {
                     return this.currentView.rowCount(e)
                 }
                 columnCount(e) {
@@ -1734,19 +1986,20 @@
                     return this._currentView
                 }
                 set currentView(e) {
                     this._currentView = e, this.emitChanged({
                         type: "model-reset"
                     });
                     const t = Array.isArray(this._dataset.schema.primaryKey) ? this._dataset.schema.primaryKey : [this._dataset.schema.primaryKey],
-                        i = e.dataset.map(((e, i) => {
-                            const r = JSON.stringify(t.map((t => e[t]))),
-                                n = this._primaryKeyMap.get(r);
-                            return void 0 === n ? i : n
-                        }));
+                        i = [];
+                    for (let r = 0; r < e.dataset.length; r++) {
+                        const n = JSON.stringify(t.map((t => e.dataset.data[t][r]))),
+                            a = this._primaryKeyMap.get(n);
+                        i.push(void 0 === a ? r : a)
+                    }
                     this.dataSync.emit({
                         type: "row-indices-updated",
                         indices: i
                     })
                 }
                 addTransform(e) {
                     this._transformState.add(e)
@@ -1759,21 +2012,17 @@
                 }
                 clearTransforms() {
                     this._transformState.clear()
                 }
                 transformMetadata(e) {
                     return this._transformState.metadata(e)
                 }
-                async uniqueValues(e, t) {
-                    return new Promise(((i, r) => {
-                        const n = this.metadata(e, 0, t).name,
-                            o = new Set;
-                        for (const e of this.dataset.data) o.add(e[n]);
-                        i(Array.from(o))
-                    }))
+                uniqueValues(e, t) {
+                    const i = this.metadata(e, 0, t).name;
+                    return Array.from(new Set(this.dataset.data[i]))
                 }
                 async uniqueValuesVisible(e, t) {
                     return this._currentView.uniqueValues(e, t)
                 }
                 get transformStateChanged() {
                     return this._transformSignal
                 }
@@ -1781,66 +2030,47 @@
                     return this._transformState.activeTransforms
                 }
                 getFilterTransform(e) {
                     return this._transformState.getFilterTransform(e)
                 }
                 getDatasetRowFromView(e, t) {
                     if ("column-header" == e || "corner-header" == e) return t;
-                    const i = (Array.isArray(this._dataset.schema.primaryKey) ? this._dataset.schema.primaryKey : [this._dataset.schema.primaryKey]).map((e => this._currentView.dataset[t][e]));
+                    const i = (Array.isArray(this._dataset.schema.primaryKey) ? this._dataset.schema.primaryKey : [this._dataset.schema.primaryKey]).map((e => this._currentView.dataset.data[e][t]));
                     return this._primaryKeyMap.get(JSON.stringify(i))
                 }
                 updateCellValue(e) {
                     if ("body" !== e.region) return;
-                    const t = Object.assign({}, this._dataset.data[e.row]);
-                    t[this.metadata("body", 0, e.column).name] = e.value;
-                    const i = Array.from(this._dataset.data);
-                    i[e.row] = t, this._dataset = {
-                        data: i,
-                        schema: this._dataset.schema
-                    }, e.syncData && this.dataSync.emit({
-                        type: "cell-updated"
-                    }), this.dataSync.emit({
+                    const t = this.metadata("body", 0, e.column).name;
+                    this._dataset.data[t][e.row] = e.value, this.dataSync.emit({
                         type: "cell-edit-event",
+                        column: t,
                         columnIndex: e.column,
                         row: e.row,
                         region: e.region,
                         value: e.value
                     }), this.currentView = this._transformState.createView(this._dataset)
                 }
                 updateRowValue(e) {
-                    const t = Object.assign({}, this._dataset.data[e.row]);
-                    for (const i of Array(e.value.length).keys()) t[this.metadata("body", 0, i).name] = e.value[i];
-                    const i = Array.from(this._dataset.data);
-                    i[e.row] = t, this._dataset = {
-                        data: i,
-                        schema: this._dataset.schema
-                    }, e.syncData && this.dataSync.emit({
-                        type: "cell-updated"
-                    }), this.currentView = this._transformState.createView(this._dataset)
+                    for (const t of Array(e.value.length).keys()) {
+                        const i = this.metadata("body", 0, t).name;
+                        this._dataset.data[i][e.row] = e.value[t]
+                    }
+                    this.currentView = this._transformState.createView(this._dataset)
                 }
                 get dataSync() {
                     return this._dataSyncSignal
                 }
                 get dataset() {
                     return this._dataset
                 }
                 getSchemaIndex(e, t) {
                     return this.currentView.getSchemaIndex(e, t)
                 }
-                static fromJsonData(e) {
-                    const t = "ipydguuid",
-                        i = o.JSONExt.deepCopy(e);
-                    i.schema.primaryKeyUuid = t;
-                    for (const e of i.schema.fields) e.rows = [e.name];
-                    let r = 0;
-                    for (const e of i.data) e[t] = r++;
-                    return new h(i)
-                }
             }
-            t.ViewBasedJSONModel = h
+            t.ViewBasedJSONModel = l
         },
         5787: function(e, t, i) {
             var r = this && this.__createBinding || (Object.create ? function(e, t, i, r) {
                     void 0 === r && (r = i), Object.defineProperty(e, r, {
                         enumerable: !0,
                         get: function() {
                             return t[i]
@@ -1853,46 +2083,64 @@
                     Object.defineProperty(e, "default", {
                         enumerable: !0,
                         value: t
                     })
                 } : function(e, t) {
                     e.default = t
                 }),
-                o = this && this.__importStar || function(e) {
+                a = this && this.__importStar || function(e) {
                     if (e && e.__esModule) return e;
                     var t = {};
                     if (null != e)
                         for (var i in e) "default" !== i && Object.prototype.hasOwnProperty.call(e, i) && r(t, e, i);
                     return n(t, e), t
                 };
             Object.defineProperty(t, "__esModule", {
                 value: !0
-            }), t.VegaExprView = t.VegaExprModel = t.TextRendererView = t.TextRendererModel = t.HyperlinkRendererView = t.HyperlinkRendererModel = t.BarRendererView = t.BarRendererModel = t.DataGridView = t.DataGridModel = void 0;
-            const a = o(i(2297)),
-                s = i(6092),
+            }), t.VegaExprView = t.VegaExprModel = t.HtmlRendererView = t.HtmlRendererModel = t.TextRendererView = t.TextRendererModel = t.HyperlinkRendererView = t.HyperlinkRendererModel = t.ImageRendererView = t.ImageRendererModel = t.BarRendererView = t.BarRendererModel = t.DataGridView = t.DataGridModel = void 0;
+            const o = a(i(2297)),
+                s = i(6479),
                 l = i(7930),
                 d = i(5633),
-                h = i(8778),
+                h = i(4882),
                 c = i(6664),
-                u = i(8785),
+                u = i(2544),
+                m = i(8785),
                 g = i(8657),
-                m = i(9453),
-                p = i(6988);
+                p = i(9453),
+                _ = i(6988),
+                f = i(4373);
+
+            function b(e) {
+                if (Array.isArray(e)) {
+                    const t = [];
+                    return e.forEach(((e, i) => {
+                        t.push(b(e))
+                    })), t
+                }
+                if (e instanceof Object && "string" != typeof e) {
+                    const t = {};
+                    return Object.keys(e).forEach((i => {
+                        t[i] = b(e[i])
+                    })), t
+                }
+                return "$NaN$" === e ? Number.NaN : "$Infinity$" === e ? Number.POSITIVE_INFINITY : "$NegInfinity$" === e ? Number.NEGATIVE_INFINITY : "$NaT$" === e ? new Date("INVALID") : e
+            }
             i(3058);
-            class _ extends c.DOMWidgetModel {
+            class y extends c.DOMWidgetModel {
                 constructor() {
                     super(...arguments), this.synchingWithKernel = !1
                 }
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_module: _.model_module,
-                        _model_module_version: _.model_module_version,
-                        _view_name: _.view_name,
-                        _view_module: _.view_module,
-                        _view_module_version: _.view_module_version,
+                        _model_module: y.model_module,
+                        _model_module_version: y.model_module_version,
+                        _view_name: y.view_name,
+                        _view_module: y.view_module,
+                        _view_module_version: y.view_module_version,
                         _visible_rows: [],
                         _transforms: [],
                         baseRowSize: 20,
                         baseColumnSize: 64,
                         baseRowHeaderSize: 64,
                         baseColumnHeaderSize: 20,
                         headerVisibility: "all",
@@ -1901,57 +2149,50 @@
                         corner_renderer: null,
                         default_renderer: null,
                         header_renderer: null,
                         selection_mode: "none",
                         selections: [],
                         grid_style: {},
                         editable: !1,
-                        column_widths: {}
+                        column_widths: {},
+                        horizontal_stripes: !1,
+                        vertical_stripes: !1
                     })
                 }
                 initialize(e, t) {
                     super.initialize(e, t), this.updateDataSync = this.updateDataSync.bind(this), this.syncTransformState = this.syncTransformState.bind(this), this.on("change:_data", this.updateData.bind(this)), this.on("change:_transforms", this.updateTransforms.bind(this)), this.on("change:selection_mode", this.updateSelectionModel, this), this.on("change:selections", this.updateSelections, this), this.updateData(), this.updateTransforms(), this.updateSelectionModel(), this.on("msg:custom", (e => {
                         "cell-changed" === e.event_type && this.data_model.setModelData("body", e.row, e.column_index, e.value), "row-changed" === e.event_type && this.data_model.setRowData(e.row, e.value)
                     }))
                 }
                 updateDataSync(e, t) {
                     switch (t.type) {
                         case "row-indices-updated":
                             this.set("_visible_rows", t.indices), this.save_changes();
                             break;
-                        case "cell-updated":
-                            this.set("_data", this.data_model.dataset), this.save_changes();
-                            break;
                         case "cell-edit-event":
                             const e = this.get("_data");
-                            e.data[t.row][t.columnIndex] = t.value, this.set("_data", e), this.send({
+                            e.data[t.column][t.row] = t.value, this.set("_data", e), this.send({
                                 event_type: "cell-changed",
                                 region: t.region,
                                 row: t.row,
+                                column: t.column,
                                 column_index: t.columnIndex,
                                 value: t.value
                             }, Object.assign({}, this._view_callbacks));
                             break;
                         default:
                             throw "unreachable"
                     }
                 }
                 syncTransformState(e, t) {
                     this.set("_transforms", t.transforms), this.save_changes()
                 }
                 updateData() {
-                    const e = this.data,
-                        t = b.createSchema(e);
-                    this.data_model && (this.data_model.updateDataset({
-                        data: e.data,
-                        schema: t
-                    }), this.data_model.transformStateChanged.disconnect(this.syncTransformState), this.data_model.dataSync.disconnect(this.updateDataSync)), this.data_model = new u.ViewBasedJSONModel({
-                        data: e.data,
-                        schema: t
-                    }), this.data_model.transformStateChanged.connect(this.syncTransformState), this.data_model.dataSync.connect(this.updateDataSync), this.updateTransforms(), this.trigger("data-model-changed"), this.updateSelectionModel()
+                    const e = this.data;
+                    this.data_model && (this.data_model.updateDataset(e), this.data_model.transformStateChanged.disconnect(this.syncTransformState), this.data_model.dataSync.disconnect(this.updateDataSync)), this.data_model = new m.ViewBasedJSONModel(this.data), this.data_model.transformStateChanged.connect(this.syncTransformState), this.data_model.dataSync.connect(this.updateDataSync), this.updateTransforms(), this.trigger("data-model-changed"), this.updateSelectionModel()
                 }
                 updateTransforms() {
                     this.selectionModel && this.selectionModel.clear(), this.data_model.replaceTransforms(this.get("_transforms"))
                 }
                 updateSelectionModel() {
                     this.selectionModel && this.selectionModel.clear();
                     const e = this.get("selection_mode");
@@ -2002,15 +2243,15 @@
                     });
                     this.synchingWithKernel = !1
                 }
                 get data() {
                     return this.get("_data")
                 }
             }
-            t.DataGridModel = _, _.serializers = Object.assign(Object.assign({}, c.DOMWidgetModel.serializers), {
+            t.DataGridModel = y, y.serializers = Object.assign(Object.assign({}, c.DOMWidgetModel.serializers), {
                 transforms: {
                     deserialize: c.unpack_models
                 },
                 renderers: {
                     deserialize: c.unpack_models
                 },
                 corner_renderer: {
@@ -2019,28 +2260,27 @@
                 default_renderer: {
                     deserialize: c.unpack_models
                 },
                 header_renderer: {
                     deserialize: c.unpack_models
                 },
                 _data: {
-                    deserialize: function e(t, i) {
-                        if (Array.isArray(t)) {
-                            const r = [];
-                            return t.forEach(((t, n) => {
-                                r.push(e(t, i))
-                            })), Promise.all(r)
-                        }
-                        if (t instanceof Object && "string" != typeof t) {
-                            const r = {};
-                            return Object.keys(t).forEach((n => {
-                                r[n] = e(t[n], i)
-                            })), c.resolvePromisesDict(r)
+                    deserialize: function(e, t) {
+                        const i = {};
+                        for (const r of Object.keys(e.data)) "raw" == e.data[r].type ? i[r] = b(e.data[r].value) : i[r] = u.array_or_json_serializer.deserialize(e.data[r], t);
+                        return new f.DataSource(i, e.fields, e.schema, !0)
+                    },
+                    serialize: function(e, t) {
+                        const i = {};
+                        for (const r of Object.keys(e.data)) i[r] = u.array_or_json_serializer.serialize(e.data[r], t);
+                        return {
+                            data: i,
+                            fields: e.fields,
+                            schema: e.schema
                         }
-                        return "$NaN$" === t ? Promise.resolve(Number.NaN) : "$Infinity$" === t ? Promise.resolve(Number.POSITIVE_INFINITY) : "$NegInfinity$" === t ? Promise.resolve(Number.NEGATIVE_INFINITY) : "$NaT$" === t ? Promise.resolve(new Date("INVALID")) : Promise.resolve(t)
                     }
                 },
                 grid_style: {
                     deserialize: function e(t, i) {
                         if (t instanceof Object && "string" != typeof t) {
                             const r = {};
                             return Object.keys(t).forEach((n => {
@@ -2054,23 +2294,23 @@
                                     return t.join("")
                                 }(n)] = e(t[n], i)
                             })), c.resolvePromisesDict(r)
                         }
                         return "string" == typeof t && "IPY_MODEL_" === t.slice(0, 10) ? Promise.resolve(i.get_model(t.slice(10, t.length))).then((e => e._function)) : Promise.resolve(t)
                     }
                 }
-            }), _.model_name = "DataGridModel", _.model_module = g.MODULE_NAME, _.model_module_version = g.MODULE_VERSION, _.view_name = "DataGridView", _.view_module = g.MODULE_NAME, _.view_module_version = g.MODULE_VERSION;
-            class f extends c.DOMWidgetView {
+            }), y.model_name = "DataGridModel", y.model_module = g.MODULE_NAME, y.model_module_version = g.MODULE_VERSION, y.view_name = "DataGridView", y.view_module = g.MODULE_NAME, y.view_module_version = g.MODULE_VERSION;
+            class w extends c.DOMWidgetView {
                 constructor() {
                     super(...arguments), this.manageResizeEvent = () => {
                         d.MessageLoop.postMessage(this.luminoWidget, h.Widget.ResizeMessage.UnknownSize)
                     }
                 }
                 _createElement(e) {
-                    const t = b.getWidgetPanel();
+                    const t = C.getWidgetPanel();
                     return this.luminoWidget = new t({
                         view: this
                     }), this._initializeTheme(), this.luminoWidget.node
                 }
                 get pWidget() {
                     return this.luminoWidget
                 }
@@ -2084,25 +2324,27 @@
                 processLuminoMessage(e) {
                     this._processLuminoMessage(e, super.processLuminoMessage)
                 }
                 processPhosphorMessage(e) {
                     this._processLuminoMessage(e, super.processPhosphorMessage)
                 }
                 render() {
-                    return this.el.classList.add("datagrid-container"), window.addEventListener("resize", this.manageResizeEvent), this.once("remove", (() => {
+                    this.el.classList.add("datagrid-container"), window.addEventListener("resize", this.manageResizeEvent), this.once("remove", (() => {
                         window.removeEventListener("resize", this.manageResizeEvent)
-                    })), this.grid = new m.FeatherGrid({
+                    }));
+                    const e = this.model.get("grid_style");
+                    return (this.model.get("horizontal_stripes") || this.model.get("vertical_stripes")) && (e[this.model.get("horizontal_stripes") ? "rowBackgroundColor" : "columnBackgroundColor"] = e => e % 2 == 0 ? _.Theme.getBackgroundColor(1) : _.Theme.getBackgroundColor(2)), this.grid = new p.FeatherGrid({
                         defaultSizes: {
                             rowHeight: this.model.get("base_row_size"),
                             columnWidth: this.model.get("base_column_size"),
                             rowHeaderWidth: this.model.get("base_row_header_size"),
                             columnHeaderHeight: this.model.get("base_column_header_size")
                         },
                         headerVisibility: this.model.get("header_visibility"),
-                        style: this.model.get("grid_style")
+                        style: e
                     }), this.grid.columnWidths = this.model.get("column_widths"), this.grid.editable = this.model.get("editable"), this.grid.isLightTheme = this._isLightTheme, this.grid.dataModel = this.model.data_model, this.grid.selectionModel = this.model.selectionModel, this.grid.backboneModel = this.model, this.grid.cellClicked.connect(((e, t) => {
                         this.model.comm && this.send({
                             event_type: "cell-click",
                             region: t.region,
                             column: t.column,
                             column_index: t.columnIndex,
                             row: t.row,
@@ -2159,15 +2401,15 @@
                         this.corner_renderer = e, this.listenTo(this.corner_renderer, "renderer-changed", this.updateGridRenderers.bind(this))
                     })));
                     const r = this.model.get("header_renderer");
                     r && e.push(this.create_child_view(r).then((e => {
                         this.header_renderer = e, this.listenTo(this.header_renderer, "renderer-changed", this.updateGridRenderers.bind(this))
                     })));
                     const n = {};
-                    return a.each(this.model.get("renderers"), ((e, t) => {
+                    return o.each(this.model.get("renderers"), ((e, t) => {
                         n[t] = this.create_child_view(e)
                     })), e.push(c.resolvePromisesDict(n).then((e => {
                         this.renderers = e;
                         for (const t in e) this.listenTo(e[t], "renderer-changed", this.updateGridRenderers.bind(this))
                     }))), Promise.all(e)
                 }
                 updateGridStyle() {
@@ -2177,123 +2419,164 @@
                     this._isLightTheme = e, this.grid && (this.grid.isLightTheme = e)
                 }
                 get isLightTheme() {
                     return this._isLightTheme
                 }
                 updateGridRenderers() {
                     let e = this.default_renderer.renderer;
-                    (this.grid.grid.style.backgroundColor !== p.Theme.getBackgroundColor() || this.grid.grid.style.rowBackgroundColor || this.grid.grid.style.columnBackgroundColor) && (e = new s.TextRenderer(Object.assign(Object.assign({}, this.default_renderer.renderer), {
+                    (this.grid.grid.style.backgroundColor !== _.Theme.getBackgroundColor() || this.grid.grid.style.rowBackgroundColor || this.grid.grid.style.columnBackgroundColor) && (e = new s.TextRenderer(Object.assign(Object.assign({}, this.default_renderer.renderer), {
                         backgroundColor: void 0
                     })));
                     const t = null !== this.model.get("header_renderer");
                     let i = null;
                     i = this.header_renderer && t ? this.header_renderer.renderer : new s.TextRenderer({
                         font: "12px sans-serif",
-                        textColor: p.Theme.getFontColor(),
-                        backgroundColor: p.Theme.getBackgroundColor(2)
+                        textColor: _.Theme.getFontColor(),
+                        backgroundColor: _.Theme.getBackgroundColor(2)
                     });
                     let r = null;
                     this.corner_renderer && (r = this.corner_renderer.renderer);
                     const n = {};
                     Object.entries(this.renderers).forEach((([e, t]) => {
                         n[e] = t.renderer
                     })), this.grid.defaultRenderer = e, this.grid.columnHeaderRenderer = i, r && (this.grid.cornerHeaderRenderer = r), this.grid.renderers = n
                 }
                 _initializeTheme() {
                     void 0 === this._isLightTheme && (this._isLightTheme = !(document.body.classList.contains("theme-dark") || "false" === document.body.dataset.jpThemeLight))
                 }
             }
-            t.DataGridView = f;
-            var y = i(2509);
+            t.DataGridView = w;
+            var v = i(2509);
             Object.defineProperty(t, "BarRendererModel", {
                 enumerable: !0,
                 get: function() {
-                    return y.BarRendererModel
+                    return v.BarRendererModel
                 }
             }), Object.defineProperty(t, "BarRendererView", {
                 enumerable: !0,
                 get: function() {
-                    return y.BarRendererView
+                    return v.BarRendererView
+                }
+            }), Object.defineProperty(t, "ImageRendererModel", {
+                enumerable: !0,
+                get: function() {
+                    return v.ImageRendererModel
+                }
+            }), Object.defineProperty(t, "ImageRendererView", {
+                enumerable: !0,
+                get: function() {
+                    return v.ImageRendererView
                 }
             }), Object.defineProperty(t, "HyperlinkRendererModel", {
                 enumerable: !0,
                 get: function() {
-                    return y.HyperlinkRendererModel
+                    return v.HyperlinkRendererModel
                 }
             }), Object.defineProperty(t, "HyperlinkRendererView", {
                 enumerable: !0,
                 get: function() {
-                    return y.HyperlinkRendererView
+                    return v.HyperlinkRendererView
                 }
             }), Object.defineProperty(t, "TextRendererModel", {
                 enumerable: !0,
                 get: function() {
-                    return y.TextRendererModel
+                    return v.TextRendererModel
                 }
             }), Object.defineProperty(t, "TextRendererView", {
                 enumerable: !0,
                 get: function() {
-                    return y.TextRendererView
+                    return v.TextRendererView
+                }
+            }), Object.defineProperty(t, "HtmlRendererModel", {
+                enumerable: !0,
+                get: function() {
+                    return v.HtmlRendererModel
+                }
+            }), Object.defineProperty(t, "HtmlRendererView", {
+                enumerable: !0,
+                get: function() {
+                    return v.HtmlRendererView
                 }
             });
-            var b, w = i(2584);
+            var C, x = i(2584);
             Object.defineProperty(t, "VegaExprModel", {
                     enumerable: !0,
                     get: function() {
-                        return w.VegaExprModel
+                        return x.VegaExprModel
                     }
                 }), Object.defineProperty(t, "VegaExprView", {
                     enumerable: !0,
                     get: function() {
-                        return w.VegaExprView
+                        return x.VegaExprView
                     }
                 }),
                 function(e) {
                     e.getWidgetPanel = function() {
                         return null !== c.JupyterLuminoPanelWidget && void 0 !== c.JupyterLuminoPanelWidget ? c.JupyterLuminoPanelWidget : c.JupyterPhosphorPanelWidget
-                    }, e.createSchema = function(e) {
-                        const t = [];
-                        return e.fields.forEach(((i, r) => {
-                            const n = Array.isArray(e.schema.fields[r].name) ? e.schema.fields[r].name : [e.schema.fields[r].name],
-                                o = {
-                                    name: Object.keys(i)[0],
-                                    type: e.schema.fields[r].type,
-                                    rows: n
-                                };
-                            t.push(o)
-                        })), {
-                            primaryKey: e.schema.primaryKey.map((t => {
-                                for (let i = 0; i < e.schema.fields.length; i++)
-                                    if ((Array.isArray(t) ? e.schema.fields[i].name[0] : e.schema.fields[i].name) == (Array.isArray(t) ? t[0] : t)) return Object.keys(e.fields[i])[0];
-                                return "unreachable"
-                            })),
-                            primaryKeyUuid: e.schema.primaryKeyUuid,
-                            fields: t
-                        }
                     }
-                }(b || (b = {}))
+                }(C || (C = {}))
+        },
+        4373: (e, t) => {
+            Object.defineProperty(t, "__esModule", {
+                value: !0
+            }), t.DataSource = void 0, t.DataSource = class {
+                constructor(e, t, i, r = !1) {
+                    this._data = Object.assign({}, e), r ? (this._fields = t, this._schema = this._createSchema(t, i)) : (this._fields = t, this._schema = i), this._columns = Object.keys(this._data)
+                }
+                get data() {
+                    return this._data
+                }
+                get fields() {
+                    return this._fields
+                }
+                get schema() {
+                    return this._schema
+                }
+                get length() {
+                    return 0 == this._columns.length ? 0 : this._data[this._columns[0]].length
+                }
+                _createSchema(e, t) {
+                    const i = [];
+                    return e.forEach(((e, r) => {
+                        const n = Array.isArray(t.fields[r].name) ? t.fields[r].name : [t.fields[r].name],
+                            a = {
+                                name: Object.keys(e)[0],
+                                type: t.fields[r].type,
+                                rows: n
+                            };
+                        i.push(a)
+                    })), {
+                        primaryKey: t.primaryKey.map((i => {
+                            for (let r = 0; r < t.fields.length; r++)
+                                if ((Array.isArray(i) ? t.fields[r].name[0] : t.fields[r].name) == (Array.isArray(i) ? i[0] : i)) return Object.keys(e[r])[0];
+                            return "unreachable"
+                        })),
+                        primaryKeyUuid: t.primaryKeyUuid,
+                        fields: i
+                    }
+                }
+            }
         },
         9453: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.FeatherGrid = void 0;
-            const r = i(6697),
-                n = i(7120),
-                o = i(6092),
+            const r = i(7120),
+                n = i(6479),
                 a = i(5633),
-                s = i(4901),
-                l = i(8778),
-                d = i(8126),
-                h = i(6175),
-                c = i(2320),
-                u = i(4377),
-                g = i(591),
+                o = i(4901),
+                s = i(4882),
+                l = i(8126),
+                d = i(6175),
+                h = i(2320),
+                c = i(4377),
+                u = i(591),
                 m = i(6988);
             i(6229), i(1318);
-            const p = new Map([
+            const g = new Map([
                 ["--ipydatagrid-filter-icon", ["var(--ipydatagrid-filter-icon-light)", "var(--ipydatagrid-filter-icon-dark)"]],
                 ["--ipydatagrid-sort-asc-icon", ["var(--ipydatagrid-sort-asc-icon-light)", "var(--ipydatagrid-sort-asc-icon-dark)"]],
                 ["--ipydatagrid-sort-desc-icon", ["var(--ipydatagrid-sort-desc-icon-light)", "var(--ipydatagrid-sort-desc-icon-dark)"]],
                 ["--ipydatagrid-layout-color0", ["white", "#111111"]],
                 ["--ipydatagrid-layout-color1", ["white", "#212121"]],
                 ["--ipydatagrid-layout-color2", ["#eeeeee", "#424242"]],
                 ["--ipydatagrid-layout-color3", ["#bdbdbd", "#616161"]],
@@ -2316,28 +2599,28 @@
                 ["--ipydatagrid-brand-color7", ["#009eb0", "#009eb0"]],
                 ["--ipydatagrid-brand-color8", ["#b09b00", "#b09b00"]],
                 ["--ipydatagrid-menu-bgcolor", ["white", "black"]],
                 ["--ipydatagrid-menu-border-color", ["#bdbdbd", "#616161"]],
                 ["--ipydatagrid-filter-dlg-textcolor", ["black", "white"]],
                 ["--ipydatagrid-filter-dlg-bgcolor", ["white", "black"]]
             ]);
-            class _ extends l.Widget {
+            class p extends s.Widget {
                 constructor(e = {}) {
-                    super(), this._baseRowSize = 20, this._baseColumnSize = 64, this._baseRowHeaderSize = 64, this._baseColumnHeaderSize = 20, this._columnWidths = {}, this._headerVisibility = "all", this._renderers = {}, this._defaultRendererSet = !1, this._cellClicked = new s.Signal(this), this._columnsResized = new s.Signal(this), this._isLightTheme = !0, this.addClass("ipydatagrid-widget"), e.defaultSizes && (this._baseRowSize = e.defaultSizes.rowHeight || this._baseRowSize, this._baseColumnSize = e.defaultSizes.columnWidth || this._baseColumnSize, this._baseRowHeaderSize = e.defaultSizes.rowHeaderWidth || this._baseRowHeaderSize, this._baseColumnHeaderSize = e.defaultSizes.columnHeaderHeight || this._baseColumnHeaderSize), this._headerVisibility = e.headerVisibility || this._headerVisibility, this._createGrid(e), this._defaultRenderer = new o.TextRenderer({
+                    super(), this._baseRowSize = 20, this._baseColumnSize = 64, this._baseRowHeaderSize = 64, this._baseColumnHeaderSize = 20, this._columnWidths = {}, this._headerVisibility = "all", this._renderers = {}, this._defaultRendererSet = !1, this._cellClicked = new o.Signal(this), this._columnsResized = new o.Signal(this), this._isLightTheme = !0, this.addClass("ipydatagrid-widget"), e.defaultSizes && (this._baseRowSize = e.defaultSizes.rowHeight || this._baseRowSize, this._baseColumnSize = e.defaultSizes.columnWidth || this._baseColumnSize, this._baseRowHeaderSize = e.defaultSizes.rowHeaderWidth || this._baseRowHeaderSize, this._baseColumnHeaderSize = e.defaultSizes.columnHeaderHeight || this._baseColumnHeaderSize), this._headerVisibility = e.headerVisibility || this._headerVisibility, this._createGrid(e), this._defaultRenderer = new n.TextRenderer({
                         font: "12px sans-serif",
                         textColor: m.Theme.getFontColor(),
                         backgroundColor: this.grid.style.backgroundColor || m.Theme.getBackgroundColor(),
                         horizontalAlignment: "center",
                         verticalAlignment: "center"
-                    }), this._rowHeaderRenderer = new o.TextRenderer({
+                    }), this._rowHeaderRenderer = new n.TextRenderer({
                         textColor: m.Theme.getFontColor(1),
                         backgroundColor: this.grid.style.headerBackgroundColor || m.Theme.getBackgroundColor(2),
                         horizontalAlignment: "center",
                         verticalAlignment: "center"
-                    }), (this.layout = new l.PanelLayout).addWidget(this.grid)
+                    }), (this.layout = new s.PanelLayout).addWidget(this.grid)
                 }
                 messageHook(e, t) {
                     if (e === this.grid.viewport) {
                         const e = this.grid.mouseHandler;
                         if ("column-resize-request" === t.type && e.mouseIsDown) {
                             const e = t,
                                 i = this.dataModel.columnIndexToName(e.index, e.region);
@@ -2400,15 +2683,15 @@
                     this._defaultRenderer = e, this._defaultRendererSet = !0, this.grid && this._updateGridRenderers()
                 }
                 get defaultRenderer() {
                     return this._defaultRenderer
                 }
                 set columnHeaderRenderer(e) {
                     const t = e;
-                    this._columnHeaderRenderer = new c.HeaderRenderer({
+                    this._columnHeaderRenderer = new h.HeaderRenderer({
                         textOptions: {
                             font: t.font,
                             wrapText: t.wrapText,
                             elideDirection: t.elideDirection,
                             textColor: t.textColor,
                             backgroundColor: this.grid.style.headerBackgroundColor || t.backgroundColor || m.Theme.getBackgroundColor(),
                             verticalAlignment: t.verticalAlignment,
@@ -2420,15 +2703,15 @@
                     }), this.grid && this._updateHeaderRenderer()
                 }
                 get columnHeaderRenderer() {
                     return this._columnHeaderRenderer
                 }
                 set cornerHeaderRenderer(e) {
                     const t = e;
-                    this._cornerHeaderRenderer = new c.HeaderRenderer({
+                    this._cornerHeaderRenderer = new h.HeaderRenderer({
                         textOptions: {
                             font: t.font,
                             wrapText: t.wrapText,
                             elideDirection: t.elideDirection,
                             textColor: t.textColor,
                             backgroundColor: this.grid.style.headerBackgroundColor || t.backgroundColor || m.Theme.getBackgroundColor(),
                             verticalAlignment: t.verticalAlignment,
@@ -2457,29 +2740,29 @@
                 get editable() {
                     return this._editable
                 }
                 get cellRenderers() {
                     return this.grid.cellRenderers
                 }
                 _createGrid(e = {}) {
-                    this.grid = new o.DataGrid(Object.assign(Object.assign({}, e), {
+                    this.grid = new n.DataGrid(Object.assign(Object.assign({}, e), {
                         defaultSizes: {
                             rowHeight: this._baseRowSize,
                             columnWidth: this._baseColumnSize,
                             rowHeaderWidth: this._baseRowHeaderSize,
                             columnHeaderHeight: this._baseColumnHeaderSize
                         },
                         headerVisibility: this._headerVisibility
-                    })), a.MessageLoop.installMessageHook(this.grid.viewport, this), this._filterDialog = new d.InteractiveFilterDialog({
+                    })), a.MessageLoop.installMessageHook(this.grid.viewport, this), this._filterDialog = new l.InteractiveFilterDialog({
                         model: this._dataModel
-                    }), this.contextMenu = new h.FeatherGridContextMenu({
+                    }), this.contextMenu = new d.FeatherGridContextMenu({
                         grid: this.grid,
                         commands: this._createCommandRegistry()
-                    }), this.grid.copyToClipboard = this.copyToClipboard.bind(this.grid), this.grid.dataModel = this._dataModel, this.grid.keyHandler = new u.KeyHandler;
-                    const t = new g.MouseHandler(this);
+                    }), this.grid.dataModel = this._dataModel, this.grid.keyHandler = new c.KeyHandler;
+                    const t = new u.MouseHandler(this);
                     t.cellClicked.connect(((e, t) => {
                         if (!this.grid.dataModel) return;
                         const i = this.grid.dataModel,
                             r = t.region;
                         this._cellClicked.emit({
                             region: r,
                             column: i.metadata(r, t.row, t.column).name,
@@ -2527,125 +2810,121 @@
                         headerSelectionBorderColor: m.Theme.getBorderColor(1),
                         cursorFillColor: m.Theme.getBrandColor(3, .4),
                         cursorBorderColor: m.Theme.getBrandColor(1),
                         scrollShadow: e
                     }
                 }
                 updateGridStyle() {
-                    this.setGridStyle(), this._defaultRendererSet && this.backboneModel || (this.defaultRenderer = new o.TextRenderer({
+                    this.setGridStyle(), this._defaultRendererSet && this.backboneModel || (this.defaultRenderer = new n.TextRenderer({
                         font: "12px sans-serif",
                         textColor: m.Theme.getFontColor(),
                         backgroundColor: this.grid.style.backgroundColor || m.Theme.getBackgroundColor(),
                         horizontalAlignment: "left",
                         verticalAlignment: "center"
-                    })), this._rowHeaderRenderer = new o.TextRenderer({
+                    })), this._rowHeaderRenderer = new n.TextRenderer({
                         textColor: m.Theme.getFontColor(1),
                         backgroundColor: this.grid.style.headerBackgroundColor || m.Theme.getBackgroundColor(2),
                         horizontalAlignment: "center",
                         verticalAlignment: "center"
-                    }), this._columnHeaderRenderer = new c.HeaderRenderer({
+                    }), this._columnHeaderRenderer = new h.HeaderRenderer({
                         textOptions: {
                             textColor: m.Theme.getFontColor(1),
                             backgroundColor: this.grid.style.headerBackgroundColor || m.Theme.getBackgroundColor(2),
                             horizontalAlignment: "left",
                             verticalAlignment: "center"
                         },
                         isLightTheme: this._isLightTheme,
                         grid: this.grid
-                    }), this._cornerHeaderRenderer = new c.HeaderRenderer({
+                    }), this._cornerHeaderRenderer = new h.HeaderRenderer({
                         textOptions: {
                             textColor: m.Theme.getFontColor(1),
                             backgroundColor: this.grid.style.headerBackgroundColor || m.Theme.getBackgroundColor(2),
                             horizontalAlignment: "left",
                             verticalAlignment: "center"
                         },
                         isLightTheme: this._isLightTheme,
                         grid: this.grid
                     }), this._updateHeaderRenderer()
                 }
-                copyToClipboard() {
-                    const e = this,
-                        t = e.dataModel;
-                    if (!t) return;
-                    const i = e.selectionModel;
-                    if (!i) return;
-                    const n = r.toArray(i.selections());
-                    if (0 === n.length) return;
-                    if (n.length > 1) return void alert("Cannot copy multiple grid selections.");
-                    const o = t.rowCount("body"),
-                        a = t.columnCount("body");
-                    if (0 === o || 0 === a) return;
-                    let {
-                        r1: s,
-                        c1: l,
-                        r2: d,
-                        c2: h
-                    } = n[0];
-                    s = Math.max(0, Math.min(s, o - 1)), l = Math.max(0, Math.min(l, a - 1)), d = Math.max(0, Math.min(d, o - 1)), h = Math.max(0, Math.min(h, a - 1)), d < s && ([s, d] = [d, s]), h < l && ([l, h] = [h, l]);
-                    let c = t.columnCount("row-header"),
-                        u = t.rowCount("column-header");
-                    const g = e.copyConfig.separator,
-                        m = e.copyConfig.format,
-                        p = e.copyConfig.headers,
-                        _ = e.copyConfig.warningThreshold;
-                    let f = d - s + 1,
-                        y = h - l + 1;
-                    switch (p) {
-                        case "none":
-                            c = 0, u = 0;
-                            break;
-                        case "row":
-                            u = 0, y += c;
-                            break;
-                        case "column":
-                            c = 0, f += u;
-                            break;
-                        case "all":
-                            f += u, y += c;
-                            break;
-                        default:
-                            throw "unreachable"
-                    }
-                    const b = f * y;
-                    if (b > _) {
-                        const e = `Copying ${b} cells may take a while. Continue?`;
-                        if (!window.confirm(e)) return
-                    }
-                    const w = {
+                downloadAsCsv(e) {
+                    let t, i, r, n, a = 0,
+                        o = 0;
+                    const s = this.grid,
+                        l = s.dataModel;
+                    if (!l) return;
+                    const d = l.rowCount("body"),
+                        h = l.columnCount("body");
+                    if (0 === d || 0 === h) return;
+                    let c = l.columnCount("row-header"),
+                        u = l.rowCount("column-header");
+                    const m = s.copyConfig.format,
+                        g = s.copyConfig.headers;
+                    if (e) {
+                        const e = s.selectionModel;
+                        if (!e) return;
+                        const l = Array.from(e.selections());
+                        if (0 === l.length) return;
+                        if (l.length > 1) return void alert("Cannot save multiple grid selections.");
+                        switch (({
+                                r1: a,
+                                c1: o,
+                                r2: r,
+                                c2: n
+                            } = l[0]), a = Math.max(0, Math.min(a, d - 1)), o = Math.max(0, Math.min(o, h - 1)), r = Math.max(0, Math.min(r, d - 1)), n = Math.max(0, Math.min(n, h - 1)), r < a && ([a, r] = [r, a]), n < o && ([o, n] = [n, o]), t = r - a + 1, i = n - o + 1, g) {
+                            case "none":
+                                c = 0, u = 0;
+                                break;
+                            case "row":
+                                u = 0, i += c;
+                                break;
+                            case "column":
+                                c = 0, t += u;
+                                break;
+                            case "all":
+                                t += u, i += c;
+                                break;
+                            default:
+                                throw "unreachable"
+                        }
+                    } else t = d + u, i = h + c;
+                    const p = {
                             region: "body",
                             row: 0,
                             column: 0,
                             value: null,
                             metadata: {}
                         },
-                        v = new Array(f);
-                    for (let e = 0; e < f; ++e) {
-                        const i = new Array(y);
-                        for (let r = 0; r < y; ++r) {
-                            let n, o, a;
-                            e < u && r < c ? (n = "corner-header", o = e, a = r) : e < u ? (n = "column-header", o = e, a = r - c + l) : r < c ? (n = "row-header", o = e - u + s, a = r) : (n = "body", o = e - u + s, a = r - c + l), w.region = n, w.row = o, w.column = a, w.value = t.data(n, o, a), w.metadata = t.metadata(n, o, a), i[r] = m(w)
-                        }
-                        v[e] = i
-                    }
-                    const x = v.map((e => e.join(g))).join("\n"),
-                        C = document.createElement("textarea");
-                    C.innerHTML = x, C.style.height = "0px", C.style.width = "0px", C.style.overflow = "hidden", C.id = "ipydatagrid-textarea", C.style.position = "absolute", document.body.appendChild(C), C.select(), document.execCommand("copy"), document.body.removeChild(C)
+                        _ = new Array(t);
+                    for (let e = 0; e < t; ++e) {
+                        const t = new Array(i);
+                        for (let r = 0; r < i; ++r) {
+                            let i, n, s;
+                            e < u && r < c ? (i = "corner-header", n = e, s = r) : e < u ? (i = "column-header", n = e, s = r - c + o) : r < c ? (i = "row-header", n = e - u + a, s = r) : (i = "body", n = e - u + a, s = r - c + o), p.region = i, p.row = n, p.column = s, p.value = l.data(i, n, s), p.metadata = l.metadata(i, n, s), t[r] = m(p)
+                        }
+                        _[e] = t
+                    }
+                    const f = _.map((e => e.join(","))).join("\n"),
+                        b = new Blob([f], {
+                            type: "text/csv"
+                        }),
+                        y = document.createElement("a");
+                    y.download = "out.csv", y.href = window.URL.createObjectURL(b), document.body.appendChild(y), y.click(), document.body.removeChild(y)
                 }
                 get cellClicked() {
                     return this._cellClicked
                 }
                 get columnsResized() {
                     return this._columnsResized
                 }
                 set isLightTheme(e) {
                     this._isLightTheme = e;
                     let t = 0;
                     e ? this.removeClass("dark") : (this.addClass("dark"), t = 1);
                     const i = document.documentElement;
-                    p.forEach(((e, r) => {
+                    g.forEach(((e, r) => {
                         i.style.setProperty(r, e[t])
                     })), this.updateGridStyle()
                 }
                 get isLightTheme() {
                     return this._isLightTheme
                 }
                 _rendererResolver(e) {
@@ -2687,57 +2966,57 @@
                     });
                     let e = !1;
                     this.backboneModel && (e = null !== this.backboneModel.get("corner_renderer")), this.grid.cellRenderers.update({
                         "corner-header": e ? this._cornerHeaderRenderer : this._columnHeaderRenderer
                     })
                 }
                 _createCommandRegistry() {
-                    const e = new n.CommandRegistry;
-                    return e.addCommand(h.FeatherGridContextMenu.CommandID.SortAscending, {
+                    const e = new r.CommandRegistry;
+                    return e.addCommand(d.FeatherGridContextMenu.CommandID.SortAscending, {
                         label: "Sort Ascending",
                         mnemonic: 1,
                         iconClass: "ipydatagrid-filterMenuIcon ipydatagrid-filterMenuIcon-sortAsc",
                         execute: e => {
                             const t = e,
                                 i = this._dataModel.getSchemaIndex(t.region, t.columnIndex);
                             this._dataModel.addTransform({
                                 type: "sort",
                                 columnIndex: i,
                                 desc: !1
                             })
                         }
-                    }), e.addCommand(h.FeatherGridContextMenu.CommandID.SortDescending, {
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.SortDescending, {
                         label: "Sort Descending",
                         mnemonic: 1,
                         iconClass: "ipydatagrid-filterMenuIcon ipydatagrid-filterMenuIcon-sortDesc",
                         execute: e => {
                             const t = e,
                                 i = this._dataModel.getSchemaIndex(t.region, t.columnIndex);
                             this._dataModel.addTransform({
                                 type: "sort",
                                 columnIndex: i,
                                 desc: !0
                             })
                         }
-                    }), e.addCommand(h.FeatherGridContextMenu.CommandID.ClearThisFilter, {
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.ClearThisFilter, {
                         label: "Clear This Filter",
                         mnemonic: -1,
                         execute: e => {
                             const t = e,
                                 i = this._dataModel.getSchemaIndex(t.region, t.columnIndex);
                             this._dataModel.removeTransform(i, "filter")
                         }
-                    }), e.addCommand(h.FeatherGridContextMenu.CommandID.ClearFiltersInAllColumns, {
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.ClearFiltersInAllColumns, {
                         label: "Clear Filters in All Columns",
                         mnemonic: -1,
                         execute: e => {
                             const t = this._dataModel.activeTransforms.filter((e => "filter" !== e.type));
                             this._dataModel.replaceTransforms(t)
                         }
-                    }), e.addCommand(h.FeatherGridContextMenu.CommandID.OpenFilterByConditionDialog, {
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.OpenFilterByConditionDialog, {
                         label: "Filter by condition...",
                         mnemonic: 4,
                         iconClass: "ipydatagrid-filterMenuIcon ipydatagrid-filterMenuIcon-filter",
                         execute: e => {
                             const t = e;
                             this._filterDialog.open({
                                 x: t.clientX,
@@ -2745,15 +3024,15 @@
                                 region: t.region,
                                 columnIndex: t.columnIndex,
                                 forceX: !1,
                                 forceY: !1,
                                 mode: "condition"
                             })
                         }
-                    }), e.addCommand(h.FeatherGridContextMenu.CommandID.OpenFilterByValueDialog, {
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.OpenFilterByValueDialog, {
                         label: "Filter by value...",
                         mnemonic: 4,
                         iconClass: "ipydatagrid-filterMenuIcon ipydatagrid-filterMenuIcon-filter",
                         execute: e => {
                             const t = e;
                             this._filterDialog.open({
                                 x: t.clientX,
@@ -2761,57 +3040,92 @@
                                 region: t.region,
                                 columnIndex: t.columnIndex,
                                 forceX: !1,
                                 forceY: !1,
                                 mode: "value"
                             })
                         }
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.CopySelectionToClipboard, {
+                        label: "Copy Selection to Clipboard",
+                        mnemonic: -1,
+                        isEnabled: () => null !== this.grid.selectionModel && !this.grid.selectionModel.isEmpty,
+                        execute: () => {
+                            this.grid.copyToClipboard()
+                        }
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.SaveSelectionAsCsv, {
+                        label: "Download Selection as CSV",
+                        mnemonic: -1,
+                        isEnabled: () => null !== this.grid.selectionModel && !this.grid.selectionModel.isEmpty,
+                        execute: () => {
+                            this.downloadAsCsv(!0)
+                        }
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.SaveAllAsCsv, {
+                        label: "Download All as CSV",
+                        mnemonic: -1,
+                        execute: () => {
+                            this.downloadAsCsv(!1)
+                        }
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.SortClear, {
+                        label: "No Sort",
+                        mnemonic: 1,
+                        execute: e => {
+                            const t = e,
+                                i = this._dataModel.getSchemaIndex(t.region, t.columnIndex);
+                            this._dataModel.removeTransform(i, "sort")
+                        }
+                    }), e.addCommand(d.FeatherGridContextMenu.CommandID.ClearSelection, {
+                        label: "Clear Selection",
+                        mnemonic: -1,
+                        execute: () => {
+                            var e;
+                            null === (e = this.grid.selectionModel) || void 0 === e || e.clear()
+                        }
                     }), e
                 }
             }
-            t.FeatherGrid = _
+            t.FeatherGrid = p
         },
         4377: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.KeyHandler = void 0;
-            const r = i(6092);
+            const r = i(6479);
             class n extends r.BasicKeyHandler {
                 constructor() {
                     super()
                 }
                 onEscape(e, t) {
                     e.selectionModel && (e.selectionModel.selections().next() ? e.selectionModel.clear() : (-1 === document.body.tabIndex && (document.body.tabIndex = 0), document.body.focus()))
                 }
             }
             t.KeyHandler = n
         },
         591: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.MouseHandler = void 0;
-            const r = i(6092),
+            const r = i(6479),
                 n = i(5593),
-                o = i(4901),
-                a = i(2320);
+                a = i(4901),
+                o = i(2320);
             class s extends r.BasicMouseHandler {
                 constructor(e) {
-                    super(), this._mouseIsDown = !1, this._cellClicked = new o.Signal(this), this._grid = e
+                    super(), this._mouseIsDown = !1, this._cellClicked = new a.Signal(this), this._grid = e
                 }
                 onMouseDown(e, t) {
                     const i = e.hitTest(t.clientX, t.clientY),
-                        o = i.region,
-                        l = 1.5 * a.HeaderRenderer.iconWidth,
-                        d = a.HeaderRenderer.buttonPadding,
+                        a = i.region,
+                        l = 1.5 * o.HeaderRenderer.iconWidth,
+                        d = o.HeaderRenderer.buttonPadding,
                         h = n.Platform.accelKey(t);
-                    if (this._mouseIsDown = !0, "void" !== i.region && this._cellClicked.emit(i), "corner-header" === o || "column-header" === o) {
-                        const r = e.columnSize("corner-header" === o ? "row-header" : "body", i.column),
+                    if (this._mouseIsDown = !0, "void" !== i.region && this._cellClicked.emit(i), "corner-header" === a || "column-header" === a) {
+                        const r = e.columnSize("corner-header" === a ? "row-header" : "body", i.column),
                             n = e.rowSize("column-header", i.row),
-                            a = "column-header" === i.region && i.row == this._grid.grid.dataModel.rowCount("column-header") - 1 || "corner-header" === i.region && 0 === i.row;
-                        if (i.x > r - l - d && i.x < r - d && i.y > n - l - d && i.y < n - d && a) return void this._grid.contextMenu.open(e, Object.assign(Object.assign({}, i), {
+                            o = "column-header" === i.region && i.row == this._grid.grid.dataModel.rowCount("column-header") - 1 || "corner-header" === i.region && 0 === i.row;
+                        if (i.x > r - l - d && i.x < r - d && i.y > n - l - d && i.y < n - d && o) return void this._grid.contextMenu.open(e, Object.assign(Object.assign({}, i), {
                             x: t.clientX + window.scrollX,
                             y: t.clientY + window.scrollY
                         }))
                     }
                     if (e) {
                         const t = s.createCellConfigObject(e, i);
                         if (!t) return;
@@ -2845,111 +3159,125 @@
                 static createCellConfigObject(e, t) {
                     const {
                         region: i,
                         row: r,
                         column: n
                     } = t;
                     if ("void" === i) return;
-                    const o = e.dataModel.data(i, r, n),
-                        a = e.dataModel.metadata(i, r, n);
+                    const a = e.dataModel.data(i, r, n),
+                        o = e.dataModel.metadata(i, r, n);
                     return Object.assign(Object.assign({}, t), {
-                        value: o,
-                        metadata: a
+                        value: a,
+                        metadata: o
                     })
                 }
             }
             t.MouseHandler = s
         },
         6988: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.Theme = t.Scalar = t.ArrayUtils = void 0;
             const r = i(6886);
-            var n;
-            (n = t.ArrayUtils || (t.ArrayUtils = {})).generateMultiIndexArrayLocations = function(e) {
+            ! function(e) {
+                function t(e, t, i) {
+                    if (0 === i) return [0, t];
+                    for (let r = 0; r < e[i - 1].length; r++) {
+                        const n = e[i - 1][r],
+                            a = n.length,
+                            o = n[0][0],
+                            s = n[a - 1][0];
+                        if (t >= o && t <= s) return [o, s]
+                    }
+                    return []
+                }
+                e.generateMultiIndexArrayLocations = function(e) {
                     const t = e._dataset.schema.primaryKey.slice(0, e._dataset.schema.primaryKey.length - 1),
                         i = e._dataset.schema.fields,
                         r = [];
                     for (let e = 0; e < i.length - 1; e++) t.includes(i[e].name) || r.push(e);
                     return r
-                }, n.generateColMergedCellLocations = function(e, t) {
+                }, e.generateColMergedCellLocations = function(e, t) {
                     if (0 === t.length) return [];
                     const i = e._dataset.schema.fields,
                         r = e._dataset.schema.primaryKey.length - 1,
                         n = [];
-                    let o = [];
-                    const a = t[0];
+                    let a = [];
+                    const o = t[0];
                     let s;
-                    for (let e = 0; e < i[a].rows.length; e++) {
-                        let a = [];
+                    for (let e = 0; e < i[o].rows.length; e++) {
+                        let o = [];
                         for (const n of t) {
                             const t = i[n].rows[e];
-                            0 == a.length || s == t ? a.push([e, n - r]) : (o.push(a), a = [
+                            0 == o.length || s == t ? o.push([e, n - r]) : (a.push(o), o = [
                                 [e, n - r]
                             ]), s = t
                         }
-                        o.push(a), n.push(o), o = []
+                        a.push(o), n.push(a), a = []
                     }
                     return n
-                }, n.generateRowMergedCellLocations = function(e) {
-                    const t = e._dataset.schema.primaryKey.slice(0, e._dataset.schema.primaryKey.length - 1);
-                    if (!(t.length > 1)) return [];
-                    const i = e._dataset.data,
-                        r = [];
-                    let n, o = [];
-                    for (let e = 0; e < t.length; e++) {
-                        let a = [];
-                        for (let r = 0; r < i.length; r++) {
-                            const s = i[r][t[e]];
-                            0 == a.length || n == s ? a.push([r, e]) : (o.push(a), a = [
-                                [r, e]
-                            ]), n = s
+                }, e.generateRowMergedCellLocations = function(e) {
+                    const i = e._dataset,
+                        r = i.schema.primaryKey.slice(0, i.schema.primaryKey.length - 1);
+                    if (!(r.length > 1)) return [];
+                    const n = i.data,
+                        a = [];
+                    let o = [];
+                    for (let e = 0; e < r.length; e++) {
+                        let s, l = [];
+                        for (let d = 0; d < i.length; d++) {
+                            const i = n[r[e]][d],
+                                [h, c] = t(a, d, e);
+                            0 == l.length || s == i && l[0][0] >= h && d <= c ? l.push([d, e]) : (o.push(l), l = [
+                                [d, e]
+                            ]), s = i
                         }
-                        o.push(a), r.push(o), o = []
+                        o.push(l), a.push(o), o = []
                     }
-                    return r
-                }, n.validateMergingHierarchy = function(e) {
+                    return a
+                }, e.validateMergingHierarchy = function(e) {
                     let t;
                     for (const i of e)
                         if (void 0 !== t) {
                             if (i.length < t) return !1;
                             t = i.length
                         } else t = i.length;
                     return !0
-                }, n.generateColumnCellGroups = function(e) {
+                }, e.generateColumnCellGroups = function(e) {
                     const t = [];
                     for (let i = 0; i < e.length; i++)
                         for (let r = 0; r < e[i].length; r++)
                             if (e[i][r].length > 1) {
                                 const n = e[i][r].length,
-                                    o = e[i][r][0][1],
-                                    a = e[i][r][n - 1][1];
+                                    a = e[i][r][0][1],
+                                    o = e[i][r][n - 1][1];
                                 t.push({
                                     r1: i,
-                                    c1: o,
+                                    c1: a,
                                     r2: i,
-                                    c2: a
+                                    c2: o
                                 })
                             } return t
-                }, n.generateRowCellGroups = function(e) {
+                }, e.generateRowCellGroups = function(e) {
                     const t = [];
                     for (let i = 0; i < e.length; i++)
                         for (let r = 0; r < e[i].length; r++)
                             if (e[i][r].length > 1) {
                                 const n = e[i][r].length,
-                                    o = e[i][r][0][0],
-                                    a = e[i][r][n - 1][0];
+                                    a = e[i][r][0][0],
+                                    o = e[i][r][n - 1][0];
                                 t.push({
-                                    r1: o,
+                                    r1: a,
                                     c1: i,
-                                    r2: a,
+                                    r2: o,
                                     c2: i
                                 })
                             } return t
-                }, (t.Scalar || (t.Scalar = {})).isScalar = function(e) {
+                }
+            }(t.ArrayUtils || (t.ArrayUtils = {})), (t.Scalar || (t.Scalar = {})).isScalar = function(e) {
                     return null === e || "boolean" == typeof e || "number" == typeof e || "string" == typeof e
                 },
                 function(e) {
                     function t(e) {
                         const t = document.querySelector(".ipydatagrid-widget") || document.body;
                         return window.getComputedStyle(t).getPropertyValue(e) || "#ffffff"
                     }
@@ -2973,27 +3301,27 @@
         },
         2584: (e, t, i) => {
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.VegaExprView = t.VegaExprModel = void 0;
             const r = i(9704),
                 n = i(2969),
-                o = i(8624),
-                a = i(6664),
+                a = i(8624),
+                o = i(6664),
                 s = i(8657),
                 l = n.defaultLocale(),
                 d = {
                     context: {
                         dataflow: {
                             locale: () => l
                         }
                     }
                 };
-            for (const e in o.functionContext) o.functionContext[e] = o.functionContext[e].bind(d);
-            class h extends a.WidgetModel {
+            for (const e in a.functionContext) a.functionContext[e] = a.functionContext[e].bind(d);
+            class h extends o.WidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
                         _model_name: h.model_name,
                         _model_module: h.model_module,
                         _model_module_version: h.model_module_version,
                         value: "default_value"
                     })
@@ -3001,22 +3329,22 @@
                 initialize(e, t) {
                     super.initialize(e, t);
                     const i = {
                         whitelist: ["cell", "default_value", "functions"],
                         globalvar: "cell",
                         functions: e => {
                             const t = r.functions(e);
-                            for (const e in o.functionContext) t[e] = "functions." + e;
+                            for (const e in a.functionContext) t[e] = "functions." + e;
                             return t
                         }
                     };
                     this._codegen = r.codegen(i), this.updateFunction(), this.on("change:value", this.updateFunction.bind(this))
                 }
                 process(e, t) {
-                    return this._function(e, t, o.functionContext)
+                    return this._function(e, t, a.functionContext)
                 }
                 _processRegex(e, t) {
                     const i = t.match(/\[(.*?)\]/g),
                         r = i[0].match(/\[(.*?)\]/)[1];
                     return 1 === i.length ? `cell.metadata.data(cell.row, ${r})` : `cell.metadata.data(cell.row, ${r})${i.splice(1).join("")}`
                 }
                 _augmentExpression(e) {
@@ -3025,15 +3353,15 @@
                 }
                 updateFunction() {
                     let e = this._codegen(r.parse(this.get("value")));
                     e = this._augmentExpression(e), this._function = Function("cell", "default_value", "functions", '"use strict";return(' + e.code + ")")
                 }
             }
             t.VegaExprModel = h, h.model_name = "VegaExprModel", h.model_module = s.MODULE_NAME, h.model_module_version = s.MODULE_VERSION, h.view_name = "VegaExprView", h.view_module = s.MODULE_NAME, h.view_module_version = s.MODULE_VERSION;
-            class c extends a.WidgetView {
+            class c extends o.WidgetView {
                 process(e, t) {
                     return this.model.process(e, t)
                 }
             }
             t.VegaExprView = c
         },
         8657: (e, t, i) => {
@@ -3041,89 +3369,89 @@
                 value: !0
             }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
             const r = i(4147);
             t.MODULE_VERSION = r.version, t.MODULE_NAME = r.name
         },
         5352: (e, t, i) => {
             i.d(t, {
-                Z: () => x
+                Z: () => C
             });
             var r = i(8012),
                 n = i.n(r),
-                o = i(905),
-                a = i.n(o),
+                a = i(905),
+                o = i.n(a),
                 s = i(7188),
                 l = i.n(s),
                 d = new URL(i(7509), i.b),
                 h = new URL(i(3719), i.b),
                 c = new URL(i(1887), i.b),
                 u = new URL(i(7888), i.b),
-                g = new URL(i(2124), i.b),
-                m = new URL(i(6e3), i.b),
-                p = a()(n()),
+                m = new URL(i(2124), i.b),
+                g = new URL(i(6e3), i.b),
+                p = o()(n()),
                 _ = l()(d),
                 f = l()(h),
-                y = l()(c),
-                b = l()(u),
-                w = l()(g),
-                v = l()(m);
-            p.push([e.id, `:root {\n  --ipydatagrid-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,\n    Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';\n  --ipydatagrid-ui-font-size0: 0.83333em;\n  --ipydatagrid-ui-font-size1: 13px; /* Base font size */\n  --ipydatagrid-ui-font-size2: 1.2em;\n  --ipydatagrid-ui-font-size3: 1.44em;\n  --ipydatagrid-padding: 3px;\n  --ipydatagrid-filter-dialog-width: 220px;\n  --ipydatagrid-filter-icon-light: url(${_});\n  --ipydatagrid-sort-asc-icon-light: url(${f});\n  --ipydatagrid-sort-desc-icon-light: url(${y});\n  --ipydatagrid-filter-icon-dark: url(${b});\n  --ipydatagrid-sort-asc-icon-dark: url(${w});\n  --ipydatagrid-sort-desc-icon-dark: url(${v});\n  --ipydatagrid-filter-icon: var(--ipydatagrid-filter-icon-light);\n  --ipydatagrid-sort-asc-icon: var(--ipydatagrid-sort-asc-icon-light);\n  --ipydatagrid-sort-desc-icon: var(--ipydatagrid-sort-desc-icon-light);\n\n  --ipydatagrid-layout-color0: white;\n  --ipydatagrid-layout-color1: white;\n  --ipydatagrid-layout-color2: #eeeeee;\n  --ipydatagrid-layout-color3: #bdbdbd;\n  --ipydatagrid-layout-color4: #757575;\n\n  --ipydatagrid-ui-font-color0: rgba(0, 0, 0, 1);\n  --ipydatagrid-ui-font-color1: rgba(0, 0, 0, 0.87);\n  --ipydatagrid-ui-font-color2: rgba(0, 0, 0, 0.54);\n  --ipydatagrid-ui-font-color3: rgba(0, 0, 0, 0.38);\n\n  --ipydatagrid-border-color0: #bdbdbd;\n  --ipydatagrid-border-color1: #bdbdbd;\n  --ipydatagrid-border-color2: #e0e0e0;\n  --ipydatagrid-border-color3: #eeeeee;\n\n  --ipydatagrid-brand-color0: #1976d2;\n  --ipydatagrid-brand-color1: #2196f3;\n  --ipydatagrid-brand-color2: #64b5f6;\n  --ipydatagrid-brand-color3: #bbdefb;\n  --ipydatagrid-brand-color4: #e3f2fd;\n  --ipydatagrid-brand-color5: #00e6ff;\n  --ipydatagrid-brand-color6: #ffe100;\n  --ipydatagrid-brand-color7: #009eb0;\n  --ipydatagrid-brand-color8: #b09b00;\n\n  --ipydatagrid-menu-bgcolor: white;\n  --ipydatagrid-menu-border-color: #bdbdbd;\n  --ipydatagrid-filter-dlg-textcolor: black;\n  --ipydatagrid-filter-dlg-bgcolor: white;\n}\n\n.ipydatagrid-widget {\n  width: 100%;\n  height: 100%;\n  font-family: var(--ipydatagrid-ui-font-family);\n  font-size: var(--ipydatagrid-ui-font-size1);\n}\n\n.ipydatagrid-widget > div {\n  width: 100%;\n  height: 100%;\n  padding: var(--ipydatagrid-padding);\n  border: none;\n  font-family: "Lato", Helvetica, sans-serif;\n}\n\n.lm-DataGrid-cellEditorOccluder {\n  margin: var(--ipydatagrid-padding);\n}\n\n.ipydatagrid-filterMenu {\n  font-family: var(--ipydatagrid-ui-font-family);\n  font-size: var(--ipydatagrid-ui-font-size1);\n  border: 1px solid var(--ipydatagrid-menu-border-color, #bdbdbd);\n  box-shadow: 5px 5px 5px rgba(0, 0, 0, .2);\n  background: var(--ipydatagrid-menu-bgcolor, white);\n  z-index: 10;\n  padding: 5px;\n  min-height: 143px;\n}\n\n.ipydatagrid-filterMenu select, .ipydatagrid-filterMenu input, .ipydatagrid-filterMenu button {\n  color: var(--ipydatagrid-ui-font-color0, black) !important;\n  background: var(--ipydatagrid-menu-bgcolor, white);\n  font-size: var(--ipydatagrid-ui-font-size1);\n}\n\n.ipydatagrid-filterMenuIcon {\n  background-size: 21px;\n  background-repeat: no-repeat;\n}\n\n.ipydatagrid-filterMenuIcon-filter {\n  background-image: var(--ipydatagrid-filter-icon);\n}\n\n.ipydatagrid-filterMenuIcon-sortAsc {\n  background-image: var(--ipydatagrid-sort-asc-icon);\n}\n\n.ipydatagrid-filterMenuIcon-sortDesc {\n  background-image: var(--ipydatagrid-sort-desc-icon);\n}\n\n.ipydatagrid-unique-value-grid {\n  min-height: 165px;\n  min-width: var(--ipydatagrid-filter-dialog-width);\n  z-index: 1;\n}\n\n.ipydatagrid-filter-title {\n  min-height: 25px;\n  min-width: var(--ipydatagrid-filter-dialog-width);\n}\n\n.ipydatagrid-filter-apply {\n  min-height: 20px;\n}\n\n.ipydatagrid-filter-condition-select {\n  min-height: 35px;\n  min-width: var(--ipydatagrid-filter-dialog-width);\n}\n\n.ipydatagrid-context-menu {\n  border: 1px solid var(--ipydatagrid-menu-border-color, #bdbdbd);\n  background-color: var(--ipydatagrid-menu-bgcolor, white) !important;\n  color: var(--ipydatagrid-ui-font-color0, black) !important;\n  font-family: var(--ipydatagrid-ui-font-family);\n  font-size: var(--ipydatagrid-ui-font-size1);\n  padding-top: 7px;\n  padding-bottom: 4px;\n  padding-left: 3px;\n}\n\n.ipydatagrid-context-menu .lm-Menu-item.lm-mod-active, .ipydatagrid-context-menu .p-Menu-item.p-mod-active {\n  background-color: var(--ipydatagrid-layout-color2);\n}\n\n.ipydatagrid-text-input-filter {\n  transform: translate(5px, 0px);\n}\n`, ""]);
-            const x = p
+                b = l()(c),
+                y = l()(u),
+                w = l()(m),
+                v = l()(g);
+            p.push([e.id, `:root {\n  --ipydatagrid-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,\n    Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';\n  --ipydatagrid-ui-font-size0: 0.83333em;\n  --ipydatagrid-ui-font-size1: 13px; /* Base font size */\n  --ipydatagrid-ui-font-size2: 1.2em;\n  --ipydatagrid-ui-font-size3: 1.44em;\n  --ipydatagrid-padding: 3px;\n  --ipydatagrid-filter-dialog-width: 220px;\n  --ipydatagrid-filter-icon-light: url(${_});\n  --ipydatagrid-sort-asc-icon-light: url(${f});\n  --ipydatagrid-sort-desc-icon-light: url(${b});\n  --ipydatagrid-filter-icon-dark: url(${y});\n  --ipydatagrid-sort-asc-icon-dark: url(${w});\n  --ipydatagrid-sort-desc-icon-dark: url(${v});\n  --ipydatagrid-filter-icon: var(--ipydatagrid-filter-icon-light);\n  --ipydatagrid-sort-asc-icon: var(--ipydatagrid-sort-asc-icon-light);\n  --ipydatagrid-sort-desc-icon: var(--ipydatagrid-sort-desc-icon-light);\n\n  --ipydatagrid-layout-color0: white;\n  --ipydatagrid-layout-color1: white;\n  --ipydatagrid-layout-color2: #eeeeee;\n  --ipydatagrid-layout-color3: #bdbdbd;\n  --ipydatagrid-layout-color4: #757575;\n\n  --ipydatagrid-ui-font-color0: rgba(0, 0, 0, 1);\n  --ipydatagrid-ui-font-color1: rgba(0, 0, 0, 0.87);\n  --ipydatagrid-ui-font-color2: rgba(0, 0, 0, 0.54);\n  --ipydatagrid-ui-font-color3: rgba(0, 0, 0, 0.38);\n\n  --ipydatagrid-border-color0: #bdbdbd;\n  --ipydatagrid-border-color1: #bdbdbd;\n  --ipydatagrid-border-color2: #e0e0e0;\n  --ipydatagrid-border-color3: #eeeeee;\n\n  --ipydatagrid-brand-color0: #1976d2;\n  --ipydatagrid-brand-color1: #2196f3;\n  --ipydatagrid-brand-color2: #64b5f6;\n  --ipydatagrid-brand-color3: #bbdefb;\n  --ipydatagrid-brand-color4: #e3f2fd;\n  --ipydatagrid-brand-color5: #00e6ff;\n  --ipydatagrid-brand-color6: #ffe100;\n  --ipydatagrid-brand-color7: #009eb0;\n  --ipydatagrid-brand-color8: #b09b00;\n\n  --ipydatagrid-menu-bgcolor: white;\n  --ipydatagrid-menu-border-color: #bdbdbd;\n  --ipydatagrid-filter-dlg-textcolor: black;\n  --ipydatagrid-filter-dlg-bgcolor: white;\n}\n\n.ipydatagrid-widget {\n  width: 100%;\n  height: 100%;\n  font-family: var(--ipydatagrid-ui-font-family);\n  font-size: var(--ipydatagrid-ui-font-size1);\n}\n\n.ipydatagrid-widget > div {\n  width: 100%;\n  height: 100%;\n  padding: var(--ipydatagrid-padding);\n  border: none;\n  font-family: "Lato", Helvetica, sans-serif;\n}\n\n.lm-DataGrid-cellEditorOccluder {\n  margin: var(--ipydatagrid-padding);\n}\n\n.ipydatagrid-filterMenu {\n  font-family: var(--ipydatagrid-ui-font-family);\n  font-size: var(--ipydatagrid-ui-font-size1);\n  border: 1px solid var(--ipydatagrid-menu-border-color, #bdbdbd);\n  box-shadow: 5px 5px 5px rgba(0, 0, 0, .2);\n  background: var(--ipydatagrid-menu-bgcolor, white);\n  z-index: 10;\n  padding: 5px;\n  min-height: 143px;\n}\n\n.ipydatagrid-filterMenu select, .ipydatagrid-filterMenu input, .ipydatagrid-filterMenu button {\n  color: var(--ipydatagrid-ui-font-color0, black) !important;\n  background: var(--ipydatagrid-menu-bgcolor, white);\n  font-size: var(--ipydatagrid-ui-font-size1);\n}\n\n.ipydatagrid-filterMenuIcon {\n  background-size: 21px;\n  background-repeat: no-repeat;\n}\n\n.ipydatagrid-filterMenuIcon-filter {\n  background-image: var(--ipydatagrid-filter-icon);\n}\n\n.ipydatagrid-filterMenuIcon-sortAsc {\n  background-image: var(--ipydatagrid-sort-asc-icon);\n}\n\n.ipydatagrid-filterMenuIcon-sortDesc {\n  background-image: var(--ipydatagrid-sort-desc-icon);\n}\n\n.ipydatagrid-unique-value-grid {\n  min-height: 165px;\n  min-width: var(--ipydatagrid-filter-dialog-width);\n  z-index: 1;\n}\n\n.ipydatagrid-filter-title {\n  min-height: 25px;\n  min-width: var(--ipydatagrid-filter-dialog-width);\n}\n\n.ipydatagrid-filter-apply {\n  min-height: 20px;\n}\n\n.ipydatagrid-filter-condition-select {\n  min-height: 35px;\n  min-width: var(--ipydatagrid-filter-dialog-width);\n}\n\n.ipydatagrid-context-menu {\n  border: 1px solid var(--ipydatagrid-menu-border-color, #bdbdbd);\n  background-color: var(--ipydatagrid-menu-bgcolor, white) !important;\n  color: var(--ipydatagrid-ui-font-color0, black) !important;\n  font-family: var(--ipydatagrid-ui-font-family);\n  font-size: var(--ipydatagrid-ui-font-size1);\n  padding-top: 7px;\n  padding-bottom: 4px;\n  padding-left: 3px;\n}\n\n.ipydatagrid-context-menu .lm-Menu-item.lm-mod-active, .ipydatagrid-context-menu .p-Menu-item.p-mod-active {\n  background-color: var(--ipydatagrid-layout-color2);\n}\n\n.ipydatagrid-text-input-filter {\n  transform: translate(5px, 0px);\n}\n`, ""]);
+            const C = p
         },
         8556: (e, t, i) => {
             i.d(t, {
                 Z: () => s
             });
             var r = i(8012),
                 n = i.n(r),
-                o = i(905),
-                a = i.n(o)()(n());
-            a.push([e.id, ".datagrid-container {\n  width: 100%;\n  height: 500px;\n}\n", ""]);
-            const s = a
+                a = i(905),
+                o = i.n(a)()(n());
+            o.push([e.id, ".datagrid-container {\n  width: 100%;\n  height: 500px;\n}\n", ""]);
+            const s = o
         },
         1318: (e, t, i) => {
             i.r(t), i.d(t, {
                 default: () => f
             });
             var r = i(3534),
                 n = i.n(r),
-                o = i(619),
-                a = i.n(o),
+                a = i(619),
+                o = i.n(a),
                 s = i(628),
                 l = i.n(s),
                 d = i(4991),
                 h = i.n(d),
                 c = i(1211),
                 u = i.n(c),
-                g = i(1034),
-                m = i.n(g),
+                m = i(1034),
+                g = i.n(m),
                 p = i(5352),
                 _ = {};
-            _.styleTagTransform = m(), _.setAttributes = h(), _.insert = l().bind(null, "head"), _.domAPI = a(), _.insertStyleElement = u(), n()(p.Z, _);
+            _.styleTagTransform = g(), _.setAttributes = h(), _.insert = l().bind(null, "head"), _.domAPI = o(), _.insertStyleElement = u(), n()(p.Z, _);
             const f = p.Z && p.Z.locals ? p.Z.locals : void 0
         },
         3058: (e, t, i) => {
             i.r(t), i.d(t, {
                 default: () => f
             });
             var r = i(3534),
                 n = i.n(r),
-                o = i(619),
-                a = i.n(o),
+                a = i(619),
+                o = i.n(a),
                 s = i(628),
                 l = i.n(s),
                 d = i(4991),
                 h = i.n(d),
                 c = i(1211),
                 u = i.n(c),
-                g = i(1034),
-                m = i.n(g),
+                m = i(1034),
+                g = i.n(m),
                 p = i(8556),
                 _ = {};
-            _.styleTagTransform = m(), _.setAttributes = h(), _.insert = l().bind(null, "head"), _.domAPI = a(), _.insertStyleElement = u(), n()(p.Z, _);
+            _.styleTagTransform = g(), _.setAttributes = h(), _.insert = l().bind(null, "head"), _.domAPI = o(), _.insertStyleElement = u(), n()(p.Z, _);
             const f = p.Z && p.Z.locals ? p.Z.locals : void 0
         },
         6e3: e => {
             e.exports = "data:image/svg+xml,%3csvg class='bi bi-arrow-down-short' width='1em' height='1em' viewBox='0 0 20 20' fill='white' xmlns='http://www.w3.org/2000/svg'%3e %3cpath fill-rule='evenodd' d='M6.646 9.646a.5.5 0 01.708 0L10 12.293l2.646-2.647a.5.5 0 01.708.708l-3 3a.5.5 0 01-.708 0l-3-3a.5.5 0 010-.708z' clip-rule='evenodd'/%3e %3cpath fill-rule='evenodd' d='M10 6.5a.5.5 0 01.5.5v5a.5.5 0 01-1 0V7a.5.5 0 01.5-.5z' clip-rule='evenodd'/%3e %3c/svg%3e"
         },
         1887: e => {
             e.exports = "data:image/svg+xml,%3csvg class='bi bi-arrow-down-short' width='1em' height='1em' viewBox='0 0 20 20' fill='black' xmlns='http://www.w3.org/2000/svg'%3e %3cpath fill-rule='evenodd' d='M6.646 9.646a.5.5 0 01.708 0L10 12.293l2.646-2.647a.5.5 0 01.708.708l-3 3a.5.5 0 01-.708 0l-3-3a.5.5 0 010-.708z' clip-rule='evenodd'/%3e %3cpath fill-rule='evenodd' d='M10 6.5a.5.5 0 01.5.5v5a.5.5 0 01-1 0V7a.5.5 0 01.5-.5z' clip-rule='evenodd'/%3e %3c/svg%3e"
@@ -3137,11 +3465,11 @@
         7888: e => {
             e.exports = "data:image/svg+xml,%3csvg class='bi bi-filter' width='1em' height='1em' viewBox='0 0 20 20' fill='white' xmlns='http://www.w3.org/2000/svg'%3e %3cpath fill-rule='evenodd' d='M7.5 13a.5.5 0 01.5-.5h4a.5.5 0 010 1H8a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h8a.5.5 0 010 1H6a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h12a.5.5 0 010 1H4a.5.5 0 01-.5-.5z' clip-rule='evenodd'/%3e %3c/svg%3e"
         },
         7509: e => {
             e.exports = "data:image/svg+xml,%3csvg class='bi bi-filter' width='1em' height='1em' viewBox='0 0 20 20' fill='black' xmlns='http://www.w3.org/2000/svg'%3e %3cpath fill-rule='evenodd' d='M7.5 13a.5.5 0 01.5-.5h4a.5.5 0 010 1H8a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h8a.5.5 0 010 1H6a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h12a.5.5 0 010 1H4a.5.5 0 01-.5-.5z' clip-rule='evenodd'/%3e %3c/svg%3e"
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.2.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
+            e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.0","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
         }
     }
 ]);
```

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/remoteEntry.55f84c86e55d5446e7ec.js` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/remoteEntry.e416f171876299bb6885.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,66 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, a, r, t, d, n, o, f, i, c, l, u, s, h, b, p, m, v, g, y = {
-            9416: (e, a, r) => {
-                var t = {
-                        "./index": () => Promise.all([r.e(939), r.e(268), r.e(787), r.e(568)]).then((() => () => r(1568))),
-                        "./extension": () => Promise.all([r.e(268), r.e(787), r.e(296)]).then((() => () => r(4480)))
+    var e, a, t, r, d, n, o, f, i, l, c, u, s, h, b, p, m, v, g, y = {
+            9416: (e, a, t) => {
+                var r = {
+                        "./index": () => Promise.all([t.e(939), t.e(268), t.e(787), t.e(568)]).then((() => () => t(1568))),
+                        "./extension": () => Promise.all([t.e(268), t.e(787), t.e(296)]).then((() => () => t(4480)))
                     },
-                    d = (e, a) => (r.R = a, a = r.o(t, e) ? t[e]() : Promise.resolve().then((() => {
+                    d = (e, a) => (t.R = a, a = t.o(r, e) ? r[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
-                    })), r.R = void 0, a),
+                    })), t.R = void 0, a),
                     n = (e, a) => {
-                        if (r.S) {
-                            var t = "default",
-                                d = r.S[t];
+                        if (t.S) {
+                            var r = "default",
+                                d = t.S[r];
                             if (d && d !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return r.S[t] = e, r.I(t, a)
+                            return t.S[r] = e, t.I(r, a)
                         }
                     };
-                r.d(a, {
+                t.d(a, {
                     get: () => d,
                     init: () => n
                 })
             }
         },
         w = {};
 
     function P(e) {
         var a = w[e];
         if (void 0 !== a) return a.exports;
-        var r = w[e] = {
+        var t = w[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
-        return y[e].call(r.exports, r, r.exports, P), r.loaded = !0, r.exports
+        return y[e].call(t.exports, t, t.exports, P), t.loaded = !0, t.exports
     }
     P.m = y, P.c = w, P.n = e => {
         var a = e && e.__esModule ? () => e.default : () => e;
         return P.d(a, {
             a
         }), a
     }, P.d = (e, a) => {
-        for (var r in a) P.o(a, r) && !P.o(e, r) && Object.defineProperty(e, r, {
+        for (var t in a) P.o(a, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
-            get: a[r]
+            get: a[t]
         })
-    }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((a, r) => (P.f[r](e, a), a)), [])), P.u = e => e + "." + {
+    }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((a, t) => (P.f[t](e, a), a)), [])), P.u = e => e + "." + {
         41: "1846c3ba970651a706b6",
         48: "732e43cec274cf5b8cf5",
         109: "bdd9793b392cc2fe87da",
         112: "4ddba6fd51d10d391fa0",
         142: "025e64e0cbb8aa528385",
         143: "171db67c9b56d395ae64",
         159: "40dbdd4ec4a2fec3a0e0",
         268: "88ce57d2bfbde9012162",
         271: "c6d995708c863e1b27ed",
-        296: "60cde3fcac5bac525295",
+        296: "d2eeaa2e543e597ac586",
         351: "372e5eec3c9010a57cf3",
         400: "95b73fc6eb3f120b823f",
         433: "75ed253aaa8060b28c81",
         455: "25b625d30041b5a1671c",
         456: "afd75d5e116998d22e56",
         462: "68e4d74f02bf2411528e",
         481: "911a23288443c8041987",
@@ -71,15 +71,15 @@
         643: "a265dd26cb50ebd06923",
         679: "e174128fe156c1cd0d10",
         683: "efe59705c1680a8f8b3a",
         689: "3cdb49d94599b1683563",
         700: "7f792a9e7380bfde28dc",
         762: "42901b906691b1301214",
         781: "ef3f9c2a235c4a40bdc0",
-        787: "0a00e3d5d9b736236907",
+        787: "f307b1ca46997f4a9051",
         794: "d7c23e15137c8752365e",
         811: "a135ebc21be585e6d76d",
         823: "18e09aad57c7797df987",
         917: "b972bc5b41fae8990bff",
         939: "04c5876588e4898127e3",
         941: "23c8b1f0eb18afd531e9",
         990: "e35c256305f259cdaeb9"
@@ -89,15 +89,15 @@
         109: "bdd9793b392cc2fe87da",
         112: "4ddba6fd51d10d391fa0",
         142: "025e64e0cbb8aa528385",
         143: "171db67c9b56d395ae64",
         159: "40dbdd4ec4a2fec3a0e0",
         268: "88ce57d2bfbde9012162",
         271: "c6d995708c863e1b27ed",
-        296: "60cde3fcac5bac525295",
+        296: "d2eeaa2e543e597ac586",
         351: "372e5eec3c9010a57cf3",
         400: "95b73fc6eb3f120b823f",
         433: "75ed253aaa8060b28c81",
         455: "25b625d30041b5a1671c",
         456: "afd75d5e116998d22e56",
         462: "68e4d74f02bf2411528e",
         481: "911a23288443c8041987",
@@ -108,46 +108,46 @@
         643: "a265dd26cb50ebd06923",
         679: "e174128fe156c1cd0d10",
         683: "efe59705c1680a8f8b3a",
         689: "3cdb49d94599b1683563",
         700: "7f792a9e7380bfde28dc",
         762: "42901b906691b1301214",
         781: "ef3f9c2a235c4a40bdc0",
-        787: "0a00e3d5d9b736236907",
+        787: "f307b1ca46997f4a9051",
         794: "d7c23e15137c8752365e",
         811: "a135ebc21be585e6d76d",
         823: "18e09aad57c7797df987",
         917: "b972bc5b41fae8990bff",
         939: "04c5876588e4898127e3",
         941: "23c8b1f0eb18afd531e9",
         990: "e35c256305f259cdaeb9"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), P.o = (e, a) => Object.prototype.hasOwnProperty.call(e, a), e = {}, a = "ipydatagrid:", P.l = (r, t, d, n) => {
-        if (e[r]) e[r].push(t);
+    }(), P.o = (e, a) => Object.prototype.hasOwnProperty.call(e, a), e = {}, a = "ipydatagrid:", P.l = (t, r, d, n) => {
+        if (e[t]) e[t].push(r);
         else {
             var o, f;
             if (void 0 !== d)
-                for (var i = document.getElementsByTagName("script"), c = 0; c < i.length; c++) {
-                    var l = i[c];
-                    if (l.getAttribute("src") == r || l.getAttribute("data-webpack") == a + d) {
-                        o = l;
+                for (var i = document.getElementsByTagName("script"), l = 0; l < i.length; l++) {
+                    var c = i[l];
+                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == a + d) {
+                        o = c;
                         break
                     }
                 }
-            o || (f = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, P.nc && o.setAttribute("nonce", P.nc), o.setAttribute("data-webpack", a + d), o.src = r), e[r] = [t];
-            var u = (a, t) => {
+            o || (f = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, P.nc && o.setAttribute("nonce", P.nc), o.setAttribute("data-webpack", a + d), o.src = t), e[t] = [r];
+            var u = (a, r) => {
                     o.onerror = o.onload = null, clearTimeout(s);
-                    var d = e[r];
-                    if (delete e[r], o.parentNode && o.parentNode.removeChild(o), d && d.forEach((e => e(t))), a) return a(t)
+                    var d = e[t];
+                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), d && d.forEach((e => e(r))), a) return a(r)
                 },
                 s = setTimeout(u.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
             o.onerror = u.bind(null, o.onerror), o.onload = u.bind(null, o.onload), f && document.head.appendChild(o)
         }
@@ -157,163 +157,164 @@
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, P.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         P.S = {};
         var e = {},
             a = {};
-        P.I = (r, t) => {
-            t || (t = []);
-            var d = a[r];
-            if (d || (d = a[r] = {}), !(t.indexOf(d) >= 0)) {
-                if (t.push(d), e[r]) return e[r];
-                P.o(P.S, r) || (P.S[r] = {});
-                var n = P.S[r],
+        P.I = (t, r) => {
+            r || (r = []);
+            var d = a[t];
+            if (d || (d = a[t] = {}), !(r.indexOf(d) >= 0)) {
+                if (r.push(d), e[t]) return e[t];
+                P.o(P.S, t) || (P.S[t] = {});
+                var n = P.S[t],
                     o = "ipydatagrid",
-                    f = (e, a, r, t) => {
+                    f = (e, a, t, r) => {
                         var d = n[e] = n[e] || {},
                             f = d[a];
-                        (!f || !f.loaded && (!t != !f.eager ? t : o > f.from)) && (d[a] = {
-                            get: r,
+                        (!f || !f.loaded && (!r != !f.eager ? r : o > f.from)) && (d[a] = {
+                            get: t,
                             from: o,
-                            eager: !!t
+                            eager: !!r
                         })
                     },
                     i = [];
-                return "default" === r && (f("d3-array", "3.2.4", (() => P.e(433).then((() => () => P(3433))))), f("d3-array", "3.2.4", (() => P.e(455).then((() => () => P(2455))))), f("d3-array", "3.2.4", (() => P.e(513).then((() => () => P(5513))))), f("d3-array", "3.2.4", (() => P.e(643).then((() => () => P(8643))))), f("d3-array", "3.2.4", (() => P.e(41).then((() => () => P(8041))))), f("d3-array", "3.2.4", (() => P.e(109).then((() => () => P(109))))), f("d3-color", "3.1.0", (() => P.e(811).then((() => () => P(4811))))), f("d3-format", "1.4.5", (() => P.e(481).then((() => () => P(8481))))), f("d3-format", "3.1.0", (() => P.e(142).then((() => () => P(2142))))), f("d3-format", "3.1.0", (() => P.e(462).then((() => () => P(7271))))), f("d3-scale", "4.0.2", (() => Promise.all([P.e(781), P.e(622), P.e(112), P.e(456)]).then((() => () => P(2781))))), f("d3-time-format", "2.3.0", (() => P.e(48).then((() => () => P(4048))))), f("d3-time-format", "4.1.0", (() => P.e(941).then((() => () => P(6941))))), f("d3-time-format", "4.1.0", (() => P.e(683).then((() => () => P(271))))), f("ipydatagrid", "1.2.1", (() => Promise.all([P.e(939), P.e(268), P.e(787), P.e(568)]).then((() => () => P(1568))))), f("moment", "2.29.4", (() => Promise.all([P.e(762), P.e(700)]).then((() => () => P(381))))), f("underscore", "1.13.6", (() => P.e(794).then((() => () => P(7794))))), f("vega-expression", "2.7.0", (() => P.e(351).then((() => () => P(6351))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(143), P.e(823)]).then((() => () => P(8143))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(917), P.e(990)]).then((() => () => P(9917))))), f("vega-format", "1.1.1", (() => Promise.all([P.e(642), P.e(689), P.e(400)]).then((() => () => P(7400))))), f("vega-functions", "5.14.0", (() => Promise.all([P.e(642), P.e(679), P.e(268), P.e(622), P.e(689), P.e(159)]).then((() => () => P(679)))))), e[r] = i.length ? Promise.all(i).then((() => e[r] = 1)) : 1
+                return "default" === t && (f("d3-array", "3.2.4", (() => P.e(433).then((() => () => P(3433))))), f("d3-array", "3.2.4", (() => P.e(455).then((() => () => P(2455))))), f("d3-array", "3.2.4", (() => P.e(513).then((() => () => P(5513))))), f("d3-array", "3.2.4", (() => P.e(643).then((() => () => P(8643))))), f("d3-array", "3.2.4", (() => P.e(41).then((() => () => P(8041))))), f("d3-array", "3.2.4", (() => P.e(109).then((() => () => P(109))))), f("d3-color", "3.1.0", (() => P.e(811).then((() => () => P(4811))))), f("d3-format", "1.4.5", (() => P.e(481).then((() => () => P(8481))))), f("d3-format", "3.1.0", (() => P.e(142).then((() => () => P(2142))))), f("d3-format", "3.1.0", (() => P.e(462).then((() => () => P(7271))))), f("d3-scale", "4.0.2", (() => Promise.all([P.e(781), P.e(622), P.e(112), P.e(456)]).then((() => () => P(2781))))), f("d3-time-format", "2.3.0", (() => P.e(48).then((() => () => P(4048))))), f("d3-time-format", "4.1.0", (() => P.e(941).then((() => () => P(6941))))), f("d3-time-format", "4.1.0", (() => P.e(683).then((() => () => P(271))))), f("ipydatagrid", "1.3.0", (() => Promise.all([P.e(939), P.e(268), P.e(787), P.e(568)]).then((() => () => P(1568))))), f("moment", "2.29.4", (() => Promise.all([P.e(762), P.e(700)]).then((() => () => P(381))))), f("underscore", "1.13.6", (() => P.e(794).then((() => () => P(7794))))), f("vega-expression", "2.7.0", (() => P.e(351).then((() => () => P(6351))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(143), P.e(823)]).then((() => () => P(8143))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(917), P.e(990)]).then((() => () => P(9917))))), f("vega-format", "1.1.1", (() => Promise.all([P.e(642), P.e(689), P.e(400)]).then((() => () => P(7400))))), f("vega-functions", "5.14.0", (() => Promise.all([P.e(642), P.e(679), P.e(268), P.e(622), P.e(689), P.e(159)]).then((() => () => P(679)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var a = P.g.document;
         if (!e && a && (a.currentScript && (e = a.currentScript.src), !e)) {
-            var r = a.getElementsByTagName("script");
-            if (r.length)
-                for (var t = r.length - 1; t > -1 && !e;) e = r[t--].src
+            var t = a.getElementsByTagName("script");
+            if (t.length)
+                for (var r = t.length - 1; r > -1 && !e;) e = t[r--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), P.p = e
-    })(), r = e => {
+    })(), t = e => {
         var a = e => e.split(".").map((e => +e == e ? +e : e)),
-            r = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            t = r[1] ? a(r[1]) : [];
-        return r[2] && (t.length++, t.push.apply(t, a(r[2]))), r[3] && (t.push([]), t.push.apply(t, a(r[3]))), t
-    }, t = (e, a) => {
-        e = r(e), a = r(a);
-        for (var t = 0;;) {
-            if (t >= e.length) return t < a.length && "u" != (typeof a[t])[0];
-            var d = e[t],
+            t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
+            r = t[1] ? a(t[1]) : [];
+        return t[2] && (r.length++, r.push.apply(r, a(t[2]))), t[3] && (r.push([]), r.push.apply(r, a(t[3]))), r
+    }, r = (e, a) => {
+        e = t(e), a = t(a);
+        for (var r = 0;;) {
+            if (r >= e.length) return r < a.length && "u" != (typeof a[r])[0];
+            var d = e[r],
                 n = (typeof d)[0];
-            if (t >= a.length) return "u" == n;
-            var o = a[t],
+            if (r >= a.length) return "u" == n;
+            var o = a[r],
                 f = (typeof o)[0];
             if (n != f) return "o" == n && "n" == f || "s" == f || "u" == n;
             if ("o" != n && "u" != n && d != o) return d < o;
-            t++
+            r++
         }
     }, d = e => {
         var a = e[0],
-            r = "";
+            t = "";
         if (1 === e.length) return "*";
         if (a + .5) {
-            r += 0 == a ? ">=" : -1 == a ? "<" : 1 == a ? "^" : 2 == a ? "~" : a > 0 ? "=" : "!=";
-            for (var t = 1, n = 1; n < e.length; n++) t--, r += "u" == (typeof(f = e[n]))[0] ? "-" : (t > 0 ? "." : "") + (t = 2, f);
-            return r
+            t += 0 == a ? ">=" : -1 == a ? "<" : 1 == a ? "^" : 2 == a ? "~" : a > 0 ? "=" : "!=";
+            for (var r = 1, n = 1; n < e.length; n++) r--, t += "u" == (typeof(f = e[n]))[0] ? "-" : (r > 0 ? "." : "") + (r = 2, f);
+            return t
         }
         var o = [];
         for (n = 1; n < e.length; n++) {
             var f = e[n];
             o.push(0 === f ? "not(" + i() + ")" : 1 === f ? "(" + i() + " || " + i() + ")" : 2 === f ? o.pop() + " " + o.pop() : d(f))
         }
         return i();
 
         function i() {
             return o.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, n = (e, a) => {
         if (0 in e) {
-            a = r(a);
-            var t = e[0],
-                d = t < 0;
-            d && (t = -t - 1);
+            a = t(a);
+            var r = e[0],
+                d = r < 0;
+            d && (r = -r - 1);
             for (var o = 0, f = 1, i = !0;; f++, o++) {
-                var c, l, u = f < e.length ? (typeof e[f])[0] : "";
-                if (o >= a.length || "o" == (l = (typeof(c = a[o]))[0])) return !i || ("u" == u ? f > t && !d : "" == u != d);
-                if ("u" == l) {
+                var l, c, u = f < e.length ? (typeof e[f])[0] : "";
+                if (o >= a.length || "o" == (c = (typeof(l = a[o]))[0])) return !i || ("u" == u ? f > r && !d : "" == u != d);
+                if ("u" == c) {
                     if (!i || "u" != u) return !1
                 } else if (i)
-                    if (u == l)
-                        if (f <= t) {
-                            if (c != e[f]) return !1
+                    if (u == c)
+                        if (f <= r) {
+                            if (l != e[f]) return !1
                         } else {
-                            if (d ? c > e[f] : c < e[f]) return !1;
-                            c != e[f] && (i = !1)
+                            if (d ? l > e[f] : l < e[f]) return !1;
+                            l != e[f] && (i = !1)
                         }
                 else if ("s" != u && "n" != u) {
-                    if (d || f <= t) return !1;
+                    if (d || f <= r) return !1;
                     i = !1, f--
                 } else {
-                    if (f <= t || l < u != d) return !1;
+                    if (f <= r || c < u != d) return !1;
                     i = !1
                 } else "s" != u && "n" != u && (i = !1, f--)
             }
         }
         var s = [],
             h = s.pop.bind(s);
         for (o = 1; o < e.length; o++) {
             var b = e[o];
             s.push(1 == b ? h() | h() : 2 == b ? h() & h() : b ? n(b, a) : !h())
         }
         return !!h()
     }, o = (e, a) => {
-        var r = P.S[e];
-        if (!r || !P.o(r, a)) throw new Error("Shared module " + a + " doesn't exist in shared scope " + e);
-        return r
+        var t = P.S[e];
+        if (!t || !P.o(t, a)) throw new Error("Shared module " + a + " doesn't exist in shared scope " + e);
+        return t
     }, f = (e, a) => {
-        var r = e[a];
-        return Object.keys(r).reduce(((e, a) => !e || !r[e].loaded && t(e, a) ? a : e), 0)
-    }, i = (e, a, r, t) => "Unsatisfied version " + r + " from " + (r && e[a][r].from) + " of shared singleton module " + a + " (required " + d(t) + ")", c = (e, a, r, t) => {
-        var d = f(e, r);
-        return n(t, d) || u(i(e, r, d, t)), s(e[r][d])
-    }, l = (e, a, r) => {
+        var t = e[a];
+        return Object.keys(t).reduce(((e, a) => !e || !t[e].loaded && r(e, a) ? a : e), 0)
+    }, i = (e, a, t, r) => "Unsatisfied version " + t + " from " + (t && e[a][t].from) + " of shared singleton module " + a + " (required " + d(r) + ")", l = (e, a, t, r) => {
+        var d = f(e, t);
+        return n(r, d) || u(i(e, t, d, r)), s(e[t][d])
+    }, c = (e, a, t) => {
         var d = e[a];
-        return (a = Object.keys(d).reduce(((e, a) => !n(r, a) || e && !t(e, a) ? e : a), 0)) && d[a]
+        return (a = Object.keys(d).reduce(((e, a) => !n(t, a) || e && !r(e, a) ? e : a), 0)) && d[a]
     }, u = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), b = (h = e => function(a, r, t, d) {
+    }, s = e => (e.loaded = 1, e.get()), b = (h = e => function(a, t, r, d) {
         var n = P.I(a);
-        return n && n.then ? n.then(e.bind(e, a, P.S[a], r, t, d)) : e(a, P.S[a], r, t, d)
-    })(((e, a, r, t) => (o(e, r), c(a, 0, r, t)))), p = h(((e, a, r, t, d) => {
-        var n = a && P.o(a, r) && l(a, r, t);
+        return n && n.then ? n.then(e.bind(e, a, P.S[a], t, r, d)) : e(a, P.S[a], t, r, d)
+    })(((e, a, t, r) => (o(e, t), l(a, 0, t, r)))), p = h(((e, a, t, r, d) => {
+        var n = a && P.o(a, t) && c(a, t, r);
         return n ? s(n) : d()
     })), m = {}, v = {
         2969: () => p("default", "vega-format", [1, 1, 1, 1], (() => Promise.all([P.e(642), P.e(689), P.e(400)]).then((() => () => P(7400))))),
         6886: () => p("default", "d3-color", [1, 3, 1, 0], (() => P.e(811).then((() => () => P(4811))))),
         2297: () => p("default", "underscore", [1, 1, 13, 6], (() => P.e(794).then((() => () => P(7794))))),
+        2544: () => b("default", "bqplot", [2, 0, 5]),
         4031: () => p("default", "moment", [1, 2, 24, 0], (() => Promise.all([P.e(762), P.e(700)]).then((() => () => P(381))))),
         4059: () => b("default", "@lumino/virtualdom", [1, 2, 0, 0]),
+        4882: () => b("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => b("default", "@lumino/signaling", [1, 2, 0, 0]),
         5058: () => p("default", "d3-format", [1, 1, 3, 2], (() => P.e(481).then((() => () => P(8481))))),
         5593: () => b("default", "@lumino/domutils", [1, 2, 0, 0]),
         5633: () => b("default", "@lumino/messaging", [1, 2, 0, 0]),
-        6092: () => b("default", "@lumino/datagrid", [1, 2, 0, 1]),
+        6479: () => b("default", "@lumino/datagrid", [1, 2, 3, 0, , "alpha", 0]),
         6664: () => b("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1
         ]),
         6697: () => b("default", "@lumino/algorithm", [1, 2, 0, 0]),
         7120: () => b("default", "@lumino/commands", [1, 2, 0, 1]),
         7831: () => p("default", "d3-time-format", [1, 2, 1, 3], (() => P.e(48).then((() => () => P(4048))))),
         7930: () => b("default", "@lumino/coreutils", [1, 2, 0, 0]),
         8624: () => p("default", "vega-functions", [1, 5, 3, 0], (() => Promise.all([P.e(642), P.e(679), P.e(622), P.e(689), P.e(159)]).then((() => () => P(679))))),
-        8778: () => b("default", "@lumino/widgets", [1, 2, 0, 1]),
         9704: () => p("default", "vega-expression", [1, 2, 6, 0], (() => P.e(351).then((() => () => P(6351))))),
-        5123: () => b("default", "@jupyterlab/apputils", [1, 4, 1, 11]),
+        1464: () => b("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
         3622: () => p("default", "d3-color", [, [1, 3],
             [-1, 3], 1, [0, 1], 2
         ], (() => P.e(811).then((() => () => P(4811))))),
         1573: () => p("default", "d3-array", [, [1, 3],
             [-1, 3], 1, [0, 2, 10, 0], 2
         ], (() => P.e(513).then((() => () => P(5513))))),
         3919: () => p("default", "d3-array", [, [1, 3],
@@ -339,71 +340,71 @@
         6476: () => p("default", "vega-expression", [1, 5, 1, 0], (() => P.e(143).then((() => () => P(8143))))),
         8581: () => p("default", "d3-array", [1, 3, 2, 2], (() => P.e(41).then((() => () => P(8041))))),
         8933: () => p("default", "d3-array", [4, 3, 2, 4], (() => P.e(643).then((() => () => P(8643)))))
     }, g = {
         112: [1573, 3919, 4603, 5551],
         159: [127, 519, 2112, 4620, 4826, 6476, 8581, 8933],
         268: [2969, 6886],
-        296: [5123],
+        296: [1464],
         400: [2257, 7751, 7868],
         622: [3622],
         689: [689],
-        787: [2297, 4031, 4059, 4901, 5058, 5593, 5633, 6092, 6664, 6697, 7120, 7831, 7930, 8624, 8778, 9704]
+        787: [2297, 2544, 4031, 4059, 4882, 4901, 5058, 5593, 5633, 6479, 6664, 6697, 7120, 7831, 7930, 8624, 9704]
     }, P.f.consumes = (e, a) => {
         P.o(g, e) && g[e].forEach((e => {
             if (P.o(m, e)) return a.push(m[e]);
-            var r = a => {
-                    m[e] = 0, P.m[e] = r => {
-                        delete P.c[e], r.exports = a()
+            var t = a => {
+                    m[e] = 0, P.m[e] = t => {
+                        delete P.c[e], t.exports = a()
                     }
                 },
-                t = a => {
-                    delete m[e], P.m[e] = r => {
+                r = a => {
+                    delete m[e], P.m[e] = t => {
                         throw delete P.c[e], a
                     }
                 };
             try {
                 var d = v[e]();
-                d.then ? a.push(m[e] = d.then(r).catch(t)) : r(d)
+                d.then ? a.push(m[e] = d.then(t).catch(r)) : t(d)
             } catch (e) {
-                t(e)
+                r(e)
             }
         }))
     }, (() => {
         P.b = document.baseURI || self.location.href;
         var e = {
             146: 0
         };
-        P.f.j = (a, r) => {
-            var t = P.o(e, a) ? e[a] : void 0;
-            if (0 !== t)
-                if (t) r.push(t[2]);
+        P.f.j = (a, t) => {
+            var r = P.o(e, a) ? e[a] : void 0;
+            if (0 !== r)
+                if (r) t.push(r[2]);
                 else if (/^(112|159|268|622|689)$/.test(a)) e[a] = 0;
             else {
-                var d = new Promise(((r, d) => t = e[a] = [r, d]));
-                r.push(t[2] = d);
+                var d = new Promise(((t, d) => r = e[a] = [t, d]));
+                t.push(r[2] = d);
                 var n = P.p + P.u(a),
                     o = new Error;
-                P.l(n, (r => {
-                    if (P.o(e, a) && (0 !== (t = e[a]) && (e[a] = void 0), t)) {
-                        var d = r && ("load" === r.type ? "missing" : r.type),
-                            n = r && r.target && r.target.src;
-                        o.message = "Loading chunk " + a + " failed.\n(" + d + ": " + n + ")", o.name = "ChunkLoadError", o.type = d, o.request = n, t[1](o)
+                P.l(n, (t => {
+                    if (P.o(e, a) && (0 !== (r = e[a]) && (e[a] = void 0), r)) {
+                        var d = t && ("load" === t.type ? "missing" : t.type),
+                            n = t && t.target && t.target.src;
+                        o.message = "Loading chunk " + a + " failed.\n(" + d + ": " + n + ")", o.name = "ChunkLoadError", o.type = d, o.request = n, r[1](o)
                     }
                 }), "chunk-" + a, a)
             }
         };
-        var a = (a, r) => {
-                var t, d, [n, o, f] = r,
+        var a = (a, t) => {
+                var r, d, [n, o, f] = t,
                     i = 0;
                 if (n.some((a => 0 !== e[a]))) {
-                    for (t in o) P.o(o, t) && (P.m[t] = o[t]);
+                    for (r in o) P.o(o, r) && (P.m[r] = o[r]);
                     f && f(P)
                 }
-                for (a && a(r); i < n.length; i++) d = n[i], P.o(e, d) && e[d] && e[d][0](), e[d] = 0
+                for (a && a(t); i < n.length; i++) d = n[i], P.o(e, d) && e[d] && e[d][0](), e[d] = 0
             },
-            r = self.webpackChunkipydatagrid = self.webpackChunkipydatagrid || [];
-        r.forEach(a.bind(null, 0)), r.push = a.bind(null, r.push.bind(r))
+            t = self.webpackChunkipydatagrid = self.webpackChunkipydatagrid || [];
+        t.forEach(a.bind(null, 0)), t.push = a.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
     var S = P(9416);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipydatagrid = S
 })();
```

### Comparing `ipydatagrid-1.2.1/ipydatagrid/labextension/static/third-party-licenses.json` & `ipydatagrid-1.3.0/ipydatagrid/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/js/cellrenderer.ts` & `ipydatagrid-1.3.0/js/cellrenderer.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 // Copyright (c) Bloomberg
 // Distributed under the terms of the Modified BSD License.
 
-import * as _ from 'underscore';
-
 const d3Format: any = require('d3-format');
 const d3TimeFormat: any = require('d3-time-format');
 
 import {
+  AsyncCellRenderer,
   CellRenderer,
-  TextRenderer,
   HyperlinkRenderer,
+  ImageRenderer,
+  TextRenderer,
 } from '@lumino/datagrid';
 
 import {
   Dict,
+  ISerializers,
   WidgetModel,
   WidgetView,
-  ISerializers,
   resolvePromisesDict,
   unpack_models,
 } from '@jupyter-widgets/base';
 
 import { MODULE_NAME, MODULE_VERSION } from './version';
 
 import { BarRenderer } from './core/barrenderer';
 
 import { VegaExprView } from './vegaexpr';
 
+import { HtmlRenderer, exportedClass } from './core/htmlRenderer';
 import { Scalar, Theme } from './utils';
 
 // Temporary, will be removed when the scales are exported from bqplot
 type Scale = any;
 
 type Processor = Scalar | VegaExprView | Scale;
 
@@ -65,37 +66,36 @@
   static model_module_version = MODULE_VERSION;
   static view_name = 'CellRendererView';
   static view_module = MODULE_NAME;
   static view_module_version = MODULE_VERSION;
 }
 
 export abstract class CellRendererView extends WidgetView {
-  render() {
-    return this.initializeRenderer().then(() => {
-      this.updateRenderer();
+  async render() {
+    await this.initializeRenderer();
 
-      this.on('renderer-needs-update', this.updateRenderer.bind(this));
-    });
+    this.updateRenderer();
+
+    this.on('renderer-needs-update', this.updateRenderer.bind(this));
   }
 
   /**
    * Method that should be called when the theme has changed.
    */
-  onThemeChanged() {
-    return this.initializeRenderer().then(() => {
-      this.updateRenderer();
-    });
+  async onThemeChanged() {
+    await this.initializeRenderer();
+    return this.updateRenderer();
   }
 
   /**
    * Initialize the CellRenderer widget.
    *
    * @return The promise to initialize the renderer
    */
-  protected initializeRenderer(): Promise<any> {
+  protected async initializeRenderer(): Promise<any> {
     const promises: Dict<PromiseLike<Processor>> = {};
     const attr_names = this.model
       .get_attrs()
       .map((attr: ICellRendererAttribute) => {
         return attr.name;
       });
 
@@ -105,17 +105,15 @@
       this,
     );
 
     for (const name of attr_names) {
       promises[name] = this.updateProcessor(name);
     }
 
-    return resolvePromisesDict(promises).then((processors: Dict<Processor>) => {
-      this.processors = processors;
-    });
+    this.processors = await resolvePromisesDict(promises);
   }
 
   private _on_some_processors_change(event: any) {
     const promises: Dict<PromiseLike<Processor>> = {};
 
     for (const name in event.changed) {
       promises[name] = this.updateProcessor(name);
@@ -457,7 +455,160 @@
     });
   }
 
   renderer: HyperlinkRenderer;
 
   model: HyperlinkRendererModel;
 }
+
+export class ImageRendererModel extends CellRendererModel {
+  defaults() {
+    return {
+      ...super.defaults(),
+      _model_name: ImageRendererModel.model_name,
+      _view_name: ImageRendererModel.view_name,
+      background_color: {},
+      placeholder: {},
+      text_color: {},
+      width: {},
+      height: {},
+    };
+  }
+
+  get_attrs(): ICellRendererAttribute[] {
+    return [
+      {
+        name: 'background_color',
+        phosphorName: 'backgroundColor',
+        defaultValue: '',
+      },
+      { name: 'placeholder', phosphorName: 'placeholder', defaultValue: '...' },
+      {
+        name: 'text_color',
+        phosphorName: 'textColor',
+        defaultValue: '#000000',
+      },
+      { name: 'width', phosphorName: 'width', defaultValue: '' },
+      { name: 'height', phosphorName: 'height', defaultValue: '100%' },
+    ];
+  }
+
+  static serializers: ISerializers = {
+    ...TextRendererModel.serializers,
+    background_color: { deserialize: unpack_models as any },
+    placeholder: { deserialize: unpack_models as any },
+    text_color: { deserialize: unpack_models as any },
+    width: { deserialize: unpack_models as any },
+    height: { deserialize: unpack_models as any },
+  };
+
+  static model_name = 'ImageRendererModel';
+  static view_name = 'ImageRendererView';
+}
+
+export class ImageRendererView extends CellRendererView {
+  createRenderer(options: ImageRenderer.IOptions) {
+    if (!ImageRenderer) {
+      return new TextRenderer({
+        format: (config) => {
+          return 'ImageRenderer not available. Check that you are using JupyterLab>=4.1.';
+        },
+        wrapText: true,
+      });
+    }
+    return new ImageRenderer({
+      ...options,
+    });
+  }
+
+  renderer: ImageRenderer;
+
+  model: ImageRendererModel;
+}
+
+export class HtmlRendererModel extends CellRendererModel {
+  defaults() {
+    return {
+      ...super.defaults(),
+      _model_name: HtmlRendererModel.model_name,
+      _view_name: HtmlRendererModel.view_name,
+      font: '12px sans-serif',
+      placeholder: '...',
+      text_color: null,
+      background_color: null,
+      vertical_alignment: 'center',
+      horizontal_alignment: 'left',
+    };
+  }
+
+  get_attrs(): ICellRendererAttribute[] {
+    return [
+      { name: 'font', phosphorName: 'font', defaultValue: '12px sans-serif' },
+      { name: 'placeholder', phosphorName: 'placeholder', defaultValue: '...' },
+      {
+        name: 'text_color',
+        phosphorName: 'textColor',
+        defaultValue: Theme.getFontColor(),
+      },
+      {
+        name: 'background_color',
+        phosphorName: 'backgroundColor',
+        defaultValue: Theme.getBackgroundColor(),
+      },
+      {
+        name: 'vertical_alignment',
+        phosphorName: 'verticalAlignment',
+        defaultValue: 'center',
+      },
+      {
+        name: 'horizontal_alignment',
+        phosphorName: 'horizontalAlignment',
+        defaultValue: 'left',
+      },
+    ];
+  }
+
+  static serializers: ISerializers = {
+    ...CellRendererModel.serializers,
+    font: { deserialize: unpack_models as any },
+    placeholder: { deserialize: unpack_models as any },
+    text_color: { deserialize: unpack_models as any },
+    background_color: { deserialize: unpack_models as any },
+    vertical_alignment: { deserialize: unpack_models as any },
+    horizontal_alignment: { deserialize: unpack_models as any },
+  };
+
+  static model_name = 'HtmlRendererModel';
+  static view_name = 'HtmlRendererView';
+}
+
+export class HtmlRendererView extends CellRendererView {
+  createRenderer(options: HtmlRenderer.IOptions) {
+    // Workaround for Jupyter Lab 3 / ipywidget 7 compatibility
+    let htmRenderer: any;
+
+    if (!AsyncCellRenderer) {
+      htmRenderer = new TextRenderer({
+        format: (config) => {
+          return 'AsyncCellRenderer not available. Check that you are using JupyterLab>=4.1.';
+        },
+        wrapText: true,
+      });
+    } else {
+      htmRenderer = new exportedClass({
+        ...options,
+      });
+      htmRenderer.imageLoaded.connect(() => {
+        setTimeout(() => {
+          this.trigger('renderer-needs-update');
+        }, 0);
+      });
+    }
+
+    return htmRenderer;
+  }
+
+  // Workaround for Jupyter Lab 3 / ipywidget 7 compatibility
+  renderer: any;
+
+  model: HtmlRendererModel;
+}
```

### Comparing `ipydatagrid-1.2.1/js/datagrid.ts` & `ipydatagrid-1.3.0/js/datagrid.ts`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,95 @@
 import { JSONExt } from '@lumino/coreutils';
 
 import { Message, MessageLoop } from '@lumino/messaging';
 
 import { Widget } from '@lumino/widgets';
 
 import {
+  Dict,
   DOMWidgetModel,
   DOMWidgetView,
   ICallbacks,
   ISerializers,
   // @ts-ignore needed for ipywidgetx 8.x compatibility
   JupyterLuminoPanelWidget,
   // @ts-ignore needed for ipywidgetx 7.x compatibility
   JupyterPhosphorPanelWidget,
   resolvePromisesDict,
   unpack_models,
-  WidgetModel
+  WidgetModel,
 } from '@jupyter-widgets/base';
 
+import { array_or_json_serializer } from 'bqplot';
+
 import { ViewBasedJSONModel } from './core/viewbasedjsonmodel';
 
 import { MODULE_NAME, MODULE_VERSION } from './version';
 
 import { CellRendererModel, CellRendererView } from './cellrenderer';
 import { FeatherGrid } from './feathergrid';
 import { Theme } from './utils';
+import { DataSource } from './datasource';
 
 // Import CSS
 import '../style/jupyter-widget.css';
 
-// Shorthand for a string->T mapping
-type Dict<T> = { [keys: string]: T };
+function unpack_raw_data(
+  value: any | Dict<unknown> | string | (Dict<unknown> | string)[],
+): any {
+  if (Array.isArray(value)) {
+    const unpacked: any[] = [];
+    value.forEach((sub_value, key) => {
+      unpacked.push(unpack_raw_data(sub_value));
+    });
+    return unpacked;
+  } else if (value instanceof Object && typeof value !== 'string') {
+    const unpacked: { [key: string]: any } = {};
+    Object.keys(value).forEach((key) => {
+      unpacked[key] = unpack_raw_data(value[key]);
+    });
+    return unpacked;
+  } else if (value === '$NaN$') {
+    return Number.NaN;
+  } else if (value === '$Infinity$') {
+    return Number.POSITIVE_INFINITY;
+  } else if (value === '$NegInfinity$') {
+    return Number.NEGATIVE_INFINITY;
+  } else if (value === '$NaT$') {
+    return new Date('INVALID');
+  } else {
+    return value;
+  }
+}
+
+function serialize_data(data: DataSource, manager: any): any {
+  const serialized_data: any = {};
+  for (const column of Object.keys(data.data)) {
+    serialized_data[column] = array_or_json_serializer.serialize(
+      data.data[column],
+      manager,
+    );
+  }
+  return { data: serialized_data, fields: data.fields, schema: data.schema };
+}
+
+function deserialize_data(data: any, manager: any): DataSource {
+  const deserialized_data: any = {};
+  for (const column of Object.keys(data.data)) {
+    if (data.data[column].type == 'raw') {
+      deserialized_data[column] = unpack_raw_data(data.data[column].value);
+    } else {
+      deserialized_data[column] = array_or_json_serializer.deserialize(
+        data.data[column],
+        manager,
+      );
+    }
+  }
+  return new DataSource(deserialized_data, data.fields, data.schema, true);
+}
 
 export class DataGridModel extends DOMWidgetModel {
   defaults() {
     return {
       ...super.defaults(),
       _model_module: DataGridModel.model_module,
       _model_module_version: DataGridModel.model_module_version,
@@ -63,14 +118,16 @@
       default_renderer: null,
       header_renderer: null,
       selection_mode: 'none',
       selections: [],
       grid_style: {},
       editable: false,
       column_widths: {},
+      horizontal_stripes: false,
+      vertical_stripes: false,
     };
   }
 
   initialize(attributes: any, options: any) {
     super.initialize(attributes, options);
 
     this.updateDataSync = this.updateDataSync.bind(this);
@@ -91,43 +148,37 @@
           content.row,
           content.column_index,
           content.value,
         );
       }
 
       if (content.event_type === 'row-changed') {
-        this.data_model.setRowData(
-          content.row,
-          content.value,
-        );
+        this.data_model.setRowData(content.row, content.value);
       }
     });
   }
 
   updateDataSync(sender: any, msg: any) {
     switch (msg.type) {
       case 'row-indices-updated':
         this.set('_visible_rows', msg.indices);
         this.save_changes();
         break;
-      case 'cell-updated':
-        this.set('_data', this.data_model.dataset);
-        this.save_changes();
-        break;
       case 'cell-edit-event':
         // Update data in widget model
-        const newData = this.get('_data');
-        newData.data[msg.row][msg.columnIndex] = msg.value;
+        const newData = this.get('_data') as DataSource;
+        newData.data[msg.column][msg.row] = msg.value;
         this.set('_data', newData);
 
         this.send(
           {
             event_type: 'cell-changed',
             region: msg.region,
             row: msg.row,
+            column: msg.column,
             column_index: msg.columnIndex,
             value: msg.value,
           },
           { ...this._view_callbacks },
         );
         break;
       default:
@@ -138,26 +189,22 @@
   syncTransformState(sender: any, value: any) {
     this.set('_transforms', value.transforms);
     this.save_changes();
   }
 
   updateData() {
     const data = this.data;
-    const schema = Private.createSchema(data);
 
     if (this.data_model) {
-      this.data_model.updateDataset({ data: data.data, schema: schema });
+      this.data_model.updateDataset(data);
       this.data_model.transformStateChanged.disconnect(this.syncTransformState);
       this.data_model.dataSync.disconnect(this.updateDataSync);
     }
 
-    this.data_model = new ViewBasedJSONModel({
-      data: data.data,
-      schema: schema,
-    });
+    this.data_model = new ViewBasedJSONModel(this.data);
 
     this.data_model.transformStateChanged.connect(this.syncTransformState);
     this.data_model.dataSync.connect(this.updateDataSync);
 
     this.updateTransforms();
     this.trigger('data-model-changed');
     this.updateSelectionModel();
@@ -201,15 +248,15 @@
         let selectionIter = sender.selections();
         // @ts-ignore
         if (typeof selectionIter.iter === 'function') {
           // Lumino 1 (JupyterLab 3)
           let selection = null;
 
           // @ts-ignore
-          selectionIter = selectionIter.iter()
+          selectionIter = selectionIter.iter();
 
           while ((selection = selectionIter.next())) {
             selections.push({
               // @ts-ignore
               r1: Math.min(selection.r1, selection.r2),
               // @ts-ignore
               r2: Math.max(selection.r1, selection.r2),
@@ -219,15 +266,15 @@
               c2: Math.max(selection.c1, selection.c2),
             });
           }
         } else {
           // Lumino 2 (JupyterLab 4)
           let selectionNode = null;
 
-          while (selectionNode = selectionIter.next()) {
+          while ((selectionNode = selectionIter.next())) {
             if (selectionNode.done) {
               break;
             }
 
             const selection = selectionNode.value;
 
             selections.push({
@@ -269,26 +316,29 @@
         clear: 'none',
       });
     }
 
     this.synchingWithKernel = false;
   }
 
-  get data(): DataGridModel.IData {
+  get data(): DataSource {
     return this.get('_data');
   }
 
   static serializers: ISerializers = {
     ...DOMWidgetModel.serializers,
     transforms: { deserialize: unpack_models as any },
     renderers: { deserialize: unpack_models as any },
     corner_renderer: { deserialize: unpack_models as any },
     default_renderer: { deserialize: unpack_models as any },
     header_renderer: { deserialize: unpack_models as any },
-    _data: { deserialize: unpack_data as any },
+    _data: {
+      deserialize: deserialize_data,
+      serialize: serialize_data,
+    },
     grid_style: { deserialize: unpack_style as any },
   };
 
   static model_name = 'DataGridModel';
   static model_module = MODULE_NAME;
   static model_module_version = MODULE_VERSION;
 
@@ -299,15 +349,15 @@
   data_model: ViewBasedJSONModel;
   selectionModel: BasicSelectionModel | null;
   synchingWithKernel = false;
   _view_callbacks: ICallbacks;
 }
 
 /**
- * Helper function to conver snake_case strings to camelCase.
+ * Helper function to convert snake_case strings to camelCase.
  * Assumes all strings are valid snake_case (all lowercase).
  * @param string snake_case string
  * @returns camelCase string
  */
 function camelCase(string: string): string {
   string = string.toLowerCase();
   const charArray = [];
@@ -345,44 +395,14 @@
       return model._function;
     });
   } else {
     return Promise.resolve(value);
   }
 }
 
-// modified from ipywidgets original
-function unpack_data(
-  value: any | Dict<unknown> | string | (Dict<unknown> | string)[],
-  manager: any,
-): Promise<WidgetModel | Dict<WidgetModel> | WidgetModel[] | any> {
-  if (Array.isArray(value)) {
-    const unpacked: any[] = [];
-    value.forEach((sub_value, key) => {
-      unpacked.push(unpack_data(sub_value, manager));
-    });
-    return Promise.all(unpacked);
-  } else if (value instanceof Object && typeof value !== 'string') {
-    const unpacked: { [key: string]: any } = {};
-    Object.keys(value).forEach((key) => {
-      unpacked[key] = unpack_data(value[key], manager);
-    });
-    return resolvePromisesDict(unpacked);
-  } else if (value === '$NaN$') {
-    return Promise.resolve(Number.NaN);
-  } else if (value === '$Infinity$') {
-    return Promise.resolve(Number.POSITIVE_INFINITY);
-  } else if (value === '$NegInfinity$') {
-    return Promise.resolve(Number.NEGATIVE_INFINITY);
-  } else if (value === '$NaT$') {
-    return Promise.resolve(new Date('INVALID'));
-  } else {
-    return Promise.resolve(value);
-  }
-}
-
 export class DataGridView extends DOMWidgetView {
   _createElement(tagName: string) {
     const panelWidget = Private.getWidgetPanel();
     this.luminoWidget = new panelWidget({ view: this });
     this._initializeTheme();
     return this.luminoWidget.node;
   }
@@ -404,18 +424,15 @@
     MessageLoop.postMessage(
       this.luminoWidget,
       Widget.ResizeMessage.UnknownSize,
     );
   };
 
   // ipywidgets 7 compatibility
-  _processLuminoMessage(
-    msg: Message,
-    _super: any,
-  ): void {
+  _processLuminoMessage(msg: Message, _super: any): void {
     _super.call(this, msg);
 
     switch (msg.type) {
       case 'after-show':
         if (this.luminoWidget.isVisible) {
           this.manageResizeEvent();
         }
@@ -436,23 +453,35 @@
   render(): Promise<void> {
     this.el.classList.add('datagrid-container');
     window.addEventListener('resize', this.manageResizeEvent);
     this.once('remove', () => {
       window.removeEventListener('resize', this.manageResizeEvent);
     });
 
+    const grid_style = this.model.get('grid_style');
+    if (this.model.get('horizontal_stripes') || this.model.get('vertical_stripes')) {
+      const index = this.model.get('horizontal_stripes')
+        ? 'rowBackgroundColor'
+        : 'columnBackgroundColor';
+      grid_style[index] = (index: number): string => {
+        return index % 2 === 0
+          ? Theme.getBackgroundColor(1)
+          : Theme.getBackgroundColor(2);
+      };
+    }
+
     this.grid = new FeatherGrid({
       defaultSizes: {
         rowHeight: this.model.get('base_row_size'),
         columnWidth: this.model.get('base_column_size'),
         rowHeaderWidth: this.model.get('base_row_header_size'),
         columnHeaderHeight: this.model.get('base_column_header_size'),
       },
       headerVisibility: this.model.get('header_visibility'),
-      style: this.model.get('grid_style'),
+      style: grid_style,
     });
 
     this.grid.columnWidths = this.model.get('column_widths');
     this.grid.editable = this.model.get('editable');
     // this.default_renderer must be created after setting grid.isLightTheme
     // for proper color variable initialization
     this.grid.isLightTheme = this._isLightTheme;
@@ -763,98 +792,55 @@
   default_renderer: CellRendererView;
   header_renderer: CellRendererView;
   grid: FeatherGrid;
   luminoWidget: JupyterLuminoPanelWidget;
   model: DataGridModel;
   backboneModel: DataGridModel;
 
+  horizontal_stripes: boolean;
+  vertical_stripes: boolean;
+
   // keep undefined since widget initializes before constructor
   private _isLightTheme: boolean;
 }
 
 export {
   BarRendererModel,
   BarRendererView,
+  ImageRendererModel,
+  ImageRendererView,
   HyperlinkRendererModel,
-  HyperlinkRendererView, TextRendererModel,
-  TextRendererView
+  HyperlinkRendererView,
+  TextRendererModel,
+  TextRendererView,
+  HtmlRendererModel,
+  HtmlRendererView,
 } from './cellrenderer';
 export { VegaExprModel, VegaExprView } from './vegaexpr';
 
-
 export namespace DataGridModel {
-  /**
-   * An options object for initializing the data model.
-   */
   export interface IData {
-    data: ViewBasedJSONModel.DataSource;
+    data: DataSource;
     schema: ISchema;
     fields: { [key: string]: null }[];
   }
   export interface IField {
-    readonly name: string | any[];
+    readonly name: string;
     readonly type: string;
     readonly rows: any[];
   }
   export interface ISchema {
     readonly fields: IField[];
-    readonly primaryKey: string[];
+    readonly primaryKey: string | string[];
     readonly primaryKeyUuid: string;
   }
 }
 
 /**
  * The namespace for the module implementation details.
  */
 namespace Private {
   export function getWidgetPanel(): any {
     // @ts-ignore needed for ipywidget 7.x compatibility
     return JupyterLuminoPanelWidget ?? JupyterPhosphorPanelWidget;
   }
-
-
-  /**
-   * Creates a valid JSON Table Schema from the schema provided by pandas.
-   *
-   * @param data - The data that has been synced from the kernel.
-   */
-  export function createSchema(
-    data: DataGridModel.IData,
-  ): ViewBasedJSONModel.ISchema {
-    // Construct a new array of schema fields based on the keys in data.fields
-    // Note: this accounts for how tuples/lists may be serialized into strings
-    // in the case of multiIndex columns.
-    const fields: ViewBasedJSONModel.IField[] = [];
-    data.fields.forEach((val: { [key: string]: null }, i: number) => {
-      const rows = Array.isArray(data.schema.fields[i].name)
-        ? <any[]>data.schema.fields[i].name
-        : <string[]>[data.schema.fields[i].name];
-      const field = {
-        name: Object.keys(val)[0],
-        type: data.schema.fields[i].type,
-        rows: rows,
-      };
-      fields.push(field);
-    });
-
-    // Updating the primary key to account for a multiIndex primary key.
-    const primaryKey = data.schema.primaryKey.map((key: string) => {
-      for (let i = 0; i < data.schema.fields.length; i++) {
-        const curFieldKey = Array.isArray(key)
-          ? data.schema.fields[i].name[0]
-          : data.schema.fields[i].name;
-        const newKey = Array.isArray(key) ? key[0] : key;
-
-        if (curFieldKey == newKey) {
-          return Object.keys(data.fields[i])[0];
-        }
-      }
-      return 'unreachable';
-    });
-
-    return {
-      primaryKey: primaryKey,
-      primaryKeyUuid: data.schema.primaryKeyUuid,
-      fields: fields,
-    };
-  }
 }
```

### Comparing `ipydatagrid-1.2.1/js/extension.ts` & `ipydatagrid-1.3.0/js/extension.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/js/feathergrid.ts` & `ipydatagrid-1.3.0/js/feathergrid.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import { toArray } from '@lumino/algorithm';
 import { CommandRegistry } from '@lumino/commands';
 import {
   BasicSelectionModel,
   CellRenderer,
   DataGrid,
   DataModel,
   RendererMap,
@@ -430,18 +429,14 @@
     });
 
     this.contextMenu = new FeatherGridContextMenu({
       grid: this.grid,
       commands: this._createCommandRegistry(),
     });
 
-    // Replace method of copying to clipboard with one that allows
-    // a ClipboardEvent to reach document.body
-    this.grid.copyToClipboard = this.copyToClipboard.bind(this.grid);
-
     this.grid.dataModel = this._dataModel;
     this.grid.keyHandler = new KeyHandler();
     const mouseHandler = new FeatherGridMouseHandler(this);
     mouseHandler.cellClicked.connect(
       (sender: FeatherGridMouseHandler, hit: DataGrid.HitTestResult) => {
         if (!this.grid.dataModel) {
           return;
@@ -582,111 +577,110 @@
       isLightTheme: this._isLightTheme,
       grid: this.grid,
     });
 
     this._updateHeaderRenderer();
   }
 
-  copyToClipboard(): void {
-    const grid = <DataGrid>(<unknown>this);
+  downloadAsCsv(isSelection: boolean): void {
+    let rowCount, colCount;
+    let r1 = 0,
+      c1 = 0,
+      r2,
+      c2;
+
+    const grid = this.grid;
     // Fetch the data model.
     const dataModel = grid.dataModel;
 
     // Bail early if there is no data model.
     if (!dataModel) {
       return;
     }
 
-    // Fetch the selection model.
-    const selectionModel = grid.selectionModel;
-
-    // Bail early if there is no selection model.
-    if (!selectionModel) {
-      return;
-    }
-
-    // Coerce the selections to an array.
-    const selections = toArray(selectionModel.selections());
-
-    // Bail early if there are no selections.
-    if (selections.length === 0) {
-      return;
-    }
-
-    // Alert that multiple selections cannot be copied.
-    if (selections.length > 1) {
-      alert('Cannot copy multiple grid selections.');
-      return;
-    }
-
     // Fetch the model counts.
     const br = dataModel.rowCount('body');
     const bc = dataModel.columnCount('body');
 
-    // Bail early if there is nothing to copy.
+    // Bail early if there is nothing to save.
     if (br === 0 || bc === 0) {
       return;
     }
 
-    // Unpack the selection.
-    let { r1, c1, r2, c2 } = selections[0];
-
-    // Clamp the selection to the model bounds.
-    r1 = Math.max(0, Math.min(r1, br - 1));
-    c1 = Math.max(0, Math.min(c1, bc - 1));
-    r2 = Math.max(0, Math.min(r2, br - 1));
-    c2 = Math.max(0, Math.min(c2, bc - 1));
-
-    // Ensure the limits are well-orderd.
-    if (r2 < r1) [r1, r2] = [r2, r1];
-    if (c2 < c1) [c1, c2] = [c2, c1];
-
     // Fetch the header counts.
     let rhc = dataModel.columnCount('row-header');
     let chr = dataModel.rowCount('column-header');
 
     // Unpack the copy config.
-    const separator = grid.copyConfig.separator;
     const format = grid.copyConfig.format;
     const headers = grid.copyConfig.headers;
-    const warningThreshold = grid.copyConfig.warningThreshold;
 
-    // Compute the number of cells to be copied.
-    let rowCount = r2 - r1 + 1;
-    let colCount = c2 - c1 + 1;
-    switch (headers) {
-      case 'none':
-        rhc = 0;
-        chr = 0;
-        break;
-      case 'row':
-        chr = 0;
-        colCount += rhc;
-        break;
-      case 'column':
-        rhc = 0;
-        rowCount += chr;
-        break;
-      case 'all':
-        rowCount += chr;
-        colCount += rhc;
-        break;
-      default:
-        throw 'unreachable';
-    }
-
-    // Compute the total cell count.
-    const cellCount = rowCount * colCount;
-
-    // Allow the user to cancel a large copy request.
-    if (cellCount > warningThreshold) {
-      const msg = `Copying ${cellCount} cells may take a while. Continue?`;
-      if (!window.confirm(msg)) {
+    if (isSelection) {
+      // Fetch the selection model.
+      const selectionModel = grid.selectionModel;
+
+      // Bail early if there is no selection model.
+      if (!selectionModel) {
+        return;
+      }
+
+      // Coerce the selections to an array.
+      const selections = Array.from(selectionModel.selections());
+
+      // Bail early if there are no selections.
+      if (selections.length === 0) {
+        return;
+      }
+
+      // Alert that multiple selections cannot be saved.
+      if (selections.length > 1) {
+        alert('Cannot save multiple grid selections.');
         return;
       }
+
+      // Unpack the selection.
+      ({ r1, c1, r2, c2 } = selections[0]);
+
+      // Clamp the selection to the model bounds.
+      r1 = Math.max(0, Math.min(r1, br - 1));
+      c1 = Math.max(0, Math.min(c1, bc - 1));
+      r2 = Math.max(0, Math.min(r2, br - 1));
+      c2 = Math.max(0, Math.min(c2, bc - 1));
+
+      // Ensure the limits are well-orderd.
+      if (r2 < r1) [r1, r2] = [r2, r1];
+      if (c2 < c1) [c1, c2] = [c2, c1];
+
+      // Compute the number of cells to be saved.
+      rowCount = r2 - r1 + 1;
+      colCount = c2 - c1 + 1;
+      switch (headers) {
+        case 'none':
+          rhc = 0;
+          chr = 0;
+          break;
+        case 'row':
+          chr = 0;
+          colCount += rhc;
+          break;
+        case 'column':
+          rhc = 0;
+          rowCount += chr;
+          break;
+        case 'all':
+          rowCount += chr;
+          colCount += rhc;
+          break;
+        default:
+          throw 'unreachable';
+      }
+    } else {
+      // Saving all the cells, headers included
+      rowCount = br + chr;
+      colCount = bc + rhc;
     }
 
     // Set up the format args.
     const args = {
       region: 'body' as DataModel.CellRegion,
       row: 0,
       column: 0,
@@ -740,36 +734,28 @@
       }
 
       // Save the row of cells.
       rows[j] = cells;
     }
 
     // Convert the cells into lines.
-    const lines = rows.map((cells) => cells.join(separator));
+    const lines = rows.map((cells) => cells.join(','));
 
     // Convert the lines into text.
     const text = lines.join('\n');
 
-    // Copy the text to the clipboard.
-    const textArea = document.createElement('textarea');
-    textArea.innerHTML = text;
-
-    // Text area has to be visible on page for copy without Clipboard API,
-    // So we create an "invisible" element, add it to the body, then remove
-    // when no longer needed.
-
-    textArea.style.height = '0px';
-    textArea.style.width = '0px';
-    textArea.style.overflow = 'hidden';
-    textArea.id = 'ipydatagrid-textarea';
-    textArea.style.position = 'absolute';
-    document.body.appendChild(textArea);
-    textArea.select();
-    document.execCommand('copy');
-    document.body.removeChild(textArea);
+    const blob = new Blob([text], { type: 'text/csv' });
+
+    // Create a link element, simulate a click, and remove link element
+    const a = document.createElement('a');
+    a.download = 'out.csv';
+    a.href = window.URL.createObjectURL(blob);
+    document.body.appendChild(a);
+    a.click();
+    document.body.removeChild(a);
   }
 
   /**
    * A signal emitted when a grid cell is clicked.
    */
   get cellClicked(): ISignal<this, FeatherGrid.ICellClickedEvent> {
     return this._cellClicked;
@@ -990,14 +976,69 @@
             forceX: false,
             forceY: false,
             mode: 'value',
           });
         },
       },
     );
+    commands.addCommand(
+      FeatherGridContextMenu.CommandID.CopySelectionToClipboard,
+      {
+        label: 'Copy Selection to Clipboard',
+        mnemonic: -1,
+        isEnabled: () => {
+          return (
+            this.grid.selectionModel !== null &&
+            !this.grid.selectionModel.isEmpty
+          );
+        },
+        execute: () => {
+          this.grid.copyToClipboard();
+        },
+      },
+    );
+    commands.addCommand(FeatherGridContextMenu.CommandID.SaveSelectionAsCsv, {
+      label: 'Download Selection as CSV',
+      mnemonic: -1,
+      isEnabled: () => {
+        return (
+          this.grid.selectionModel !== null && !this.grid.selectionModel.isEmpty
+        );
+      },
+      execute: () => {
+        this.downloadAsCsv(true);
+      },
+    });
+    commands.addCommand(FeatherGridContextMenu.CommandID.SaveAllAsCsv, {
+      label: 'Download All as CSV',
+      mnemonic: -1,
+      execute: () => {
+        this.downloadAsCsv(false);
+      },
+    });
+    commands.addCommand(FeatherGridContextMenu.CommandID.SortClear, {
+      label: 'No Sort',
+      mnemonic: 1,
+      execute: (args) => {
+        const commandArgs = <FeatherGridContextMenu.CommandArgs>args;
+        const schemaIndex: number = this._dataModel.getSchemaIndex(
+          commandArgs.region,
+          commandArgs.columnIndex,
+        );
+        this._dataModel.removeTransform(schemaIndex, 'sort');
+      },
+    });
+    commands.addCommand(FeatherGridContextMenu.CommandID.ClearSelection, {
+      label: 'Clear Selection',
+      mnemonic: -1,
+      execute: () => {
+        this.grid.selectionModel?.clear();
+      },
+    });
+
     return commands;
   }
 
   grid: DataGrid;
   backboneModel: BackBoneModel;
   contextMenu: FeatherGridContextMenu;
   private _filterDialog: InteractiveFilterDialog;
```

### Comparing `ipydatagrid-1.2.1/js/keyhandler.ts` & `ipydatagrid-1.3.0/js/keyhandler.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/js/mousehandler.ts` & `ipydatagrid-1.3.0/js/mousehandler.ts`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         hit.column,
       );
       const rowHeight = grid.rowSize('column-header', hit.row);
 
       const isMenuRow =
         (hit.region === 'column-header' &&
           hit.row ==
-          this._grid.grid.dataModel!.rowCount('column-header') - 1) ||
+            this._grid.grid.dataModel!.rowCount('column-header') - 1) ||
         (hit.region === 'corner-header' && hit.row === 0);
 
       const isMenuClick =
         hit.x > columnWidth - buttonSize - buttonPadding &&
         hit.x < columnWidth - buttonPadding &&
         hit.y > rowHeight - buttonSize - buttonPadding &&
         hit.y < rowHeight - buttonPadding &&
@@ -134,19 +134,19 @@
    * A signal emitted when a grid cell is clicked.
    */
   get cellClicked(): ISignal<this, DataGrid.HitTestResult> {
     return this._cellClicked;
   }
 
   /**
-  * Creates a CellConfig object from a hit region.
-  */
+   * Creates a CellConfig object from a hit region.
+   */
   private static createCellConfigObject(
     grid: DataGrid,
-    hit: DataGrid.HitTestResult
+    hit: DataGrid.HitTestResult,
   ): CellRenderer.CellConfig | undefined {
     const { region, row, column } = hit;
 
     // Terminate call if region is void.
     if (region === 'void') {
       return undefined;
     }
@@ -155,15 +155,15 @@
     const value = grid.dataModel!.data(region, row, column);
     const metadata = grid.dataModel!.metadata(region, row, column);
 
     // Create cell config object to retrieve cell renderer.
     const config = {
       ...hit,
       value: value,
-      metadata: metadata
+      metadata: metadata,
     } as CellRenderer.CellConfig;
 
     return config;
   }
 
   private _grid: FeatherGrid;
   private _mouseIsDown = false;
```

### Comparing `ipydatagrid-1.2.1/js/plugin.ts` & `ipydatagrid-1.3.0/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/js/utils.ts` & `ipydatagrid-1.3.0/js/utils.ts`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 const d3Color: any = require('d3-color');
 import { CellGroup } from '@lumino/datagrid';
+import { DataSource } from './datasource';
 
 export namespace ArrayUtils {
   /**
    * Returns the locations of multi-index column arrays.
    * @param model the datamodel instance.
    */
   export function generateMultiIndexArrayLocations(model: any): number[] {
@@ -76,35 +77,47 @@
   /**
    * Returns an array of [mergedCellSiblingGroup]. Each element represents a column of rows.
    * The 0th row will be the top level group, and the n-th will be the last.
    * @param model data model with schema and data fields
    * @returns index-based locations of all mutli-index rows.
    */
   export function generateRowMergedCellLocations(model: any): number[][][][] {
+    const dataset = model._dataset as DataSource;
+
     // Removing internal primary key identifier.
-    const primaryKey = model._dataset.schema.primaryKey.slice(
+    const primaryKey = dataset.schema.primaryKey.slice(
       0,
-      model._dataset.schema.primaryKey.length - 1,
+      dataset.schema.primaryKey.length - 1,
     );
 
     // Terminate if we're not dealing with nested row headers.
     if (!(primaryKey.length > 1)) {
       return [];
     }
 
-    const data = model._dataset.data;
+    const data = dataset.data;
     const retArr = [];
     let curCol = [];
 
-    let prevVal = undefined;
     for (let i = 0; i < primaryKey.length; i++) {
+      let prevVal = undefined;
       let curMergedRange: any = [];
-      for (let j = 0; j < data.length; j++) {
-        const curVal = data[j][primaryKey[i]];
-        if (curMergedRange.length == 0 || prevVal == curVal) {
+      for (let j = 0; j < dataset.length; j++) {
+        const curVal = data[primaryKey[i]][j];
+        // if (curMergedRange.length == 0 || prevVal == curVal) {
+        const [parentGroupStart, parentGroupEnd] = getParentGroupPosition(
+            retArr,
+            j,
+            i,
+          );
+        if (
+            curMergedRange.length == 0 || (prevVal == curVal) &&
+            curMergedRange[0][0] >= parentGroupStart &&
+            j <= parentGroupEnd
+          ) {
           curMergedRange.push([j, i]);
         } else {
           curCol.push(curMergedRange);
           curMergedRange = [[j, i]];
         }
         prevVal = curVal;
       }
@@ -113,14 +126,41 @@
       curCol = [];
     }
 
     return retArr;
   }
 
   /**
+   * Returns [startRow, endRow] of parent column at the same row position.
+   * The 0th row will be the top level group, and the n-th will be the last.
+   * @param retArr array of merge cellgroups in all previous columns
+   * @param rowNum current row number
+   * @param colNum current column number
+   * @returns.[startRow, endRow] of previous column
+   */
+  function getParentGroupPosition(
+    retArr: any,
+    rowNum: number,
+    colNum: number,
+  ): number[] {
+    if (colNum === 0) {return [0, rowNum]};
+    for (let i = 0; i < retArr[colNum-1].length; i++) {
+      // iterate mergegroups of previous row
+      const curMergedGroup = retArr[colNum-1][i];
+      const curMergedGroupLen = curMergedGroup.length;
+      const firstRow = curMergedGroup[0][0];
+      const lastRow = curMergedGroup[curMergedGroupLen - 1][0];
+      if (rowNum >= firstRow && rowNum <= lastRow) {
+        return [firstRow!, lastRow!];
+      }
+    }
+    return [];
+  }
+
+  /**
    * Checks whether the merged cell ranges conform to a valid hierarchy.
    * @param retVal boolean
    */
   export function validateMergingHierarchy(retVal: number[][][][]): boolean {
     let prevLevelLength;
     for (const mergeRange of retVal) {
       // First element - setting up the value of prevLevelLength
```

### Comparing `ipydatagrid-1.2.1/js/vegaexpr.ts` & `ipydatagrid-1.3.0/js/vegaexpr.ts`

 * *Files 0% similar despite different names*

```diff
@@ -121,12 +121,12 @@
   }
 
   model: VegaExprModel;
 }
 
 export interface ParsedVegaExpr {
   /**
-   * A JavaScript soring literal describing
+   * A JavaScript storing literal describing
    * the converted vega expression
    */
   code: string;
 }
```

### Comparing `ipydatagrid-1.2.1/js/core/barrenderer.ts` & `ipydatagrid-1.3.0/js/core/barrenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/js/core/filterMenu.ts` & `ipydatagrid-1.3.0/js/core/filterMenu.ts`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import { Widget, BoxPanel } from '@lumino/widgets';
 
 import { VirtualDOM, VirtualElement, h } from '@lumino/virtualdom';
 
 import { FilterValueRenderer } from './valueRenderer';
 
 import { Theme } from '../utils';
+import { DataSource } from '../datasource';
 
 /**
  * An interactive widget to add filter transformations to the data model.
  */
 export class InteractiveFilterDialog extends BoxPanel {
   /**
    * Construct a new InteractiveFilterDialog.
@@ -147,17 +148,17 @@
       return;
     }
 
     const value =
       this._mode === 'condition'
         ? <Transform.FilterValue>this._filterValue
         : this._uniqueValueStateManager.getValues(
-          this.region,
-          this._columnIndex,
-        );
+            this.region,
+            this._columnIndex,
+          );
 
     // Construct transform
     const transform: Transform.TransformSpec = {
       type: 'filter',
       columnIndex: this.model.getSchemaIndex(this._region, this._columnIndex),
       operator: this._filterOperator,
       value: value,
@@ -248,49 +249,41 @@
       throw 'unreachable';
     }
   }
 
   /**
    * Displays the unique values of a column.
    */
-  async _renderUniqueVals() {
+  _renderUniqueVals() {
     const uniqueVals = this._model.uniqueValues(
       this._region,
       this._columnIndex,
     );
-
-    uniqueVals.then((value) => {
-      const items = value.map((val, i) => {
-        return { index: i, uniqueVals: val };
-      });
-
-      const data: ViewBasedJSONModel.IData = {
-        schema: {
-          fields: [
-            { name: 'index', type: 'integer', rows: [] },
-            { name: 'uniqueVals', type: 'number', rows: [] },
-          ],
-          primaryKey: ['index'],
-          primaryKeyUuid: 'index',
-        },
-        data: items,
-      };
-      this._uniqueValueGrid.dataModel = new ViewBasedJSONModel(data);
-
-      const sortTransform: Transform.Sort = {
-        type: 'sort',
-        columnIndex: this.model.getSchemaIndex(this._region, 0),
-        desc: false,
-      };
-
-      // Sort items in filter-by-value menu in ascending order
-      (<ViewBasedJSONModel>this._uniqueValueGrid.dataModel).addTransform(
-        sortTransform,
-      );
-    });
+    const data = new DataSource(
+      { index: [...uniqueVals.keys()], uniqueVals },
+      [{ index: null }, { uniqueVals: null }],
+      {
+        fields: [
+          { name: 'index', type: 'integer', rows: [] },
+          { name: 'uniqueVals', type: 'number', rows: [] },
+        ],
+        primaryKey: ['index'],
+        primaryKeyUuid: 'index',
+      },
+    );
+    this._uniqueValueGrid.dataModel = new ViewBasedJSONModel(data);
+    const sortTransform: Transform.Sort = {
+      type: 'sort',
+      columnIndex: this.model.getSchemaIndex(this._region, 0),
+      desc: false,
+    };
+    // Sort items in filter-by-value menu in ascending order
+    (<ViewBasedJSONModel>this._uniqueValueGrid.dataModel).addTransform(
+      sortTransform,
+    );
   }
 
   /**
    * Checks whether all unique elements in the column
    * are present as "selected" in the state. This
    * function is used to determine whether the
    * "Select all" button should be ticked when
@@ -303,32 +296,30 @@
     }
 
     const uniqueVals = this._model.uniqueValues(
       this._region,
       this._columnIndex,
     );
 
-    uniqueVals.then((values) => {
-      let showAsChecked = true;
-      for (const value of values) {
-        // If there is a unique value which is not present in the state then it is
-        // not ticked, and therefore we should not tick the "Select all" checkbox.
-        if (
-          !this._uniqueValueStateManager.has(
-            this._region,
-            this._columnIndex,
-            value,
-          )
-        ) {
-          showAsChecked = false;
-          break;
-        }
+    let showAsChecked = true;
+    for (const value of uniqueVals) {
+      // If there is a unique value which is not present in the state then it is
+      // not ticked, and therefore we should not tick the "Select all" checkbox.
+      if (
+        !this._uniqueValueStateManager.has(
+          this._region,
+          this._columnIndex,
+          value,
+        )
+      ) {
+        showAsChecked = false;
+        break;
       }
-      this._selectAllCheckbox.checked = showAsChecked;
-    });
+    }
+    this._selectAllCheckbox.checked = showAsChecked;
   }
 
   /**
    * Open the menu at the specified location.
    *
    * @param options - The additional options for opening the menu.
    */
@@ -347,15 +338,15 @@
     this.hasFilter =
       this._model.getFilterTransform(
         this.model.getSchemaIndex(this._region, this._columnIndex),
       ) !== undefined;
 
     this.userInteractedWithDialog = false;
 
-    // Determines whether we should or not tick the "Select all" chekcbox
+    // Determines whether we should or not tick the "Select all" checkbox
     this.updateSelectAllCheckboxState();
 
     // Update styling on unique value grid
     this._uniqueValueGrid.style = {
       voidColor: Theme.getBackgroundColor(),
       backgroundColor: Theme.getBackgroundColor(),
       gridLineColor: Theme.getBackgroundColor(),
@@ -584,16 +575,16 @@
         type: 'text',
         style: {
           marginRight: '5px',
           width: '200px',
           background: 'var(--ipydatagrid-filter-dlg-bgcolor,white)',
           visibility:
             this._filterOperator === 'empty' ||
-              this._filterOperator === 'notempty' ||
-              this._mode === 'value'
+            this._filterOperator === 'notempty' ||
+            this._mode === 'value'
               ? 'hidden'
               : 'visible',
         },
         // Assigning a random key ensures that this element is always
         // rerendered
         key: String(Math.random()),
         oninput: (evt) => {
@@ -733,15 +724,15 @@
   }
 
   /**
    * Creates a Promise that resolves to a `VirtualElement` to display the unique
    * values of a column.
    */
   protected async createUniqueValueNodes(): Promise<VirtualElement> {
-    const uniqueVals = await this._model.uniqueValues(
+    const uniqueVals = this._model.uniqueValues(
       this._region,
       this._columnIndex,
     );
     const optionElems = uniqueVals.map((val) => {
       return h.option({ value: val }, String(val));
     });
 
@@ -1145,34 +1136,32 @@
           ...(op === 'between' && { selected: '' }),
         },
         'Is in between',
       ),
     ];
   }
 
-  async addRemoveAllUniqueValuesToState(add: boolean) {
+  addRemoveAllUniqueValuesToState(add: boolean) {
     const uniqueVals = this.model.uniqueValues(this._region, this._columnIndex);
 
-    return uniqueVals.then((values) => {
-      for (const value of values) {
-        if (add) {
-          this._uniqueValueStateManager.add(
-            this._region,
-            this._columnIndex,
-            value,
-          );
-        } else {
-          this._uniqueValueStateManager.remove(
-            this._region,
-            this._columnIndex,
-            value,
-          );
-        }
+    for (const value of uniqueVals) {
+      if (add) {
+        this._uniqueValueStateManager.add(
+          this._region,
+          this._columnIndex,
+          value,
+        );
+      } else {
+        this._uniqueValueStateManager.remove(
+          this._region,
+          this._columnIndex,
+          value,
+        );
       }
-    });
+    }
   }
 
   /**
    * Returns a reference to the data model used for this menu.
    */
   get model(): ViewBasedJSONModel {
     return this._model;
@@ -1543,18 +1532,17 @@
     };
 
     // User is clicking for the first time when no filter is applied
     if (
       !this._filterDialog.hasFilter &&
       !this._filterDialog.userInteractedWithDialog
     ) {
-      this._filterDialog.addRemoveAllUniqueValuesToState(true).then(() => {
-        this._filterDialog.userInteractedWithDialog = true;
-        updateCheckState();
-      });
+      this._filterDialog.addRemoveAllUniqueValuesToState(true);
+      this._filterDialog.userInteractedWithDialog = true;
+      updateCheckState();
     } else {
       updateCheckState();
     }
   }
 
   private _uniqueValuesSelectionState: UniqueValueStateManager;
   private _filterDialog: InteractiveFilterDialog;
```

### Comparing `ipydatagrid-1.2.1/js/core/headerRenderer.ts` & `ipydatagrid-1.3.0/js/core/headerRenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/js/core/transform.ts` & `ipydatagrid-1.3.0/js/core/transform.ts`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,25 @@
   };
 
   /**
    * A declarative spec for the `Filter` transformation.
    */
   export type Filter = {
     /**
-     * A type alias for this trasformation.
+     * A type alias for this transformation.
      */
     type: 'filter';
 
     /**
      * The column in the data schema to apply the transformation to.
      */
     columnIndex: number;
 
     /**
-     * The operator for this trasformation.
+     * The operator for this transformation.
      */
     operator: FilterOperator;
 
     /**
      * The value(s) to apply for this transformation.
      */
     value: string | string[] | number | number[];
```

### Comparing `ipydatagrid-1.2.1/js/core/transformExecutors.ts` & `ipydatagrid-1.3.0/js/core/transformExecutors.ts`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import { ViewBasedJSONModel } from './viewbasedjsonmodel';
-
-import { toArray, filter } from '@lumino/algorithm';
+import { Dict } from '@jupyter-widgets/base';
 
 import { Transform } from './transform';
+import { DataSource } from '../datasource';
 
 import * as moment from 'moment';
 
 /**
  * An object that defines a data transformation executor.
  */
 export abstract class TransformExecutor {
@@ -19,15 +18,15 @@
 /**
  * The namespace for the `Transform` class statics.
  */
 export namespace TransformExecutor {
   /**
    * A read only type for the input/output of .apply().
    */
-  export type IData = Readonly<ViewBasedJSONModel.IData>;
+  export type IData = Readonly<DataSource>;
 }
 
 /**
  * A transformation that filters a single field by the provided operator and
  * value.
  *
  * Note: This is a WIP
@@ -45,152 +44,167 @@
 
   /**
    * Apply a transformation to the provided data.
    *
    * @param input - The data to be operated on.
    */
   public apply(input: TransformExecutor.IData): TransformExecutor.IData {
-    let filterFunc: any;
+    let filterFunc: (idx: number) => boolean;
+    const field = this._options.field;
     switch (this._options.operator) {
       case '>':
-        filterFunc = (item: any) => {
+        filterFunc = (idx: number) => {
           if (['date', 'datetime', 'time'].includes(this._options.dType)) {
-            const target = moment.default.utc(item[this._options.field]);
+            const target = moment.default.utc(input.data[field][idx]);
             const value = moment.default.utc(this._options.value);
             return target.isAfter(value, 'day');
           }
-          return item[this._options.field] > this._options.value;
+          return input.data[field][idx] > this._options.value;
         };
         break;
       case '<':
-        filterFunc = (item: any) => {
+        filterFunc = (idx: number) => {
           if (['date', 'datetime', 'time'].includes(this._options.dType)) {
-            const target = moment.default.utc(item[this._options.field]);
+            const target = moment.default.utc(input.data[field][idx]);
             const value = moment.default.utc(this._options.value);
             return target.isBefore(value, 'day');
           }
-          return item[this._options.field] < this._options.value;
+          return input.data[field][idx] < this._options.value;
         };
         break;
       case '<=':
-        filterFunc = (item: any) => {
+        filterFunc = (idx: number) => {
           if (['date', 'datetime', 'time'].includes(this._options.dType)) {
-            const target = moment.default.utc(item[this._options.field]);
+            const target = moment.default.utc(input.data[field][idx]);
             const value = moment.default.utc(this._options.value);
             return target.isSameOrBefore(value, 'day');
           }
-          return item[this._options.field] <= this._options.value;
+          return input.data[field][idx] <= this._options.value;
         };
         break;
       case '>=':
-        filterFunc = (item: any) => {
+        filterFunc = (idx: number) => {
           if (['date', 'datetime', 'time'].includes(this._options.dType)) {
-            const target = moment.default.utc(item[this._options.field]);
+            const target = moment.default.utc(input.data[field][idx]);
             const value = moment.default.utc(this._options.value);
             return target.isSameOrAfter(value, 'day');
           }
-          return item[this._options.field] >= this._options.value;
+          return input.data[field][idx] >= this._options.value;
         };
         break;
       case '=':
-        filterFunc = (item: any) => {
+        filterFunc = (idx: number) => {
           if (['date', 'datetime', 'time'].includes(this._options.dType)) {
-            const target = moment.default.utc(item[this._options.field]);
+            const target = moment.default.utc(input.data[field][idx]);
             const value = moment.default.utc(this._options.value);
             return target.isSame(value);
           }
-          return item[this._options.field] == this._options.value;
+          return input.data[field][idx] == this._options.value;
         };
         break;
       case '!=':
-        filterFunc = (item: any) => {
+        filterFunc = (idx: number) => {
           if (['date', 'datetime', 'time'].includes(this._options.dType)) {
-            const target = moment.default.utc(item[this._options.field]);
+            const target = moment.default.utc(input.data[field][idx]);
             const value = moment.default.utc(this._options.value);
             return !target.isSame(value);
           }
-          return item[this._options.field] !== this._options.value;
+          return input.data[field][idx] !== this._options.value;
         };
         break;
       case 'empty':
-        filterFunc = (item: any) => {
-          return item[this._options.field] === null;
+        filterFunc = (idx: number) => {
+          return input.data[field][idx] === null;
         };
         break;
       case 'notempty':
-        filterFunc = (item: any) => {
-          return item[this._options.field] !== null;
+        filterFunc = (idx: number) => {
+          return input.data[field][idx] !== null;
         };
         break;
       case 'in':
-        filterFunc = (item: any) => {
+        filterFunc = (idx: number) => {
           const values = <any[]>this._options.value;
-          return values.includes(item[this._options.field]);
+          return values.includes(input.data[field][idx]);
         };
         break;
       case 'between':
-        filterFunc = (item: any) => {
+        filterFunc = (idx: number) => {
           const values = <any[]>this._options.value;
 
           if (['date', 'datetime', 'time'].includes(this._options.dType)) {
-            const target = moment.default.utc(item[this._options.field]);
+            const target = moment.default.utc(input.data[field][idx]);
             const lowValue = moment.default.utc(values[0]);
             const highValue = moment.default.utc(values[1]);
 
             return target.isBetween(lowValue, highValue, 'day');
           }
 
           return (
-            item[this._options.field] > values[0] &&
-            item[this._options.field] < values[1]
+            input.data[field][idx] > values[0] &&
+            input.data[field][idx] < values[1]
           );
         };
         break;
       case 'startswith':
-        filterFunc = (item: any) => {
-          return item[this._options.field].startsWith(this._options.value);
+        filterFunc = (idx: number) => {
+          return input.data[field][idx].startsWith(this._options.value);
         };
         break;
       case 'endswith':
-        filterFunc = (item: any) => {
-          return item[this._options.field].endsWith(this._options.value);
+        filterFunc = (idx: number) => {
+          return input.data[field][idx].endsWith(this._options.value);
         };
         break;
       case 'stringContains':
-        filterFunc = (item: any) => {
-          return String(item[this._options.field])
+        filterFunc = (idx: number) => {
+          return String(input.data[field][idx])
             .toLowerCase()
             .includes(String(this._options.value).toLowerCase());
         };
         break;
       case 'contains':
-        filterFunc = (item: any) => {
-          return item[this._options.field].includes(this._options.value);
+        filterFunc = (idx: number) => {
+          return input.data[field][idx].includes(this._options.value);
         };
         break;
       case '!contains':
-        filterFunc = (item: any) => {
-          return !item[this._options.field].includes(this._options.value);
+        filterFunc = (idx: number) => {
+          return !input.data[field][idx].includes(this._options.value);
         };
         break;
       case 'isOnSameDay':
-        filterFunc = (item: any) => {
-          const target = moment.default.utc(item[this._options.field]);
+        filterFunc = (idx: number) => {
+          const target = moment.default.utc(input.data[field][idx]);
           const value = moment.default.utc(this._options.value);
           return target.isSame(value, 'day');
         };
         break;
       default:
         throw 'unreachable';
     }
 
-    return {
-      schema: input.schema,
-      data: toArray(filter(input.data, filterFunc)),
-    };
+    const data: Dict<any[]> = {};
+    const indices = Array.from(Array(input.length).keys()).filter(filterFunc);
+
+    // There is a better approach for this
+    // We don't need to copy the data
+    // We should always keep the datasource intact and
+    // create the "views" in the transform's apply methods
+    // The view would then keep the indices in memory and apply the sorting
+    // upon data request
+    for (const column of Object.keys(input.data)) {
+      let i = 0;
+      data[column] = [];
+      for (const idx of indices) {
+        data[column][i++] = input.data[column][idx];
+      }
+    }
+
+    return new DataSource(data, input.fields, input.schema);
   }
 
   protected _options: FilterExecutor.IOptions;
 }
 
 /**
  * The namespace for the `FilterExecutor` class statics.
@@ -242,15 +256,15 @@
    * Apply a transformation to the provided data.
    *
    * Note: Currently ignores the `desc` parameter.
    *
    * @param input - The data to be operated on.
    */
   public apply(input: TransformExecutor.IData): TransformExecutor.IData {
-    let sortFunc: (a: any, b: any) => number;
+    let sortFunc: (a: number, b: number) => number;
     const field = this._options.field;
     const columnDataType = this._options.dType;
 
     // Adding string checks within the sort function so we do
     // not have to mutate in-place the original types of the
     // values of the column into strings. This allows the
     // displayed values to maintain their original types but
@@ -258,62 +272,80 @@
     const stringifyIfNeeded = (value: any) => {
       if (typeof value != 'string') {
         return String(value);
       }
       return value;
     };
 
+    const isNaNorNull = (value: any) => {
+      return (
+        value === null ||
+        (typeof value === 'number' && Number.isNaN(value)) ||
+        (value instanceof Date && Number.isNaN(value.getTime()))
+      );
+    };
+
+    const nanIndices = Array.from(Array(input.length).keys()).filter(
+      (idx: number) => {
+        return isNaNorNull(input.data[field][idx]);
+      },
+    );
+    const nonNanIndices = Array.from(Array(input.length).keys()).filter(
+      (idx: number) => {
+        return !isNaNorNull(input.data[field][idx]);
+      },
+    );
     if (columnDataType == 'string') {
       if (this._options.desc) {
-        sortFunc = (a: any, b: any): number => {
-          return stringifyIfNeeded(a[field]) < stringifyIfNeeded(b[field])
+        sortFunc = (a: number, b: number): number => {
+          return stringifyIfNeeded(input.data[field][a]) <
+            stringifyIfNeeded(input.data[field][b])
             ? 1
             : -1;
         };
       } else {
-        sortFunc = (a: any, b: any): number => {
-          return stringifyIfNeeded(a[field]) > stringifyIfNeeded(b[field])
+        sortFunc = (a: number, b: number): number => {
+          return stringifyIfNeeded(input.data[field][a]) >
+            stringifyIfNeeded(input.data[field][b])
             ? 1
             : -1;
         };
       }
     } else {
       if (this._options.desc) {
-        sortFunc = (a: any, b: any): number => {
-          return a[field] < b[field] ? 1 : -1;
+        sortFunc = (a: number, b: number): number => {
+          return input.data[field][a] < input.data[field][b] ? 1 : -1;
         };
       } else {
-        sortFunc = (a: any, b: any): number => {
-          return a[field] > b[field] ? 1 : -1;
+        sortFunc = (a: number, b: number): number => {
+          return input.data[field][a] > input.data[field][b] ? 1 : -1;
         };
       }
     }
 
-    const data = input.data.slice(0);
-    const sortables: any[] = [],
-      notSortables: any[] = [];
-
-    data.forEach((value: any) => {
-      const cellValue = value[field];
-      const notSortable =
-        cellValue === null ||
-        (typeof cellValue === 'number' && Number.isNaN(cellValue)) ||
-        (cellValue instanceof Date && Number.isNaN(cellValue.getTime()));
+    const data: Dict<any[]> = {};
 
-      if (notSortable) {
-        notSortables.push(value);
-      } else {
-        sortables.push(value);
+    let indices = nonNanIndices.sort(sortFunc);
+    indices = indices.concat(nanIndices);
+
+    // There is a better approach for this
+    // We don't need to copy the data
+    // We should always keep the datasource intact and
+    // create the "views" in the transform's apply methods
+    // The view would then keep the indices in memory and apply the sorting
+    // upon data request
+    for (const column of Object.keys(input.data)) {
+      let i = 0;
+      data[column] = [];
+      for (const idx of indices) {
+        data[column][i++] = input.data[column][idx];
       }
-    });
+    }
 
-    return {
-      schema: input.schema,
-      data: sortables.sort(sortFunc).concat(notSortables),
-    };
+    return new DataSource(data, input.fields, input.schema);
   }
 
   protected _options: SortExecutor.IOptions;
 }
 
 /**
  * The namespace for the `SortExecutor` class statics.
```

### Comparing `ipydatagrid-1.2.1/js/core/transformStateManager.ts` & `ipydatagrid-1.3.0/js/core/transformStateManager.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import { Transform } from './transform';
 
 import { View } from './view';
 
-import { ViewBasedJSONModel } from './viewbasedjsonmodel';
-
 import {
   SortExecutor,
   FilterExecutor,
   TransformExecutor,
 } from './transformExecutors';
 
 import { each } from '@lumino/algorithm';
 
 import { JSONExt } from '@lumino/coreutils';
 
 import { Signal, ISignal } from '@lumino/signaling';
+import { DataSource } from '../datasource';
 
 /**
  * A state manager for tracking the active transformations of a model.
  */
 export class TransformStateManager {
   protected _add(transform: Transform.TransformSpec): void {
     // Add column to state if not already present
@@ -90,31 +89,29 @@
   }
 
   /**
    * Creates a new data model View with the active transformations.
    *
    * @param data - The dataset to operate on.
    */
-  createView(data: Readonly<ViewBasedJSONModel.IData>): View {
+  createView(data: Readonly<DataSource>): View {
     const executors = this._createExecutors(data);
     let transformedData = data;
     each(executors, (transform: TransformExecutor) => {
       transformedData = transform.apply(transformedData);
     });
     return new View(transformedData);
   }
 
   /**
-   * Creates an optimzed list of TransformExecutors for the provided data.
+   * Creates an optimized list of TransformExecutors for the provided data.
    *
    * @param data - The dataset to operate on.
    */
-  private _createExecutors(
-    data: ViewBasedJSONModel.IData,
-  ): TransformExecutor[] {
+  private _createExecutors(data: Readonly<DataSource>): TransformExecutor[] {
     const sortExecutors: SortExecutor[] = [];
     const filterExecutors: FilterExecutor[] = [];
 
     Object.keys(this._state).forEach((columnIndex) => {
       const transform: TransformStateManager.IColumn = this._state[columnIndex];
 
       if (transform.sort) {
```

### Comparing `ipydatagrid-1.2.1/js/core/valueRenderer.ts` & `ipydatagrid-1.3.0/js/core/valueRenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/js/core/view.ts` & `ipydatagrid-1.3.0/js/core/view.ts`

 * *Files 16% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 | Copyright (c) 2014-2017, PhosphorJS Contributors
 |
 | Distributed under the terms of the BSD 3-Clause License.
 |
 | The full license is in the file LICENSE, distributed with this software.
 |----------------------------------------------------------------------------*/
 
-import { ReadonlyJSONObject } from '@lumino/coreutils';
+// import { ReadonlyJSONObject } from '@lumino/coreutils';
 
 import { DataModel } from '@lumino/datagrid';
-import { ViewBasedJSONModel } from './viewbasedjsonmodel';
+import { DataSource } from '../datasource';
 
 /**
  * A View implementation for immutable in-memory JSON data.
  *
  * Note: Most of this is just repurposed from JSONModel, and can likely be
  * streamlined quite a bit.
  */
 export class View {
   /**
    * Create a view with static JSON data.
    *
-   * @param options - The options for initializing the view.
+   * @param datasource - The datasource for initializing the view.
    */
-  constructor(options: View.IOptions) {
-    const split = Private.splitFields(options.schema);
-    this._data = options.data;
+  constructor(datasource: DataSource | Readonly<DataSource>) {
+    const split = Private.splitFields(datasource.schema);
+    this._data = datasource;
     this._bodyFields = split.bodyFields;
     this._headerFields = split.headerFields;
-    this._missingValues = Private.createMissingMap(options.schema);
+    this._missingValues = Private.createMissingMap(datasource.schema);
   }
 
   /**
    * Get the row count for a region in the view.
    *
    * @param region - The row region of interest.
    *
    * @returns - The row count for the region.
    */
   rowCount(region: DataModel.RowRegion): number {
     if (region === 'body') {
       return this._data.length;
     } else {
-      return this._bodyFields[0].rows.length;
+      return this._bodyFields[0]?.rows.length ?? 1;
     }
   }
 
   /**
    * Get the column count for a region in the view.
    *
    * @param region - The column region of interest.
@@ -93,30 +93,30 @@
    *
    * #### Notes
    * A `missingValue` as defined by the schema is converted to `null`.
    */
   data(region: DataModel.CellRegion, row: number, column: number): any {
     // Set up the field and value variables.
 
-    let field: ViewBasedJSONModel.IField;
+    let field: DataSource.IField;
     let value: any;
 
     // Look up the field and value for the region.
     switch (region) {
       case 'body':
         field = this._bodyFields[column];
-        value = this._data[row][field.name];
+        value = this._data.data[field.name][row];
         break;
       case 'column-header':
         field = this._bodyFields[column];
         value = field.rows[row];
         break;
       case 'row-header':
         field = this._headerFields[column];
-        value = this._data[row][field.name];
+        value = this._data.data[field.name][row];
         break;
       case 'corner-header':
         field = this._headerFields[column];
         value = field.rows[row];
         break;
       default:
         throw 'unreachable';
@@ -131,15 +131,15 @@
     // Return the final value.
     return missing ? null : value;
   }
 
   /**
    * Returns a reference to the dataset from this View.
    */
-  get dataset(): View.DataSource {
+  get dataset(): DataSource | Readonly<DataSource> {
     return this._data;
   }
 
   /**
    * Returns the index in the schema that relates to the index by region.
    *
    * @param region - The `CellRegion` of interest.
@@ -156,102 +156,34 @@
 
   /**
    * Returns a Promise that resolves to an array of unique values contained in
    * the provided column index.
    *
    * @param columnIndex - The index to retrieve unique values for.
    */
-  async uniqueValues(
-    region: DataModel.CellRegion,
-    columnIndex: number,
-  ): Promise<any[]> {
-    return new Promise((resolve, reject) => {
-      const columnName = this.metadata(region, 0, columnIndex)['name'];
-      const uniqueVals = new Set();
-      for (const row of this.dataset) {
-        uniqueVals.add(row[columnName]);
-      }
-      resolve(Array.from(uniqueVals));
-    });
+  uniqueValues(region: DataModel.CellRegion, columnIndex: number): any[] {
+    const columnName = this.metadata(region, 0, columnIndex)['name'];
+    return Array.from(new Set(this.dataset.data[columnName]));
   }
 
-  private readonly _data: View.DataSource;
-  private readonly _bodyFields: ViewBasedJSONModel.IField[];
-  private readonly _headerFields: ViewBasedJSONModel.IField[];
+  private readonly _data: DataSource | Readonly<DataSource>;
+  private readonly _bodyFields: DataSource.IField[];
+  private readonly _headerFields: DataSource.IField[];
   private readonly _missingValues: Private.MissingValuesMap | null;
 }
 
 /**
  * The namespace for the `View` class statics.
  */
 export namespace View {
   /**
-   * An object which describes a column of data in the view.
-   *
-   * #### Notes
-   * This is based on the JSON Table Schema specification:
-   * https://specs.frictionlessdata.io/table-schema/
-   */
-
-  /**
-   * An object when specifies the schema for a view.
-   *
-   * #### Notes
-   * This is based on the JSON Table Schema specification:
-   * https://specs.frictionlessdata.io/table-schema/
-   */
-  export interface ISchema {
-    /**
-     * The fields which describe the view columns.
-     *
-     * Primary key fields are rendered as row header columns.
-     */
-    readonly fields: ViewBasedJSONModel.IField[];
-
-    /**
-     * The values to treat as "missing" data.
-     *
-     * Missing values are automatically converted to `null`.
-     */
-    readonly missingValues?: string[];
-
-    /**
-     * The field names which act as primary keys.
-     *
-     * Primary key fields are rendered as row header columns.
-     */
-    readonly primaryKey?: string | string[];
-
-    /**
-     * The name of the unique identifier in the primary key array
-     */
-    readonly primaryKeyUuid: string;
-  }
-
-  /**
-   * A type alias for a data source for a JSON data model.
-   *
-   * A data source is an array of JSON object records which represent
-   * the rows of the table. The keys of the records correspond to the
-   * field names of the columns.
-   */
-  export type DataSource = ReadonlyArray<ReadonlyJSONObject>;
-
-  /**
    * An options object for initializing a view.
    */
   export interface IOptions {
     /**
-     * The schema for the for the view.
-     *
-     * The schema should be treated as an immutable object.
-     */
-    schema: ISchema;
-
-    /**
      * The data source for the view.
      *
      * The data model takes full ownership of the data source.
      */
     data: DataSource;
   }
 }
@@ -263,38 +195,38 @@
   /**
    * An object which holds the results of splitting schema fields.
    */
   export interface ISplitFieldsResult {
     /**
      * The non-primary key fields to use for the grid body.
      */
-    bodyFields: ViewBasedJSONModel.IField[];
+    bodyFields: DataSource.IField[];
 
     /**
      * The primary key fields to use for the grid headers.
      */
-    headerFields: ViewBasedJSONModel.IField[];
+    headerFields: DataSource.IField[];
   }
 
   /**
    * Split the schema fields into header and body fields.
    */
-  export function splitFields(schema: View.ISchema): ISplitFieldsResult {
+  export function splitFields(schema: DataSource.ISchema): ISplitFieldsResult {
     // Normalize the primary keys.
     let primaryKeys: string[];
     if (schema.primaryKey === undefined) {
       primaryKeys = [];
     } else if (typeof schema.primaryKey === 'string') {
       primaryKeys = [schema.primaryKey];
     } else {
       primaryKeys = schema.primaryKey;
     }
     // Separate the fields for the body and header.
-    const bodyFields: ViewBasedJSONModel.IField[] = [];
-    const headerFields: ViewBasedJSONModel.IField[] = [];
+    const bodyFields: DataSource.IField[] = [];
+    const headerFields: DataSource.IField[] = [];
     for (const field of schema.fields) {
       // Skipping the primary key unique identifier so
       // it is not rendered.
       if (field.rows[0] == schema.primaryKeyUuid) {
         continue;
       }
       if (primaryKeys.indexOf(field.name) === -1) {
@@ -315,15 +247,15 @@
 
   /**
    * Create a missing values map for a schema.
    *
    * This returns `null` if there are no missing values.
    */
   export function createMissingMap(
-    schema: View.ISchema,
+    schema: DataSource.ISchema,
   ): MissingValuesMap | null {
     // Bail early if there are no missing values.
     if (!schema.missingValues || schema.missingValues.length === 0) {
       return null;
     }
 
     // Collect the missing values into a map.
```

### Comparing `ipydatagrid-1.2.1/js/core/viewbasedjsonmodel.ts` & `ipydatagrid-1.3.0/js/core/viewbasedjsonmodel.ts`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 import { CellGroup, DataModel, MutableDataModel } from '@lumino/datagrid';
 
-import { each } from '@lumino/algorithm';
-
-import {
-  ReadonlyJSONObject,
-  ReadonlyJSONValue,
-  JSONExt,
-} from '@lumino/coreutils';
+import { ReadonlyJSONValue } from '@lumino/coreutils';
 
 import { ISignal, Signal } from '@lumino/signaling';
 
 import { Transform } from './transform';
 
 import { View } from './view';
 
 import { TransformStateManager } from './transformStateManager';
 
 import { ArrayUtils } from '../utils';
+import { DataSource } from '../datasource';
 
 /**
  * A view based data model implementation for in-memory JSON data.
  */
 export class ViewBasedJSONModel extends MutableDataModel {
   /**
    * Create a data model with static JSON data.
    *
    * @param data - The dataset for initializing the data model.
    */
-  constructor(data: ViewBasedJSONModel.IData) {
+  constructor(data: DataSource) {
     super();
     this.updateDataset(data);
 
     this._transformState = new TransformStateManager();
     // Repaint grid on transform state update
     // Note: This will also result in the `model-reset` signal being sent.
     this._transformState.changed.connect((sender, value) => {
@@ -61,45 +56,48 @@
     // Creating column merged cell groups from index locations
     this._columnCellGroups = ArrayUtils.generateColumnCellGroups(
       this._mergedColumnCellLocations,
     );
 
     // Creating merged row cell groups
     let mergedRowLocations = ArrayUtils.generateRowMergedCellLocations(this);
-    if (!ArrayUtils.validateMergingHierarchy(mergedColumnLocations)) {
+    if (!ArrayUtils.validateMergingHierarchy(mergedRowLocations)) {
       mergedRowLocations = [];
     }
-    this._rowCellGroups = ArrayUtils.generateRowCellGroups(mergedRowLocations);
+    this._mergedRowCellLocations = mergedRowLocations;
+    this._rowCellGroups = ArrayUtils.generateRowCellGroups(
+      this._mergedRowCellLocations,
+    );
   }
 
   /**
    * Sets the dataset for this model.
    *
    * @param data - The data to be set on this data model
    */
-  updateDataset(data: ViewBasedJSONModel.IData): void {
+  updateDataset(data: DataSource): void {
     this._dataset = data;
     this._updatePrimaryKeyMap();
     const view = new View(this._dataset);
     this.currentView = view;
   }
 
   /**
    * Updates the primary key map, which provides a mapping from primary key
    * value to row in the full dataset.
    */
   private _updatePrimaryKeyMap(): void {
     this._primaryKeyMap.clear();
 
-    const primaryKey = this._dataset.schema.primaryKey;
+    const primaryKey = this._dataset.schema.primaryKey as string[];
 
-    each(this._dataset.data, (rowData, index) => {
-      const keys = primaryKey.map((key) => rowData[key]);
-      this._primaryKeyMap.set(JSON.stringify(keys), index);
-    });
+    for (let idx = 0; idx < this._dataset.length; idx++) {
+      const keys = primaryKey.map((key) => this._dataset.data[key][idx]);
+      this._primaryKeyMap.set(JSON.stringify(keys), idx);
+    }
   }
 
   areCellsMerged(cell1: number[], cell2: number[]): boolean {
     const [row2, col2] = cell2;
 
     const siblings = this.getMergedSiblingCells(cell1);
 
@@ -190,32 +188,34 @@
       return this._rowCellGroups[groupIndex];
     }
 
     return null;
   }
 
   /**
-   * Get the metadata for a column in the data model.
+   * Get the metadata for a cell in the data model.
    *
    * @param region - The cell region of interest.
    *
+   * @param row - The index of the row of interest.
+   *
    * @param column - The index of the column of interest.
    *
-   * @returns The metadata for the column.
+   * @returns The metadata for the cell.
    */
   metadata(
     region: DataModel.CellRegion,
     row: number,
     column: number,
   ): DataModel.Metadata {
     const md = this.currentView.metadata(region, row, column);
     if (region == 'body') {
       md.row = row;
       md.column = column;
-      md.data = (row: number, column: number) => {
+      md.data = (row: number, column: string) => {
         const columnIndex = this.columnNameToIndex(column.toString());
         return this.data('body', row, columnIndex);
       };
     }
     return md;
   }
 
@@ -311,18 +311,15 @@
    * Updates the row value of the currently displayed View.
    *
    * @param row - The row index of the cell of interest.
    *
    * @param value - The new value to update the indicated row with.
    *
    */
-  setRowData(
-    row: number,
-    value: any,
-  ): boolean {
+  setRowData(row: number, value: any): boolean {
     this.updateRowValue({
       row: row,
       value: value,
     });
     this.emitChanged({
       type: 'cells-changed',
       region: 'body',
@@ -385,26 +382,31 @@
   }
 
   /**
    * Sets the provided View as the current View, then emits a changed signal.
    */
   protected set currentView(view: View) {
     this._currentView = view;
+
     this.emitChanged({ type: 'model-reset' });
 
     const primaryKey = !Array.isArray(this._dataset.schema.primaryKey)
       ? [this._dataset.schema.primaryKey]
       : this._dataset.schema.primaryKey;
 
-    const indices: number[] = view.dataset.map((val, i) => {
-      const lookupVal = JSON.stringify(primaryKey.map((key) => val[key]));
+    const indices: number[] = [];
+
+    for (let idx = 0; idx < view.dataset.length; idx++) {
+      const lookupVal = JSON.stringify(
+        primaryKey.map((key) => view.dataset.data[key][idx]),
+      );
       const retrievedVal = this._primaryKeyMap.get(lookupVal);
 
-      return typeof retrievedVal === 'undefined' ? i : retrievedVal;
-    });
+      indices.push(typeof retrievedVal === 'undefined' ? idx : retrievedVal);
+    }
 
     this.dataSync.emit({
       type: 'row-indices-updated',
       indices: indices,
     });
   }
 
@@ -459,26 +461,17 @@
   /**
    * Returns a Promise that resolves to an array of unique values contained in
    * the provided column index.
    *
    * @param region - The CellRegion to retrieve unique values for.
    * @param columnIndex - The index to retrieve unique values for.
    */
-  async uniqueValues(
-    region: DataModel.CellRegion,
-    columnIndex: number,
-  ): Promise<any[]> {
-    return new Promise((resolve, reject) => {
-      const columnName = this.metadata(region, 0, columnIndex)['name'];
-      const uniqueVals = new Set();
-      for (const row of this.dataset.data) {
-        uniqueVals.add(row[columnName]);
-      }
-      resolve(Array.from(uniqueVals));
-    });
+  uniqueValues(region: DataModel.CellRegion, columnIndex: number): any[] {
+    const columnName = this.metadata(region, 0, columnIndex)['name'];
+    return Array.from(new Set(this.dataset.data[columnName]));
   }
 
   /**
    * Returns a Promise that resolves to an array of unique values contained in
    * the provided column index after all transforms have been applied.
    *
    * @param region - The CellRegion to retrieve unique values for.
@@ -521,15 +514,15 @@
     }
     // Get the index of the row in the full dataset to be updated
     const primaryKey = Array.isArray(this._dataset.schema.primaryKey)
       ? this._dataset.schema.primaryKey
       : [this._dataset.schema.primaryKey];
 
     const keyValues = primaryKey.map(
-      (key) => this._currentView.dataset[row][key],
+      (key) => this._currentView.dataset.data[key][row],
     );
 
     const lookupIndex: number = this._primaryKeyMap.get(
       JSON.stringify(keyValues),
     )!;
 
     return lookupIndex;
@@ -542,71 +535,42 @@
    */
   updateCellValue(options: ViewBasedJSONModel.IUpdateCellValuesOptions): void {
     // Bail if cell region isn't the body
     // TODO: Support modifying the schema
     if (options.region !== 'body') {
       return;
     }
-
-    // Create new row and add it to new dataset
-    const newRow = { ...this._dataset.data[options.row] };
-    newRow[this.metadata('body', 0, options.column)['name']] = options.value;
-    const newData = Array.from(this._dataset.data);
-    newData[options.row] = newRow;
-
-    this._dataset = {
-      data: newData,
-      schema: this._dataset.schema,
-    };
-
-    if (options.syncData) {
-      this.dataSync.emit({
-        type: 'cell-updated',
-      });
-    }
+    const columnName = this.metadata('body', 0, options.column)['name'];
+    this._dataset.data[columnName][options.row] = options.value;
 
     // Notify listeners of the cell change event
     this.dataSync.emit({
       type: 'cell-edit-event',
+      column: columnName,
       columnIndex: options.column,
       row: options.row,
       region: options.region,
       value: options.value,
     });
-
     // We need to rerun the transforms, as the changed cell may change the order
     // or visibility of other rows
     this.currentView = this._transformState.createView(this._dataset);
   }
 
   /**
    * Updates a row in the full dataset of the model.
    *
    * @param options - The options for this function.
    */
   updateRowValue(options: ViewBasedJSONModel.IUpdateRowValuesOptions): void {
     // Create new row and add it to new dataset
-    const newRow = { ...this._dataset.data[options.row] };
     for (const columnIndex of Array(options.value.length).keys()) {
-      newRow[this.metadata('body', 0, columnIndex)['name']] = options.value[columnIndex];
+      const columnName = this.metadata('body', 0, columnIndex)['name'];
+      this._dataset.data[columnName][options.row] = options.value[columnIndex];
     }
-    const newData = Array.from(this._dataset.data);
-    newData[options.row] = newRow;
-
-    this._dataset = {
-      data: newData,
-      schema: this._dataset.schema,
-    };
-
-    if (options.syncData) {
-      this.dataSync.emit({
-        type: 'cell-updated',
-      });
-    }
-
     // We need to rerun the transforms, as the changed cells may change the order
     // or visibility of other rows
     this.currentView = this._transformState.createView(this._dataset);
   }
 
   /**
    * A signal emitted when the data model has changes to sync to the kernel.
@@ -614,131 +578,50 @@
   get dataSync(): Signal<this, ViewBasedJSONModel.IDataSyncEvent> {
     return this._dataSyncSignal;
   }
 
   /**
    * Returns the current full dataset.
    */
-  get dataset(): ViewBasedJSONModel.IData {
+  get dataset(): DataSource {
     return this._dataset;
   }
 
   /**
    * Returns the index in the schema that relates to the index by region.
    *
    * @param region - The `CellRegion` of interest.
    *
    * @param index - The column index to look up.
    */
   getSchemaIndex(region: DataModel.CellRegion, index: number): number {
     return this.currentView.getSchemaIndex(region, index);
   }
 
-  /**
-   * Deep copies data object and mutates it before
-   * returning a ViewBasedJSONModel of the data.
-   * ts-ignores are added since the properties to be mutated
-   * are readonly
-   *
-   * @param data - Data passed in to be transformed
-   *
-   */
-  static fromJsonData(data: ViewBasedJSONModel.IData): ViewBasedJSONModel {
-    const primaryKeyUuid = 'ipydguuid';
-
-    const newData = <ViewBasedJSONModel.IData>(
-      (<unknown>JSONExt.deepCopy(<ReadonlyJSONObject>(<unknown>data)))
-    );
-
-    //@ts-ignore
-    newData.schema.primaryKeyUuid = primaryKeyUuid;
-
-    for (const field of newData.schema.fields) {
-      //@ts-ignore
-      field.rows = [field.name];
-    }
-    let count = 0;
-    for (const row of newData.data) {
-      //@ts-ignore
-      row[primaryKeyUuid] = count++;
-    }
-
-    return new ViewBasedJSONModel(newData);
-  }
-
   private _currentView: View;
   private _transformSignal = new Signal<this, TransformStateManager.IEvent>(
     this,
   );
   private _dataSyncSignal = new Signal<this, ViewBasedJSONModel.IDataSyncEvent>(
     this,
   );
   private _primaryKeyMap: Map<ReadonlyJSONValue, number> = new Map();
 
-  protected _dataset: ViewBasedJSONModel.IData;
+  protected _dataset: DataSource;
   protected readonly _transformState: TransformStateManager;
   private _mergedColumnCellLocations: any[];
+  private _mergedRowCellLocations: any[];
   private _rowCellGroups: CellGroup[];
   private _columnCellGroups: CellGroup[];
 }
 
 /**
  * The namespace for the `ViewBasedJSONModel` class statics.
  */
 export namespace ViewBasedJSONModel {
-  /**
-   * An object which describes a column of data in the model.
-   *
-   * #### Notes
-   * This is based on the JSON Table Schema specification:
-   * https://specs.frictionlessdata.io/table-schema/
-   */
-  export interface IField {
-    /**
-     * The name of the column.
-     *
-     * This is used as the key to extract a value from a data record.
-     */
-    readonly name: string;
-
-    /**
-     * The type of data held in the column.
-     */
-    readonly type: string;
-
-    /**
-     * An array of the column labels per header row.
-     */
-    readonly rows: any[];
-  }
-
-  /**
-   * An object when specifies the schema for a data model.
-   *
-   * #### Notes
-   * This is based on the JSON Table Schema specification:
-   * https://specs.frictionlessdata.io/table-schema/
-   */
-  export interface ISchema {
-    /**
-     * The fields which describe the data model columns.
-     *
-     * Primary key fields are rendered as row header columns.
-     */
-    readonly fields: IField[];
-
-    /**
-     * The field names which act as primary keys.
-     *
-     * Primary key fields are rendered as row header columns.
-     */
-    readonly primaryKey: string[];
-    readonly primaryKeyUuid: string;
-  }
-
   export interface IUpdateCellValuesOptions {
     /**
      * The `CellRegion` of the cell to be updated.
      */
     region: DataModel.CellRegion;
 
     /**
@@ -751,76 +634,30 @@
      */
     row: number;
 
     /**
      * The new value to replace the old one.
      */
     value: any;
-
-    /**
-     * The flag to trigger full data sync with backend.
-     */
-    syncData?: boolean;
   }
 
   export interface IUpdateRowValuesOptions {
     /**
      * The index of the target row in the current view.
      */
     row: number;
 
     /**
      * The new value to replace the old one.
      */
     value: any[];
-
-    /**
-     * The flag to trigger full data sync with backend.
-     */
-    syncData?: boolean;
   }
 
-  /**
-   * A type alias for a data source for a JSON data model.
-   *
-   * A data source is an array of JSON object records which represent
-   * the rows of the table. The keys of the records correspond to the
-   * field names of the columns.
-   */
-  export type DataSource = ReadonlyArray<ReadonlyJSONObject>;
-
-  /**
-   * An options object for initializing the data model.
-   */
-  export interface IData {
-    /**
-     * The schema for the for the data model.
-     *
-     * The schema should be treated as an immutable object.
-     */
-    schema: ISchema;
-
-    /**
-     * The data source for the data model.
-     *
-     * The data model takes full ownership of the data source.
-     */
-    data: DataSource;
-  }
-  export type IDataSyncEvent = ISyncCell | ISyncRowIndices | ICellEditEvent;
+  export type IDataSyncEvent = ISyncRowIndices | ICellEditEvent;
 
-  /**
-   * An event that indicates a needed change to the kernel-side dataset.
-   */
-  export interface ISyncCell {
-    /**
-     * The discriminated type of the args object.
-     */
-    type: 'cell-updated';
-  }
   export interface ISyncRowIndices {
     /**
      * The discriminated type of the args object.
      */
     type: 'row-indices-updated';
 
     /**
@@ -843,14 +680,20 @@
 
     /**
      * The row number associated with this change.
      */
     row: number;
 
     /**
+     * The column name associated with this change.
+     */
+    column: string;
+
+    /**
+     * TODO Deprecate this
      * The column index associated with this change.
      */
     columnIndex: number;
 
     /**
      * The new data value
      */
```

### Comparing `ipydatagrid-1.2.1/static/ipydatagrid_1.gif` & `ipydatagrid-1.3.0/static/ipydatagrid_1.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/static/ipydatagrid_2.gif` & `ipydatagrid-1.3.0/static/ipydatagrid_2.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/static/ipydatagrid_3.gif` & `ipydatagrid-1.3.0/static/ipydatagrid_3.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/static/ipydatagrid_4.gif` & `ipydatagrid-1.3.0/static/ipydatagrid_4.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/static/ipydatagrid_5.gif` & `ipydatagrid-1.3.0/static/ipydatagrid_5.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/style/feathergrid.css` & `ipydatagrid-1.3.0/style/feathergrid.css`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/.gitignore` & `ipydatagrid-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/LICENSE.txt` & `ipydatagrid-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.2.1/README.md` & `ipydatagrid-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,24 @@
 Enabling development install for JupyterLab:
 
 ```bash
 jupyter labextension develop . --overwrite
 ```
 
 Note for developers: the `--symlink` argument on Linux or OS X allows one to modify the JavaScript code in-place. This feature is not available with Windows.
-`
+
+If you are changing TypeScript code you can watch for code changes and automatically rebuild using
+```bash
+jlpm watch
+```
+in one terminal and
+```bash
+jupyter lab
+```
+(or `jupyter notebook` or similar) in another.
 
 ## Contributions
 
 We :heart: contributions.
 
 Have you had a good experience with this project? Why not share some love and contribute code, or just let us know about any issues you had with it?
```

### Comparing `ipydatagrid-1.2.1/pyproject.toml` & `ipydatagrid-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 requires = [
   "hatchling>=1.18",
   "jupyterlab>=4.0.5",
 ]
 
 [project]
 name = "ipydatagrid"
-version = "1.2.1"
+version = "1.3.0"
 description = "Fast Datagrid widget for the Jupyter Notebook and JupyterLab"
 readme = "README.md"
 keywords = [
   "IPython",
   "Jupyter",
   "Widgets",
 ]
 authors = [
     { name = "Bloomberg" },
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
   "Framework :: Jupyter",
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "bqplot>=0.11.6",
   "ipywidgets<9,>=7.6",
-  "pandas>=1.3.5", # 1.3.5 is the last version supporting 3.7
+  "pandas>=1.3.5",
   "py2vega>=0.5",
 ]
 optional-dependencies.test = [
   "nbval>=0.10",
   "pytest>=7.4",
   "pytest-cov>=4.1",
 ]
@@ -104,22 +104,26 @@
 
 [tool.pylint.messages_control]
 disable = "C0330, C0326"
 
 [tool.pylint.format]
 max-line-length = "80"
 
+[tool.codespell]
+ignore-words-list = "statics"
+skip = "*/yarn.lock"
+
 [tool.tbump]
 field = [
     { name = "channel", default = "" },
     { name = "release", default = "" },
 ]
 
 [tool.tbump.version]
-current = "1.2.1"
+current = "1.3.0"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
```

### Comparing `ipydatagrid-1.2.1/PKG-INFO` & `ipydatagrid-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ipydatagrid
-Version: 1.2.1
+Version: 1.3.0
 Summary: Fast Datagrid widget for the Jupyter Notebook and JupyterLab
 Project-URL: Homepage, https://github.com/bloomberg/ipydatagrid
 Author: Bloomberg
 License-File: LICENSE.txt
 Keywords: IPython,Jupyter,Widgets
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Requires-Dist: bqplot>=0.11.6
 Requires-Dist: ipywidgets<9,>=7.6
 Requires-Dist: pandas>=1.3.5
 Requires-Dist: py2vega>=0.5
 Provides-Extra: test
 Requires-Dist: nbval>=0.10; extra == 'test'
 Requires-Dist: pytest-cov>=4.1; extra == 'test'
@@ -115,15 +115,24 @@
 Enabling development install for JupyterLab:
 
 ```bash
 jupyter labextension develop . --overwrite
 ```
 
 Note for developers: the `--symlink` argument on Linux or OS X allows one to modify the JavaScript code in-place. This feature is not available with Windows.
-`
+
+If you are changing TypeScript code you can watch for code changes and automatically rebuild using
+```bash
+jlpm watch
+```
+in one terminal and
+```bash
+jupyter lab
+```
+(or `jupyter notebook` or similar) in another.
 
 ## Contributions
 
 We :heart: contributions.
 
 Have you had a good experience with this project? Why not share some love and contribute code, or just let us know about any issues you had with it?
```

