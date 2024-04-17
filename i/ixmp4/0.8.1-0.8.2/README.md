# Comparing `tmp/ixmp4-0.8.1.tar.gz` & `tmp/ixmp4-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixmp4-0.8.1.tar", max compression
+gzip compressed data, was "ixmp4-0.8.2.tar", max compression
```

## Comparing `ixmp4-0.8.1.tar` & `ixmp4-0.8.2.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0     1067 2024-04-16 11:25:24.345074 ixmp4-0.8.1/LICENSE
--rw-r--r--   0        0        0     3561 2024-04-16 11:25:24.345074 ixmp4-0.8.1/README.md
--rw-r--r--   0        0        0      800 2024-04-16 11:25:48.353925 ixmp4-0.8.1/ixmp4/__init__.py
--rw-r--r--   0        0        0       64 2024-04-16 11:25:24.345074 ixmp4-0.8.1/ixmp4/__main__.py
--rw-r--r--   0        0        0     2724 2024-04-16 11:25:24.345074 ixmp4-0.8.1/ixmp4/cli/__init__.py
--rw-r--r--   0        0        0     9357 2024-04-16 11:25:24.345074 ixmp4-0.8.1/ixmp4/cli/platforms.py
--rw-r--r--   0        0        0     1130 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/cli/server.py
--rw-r--r--   0        0        0      393 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/cli/utils.py
--rw-r--r--   0        0        0      243 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/__init__.py
--rw-r--r--   0        0        0     4877 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/auth.py
--rw-r--r--   0        0        0      271 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/base.py
--rw-r--r--   0        0        0      827 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/credentials.py
--rw-r--r--   0        0        0      337 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/logging/debug.conf
--rw-r--r--   0        0        0      336 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/logging/development.conf
--rw-r--r--   0        0        0      413 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/logging/production.conf
--rw-r--r--   0        0        0     1301 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/logging/server.conf
--rw-r--r--   0        0        0     6326 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/manager.py
--rw-r--r--   0        0        0     5051 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/settings.py
--rw-r--r--   0        0        0     1857 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/toml.py
--rw-r--r--   0        0        0      468 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/conf/user.py
--rw-r--r--   0        0        0      432 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/__init__.py
--rw-r--r--   0        0        0      656 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/base.py
--rw-r--r--   0        0        0      525 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/decorators.py
--rw-r--r--   0        0        0     4419 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/exceptions.py
--rw-r--r--   0        0        0       64 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/iamc/__init__.py
--rw-r--r--   0        0        0     5596 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/iamc/data.py
--rw-r--r--   0        0        0     3658 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/iamc/variable.py
--rw-r--r--   0        0        0      381 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/meta.py
--rw-r--r--   0        0        0     3434 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/model.py
--rw-r--r--   0        0        0       35 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/__init__.py
--rw-r--r--   0        0        0      762 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/data.py
--rw-r--r--   0        0        0     3180 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/indexset.py
--rw-r--r--   0        0        0     4245 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/scalar.py
--rw-r--r--   0        0        0     3519 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/optimization/table.py
--rw-r--r--   0        0        0     2905 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/platform.py
--rw-r--r--   0        0        0     4565 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/region.py
--rw-r--r--   0        0        0     4566 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/run.py
--rw-r--r--   0        0        0     3568 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/scenario.py
--rw-r--r--   0        0        0     4245 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/unit.py
--rw-r--r--   0        0        0      708 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/core/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/__init__.py
--rw-r--r--   0        0        0     1041 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/__init__.py
--rw-r--r--   0        0        0     2080 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/base.py
--rw-r--r--   0        0        0     2849 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/docs.py
--rw-r--r--   0        0        0      308 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/__init__.py
--rw-r--r--   0        0        0     4620 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/datapoint.py
--rw-r--r--   0        0        0     1137 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/measurand.py
--rw-r--r--   0        0        0     4890 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/timeseries.py
--rw-r--r--   0        0        0     2659 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/iamc/variable.py
--rw-r--r--   0        0        0     5045 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/meta.py
--rw-r--r--   0        0        0     2704 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/model.py
--rw-r--r--   0        0        0      165 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/__init__.py
--rw-r--r--   0        0        0      798 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/column.py
--rw-r--r--   0        0        0     3833 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/indexset.py
--rw-r--r--   0        0        0     4709 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/scalar.py
--rw-r--r--   0        0        0     6019 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/optimization/table.py
--rw-r--r--   0        0        0     4104 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/region.py
--rw-r--r--   0        0        0     5775 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/run.py
--rw-r--r--   0        0        0     2693 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/scenario.py
--rw-r--r--   0        0        0     3692 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/abstract/unit.py
--rw-r--r--   0        0        0      750 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/__init__.py
--rw-r--r--   0        0        0    13984 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/base.py
--rw-r--r--   0        0        0     1160 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/docs.py
--rw-r--r--   0        0        0      255 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/iamc/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/iamc/datapoint.py
--rw-r--r--   0        0        0     1589 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/iamc/timeseries.py
--rw-r--r--   0        0        0     1483 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/iamc/variable.py
--rw-r--r--   0        0        0     1766 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/meta.py
--rw-r--r--   0        0        0     1417 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/model.py
--rw-r--r--   0        0        0      138 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/__init__.py
--rw-r--r--   0        0        0      474 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/column.py
--rw-r--r--   0        0        0     2052 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/indexset.py
--rw-r--r--   0        0        0     2282 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/scalar.py
--rw-r--r--   0        0        0     2376 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/optimization/table.py
--rw-r--r--   0        0        0     1675 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/region.py
--rw-r--r--   0        0        0     2214 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/run.py
--rw-r--r--   0        0        0     1470 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/scenario.py
--rw-r--r--   0        0        0     1593 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/api/unit.py
--rw-r--r--   0        0        0     3679 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/auth/context.py
--rw-r--r--   0        0        0     1465 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/auth/decorators.py
--rw-r--r--   0        0        0      141 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/backend/__init__.py
--rw-r--r--   0        0        0     6207 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/backend/api.py
--rw-r--r--   0        0        0     1234 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/backend/base.py
--rw-r--r--   0        0        0     4761 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/backend/db.py
--rw-r--r--   0        0        0      874 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/db/__init__.py
--rw-r--r--   0        0        0    15233 2024-04-16 11:25:24.349074 ixmp4-0.8.1/ixmp4/data/db/base.py
--rw-r--r--   0        0        0     3459 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/docs.py
--rw-r--r--   0        0        0      502 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/__init__.py
--rw-r--r--   0        0        0      528 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/meta.py
--rw-r--r--   0        0        0      391 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/model.py
--rw-r--r--   0        0        0      440 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/optimizationcolumn.py
--rw-r--r--   0        0        0      448 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/optimizationindexset.py
--rw-r--r--   0        0        0      581 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/optimizationscalar.py
--rw-r--r--   0        0        0      436 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/optimizationtable.py
--rw-r--r--   0        0        0      385 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/region.py
--rw-r--r--   0        0        0      776 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/run.py
--rw-r--r--   0        0        0      409 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/scenario.py
--rw-r--r--   0        0        0      419 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/timeseries.py
--rw-r--r--   0        0        0      470 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/unit.py
--rw-r--r--   0        0        0      490 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/filters/variable.py
--rw-r--r--   0        0        0      331 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/base.py
--rw-r--r--   0        0        0      129 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/__init__.py
--rw-r--r--   0        0        0     5896 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/filter.py
--rw-r--r--   0        0        0     1356 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/model.py
--rw-r--r--   0        0        0     7583 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/repository.py
--rw-r--r--   0        0        0     2917 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/measurand.py
--rw-r--r--   0        0        0       75 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/__init__.py
--rw-r--r--   0        0        0      401 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/filter.py
--rw-r--r--   0        0        0     1160 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/model.py
--rw-r--r--   0        0        0     4440 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/repository.py
--rw-r--r--   0        0        0       86 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/__init__.py
--rw-r--r--   0        0        0      235 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/docs.py
--rw-r--r--   0        0        0      806 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/filter.py
--rw-r--r--   0        0        0      584 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/model.py
--rw-r--r--   0        0        0     1444 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/iamc/variable/repository.py
--rw-r--r--   0        0        0       79 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/meta/__init__.py
--rw-r--r--   0        0        0      570 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/meta/filter.py
--rw-r--r--   0        0        0     2246 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/meta/model.py
--rw-r--r--   0        0        0     6937 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/meta/repository.py
--rw-r--r--   0        0        0      118 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/__init__.py
--rw-r--r--   0        0        0      426 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/docs.py
--rw-r--r--   0        0        0     1780 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/filter.py
--rw-r--r--   0        0        0      517 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/model.py
--rw-r--r--   0        0        0     1371 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/model/repository.py
--rw-r--r--   0        0        0      183 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/__init__.py
--rw-r--r--   0        0        0      310 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/base.py
--rw-r--r--   0        0        0       67 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/__init__.py
--rw-r--r--   0        0        0      225 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/docs.py
--rw-r--r--   0        0        0      692 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/filter.py
--rw-r--r--   0        0        0     1170 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/model.py
--rw-r--r--   0        0        0     2440 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/column/repository.py
--rw-r--r--   0        0        0       71 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/__init__.py
--rw-r--r--   0        0        0      235 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/docs.py
--rw-r--r--   0        0        0      534 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/filter.py
--rw-r--r--   0        0        0     1278 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/model.py
--rw-r--r--   0        0        0     2348 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/repository.py
--rw-r--r--   0        0        0       67 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/__init__.py
--rw-r--r--   0        0        0      225 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/docs.py
--rw-r--r--   0        0        0      809 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/filter.py
--rw-r--r--   0        0        0     1084 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/model.py
--rw-r--r--   0        0        0     2552 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/repository.py
--rw-r--r--   0        0        0       65 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/__init__.py
--rw-r--r--   0        0        0      220 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/docs.py
--rw-r--r--   0        0        0      522 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/filter.py
--rw-r--r--   0        0        0     3554 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/model.py
--rw-r--r--   0        0        0     5079 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/optimization/table/repository.py
--rw-r--r--   0        0        0      121 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/__init__.py
--rw-r--r--   0        0        0      496 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/docs.py
--rw-r--r--   0        0        0     1547 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/filter.py
--rw-r--r--   0        0        0      611 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/model.py
--rw-r--r--   0        0        0     1569 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/region/repository.py
--rw-r--r--   0        0        0       61 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/run/__init__.py
--rw-r--r--   0        0        0     1254 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/run/filter.py
--rw-r--r--   0        0        0     1563 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/run/model.py
--rw-r--r--   0        0        0     5064 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/run/repository.py
--rw-r--r--   0        0        0      127 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/__init__.py
--rw-r--r--   0        0        0      222 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/docs.py
--rw-r--r--   0        0        0     1827 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/filter.py
--rw-r--r--   0        0        0      545 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/model.py
--rw-r--r--   0        0        0     1814 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/scenario/repository.py
--rw-r--r--   0        0        0     3331 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/timeseries.py
--rw-r--r--   0        0        0      126 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/__init__.py
--rw-r--r--   0        0        0      495 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/docs.py
--rw-r--r--   0        0        0     1714 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/filter.py
--rw-r--r--   0        0        0      469 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/model.py
--rw-r--r--   0        0        0     1725 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/unit/repository.py
--rw-r--r--   0        0        0      436 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/db/utils.py
--rw-r--r--   0        0        0     5531 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/generator.py
--rw-r--r--   0        0        0      292 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/data/types.py
--rw-r--r--   0        0        0     1585 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/__init__.py
--rw-r--r--   0        0        0     9465 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/filters.py
--rw-r--r--   0        0        0     2408 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/migrations/env.py
--rw-r--r--   0        0        0      509 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/migrations/script.py.mako
--rw-r--r--   0        0        0     5559 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py
--rw-r--r--   0        0        0     3777 2024-04-16 11:25:24.353074 ixmp4-0.8.1/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py
--rw-r--r--   0        0        0    19021 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py
--rw-r--r--   0        0        0     5175 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py
--rw-r--r--   0        0        0     1478 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/utils/__init__.py
--rw-r--r--   0        0        0     1496 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/utils/alembic.py
--rw-r--r--   0        0        0     1052 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/db/utils/sqlite.py
--rw-r--r--   0        0        0        0 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/py.typed
--rw-r--r--   0        0        0      297 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/__init__.py
--rw-r--r--   0        0        0     2810 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/base.py
--rw-r--r--   0        0        0      192 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/decorators.py
--rw-r--r--   0        0        0     3606 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/deps.py
--rw-r--r--   0        0        0     6969 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/docs.py
--rw-r--r--   0        0        0       61 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/__init__.py
--rw-r--r--   0        0        0     2550 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/datapoint.py
--rw-r--r--   0        0        0      921 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/model.py
--rw-r--r--   0        0        0      930 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/region.py
--rw-r--r--   0        0        0      948 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/scenario.py
--rw-r--r--   0        0        0     1916 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/timeseries.py
--rw-r--r--   0        0        0      912 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/unit.py
--rw-r--r--   0        0        0     1263 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/iamc/variable.py
--rw-r--r--   0        0        0     1976 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/meta.py
--rw-r--r--   0        0        0      696 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/middleware.py
--rw-r--r--   0        0        0     1185 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/model.py
--rw-r--r--   0        0        0       38 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/optimization/__init__.py
--rw-r--r--   0        0        0     1830 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/optimization/indexset.py
--rw-r--r--   0        0        0     1946 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/optimization/scalar.py
--rw-r--r--   0        0        0     1928 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/optimization/table.py
--rw-r--r--   0        0        0     1372 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/region.py
--rw-r--r--   0        0        0     1621 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/run.py
--rw-r--r--   0        0        0     1227 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/scenario.py
--rw-r--r--   0        0        0     1304 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/rest/unit.py
--rw-r--r--   0        0        0      187 2024-04-16 11:25:24.357074 ixmp4-0.8.1/ixmp4/server/workers.py
--rw-r--r--   0        0        0     3042 2024-04-16 11:25:48.353925 ixmp4-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 ixmp4-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-17 05:46:29.794208 ixmp4-0.8.2/LICENSE
+-rw-r--r--   0        0        0     3561 2024-04-17 05:46:29.794208 ixmp4-0.8.2/README.md
+-rw-r--r--   0        0        0      800 2024-04-17 05:46:50.962215 ixmp4-0.8.2/ixmp4/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/__main__.py
+-rw-r--r--   0        0        0     2724 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/cli/__init__.py
+-rw-r--r--   0        0        0     9357 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/cli/platforms.py
+-rw-r--r--   0        0        0     1130 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/cli/server.py
+-rw-r--r--   0        0        0      393 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/cli/utils.py
+-rw-r--r--   0        0        0      243 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/__init__.py
+-rw-r--r--   0        0        0     4877 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/auth.py
+-rw-r--r--   0        0        0      271 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/base.py
+-rw-r--r--   0        0        0      827 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/credentials.py
+-rw-r--r--   0        0        0      337 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/logging/debug.conf
+-rw-r--r--   0        0        0      336 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/logging/development.conf
+-rw-r--r--   0        0        0      413 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/logging/production.conf
+-rw-r--r--   0        0        0     1301 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/logging/server.conf
+-rw-r--r--   0        0        0     6326 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/manager.py
+-rw-r--r--   0        0        0     5051 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/settings.py
+-rw-r--r--   0        0        0     1857 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/toml.py
+-rw-r--r--   0        0        0      468 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/conf/user.py
+-rw-r--r--   0        0        0      432 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/__init__.py
+-rw-r--r--   0        0        0      656 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/base.py
+-rw-r--r--   0        0        0      525 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/decorators.py
+-rw-r--r--   0        0        0     4419 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/exceptions.py
+-rw-r--r--   0        0        0       64 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/iamc/__init__.py
+-rw-r--r--   0        0        0     5596 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/iamc/data.py
+-rw-r--r--   0        0        0     3658 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/iamc/variable.py
+-rw-r--r--   0        0        0      381 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/meta.py
+-rw-r--r--   0        0        0     3434 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/model.py
+-rw-r--r--   0        0        0       35 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/optimization/__init__.py
+-rw-r--r--   0        0        0      762 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/optimization/data.py
+-rw-r--r--   0        0        0     3180 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/optimization/indexset.py
+-rw-r--r--   0        0        0     4245 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/optimization/scalar.py
+-rw-r--r--   0        0        0     3519 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/optimization/table.py
+-rw-r--r--   0        0        0     2905 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/platform.py
+-rw-r--r--   0        0        0     4565 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/region.py
+-rw-r--r--   0        0        0     4566 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/run.py
+-rw-r--r--   0        0        0     3568 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/scenario.py
+-rw-r--r--   0        0        0     4245 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/unit.py
+-rw-r--r--   0        0        0      708 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/core/utils.py
+-rw-r--r--   0        0        0        0 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/__init__.py
+-rw-r--r--   0        0        0     2080 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/base.py
+-rw-r--r--   0        0        0     2849 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/docs.py
+-rw-r--r--   0        0        0      308 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/iamc/__init__.py
+-rw-r--r--   0        0        0     4620 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/iamc/datapoint.py
+-rw-r--r--   0        0        0     1137 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/iamc/measurand.py
+-rw-r--r--   0        0        0     4890 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/iamc/timeseries.py
+-rw-r--r--   0        0        0     2659 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/iamc/variable.py
+-rw-r--r--   0        0        0     5045 2024-04-17 05:46:29.798208 ixmp4-0.8.2/ixmp4/data/abstract/meta.py
+-rw-r--r--   0        0        0     2704 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/model.py
+-rw-r--r--   0        0        0      165 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/optimization/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/optimization/column.py
+-rw-r--r--   0        0        0     3833 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/optimization/indexset.py
+-rw-r--r--   0        0        0     4709 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/optimization/scalar.py
+-rw-r--r--   0        0        0     6019 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/optimization/table.py
+-rw-r--r--   0        0        0     4104 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/region.py
+-rw-r--r--   0        0        0     5775 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/run.py
+-rw-r--r--   0        0        0     2693 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/scenario.py
+-rw-r--r--   0        0        0     3692 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/abstract/unit.py
+-rw-r--r--   0        0        0      750 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/__init__.py
+-rw-r--r--   0        0        0    13984 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/base.py
+-rw-r--r--   0        0        0     1160 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/docs.py
+-rw-r--r--   0        0        0      255 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/iamc/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/iamc/datapoint.py
+-rw-r--r--   0        0        0     1589 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/iamc/timeseries.py
+-rw-r--r--   0        0        0     1483 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/iamc/variable.py
+-rw-r--r--   0        0        0     1766 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/meta.py
+-rw-r--r--   0        0        0     1417 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/model.py
+-rw-r--r--   0        0        0      138 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/optimization/__init__.py
+-rw-r--r--   0        0        0      474 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/optimization/column.py
+-rw-r--r--   0        0        0     2052 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/optimization/indexset.py
+-rw-r--r--   0        0        0     2282 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/optimization/scalar.py
+-rw-r--r--   0        0        0     2376 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/optimization/table.py
+-rw-r--r--   0        0        0     1675 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/region.py
+-rw-r--r--   0        0        0     2214 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/run.py
+-rw-r--r--   0        0        0     1470 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/scenario.py
+-rw-r--r--   0        0        0     1593 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/api/unit.py
+-rw-r--r--   0        0        0     3679 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/auth/context.py
+-rw-r--r--   0        0        0     1465 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/auth/decorators.py
+-rw-r--r--   0        0        0      141 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/backend/__init__.py
+-rw-r--r--   0        0        0     6207 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/backend/api.py
+-rw-r--r--   0        0        0     1234 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/backend/base.py
+-rw-r--r--   0        0        0     4761 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/backend/db.py
+-rw-r--r--   0        0        0      874 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/__init__.py
+-rw-r--r--   0        0        0    15233 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/base.py
+-rw-r--r--   0        0        0     3459 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/docs.py
+-rw-r--r--   0        0        0      502 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/meta.py
+-rw-r--r--   0        0        0      391 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/model.py
+-rw-r--r--   0        0        0      440 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/optimizationcolumn.py
+-rw-r--r--   0        0        0      448 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/optimizationindexset.py
+-rw-r--r--   0        0        0      581 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/optimizationscalar.py
+-rw-r--r--   0        0        0      436 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/optimizationtable.py
+-rw-r--r--   0        0        0      385 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/region.py
+-rw-r--r--   0        0        0      776 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/run.py
+-rw-r--r--   0        0        0      409 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/scenario.py
+-rw-r--r--   0        0        0      419 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/timeseries.py
+-rw-r--r--   0        0        0      470 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/unit.py
+-rw-r--r--   0        0        0      490 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/filters/variable.py
+-rw-r--r--   0        0        0      331 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/base.py
+-rw-r--r--   0        0        0      129 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/datapoint/__init__.py
+-rw-r--r--   0        0        0     5896 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/datapoint/filter.py
+-rw-r--r--   0        0        0     1356 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/datapoint/model.py
+-rw-r--r--   0        0        0     7583 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/datapoint/repository.py
+-rw-r--r--   0        0        0     2917 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/measurand.py
+-rw-r--r--   0        0        0       75 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/timeseries/__init__.py
+-rw-r--r--   0        0        0      401 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/timeseries/filter.py
+-rw-r--r--   0        0        0     1160 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/timeseries/model.py
+-rw-r--r--   0        0        0     4707 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/timeseries/repository.py
+-rw-r--r--   0        0        0       86 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/variable/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/variable/docs.py
+-rw-r--r--   0        0        0      806 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/variable/filter.py
+-rw-r--r--   0        0        0      584 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/variable/model.py
+-rw-r--r--   0        0        0     1444 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/iamc/variable/repository.py
+-rw-r--r--   0        0        0       79 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/meta/__init__.py
+-rw-r--r--   0        0        0      570 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/meta/filter.py
+-rw-r--r--   0        0        0     2246 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/meta/model.py
+-rw-r--r--   0        0        0     7204 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/meta/repository.py
+-rw-r--r--   0        0        0      118 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/model/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/model/docs.py
+-rw-r--r--   0        0        0     1780 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/model/filter.py
+-rw-r--r--   0        0        0      517 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/model/model.py
+-rw-r--r--   0        0        0     1371 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/model/repository.py
+-rw-r--r--   0        0        0      183 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/optimization/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/optimization/base.py
+-rw-r--r--   0        0        0       67 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/optimization/column/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/optimization/column/docs.py
+-rw-r--r--   0        0        0      692 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/optimization/column/filter.py
+-rw-r--r--   0        0        0     1170 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/optimization/column/model.py
+-rw-r--r--   0        0        0     2440 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/optimization/column/repository.py
+-rw-r--r--   0        0        0       71 2024-04-17 05:46:29.802208 ixmp4-0.8.2/ixmp4/data/db/optimization/indexset/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/indexset/docs.py
+-rw-r--r--   0        0        0      534 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/indexset/filter.py
+-rw-r--r--   0        0        0     1278 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/indexset/model.py
+-rw-r--r--   0        0        0     2348 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/indexset/repository.py
+-rw-r--r--   0        0        0       67 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/scalar/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/scalar/docs.py
+-rw-r--r--   0        0        0      809 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/scalar/filter.py
+-rw-r--r--   0        0        0     1084 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/scalar/model.py
+-rw-r--r--   0        0        0     2552 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/scalar/repository.py
+-rw-r--r--   0        0        0       65 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/table/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/table/docs.py
+-rw-r--r--   0        0        0      522 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/table/filter.py
+-rw-r--r--   0        0        0     3554 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/table/model.py
+-rw-r--r--   0        0        0     5079 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/optimization/table/repository.py
+-rw-r--r--   0        0        0      121 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/region/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/region/docs.py
+-rw-r--r--   0        0        0     1547 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/region/filter.py
+-rw-r--r--   0        0        0      611 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/region/model.py
+-rw-r--r--   0        0        0     1569 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/region/repository.py
+-rw-r--r--   0        0        0       61 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/run/__init__.py
+-rw-r--r--   0        0        0     1254 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/run/filter.py
+-rw-r--r--   0        0        0     1563 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/run/model.py
+-rw-r--r--   0        0        0     5064 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/run/repository.py
+-rw-r--r--   0        0        0      127 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/scenario/__init__.py
+-rw-r--r--   0        0        0      222 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/scenario/docs.py
+-rw-r--r--   0        0        0     1827 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/scenario/filter.py
+-rw-r--r--   0        0        0      545 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/scenario/model.py
+-rw-r--r--   0        0        0     1814 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/scenario/repository.py
+-rw-r--r--   0        0        0     3331 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/timeseries.py
+-rw-r--r--   0        0        0      126 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/unit/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/unit/docs.py
+-rw-r--r--   0        0        0     1714 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/unit/filter.py
+-rw-r--r--   0        0        0      469 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/unit/model.py
+-rw-r--r--   0        0        0     1725 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/unit/repository.py
+-rw-r--r--   0        0        0      436 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/db/utils.py
+-rw-r--r--   0        0        0     5531 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/generator.py
+-rw-r--r--   0        0        0      292 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/data/types.py
+-rw-r--r--   0        0        0     1585 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/__init__.py
+-rw-r--r--   0        0        0     9465 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/filters.py
+-rw-r--r--   0        0        0     2408 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/migrations/env.py
+-rw-r--r--   0        0        0      509 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/migrations/script.py.mako
+-rw-r--r--   0        0        0     5559 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py
+-rw-r--r--   0        0        0     3777 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py
+-rw-r--r--   0        0        0    19021 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py
+-rw-r--r--   0        0        0     5175 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py
+-rw-r--r--   0        0        0     1478 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/utils/__init__.py
+-rw-r--r--   0        0        0     1496 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/utils/alembic.py
+-rw-r--r--   0        0        0     1052 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/db/utils/sqlite.py
+-rw-r--r--   0        0        0        0 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/py.typed
+-rw-r--r--   0        0        0      297 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/__init__.py
+-rw-r--r--   0        0        0     2810 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/base.py
+-rw-r--r--   0        0        0      192 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/decorators.py
+-rw-r--r--   0        0        0     3606 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/deps.py
+-rw-r--r--   0        0        0     6969 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/docs.py
+-rw-r--r--   0        0        0       61 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/iamc/__init__.py
+-rw-r--r--   0        0        0     2550 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/iamc/datapoint.py
+-rw-r--r--   0        0        0      921 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/iamc/model.py
+-rw-r--r--   0        0        0      930 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/iamc/region.py
+-rw-r--r--   0        0        0      948 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/iamc/scenario.py
+-rw-r--r--   0        0        0     1916 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/iamc/timeseries.py
+-rw-r--r--   0        0        0      912 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/iamc/unit.py
+-rw-r--r--   0        0        0     1263 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/iamc/variable.py
+-rw-r--r--   0        0        0     1976 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/meta.py
+-rw-r--r--   0        0        0      696 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/middleware.py
+-rw-r--r--   0        0        0     1185 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/model.py
+-rw-r--r--   0        0        0       38 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/optimization/__init__.py
+-rw-r--r--   0        0        0     1830 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/optimization/indexset.py
+-rw-r--r--   0        0        0     1946 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/optimization/scalar.py
+-rw-r--r--   0        0        0     1928 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/optimization/table.py
+-rw-r--r--   0        0        0     1372 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/region.py
+-rw-r--r--   0        0        0     1621 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/run.py
+-rw-r--r--   0        0        0     1227 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/scenario.py
+-rw-r--r--   0        0        0     1304 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/rest/unit.py
+-rw-r--r--   0        0        0      187 2024-04-17 05:46:29.806208 ixmp4-0.8.2/ixmp4/server/workers.py
+-rw-r--r--   0        0        0     3135 2024-04-17 05:46:50.958215 ixmp4-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 ixmp4-0.8.2/PKG-INFO
```

### Comparing `ixmp4-0.8.1/LICENSE` & `ixmp4-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/README.md` & `ixmp4-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/__init__.py` & `ixmp4-0.8.2/ixmp4/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 from ixmp4.core import Table as Table
 from ixmp4.core.exceptions import InconsistentIamcType as InconsistentIamcType
 from ixmp4.core.exceptions import IxmpError as IxmpError
 from ixmp4.core.exceptions import NotFound as NotFound
 from ixmp4.core.exceptions import NotUnique as NotUnique
 from ixmp4.data.abstract import DataPoint as DataPoint
 
