# Comparing `tmp/roulier-1.1.0.tar.gz` & `tmp/roulier-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/roulier-1.1.0.tar", last modified: Fri Apr  2 08:59:05 2021, max compression
+gzip compressed data, was "roulier-1.1.1.tar", last modified: Wed Apr 17 15:02:45 2024, max compression
```

## Comparing `roulier-1.1.0.tar` & `roulier-1.1.1.tar`

### file list

```diff
@@ -1,136 +1,166 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        6 2021-04-02 08:58:41.000000 roulier-1.1.0/VERSION
--rwxrwxr-x   0 travis    (2000) travis    (2000)      125 2021-04-02 08:58:41.000000 roulier-1.1.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3952 2021-04-02 08:59:05.000000 roulier-1.1.0/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2513 2021-04-02 08:58:41.000000 roulier-1.1.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2021-04-02 08:59:05.000000 roulier-1.1.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2903 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/transport.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/templates/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      437 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/templates/remove_empty_tags.xsl
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/gls_fr/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1341 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/decoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3151 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/transport.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1515 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      713 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/carrier_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4193 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/tests/credential_demo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10476 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/tests/test_rest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1104 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/tests/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6998 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/rest/encoder.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4538 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/decoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1560 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/transport.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3108 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/templates/zpl.zpl
--rw-rw-r--   0 travis    (2000) travis    (2000)      706 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/carrier_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1239 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/gls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2939 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      212 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/tests/credential_demo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1895 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/tests/test_roulier_gls_fr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3432 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/glsbox/encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/gls_fr/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1054 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/decoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1799 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/transport.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      367 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/templates/chronopost_soap.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4190 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/templates/chronopost_get_label.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/carrier_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3704 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/chronopost_fr/encoder.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/laposte_fr/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4753 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/decoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3148 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/transport.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      590 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_getProductInter.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      512 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_service.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      184 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_soap.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      258 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_getBordereauByNumber.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1019 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_get_label.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      719 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_address.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2917 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_customsDeclarations.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      425 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_generateBordereauByParcelsNumbers.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      275 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_outputFormat.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      125 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_get_packing_slip.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      606 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_parcel.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1284 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/carrier_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12678 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/laposte_fr/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2206 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/tests/test_laposte_europe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/tests/credential_demo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3459 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/tests/test_laposte_outside_europe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6742 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/tests/test_laposte_basic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1245 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/tests/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      109 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3099 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/laposte_fr/encoder.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      187 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/geodis/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3625 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_encoder_ws.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/geodis/templates/
--rwxrwxr-x   0 travis    (2000) travis    (2000)      234 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/templates/geodis_soap.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      281 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/templates/geodis_findLocalite.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2043 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/templates/geodis_demandeImpressionEtiquette.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/templates/geodis_header.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1313 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_common_ws.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      924 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_encoder_rest_ws.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3977 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_transport_ws.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2852 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_api_ws.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4552 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_encoder_edi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      986 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_api_find_localite_ws.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6474 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_api_rest_ws.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2375 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_decoder_ws.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1330 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_decoder_rest_ws.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2286 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_transport_edi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5397 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_api_edi.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3236 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      487 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/geodis/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10399 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/tests/wip_test_rest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3479 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/geodis/geodis_transport_rest_ws.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1237 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/decoder.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2147 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/transport.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/templates/dpd_header.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      213 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/templates/dpd_soap.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1589 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/templates/dpd_createShipmentWithLabels.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      266 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/templates/dpd_addressInfo.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      288 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/templates/dpd_address.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)      725 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/carrier_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4841 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/api.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      115 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6010 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/tests/test_dpd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      369 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/tests/credential_demo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1374 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/tests/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/tests/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2324 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carriers/dpd_fr_soap/encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/exception.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1184 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/roulier.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3579 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/codec.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2586 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/carrier_action.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8071 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/api.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      339 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3321 2021-04-02 08:58:41.000000 roulier-1.1.0/roulier/ws_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3676 2021-04-02 08:58:41.000000 roulier-1.1.0/CHANGELOG.md
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1284 2021-04-02 08:58:41.000000 roulier-1.1.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-04-02 08:58:41.000000 roulier-1.1.0/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3952 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4871 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2021-04-02 08:59:05.000000 roulier-1.1.0/roulier.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.441322 roulier-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-17 15:02:41.000000 roulier-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-17 15:02:41.000000 roulier-1.1.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-17 15:02:41.000000 roulier-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-17 15:02:45.441322 roulier-1.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-04-17 15:02:41.000000 roulier-1.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)        6 2024-04-17 15:02:41.000000 roulier-1.1.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.425322 roulier-1.1.1/roulier/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      315 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4755 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carrier_action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.425322 roulier-1.1.1/roulier/carriers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      214 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.425322 roulier-1.1.1/roulier/carriers/chronopost_fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/chronopost_fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/chronopost_fr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/chronopost_fr/carrier_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/chronopost_fr/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/chronopost_fr/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.425322 roulier-1.1.1/roulier/carriers/chronopost_fr/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/chronopost_fr/templates/chronopost_get_label.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/chronopost_fr/templates/chronopost_soap.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/chronopost_fr/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.425322 roulier-1.1.1/roulier/carriers/dpd_fr_soap/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      115 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/carrier_action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2194 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/decoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2689 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.429322 roulier-1.1.1/roulier/carriers/dpd_fr_soap/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      288 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/templates/dpd_address.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/templates/dpd_addressInfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/templates/dpd_createShipmentWithLabels.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/templates/dpd_header.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/templates/dpd_soap.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.429322 roulier-1.1.1/roulier/carriers/dpd_fr_soap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/tests/credential_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/tests/test_dpd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2187 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/dpd_fr_soap/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.429322 roulier-1.1.1/roulier/carriers/geodis_fr/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      198 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.429322 roulier-1.1.1/roulier/carriers/geodis_fr/edi/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/edi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/edi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/edi/carrier_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/edi/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/edi/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/geodis_rest_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3481 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/geodis_soap_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/geodis_transport_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.429322 roulier-1.1.1/roulier/carriers/geodis_fr/get_label/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/get_label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/get_label/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/get_label/carrier_action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2085 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/get_label/decoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1667 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/get_label/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.429322 roulier-1.1.1/roulier/carriers/geodis_fr/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/templates/geodis_get_label.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/templates/geodis_header.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      234 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/templates/geodis_soap.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/templates/geodis_validate_address.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.433322 roulier-1.1.1/roulier/carriers/geodis_fr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tests/test_edi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tests/test_get_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tests/test_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tests/test_validate_address.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.433322 roulier-1.1.1/roulier/carriers/geodis_fr/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tracking/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tracking/carrier_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tracking/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/tracking/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.433322 roulier-1.1.1/roulier/carriers/geodis_fr/validate_address/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/validate_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/validate_address/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/validate_address/carrier_action.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      524 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/validate_address/decoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      783 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/geodis_fr/validate_address/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.433322 roulier-1.1.1/roulier/carriers/gls_fr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.433322 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/carrier_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/gls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.433322 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/templates/zpl.zpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.433322 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/tests/credential_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/tests/test_roulier_gls_fr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/glsbox/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.437322 roulier-1.1.1/roulier/carriers/gls_fr/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/carrier_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.437322 roulier-1.1.1/roulier/carriers/gls_fr/rest/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/tests/credential_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/gls_fr/rest/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.437322 roulier-1.1.1/roulier/carriers/laposte_fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/carrier_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.441322 roulier-1.1.1/roulier/carriers/laposte_fr/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1074 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_address.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2917 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_customsDeclarations.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_generateBordereauByParcelsNumbers.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_getBordereauByNumber.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      590 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_getProductInter.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1019 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_get_label.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_get_packing_slip.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      275 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_outputFormat.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      606 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_parcel.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_service.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      184 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_soap.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.441322 roulier-1.1.1/roulier/carriers/laposte_fr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/tests/credential_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/tests/test_laposte_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/tests/test_laposte_europe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/tests/test_laposte_outside_europe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/tests/test_laposte_parcel_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/laposte_fr/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.441322 roulier-1.1.1/roulier/carriers/mondialrelay/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/carrier_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/statuses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.441322 roulier-1.1.1/roulier/carriers/mondialrelay/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/templates/mondial_relay_action.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/templates/mondial_relay_soap.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/carriers/mondialrelay/transport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5918 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1184 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/roulier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.441322 roulier-1.1.1/roulier/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/templates/remove_empty_tags.xsl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/transport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3243 2024-04-17 15:02:41.000000 roulier-1.1.1/roulier/ws_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.441322 roulier-1.1.1/roulier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-17 15:02:45.000000 roulier-1.1.1/roulier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-17 15:02:45.000000 roulier-1.1.1/roulier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:02:45.000000 roulier-1.1.1/roulier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 15:02:45.000000 roulier-1.1.1/roulier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 15:02:45.000000 roulier-1.1.1/roulier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 15:02:45.441322 roulier-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1298 2024-04-17 15:02:41.000000 roulier-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:45.441322 roulier-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:02:41.000000 roulier-1.1.1/tests/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `roulier-1.1.0/README.md` & `roulier-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/transport.py` & `roulier-1.1.1/roulier/transport.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,55 @@
-# -*- coding: utf-8 -*-
 """Send a request to a carrier and get the result."""
-from abc import ABC, abstractmethod
+import logging
+import os
 import requests
+from abc import ABC, abstractmethod
 from .exception import CarrierError
-import logging
 
 log = logging.getLogger(__name__)
 
 
-class RequestsTransport(ABC):
+class TransportBase(ABC):
     def __init__(self, config_object):
         self.config = config_object
 
+
+class RequestsTransport(TransportBase, ABC):
     def before_ws_call_prepare_request_kwargs(self, payload):
         return {
             "body": self.before_ws_call_transform_payload(payload),
             "headers": self._get_requests_headers(payload),
             "auth": self._get_requests_auth(payload),
             "url": self._get_requests_url(payload),
+            "files": self._get_requests_files(payload),
         }
 
     def before_ws_call_transform_payload(self, payload):
         return payload
 
     def send(self, payload):
         request_kwargs = self.before_ws_call_prepare_request_kwargs(payload)
         log.debug(request_kwargs["body"])
+
+        if os.environ.get("ROULIER_PROXY"):
+            request_kwargs["proxies"] = {
+                "http": os.environ["ROULIER_PROXY"],
+                "https": os.environ["ROULIER_PROXY"],
+            }
+
         response = self.send_request(**request_kwargs)
-        log.info("WS response time %s" % response.elapsed.total_seconds())
+        log.debug("WS response time %s" % response.elapsed.total_seconds())
         return self.handle_response(response)
 
     def _get_requests_headers(self, payload=None):
         return None
 
+    def _get_requests_files(self, payload=None):
+        return None
+
     def _get_requests_auth(self, payload=None):
         return None
 
     def _get_requests_url(self, payload=None):
         if self.config.is_test and self.config.ws_test_url:
             return self.config.ws_test_url
         return self.config.ws_url
```

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/rest/decoder.py` & `roulier-1.1.1/roulier/carriers/gls_fr/rest/decoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Laposte XML -> Python."""
 
 import base64
 from datetime import datetime
 from lxml import objectify
 
 from roulier.codec import DecoderGetLabel
```

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/rest/transport.py` & `roulier-1.1.1/roulier/carriers/gls_fr/rest/transport.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/rest/constants.py` & `roulier-1.1.1/roulier/carriers/gls_fr/rest/constants.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/rest/carrier_action.py` & `roulier-1.1.1/roulier/carriers/gls_fr/rest/carrier_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .transport import GlsEuTransport
 
 
 class GlsEuGetabel(CarrierGetLabel):
     """Implementation for GLS via it's REST WebService."""
 
     ws_url = "https://api.gls-group.eu/public/v1/shipments"
-    ws_test_url = "https://api-qs.gls-group.eu/public/v1/shipments"
+    ws_test_url = "https://api-qs1.gls-group.eu/public/v1/shipments"
     encoder = GlsEuEncoder
     decoder = GlsEuDecoderGetLabel
     transport = GlsEuTransport
     api = GlsEuApiParcel
     manage_multi_label = True
```

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/rest/api.py` & `roulier-1.1.1/roulier/carriers/gls_fr/rest/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Implementation of Laposte Api."""
 
 from roulier.api import ApiParcel
 
 from .constants import SERVICE_CHOICES
 from .constants import SERVICE_STANDARD
 
@@ -21,46 +20,54 @@
         schema["pickupLocationId"] = {"type": "string"}
         schema["labelSize"] = {
             "type": "string",
             "default": "A6",
             "allowed": ["A6", "A5", "A4"],
         }
         schema["labelFormat"].update(
-            {"type": "string", "default": "PDF", "allowed": ["PDF", "PNG"],}
+            {
+                "type": "string",
+                "default": "PDF",
+                "allowed": ["PDF", "PNG", "ZPL"],
+            }
         )
+        schema["incoterm"] = {
+            "type": "string",
+            # "regex": r"^\d{2}$",
+            # "allowed": ["10", "13", 18", "20", "23", "30", "40", "43", "50", "60"],
+        }
         return schema
 
     def _address(self):
         string_1_10 = {"type": "string", "minlength": 1, "maxlength": 10}
         string_2_35 = {"type": "string", "minlength": 2, "maxlength": 35}
         string_0_35 = {"type": "string", "minlength": 0, "maxlength": 35}
         schema = super()._address()
         schema["name"].update(string_2_35)
         schema["street1"].update({"minlength": 3, "maxlength": 35})
         schema["country"].update({"minlength": 2, "maxlength": 2})
         schema["zip"].update(string_1_10)
         schema["phone"].update({"maxlength": 20})
         schema["email"].update(
-            {"required": True, "minlength": 3, "maxlength": 100,}
+            {
+                "required": True,
+                "minlength": 3,
+                "maxlength": 100,
+            }
         )
         schema["city"].update(string_2_35)
         schema.update(
             {
                 "id": {"type": "string", "minlength": 0, "maxlength": 20},
                 "street2": string_0_35,
                 "street3": string_0_35,
                 "blockNo1": string_1_10,
                 "province": string_2_35,
                 "contact": string_2_35,
                 "mobile": schema["phone"],
-                "incoterm": {
-                    "type": "string",
-                    # "regex": r"^\d{2}$",
-                    # "allowed": ["10", "13", 18", "20", "23", "30", "40", "43", "50", "60"],
-                },
             }
         )
         return schema
 
     def _opt_schema(self, schema):
         return {
             "type": "dict",
```

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/rest/tests/test_rest.py` & `roulier-1.1.1/roulier/carriers/gls_fr/rest/tests/test_rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,72 +89,70 @@
 def test_eu_country():
     vals = copy.deepcopy(DATA)
     vals["to_address"]["country"] = "DE"
     result = roulier.get("gls_fr_rest", "get_label", vals)
     assert_result(vals, result, 1, 0)
 
 
