# Comparing `tmp/cognite_neat-0.72.2.tar.gz` & `tmp/cognite_neat-0.72.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.72.2.tar", max compression
+gzip compressed data, was "cognite_neat-0.72.3.tar", max compression
```

## Comparing `cognite_neat-0.72.2.tar` & `cognite_neat-0.72.3.tar`

### file list

```diff
@@ -1,233 +1,233 @@
--rw-r--r--   0        0        0    11351 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/README.md
--rw-r--r--   0        0        0       61 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3583 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13653 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     6369 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12402 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-15 13:29:17.391325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      629 2024-04-15 13:29:17.395325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-15 13:29:17.395325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-15 13:29:17.395325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-15 13:29:17.395325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-15 13:29:17.395325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-04-15 13:29:17.395325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1403545 2024-04-15 13:29:17.399325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js
--rw-r--r--   0        0        0     2667 2024-04-15 13:29:17.399325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt
--rw-r--r--   0        0        0  6234629 2024-04-15 13:29:17.427325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map
--rw-r--r--   0        0        0   240334 2024-04-15 13:29:17.427325 cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-15 13:29:17.435325 cognite_neat-0.72.2/cognite/neat/config.py
--rw-r--r--   0        0        0     1228 2024-04-15 13:29:17.435325 cognite_neat-0.72.2/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-15 13:29:17.435325 cognite_neat-0.72.2/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-15 13:29:17.435325 cognite_neat-0.72.2/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-15 13:29:17.439325 cognite_neat-0.72.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/extractor/__init__.py
--rw-r--r--   0        0        0      356 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/extractor/_base.py
--rw-r--r--   0        0        0    11232 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/extractor/_dexpi.py
--rw-r--r--   0        0        0    17408 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/extractor/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14872 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/extractor/_mock_graph_generator.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14969 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      693 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/__init__.py
--rw-r--r--   0        0        0    23838 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/_asset_loader.py
--rw-r--r--   0        0        0     2370 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/_base.py
--rw-r--r--   0        0        0     2837 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/core/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/core/labels.py
--rw-r--r--   0        0        0     5016 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/core/models.py
--rw-r--r--   0        0        0    40458 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22678 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12957 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/loader/validator.py
--rw-r--r--   0        0        0      149 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    14254 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/transformation/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/transformation/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/transformation/query_generator/__init__.py
--rw-r--r--   0        0        0    18659 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/transformation/query_generator/sparql.py
--rw-r--r--   0        0        0    14673 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/graph/transformation/transformer.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/_analysis/__init__.py
--rw-r--r--   0        0        0      674 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/_analysis/_base.py
--rw-r--r--   0        0        0    19613 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/_analysis/_information_rules.py
--rw-r--r--   0        0        0      177 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0     8596 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0     2538 2024-04-15 13:29:17.443325 cognite_neat-0.72.2/cognite/neat/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5501 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0     1439 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_base.py
--rw-r--r--   0        0        0      102 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_core/__init__.py
--rw-r--r--   0        0        0      764 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_core/rules2labels.py
--rw-r--r--   0        0        0    37099 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2dms.py
--rw-r--r--   0        0        0     8220 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2excel.py
--rw-r--r--   0        0        0     6215 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2graphql.py
--rw-r--r--   0        0        0    18414 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2ontology.py
--rw-r--r--   0        0        0    28745 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3866 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2rules.py
--rw-r--r--   0        0        0     1104 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2triples.py
--rw-r--r--   0        0        0     5769 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporter/_validation.py
--rw-r--r--   0        0        0      413 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    12221 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     9080 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19768 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4092 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_base.py
--rw-r--r--   0        0        0     6469 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_dict2rules.py
--rw-r--r--   0        0        0     7890 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_dms2rules.py
--rw-r--r--   0        0        0    12097 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9320 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10521 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1529 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_spreadsheet2rules.py
--rw-r--r--   0        0        0      448 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_xsd2rules.py
--rw-r--r--   0        0        0     1628 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importer/_yaml2rules.py
--rw-r--r--   0        0        0      408 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4268 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0     9138 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12554 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6925 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11926 2024-04-15 13:29:17.447325 cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7674 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7319 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     7119 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    10573 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4198 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     5856 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    12722 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      127 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0      517 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/__init__.py
--rw-r--r--   0        0        0     1299 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/_types/__init__.py
--rw-r--r--   0        0        0    17145 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/_types/_field.py
--rw-r--r--   0        0        0     6308 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/_types/_value.py
--rw-r--r--   0        0        0    10635 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/base.py
--rw-r--r--   0        0        0    50201 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/dms_architect_rules.py
--rw-r--r--   0        0        0    30229 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/dms_schema.py
--rw-r--r--   0        0        0     2051 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/domain_rules.py
--rw-r--r--   0        0        0    21026 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/_rules/information_rules.py
--rw-r--r--   0        0        0    12368 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7344 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51063 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/tables.py
--rw-r--r--   0        0        0     4395 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/rules/models/value_types.py
--rw-r--r--   0        0        0       68 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2699 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26857 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/examples/Export DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/examples/Import DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-15 13:29:17.451326 cognite_neat-0.72.2/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
--rw-r--r--   0        0        0    13659 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6568 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6288 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18272 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0     7327 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4785 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29390 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27269 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12522 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2345 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20657 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28072 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-15 13:29:17.455325 cognite_neat-0.72.2/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4543 2024-04-15 13:29:17.843329 cognite_neat-0.72.2/pyproject.toml
--rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.72.2/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/README.md
+-rw-r--r--   0        0        0       61 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3583 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13653 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     6369 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12402 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      629 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1403545 2024-04-17 07:13:57.588078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js
+-rw-r--r--   0        0        0     2667 2024-04-17 07:13:57.588078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6234629 2024-04-17 07:13:57.612078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map
+-rw-r--r--   0        0        0   240334 2024-04-17 07:13:57.612078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-04-17 07:13:57.620077 cognite_neat-0.72.3/cognite/neat/config.py
+-rw-r--r--   0        0        0     1205 2024-04-17 07:13:57.620077 cognite_neat-0.72.3/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-17 07:13:57.620077 cognite_neat-0.72.3/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-17 07:13:57.620077 cognite_neat-0.72.3/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-17 07:13:57.624078 cognite_neat-0.72.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/_base.py
+-rw-r--r--   0        0        0    11232 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/_dexpi.py
+-rw-r--r--   0        0        0    17408 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14872 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/_mock_graph_generator.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14969 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      693 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/__init__.py
+-rw-r--r--   0        0        0    23838 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/_asset_loader.py
+-rw-r--r--   0        0        0     2370 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/labels.py
+-rw-r--r--   0        0        0     5016 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/models.py
+-rw-r--r--   0        0        0    40458 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22678 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12957 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/validator.py
+-rw-r--r--   0        0        0      149 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14254 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/query_generator/__init__.py
+-rw-r--r--   0        0        0    18659 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/query_generator/sparql.py
+-rw-r--r--   0        0        0    14673 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/_analysis/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/_analysis/_base.py
+-rw-r--r--   0        0        0    19613 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/_analysis/_information_rules.py
+-rw-r--r--   0        0        0      177 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0     8596 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2538 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5501 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0     1439 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_base.py
+-rw-r--r--   0        0        0      102 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_core/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_core/rules2labels.py
+-rw-r--r--   0        0        0    37099 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2dms.py
+-rw-r--r--   0        0        0     8220 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2excel.py
+-rw-r--r--   0        0        0     6215 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2graphql.py
+-rw-r--r--   0        0        0    18414 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2ontology.py
+-rw-r--r--   0        0        0    28745 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3866 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2rules.py
+-rw-r--r--   0        0        0     1104 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2triples.py
+-rw-r--r--   0        0        0     5769 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_validation.py
+-rw-r--r--   0        0        0      413 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    11854 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     9080 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19922 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4092 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0     2316 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_base.py
+-rw-r--r--   0        0        0     6469 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_dict2rules.py
+-rw-r--r--   0        0        0     7890 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_dms2rules.py
+-rw-r--r--   0        0        0    12097 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9320 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10521 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1529 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      448 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_xsd2rules.py
+-rw-r--r--   0        0        0     1628 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_yaml2rules.py
+-rw-r--r--   0        0        0      408 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4268 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0     9138 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12554 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6925 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11926 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7791 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     7120 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11481 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4198 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     5856 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    12722 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      127 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0      517 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/__init__.py
+-rw-r--r--   0        0        0     1299 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/__init__.py
+-rw-r--r--   0        0        0    16681 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_base.py
+-rw-r--r--   0        0        0    10295 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_field.py
+-rw-r--r--   0        0        0     6308 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_value.py
+-rw-r--r--   0        0        0    10635 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/base.py
+-rw-r--r--   0        0        0    50424 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/dms_architect_rules.py
+-rw-r--r--   0        0        0    30229 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/dms_schema.py
+-rw-r--r--   0        0        0     2051 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/domain_rules.py
+-rw-r--r--   0        0        0    21026 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/information_rules.py
+-rw-r--r--   0        0        0    12368 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7344 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51063 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/tables.py
+-rw-r--r--   0        0        0     4395 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/value_types.py
+-rw-r--r--   0        0        0       68 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11063 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2699 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26857 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Export DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Import DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
+-rw-r--r--   0        0        0    13659 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6568 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6288 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18234 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0     7327 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4785 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29390 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27269 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12522 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2345 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20657 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28072 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4543 2024-04-17 07:13:58.032077 cognite_neat-0.72.3/pyproject.toml
+-rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.72.3/PKG-INFO
```

### Comparing `cognite_neat-0.72.2/LICENSE` & `cognite_neat-0.72.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/README.md` & `cognite_neat-0.72.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/configuration.py` & `cognite_neat-0.72.3/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.72.3/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.72.3/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/explorer.py` & `cognite_neat-0.72.3/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.72.3/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.72.3/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.72.3/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.72.3/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.72.3/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.72.3/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.72.3/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.72.3/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.72.3/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.72.3/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/config.py` & `cognite_neat-0.72.3/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/constants.py` & `cognite_neat-0.72.3/cognite/neat/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 PACKAGE_DIRECTORY = Path(neat.__file__).parent
 
 
 EXAMPLE_RULES = PACKAGE_DIRECTORY / "rules" / "examples"
 EXAMPLE_GRAPHS = PACKAGE_DIRECTORY / "graph" / "examples"
 EXAMPLE_WORKFLOWS = PACKAGE_DIRECTORY / "workflows" / "examples"
 
