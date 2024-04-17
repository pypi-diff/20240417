# Comparing `tmp/pypots-0.4.tar.gz` & `tmp/pypots-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypots-0.4.tar", last modified: Tue Apr  9 13:48:49 2024, max compression
+gzip compressed data, was "pypots-0.4.1.tar", last modified: Wed Apr 17 16:06:57 2024, max compression
```

## Comparing `pypots-0.4.tar` & `pypots-0.4.1.tar`

### file list

```diff
@@ -1,271 +1,282 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 13:46:55.000000 pypots-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 13:46:55.000000 pypots-0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27890 2024-04-09 13:48:49.892830 pypots-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26077 2024-04-09 13:46:55.000000 pypots-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-09 13:46:55.000000 pypots-0.4/pypots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22426 2024-04-09 13:46:55.000000 pypots-0.4/pypots/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/brits/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/brits/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/grud/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/grud/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/grud/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/raindrop/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots/classification/raindrop/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-04-09 13:46:55.000000 pypots-0.4/pypots/classification/raindrop/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/pypots_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 13:46:55.000000 pypots-0.4/pypots/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/crli/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/crli/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9460 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/crli/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/vader/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.868830 pypots-0.4/pypots/clustering/vader/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-09 13:46:55.000000 pypots-0.4/pypots/clustering/vader/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/data/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/checking.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/generating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/load_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/load_specific_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/data/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/saving/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/saving/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-09 13:46:55.000000 pypots-0.4/pypots/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/forecasting/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/forecasting/bttf/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/forecasting/bttf/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-09 13:46:55.000000 pypots-0.4/pypots/forecasting/bttf/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/imputation/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/imputation/autoformer/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/imputation/autoformer/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/autoformer/modules/submodules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.872830 pypots-0.4/pypots/imputation/brits/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/brits/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/brits/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/crossformer/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/crossformer/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/crossformer/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/csdi/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17279 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/csdi/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/csdi/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/dlinear/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/dlinear/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/dlinear/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/etsformer/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.876830 pypots-0.4/pypots/imputation/etsformer/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/etsformer/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/fedformer/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/fedformer/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/fedformer/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/gpvae/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18007 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/gpvae/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/gpvae/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/informer/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/informer/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/informer/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/locf/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/locf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/locf/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/locf/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/locf/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/locf/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/mean/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mean/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.880830 pypots-0.4/pypots/imputation/median/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/median/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/median/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/mrnn/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/mrnn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/mrnn/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/patchtst/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/patchtst/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/patchtst/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/saits/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/saits/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/saits/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/timesnet/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/timesnet/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/timesnet/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.884830 pypots-0.4/pypots/imputation/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/imputation/transformer/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/transformer/modules/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/imputation/usgan/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17811 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/imputation/usgan/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/modules/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-09 13:46:55.000000 pypots-0.4/pypots/imputation/usgan/modules/submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/functional/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/rnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/nn/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-09 13:46:55.000000 pypots-0.4/pypots/nn/modules/transformer/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.888830 pypots-0.4/pypots/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/pypots/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/constant_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/exponential_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/lambda_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/linear_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/multiplicative_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/multistep_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/lr_scheduler/step_lrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-09 13:46:55.000000 pypots-0.4/pypots/optim/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/pypots/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/pypots/utils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/metrics/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/metrics/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.892830 pypots-0.4/pypots/utils/visual/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/visual/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-09 13:46:55.000000 pypots-0.4/pypots/utils/visual/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:48:49.864830 pypots-0.4/pypots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27890 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 13:48:49.000000 pypots-0.4/pypots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 13:48:49.892830 pypots-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-09 13:46:55.000000 pypots-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.847941 pypots-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-17 16:04:57.000000 pypots-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 16:04:57.000000 pypots-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27877 2024-04-17 16:06:57.847941 pypots-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26062 2024-04-17 16:04:57.000000 pypots-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22426 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/classification/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/brits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/brits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/classification/grud/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/grud/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/grud/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/grud/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots/classification/raindrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/raindrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/raindrop/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/raindrop/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/classification/raindrop/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7915 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/pypots_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/clustering/crli/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/crli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/crli/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/crli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18627 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/crli/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/clustering/vader/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/vader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/vader/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/vader/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/clustering/vader/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/generating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/load_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/load_specific_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.819940 pypots-0.4.1/pypots/data/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/saving/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/saving/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/forecasting/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/forecasting/bttf/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/bttf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/bttf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/bttf/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/forecasting/bttf/submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/autoformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/autoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/autoformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/autoformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/autoformer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/brits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/brits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/crossformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/crossformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/crossformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/crossformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/crossformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.823940 pypots-0.4.1/pypots/imputation/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/csdi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/csdi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/csdi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/dlinear/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/dlinear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/dlinear/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/dlinear/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/dlinear/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/etsformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/etsformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/etsformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/etsformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11171 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/etsformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/fedformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/fedformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/fedformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/fedformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/fedformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/gpvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/gpvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/gpvae/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/gpvae/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18004 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/gpvae/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/informer/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/informer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/informer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/informer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/locf/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/locf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/locf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/locf/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mean/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.827940 pypots-0.4.1/pypots/imputation/median/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/median/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/median/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/mrnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mrnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mrnn/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mrnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/mrnn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/patchtst/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/patchtst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/patchtst/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/patchtst/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/patchtst/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/saits/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/saits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/saits/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/saits/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14631 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/saits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/timesnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/timesnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/timesnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/timesnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11290 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/timesnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/transformer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/transformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/transformer/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/imputation/usgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/usgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/usgan/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/usgan/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17737 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/imputation/usgan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.831941 pypots-0.4.1/pypots/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/functional/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/autoformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/autoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/autoformer/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/autoformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/brits/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/brits/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/brits/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/crli/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crli/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crli/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/crossformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crossformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crossformer/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/crossformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/csdi/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/csdi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/csdi/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/csdi/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/dlinear/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/dlinear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/dlinear/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/etsformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/etsformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/etsformer/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/etsformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.835940 pypots-0.4.1/pypots/nn/modules/fedformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/fedformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/fedformer/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/fedformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/gpvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/gpvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/gpvae/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/gpvae/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/grud/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/grud/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/grud/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/informer/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/informer/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/informer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/mrnn/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/mrnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/mrnn/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/mrnn/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/patchtst/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/patchtst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/patchtst/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/patchtst/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/raindrop/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/raindrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/raindrop/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/raindrop/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/saits/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/saits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/saits/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/saits/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.839940 pypots-0.4.1/pypots/nn/modules/timesnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/timesnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/timesnet/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/timesnet/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/nn/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/transformer/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/nn/modules/usgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/usgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/usgan/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/usgan/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/nn/modules/vader/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/vader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/vader/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/nn/modules/vader/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.843941 pypots-0.4.1/pypots/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/constant_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/exponential_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/lambda_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/linear_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/multiplicative_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/multistep_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/lr_scheduler/step_lrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/optim/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.847941 pypots-0.4.1/pypots/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.847941 pypots-0.4.1/pypots/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/metrics/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13674 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/metrics/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.847941 pypots-0.4.1/pypots/utils/visual/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/visual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/visual/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-17 16:04:57.000000 pypots-0.4.1/pypots/utils/visual/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:06:57.815940 pypots-0.4.1/pypots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27877 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 16:06:57.000000 pypots-0.4.1/pypots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-17 16:06:57.847941 pypots-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-17 16:04:57.000000 pypots-0.4.1/setup.py
```

### Comparing `pypots-0.4/LICENSE` & `pypots-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypots-0.4/PKG-INFO` & `pypots-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.4
+Version: 0.4.1
 Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
 Home-page: https://pypots.com/
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/
 Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
@@ -221,21 +221,22 @@
 ```
 </details>
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
 The currently available algorithms of four tasks are cataloged in the following table with four partitions.
-The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
+The paper references are all listed at the bottom of this readme file.
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
 
 🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
-and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
+the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
 
 |   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
 |:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
 |        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
 |       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
 |       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
 |       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.4 Summary: A Python Toolbox for
+Metadata-Version: 2.1 Name: pypots Version: 0.4.1 Summary: A Python Toolbox for
 Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
 Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
 https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
 WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
 PyPOTS/archive/main.zip Keywords: data science,data mining,neural
 networks,machine learning,deep learning,artificial intelligence,time-series
@@ -115,61 +115,61 @@
 values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
 imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
 indicating_mask) # calculate mean absolute error on the ground truth
 (artificially-missing values) ``` ## â Available Algorithms PyPOTS supports
 imputation, classification, clustering, and forecasting tasks on multivariate
 time series with missing values. The currently available algorithms of four
 tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. Please refer to
-them if you want more details. ð Since **v0.2**, all neural-network models
-in PyPOTS has got hyperparameter-optimization support. This functionality is
-implemented with the [Microsoft NNI](https://github.com/microsoft/nni)
-framework. ð¥ Note that Transformer, Crossformer, PatchTST, DLinear,
-ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation
-methods in their original papers, and they cannot accept POTS as input. **To
-make them applicable on POTS data, we apply the embedding strategy the same as
-we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).** |
-***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:----------------------:|:----------
--:|:---------------------------------------------------------------------------
---------------------:|:--------:| | **Type** | **Abbr.** | **Full name of the
-algorithm/model** | **Year** | | Neural Net | SAITS | Self-Attention-based
-Imputation for Time Series [^1] | 2023 | | Neural Net | Transformer | Attention
-is All you Need [^2] | 2017 | | Neural Net | Crossformer | Transformer
-Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting
-[^16] | 2023 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for
-General Time Series Analysis [^14] | 2023 | | Neural Net | PatchTST | A Time
-Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18] | 2023
-| | Neural Net | DLinear | Are Transformers Effective for Time Series
-Forecasting? [^17] | 2023 | | Neural Net | ETSformer | Exponential Smoothing
-Transformers for Time-series Forecasting [^19] | 2023 | | Neural Net |
-FEDformer | Frequency Enhanced Decomposed Transformer for Long-term Series
-Forecasting [^20] | 2022 | | Neural Net | Informer | Beyond Efficient
-Transformer for Long Sequence Time-Series Forecasting [^21] | 2021 | | Neural
-Net | Autoformer | Decomposition Transformers with Auto-Correlation for Long-
-Term Series Forecasting [^15] | 2021 | | Neural Net | CSDI | Conditional Score-
-based Diffusion Models for Probabilistic Time Series Imputation [^12] | 2021 |
-| Neural Net | US-GAN | Unsupervised GAN for Multivariate Time Series
-Imputation [^10] | 2021 | | Neural Net | GP-VAE | Gaussian Process Variational
-Autoencoder [^11] | 2020 | | Neural Net | BRITS | Bidirectional Recurrent
-Imputation for Time Series [^3] | 2018 | | Neural Net | M-RNN | Multi-
-directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF/NOCB | Last
-Observation Carried Forward / Next Observation Carried Backward | - | | Naive |
-Median | Median Value Imputation | - | | Naive | Mean | Mean Value Imputation |
-- | | ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** |
-**Full name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
-Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
-GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
-Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
-Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
-| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Neural Net | CRLI | Clustering Representation
-Learning on Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER |
-Variational Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`***
-| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
+references are all listed at the bottom of this readme file. ð Since
+**v0.2**, all neural-network models in PyPOTS has got hyperparameter-
+optimization support. This functionality is implemented with the [Microsoft
+NNI](https://github.com/microsoft/nni) framework. ð¥ Note that Transformer,
+Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are
+not proposed as imputation methods in their original papers, and they cannot
+accept POTS as input. **To make them applicable on POTS data, we apply the
+embedding strategy and training approach (ORT+MIT) the same as we did in [SAITS
+paper](https://arxiv.org/pdf/2202.08516).** | ***`Imputation`*** | ð¥ | ð¥
+| ð¥ | |:----------------------:|:-----------:|:-----------------------------
+------------------------------------------------------------------:|:--------:
+| | **Type** | **Abbr.** | **Full name of the algorithm/model** | **Year** | |
+Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
+2023 | | Neural Net | Transformer | Attention is All you Need [^2] | 2017 | |
+Neural Net | Crossformer | Transformer Utilizing Cross-Dimension Dependency for
+Multivariate Time Series Forecasting [^16] | 2023 | | Neural Net | TimesNet |
+Temporal 2D-Variation Modeling for General Time Series Analysis [^14] | 2023 |
+| Neural Net | PatchTST | A Time Series is Worth 64 Words: Long-Term
+Forecasting with Transformers [^18] | 2023 | | Neural Net | DLinear | Are
+Transformers Effective for Time Series Forecasting? [^17] | 2023 | | Neural Net
+| ETSformer | Exponential Smoothing Transformers for Time-series Forecasting
+[^19] | 2023 | | Neural Net | FEDformer | Frequency Enhanced Decomposed
+Transformer for Long-term Series Forecasting [^20] | 2022 | | Neural Net |
+Informer | Beyond Efficient Transformer for Long Sequence Time-Series
+Forecasting [^21] | 2021 | | Neural Net | Autoformer | Decomposition
+Transformers with Auto-Correlation for Long-Term Series Forecasting [^15] |
+2021 | | Neural Net | CSDI | Conditional Score-based Diffusion Models for
+Probabilistic Time Series Imputation [^12] | 2021 | | Neural Net | US-GAN |
+Unsupervised GAN for Multivariate Time Series Imputation [^10] | 2021 | |
+Neural Net | GP-VAE | Gaussian Process Variational Autoencoder [^11] | 2020 | |
+Neural Net | BRITS | Bidirectional Recurrent Imputation for Time Series [^3] |
+2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural Network [^9] |
+2019 | | Naive | LOCF/NOCB | Last Observation Carried Forward / Next
+Observation Carried Backward | - | | Naive | Median | Median Value Imputation |
+- | | Naive | Mean | Mean Value Imputation | - | | ***`Classification`*** |
+ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Neural Net | BRITS | Bidirectional Recurrent
+Imputation for Time Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent
+Neural Networks for Multivariate Time Series with Missing Values [^4] | 2018 |
+| Neural Net | Raindrop | Graph-Guided Network for Irregularly Sampled
+Multivariate Time Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ |
+ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
+**Year** | | Neural Net | CRLI | Clustering Representation Learning on
+Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER | Variational
+Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`*** | ð¥ |
+ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/
+paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
 Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
 2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
 Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
 arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
 github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
 literature of the state-of-the-art deep-learning imputation methods for time
 series, provide a taxonomy for them, and discuss the challenges and future
```

### Comparing `pypots-0.4/README.md` & `pypots-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -183,21 +183,22 @@
 ```
 </details>
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
 The currently available algorithms of four tasks are cataloged in the following table with four partitions.
-The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
+The paper references are all listed at the bottom of this readme file.
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
 
 🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
-and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
+the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
 
 |   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
 |:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
 |        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
 |       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
 |       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
 |       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
```

#### html2text {}

```diff
@@ -90,61 +90,61 @@
 values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
 imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
 indicating_mask) # calculate mean absolute error on the ground truth
 (artificially-missing values) ``` ## â Available Algorithms PyPOTS supports
 imputation, classification, clustering, and forecasting tasks on multivariate
 time series with missing values. The currently available algorithms of four
 tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. Please refer to
-them if you want more details. ð Since **v0.2**, all neural-network models
-in PyPOTS has got hyperparameter-optimization support. This functionality is
-implemented with the [Microsoft NNI](https://github.com/microsoft/nni)
-framework. ð¥ Note that Transformer, Crossformer, PatchTST, DLinear,
-ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation
-methods in their original papers, and they cannot accept POTS as input. **To
-make them applicable on POTS data, we apply the embedding strategy the same as
-we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).** |
-***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:----------------------:|:----------
--:|:---------------------------------------------------------------------------
---------------------:|:--------:| | **Type** | **Abbr.** | **Full name of the
-algorithm/model** | **Year** | | Neural Net | SAITS | Self-Attention-based
-Imputation for Time Series [^1] | 2023 | | Neural Net | Transformer | Attention
-is All you Need [^2] | 2017 | | Neural Net | Crossformer | Transformer
-Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting
-[^16] | 2023 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for
-General Time Series Analysis [^14] | 2023 | | Neural Net | PatchTST | A Time
-Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18] | 2023
-| | Neural Net | DLinear | Are Transformers Effective for Time Series
-Forecasting? [^17] | 2023 | | Neural Net | ETSformer | Exponential Smoothing
-Transformers for Time-series Forecasting [^19] | 2023 | | Neural Net |
-FEDformer | Frequency Enhanced Decomposed Transformer for Long-term Series
-Forecasting [^20] | 2022 | | Neural Net | Informer | Beyond Efficient
-Transformer for Long Sequence Time-Series Forecasting [^21] | 2021 | | Neural
-Net | Autoformer | Decomposition Transformers with Auto-Correlation for Long-
-Term Series Forecasting [^15] | 2021 | | Neural Net | CSDI | Conditional Score-
-based Diffusion Models for Probabilistic Time Series Imputation [^12] | 2021 |
-| Neural Net | US-GAN | Unsupervised GAN for Multivariate Time Series
-Imputation [^10] | 2021 | | Neural Net | GP-VAE | Gaussian Process Variational
-Autoencoder [^11] | 2020 | | Neural Net | BRITS | Bidirectional Recurrent
-Imputation for Time Series [^3] | 2018 | | Neural Net | M-RNN | Multi-
-directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF/NOCB | Last
-Observation Carried Forward / Next Observation Carried Backward | - | | Naive |
-Median | Median Value Imputation | - | | Naive | Mean | Mean Value Imputation |
-- | | ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** |
-**Full name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
-Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
-GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
-Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
-Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
-| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Neural Net | CRLI | Clustering Representation
-Learning on Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER |
-Variational Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`***
-| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
+references are all listed at the bottom of this readme file. ð Since
+**v0.2**, all neural-network models in PyPOTS has got hyperparameter-
+optimization support. This functionality is implemented with the [Microsoft
+NNI](https://github.com/microsoft/nni) framework. ð¥ Note that Transformer,
+Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are
+not proposed as imputation methods in their original papers, and they cannot
+accept POTS as input. **To make them applicable on POTS data, we apply the
+embedding strategy and training approach (ORT+MIT) the same as we did in [SAITS
+paper](https://arxiv.org/pdf/2202.08516).** | ***`Imputation`*** | ð¥ | ð¥
+| ð¥ | |:----------------------:|:-----------:|:-----------------------------
+------------------------------------------------------------------:|:--------:
+| | **Type** | **Abbr.** | **Full name of the algorithm/model** | **Year** | |
+Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
+2023 | | Neural Net | Transformer | Attention is All you Need [^2] | 2017 | |
+Neural Net | Crossformer | Transformer Utilizing Cross-Dimension Dependency for
+Multivariate Time Series Forecasting [^16] | 2023 | | Neural Net | TimesNet |
+Temporal 2D-Variation Modeling for General Time Series Analysis [^14] | 2023 |
+| Neural Net | PatchTST | A Time Series is Worth 64 Words: Long-Term
+Forecasting with Transformers [^18] | 2023 | | Neural Net | DLinear | Are
+Transformers Effective for Time Series Forecasting? [^17] | 2023 | | Neural Net
+| ETSformer | Exponential Smoothing Transformers for Time-series Forecasting
+[^19] | 2023 | | Neural Net | FEDformer | Frequency Enhanced Decomposed
+Transformer for Long-term Series Forecasting [^20] | 2022 | | Neural Net |
+Informer | Beyond Efficient Transformer for Long Sequence Time-Series
+Forecasting [^21] | 2021 | | Neural Net | Autoformer | Decomposition
+Transformers with Auto-Correlation for Long-Term Series Forecasting [^15] |
+2021 | | Neural Net | CSDI | Conditional Score-based Diffusion Models for
+Probabilistic Time Series Imputation [^12] | 2021 | | Neural Net | US-GAN |
+Unsupervised GAN for Multivariate Time Series Imputation [^10] | 2021 | |
+Neural Net | GP-VAE | Gaussian Process Variational Autoencoder [^11] | 2020 | |
+Neural Net | BRITS | Bidirectional Recurrent Imputation for Time Series [^3] |
+2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural Network [^9] |
+2019 | | Naive | LOCF/NOCB | Last Observation Carried Forward / Next
+Observation Carried Backward | - | | Naive | Median | Median Value Imputation |
+- | | Naive | Mean | Mean Value Imputation | - | | ***`Classification`*** |
+ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Neural Net | BRITS | Bidirectional Recurrent
+Imputation for Time Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent
+Neural Networks for Multivariate Time Series with Missing Values [^4] | 2018 |
+| Neural Net | Raindrop | Graph-Guided Network for Irregularly Sampled
+Multivariate Time Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ |
+ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
+**Year** | | Neural Net | CRLI | Clustering Representation Learning on
+Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER | Variational
+Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`*** | ð¥ |
+ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/
+paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
 Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
 2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
 Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
 arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
 github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
 literature of the state-of-the-art deep-learning imputation methods for time
 series, provide a taxonomy for them, and discuss the challenges and future
