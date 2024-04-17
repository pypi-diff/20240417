# Comparing `tmp/cognite_neat-0.72.3.tar.gz` & `tmp/cognite_neat-0.73.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.72.3.tar", max compression
+gzip compressed data, was "cognite_neat-0.73.0.tar", max compression
```

## Comparing `cognite_neat-0.72.3.tar` & `cognite_neat-0.73.0.tar`

### file list

```diff
@@ -1,233 +1,232 @@
--rw-r--r--   0        0        0    11351 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/README.md
--rw-r--r--   0        0        0       61 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3583 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13653 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     6369 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12402 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      629 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-04-17 07:13:57.580078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1403545 2024-04-17 07:13:57.588078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js
--rw-r--r--   0        0        0     2667 2024-04-17 07:13:57.588078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt
--rw-r--r--   0        0        0  6234629 2024-04-17 07:13:57.612078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map
--rw-r--r--   0        0        0   240334 2024-04-17 07:13:57.612078 cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-17 07:13:57.620077 cognite_neat-0.72.3/cognite/neat/config.py
--rw-r--r--   0        0        0     1205 2024-04-17 07:13:57.620077 cognite_neat-0.72.3/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-17 07:13:57.620077 cognite_neat-0.72.3/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-17 07:13:57.620077 cognite_neat-0.72.3/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-17 07:13:57.624078 cognite_neat-0.72.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/__init__.py
--rw-r--r--   0        0        0      356 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/_base.py
--rw-r--r--   0        0        0    11232 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/_dexpi.py
--rw-r--r--   0        0        0    17408 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14872 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractor/_mock_graph_generator.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14969 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      693 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/__init__.py
--rw-r--r--   0        0        0    23838 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/_asset_loader.py
--rw-r--r--   0        0        0     2370 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/_base.py
--rw-r--r--   0        0        0     2837 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/labels.py
--rw-r--r--   0        0        0     5016 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/models.py
--rw-r--r--   0        0        0    40458 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22678 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12957 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/loader/validator.py
--rw-r--r--   0        0        0      149 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    14254 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-17 07:13:57.628078 cognite_neat-0.72.3/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/query_generator/__init__.py
--rw-r--r--   0        0        0    18659 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/query_generator/sparql.py
--rw-r--r--   0        0        0    14673 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/graph/transformation/transformer.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/_analysis/__init__.py
--rw-r--r--   0        0        0      674 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/_analysis/_base.py
--rw-r--r--   0        0        0    19613 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/_analysis/_information_rules.py
--rw-r--r--   0        0        0      177 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0     8596 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0     2538 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5501 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0     1439 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_base.py
--rw-r--r--   0        0        0      102 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_core/__init__.py
--rw-r--r--   0        0        0      764 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_core/rules2labels.py
--rw-r--r--   0        0        0    37099 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2dms.py
--rw-r--r--   0        0        0     8220 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2excel.py
--rw-r--r--   0        0        0     6215 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2graphql.py
--rw-r--r--   0        0        0    18414 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2ontology.py
--rw-r--r--   0        0        0    28745 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3866 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2rules.py
--rw-r--r--   0        0        0     1104 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2triples.py
--rw-r--r--   0        0        0     5769 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporter/_validation.py
--rw-r--r--   0        0        0      413 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    11854 2024-04-17 07:13:57.632078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     9080 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19922 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4092 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_base.py
--rw-r--r--   0        0        0     6469 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_dict2rules.py
--rw-r--r--   0        0        0     7890 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_dms2rules.py
--rw-r--r--   0        0        0    12097 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9320 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10521 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1529 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_spreadsheet2rules.py
--rw-r--r--   0        0        0      448 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_xsd2rules.py
--rw-r--r--   0        0        0     1628 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importer/_yaml2rules.py
--rw-r--r--   0        0        0      408 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4268 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0     9138 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12554 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6925 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11926 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7791 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7443 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     7120 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11481 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4198 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     5856 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    12722 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      127 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0      517 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/__init__.py
--rw-r--r--   0        0        0     1299 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/__init__.py
--rw-r--r--   0        0        0    16681 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_field.py
--rw-r--r--   0        0        0     6308 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_value.py
--rw-r--r--   0        0        0    10635 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/base.py
--rw-r--r--   0        0        0    50424 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/dms_architect_rules.py
--rw-r--r--   0        0        0    30229 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/dms_schema.py
--rw-r--r--   0        0        0     2051 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/domain_rules.py
--rw-r--r--   0        0        0    21026 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/_rules/information_rules.py
--rw-r--r--   0        0        0    12368 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7344 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51063 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/tables.py
--rw-r--r--   0        0        0     4395 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/rules/models/value_types.py
--rw-r--r--   0        0        0       68 2024-04-17 07:13:57.636078 cognite_neat-0.72.3/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2699 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26857 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Export DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Import DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
--rw-r--r--   0        0        0    13659 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6568 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6288 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18234 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0     7327 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4785 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29390 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27269 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12522 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2345 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20657 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28072 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-17 07:13:57.640077 cognite_neat-0.72.3/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4543 2024-04-17 07:13:58.032077 cognite_neat-0.72.3/pyproject.toml
--rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.72.3/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/README.md
+-rw-r--r--   0        0        0       61 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3583 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13653 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     6369 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12402 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      629 2024-04-17 13:30:03.759485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-04-17 13:30:03.763485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-17 13:30:03.763485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-17 13:30:03.763485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-17 13:30:03.763485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-04-17 13:30:03.763485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1403545 2024-04-17 13:30:03.767485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js
+-rw-r--r--   0        0        0     2667 2024-04-17 13:30:03.767485 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt
+-rw-r--r--   0        0        0  6234629 2024-04-17 13:30:03.795484 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map
+-rw-r--r--   0        0        0   240334 2024-04-17 13:30:03.795484 cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-04-17 13:30:03.803484 cognite_neat-0.73.0/cognite/neat/config.py
+-rw-r--r--   0        0        0     1205 2024-04-17 13:30:03.803484 cognite_neat-0.73.0/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-17 13:30:03.803484 cognite_neat-0.73.0/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-17 13:30:03.803484 cognite_neat-0.73.0/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-17 13:30:03.807484 cognite_neat-0.73.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/extractor/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/extractor/_base.py
+-rw-r--r--   0        0        0    11232 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/extractor/_dexpi.py
+-rw-r--r--   0        0        0    17652 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/extractor/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14872 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/extractor/_mock_graph_generator.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14969 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      693 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/__init__.py
+-rw-r--r--   0        0        0    23838 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/_asset_loader.py
+-rw-r--r--   0        0        0     2370 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/core/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/core/labels.py
+-rw-r--r--   0        0        0     5016 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/core/models.py
+-rw-r--r--   0        0        0    40458 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22678 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12957 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/loader/validator.py
+-rw-r--r--   0        0        0      149 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14254 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/transformation/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/transformation/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/transformation/query_generator/__init__.py
+-rw-r--r--   0        0        0    18659 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/transformation/query_generator/sparql.py
+-rw-r--r--   0        0        0    14673 2024-04-17 13:30:03.811484 cognite_neat-0.73.0/cognite/neat/graph/transformation/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/_analysis/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/_analysis/_base.py
+-rw-r--r--   0        0        0    19613 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/_analysis/_information_rules.py
+-rw-r--r--   0        0        0      177 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0     8596 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0     1439 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_base.py
+-rw-r--r--   0        0        0      102 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_core/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_core/rules2labels.py
+-rw-r--r--   0        0        0    36770 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2dms.py
+-rw-r--r--   0        0        0     8305 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2excel.py
+-rw-r--r--   0        0        0     6215 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2graphql.py
+-rw-r--r--   0        0        0    18414 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2ontology.py
+-rw-r--r--   0        0        0    28745 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3866 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2rules.py
+-rw-r--r--   0        0        0     1104 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2triples.py
+-rw-r--r--   0        0        0     5769 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporter/_validation.py
+-rw-r--r--   0        0        0      413 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    11854 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    13146 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19922 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4092 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0     2316 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/importer/_base.py
+-rw-r--r--   0        0        0     6469 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/importer/_dict2rules.py
+-rw-r--r--   0        0        0     7713 2024-04-17 13:30:03.815484 cognite_neat-0.73.0/cognite/neat/rules/importer/_dms2rules.py
+-rw-r--r--   0        0        0    12097 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9320 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10521 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1529 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      448 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_xsd2rules.py
+-rw-r--r--   0        0        0     1628 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importer/_yaml2rules.py
+-rw-r--r--   0        0        0      408 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4268 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    10427 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12554 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6925 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11926 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7791 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     7120 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11481 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4198 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6158 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    15314 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      127 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0      517 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/__init__.py
+-rw-r--r--   0        0        0     1299 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/_types/__init__.py
+-rw-r--r--   0        0        0    16681 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/_types/_base.py
+-rw-r--r--   0        0        0    10295 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/_types/_field.py
+-rw-r--r--   0        0        0     6308 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/_types/_value.py
+-rw-r--r--   0        0        0    11025 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/base.py
+-rw-r--r--   0        0        0    55886 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/dms_architect_rules.py
+-rw-r--r--   0        0        0    30418 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/dms_schema.py
+-rw-r--r--   0        0        0     2566 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/domain_rules.py
+-rw-r--r--   0        0        0    21555 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/_rules/information_rules.py
+-rw-r--r--   0        0        0    12368 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7344 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51063 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/tables.py
+-rw-r--r--   0        0        0     4395 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/rules/models/value_types.py
+-rw-r--r--   0        0        0       68 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11063 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2722 2024-04-17 13:30:03.819484 cognite_neat-0.73.0/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26857 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Export DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Import DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
+-rw-r--r--   0        0        0    13659 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6568 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6288 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18234 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0     7327 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4785 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29390 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27269 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12522 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2345 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20657 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28072 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-17 13:30:03.823484 cognite_neat-0.73.0/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4543 2024-04-17 13:30:04.211479 cognite_neat-0.73.0/pyproject.toml
+-rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.73.0/PKG-INFO
```

### Comparing `cognite_neat-0.72.3/LICENSE` & `cognite_neat-0.73.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/README.md` & `cognite_neat-0.73.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/configuration.py` & `cognite_neat-0.73.0/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.73.0/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.73.0/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/explorer.py` & `cognite_neat-0.73.0/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.73.0/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.73.0/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.73.0/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.73.0/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.73.0/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.73.0/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.73.0/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.73.0/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.73.0/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.73.0/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/js/main.2efd96b2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.73.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/config.py` & `cognite_neat-0.73.0/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/constants.py` & `cognite_neat-0.73.0/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/exceptions.py` & `cognite_neat-0.73.0/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.73.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.73.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.73.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/exceptions.py` & `cognite_neat-0.73.0/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/extractor/_dexpi.py` & `cognite_neat-0.73.0/cognite/neat/graph/extractor/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/extractor/_graph_capturing_sheet.py` & `cognite_neat-0.73.0/cognite/neat/graph/extractor/_graph_capturing_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 import pandas as pd
 from openpyxl import Workbook, load_workbook
 from openpyxl.cell import Cell
 from openpyxl.styles import Alignment, Border, Font, NamedStyle, PatternFill, Side
 from openpyxl.utils import get_column_letter
 from openpyxl.worksheet.datavalidation import DataValidation