+DEFAULT_NAMESPACE = Namespace("http://purl.org/cognite/neat#")
 
 PREFIXES = {
     "rdf": RDF._NS,
     "rdfs": RDFS._NS,
     "dct": DCTERMS._NS,
     "skos": SKOS._NS,
     "owl": OWL._NS,
@@ -23,14 +24,14 @@
     "cim": Namespace("http://iec.ch/TC57/2013/CIM-schema-cim16#"),
     "icim": Namespace("http://iec.ch/TC57/2013/CIM-schema-cim16-info#"),
     "entsoe": Namespace("http://entsoe.eu/CIM/SchemaExtension/3/1#"),
     "entsoe2": Namespace("http://entsoe.eu/CIM/SchemaExtension/3/2#"),
     "md": Namespace("http://iec.ch/TC57/61970-552/ModelDescription/1#"),
     "pti": Namespace("http://www.pti-us.com/PTI_CIM-schema-cim16#"),
     "tnt": Namespace("http://purl.org/cognite/tnt#"),
-    "neat": Namespace("http://purl.org/cognite/neat#"),
+    "neat": DEFAULT_NAMESPACE,
 }
 
-DEFAULT_NAMESPACE = Namespace("http://purl.org/cognite/app#")
+
 DEFAULT_URI = ""
 
 DEFAULT_DOCS_URL = "https://cognite-neat.readthedocs-hosted.com/en/latest/"
```

### Comparing `cognite_neat-0.72.2/cognite/neat/exceptions.py` & `cognite_neat-0.72.3/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.72.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.72.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.72.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/exceptions.py` & `cognite_neat-0.72.3/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/extractor/_dexpi.py` & `cognite_neat-0.72.3/cognite/neat/graph/extractor/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/extractor/_graph_capturing_sheet.py` & `cognite_neat-0.72.3/cognite/neat/graph/extractor/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/extractor/_mock_graph_generator.py` & `cognite_neat-0.72.3/cognite/neat/graph/extractor/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.72.3/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/__init__.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/_asset_loader.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/_base.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/_exceptions.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/core/labels.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/core/models.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/core/rdf_to_assets.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/core/rdf_to_relationships.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/rdf_to_dms.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/loader/validator.py` & `cognite_neat-0.72.3/cognite/neat/graph/loader/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.72.3/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.72.3/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.72.3/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.72.3/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.72.3/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.72.3/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.72.3/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/transformation/entity_matcher.py` & `cognite_neat-0.72.3/cognite/neat/graph/transformation/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/transformation/query_generator/sparql.py` & `cognite_neat-0.72.3/cognite/neat/graph/transformation/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/graph/transformation/transformer.py` & `cognite_neat-0.72.3/cognite/neat/graph/transformation/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/_analysis/_base.py` & `cognite_neat-0.72.3/cognite/neat/rules/_analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/_analysis/_information_rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/_analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/analysis.py` & `cognite_neat-0.72.3/cognite/neat/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.72.3/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.72.3/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/__init__.py` & `cognite_neat-0.72.3/cognite/neat/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/power-grid-model.yaml` & `cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/rules-template.xlsx` & `cognite_neat-0.72.3/cognite/neat/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.72.3/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/skos-rules.xlsx` & `cognite_neat-0.72.3/cognite/neat/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.72.3/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.72.3/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exceptions.py` & `cognite_neat-0.72.3/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/__init__.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_base.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_core/rules2labels.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2dms.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2excel.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2graphql.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2ontology.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2pydantic_models.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_rules2triples.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporter/_validation.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporter/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,14 @@
     Args:
         export_components (frozenset[Literal["all", "spaces", "data_models", "views", "containers"]], optional):
             Which components to export. Defaults to frozenset({"all"}).
         include_space (set[str], optional):
             If set, only export components in the given spaces. Defaults to None which means all spaces.
         existing_handling (Literal["fail", "skip", "update", "force"], optional): How to handle existing components.
             Defaults to "update". See below for details.