-# Test currently disabled because it seems impossible to have a valid incoterm with this API
-# and documentation given. GLS-EU France support contacted. Waiting for an answer to fix it
-# def test_vat_country_valid():
-#     """
-#     Test using incoterm for VAT countries
-#     From https://gls-group.eu/IE/media/downloads/Customer_information_Brexit~1.pdf
-#     When exporting with GLS to the UK, dispatchers can choosebetween these Incoterms for
-#     commercial customs clearance:
-#     •Incoterm 10 (DDP):
-#         Freight costs, customs clearance costs, customs duties and taxes paid –
-#         the sender pays all costsincurred, the importer bears no costs.
-#     •Incoterm 20 (DAP):
-#         Freight costs paid, customs clearance costs, customs duties and taxes unpaid –
-#         the sender pays for freight only, the importer bears all other costs.
-#     •Incoterm 30 (DDP, VAT unpaid):
-#         Freight costs, customs clearance costs and customs duties paid, taxes unpaid –
-#         the sender pays for freight, customs clearance costs and customs duties,
-#         the importer pays for the taxes incurred.
-#     •Incoterm 40 (DAP, cleared):
-#         Freight costs and customs  clearance costs paid, customs duties and taxes unpaid –
-#         the sender pays for freight and customs clearance costs, the importer pays customs
-#         duties and taxes.
-#     •Incoterm 60 (Pick&ShipService, Pick&ReturnService):
-#         Freight costs, customs clearance costs, customs duties and taxes paid –
-#         the customer pays all costs incurred, the importer bears no costs.
-
-#     In future, we will be able to offer additional, cost-effective inco-terms for customs
-#     clearance of single parcels to the UK.
-#     •Incoterm 13 (DDP):
-#         Freight costs, customs clearance costs, customs duties and taxes paid –
-#         the sender pays all costs incurred, the importer bears no costs.
-#     •Incoterm 23 (DAP):
-#         Freight costs paid, customs clearance costs, customs duties and taxes unpaid –
-#         the sender paysfor freight only, the importer bears all other costs.
-#     •Incoterm 43 (DAP, cleared):
-#         Freight costs and customs clear-ance costs paid, customs duties and taxes unpaid –
-#         the sender pays for freight and customs clearance costs, the  importer pays customs
-#         duties and taxes.
-#     •Incoterm 18 (DDP, VAT pre-registration):
-#         Freight costs, cus-toms clearance costs and taxes paid –
-#         the sender pays all costs incurred, the importer bears no costs.
-#         For single or various parcels with a goods value of less than GBP 135.
-#         Here, the import VAT can be paid directly to the British tax authorities.
-
-#     From GLS-Web-API_FR_V01-03.pdf
-#     •Incoterm 50:
-#         Marchandise livrée, dédouanement export & import payés, exemption de faible valeur
-#         autorisation libre.
-#     """
-#     vals = copy.deepcopy(DATA)
-#     vals["to_address"]["name"] = "Prince"
-#     vals["to_address"]["street1"] = "Place de Bel-Air"
-#     vals["to_address"]["zip"] = "1204"
-#     vals["to_address"]["city"] = "Geneve"
-#     vals["to_address"]["country"] = "CH"
-#     vals["to_address"]["incoterm"] = "20"
-#     result = roulier.get("gls_fr_rest", "get_label", vals)
-#     assert_result(vals, result, 1, 0)
+def test_vat_country_valid():
+    """
+    Test using incoterm for VAT countries
+    From https://gls-group.eu/IE/media/downloads/Customer_information_Brexit~1.pdf
+    When exporting with GLS to the UK, dispatchers can choosebetween these Incoterms for
+    commercial customs clearance:
+    •Incoterm 10 (DDP):
+        Freight costs, customs clearance costs, customs duties and taxes paid –
+        the sender pays all costsincurred, the importer bears no costs.
+    •Incoterm 20 (DAP):
+        Freight costs paid, customs clearance costs, customs duties and taxes unpaid –
+        the sender pays for freight only, the importer bears all other costs.
+    •Incoterm 30 (DDP, VAT unpaid):
+        Freight costs, customs clearance costs and customs duties paid, taxes unpaid –
+        the sender pays for freight, customs clearance costs and customs duties,
+        the importer pays for the taxes incurred.
+    •Incoterm 40 (DAP, cleared):
+        Freight costs and customs  clearance costs paid, customs duties and taxes unpaid –
+        the sender pays for freight and customs clearance costs, the importer pays customs
+        duties and taxes.
+    •Incoterm 60 (Pick&ShipService, Pick&ReturnService):
+        Freight costs, customs clearance costs, customs duties and taxes paid –
+        the customer pays all costs incurred, the importer bears no costs.
+
+    In future, we will be able to offer additional, cost-effective inco-terms for customs
+    clearance of single parcels to the UK.
+    •Incoterm 13 (DDP):
+        Freight costs, customs clearance costs, customs duties and taxes paid –
+        the sender pays all costs incurred, the importer bears no costs.
+    •Incoterm 23 (DAP):
+        Freight costs paid, customs clearance costs, customs duties and taxes unpaid –
+        the sender paysfor freight only, the importer bears all other costs.
+    •Incoterm 43 (DAP, cleared):
+        Freight costs and customs clear-ance costs paid, customs duties and taxes unpaid –
+        the sender pays for freight and customs clearance costs, the  importer pays customs
+        duties and taxes.
+    •Incoterm 18 (DDP, VAT pre-registration):
+        Freight costs, cus-toms clearance costs and taxes paid –
+        the sender pays all costs incurred, the importer bears no costs.
+        For single or various parcels with a goods value of less than GBP 135.
+        Here, the import VAT can be paid directly to the British tax authorities.
+
+    From GLS-Web-API_FR_V01-03.pdf
+    •Incoterm 50:
+        Marchandise livrée, dédouanement export & import payés, exemption de faible valeur
+        autorisation libre.
+    """
+    vals = copy.deepcopy(DATA)
+    vals["to_address"]["name"] = "Prince"
+    vals["to_address"]["street1"] = "Place de Bel-Air"
+    vals["to_address"]["zip"] = "1204"
+    vals["to_address"]["city"] = "Geneve"
+    vals["to_address"]["country"] = "CH"
+    vals["service"]["incoterm"] = "20"
+    result = roulier.get("gls_fr_rest", "get_label", vals)
+    assert_result(vals, result, 1, 0)
 
 
 def test_vat_country_missing_icoterm():
     vals = copy.deepcopy(DATA)
     vals["to_address"]["name"] = "Prince"
     vals["to_address"]["street1"] = "Place de Bel-Air"
     vals["to_address"]["zip"] = "1204"
@@ -167,16 +165,16 @@
 def test_vat_country_wrong_icoterm():
     vals = copy.deepcopy(DATA)
     vals["to_address"]["name"] = "Prince"
     vals["to_address"]["street1"] = "Place de Bel-Air"
     vals["to_address"]["zip"] = "1204"
     vals["to_address"]["city"] = "Geneve"
     vals["to_address"]["country"] = "CH"
-    vals["to_address"]["incoterm"] = "00"
-    with pytest.raises(CarrierError, match="Field 'incoterm' not valid"):
+    vals["service"]["incoterm"] = "00"
+    with pytest.raises(CarrierError, match="Incoterm is invalid"):
         result = roulier.get("gls_fr_rest", "get_label", vals)
 
 
 def test_FDS():
     vals = copy.deepcopy(DATA)
     vals["parcels"][0]["services"] = [{"product": SERVICE_FDS}]
     result = roulier.get("gls_fr_rest", "get_label", vals)
```

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/rest/tests/data.py` & `roulier-1.1.1/roulier/carriers/gls_fr/rest/tests/data.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/rest/encoder.py` & `roulier-1.1.1/roulier/carriers/gls_fr/rest/encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Transform input to laposte compatible xml."""
 
 from jinja2 import Environment, PackageLoader
 import logging
 
 from roulier.codec import Encoder
 from roulier.exception import InvalidApiInput
@@ -22,14 +21,16 @@
         body = {
             "shipperId": "%s %s"
             % (data["service"]["customerId"], data["service"]["agencyId"]),
             "shipmentDate": "%s" % data["service"]["shippingDate"],
             "labelFormat": data["service"]["labelFormat"],
             "labelSize": data["service"]["labelSize"],
         }
+        if data["service"].get("incoterm"):
+            body["incoterm"] = data["service"]["incoterm"]
         body["addresses"] = self._transforms_addresses(data, body)
         if "return" in body["addresses"] and data.get("return_weight"):
             body["returns"] = {"weight": "%.2f" % data["return_weight"]}
         references = [
             ref.strip()
             for ref in (
                 data.get("reference1", ""),
@@ -96,23 +97,23 @@
             ("contact", "contact"),  # Nom d'un contact
             ("phone", "phone"),  # Numéro de téléphone : obligatoire si pas de mobile
             (
                 "mobile",
                 "mobile",
             ),  # Numéro de téléphone mobile : obligatoire si pas de fixe
             ("email", "email"),  # Adresse E-mail - /!\Obligatoire en BtoC
-            (
-                "incoterm",
-                "incoterm",
-            ),  # code incoterm international selon destination et formalités douanières.
         )
         for from_addr, to_addr in available_addr:
             addr = data.get(from_addr)
             if not addr:
                 continue
+            # if the company address field is set, then the name is actually the contact
+            if addr["company"] and addr["name"]:
+                addr["contact"] = addr["name"]
+                addr["name"] = addr["company"]
             addresses[to_addr] = dict(
                 (to_field, addr[from_field]) for from_field, to_field in addr_req_fields
             )
             addresses[to_addr]["country"] = addresses[to_addr]["country"].upper()
             addresses[to_addr].update(
                 dict(
                     (to_field, addr[from_field])
```

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/glsbox/decoder.py` & `roulier-1.1.1/roulier/carriers/gls_fr/glsbox/decoder.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/glsbox/transport.py` & `roulier-1.1.1/roulier/carriers/gls_fr/glsbox/transport.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/glsbox/templates/zpl.zpl` & `roulier-1.1.1/roulier/carriers/gls_fr/glsbox/templates/zpl.zpl`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/glsbox/carrier_action.py` & `roulier-1.1.1/roulier/carriers/gls_fr/glsbox/carrier_action.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/glsbox/gls.py` & `roulier-1.1.1/roulier/carriers/gls_fr/glsbox/gls.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     """Implementation for GLS"""
 
     encoder = GlsEncoder()
     decoder = GlsDecoder()
     ws = GlsTransport()
 
     def api(self):
-        """ Expose how to communicate with GLS """
+        """Expose how to communicate with GLS"""
         return self.encoder.api()
 
     def get(self, data, action=None):
-        """ Run an action with data against Gls WS """
+        """Run an action with data against Gls WS"""
         if not action:
             action = "label"
         request = self.encoder.encode(data, action)
         response = self.ws.send(request)
         if isinstance(response, dict):
             response["data_request"] = data
         if action == "label":
@@ -34,9 +34,9 @@
                 {"request_string": request, "response_string": response["body"]}
             )
             return dict_response
         return NotImplementedError
 
     # shortcuts
     def get_label(self, data):
-        """ Generate a label """
+        """Generate a label"""
         return self.get(data, "label")
```

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/glsbox/api.py` & `roulier-1.1.1/roulier/carriers/gls_fr/glsbox/api.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/glsbox/tests/test_roulier_gls_fr.py` & `roulier-1.1.1/roulier/carriers/gls_fr/glsbox/tests/test_roulier_gls_fr.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,50 +13,50 @@
     logger.debug(
         "To test with real credentials copy and paste "
         "tests/credential_demo.py to tests/credential.py and "
         "fill it with real values"
     )
 
 
-def test_connexion():
-    roulier.get(
-        "gls_fr_glsbox",
-        "get_label",
-        {
-            "auth": {"login": credentials["login"], "isTest": credentials["isTest"]},
-            "service": {
-                "agencyId": credentials["agencyId"],
-                "customerId": credentials["customerId"],
-                "shippingDate": date.today(),
-                "shippingId": "125874",
-                "intructions": "Sent from automatic test",
-                "parcel_total_number": 1,
-            },
-            "from_address": {
-                "company": "my company",
-                "name": "my name",
-                "street1": "blablabla street",
-                "zip": "69000",
-                "city": "Lyon",
-                "phone": "04 99 99 99 99",
-                "email": "contact@mycompany.fr",
-            },
-            "to_address": {
-                "company": "my customer",
-                "name": "Martine MARTIN",
-                "street1": "13 avenue des champs Elysées",
-                "zip": "75001",
-                "city": "Paris",
-                "phone": "01 99 99 99 99",
-                "email": "contact@mycustomer.fr",
-                "country": "FR",
-            },
-            "parcels": [
-                {
-                    "weight": 3.4,
-                    "parcel_number_label": 1,
-                    "parcel_number_barcode": 1,
-                    "custom_sequence": "1234567899",
-                }
-            ],
-        },
-    )
+# def test_connexion():
+#    roulier.get(
+#        "gls_fr_glsbox",
+#        "get_label",
+#        {
+#            "auth": {"login": credentials["login"], "isTest": credentials["isTest"]},
+#            "service": {
+#                "agencyId": credentials["agencyId"],
+#                "customerId": credentials["customerId"],
+#                "shippingDate": date.today(),
+#                "shippingId": "125874",
+#                "intructions": "Sent from automatic test",
+#                "parcel_total_number": 1,
+#            },
+#            "from_address": {
+#                "company": "my company",
+#                "name": "my name",
+#                "street1": "blablabla street",
+#                "zip": "69000",
+#                "city": "Lyon",
+#                "phone": "04 99 99 99 99",
+#                "email": "contact@mycompany.fr",
+#            },
+#            "to_address": {
+#                "company": "my customer",
+#                "name": "Martine MARTIN",
+#                "street1": "13 avenue des champs Elysées",
+#                "zip": "75001",
+#                "city": "Paris",
+#                "phone": "01 99 99 99 99",
+#                "email": "contact@mycustomer.fr",
+#                "country": "FR",
+#            },
+#            "parcels": [
+#                {
+#                    "weight": 3.4,
+#                    "parcel_number_label": 1,
+#                    "parcel_number_barcode": 1,
+#                    "custom_sequence": "1234567899",
+#                }
+#            ],
+#        },
+#    )
```

### Comparing `roulier-1.1.0/roulier/carriers/gls_fr/glsbox/encoder.py` & `roulier-1.1.1/roulier/carriers/gls_fr/glsbox/encoder.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/chronopost_fr/decoder.py` & `roulier-1.1.1/roulier/carriers/chronopost_fr/decoder.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/chronopost_fr/transport.py` & `roulier-1.1.1/roulier/carriers/chronopost_fr/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     def before_ws_call_transform_payload(self, payload):
         soap_message = self.soap_wrap(payload["body"])
         return soap_message
 
     def soap_wrap(self, body):
         """Wrap body in a soap:Enveloppe."""
         env = Environment(
-            loader=PackageLoader("roulier", "/carriers/chronopost_fr/templates"),
-            extensions=["jinja2.ext.with_"],
+            loader=PackageLoader("roulier", "carriers/chronopost_fr/templates"),
         )
 
         template = env.get_template("chronopost_soap.xml")
         data = template.render(body=body)
         return data.encode("utf8")
 
     def _get_requests_headers(self, payload=None):
```

### Comparing `roulier-1.1.0/roulier/carriers/chronopost_fr/templates/chronopost_get_label.xml` & `roulier-1.1.1/roulier/carriers/chronopost_fr/templates/chronopost_get_label.xml`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/chronopost_fr/carrier_action.py` & `roulier-1.1.1/roulier/carriers/chronopost_fr/carrier_action.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/chronopost_fr/api.py` & `roulier-1.1.1/roulier/carriers/chronopost_fr/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,18 @@
         schema["customsValue"] = {"type": "integer"}
         schema["customsCurrency"] = {"type": "string"}
         return schema
 
     def _address(self):
         schema = super(ChronopostFrApiParcel, self)._address()
         additional_fields = {
-            "civility": {"type": "string", "allowed": ["E", "L", "M"],},
+            "civility": {
+                "type": "string",
+                "allowed": ["E", "L", "M"],
+            },
             "contact_name": {"type": "string", "maxlength": 100},
             "preAlert": {"type": "integer"},
         }
         schema["name"].update({"maxlength": 100})
         schema["street1"].update({"maxlength": 38})
         schema["street2"].update({"maxlength": 38})
         schema["country"].update({"maxlength": 2, "minlength": 2})
@@ -92,15 +95,18 @@
         return schema
 
     def _from_address(self):
         schema = super(ChronopostFrApiParcel, self)._from_address()
         schema["preAlert"].update({"allowed": [0, 11]})
         # strangely, civility seem really mandatory for shipper
         schema["civility"].update(
-            {"required": True, "empty": False,}
+            {
+                "required": True,
+                "empty": False,
+            }
         )
         return schema
 
     def _auth(self):
         schema = super(ChronopostFrApiParcel, self)._auth()
         schema["login"].update({"required": True, "empty": False})
         schema["password"].update({"required": True, "empty": False, "maxlength": 6})
```

