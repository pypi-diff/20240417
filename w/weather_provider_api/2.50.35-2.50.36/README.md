# Comparing `tmp/weather_provider_api-2.50.35.tar.gz` & `tmp/weather_provider_api-2.50.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_provider_api-2.50.35.tar", max compression
+gzip compressed data, was "weather_provider_api-2.50.36.tar", max compression
```

## Comparing `weather_provider_api-2.50.35.tar` & `weather_provider_api-2.50.36.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    17098 2024-04-17 09:39:15.841496 weather_provider_api-2.50.35/LICENSE
-drwxr-xr-x   0        0        0        0 2024-04-17 09:39:15.841496 weather_provider_api-2.50.35/LICENSES/
--rw-r--r--   0        0        0    10438 2024-04-17 09:39:15.841496 weather_provider_api-2.50.35/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    12890 2024-04-17 09:39:15.841496 weather_provider_api-2.50.35/LICENSES/CC-BY-2.5.txt
--rw-r--r--   0        0        0    15199 2024-04-17 09:39:15.841496 weather_provider_api-2.50.35/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0    11816 2024-04-17 09:39:15.841496 weather_provider_api-2.50.35/README.md
--rw-r--r--   0        0        0     3110 2024-04-17 09:39:37.917474 weather_provider_api-2.50.35/pyproject.toml
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.845496 weather_provider_api-2.50.35/weather_provider_api/__init__.py
--rw-r--r--   0        0        0     2651 2024-04-17 09:39:15.845496 weather_provider_api-2.50.35/weather_provider_api/__main__.py
--rw-r--r--   0        0        0     1821 2024-04-17 09:39:15.845496 weather_provider_api-2.50.35/weather_provider_api/app_version.py
--rw-r--r--   0        0        0     1054 2024-04-17 09:39:15.845496 weather_provider_api-2.50.35/weather_provider_api/config/__init__.py
--rw-r--r--   0        0        0      913 2024-04-17 09:39:15.845496 weather_provider_api-2.50.35/weather_provider_api/config/config.toml
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/__init__.py
--rw-r--r--   0        0        0     2995 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/application.py
--rw-r--r--   0        0        0      478 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/base_model.py
--rw-r--r--   0        0        0      135 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/exceptions/__init__.py
--rw-r--r--   0        0        0      263 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/exceptions/additional_responses.py
--rw-r--r--   0        0        0      267 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/exceptions/api_models.py
--rw-r--r--   0        0        0      704 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/exceptions/exceptions.py
--rw-r--r--   0        0        0     2278 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/gunicorn_application.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/__init__.py
--rw-r--r--   0        0        0     2157 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/cors.py
--rw-r--r--   0        0        0     2006 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/exception_handling.py
--rw-r--r--   0        0        0     1310 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/headers.py
--rw-r--r--   0        0        0     5297 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/logging_handler.py
--rw-r--r--   0        0        0     1318 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/mounting.py
--rw-r--r--   0        0        0     1642 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/prometheus.py
--rw-r--r--   0        0        0      348 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/rate_limiter.py
--rw-r--r--   0        0        0     4375 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/initializers/validation.py
--rw-r--r--   0        0        0       46 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/utils/__init__.py
--rw-r--r--   0        0        0      696 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/core/utils/example_responses.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/__init__.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/__init__.py
--rw-r--r--   0        0        0     6446 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/api_models.py
--rw-r--r--   0        0        0     5806 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/api_view_v1.py
--rw-r--r--   0        0        0     9649 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/api_view_v2.py
--rw-r--r--   0        0        0       91 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/base_models/__init__.py
--rw-r--r--   0        0        0     5975 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/base_models/model.py
--rw-r--r--   0        0        0     1135 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/base_models/source.py
--rw-r--r--   0        0        0     6686 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/controller.py
--rw-r--r--   0        0        0      726 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/exceptions.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/repository/__init__.py
--rw-r--r--   0        0        0    14191 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/repository/repository.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/__init__.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/__init__.py
--rw-r--r--   0        0        0      681 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/cds.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/__init__.py
--rw-r--r--   0        0        0    13309 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/downloader.py
--rw-r--r--   0        0        0     6408 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
--rw-r--r--   0        0        0     6840 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
--rw-r--r--   0        0        0    15187 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
--rw-r--r--   0        0        0      591 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/factors.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/models/__init__.py
--rw-r--r--   0        0        0     8711 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/models/era5land.py
--rw-r--r--   0        0        0     7833 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/__init__.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
--rw-r--r--   0        0        0     6930 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py
--rw-r--r--   0        0        0    23812 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
--rw-r--r--   0        0        0     9169 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
--rw-r--r--   0        0        0     1495 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/knmi.py
--rw-r--r--   0        0        0      421 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
--rw-r--r--   0        0        0     4963 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
--rw-r--r--   0        0        0     5320 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py
--rw-r--r--   0        0        0    15117 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
--rw-r--r--   0        0        0     4781 2024-04-17 09:39:15.849496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
--rw-r--r--   0        0        0    11062 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
--rw-r--r--   0        0        0    13328 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
--rw-r--r--   0        0        0    19917 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/stations.py
--rw-r--r--   0        0        0     7014 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/utils.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
--rw-r--r--   0        0        0     5148 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/__init__.py
--rw-r--r--   0        0        0     3048 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/date_helpers.py
--rw-r--r--   0        0        0     1397 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/file_helpers.py
--rw-r--r--   0        0        0     5742 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/geo_position.py
--rw-r--r--   0        0        0     1791 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/grid_helpers.py
--rw-r--r--   0        0        0      447 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/pandas_helpers.py
--rw-r--r--   0        0        0     5052 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/serializers.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/__init__.py
--rw-r--r--   0        0        0      393 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/erase_arome_repository.py
--rw-r--r--   0        0        0      413 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/erase_era5land_repository.py
--rw-r--r--   0        0        0      438 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/erase_era5sl_repository.py
--rw-r--r--   0        0        0      497 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/erase_waarnemingen_register.py
--rw-r--r--   0        0        0      383 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/update_arome_repository.py
--rw-r--r--   0        0        0      401 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/update_era5land_repository.py
--rw-r--r--   0        0        0      371 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/update_era5sl_repository.py
--rw-r--r--   0        0        0      462 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/scripts/update_waarnemingen_register.py
--rw-r--r--   0        0        0      140 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/versions/__init__.py
--rw-r--r--   0        0        0      796 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/versions/v1.py
--rw-r--r--   0        0        0      772 2024-04-17 09:39:15.853496 weather_provider_api-2.50.35/weather_provider_api/versions/v2.py
--rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 weather_provider_api-2.50.35/PKG-INFO
+-rw-r--r--   0        0        0    17098 2024-04-17 09:51:20.591168 weather_provider_api-2.50.36/LICENSE
+drwxr-xr-x   0        0        0        0 2024-04-17 09:51:20.591168 weather_provider_api-2.50.36/LICENSES/
+-rw-r--r--   0        0        0    10438 2024-04-17 09:51:20.591168 weather_provider_api-2.50.36/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    12890 2024-04-17 09:51:20.591168 weather_provider_api-2.50.36/LICENSES/CC-BY-2.5.txt
+-rw-r--r--   0        0        0    15199 2024-04-17 09:51:20.591168 weather_provider_api-2.50.36/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0    11816 2024-04-17 09:51:20.591168 weather_provider_api-2.50.36/README.md
+-rw-r--r--   0        0        0     3110 2024-04-17 09:51:50.547309 weather_provider_api-2.50.36/pyproject.toml
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/__init__.py
+-rw-r--r--   0        0        0     2651 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/__main__.py
+-rw-r--r--   0        0        0     1821 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/app_version.py
+-rw-r--r--   0        0        0     1054 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/config/__init__.py
+-rw-r--r--   0        0        0      913 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/config/config.toml
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/__init__.py
+-rw-r--r--   0        0        0     2995 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/application.py
+-rw-r--r--   0        0        0      478 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/base_model.py
+-rw-r--r--   0        0        0      135 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/exceptions/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/exceptions/additional_responses.py
+-rw-r--r--   0        0        0      267 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/exceptions/api_models.py
+-rw-r--r--   0        0        0      704 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2278 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/gunicorn_application.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/__init__.py
+-rw-r--r--   0        0        0     2157 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/cors.py
+-rw-r--r--   0        0        0     2006 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/exception_handling.py
+-rw-r--r--   0        0        0     1310 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/headers.py
+-rw-r--r--   0        0        0     5297 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/logging_handler.py
+-rw-r--r--   0        0        0     1318 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/mounting.py
+-rw-r--r--   0        0        0     1642 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/prometheus.py
+-rw-r--r--   0        0        0      348 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/rate_limiter.py
+-rw-r--r--   0        0        0     4375 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/initializers/validation.py
+-rw-r--r--   0        0        0       46 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/utils/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/core/utils/example_responses.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/__init__.py
+-rw-r--r--   0        0        0     6446 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/api_models.py
+-rw-r--r--   0        0        0     5806 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/api_view_v1.py
+-rw-r--r--   0        0        0     9649 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/api_view_v2.py
+-rw-r--r--   0        0        0       91 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/base_models/__init__.py
+-rw-r--r--   0        0        0     5975 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/base_models/model.py
+-rw-r--r--   0        0        0     1135 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/base_models/source.py
+-rw-r--r--   0        0        0     6686 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/controller.py
+-rw-r--r--   0        0        0      726 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/exceptions.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/repository/__init__.py
+-rw-r--r--   0        0        0    14191 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/repository/repository.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/__init__.py
+-rw-r--r--   0        0        0      681 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/cds.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/__init__.py
+-rw-r--r--   0        0        0    13309 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/downloader.py
+-rw-r--r--   0        0        0     6408 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
+-rw-r--r--   0        0        0     6840 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
+-rw-r--r--   0        0        0    15187 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
+-rw-r--r--   0        0        0      591 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/factors.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/models/__init__.py
+-rw-r--r--   0        0        0     8711 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/models/era5land.py
+-rw-r--r--   0        0        0     7833 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
+-rw-r--r--   0        0        0     6930 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py
+-rw-r--r--   0        0        0    23812 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
+-rw-r--r--   0        0        0     9169 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
+-rw-r--r--   0        0        0     1495 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/knmi.py
+-rw-r--r--   0        0        0      421 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
+-rw-r--r--   0        0        0     4963 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
+-rw-r--r--   0        0        0     5320 2024-04-17 09:51:20.595167 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py
+-rw-r--r--   0        0        0    15117 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
+-rw-r--r--   0        0        0     4781 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
+-rw-r--r--   0        0        0    11062 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
+-rw-r--r--   0        0        0    13403 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
+-rw-r--r--   0        0        0    19917 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/stations.py
+-rw-r--r--   0        0        0     7014 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/utils.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
+-rw-r--r--   0        0        0     5148 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/__init__.py
+-rw-r--r--   0        0        0     3048 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/date_helpers.py
+-rw-r--r--   0        0        0     1397 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/file_helpers.py
+-rw-r--r--   0        0        0     5742 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/geo_position.py
+-rw-r--r--   0        0        0     1791 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/grid_helpers.py
+-rw-r--r--   0        0        0      447 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/pandas_helpers.py
+-rw-r--r--   0        0        0     5053 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/serializers.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/erase_arome_repository.py
+-rw-r--r--   0        0        0      413 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/erase_era5land_repository.py
+-rw-r--r--   0        0        0      438 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/erase_era5sl_repository.py
+-rw-r--r--   0        0        0      497 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/erase_waarnemingen_register.py
+-rw-r--r--   0        0        0      383 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/update_arome_repository.py
+-rw-r--r--   0        0        0      401 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/update_era5land_repository.py
+-rw-r--r--   0        0        0      371 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/update_era5sl_repository.py
+-rw-r--r--   0        0        0      462 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/scripts/update_waarnemingen_register.py
+-rw-r--r--   0        0        0      140 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/versions/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/versions/v1.py
+-rw-r--r--   0        0        0      772 2024-04-17 09:51:20.599168 weather_provider_api-2.50.36/weather_provider_api/versions/v2.py
+-rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 weather_provider_api-2.50.36/PKG-INFO
```

### Comparing `weather_provider_api-2.50.35/LICENSE` & `weather_provider_api-2.50.36/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/LICENSES/Apache-2.0.txt` & `weather_provider_api-2.50.36/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/LICENSES/CC-BY-2.5.txt` & `weather_provider_api-2.50.36/LICENSES/CC-BY-2.5.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/LICENSES/MPL-2.0.txt` & `weather_provider_api-2.50.36/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/README.md` & `weather_provider_api-2.50.36/README.md`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/pyproject.toml` & `weather_provider_api-2.50.36/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weather_provider_api"
-version = "2.50.035"
+version = "2.50.036"
 description = "Weather Provider Libraries and API"
 authors = ["Verbindingsteam", "Raoul Linnenbank <58594297+rflinnenbank@users.noreply.github.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository="https://github.com/alliander-opensource/wpla/"
 include = [
     {path = "var_maps/*.json", format = "wheel"}
```