-        standardize_casing(bool, optional): Whether to standardize the casing. This means PascalCase for external ID
-            of views, containers, and data models, and camelCase for properties.
         export_pipeline (bool, optional): Whether to export the pipeline. Defaults to False. This means setting
             up transformations, RAW databases and tables to populate the data model.
         instance_space (str, optional): The space to use for the instance. Defaults to None.
     ... note::
 
         - "fail": If any component already exists, the export will fail.
         - "skip": If any component already exists, it will be skipped.
@@ -55,22 +53,20 @@
     """
 
     def __init__(
         self,
         export_components: Component | Collection[Component] = "all",
         include_space: set[str] | None = None,
         existing_handling: Literal["fail", "skip", "update", "force"] = "update",
-        standardize_casing: bool = True,
         export_pipeline: bool = False,
         instance_space: str | None = None,
     ):
         self.export_components = {export_components} if isinstance(export_components, str) else set(export_components)
         self.include_space = include_space
         self.existing_handling = existing_handling
-        self.standardize_casing = standardize_casing
         self.export_pipeline = export_pipeline
         self.instance_space = instance_space
         self._schema: DMSSchema | None = None
 
     def export_to_file(self, rules: Rules, filepath: Path) -> None:
         """Export the rules to a file(s).
 
@@ -115,19 +111,19 @@
             raise ValueError(f"{type(rules).__name__} cannot be exported to DMS")
 
         is_solution_model = (
             dms_rules.reference and dms_rules.metadata.external_id != dms_rules.reference.metadata.external_id
         )
         is_new_model = dms_rules.reference is None
         if is_new_model or is_solution_model:
-            return dms_rules.as_schema(self.standardize_casing, self.export_pipeline, self.instance_space)
+            return dms_rules.as_schema(self.export_pipeline, self.instance_space)
 
         # This is an extension of an existing model.
         reference_rules = cast(DMSRules, dms_rules.reference).copy(deep=True)
-        reference_schema = reference_rules.as_schema(self.standardize_casing, self.export_pipeline)
+        reference_schema = reference_rules.as_schema(self.export_pipeline)
 
         # Todo Move this to an appropriate location
         # Merging Reference with User Rules
         combined_rules = dms_rules.copy(deep=True)
         existing_containers = {container.class_ for container in combined_rules.containers or []}
         if combined_rules.containers is None:
             combined_rules.containers = SheetList[DMSContainer](data=[])
@@ -142,15 +138,15 @@
                 combined_rules.views.append(view)
         existing_properties = {(property_.class_, property_.property_) for property_ in combined_rules.properties}
         for property_ in reference_rules.properties:
             if (property_.class_, property_.property_) not in existing_properties:
                 property_.reference = None
                 combined_rules.properties.append(property_)
 
-        schema = combined_rules.as_schema(self.standardize_casing, self.export_pipeline, self.instance_space)
+        schema = combined_rules.as_schema(self.export_pipeline, self.instance_space)
 
         if dms_rules.metadata.extension in (ExtensionCategory.addition, ExtensionCategory.reshape):
             # We do not freeze views as they might be changed, even for addition,
             # in case, for example, new properties are added. The validation will catch this.
             schema.frozen_ids.update(set(reference_schema.containers.as_ids()))
             schema.frozen_ids.update(set(reference_schema.node_types.as_ids()))
         return schema
```

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from typing import ClassVar
 
 from pydantic import BaseModel, ConfigDict, ValidationInfo, field_validator
 from rdflib import DCTERMS, OWL, RDF, RDFS, XSD, BNode, Graph, Literal, Namespace, URIRef
 from rdflib.collection import Collection as GraphCollection
 
+from cognite.neat.constants import DEFAULT_NAMESPACE as NEAT_NAMESPACE
 from cognite.neat.rules import exceptions
 from cognite.neat.rules._analysis._information_rules import InformationArchitectRulesAnalysis
 from cognite.neat.rules.models._rules import DMSRules
 from cognite.neat.rules.models._rules._types import XSD_VALUE_TYPE_MAPPINGS, EntityTypes
 from cognite.neat.rules.models._rules.information_rules import (
     InformationClass,
     InformationMetadata,
@@ -213,14 +214,15 @@
         # Mandatory triples originating from Metadata mandatory fields
         if self.namespace is None:
             raise exceptions.MetadataSheetNamespaceNotDefined()
         triples: list[tuple] = [
             (URIRef(self.namespace), DCTERMS.hasVersion, Literal(self.version)),
             (URIRef(self.namespace), OWL.versionInfo, Literal(self.version)),
             (URIRef(self.namespace), RDFS.label, Literal(self.name)),
+            (URIRef(self.namespace), NEAT_NAMESPACE.prefix, Literal(self.prefix)),
             (URIRef(self.namespace), DCTERMS.title, Literal(self.name)),
             (URIRef(self.namespace), DCTERMS.created, Literal(self.created, datatype=XSD.dateTime)),
             (URIRef(self.namespace), DCTERMS.description, Literal(self.description)),
         ]
         if isinstance(self.creator, list):
             triples.extend([(URIRef(self.namespace), DCTERMS.creator, Literal(creator)) for creator in self.creator])
         else:
```

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.72.3/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/__init__.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_base.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_dict2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_dms2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_graph2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_json2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/_owl2classes.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/_owl2properties.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_owl2rules/_owl2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_spreadsheet2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importer/_yaml2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importer/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import re
 
 from rdflib import Graph, Namespace
 
+from cognite.neat.constants import DEFAULT_NAMESPACE
 from cognite.neat.rules.models._rules.base import RoleTypes, SchemaCompleteness
 from cognite.neat.rules.models.rules import (
     prefix_compliance_regex,
     version_compliance_regex,
 )
 from cognite.neat.utils.utils import convert_rdflib_content, remove_none_elements_from_set
 