### Comparing `roulier-1.1.0/roulier/carriers/chronopost_fr/encoder.py` & `roulier-1.1.1/roulier/carriers/chronopost_fr/encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,15 @@
         data["service"]["shippingDate"] = data["service"]["shippingDate"].strftime(
             "%Y/%M/%d"
         )
         return data
 
     def transform_input_to_carrier_webservice(self, data):
         env = Environment(
-            loader=PackageLoader("roulier", "/carriers/chronopost_fr/templates"),
-            extensions=["jinja2.ext.with_", "jinja2.ext.autoescape"],
+            loader=PackageLoader("roulier", "carriers/chronopost_fr/templates"),
             autoescape=True,
         )
         action = self.config.action
         template = env.get_template("chronopost_%s.xml" % action)
         return {
             "body": template.render(
                 service=data["service"],
```

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/decoder.py` & `roulier-1.1.1/roulier/carriers/laposte_fr/decoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# -*- coding: utf-8 -*-
 """Laposte XML -> Python."""
 from datetime import datetime
 from lxml import objectify
 
 from ...codec import DecoderGetLabel
 from ...codec import DecoderGetPackingSlip
+from ...codec import DecoderParcelDocument
 import base64
 
 
 class _UNSPECIFIED:
     pass
 
 
@@ -57,15 +57,14 @@
             data = parts.get(cn23_cid)
             annexes.append(
                 {"name": "cn23", "data": base64.b64encode(data), "type": "pdf"}
             )
 
         if rep.find("pdfUrl"):
             annexes.append({"name": "label", "data": rep.find("pdfUrl"), "type": "url"})
-
         parcel = {
             "id": 1,  # no multi parcel management for now.
             "reference": self._get_parcel_number(input_payload),
             "tracking": {
                 # we need to force to real string because of those data can be reused
                 # and cerberus won't accept an ElementString insteadof a string.
                 "number": _get_text(rep, "parcelNumber"),
@@ -126,7 +125,34 @@
                 {
                     "name": "packing_slip",
                     "data": base64.b64encode(parts.get(packing_slip_cid)),
                     "type": "pdf",
                 }
             )
         return self.result
+
+
+class LaposteFrDecoderParcelDocument(DecoderParcelDocument):
+    """Laposte Document Response JSON -> Python."""
+
+    def decode(self, response, input_payload):
+        error_code = response.get("errorCode") or "000"
+        error_label = response.get("errorLabel") or ""
+        if error_code != "000":
+            self.result = None
+            return self.result
+        self.result = getattr(self, "_decode_%s" % self.current_action)(
+            response, input_payload
+        )
+        return self.result
+
+    def _decode_get_document(self, response, input_payload):
+        return {"file": response["body"]}
+
+    def _decode_get_documents(self, response, input_payload):
+        return {d["uuid"]: {**d} for d in response["body"]["documents"]}
+
+    def _decode_create_document(self, response, input_payload):
+        return response["body"]["documentId"]
+
+    def _decode_update_document(self, response, input_payload):
+        return response["body"]["documentId"]
```

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/transport.py` & `roulier-1.1.1/roulier/carriers/dpd_fr_soap/transport.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,69 @@
-# -*- coding: utf-8 -*-
-"""Implement laposteWS."""
-from lxml import objectify, etree
+"""Implement dpdWS."""
+
 from jinja2 import Environment, PackageLoader
-from roulier.ws_tools import remove_empty_tags, get_parts
-from roulier.exception import CarrierError
-import logging
+from lxml import objectify, etree
 
+from roulier.exception import CarrierError
 from roulier.transport import RequestsTransport
+from roulier.ws_tools import remove_empty_tags
+
+import logging
 
 log = logging.getLogger(__name__)
 
 
-class LaposteFrTransport(RequestsTransport):
-    """Implement Laposte WS communication."""
+class DpdTransport(RequestsTransport):
+    """Implement Dpd WS communication."""
 
     def before_ws_call_transform_payload(self, payload):
         body = payload["body"]
         headers = payload["headers"]
         soap_message = self.soap_wrap(body, headers)
+        log.debug(soap_message)
         return soap_message
 
-    def soap_wrap(self, body, headers):
+    def soap_wrap(self, body, auth):
         """Wrap body in a soap:Enveloppe."""
         env = Environment(
-            loader=PackageLoader("roulier", "/carriers/laposte_fr/templates"),
-            extensions=["jinja2.ext.with_"],
+            loader=PackageLoader("roulier", "carriers/dpd_fr_soap/templates"),
         )
 
-        template = env.get_template("laposte_soap.xml")
+        template = env.get_template("dpd_soap.xml")
         body_stripped = remove_empty_tags(body)
-        data = template.render(body=body_stripped)
+        header_template = env.get_template("dpd_header.xml")
+        header_xml = header_template.render(auth=auth)
+        data = template.render(body=body_stripped, header=header_xml)
         return data.encode("utf8")
 
     def _get_requests_headers(self, payload=None):
-        return {"content-type": "text/xml;charset=UTF-8"}
+        """Send body to dpd WS."""
+        return {"content-type": "text/xml"}
 
     def handle_500(self, response):
         """Handle reponse in case of ERROR 500 type."""
-        log.warning("Laposte error 500")
-        obj = objectify.fromstring(response.text)
-        errors = [
-            {
-                "id": obj.xpath("//faultcode")[0],
-                "message": obj.xpath("//faultstring")[0],
-            }
-        ]
-        raise CarrierError(response, errors)
+        obj = objectify.fromstring(response.content)
+        error_id = (obj.xpath("//ErrorId") or obj.xpath("//faultcode"))[0]
+        error_message = (obj.xpath("//ErrorMessage") or obj.xpath("//faultstring"))[0]
+        raise CarrierError(
+            response,
+            [
+                {
+                    "id": error_id,
+                    "message": error_message,
+                }
+            ],
+        )
 
     def handle_200(self, response):
-        """
-        Handle response type 200 (success).
-
-        It still can be a success or a failure.
-        """
+        """Handle response type 200 (success)."""
 
-        def raise_on_error(response_xml):
-            xml = objectify.fromstring(response_xml)
-            messages = xml.xpath("//messages")
-            errors = [
-                {"id": message.id, "message": str(message.messageContent),}
-                for message in messages
-                if message.type == "ERROR"
-            ]
-            if len(errors) > 0:
-                raise CarrierError(response, errors)
-
-        def extract_xml(response):
-            """Because the answer is mixedpart we need to extract."""
-            content_type = response.headers["Content-Type"]
-            boundary = content_type.split('boundary="')[1].split('";')[0]
-            start = content_type.split('start="')[1].split('";')[0]
-
-            between_boundaries = response.text.split("--%s" % boundary)[1]
-            after_start = between_boundaries.split(start)[1]
-            clean_xml = after_start.strip()  # = trim()
-            return clean_xml
-
-        def extract_body(response_xml):
-            """Remove soap wrapper."""
-            xml = objectify.fromstring(response_xml)
-            payload_xml = xml.Body.getchildren()[0]
-            return etree.tostring(payload_xml)
+        def extract_soap(response_xml):
+            obj = objectify.fromstring(response_xml)
+            return obj.Body.getchildren()[0]
 
-        response_xml = extract_xml(response)
-        raise_on_error(response_xml)
+        body = extract_soap(response.content)
+        body_xml = etree.tostring(body)
         return {
-            "body": extract_body(response_xml),
-            "parts": get_parts(response),
+            "body": body_xml,
             "response": response,
         }
```

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_getProductInter.xml` & `roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_getProductInter.xml`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_get_label.xml` & `roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_get_label.xml`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_customsDeclarations.xml` & `roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_customsDeclarations.xml`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/templates/laposte_parcel.xml` & `roulier-1.1.1/roulier/carriers/laposte_fr/templates/laposte_parcel.xml`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/carrier_action.py` & `roulier-1.1.1/roulier/carriers/laposte_fr/carrier_action.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Implementation for Laposte."""
 from ...carrier_action import CarrierGetLabel
 from ...carrier_action import CarrierGetPackingSlip
+from ...carrier_action import CarrierParcelDocument
 from ...roulier import factory
 from .encoder import LaposteFrEncoder
 from .encoder import LaposteFrEncoderGetPackingSlip
+from .encoder import LaposteFrEncoderParcelDocument
 from .decoder import LaposteFrDecoderGetLabel
 from .decoder import LaposteFrDecoderGetPackingSlip
+from .decoder import LaposteFrDecoderParcelDocument
 from .transport import LaposteFrTransport
+from .transport import LaposteFrParcelDocumentTransport
 from .api import LaposteFrApiPackingSlip
 from .api import LaposteFrApiParcel
+from .api import LaposteFrApiParcelDocument
 
 
 class LaposteFrGetabel(CarrierGetLabel):
     """Implementation for Laposte."""
 
     ws_url = "https://ws.colissimo.fr/sls-ws/SlsServiceWS/2.0?wsdl"
     encoder = LaposteFrEncoder
@@ -29,9 +34,23 @@
     encoder = LaposteFrEncoderGetPackingSlip
     decoder = LaposteFrDecoderGetPackingSlip
     transport = LaposteFrTransport
     api = LaposteFrApiPackingSlip
     manage_multi_slip = False
 
 
+class LaposteFrParcelDocument(CarrierParcelDocument):
+    """Implementation for Laposte."""
+
+    ws_url = "https://ws.colissimo.fr/api-document/rest/"
+    encoder = LaposteFrEncoderParcelDocument
+    decoder = LaposteFrDecoderParcelDocument
+    transport = LaposteFrParcelDocumentTransport
+    api = LaposteFrApiParcelDocument
+
+
 factory.register_builder("laposte_fr", "get_label", LaposteFrGetabel)
 factory.register_builder("laposte_fr", "get_packing_slip", LaposteFrGetPackingSlip)
+factory.register_builder("laposte_fr", "get_documents", LaposteFrParcelDocument)
+factory.register_builder("laposte_fr", "get_document", LaposteFrParcelDocument)
+factory.register_builder("laposte_fr", "create_document", LaposteFrParcelDocument)
+factory.register_builder("laposte_fr", "update_document", LaposteFrParcelDocument)
```

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/api.py` & `roulier-1.1.1/roulier/carriers/laposte_fr/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# -*- coding: utf-8 -*-
 """Implementation of Laposte Api."""
+from roulier.api import BaseApi
 from roulier.api import ApiPackingSlip
+from roulier.api import ApiParcelDocument
 from roulier.api import ApiParcel
 
 LAPOSTE_LABEL_FORMAT = (
     "ZPL_10x15_203dpi",
     "ZPL_10x15_300dpi",
     "DPL_10x15_203dpi",
     "DPL_10x15_300dpi",
@@ -157,14 +158,20 @@
             # "et de droits."""
         }
         schema["totalAmount"] = {
             "default": "",
             # 'description': 'Needed for cn23'
         }
         schema["customs"] = {"type": "dict", "schema": self._customs()}
+        schema["pickupLocationId"] = {
+            "default": "",
+            # 'description': """Si productCode = A2P, BPR, ACP, CDI, CMT, BDP. "
+            # "Identifiant du point de retrait "
+            # "(dans le cas d’une livraison Colissimo hors domicile)"""
+        }
         return schema
 
     def _auth(self):
         schema = super()._auth()
         schema["login"].update({"required": True, "empty": False})
         schema["password"]["required"] = False
         return schema
@@ -195,15 +202,19 @@
                         "originalIdent": {"type": "string", "regex": "^[a-zA-Z]{1}$"},
                         "vatAmount": {"type": "float", "required": False},
                         "customsFees": {"type": "float", "required": False},
                     },
                 },
                 "default": [],
             },