-__version__ = "0.8.1"
-__version_tuple__ = (0, 8, 1)
+__version__ = "0.8.2"
+__version_tuple__ = (0, 8, 2)
```

### Comparing `ixmp4-0.8.1/ixmp4/cli/__init__.py` & `ixmp4-0.8.2/ixmp4/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/cli/platforms.py` & `ixmp4-0.8.2/ixmp4/cli/platforms.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/cli/server.py` & `ixmp4-0.8.2/ixmp4/cli/server.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/conf/auth.py` & `ixmp4-0.8.2/ixmp4/conf/auth.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/conf/credentials.py` & `ixmp4-0.8.2/ixmp4/conf/credentials.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/conf/logging/server.conf` & `ixmp4-0.8.2/ixmp4/conf/logging/server.conf`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/conf/manager.py` & `ixmp4-0.8.2/ixmp4/conf/manager.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/conf/settings.py` & `ixmp4-0.8.2/ixmp4/conf/settings.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/conf/toml.py` & `ixmp4-0.8.2/ixmp4/conf/toml.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/base.py` & `ixmp4-0.8.2/ixmp4/core/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/decorators.py` & `ixmp4-0.8.2/ixmp4/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/exceptions.py` & `ixmp4-0.8.2/ixmp4/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/iamc/data.py` & `ixmp4-0.8.2/ixmp4/core/iamc/data.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/iamc/variable.py` & `ixmp4-0.8.2/ixmp4/core/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/model.py` & `ixmp4-0.8.2/ixmp4/core/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/optimization/data.py` & `ixmp4-0.8.2/ixmp4/core/optimization/data.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/optimization/indexset.py` & `ixmp4-0.8.2/ixmp4/core/optimization/indexset.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/optimization/scalar.py` & `ixmp4-0.8.2/ixmp4/core/optimization/scalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/optimization/table.py` & `ixmp4-0.8.2/ixmp4/core/optimization/table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/platform.py` & `ixmp4-0.8.2/ixmp4/core/platform.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/region.py` & `ixmp4-0.8.2/ixmp4/core/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/run.py` & `ixmp4-0.8.2/ixmp4/core/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/scenario.py` & `ixmp4-0.8.2/ixmp4/core/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/unit.py` & `ixmp4-0.8.2/ixmp4/core/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/core/utils.py` & `ixmp4-0.8.2/ixmp4/core/utils.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/__init__.py` & `ixmp4-0.8.2/ixmp4/data/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/base.py` & `ixmp4-0.8.2/ixmp4/data/abstract/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/docs.py` & `ixmp4-0.8.2/ixmp4/data/abstract/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/iamc/datapoint.py` & `ixmp4-0.8.2/ixmp4/data/abstract/iamc/datapoint.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/iamc/measurand.py` & `ixmp4-0.8.2/ixmp4/data/abstract/iamc/measurand.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/iamc/timeseries.py` & `ixmp4-0.8.2/ixmp4/data/abstract/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/iamc/variable.py` & `ixmp4-0.8.2/ixmp4/data/abstract/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/meta.py` & `ixmp4-0.8.2/ixmp4/data/abstract/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/model.py` & `ixmp4-0.8.2/ixmp4/data/abstract/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/optimization/column.py` & `ixmp4-0.8.2/ixmp4/data/abstract/optimization/column.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/optimization/indexset.py` & `ixmp4-0.8.2/ixmp4/data/abstract/optimization/indexset.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/optimization/scalar.py` & `ixmp4-0.8.2/ixmp4/data/abstract/optimization/scalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/optimization/table.py` & `ixmp4-0.8.2/ixmp4/data/abstract/optimization/table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/region.py` & `ixmp4-0.8.2/ixmp4/data/abstract/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/run.py` & `ixmp4-0.8.2/ixmp4/data/abstract/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/scenario.py` & `ixmp4-0.8.2/ixmp4/data/abstract/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/abstract/unit.py` & `ixmp4-0.8.2/ixmp4/data/abstract/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/__init__.py` & `ixmp4-0.8.2/ixmp4/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/base.py` & `ixmp4-0.8.2/ixmp4/data/api/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/docs.py` & `ixmp4-0.8.2/ixmp4/data/api/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/iamc/datapoint.py` & `ixmp4-0.8.2/ixmp4/data/api/iamc/datapoint.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/iamc/timeseries.py` & `ixmp4-0.8.2/ixmp4/data/api/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/iamc/variable.py` & `ixmp4-0.8.2/ixmp4/data/api/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/meta.py` & `ixmp4-0.8.2/ixmp4/data/api/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/model.py` & `ixmp4-0.8.2/ixmp4/data/api/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/optimization/indexset.py` & `ixmp4-0.8.2/ixmp4/data/api/optimization/indexset.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/optimization/scalar.py` & `ixmp4-0.8.2/ixmp4/data/api/optimization/scalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/optimization/table.py` & `ixmp4-0.8.2/ixmp4/data/api/optimization/table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/region.py` & `ixmp4-0.8.2/ixmp4/data/api/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/run.py` & `ixmp4-0.8.2/ixmp4/data/api/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/scenario.py` & `ixmp4-0.8.2/ixmp4/data/api/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/api/unit.py` & `ixmp4-0.8.2/ixmp4/data/api/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/auth/context.py` & `ixmp4-0.8.2/ixmp4/data/auth/context.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/auth/decorators.py` & `ixmp4-0.8.2/ixmp4/data/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/backend/api.py` & `ixmp4-0.8.2/ixmp4/data/backend/api.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/backend/base.py` & `ixmp4-0.8.2/ixmp4/data/backend/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/backend/db.py` & `ixmp4-0.8.2/ixmp4/data/backend/db.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/__init__.py` & `ixmp4-0.8.2/ixmp4/data/db/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/base.py` & `ixmp4-0.8.2/ixmp4/data/db/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/docs.py` & `ixmp4-0.8.2/ixmp4/data/db/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/filters/meta.py` & `ixmp4-0.8.2/ixmp4/data/db/filters/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/filters/optimizationscalar.py` & `ixmp4-0.8.2/ixmp4/data/db/filters/optimizationscalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/filters/run.py` & `ixmp4-0.8.2/ixmp4/data/db/filters/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/datapoint/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/model.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/datapoint/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/datapoint/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/datapoint/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/measurand.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/measurand.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/model.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/timeseries/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/timeseries/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/timeseries/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,17 +123,24 @@
                 variable_name=variable_name, unit__id=int(unit__id)
             )
             df["measurand__id"] = measurand.id
             df["variable"] = variable_name
             df["unit__id"] = unit__id
             return df
 
+        # ensure compatibility with pandas < 2.2
+        # TODO remove legacy-handling when dropping support for pandas < 2.2
+        if pd.__version__[0:3] in ["2.0", "2.1"]:
+            apply_args = dict()
+        else:
+            apply_args = dict(include_groups=False)
+
         return pd.DataFrame(
             df.groupby(["variable", "unit__id"], group_keys=False).apply(
-                map_measurand, include_groups=False
+                map_measurand, **apply_args
             )
         )
 
     def map_relationships(self, df: pd.DataFrame) -> pd.DataFrame:
         df = self.map_regions(df)
         df = self.map_measurands(df)
         return df
```

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/variable/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/variable/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/variable/model.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/variable/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/iamc/variable/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/iamc/variable/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/meta/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/meta/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/meta/model.py` & `ixmp4-0.8.2/ixmp4/data/db/meta/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/meta/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/meta/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,16 +187,23 @@
             type_str = df.name
             type_ = RunMetaEntry.Type(type_str)
             col = RunMetaEntry._column_map[type_]
             df["value"] = df[col]
             df["type"] = type_str
             return df.drop(columns=RunMetaEntry._column_map.values())
 