+from openpyxl.worksheet.worksheet import Worksheet
 from rdflib import RDF, XSD, Literal, Namespace, URIRef
 
 from cognite.neat.graph import exceptions
 from cognite.neat.graph.exceptions import NamespaceRequired
 from cognite.neat.graph.models import Triple
 from cognite.neat.rules.analysis import get_defined_classes, to_class_property_pairs
 from cognite.neat.rules.exporter._rules2rules import to_dms_name
@@ -317,15 +318,15 @@
     # Remove default sheet named "Sheet"
     workbook.remove(workbook["Sheet"])
 
     for class_, properties in to_class_property_pairs(rules).items():
         workbook.create_sheet(title=class_)
 
         # Add header rows
-        workbook[class_].append(["identifier", *list(properties.keys())])
+        cast(Worksheet, workbook[class_]).append(["identifier", *list(properties.keys())])
 
         if auto_identifier_type and auto_identifier_type == "index-based":  # default, easy to read
             logging.debug(f"Configuring index-based automatic identifiers for sheet {class_}")
             _add_index_identifiers(workbook, class_, no_rows)
         elif auto_identifier_type and auto_identifier_type == "uuid-based":
             logging.debug(f"Configuring UUID-based automatic identifiers for sheet {class_}")
             _add_uuid_identifiers(workbook, class_, no_rows)
@@ -346,56 +347,57 @@
     workbook.close()
 
 
 def _add_index_identifiers(workbook: Workbook, sheet: str, no_rows: int):
     """Adds index-based auto identifier to a sheet identifier column"""
     for i in range(no_rows):
         prefix = to_dms_name(sheet, "class", True)
-        workbook[sheet][f"A{i+2}"] = f'=IF(ISBLANK(B{i+2}), "","{prefix}-{i+1}")'
+        workbook[sheet][f"A{i+2}"] = f'=IF(ISBLANK(B{i+2}), "","{prefix}-{i+1}")'  # type: ignore[index]
 
 
 def _add_uuid_identifiers(workbook: Workbook, sheet: str, no_rows: int):
     """Adds UUID-based auto identifier to a sheet identifier column"""
     for i in range(no_rows):
         prefix = to_dms_name(sheet, "class", True)
-        workbook[sheet][f"A{i+2}"] = f'=IF(ISBLANK(B{i+2}), "","{prefix}-{uuid.uuid4()}")'
+        workbook[sheet][f"A{i+2}"] = f'=IF(ISBLANK(B{i+2}), "","{prefix}-{uuid.uuid4()}")'  # type: ignore[index]
 
 
 def _add_drop_down_list(workbook: Workbook, sheet: str, column: str, no_rows: int, value_sheet: str, value_column: str):
     """Adds a drop down list to a column"""
     drop_down_list = DataValidation(type="list", formula1=f"={value_sheet}!{value_column}$2:{value_column}${no_rows}")
 
-    workbook[sheet].add_data_validation(drop_down_list)
+    cast(Worksheet, workbook[sheet]).add_data_validation(drop_down_list)
 
     for i in range(no_rows):
-        drop_down_list.add(workbook[sheet][f"{column}{i+2}"])
+        drop_down_list.add(workbook[sheet][f"{column}{i+2}"])  # type: ignore[index, misc]
 
 
 def _adjust_column_width(workbook: Workbook):
     """Adjusts the column width based on the content"""
     for sheet in workbook.sheetnames:
-        for cell_tuple in workbook[sheet].columns:
+        for cell_tuple in cast(Worksheet, workbook[sheet]).columns:
             # Wrong type annotation in openpyxl
             cell = cast(Cell, cell_tuple[0])  # type: ignore[index]
             if cell.value:
                 adjusted_width = (len(str(cell.value)) + 5) * 1.2
-                workbook[sheet].column_dimensions[cell.column_letter].width = adjusted_width
+                cast(Worksheet, workbook[sheet]).column_dimensions[cell.column_letter].width = adjusted_width
 
 
 def _set_header_style(workbook: Workbook):
     """Sets the header style for all sheets in the workbook"""
     style = NamedStyle(name="header style")
     style.font = Font(bold=True, size=16)
     side = Side(style="thin", color="000000")
     style.border = Border(left=side, right=side, top=side, bottom=side)
     workbook.add_named_style(style)
 
     for sheet in workbook.sheetnames:
-        for cell_tuple in workbook[sheet].columns:
+        for cell_tuple in cast(Worksheet, workbook[sheet]).columns:
             # Wrong type annotation in openpyxl
             cell = cast(Cell, cell_tuple[0])  # type: ignore[index]
-            workbook[sheet][f"{cell.column_letter}1"].style = style
+            worksheet = cast(Worksheet, workbook[sheet])
+            worksheet[f"{cell.column_letter}1"].style = style
             if f"{cell.column_letter}1" == "A1":
-                workbook[sheet][f"{cell.column_letter}1"].fill = PatternFill("solid", start_color="2FB5F2")
+                worksheet[f"{cell.column_letter}1"].fill = PatternFill("solid", start_color="2FB5F2")
             else:
-                workbook[sheet][f"{cell.column_letter}1"].fill = PatternFill("solid", start_color="FFB202")
-            workbook[sheet][f"{cell.column_letter}1"].alignment = Alignment(horizontal="center", vertical="center")
+                worksheet[f"{cell.column_letter}1"].fill = PatternFill("solid", start_color="FFB202")
+            worksheet[f"{cell.column_letter}1"].alignment = Alignment(horizontal="center", vertical="center")
```

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/extractor/_mock_graph_generator.py` & `cognite_neat-0.73.0/cognite/neat/graph/extractor/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.73.0/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/__init__.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/_asset_loader.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/_base.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/_exceptions.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/core/labels.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/core/models.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/core/rdf_to_assets.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/core/rdf_to_relationships.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/rdf_to_dms.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/loader/validator.py` & `cognite_neat-0.73.0/cognite/neat/graph/loader/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.73.0/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.73.0/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.73.0/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.73.0/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.73.0/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.73.0/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.73.0/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/transformation/entity_matcher.py` & `cognite_neat-0.73.0/cognite/neat/graph/transformation/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/transformation/query_generator/sparql.py` & `cognite_neat-0.73.0/cognite/neat/graph/transformation/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/graph/transformation/transformer.py` & `cognite_neat-0.73.0/cognite/neat/graph/transformation/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/_analysis/_base.py` & `cognite_neat-0.73.0/cognite/neat/rules/_analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/_analysis/_information_rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/_analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/analysis.py` & `cognite_neat-0.73.0/cognite/neat/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.73.0/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.73.0/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/__init__.py` & `cognite_neat-0.73.0/cognite/neat/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.73.0/cognite/neat/rules/examples/power-grid-containers.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
         @name substation'
       name: substation
       nullable: true
       type:
         container: null
         type: direct
+        list: false
   space: workshop
   usedFor: node
 - externalId: SubGeographicalRegion
   name: SubGeographicalRegion
   properties:
     name:
       autoIncrement: false
@@ -77,14 +78,15 @@
 
         @name region'
       name: region
       nullable: true
       type:
         container: null
         type: direct
+        list: false
   space: workshop
   usedFor: node
 - externalId: Substation
   name: Substation
   properties:
     name:
       autoIncrement: false
@@ -105,9 +107,10 @@
 
         @name subGeographicalRegion'
       name: subGeographicalRegion
       nullable: true
       type:
         container: null
         type: direct
+        list: false
   space: workshop
   usedFor: node
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.73.0/cognite/neat/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/power-grid-model.yaml` & `cognite_neat-0.73.0/cognite/neat/rules/examples/power-grid-model.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         container:
           space: workshop
           externalId: SubGeographicalRegion
         containerPropertyIdentifier: region
         type:
           container: null
           type: direct
+          list: false
           source:
             space: workshop
             externalId: GeographicalRegion
             version: "1"
         nullable: true
         autoIncrement: false
         defaultValue: null
@@ -128,14 +129,15 @@
         container:
           space: workshop
           externalId: Substation
         containerPropertyIdentifier: subGeographicalRegion
         type:
           container: null
           type: direct
+          list: false
           source:
             space: workshop
             externalId: SubGeographicalRegion
             version: bbe4295878a47f
         nullable: true
         autoIncrement: false
         defaultValue: null
@@ -191,14 +193,15 @@
         container:
           space: workshop
           externalId: Terminal
         containerPropertyIdentifier: substation
         type:
           container: null
           type: direct
+          list: false
           source:
             space: workshop
             externalId: Substation
             version: "1"
         nullable: true
         autoIncrement: false
         defaultValue: null
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/rules-template.xlsx` & `cognite_neat-0.73.0/cognite/neat/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.73.0/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/skos-rules.xlsx` & `cognite_neat-0.73.0/cognite/neat/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.73.0/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.73.0/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exceptions.py` & `cognite_neat-0.73.0/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/__init__.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_base.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_core/rules2labels.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2dms.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     DirectRelationReference,
     MappedPropertyApply,
     PropertyType,
     SpaceApply,
     ViewApply,
     ViewId,
 )
-from cognite.client.data_classes.data_modeling.data_types import ListablePropertyType
 from cognite.client.data_classes.data_modeling.views import (
     ConnectionDefinitionApply,
     SingleHopConnectionDefinitionApply,
 )
 from cognite.client.exceptions import CogniteAPIError
 from pydantic import BaseModel, ConfigDict, field_validator
 
@@ -280,36 +279,30 @@
                             existing_property, default_value=None
                         )
 
                     # scenario: property hold multiple values -> set is_list to True
                     if (
                         not isinstance(existing_property.type, DirectRelation)
                         and not isinstance(api_container_property.type, DirectRelation)
-                        and cast(ListablePropertyType, existing_property.type).is_list
-                        != cast(ListablePropertyType, api_container_property.type).is_list
+                        and existing_property.type.is_list != api_container_property.type.is_list
                     ):
-                        cast(
-                            ListablePropertyType, containers[container_id].properties[container_property_id].type
-                        ).is_list = True
+                        containers[container_id].properties[container_property_id].type.is_list = True
 
         if errors:
             raise ExceptionGroup("Properties value types have been redefined! This is prohibited! Aborting!", errors)
 
         return containers
 
     @classmethod
     def as_api_container_property(cls, property_: Property) -> ContainerProperty:
         is_one_to_many = property_.max_count != 1
 
         # Literal, i.e. Node attribute
         if property_.property_type is EntityTypes.data_property:
-            property_type = cast(
-                type[ListablePropertyType],
-                cast(ValueTypeMapping, property_.expected_value_type.mapping).dms,
-            )
+            property_type = cast(ValueTypeMapping, property_.expected_value_type.mapping).dms
             return ContainerProperty(
                 type=property_type(is_list=is_one_to_many),
                 nullable=property_.min_count == 0,
                 default_value=property_.default,
                 name=property_.property_name,
                 description=property_.description,
             )
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2excel.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from typing import cast
 
 from openpyxl import Workbook
 from openpyxl.cell import Cell
 from openpyxl.styles import Alignment, Border, Font, NamedStyle, PatternFill, Side
+from openpyxl.worksheet.worksheet import Worksheet
 
 from cognite.neat.rules.models._base import EntityTypes
 
 from ._base import BaseExporter
 
 
 class ExcelExporter(BaseExporter[Workbook]):
@@ -186,15 +187,15 @@
         style.border = Border(left=side, right=side, top=side, bottom=side)
         data.add_named_style(style)
 
         for sheet in data.sheetnames:
             if sheet == "Metadata":
                 continue
             if sheet == "Classes" or sheet == "Properties":
-                sheet_obj = data[sheet]
+                sheet_obj = cast(Worksheet, data[sheet])
                 if sheet == "Classes":
                     sheet_obj.freeze_panes = "A3"
                 else:
                     sheet_obj.freeze_panes = "D3"
 
                 for cell in sheet_obj[1]:
                     cell = cast(Cell, cell)  # type: ignore[index]
@@ -203,10 +204,10 @@
                     cell.alignment = Alignment(horizontal="center", vertical="center")
                 for cell in sheet_obj[2]:
                     cell = cast(Cell, cell)  # type: ignore[index]
                     cell.style = style
                     cell.fill = PatternFill("solid", start_color="D5DBD5")
                     cell.alignment = Alignment(horizontal="center", vertical="center")
                     adjusted_width = (len(str(cell.value)) + 5) * 1.2
-                    data[sheet].column_dimensions[cell.column_letter].width = adjusted_width
+                    cast(Worksheet, data[sheet]).column_dimensions[cell.column_letter].width = adjusted_width
 
         return data
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2graphql.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2ontology.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2pydantic_models.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_rules2triples.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporter/_validation.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporter/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from __future__ import annotations
 
 import itertools
+from datetime import datetime
 from pathlib import Path
 from types import GenericAlias
-from typing import Any, ClassVar, Literal, get_args
+from typing import Any, ClassVar, Literal, cast, get_args
 
 from openpyxl import Workbook
 from openpyxl.cell import MergedCell
 from openpyxl.styles import Alignment, Border, Font, PatternFill, Side
+from openpyxl.worksheet.worksheet import Worksheet
 
 from cognite.neat.rules._shared import Rules
-from cognite.neat.rules.models._rules.base import RoleTypes, SheetEntity
+from cognite.neat.rules.models._rules import DMSRules, DomainRules, InformationRules
+from cognite.neat.rules.models._rules.base import RoleTypes, SchemaCompleteness, SheetEntity
 
 from ._base import BaseExporter
 
 
 class ExcelExporter(BaseExporter[Workbook]):
     """Export rules to Excel.
 
     Args:
         styling: The styling to use for the Excel file. Defaults to "default". See below for details
             on the different styles.
         output_role: The role to use for the exported spreadsheet. If provided, the rules will be converted to
             this role formate before being written to excel. If not provided, the role from the rules will be used.
+        new_model_id: The new model ID to use for the exported spreadsheet. This is only applicable if the input
+            rules have 'is_reference' set. If provided, the model ID will be used to automatically create the
+            new metadata sheet in the Excel file.
 
     The following styles are available:
 
     - "none":    No styling is applied.
     - "minimal": Column widths are adjusted to fit the content, and the header row(s) is frozen.
     - "default": Minimal + headers are bold, increased size, and colored.
     - "maximal": Default + alternating row colors in the properties sheet for each class in addition to extra
@@ -39,20 +45,26 @@
         "Properties": "Definition of Properties per Class",
         "Classes": "Definition of Classes",
         "Views": "Definition of Views",
         "Containers": "Definition of Containers",
     }
     style_options = get_args(Style)
 
-    def __init__(self, styling: Style = "default", output_role: RoleTypes | None = None):
+    def __init__(
+        self,
+        styling: Style = "default",
+        output_role: RoleTypes | None = None,
+        new_model_id: tuple[str, str, str] | None = None,
+    ):
         if styling not in self.style_options:
             raise ValueError(f"Invalid styling: {styling}. Valid options are {self.style_options}")
         self.styling = styling
         self._styling_level = self.style_options.index(styling)
         self.output_role = output_role
+        self.new_model_id = new_model_id
 
     def export_to_file(self, rules: Rules, filepath: Path) -> None:
         """Exports transformation rules to excel file."""
         data = self.export(rules)
         try:
             data.save(filepath)
         finally:
@@ -66,15 +78,15 @@
         workbook.remove(workbook["Sheet"])
 
         dumped_rules: dict[str, Any]
         dumped_reference_rules: dict[str, Any] | None = None
         if rules.is_reference:
             # Writes empty reference sheets
             dumped_rules = {
-                "Metadata": {field_alias: None for field_alias in rules.metadata.model_dump(by_alias=True).keys()},
+                "Metadata": self._create_metadata_sheet_user_rules(rules),
             }
             dumped_rules["Metadata"]["role"] = (
                 self.output_role and self.output_role.value
             ) or rules.metadata.role.value
             dumped_reference_rules = rules.reference_self().model_dump(by_alias=True)
         else:
             dumped_rules = rules.model_dump(by_alias=True)
@@ -151,14 +163,20 @@
                 # Make the header row bold, larger, and colored
                 sheet["A1"].font = Font(bold=True, size=20)
                 sheet["A1"].fill = PatternFill(fgColor="FFC000", patternType="solid")
                 for cell in sheet["2"]:
                     cell.font = Font(bold=True, size=14)
 
     def _write_metadata_sheet(self, workbook: Workbook, metadata: dict[str, Any], is_reference: bool = False) -> None:
+        # Excel does not support timezone in datetime strings
+        if isinstance(metadata.get("created"), datetime):
+            metadata["created"] = metadata["created"].replace(tzinfo=None)
+        if isinstance(metadata.get("updated"), datetime):
+            metadata["updated"] = metadata["updated"].replace(tzinfo=None)
+
         if is_reference:
             metadata_sheet = workbook.create_sheet("RefMetadata")
         else:
             metadata_sheet = workbook.create_sheet("Metadata")
         for key, value in metadata.items():
             metadata_sheet.append([key, value])
 
@@ -177,20 +195,92 @@
         if not issubclass(arg, SheetEntity):
             raise ValueError(f"Expected annotation to have a BaseModel argument, but got {type(arg)}")
         return arg
 
     @classmethod
     def _adjust_column_widths(cls, workbook: Workbook) -> None:
         for sheet in workbook:
+            sheet = cast(Worksheet, sheet)
             for column_cells in sheet.columns:
                 try:
                     max_length = max(len(str(cell.value)) for cell in column_cells if cell.value is not None)
                 except ValueError:
                     max_length = 0
 
                 selected_column = column_cells[0]
                 if isinstance(selected_column, MergedCell):
                     selected_column = column_cells[1]
 
                 current = sheet.column_dimensions[selected_column.column_letter].width or (max_length + 0.5)
                 sheet.column_dimensions[selected_column.column_letter].width = max(current, max_length + 0.5)
         return None
+
+    def _create_metadata_sheet_user_rules(self, rules: Rules) -> dict[str, Any]:
+        metadata: dict[str, Any] = {
+            field_alias: None for field_alias in rules.metadata.model_dump(by_alias=True).keys()
+        }
+        if "creator" in metadata:
+            metadata["creator"] = "YOUR NAME"
+
+        if isinstance(rules, DomainRules):
+            return metadata
+        elif isinstance(rules, DMSRules):
+            existing_model_id = (rules.metadata.space, rules.metadata.external_id, rules.metadata.version)
+        elif isinstance(rules, InformationRules):
+            existing_model_id = (rules.metadata.prefix, rules.metadata.name, rules.metadata.version)
+        else:
+            raise ValueError(f"Unsupported rules type: {type(rules)}")
+        existing_metadata = rules.metadata.model_dump(by_alias=True)
+        if isinstance(existing_metadata["created"], datetime):
+            metadata["created"] = existing_metadata["created"].replace(tzinfo=None)
+        if isinstance(existing_metadata["updated"], datetime):
+            metadata["updated"] = existing_metadata["updated"].replace(tzinfo=None)
+        # Excel does not support timezone in datetime strings
+        now_iso = datetime.now().replace(tzinfo=None).isoformat()
+        is_info = isinstance(rules, InformationRules)
+        is_dms = not is_info
+        is_extension = self.new_model_id is not None
+        is_solution = is_extension and self.new_model_id != existing_model_id
+
+        if is_solution:
+            metadata["prefix" if is_info else "space"] = self.new_model_id[0]  # type: ignore[index]
+            metadata["title" if is_info else "externalId"] = self.new_model_id[1]  # type: ignore[index]
+            metadata["version"] = self.new_model_id[2]  # type: ignore[index]
+        else:
+            metadata["prefix" if is_info else "space"] = existing_model_id[0]
+            metadata["title" if is_info else "externalId"] = existing_model_id[1]
+            metadata["version"] = existing_model_id[2]
+
+        if is_solution and is_info:
+            metadata["namespace"] = f"http://purl.org/{self.new_model_id[0]}/"  # type: ignore[index]
+        elif is_info:
+            metadata["namespace"] = existing_metadata["namespace"]
+
+        if is_solution and is_dms:
+            metadata["name"] = self.new_model_id[1]  # type: ignore[index]
+
+        if is_solution:
+            metadata["created"] = now_iso
+        else:
+            metadata["created"] = existing_metadata["created"]
+
+        if is_solution or is_extension:
+            metadata["updated"] = now_iso
+        else:
+            metadata["updated"] = existing_metadata["updated"]
+
+        if is_solution:
+            metadata["creator"] = "YOUR NAME"
+        else:
+            metadata["creator"] = existing_metadata["creator"]
+
+        if not is_solution:
+            metadata["description"] = existing_metadata["description"]
+
+        if is_extension:
+            metadata["schema"] = SchemaCompleteness.extended.value
+        else:
+            metadata["schema"] = SchemaCompleteness.complete.value
+
+        metadata["extension"] = "addition"
+
+        return metadata
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.73.0/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/__init__.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_base.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_dict2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_dms2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_dms2rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     DataModel,
     DirectRelation,
     EdgeConnection,
     MappedProperty,
     SingleHopConnectionDefinition,
     View,
 )
-from cognite.client.data_classes.data_modeling.data_types import ListablePropertyType
 from cognite.client.data_classes.data_modeling.ids import DataModelIdentifier, ViewId
 
 from cognite.neat.rules.models.tables import Tables
 from cognite.neat.rules.models.value_types import DMS_VALUE_TYPE_MAPPINGS, XSD_VALUE_TYPE_MAPPINGS
 
 from ._base import BaseImporter
 
@@ -128,17 +127,15 @@
                     name = prop.name or prop_id
                     description = prop.description or float("nan")
                 else:
                     raise NotImplementedError(f"Property type {type(prop)} not supported")
 
                 max_count: str | float = "1"
                 if isinstance(prop, SingleHopConnectionDefinition) or (
-                    isinstance(prop, MappedProperty)
-                    and isinstance(prop.type, ListablePropertyType)
-                    and prop.type.is_list
+                    isinstance(prop, MappedProperty) and prop.type.is_list
                 ):
                     max_count = float("nan")
 
                 min_count: str | float = "1"
                 if isinstance(prop, SingleHopConnectionDefinition) or (
                     isinstance(prop, MappedProperty) and prop.nullable
                 ):
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_graph2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_json2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2classes.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2properties.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_owl2rules/_owl2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_spreadsheet2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importer/_yaml2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importer/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,79 @@
 from pathlib import Path
 from typing import Literal, cast, overload
 
 from cognite.client import CogniteClient
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes.data_modeling import DataModelIdentifier
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex, InvertedIndex
-from cognite.client.data_classes.data_modeling.data_types import ListablePropertyType
+from cognite.client.utils import ms_to_datetime
 
 from cognite.neat.rules import issues
+from cognite.neat.rules.importers._base import BaseImporter, Rules
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models._rules import DMSRules, DMSSchema, RoleTypes
 from cognite.neat.rules.models._rules._types import (
     ClassEntity,
     ContainerEntity,
     DMSValueType,
     Undefined,
     Unknown,
     ViewEntity,
     ViewPropEntity,
 )
+from cognite.neat.rules.models._rules.base import ExtensionCategory, SchemaCompleteness
 from cognite.neat.rules.models._rules.dms_architect_rules import (
     DMSContainer,
     DMSMetadata,
     DMSProperty,
     DMSView,
     SheetList,
 )
 
-from ._base import BaseImporter, Rules
-
 
 class DMSImporter(BaseImporter):
-    def __init__(self, schema: DMSSchema):
+    def __init__(self, schema: DMSSchema, metadata: DMSMetadata | None = None):
         self.schema = schema
+        self.metadata = metadata
 
     @classmethod
     def from_data_model_id(cls, client: CogniteClient, data_model_id: DataModelIdentifier) -> "DMSImporter":
-        return cls(DMSSchema.from_model_id(client, data_model_id))
+        """Create a DMSImporter ready to convert the given data model to rules.
+
+        Args:
+            client: Instantiated CogniteClient to retrieve data model.
+            data_model_id: Data Model to retrieve.
+
+        Returns:
+            DMSImporter: DMSImporter instance
+        """
+        data_models = client.data_modeling.data_models.retrieve(data_model_id, inline_views=True)
+        if len(data_models) == 0:
+            raise ValueError(f"Data model {data_model_id} not found")
+        data_model = data_models.latest_version()
+        schema = DMSSchema.from_data_model(client, data_model)
+        description, creator = DMSMetadata._get_description_and_creator(data_model.description)
+
+        created = ms_to_datetime(data_model.created_time)
+        updated = ms_to_datetime(data_model.last_updated_time)
+
+        metadata = DMSMetadata(
+            schema_=SchemaCompleteness.complete,
+            extension=ExtensionCategory.addition,
+            space=data_model.space,
+            external_id=data_model.external_id,
+            name=data_model.name or data_model.external_id,
+            version=data_model.version or "0.1.0",
+            updated=updated,
+            created=created,
+            creator=creator,
+            description=description,
+            default_view_version=data_model.version or "0.1.0",
+        )
+        return cls(schema, metadata)
 
     @classmethod
     def from_directory(cls, directory: str | Path) -> "DMSImporter":
         return cls(DMSSchema.from_directory(directory))
 
     @classmethod
     def from_zip_file(cls, zip_file: str | Path) -> "DMSImporter":
@@ -134,19 +167,15 @@
                     else:
                         dms_property = DMSProperty(
                             class_=ClassEntity(prefix=view.space, suffix=view.external_id, version=view.version),
                             property_=prop_id,
                             description=prop.description,
                             value_type=cast(ViewPropEntity | DMSValueType, container_prop.type._type),
                             nullable=container_prop.nullable,
-                            is_list=(
-                                container_prop.type.is_list
-                                if isinstance(container_prop.type, ListablePropertyType)
-                                else False
-                            ),
+                            is_list=container_prop.type.is_list,
                             default=container_prop.default_value,
                             container=ContainerEntity.from_id(container.as_id()),
                             container_property=prop.container_property_identifier,
                             view=ViewEntity.from_id(view.as_id()),
                             view_property=prop_id,
                             index=index or None,
                             constraint=unique_constraints or None,
@@ -168,15 +197,15 @@
                 properties.append(dms_property)
 
         data_model_view_ids: set[dm.ViewId] = {
             view.as_id() if isinstance(view, dm.View | dm.ViewApply) else view for view in data_model.views or []
         }
 
         dms_rules = DMSRules(
-            metadata=DMSMetadata.from_data_model(data_model),
+            metadata=self.metadata or DMSMetadata.from_data_model(data_model),
             properties=properties,
             containers=SheetList[DMSContainer](
                 data=[DMSContainer.from_container(container) for container in self.schema.containers]
             ),
             views=SheetList[DMSView](data=[DMSView.from_view(view, data_model_view_ids) for view in self.schema.views]),
             is_reference=is_reference,
         )
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.73.0/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/issues/base.py` & `cognite_neat-0.73.0/cognite/neat/rules/issues/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,23 @@
 
     @classmethod
     def from_pydantic_errors(cls, errors: list[ErrorDetails], **kwargs) -> "list[NeatValidationError]":
         """Convert a list of pydantic errors to a list of Error instances.
 
         This is intended to be overridden in subclasses to handle specific error types.
         """
-        return [DefaultPydanticError.from_pydantic_error(error) for error in errors]
+        all_errors = []
+        for error in errors:
+            if isinstance(ctx := error.get("ctx"), dict) and isinstance(
+                multi_error := ctx.get("error"), MultiValueError
+            ):
+                all_errors.extend(multi_error.errors)
+            else:
+                all_errors.append(DefaultPydanticError.from_pydantic_error(error))
+        return all_errors
 
 
 @dataclass(frozen=True)
 class DefaultPydanticError(NeatValidationError):
     type: str
     loc: tuple[int | str, ...]
     msg: str
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.73.0/cognite/neat/rules/issues/dms.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     "DirectRelationListWarning",
     "ReverseOfDirectRelationListWarning",
     "EmptyContainerWarning",
     "UnsupportedRelationWarning",
     "MultipleReferenceWarning",
     "HasDataFilterOnNoPropertiesViewWarning",
     "NodeTypeFilterOnParentViewWarning",
+    "ChangingContainerError",
+    "ChangingViewError",
 ]
 
 
 @dataclass(frozen=True)
 class DMSSchemaError(NeatValidationError, ABC):
     ...
 
@@ -222,14 +224,86 @@
         output["container"] = self.container
         output["property"] = self.property
         output["referred_by"] = sorted(self.referred_by)
         return output
 
 
 @dataclass(frozen=True)
+class ChangingContainerError(DMSSchemaError):
+    description = "You are adding to an existing model. "
+    fix = "Keep the container the same"
+    error_name: ClassVar[str] = "ChangingContainerError"
+    container_id: dm.ContainerId
+    changed_properties: list[str] | None = None
+    changed_attributes: list[str] | None = None
+
+    def __post_init__(self):
+        # Sorting for deterministic output
+        if self.changed_properties:
+            self.changed_properties.sort()
+        if self.changed_attributes:
+            self.changed_attributes.sort()
+
+    def message(self) -> str:
+        if self.changed_properties:
+            changed = f" properties {self.changed_properties}."
+        elif self.changed_attributes:
+            changed = f" attributes {self.changed_attributes}."
+        else:
+            changed = "."
+        return (
+            f"The container {self.container_id} has changed{changed}"
+            "When extending model with extension set to addition or reshape, the container "
+            "properties must remain the same"
+        )
+
+    def dump(self) -> dict[str, Any]:
+        output = super().dump()
+        output["container_id"] = self.container_id.dump()
+        output["changed_properties"] = self.changed_properties
+        return output
+
+
+@dataclass(frozen=True)
+class ChangingViewError(DMSSchemaError):
+    description = "You are adding to an existing model. "
+    fix = "Keep the view the same"
+    error_name: ClassVar[str] = "ChangingViewError"
+    view_id: dm.ViewId
+    changed_properties: list[str] | None = None
+    changed_attributes: list[str] | None = None
+
+    def __post_init__(self):
+        # Sorting for deterministic output
+        if self.changed_properties:
+            self.changed_properties.sort()
+        if self.changed_attributes:
+            self.changed_attributes.sort()
+
+    def message(self) -> str:
+        if self.changed_properties:
+            changed = f" properties {self.changed_properties}."
+        elif self.changed_attributes:
+            changed = f" attributes {self.changed_attributes}."
+        else:
+            changed = "."
+
+        return (
+            f"The view {self.view_id} has changed{changed}"
+            "When extending model with extension set to addition, the view properties must remain the same"
+        )
+
+    def dump(self) -> dict[str, Any]:
+        output = super().dump()
+        output["view_id"] = self.view_id.dump()
+        output["difference"] = self.changed_properties
+        return output
+
+
+@dataclass(frozen=True)
 class DirectRelationListWarning(DMSSchemaWarning):
     description = "The container property is set to a direct relation list, which is not supported by the CDF API"
     fix = "Make the property into a multiedge connection instead"
     error_name: ClassVar[str] = "DirectRelationListWarning"
     view_id: dm.ViewId
     container_id: dm.ContainerId
     property: str
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.73.0/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.73.0/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.73.0/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.73.0/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.73.0/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_base.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/__init__.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/__init__.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_base.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_field.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/_types/_value.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/base.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,29 @@
 
 import math
 import sys
 import types
 from abc import abstractmethod
 from collections.abc import Callable, Iterator
 from functools import wraps
-from typing import Any, ClassVar, Generic, TypeAlias, TypeVar
+from typing import Annotated, Any, ClassVar, Generic, TypeAlias, TypeVar
 
 import pandas as pd
-from pydantic import BaseModel, ConfigDict, Field, HttpUrl, constr, field_validator, model_serializer, model_validator
+from pydantic import (
+    BaseModel,
+    BeforeValidator,
+    ConfigDict,
+    Field,
+    HttpUrl,
+    PlainSerializer,
+    constr,
+    field_validator,
+    model_serializer,
+    model_validator,
+)
 from pydantic.fields import FieldInfo
 
 from cognite.neat.rules.models._rules._types import ClassType
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
@@ -314,7 +325,18 @@
         """Returns HTML representation of ResourceDict."""
         return self.to_pandas(drop_na_columns=True)._repr_html_()  # type: ignore[operator]
 
     @classmethod
     def mandatory_fields(cls, use_alias=False) -> set[str]:
         """Returns a set of mandatory fields for the model."""
         return _get_required_fields(cls, use_alias)
+
+
+ExtensionCategoryType = Annotated[
+    ExtensionCategory,
+    PlainSerializer(
+        lambda v: v.value if isinstance(v, ExtensionCategory) else v,
+        return_type=str,
+        when_used="unless-none",
+    ),
+    BeforeValidator(lambda v: ExtensionCategory(v) if isinstance(v, str) else v),
+]
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/dms_architect_rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/dms_architect_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from collections import defaultdict
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, ClassVar, Literal, cast
 
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes.data_modeling import PropertyType as CognitePropertyType
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex
-from cognite.client.data_classes.data_modeling.data_types import ListablePropertyType
 from cognite.client.data_classes.data_modeling.views import SingleReverseDirectRelationApply, ViewPropertyApply
 from pydantic import Field, field_validator, model_serializer, model_validator
 from pydantic_core.core_schema import SerializationInfo, ValidationInfo
 from rdflib import Namespace
 
 import cognite.neat.rules.issues.spreadsheet
 from cognite.neat.rules import issues
@@ -130,26 +129,29 @@
             name=self.name or None,
             version=self.version or "missing",
             description=description,
             views=[],
         )
 
     @classmethod
-    def from_data_model(cls, data_model: dm.DataModelApply) -> "DMSMetadata":
-        description = None
-        if data_model.description and (description_match := re.search(r"Creator: (.+)", data_model.description)):
+    def _get_description_and_creator(cls, description_raw: str | None) -> tuple[str | None, list[str]]:
+        if description_raw and (description_match := re.search(r"Creator: (.+)", description_raw)):
             creator = description_match.group(1).split(", ")
-            data_model.description.replace(f" Creator: {', '.join(creator)}", "")
-        elif data_model.description:
+            description = description_raw.replace(description_match.string, "").strip() or None
+        elif description_raw:
             creator = ["MISSING"]
-            description = data_model.description
+            description = description_raw
         else:
             creator = ["MISSING"]
-            description = "Missing description"
+            description = None
+        return description, creator
 
+    @classmethod
+    def from_data_model(cls, data_model: dm.DataModelApply) -> "DMSMetadata":
+        description, creator = cls._get_description_and_creator(data_model.description)
         return cls(
             schema_=SchemaCompleteness.complete,
             space=data_model.space,
             name=data_model.name or None,
             description=description,
             external_id=data_model.external_id,
             version=data_model.version,
@@ -487,19 +489,124 @@
                             )
                         )
         if errors:
             raise issues.MultiValueError(errors)
         return self
 
     @model_validator(mode="after")
+    def validate_extension(self) -> "DMSRules":
+        if self.metadata.schema_ is not SchemaCompleteness.extended:
+            return self
+        if not self.reference:
+            raise ValueError("The schema is set to 'extended', but no reference rules are provided to validate against")
+        is_solution = self.metadata.space != self.reference.metadata.space
+        if is_solution:
+            return self
+        if self.metadata.extension is ExtensionCategory.rebuild:
+            # Everything is allowed
+            return self
+        # Is an extension of an existing model.
+        user_schema = self.as_schema()
+        ref_schema = self.reference.as_schema()
+        new_containers = {container.as_id(): container for container in user_schema.containers}
+        existing_containers = {container.as_id(): container for container in ref_schema.containers}
+
+        errors: list[issues.NeatValidationError] = []
+        for container_id, container in new_containers.items():
+            existing_container = existing_containers.get(container_id)
+            if not existing_container or existing_container == container:
+                # No problem
+                continue
+            new_dumped = container.dump()
+            existing_dumped = existing_container.dump()
+            changed_attributes, changed_properties = self._changed_attributes_and_properties(
+                new_dumped, existing_dumped
+            )
+            errors.append(
+                issues.dms.ChangingContainerError(
+                    container_id=container_id,
+                    changed_properties=changed_properties or None,
+                    changed_attributes=changed_attributes or None,
+                )
+            )
+
+        if self.metadata.extension is ExtensionCategory.reshape and errors:
+            raise issues.MultiValueError(errors)
+        elif self.metadata.extension is ExtensionCategory.reshape:
+            # Reshape allows changes to views
+            return self
+
+        new_views = {view.as_id(): view for view in user_schema.views}
+        existing_views = {view.as_id(): view for view in ref_schema.views}
+        for view_id, view in new_views.items():
+            existing_view = existing_views.get(view_id)
+            if not existing_view or existing_view == view:
+                # No problem
+                continue
+            changed_attributes, changed_properties = self._changed_attributes_and_properties(
+                view.dump(), existing_view.dump()
+            )
+            errors.append(
+                issues.dms.ChangingViewError(
+                    view_id=view_id,
+                    changed_properties=changed_properties or None,
+                    changed_attributes=changed_attributes or None,
+                )
+            )
+
+        if errors:
+            raise issues.MultiValueError(errors)
+        return self
+
+    @staticmethod
+    def _changed_attributes_and_properties(
+        new_dumped: dict[str, Any], existing_dumped: dict[str, Any]
+    ) -> tuple[list[str], list[str]]:
+        """Helper method to find the changed attributes and properties between two containers or views."""
+        new_attributes = {key: value for key, value in new_dumped.items() if key != "properties"}
+        existing_attributes = {key: value for key, value in existing_dumped.items() if key != "properties"}
+        changed_attributes = [key for key in new_attributes if new_attributes[key] != existing_attributes.get(key)]
+        new_properties = new_dumped.get("properties", {})
+        existing_properties = existing_dumped.get("properties", {})
+        changed_properties = [prop for prop in new_properties if new_properties[prop] != existing_properties.get(prop)]
+        return changed_attributes, changed_properties
+
+    @model_validator(mode="after")
     def validate_schema(self) -> "DMSRules":
-        if self.metadata.schema_ is not SchemaCompleteness.complete:
+        if self.metadata.schema_ is SchemaCompleteness.partial:
             return self
+        elif self.metadata.schema_ is SchemaCompleteness.complete:
+            rules: DMSRules = self
+        elif self.metadata.schema_ is SchemaCompleteness.extended:
+            if not self.reference:
+                raise ValueError(
+                    "The schema is set to 'extended', but no reference rules are provided to validate against"
+                )
+            # This is an extension of the reference rules, we need to merge the two
+            rules = self.copy(deep=True)
+            rules.properties.extend(self.reference.properties.data)
+            existing_views = {view.view.as_id(False) for view in rules.views}
+            rules.views.extend([view for view in self.reference.views if view.view.as_id(False) not in existing_views])
+            if rules.containers and self.reference.containers:
+                existing_containers = {
+                    container.container.as_id(self.metadata.space) for container in rules.containers.data
+                }
+                rules.containers.extend(
+                    [
+                        container
+                        for container in self.reference.containers
+                        if container.container.as_id(self.reference.metadata.space) not in existing_containers
+                    ]
+                )
+            elif not rules.containers and self.reference.containers:
+                rules.containers = self.reference.containers
+        else:
+            raise ValueError("Unknown schema completeness")
 
-        schema = self.as_schema()
+        schema = rules.as_schema()
         errors = schema.validate()
         if errors:
             raise issues.MultiValueError(errors)
         return self
 
     @model_serializer(mode="plain", when_used="always")
     def dms_rules_serialization(self, info: SerializationInfo) -> dict[str, Any]:
@@ -549,20 +656,24 @@
                 if value := dumped.get(constraint_name):
                     dumped[constraint_name] = ",".join(
                         constraint.strip().removeprefix(default_space).removesuffix(default_version_wrapped)
                         for constraint in value.split(",")
                     )
             containers.append(dumped)
 
-        return {
+        output = {
             "Metadata" if info.by_alias else "metadata": self.metadata.model_dump(**kwargs),
             "Properties" if info.by_alias else "properties": properties,
             "Views" if info.by_alias else "views": views,
             "Containers" if info.by_alias else "containers": containers,
+            "is_reference": self.is_reference,
         }
+        if self.reference is not None:
+            output["Reference" if info.by_alias else "reference"] = self.reference.model_dump(**kwargs)
+        return output
 
     def as_schema(self, include_pipeline: bool = False, instance_space: str | None = None) -> DMSSchema:
         return _DMSExporter(include_pipeline, instance_space).to_schema(self)
 
     def as_information_architect_rules(self) -> "InformationRules":
         return _DMSRulesConverter(self).as_information_architect_rules()
 
@@ -868,18 +979,15 @@
                         nullable=prop.nullable if prop.nullable is not None else True,
                         default_value=prop.default,
                         name=prop.name,
                         description=prop.description,
                     )
                 else:
                     type_: CognitePropertyType
-                    if issubclass(type_cls, ListablePropertyType):
-                        type_ = type_cls(is_list=prop.is_list or False)
-                    else:
-                        type_ = cast(CognitePropertyType, type_cls())
+                    type_ = type_cls(is_list=prop.is_list or False)
                     container.properties[prop_name] = dm.ContainerProperty(
                         type=type_,
                         nullable=prop.nullable if prop.nullable is not None else True,
                         default_value=prop.default,
                         name=prop.name,
                         description=prop.description,
                     )
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/dms_schema.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/dms_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,18 @@
 
     @classmethod
     def from_model_id(cls, client: CogniteClient, data_model_id: dm.DataModelIdentifier) -> "DMSSchema":
         data_models = client.data_modeling.data_models.retrieve(data_model_id, inline_views=True)
         if len(data_models) == 0:
             raise ValueError(f"Data model {data_model_id} not found")
         data_model = data_models.latest_version()
+        return cls.from_data_model(client, data_model)
+
+    @classmethod
+    def from_data_model(cls, client: CogniteClient, data_model: dm.DataModel) -> "DMSSchema":
         views = dm.ViewList(data_model.views)
         container_ids = views.referenced_containers()
         containers = client.data_modeling.containers.retrieve(list(container_ids))
         cls._append_referenced_containers(client, containers)
 
         space_read = client.data_modeling.spaces.retrieve(data_model.space)
         if space_read is None:
@@ -263,15 +267,15 @@
         return output
 
     @classmethod
     def _to_sortable_identifier(cls, item: Any) -> str | tuple[str, str] | tuple[str, str, str]:
         if isinstance(item, dm.ContainerApply | dm.ViewApply | dm.DataModelApply | dm.NodeApply | RawTableWrite):
             identifier = item.as_id().as_tuple()
             if len(identifier) == 3 and identifier[2] is None:
-                return identifier[:2]
+                return identifier[:2]  # type: ignore[misc]
             return cast(tuple[str, str] | tuple[str, str, str], identifier)
         elif isinstance(item, dm.SpaceApply):
             return item.space
         elif isinstance(item, TransformationWrite):
             return item.external_id or ""
         elif isinstance(item, DatabaseWrite):
             return item.name or ""
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/domain_rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/domain_rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import math
 from typing import Any, ClassVar
 
-from pydantic import Field, model_serializer
+from pydantic import Field, field_serializer, field_validator, model_serializer
 from pydantic_core.core_schema import SerializationInfo
 
 from ._types import ParentClassType, PropertyType, SemanticValueType, StrOrListType
 from .base import (
     BaseMetadata,
     RoleTypes,
     RuleModel,
@@ -20,14 +21,26 @@
 
 class DomainProperty(SheetEntity):
     property_: PropertyType = Field(alias="Property")
     value_type: SemanticValueType = Field(alias="Value Type")
     min_count: int | None = Field(alias="Min Count", default=None)
     max_count: int | float | None = Field(alias="Max Count", default=None)
 
+    @field_serializer("max_count", when_used="json-unless-none")
+    def serialize_max_count(self, value: int | float | None) -> int | float | None | str:
+        if isinstance(value, float) and math.isinf(value):
+            return None
+        return value
+
+    @field_validator("max_count", mode="before")
+    def parse_max_count(cls, value: int | float | None) -> int | float | None:
+        if value is None:
+            return float("inf")
+        return value
+
 
 class DomainClass(SheetEntity):
     description: str | None = Field(None, alias="Description")
     parent: ParentClassType = Field(alias="Parent Class")
 
 
 class DomainRules(RuleModel):
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/_rules/information_rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/_rules/information_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import math
 import re
 import sys
 import warnings
 from collections import defaultdict
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, ClassVar, Literal, cast
 
-from pydantic import Field, field_validator, model_serializer, model_validator
+from pydantic import Field, field_serializer, field_validator, model_serializer, model_validator
 from pydantic_core.core_schema import SerializationInfo
 from rdflib import Namespace
 
 import cognite.neat.rules.issues.spreadsheet
 from cognite.neat.constants import PREFIXES
 from cognite.neat.rules import exceptions
 from cognite.neat.rules.models.rdfpath import (
@@ -43,14 +44,15 @@
     ViewPropEntity,
     XSDValueType,
 )
 from ._types._base import Unknown
 from .base import (
     BaseMetadata,
     ExtensionCategory,
+    ExtensionCategoryType,
     MatchType,
     RoleTypes,
     RuleModel,
     SchemaCompleteness,
     SheetEntity,
     SheetList,
 )
@@ -65,15 +67,15 @@
 else:
     from typing_extensions import Self
 
 
 class InformationMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.information_architect
     schema_: SchemaCompleteness = Field(alias="schema")
-    extension: ExtensionCategory | None = ExtensionCategory.addition
+    extension: ExtensionCategoryType | None = ExtensionCategory.addition
     prefix: PrefixType
     namespace: NamespaceType
 
     name: str = Field(
         alias="title",
         description="Human readable name of the data model",
         min_length=1,
@@ -152,14 +154,26 @@
     match_type: MatchType | None = Field(alias="Match Type", default=None)
     rule_type: str | TransformationRuleType | None = Field(alias="Rule Type", default=None)
     rule: str | AllReferences | SingleProperty | Hop | RawLookup | SPARQLQuery | Traversal | None = Field(
         alias="Rule", default=None
     )
     comment: str | None = Field(alias="Comment", default=None)
 
+    @field_serializer("max_count", when_used="json-unless-none")
+    def serialize_max_count(self, value: int | float | None) -> int | float | None | str:
+        if isinstance(value, float) and math.isinf(value):
+            return None
+        return value
+
+    @field_validator("max_count", mode="before")
+    def parse_max_count(cls, value: int | float | None) -> int | float | None:
+        if value is None:
+            return float("inf")
+        return value
+
     @model_validator(mode="after")
     def is_valid_rule(self):
         # TODO: Can we skip rule_type and simply try to parse the rule and if it fails, raise an error?
         if self.rule_type:
             self.rule_type = self.rule_type.lower()
             if not self.rule:
                 raise exceptions.RuleTypeProvidedButRuleMissing(
```

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/raw_rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/rules.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/rules/models/value_types.py` & `cognite_neat-0.73.0/cognite/neat/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/cdf.py` & `cognite_neat-0.73.0/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.73.0/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/exceptions.py` & `cognite_neat-0.73.0/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.73.0/cognite/neat/utils/spreadsheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Literal, overload
+from typing import Literal, cast, overload
 
 import pandas as pd
 from openpyxl import load_workbook
 from openpyxl.worksheet.worksheet import Worksheet
 
 
 @dataclass