@@ -25,31 +26,31 @@
         If `make_compliant` is set to True, in presence of errors, default values will be used instead.
         This makes the method very opinionated, but results in a compliant metadata.
 
 
     """
     # TODO: Move dataframe to dict representation
 
-    query = """SELECT ?namespace ?prefix ?version ?created ?updated ?title ?description ?creator ?rights ?license
-    WHERE {
+    query = f"""SELECT ?namespace ?prefix ?version ?created ?updated ?title ?description ?creator ?rights ?license
+    WHERE {{
         ?namespace a owl:Ontology .
-        OPTIONAL {?namespace owl:versionInfo ?version }.
-        OPTIONAL {?namespace dcterms:creator ?creator }.
-        OPTIONAL {?namespace dcterms:title|rdfs:label|skos:prefLabel ?title }.
-        OPTIONAL {?namespace dcterms:modified ?updated }.
-        OPTIONAL {?namespace dcterms:created ?created }.
-        OPTIONAL {?namespace dcterms:description ?description }.
+        OPTIONAL {{?namespace owl:versionInfo ?version }}.
+        OPTIONAL {{?namespace dcterms:creator ?creator }}.
+        OPTIONAL {{?namespace <{DEFAULT_NAMESPACE.prefix}> ?prefix }}.
+        OPTIONAL {{?namespace dcterms:title|rdfs:label|skos:prefLabel ?title }}.
+        OPTIONAL {{?namespace dcterms:modified ?updated }}.
+        OPTIONAL {{?namespace dcterms:created ?created }}.
+        OPTIONAL {{?namespace dcterms:description ?description }}.
+        OPTIONAL {{?namespace dcterms:rights|dc:rights ?rights }}.
 
-        OPTIONAL {?namespace dcterms:rights|dc:rights ?rights }.
-
-        OPTIONAL {?namespace dcterms:license|dc:license ?license }.
+        OPTIONAL {{?namespace dcterms:license|dc:license ?license }}.
         FILTER (!isBlank(?namespace))
         FILTER (!bound(?description) || LANG(?description) = "" || LANGMATCHES(LANG(?description), "en"))
         FILTER (!bound(?title) || LANG(?title) = "" || LANGMATCHES(LANG(?title), "en"))
-    }
+    }}
     """
 
     results = [{item for item in sublist} for sublist in list(zip(*graph.query(query), strict=True))]
 
     raw_metadata = convert_rdflib_content(
         {
             "role": RoleTypes.information_architect,
@@ -68,15 +69,14 @@
             ),
             "rights": results[8].pop(),
             "license": results[9].pop(),
         }
     )
 
     if make_compliant:
-        raw_metadata.pop("created")
         return make_metadata_compliant(raw_metadata)
 
     return raw_metadata
 
 
 def make_metadata_compliant(metadata: dict) -> dict:
     """Attempts to fix errors in metadata, otherwise defaults to values that will pass validation.
@@ -172,15 +172,15 @@
     metadata: dict,
     date_type: str,
     default: datetime.datetime,
 ) -> dict:
     if date := metadata.get(date_type, None):
         try:
             if isinstance(date, datetime.datetime):
-                pass
+                return metadata
             elif isinstance(date, datetime.date):
                 metadata[date_type] = datetime.datetime.combine(metadata[date_type], datetime.datetime.min.time())
             elif isinstance(date, str):
                 metadata[date_type] = datetime.datetime.strptime(metadata[date_type], "%Y-%m-%dT%H:%M:%SZ")
             else:
                 metadata[date_type] = default
         except Exception:
```

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         OPTIONAL {?property owl:maxCardinality ?maxCount} .
         OPTIONAL {?property owl:minCardinality ?minCount} .
         FILTER (!isBlank(?property))
         FILTER (!bound(?type) || !isBlank(?type))
         FILTER (!bound(?class) || !isBlank(?class))
         FILTER (!bound(?name) || LANG(?name) = "" || LANGMATCHES(LANG(?name), "en"))
         FILTER (!bound(?description) || LANG(?description) = "" || LANGMATCHES(LANG(?description), "en"))
+        BIND(IF(bound(?minCount), ?minCount, 0) AS ?minCount)
+        BIND(IF(bound(?maxCount), ?maxCount, 1) AS ?maxCount)
     }
     """
 
     raw_df = _parse_raw_dataframe(cast(list[tuple], list(graph.query(query.replace("en", language)))))
     if raw_df.empty:
         return []