+        # ensure compatibility with pandas y 2.2
+        # TODO remove legacy-handling when dropping support for pandas < 2.2
+        if pd.__version__[0:3] in ["2.0", "2.1"]:
+            apply_args = dict()
+        else:
+            apply_args = dict(include_groups=False)
+
         return df.groupby("type", group_keys=False).apply(
-            map_value_column, include_groups=False
+            map_value_column, **apply_args
         )
 
     @check_types
     @guard("edit")
     def bulk_upsert(self, df: DataFrame[AddRunMetaEntryFrameSchema]) -> None:
         self.check_df_access(df)
         df["type"] = df["value"].map(type).map(RunMetaEntry.Type.from_pytype)
```

### Comparing `ixmp4-0.8.1/ixmp4/data/db/model/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/model/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/model/model.py` & `ixmp4-0.8.2/ixmp4/data/db/model/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/model/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/model/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/column/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/column/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/column/model.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/column/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/column/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/column/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/indexset/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/model.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/indexset/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/indexset/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/indexset/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/scalar/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/model.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/scalar/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/scalar/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/scalar/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/table/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/table/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/table/model.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/table/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/optimization/table/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/optimization/table/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/region/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/region/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/region/model.py` & `ixmp4-0.8.2/ixmp4/data/db/region/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/region/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/region/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/run/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/run/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/run/model.py` & `ixmp4-0.8.2/ixmp4/data/db/run/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/run/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/run/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/scenario/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/scenario/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/scenario/model.py` & `ixmp4-0.8.2/ixmp4/data/db/scenario/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/scenario/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/scenario/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/timeseries.py` & `ixmp4-0.8.2/ixmp4/data/db/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/unit/filter.py` & `ixmp4-0.8.2/ixmp4/data/db/unit/filter.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/db/unit/repository.py` & `ixmp4-0.8.2/ixmp4/data/db/unit/repository.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/data/generator.py` & `ixmp4-0.8.2/ixmp4/data/generator.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/__init__.py` & `ixmp4-0.8.2/ixmp4/db/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/filters.py` & `ixmp4-0.8.2/ixmp4/db/filters.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/migrations/env.py` & `ixmp4-0.8.2/ixmp4/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py` & `ixmp4-0.8.2/ixmp4/db/migrations/versions/081bbda6bb7b_create_optimization_table_table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py` & `ixmp4-0.8.2/ixmp4/db/migrations/versions/97ba231770e2_create_optimization_scalar_table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py` & `ixmp4-0.8.2/ixmp4/db/migrations/versions/c71efc396d2b_initial_migration.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py` & `ixmp4-0.8.2/ixmp4/db/migrations/versions/da1fba23f206_create_optimization_indexset_table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/utils/__init__.py` & `ixmp4-0.8.2/ixmp4/db/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/utils/alembic.py` & `ixmp4-0.8.2/ixmp4/db/utils/alembic.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/db/utils/sqlite.py` & `ixmp4-0.8.2/ixmp4/db/utils/sqlite.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/__init__.py` & `ixmp4-0.8.2/ixmp4/server/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/base.py` & `ixmp4-0.8.2/ixmp4/server/rest/base.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/deps.py` & `ixmp4-0.8.2/ixmp4/server/rest/deps.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/docs.py` & `ixmp4-0.8.2/ixmp4/server/rest/docs.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/iamc/datapoint.py` & `ixmp4-0.8.2/ixmp4/server/rest/iamc/datapoint.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/iamc/model.py` & `ixmp4-0.8.2/ixmp4/server/rest/iamc/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/iamc/region.py` & `ixmp4-0.8.2/ixmp4/server/rest/iamc/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/iamc/scenario.py` & `ixmp4-0.8.2/ixmp4/server/rest/iamc/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/iamc/timeseries.py` & `ixmp4-0.8.2/ixmp4/server/rest/iamc/timeseries.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/iamc/unit.py` & `ixmp4-0.8.2/ixmp4/server/rest/iamc/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/iamc/variable.py` & `ixmp4-0.8.2/ixmp4/server/rest/iamc/variable.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/meta.py` & `ixmp4-0.8.2/ixmp4/server/rest/meta.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/middleware.py` & `ixmp4-0.8.2/ixmp4/server/rest/middleware.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/model.py` & `ixmp4-0.8.2/ixmp4/server/rest/model.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/optimization/indexset.py` & `ixmp4-0.8.2/ixmp4/server/rest/optimization/indexset.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/optimization/scalar.py` & `ixmp4-0.8.2/ixmp4/server/rest/optimization/scalar.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/optimization/table.py` & `ixmp4-0.8.2/ixmp4/server/rest/optimization/table.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/region.py` & `ixmp4-0.8.2/ixmp4/server/rest/region.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/run.py` & `ixmp4-0.8.2/ixmp4/server/rest/run.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/scenario.py` & `ixmp4-0.8.2/ixmp4/server/rest/scenario.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/ixmp4/server/rest/unit.py` & `ixmp4-0.8.2/ixmp4/server/rest/unit.py`

 * *Files identical despite different names*

### Comparing `ixmp4-0.8.1/pyproject.toml` & `ixmp4-0.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors = [
     "Max Wolschlager <wolschlager@iiasa.ac.at>",
     "Fridolin Glatter <glatter@iiasa.ac.at>",
     "Daniel Huppmann <huppmann@iiasa.ac.at>",
     "Philip Hackstock <hackstock@iiasa.ac.at>",
 ]
 name = "ixmp4"