@@ -54,15 +54,15 @@
 def read_individual_sheet(
     excel_file: pd.ExcelFile,
     sheet_name: str,
     return_read_info: bool = False,
     expected_headers: list[str] | None = None,
 ) -> tuple[list[dict], SpreadsheetRead] | list[dict]:
     if expected_headers:
-        target_row = _get_row_number(load_workbook(excel_file)[sheet_name], expected_headers)
+        target_row = _get_row_number(cast(Worksheet, load_workbook(excel_file)[sheet_name]), expected_headers)
         skiprows = target_row - 1 if target_row is not None else 0
     else:
         skiprows = 0
 
     raw = pd.read_excel(excel_file, sheet_name, skiprows=skiprows)
     is_na = raw.isnull().all(axis=1)
     empty_rows = is_na[is_na].index.tolist()
```

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/text.py` & `cognite_neat-0.73.0/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/utils.py` & `cognite_neat-0.73.0/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/utils/xml.py` & `cognite_neat-0.73.0/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.73.0/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/base.py` & `cognite_neat-0.73.0/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.73.0/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Export DMS/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Export DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Import DMS/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Import DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Validate Rules/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Validate Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml` & `cognite_neat-0.73.0/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/manager.py` & `cognite_neat-0.73.0/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.73.0/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.73.0/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/model.py` & `cognite_neat-0.73.0/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.73.0/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/tasks.py` & `cognite_neat-0.73.0/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/cognite/neat/workflows/triggers.py` & `cognite_neat-0.73.0/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.72.3/pyproject.toml` & `cognite_neat-0.73.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.72.3"
+version = "0.73.0"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
@@ -66,15 +66,15 @@
 exceptiongroup = { version = "^1.1.3", python = "<3.11" }
 'backports.strenum' = { version = "^1.2", python = "<3.11" }
 typing_extensions = { version = "^4.8", python = "<3.11" }
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 uvicorn = { extras = ["standard"], version = "^0.21.0" }
 prometheus-client = "^0.17.0"
-cognite-sdk = "^7.28.2"
+cognite-sdk = "^7.37.0"
 deepdiff = "*"
 fastapi = "^0.100"
 schedule = "^1"
 python-multipart = "^0.0.6"
 oxrdflib = { version = "^0.3.3", optional = true, extras = ["oxigraph"] }
```

### Comparing `cognite_neat-0.72.3/PKG-INFO` & `cognite_neat-0.73.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.72.3
+Version: 0.73.0
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,15 +15,15 @@
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: google
 Provides-Extra: graphql
 Provides-Extra: oxi
 Requires-Dist: PyYAML
 Requires-Dist: backports.strenum (>=1.2,<2.0) ; python_version < "3.11"
-Requires-Dist: cognite-sdk (>=7.28.2,<8.0.0)
+Requires-Dist: cognite-sdk (>=7.37.0,<8.0.0)
 Requires-Dist: deepdiff
 Requires-Dist: exceptiongroup (>=1.1.3,<2.0.0) ; python_version < "3.11"
 Requires-Dist: fastapi (>=0.100,<0.101)
 Requires-Dist: google-api-python-client ; extra == "google" or extra == "all"
 Requires-Dist: google-auth-oauthlib ; extra == "google" or extra == "all"
 Requires-Dist: gspread ; extra == "google" or extra == "all"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "graphql" or extra == "all"
```