-            "category": {"required": True, "type": "integer", "maxlength": 1,},
+            "category": {
+                "required": True,
+                "type": "integer",
+                "maxlength": 1,
+            },
             "explanations": {"required": False, "type": "string", "regex": "^.{0,35}$"},
             "original": {
                 "type": "dict",
                 "schema": {
                     "originalIdent": {"type": "string", "regex": "^[a-zA-Z]{1}$"},
                     "originalInvoiceNumber": {"type": "string", "regex": "^.{1,35}$"},
                     "originalInvoiceDate": {
@@ -217,15 +228,18 @@
             "importersContact": {
                 "type": "string",
                 "regex": "^.{0,35}$",
                 "required": False,
             },
             "officeOrigin": {"type": "string", "regex": "^.{0,35}$", "required": False},
             "comments": {"type": "string", "regex": "^.{0,35}$", "required": False},
-            "description": {"type": "string", "regex": "^.{1,}$",},
+            "description": {
+                "type": "string",
+                "regex": "^.{1,}$",
+            },
             "invoiceNumber": {
                 "type": "string",
                 "regex": "^.{0,35}$",
                 "required": False,
             },
             "licenceNumber": {
                 "type": "string",
@@ -327,7 +341,63 @@
 
 class LaposteFrApiPackingSlip(ApiPackingSlip):
     def _auth(self):
         schema = super()._auth()
         schema["login"].update({"required": True, "empty": False})
         schema["password"]["required"] = False
         return schema
+
+
+class LaposteFrApiParcelDocument(ApiParcelDocument):
+    def _auth(self):
+        schema = super()._auth()
+        schema["app_key"] = {
+            "type": "string",
+            "regex": "^.{0,8}$",
+            "required": False,
+        }
+        schema["password"]["required"] = False
+        return schema
+
+    def _document_type(self):
+        schema = super()._document_type()
+        schema["allowed"] = [
+            # for creation:
+            "CERTIFICATE_OF_ORIGIN",  # Certificat d'origine
+            "EXPORT_LICENSE",  # Licence d'exportation
+            "COMMERCIAL_INVOICE",  # Facture du colis
+            "OTHER",  # Autre
+            # existing documents can have those types below too, but encoder is only for creation
+            # "C50",  # C50
+            # "COMPENSATION",  # Bilan d’indemnisation
+            # "DAU",  # Facture de droits et taxes
+            # "DELIVERY_CERTIFICATE",  # Attestation de livraison
+            # "SIGNATURE",  # Preuve de livraison
+        ]
+        return schema
+
+    def _schemas(self):
+        schemas = super()._schemas()
+        schemas["service"]["language"] = {
+            "default": "fr_FR",
+            "type": "string",
+            "allowed": [
+                "fr_FR",
+                "en_GB",
+                "es_ES",
+                "de_DE",
+                "it_IT",
+            ],
+            "required": False,
+        }
+        if self.current_action in ("create_document", "update_document"):
+            schemas["service"]["account_number"] = {
+                "schema": {"type": "string", "empty": False, "default": ""},
+                "required": True,
+            }
+            # Liste des colis suiveurs du colis maître dans le cas des expéditions
+            # multi colis. les colis sont séparés par une virgule
+            schemas["service"]["parcelNumberList"] = {
+                "schema": {"type": "string", "empty": True, "default": ""},
+                "required": False,
+            }
+        return schemas
```

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/tests/test_laposte_europe.py` & `roulier-1.1.1/roulier/carriers/laposte_fr/tests/test_laposte_europe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import logging
 import copy
 import pytest
 
 from roulier import roulier
 from roulier.exception import InvalidApiInput, CarrierError
```

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/tests/test_laposte_outside_europe.py` & `roulier-1.1.1/roulier/carriers/laposte_fr/tests/test_laposte_outside_europe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import logging
 import copy
 
 from roulier import roulier
 from roulier.exception import InvalidApiInput, CarrierError
 
 from .data import DATA
```

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/tests/test_laposte_basic.py` & `roulier-1.1.1/roulier/carriers/laposte_fr/tests/test_laposte_basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import logging
 import copy
 import base64
 import requests
 import shutil
 import pytest
 
@@ -18,18 +17,27 @@
 EXCEPTION_MESSAGE = "Failed call with parameters %s"
 
 
 def test_methods():
     assert (
         "laposte_fr" in roulier.get_carriers_action_available().keys()
     ), "Laposte carrier unavailable"
-    assert roulier.get_carriers_action_available()["laposte_fr"] == [
-        "get_label",
-        "get_packing_slip",
-    ], "get_label() or get_packing_slip() methods unavailable"
+    available = set(roulier.get_carriers_action_available()["laposte_fr"])
+    expected = set(
+        (
+            "get_label",
+            "get_packing_slip",
+            "get_documents",
+            "get_document",
+            "create_document",
+            "update_document",
+        )
+    )
+    diff = expected - available
+    assert not diff, "%s methods unavailable" % ", ".join(diff)
 
 
 def test_label_basic_checks():
     if _do_not_execute_test_on_remote():
         return
     with pytest.raises(InvalidApiInput, match="empty values not allowed"):
         roulier.get("laposte_fr", "get_label", DATA)
@@ -39,15 +47,16 @@
     with pytest.raises(CarrierError, match="'id': 30109"):
         roulier.get("laposte_fr", "get_label", vals)
 
     vals["service"]["product"] = "COL"
     vals["parcels"][0]["nonMachinable"] = True
     result = roulier.get("laposte_fr", "get_label", vals)
     assert sorted(result.keys()) == ["annexes", "parcels"], EXCEPTION_MESSAGE % vals
-    print(_print_label_with_labelary_dot_com(result))
+    output, errors = _print_label_with_labelary_dot_com(result)
+    assert not errors, "\n".join(errors)
 
     parcel = result["parcels"][0]
     assert sorted(parcel.keys()) == ["id", "label", "reference", "tracking"], (
         EXCEPTION_MESSAGE % vals
     )
 
 
@@ -59,25 +68,58 @@
     # Weight
     vals["parcels"][0]["weight"] = 35
     with pytest.raises(CarrierError, match="Le poids du colis est incorrect"):
         roulier.get("laposte_fr", "get_label", vals)
     vals["parcels"][0]["weight"] = 0
     with pytest.raises(CarrierError, match="Le poids du colis n'a pas été transmis"):
         roulier.get("laposte_fr", "get_label", vals)
-        vals["parcels"][0]["weight"] = DATA["parcels"][0]["weight"]
+    vals["parcels"][0]["weight"] = DATA["parcels"][0]["weight"]
     # country
-    old = "FR"
+    old = vals["from_address"]["country"]
+    del vals["from_address"]["country"]
     with pytest.raises(InvalidApiInput, match="empty values not allowed"):
-        del vals["from_address"]["country"]
         roulier.get("laposte_fr", "get_label", vals)
+    vals["from_address"]["country"] = old
+    old = vals["to_address"]["country"]
+    del vals["to_address"]["country"]
     with pytest.raises(InvalidApiInput, match="empty values not allowed"):
-        vals["from_address"]["country"] = old
-        del vals["to_address"]["country"]
         roulier.get("laposte_fr", "get_label", vals)
-        vals["to_address"]["country"] = old
+    vals["to_address"]["country"] = old
+
+
+def test_pickup():
+    if _do_not_execute_test_on_remote():
+        return
+    vals = copy.deepcopy(DATA)
+    vals["service"]["product"] = "BPR"
+    vals["to_address"]["email"] = "no-reply@webu.coop"
+    vals["service"]["pickupLocationId"] = "929750"
+    vals["service"]["commercialName"] = "Webu"
+
+    # no mobile phone
+    with pytest.raises(CarrierError, match="'id': 30220,"):
+        roulier.get("laposte_fr", "get_label", vals)
+    with pytest.raises(CarrierError, match="'id': 30220,"):
+        vals["to_address"]["homePhone"] = "0123456789"
+        roulier.get("laposte_fr", "get_label", vals)
+        del vals["to_address"]["homePhone"]
+
+    # backward compatibility : mobile phone in standard phone arg
+    # invalid mobile phone
+    with pytest.raises(CarrierError, match="'id': 30221,"):
+        vals["to_address"]["phone"] = "0123456789"
+        roulier.get("laposte_fr", "get_label", vals)
+    vals["to_address"]["phone"] = "0623456789"
+    roulier.get("laposte_fr", "get_label", vals)
+    del vals["to_address"]["phone"]
+
+    # better way : home and mobile phone in two fields
+    vals["to_address"]["mobilePhone"] = "0623456789"
+    vals["to_address"]["homePhone"] = "0123456789"
+    roulier.get("laposte_fr", "get_label", vals)
 
 
 def test_auth():
     if _do_not_execute_test_on_remote():
         return
     vals = copy.deepcopy(DATA)
     vals["auth"]["login"] = "test"
@@ -155,33 +197,36 @@
         return True
     return False
 
 
 def _print_label_with_labelary_dot_com(result):
     """This method convert zpl data in pdf file"""
     if not DOWNLOAD_PDF_FILE:
-        return
+        return [], []
     url = "http://api.labelary.com/v1/printers/8dpmm/labels/4x6/%s"
     headers = {"Accept": "application/pdf"}
+    output = []
+    errors = []
     for parcel in result.get("parcels"):
         if parcel.get("label") and parcel["label"].get("data"):
             zpl = base64.b64decode(parcel["label"]["data"]).decode("utf8")
             response = requests.post(
                 url % parcel.get("id"),
                 headers=headers,
                 files={"file": zpl},
                 stream=True,
             )
             if response.status_code == 200:
                 response.raw.decode_content = True
                 with open("label%s.png" % parcel.get("id"), "wb") as out_file:
                     shutil.copyfileobj(response.raw, out_file)
-                    print("label %s downloaded" % parcel.get("id"))
+                    output.append("label %s downloaded" % parcel.get("id"))
             else:
-                print("Error: " + response.text)
+                errors.append("Error: " + response.text)
+    return output, errors
 
 
 def assert_label(result):
     assert "parcels" in result
     assert len(result["parcels"]) > 0
     assert "label" in result["parcels"][0]
     assert "data" in result["parcels"][0]["label"]
```

### Comparing `roulier-1.1.0/roulier/carriers/laposte_fr/tests/data.py` & `roulier-1.1.1/roulier/carriers/laposte_fr/tests/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import logging
 from datetime import date
 
 logger = logging.getLogger(__name__)
 
 try:
     from .credential import credentials
@@ -45,7 +43,16 @@
 PACKING_SLIP_DATA = {
     "auth": {
         "login": credentials["login"],
         "password": credentials["password"],
         "isTest": credentials["isTest"],
     },
 }
+
+PARCEL_DOCUMENT_DATA = {
+    "auth": {
+        "login": credentials["login"],
+        "password": credentials["password"],
+        "isTest": credentials["isTest"],
+    },
+    "service": {},
+}
```

### Comparing `roulier-1.1.0/roulier/carriers/geodis/geodis_encoder_ws.py` & `roulier-1.1.1/roulier/carriers/geodis_fr/geodis_soap_transport.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,103 @@
-# -*- coding: utf-8 -*-
-"""Transform input to geodis compatible xml."""
+"""Implement geodisWS."""
+from lxml import objectify
 from jinja2 import Environment, PackageLoader
-from roulier.codec import Encoder
-from roulier.exception import InvalidApiInput
-from .geodis_common_ws import GEODIS_INFOS
+from roulier.ws_tools import remove_empty_tags, get_parts
+from roulier.exception import CarrierError
+import logging
 
+from roulier.transport import RequestsTransport
 
-GEODIS_ACTIONS = GEODIS_INFOS.keys()
+log = logging.getLogger(__name__)
 
 
-class GeodisEncoderWs(Encoder):
-    """Transform input to geodis compatible xml."""
+class GeodisFrSoapTransport(RequestsTransport):
+    """Implement Geodis WS communication."""
 
-    def get_api(self, action):
-        """Get Api object based on action.
+    def before_ws_call_transform_payload(self, payload):
+        soap_message = self.soap_wrap(payload)
+        return soap_message
 
-        raise if action is not known"""
-        if not (action in GEODIS_ACTIONS):
-            raise InvalidApiInput(
-                "action %s not in %s" % (action, ", ".join(GEODIS_INFOS))
-            )
-
-        return GEODIS_INFOS[action]["api"]()
-
-    def encode(self, api_input, action):
-        """Transform input to geodis compatible xml."""
-        api = self.get_api(action)
-        if not api.validate(api_input):
-            raise InvalidApiInput("Input error : %s" % api.errors(api_input))
+    def soap_wrap(self, payload):
+        """Wrap body in a soap:Enveloppe."""
         env = Environment(
-            loader=PackageLoader("roulier", "/carriers/geodis/templates"),
-            extensions=["jinja2.ext.with_", "jinja2.ext.autoescape"],
-            autoescape=True,
+            loader=PackageLoader("roulier", "carriers/geodis_fr/templates"),
         )
-        template = env.get_template("geodis_%s.xml" % action)
-
-        data = api.normalize(api_input)
-        infos = {
-            "xmlns": GEODIS_INFOS[action]["xmlns"],
-            "url": (
-                data["service"]["is_test"]
-                and GEODIS_INFOS[action]["endpoint_test"]
-                or GEODIS_INFOS[action]["endpoint"]
-            ),
-            "action": action,
-        }
-
-        def request_impression_etiquette():
-            infos["output_format"] = (api_input["service"]["labelFormat"],)
-            data["service"]["labelFormat"] = self.lookup_label_format(
-                data["service"]["labelFormat"]
+        body = payload["body"]
+        headers = payload["headers"]
+        template = env.get_template("geodis_soap.xml")
+        body_stripped = remove_empty_tags(body)
+        header_template = env.get_template("geodis_header.xml")
+        xmlns = self.config.xmlns
+        header_xml = header_template.render(auth=headers, xmlns=xmlns)
+        data = template.render(body=body_stripped, header=header_xml, xmlns=xmlns)
+
+        return data.encode("utf8")
+
+    def _get_requests_headers(self, payload=None):
+        return {"content-type": "text/xml", "SOAPAction": "<SOAP Action>"}
+
+    def handle_500(self, response):
+        """Handle reponse in case of ERROR 500 type."""
+        # TODO : put a try catch (like wrong server)
+        log.warning("Geodis error 500")
+        xml = get_parts(response)["start"]
+        obj = objectify.fromstring(xml)
+        message = obj.xpath("//*[local-name() = 'message']")
+        if not message:
+            message = obj.xpath("//*[local-name() = 'faultstring']")
+        id_message = None
+        if len(message) > 0:
+            message = message[0] or obj.xpath("//faultstring")[0]
+            id_message = (
+                obj.xpath("//*[local-name() = 'code']")
+                and obj.xpath("//*[local-name() = 'code']")[0]
+                or ""
             )
-            data["service"]["shippingDate"] = data["service"]["shippingDate"].strftime(
-                "%Y%M%d"
-            )
-            data["from_address"]["departement"] = data["from_address"]["zip"][:2]
-            return {
-                "body": template.render(
-                    service=data["service"],
-                    parcels=data["parcels"],
-                    sender_address=data["from_address"],
-                    receiver_address=data["to_address"],
-                    xmlns=infos["xmlns"],
-                ),
-                "headers": data["auth"],
-                "infos": infos,
-            }
-
-        def request_find_localite():
-            return {
-                "body": template.render(
-                    receiver_address=data["to_address"], xmlns=infos["xmlns"],
-                ),
-                "headers": data["auth"],
-                "infos": infos,
+        errors = [
+            {
+                "id": id_message,
+                "message": message,
             }
+        ]
+        raise CarrierError(response, errors)
 
-        if action == "demandeImpressionEtiquette":
-            return request_impression_etiquette()
-        elif action == "findLocalite":
-            return request_find_localite()
-
-    def api(self, action="demandeImpressionEtiquette"):
-        """Provide a dict prefilled with default values."""
-        return self.get_api(action).api_values()
-
-    def lookup_label_format(self, label_format="ZPL"):
-        """Get a Geodis compatible format of label.
-
-        args:
-            label_format: (str) ZPL or PDF
-        return
-            a value taken in GEODIS_LABEL_FORMAT
-        """
-        lookup = {
-            "ZPL": "Z",
-            "PDF": "P",
-            "HTML": "H",
-            "XML": "X",
-            "EPL2": "E",
-            "Z": "Z",
-            "P": "P",
-            "H": "H",
-            "X": "X",
-            "E": "E",
+    def handle_200(self, response):
+        """Handle response type 200."""
+        parts = get_parts(response)
+        xml = parts["start"]
+
+        def extract_soap(response_xml):
+            obj = objectify.fromstring(response_xml)
+            return obj.Body.getchildren()[0]
+
+        payload = extract_soap(xml)
+        try:
+            # TODO : may be extract this elsewere
+            # rechercheLocalite has no attachment
+            attachement_cid = payload.codeAttachement.text[len("cid:") :]
+            attachement = parts[attachement_cid]
+        except AttributeError:
+            attachement = None
+
+        return {
+            "body": payload,
+            "parts": attachement,
+            "response": response,
         }
-        return lookup.get(label_format.upper(), "Z")
+
+    def handle_response(self, response):
+        """Handle response of webservice."""
+        if response.status_code == 500:
+            return self.handle_500(response)
+        elif response.status_code == 200:
+            return self.handle_200(response)
+        else:
+            raise CarrierError(
+                response,
+                [
+                    {
+                        "id": None,
+                        "message": "Unexpected status code from server",
+                    }
+                ],
+            )
```

### Comparing `roulier-1.1.0/roulier/carriers/geodis/templates/geodis_demandeImpressionEtiquette.xml` & `roulier-1.1.1/roulier/carriers/geodis_fr/templates/geodis_get_label.xml`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/geodis/geodis_transport_ws.py` & `roulier-1.1.1/roulier/carriers/geodis_fr/geodis_transport_rest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-# -*- coding: utf-8 -*-
 """Implement geodisWS."""
 import requests
-from lxml import objectify
-from jinja2 import Environment, PackageLoader
-from roulier.transport import Transport
-from roulier.ws_tools import remove_empty_tags, get_parts
+
+from roulier.transport import RequestsTransport
 from roulier.exception import CarrierError
+import json
 import logging
+import hashlib
+import time
 
 log = logging.getLogger(__name__)
 
 
-class GeodisTransportWs(Transport):
-    """Implement Geodis WS communication."""
+class GeodisTransportRestWs(RequestsTransport):
+    """Implement Geodis Rest WS communication."""
+
+    def get_token(self, id, timestamp, lang, hash):
+        params = [id, timestamp, lang, hash]
+        return ";".join(params)
+
+    def get_hash(self, api_key, id, timestamp, lang, service, json_data):
+        return hashlib.sha256(
+            ";".join([api_key, id, timestamp, lang, service, json_data]).encode("utf-8")
+        ).hexdigest()
+
+    def prepare_data(self, data, login, api_key):
+        timestamp = "%d" % (time.time() * 1000)
+        lang = "fr"
+        body = json.dumps(data)
+        service = self.config.service
+        hash = self.get_hash(api_key, login, timestamp, lang, service, body)
+        token = self.get_token(login, timestamp, lang, hash)
+        return body, token
 
     def send(self, payload):
         """Call this function.
 
         Args:
-            payload.body: XML in a string
+            payload.body: JSON
             payload.header : auth
             payload.infos: { url: string, xmlns: string}
         Return:
             {
                 response: (Requests.response)
                 body: XML response (without soap)
-                parts: dict of attachments
+                parts: empty dict // compat with WS
             }
         """
-        body = payload["body"]
-        headers = payload["headers"]
-        infos = payload["infos"]
-        soap_message = self.soap_wrap(body, headers, infos)
-        response = self.send_request(soap_message, infos)
-        log.info("WS response time %s" % response.elapsed.total_seconds())
-        return self.handle_response(response)
-
-    def soap_wrap(self, body, auth, infos):
-        """Wrap body in a soap:Enveloppe."""
-        env = Environment(
-            loader=PackageLoader("roulier", "/carriers/geodis/templates"),
-            extensions=["jinja2.ext.with_"],
+        body, token = self.prepare_data(
+            payload["body"],
+            payload["headers"]["login"],
+            payload["headers"]["password"],
         )
 
-        template = env.get_template("geodis_soap.xml")
-        body_stripped = remove_empty_tags(body)
-        header_template = env.get_template("geodis_header.xml")
-        header_xml = header_template.render(auth=auth, xmlns=infos["xmlns"])
-        data = template.render(
-            body=body_stripped, header=header_xml, xmlns=infos["xmlns"]
-        )
-        return data.encode("utf8")
+        response = self.send_request(body, token)
+        log.info("WS response time %s" % response.elapsed.total_seconds())
+        return self.handle_response(response)
 
-    def send_request(self, body, infos):
+    def send_request(self, body, token):
         """Send body to geodis WS."""
-        ws_url = infos["url"]
+        ws_url = self.config.ws_url
         return requests.post(
             ws_url,
-            headers={"content-type": "text/xml", "SOAPAction": "<SOAP Action>"},
+            headers={"X-GEODIS-Service": token},
             data=body,
         )
 
     def handle_500(self, response):
         """Handle reponse in case of ERROR 500 type."""
         # TODO : put a try catch (like wrong server)
         log.warning("Geodis error 500")
-        xml = get_parts(response)["start"]
-        obj = objectify.fromstring(xml)
-        message = obj.xpath("//*[local-name() = 'message']")
-        id_message = None
-        if len(message) > 0:
-            message = message[0] or obj.xpath("//faultstring")[0]
-            id_message = (
-                obj.xpath("//*[local-name() = 'code']")
-                and obj.xpath("//*[local-name() = 'code']")[0]
-                or ""
-            )
-        errors = [{"id": id_message, "message": message,}]
+        errors = [
+            {
+                "id": "",
+                "message": "",
+            }
+        ]
+        raise CarrierError(response, errors)
+
+    def handle_true_negative_error(self, response, payload):
+        """When servers answer an error with a 200 status code."""
+        errors = [
+            {
+                "id": payload.get("codeErreur", ""),
+                "message": payload.get("texteErreur", ""),
+            }
+        ]
         raise CarrierError(response, errors)
 
     def handle_200(self, response):
         """Handle response type 200."""
-        parts = get_parts(response)
-        xml = parts["start"]
-
-        def extract_soap(response_xml):
-            obj = objectify.fromstring(response_xml)
-            return obj.Body.getchildren()[0]
-
-        payload = extract_soap(xml)
-        try:
-            # TODO : may be extract this elsewere
-            # rechercheLocalite has no attachment
-            attachement_cid = payload.codeAttachement.text[len("cid:") :]
-            attachement = parts[attachement_cid]
-        except AttributeError:
-            attachement = None
-
+        payload = json.loads(response.text)
+        if payload["ok"] is not True:
+            self.handle_true_negative_error(response, payload)
         return {
-            "body": payload,
-            "parts": attachement,
+            "body": payload.get("contenu", []),
+            "parts": [],
             "response": response,
         }
 
     def handle_response(self, response):
         """Handle response of webservice."""
         if response.status_code == 500:
             return self.handle_500(response)
         elif response.status_code == 200:
             return self.handle_200(response)
         else:
             raise CarrierError(
                 response,
-                [{"id": None, "message": "Unexpected status code from server",}],
+                [
+                    {
+                        "id": None,
+                        "message": "Unexpected status code from server",
+                    }
+                ],
             )
```

### Comparing `roulier-1.1.0/roulier/carriers/geodis/geodis_encoder_edi.py` & `roulier-1.1.1/roulier/carriers/geodis_fr/edi/encoder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-# -*- coding: utf-8 -*-
 """Implementation of Geodis Api."""
 from datetime import datetime
 from roulier.codec import Encoder
-from roulier.exception import InvalidApiInput
-from .geodis_api_edi import GeodisApiEdi
 
 
-class GeodisEncoderEdi(Encoder):
-    def api(self):
-        api = GeodisApiEdi()
-        return api.api_values()
-
-    def encode(self, api_input):
-        api = GeodisApiEdi()
-        if not api.validate(api_input):
-            raise InvalidApiInput("Input error : %s" % api.errors(api_input))
-        data = api.normalize(api_input)
-
+class GeodisFrEncoderEdi(Encoder):
+    def transform_input_to_carrier_webservice(self, data):
         return {
             "body": self.encode_agency(
                 agency_address=data["agency_address"],
                 from_address=data["from_address"],
                 shipments=data["shipments"],
                 service=data["service"],
             ),
```

### Comparing `roulier-1.1.0/roulier/carriers/geodis/geodis_api_find_localite_ws.py` & `roulier-1.1.1/roulier/carriers/geodis_fr/validate_address/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-# -*- coding: utf-8 -*-
 """Implementation of Geodis Ws Api."""
-from roulier.api import Api
+from roulier.api import ApiParcel
 
 
-class GeodisApiFindLocaliteWs(Api):
-    def _service(self):
-        schema = {}
-        # 'description': 'Use test Ws'
-        schema["is_test"] = {"type": "boolean", "default": True}
-        return schema
-
+class GeodisApiFindLocaliteWs(ApiParcel):
     def _address(self):
-        schema = super(GeodisApiFindLocaliteWs, self)._address()
+        schema = super()._address()
         schema["country"].update({"required": True, "empty": False})
         return {
             "country": schema["country"],
             "zip": schema["zip"],
             "city": schema["city"],
         }
 
     def _auth(self):
-        schema = super(GeodisApiFindLocaliteWs, self)._auth()
+        schema = super()._auth()
         schema["login"].update({"required": True, "empty": False})
         schema["password"]["required"] = False
+        # 'description': 'Use test Ws'
         return schema
 
     def _schemas(self):
         return {
             "auth": self._auth(),
             "to_address": self._address(),
-            "service": self._service(),
         }
```

### Comparing `roulier-1.1.0/roulier/carriers/geodis/geodis_decoder_ws.py` & `roulier-1.1.1/roulier/carriers/geodis_fr/get_label/decoder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,49 @@
-# -*- coding: utf-8 -*-
 """Geodis XML -> Python."""
-from roulier.codec import Decoder
-from .geodis_common_ws import GEODIS_INFOS
+from roulier.codec import DecoderGetLabel
+import base64
 
 
-class GeodisDecoderWs(Decoder):
+class GeodisFrParcelDecoder(DecoderGetLabel):
     """Geodis XML -> Python."""
 
-    def decode(self, body, parts, infos):
-        """Geodis XML -> Python."""
-
-        def reponse_impression_etiquette(msg, parts):
-            output_format = infos["output_format"]
-            labels = "^XZ•^XA".join(parts.split("^XZ\r\n^XA")).split("•")
-            labels_idx = iter(range(len(labels)))
-            labels_data = iter(labels)
-            return {
-                "tracking": {"number": body.cabRouting,},
-                "label": {"name": "label", "data": parts, "type": output_format},
-                "parcels": [
-                    {
-                        "codeUmg": getattr(colis, "codumg", ""),
-                        "id": getattr(colis, "numero", ""),
-                        "number": getattr(colis, "cab", ""),
-                        "reference": getattr(colis, "cabclt", ""),
-                        "label": {
-                            "name": "label_%s" % labels_idx.next(),
-                            "data": labels_data.next(),
-                            "type": output_format,
-                        },
-                    }
-                    for colis in body.infoColis
-                ],
-                "annexes": [],
-                "extra": {
-                    "reseau": getattr(body, "reseau", ""),
-                    "priorite": getattr(body, "priorite", ""),
-                    "codeDirectionel": getattr(body, "codire", ""),
-                    "cabRouting": getattr(body, "cabRouting", ""),
+    def decode(self, response, input_payload):
+        """Chronopost XML -> Python."""
+        body = response["body"]
+        parts = response["parts"].decode()
+        output_format = self.config.roulier_input.get("service", {}).get("labelFormat")
+        extension = self.config.label_formats.get(output_format)[1]
+        labels = parts.replace("\r\n", "\n")
+        labels = "^XZ•^XA".join(labels.split("^XZ\n^XA")).split("•")
+        labels_idx = iter(range(len(labels)))
+        labels_data = iter(labels)
+        for colis in body.infoColis:
+            codeUmg = getattr(colis, "codumg", "") and colis.codumg.text or ""
+            numero = getattr(colis, "numero", "") and colis.numero.text or ""
+            cabclt = getattr(colis, "cabclt", "") and colis.cabclt.text or ""
+            cab = getattr(colis, "cab", "") and colis.cab.text or ""
+            tracking = body.cabRouting.text or ""
+            parcel = {
+                "codeUmg": codeUmg,
+                "id": numero,
+                "reference": cabclt,
+                "number": cab,
+                "tracking": {"number": "", "url": ""},
+                "label": {
+                    "data": base64.b64encode(next(labels_data).encode()),
+                    "name": cabclt or cab or numero or "label_%s" % next(labels_idx),
+                    "type": extension,
                 },
             }
-
-        def response_find_localite(msg, parts):
-            return [
-                {
-                    "ordre": localite.numOrdre,
-                    "region": localite.codeRegion,
-                    "zip": localite.codePostal,
-                    "city": localite.libelle,
-                }
-                for localite in msg.infoLocalite
-            ]
-
-        tag = body.tag
-        lookup = {
-            "{http://impression.service.web.etiquette.geodis.com}reponseImpressionEtiquette": reponse_impression_etiquette,
-            "{http://localite.service.web.etiquette.geodis.com}findLocaliteResponse": response_find_localite,
-        }
-        return lookup[tag](body, parts)
+            self.result["parcels"].append(parcel)
+        self.result["extra"] = (
+            {
+                "reseau": getattr(body, "reseau", "") and body.reseau.text or "",
+                "priorite": getattr(body, "priorite", "") and body.priorite.text or "",
+                "codeDirectionel": getattr(body, "codire", "")
+                and body.codire.text
+                or "",
+                "cabRouting": getattr(body, "cabRouting", "")
+                and body.cabRouting.text
+                or "",
+            },
+        )
```

### Comparing `roulier-1.1.0/roulier/carriers/geodis/geodis_transport_edi.py` & `roulier-1.1.1/roulier/carriers/geodis_fr/edi/transport.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# -*- coding: utf-8 -*-
 """Implement geodisWS."""
-from roulier.transport import Transport
+from roulier.transport import TransportBase
 from datetime import datetime
 import logging
 
 log = logging.getLogger(__name__)
 
 
-class GeodisTransportEdi(Transport):
+class GeodisTransportEdi(TransportBase):
     """Implement Geodis EDI"""
 
     def send(self, payload):
         """Call this function.
 
         Args:
             payload.body: XML in a string
@@ -59,18 +58,22 @@
             return "\n".join([parse_segment(segment) for segment in lines])
 
         def sanitize(token):
             # remove accents and replace escapable chars by space
             # because, replacing "'" by "?'"
             # increase length of the token
             # which is limited by 35
+            if not token:
+                return ""
             sanitized = (
-                token.replace("?", " ")
-                .replace("'", " ")
-                .replace("+", " ")
-                .replace(":", " ")
-            ).encode(
-                "ascii", "ignore"
+                (
+                    token.replace("?", " ")
+                    .replace("'", " ")
+                    .replace("+", " ")
+                    .replace(":", " ")
+                )
+                .encode("ascii", "ignore")
+                .decode()
             )  # cut remaining chars
             return sanitized
 
         return parse_lines(arr)
```

### Comparing `roulier-1.1.0/roulier/carriers/geodis/geodis_api_edi.py` & `roulier-1.1.1/roulier/carriers/geodis_fr/edi/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 """Implementation of Geodis Api."""
-from roulier.api import Api, MyValidator
-from .geodis_api_ws import GeodisApiWs, GEODIS_ALLOWED_NOTIFICATIONS
+from roulier.api import MyValidator
+from ..get_label.api import GeodisFrParcelApi, GEODIS_ALLOWED_NOTIFICATIONS
 
 
-class GeodisApiEdi(Api):
+class GeodisFrApiEdi(GeodisFrParcelApi):
     def _service(self):
         schema = {
             "depositId": {
                 "type": "string",
                 "coerce": "accents",
                 "default": "",
                 "empty": False,
@@ -42,54 +41,43 @@
                 "empty": False,
                 "required": True,
             },
         }
         return schema
 
     def _address(self):
-        schema = super(GeodisApiEdi, self)._address()
-        schema["country"].update({"required": True, "empty": False, "maxlength": 2})
-        schema["zip"].update({"required": True, "empty": False})
-        schema["city"].update({"required": True, "empty": False})
+        schema = super()._address()
         for key in schema:
             if schema[key].get("type", "") == "string":
                 schema[key].update({"coerce": "accents"})
         return schema
 
     def _from_address(self):
-        schema = super(GeodisApiEdi, self)._from_address()
-        schema["phone"].update({"required": True, "empty": False})
-        schema["street1"]["required"] = True
-        schema["siret"] = {
-            "type": "string",
-            "required": True,
-            "default": "",
-            "empty": False,
-        }
+        schema = super()._from_address()
         for key in schema:
             if schema[key].get("type", "") == "string":
                 schema[key].update({"coerce": "accents"})
         return schema
 
     def _parcel(self):
-        weight = GeodisApiWs()._parcel()["weight"]
+        weight = super()._parcel()["weight"]
         return {
             "weight": weight,
             # 'description': 'Barcode of the parcel'
             "barcode": {
                 "type": "string",
                 "empty": False,
                 "default": "",
                 "required": True,
                 "coerce": "accents",
             },
         }
 
     def _to_address(self):
-        schema = GeodisApiWs()._to_address()
+        schema = super()._to_address()
         for key in schema:
             if schema[key].get("type", "") == "string":
                 schema[key].update({"coerce": "accents"})
         return schema
 
     def _shipments(self):
         v = MyValidator()
@@ -97,15 +85,15 @@
             "to_address": {
                 "type": "dict",
                 "schema": self._to_address(),
                 "default": v.normalized({}, self._to_address()),
             },
             "parcels": {
                 "type": "list",
-                "schema": self._parcel(),
+                "schema": {"schema": self._parcel(), "type": "dict"},
                 "default": [v.normalized({}, self._parcel())],
             },
             "product": {
                 "type": "string",
                 "default": "",
                 "empty": False,
                 "required": True,
```

### Comparing `roulier-1.1.0/roulier/carriers/geodis/tests/wip_test_rest.py` & `roulier-1.1.1/roulier/carriers/geodis_fr/tests/test_tracking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-# -*- coding: utf-8 -*-
 from datetime import date
 import json
 from collections import OrderedDict
 
-from ..geodis_decoder_rest_ws import GeodisDecoderRestWs
-from ..geodis_encoder_rest_ws import GeodisEncoderRestWs
-from ..geodis_transport_rest_ws import GeodisTransportRestWs
-from ..geodis_api_rest_ws import GeodisApiTrackingListOut
+from ..tracking.decoder import GeodisFrTrackingListDecoder
+from ..tracking.encoder import GeodisEncoderRestWs
+from ..geodis_transport_rest import GeodisTransportRestWs
+from ..tracking.api import GeodisApiTrackingListOut, GeodisApiTrackingList
+from ..tracking.carrier_action import GeodisFrTrackingList
 
-
-def test_encode():
-    encoder = GeodisEncoderRestWs()
-    api = encoder.api("trackingList")
-    payload = encoder.encode(api, "trackingList")
-    infos = payload["infos"]
-    assert infos["action"] == "trackingList"
-    assert infos["service"] in infos["url"]
+action = GeodisFrTrackingList("geodis_fr", "get_tracking_list")
 
 
 def test_encode_api():
-    encoder = GeodisEncoderRestWs()
-    data = encoder.api("trackingList")
+    encoder = GeodisEncoderRestWs(action)
+    api = GeodisApiTrackingList(action)
+    data = api.api_values()
 
     data["service"]["shippingDateStart"] = date(2019, 7, 2)
     data["service"]["shippingDateEnd"] = date(2019, 7, 2)
     data["auth"]["login"] = "Akretion"
     data["auth"]["password"] = "121221789271"
 
-    payload = encoder.encode(data, "trackingList")
+    payload = encoder.encode(data)
     body = payload["body"]
     assert body["dateDepartFin"] == "2019-07-02"
 
 
 def test_transport_hash():
     """Ensure we encode the has the same way as the specification
 
@@ -59,30 +53,33 @@
             ("refDest", ""),
             ("nomDest", ""),
             ("codePostalDest", ""),
             ("natureMarchandise", ""),
         ]
     )
     body = json.dumps(params, separators=(",", ":"))
-    transport = GeodisTransportRestWs()
+    transport = GeodisTransportRestWs(action)
     hash = transport.get_hash(api_key, login, timestamp, lang, service, body)
     token = transport.get_token(login, timestamp, lang, hash)
     expected = (
         "QTTCLT;1546941256145;fr;"
         + "1b59ef28395469bdd3c823adc2603c469c657ed968e96375b0095307e0460fdf"
     )
     assert token == expected
 
 
 def test_decoder_visit():
-    api = GeodisApiTrackingListOut()
+    api = GeodisApiTrackingListOut(action)
     schema = {
         "str": "simple_string",
         "int": "simple_integer",
-        "inner": {"inner_a": "inner_a", "inner_b": "inner_b",},
+        "inner": {
+            "inner_a": "inner_a",
+            "inner_b": "inner_b",
+        },
     }
     data = {
         "simple_string": "abcdef",
         "simple_integer": 3,
         "inner_a": "a",
         "inner_b": "b",
         "no_lookup": "should not fail",
@@ -163,101 +160,102 @@
     """ 5.0, "reference2": ""}], "codeErreur": null,"""
     """ "ok": true, "texteErreur": null}"""
 )
 
 ret_val = [
     {
         "from_address": {
-            "city": u"STRASBOURG",
-            "country": u"FR",
-            "country_name": u"France",
-            "name": u"RETOUR",
-            "street1": u"axxxZ",
-            "street2": u"wcvwv",
-            "zip": u"69100",
+            "city": "STRASBOURG",
+            "country": "FR",
+            "country_name": "France",
+            "name": "RETOUR",
+            "street1": "axxxZ",
+            "street2": "wcvwv",
+            "zip": "69100",
         },
         "parcels": {"weight": 9.0},
         "service": {
-            "agencyId": u"122121",
-            "customerId": u"01234",
-            "option": u"RET",
-            "product": u"ENE",
-            "reference1": u"abcdeefefefe",
-            "reference2": u"",
-            "reference3": u"",
-            "shippingDate": u"2019-07-09",
-            "shippingId": u"12212122",
+            "agencyId": "122121",
+            "customerId": "01234",
+            "option": "RET",
+            "product": "ENE",
+            "reference1": "abcdeefefefe",
+            "reference2": "",
+            "reference3": "",
+            "shippingDate": "2019-07-09",
+            "shippingId": "12212122",
         },
         "to_address": {
-            "city": u"LESQUIN",
-            "country": u"FR",
-            "country_name": u"France",
-            "name": u"TdsdsfsfsfsT",
-            "street1": u"27 rue Henri Rolland",
-            "street2": u"",
-            "zip": u"59810",
+            "city": "LESQUIN",
+            "country": "FR",
+            "country_name": "France",
+            "name": "TdsdsfsfsfsT",
+            "street1": "27 rue Henri Rolland",
+            "street2": "",
+            "zip": "59810",
         },
         "tracking": {
-            "estDeliveryDate": u"2019-07-10",
-            "proofUrl": u"http://github.com/akretion/roulier",
-            "publicUrl": u"https://akretion.com",
+            "estDeliveryDate": "2019-07-10",
+            "proofUrl": "http://github.com/akretion/roulier",
+            "publicUrl": "https://akretion.com",
             "status": "DELIVERED",
-            "statusDate": u"2019-07-10",
-            "statusDetails": u"Livr\xe9e",
-            "trackingCode": u"12122121",
+            "statusDate": "2019-07-10",
+            "statusDetails": "Livr\xe9e",
+            "trackingCode": "12122121",
         },
     },
     {
         "from_address": {
-            "city": u"VILLEURBANNE",
-            "country": u"FR",
-            "country_name": u"France",
-            "name": u"RETOUR POUR AVARIE",
-            "street1": u"Akretion",
-            "street2": u"GRAND",
-            "zip": u"69100",
+            "city": "VILLEURBANNE",
+            "country": "FR",
+            "country_name": "France",
+            "name": "RETOUR POUR AVARIE",
+            "street1": "Akretion",
+            "street2": "GRAND",
+            "zip": "69100",
         },
         "parcels": {"weight": 5.0},
         "service": {
-            "agencyId": u"12121",
-            "customerId": u"1212121",
-            "option": u"RET",
-            "product": u"ENE",
-            "reference1": u"Shopinvader",
-            "reference2": u"",
-            "reference3": u"",
-            "shippingDate": u"2019-07-09",
-            "shippingId": u"1212121ae",
+            "agencyId": "12121",
+            "customerId": "1212121",
+            "option": "RET",
+            "product": "ENE",
+            "reference1": "Shopinvader",
+            "reference2": "",
+            "reference3": "",
+            "shippingDate": "2019-07-09",
+            "shippingId": "1212121ae",
         },
         "to_address": {
-            "city": u"Villeurbanne",
-            "country": u"FR",
-            "country_name": u"France",
-            "name": u"Akretion",
-            "street1": u"27 Rue Henri Rolland",
-            "street2": u"",
-            "zip": u"69100",
+            "city": "Villeurbanne",
+            "country": "FR",
+            "country_name": "France",
+            "name": "Akretion",
+            "street1": "27 Rue Henri Rolland",
+            "street2": "",
+            "zip": "69100",
         },
         "tracking": {
-            "estDeliveryDate": u"2019-07-10",
-            "proofUrl": u"http://github.com/akretion/roulier",
-            "publicUrl": u"http://akretion.com",
+            "estDeliveryDate": "2019-07-10",
+            "proofUrl": "http://github.com/akretion/roulier",
+            "publicUrl": "http://akretion.com",
             "status": "DELIVERED",
-            "statusDate": u"2019-07-10",
-            "statusDetails": u"Livr\xe9e",
-            "trackingCode": u"12212121",
+            "statusDate": "2019-07-10",
+            "statusDetails": "Livr\xe9e",
+            "trackingCode": "12212121",
         },
     },
 ]
 
 
 def test_decode():
     payload = json.loads(data)
     rep = {
         "body": payload.get("contenu", []),
         "parts": [],
         "response": None,
     }
-    decode = GeodisDecoderRestWs()
-    ret = decode.decode(rep, "trackingList")
+    decode = GeodisFrTrackingListDecoder(action)
+    decode.decode(rep, False)
+    ret = decode.result
 
     assert ret == ret_val
```

### Comparing `roulier-1.1.0/roulier/carriers/dpd_fr_soap/templates/dpd_createShipmentWithLabels.xml` & `roulier-1.1.1/roulier/carriers/dpd_fr_soap/templates/dpd_createShipmentWithLabels.xml`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,122 @@
 00000000: 3c63 6172 3a43 7265 6174 6553 6869 706d  <car:CreateShipm
-00000010: 656e 7457 6974 684c 6162 656c 7320 786d  entWithLabels xm
-00000020: 6c6e 733a 6361 723d 2268 7474 703a 2f2f  lns:car="http://
-00000030: 7777 772e 6361 7267 6f6e 6574 2e73 6f66  www.cargonet.sof
-00000040: 7477 6172 6522 3e0a 093c 6361 723a 7265  tware">..<car:re
-00000050: 7175 6573 743e 0a09 097b 2520 7769 7468  quest>...{% with
-00000060: 2061 6464 7265 7373 203d 2072 6563 6569   address = recei
-00000070: 7665 725f 6164 6472 6573 7320 257d 0a09  ver_address %}..
-00000080: 093c 6361 723a 7265 6365 6976 6572 6164  .<car:receiverad
-00000090: 6472 6573 733e 0a09 0909 7b25 2069 6e63  dress>....{% inc
-000000a0: 6c75 6465 2022 6470 645f 6164 6472 6573  lude "dpd_addres
-000000b0: 732e 786d 6c22 2025 7d0a 0909 3c2f 6361  s.xml" %}...</ca
-000000c0: 723a 7265 6365 6976 6572 6164 6472 6573  r:receiveraddres
-000000d0: 733e 0a09 093c 6361 723a 7265 6365 6976  s>...<car:receiv
-000000e0: 6572 696e 666f 3e0a 0909 097b 2520 696e  erinfo>....{% in
-000000f0: 636c 7564 6520 2264 7064 5f61 6464 7265  clude "dpd_addre
-00000100: 7373 496e 666f 2e78 6d6c 2220 257d 0a09  ssInfo.xml" %}..
-00000110: 093c 2f63 6172 3a72 6563 6569 7665 7269  .</car:receiveri
-00000120: 6e66 6f3e 0a09 097b 2520 656e 6477 6974  nfo>...{% endwit
-00000130: 6820 257d 0a0a 0909 7b25 2077 6974 6820  h %}....{% with 
-00000140: 6164 6472 6573 7320 3d20 7365 6e64 6572  address = sender
-00000150: 5f61 6464 7265 7373 2025 7d0a 0909 3c63  _address %}...<c
-00000160: 6172 3a73 6869 7070 6572 6164 6472 6573  ar:shipperaddres
-00000170: 733e 0a09 0909 7b25 2069 6e63 6c75 6465  s>....{% include
-00000180: 2022 6470 645f 6164 6472 6573 732e 786d   "dpd_address.xm
-00000190: 6c22 2025 7d0a 0909 3c2f 6361 723a 7368  l" %}...</car:sh
-000001a0: 6970 7065 7261 6464 7265 7373 3e0a 0909  ipperaddress>...
-000001b0: 7b25 2065 6e64 7769 7468 2025 7d0a 0a09  {% endwith %}...
-000001c0: 093c 6361 723a 7365 7276 6963 6573 3e0a  .<car:services>.
-000001d0: 0909 097b 2520 7769 7468 2061 6464 7265  ...{% with addre
-000001e0: 7373 203d 2072 6563 6569 7665 725f 6164  ss = receiver_ad
-000001f0: 6472 6573 7320 257d 0a09 0909 3c63 6172  dress %}....<car
-00000200: 3a63 6f6e 7461 6374 3e0a 0909 0909 3c63  :contact>.....<c
-00000210: 6172 3a73 6d73 3e7b 7b20 6164 6472 6573  ar:sms>{{ addres
-00000220: 732e 7068 6f6e 6520 7d7d 3c2f 6361 723a  s.phone }}</car:
-00000230: 736d 733e 0a09 0909 093c 6361 723a 656d  sms>.....<car:em
-00000240: 6169 6c3e 7b7b 2061 6464 7265 7373 2e65  ail>{{ address.e
-00000250: 6d61 696c 207d 7d3c 2f63 6172 3a65 6d61  mail }}</car:ema
-00000260: 696c 3e0a 0909 0909 3c63 6172 3a74 7970  il>.....<car:typ
-00000270: 653e 7b7b 2073 6572 7669 6365 2e6e 6f74  e>{{ service.not
-00000280: 6966 6963 6174 696f 6e73 207d 7d3c 2f63  ifications }}</c
-00000290: 6172 3a74 7970 653e 0a09 0909 3c2f 6361  ar:type>....</ca
-000002a0: 723a 636f 6e74 6163 743e 0a09 0909 7b25  r:contact>....{%
-000002b0: 2065 6e64 7769 7468 2025 7d0a 0909 097b   endwith %}....{
-000002c0: 2520 6966 2073 6572 7669 6365 2e64 726f  % if service.dro
-000002d0: 704f 6666 4c6f 6361 7469 6f6e 2025 7d0a  pOffLocation %}.
-000002e0: 0909 093c 6361 723a 7061 7263 656c 7368  ...<car:parcelsh
-000002f0: 6f70 3e0a 0909 0909 3c63 6172 3a73 686f  op>.....<car:sho
-00000300: 7061 6464 7265 7373 3e0a 0909 0909 093c  paddress>......<
-00000310: 6361 723a 7368 6f70 6964 3e7b 7b20 7365  car:shopid>{{ se
-00000320: 7276 6963 652e 6472 6f70 4f66 664c 6f63  rvice.dropOffLoc
-00000330: 6174 696f 6e20 7d7d 3c2f 6361 723a 7368  ation }}</car:sh
-00000340: 6f70 6964 3e0a 0909 0909 3c2f 6361 723a  opid>.....</car:
-00000350: 7368 6f70 6164 6472 6573 733e 0a09 0909  shopaddress>....
-00000360: 3c2f 6361 723a 7061 7263 656c 7368 6f70  </car:parcelshop
-00000370: 3e0a 0909 097b 2520 656e 6469 6620 257d  >....{% endif %}
-00000380: 0a09 093c 2f63 6172 3a73 6572 7669 6365  ...</car:service
-00000390: 733e 0a0a 0909 3c63 6172 3a6c 6162 656c  s>....<car:label
-000003a0: 5479 7065 3e0a 0909 2020 203c 6361 723a  Type>...   <car:
-000003b0: 7479 7065 3e7b 7b20 7365 7276 6963 652e  type>{{ service.
-000003c0: 6c61 6265 6c46 6f72 6d61 7420 7d7d 3c2f  labelFormat }}</
-000003d0: 6361 723a 7479 7065 3e0a 0909 3c2f 6361  car:type>...</ca
-000003e0: 723a 6c61 6265 6c54 7970 653e 0a09 093c  r:labelType>...<
-000003f0: 6361 723a 6375 7374 6f6d 6572 5f63 6f75  car:customer_cou
-00000400: 6e74 7279 636f 6465 3e7b 7b20 7365 7276  ntrycode>{{ serv
-00000410: 6963 652e 6375 7374 6f6d 6572 436f 756e  ice.customerCoun
-00000420: 7472 7920 7d7d 3c2f 6361 723a 6375 7374  try }}</car:cust
-00000430: 6f6d 6572 5f63 6f75 6e74 7279 636f 6465  omer_countrycode
-00000440: 3e0a 0909 3c63 6172 3a63 7573 746f 6d65  >...<car:custome
-00000450: 725f 6365 6e74 6572 6e75 6d62 6572 3e7b  r_centernumber>{
-00000460: 7b20 7365 7276 6963 652e 6167 656e 6379  { service.agency
-00000470: 4964 207d 7d3c 2f63 6172 3a63 7573 746f  Id }}</car:custo
-00000480: 6d65 725f 6365 6e74 6572 6e75 6d62 6572  mer_centernumber
-00000490: 3e0a 0909 3c63 6172 3a73 6869 7070 696e  >...<car:shippin
-000004a0: 6764 6174 653e 7b7b 2073 6572 7669 6365  gdate>{{ service
-000004b0: 2e73 6869 7070 696e 6744 6174 6520 7d7d  .shippingDate }}
-000004c0: 3c2f 6361 723a 7368 6970 7069 6e67 6461  </car:shippingda
-000004d0: 7465 3e0a 0909 3c63 6172 3a63 7573 746f  te>...<car:custo
-000004e0: 6d65 725f 6e75 6d62 6572 3e7b 7b20 7365  mer_number>{{ se
-000004f0: 7276 6963 652e 6375 7374 6f6d 6572 4964  rvice.customerId
-00000500: 7d7d 3c2f 6361 723a 6375 7374 6f6d 6572  }}</car:customer
-00000510: 5f6e 756d 6265 723e 0a09 093c 6361 723a  _number>...<car:
-00000520: 7765 6967 6874 3e7b 7b20 7061 7263 656c  weight>{{ parcel
-00000530: 2e77 6569 6768 7420 7d7d 3c2f 6361 723a  .weight }}</car:
-00000540: 7765 6967 6874 3e0a 0909 3c63 6172 3a72  weight>...<car:r
-00000550: 6566 6572 656e 6365 6e75 6d62 6572 3e7b  eferencenumber>{
-00000560: 7b20 7365 7276 6963 652e 7265 6665 7265  { service.refere
-00000570: 6e63 6531 207d 7d3c 2f63 6172 3a72 6566  nce1 }}</car:ref
-00000580: 6572 656e 6365 6e75 6d62 6572 3e0a 0909  erencenumber>...
-00000590: 3c63 6172 3a72 6566 6572 656e 6365 323e  <car:reference2>
-000005a0: 7b7b 2073 6572 7669 6365 2e72 6566 6572  {{ service.refer
-000005b0: 656e 6365 3220 7d7d 3c2f 6361 723a 7265  ence2 }}</car:re
-000005c0: 6665 7265 6e63 6532 3e0a 0909 3c63 6172  ference2>...<car
-000005d0: 3a72 6566 6572 656e 6365 333e 7b7b 2073  :reference3>{{ s
-000005e0: 6572 7669 6365 2e72 6566 6572 656e 6365  ervice.reference
-000005f0: 3320 7d7d 3c2f 6361 723a 7265 6665 7265  3 }}</car:refere
-00000600: 6e63 6533 3e0a 093c 2f63 6172 3a72 6571  nce3>..</car:req
-00000610: 7565 7374 3e0a 3c2f 6361 723a 4372 6561  uest>.</car:Crea
-00000620: 7465 5368 6970 6d65 6e74 5769 7468 4c61  teShipmentWithLa
-00000630: 6265 6c73 3e                             bels>
+00000010: 656e 7457 6974 684c 6162 656c 737b 7b20  entWithLabels{{ 
+00000020: 2727 2069 6620 6c65 6761 6379 2065 6c73  '' if legacy els
+00000030: 6520 2742 6327 7d7d 2078 6d6c 6e73 3a63  e 'Bc'}} xmlns:c
+00000040: 6172 3d22 6874 7470 3a2f 2f77 7777 2e63  ar="http://www.c
+00000050: 6172 676f 6e65 742e 736f 6674 7761 7265  argonet.software
+00000060: 223e 0a09 3c63 6172 3a72 6571 7565 7374  ">..<car:request
+00000070: 3e0a 0909 7b25 2077 6974 6820 6164 6472  >...{% with addr
+00000080: 6573 7320 3d20 7265 6365 6976 6572 5f61  ess = receiver_a
+00000090: 6464 7265 7373 2025 7d0a 0909 3c63 6172  ddress %}...<car
+000000a0: 3a63 7573 746f 6d4c 6162 656c 5465 7874  :customLabelText
+000000b0: 3e0a 0909 097b 7b20 6164 6472 6573 732e  >....{{ address.
+000000c0: 6465 6c69 7665 7279 5f69 6e73 7472 7563  delivery_instruc
+000000d0: 7469 6f6e 207d 7d0a 0909 3c2f 6361 723a  tion }}...</car:
+000000e0: 6375 7374 6f6d 4c61 6265 6c54 6578 743e  customLabelText>
+000000f0: 0a09 093c 6361 723a 7265 6365 6976 6572  ...<car:receiver
+00000100: 6164 6472 6573 733e 0a09 0909 7b25 2069  address>....{% i
+00000110: 6e63 6c75 6465 2022 6470 645f 6164 6472  nclude "dpd_addr
+00000120: 6573 732e 786d 6c22 2025 7d0a 0909 3c2f  ess.xml" %}...</
+00000130: 6361 723a 7265 6365 6976 6572 6164 6472  car:receiveraddr
+00000140: 6573 733e 0a09 093c 6361 723a 7265 6365  ess>...<car:rece
+00000150: 6976 6572 696e 666f 3e0a 0909 097b 2520  iverinfo>....{% 
+00000160: 696e 636c 7564 6520 2264 7064 5f61 6464  include "dpd_add
+00000170: 7265 7373 496e 666f 2e78 6d6c 2220 257d  ressInfo.xml" %}
+00000180: 0a09 093c 2f63 6172 3a72 6563 6569 7665  ...</car:receive
+00000190: 7269 6e66 6f3e 0a09 097b 2520 656e 6477  rinfo>...{% endw
+000001a0: 6974 6820 257d 0a0a 0909 7b25 2077 6974  ith %}....{% wit
+000001b0: 6820 6164 6472 6573 7320 3d20 7365 6e64  h address = send
+000001c0: 6572 5f61 6464 7265 7373 2025 7d0a 0909  er_address %}...
+000001d0: 3c63 6172 3a73 6869 7070 6572 6164 6472  <car:shipperaddr
+000001e0: 6573 733e 0a09 0909 7b25 2069 6e63 6c75  ess>....{% inclu
+000001f0: 6465 2022 6470 645f 6164 6472 6573 732e  de "dpd_address.
+00000200: 786d 6c22 2025 7d0a 0909 3c2f 6361 723a  xml" %}...</car:
+00000210: 7368 6970 7065 7261 6464 7265 7373 3e0a  shipperaddress>.
+00000220: 0909 7b25 2065 6e64 7769 7468 2025 7d0a  ..{% endwith %}.
+00000230: 0a09 093c 6361 723a 7365 7276 6963 6573  ...<car:services
+00000240: 3e0a 0909 097b 2520 7769 7468 2061 6464  >....{% with add
+00000250: 7265 7373 203d 2072 6563 6569 7665 725f  ress = receiver_
+00000260: 6164 6472 6573 7320 257d 0a09 0909 3c63  address %}....<c
+00000270: 6172 3a63 6f6e 7461 6374 3e0a 0909 0909  ar:contact>.....
+00000280: 3c63 6172 3a73 6d73 3e7b 7b20 6164 6472  <car:sms>{{ addr
+00000290: 6573 732e 7068 6f6e 6520 7d7d 3c2f 6361  ess.phone }}</ca
+000002a0: 723a 736d 733e 0a09 0909 093c 6361 723a  r:sms>.....<car:
+000002b0: 656d 6169 6c3e 7b7b 2061 6464 7265 7373  email>{{ address
+000002c0: 2e65 6d61 696c 207d 7d3c 2f63 6172 3a65  .email }}</car:e
+000002d0: 6d61 696c 3e0a 0909 0909 3c63 6172 3a74  mail>.....<car:t
+000002e0: 7970 653e 7b7b 2073 6572 7669 6365 2e6e  ype>{{ service.n
+000002f0: 6f74 6966 6963 6174 696f 6e73 207d 7d3c  otifications }}<
+00000300: 2f63 6172 3a74 7970 653e 0a09 0909 3c2f  /car:type>....</
+00000310: 6361 723a 636f 6e74 6163 743e 0a09 0909  car:contact>....
+00000320: 7b25 2065 6e64 7769 7468 2025 7d0a 0909  {% endwith %}...
+00000330: 097b 2520 6966 2073 6572 7669 6365 2e64  .{% if service.d
+00000340: 726f 704f 6666 4c6f 6361 7469 6f6e 2025  ropOffLocation %
+00000350: 7d0a 0909 093c 6361 723a 7061 7263 656c  }....<car:parcel
+00000360: 7368 6f70 3e0a 0909 0909 3c63 6172 3a73  shop>.....<car:s
+00000370: 686f 7061 6464 7265 7373 3e0a 0909 0909  hopaddress>.....
+00000380: 093c 6361 723a 7368 6f70 6964 3e7b 7b20  .<car:shopid>{{ 
+00000390: 7365 7276 6963 652e 6472 6f70 4f66 664c  service.dropOffL
+000003a0: 6f63 6174 696f 6e20 7d7d 3c2f 6361 723a  ocation }}</car:
+000003b0: 7368 6f70 6964 3e0a 0909 0909 3c2f 6361  shopid>.....</ca
+000003c0: 723a 7368 6f70 6164 6472 6573 733e 0a09  r:shopaddress>..
+000003d0: 0909 3c2f 6361 723a 7061 7263 656c 7368  ..</car:parcelsh
+000003e0: 6f70 3e0a 0909 097b 2520 656e 6469 6620  op>....{% endif 
+000003f0: 257d 0a09 093c 2f63 6172 3a73 6572 7669  %}...</car:servi
+00000400: 6365 733e 0a0a 0909 3c63 6172 3a6c 6162  ces>....<car:lab
+00000410: 656c 5479 7065 3e0a 2020 2020 2020 3c63  elType>.      <c
+00000420: 6172 3a74 7970 653e 7b7b 2073 6572 7669  ar:type>{{ servi
+00000430: 6365 2e6c 6162 656c 466f 726d 6174 207d  ce.labelFormat }
+00000440: 7d3c 2f63 6172 3a74 7970 653e 0a09 093c  }</car:type>...<
+00000450: 2f63 6172 3a6c 6162 656c 5479 7065 3e0a  /car:labelType>.
+00000460: 0909 3c63 6172 3a63 7573 746f 6d65 725f  ..<car:customer_
+00000470: 636f 756e 7472 7963 6f64 653e 7b7b 2073  countrycode>{{ s
+00000480: 6572 7669 6365 2e63 7573 746f 6d65 7243  ervice.customerC
+00000490: 6f75 6e74 7279 207d 7d3c 2f63 6172 3a63  ountry }}</car:c
+000004a0: 7573 746f 6d65 725f 636f 756e 7472 7963  ustomer_countryc
+000004b0: 6f64 653e 0a09 093c 6361 723a 6375 7374  ode>...<car:cust
+000004c0: 6f6d 6572 5f63 656e 7465 726e 756d 6265  omer_centernumbe
+000004d0: 723e 7b7b 2073 6572 7669 6365 2e61 6765  r>{{ service.age
+000004e0: 6e63 7949 6420 7d7d 3c2f 6361 723a 6375  ncyId }}</car:cu
+000004f0: 7374 6f6d 6572 5f63 656e 7465 726e 756d  stomer_centernum
+00000500: 6265 723e 0a09 093c 6361 723a 7368 6970  ber>...<car:ship
+00000510: 7069 6e67 6461 7465 3e7b 7b20 7365 7276  pingdate>{{ serv
+00000520: 6963 652e 7368 6970 7069 6e67 4461 7465  ice.shippingDate
+00000530: 207d 7d3c 2f63 6172 3a73 6869 7070 696e   }}</car:shippin
+00000540: 6764 6174 653e 0a09 093c 6361 723a 6375  gdate>...<car:cu
+00000550: 7374 6f6d 6572 5f6e 756d 6265 723e 7b7b  stomer_number>{{
+00000560: 2073 6572 7669 6365 2e63 7573 746f 6d65   service.custome
+00000570: 7249 647d 7d3c 2f63 6172 3a63 7573 746f  rId}}</car:custo
+00000580: 6d65 725f 6e75 6d62 6572 3e0a 0909 3c63  mer_number>...<c
+00000590: 6172 3a77 6569 6768 743e 7b7b 2070 6172  ar:weight>{{ par
+000005a0: 6365 6c2e 7765 6967 6874 207d 7d3c 2f63  cel.weight }}</c
+000005b0: 6172 3a77 6569 6768 743e 0a09 093c 6361  ar:weight>...<ca
+000005c0: 723a 7265 6665 7265 6e63 656e 756d 6265  r:referencenumbe
+000005d0: 723e 7b7b 2073 6572 7669 6365 2e72 6566  r>{{ service.ref
+000005e0: 6572 656e 6365 3120 7d7d 3c2f 6361 723a  erence1 }}</car:
+000005f0: 7265 6665 7265 6e63 656e 756d 6265 723e  referencenumber>
+00000600: 0a09 093c 6361 723a 7265 6665 7265 6e63  ...<car:referenc
+00000610: 6532 3e7b 7b20 7365 7276 6963 652e 7265  e2>{{ service.re
+00000620: 6665 7265 6e63 6532 207d 7d3c 2f63 6172  ference2 }}</car
+00000630: 3a72 6566 6572 656e 6365 323e 0a09 093c  :reference2>...<
+00000640: 6361 723a 7265 6665 7265 6e63 6533 3e7b  car:reference3>{
+00000650: 7b20 7365 7276 6963 652e 7265 6665 7265  { service.refere
+00000660: 6e63 6533 207d 7d3c 2f63 6172 3a72 6566  nce3 }}</car:ref
+00000670: 6572 656e 6365 333e 0a20 2020 2020 2020  erence3>.       
+00000680: 203c 6361 723a 7265 666e 7261 7362 6172   <car:refnrasbar
+00000690: 636f 6465 3e7b 7b20 2774 7275 6527 2069  code>{{ 'true' i
+000006a0: 6620 7365 7276 6963 652e 7265 6665 7265  f service.refere
+000006b0: 6e63 6532 2065 6c73 6520 2766 616c 7365  nce2 else 'false
+000006c0: 277d 7d3c 2f63 6172 3a72 6566 6e72 6173  '}}</car:refnras
+000006d0: 6261 7263 6f64 653e 0a20 2020 2020 2020  barcode>.       
+000006e0: 203c 6361 723a 7265 6665 7265 6e63 6549   <car:referenceI
+000006f0: 6e42 6172 636f 6465 3e0a 2020 2020 2020  nBarcode>.      
+00000700: 2020 2020 2020 3c63 6172 3a74 7970 653e        <car:type>
+00000710: 5265 6665 7265 6e63 6532 3c2f 6361 723a  Reference2</car:
+00000720: 7479 7065 3e0a 2020 2020 2020 2020 3c2f  type>.        </
+00000730: 6361 723a 7265 6665 7265 6e63 6549 6e42  car:referenceInB
+00000740: 6172 636f 6465 3e0a 093c 2f63 6172 3a72  arcode>..</car:r
+00000750: 6571 7565 7374 3e0a 3c2f 6361 723a 4372  equest>.</car:Cr
+00000760: 6561 7465 5368 6970 6d65 6e74 5769 7468  eateShipmentWith
+00000770: 4c61 6265 6c73 7b7b 2027 2720 6966 206c  Labels{{ '' if l
+00000780: 6567 6163 7920 656c 7365 2027 4263 277d  egacy else 'Bc'}
+00000790: 7d3e 0a                                  }>.
```

### Comparing `roulier-1.1.0/roulier/carriers/dpd_fr_soap/carrier_action.py` & `roulier-1.1.1/roulier/carriers/dpd_fr_soap/carrier_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,22 @@
 
 from .api import DpdApi
 from .decoder import DpdDecoder
 from .encoder import DpdEncoder
 from .transport import DpdTransport
 
 
-class DpdGetabel(CarrierGetLabel):
+class DpdGetLabel(CarrierGetLabel):
     """Implementation for Dpd."""
 
     ws_url = (
         "https://e-station.cargonet.software/dpd-eprintwebservice/eprintwebservice.asmx"
     )
-    ws_test_url = (
-        "http://92.103.148.116/exa-eprintwebservice/eprintwebservice.asmx?WSDL"
-    )
+    ws_test_url = "https://e-station-testenv.cargonet.software/eprintwebservice/eprintwebservice.asmx"
     encoder = DpdEncoder
     decoder = DpdDecoder
     transport = DpdTransport
     api = DpdApi
     manage_multi_label = False
 
 
-factory.register_builder("dpd_fr_soap", "get_label", DpdGetabel)
+factory.register_builder("dpd_fr_soap", "get_label", DpdGetLabel)
```

### Comparing `roulier-1.1.0/roulier/carriers/dpd_fr_soap/api.py` & `roulier-1.1.1/roulier/carriers/dpd_fr_soap/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# -*- coding: utf-8 -*-
 """Implementation of Dpd Api."""
 
 from roulier.api import ApiParcel
 from roulier.api import MyValidator
 
 DPD_LABEL_FORMAT = (
     "PDF",
+    "PDF_A6",
     "PNG",
     "ZPL",
 )
 
 DPD_ALLOWED_NOTIFICATIONS = (
     "No",
     "Predict",
@@ -36,15 +36,15 @@
         pickup_id = self.document.get("pickupLocationId", "").strip()
         notifications = self.document.get("notifications")
         if pickup_id and product in ("DPD_Predict", "DPD_Classic"):
             self._error(
                 "pickupLocationId", "pickupLocationId can't be used with %s" % product
             )
         if product == "DPD_Predict":
-            if notifications and "notifications" != "Predict":
+            if notifications and notifications != "Predict":
                 self._error(
                     "notifications", "must be set to Predict when using Predict"
                 )
         else:
             if notifications == "Predict":
                 self._error(
                     "notifications",
@@ -108,14 +108,20 @@
         schema["pickupLocationId"] = {
             "default": "",
             "empty": True,
             "required": False,
             # 'description': 'Drop-off Location id (Relais Colis)'
         }
 
+        # Whether to use the legacy DPD API or the new GeoLabel compatible one
+        schema["legacy"] = {
+            "required": False,
+            "default": False,
+        }
+
         return schema
 
     def _address(self):
         schema = super(DpdApi, self)._address()
         # schema['street2']['description'] = (
         #     "N/A for DPD. It will be appended to street1")
         schema["country"].update({"required": True, "empty": False})
```

### Comparing `roulier-1.1.0/roulier/carriers/dpd_fr_soap/tests/data.py` & `roulier-1.1.1/roulier/carriers/dpd_fr_soap/tests/data.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carriers/dpd_fr_soap/encoder.py` & `roulier-1.1.1/roulier/carriers/dpd_fr_soap/encoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,21 @@
         if data["service"]["product"] == "DPD_Predict":
             data["service"]["notifications"] = "Predict"
         if "pickupLocationId" in data["service"]:
             data["service"]["dropOffLocation"] = data["service"].pop("pickupLocationId")
         data["service"]["shippingDate"] = data["service"]["shippingDate"].strftime(
             "%d/%m/%Y"
         )
+        # dpd is configure with manage_multi_label = False, so always only 1 pack
+        if (
+            data.get("parcels")
+            and data["parcels"][0].get("reference")
+            and not data["service"].get("reference2")
+        ):
+            data["service"]["reference2"] = data["parcels"][0]["reference"]
 
         def reduce_address(address):
             """Concat some fields.
 
             Because there is no street2 nor company in DPD api.
             append street2 to street1 and truncate at 70
             append company to name
@@ -36,30 +43,32 @@
             ]
             address["name"] = ("%s, %s" % (address["name"], address["company"]))[0:35]
 
         reduce_address(data["to_address"])
         reduce_address(data["from_address"])
 
         output_format = data["service"]["labelFormat"]
+        is_legacy = data["service"]["legacy"]
         # if data["service"]["labelFormat"] in ("PNG", "ZPL"):
         if data["service"]["labelFormat"] == "PNG":
             # WS doesn't handle zpl yet, we convert it later
             # png is named Default, WTF DPD?
             data["service"]["labelFormat"] = "Default"
 
         env = Environment(
-            loader=PackageLoader("roulier", "/carriers/dpd_fr_soap/templates"),
-            extensions=["jinja2.ext.with_", "jinja2.ext.autoescape"],
+            loader=PackageLoader("roulier", "carriers/dpd_fr_soap/templates"),
             autoescape=True,
         )
 
         template = env.get_template("dpd_createShipmentWithLabels.xml")
         return {
             "body": template.render(
                 service=data["service"],
                 parcel=data["parcels"][0],
                 sender_address=data["from_address"],
                 receiver_address=data["to_address"],
+                legacy=is_legacy,
             ),
             "headers": data["auth"],
             "output_format": output_format,
+            "is_legacy": is_legacy,
         }
```

### Comparing `roulier-1.1.0/roulier/exception.py` & `roulier-1.1.1/roulier/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Exception classes"""
 import logging
 
 log = logging.getLogger(__name__)
 
 
 class InvalidApiInput(Exception):
```

### Comparing `roulier-1.1.0/roulier/roulier.py` & `roulier-1.1.1/roulier/roulier.py`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/roulier/carrier_action.py` & `roulier-1.1.1/roulier/carrier_action.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """Abstract classes for different Carrier actions"""
 from abc import ABC, abstractmethod
 
 
-class Carrier(ABC):
+class CarrierBase(ABC):
     def __init__(self, carrier_type, action, **kwargs):
         self.carrier_type = carrier_type
         self.action = action
 
+
+class CarrierWebservice(CarrierBase, ABC):
+
+    is_test = False
+    ws_test_url = ""
+    roulier_input = None
+
     @property
     @abstractmethod
     def ws_url(self):
         pass
 
     @property
     @abstractmethod
@@ -28,22 +35,27 @@
         pass
 
     @property
     @abstractmethod
     def api(self):
         pass
 
-    ws_test_url = ""
+    def _get_data_from_webservice(self, data):
+        encoder = self.encoder(self)
+        decoder = self.decoder(self)
+        transport = self.transport(self)
+        self.roulier_input = data
 
+        payload = encoder.encode(data)
+        response = transport.send(payload)
+        decoder.decode(response, payload)
+        return decoder.result
 
-class CarrierGetLabel(Carrier, ABC):
-
-    is_test = False
-    roulier_input = None
 
+class CarrierGetLabel(CarrierWebservice, ABC):
     @property
     @abstractmethod
     def manage_multi_label(self):
         """
         True if carrier webservice accept multiple parcels in one call or False
         if we have to make one call per parcels, even if it belongs to a same shipment
         """
@@ -67,31 +79,95 @@
                 data["parcels"] = [parcel]
                 payload = encoder.encode(data)
                 response = transport.send(payload)
                 decoder.decode(response, payload)
         return decoder.result
 
 
-class CarrierGetPackingSlip(Carrier, ABC):
+class CarrierGetPackingSlip(CarrierWebservice, ABC):
     """
     Manages the "packing slip" to give to the carrier who should sign it before taking
     the packages he will deliver
     """
 
-    is_test = False
-    roulier_input = None
-
     def get_packing_slip(self, carrier_type, action, data):
         """
         Retrieves the packing slip if the webservice handles it.
         If the webservice does not handle packing slip, we can generate out own printable html
         packing slip to give to the carrier.
         """
+        return self._get_data_from_webservice(data)
+
+
+class CarrierAddressValidation(CarrierWebservice, ABC):
+    """
+    Check if address is valid/known from the carrier and eventually get proposal
+    if addresses that could match the input
+    """
+
+    def validate_address(self, carrier_type, action, data):
+        return self._get_data_from_webservice(data)
+
+
+class CarrierGetEdi(CarrierBase, ABC):
+    """
+    Generate an EDI file.
+    """
+
+    @property
+    @abstractmethod
+    def transport(self):
+        pass
+
+    @property
+    @abstractmethod
+    def encoder(self):
+        pass
+
+    @property
+    @abstractmethod
+    def api(self):
+        pass
+
+    def get_edi(self, carrier_type, action, data):
+        """
+        Generate EDI file
+        """
         encoder = self.encoder(self)
-        decoder = self.decoder(self)
         transport = self.transport(self)
         self.roulier_input = data
 
         payload = encoder.encode(data)
+        return transport.send(payload)
+
+
+class CarrierParcelDocument(CarrierWebservice, ABC):
+    """
+    Retrieve (or generate) a document for a specific parcel
+    """
+
+    is_test = False
+    roulier_input = None
+    current_action = None
+
+    def _action(self, current_action, carrier_type, action, data):
+        self.current_action = current_action
+        encoder = self.encoder(self)
+        decoder = self.decoder(self)
+        transport = self.transport(self)
+        self.roulier_input = data
+        payload = encoder.encode(data)
         response = transport.send(payload)
         decoder.decode(response, payload)
         return decoder.result
+
+    def get_documents(self, carrier_type, action, data):
+        return self._action("get_documents", carrier_type, action, data)
+
+    def get_document(self, carrier_type, action, data):
+        return self._action("get_document", carrier_type, action, data)
+
+    def create_document(self, carrier_type, action, data):
+        return self._action("create_document", carrier_type, action, data)
+
+    def update_document(self, carrier_type, action, data):
+        return self._action("update_document", carrier_type, action, data)
```

### Comparing `roulier-1.1.0/roulier/api.py` & `roulier-1.1.1/roulier/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -170,14 +170,20 @@
 
     def _to_address(self):
         address = self._address()
         address["street1"].update({"required": True, "empty": False})
         address["country"].update({"required": True, "empty": False})
         address["city"].update({"required": True, "empty": False})
         address["zip"].update({"required": True, "empty": False})
+        address["delivery_instruction"] = {
+            "type": "string",
+            "default": "",
+            "required": False,
+            "empty": True,
+        }
         return address
 
     def _parcel(self):
         return {
             "weight": {
                 "type": "float",
                 "default": "",
@@ -200,16 +206,19 @@
 
     def _service(self):
         return {
             "product": {"default": ""},
             "agencyId": {"default": ""},
             "customerId": {"default": ""},
             "shippingId": {"default": ""},
-            # 'description': 'When the carrier has the package. Format: YYYY/MM/DD'
-            "shippingDate": {"type": "date", "required": True, "empty": False,},
+            "shippingDate": {
+                "type": "date",
+                "required": True,
+                "empty": False,
+            },
             # 'description': 'Additionnal info visible by the client. Example : order number'
             "reference1": {"type": "string", "default": ""},
             "reference2": {"type": "string", "default": ""},
             "reference3": {"type": "string", "default": ""},
             # 'description': 'Format of output (usually pdf or zpl)'
             "labelFormat": {"default": ""},
             # 'description': 'Additionnal instructions for delivery',
@@ -225,27 +234,105 @@
             "to_address": self._to_address(),
         }
 
 
 class ApiPackingSlip(BaseApi):
     def _packing_slip_number(self):
         return {
-            "schema": {"type": "string", "empty": False,},
+            "schema": {
+                "type": "string",
+                "empty": False,
+            },
             "required": True,
             "excludes": "parcels_numbers",
         }
 
     def _parcels_numbers(self):
         return {
             "type": "list",
-            "schema": {"type": "string", "empty": False,},
+            "schema": {
+                "type": "string",
+                "empty": False,
+            },
             "empty": False,
             "required": True,
             "excludes": "packing_slip_number",
         }
 
     def _schemas(self):
         return {
             "packing_slip_number": self._packing_slip_number(),
             "parcels_numbers": self._parcels_numbers(),
             "auth": self._auth(),
         }
+
+
+class ApiParcelDocument(BaseApi):
+    # https://www.colissimo.entreprise.laposte.fr/sites/default/files/2021-11/DocTechnique-WS-Documents_FR.pdf
+    def __init__(self, config_object):
+        self.config = config_object
+        self.current_action = config_object.current_action
+
+    def _parcel_number(self):
+        return {
+            "schema": {
+                "type": "string",
+                "empty": False,
+                "default": "",
+            },
+            "required": True,
+        }
+
+    def _document_id(self):
+        return {
+            "schema": {
+                "type": "string",
+                "empty": False,
+                "default": "",
+            },
+            "required": True,
+        }
+
+    def _document_type(self):
+        return {
+            "schema": {
+                "type": "string",
+                "empty": False,
+                "default": "",
+            },
+            "required": True,
+        }
+
+    def _document_path(self):
+        return {
+            "schema": {
+                "type": "string",
+                "empty": False,
+                "default": "",
+            },
+            "required": True,
+        }
+
+    def _schemas(self):
+        schema = {"auth": self._auth(), "service": {}}
+        if self.current_action == "get_documents":
+            schema["service"].update(
+                {
+                    "parcel_number": self._parcel_number(),
+                }
+            )
+        elif self.current_action == "get_document":
+            schema["service"].update(
+                {
+                    "parcel_number": self._parcel_number(),
+                    "document_id": self._document_id(),
+                }
+            )
+        elif self.current_action in ("create_document", "update_document"):
+            schema["service"].update(
+                {
+                    "parcel_number": self._parcel_number(),
+                    "document_type": self._document_type(),
+                    "document_path": self._document_path(),
+                }
+            )
+        return schema
```

### Comparing `roulier-1.1.0/roulier/ws_tools.py` & `roulier-1.1.1/roulier/ws_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Utilities for WS."""
 from lxml import etree
 from jinja2 import Environment, PackageLoader
 from zplgrf import GRF
 from PIL import Image
 from io import BytesIO
 import email.parser
@@ -15,17 +14,15 @@
 
     param: xml a string or a etree type
     return: unicode string or lxml.etree._XSLTResultTree
     """
     # use Jinja env for getting the path of template file
     # pkg_resouces may be an alternative, but we already
     # have Jinja
-    env = Environment(
-        loader=PackageLoader("roulier", "templates"), extensions=["jinja2.ext.with_"]
-    )
+    env = Environment(loader=PackageLoader("roulier", "templates"))
     template = env.get_template("remove_empty_tags.xsl")
     xsl = etree.parse(open(template.filename))
     transform = etree.XSLT(xsl)
 
     if isinstance(xml, str):
         xml = etree.fromstring(xml)
     # else we asume xml is an lxml.etree
@@ -40,15 +37,15 @@
 
     Params:
         response: a request object
     Returns:
         an array of content-ids
     """
     head_lines = ""
-    for k, v in response.raw.getheaders().items():
+    for k, v in response.raw.headers.items():
         head_lines += str(k) + ":" + str(v) + "\n"
     full = head_lines.encode() + response.content
     parser = email.parser.BytesParser()
     decoded_reply = parser.parsebytes(full)
     parts = {}
     start = decoded_reply.get_param("start").lstrip("<").rstrip(">")
     i = 0
@@ -59,15 +56,15 @@
         else:
             parts[cid or "Attachment%d" % i] = part.get_payload(decode=True)
         i += 1
     return parts
 
 
 def png_to_zpl(png, rotate):
-    u"""Transform a PNG in a suitable format for ZPL.
+    """Transform a PNG in a suitable format for ZPL.
 
     .png is converted to GRF format.
     Printing a Portable Network Graphics (PNG) with zpl instructions (like DY)
     is possible but hard (the spec is not really understandable).
 
     params:
         png : base64 encoded png
@@ -77,15 +74,15 @@
         a ^GFA instruction with the image.
     """
 
     def base64_to_png(data):
         return BytesIO(base64.b64decode(data))
 
     def get_grf(png, rotate):
-        u"""Get a GRF from a png.
+        """Get a GRF from a png.
 
         params:
             png: BytesIO stream
             rotate: rotate 90° if true
         """
         if rotate:
             png_bytes = BytesIO()
```

### Comparing `roulier-1.1.0/CHANGELOG.md` & `roulier-1.1.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `roulier-1.1.0/setup.py` & `roulier-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,17 @@
         "Jinja2",
         "requests",
         "cerberus",
         "zplgrf",
         "unidecode",
         "pycountry",
     ],
-    extras_requires={"dev": ["ptpython", "pytest"],},
+    extras_requires={
+        "dev": ["ptpython", "pytest"],
+    },
     author="Hparfr <https://github.com/hparfr>",
     author_email="roulier@hpar.fr",
     description="Label parcels without pain",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"roulier": ["*.xml", "*.xsl", "*.zpl"]},
```

### Comparing `roulier-1.1.0/roulier.egg-info/SOURCES.txt` & `roulier-1.1.1/roulier.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.md
+LICENSE
 MANIFEST.in
 README.md
 VERSION
 setup.cfg
 setup.py
 roulier/__init__.py
 roulier/api.py
@@ -37,35 +38,48 @@
 roulier/carriers/dpd_fr_soap/templates/dpd_createShipmentWithLabels.xml
 roulier/carriers/dpd_fr_soap/templates/dpd_header.xml
 roulier/carriers/dpd_fr_soap/templates/dpd_soap.xml
 roulier/carriers/dpd_fr_soap/tests/__init__.py
 roulier/carriers/dpd_fr_soap/tests/credential_demo.py
 roulier/carriers/dpd_fr_soap/tests/data.py
 roulier/carriers/dpd_fr_soap/tests/test_dpd.py
-roulier/carriers/geodis/__init__.py
-roulier/carriers/geodis/geodis.py
-roulier/carriers/geodis/geodis_api_edi.py
-roulier/carriers/geodis/geodis_api_find_localite_ws.py
-roulier/carriers/geodis/geodis_api_rest_ws.py
-roulier/carriers/geodis/geodis_api_ws.py
-roulier/carriers/geodis/geodis_common_ws.py
-roulier/carriers/geodis/geodis_decoder_rest_ws.py
-roulier/carriers/geodis/geodis_decoder_ws.py
-roulier/carriers/geodis/geodis_encoder_edi.py
-roulier/carriers/geodis/geodis_encoder_rest_ws.py
-roulier/carriers/geodis/geodis_encoder_ws.py
-roulier/carriers/geodis/geodis_transport_edi.py
-roulier/carriers/geodis/geodis_transport_rest_ws.py
-roulier/carriers/geodis/geodis_transport_ws.py
-roulier/carriers/geodis/templates/geodis_demandeImpressionEtiquette.xml
-roulier/carriers/geodis/templates/geodis_findLocalite.xml
-roulier/carriers/geodis/templates/geodis_header.xml
-roulier/carriers/geodis/templates/geodis_soap.xml
-roulier/carriers/geodis/tests/__init__.py
-roulier/carriers/geodis/tests/wip_test_rest.py
+roulier/carriers/geodis_fr/__init__.py
+roulier/carriers/geodis_fr/geodis_rest_api.py
+roulier/carriers/geodis_fr/geodis_soap_transport.py
+roulier/carriers/geodis_fr/geodis_transport_rest.py
+roulier/carriers/geodis_fr/edi/__init__.py
+roulier/carriers/geodis_fr/edi/api.py
+roulier/carriers/geodis_fr/edi/carrier_action.py
+roulier/carriers/geodis_fr/edi/encoder.py
+roulier/carriers/geodis_fr/edi/transport.py
+roulier/carriers/geodis_fr/get_label/__init__.py
+roulier/carriers/geodis_fr/get_label/api.py
+roulier/carriers/geodis_fr/get_label/carrier_action.py
+roulier/carriers/geodis_fr/get_label/decoder.py
+roulier/carriers/geodis_fr/get_label/encoder.py
+roulier/carriers/geodis_fr/templates/geodis_get_label.xml
+roulier/carriers/geodis_fr/templates/geodis_header.xml
+roulier/carriers/geodis_fr/templates/geodis_soap.xml
+roulier/carriers/geodis_fr/templates/geodis_validate_address.xml
+roulier/carriers/geodis_fr/tests/__init__.py
+roulier/carriers/geodis_fr/tests/common.py
+roulier/carriers/geodis_fr/tests/test_edi.py
+roulier/carriers/geodis_fr/tests/test_get_label.py
+roulier/carriers/geodis_fr/tests/test_tracking.py
+roulier/carriers/geodis_fr/tests/test_validate_address.py
+roulier/carriers/geodis_fr/tracking/__init__.py
+roulier/carriers/geodis_fr/tracking/api.py
+roulier/carriers/geodis_fr/tracking/carrier_action.py
+roulier/carriers/geodis_fr/tracking/decoder.py
+roulier/carriers/geodis_fr/tracking/encoder.py
+roulier/carriers/geodis_fr/validate_address/__init__.py
+roulier/carriers/geodis_fr/validate_address/api.py
+roulier/carriers/geodis_fr/validate_address/carrier_action.py
+roulier/carriers/geodis_fr/validate_address/decoder.py
+roulier/carriers/geodis_fr/validate_address/encoder.py
 roulier/carriers/gls_fr/__init__.py
 roulier/carriers/gls_fr/glsbox/__init__.py
 roulier/carriers/gls_fr/glsbox/api.py
 roulier/carriers/gls_fr/glsbox/carrier_action.py
 roulier/carriers/gls_fr/glsbox/decoder.py
 roulier/carriers/gls_fr/glsbox/encoder.py
 roulier/carriers/gls_fr/glsbox/gls.py
@@ -104,9 +118,19 @@
 roulier/carriers/laposte_fr/templates/laposte_soap.xml
 roulier/carriers/laposte_fr/tests/__init__.py
 roulier/carriers/laposte_fr/tests/credential_demo.py
 roulier/carriers/laposte_fr/tests/data.py
 roulier/carriers/laposte_fr/tests/test_laposte_basic.py
 roulier/carriers/laposte_fr/tests/test_laposte_europe.py
 roulier/carriers/laposte_fr/tests/test_laposte_outside_europe.py
+roulier/carriers/laposte_fr/tests/test_laposte_parcel_document.py
+roulier/carriers/mondialrelay/__init__.py
+roulier/carriers/mondialrelay/api.py
+roulier/carriers/mondialrelay/carrier_action.py
+roulier/carriers/mondialrelay/decoder.py
+roulier/carriers/mondialrelay/encoder.py
+roulier/carriers/mondialrelay/statuses.py
+roulier/carriers/mondialrelay/transport.py
+roulier/carriers/mondialrelay/templates/mondial_relay_action.xml
+roulier/carriers/mondialrelay/templates/mondial_relay_soap.xml
 roulier/templates/remove_empty_tags.xsl
 tests/__init__.py
```