-version = "0.8.1"
+version = "0.8.2"
 description = "a data warehouse for scenario analysis"
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ixmp4" }, { include = "ixmp4/py.typed" }]
 homepage = "https://software.ece.iiasa.ac.at"
 repository = "https://github.com/iiasa/ixmp4"
 documentation = "https://docs.ece.iiasa.ac.at/projects/ixmp4"
@@ -19,17 +19,18 @@
 PyJWT = ">=2.4.0"
 SQLAlchemy = { extras = ["mypy"], version = ">=2.0.22" }
 SQLAlchemy-Utils = ">=0.41.0"
 alembic = ">=1.12.0"
 fastapi = ">=0.100.0"
 httpx = { extras = ["http2"], version = ">=0.25.0" }
 openpyxl = ">=3.0.9"
+# remove legacy-handling in timeseries- and meta-repositories when dropping pandas < 2.2
 pandas = [
-    {version = ">=2.1.1", python = ">=3.12"},
-    {version = ">=2.0.0", python = ">=3.10"}
+    { version = ">=2.1.1", python = ">=3.12" },
+    { version = ">=2.0.0", python = ">=3.10" }
 ]
 pandera = ">=0.17.0"
 pydantic = ">=2.3.0"
 python = ">=3.10, <3.13"
 python-dotenv = ">=1.0.1"
 typer = ">=0.9.0"
 toml = ">=0.10.2"
```

### Comparing `ixmp4-0.8.1/PKG-INFO` & `ixmp4-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ixmp4
-Version: 0.8.1
+Version: 0.8.2
 Summary: a data warehouse for scenario analysis
 Home-page: https://software.ece.iiasa.ac.at
 License: MIT
 Author: Max Wolschlager
 Author-email: wolschlager@iiasa.ac.at
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