```

### Comparing `pypots-0.4/pypots/__init__.py` & `pypots-0.4.1/pypots/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # X.YaN # Alpha release
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-__version__ = "0.4"
+__version__ = "0.4.1"
 
 
 from . import imputation, classification, clustering, forecasting, optim, data, utils
 
 __all__ = [
     "imputation",
     "classification",
```

### Comparing `pypots-0.4/pypots/base.py` & `pypots-0.4.1/pypots/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/classification/base.py` & `pypots-0.4.1/pypots/classification/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/classification/brits/__init__.py` & `pypots-0.4.1/pypots/classification/brits/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/classification/brits/data.py` & `pypots-0.4.1/pypots/classification/brits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/classification/brits/model.py` & `pypots-0.4.1/pypots/classification/brits/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 from typing import Optional, Union
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _BRITS
 from .data import DatasetForBRITS
-from .modules import _BRITS
 from ..base import BaseNNClassifier
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
 class BRITS(BaseNNClassifier):
@@ -131,15 +131,14 @@
         self.model = _BRITS(
             self.n_steps,
             self.n_features,
             self.rnn_hidden_size,
             self.n_classes,
             self.classification_weight,
             self.reconstruction_weight,
-            self.device,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/classification/brits/modules/core.py` & `pypots-0.4.1/pypots/classification/brits/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,115 +10,80 @@
 are fixed here.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from typing import Union
-
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from ....imputation.brits.modules.core import RITS as imputation_RITS
-from ....imputation.brits.modules.core import _BRITS as imputation_BRITS
+from ...nn.modules.brits import BackboneBRITS
 
 
-class RITS(imputation_RITS):
-    def __init__(
-        self,
-        n_steps: int,
-        n_features: int,
-        rnn_hidden_size: int,
-        n_classes: int,
-        device: Union[str, torch.device],
-    ):
-        super().__init__(n_steps, n_features, rnn_hidden_size, device)
-        self.dropout = nn.Dropout(p=0.25)
-        self.classifier = nn.Linear(self.rnn_hidden_size, n_classes)
-
-    def forward(self, inputs: dict, direction: str = "forward") -> dict:
-        ret_dict = super().forward(inputs, direction)
-        logits = self.classifier(ret_dict["final_hidden_state"])
-        ret_dict["prediction"] = torch.softmax(logits, dim=1)
-        return ret_dict
-
-
-class _BRITS(imputation_BRITS, nn.Module):
+class _BRITS(nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         rnn_hidden_size: int,
         n_classes: int,
         classification_weight: float,
         reconstruction_weight: float,
-        device: Union[str, torch.device],
     ):
-        super().__init__(n_steps, n_features, rnn_hidden_size, device)
+        super().__init__()
         self.n_steps = n_steps
         self.n_features = n_features
         self.rnn_hidden_size = rnn_hidden_size
         self.n_classes = n_classes
-
-        # create models
-        self.rits_f = RITS(n_steps, n_features, rnn_hidden_size, n_classes, device)
-        self.rits_b = RITS(n_steps, n_features, rnn_hidden_size, n_classes, device)
         self.classification_weight = classification_weight
         self.reconstruction_weight = reconstruction_weight
 
-    def impute(self, inputs: dict) -> torch.Tensor:
-        return super().impute(inputs)
+        # create models
+        self.model = BackboneBRITS(n_steps, n_features, rnn_hidden_size)
+        self.f_classifier = nn.Linear(self.rnn_hidden_size, n_classes)
+        self.b_classifier = nn.Linear(self.rnn_hidden_size, n_classes)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
-        """Forward processing of BRITS.
-
-        Parameters
-        ----------
-        inputs :
-            The input data.
-
-        training :
-            Whether in training mode.
-
-        Returns
-        -------
-        dict, A dictionary includes all results.
-        """
-        ret_f = self.rits_f(inputs, "forward")
-        ret_b = self._reverse(self.rits_b(inputs, "backward"))
-
-        classification_pred = (ret_f["prediction"] + ret_b["prediction"]) / 2
-        results = {"classification_pred": classification_pred}
+        (
+            imputed_data,
+            f_reconstruction,
+            b_reconstruction,
+            f_hidden_states,
+            b_hidden_states,
+            consistency_loss,
+            reconstruction_loss,
+        ) = self.model(inputs)
+
+        f_logits = self.f_classifier(f_hidden_states)
+        b_logits = self.b_classifier(b_hidden_states)
+        f_prediction = torch.softmax(f_logits, dim=1)
+        b_prediction = torch.softmax(b_logits, dim=1)
+        classification_pred = (f_prediction + b_prediction) / 2
+
+        results = {
+            "imputed_data": imputed_data,
+            "classification_pred": classification_pred,
+        }
 
         # if in training mode, return results with losses
         if training:
-            ret_f["classification_loss"] = F.nll_loss(
-                torch.log(ret_f["prediction"]), inputs["label"]
-            )
-            ret_b["classification_loss"] = F.nll_loss(
-                torch.log(ret_b["prediction"]), inputs["label"]
-            )
-            consistency_loss = self._get_consistency_loss(
-                ret_f["imputed_data"], ret_b["imputed_data"]
-            )
-            classification_loss = (
-                ret_f["classification_loss"] + ret_b["classification_loss"]
-            ) / 2
-            reconstruction_loss = (
-                ret_f["reconstruction_loss"] + ret_b["reconstruction_loss"]
-            ) / 2
-
             results["consistency_loss"] = consistency_loss
-            results["classification_loss"] = classification_loss
             results["reconstruction_loss"] = reconstruction_loss
-
-            # `loss` is always the item for backward propagating to update the model
+            f_classification_loss = F.nll_loss(torch.log(f_prediction), inputs["label"])
+            b_classification_loss = F.nll_loss(torch.log(b_prediction), inputs["label"])
+            classification_loss = (f_classification_loss + b_classification_loss) / 2
             loss = (
                 consistency_loss
                 + reconstruction_loss * self.reconstruction_weight
                 + classification_loss * self.classification_weight
             )
+
+            # `loss` is always the item for backward propagating to update the model
             results["loss"] = loss
+            results["reconstruction"] = (f_reconstruction + b_reconstruction) / 2
+            results["classification_loss"] = classification_loss
+            results["f_reconstruction"] = f_reconstruction
+            results["b_reconstruction"] = b_reconstruction
 
         return results
```

### Comparing `pypots-0.4/pypots/classification/grud/data.py` & `pypots-0.4.1/pypots/classification/grud/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/classification/grud/model.py` & `pypots-0.4.1/pypots/classification/grud/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-The implementation of GRU-D for the partially-observed time-series imputation task.
+The implementation of GRU-D for the partially-observed time-series classification task.
 
 Refer to the paper "Zhengping Che, Sanjay Purushotham, Kyunghyun Cho, David Sontag, and Yan Liu.
 Recurrent Neural Networks for Multivariate Time Series with Missing Values.
 Scientific Reports, 8(1):6085, April 2018."
 
 """
 
@@ -13,16 +13,16 @@
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _GRUD
 from .data import DatasetForGRUD
-from .modules import _GRUD
 from ..base import BaseNNClassifier
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
 class GRUD(BaseNNClassifier):
```

### Comparing `pypots-0.4/pypots/classification/raindrop/data.py` & `pypots-0.4.1/pypots/classification/raindrop/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/classification/raindrop/model.py` & `pypots-0.4.1/pypots/classification/raindrop/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .modules import _Raindrop
+from .core import _Raindrop
 from ...classification.base import BaseNNClassifier
 from ...classification.grud.data import DatasetForGRUD
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
@@ -155,16 +155,15 @@
             n_heads,
             n_classes,
             dropout,
             n_steps,
             d_static,
             aggregation,
             sensor_wise_mask,
-            static=static,
-            device=self.device,
+            static,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/classification/raindrop/modules/core.py` & `pypots-0.4.1/pypots/nn/modules/raindrop/backbone.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 """
 
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
+from typing import Tuple
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn import TransformerEncoderLayer, TransformerEncoder
 from torch.nn.parameter import Parameter
 
 from ....utils.logging import logger
 
 try:
-    from .submodules import PositionalEncoding, ObservationPropagation
+    from .layers import PositionalEncoding, ObservationPropagation
     from torch_geometric.nn.inits import glorot
 except ImportError as e:
     logger.error(
         f"❌ {e}\n"
         "Note torch_geometric is missing, please install it with "
         "'pip install torch_geometric torch_scatter torch_sparse' or "
         "'conda install -c pyg pyg pytorch-scatter pytorch-sparse'"
@@ -34,55 +36,54 @@
         f"❌ {e}\n"
         "Note torch_geometric is missing, please install it with "
         "'pip install torch_geometric torch_scatter torch_sparse' or "
         "'conda install -c pyg pyg pytorch-scatter pytorch-sparse'"
     )
 
 
-class _Raindrop(nn.Module):
+class BackboneRaindrop(nn.Module):
     def __init__(
         self,
         n_features,
         n_layers,
         d_model,
         d_ffn,
         n_heads,
         n_classes,
         dropout=0.3,
         max_len=215,
         d_static=9,
+        d_pe=16,
         aggregation="mean",
         sensor_wise_mask=False,
         static=False,
-        device=None,
     ):
         super().__init__()
         self.n_layers = n_layers
         self.n_features = n_features
         self.d_model = d_model
         self.d_ffn = d_ffn
         self.n_heads = n_heads
         self.n_classes = n_classes
         self.dropout = dropout
         self.max_len = max_len
         self.d_static = d_static
         self.aggregation = aggregation
         self.sensor_wise_mask = sensor_wise_mask
         self.static = static
-        self.device = device
 
         # create modules
         if self.static:
             self.static_emb = nn.Linear(d_static, n_features)
         else:
             self.static_emb = None
         assert d_model % n_features == 0, "d_model must be divisible by n_features"
         self.d_ob = int(d_model / n_features)
         self.encoder = nn.Linear(n_features * self.d_ob, n_features * self.d_ob)
-        d_pe = 16
+
         self.pos_encoder = PositionalEncoding(d_pe, max_len)
         if self.sensor_wise_mask:
             dim_check = n_features * (self.d_ob + d_pe)
             assert dim_check % n_heads == 0, "dim_check must be divisible by n_heads"
             encoder_layers = TransformerEncoderLayer(
                 n_features * (self.d_ob + d_pe), n_heads, d_ffn, dropout
             )
@@ -117,80 +118,84 @@
 
         self.mlp_static = nn.Sequential(
             nn.Linear(d_final, d_final),
             nn.ReLU(),
             nn.Linear(d_final, n_classes),
         )
 
-        self.dropout = nn.Dropout(dropout)
+        self.dropout_layer = nn.Dropout(dropout)
         self.init_weights()
 
     def init_weights(self):
         init_range = 1e-10
         self.encoder.weight.data.uniform_(-init_range, init_range)
         if self.static:
             self.static_emb.weight.data.uniform_(-init_range, init_range)
         glorot(self.R_u)
 
-    def classify(self, inputs: dict) -> torch.Tensor:
+    def forward(
+        self,
+        X: torch.Tensor,
+        timestamps: torch.Tensor,
+        lengths: torch.Tensor,
+    ) -> Tuple[torch.Tensor, ...]:
         """Forward processing of BRITS.
 
         Parameters
         ----------
-        inputs : dict,
-            The input data.
+        X :
+            The input tensor of shape (batch_size, n_features, max_len).
+
+        timestamps :
+            The timestamps tensor of shape (batch_size, max_len).
+
+        lengths :
+            The lengths tensor of shape (batch_size, 1).
 
         Returns
         -------
         prediction : torch.Tensor
         """
-        src = inputs["X"].permute(1, 0, 2)
-        static = inputs["static"]
-        times = inputs["timestamps"].permute(1, 0)
-        lengths = inputs["lengths"]
-        missing_mask = inputs["missing_mask"].permute(1, 0, 2)
+        src = X.permute(1, 0, 2)
+        times = timestamps.permute(1, 0)
 
+        device = src.device
         max_len, batch_size = src.shape[0], src.shape[1]
 
         src = torch.repeat_interleave(src, self.d_ob, dim=-1)
         h = F.relu(src * self.R_u)
-        pe = self.pos_encoder(times).to(src.device)
-        if static is not None:
-            emb = self.static_emb(static)
-
-        h = self.dropout(h)
+        pe = self.pos_encoder(times).to(device)
+        h = self.dropout_layer(h)
 
         mask = torch.arange(max_len)[None, :] >= (lengths.cpu()[:, None])
-        mask = mask.squeeze(1).to(src.device)
+        mask = mask.squeeze(1).to(device)
 
         x = h
 
-        adj = torch.ones(self.n_features, self.n_features, device=src.device)
+        adj = torch.ones(self.n_features, self.n_features, device=device)
         adj[torch.eye(self.n_features, dtype=torch.bool)] = 1
 
         edge_index = torch.nonzero(adj).T
         edge_weights = adj[edge_index[0], edge_index[1]]
 
-        batch_size = src.shape[1]
-        n_step = src.shape[0]
         output = torch.zeros(
-            [n_step, batch_size, self.n_features * self.d_ob], device=src.device
+            [max_len, batch_size, self.n_features * self.d_ob], device=device
         )
 
-        alpha_all = torch.zeros([edge_index.shape[1], batch_size], device=src.device)
+        alpha_all = torch.zeros([edge_index.shape[1], batch_size], device=device)
 
         # iterate on each sample
         for unit in range(0, batch_size):
             step_data = x[:, unit, :]
             p_t = pe[:, unit, :]
 
-            step_data = step_data.reshape([n_step, self.n_features, self.d_ob]).permute(
-                1, 0, 2
-            )
-            step_data = step_data.reshape(self.n_features, n_step * self.d_ob)
+            step_data = step_data.reshape(
+                [max_len, self.n_features, self.d_ob]
+            ).permute(1, 0, 2)
+            step_data = step_data.reshape(self.n_features, max_len * self.d_ob)
 
             step_data, attention_weights = self.ob_propagation(
                 step_data,
                 p_t=p_t,
                 edge_index=edge_index,
                 edge_weights=edge_weights,
                 use_beta=False,
@@ -207,15 +212,15 @@
                 edge_index=edge_index_layer2,
                 edge_weights=edge_weights_layer2,
                 use_beta=False,
                 edge_attr=None,
                 return_attention_weights=True,
             )
 
-            step_data = step_data.view([self.n_features, n_step, self.d_ob])
+            step_data = step_data.view([self.n_features, max_len, self.d_ob])
             step_data = step_data.permute([1, 0, 2])  # [n_step, n_features, d_ob]
             step_data = step_data.reshape([-1, self.n_features * self.d_ob])
 
             output[:, unit, :] = step_data
             alpha_all[:, unit] = attention_weights[1].squeeze(-1)
 
         # distance = torch.cdist(alpha_all.T, alpha_all.T, p=2)
@@ -225,52 +230,9 @@
             extend_output = output.view(-1, batch_size, self.n_features, self.d_ob)
             extended_pe = pe.unsqueeze(2).repeat([1, 1, self.n_features, 1])
             output = torch.cat([extend_output, extended_pe], dim=-1)
             output = output.view(-1, batch_size, self.n_features * (self.d_ob + 16))
         else:
             output = torch.cat([output, pe], dim=2)
 
-        r_out = self.transformer_encoder(output, src_key_padding_mask=mask)
-
-        lengths2 = lengths.unsqueeze(1).to(src.device)
-        mask2 = mask.permute(1, 0).unsqueeze(2).long()
-        if self.sensor_wise_mask:
-            output = torch.zeros(
-                [batch_size, self.n_features, self.d_ob + 16], device=src.device
-            )
-            extended_missing_mask = missing_mask.view(-1, batch_size, self.n_features)
-            for se in range(self.n_features):
-                r_out = r_out.view(-1, batch_size, self.n_features, (self.d_ob + 16))
-                out = r_out[:, :, se, :]
-                l_ = torch.sum(extended_missing_mask[:, :, se], dim=0).unsqueeze(
-                    1
-                )  # length
-                out_sensor = torch.sum(
-                    out * (1 - extended_missing_mask[:, :, se].unsqueeze(-1)), dim=0
-                ) / (l_ + 1)
-                output[:, se, :] = out_sensor
-            output = output.view([-1, self.n_features * (self.d_ob + 16)])
-        elif self.aggregation == "mean":
-            output = torch.sum(r_out * (1 - mask2), dim=0) / (lengths2 + 1)
-        else:
-            raise RuntimeError
-
-        if static is not None:
-            output = torch.cat([output, emb], dim=1)
-
-        logits = self.mlp_static(output)
-        prediction = torch.softmax(logits, dim=1)
-
-        return prediction
-
-    def forward(self, inputs, training=True):
-        classification_pred = self.classify(inputs)
-        results = {"classification_pred": classification_pred}
-
-        # if in training mode, return results with losses
-        if training:
-            classification_loss = F.nll_loss(
-                torch.log(classification_pred), inputs["label"]
-            )
-            results["loss"] = classification_loss
-
-        return results
+        output = self.transformer_encoder(output, src_key_padding_mask=mask)
+        return output, mask
```

### Comparing `pypots-0.4/pypots/classification/raindrop/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/raindrop/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/cli/base.py` & `pypots-0.4.1/pypots/cli/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/cli/dev.py` & `pypots-0.4.1/pypots/cli/dev.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/cli/doc.py` & `pypots-0.4.1/pypots/cli/doc.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/cli/env.py` & `pypots-0.4.1/pypots/cli/env.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/cli/pypots_cli.py` & `pypots-0.4.1/pypots/cli/pypots_cli.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/cli/tuning.py` & `pypots-0.4.1/pypots/cli/tuning.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/cli/utils.py` & `pypots-0.4.1/pypots/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/clustering/base.py` & `pypots-0.4.1/pypots/clustering/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/clustering/crli/data.py` & `pypots-0.4.1/pypots/clustering/crli/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/clustering/crli/model.py` & `pypots-0.4.1/pypots/clustering/crli/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 import os
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _CRLI
 from .data import DatasetForCRLI
-from .modules import _CRLI
 from ..base import BaseNNClusterer
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 try:
     import nni
@@ -157,29 +157,28 @@
             n_features,
             n_clusters,
             n_generator_layers,
             rnn_hidden_size,
             decoder_fcn_output_dims,
             lambda_kmeans,
             rnn_cell_type,
-            self.device,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.G_optimizer = G_optimizer
         self.G_optimizer.init_optimizer(
             [
-                {"params": self.model.generator.parameters()},
-                {"params": self.model.decoder.parameters()},
+                {"params": self.model.backbone.generator.parameters()},
+                {"params": self.model.backbone.decoder.parameters()},
             ]
         )
         self.D_optimizer = D_optimizer
-        self.D_optimizer.init_optimizer(self.model.discriminator.parameters())
+        self.D_optimizer.init_optimizer(self.model.backbone.discriminator.parameters())
 
     def _assemble_input_for_training(self, data: list) -> dict:
         # fetch data
         indices, X, missing_mask = self._send_data_to_given_device(data)
 
         inputs = {
             "X": X,
```

### Comparing `pypots-0.4/pypots/clustering/crli/modules/core.py` & `pypots-0.4.1/pypots/clustering/crli/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,105 +6,100 @@
 Learning Representations for Incomplete Time Series Clustering. AAAI 2021."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from typing import Union, Optional
+from typing import Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from sklearn.cluster import KMeans
 
-from .submodules import Generator, Decoder, Discriminator
-from ....utils.metrics import calc_mse
+from ...nn.modules.crli import BackboneCRLI
+from ...utils.metrics import calc_mse
 
 
 class _CRLI(nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_clusters: int,
         n_generator_layers: int,
         rnn_hidden_size: int,
         decoder_fcn_output_dims: Optional[list],
         lambda_kmeans: float,
         rnn_cell_type: str = "GRU",
-        device: Union[str, torch.device] = "cpu",
     ):
         super().__init__()
-        self.generator = Generator(
-            n_generator_layers, n_features, rnn_hidden_size, rnn_cell_type, device
+
+        self.backbone = BackboneCRLI(
+            n_steps,
+            n_features,
+            n_generator_layers,
+            rnn_hidden_size,
+            decoder_fcn_output_dims,
+            rnn_cell_type,
         )
-        self.discriminator = Discriminator(rnn_cell_type, n_features, device)
-        self.decoder = Decoder(
-            n_steps, rnn_hidden_size * 2, n_features, decoder_fcn_output_dims, device
-        )  # fully connected network is included in Decoder
+
         self.kmeans = KMeans(
             n_clusters=n_clusters,
             n_init=10,  # FutureWarning: The default value of `n_init` will change from 10 to 'auto' in 1.4. Set the
             # value of `n_init` explicitly to suppress the warning.
         )
         self.term_F = None
         self.counter_for_updating_F = 0
 
         self.n_clusters = n_clusters
         self.lambda_kmeans = lambda_kmeans
-        self.device = device
 
     def forward(
         self,
         inputs: dict,
         training_object: str = "generator",
         training: bool = True,
     ) -> dict:
-        X = inputs["X"]
-        missing_mask = inputs["missing_mask"]
-        losses = {}
-
-        # concat final states from generator and input it as the initial state of decoder
-        imputation_latent, generator_fb_hidden_states = self.generator(inputs)
-        inputs["imputation_latent"] = imputation_latent
-        inputs["generator_fb_hidden_states"] = generator_fb_hidden_states
-        discrimination = self.discriminator(inputs)
-        inputs["discrimination"] = discrimination
-
-        reconstruction, fcn_latent = self.decoder(inputs)
-        inputs["reconstruction"] = reconstruction
-        inputs["fcn_latent"] = fcn_latent
+        X, missing_mask = inputs["X"], inputs["missing_mask"]
+        imputation_latent, discrimination, reconstruction, fcn_latent = self.backbone(
+            X, missing_mask
+        )
+        results = {
+            "imputation_latent": imputation_latent,
+            "discrimination": discrimination,
+            "reconstruction": reconstruction,
+            "fcn_latent": fcn_latent,
+        }
 
         # return results directly, skip loss calculation to reduce inference time
         if not training:
-            return inputs
+            return results
 
         if training_object == "discriminator":
-            l_D = F.binary_cross_entropy_with_logits(
-                inputs["discrimination"], missing_mask
-            )
-            losses["discrimination_loss"] = l_D
+            l_D = F.binary_cross_entropy_with_logits(discrimination, missing_mask)
+            results["discrimination_loss"] = l_D
         else:
-            inputs["discrimination"] = inputs["discrimination"].detach()
+            # discrimination = discrimination.detach()
             l_G = F.binary_cross_entropy_with_logits(
-                inputs["discrimination"], 1 - missing_mask, weight=1 - missing_mask
+                discrimination, 1 - missing_mask, weight=1 - missing_mask
             )
-            l_pre = calc_mse(inputs["imputation_latent"], X, missing_mask)
-            l_rec = calc_mse(inputs["reconstruction"], X, missing_mask)
-            HTH = torch.matmul(inputs["fcn_latent"], inputs["fcn_latent"].permute(1, 0))
+            l_pre = calc_mse(imputation_latent, X, missing_mask)
+            l_rec = calc_mse(reconstruction, X, missing_mask)
+            HTH = torch.matmul(fcn_latent, fcn_latent.permute(1, 0))
 
             if (
                 self.counter_for_updating_F == 0
                 or self.counter_for_updating_F % 10 == 0
             ):
                 U, s, V = torch.linalg.svd(fcn_latent)
                 self.term_F = U[:, : self.n_clusters]
 
             FTHTHF = torch.matmul(
                 torch.matmul(self.term_F.permute(1, 0), HTH), self.term_F
             )
             l_kmeans = torch.trace(HTH) - torch.trace(FTHTHF)  # k-means loss
             loss_gene = l_G + l_pre + l_rec + l_kmeans * self.lambda_kmeans
-            losses["generation_loss"] = loss_gene
+            results["generation_loss"] = loss_gene
 
-        return losses
+        return results
```

### Comparing `pypots-0.4/pypots/clustering/crli/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/crli/layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Learning Representations for Incomplete Time Series Clustering. AAAI 2021."
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from typing import Tuple, Union
+from typing import Tuple
 
 import torch
 import torch.nn as nn
 
 RNN_CELL = {
     "LSTM": nn.LSTMCell,
     "GRU": nn.GRUCell,
@@ -33,45 +33,47 @@
 class MultiRNNCell(nn.Module):
     def __init__(
         self,
         cell_type: str,
         n_layer: int,
         d_input: int,
         d_hidden: int,
-        device: Union[str, torch.device],
     ):
         super().__init__()
         self.cell_type = cell_type
         self.n_layer = n_layer
         self.d_input = d_input
         self.d_hidden = d_hidden
-        self.device = device
 
         self.model = nn.ModuleList()
         if cell_type in ["LSTM", "GRU"]:
             for i in range(n_layer):
                 if i == 0:
                     self.model.append(RNN_CELL[cell_type](d_input, d_hidden))
                 else:
                     self.model.append(RNN_CELL[cell_type](d_hidden, d_hidden))
 
         self.output_layer = nn.Linear(d_hidden, d_input)
 
-    def forward(self, inputs: dict) -> Tuple[torch.Tensor, torch.Tensor]:
-        X, missing_mask = inputs["X"], inputs["missing_mask"]
+    def forward(
+        self, X: torch.Tensor, missing_mask: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+
         bz, n_steps, _ = X.shape
-        hidden_state = torch.zeros((bz, self.d_hidden), device=self.device)
+        device = X.device
+
+        hidden_state = torch.zeros((bz, self.d_hidden), device=device)
         hidden_state_collector = torch.empty(
-            (bz, n_steps, self.d_hidden), device=self.device
+            (bz, n_steps, self.d_hidden), device=device
         )
-        output_collector = torch.empty((bz, n_steps, self.d_input), device=self.device)
+        output_collector = torch.empty((bz, n_steps, self.d_input), device=device)
         if self.cell_type == "LSTM":
             cell_states = [
-                torch.zeros((bz, self.d_hidden), device=self.device)
-                for i in range(self.n_layer)
+                torch.zeros((bz, self.d_hidden), device=device)
+                for _ in range(self.n_layer)
             ]
 
             for step in range(n_steps):
                 x = X[:, step, :]
                 estimation = self.output_layer(hidden_state)
                 output_collector[:, step] = estimation
                 imputed_x = (
@@ -107,81 +109,84 @@
 
         output_collector = output_collector[:, 1:]
         estimation = self.output_layer(hidden_state).unsqueeze(1)
         output_collector = torch.concat([output_collector, estimation], dim=1)
         return output_collector, hidden_state
 
 
-class Generator(nn.Module):
+class CrliGenerator(nn.Module):
     def __init__(
         self,
         n_layers: int,
         n_features: int,
         d_hidden: int,
         cell_type: str,
-        device: Union[str, torch.device],
     ):
         super().__init__()
-        self.f_rnn = MultiRNNCell(cell_type, n_layers, n_features, d_hidden, device)
-        self.b_rnn = MultiRNNCell(cell_type, n_layers, n_features, d_hidden, device)
+        self.f_rnn = MultiRNNCell(cell_type, n_layers, n_features, d_hidden)
+        self.b_rnn = MultiRNNCell(cell_type, n_layers, n_features, d_hidden)
 
-    def forward(self, inputs: dict) -> Tuple[torch.Tensor, torch.Tensor]:
-        f_outputs, f_final_hidden_state = self.f_rnn(inputs)
-        b_outputs, b_final_hidden_state = self.b_rnn(inputs)
+    def forward(
+        self, X: torch.Tensor, missing_mask: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        f_outputs, f_final_hidden_state = self.f_rnn(X, missing_mask)
+        b_outputs, b_final_hidden_state = self.b_rnn(X, missing_mask)
         b_outputs = reverse_tensor(b_outputs)  # reverse the output of the backward rnn
         imputation_latent = (f_outputs + b_outputs) / 2
         fb_final_hidden_states = torch.concat(
             [f_final_hidden_state, b_final_hidden_state], dim=-1
         )
         return imputation_latent, fb_final_hidden_states
 
 
-class Discriminator(nn.Module):
+class CrliDiscriminator(nn.Module):
     def __init__(
         self,
         cell_type: str,
         d_input: int,
-        device: Union[str, torch.device],
     ):
         super().__init__()
         self.cell_type = cell_type
-        self.device = device
         # this setting is the same with the official implementation
         self.rnn_cell_module_list = nn.ModuleList(
             [
                 RNN_CELL[cell_type](d_input, 32),
                 RNN_CELL[cell_type](32, 16),
                 RNN_CELL[cell_type](16, 8),
                 RNN_CELL[cell_type](8, 16),
                 RNN_CELL[cell_type](16, 32),
             ]
         )
         self.output_layer = nn.Linear(32, d_input)
 
-    def forward(self, inputs: dict) -> torch.Tensor:
-        imputed_X = (inputs["X"] * inputs["missing_mask"]) + (
-            inputs["imputation_latent"] * (1 - inputs["missing_mask"])
-        )
+    def forward(
+        self,
+        X: torch.Tensor,
+        missing_mask: torch.Tensor,
+        imputation_latent: torch.Tensor,
+    ) -> torch.Tensor:
+        imputed_X = (X * missing_mask) + (imputation_latent * (1 - missing_mask))
 
         bz, n_steps, _ = imputed_X.shape
+        device = imputed_X.device
         hidden_states = [
-            torch.zeros((bz, 32), device=self.device),
-            torch.zeros((bz, 16), device=self.device),
-            torch.zeros((bz, 8), device=self.device),
-            torch.zeros((bz, 16), device=self.device),
-            torch.zeros((bz, 32), device=self.device),
+            torch.zeros((bz, 32), device=device),
+            torch.zeros((bz, 16), device=device),
+            torch.zeros((bz, 8), device=device),
+            torch.zeros((bz, 16), device=device),
+            torch.zeros((bz, 32), device=device),
         ]
-        hidden_state_collector = torch.empty((bz, n_steps, 32), device=self.device)
+        hidden_state_collector = torch.empty((bz, n_steps, 32), device=device)
         if self.cell_type == "LSTM":
             cell_states = [
-                torch.zeros((bz, 32), device=self.device),
-                torch.zeros((bz, 16), device=self.device),
-                torch.zeros((bz, 8), device=self.device),
-                torch.zeros((bz, 16), device=self.device),
-                torch.zeros((bz, 32), device=self.device),
+                torch.zeros((bz, 32), device=device),
+                torch.zeros((bz, 16), device=device),
+                torch.zeros((bz, 8), device=device),
+                torch.zeros((bz, 16), device=device),
+                torch.zeros((bz, 32), device=device),
             ]
             for step in range(n_steps):
                 x = imputed_X[:, step, :]
                 for i, rnn_cell in enumerate(self.rnn_cell_module_list):
                     if i == 0:
                         hidden_state, cell_state = rnn_cell(
                             x, (hidden_states[i], cell_states[i])
@@ -206,48 +211,49 @@
                     hidden_states[i] = hidden_state
                 hidden_state_collector[:, step, :] = hidden_state
 
         output_collector = self.output_layer(hidden_state_collector)
         return output_collector
 
 
-class Decoder(nn.Module):
+class CrliDecoder(nn.Module):
     def __init__(
         self,
         n_steps: int,
         d_input: int,
         d_output: int,
         fcn_output_dims: list = None,
-        device: Union[str, torch.device] = "cpu",
     ):
         super().__init__()
         self.n_steps = n_steps
         self.d_output = d_output
-        self.device = device
 
         if fcn_output_dims is None:
             fcn_output_dims = [d_input]
         self.fcn_output_dims = fcn_output_dims
 
         self.fcn = nn.ModuleList()
         for output_dim in fcn_output_dims:
             self.fcn.append(nn.Linear(d_input, output_dim))
             d_input = output_dim
 
         self.rnn_cell = nn.GRUCell(fcn_output_dims[-1], fcn_output_dims[-1])
         self.output_layer = nn.Linear(fcn_output_dims[-1], d_output)
 
-    def forward(self, inputs: dict) -> Tuple[torch.Tensor, torch.Tensor]:
-        generator_fb_hidden_states = inputs["generator_fb_hidden_states"]
+    def forward(
+        self, generator_fb_hidden_states: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        device = generator_fb_hidden_states.device
         bz, _ = generator_fb_hidden_states.shape
+
         fcn_latent = generator_fb_hidden_states
         for layer in self.fcn:
             fcn_latent = layer(fcn_latent)
         hidden_state = fcn_latent
         hidden_state_collector = torch.empty(
-            (bz, self.n_steps, self.fcn_output_dims[-1]), device=self.device
+            (bz, self.n_steps, self.fcn_output_dims[-1]), device=device
         )
         for i in range(self.n_steps):
             hidden_state = self.rnn_cell(hidden_state, hidden_state)
             hidden_state_collector[:, i, :] = hidden_state
         reconstruction = self.output_layer(hidden_state_collector)
         return reconstruction, fcn_latent
```

### Comparing `pypots-0.4/pypots/clustering/vader/__init__.py` & `pypots-0.4.1/pypots/clustering/vader/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/clustering/vader/data.py` & `pypots-0.4.1/pypots/clustering/vader/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/clustering/vader/model.py` & `pypots-0.4.1/pypots/clustering/vader/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import numpy as np
 import torch
 from scipy.stats import multivariate_normal
 from sklearn.mixture import GaussianMixture
 from torch.utils.data import DataLoader
 
 from .data import DatasetForVaDER
-from .modules import inverse_softplus, _VaDER
+from .core import inverse_softplus, _VaDER
 from ..base import BaseNNClusterer
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 try:
     import nni
@@ -234,21 +234,21 @@
             mu = gmm.means_
             var = inverse_softplus(gmm.covariances_)
             phi = np.log(gmm.weights_ + 1e-9)  # inverse softmax
             device = results["z"].device
 
             # use trained GMM's parameters to init GMM layer's
             if isinstance(self.device, list):  # if using multi-GPU
-                self.model.module.gmm_layer.set_values(
+                self.model.module.backbone.gmm_layer.set_values(
                     torch.from_numpy(mu).to(device),
                     torch.from_numpy(var).to(device),
                     torch.from_numpy(phi).to(device),
                 )
             else:
-                self.model.gmm_layer.set_values(
+                self.model.backbone.gmm_layer.set_values(
                     torch.from_numpy(mu).to(device),
                     torch.from_numpy(var).to(device),
                     torch.from_numpy(phi).to(device),
                 )
 
         try:
             training_step = 0
```

### Comparing `pypots-0.4/pypots/clustering/vader/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/vader/layers.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,28 +9,21 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 from typing import Tuple, Optional
 
-import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Variable
 from torch.nn.parameter import Parameter
 
 
-def inverse_softplus(x: np.ndarray) -> np.ndarray:
-    b = x < 1e2
-    x[b] = np.log(np.exp(x[b]) - 1.0 + 1e-9)
-    return x
-
-
 class ImplicitImputation(nn.Module):
     def __init__(self, d_input: int):
         super().__init__()
         self.projection_layer = nn.Linear(d_input, d_input, bias=False)
 
     def forward(self, X: torch.Tensor, missing_mask: torch.Tensor) -> torch.Tensor:
         imputation = self.projection_layer(X)
```

### Comparing `pypots-0.4/pypots/data/__init__.py` & `pypots-0.4.1/pypots/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/data/base.py` & `pypots-0.4.1/pypots/data/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/data/generating.py` & `pypots-0.4.1/pypots/data/generating.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/data/load_preprocessing.py` & `pypots-0.4.1/pypots/data/load_preprocessing.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/data/load_specific_datasets.py` & `pypots-0.4.1/pypots/data/load_specific_datasets.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/data/saving/h5.py` & `pypots-0.4.1/pypots/data/saving/h5.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/data/saving/pickle.py` & `pypots-0.4.1/pypots/data/saving/pickle.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/data/utils.py` & `pypots-0.4.1/pypots/data/utils.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/forecasting/base.py` & `pypots-0.4.1/pypots/forecasting/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/forecasting/bttf/model.py` & `pypots-0.4.1/pypots/forecasting/bttf/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import warnings
 from typing import Union, Optional
 
 import numpy as np
 import torch
 
-from .modules import BTTF_forecast
+from .core import BTTF_forecast
 from ..base import BaseForecaster
 from ...utils.logging import logger
 
 
 class BTTF(BaseForecaster):
     """The implementation of the BTTF model :cite:`chen2021BTMF`.
```

### Comparing `pypots-0.4/pypots/forecasting/bttf/modules/core.py` & `pypots-0.4.1/pypots/forecasting/bttf/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,19 @@
     time_lags,
     burn_iter,
     gibbs_iter,
     gamma=10,
 ):
     dim1, dim2, T = dense_tensor.shape
     start_time = T - pred_step
+    assert start_time > -1, (
+        "start_time should be larger than -1, "
+        "namely the number of the input tensor's time steps should be larger than pred_step."
+    )
+    assert start_time >= np.max(time_lags), "start_time should be >= max(time_lags)"
     max_count = int(np.ceil(pred_step / multi_step))
     tensor_hat = np.zeros((dim1, dim2, max_count * multi_step))
 
     # t==0
     init = {
         "U": 0.1 * np.random.randn(dim1, rank),
         "V": 0.1 * np.random.randn(dim2, rank),
```

### Comparing `pypots-0.4/pypots/forecasting/bttf/modules/submodules.py` & `pypots-0.4.1/pypots/forecasting/bttf/submodules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/__init__.py` & `pypots-0.4.1/pypots/imputation/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/autoformer/__init__.py` & `pypots-0.4.1/pypots/imputation/autoformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/autoformer/data.py` & `pypots-0.4.1/pypots/imputation/autoformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/autoformer/model.py` & `pypots-0.4.1/pypots/imputation/autoformer/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .data import DatasetForAutoformer
-from .modules.core import _Autoformer
+from pypots.imputation.autoformer.core import _Autoformer
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
@@ -59,14 +59,20 @@
 
     moving_avg_window_size :
         The window size of moving average.
 
     dropout :
         The dropout rate for the model.
 
+    ORT_weight :
+        The weight for the ORT loss, the same as SAITS.
+
+    MIT_weight :
+        The weight for the MIT loss, the same as SAITS.
+
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
     patience :
@@ -111,14 +117,16 @@
         n_layers: int,
         n_heads: int,
         d_model: int,
         d_ffn: int,
         factor: int,
         moving_avg_window_size: int,
         dropout: float = 0,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -140,26 +148,30 @@
         self.n_heads = n_heads
         self.n_layers = n_layers
         self.d_model = d_model
         self.d_ffn = d_ffn
         self.factor = factor
         self.moving_avg_window_size = moving_avg_window_size
         self.dropout = dropout
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _Autoformer(
             self.n_steps,
             self.n_features,
             self.n_layers,
             self.n_heads,
             self.d_model,
             self.d_ffn,
             self.factor,
             self.moving_avg_window_size,
             self.dropout,
+            self.ORT_weight,
+            self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/imputation/autoformer/modules/core.py` & `pypots-0.4.1/pypots/imputation/autoformer/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,55 +4,56 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import torch
 import torch.nn as nn
 
-from .submodules import (
+from ...nn.modules.autoformer import (
     SeasonalLayerNorm,
     AutoformerEncoderLayer,
     AutoCorrelation,
     AutoCorrelationLayer,
 )
-from ...informer.modules.submodules import InformerEncoder
-from ....nn.modules.transformer.embedding import DataEmbedding
-from ....utils.metrics import calc_mse
+from ...nn.modules.informer import InformerEncoder
+from ...nn.modules.saits import SaitsLoss
+from ...nn.modules.transformer.embedding import DataEmbedding
 
 
 class _Autoformer(nn.Module):
     def __init__(
         self,
         n_steps,
         n_features,
         n_layers,
         n_heads,
         d_model,
         d_ffn,
         factor,
         moving_avg_window_size,
         dropout,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         activation="relu",
-        output_attention=False,
     ):
         super().__init__()
 
-        self.seq_len = n_steps
-        self.n_layers = n_layers
+        self.n_steps = n_steps
+
         self.enc_embedding = DataEmbedding(
             n_features * 2,
             d_model,
             dropout=dropout,
             with_pos=False,
         )
         self.encoder = InformerEncoder(
             [
                 AutoformerEncoderLayer(
                     AutoCorrelationLayer(
-                        AutoCorrelation(False, factor, dropout, output_attention),
+                        AutoCorrelation(factor, dropout),
                         d_model,
                         n_heads,
                     ),
                     d_model,
                     d_ffn,
                     moving_avg_window_size,
                     dropout,
@@ -61,38 +62,44 @@
                 for _ in range(n_layers)
             ],
             norm_layer=SeasonalLayerNorm(d_model),
         )
 
         # for the imputation task, the output dim is the same as input dim
         self.output_projection = nn.Linear(d_model, n_features)
+        self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
-        X, masks = inputs["X"], inputs["missing_mask"]
+        X, missing_mask = inputs["X"], inputs["missing_mask"]
 
         # WDU: the original Autoformer paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
         # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
         # embedding layers to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
 
         # the same as SAITS, concatenate the time series data and the missing mask for embedding
-        input_X = torch.cat([X, masks], dim=2)
+        input_X = torch.cat([X, missing_mask], dim=2)
         enc_out = self.enc_embedding(input_X)
 
         # Autoformer encoder processing
         enc_out, attns = self.encoder(enc_out)
-
         # project back the original data space
-        output = self.output_projection(enc_out)
+        reconstruction = self.output_projection(enc_out)
 
-        imputed_data = masks * X + (1 - masks) * output
+        imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
         results = {
             "imputed_data": imputed_data,
         }
 
+        # if in training mode, return results with losses
         if training:
+            X_ori, indicating_mask = inputs["X_ori"], inputs["indicating_mask"]
+            loss, ORT_loss, MIT_loss = self.saits_loss_func(
+                reconstruction, X_ori, missing_mask, indicating_mask
+            )
+            results["ORT_loss"] = ORT_loss
+            results["MIT_loss"] = MIT_loss
             # `loss` is always the item for backward propagating to update the model
-            loss = calc_mse(output, inputs["X_ori"], inputs["indicating_mask"])
             results["loss"] = loss
 
         return results
```

### Comparing `pypots-0.4/pypots/imputation/autoformer/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/autoformer/layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,19 @@
         (2) time delay aggregation
 
     This block can replace the self-attention family mechanism seamlessly.
     """
 
     def __init__(
         self,
-        mask_flag=True,
         factor=1,
-        scale=None,
         attention_dropout=0.1,
-        output_attention=False,
     ):
         super().__init__()
         self.factor = factor
-        self.scale = scale
-        self.mask_flag = mask_flag
-        self.output_attention = output_attention
         self.dropout = nn.Dropout(attention_dropout)
 
     def time_delay_agg_training(self, values, corr):
         """
         SpeedUp version of Autocorrelation (a batch-normalization style design)
         This is for the training phase.
         """
@@ -161,18 +155,15 @@
                 values.permute(0, 2, 3, 1).contiguous(), corr
             ).permute(0, 3, 1, 2)
         else:
             V = self.time_delay_agg_inference(
                 values.permute(0, 2, 3, 1).contiguous(), corr
             ).permute(0, 3, 1, 2)
 
-        if self.output_attention:
-            return (V.contiguous(), corr.permute(0, 3, 1, 2))
-        else:
-            return (V.contiguous(), None)
+        return V.contiguous(), corr.permute(0, 3, 1, 2)
 
 
 class AutoCorrelationLayer(nn.Module):
     def __init__(self, correlation, d_model, n_heads, d_keys=None, d_values=None):
         super().__init__()
 
         d_keys = d_keys or (d_model // n_heads)
```

### Comparing `pypots-0.4/pypots/imputation/base.py` & `pypots-0.4.1/pypots/imputation/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/brits/__init__.py` & `pypots-0.4.1/pypots/imputation/brits/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/brits/data.py` & `pypots-0.4.1/pypots/imputation/brits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/brits/model.py` & `pypots-0.4.1/pypots/imputation/brits/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _BRITS
 from .data import DatasetForBRITS
-from .modules import _BRITS
 from ..base import BaseNNImputer
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
@@ -114,15 +114,14 @@
         self.rnn_hidden_size = rnn_hidden_size
 
         # set up the model
         self.model = _BRITS(
             self.n_steps,
             self.n_features,
             self.rnn_hidden_size,
-            self.device,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/imputation/brits/modules/core.py` & `pypots-0.4.1/pypots/imputation/fedformer/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,339 +1,346 @@
 """
-The implementation of BRITS for the partially-observed time-series imputation task.
+The implementation of FEDformer for the partially-observed time-series imputation task.
 
-Refer to the paper "Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018).
-BRITS: Bidirectional Recurrent Imputation for Time Series. NeurIPS 2018."
+Refer to the paper "Tian Zhou, Ziqing Ma, Qingsong Wen, Xue Wang, Liang Sun, and Rong Jin.
+FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting.
+In ICML, volume 162 of Proceedings of Machine Learning Research, pages 27268–27286. PMLR, 17–23 Jul 2022.".
 
 Notes
 -----
-Partial implementation uses code from https://github.com/caow13/BRITS. The bugs in the original implementation
-are fixed here.
+Partial implementation uses code from https://github.com/MAZiqing/FEDformer
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from typing import Tuple, Union
+from typing import Union, Optional
 
+import numpy as np
 import torch
-import torch.nn as nn
+from torch.utils.data import DataLoader
 
-from .submodules import FeatureRegression
-from ....nn.modules.rnn import TemporalDecay
-from ....utils.metrics import calc_mae
+from .core import _FEDformer
+from .data import DatasetForFEDformer
+from ..base import BaseNNImputer
+from ...data.base import BaseDataset
+from ...data.checking import check_X_ori_in_val_set
+from ...optim.adam import Adam
+from ...optim.base import Optimizer
+from ...utils.logging import logger
 
 
-class RITS(nn.Module):
-    """model RITS: Recurrent Imputation for Time Series
+class FEDformer(BaseNNImputer):
+    """The PyTorch implementation of the FEDformer model.
+    FEDformer is originally proposed by Woo et al. in :cite:`zhou2022fedformer`.
 
-    Attributes
+    Parameters
     ----------
     n_steps :
-        sequence length (number of time steps)
+        The number of time steps in the time-series data sample.
 
     n_features :
-        number of features (input dimensions)
+        The number of features in the time-series data sample.
 
-    rnn_hidden_size :
-        the hidden size of the RNN cell
+    n_layers :
+        The number of layers in the FEDformer.
 
-    device :
-        specify running the model on which device, CPU/GPU
+    n_heads :
+        The number of heads in the multi-head attention mechanism.
 
-    rnn_cell :
-        the LSTM cell to model temporal data
+    d_model :
+        The dimension of the model.
 
-    temp_decay_h :
-        the temporal decay module to decay RNN hidden state
+    d_ffn :
+        The dimension of the feed-forward network.
 
-    temp_decay_x :
-        the temporal decay module to decay data in the raw feature space
+    moving_avg_window_size :
+        The window size of moving average.
 
-    hist_reg :
-        the temporal-regression module to project RNN hidden state into the raw feature space
+    dropout :
+        The dropout rate for the model.
 
-    feat_reg :
-        the feature-regression module
+    version :
+        The version of the model. It has to be one of ["Wavelets", "Fourier"].
+        The default value is "Fourier".
 
-    combining_weight :
-        the module used to generate the weight to combine history regression and feature regression
+    modes :
+        The number of modes to be selected. The default value is 32.
 
-    Parameters
-    ----------
-    n_steps :
-        sequence length (number of time steps)
+    mode_select :
+        Get modes on frequency domain. It has to "random" or "low". The default value is "random".
+        'random' means sampling randomly; 'low' means sampling the lowest modes;
 
-    n_features :
-        number of features (input dimensions)
+    ORT_weight :
+        The weight for the ORT loss, the same as SAITS.
+
+    MIT_weight :
+        The weight for the MIT loss, the same as SAITS.
+
+    batch_size :
+        The batch size for training and evaluating the model.
+
+    epochs :
+        The number of epochs for training the model.
+
+    patience :
+        The patience for the early-stopping mechanism. Given a positive integer, the training process will be
+        stopped when the model does not perform better after that number of epochs.
+        Leaving it default as None will disable the early-stopping.
 
-    rnn_hidden_size :
-        the hidden size of the RNN cell
+    optimizer :
+        The optimizer for model training.
+        If not given, will use a default Adam optimizer.
+
+    num_workers :
+        The number of subprocesses to use for data loading.
+        `0` means data loading will be in the main process, i.e. there won't be subprocesses.
 
     device :
-        specify running the model on which device, CPU/GPU
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
+        then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
+        Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
+
+    saving_path :
+        The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
+        training into a tensorboard file). Will not save if not given.
+
+    model_saving_strategy :
+        The strategy to save model checkpoints. It has to be one of [None, "best", "better", "all"].
+        No model will be saved when it is set as None.
+        The "best" strategy will only automatically save the best model after the training finished.
+        The "better" strategy will automatically save the model during training whenever the model performs
+        better than in previous epochs.
+        The "all" strategy will save every model after each epoch training.
 
     """
 
     def __init__(
         self,
-        n_steps: int,
-        n_features: int,
-        rnn_hidden_size: int,
-        device: Union[str, torch.device],
+        n_steps,
+        n_features,
+        n_layers,
+        n_heads,
+        d_model,
+        d_ffn,
+        moving_avg_window_size,
+        dropout: float = 0,
+        version="Fourier",
+        modes=32,
+        mode_select="random",
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
+        batch_size: int = 32,
+        epochs: int = 100,
+        patience: int = None,
+        optimizer: Optional[Optimizer] = Adam(),
+        num_workers: int = 0,
+        device: Optional[Union[str, torch.device, list]] = None,
+        saving_path: str = None,
+        model_saving_strategy: Optional[str] = "best",
     ):
-        super().__init__()
+        super().__init__(
+            batch_size,
+            epochs,
+            patience,
+            num_workers,
+            device,
+            saving_path,
+            model_saving_strategy,
+        )
+
         self.n_steps = n_steps
         self.n_features = n_features
-        self.rnn_hidden_size = rnn_hidden_size
-        self.device = device
-
-        self.rnn_cell = nn.LSTMCell(self.n_features * 2, self.rnn_hidden_size)
-        self.temp_decay_h = TemporalDecay(
-            input_size=self.n_features, output_size=self.rnn_hidden_size, diag=False
-        )
-        self.temp_decay_x = TemporalDecay(
-            input_size=self.n_features, output_size=self.n_features, diag=True
+        # model hype-parameters
+        self.n_layers = n_layers
+        self.n_heads = n_heads
+        self.d_model = d_model
+        self.d_ffn = d_ffn
+        self.moving_avg_window_size = moving_avg_window_size
+        self.dropout = dropout
+        self.version = version
+        self.modes = modes
+        self.mode_select = mode_select
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
+
+        # set up the model
+        self.model = _FEDformer(
+            self.n_steps,
+            self.n_features,
+            self.n_layers,
+            self.n_heads,
+            self.d_model,
+            self.d_ffn,
+            self.moving_avg_window_size,
+            self.dropout,
+            self.version,
+            self.modes,
+            self.mode_select,
+            self.ORT_weight,
+            self.MIT_weight,
         )
-        self.hist_reg = nn.Linear(self.rnn_hidden_size, self.n_features)
-        self.feat_reg = FeatureRegression(self.n_features)
-        self.combining_weight = nn.Linear(self.n_features * 2, self.n_features)
+        self._send_model_to_given_device()
+        self._print_model_size()
 
-    def impute(
-        self, inputs: dict, direction: str
-    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
-        """The imputation function.
-        Parameters
-        ----------
-        inputs :
-            Input data, a dictionary includes feature values, missing masks, and time-gap values.
+        # set up the optimizer
+        self.optimizer = optimizer
+        self.optimizer.init_optimizer(self.model.parameters())
+
+    def _assemble_input_for_training(self, data: list) -> dict:
+        (
+            indices,
+            X,
+            missing_mask,
+            X_ori,
+            indicating_mask,
+        ) = self._send_data_to_given_device(data)
+
+        inputs = {
+            "X": X,
+            "missing_mask": missing_mask,
+            "X_ori": X_ori,
+            "indicating_mask": indicating_mask,
+        }
 
-        direction :
-            A keyword to extract data from parameter `data`.
+        return inputs
 
-        Returns
-        -------
-        imputed_data :
-            Input data with missing parts imputed. Shape of [batch size, sequence length, feature number].
+    def _assemble_input_for_validating(self, data: list) -> dict:
+        return self._assemble_input_for_training(data)
 
-        estimations :
-            Reconstructed data. Shape of [batch size, sequence length, feature number].
+    def _assemble_input_for_testing(self, data: list) -> dict:
+        indices, X, missing_mask = self._send_data_to_given_device(data)
 
-        hidden_states: tensor,
-            [batch size, RNN hidden size]
+        inputs = {
+            "X": X,
+            "missing_mask": missing_mask,
+        }
 
-        reconstruction_loss :
-            reconstruction loss
+        return inputs
 
-        """
-        values = inputs[direction]["X"]  # feature values
-        masks = inputs[direction]["missing_mask"]  # missing masks
-        deltas = inputs[direction]["deltas"]  # time-gap values
-
-        # create hidden states and cell states for the lstm cell
-        hidden_states = torch.zeros(
-            (values.size()[0], self.rnn_hidden_size), device=values.device
+    def fit(
+        self,
+        train_set: Union[dict, str],
+        val_set: Optional[Union[dict, str]] = None,
+        file_type: str = "h5py",
+    ) -> None:
+        # Step 1: wrap the input data with classes Dataset and DataLoader
+        training_set = DatasetForFEDformer(
+            train_set, return_X_ori=False, return_labels=False, file_type=file_type
         )
-        cell_states = torch.zeros(
-            (values.size()[0], self.rnn_hidden_size), device=values.device
+        training_loader = DataLoader(
+            training_set,
+            batch_size=self.batch_size,
+            shuffle=True,
+            num_workers=self.num_workers,
         )
+        val_loader = None
+        if val_set is not None:
+            if not check_X_ori_in_val_set(val_set):
+                raise ValueError("val_set must contain 'X_ori' for model validation.")
+            val_set = DatasetForFEDformer(
+                val_set, return_X_ori=True, return_labels=False, file_type=file_type
+            )
+            val_loader = DataLoader(
+                val_set,
+                batch_size=self.batch_size,
+                shuffle=False,
+                num_workers=self.num_workers,
+            )
 
-        estimations = []
-        reconstruction_loss = torch.tensor(0.0).to(values.device)
-
-        # imputation period
-        for t in range(self.n_steps):
-            # data shape: [batch, time, features]
-            x = values[:, t, :]  # values
-            m = masks[:, t, :]  # mask
-            d = deltas[:, t, :]  # delta, time gap
-
-            gamma_h = self.temp_decay_h(d)
-            gamma_x = self.temp_decay_x(d)
-
-            hidden_states = hidden_states * gamma_h  # decay hidden states
-            x_h = self.hist_reg(hidden_states)
-            reconstruction_loss += calc_mae(x_h, x, m)
-
-            x_c = m * x + (1 - m) * x_h
-
-            z_h = self.feat_reg(x_c)
-            reconstruction_loss += calc_mae(z_h, x, m)
-
-            alpha = torch.sigmoid(self.combining_weight(torch.cat([gamma_x, m], dim=1)))
-
-            c_h = alpha * z_h + (1 - alpha) * x_h
-            reconstruction_loss += calc_mae(c_h, x, m)
+        # Step 2: train the model and freeze it
+        self._train_model(training_loader, val_loader)
+        self.model.load_state_dict(self.best_model_dict)
+        self.model.eval()  # set the model as eval status to freeze it.
 
-            c_c = m * x + (1 - m) * c_h
-            estimations.append(c_h.unsqueeze(dim=1))
+        # Step 3: save the model if necessary
+        self._auto_save_model_if_necessary(confirm_saving=True)
 
-            inputs = torch.cat([c_c, m], dim=1)
-            hidden_states, cell_states = self.rnn_cell(
-                inputs, (hidden_states, cell_states)
-            )
-
-        estimations = torch.cat(estimations, dim=1)
-        imputed_data = masks * values + (1 - masks) * estimations
-        return imputed_data, estimations, hidden_states, reconstruction_loss
+    def predict(
+        self,
+        test_set: Union[dict, str],
+        file_type: str = "h5py",
+    ) -> dict:
+        """Make predictions for the input data with the trained model.
 
-    def forward(self, inputs: dict, direction: str = "forward") -> dict:
-        """Forward processing of the NN module.
         Parameters
         ----------
-        inputs :
-            The input data.
+        test_set : dict or str
+            The dataset for model validating, should be a dictionary including keys as 'X',
+            or a path string locating a data file supported by PyPOTS (e.g. h5 file).
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            which is time-series data for validating, can contain missing values, and y should be array-like of shape
+            [n_samples], which is classification labels of X.
+            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
+            key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
 
-        direction :
-            A keyword to extract data from parameter `data`.
+        file_type : str
+            The type of the given file if test_set is a path string.
 
         Returns
         -------
-        dict,
-            A dictionary includes all results.
+        result_dict : dict,
+            The dictionary containing the clustering results and latent variables if necessary.
 
         """
-        imputed_data, estimations, hidden_state, reconstruction_loss = self.impute(
-            inputs, direction
+        # Step 1: wrap the input data with classes Dataset and DataLoader
+        self.model.eval()  # set the model as eval status to freeze it.
+        test_set = BaseDataset(
+            test_set, return_X_ori=False, return_labels=False, file_type=file_type
         )
-        # for each iteration, reconstruction_loss increases its value for 3 times
-        reconstruction_loss /= self.n_steps * 3
+        test_loader = DataLoader(
+            test_set,
+            batch_size=self.batch_size,
+            shuffle=False,
+            num_workers=self.num_workers,
+        )
+        imputation_collector = []
 
-        ret_dict = {
-            "consistency_loss": torch.tensor(
-                0.0, device=imputed_data.device
-            ),  # single direction, has no consistency loss
-            "reconstruction_loss": reconstruction_loss,
-            "imputed_data": imputed_data,
-            "reconstructed_data": estimations,
-            "final_hidden_state": hidden_state,
+        # Step 2: process the data with the model
+        with torch.no_grad():
+            for idx, data in enumerate(test_loader):
+                inputs = self._assemble_input_for_testing(data)
+                results = self.model.forward(inputs, training=False)
+                imputation_collector.append(results["imputed_data"])
+
+        # Step 3: output collection and return
+        imputation = torch.cat(imputation_collector).cpu().detach().numpy()
+        result_dict = {
+            "imputation": imputation,
         }
-        return ret_dict
-
+        return result_dict
 
-class _BRITS(nn.Module):
-    """model BRITS: Bidirectional RITS
-    BRITS consists of two RITS, which take time-series data from two directions (forward/backward) respectively.
-
-    Attributes
-    ----------
-    n_steps :
-        sequence length (number of time steps)
-
-    n_features :
-        number of features (input dimensions)
-
-    rnn_hidden_size :
-        the hidden size of the RNN cell
-
-    rits_f: RITS object
-        the forward RITS model
-
-    rits_b: RITS object
-        the backward RITS model
-
-    """
-
-    def __init__(
+    def impute(
         self,
-        n_steps: int,
-        n_features: int,
-        rnn_hidden_size: int,
-        device: Union[str, torch.device],
-    ):
-        super().__init__()
-        # data settings
-        self.n_steps = n_steps
-        self.n_features = n_features
-        # imputer settings
-        self.rnn_hidden_size = rnn_hidden_size
-        # create models
-        self.rits_f = RITS(n_steps, n_features, rnn_hidden_size, device)
-        self.rits_b = RITS(n_steps, n_features, rnn_hidden_size, device)
-
-    @staticmethod
-    def _get_consistency_loss(
-        pred_f: torch.Tensor, pred_b: torch.Tensor
-    ) -> torch.Tensor:
-        """Calculate the consistency loss between the imputation from two RITS models.
+        X: Union[dict, str],
+        file_type="h5py",
+    ) -> np.ndarray:
+        """Impute missing values in the given data with the trained model.
+
+        Warnings
+        --------
+        The method impute is deprecated. Please use `predict()` instead.
 
         Parameters
         ----------
-        pred_f :
-            The imputation from the forward RITS.
-
-        pred_b :
-            The imputation from the backward RITS (already gets reverted).
-
-        Returns
-        -------
-        float tensor,
-            The consistency loss.
-
-        """
-        loss = torch.abs(pred_f - pred_b).mean() * 1e-1
-        return loss
+        X :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
 
-    @staticmethod
-    def _reverse(ret: dict) -> dict:
-        """Reverse the array values on the time dimension in the given dictionary.
-
-        Parameters
-        ----------
-        ret :
+        file_type :
+            The type of the given file if X is a path string.
 
         Returns
         -------
-        dict,
-            A dictionary contains values reversed on the time dimension from the given dict.
-
+        array-like, shape [n_samples, sequence length (time steps), n_features],
+            Imputed data.
         """
+        logger.warning(
+            "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
+        )
 
-        def reverse_tensor(tensor_):
-            if tensor_.dim() <= 1:
-                return tensor_
-            indices = range(tensor_.size()[1])[::-1]
-            indices = torch.tensor(
-                indices, dtype=torch.long, device=tensor_.device, requires_grad=False
-            )
-            return tensor_.index_select(1, indices)
-
-        for key in ret:
-            ret[key] = reverse_tensor(ret[key])
-
-        return ret
-
-    def forward(self, inputs: dict, training: bool = True) -> dict:
-        # Results from the forward RITS.
-        ret_f = self.rits_f(inputs, "forward")
-        # Results from the backward RITS.
-        ret_b = self._reverse(self.rits_b(inputs, "backward"))
-
-        imputed_data = (ret_f["imputed_data"] + ret_b["imputed_data"]) / 2
-        reconstructed_data = (
-            ret_f["reconstructed_data"] + ret_b["reconstructed_data"]
-        ) / 2
-
-        results = {
-            "imputed_data": imputed_data,
-        }
-
-        # if in training mode, return results with losses
-        if training:
-            consistency_loss = self._get_consistency_loss(
-                ret_f["imputed_data"], ret_b["imputed_data"]
-            )
-            results["consistency_loss"] = consistency_loss
-            loss = (
-                consistency_loss
-                + ret_f["reconstruction_loss"]
-                + ret_b["reconstruction_loss"]
-            )
-
-            # `loss` is always the item for backward propagating to update the model
-            results["loss"] = loss
-            results["reconstructed_data"] = reconstructed_data
-            results["f_reconstructed_data"] = ret_f["reconstructed_data"]
-            results["b_reconstructed_data"] = ret_b["reconstructed_data"]
-
-        return results
+        results_dict = self.predict(X, file_type=file_type)
+        return results_dict["imputation"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypots-0.4/pypots/imputation/brits/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/brits/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Variable
 from torch.nn.parameter import Parameter
 
 
 class FeatureRegression(nn.Module):
-    """The module used to capture the correlation between features for imputation.
+    """The module used to capture the correlation between features for imputation in BRITS.
 
     Attributes
     ----------
     W : tensor
         The weights (parameters) of the module.
 
     b : tensor
```

### Comparing `pypots-0.4/pypots/imputation/crossformer/data.py` & `pypots-0.4.1/pypots/imputation/crossformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/crossformer/model.py` & `pypots-0.4.1/pypots/imputation/crossformer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .data import DatasetForCrossformer
-from .modules.core import _Crossformer
+from pypots.imputation.crossformer.core import _Crossformer
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
@@ -63,14 +63,20 @@
 
     win_size :
         The window size for merging segment.
 
     dropout :
         The dropout rate for the model.
 
+    ORT_weight :
+        The weight for the ORT loss, the same as SAITS.
+
+    MIT_weight :
+        The weight for the MIT loss, the same as SAITS.
+
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
     patience :
@@ -116,14 +122,16 @@
         n_heads: int,
         d_model: int,
         d_ffn: int,
         factor: int,
         seg_len: int,
         win_size: int,
         dropout: float = 0,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -146,27 +154,31 @@
         self.n_heads = n_heads
         self.d_model = d_model
         self.d_ffn = d_ffn
         self.factor = factor
         self.seg_len = seg_len
         self.win_size = win_size
         self.dropout = dropout
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _Crossformer(
             self.n_steps,
             self.n_features,
             self.n_layers,
             self.n_heads,
             self.d_model,
             self.d_ffn,
             self.factor,
             self.seg_len,
             self.win_size,
             self.dropout,
+            self.ORT_weight,
+            self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/imputation/crossformer/modules/core.py` & `pypots-0.4.1/pypots/imputation/crossformer/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from math import ceil
 
 import torch
 import torch.nn as nn
 from einops import rearrange
 
-from .submodules import CrossformerEncoder, ScaleBlock
-from ...patchtst.modules.submodules import FlattenHead, PatchEmbedding
-from ....utils.metrics import calc_mse
+from ...nn.modules.crossformer import CrossformerEncoder, ScaleBlock
+from ...nn.modules.patchtst import PredictionHead, PatchEmbedding
+from ...nn.modules.saits import SaitsLoss
 
 
 class _Crossformer(nn.Module):
     def __init__(
         self,
         n_steps,
         n_features,
@@ -25,25 +25,25 @@
         n_heads,
         d_model,
         d_ffn,
         factor,
         seg_len,
         win_size,
         dropout,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
     ):
         super().__init__()
 
-        self.n_features = n_features
         self.d_model = d_model
 
         # The padding operation to handle invisible sgemnet length
         pad_in_len = ceil(1.0 * n_steps / seg_len) * seg_len
         in_seg_num = pad_in_len // seg_len
         out_seg_num = ceil(in_seg_num / (win_size ** (n_layers - 1)))
-        head_nf = d_model * out_seg_num
 
         # Embedding
         self.enc_value_embedding = PatchEmbedding(
             d_model,
             seg_len,
             seg_len,
             pad_in_len - n_steps,
@@ -67,45 +67,55 @@
                     in_seg_num if layer == 0 else ceil(in_seg_num / win_size**layer),
                     factor,
                 )
                 for layer in range(n_layers)
             ]
         )
 
-        self.head = FlattenHead(head_nf, n_steps, dropout)
+        self.head = PredictionHead(d_model, out_seg_num, n_steps, dropout)
         self.embedding = nn.Linear(n_features * 2, d_model)
         self.output_projection = nn.Linear(d_model, n_features)
 
+        # apply SAITS loss function to Crossformer on the imputation task
+        self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
+
     def forward(self, inputs: dict, training: bool = True) -> dict:
-        X, masks = inputs["X"], inputs["missing_mask"]
+        X, missing_mask = inputs["X"], inputs["missing_mask"]
 
         # WDU: the original Crossformer paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
         # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
         # embedding layers to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
         # embedding
-        input_X = self.embedding(torch.cat([X, masks], dim=2))
+        input_X = self.embedding(torch.cat([X, missing_mask], dim=2))
         x_enc = self.enc_value_embedding(input_X.permute(0, 2, 1))
-
-        # Crossformer processing
         x_enc = rearrange(
             x_enc, "(b d) seg_num d_model -> b d seg_num d_model", d=self.d_model
         )
         x_enc += self.enc_pos_embedding
+
+        # Crossformer processing
         x_enc = self.pre_norm(x_enc)
         enc_out, attns = self.encoder(x_enc)
         # project back the original data space
-        dec_out = self.head(enc_out[-1].permute(0, 1, 3, 2)).permute(0, 2, 1)
-        output = self.output_projection(dec_out)
+        enc_out = enc_out.permute(0, 1, 3, 2)
+        dec_out = self.head(enc_out)
+        reconstruction = self.output_projection(dec_out)
 
-        imputed_data = masks * X + (1 - masks) * output
+        imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
         results = {
             "imputed_data": imputed_data,
         }
 
+        # if in training mode, return results with losses
         if training:
+            X_ori, indicating_mask = inputs["X_ori"], inputs["indicating_mask"]
+            loss, ORT_loss, MIT_loss = self.saits_loss_func(
+                reconstruction, X_ori, missing_mask, indicating_mask
+            )
+            results["ORT_loss"] = ORT_loss
+            results["MIT_loss"] = MIT_loss
             # `loss` is always the item for backward propagating to update the model
-            loss = calc_mse(output, inputs["X_ori"], inputs["indicating_mask"])
             results["loss"] = loss
 
         return results
```

### Comparing `pypots-0.4/pypots/imputation/crossformer/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/crossformer/layers.py`

 * *Files 26% similar despite different names*

```diff
@@ -172,30 +172,14 @@
 
         for layer in self.encode_layers:
             x = layer(x)
 
         return x, None
 
 
-class CrossformerEncoder(nn.Module):
-    def __init__(self, attn_layers):
-        super().__init__()
-        self.encode_blocks = nn.ModuleList(attn_layers)
-
-    def forward(self, x):
-        encode_x = []
-        encode_x.append(x)
-
-        for block in self.encode_blocks:
-            x, attns = block(x)
-            encode_x.append(x)
-
-        return encode_x, None
-
-
 class CrossformerDecoderLayer(nn.Module):
     def __init__(
         self, self_attention, cross_attention, seg_len, d_model, d_ff=None, dropout=0.1
     ):
         super().__init__()
         self.self_attention = self_attention
         self.cross_attention = cross_attention
@@ -235,35 +219,7 @@
         )
         layer_predict = self.linear_pred(dec_output)
         layer_predict = rearrange(
             layer_predict, "b out_d seg_num seg_len -> b (out_d seg_num) seg_len"
         )
 
         return dec_output, layer_predict
-
-
-class CrossformerDecoder(nn.Module):
-    def __init__(self, layers):
-        super().__init__()
-        self.decode_layers = nn.ModuleList(layers)
-
-    def forward(self, x, cross):
-        final_predict = None
-        i = 0
-
-        ts_d = x.shape[1]
-        for layer in self.decode_layers:
-            cross_enc = cross[i]
-            x, layer_predict = layer(x, cross_enc)
-            if final_predict is None:
-                final_predict = layer_predict
-            else:
-                final_predict = final_predict + layer_predict
-            i += 1
-
-        final_predict = rearrange(
-            final_predict,
-            "b (out_d seg_num) seg_len -> b (seg_num seg_len) out_d",
-            out_d=ts_d,
-        )
-
-        return final_predict
```

### Comparing `pypots-0.4/pypots/imputation/csdi/data.py` & `pypots-0.4.1/pypots/imputation/csdi/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/csdi/model.py` & `pypots-0.4.1/pypots/imputation/csdi/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from torch.utils.data import DataLoader
 
 try:
     import nni
 except ImportError:
     pass
 
+from .core import _CSDI
 from .data import DatasetForCSDI, TestDatasetForCSDI
-from .modules import _CSDI
 from ..base import BaseNNImputer
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
```

### Comparing `pypots-0.4/pypots/imputation/csdi/modules/core.py` & `pypots-0.4.1/pypots/nn/modules/csdi/backbone.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+"""
+
+"""
+
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from .submodules import DiffusionModel
+from .layers import CsdiDiffusionModel
 
 
-class _CSDI(nn.Module):
+class BackboneCSDI(nn.Module):
     def __init__(
         self,
         n_layers,
         n_heads,
         n_channels,
         d_target,
         d_time_embedding,
@@ -37,19 +41,19 @@
         if self.is_unconditional:
             d_input = 1
         else:
             d_side += 1  # for conditional mask
             d_input = 2
 
         self.embed_layer = nn.Embedding(
-            num_embeddings=self.d_target,
-            embedding_dim=self.d_feature_embedding,
+            num_embeddings=d_target,
+            embedding_dim=d_feature_embedding,
         )
 
-        self.diff_model = DiffusionModel(
+        self.diff_model = CsdiDiffusionModel(
             n_diffusion_steps,
             d_diffusion_embedding,
             d_input,
             d_side,
             n_channels,
             n_heads,
             n_layers,
@@ -105,14 +109,24 @@
 
         if not self.is_unconditional:
             side_mask = cond_mask.unsqueeze(1)  # (B,1,K,L)
             side_info = torch.cat([side_info, side_mask], dim=1)
 
         return side_info
 
+    def set_input_to_diffmodel(self, noisy_data, observed_data, cond_mask):
+        if self.is_unconditional:
+            total_input = noisy_data.unsqueeze(1)  # (B,1,K,L)
+        else:
+            cond_obs = (cond_mask * observed_data).unsqueeze(1)
+            noisy_target = ((1 - cond_mask) * noisy_data).unsqueeze(1)
+            total_input = torch.cat([cond_obs, noisy_target], dim=1)  # (B,2,K,L)
+
+        return total_input
+
     def calc_loss_valid(
         self, observed_data, cond_mask, indicating_mask, side_info, is_train
     ):
         loss_sum = 0
         for t in range(self.n_diffusion_steps):  # calculate loss for all t
             loss = self.calc_loss(
                 observed_data, cond_mask, indicating_mask, side_info, is_train, set_t=t
@@ -142,25 +156,15 @@
 
         target_mask = indicating_mask
         residual = (noise - predicted) * target_mask
         num_eval = target_mask.sum()
         loss = (residual**2).sum() / (num_eval if num_eval > 0 else 1)
         return loss
 
-    def set_input_to_diffmodel(self, noisy_data, observed_data, cond_mask):
-        if self.is_unconditional:
-            total_input = noisy_data.unsqueeze(1)  # (B,1,K,L)
-        else:
-            cond_obs = (cond_mask * observed_data).unsqueeze(1)
-            noisy_target = ((1 - cond_mask) * noisy_data).unsqueeze(1)
-            total_input = torch.cat([cond_obs, noisy_target], dim=1)  # (B,2,K,L)
-
-        return total_input
-
-    def impute(self, observed_data, cond_mask, side_info, n_sampling_times):
+    def forward(self, observed_data, cond_mask, side_info, n_sampling_times):
         B, K, L = observed_data.shape
         device = observed_data.device
         imputed_samples = torch.zeros(B, n_sampling_times, K, L).to(device)
 
         for i in range(n_sampling_times):
             # generate noisy observation for unconditional model
             if self.is_unconditional:
@@ -199,53 +203,7 @@
                     sigma = (
                         (1.0 - self.alpha[t - 1]) / (1.0 - self.alpha[t]) * self.beta[t]
                     ) ** 0.5
                     current_sample += sigma * noise
 
             imputed_samples[:, i] = current_sample.detach()
         return imputed_samples
-
-    def forward(self, inputs, training=True, n_sampling_times=1):
-        results = {}
-        if training:  # for training
-            (observed_data, indicating_mask, cond_mask, observed_tp) = (
-                inputs["X_ori"],
-                inputs["indicating_mask"],
-                inputs["cond_mask"],
-                inputs["observed_tp"],
-            )
-            side_info = self.get_side_info(observed_tp, cond_mask)
-            training_loss = self.calc_loss(
-                observed_data, cond_mask, indicating_mask, side_info, training
-            )
-            results["loss"] = training_loss
-        elif not training and n_sampling_times == 0:  # for validating
-            (observed_data, indicating_mask, cond_mask, observed_tp) = (
-                inputs["X_ori"],
-                inputs["indicating_mask"],
-                inputs["cond_mask"],
-                inputs["observed_tp"],
-            )
-            side_info = self.get_side_info(observed_tp, cond_mask)
-            validating_loss = self.calc_loss_valid(
-                observed_data, cond_mask, indicating_mask, side_info, training
-            )
-            results["loss"] = validating_loss
-        elif not training and n_sampling_times > 0:  # for testing
-            observed_data, cond_mask, observed_tp = (
-                inputs["X"],
-                inputs["cond_mask"],
-                inputs["observed_tp"],
-            )
-            side_info = self.get_side_info(observed_tp, cond_mask)
-            samples = self.impute(
-                observed_data, cond_mask, side_info, n_sampling_times
-            )  # (n_samples, n_sampling_times, n_features, n_steps)
-            repeated_obs = observed_data.unsqueeze(1).repeat(1, n_sampling_times, 1, 1)
-            repeated_mask = cond_mask.unsqueeze(1).repeat(1, n_sampling_times, 1, 1)
-            imputed_data = repeated_obs + samples * (1 - repeated_mask)
-
-            results["imputed_data"] = imputed_data.permute(
-                0, 1, 3, 2
-            )  # (n_samples, n_sampling_times, n_steps, n_features)
-
-        return results
```

### Comparing `pypots-0.4/pypots/imputation/csdi/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/csdi/layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def conv1d_with_init(in_channels, out_channels, kernel_size):
     layer = nn.Conv1d(in_channels, out_channels, kernel_size)
     nn.init.kaiming_normal_(layer.weight)
     return layer
 
 
-class DiffusionEmbedding(nn.Module):
+class CsdiDiffusionEmbedding(nn.Module):
     def __init__(self, n_diffusion_steps, d_embedding=128, d_projection=None):
         super().__init__()
         if d_projection is None:
             d_projection = d_embedding
         self.register_buffer(
             "embedding",
             self._build_embedding(n_diffusion_steps, d_embedding // 2),
@@ -55,15 +55,15 @@
         x = self.projection1(x)
         x = F.silu(x)
         x = self.projection2(x)
         x = F.silu(x)
         return x
 
 
-class ResidualBlock(nn.Module):
+class CsdiResidualBlock(nn.Module):
     def __init__(self, d_side, n_channels, diffusion_embedding_dim, nheads):
         super().__init__()
         self.diffusion_projection = nn.Linear(diffusion_embedding_dim, n_channels)
         self.cond_projection = conv1d_with_init(d_side, 2 * n_channels, 1)
         self.mid_projection = conv1d_with_init(n_channels, 2 * n_channels, 1)
         self.output_projection = conv1d_with_init(n_channels, 2 * n_channels, 1)
 
@@ -116,38 +116,38 @@
         residual, skip = torch.chunk(y, 2, dim=1)
         x = x.reshape(base_shape)
         residual = residual.reshape(base_shape)
         skip = skip.reshape(base_shape)
         return (x + residual) / math.sqrt(2.0), skip
 
 
-class DiffusionModel(nn.Module):
+class CsdiDiffusionModel(nn.Module):
     def __init__(
         self,
         n_diffusion_steps,
         d_diffusion_embedding,
         d_input,
         d_side,
         n_channels,
         n_heads,
         n_layers,
     ):
         super().__init__()
-        self.diffusion_embedding = DiffusionEmbedding(
+        self.diffusion_embedding = CsdiDiffusionEmbedding(
             n_diffusion_steps=n_diffusion_steps,
             d_embedding=d_diffusion_embedding,
         )
         self.input_projection = conv1d_with_init(d_input, n_channels, 1)
         self.output_projection1 = conv1d_with_init(n_channels, n_channels, 1)
         self.output_projection2 = conv1d_with_init(n_channels, 1, 1)
         nn.init.zeros_(self.output_projection2.weight)
 
         self.residual_layers = nn.ModuleList(
             [
-                ResidualBlock(
+                CsdiResidualBlock(
                     d_side=d_side,
                     n_channels=n_channels,
                     diffusion_embedding_dim=d_diffusion_embedding,
                     nheads=n_heads,
                 )
                 for _ in range(n_layers)
             ]
```

### Comparing `pypots-0.4/pypots/imputation/dlinear/data.py` & `pypots-0.4.1/pypots/imputation/dlinear/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/dlinear/model.py` & `pypots-0.4.1/pypots/imputation/dlinear/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .data import DatasetForDLinear
-from .modules.core import _DLinear
+from pypots.imputation.dlinear.core import _DLinear
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
@@ -49,14 +49,20 @@
     individual :
         Whether to make a linear layer for each variate/channel/feature individually.
 
     d_model:
         The dimension of the space in which the time-series data will be embedded and modeled.
         It is necessary only for DLinear in the non-individual mode.
 
+    ORT_weight :
+        The weight for the ORT loss, the same as SAITS.
+
+    MIT_weight :
+        The weight for the MIT loss, the same as SAITS.
+
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
     patience :
@@ -97,14 +103,16 @@
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         moving_avg_window_size: int,
         individual: bool = False,
         d_model: Optional[int] = None,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -122,22 +130,26 @@
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
         self.moving_avg_window_size = moving_avg_window_size
         self.individual = individual
         self.d_model = d_model
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _DLinear(
-            n_steps,
-            n_features,
-            moving_avg_window_size,
-            individual,
-            d_model,
+            self.n_steps,
+            self.n_features,
+            self.moving_avg_window_size,
+            self.individual,
+            self.d_model,
+            self.ORT_weight,
+            self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/imputation/etsformer/data.py` & `pypots-0.4.1/pypots/imputation/etsformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/etsformer/model.py` & `pypots-0.4.1/pypots/imputation/etsformer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .data import DatasetForETSformer
-from .modules.core import _ETSformer
+from pypots.imputation.etsformer.core import _ETSformer
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
@@ -59,14 +59,20 @@
 
     top_k :
         Top-K Fourier bases.
 
     dropout :
         The dropout rate for the model.
 
+    ORT_weight :
+        The weight for the ORT loss, the same as SAITS.
+
+    MIT_weight :
+        The weight for the MIT loss, the same as SAITS.
+
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
     patience :
@@ -111,14 +117,16 @@
         n_e_layers,
         n_d_layers,
         n_heads,
         d_model,
         d_ffn,
         top_k,
         dropout: float = 0,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -140,26 +148,30 @@
         self.n_heads = n_heads
         self.n_e_layers = n_e_layers
         self.n_d_layers = n_d_layers
         self.d_model = d_model
         self.d_ffn = d_ffn
         self.dropout = dropout
         self.top_k = top_k
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _ETSformer(
             self.n_steps,
             self.n_features,
             self.n_e_layers,
             self.n_d_layers,
             self.n_heads,
             self.d_model,
             self.d_ffn,
             self.dropout,
             self.top_k,
+            self.ORT_weight,
+            self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/imputation/etsformer/modules/core.py` & `pypots-0.4.1/pypots/imputation/etsformer/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import torch
 import torch.nn as nn
 
-from .submodules import (
+from ...nn.modules.etsformer import (
     ETSformerEncoderLayer,
     ETSformerEncoder,
     ETSformerDecoderLayer,
     ETSformerDecoder,
 )
-from ....nn.modules.transformer.embedding import DataEmbedding
-from ....utils.metrics import calc_mse
+from ...nn.modules.saits import SaitsLoss
+from ...nn.modules.transformer.embedding import DataEmbedding
 
 
 class _ETSformer(nn.Module):
     def __init__(
         self,
         n_steps,
         n_features,
         n_e_layers,
         n_d_layers,
         n_heads,
         d_model,
         d_ffn,
         dropout,
         top_k,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         activation="sigmoid",
     ):
         super().__init__()
 
-        self.n_steps = n_steps
-
         self.enc_embedding = DataEmbedding(
             n_features * 2,
             d_model,
             dropout=dropout,
         )
 
         # Encoder
@@ -68,38 +68,46 @@
                     n_features,
                     n_steps,
                     dropout=dropout,
                 )
                 for _ in range(n_d_layers)
             ],
         )
-        # self.transform = Transform(sigma=0.2)  # for forecasting
+
+        # apply SAITS loss function to ETSformer on the imputation task
+        self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
-        X, masks = inputs["X"], inputs["missing_mask"]
+        X, missing_mask = inputs["X"], inputs["missing_mask"]
 
         # WDU: the original ETSformer paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
         # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
         # embedding layers to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
 
         # the same as SAITS, concatenate the time series data and the missing mask for embedding
-        input_X = torch.cat([X, masks], dim=2)
+        input_X = torch.cat([X, missing_mask], dim=2)
         res = self.enc_embedding(input_X)
 
         # ETSformer encoder processing
         level, growths, seasons = self.encoder(res, X, attn_mask=None)
         growth, season = self.decoder(growths, seasons)
-        output = level[:, -1:] + growth + season
+        reconstruction = level[:, -1:] + growth + season
 
-        imputed_data = masks * X + (1 - masks) * output
+        imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
         results = {
             "imputed_data": imputed_data,
         }
 
+        # if in training mode, return results with losses
         if training:
+            X_ori, indicating_mask = inputs["X_ori"], inputs["indicating_mask"]
+            loss, ORT_loss, MIT_loss = self.saits_loss_func(
+                reconstruction, X_ori, missing_mask, indicating_mask
+            )
+            results["ORT_loss"] = ORT_loss
+            results["MIT_loss"] = MIT_loss
             # `loss` is always the item for backward propagating to update the model
-            loss = calc_mse(output, inputs["X_ori"], inputs["indicating_mask"])
             results["loss"] = loss
 
         return results
```

### Comparing `pypots-0.4/pypots/imputation/etsformer/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/etsformer/layers.py`

 * *Files 8% similar despite different names*

```diff
@@ -266,30 +266,14 @@
         return self.dropout1(x)
 
     def _season_block(self, x):
         x = self.seasonal_layer(x)
         return self.dropout2(x)
 
 
-class ETSformerEncoder(nn.Module):
-    def __init__(self, layers):
-        super().__init__()
-        self.layers = nn.ModuleList(layers)
-
-    def forward(self, res, level, attn_mask=None):
-        growths = []
-        seasons = []
-        for layer in self.layers:
-            res, level, growth, season = layer(res, level, attn_mask=None)
-            growths.append(growth)
-            seasons.append(season)
-
-        return level, growths, seasons
-
-
 class DampingLayer(nn.Module):
     def __init__(self, pred_len, nhead, dropout=0.1):
         super().__init__()
         self.pred_len = pred_len
         self.nhead = nhead
         self._damping_factor = nn.Parameter(torch.randn(1, nhead))
         self.dropout = nn.Dropout(dropout)
@@ -324,31 +308,7 @@
 
     def forward(self, growth, season):
         growth_horizon = self.growth_damping(growth[:, -1:])
         growth_horizon = self.dropout1(growth_horizon)
 
         seasonal_horizon = season[:, -self.pred_len :]
         return growth_horizon, seasonal_horizon
-
-
-class ETSformerDecoder(nn.Module):
-    def __init__(self, layers):
-        super().__init__()
-        self.d_model = layers[0].d_model
-        self.c_out = layers[0].c_out
-        self.pred_len = layers[0].pred_len
-        self.nhead = layers[0].nhead
-
-        self.layers = nn.ModuleList(layers)
-        self.pred = nn.Linear(self.d_model, self.c_out)
-
-    def forward(self, growths, seasons):
-        growth_repr = []
-        season_repr = []
-
-        for idx, layer in enumerate(self.layers):
-            growth_horizon, season_horizon = layer(growths[idx], seasons[idx])
-            growth_repr.append(growth_horizon)
-            season_repr.append(season_horizon)
-        growth_repr = sum(growth_repr)
-        season_repr = sum(season_repr)
-        return self.pred(growth_repr), self.pred(season_repr)
```

### Comparing `pypots-0.4/pypots/imputation/fedformer/__init__.py` & `pypots-0.4.1/pypots/imputation/fedformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/fedformer/data.py` & `pypots-0.4.1/pypots/imputation/fedformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/fedformer/model.py` & `pypots-0.4.1/pypots/imputation/timesnet/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,73 @@
 """
-The implementation of FEDformer for the partially-observed time-series imputation task.
+The implementation of TimesNet for the partially-observed time-series imputation task.
 
-Refer to the paper "Tian Zhou, Ziqing Ma, Qingsong Wen, Xue Wang, Liang Sun, and Rong Jin.
-FEDformer: Frequency enhanced decomposed transformer for long-term series forecasting.
-In ICML, volume 162 of Proceedings of Machine Learning Research, pages 27268–27286. PMLR, 17–23 Jul 2022.".
+Refer to the paper "Haixu Wu, Tengge Hu, Yong Liu, Hang Zhou, Jianmin Wang, and Mingsheng Long.
+TimesNet: Temporal 2D-Variation Modeling for General Time Series Analysis.
+In ICLR, 2023."
 
 Notes
 -----
-Partial implementation uses code from https://github.com/MAZiqing/FEDformer
+Partial implementation uses code from https://github.com/thuml/Time-Series-Library.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .data import DatasetForFEDformer
-from .modules.core import _FEDformer
+from .core import _TimesNet
+from .data import DatasetForTimesNet
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
-class FEDformer(BaseNNImputer):
-    """The PyTorch implementation of the FEDformer model.
-    FEDformer is originally proposed by Woo et al. in :cite:`zhou2022fedformer`.
+class TimesNet(BaseNNImputer):
+    """The PyTorch implementation of the TimesNet model.
+    TimesNet is originally proposed by Wu et al. in :cite:`wu2023timesnet`.
 
     Parameters
     ----------
     n_steps :
         The number of time steps in the time-series data sample.
 
     n_features :
         The number of features in the time-series data sample.
 
     n_layers :
-        The number of layers in the FEDformer.
+        The number of layers in the TimesNet model.
 
-    n_heads :
-        The number of heads in the multi-head attention mechanism.
+    top_k :
+        The number of top-k amplitude values to be selected to  obtain the most significant frequencies.
 
     d_model :
         The dimension of the model.
 
     d_ffn :
         The dimension of the feed-forward network.
 
-    moving_avg_window_size :
-        The window size of moving average.
+    n_kernels :
+        The number of 2D kernels (2D convolutional layers) to use in the submodule InceptionBlockV1.
 
     dropout :
         The dropout rate for the model.
 
-    version :
-        The version of the model. It has to be one of ["Wavelets", "Fourier"].
-        The default value is "Fourier".
-
-    modes :
-        The number of modes to be selected. The default value is 32.
-
-    mode_select :
-        Get modes on frequency domain. It has to "random" or "low". The default value is "random".
-        'random' means sampling randomly; 'low' means sampling the lowest modes;
+    apply_nonstationary_norm :
+        Whether to apply non-stationary normalization to the input data for TimesNet.
+        Please refer to :cite:`liu2022nonstationary` for details about non-stationary normalization,
+        which is not the idea of the original TimesNet paper. Hence, we make it optional and default not to use here.
 
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
@@ -110,25 +104,23 @@
         better than in previous epochs.
         The "all" strategy will save every model after each epoch training.
 
     """
 
     def __init__(
         self,
-        n_steps,
-        n_features,
-        n_layers,
-        n_heads,
-        d_model,
-        d_ffn,
-        moving_avg_window_size,
+        n_steps: int,
+        n_features: int,
+        n_layers: int,
+        top_k: int,
+        d_model: int,
+        d_ffn: int,
+        n_kernels: int,
         dropout: float = 0,
-        version="Fourier",
-        modes=32,
-        mode_select="random",
+        apply_nonstationary_norm: bool = False,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -144,36 +136,32 @@
             model_saving_strategy,
         )
 
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
         self.n_layers = n_layers
-        self.n_heads = n_heads
+        self.top_k = top_k
         self.d_model = d_model
         self.d_ffn = d_ffn
-        self.modes = modes
-        self.mode_select = mode_select
-        self.moving_avg_window_size = moving_avg_window_size
+        self.n_kernels = n_kernels
         self.dropout = dropout
-        self.version = version
+        self.apply_nonstationary_norm = apply_nonstationary_norm
 
         # set up the model
-        self.model = _FEDformer(
+        self.model = _TimesNet(
+            self.n_layers,
             self.n_steps,
             self.n_features,
-            self.n_layers,
-            self.n_heads,
+            self.top_k,
             self.d_model,
             self.d_ffn,
-            self.moving_avg_window_size,
+            self.n_kernels,
             self.dropout,
-            self.version,
-            self.modes,
-            self.mode_select,
+            self.apply_nonstationary_norm,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
@@ -212,28 +200,28 @@
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForFEDformer(
+        training_set = DatasetForTimesNet(
             train_set, return_X_ori=False, return_labels=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
             if not check_X_ori_in_val_set(val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
-            val_set = DatasetForFEDformer(
+            val_set = DatasetForTimesNet(
                 val_set, return_X_ori=True, return_labels=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
```

### Comparing `pypots-0.4/pypots/imputation/fedformer/modules/core.py` & `pypots-0.4.1/pypots/classification/raindrop/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,127 @@
 """
+The implementation of Raindrop for the partially-observed time-series classification task.
+
+Refer to the paper "Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022).
+Graph-Guided Network for Irregularly Sampled Multivariate Time Series. ICLR 2022."
 
 """
 
+
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
+
 import torch
 import torch.nn as nn
+import torch.nn.functional as F
 
-from .submodules import MultiWaveletTransform, FourierBlock
-from ...autoformer.modules.submodules import (
-    AutoformerEncoderLayer,
-    AutoCorrelationLayer,
-    SeasonalLayerNorm,
-)
-from ...informer.modules.submodules import InformerEncoder
-from ....nn.modules.transformer.embedding import DataEmbedding
-from ....utils.metrics import calc_mse
+from ...nn.modules.raindrop import BackboneRaindrop
 
 
-class _FEDformer(nn.Module):
+class _Raindrop(nn.Module):
     def __init__(
         self,
-        n_steps,
         n_features,
         n_layers,
-        n_heads,
         d_model,
         d_ffn,
-        moving_avg_window_size,
-        dropout,
-        version="Fourier",
-        modes=32,
-        mode_select="random",
-        activation="relu",
+        n_heads,
+        n_classes,
+        dropout=0.3,
+        max_len=215,
+        d_static=9,
+        aggregation="mean",
+        sensor_wise_mask=False,
+        static=False,
     ):
         super().__init__()
 
-        self.enc_embedding = DataEmbedding(
-            n_features * 2,
+        d_pe = 16
+        self.aggregation = aggregation
+        self.sensor_wise_mask = sensor_wise_mask
+
+        self.backbone = BackboneRaindrop(
+            n_features,
+            n_layers,
             d_model,
-            dropout=dropout,
+            d_ffn,
+            n_heads,
+            n_classes,
+            dropout,
+            max_len,
+            d_static,
+            d_pe,
+            aggregation,
+            sensor_wise_mask,
+            static,
         )
 
-        if version == "Wavelets":
-            encoder_self_att = MultiWaveletTransform(ich=d_model, L=1, base="legendre")
-        elif version == "Fourier":
-            encoder_self_att = FourierBlock(
-                in_channels=d_model,
-                out_channels=d_model,
-                seq_len=n_steps,
-                modes=modes,
-                mode_select_method=mode_select,
-            )
+        if static:
+            d_final = d_model + n_features
         else:
-            raise ValueError(
-                f"Unsupported version: {version}. Please choose from ['Wavelets', 'Fourier']."
-            )
+            d_final = d_model + d_pe
 
-        self.encoder = InformerEncoder(
-            [
-                AutoformerEncoderLayer(
-                    AutoCorrelationLayer(
-                        encoder_self_att,  # instead of multi-head attention in transformer
-                        d_model,
-                        n_heads,
-                    ),
-                    d_model,
-                    d_ffn,
-                    moving_avg_window_size,
-                    dropout,
-                    activation,
-                )
-                for _ in range(n_layers)
-            ],
-            norm_layer=SeasonalLayerNorm(d_model),
+        self.mlp_static = nn.Sequential(
+            nn.Linear(d_final, d_final),
+            nn.ReLU(),
+            nn.Linear(d_final, n_classes),
         )
-        self.output_projection = nn.Linear(d_model, n_features)
 
-    def forward(self, inputs: dict, training: bool = True) -> dict:
-        X, masks = inputs["X"], inputs["missing_mask"]
+    def forward(self, inputs, training=True):
+        X, missing_mask, static, timestamps, lengths = (
+            inputs["X"],
+            inputs["missing_mask"],
+            inputs["static"],
+            inputs["timestamps"],
+            inputs["lengths"],
+        )
+        device = X.device
+        batch_size = X.shape[1]
 
-        # WDU: the original FEDformer paper isn't proposed for imputation task. Hence the model doesn't take
-        # the missing mask into account, which means, in the process, the model doesn't know which part of
-        # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
-        # embedding layers to project the concatenation of features and masks into a hidden space, as well as
-        # the output layers to project back from the hidden space to the original space.
-
-        # the same as SAITS, concatenate the time series data and the missing mask for embedding
-        input_X = torch.cat([X, masks], dim=2)
-        enc_out = self.enc_embedding(input_X)
-
-        # FEDformer encoder processing
-        enc_out, attns = self.encoder(enc_out)
-        output = self.output_projection(enc_out)
-
-        imputed_data = masks * X + (1 - masks) * output
-        results = {
-            "imputed_data": imputed_data,
-        }
+        representation, mask = self.backbone(
+            X,
+            timestamps,
+            lengths,
+        )
+
+        lengths2 = lengths.unsqueeze(1).to(device)
+        mask2 = mask.permute(1, 0).unsqueeze(2).long()
+        if self.sensor_wise_mask:
+            output = torch.zeros(
+                [batch_size, self.n_features, self.d_ob + 16], device=device
+            )
+            extended_missing_mask = missing_mask.view(-1, batch_size, self.n_features)
+            for se in range(self.n_features):
+                representation = representation.view(
+                    -1, batch_size, self.n_features, (self.d_ob + 16)
+                )
+                out = representation[:, :, se, :]
+                l_ = torch.sum(extended_missing_mask[:, :, se], dim=0).unsqueeze(
+                    1
+                )  # length
+                out_sensor = torch.sum(
+                    out * (1 - extended_missing_mask[:, :, se].unsqueeze(-1)), dim=0
+                ) / (l_ + 1)
+                output[:, se, :] = out_sensor
+            output = output.view([-1, self.n_features * (self.d_ob + 16)])
+        elif self.aggregation == "mean":
+            output = torch.sum(representation * (1 - mask2), dim=0) / (lengths2 + 1)
+        else:
+            raise RuntimeError
+
+        if static is not None:
+            emb = self.static_emb(static)
+            output = torch.cat([output, emb], dim=1)
 
+        logits = self.mlp_static(output)
+        classification_pred = torch.softmax(logits, dim=1)
+        results = {"classification_pred": classification_pred}
+
+        # if in training mode, return results with losses
         if training:
-            # `loss` is always the item for backward propagating to update the model
-            loss = calc_mse(output, inputs["X_ori"], inputs["indicating_mask"])
-            results["loss"] = loss
+            classification_loss = F.nll_loss(
+                torch.log(classification_pred), inputs["label"]
+            )
+            results["loss"] = classification_loss
 
         return results
```

### Comparing `pypots-0.4/pypots/imputation/fedformer/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/fedformer/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/gpvae/__init__.py` & `pypots-0.4.1/pypots/imputation/gpvae/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/gpvae/data.py` & `pypots-0.4.1/pypots/imputation/gpvae/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/gpvae/model.py` & `pypots-0.4.1/pypots/imputation/gpvae/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 try:
     import nni
 except ImportError:
     pass
 
 
+from .core import _GPVAE
 from .data import DatasetForGPVAE
-from .modules import _GPVAE
 from ..base import BaseNNImputer
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 from ...utils.metrics import calc_mse
```

### Comparing `pypots-0.4/pypots/imputation/gpvae/modules/core.py` & `pypots-0.4.1/pypots/nn/modules/gpvae/backbone.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 """
-The implementation of GP-VAE for the partially-observed time-series imputation task.
-
-Refer to the paper Fortuin V, Baranchuk D, Rätsch G, et al.
-GP-VAE: Deep probabilistic time series imputation. AISTATS. PMLR, 2020: 1651-1661.
 
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from .submodules import (
-    Encoder,
+from .layers import (
+    GpvaeEncoder,
     rbf_kernel,
     diffusion_kernel,
     matern_kernel,
     cauchy_kernel,
-    Decoder,
+    GpvaeDecoder,
 )
 
 
-class _GPVAE(nn.Module):
+class BackboneGPVAE(nn.Module):
     """model GPVAE with Gaussian Process prior
 
     Parameters
     ----------
     input_dim : int,
         the feature dimension of the input
 
@@ -88,16 +84,16 @@
         self.length_scale = length_scale
         self.kernel_scales = kernel_scales
 
         self.input_dim = input_dim
         self.time_length = time_length
         self.latent_dim = latent_dim
         self.beta = beta
-        self.encoder = Encoder(input_dim, latent_dim, encoder_sizes, window_size)
-        self.decoder = Decoder(latent_dim, input_dim, decoder_sizes)
+        self.encoder = GpvaeEncoder(input_dim, latent_dim, encoder_sizes, window_size)
+        self.decoder = GpvaeDecoder(latent_dim, input_dim, decoder_sizes)
         self.M = M
         self.K = K
 
         self.prior = None
 
     def encode(self, x):
         return self.encoder(x)
@@ -152,61 +148,53 @@
         assert len(kernel_matrix_tiled) == self.latent_dim
         prior = torch.distributions.MultivariateNormal(
             loc=torch.zeros(self.latent_dim, self.time_length, device=device),
             covariance_matrix=kernel_matrix_tiled.to(device),
         )
         return prior
 
-    def forward(self, inputs, training=True, n_sampling_times=1):
-        x = inputs["X"]
-        n_samples, n_steps, n_features = x.shape
-        m_mask = inputs["missing_mask"]
-
-        results = {}
-        if training:
-            x = x.repeat(self.K * self.M, 1, 1)
-            m_mask = m_mask.repeat(self.K * self.M, 1, 1).type(torch.bool)
-
-            if self.prior is None:
-                self.prior = self._init_prior(device=x.device)
-
-            qz_x = self.encode(x)
-            z = qz_x.rsample()
-            px_z = self.decode(z)
-            nll = -px_z.log_prob(x)
-            nll = torch.where(torch.isfinite(nll), nll, torch.zeros_like(nll))
-            if m_mask is not None:
-                nll = torch.where(m_mask, nll, torch.zeros_like(nll))
-            nll = nll.sum(dim=(1, 2))
-
-            if self.K > 1:
-                kl = qz_x.log_prob(z) - self.prior.log_prob(z)
-                kl = torch.where(torch.isfinite(kl), kl, torch.zeros_like(kl))
-                kl = kl.sum(1)
+    def impute(self, X, missing_mask, n_sampling_times=1):
+        n_samples, n_steps, n_features = X.shape
+        X = X.repeat(n_sampling_times, 1, 1)
+        missing_mask = missing_mask.repeat(n_sampling_times, 1, 1).type(torch.bool)
+        decode_x_mean = self.decode(self.encode(X).mean).mean
+        imputed_data = decode_x_mean * ~missing_mask + X * missing_mask
+        imputed_data = imputed_data.reshape(
+            n_sampling_times, n_samples, n_steps, n_features
+        ).permute(1, 0, 2, 3)
+        return imputed_data
+
+    def forward(self, X, missing_mask):
+        X = X.repeat(self.K * self.M, 1, 1)
+        missing_mask = missing_mask.repeat(self.K * self.M, 1, 1).type(torch.bool)
+
+        if self.prior is None:
+            self.prior = self._init_prior(device=X.device)
+
+        qz_x = self.encode(X)
+        z = qz_x.rsample()
+        px_z = self.decode(z)
+        nll = -px_z.log_prob(X)
+        nll = torch.where(torch.isfinite(nll), nll, torch.zeros_like(nll))
+        if missing_mask is not None:
+            nll = torch.where(missing_mask, nll, torch.zeros_like(nll))
+        nll = nll.sum(dim=(1, 2))
+
+        if self.K > 1:
+            kl = qz_x.log_prob(z) - self.prior.log_prob(z)
+            kl = torch.where(torch.isfinite(kl), kl, torch.zeros_like(kl))
+            kl = kl.sum(1)
 
-                weights = -nll - kl
-                weights = torch.reshape(weights, [self.M, self.K, -1])
+            weights = -nll - kl
+            weights = torch.reshape(weights, [self.M, self.K, -1])
 
-                elbo = torch.logsumexp(weights, dim=1)
-                elbo = elbo.mean()
-            else:
-                kl = self.kl_divergence(qz_x, self.prior)
-                kl = torch.where(torch.isfinite(kl), kl, torch.zeros_like(kl))
-                kl = kl.sum(1)
-
-                elbo = -nll - self.beta * kl
-                elbo = elbo.mean()
-            results["loss"] = -elbo.mean()
+            elbo = torch.logsumexp(weights, dim=1)
+            elbo = elbo.mean()
         else:
-            x = x.repeat(n_sampling_times, 1, 1)
-            m_mask = m_mask.repeat(n_sampling_times, 1, 1).type(torch.bool)
-            decode_x_mean = self.decode(self.encode(x).mean).mean
-            imputed_data = decode_x_mean * ~m_mask + x * m_mask
-            imputed_data = imputed_data.reshape(
-                n_sampling_times, n_samples, n_steps, n_features
-            ).permute(1, 0, 2, 3)
-
-            results = {
-                "imputed_data": imputed_data,
-            }
+            kl = self.kl_divergence(qz_x, self.prior)
+            kl = torch.where(torch.isfinite(kl), kl, torch.zeros_like(kl))
+            kl = kl.sum(1)
+
+            elbo = -nll - self.beta * kl
+            elbo = elbo.mean()
 
-        return results
+        return -elbo
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4/pypots/imputation/gpvae/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/gpvae/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,8 @@
 """
-The implementation of GP-VAE for the partially-observed time-series imputation task.
-
-Refer to the paper Fortuin V, Baranchuk D, Rätsch G, et al.
-GP-VAE: Deep probabilistic time series imputation. AISTATS. PMLR, 2020: 1651-1661.
-
 
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import numpy as np
@@ -153,15 +148,15 @@
         net = nn.Sequential(*layers)
         return [net] + [nn.Linear(hidden_sizes[-1], o) for o in output_size]
 
     layers.append(nn.Linear(hidden_sizes[-1], output_size))
     return nn.Sequential(*layers)
 
 
-class Encoder(nn.Module):
+class GpvaeEncoder(nn.Module):
     def __init__(self, input_size, z_size, hidden_sizes=(128, 128), window_size=24):
         """This module is an encoder with 1d-convolutional network and multivariate Normal posterior used by GP-VAE with
         proposed banded covariance matrix
 
         Parameters
         ----------
         input_size : int,
@@ -236,15 +231,15 @@
 
         z_dist = torch.distributions.MultivariateNormal(
             loc=mapped_mean, scale_tril=cov_tril_lower
         )
         return z_dist
 
 
-class Decoder(nn.Module):
+class GpvaeDecoder(nn.Module):
     def __init__(self, input_size, output_size, hidden_sizes=(256, 256)):
         """This module is a decoder with Gaussian output distribution.
 
         Parameters
         ----------
         output_size : int,
             the feature dimension of the output
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4/pypots/imputation/informer/__init__.py` & `pypots-0.4.1/pypots/imputation/informer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/informer/data.py` & `pypots-0.4.1/pypots/imputation/informer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/informer/model.py` & `pypots-0.4.1/pypots/imputation/informer/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _Informer
 from .data import DatasetForInformer
-from .modules.core import _Informer
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
@@ -57,14 +57,20 @@
 
     factor :
         The factor of the ProbSparse self-attention mechanism for the Informer model.
 
     dropout :
         The dropout rate for the model.
 
+    ORT_weight :
+        The weight for the ORT loss, the same as SAITS.
+
+    MIT_weight :
+        The weight for the MIT loss, the same as SAITS.
+
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
     patience :
@@ -108,14 +114,16 @@
         n_features: int,
         n_layers: int,
         n_heads: int,
         d_model: int,
         d_ffn: int,
         factor: int,
         dropout: float = 0,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -136,25 +144,29 @@
         # model hype-parameters
         self.n_heads = n_heads
         self.n_layers = n_layers
         self.d_model = d_model
         self.d_ffn = d_ffn
         self.factor = factor
         self.dropout = dropout
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _Informer(
             self.n_steps,
             self.n_features,
             self.n_layers,
             self.n_heads,
             self.d_model,
             self.d_ffn,
             self.factor,
             self.dropout,
+            self.ORT_weight,
+            self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/imputation/informer/modules/core.py` & `pypots-0.4.1/pypots/imputation/patchtst/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,91 +4,83 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import torch
 import torch.nn as nn
 
-from .submodules import ProbAttention, ConvLayer, InformerEncoderLayer, InformerEncoder
-from ....nn.modules.transformer import MultiHeadAttention
-from ....nn.modules.transformer.embedding import DataEmbedding
-from ....utils.metrics import calc_mse
+from ...nn.modules.patchtst import PatchEmbedding, PatchtstEncoder, PredictionHead
+from ...nn.modules.saits import SaitsLoss
 
 
-class _Informer(nn.Module):
+class _PatchTST(nn.Module):
     def __init__(
         self,
-        n_steps,
-        n_features,
-        n_layers,
-        n_heads,
-        d_model,
-        d_ffn,
-        factor,
-        dropout,
-        distil=False,
-        activation="relu",
-        output_attention=False,
+        n_steps: int,
+        n_features: int,
+        n_layers: int,
+        n_heads: int,
+        d_model: int,
+        d_ffn: int,
+        d_k: int,
+        d_v: int,
+        patch_len: int,
+        stride: int,
+        dropout: float,
+        attn_dropout: float,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
     ):
         super().__init__()
 
-        self.seq_len = n_steps
-        self.n_layers = n_layers
-        self.enc_embedding = DataEmbedding(
-            n_features * 2,
-            d_model,
-            dropout=dropout,
+        n_patches = int((n_steps - patch_len) / stride + 2)  # number of patches
+        padding = stride
+
+        self.embedding = nn.Linear(n_features * 2, d_model)
+        self.patch_embedding = PatchEmbedding(
+            d_model, patch_len, stride, padding, dropout
         )
-        self.encoder = InformerEncoder(
-            [
-                InformerEncoderLayer(
-                    MultiHeadAttention(
-                        n_heads,
-                        d_model,
-                        d_model // n_heads,
-                        d_model // n_heads,
-                        ProbAttention(False, factor, dropout, output_attention),
-                    ),
-                    d_model,
-                    d_ffn,
-                    dropout,
-                    activation,
-                )
-                for _ in range(n_layers)
-            ],
-            [ConvLayer(d_model) for _ in range(n_layers - 1)] if distil else None,
-            norm_layer=nn.LayerNorm(d_model),
+        self.encoder = PatchtstEncoder(
+            n_layers, n_heads, d_model, d_ffn, d_k, d_v, dropout, attn_dropout
         )
-
-        # for the imputation task, the output dim is the same as input dim
+        self.head = PredictionHead(d_model, n_patches, n_steps, dropout)
         self.output_projection = nn.Linear(d_model, n_features)
+        self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
-        X, masks = inputs["X"], inputs["missing_mask"]
+        X, missing_mask = inputs["X"], inputs["missing_mask"]
 
-        # WDU: the original Informer paper isn't proposed for imputation task. Hence the model doesn't take
+        # WDU: the original PatchTST paper isn't proposed for imputation task. Hence the model doesn't take
         # the missing mask into account, which means, in the process, the model doesn't know which part of
         # the input data is missing, and this may hurt the model's imputation performance. Therefore, I add the
         # embedding layers to project the concatenation of features and masks into a hidden space, as well as
         # the output layers to project back from the hidden space to the original space.
 
-        # the same as SAITS, concatenate the time series data and the missing mask for embedding
-        input_X = torch.cat([X, masks], dim=2)
-        enc_out = self.enc_embedding(input_X)
+        # do patching and embedding
+        input_X = self.embedding(torch.cat([X, missing_mask], dim=2))
+        enc_out = self.patch_embedding(
+            input_X.permute(0, 2, 1)
+        )  # [bz * d_model, n_patches, d_model]
 
-        # Informer encoder processing
+        # PatchTST encoder processing
         enc_out, attns = self.encoder(enc_out)
 
         # project back the original data space
-        output = self.output_projection(enc_out)
+        dec_out = self.head(enc_out)  # [bz, n_steps, d_model]
+        reconstruction = self.output_projection(dec_out)
 
-        imputed_data = masks * X + (1 - masks) * output
+        imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
         results = {
             "imputed_data": imputed_data,
         }
 
         if training:
+            X_ori, indicating_mask = inputs["X_ori"], inputs["indicating_mask"]
+            loss, ORT_loss, MIT_loss = self.saits_loss_func(
+                reconstruction, X_ori, missing_mask, indicating_mask
+            )
+            results["ORT_loss"] = ORT_loss
+            results["MIT_loss"] = MIT_loss
             # `loss` is always the item for backward propagating to update the model
-            loss = calc_mse(output, inputs["X_ori"], inputs["indicating_mask"])
             results["loss"] = loss
 
         return results
```

### Comparing `pypots-0.4/pypots/imputation/informer/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/informer/layers.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,23 +56,21 @@
 
 
 class ProbAttention(AttentionOperator):
     def __init__(
         self,
         mask_flag=True,
         factor=5,
-        scale=None,
         attention_dropout=0.1,
-        output_attention=False,
+        scale=None,
     ):
         super().__init__()
         self.factor = factor
         self.scale = scale
         self.mask_flag = mask_flag
-        self.output_attention = output_attention
         self.dropout = nn.Dropout(attention_dropout)
 
     def _prob_QK(self, Q, K, sample_k, n_top):  # n_top: c*ln(L_q)
         # Q [B, H, L, D]
         B, H, L_K, E = K.shape
         _, _, L_Q, _ = Q.shape
 
@@ -117,22 +115,20 @@
             scores.masked_fill_(attn_mask.mask, -np.inf)
 
         attn = torch.softmax(scores, dim=-1)  # nn.Softmax(dim=-1)(scores)
 
         context_in[
             torch.arange(B)[:, None, None], torch.arange(H)[None, :, None], index, :
         ] = torch.matmul(attn, V).type_as(context_in)
-        if self.output_attention:
-            attns = (torch.ones([B, H, L_V, L_V]) / L_V).type_as(attn).to(attn.device)
-            attns[
-                torch.arange(B)[:, None, None], torch.arange(H)[None, :, None], index, :
-            ] = attn
-            return (context_in, attns)
-        else:
-            return (context_in, None)
+
+        attns = (torch.ones([B, H, L_V, L_V]) / L_V).type_as(attn).to(attn.device)
+        attns[
+            torch.arange(B)[:, None, None], torch.arange(H)[None, :, None], index, :
+        ] = attn
+        return context_in, attns
 
     def forward(
         self,
         q: torch.Tensor,
         k: torch.Tensor,
         v: torch.Tensor,
         attn_mask: Optional[torch.Tensor] = None,
@@ -187,54 +183,46 @@
         y = x = self.norm1(x)
         y = self.dropout(self.activation(self.conv1(y.transpose(-1, 1))))
         y = self.dropout(self.conv2(y).transpose(-1, 1))
 
         return self.norm2(x + y), attn
 
 
-class InformerEncoder(nn.Module):
-    def __init__(self, attn_layers, conv_layers=None, norm_layer=None):
+class InformerDecoderLayer(nn.Module):
+    def __init__(
+        self,
+        self_attention,
+        cross_attention,
+        d_model,
+        d_ff=None,
+        dropout=0.1,
+        activation="relu",
+    ):
         super().__init__()
-        self.attn_layers = nn.ModuleList(attn_layers)
-        self.conv_layers = (
-            nn.ModuleList(conv_layers) if conv_layers is not None else None
-        )
-        self.norm = norm_layer
-
-    def forward(self, x, attn_mask=None):
-        attns = []
-        if self.conv_layers is not None:
-            for attn_layer, conv_layer in zip(self.attn_layers, self.conv_layers):
-                x, attn = attn_layer(x, attn_mask=attn_mask)
-                x = conv_layer(x)
-                attns.append(attn)
-            x, attn = self.attn_layers[-1](x)
-            attns.append(attn)
-        else:
-            for attn_layer in self.attn_layers:
-                x, attn = attn_layer(x, attn_mask=attn_mask)
-                attns.append(attn)
+        d_ff = d_ff or 4 * d_model
+        self.self_attention = self_attention
+        self.cross_attention = cross_attention
+        self.conv1 = nn.Conv1d(in_channels=d_model, out_channels=d_ff, kernel_size=1)
+        self.conv2 = nn.Conv1d(in_channels=d_ff, out_channels=d_model, kernel_size=1)
+        self.norm1 = nn.LayerNorm(d_model)
+        self.norm2 = nn.LayerNorm(d_model)
+        self.norm3 = nn.LayerNorm(d_model)
+        self.dropout = nn.Dropout(dropout)
+        self.activation = F.relu if activation == "relu" else F.gelu
 
-        if self.norm is not None:
-            x = self.norm(x)
+    def forward(self, x, cross, x_mask=None, cross_mask=None, tau=None, delta=None):
+        x = x + self.dropout(
+            self.self_attention(x, x, x, attn_mask=x_mask, tau=tau, delta=None)[0]
+        )
+        x = self.norm1(x)
 
-        return x, attns
+        x = x + self.dropout(
+            self.cross_attention(
+                x, cross, cross, attn_mask=cross_mask, tau=tau, delta=delta
+            )[0]
+        )
 
+        y = x = self.norm2(x)
+        y = self.dropout(self.activation(self.conv1(y.transpose(-1, 1))))
+        y = self.dropout(self.conv2(y).transpose(-1, 1))
 
-class InformerDecoder(nn.Module):
-    def __init__(self, layers, norm_layer=None, projection=None):
-        super().__init__()
-        self.layers = nn.ModuleList(layers)
-        self.norm = norm_layer
-        self.projection = projection
-
-    def forward(self, x, cross, x_mask=None, cross_mask=None, trend=None):
-        for layer in self.layers:
-            x, residual_trend = layer(x, cross, x_mask=x_mask, cross_mask=cross_mask)
-            trend = trend + residual_trend
-
-        if self.norm is not None:
-            x = self.norm(x)
-
-        if self.projection is not None:
-            x = self.projection(x)
-        return x, trend
+        return self.norm3(x + y)
```

### Comparing `pypots-0.4/pypots/imputation/locf/model.py` & `pypots-0.4.1/pypots/imputation/locf/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 import warnings
 from typing import Union, Optional
 
 import h5py
 import numpy as np
 import torch
 
-from .modules.core import locf_numpy, locf_torch
+from .core import locf_numpy, locf_torch
 from ..base import BaseImputer
 from ...utils.logging import logger
 
 
 class LOCF(BaseImputer):
     """LOCF (Last Observed Carried Forward) imputation method. A naive imputation method that fills missing values
-    with the last observed value. Simple but commonly used in practice.
+    with the last observed value. When time-series data gets inverse on the time dimension, this method can also be
+    seen as NOCB (Next Observation Carried Backward). Simple but commonly used in practice.
 
     Parameters
     ----------
     first_step_imputation : str, default='backward'
         With LOCF, the observed values are carried forward to impute the missing ones. But if the first value
         is missing, there is no value to carry forward. This parameter is used to determine the strategy to
         impute the missing values at the beginning of the time-series sequence after LOCF is applied.
```

### Comparing `pypots-0.4/pypots/imputation/locf/modules/core.py` & `pypots-0.4.1/pypots/imputation/locf/core.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/mean/model.py` & `pypots-0.4.1/pypots/imputation/mean/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/median/model.py` & `pypots-0.4.1/pypots/imputation/median/model.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/mrnn/data.py` & `pypots-0.4.1/pypots/imputation/mrnn/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/mrnn/model.py` & `pypots-0.4.1/pypots/imputation/mrnn/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _MRNN
 from .data import DatasetForMRNN
-from .modules import _MRNN
 from ..base import BaseNNImputer
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
@@ -113,15 +113,14 @@
         self.rnn_hidden_size = rnn_hidden_size
 
         # set up the model
         self.model = _MRNN(
             self.n_steps,
             self.n_features,
             self.rnn_hidden_size,
-            self.device,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/imputation/mrnn/modules/core.py` & `pypots-0.4.1/pypots/nn/modules/mrnn/backbone.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,35 +3,34 @@
 This implementation is inspired by the official one https://github.com/jsyoon0823/MRNN.
 Some part of the code is from https://github.com/WenjieDu/SAITS.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
+from typing import Tuple
 
 import torch
 import torch.nn as nn
 
-from .submodules import FCN_Regression
-from ....utils.metrics import calc_rmse
+from .layers import MrnnFcnRegression
 
 
-class _MRNN(nn.Module):
-    def __init__(self, seq_len, feature_num, rnn_hidden_size, device):
+class BackboneMRNN(nn.Module):
+    def __init__(self, n_steps, n_features, rnn_hidden_size):
         super().__init__()
-        # data settings
-        self.seq_len = seq_len
-        self.feature_num = feature_num
+
+        self.n_steps = n_steps
+        self.n_features = n_features
         self.rnn_hidden_size = rnn_hidden_size
-        self.device = device
 
         self.f_rnn = nn.GRU(3, self.rnn_hidden_size, batch_first=True)
         self.b_rnn = nn.GRU(3, self.rnn_hidden_size, batch_first=True)
         self.concated_hidden_project = nn.Linear(self.rnn_hidden_size * 2, 1)
-        self.fcn_regression = FCN_Regression(feature_num)
+        self.fcn_regression = MrnnFcnRegression(n_features)
 
     def gene_hidden_states(self, inputs, feature_idx):
         X_f = inputs["forward"]["X"][:, :, feature_idx].unsqueeze(dim=2)
         M_f = inputs["forward"]["missing_mask"][:, :, feature_idx].unsqueeze(dim=2)
         D_f = inputs["forward"]["deltas"][:, :, feature_idx].unsqueeze(dim=2)
         X_b = inputs["backward"]["X"][:, :, feature_idx].unsqueeze(dim=2)
         M_b = inputs["backward"]["missing_mask"][:, :, feature_idx].unsqueeze(dim=2)
@@ -53,34 +52,22 @@
 
         feature_estimation = self.concated_hidden_project(
             torch.cat([hidden_states_f, hidden_states_b], dim=2)
         )
 
         return feature_estimation, hidden_states_f, hidden_states_b
 
-    def forward(self, inputs: dict, training: bool = True) -> dict:
+    def forward(self, inputs: dict) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         X = inputs["forward"]["X"]
         M = inputs["forward"]["missing_mask"]
 
         feature_collector = []
-        for f in range(self.feature_num):
+        for f in range(self.n_features):
             feat_estimation, hid_states_f, hid_states_b = self.gene_hidden_states(
                 inputs, f
             )
             feature_collector.append(feat_estimation)
+
         RNN_estimation = torch.concat(feature_collector, dim=2)
         RNN_imputed_data = M * X + (1 - M) * RNN_estimation
         FCN_estimation = self.fcn_regression(X, M, RNN_imputed_data)
-
-        imputed_data = M * X + (1 - M) * FCN_estimation
-        results = {
-            "imputed_data": imputed_data,
-        }
-
-        # if in training mode, return results with losses
-        if training:
-            RNN_loss = calc_rmse(RNN_estimation, X, M)
-            FCN_loss = calc_rmse(FCN_estimation, RNN_imputed_data)
-            reconstruction_loss = RNN_loss + FCN_loss
-            results["loss"] = reconstruction_loss
-
-        return results
+        return RNN_estimation, RNN_imputed_data, FCN_estimation
```

### Comparing `pypots-0.4/pypots/imputation/mrnn/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/mrnn/layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
-The submodules of the MRNN model.
+The layers of the M-RNN model.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 
 import math
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn.parameter import Parameter
 
 
-class FCN_Regression(nn.Module):
+class MrnnFcnRegression(nn.Module):
+    """M-RNN fully connection regression Layer"""
+
     def __init__(self, feature_num):
         super().__init__()
         self.U = Parameter(torch.Tensor(feature_num, feature_num))
         self.V1 = Parameter(torch.Tensor(feature_num, feature_num))
         self.V2 = Parameter(torch.Tensor(feature_num, feature_num))
         self.beta = Parameter(torch.Tensor(feature_num))  # bias beta
         self.final_linear = nn.Linear(feature_num, feature_num)
```

### Comparing `pypots-0.4/pypots/imputation/patchtst/data.py` & `pypots-0.4.1/pypots/imputation/patchtst/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/patchtst/model.py` & `pypots-0.4.1/pypots/imputation/patchtst/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .data import DatasetForPatchTST
-from .modules.core import _PatchTST
+from pypots.imputation.patchtst.core import _PatchTST
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
@@ -69,14 +69,20 @@
 
     d_ffn :
         The dimension of the feed-forward network.
 
     dropout :
         The dropout rate for the model.
 
+    ORT_weight :
+        The weight for the ORT loss, the same as SAITS.
+
+    MIT_weight :
+        The weight for the MIT loss, the same as SAITS.
+
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
     patience :
@@ -124,14 +130,16 @@
         n_heads: int,
         d_k: int,
         d_v: int,
         d_model: int,
         d_ffn: int,
         dropout: float,
         attn_dropout: float,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
@@ -165,14 +173,16 @@
         self.n_heads = n_heads
         self.d_k = d_k
         self.d_v = d_v
         self.d_model = d_model
         self.d_ffn = d_ffn
         self.dropout = dropout
         self.attn_dropout = attn_dropout
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
 
         # set up the model
         self.model = _PatchTST(
             self.n_steps,
             self.n_features,
             self.n_layers,
             self.n_heads,
@@ -180,14 +190,16 @@
             self.d_ffn,
             self.d_k,
             self.d_v,
             self.patch_len,
             self.stride,
             self.dropout,
             self.attn_dropout,
+            self.ORT_weight,
+            self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
```

### Comparing `pypots-0.4/pypots/imputation/saits/data.py` & `pypots-0.4.1/pypots/imputation/saits/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/saits/model.py` & `pypots-0.4.1/pypots/imputation/saits/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import Union, Optional, Callable
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
 from .data import DatasetForSAITS
-from .modules import _SAITS
+from .core import _SAITS
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 from ...utils.metrics import calc_mae
```

### Comparing `pypots-0.4/pypots/imputation/timesnet/data.py` & `pypots-0.4.1/pypots/imputation/timesnet/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/timesnet/model.py` & `pypots-0.4.1/pypots/imputation/transformer/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,87 @@
 """
-The implementation of TimesNet for the partially-observed time-series imputation task.
+The implementation of Transformer for the partially-observed time-series imputation task.
 
-Refer to the paper "Haixu Wu, Tengge Hu, Yong Liu, Hang Zhou, Jianmin Wang, and Mingsheng Long.
-TimesNet: Temporal 2D-Variation Modeling for General Time Series Analysis.
-In ICLR, 2023."
+Refer to the paper "Wenjie Du, David Cote, and Yan Liu.
+SAITS: Self-Attention-based Imputation for Time Series.
+Expert Systems with Applications, 219:119619, 2023."
 
 Notes
 -----
-Partial implementation uses code from https://github.com/thuml/Time-Series-Library.
+Partial implementation uses code from https://github.com/WenjieDu/SAITS.
 
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-from .data import DatasetForTimesNet
-from .modules.core import _TimesNet
+from .core import _Transformer
+from .data import DatasetForTransformer
 from ..base import BaseNNImputer
 from ...data.base import BaseDataset
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 
 
-class TimesNet(BaseNNImputer):
-    """The PyTorch implementation of the TimesNet model.
-    TimesNet is originally proposed by Wu et al. in :cite:`wu2023timesnet`.
+class Transformer(BaseNNImputer):
+    """The PyTorch implementation of the Transformer model.
+    Transformer is originally proposed by Vaswani et al. in :cite:`vaswani2017Transformer`,
+    and gets re-implemented as a time-series imputation model by Du et al. in :cite:`du2023SAITS`.
+    Here you should refer to :cite:`du2023SAITS` for details about this Transformer imputation model.
 
     Parameters
     ----------
     n_steps :
         The number of time steps in the time-series data sample.
 
     n_features :
         The number of features in the time-series data sample.
 
     n_layers :
-        The number of layers in the TimesNet model.
-
-    top_k :
-        The number of top-k amplitude values to be selected to  obtain the most significant frequencies.
+        The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
 
     d_model :
-        The dimension of the model.
+        The dimension of the model's backbone.
+        It is the input dimension of the multi-head self-attention layers.
 
     d_ffn :
-        The dimension of the feed-forward network.
+        The dimension of the layer in the Feed-Forward Networks (FFN).
+
+    n_heads :
+        The number of heads in the multi-head self-attention mechanism.
+        ``d_model`` must be divisible by ``n_heads``, and the result should be equal to ``d_k``.
+
+    d_k :
+        The dimension of the `keys` (K) and the `queries` (Q) in the DMSA mechanism.
+        ``d_k`` should be the result of ``d_model`` divided by ``n_heads``. Although ``d_k`` can be directly calculated
+        with given ``d_model`` and ``n_heads``, we want it be explicitly given together with ``d_v`` by users to ensure
+        users be aware of them and to avoid any potential mistakes.
 
-    n_kernels :
-        The number of 2D kernels (2D convolutional layers) to use in the submodule InceptionBlockV1.
+    d_v :
+        The dimension of the `values` (V) in the DMSA mechanism.
 
     dropout :
-        The dropout rate for the model.
+        The dropout rate for all fully-connected layers in the model.
+
+    attn_dropout :
+        The dropout rate for DMSA.
 
-    apply_nonstationary_norm :
-        Whether to apply non-stationary normalization to the input data for TimesNet.
-        Please refer to :cite:`liu2022nonstationary` for details about non-stationary normalization,
-        which is not the idea of the original TimesNet paper. Hence, we make it optional and default not to use here.
+    ORT_weight :
+        The weight for the ORT loss.
+
+    MIT_weight :
+        The weight for the MIT loss.
 
     batch_size :
         The batch size for training and evaluating the model.
 
     epochs :
         The number of epochs for training the model.
 
@@ -107,23 +121,26 @@
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         n_layers: int,
-        top_k: int,
         d_model: int,
         d_ffn: int,
-        n_kernels: int,
+        n_heads: int,
+        d_k: int,
+        d_v: int,
         dropout: float = 0,
-        apply_nonstationary_norm: bool = False,
+        attn_dropout: float = 0,
+        ORT_weight: int = 1,
+        MIT_weight: int = 1,
         batch_size: int = 32,
         epochs: int = 100,
-        patience: int = None,
+        patience: Optional[int] = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
         device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
         super().__init__(
@@ -132,36 +149,52 @@
             patience,
             num_workers,
             device,
             saving_path,
             model_saving_strategy,
         )
 
+        if d_model != n_heads * d_k:
+            logger.warning(
+                "‼️ d_model must = n_heads * d_k, it should be divisible by n_heads "
+                f"and the result should be equal to d_k, but got d_model={d_model}, n_heads={n_heads}, d_k={d_k}"
+            )
+            d_model = n_heads * d_k
+            logger.warning(
+                f"⚠️ d_model is reset to {d_model} = n_heads ({n_heads}) * d_k ({d_k})"
+            )
+
         self.n_steps = n_steps
         self.n_features = n_features
         # model hype-parameters
         self.n_layers = n_layers
-        self.top_k = top_k
         self.d_model = d_model
         self.d_ffn = d_ffn
-        self.n_kernels = n_kernels
+        self.n_heads = n_heads
+        self.d_k = d_k
+        self.d_v = d_v
         self.dropout = dropout
-        self.apply_nonstationary_norm = apply_nonstationary_norm
+        self.attn_dropout = attn_dropout
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
 
         # set up the model
-        self.model = _TimesNet(
-            self.n_layers,
+        self.model = _Transformer(
             self.n_steps,
             self.n_features,
-            self.top_k,
+            self.n_layers,
             self.d_model,
             self.d_ffn,
-            self.n_kernels,
+            self.n_heads,
+            self.d_k,
+            self.d_v,
             self.dropout,
-            self.apply_nonstationary_norm,
+            self.attn_dropout,
+            self.ORT_weight,
+            self.MIT_weight,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
@@ -200,28 +233,28 @@
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForTimesNet(
+        training_set = DatasetForTransformer(
             train_set, return_X_ori=False, return_labels=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
         if val_set is not None:
             if not check_X_ori_in_val_set(val_set):
                 raise ValueError("val_set must contain 'X_ori' for model validation.")
-            val_set = DatasetForTimesNet(
+            val_set = DatasetForTransformer(
                 val_set, return_X_ori=True, return_labels=False, file_type=file_type
             )
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
@@ -236,57 +269,33 @@
         self._auto_save_model_if_necessary(confirm_saving=True)
 
     def predict(
         self,
         test_set: Union[dict, str],
         file_type: str = "h5py",
     ) -> dict:
-        """Make predictions for the input data with the trained model.
-
-        Parameters
-        ----------
-        test_set : dict or str
-            The dataset for model validating, should be a dictionary including keys as 'X',
-            or a path string locating a data file supported by PyPOTS (e.g. h5 file).
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for validating, can contain missing values, and y should be array-like of shape
-            [n_samples], which is classification labels of X.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
-
-        file_type : str
-            The type of the given file if test_set is a path string.
-
-        Returns
-        -------
-        result_dict : dict,
-            The dictionary containing the clustering results and latent variables if necessary.
-
-        """
-        # Step 1: wrap the input data with classes Dataset and DataLoader
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = BaseDataset(
             test_set, return_X_ori=False, return_labels=False, file_type=file_type
         )
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         imputation_collector = []
 
-        # Step 2: process the data with the model
         with torch.no_grad():
             for idx, data in enumerate(test_loader):
                 inputs = self._assemble_input_for_testing(data)
                 results = self.model.forward(inputs, training=False)
-                imputation_collector.append(results["imputed_data"])
+                imputed_data = results["imputed_data"]
+                imputation_collector.append(imputed_data)
 
-        # Step 3: output collection and return
         imputation = torch.cat(imputation_collector).cpu().detach().numpy()
         result_dict = {
             "imputation": imputation,
         }
         return result_dict
 
     def impute(
@@ -313,10 +322,9 @@
         -------
         array-like, shape [n_samples, sequence length (time steps), n_features],
             Imputed data.
         """
         logger.warning(
             "🚨DeprecationWarning: The method impute is deprecated. Please use `predict` instead."
         )
-
         results_dict = self.predict(X, file_type=file_type)
         return results_dict["imputation"]
```

### Comparing `pypots-0.4/pypots/imputation/timesnet/modules/core.py` & `pypots-0.4.1/pypots/imputation/timesnet/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import torch.nn as nn
 
-from .submodules import TimesBlock
-from ....nn.functional import nonstationary_norm, nonstationary_denorm
-from ....nn.modules.transformer.embedding import DataEmbedding
-from ....utils.metrics import calc_mse
+from ...nn.functional import nonstationary_norm, nonstationary_denorm
+from ...nn.modules.timesnet import BackboneTimesNet
+from ...nn.modules.transformer.embedding import DataEmbedding
+from ...utils.metrics import calc_mse
 
 
 class _TimesNet(nn.Module):
     def __init__(
         self,
         n_layers,
         n_steps,
@@ -28,53 +28,53 @@
     ):
         super().__init__()
 
         self.seq_len = n_steps
         self.n_layers = n_layers
         self.apply_nonstationary_norm = apply_nonstationary_norm
 
-        self.pred_len = 0  # for the imputation task, the pred_len is always 0
-        self.model = nn.ModuleList(
-            [
-                TimesBlock(n_steps, self.pred_len, top_k, d_model, d_ffn, n_kernels)
-                for _ in range(n_layers)
-            ]
-        )
         self.enc_embedding = DataEmbedding(
             n_features,
             d_model,
             dropout=dropout,
         )
+        self.model = BackboneTimesNet(
+            n_layers,
+            n_steps,
+            0,  # n_pred_steps should be 0 for the imputation task
+            top_k,
+            d_model,
+            d_ffn,
+            n_kernels,
+        )
         self.layer_norm = nn.LayerNorm(d_model)
 
         # for the imputation task, the output dim is the same as input dim
-        c_out = n_features
-        self.projection = nn.Linear(d_model, c_out)
+        self.projection = nn.Linear(d_model, n_features)
 
     def forward(self, inputs: dict, training: bool = True) -> dict:
-        X, masks = inputs["X"], inputs["missing_mask"]
+        X, missing_mask = inputs["X"], inputs["missing_mask"]
 
         if self.apply_nonstationary_norm:
             # Normalization from Non-stationary Transformer
-            X, means, stdev = nonstationary_norm(X, masks)
+            X, means, stdev = nonstationary_norm(X, missing_mask)
 
         # embedding
-        enc_out = self.enc_embedding(X)  # [B,T,C]
-        # TimesNet
-        for i in range(self.n_layers):
-            enc_out = self.layer_norm(self.model[i](enc_out))
+        input_X = self.enc_embedding(X)  # [B,T,C]
+        # TimesNet processing
+        enc_out = self.model(input_X)
 
         # project back the original data space
         dec_out = self.projection(enc_out)
 
         if self.apply_nonstationary_norm:
             # De-Normalization from Non-stationary Transformer
             dec_out = nonstationary_denorm(dec_out, means, stdev)
 
-        imputed_data = masks * X + (1 - masks) * dec_out
+        imputed_data = missing_mask * X + (1 - missing_mask) * dec_out
         results = {
             "imputed_data": imputed_data,
         }
 
         if training:
             # `loss` is always the item for backward propagating to update the model
             loss = calc_mse(dec_out, inputs["X_ori"], inputs["indicating_mask"])
```

### Comparing `pypots-0.4/pypots/imputation/timesnet/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/timesnet/layers.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/transformer/__init__.py` & `pypots-0.4.1/pypots/imputation/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/transformer/data.py` & `pypots-0.4.1/pypots/imputation/transformer/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/usgan/data.py` & `pypots-0.4.1/pypots/imputation/usgan/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/imputation/usgan/model.py` & `pypots-0.4.1/pypots/imputation/usgan/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import os
 from typing import Union, Optional
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
+from .core import _USGAN
 from .data import DatasetForUSGAN
-from .modules import _USGAN
 from ..base import BaseNNImputer
 from ...data.checking import check_X_ori_in_val_set
 from ...optim.adam import Adam
 from ...optim.base import Optimizer
 from ...utils.logging import logger
 from ...utils.metrics import calc_mse
 
@@ -145,24 +145,23 @@
         self.model = _USGAN(
             n_steps,
             n_features,
             rnn_hidden_size,
             lambda_mse,
             hint_rate,
             dropout,
-            self.device,
         )
         self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.G_optimizer = G_optimizer
-        self.G_optimizer.init_optimizer(self.model.generator.parameters())
+        self.G_optimizer.init_optimizer(self.model.backbone.generator.parameters())
         self.D_optimizer = D_optimizer
-        self.D_optimizer.init_optimizer(self.model.discriminator.parameters())
+        self.D_optimizer.init_optimizer(self.model.backbone.discriminator.parameters())
 
     def _assemble_input_for_training(self, data: list) -> dict:
         # fetch data
         (
             indices,
             X,
             missing_mask,
@@ -245,30 +244,28 @@
                     inputs = self._assemble_input_for_training(data)
 
                     if idx % self.G_steps == 0:
                         self.G_optimizer.zero_grad()
                         results = self.model.forward(
                             inputs, training_object="generator"
                         )
-                        results["generation_loss"].backward()
+                        results["loss"].backward()  # generation loss
                         self.G_optimizer.step()
-                        step_train_loss_G_collector.append(
-                            results["generation_loss"].item()
-                        )
+                        step_train_loss_G_collector.append(results["loss"].item())
 
                     if idx % self.D_steps == 0:
                         self.D_optimizer.zero_grad()
                         results = self.model.forward(
                             inputs, training_object="discriminator"
                         )
-                        results["discrimination_loss"].backward(retain_graph=True)
+                        results["loss"].backward(
+                            retain_graph=True
+                        )  # discrimination loss
                         self.D_optimizer.step()
-                        step_train_loss_D_collector.append(
-                            results["discrimination_loss"].item()
-                        )
+                        step_train_loss_D_collector.append(results["loss"].item())
 
                     mean_step_train_D_loss = np.mean(step_train_loss_D_collector)
                     mean_step_train_G_loss = np.mean(step_train_loss_G_collector)
 
                     # save training loss logs into the tensorboard file for every step if in need
                     # Note: the `training_step` is not the actual number of steps that Discriminator and Generator get
                     # trained, the actual number should be D_steps*training_step and G_steps*training_step accordingly
```

### Comparing `pypots-0.4/pypots/imputation/usgan/modules/core.py` & `pypots-0.4.1/pypots/imputation/transformer/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,94 @@
 """
-The implementation of USGAN for the partially-observed time-series imputation task.
+The implementation of Transformer for the partially-observed time-series imputation task.
 
-Refer to the paper "Miao, X., Wu, Y., Wang, J., Gao, Y., Mao, X., & Yin, J. (2021).
-Generative Semi-supervised Learning for Multivariate Time Series Imputation. AAAI 2021."
+Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
+Expert systems with applications."
+
+Notes
+-----
+Partial implementation uses code from https://github.com/WenjieDu/SAITS.
 
 """
 
-# Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
+# Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from typing import Union
-
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
-from ....utils.metrics import calc_mse
 
-from .submodules import Discriminator
-from ...brits.modules import _BRITS
+from ...nn.modules.saits import SaitsLoss
+from ...nn.modules.transformer import TransformerEncoder, PositionalEncoding
 
 
-class _USGAN(nn.Module):
-    """USGAN model"""
-
+class _Transformer(nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
-        rnn_hidden_size: int,
-        lambda_mse: float,
-        hint_rate: float = 0.7,
-        dropout_rate: float = 0.0,
-        device: Union[str, torch.device] = "cpu",
+        n_layers: int,
+        d_model: int,
+        d_ffn: int,
+        n_heads: int,
+        d_k: int,
+        d_v: int,
+        dropout: float,
+        attn_dropout: float,
+        ORT_weight: float = 1,
+        MIT_weight: float = 1,
     ):
         super().__init__()
-        self.generator = _BRITS(n_steps, n_features, rnn_hidden_size, device)
-        self.discriminator = Discriminator(
-            n_features,
-            rnn_hidden_size,
-            hint_rate=hint_rate,
-            dropout_rate=dropout_rate,
-            device=device,
+        self.n_layers = n_layers
+        self.ORT_weight = ORT_weight
+        self.MIT_weight = MIT_weight
+
+        self.embedding = nn.Linear(n_features * 2, d_model)
+        self.dropout = nn.Dropout(dropout)
+        self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
+        self.encoder = TransformerEncoder(
+            n_layers,
+            d_model,
+            d_ffn,
+            n_heads,
+            d_k,
+            d_v,
+            dropout,
+            attn_dropout,
         )
+        self.output_projection = nn.Linear(d_model, n_features)
 
-        self.lambda_mse = lambda_mse
-        self.device = device
+        # apply SAITS loss function to Transformer on the imputation task
+        self.saits_loss_func = SaitsLoss(ORT_weight, MIT_weight)
 
-    def forward(
-        self,
-        inputs: dict,
-        training_object: str = "generator",
-        training: bool = True,
-    ) -> dict:
-        assert training_object in [
-            "generator",
-            "discriminator",
-        ], 'training_object should be "generator" or "discriminator"'
+    def forward(self, inputs: dict, training: bool = True) -> dict:
+        X, missing_mask = inputs["X"], inputs["missing_mask"]
 
-        results = self.generator(inputs, training=training)
+        # apply the SAITS embedding strategy, concatenate X and missing mask for input
+        input_X = torch.cat([X, missing_mask], dim=2)
+
+        # Transformer encoder processing
+        input_X = self.embedding(input_X)
+        input_X = self.dropout(self.position_enc(input_X))
+        enc_output, _ = self.encoder(input_X)
+        # project the representation from the d_model-dimensional space to the original data space for output
+        reconstruction = self.output_projection(enc_output)
+
+        # replace the observed part with values from X
+        imputed_data = missing_mask * X + (1 - missing_mask) * reconstruction
+
+        # ensemble the results as a dictionary for return
+        results = {
+            "imputed_data": imputed_data,
+        }
 
         # if in training mode, return results with losses
         if training:
-            forward_X = inputs["forward"]["X"]
-            forward_missing_mask = inputs["forward"]["missing_mask"]
-            imputed_data = results["imputed_data"]
-
-            if training_object == "discriminator":
-                inputs["discrimination"] = self.discriminator(
-                    imputed_data.detach(), forward_missing_mask
-                )
-                l_D = F.binary_cross_entropy_with_logits(
-                    inputs["discrimination"], forward_missing_mask
-                )
-                results["discrimination_loss"] = l_D
-            else:
-                inputs["discrimination"] = self.discriminator(
-                    imputed_data, forward_missing_mask
-                )
-                l_G = -F.binary_cross_entropy_with_logits(
-                    inputs["discrimination"],
-                    forward_missing_mask,
-                    weight=1 - forward_missing_mask,
-                )
-                reconstruction_loss = calc_mse(
-                    forward_X, results["reconstructed_data"], forward_missing_mask
-                ) + 0.1 * calc_mse(
-                    results["f_reconstructed_data"], results["b_reconstructed_data"]
-                )
-                loss_gene = l_G + self.lambda_mse * reconstruction_loss
-                results["generation_loss"] = loss_gene
+            X_ori, indicating_mask = inputs["X_ori"], inputs["indicating_mask"]
+            loss, ORT_loss, MIT_loss = self.saits_loss_func(
+                reconstruction, X_ori, missing_mask, indicating_mask
+            )
+            results["ORT_loss"] = ORT_loss
+            results["MIT_loss"] = MIT_loss
+            # `loss` is always the item for backward propagating to update the model
+            results["loss"] = loss
 
         return results
```

### Comparing `pypots-0.4/pypots/imputation/usgan/modules/submodules.py` & `pypots-0.4.1/pypots/nn/modules/usgan/layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
 
 """
 
 # Created by Jun Wang <jwangfx@connect.ust.hk> and Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
-from typing import Union
-
 import torch
 import torch.nn as nn
 
 
-class Discriminator(nn.Module):
+class UsganDiscriminator(nn.Module):
     """model Discriminator: built on BiRNN
 
     Parameters
     ----------
     n_features :
         the feature dimension of the input
 
@@ -35,24 +33,22 @@
 
     def __init__(
         self,
         n_features: int,
         rnn_hidden_size: int,
         hint_rate: float = 0.7,
         dropout_rate: float = 0.0,
-        device: Union[str, torch.device] = "cpu",
     ):
         super().__init__()
         self.hint_rate = hint_rate
-        self.device = device
         self.biRNN = nn.GRU(
             n_features * 2, rnn_hidden_size, bidirectional=True, batch_first=True
-        ).to(device)
-        self.dropout = nn.Dropout(dropout_rate).to(device)
-        self.read_out = nn.Linear(rnn_hidden_size * 2, n_features).to(device)
+        )
+        self.dropout = nn.Dropout(dropout_rate)
+        self.read_out = nn.Linear(rnn_hidden_size * 2, n_features)
 
     def forward(
         self,
         imputed_X: torch.Tensor,
         missing_mask: torch.Tensor,
     ) -> torch.Tensor:
         """Forward processing of USGAN Discriminator.
@@ -68,16 +64,17 @@
         Returns
         -------
         logits : torch.Tensor,
             the logits of the probability of being the true value.
 
         """
 
+        device = imputed_X.device
         hint = (
-            torch.rand_like(missing_mask, dtype=torch.float, device=self.device)
+            torch.rand_like(missing_mask, dtype=torch.float, device=device)
             < self.hint_rate
         )
         hint = hint.int()
         h = hint * missing_mask + (1 - hint) * 0.5
         x_in = torch.cat([imputed_X, h], dim=-1)
 
         out, _ = self.biRNN(x_in)
```

### Comparing `pypots-0.4/pypots/nn/functional/normalization.py` & `pypots-0.4.1/pypots/nn/functional/normalization.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/nn/modules/rnn.py` & `pypots-0.4.1/pypots/nn/modules/grud/layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-"""
-The implementation of some common-use modules related to RNN.
-"""
-
-# Created by Wenjie Du <wenjay.du@gmail.com>
-# License: BSD-3-Clause
-
 import math
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Variable
 from torch.nn.parameter import Parameter
 
 
 class TemporalDecay(nn.Module):
-    """The module used to generate the temporal decay factor gamma in the GRUD model.
-    Please refer to the original paper :cite:`che2018GRUD` for more deinails.
+    """The module used to generate the temporal decay factor gamma in the GRU-D model.
+    Please refer to the original paper :cite:`che2018GRUD` for more details.
 
     Attributes
     ----------
     W: tensor,
         The weights (parameters) of the module.
     b: tensor,
         The bias of the module.
```

### Comparing `pypots-0.4/pypots/nn/modules/transformer/attention.py` & `pypots-0.4.1/pypots/nn/modules/transformer/attention.py`

 * *Files 6% similar despite different names*

```diff
@@ -190,30 +190,31 @@
             The attention map.
 
         """
         # the input q, k, v currently have 3 dimensions [batch_size, n_steps, d_tensor]
         # d_tensor could be n_heads*d_k, n_heads*d_v
 
         # keep useful variables
-        batch_size, n_steps = q.size(0), q.size(1)
-        k_n_steps = k.size(1)
+        batch_size, q_len = q.size(0), q.size(1)
+        k_len = k.size(1)
+        v_len = v.size(1)
 
         # now separate the last dimension of q, k, v into different heads -> [batch_size, n_steps, n_heads, d_k or d_v]
-        q = self.w_qs(q).view(batch_size, n_steps, self.n_heads, self.d_k)
-        k = self.w_ks(k).view(batch_size, k_n_steps, self.n_heads, self.d_k)
-        v = self.w_vs(v).view(batch_size, k_n_steps, self.n_heads, self.d_v)
+        q = self.w_qs(q).view(batch_size, q_len, self.n_heads, self.d_k)
+        k = self.w_ks(k).view(batch_size, k_len, self.n_heads, self.d_k)
+        v = self.w_vs(v).view(batch_size, v_len, self.n_heads, self.d_v)
 
         # transpose for self-attention calculation -> [batch_size, n_steps, d_k or d_v, n_heads]
         q, k, v = q.transpose(1, 2), k.transpose(1, 2), v.transpose(1, 2)
 
         if attn_mask is not None:
             # broadcasting on the head axis
             attn_mask = attn_mask.unsqueeze(1)
 
         v, attn_weights = self.attention_operator(q, k, v, attn_mask, **kwargs)
 
         # transpose back -> [batch_size, n_steps, n_heads, d_v]
         # then merge the last two dimensions to combine all the heads -> [batch_size, n_steps, n_heads*d_v]
-        v = v.transpose(1, 2).contiguous().view(batch_size, n_steps, -1)
+        v = v.transpose(1, 2).contiguous().view(batch_size, q_len, -1)
         v = self.fc(v)
 
         return v, attn_weights
```

### Comparing `pypots-0.4/pypots/nn/modules/transformer/auto_encoder.py` & `pypots-0.4.1/pypots/nn/modules/transformer/auto_encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,31 +8,25 @@
 from typing import Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from .attention import ScaledDotProductAttention
 from .embedding import PositionalEncoding
-from .layers import EncoderLayer, DecoderLayer
+from .layers import TransformerEncoderLayer, TransformerDecoderLayer
 
 
-class Encoder(nn.Module):
+class TransformerEncoder(nn.Module):
     """Transformer encoder.
 
     Parameters
     ----------
     n_layers:
         The number of layers in the encoder.
 
-    n_steps:
-        The number of time steps in the input tensor.
-
-    n_features:
-        The number of features in the input tensor.
-
     d_model:
         The dimension of the module manipulation space.
         The input tensor will be projected to a space with d_model dimensions.
 
     d_ffn:
         The dimension of the hidden layer in the feed-forward network.
 
@@ -52,32 +46,27 @@
         The dropout rate for the attention map.
 
     """
 
     def __init__(
         self,
         n_layers: int,
-        n_steps: int,
-        n_features: int,
         d_model: int,
         d_ffn: int,
         n_heads: int,
         d_k: int,
         d_v: int,
         dropout: float,
         attn_dropout: float,
     ):
         super().__init__()
 
-        self.embedding = nn.Linear(n_features, d_model)
-        self.dropout = nn.Dropout(dropout)
-        self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
         self.enc_layer_stack = nn.ModuleList(
             [
-                EncoderLayer(
+                TransformerEncoderLayer(
                     d_model,
                     d_ffn,
                     n_heads,
                     d_k,
                     d_v,
                     ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     dropout,
@@ -86,53 +75,45 @@
             ]
         )
 
     def forward(
         self,
         x: torch.Tensor,
         src_mask: Optional[torch.Tensor] = None,
-        return_attn_weights: bool = False,
     ) -> Union[torch.Tensor, Tuple[torch.Tensor, list]]:
         """Forward processing of the encoder.
 
         Parameters
         ----------
         x:
             Input tensor.
 
         src_mask:
             Masking tensor for the attention map. The shape should be [batch_size, n_heads, n_steps, n_steps].
 
-        return_attn_weights:
-            Whether to return the attention map.
-
         Returns
         -------
         enc_output:
             Output tensor.
 
         attn_weights_collector:
             A list containing the attention map from each encoder layer.
 
         """
-        x = self.embedding(x)
-        enc_output = self.dropout(self.position_enc(x))
         attn_weights_collector = []
+        enc_output = x
 
         for layer in self.enc_layer_stack:
             enc_output, attn_weights = layer(enc_output, src_mask)
             attn_weights_collector.append(attn_weights)
 
-        if return_attn_weights:
-            return enc_output, attn_weights_collector
-
-        return enc_output
+        return enc_output, attn_weights_collector
 
 
-class Decoder(nn.Module):
+class TransformerDecoder(nn.Module):
     """Transformer decoder.
 
     Parameters
     ----------
     n_layers:
         The number of layers in the decoder.
 
@@ -181,15 +162,15 @@
     ):
         super().__init__()
         self.embedding = nn.Linear(n_features, d_model)
         self.dropout = nn.Dropout(dropout)
         self.position_enc = PositionalEncoding(d_model, n_positions=n_steps)
         self.layer_stack = nn.ModuleList(
             [
-                DecoderLayer(
+                TransformerDecoderLayer(
                     d_model,
                     d_ffn,
                     n_heads,
                     d_k,
                     d_v,
                     ScaledDotProductAttention(d_k**0.5, attn_dropout),
                     ScaledDotProductAttention(d_k**0.5, attn_dropout),
```

### Comparing `pypots-0.4/pypots/nn/modules/transformer/embedding.py` & `pypots-0.4.1/pypots/nn/modules/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/nn/modules/transformer/layers.py` & `pypots-0.4.1/pypots/nn/modules/transformer/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         # apply residual connection
         x += residual
         # apply layer-norm
         x = self.layer_norm(x)
         return x
 
 
-class EncoderLayer(nn.Module):
+class TransformerEncoderLayer(nn.Module):
     """Transformer encoder layer.
 
     Parameters
     ----------
     d_model:
         The dimension of the input tensor.
 
@@ -149,15 +149,15 @@
         # apply layer-norm
         enc_output = self.layer_norm(enc_output)
 
         enc_output = self.pos_ffn(enc_output)
         return enc_output, attn_weights
 
 
-class DecoderLayer(nn.Module):
+class TransformerDecoderLayer(nn.Module):
     """Transformer decoder layer.
 
     Parameters
     ----------
     d_model:
         The dimension of the input tensor.
```

### Comparing `pypots-0.4/pypots/optim/adadelta.py` & `pypots-0.4.1/pypots/optim/adadelta.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/adagrad.py` & `pypots-0.4.1/pypots/optim/adagrad.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/adam.py` & `pypots-0.4.1/pypots/optim/adam.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/adamw.py` & `pypots-0.4.1/pypots/optim/adamw.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/base.py` & `pypots-0.4.1/pypots/optim/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/__init__.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/base.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/base.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/constant_lrs.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/constant_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/exponential_lrs.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/exponential_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/lambda_lrs.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/lambda_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/linear_lrs.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/linear_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/multiplicative_lrs.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/multiplicative_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/multistep_lrs.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/multistep_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/lr_scheduler/step_lrs.py` & `pypots-0.4.1/pypots/optim/lr_scheduler/step_lrs.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/rmsprop.py` & `pypots-0.4.1/pypots/optim/rmsprop.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/optim/sgd.py` & `pypots-0.4.1/pypots/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/utils/file.py` & `pypots-0.4.1/pypots/utils/file.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/utils/metrics/classification.py` & `pypots-0.4.1/pypots/utils/metrics/classification.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 # License: BSD-3-Clause
 
 from typing import Tuple
 
 import numpy as np
 from sklearn import metrics
 
-from ..logging import logger
-
 
 def calc_binary_classification_metrics(
     prob_predictions: np.ndarray,
     targets: np.ndarray,
     pos_label: int = 1,
 ) -> dict:
     """Calculate the evaluation metrics for the binary classification task,
@@ -252,42 +250,7 @@
     -------
     acc_score :
         The accuracy of model predictions.
 
     """
     acc_score = metrics.accuracy_score(targets, class_predictions)
     return acc_score
-
-
-########################################################################################################################
-# Deprecated functions
-########################################################################################################################
-
-
-def cal_binary_classification_metrics(*args):
-    logger.warning(
-        "🚨 cal_binary_classification_metrics() is deprecated, "
-        "use calc_binary_classification_metrics() instead."
-    )
-    return calc_binary_classification_metrics(*args)
-
-
-def cal_precision_recall_f1(*args):
-    logger.warning(
-        "🚨 cal_precision_recall_f1() is deprecated, use calc_precision_recall_f1() instead."
-    )
-    return calc_precision_recall_f1(*args)
-
-
-def cal_pr_auc(*args):
-    logger.warning("🚨 cal_pr_auc() is deprecated, use calc_pr_auc() instead.")
-    return calc_pr_auc(*args)
-
-
-def cal_roc_auc(*args):
-    logger.warning("🚨 cal_roc_auc() is deprecated, use calc_roc_auc() instead.")
-    return calc_roc_auc(*args)
-
-
-def cal_acc(*args):
-    logger.warning("🚨 cal_acc() is deprecated, use calc_acc() instead.")
-    return calc_acc(*args)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4/pypots/utils/metrics/clustering.py` & `pypots-0.4.1/pypots/utils/metrics/clustering.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 import numpy as np
 from sklearn import metrics
 
-from ..logging import logger
-
 
 def calc_rand_index(
     class_predictions: np.ndarray,
     targets: np.ndarray,
 ) -> float:
     """Calculate Rand Index, a measure of the similarity between two data clusterings.
     Refer to :cite:`rand1971RandIndex`.
@@ -298,63 +296,7 @@
 
     internal_cluster_validation_metrics = {
         "silhouette_score": silhouette_score,
         "calinski_harabasz_score": calinski_harabasz_score,
         "davies_bouldin_score": davies_bouldin_score,
     }
     return internal_cluster_validation_metrics
-
-
-########################################################################################################################
-# Deprecated functions
-########################################################################################################################
-
-
-def cal_rand_index(*args):
-    logger.warning("🚨 Deprecated function, please use `calc_rand_index` instead.")
-    return calc_rand_index(*args)
-
-
-def cal_adjusted_rand_index(*args):
-    logger.warning(
-        "🚨 Deprecated function, please use `calc_adjusted_rand_index` instead."
-    )
-    return calc_adjusted_rand_index(*args)
-
-
-def cal_nmi(*args):
-    logger.warning("🚨 Deprecated function, please use `calc_nmi` instead.")
-    return calc_nmi(*args)
-
-
-def cal_cluster_purity(*args):
-    logger.warning("🚨 Deprecated function, please use `calc_cluster_purity` instead.")
-    return calc_cluster_purity(*args)
-
-
-def cal_external_cluster_validation_metrics(*args):
-    logger.warning(
-        "🚨 Deprecated function, please use `calc_external_cluster_validation_metrics` instead."
-    )
-    return calc_external_cluster_validation_metrics(*args)
-
-
-def cal_silhouette(*args):
-    logger.warning("🚨 Deprecated function, please use `calc_silhouette` instead.")
-    return calc_silhouette(*args)
-
-
-def cal_chs(*args):
-    logger.warning("🚨 Deprecated function, please use `calc_chs` instead.")
-    return calc_chs(*args)
-
-
-def cal_dbs(*args):
-    logger.warning("🚨 Deprecated function, please use `calc_dbs` instead.")
-    return calc_dbs(*args)
-
-
-def cal_internal_cluster_validation_metrics(*args):
-    logger.warning(
-        "🚨 Deprecated function, please use `calc_internal_cluster_validation_metrics` instead."
-    )
-    return calc_internal_cluster_validation_metrics(*args)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4/pypots/utils/metrics/error.py` & `pypots-0.4.1/pypots/utils/metrics/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 # License: BSD-3-Clause
 
 from typing import Union, Optional
 
 import numpy as np
 import torch
 
-from ..logging import logger
-
 
 def _check_inputs(
     predictions: Union[np.ndarray, torch.Tensor, list],
     targets: Union[np.ndarray, torch.Tensor, list],
     masks: Optional[Union[np.ndarray, torch.Tensor, list]] = None,
     check_shape: bool = True,
 ):
@@ -390,32 +388,7 @@
     denominator = torch.sum(torch.abs(targets * masks))
     CRPS = torch.tensor(0.0)
     for i in range(len(quantiles)):
         q_pred = torch.quantile(predictions.sum(-1), quantiles[i], dim=1)
         q_loss = calc_quantile_loss(targets, q_pred, quantiles[i], masks)
         CRPS += q_loss / denominator
     return CRPS.item() / len(quantiles)
-
-
-########################################################################################################################
-# Deprecated functions
-########################################################################################################################
-
-
-def cal_mae(*args):
-    logger.warning("🚨 cal_mae() is deprecated, use calc_mae() instead.")
-    return calc_mae(*args)
-
-
-def cal_rmse(*args):
-    logger.warning("🚨 cal_rmse() is deprecated, use calc_rmse() instead.")
-    return calc_rmse(*args)
-
-
-def cal_mse(*args):
-    logger.warning("🚨 cal_mse() is deprecated, use calc_mse() instead.")
-    return calc_mse(*args)
-
-
-def cal_mre(*args):
-    logger.warning("🚨 cal_mre() is deprecated, use calc_mre() instead.")
-    return calc_mre(*args)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pypots-0.4/pypots/utils/random.py` & `pypots-0.4.1/pypots/utils/random.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/utils/visual/clustering.py` & `pypots-0.4.1/pypots/utils/visual/clustering.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots/utils/visual/data.py` & `pypots-0.4.1/pypots/utils/visual/data.py`

 * *Files identical despite different names*

### Comparing `pypots-0.4/pypots.egg-info/PKG-INFO` & `pypots-0.4.1/pypots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.4
+Version: 0.4.1
 Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
 Home-page: https://pypots.com/
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/
 Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
@@ -221,21 +221,22 @@
 ```
 </details>
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values.
 The currently available algorithms of four tasks are cataloged in the following table with four partitions.
-The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
+The paper references are all listed at the bottom of this readme file.
 
 🌟 Since **v0.2**, all neural-network models in PyPOTS has got hyperparameter-optimization support.
 This functionality is implemented with the [Microsoft NNI](https://github.com/microsoft/nni) framework.
 
 🔥 Note that Transformer, Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation methods in their original papers,
-and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
+and they cannot accept POTS as input. **To make them applicable on POTS data, we apply the embedding strategy and training approach (ORT+MIT)
+the same as we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).**
 
 |   ***`Imputation`***   |     🚥      |                                               🚥                                                |    🚥    |
 |:----------------------:|:-----------:|:-----------------------------------------------------------------------------------------------:|:--------:|
 |        **Type**        |  **Abbr.**  |                              **Full name of the algorithm/model**                               | **Year** |
 |       Neural Net       |    SAITS    |                      Self-Attention-based Imputation for Time Series [^1]                       |   2023   |
 |       Neural Net       | Transformer |                                 Attention is All you Need [^2]                                  |   2017   |
 |       Neural Net       | Crossformer | Transformer Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting [^16] |   2023   |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.4 Summary: A Python Toolbox for
+Metadata-Version: 2.1 Name: pypots Version: 0.4.1 Summary: A Python Toolbox for
 Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
 Author: Wenjie Du Author-email: wenjay.du@gmail.com License: BSD-3-Clause
 Project-URL: Documentation, https://docs.pypots.com/ Project-URL: Source,
 https://github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/
 WenjieDu/PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/
 PyPOTS/archive/main.zip Keywords: data science,data mining,neural
 networks,machine learning,deep learning,artificial intelligence,time-series
@@ -115,61 +115,61 @@
 values indicating_mask = np.isnan(X) ^ np.isnan(X_ori) # indicating mask for
 imputation error calculation mae = calc_mae(imputation, np.nan_to_num(X_ori),
 indicating_mask) # calculate mean absolute error on the ground truth
 (artificially-missing values) ``` ## â Available Algorithms PyPOTS supports
 imputation, classification, clustering, and forecasting tasks on multivariate
 time series with missing values. The currently available algorithms of four
 tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. Please refer to
-them if you want more details. ð Since **v0.2**, all neural-network models
-in PyPOTS has got hyperparameter-optimization support. This functionality is
-implemented with the [Microsoft NNI](https://github.com/microsoft/nni)
-framework. ð¥ Note that Transformer, Crossformer, PatchTST, DLinear,
-ETSformer, FEDformer, Informer, Autoformer are not proposed as imputation
-methods in their original papers, and they cannot accept POTS as input. **To
-make them applicable on POTS data, we apply the embedding strategy the same as
-we did in [SAITS paper](https://arxiv.org/pdf/2202.08516).** |
-***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:----------------------:|:----------
--:|:---------------------------------------------------------------------------
---------------------:|:--------:| | **Type** | **Abbr.** | **Full name of the
-algorithm/model** | **Year** | | Neural Net | SAITS | Self-Attention-based
-Imputation for Time Series [^1] | 2023 | | Neural Net | Transformer | Attention
-is All you Need [^2] | 2017 | | Neural Net | Crossformer | Transformer
-Utilizing Cross-Dimension Dependency for Multivariate Time Series Forecasting
-[^16] | 2023 | | Neural Net | TimesNet | Temporal 2D-Variation Modeling for
-General Time Series Analysis [^14] | 2023 | | Neural Net | PatchTST | A Time
-Series is Worth 64 Words: Long-Term Forecasting with Transformers [^18] | 2023
-| | Neural Net | DLinear | Are Transformers Effective for Time Series
-Forecasting? [^17] | 2023 | | Neural Net | ETSformer | Exponential Smoothing
-Transformers for Time-series Forecasting [^19] | 2023 | | Neural Net |
-FEDformer | Frequency Enhanced Decomposed Transformer for Long-term Series
-Forecasting [^20] | 2022 | | Neural Net | Informer | Beyond Efficient
-Transformer for Long Sequence Time-Series Forecasting [^21] | 2021 | | Neural
-Net | Autoformer | Decomposition Transformers with Auto-Correlation for Long-
-Term Series Forecasting [^15] | 2021 | | Neural Net | CSDI | Conditional Score-
-based Diffusion Models for Probabilistic Time Series Imputation [^12] | 2021 |
-| Neural Net | US-GAN | Unsupervised GAN for Multivariate Time Series
-Imputation [^10] | 2021 | | Neural Net | GP-VAE | Gaussian Process Variational
-Autoencoder [^11] | 2020 | | Neural Net | BRITS | Bidirectional Recurrent
-Imputation for Time Series [^3] | 2018 | | Neural Net | M-RNN | Multi-
-directional Recurrent Neural Network [^9] | 2019 | | Naive | LOCF/NOCB | Last
-Observation Carried Forward / Next Observation Carried Backward | - | | Naive |
-Median | Median Value Imputation | - | | Naive | Mean | Mean Value Imputation |
-- | | ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** |
-**Full name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
-Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
-GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
-Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
-Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
-| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Neural Net | CRLI | Clustering Representation
-Learning on Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER |
-Variational Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`***
-| ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
-model/paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
+references are all listed at the bottom of this readme file. ð Since
+**v0.2**, all neural-network models in PyPOTS has got hyperparameter-
+optimization support. This functionality is implemented with the [Microsoft
+NNI](https://github.com/microsoft/nni) framework. ð¥ Note that Transformer,
+Crossformer, PatchTST, DLinear, ETSformer, FEDformer, Informer, Autoformer are
+not proposed as imputation methods in their original papers, and they cannot
+accept POTS as input. **To make them applicable on POTS data, we apply the
+embedding strategy and training approach (ORT+MIT) the same as we did in [SAITS
+paper](https://arxiv.org/pdf/2202.08516).** | ***`Imputation`*** | ð¥ | ð¥
+| ð¥ | |:----------------------:|:-----------:|:-----------------------------
+------------------------------------------------------------------:|:--------:
+| | **Type** | **Abbr.** | **Full name of the algorithm/model** | **Year** | |
+Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
+2023 | | Neural Net | Transformer | Attention is All you Need [^2] | 2017 | |
+Neural Net | Crossformer | Transformer Utilizing Cross-Dimension Dependency for
+Multivariate Time Series Forecasting [^16] | 2023 | | Neural Net | TimesNet |
+Temporal 2D-Variation Modeling for General Time Series Analysis [^14] | 2023 |
+| Neural Net | PatchTST | A Time Series is Worth 64 Words: Long-Term
+Forecasting with Transformers [^18] | 2023 | | Neural Net | DLinear | Are
+Transformers Effective for Time Series Forecasting? [^17] | 2023 | | Neural Net
+| ETSformer | Exponential Smoothing Transformers for Time-series Forecasting
+[^19] | 2023 | | Neural Net | FEDformer | Frequency Enhanced Decomposed
+Transformer for Long-term Series Forecasting [^20] | 2022 | | Neural Net |
+Informer | Beyond Efficient Transformer for Long Sequence Time-Series
+Forecasting [^21] | 2021 | | Neural Net | Autoformer | Decomposition
+Transformers with Auto-Correlation for Long-Term Series Forecasting [^15] |
+2021 | | Neural Net | CSDI | Conditional Score-based Diffusion Models for
+Probabilistic Time Series Imputation [^12] | 2021 | | Neural Net | US-GAN |
+Unsupervised GAN for Multivariate Time Series Imputation [^10] | 2021 | |
+Neural Net | GP-VAE | Gaussian Process Variational Autoencoder [^11] | 2020 | |
+Neural Net | BRITS | Bidirectional Recurrent Imputation for Time Series [^3] |
+2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural Network [^9] |
+2019 | | Naive | LOCF/NOCB | Last Observation Carried Forward / Next
+Observation Carried Backward | - | | Naive | Median | Median Value Imputation |
+- | | Naive | Mean | Mean Value Imputation | - | | ***`Classification`*** |
+ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
+model/paper** | **Year** | | Neural Net | BRITS | Bidirectional Recurrent
+Imputation for Time Series [^3] | 2018 | | Neural Net | GRU-D | Recurrent
+Neural Networks for Multivariate Time Series with Missing Values [^4] | 2018 |
+| Neural Net | Raindrop | Graph-Guided Network for Irregularly Sampled
+Multivariate Time Series [^5] | 2022 | | ***`Clustering`*** | ð¥ | ð¥ |
+ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/paper** |
+**Year** | | Neural Net | CRLI | Clustering Representation Learning on
+Incomplete time-series data [^6] | 2021 | | Neural Net | VaDER | Variational
+Deep Embedding with Recurrence [^7] | 2019 | | ***`Forecasting`*** | ð¥ |
+ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/model/
+paper** | **Year** | | Probabilistic | BTTF | Bayesian Temporal Tensor
 Factorization [^8] | 2021 | ## â Citing PyPOTS > [!TIP] > **[Updates in Feb
 2024]** ð Our survey paper [Deep Learning for Multivariate Time Series
 Imputation: A Survey](https://arxiv.org/abs/2402.04059) has been released on
 arXiv. The code is open source in the GitHub repo [Awesome_Imputation](https://
 github.com/WenjieDu/Awesome_Imputation). We comprehensively review the
 literature of the state-of-the-art deep-learning imputation methods for time
 series, provide a taxonomy for them, and discuss the challenges and future
```

### Comparing `pypots-0.4/pypots.egg-info/SOURCES.txt` & `pypots-0.4.1/pypots.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,175 +10,190 @@
 pypots.egg-info/dependency_links.txt
 pypots.egg-info/entry_points.txt
 pypots.egg-info/requires.txt
 pypots.egg-info/top_level.txt
 pypots/classification/__init__.py
 pypots/classification/base.py
 pypots/classification/brits/__init__.py
+pypots/classification/brits/core.py
 pypots/classification/brits/data.py
 pypots/classification/brits/model.py
-pypots/classification/brits/modules/__init__.py
-pypots/classification/brits/modules/core.py
 pypots/classification/grud/__init__.py
+pypots/classification/grud/core.py
 pypots/classification/grud/data.py
 pypots/classification/grud/model.py
-pypots/classification/grud/modules/__init__.py
-pypots/classification/grud/modules/core.py
 pypots/classification/raindrop/__init__.py
+pypots/classification/raindrop/core.py
 pypots/classification/raindrop/data.py
 pypots/classification/raindrop/model.py
-pypots/classification/raindrop/modules/__init__.py
-pypots/classification/raindrop/modules/core.py
-pypots/classification/raindrop/modules/submodules.py
 pypots/cli/__init__.py
 pypots/cli/base.py
 pypots/cli/dev.py
 pypots/cli/doc.py
 pypots/cli/env.py
 pypots/cli/pypots_cli.py
 pypots/cli/tuning.py
 pypots/cli/utils.py
 pypots/clustering/__init__.py
 pypots/clustering/base.py
 pypots/clustering/crli/__init__.py
+pypots/clustering/crli/core.py
 pypots/clustering/crli/data.py
 pypots/clustering/crli/model.py
-pypots/clustering/crli/modules/__init__.py
-pypots/clustering/crli/modules/core.py
-pypots/clustering/crli/modules/submodules.py
 pypots/clustering/vader/__init__.py
+pypots/clustering/vader/core.py
 pypots/clustering/vader/data.py
 pypots/clustering/vader/model.py
-pypots/clustering/vader/modules/__init__.py
-pypots/clustering/vader/modules/core.py
-pypots/clustering/vader/modules/submodules.py
 pypots/data/__init__.py
 pypots/data/base.py
 pypots/data/checking.py
 pypots/data/generating.py
 pypots/data/load_preprocessing.py
 pypots/data/load_specific_datasets.py
 pypots/data/utils.py
 pypots/data/saving/__init__.py
 pypots/data/saving/h5.py
 pypots/data/saving/pickle.py
 pypots/forecasting/__init__.py
 pypots/forecasting/base.py
 pypots/forecasting/bttf/__init__.py
+pypots/forecasting/bttf/core.py
 pypots/forecasting/bttf/model.py
-pypots/forecasting/bttf/modules/__init__.py
-pypots/forecasting/bttf/modules/core.py
-pypots/forecasting/bttf/modules/submodules.py
+pypots/forecasting/bttf/submodules.py
 pypots/imputation/__init__.py
 pypots/imputation/base.py
 pypots/imputation/autoformer/__init__.py
+pypots/imputation/autoformer/core.py
 pypots/imputation/autoformer/data.py
 pypots/imputation/autoformer/model.py
-pypots/imputation/autoformer/modules/__init__.py
-pypots/imputation/autoformer/modules/core.py
-pypots/imputation/autoformer/modules/submodules.py
 pypots/imputation/brits/__init__.py
+pypots/imputation/brits/core.py
 pypots/imputation/brits/data.py
 pypots/imputation/brits/model.py
-pypots/imputation/brits/modules/__init__.py
-pypots/imputation/brits/modules/core.py
-pypots/imputation/brits/modules/submodules.py
 pypots/imputation/crossformer/__init__.py
+pypots/imputation/crossformer/core.py
 pypots/imputation/crossformer/data.py
 pypots/imputation/crossformer/model.py
-pypots/imputation/crossformer/modules/__init__.py
-pypots/imputation/crossformer/modules/core.py
-pypots/imputation/crossformer/modules/submodules.py
 pypots/imputation/csdi/__init__.py
+pypots/imputation/csdi/core.py
 pypots/imputation/csdi/data.py
 pypots/imputation/csdi/model.py
-pypots/imputation/csdi/modules/__init__.py
-pypots/imputation/csdi/modules/core.py
-pypots/imputation/csdi/modules/submodules.py
 pypots/imputation/dlinear/__init__.py
+pypots/imputation/dlinear/core.py
 pypots/imputation/dlinear/data.py
 pypots/imputation/dlinear/model.py
-pypots/imputation/dlinear/modules/__init__.py
-pypots/imputation/dlinear/modules/core.py
 pypots/imputation/etsformer/__init__.py
+pypots/imputation/etsformer/core.py
 pypots/imputation/etsformer/data.py
 pypots/imputation/etsformer/model.py
-pypots/imputation/etsformer/modules/__init__.py
-pypots/imputation/etsformer/modules/core.py
-pypots/imputation/etsformer/modules/submodules.py
 pypots/imputation/fedformer/__init__.py
+pypots/imputation/fedformer/core.py
 pypots/imputation/fedformer/data.py
 pypots/imputation/fedformer/model.py
-pypots/imputation/fedformer/modules/__init__.py
-pypots/imputation/fedformer/modules/core.py
-pypots/imputation/fedformer/modules/submodules.py
 pypots/imputation/gpvae/__init__.py
+pypots/imputation/gpvae/core.py
 pypots/imputation/gpvae/data.py
 pypots/imputation/gpvae/model.py
-pypots/imputation/gpvae/modules/__init__.py
-pypots/imputation/gpvae/modules/core.py
-pypots/imputation/gpvae/modules/submodules.py
 pypots/imputation/informer/__init__.py
+pypots/imputation/informer/core.py
 pypots/imputation/informer/data.py
 pypots/imputation/informer/model.py
-pypots/imputation/informer/modules/__init__.py
-pypots/imputation/informer/modules/core.py
-pypots/imputation/informer/modules/submodules.py
 pypots/imputation/locf/__init__.py
+pypots/imputation/locf/core.py
 pypots/imputation/locf/model.py
-pypots/imputation/locf/modules/__init__.py
-pypots/imputation/locf/modules/core.py
 pypots/imputation/mean/__init__.py
 pypots/imputation/mean/model.py
 pypots/imputation/median/__init__.py
 pypots/imputation/median/model.py
 pypots/imputation/mrnn/__init__.py
+pypots/imputation/mrnn/core.py
 pypots/imputation/mrnn/data.py
 pypots/imputation/mrnn/model.py
-pypots/imputation/mrnn/modules/__init__.py
-pypots/imputation/mrnn/modules/core.py
-pypots/imputation/mrnn/modules/submodules.py
 pypots/imputation/patchtst/__init__.py
+pypots/imputation/patchtst/core.py
 pypots/imputation/patchtst/data.py
 pypots/imputation/patchtst/model.py
-pypots/imputation/patchtst/modules/__init__.py
-pypots/imputation/patchtst/modules/core.py
-pypots/imputation/patchtst/modules/submodules.py
 pypots/imputation/saits/__init__.py
+pypots/imputation/saits/core.py
 pypots/imputation/saits/data.py
 pypots/imputation/saits/model.py
-pypots/imputation/saits/modules/__init__.py
-pypots/imputation/saits/modules/core.py
 pypots/imputation/timesnet/__init__.py
+pypots/imputation/timesnet/core.py
 pypots/imputation/timesnet/data.py
 pypots/imputation/timesnet/model.py
-pypots/imputation/timesnet/modules/__init__.py
-pypots/imputation/timesnet/modules/core.py
-pypots/imputation/timesnet/modules/submodules.py
 pypots/imputation/transformer/__init__.py
+pypots/imputation/transformer/core.py
 pypots/imputation/transformer/data.py
 pypots/imputation/transformer/model.py
-pypots/imputation/transformer/modules/__init__.py
-pypots/imputation/transformer/modules/core.py
 pypots/imputation/usgan/__init__.py
+pypots/imputation/usgan/core.py
 pypots/imputation/usgan/data.py
 pypots/imputation/usgan/model.py
-pypots/imputation/usgan/modules/__init__.py
-pypots/imputation/usgan/modules/core.py
-pypots/imputation/usgan/modules/submodules.py
 pypots/nn/__init__.py
 pypots/nn/functional/__init__.py
 pypots/nn/functional/normalization.py
 pypots/nn/modules/__init__.py
-pypots/nn/modules/rnn.py
+pypots/nn/modules/autoformer/__init__.py
+pypots/nn/modules/autoformer/auto_encoder.py
+pypots/nn/modules/autoformer/layers.py
+pypots/nn/modules/brits/__init__.py
+pypots/nn/modules/brits/backbone.py
+pypots/nn/modules/brits/layers.py
+pypots/nn/modules/crli/__init__.py
+pypots/nn/modules/crli/backbone.py
+pypots/nn/modules/crli/layers.py
+pypots/nn/modules/crossformer/__init__.py
+pypots/nn/modules/crossformer/auto_encoder.py
+pypots/nn/modules/crossformer/layers.py
+pypots/nn/modules/csdi/__init__.py
+pypots/nn/modules/csdi/backbone.py
+pypots/nn/modules/csdi/layers.py
+pypots/nn/modules/dlinear/__init__.py
+pypots/nn/modules/dlinear/backbone.py
+pypots/nn/modules/etsformer/__init__.py
+pypots/nn/modules/etsformer/auto_encoder.py
+pypots/nn/modules/etsformer/layers.py
+pypots/nn/modules/fedformer/__init__.py
+pypots/nn/modules/fedformer/autoencoder.py
+pypots/nn/modules/fedformer/layers.py
+pypots/nn/modules/gpvae/__init__.py
+pypots/nn/modules/gpvae/backbone.py
+pypots/nn/modules/gpvae/layers.py
+pypots/nn/modules/grud/__init__.py
+pypots/nn/modules/grud/backbone.py
+pypots/nn/modules/grud/layers.py
+pypots/nn/modules/informer/__init__.py
+pypots/nn/modules/informer/auto_encoder.py
+pypots/nn/modules/informer/layers.py
+pypots/nn/modules/mrnn/__init__.py
+pypots/nn/modules/mrnn/backbone.py
+pypots/nn/modules/mrnn/layers.py
+pypots/nn/modules/patchtst/__init__.py
+pypots/nn/modules/patchtst/auto_encoder.py
+pypots/nn/modules/patchtst/layers.py
+pypots/nn/modules/raindrop/__init__.py
+pypots/nn/modules/raindrop/backbone.py
+pypots/nn/modules/raindrop/layers.py
+pypots/nn/modules/saits/__init__.py
+pypots/nn/modules/saits/backbone.py
+pypots/nn/modules/saits/loss.py
+pypots/nn/modules/timesnet/__init__.py
+pypots/nn/modules/timesnet/backbone.py
+pypots/nn/modules/timesnet/layers.py
 pypots/nn/modules/transformer/__init__.py
 pypots/nn/modules/transformer/attention.py
 pypots/nn/modules/transformer/auto_encoder.py
 pypots/nn/modules/transformer/embedding.py
 pypots/nn/modules/transformer/layers.py
+pypots/nn/modules/usgan/__init__.py
+pypots/nn/modules/usgan/backbone.py
+pypots/nn/modules/usgan/layers.py
+pypots/nn/modules/vader/__init__.py
+pypots/nn/modules/vader/backbone.py
+pypots/nn/modules/vader/layers.py
 pypots/optim/__init__.py
 pypots/optim/adadelta.py
 pypots/optim/adagrad.py
 pypots/optim/adam.py
 pypots/optim/adamw.py
 pypots/optim/base.py
 pypots/optim/rmsprop.py
```

### Comparing `pypots-0.4/pypots.egg-info/requires.txt` & `pypots-0.4.1/pypots.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pypots-0.4/setup.cfg` & `pypots-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pypots-0.4/setup.py` & `pypots-0.4.1/setup.py`

 * *Files identical despite different names*