### Comparing `weather_provider_api-2.50.35/weather_provider_api/__main__.py` & `weather_provider_api-2.50.36/weather_provider_api/__main__.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/app_version.py` & `weather_provider_api-2.50.36/weather_provider_api/app_version.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/config/__init__.py` & `weather_provider_api-2.50.36/weather_provider_api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/config/config.toml` & `weather_provider_api-2.50.36/weather_provider_api/config/config.toml`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/application.py` & `weather_provider_api-2.50.36/weather_provider_api/core/application.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/exceptions/exceptions.py` & `weather_provider_api-2.50.36/weather_provider_api/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/gunicorn_application.py` & `weather_provider_api-2.50.36/weather_provider_api/core/gunicorn_application.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/initializers/cors.py` & `weather_provider_api-2.50.36/weather_provider_api/core/initializers/cors.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/initializers/exception_handling.py` & `weather_provider_api-2.50.36/weather_provider_api/core/initializers/exception_handling.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/initializers/headers.py` & `weather_provider_api-2.50.36/weather_provider_api/core/initializers/headers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/initializers/logging_handler.py` & `weather_provider_api-2.50.36/weather_provider_api/core/initializers/logging_handler.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/initializers/mounting.py` & `weather_provider_api-2.50.36/weather_provider_api/core/initializers/mounting.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/initializers/prometheus.py` & `weather_provider_api-2.50.36/weather_provider_api/core/initializers/prometheus.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/initializers/validation.py` & `weather_provider_api-2.50.36/weather_provider_api/core/initializers/validation.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/core/utils/example_responses.py` & `weather_provider_api-2.50.36/weather_provider_api/core/utils/example_responses.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/api_models.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/api_models.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/api_view_v1.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/api_view_v1.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/api_view_v2.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/api_view_v2.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/base_models/model.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/base_models/model.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/base_models/source.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/base_models/source.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/controller.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/controller.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/exceptions.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/exceptions.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/repository/repository.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/repository/repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/cds.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/cds.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/downloader.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/factors.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/factors.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/models/era5land.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/models/era5land.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/cds/models/era5sl.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/cds/models/era5sl.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/knmi.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/knmi.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/pluim.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/pluim.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #  SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
-"""KNMI hour models data fetcher.
-"""
+"""KNMI hour models data fetcher."""
 import copy
 import json
 from datetime import datetime
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
@@ -23,19 +22,15 @@
 from weather_provider_api.routers.weather.sources.knmi.utils import find_closest_stn_list
 from weather_provider_api.routers.weather.utils.date_helpers import validate_begin_and_end
 from weather_provider_api.routers.weather.utils.geo_position import GeoPosition
 from weather_provider_api.routers.weather.utils.pandas_helpers import coords_to_pd_index
 
 
 class UurgegevensModel(WeatherModelBase):