```

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         the imported rules compliant by adding default values for missing information, attaching dangling
         properties to default containers based on the property type, etc. One has to be aware
         that NEAT will be opinionated about how to make the ontology compliant, and that the resulting
         rules may not be what you expect.
 
     """
 
-    def __init__(self, owl_filepath: Path, make_compliant: bool = True):
+    def __init__(self, owl_filepath: Path, make_compliant: bool = False):
         self.owl_filepath = owl_filepath
         self.make_compliant = make_compliant
 
     @overload
     def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
         ...
```

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This module performs importing of graph to TransformationRules pydantic class.
 In more details, it traverses the graph and abstracts class and properties, basically
 generating a list of rules based on which nodes that form the graph are made.
 """
 
 from collections import UserDict, defaultdict
+from dataclasses import dataclass
 from pathlib import Path
 from typing import Literal, cast, overload
 
 import pandas as pd
 from pandas import ExcelFile
 
 from cognite.neat.rules import issues
@@ -45,26 +46,40 @@
     def role(self) -> RoleTypes:
         return RoleTypes(self["role"])
 
     @property
     def has_schema_field(self) -> bool:
         return self.get("schema") in [schema.value for schema in SchemaCompleteness.__members__.values()]
 
+    @property
+    def schema(self) -> SchemaCompleteness | None:
+        if not self.has_schema_field:
+            return None
+        return SchemaCompleteness(self["schema"])
+
     def is_valid(self, issue_list: IssueList, filepath: Path) -> bool:
         if not self.has_role_field:
             issue_list.append(issues.spreadsheet_file.RoleMissingOrUnsupportedError(filepath))
             return False
 
         # check if there is a schema field if role is not domain expert
         if self.role != RoleTypes.domain_expert and not self.has_schema_field:
             issue_list.append(issues.spreadsheet_file.SchemaMissingOrUnsupportedError(filepath))
             return False
         return True
 
 
+@dataclass
+class ReadResult:
+    sheets: dict[str, dict | list]
+    read_info_by_sheet: dict[str, SpreadsheetRead]
+    role: RoleTypes
+    schema: SchemaCompleteness | None
+
+
 class SpreadsheetReader:
     def __init__(self, issue_list: IssueList, is_reference: bool = False):
         self.issue_list = issue_list
         self._is_reference = is_reference
 
     @property
     def metadata_sheet_name(self) -> str:
@@ -75,15 +90,15 @@
         names = MANDATORY_SHEETS_BY_ROLE[role]
         return {self.to_reference_sheet(sheet_name) for sheet_name in names} if self._is_reference else names
 
     @classmethod
     def to_reference_sheet(cls, sheet_name: str) -> str:
         return f"Ref{sheet_name}"
 
-    def read(self, filepath: Path) -> Rules | None:
+    def read(self, filepath: Path) -> None | ReadResult:
         with pd.ExcelFile(filepath) as excel_file:
             if self.metadata_sheet_name not in excel_file.sheet_names:
                 self.issue_list.append(
                     issues.spreadsheet_file.MetadataSheetMissingOrFailedError(
                         filepath, sheet_name=self.metadata_sheet_name
                     )
                 )
@@ -91,29 +106,18 @@
 
             metadata = MetadataRaw.from_excel(excel_file, self.metadata_sheet_name)
 
             if not metadata.is_valid(self.issue_list, filepath):
                 return None
 
             sheets, read_info_by_sheet = self._read_sheets(metadata, excel_file)
-            if self.issue_list.has_errors:
-                return None
-
-            rules_cls = RULES_PER_ROLE[metadata.role]
-            with _handle_issues(
-                self.issue_list,
-                error_cls=issues.spreadsheet.InvalidSheetError,
-                error_args={"read_info_by_sheet": read_info_by_sheet},
-            ) as future:
-                rules = rules_cls.model_validate(sheets)  # type: ignore[attr-defined]
-
-            if future.result == "failure" or self.issue_list.has_errors:
+            if sheets is None or self.issue_list.has_errors:
                 return None
 
-        return rules
+            return ReadResult(sheets, read_info_by_sheet, metadata.role, metadata.schema)
 
     def _read_sheets(
         self, metadata: MetadataRaw, excel_file: ExcelFile
     ) -> tuple[dict[str, dict | list] | None, dict[str, SpreadsheetRead]]:
         read_info_by_sheet: dict[str, SpreadsheetRead] = defaultdict(SpreadsheetRead)
 
         sheets: dict[str, dict | list] = {"Metadata": dict(metadata)}
@@ -163,51 +167,68 @@
     def to_rules(
         self,
         errors: Literal["raise", "continue"] = "continue",
         role: RoleTypes | None = None,
         is_reference: bool = False,
     ) -> tuple[Rules | None, IssueList] | Rules:
         issue_list = IssueList(title=f"'{self.filepath.name}'")
-
         if not self.filepath.exists():
             issue_list.append(issues.spreadsheet_file.SpreadsheetNotFoundError(self.filepath))
             return self._return_or_raise(issue_list, errors)
 
-        user_rules: Rules | None = None
+        user_result: ReadResult | None = None
         if not is_reference:
-            user_rules = SpreadsheetReader(issue_list, is_reference=False).read(self.filepath)
-            if issue_list.has_errors:
+            user_result = SpreadsheetReader(issue_list, is_reference=False).read(self.filepath)
+            if user_result is None or issue_list.has_errors:
                 return self._return_or_raise(issue_list, errors)
 
-        reference_rules: Rules | None = None
+        reference_result: ReadResult | None = None
         if is_reference or (
-            user_rules
-            and user_rules.metadata.role != RoleTypes.domain_expert
-            and cast(DMSRules | InformationRules, user_rules).metadata.schema_ == SchemaCompleteness.extended
+            user_result
+            and user_result.role != RoleTypes.domain_expert
+            and user_result.schema == SchemaCompleteness.extended
         ):
-            reference_rules = SpreadsheetReader(issue_list, is_reference=True).read(self.filepath)
+            reference_result = SpreadsheetReader(issue_list, is_reference=True).read(self.filepath)
             if issue_list.has_errors:
                 return self._return_or_raise(issue_list, errors)
 
-        if user_rules and reference_rules and user_rules.metadata.role != reference_rules.metadata.role:
+        if user_result and reference_result and user_result.role != reference_result.role:
             issue_list.append(issues.spreadsheet_file.RoleMismatchError(self.filepath))
             return self._return_or_raise(issue_list, errors)
 
-        if user_rules and reference_rules:
-            rules = user_rules
-            rules.reference = reference_rules
-        elif user_rules:
-            rules = user_rules
-        elif reference_rules:
-            rules = reference_rules
+        if user_result and reference_result:
+            user_result.sheets["reference"] = reference_result.sheets
+            sheets = user_result.sheets
+            original_role = user_result.role
+            read_info_by_sheet = user_result.read_info_by_sheet
+            read_info_by_sheet.update(reference_result.read_info_by_sheet)
+        elif user_result:
+            sheets = user_result.sheets
+            original_role = user_result.role
+            read_info_by_sheet = user_result.read_info_by_sheet
+        elif reference_result:
+            sheets = reference_result.sheets
+            original_role = reference_result.role
+            read_info_by_sheet = reference_result.read_info_by_sheet
         else:
             raise ValueError(
                 "No rules were generated. This should have been caught earlier. " f"Bug in {type(self).__name__}."
             )
 
+        rules_cls = RULES_PER_ROLE[original_role]
+        with _handle_issues(
+            issue_list,
+            error_cls=issues.spreadsheet.InvalidSheetError,
+            error_args={"read_info_by_sheet": read_info_by_sheet},
+        ) as future:
+            rules = rules_cls.model_validate(sheets)  # type: ignore[attr-defined]
+
+        if future.result == "failure" or issue_list.has_errors:
+            return self._return_or_raise(issue_list, errors)
+
         return self._to_output(
             rules,
             issue_list,
             errors=errors,
             role=role,
             is_reference=is_reference,
         )
```

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.72.3/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/issues/base.py` & `cognite_neat-0.72.3/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.72.3/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.72.3/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.72.3/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.72.3/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.72.3/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.72.3/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_base.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/__init__.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/_types/__init__.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/_types/_base.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     SINGLE_PROPERTY_REGEX_COMPILED,
     AllReferences,
     RDFPath,
     SingleProperty,
     TransformationRuleType,
     parse_rule,
 )
-from cognite.neat.utils.text import to_pascal
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:
     from backports.strenum import StrEnum
     from typing_extensions import Self
@@ -193,23 +192,22 @@
         else:
             return ContainerEntity(prefix=Undefined, suffix=value)
 
     @classmethod
     def from_id(cls, container_id: ContainerId) -> "ContainerEntity":
         return ContainerEntity(prefix=container_id.space, suffix=container_id.external_id)
 
-    def as_id(self, default_space: str | None, standardize_casing: bool = True) -> ContainerId:
+    def as_id(self, default_space: str | None) -> ContainerId:
         if self.space is Undefined and default_space is None:
             raise ValueError("Space is Undefined! Set default_space!")
 
-        external_id = to_pascal(self.external_id) if standardize_casing else self.external_id
         if self.space is Undefined:
-            return ContainerId(space=cast(str, default_space), external_id=external_id)
+            return ContainerId(space=cast(str, default_space), external_id=self.external_id)
         else:
-            return ContainerId(space=self.space, external_id=external_id)
+            return ContainerId(space=self.space, external_id=self.external_id)
 
 
 class ViewEntity(Entity):
     type_: ClassVar[EntityTypes] = EntityTypes.view
 
     @classmethod
     def from_raw(cls, value: Any) -> "ViewEntity":
@@ -229,48 +227,44 @@
 
     @overload
     def as_id(
         self,
         allow_none: Literal[False] = False,
         default_space: str | None = None,
         default_version: str | None = None,
-        standardize_casing: bool = True,
     ) -> ViewId:
         ...
 
     @overload
     def as_id(
         self,
         allow_none: Literal[True],
         default_space: str | None = None,
         default_version: str | None = None,
-        standardize_casing: bool = True,
     ) -> ViewId | None:
         ...
 
     def as_id(
         self,
         allow_none: bool = False,
         default_space: str | None = None,
         default_version: str | None = None,
-        standardize_casing: bool = True,
     ) -> ViewId | None:
         if self.suffix is Unknown and allow_none:
             return None
         elif self.suffix is Unknown:
             raise ValueError("suffix is Unknown and cannot be converted to ViewId")
         space = default_space if self.space is Undefined else self.space
         version = self.version or default_version
 
         if space is None or space is Undefined:
             raise ValueError("space is required")
         if version is None:
             raise ValueError("version is required")
-        external_id = to_pascal(self.external_id) if standardize_casing else self.external_id
-        return ViewId(space=space, external_id=external_id, version=version)
+        return ViewId(space=space, external_id=self.external_id, version=version)
 
 
 class ViewPropEntity(ViewEntity):
     type_: ClassVar[EntityTypes] = EntityTypes.view_prop
     property_: str | None = None
 
     @classmethod
@@ -299,22 +293,18 @@
         return ViewPropEntity(
             prefix=prop_id.source.space,
             suffix=prop_id.source.external_id,
             version=prop_id.source.version,
             property_=prop_id.property,
         )
 
-    def as_prop_id(
-        self, default_space: str | None = None, default_version: str | None = None, standardize_casing: bool = True
-    ) -> PropertyId:
+    def as_prop_id(self, default_space: str | None = None, default_version: str | None = None) -> PropertyId:
         if self.property_ is None:
             raise ValueError("property is required to create PropertyId")
-        return PropertyId(
-            source=self.as_id(False, default_space, default_version, standardize_casing), property=self.property_
-        )
+        return PropertyId(source=self.as_id(False, default_space, default_version), property=self.property_)
 
     @property
     def versioned_id(self) -> str:
         if self.version is None and self.property_ is None:
             output = self.id
         elif self.version is None:
             output = f"{self.id}(property={self.property_})"
```

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/_types/_field.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/_types/_value.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/base.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/dms_architect_rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/dms_architect_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from pydantic import Field, field_validator, model_serializer, model_validator
 from pydantic_core.core_schema import SerializationInfo, ValidationInfo
 from rdflib import Namespace
 
 import cognite.neat.rules.issues.spreadsheet
 from cognite.neat.rules import issues
 from cognite.neat.rules.models._rules.domain_rules import DomainRules
-from cognite.neat.utils.text import to_camel
 
 from ._types import (
     CdfValueType,
     ClassEntity,
     ContainerEntity,
     ContainerListType,
     ContainerType,
@@ -203,19 +202,19 @@
 
 
 class DMSContainer(SheetEntity):
     container: ContainerType = Field(alias="Container")
     reference: ReferenceType = Field(alias="Reference", default=None)
     constraint: ContainerListType | None = Field(None, alias="Constraint")
 
-    def as_container(self, default_space: str, standardize_casing: bool = True) -> dm.ContainerApply:
-        container_id = self.container.as_id(default_space, standardize_casing)
+    def as_container(self, default_space: str) -> dm.ContainerApply:
+        container_id = self.container.as_id(default_space)
         constraints: dict[str, dm.Constraint] = {}
         for constraint in self.constraint or []:
-            requires = dm.RequiresConstraint(constraint.as_id(default_space, standardize_casing))
+            requires = dm.RequiresConstraint(constraint.as_id(default_space))
             constraints[f"{constraint.space}_{constraint.external_id}"] = requires
 
         return dm.ContainerApply(
             space=container_id.space,
             external_id=container_id.external_id,
             name=self.name or None,
             description=self.description,
@@ -242,26 +241,23 @@
 class DMSView(SheetEntity):
     view: ViewType = Field(alias="View")
     implements: ViewListType | None = Field(None, alias="Implements")
     reference: ReferenceType = Field(alias="Reference", default=None)
     filter_: Literal["hasData", "nodeType"] | None = Field(None, alias="Filter")
     in_model: bool = Field(True, alias="InModel")
 
-    def as_view(self, default_space: str, default_version: str, standardize_casing: bool = True) -> dm.ViewApply:
-        view_id = self.view.as_id(False, default_space, default_version, standardize_casing)
+    def as_view(self, default_space: str, default_version: str) -> dm.ViewApply:
+        view_id = self.view.as_id(False, default_space, default_version)
         return dm.ViewApply(
             space=view_id.space,
             external_id=view_id.external_id,
             version=view_id.version or default_version,
             name=self.name or None,
             description=self.description,
-            implements=[
-                parent.as_id(False, default_space, default_version, standardize_casing)
-                for parent in self.implements or []
-            ]
+            implements=[parent.as_id(False, default_space, default_version) for parent in self.implements or []]
             or None,
             properties={},
         )
 
     @classmethod
     def from_view(cls, view: dm.ViewApply, data_model_view_ids: set[dm.ViewId]) -> "DMSView":
         return cls(
@@ -560,18 +556,16 @@
         return {
             "Metadata" if info.by_alias else "metadata": self.metadata.model_dump(**kwargs),
             "Properties" if info.by_alias else "properties": properties,
             "Views" if info.by_alias else "views": views,
             "Containers" if info.by_alias else "containers": containers,
         }
 
-    def as_schema(
-        self, standardize_casing: bool = True, include_pipeline: bool = False, instance_space: str | None = None
-    ) -> DMSSchema:
-        return _DMSExporter(standardize_casing, include_pipeline, instance_space).to_schema(self)
+    def as_schema(self, include_pipeline: bool = False, instance_space: str | None = None) -> DMSSchema:
+        return _DMSExporter(include_pipeline, instance_space).to_schema(self)
 
     def as_information_architect_rules(self) -> "InformationRules":
         return _DMSRulesConverter(self).as_information_architect_rules()
 
     def as_domain_expert_rules(self) -> DomainRules:
         return _DMSRulesConverter(self).as_domain_rules()
 
@@ -595,25 +589,20 @@
 class _DMSExporter:
     """The DMS Exporter is responsible for exporting the DMSRules to a DMSSchema.
 
     This kept in this location such that it can be used by the DMSRules to validate the schema.
     (This module cannot have a dependency on the exporter module, as it would create a circular dependency.)
 
     Args
-        standardize_casing (bool): If True, the casing of the identifiers will be standardized. This means external IDs
-            are PascalCase and property names are camelCase.
         include_pipeline (bool): If True, the pipeline will be included with the schema. Pipeline means the
             raw tables and transformations necessary to populate the data model.
         instance_space (str): The space to use for the instance. Defaults to None,`Rules.metadata.space` will be used
     """
 
-    def __init__(
-        self, standardize_casing: bool = True, include_pipeline: bool = False, instance_space: str | None = None
-    ):
-        self.standardize_casing = standardize_casing
+    def __init__(self, include_pipeline: bool = False, instance_space: str | None = None):
         self.include_pipeline = include_pipeline
         self.instance_space = instance_space
 
     def to_schema(self, rules: DMSRules) -> DMSSchema:
         default_version = "1"
         default_space = rules.metadata.space
 
@@ -624,17 +613,15 @@
         containers = self._create_containers(rules.containers, container_properties_by_id, default_space)
 
         views, node_types = self._create_views_with_node_types(
             rules.views, view_properties_by_id, default_space, default_version
         )
 
         views_not_in_model = {
-            view.view.as_id(False, default_space, default_version, self.standardize_casing)
-            for view in rules.views
-            if not view.in_model
+            view.view.as_id(False, default_space, default_version) for view in rules.views if not view.in_model
         }
         data_model = rules.metadata.as_data_model()
         data_model.views = sorted(
             [view_id for view_id in views.as_ids() if view_id not in views_not_in_model], key=lambda v: v.as_tuple()  # type: ignore[union-attr]
         )
 
         spaces = self._create_spaces(rules.metadata, containers, views, data_model)
@@ -671,85 +658,87 @@
     def _create_views_with_node_types(
         self,
         dms_views: SheetList[DMSView],
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]],
         default_space: str,
         default_version: str,
     ) -> tuple[dm.ViewApplyList, dm.NodeApplyList]:
-        views = dm.ViewApplyList(
-            [dms_view.as_view(default_space, default_version, self.standardize_casing) for dms_view in dms_views]
-        )
+        views = dm.ViewApplyList([dms_view.as_view(default_space, default_version) for dms_view in dms_views])
         dms_view_by_id = {
-            dms_view.view.as_id(False, default_space, default_version, self.standardize_casing): dms_view
-            for dms_view in dms_views
+            dms_view.view.as_id(False, default_space, default_version): dms_view for dms_view in dms_views
         }
 
         for view in views:
             view_id = view.as_id()
             view.properties = {}
             if not (view_properties := view_properties_by_id.get(view_id)):
                 continue
             for prop in view_properties:
                 view_property: ViewPropertyApply
                 if prop.is_list and prop.relation == "direct":
                     # This is not yet supported in the CDF API, a warning has already been issued, here we convert it to
                     # a multi-edge connection.
                     if isinstance(prop.value_type, ViewEntity):
-                        source = prop.value_type.as_id(False, default_space, default_version, self.standardize_casing)
+                        source = prop.value_type.as_id(False, default_space, default_version)
                     else:
                         raise ValueError(
                             "Direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     view_property = dm.MultiEdgeConnectionApply(
                         type=dm.DirectRelationReference(
                             space=source.space,
                             external_id=f"{prop.view.external_id}.{prop.view_property}",
                         ),
                         source=source,
                         direction="outwards",
                     )
                 elif prop.container and prop.container_property and prop.view_property:
-                    container_prop_identifier = (
-                        to_camel(prop.container_property) if self.standardize_casing else prop.container_property
-                    )
+                    container_prop_identifier = prop.container_property
                     extra_args: dict[str, Any] = {}
                     if prop.relation == "direct" and isinstance(prop.value_type, ViewEntity):
-                        extra_args["source"] = prop.value_type.as_id(
-                            True, default_space, default_version, self.standardize_casing
-                        )
+                        extra_args["source"] = prop.value_type.as_id(True, default_space, default_version)
                     elif prop.relation == "direct" and not isinstance(prop.value_type, ViewEntity):
                         raise ValueError(
                             "Direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     view_property = dm.MappedPropertyApply(
-                        container=prop.container.as_id(default_space, self.standardize_casing),
+                        container=prop.container.as_id(default_space),
                         container_property_identifier=container_prop_identifier,
                         **extra_args,
                     )
                 elif prop.view and prop.view_property and prop.relation == "multiedge":
                     if isinstance(prop.value_type, ViewEntity):
-                        source = prop.value_type.as_id(False, default_space, default_version, self.standardize_casing)
+                        source = prop.value_type.as_id(False, default_space, default_version)
                     else:
                         raise ValueError(
                             "Multiedge relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
-                    view_property = dm.MultiEdgeConnectionApply(
-                        type=dm.DirectRelationReference(
+                    if isinstance(prop.reference, ReferenceEntity):
+                        ref_view_prop = prop.reference.as_prop_id(default_space, default_version)
+                        edge_type = dm.DirectRelationReference(
+                            space=ref_view_prop.source.space,
+                            external_id=f"{ref_view_prop.source.external_id}.{ref_view_prop.property}",
+                        )
+                    else:
+                        edge_type = dm.DirectRelationReference(
                             space=source.space,
                             external_id=f"{prop.view.external_id}.{prop.view_property}",
-                        ),
+                        )
+
+                    view_property = dm.MultiEdgeConnectionApply(
+                        type=edge_type,
                         source=source,
                         direction="outwards",
                     )
                 elif prop.view and prop.view_property and prop.relation == "reversedirect":
                     if isinstance(prop.value_type, ViewPropEntity):
-                        source = prop.value_type.as_id(False, default_space, default_version, self.standardize_casing)
+                        source = prop.value_type.as_id(False, default_space, default_version)
                     else:
                         raise ValueError(
                             "Reverse direct relation must have a view as value type. "
                             "This should have been validated in the rules"
                         )
                     source_prop = prop.value_type.property_
                     if source_prop is None:
@@ -761,19 +750,27 @@
                     reverse_prop = next(
                         (prop for prop in view_properties_by_id.get(source, []) if prop.property_ == source_prop), None
                     )
                     if reverse_prop and reverse_prop.relation == "direct" and reverse_prop.is_list:
                         warnings.warn(
                             issues.dms.ReverseOfDirectRelationListWarning(view_id, prop.property_), stacklevel=2
                         )
-                        view_property = dm.MultiEdgeConnectionApply(
-                            type=dm.DirectRelationReference(
+                        if isinstance(reverse_prop.reference, ReferenceEntity):
+                            ref_view_prop = reverse_prop.reference.as_prop_id(default_space, default_version)
+                            edge_type = dm.DirectRelationReference(
+                                space=ref_view_prop.source.space,
+                                external_id=f"{ref_view_prop.source.external_id}.{ref_view_prop.property}",
+                            )
+                        else:
+                            edge_type = dm.DirectRelationReference(
                                 space=source.space,
                                 external_id=f"{reverse_prop.view.external_id}.{reverse_prop.view_property}",
-                            ),
+                            )
+                        view_property = dm.MultiEdgeConnectionApply(
+                            type=edge_type,
                             source=source,
                             direction="inwards",
                         )
                     else:
                         args: dict[str, Any] = dict(
                             source=source,
                             through=dm.PropertyId(source, source_prop),
@@ -793,24 +790,32 @@
                 elif prop.view and prop.view_property and prop.relation:
                     warnings.warn(
                         issues.dms.UnsupportedRelationWarning(view_id, prop.view_property, prop.relation), stacklevel=2
                     )
                     continue
                 else:
                     continue
-                prop_name = to_camel(prop.view_property) if self.standardize_casing else prop.view_property
+                prop_name = prop.view_property
                 view.properties[prop_name] = view_property
 
         node_types = dm.NodeApplyList([])
         parent_views = {parent for view in views for parent in view.implements or []}
         for view in views:
             ref_containers = sorted(view.referenced_containers(), key=lambda c: c.as_tuple())
-            has_data = dm.filters.HasData(containers=list(ref_containers)) if ref_containers else None
-            node_type = dm.filters.Equals(["node", "type"], {"space": view.space, "externalId": view.external_id})
             dms_view = dms_view_by_id.get(view.as_id())
+            has_data = dm.filters.HasData(containers=list(ref_containers)) if ref_containers else None
+            if dms_view and isinstance(dms_view.reference, ReferenceEntity):
+                # If the view is a reference, we implement the reference view,
+                # and need the filter to match the reference
+                ref_view = dms_view.reference.as_id(False, default_space, default_version)
+                node_type = dm.filters.Equals(
+                    ["node", "type"], {"space": ref_view.space, "externalId": ref_view.external_id}
+                )
+            else:
+                node_type = dm.filters.Equals(["node", "type"], {"space": view.space, "externalId": view.external_id})
             if view.as_id() in parent_views:
                 if dms_view and dms_view.filter_ == "nodeType":
                     warnings.warn(issues.dms.NodeTypeFilterOnParentViewWarning(view.as_id()), stacklevel=2)
                     view.filter = node_type
                     node_types.append(dm.NodeApply(space=view.space, external_id=view.external_id, sources=[]))
                 else:
                     view.filter = has_data
@@ -834,18 +839,15 @@
     def _create_containers(
         self,
         dms_container: SheetList[DMSContainer] | None,
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]],
         default_space: str,
     ) -> dm.ContainerApplyList:
         containers = dm.ContainerApplyList(
-            [
-                dms_container.as_container(default_space, self.standardize_casing)
-                for dms_container in dms_container or []
-            ]
+            [dms_container.as_container(default_space) for dms_container in dms_container or []]
         )
         container_to_drop = set()
         for container in containers:
             container_id = container.as_id()
             if not (container_properties := container_properties_by_id.get(container_id)):
                 warnings.warn(issues.dms.EmptyContainerWarning(container_id=container_id), stacklevel=2)
                 container_to_drop.add(container_id)
@@ -854,15 +856,15 @@
                 if prop.container_property is None:
                     continue
                 if isinstance(prop.value_type, DMSValueType):
                     type_cls = prop.value_type.dms
                 else:
                     type_cls = dm.DirectRelation
 
-                prop_name = to_camel(prop.container_property) if self.standardize_casing else prop.container_property
+                prop_name = prop.container_property
 
                 if type_cls is dm.DirectRelation:
                     container.properties[prop_name] = dm.ContainerProperty(
                         type=dm.DirectRelation(),
                         nullable=prop.nullable if prop.nullable is not None else True,
                         default_value=prop.default,
                         name=prop.name,
@@ -915,29 +917,29 @@
 
     def _gather_properties(
         self, rules: DMSRules, default_space: str, default_version: str
     ) -> tuple[dict[dm.ContainerId, list[DMSProperty]], dict[dm.ViewId, list[DMSProperty]]]:
         container_properties_by_id: dict[dm.ContainerId, list[DMSProperty]] = defaultdict(list)
         view_properties_by_id: dict[dm.ViewId, list[DMSProperty]] = defaultdict(list)
         for prop in rules.properties:
-            view_id = prop.view.as_id(False, default_space, default_version, self.standardize_casing)
+            view_id = prop.view.as_id(False, default_space, default_version)
             view_properties_by_id[view_id].append(prop)
 
             if prop.container and prop.container_property:
                 if prop.relation == "direct" and prop.is_list:
                     warnings.warn(
                         issues.dms.DirectRelationListWarning(
-                            container_id=prop.container.as_id(default_space, self.standardize_casing),
-                            view_id=prop.view.as_id(False, default_space, default_version, self.standardize_casing),
+                            container_id=prop.container.as_id(default_space),
+                            view_id=prop.view.as_id(False, default_space, default_version),
                             property=prop.container_property,
                         ),
                         stacklevel=2,
                     )
                     continue
-                container_id = prop.container.as_id(default_space, self.standardize_casing)
+                container_id = prop.container.as_id(default_space)
                 container_properties_by_id[container_id].append(prop)
 
         return container_properties_by_id, view_properties_by_id
 
 
 class _DMSRulesConverter:
     def __init__(self, dms: DMSRules):
```

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/dms_schema.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/dms_schema.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/domain_rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/domain_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/_rules/information_rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/raw_rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/rules.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/rules/models/value_types.py` & `cognite_neat-0.72.3/cognite/neat/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/cdf.py` & `cognite_neat-0.72.3/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/exceptions.py` & `cognite_neat-0.72.3/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.72.3/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/text.py` & `cognite_neat-0.72.3/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/utils.py` & `cognite_neat-0.72.3/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/utils/xml.py` & `cognite_neat-0.72.3/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.72.3/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/base.py` & `cognite_neat-0.72.3/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.72.3/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Export DMS/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Export DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Import DMS/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Import DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Validate Rules/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Validate Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml` & `cognite_neat-0.72.3/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/manager.py` & `cognite_neat-0.72.3/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.72.3/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.72.3/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/model.py` & `cognite_neat-0.72.3/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
 
         dms_exporter = exporters.DMSExporter(
             export_components=frozenset(components_to_create),
             include_space=None
             if multi_space_components_create
             else {input_rules.metadata.space if isinstance(input_rules, DMSRules) else input_rules.metadata.prefix},
             existing_handling=existing_components_handling,
-            standardize_casing=False,
         )
 
         output_dir = self.data_store_path / Path("staging")
         output_dir.mkdir(parents=True, exist_ok=True)
         file_name = (
             input_rules.metadata.external_id
             if isinstance(input_rules, DMSRules)
```

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.72.3/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/tasks.py` & `cognite_neat-0.72.3/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/cognite/neat/workflows/triggers.py` & `cognite_neat-0.72.3/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.2/pyproject.toml` & `cognite_neat-0.72.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.72.2"
+version = "0.72.3"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.72.2/PKG-INFO` & `cognite_neat-0.72.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.72.2
+Version: 0.72.3
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