-    """
-    A Weather Model that incorporates the:
-        KNMI Uurgegevens
-    dataset into the Weather Provider API
-    """
+    """A Weather Model that incorporates the: KNMI Uurgegevens dataset into the Weather Provider API."""
 
     def __init__(self):
         super().__init__()
         self.id = "uurgegevens"
         self.name = "KNMI uurgegevens"
         self.version = ""
         self.url = "https://daggegevens.knmi.nl/klimatologie/uurgegevens"
@@ -136,26 +131,28 @@
         logger.debug(f"Weather model [{self.id}] initialized successfully")
 
     def get_weather(
         self,
         coords: List[GeoPosition],
         begin: datetime,
         end: datetime,
-        weather_factors: List[str] = None,
+        weather_factors: List[str] | None = None,
     ) -> xr.Dataset:
-        """
-            The function that gathers and processes the requested Daggegevens weather data from the KNMI site
-            and returns it as a Xarray Dataset.
-            (Though this model downloads from a specific download url, the question remains whether this source is also
-            listed on the new KNMI Data Platform)
+        """The function that gathers and processes the requested Daggegevens weather data from the KNMI site
+        and returns it as a Xarray Dataset.
+
+        (Though this model downloads from a specific download url, the question remains whether this source is also
+        listed on the new KNMI Data Platform).
+
         Args:
             coords:             A list of GeoPositions containing the locations the data is requested for.
             begin:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             An Xarray Dataset containing the weather data for the requested period, locations and factors.
         """
         # Test and account for invalid datetime timeframes or input
         begin, end = validate_begin_and_end(begin, end, None, datetime.utcnow() - relativedelta(days=1))
         # Get a list of the relevant STNs and choose the closest STN for each coordinate
         station_id, stns, _ = find_closest_stn_list(stations_history, coords)
@@ -182,29 +179,29 @@
         return self.async_model
 
     def _download_weather(
         self,
         stations: List[int],
         start: datetime,
         end: datetime,
-        weather_factors: List[str] = None,
+        weather_factors: List[str] | None = None,
     ):
         """
             A function that downloads the weather from the KNMI download location and returns it as a text
         Args:
             stations:           A list containing the requested stations
             start:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             weather_factors:    A list of weather factors to request data for (in string format)
         Returns:
             A field containing the full response of the made download-request (text-based)
         """
         # fetch data
         params = self._create_request_params(start, end, stations, weather_factors)
-        r = requests.post(url=self.download_url, data=params)
+        r = requests.post(url=self.download_url, data=params, timeout=60)
 
         if r.status_code != 200:
             raise requests.HTTPError(
                 "Failed to retrieve data from the KNMI website",
                 r.status_code,
                 self.download_url,
                 params,
@@ -212,22 +209,23 @@
         elif r.text == "[]":
             raise ValueError(
                 "No data was returned for this request. Make that the requested data exist for this "
                 "dataset, and that is was properly requested. In case of doubt, contact support."
             )
         return r.text
 
-    def _create_request_params(self, start, end, stations, weather_factors):
-        """
-            A Function that transforms the request settings into parameters usable for the KMNI download request.
+    def _create_request_params(self, start: datetime, end: datetime, stations: list[int], weather_factors: list[str]):
+        """A Function that transforms the request settings into parameters usable for the KMNI download request.
+
         Args:
             start:              A datetime containing the start of the period to request data for.
             end:                A datetime containing the end of the period to request data for.
             stations:           A list containing the requested stations
             weather_factors:    A list of weather factors to request data for (in string format)
+
         Returns:
             A params field (string) containing the matching settings for a KNMI Daggegevens download request.
         """
         params = {
             "fmt": "json",
             "stns": ":".join(str(station) for station in stations),
             "start": f"{start.strftime('%Y%m%d')}01",
@@ -267,18 +265,19 @@
         dataframe_data = dataframe_data.drop(["hour", "timestamp"], axis=1)
 
         dataframe_data = dataframe_data.set_index(["station_code", "date"])
 
         return dataframe_data.to_xarray()
 
     @staticmethod
-    def _prepare_weather_data(coordinates: List[GeoPosition], station_id, raw_ds):
-        # A function that prepares the weather data for return by the API, by replacing the matching station with the
-        # lat/lon location that was requested, and properly formatting the dimensions.
+    def _prepare_weather_data(coordinates: List[GeoPosition], station_id: list[np.int64], raw_ds: xr.Dataset):
+        """A function that prepares the weather data for return by the API, by replacing the matching station with the
+        lat/lon location that was requested, and properly formatting the dimensions.
 
+        """
         # re-arrange stns
         ds = raw_ds.sel(station_code=station_id)
 
         # dict of data
         data_dict = {var_name: (["coord", "time"], var.values) for var_name, var in ds.data_vars.items()}
         timeline = pd.DatetimeIndex(ds.coords["date"].values)
 
@@ -286,15 +285,17 @@
             data_vars=data_dict,
             coords={"time": timeline, "coord": coords_to_pd_index(coordinates)},
         )
         ds = ds.unstack("coord")
         return ds
 
     def _request_weather_factors(self, factors: Optional[List[str]]) -> List[str]:
-        # Implementation of the Base Weather Model function that returns a list of known weather factors for the model.
+        """Implementation of the Base Weather Model function that returns a list of known weather factors for the
+        model.
+        """
         if factors is None:
             return list(self.to_si.keys())
 
         new_factors = []
 
         for f in factors:
             f_up = f.upper()
```

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/stations.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/stations.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/knmi/utils.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/knmi/utils.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/date_helpers.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/date_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/file_helpers.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/geo_position.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/geo_position.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/grid_helpers.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/grid_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/routers/weather/utils/serializers.py` & `weather_provider_api-2.50.36/weather_provider_api/routers/weather/utils/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 def get_weather_slice_for_coords(coord, unserialized_data) -> pd.DataFrame:
     # We use .sel to create slices from the unserialized dataset
     # We then switch to a Pandas dataframe
     if isinstance(coord, list):
         coord = coord[0]
     weather = unserialized_data.sel(lat=coord[0], lon=coord[1], method="nearest")
-    if weather.dims["time"] == 1:
+    if weather.sizes["time"] == 1:
         # Because a single moment in time can't be squeezed...
         df = weather.to_dataframe()
     else:
         # ... and multiple times need to be.
         df = weather.squeeze().to_dataframe()
     return df
```

### Comparing `weather_provider_api-2.50.35/weather_provider_api/versions/v1.py` & `weather_provider_api-2.50.36/weather_provider_api/versions/v1.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/weather_provider_api/versions/v2.py` & `weather_provider_api-2.50.36/weather_provider_api/versions/v2.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.50.35/PKG-INFO` & `weather_provider_api-2.50.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather_provider_api
-Version: 2.50.35
+Version: 2.50.36
 Summary: Weather Provider Libraries and API
 Home-page: https://github.com/alliander-opensource/wpla/
 License: MPL-2.0
 Author: Verbindingsteam
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

