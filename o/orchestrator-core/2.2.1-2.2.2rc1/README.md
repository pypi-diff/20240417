# Comparing `tmp/orchestrator_core-2.2.1.tar.gz` & `tmp/orchestrator_core-2.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-2.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-2.2.2rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-2.2.1.tar` & `orchestrator_core-2.2.2rc1.tar`

### file list

```diff
@@ -1,535 +1,543 @@
--rw-r--r--   0        0        0      339 2024-04-08 13:21:43.970748 orchestrator_core-2.2.1/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.coveragerc
--rw-r--r--   0        0        0     1564 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1149 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      502 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2620 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      346 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      583 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/issues.yml
--rw-r--r--   0        0        0      550 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1215 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2255 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.gitignore
--rw-r--r--   0        0        0     2599 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/.stignore
--rw-r--r--   0        0        0    30927 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      333 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/Dockerfile
--rw-r--r--   0        0        0    11409 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/LICENSE
--rw-r--r--   0        0        0      150 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/NOTICE
--rw-r--r--   0        0        0     5595 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/README.md
--rw-r--r--   0        0        0      196 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/codecov.yml
--rw-r--r--   0        0        0       45 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/api.md
--rw-r--r--   0        0        0     5505 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/callbacks.md
--rw-r--r--   0        0        0    30737 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13882 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    24522 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/graphql.md
--rw-r--r--   0        0        0    48994 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5585 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2500 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11462 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0      668 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/context.md
--rw-r--r--   0        0        0      802 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/introduction.md
--rw-r--r--   0        0        0     1671 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/ip_static.md
--rw-r--r--   0        0        0    84576 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/ip_static.png
--rw-r--r--   0        0        0     1311 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/l2_point_to_point.md
--rw-r--r--   0        0        0    55937 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/l2_point_to_point.png
--rw-r--r--   0        0        0      854 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/l2_vpn.md
--rw-r--r--   0        0        0    29551 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/l2_vpn.png
--rw-r--r--   0        0        0     1398 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/modelling.md
--rw-r--r--   0        0        0     1138 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/node.md
--rw-r--r--   0        0        0    23110 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/node.png
--rw-r--r--   0        0        0     1147 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/port.md
--rw-r--r--   0        0        0    37248 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/port.png
--rw-r--r--   0        0        0     1694 2024-04-08 13:21:43.974748 orchestrator_core-2.2.1/docs/architecture/product_modelling/product_block_graph.md
--rw-r--r--   0        0        0    78824 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/architecture/product_modelling/product_block_graph.png
--rw-r--r--   0        0        0      989 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/architecture/product_modelling/standards.md
--rw-r--r--   0        0        0     1114 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/architecture/product_modelling/terminology.md
--rw-r--r--   0        0        0     2080 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/contributing/guidelines.md
--rw-r--r--   0        0        0     9997 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/css/custom.css
--rw-r--r--   0        0        0      656 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/css/style.css
--rw-r--r--   0        0        0     2165 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/getting-started/development.md
--rw-r--r--   0        0        0     3438 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/getting-started/prepare-source-folder.md
--rw-r--r--   0        0        0    17905 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/img/WFO-Emblem-White.png
--rw-r--r--   0        0        0      842 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/img/favicon.ico
--rw-r--r--   0        0        0     4020 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/index.md
--rw-r--r--   0        0        0     3897 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/js/termynal.js
--rw-r--r--   0        0        0    11084 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/migration-guide/2.0.md
--rw-r--r--   0        0        0     9063 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3719 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     6048 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3087 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5602 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4623 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7447 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3697 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3051 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6156 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1953 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3991 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3596 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2141 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2878 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      785 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3632 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2024-04-08 13:21:43.978748 orchestrator_core-2.2.1/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2024-04-08 13:21:43.982748 orchestrator_core-2.2.1/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0     5478 2024-04-08 13:21:43.982748 orchestrator_core-2.2.1/mkdocs.yml
--rw-r--r--   0        0        0     1262 2024-04-08 13:21:43.982748 orchestrator_core-2.2.1/mutmut_config.py
--rw-r--r--   0        0        0       70 2024-04-08 13:21:43.982748 orchestrator_core-2.2.1/nitpick-style.toml
--rw-r--r--   0        0        0     1095 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     3145 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     1034 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1284 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    14531 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     4021 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     4806 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     3657 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     6106 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2977 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    15675 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      963 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1827 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     2563 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1722 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/ws.py
--rw-r--r--   0        0        0     1502 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    10612 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5996 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/api/models.py
--rw-r--r--   0        0        0     8365 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/app.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13792 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6775 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     2172 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10474 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9379 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    23981 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1399 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     7377 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0      173 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/README
--rw-r--r--   0        0        0      307 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
--rw-r--r--   0        0        0      115 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
--rw-r--r--   0        0        0      307 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
--rw-r--r--   0        0        0      115 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
--rw-r--r--   0        0        0      234 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
--rw-r--r--   0        0        0      131 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     2007 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/enums.py
--rw-r--r--   0        0        0     5452 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     6341 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2073 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5285 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1379 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1878 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4541 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1815 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     8026 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      759 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      538 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      532 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      361 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      431 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/additional_create_imports.j2
--rw-r--r--   0        0        0       25 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/additional_create_steps.j2
--rw-r--r--   0        0        0      394 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/additional_modify_imports.j2
--rw-r--r--   0        0        0       25 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/additional_modify_steps.j2
--rw-r--r--   0        0        0       25 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0      282 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0      361 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/create_data_head.j2
--rw-r--r--   0        0        0     4806 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      298 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/enums.j2
--rw-r--r--   0        0        0      523 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
--rw-r--r--   0        0        0      277 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      904 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4719 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2901 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1365 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2454 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      545 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     1274 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/shared_workflows.j2
--rw-r--r--   0        0        0      291 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/subscription_model_registry.j2
--rw-r--r--   0        0        0     1883 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1802 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1677 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2024-04-08 13:21:43.986748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      985 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2315 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1139 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      857 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20371 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8979 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4110 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2970 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10269 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/database.py
--rw-r--r--   0        0        0      371 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     5020 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0     4098 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0      899 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0     1089 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/product_block.py
--rw-r--r--   0        0        0      889 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/resource_type.py
--rw-r--r--   0        0        0      562 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/search_filters/__init__.py
--rw-r--r--   0        0        0     5170 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/search_filters/inferred_filter.py
--rw-r--r--   0        0        0     1466 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/subscription.py
--rw-r--r--   0        0        0     1276 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/filters/workflow.py
--rw-r--r--   0        0        0      283 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/helpers.py
--rw-r--r--   0        0        0    24840 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/models.py
--rw-r--r--   0        0        0      162 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     2175 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      353 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0     1987 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      570 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0      617 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/sorting/product_block.py
--rw-r--r--   0        0        0      617 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/sorting/resource_type.py
--rw-r--r--   0        0        0     4455 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0     1441 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/sorting/subscription.py
--rw-r--r--   0        0        0      576 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/db/sorting/workflow.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    18847 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/devtools/scripts/__init__.py
--rw-r--r--   0        0        0     8359 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/devtools/scripts/migrate_20.py
--rw-r--r--   0        0        0     2494 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2508 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3114 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3271 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      894 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    59246 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/domain/base.py
--rw-r--r--   0        0        0      989 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/domain/helpers.py
--rw-r--r--   0        0        0     2882 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     1268 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0      892 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     1906 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/forms/validators/__init__.py
--rw-r--r--   0        0        0     1505 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/forms/validators/customer_contact_list.py
--rw-r--r--   0        0        0      708 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/forms/validators/customer_id.py
--rw-r--r--   0        0        0      779 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/forms/validators/display_subscription.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/forms/validators/network_type_validators.py
--rw-r--r--   0        0        0     2114 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/forms/validators/product_id.py
--rw-r--r--   0        0        0     1378 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0     6161 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/autoregistration.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4304 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     1746 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/extensions/error_collector_extension.py
--rw-r--r--   0        0        0     5826 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/extensions/error_handler_extension.py
--rw-r--r--   0        0        0     2413 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      851 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0      934 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/customer.py
--rw-r--r--   0        0        0      636 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/helpers.py
--rw-r--r--   0        0        0     4491 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2562 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     2748 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/product_block.py
--rw-r--r--   0        0        0     2741 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/resource_type.py
--rw-r--r--   0        0        0     3700 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0     5531 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/subscription.py
--rw-r--r--   0        0        0     2681 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/resolvers/workflow.py
--rw-r--r--   0        0        0     6699 2024-04-08 13:21:43.990748 orchestrator_core-2.2.1/orchestrator/graphql/schema.py
--rw-r--r--   0        0        0     1003 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/__init__.py
--rw-r--r--   0        0        0      115 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/customer.py
--rw-r--r--   0        0        0      203 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     3475 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     2134 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0     1203 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      755 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      999 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0     7958 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/subscription.py
--rw-r--r--   0        0        0     1140 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     3813 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      524 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0     1191 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/utils/create_resolver_error_handler.py
--rw-r--r--   0        0        0     1002 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0     3897 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/utils/get_subscription_product_blocks.py
--rw-r--r--   0        0        0     2156 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/utils/is_query_detailed.py
--rw-r--r--   0        0        0     1370 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/utils/override_class.py
--rw-r--r--   0        0        0      902 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/graphql/utils/to_graphql_result_page.py
--rw-r--r--   0        0        0       39 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3382 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40911 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2698 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1265 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    39307 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      950 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1214 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1603 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5106 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7964 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0     1014 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0      591 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
--rw-r--r--   0        0        0      755 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
--rw-r--r--   0        0        0      967 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
--rw-r--r--   0        0        0     4491 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
--rw-r--r--   0        0        0     1036 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
--rw-r--r--   0        0        0     5480 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
--rw-r--r--   0        0        0     2246 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/py.typed
--rw-r--r--   0        0        0     1066 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1526 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1234 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2195 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2708 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      888 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1286 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1356 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      802 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     2693 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1698 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1792 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      973 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3366 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1030 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1977 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1744 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/security.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3635 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/celery.py
--rw-r--r--   0        0        0      876 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/fixed_inputs.py
--rw-r--r--   0        0        0    28515 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1933 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/products.py
--rw-r--r--   0        0        0      884 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/resource_types.py
--rw-r--r--   0        0        0     2723 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/settings.py
--rw-r--r--   0        0        0    25733 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5867 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1713 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/translations.py
--rw-r--r--   0        0        0     1638 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/services/workflows.py
--rw-r--r--   0        0        0     3634 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/targets.py
--rw-r--r--   0        0        0    16236 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/types.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.994748 orchestrator_core-2.2.1/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5584 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0      875 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/deprecation_logger.py
--rw-r--r--   0        0        0     6172 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     4658 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/enrich_process.py
--rw-r--r--   0        0        0     4250 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     2665 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/fixed_inputs.py
--rw-r--r--   0        0        0     8063 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     1322 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/get_updated_properties.py
--rw-r--r--   0        0        0     3212 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8341 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/json.py
--rw-r--r--   0        0        0     5582 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/redis.py
--rw-r--r--   0        0        0    15801 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/search_query.py
--rw-r--r--   0        0        0    12998 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     1366 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/version.py
--rw-r--r--   0        0        0     4828 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     4596 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3324 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2924 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    42689 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflow.py
--rw-r--r--   0        0        0     4048 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9528 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1614 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2349 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8511 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    12929 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     5073 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     2725 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/setup.cfg
--rw-r--r--   0        0        0      665 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/setup.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1529 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2887 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5160 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1626 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1139 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3055 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    21379 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    15509 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3863 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     8209 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2614 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     3000 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     3005 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    41173 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     3457 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0     3777 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/api/test_ws.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/cli/__init__.py
--rw-r--r--   0        0        0      744 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate.sh
--rw-r--r--   0        0        0      885 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/alembic.ini
--rw-r--r--   0        0        0      233 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/main.py
--rw-r--r--   0        0        0     2821 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/env.py
--rw-r--r--   0        0        0       98 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-04-08 13:21:43.998748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/script.py.mako
--rw-r--r--   0        0        0      315 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
--rw-r--r--   0        0        0     2227 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
--rw-r--r--   0        0        0     3852 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
--rw-r--r--   0        0        0      467 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1995 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
--rw-r--r--   0        0        0      812 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_types/__init__.py
--rw-r--r--   0        0        0      764 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_types/example1.py
--rw-r--r--   0        0        0      559 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_types/example2.py
--rw-r--r--   0        0        0     1499 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
--rw-r--r--   0        0        0     1499 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
--rw-r--r--   0        0        0     2442 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
--rw-r--r--   0        0        0     2014 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
--rw-r--r--   0        0        0     1345 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
--rw-r--r--   0        0        0     1010 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
--rw-r--r--   0        0        0      902 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
--rw-r--r--   0        0        0      872 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
--rw-r--r--   0        0        0      755 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
--rw-r--r--   0        0        0      405 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
--rw-r--r--   0        0        0      415 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/translations/en-GB.json
--rw-r--r--   0        0        0      701 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/__init__.py
--rw-r--r--   0        0        0     3940 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
--rw-r--r--   0        0        0     3602 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
--rw-r--r--   0        0        0      620 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
--rw-r--r--   0        0        0     1560 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
--rw-r--r--   0        0        0     1025 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
--rw-r--r--   0        0        0     2683 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
--rw-r--r--   0        0        0     2508 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
--rw-r--r--   0        0        0        1 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
--rw-r--r--   0        0        0     1220 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
--rw-r--r--   0        0        0     1273 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/shared.py
--rw-r--r--   0        0        0     2656 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/product_config1.yaml
--rw-r--r--   0        0        0      549 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/product_config2.yaml
--rw-r--r--   0        0        0      590 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/data/product_config3.yaml
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/generator/__init__.py
--rw-r--r--   0        0        0      812 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/generator/test_enums.py
--rw-r--r--   0        0        0     2509 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/test_cli_generate.py
--rw-r--r--   0        0        0     2930 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/test_generate_code.py
--rw-r--r--   0        0        0    26343 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27644 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/config.py
--rw-r--r--   0        0        0    23677 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    53002 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8230 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4670 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     1992 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/domain/test_lifecycle.py
--rw-r--r--   0        0        0     2841 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7794 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1645 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2970 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1606 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2573 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2518 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1194 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1123 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2172 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4217 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3428 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2951 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2272 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2256 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1639 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1838 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      644 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0      451 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/fixtures/workflows.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     4706 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/forms/test_customer_contact_list.py
--rw-r--r--   0        0        0      495 2024-04-08 13:21:44.002748 orchestrator_core-2.2.1/test/unit_tests/forms/test_customer_id.py
--rw-r--r--   0        0        0     1746 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/forms/test_display_subscription.py
--rw-r--r--   0        0        0     4109 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/__init__.py
--rw-r--r--   0        0        0      690 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/conftest.py
--rw-r--r--   0        0        0     2316 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_customer.py
--rw-r--r--   0        0        0    18677 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     8514 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0    10211 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_product_blocks.py
--rw-r--r--   0        0        0     5635 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_resource_types.py
--rw-r--r--   0        0        0     5179 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0     2939 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_sort_and_filter_fields.py
--rw-r--r--   0        0        0     3239 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_subscription.py
--rw-r--r--   0        0        0    48810 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_subscriptions.py
--rw-r--r--   0        0        0     6682 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/test_workflows.py
--rw-r--r--   0        0        0      608 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/utils/test_autoregistration.py
--rw-r--r--   0        0        0     7669 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/utils/test_is_query_detailed.py
--rw-r--r--   0        0        0     3042 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/utils/test_is_querying_page_data.py
--rw-r--r--   0        0        0     8760 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/graphql/utils/test_override_class.py
--rw-r--r--   0        0        0      631 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/helpers.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    28556 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1155 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     6171 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     6650 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      379 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    17406 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1891 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3486 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3529 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/test_get_updated_properties.py
--rw-r--r--   0        0        0     3052 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     4613 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/test_search_query.py
--rw-r--r--   0        0        0    11471 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/websocket/__init__.py
--rw-r--r--   0        0        0     3561 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/websocket/test_broadcast.py
--rw-r--r--   0        0        0    14040 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2094 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2746 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     5378 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/test_async_workflow.py
--rw-r--r--   0        0        0     3495 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1884 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2024-04-08 13:21:44.006748 orchestrator_core-2.2.1/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 orchestrator_core-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      342 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.coveragerc
+-rw-r--r--   0        0        0     1564 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1149 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      502 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2620 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      346 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      583 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/issues.yml
+-rw-r--r--   0        0        0      550 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1215 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2255 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.gitignore
+-rw-r--r--   0        0        0     2599 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.stignore
+-rw-r--r--   0        0        0    30927 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/Dockerfile
+-rw-r--r--   0        0        0    11409 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/LICENSE
+-rw-r--r--   0        0        0      150 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/NOTICE
+-rw-r--r--   0        0        0     5595 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/README.md
+-rw-r--r--   0        0        0      196 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/codecov.yml
+-rw-r--r--   0        0        0       45 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/api.md
+-rw-r--r--   0        0        0     5505 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/callbacks.md
+-rw-r--r--   0        0        0    30737 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13882 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    24522 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/graphql.md
+-rw-r--r--   0        0        0    48994 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5585 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2500 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11462 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0      668 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/context.md
+-rw-r--r--   0        0        0      802 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/introduction.md
+-rw-r--r--   0        0        0     1671 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/ip_static.md
+-rw-r--r--   0        0        0    84576 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/ip_static.png
+-rw-r--r--   0        0        0     1311 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_point_to_point.md
+-rw-r--r--   0        0        0    55937 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_point_to_point.png
+-rw-r--r--   0        0        0      854 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_vpn.md
+-rw-r--r--   0        0        0    29551 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_vpn.png
+-rw-r--r--   0        0        0     1398 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/modelling.md
+-rw-r--r--   0        0        0     1138 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/node.md
+-rw-r--r--   0        0        0    23110 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/node.png
+-rw-r--r--   0        0        0     1147 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/port.md
+-rw-r--r--   0        0        0    37248 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/port.png
+-rw-r--r--   0        0        0     1694 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/product_block_graph.md
+-rw-r--r--   0        0        0    78824 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/product_block_graph.png
+-rw-r--r--   0        0        0      989 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/standards.md
+-rw-r--r--   0        0        0     1114 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/terminology.md
+-rw-r--r--   0        0        0     2080 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0     9997 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/css/custom.css
+-rw-r--r--   0        0        0      656 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/css/style.css
+-rw-r--r--   0        0        0     2165 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/getting-started/development.md
+-rw-r--r--   0        0        0     3438 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/getting-started/prepare-source-folder.md
+-rw-r--r--   0        0        0    17905 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/img/WFO-Emblem-White.png
+-rw-r--r--   0        0        0      842 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/img/favicon.ico
+-rw-r--r--   0        0        0     4020 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/index.md
+-rw-r--r--   0        0        0     3897 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/js/termynal.js
+-rw-r--r--   0        0        0    11084 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/migration-guide/2.0.md
+-rw-r--r--   0        0        0     9063 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3719 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     6048 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3087 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5602 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4623 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7447 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3697 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3051 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6156 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1953 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3991 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3596 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2141 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2878 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      785 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3632 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0     5478 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/mkdocs.yml
+-rw-r--r--   0        0        0     1262 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/mutmut_config.py
+-rw-r--r--   0        0        0       70 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/nitpick-style.toml
+-rw-r--r--   0        0        0     1098 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     3145 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     1034 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1284 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    14585 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     4021 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     4806 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     3657 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     6106 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     3081 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    15675 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      963 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1827 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     2563 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1722 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/ws.py
+-rw-r--r--   0        0        0     1502 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    10612 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5996 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/models.py
+-rw-r--r--   0        0        0     8416 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13792 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6775 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     2172 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10474 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9379 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    23981 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1399 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     7377 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/README
+-rw-r--r--   0        0        0      307 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
+-rw-r--r--   0        0        0      115 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      307 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0      115 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0      234 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
+-rw-r--r--   0        0        0      131 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     2007 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/enums.py
+-rw-r--r--   0        0        0     5452 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     6341 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2073 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5285 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1379 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1878 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4541 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1815 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     8026 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      759 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      538 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      532 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      361 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      431 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_create_imports.j2
+-rw-r--r--   0        0        0       25 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      394 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0       25 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0       25 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0      282 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0      361 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/create_data_head.j2
+-rw-r--r--   0        0        0     4806 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      298 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/enums.j2
+-rw-r--r--   0        0        0      523 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
+-rw-r--r--   0        0        0      277 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      904 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4719 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2901 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1365 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2454 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      545 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     1274 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/shared_workflows.j2
+-rw-r--r--   0        0        0      291 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/subscription_model_registry.j2
+-rw-r--r--   0        0        0     1883 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1802 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1677 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      985 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2315 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1139 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      857 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20371 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8979 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4110 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2970 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10269 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/database.py
+-rw-r--r--   0        0        0      371 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     5020 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0     4098 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0      899 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     1089 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/product_block.py
+-rw-r--r--   0        0        0      889 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/resource_type.py
+-rw-r--r--   0        0        0      562 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/search_filters/__init__.py
+-rw-r--r--   0        0        0     5170 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/search_filters/inferred_filter.py
+-rw-r--r--   0        0        0     1466 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0     1276 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/workflow.py
+-rw-r--r--   0        0        0      283 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/helpers.py
+-rw-r--r--   0        0        0    24840 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/models.py
+-rw-r--r--   0        0        0      162 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     2175 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      353 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0     1987 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      570 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0      617 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/product_block.py
+-rw-r--r--   0        0        0      617 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/resource_type.py
+-rw-r--r--   0        0        0     4455 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0     1441 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0      576 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    18847 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/devtools/scripts/__init__.py
+-rw-r--r--   0        0        0     8359 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/devtools/scripts/migrate_20.py
+-rw-r--r--   0        0        0     2494 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2508 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3114 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3271 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      894 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    59246 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2732 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/domain/customer_description.py
+-rw-r--r--   0        0        0      989 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/domain/helpers.py
+-rw-r--r--   0        0        0     2882 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     1268 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0      892 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     1906 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/__init__.py
+-rw-r--r--   0        0        0     1505 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/customer_contact_list.py
+-rw-r--r--   0        0        0      708 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/customer_id.py
+-rw-r--r--   0        0        0      779 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/display_subscription.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/network_type_validators.py
+-rw-r--r--   0        0        0     2114 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/product_id.py
+-rw-r--r--   0        0        0     1378 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0     6161 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/autoregistration.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4304 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1746 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     5826 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/error_handler_extension.py
+-rw-r--r--   0        0        0     3100 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/mutations/customer_description.py
+-rw-r--r--   0        0        0     1553 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/mutations/start_process.py
+-rw-r--r--   0        0        0     2413 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      851 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/customer.py
+-rw-r--r--   0        0        0      636 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/helpers.py
+-rw-r--r--   0        0        0     4491 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2562 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     2748 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/product_block.py
+-rw-r--r--   0        0        0     2741 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/resource_type.py
+-rw-r--r--   0        0        0     3700 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     5531 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0     2681 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/workflow.py
+-rw-r--r--   0        0        0     7403 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schema.py
+-rw-r--r--   0        0        0     1003 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/__init__.py
+-rw-r--r--   0        0        0      115 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/customer.py
+-rw-r--r--   0        0        0      213 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/customer_description.py
+-rw-r--r--   0        0        0      203 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3475 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     2134 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0     1203 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      755 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      999 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7838 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0     1140 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     4470 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      524 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1191 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0     1002 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0     3897 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/get_subscription_product_blocks.py
+-rw-r--r--   0        0        0     2156 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/is_query_detailed.py
+-rw-r--r--   0        0        0     1370 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/override_class.py
+-rw-r--r--   0        0        0      902 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/to_graphql_result_page.py
+-rw-r--r--   0        0        0       39 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3382 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40911 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2698 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1265 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    39307 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      950 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1214 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1603 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5106 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7964 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0     1014 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0      591 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
+-rw-r--r--   0        0        0      755 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
+-rw-r--r--   0        0        0      967 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
+-rw-r--r--   0        0        0     4491 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
+-rw-r--r--   0        0        0     1036 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
+-rw-r--r--   0        0        0     5480 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
+-rw-r--r--   0        0        0     2246 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/py.typed
+-rw-r--r--   0        0        0     1066 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1526 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1234 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2195 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2708 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      888 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1286 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1356 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      802 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     2693 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1698 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1792 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      973 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3366 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1030 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1977 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1744 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3635 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/celery.py
+-rw-r--r--   0        0        0      876 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/fixed_inputs.py
+-rw-r--r--   0        0        0     3710 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/process_broadcast_thread.py
+-rw-r--r--   0        0        0    26253 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1933 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/products.py
+-rw-r--r--   0        0        0      884 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/resource_types.py
+-rw-r--r--   0        0        0     2723 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    25733 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5867 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1713 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     1638 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/workflows.py
+-rw-r--r--   0        0        0     3634 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/targets.py
+-rw-r--r--   0        0        0    16236 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5584 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0      875 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/deprecation_logger.py
+-rw-r--r--   0        0        0     6172 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     4658 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/enrich_process.py
+-rw-r--r--   0        0        0     4250 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     2665 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/fixed_inputs.py
+-rw-r--r--   0        0        0     8063 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     1322 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/get_updated_properties.py
+-rw-r--r--   0        0        0     3212 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8341 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     6378 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0    15801 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/search_query.py
+-rw-r--r--   0        0        0    12998 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     1366 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/version.py
+-rw-r--r--   0        0        0     4828 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     4596 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3324 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2924 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    42689 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4048 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9528 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1614 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2349 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8511 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12929 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     5073 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2725 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/setup.cfg
+-rw-r--r--   0        0        0      665 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/setup.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1529 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2887 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5160 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1626 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1139 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3055 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    21379 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    15509 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3863 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     8209 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2614 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     3000 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     3038 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    41173 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     3457 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0     3777 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_ws.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate.sh
+-rw-r--r--   0        0        0      885 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/alembic.ini
+-rw-r--r--   0        0        0      233 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/main.py
+-rw-r--r--   0        0        0     2821 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/env.py
+-rw-r--r--   0        0        0       98 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/script.py.mako
+-rw-r--r--   0        0        0      315 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
+-rw-r--r--   0        0        0     2227 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
+-rw-r--r--   0        0        0     3852 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
+-rw-r--r--   0        0        0      467 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1995 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
+-rw-r--r--   0        0        0      812 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/example1.py
+-rw-r--r--   0        0        0      559 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/example2.py
+-rw-r--r--   0        0        0     1499 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
+-rw-r--r--   0        0        0     1499 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
+-rw-r--r--   0        0        0     2442 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
+-rw-r--r--   0        0        0     2014 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
+-rw-r--r--   0        0        0     1345 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
+-rw-r--r--   0        0        0     1010 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
+-rw-r--r--   0        0        0      902 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
+-rw-r--r--   0        0        0      872 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
+-rw-r--r--   0        0        0      755 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
+-rw-r--r--   0        0        0      405 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
+-rw-r--r--   0        0        0      415 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/translations/en-GB.json
+-rw-r--r--   0        0        0      701 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/__init__.py
+-rw-r--r--   0        0        0     3940 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
+-rw-r--r--   0        0        0     3602 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
+-rw-r--r--   0        0        0      620 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
+-rw-r--r--   0        0        0     1560 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
+-rw-r--r--   0        0        0     1025 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
+-rw-r--r--   0        0        0     2683 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
+-rw-r--r--   0        0        0     2508 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
+-rw-r--r--   0        0        0        1 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
+-rw-r--r--   0        0        0     1220 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
+-rw-r--r--   0        0        0     1273 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/shared.py
+-rw-r--r--   0        0        0     2656 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config1.yaml
+-rw-r--r--   0        0        0      549 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config2.yaml
+-rw-r--r--   0        0        0      590 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config3.yaml
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/generator/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/generator/test_enums.py
+-rw-r--r--   0        0        0     2509 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_cli_generate.py
+-rw-r--r--   0        0        0     2930 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_generate_code.py
+-rw-r--r--   0        0        0    26343 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27644 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/config.py
+-rw-r--r--   0        0        0    23677 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    53002 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8230 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4670 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     1992 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_lifecycle.py
+-rw-r--r--   0        0        0     2841 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7794 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1645 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2970 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1606 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2573 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2518 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1194 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1123 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2172 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4217 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3428 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2951 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2272 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2256 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1639 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1838 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      644 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0      451 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     4706 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_customer_contact_list.py
+-rw-r--r--   0        0        0      495 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_customer_id.py
+-rw-r--r--   0        0        0     1746 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_display_subscription.py
+-rw-r--r--   0        0        0     4109 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/conftest.py
+-rw-r--r--   0        0        0      488 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/mutations/helpers.py
+-rw-r--r--   0        0        0     6235 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/mutations/test_customer_description.py
+-rw-r--r--   0        0        0     2449 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/mutations/test_start_process.py
+-rw-r--r--   0        0        0     2316 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_customer.py
+-rw-r--r--   0        0        0    18677 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     8514 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0    10211 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_product_blocks.py
+-rw-r--r--   0        0        0     5635 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_resource_types.py
+-rw-r--r--   0        0        0     5179 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0     2939 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_sort_and_filter_fields.py
+-rw-r--r--   0        0        0     3239 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_subscription.py
+-rw-r--r--   0        0        0    48810 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0     6682 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_workflows.py
+-rw-r--r--   0        0        0      608 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_autoregistration.py
+-rw-r--r--   0        0        0     7669 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_is_query_detailed.py
+-rw-r--r--   0        0        0     3042 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_is_querying_page_data.py
+-rw-r--r--   0        0        0     8760 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_override_class.py
+-rw-r--r--   0        0        0      631 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    28556 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1155 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     6171 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     6650 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      379 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    17406 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1891 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3486 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3529 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_get_updated_properties.py
+-rw-r--r--   0        0        0     3052 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     4613 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_search_query.py
+-rw-r--r--   0        0        0    11471 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/websocket/__init__.py
+-rw-r--r--   0        0        0     3561 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/websocket/test_broadcast.py
+-rw-r--r--   0        0        0    14040 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2094 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2746 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     5378 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_async_workflow.py
+-rw-r--r--   0        0        0     3495 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1884 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 orchestrator_core-2.2.2rc1/PKG-INFO
```

### Comparing `orchestrator_core-2.2.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `orchestrator_core-2.2.2rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/ISSUE_TEMPLATE/feature-request.yml` & `orchestrator_core-2.2.2rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/workflows/README.md` & `orchestrator_core-2.2.2rc1/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/workflows/build-push-container.yml` & `orchestrator_core-2.2.2rc1/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/workflows/codeql-analysis.yml` & `orchestrator_core-2.2.2rc1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/workflows/issues.yml` & `orchestrator_core-2.2.2rc1/.github/workflows/issues.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/workflows/publish-package.yml` & `orchestrator_core-2.2.2rc1/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/workflows/run-linting-tests.yml` & `orchestrator_core-2.2.2rc1/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/workflows/run-unit-tests.yml` & `orchestrator_core-2.2.2rc1/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.github/workflows/scheduled-build.yml` & `orchestrator_core-2.2.2rc1/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.gitignore` & `orchestrator_core-2.2.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.pre-commit-config.yaml` & `orchestrator_core-2.2.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/.stignore` & `orchestrator_core-2.2.2rc1/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/CHANGELOG.md` & `orchestrator_core-2.2.2rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/LICENSE` & `orchestrator_core-2.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/README.md` & `orchestrator_core-2.2.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/callbacks.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/callbacks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/cli.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/domainmodels.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/forms.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/graphql.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/graphql.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/openapi.json` & `orchestrator_core-2.2.2rc1/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/python.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/scaling.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/tasks.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/websockets.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/application/workflow.md` & `orchestrator_core-2.2.2rc1/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/context.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/context.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/introduction.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/ip_static.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/ip_static.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/ip_static.png` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/ip_static.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/l2_point_to_point.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_point_to_point.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/l2_point_to_point.png` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_point_to_point.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/l2_vpn.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_vpn.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/l2_vpn.png` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_vpn.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/modelling.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/modelling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/node.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/node.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/node.png` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/node.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/port.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/port.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/port.png` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/port.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/product_block_graph.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/product_block_graph.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/product_block_graph.png` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/product_block_graph.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/standards.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/standards.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/product_modelling/terminology.md` & `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/terminology.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/architecture/tldr.md` & `orchestrator_core-2.2.2rc1/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/contributing/guidelines.md` & `orchestrator_core-2.2.2rc1/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/contributing/testing.md` & `orchestrator_core-2.2.2rc1/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/css/style.css` & `orchestrator_core-2.2.2rc1/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/css/termynal.css` & `orchestrator_core-2.2.2rc1/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/getting-started/base.md` & `orchestrator_core-2.2.2rc1/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/getting-started/development.md` & `orchestrator_core-2.2.2rc1/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/getting-started/prepare-source-folder.md` & `orchestrator_core-2.2.2rc1/docs/getting-started/prepare-source-folder.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/img/WFO-Emblem-White.png` & `orchestrator_core-2.2.2rc1/docs/img/WFO-Emblem-White.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/img/favicon.ico` & `orchestrator_core-2.2.2rc1/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/index.md` & `orchestrator_core-2.2.2rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/js/custom.js` & `orchestrator_core-2.2.2rc1/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/js/termynal.js` & `orchestrator_core-2.2.2rc1/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/migration-guide/2.0.md` & `orchestrator_core-2.2.2rc1/docs/migration-guide/2.0.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-2.2.2rc1/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-2.2.2rc1/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/advanced/domain-models.md` & `orchestrator_core-2.2.2rc1/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-2.2.2rc1/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/advanced/overview.md` & `orchestrator_core-2.2.2rc1/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/advanced/scenario.md` & `orchestrator_core-2.2.2rc1/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-2.2.2rc1/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/create-user.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/database-migration.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/debian.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/docker.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/domain-models.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/explore.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/input-forms.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/macos.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/modify-user.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/overview.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/scenario.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/start-applications.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-2.2.2rc1/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/images/metadata_products.png` & `orchestrator_core-2.2.2rc1/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-2.2.2rc1/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/mkdocs.yml` & `orchestrator_core-2.2.2rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/mutmut_config.py` & `orchestrator_core-2.2.2rc1/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "2.2.1"
+__version__ = "2.2.2rc1"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-2.2.1/orchestrator/api/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/api.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,20 +47,20 @@
     ProcessSchema,
     ProcessStatusCounts,
     ProcessSubscriptionBaseSchema,
     ProcessSubscriptionSchema,
     Reporter,
 )
 from orchestrator.security import oidc_user
+from orchestrator.services.process_broadcast_thread import api_broadcast_process_data
 from orchestrator.services.processes import (
     SYSTEM_USER,
     _async_resume_processes,
     _get_process,
     abort_process,
-    api_broadcast_process_data,
     continue_awaiting_process,
     load_process,
     resume_process,
     start_process,
 )
 from orchestrator.services.settings import get_engine_settings
 from orchestrator.settings import app_settings
```

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,44 +7,44 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from datetime import datetime
 from http import HTTPStatus
 from uuid import UUID
 
 from fastapi.param_functions import Body
 from fastapi.routing import APIRouter
-from pytz import timezone
-from sqlalchemy import select
 
 from orchestrator.api.error_handling import raise_status
-from orchestrator.api.models import delete, save, update
+from orchestrator.api.models import delete
 from orchestrator.db import SubscriptionCustomerDescriptionTable, db
+from orchestrator.domain.customer_description import (
+    create_subscription_customer_description,
+    get_customer_description_by_customer_subscription,
+    update_subscription_customer_description,
+)
 from orchestrator.schemas import SubscriptionDescriptionBaseSchema, SubscriptionDescriptionSchema
 from orchestrator.utils.redis import delete_from_redis
 
 router = APIRouter()
 
 
 @router.post("/", response_model=None, status_code=HTTPStatus.NO_CONTENT)
-def save_subscription_customer_description(data: SubscriptionDescriptionBaseSchema = Body(...)) -> None:
-    save(SubscriptionCustomerDescriptionTable, data)
-    delete_from_redis(data.subscription_id)
+def save_subscription_customer_description_endpoint(data: SubscriptionDescriptionBaseSchema = Body(...)) -> None:
+    create_subscription_customer_description(data.customer_id, data.subscription_id, data.description)
 
 
 @router.put("/", response_model=None, status_code=HTTPStatus.NO_CONTENT)
-def update_subscription_customer_descriptions(data: SubscriptionDescriptionSchema = Body(...)) -> None:
-    if data.created_at is None:
-        data.created_at = datetime.now(tz=timezone("UTC"))
-    update(SubscriptionCustomerDescriptionTable, data)
-    delete_from_redis(data.subscription_id)
+def update_subscription_customer_description_endpoint(data: SubscriptionDescriptionSchema = Body(...)) -> None:
+    description = get_customer_description_by_customer_subscription(data.customer_id, data.subscription_id)
+    if description:
+        update_subscription_customer_description(description, data.description, data.created_at)
 
 
 @router.delete("/{_id}", response_model=None, status_code=HTTPStatus.NO_CONTENT)
 def delete_subscription_customer_descriptions(_id: UUID) -> None:
     description = db.session.get(SubscriptionCustomerDescriptionTable, _id)
     if description:
         delete(SubscriptionCustomerDescriptionTable, _id)
@@ -56,15 +56,14 @@
     description = db.session.get(SubscriptionCustomerDescriptionTable, _id)
     if description is None:
         raise_status(HTTPStatus.NOT_FOUND)
     return description
 
 
 @router.get("/customer/{customer_id}/subscription/{subscription_id}", response_model=SubscriptionDescriptionSchema)
-def get_subscription_customer_description_by_customer_subscription(customer_id: str, subscription_id: UUID) -> str:
-    stmt = select(SubscriptionCustomerDescriptionTable).filter_by(
-        customer_id=customer_id, subscription_id=subscription_id
-    )
-    description = db.session.scalars(stmt).one_or_none()
+def get_subscription_customer_description_by_customer_subscription(
+    customer_id: str, subscription_id: UUID
+) -> SubscriptionCustomerDescriptionTable:
+    description = get_customer_description_by_customer_subscription(customer_id, subscription_id)
     if description is None:
         raise_status(HTTPStatus.NOT_FOUND)
     return description
```

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/api_v1/endpoints/ws.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/error_handling.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/api/models.py` & `orchestrator_core-2.2.2rc1/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/app.py` & `orchestrator_core-2.2.2rc1/orchestrator/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from orchestrator.db import db, init_database
 from orchestrator.db.database import DBSessionMiddleware
 from orchestrator.distlock import init_distlock_manager
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY, SubscriptionModel
 from orchestrator.exception_handlers import problem_detail_handler
 from orchestrator.graphql import Mutation, Query, create_graphql_router
 from orchestrator.graphql.schemas.subscription import SubscriptionInterface
-from orchestrator.services.processes import ProcessDataBroadcastThread
+from orchestrator.services.process_broadcast_thread import ProcessDataBroadcastThread
 from orchestrator.settings import AppSettings, ExecutorType, app_settings
 from orchestrator.version import GIT_COMMIT_HASH
 from orchestrator.websocket import init_websocket_manager
 from pydantic_forms.exception_handlers.fastapi import form_error_handler
 from pydantic_forms.exceptions import FormException
 
 logger = structlog.get_logger(__name__)
@@ -59,14 +59,15 @@
     AsyncioIntegration(),
     ThreadingIntegration(propagate_hub=True),
 ]
 
 
 class OrchestratorCore(FastAPI):
     graphql_router: Any | None = None
+    broadcast_thread: ProcessDataBroadcastThread | None = None
 
     def __init__(
         self,
         title: str = "The Orchestrator",
         description: str = "The orchestrator is a project that enables users to run workflows.",
         openapi_url: str = "/api/openapi.json",
         docs_url: str = "/api/docs",
@@ -82,15 +83,14 @@
 
         startup_functions: list[Callable] = [distlock_manager.connect_redis]
         shutdown_functions: list[Callable] = [distlock_manager.disconnect_redis]
         if websocket_manager.enabled:
             startup_functions.append(websocket_manager.connect_redis)
             shutdown_functions.extend([websocket_manager.disconnect_all, websocket_manager.disconnect_redis])
 
-        self.broadcast_thread: ProcessDataBroadcastThread | None = None
         if base_settings.EXECUTOR == ExecutorType.THREADPOOL:
             # Only need broadcast thread when using threadpool executor
             self.broadcast_thread = ProcessDataBroadcastThread(websocket_manager)
             startup_functions.append(self.broadcast_thread.start)
             shutdown_functions.append(self.broadcast_thread.stop)
 
         super().__init__(
@@ -185,15 +185,17 @@
     def register_graphql(
         self: "OrchestratorCore",
         query: Any = Query,
         mutation: Any = Mutation,
         register_models: bool = True,
         subscription_interface: Any = SubscriptionInterface,
     ) -> None:
-        new_router = create_graphql_router(query, mutation, register_models, subscription_interface)
+        new_router = create_graphql_router(
+            query, mutation, register_models, subscription_interface, self.broadcast_thread
+        )
         if not self.graphql_router:
             self.graphql_router = new_router
             self.include_router(new_router, prefix="/api/graphql")
         else:
             self.graphql_router.schema = new_router.schema
```

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/database.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generate.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/enums.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/shared_workflows.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/shared_workflows.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/main.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/migration_helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/cli/scheduler.py` & `orchestrator_core-2.2.2rc1/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/config/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/config/assignee.py` & `orchestrator_core-2.2.2rc1/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/database.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/filters.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/process.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/product.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/product_block.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/resource_type.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/search_filters/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/search_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/search_filters/inferred_filter.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/search_filters/inferred_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/subscription.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/filters/workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/filters/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/models.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/range/range.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/sorting/process.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/sorting/product.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/sorting/product_block.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/sorting/resource_type.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/sorting/sorting.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/sorting/subscription.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/db/sorting/workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/devtools/populator.py` & `orchestrator_core-2.2.2rc1/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/devtools/scripts/migrate_20.py` & `orchestrator_core-2.2.2rc1/orchestrator/devtools/scripts/migrate_20.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/distlock/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-2.2.2rc1/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/domain/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/domain/base.py` & `orchestrator_core-2.2.2rc1/orchestrator/domain/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/domain/helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/domain/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/domain/lifecycle.py` & `orchestrator_core-2.2.2rc1/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/exception_handlers.py` & `orchestrator_core-2.2.2rc1/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/forms/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/forms/validators/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/forms/validators/customer_contact_list.py` & `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/customer_contact_list.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/forms/validators/customer_id.py` & `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/customer_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/forms/validators/display_subscription.py` & `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/forms/validators/network_type_validators.py` & `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/forms/validators/product_id.py` & `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/product_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/autoregistration.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/autoregistration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/extensions/error_collector_extension.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/extensions/error_handler_extension.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/error_handler_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/pagination.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/customer.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/product_block.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/resource_type.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/subscription.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/resolvers/workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schema.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections.abc import Callable
 from http import HTTPStatus
-from typing import Any
+from typing import Any, Coroutine
 
 import strawberry
 import structlog
 from fastapi import Depends
 from fastapi.routing import APIRouter
 from graphql import GraphQLError
 from httpx import HTTPStatusError
@@ -26,14 +26,16 @@
 from strawberry.utils.logging import StrawberryLogger
 
 from oauth2_lib.strawberry import authenticated_field
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.graphql.autoregistration import register_domain_models
 from orchestrator.graphql.extensions.deprecation_checker_extension import make_deprecation_checker_extension
 from orchestrator.graphql.extensions.error_handler_extension import ErrorHandlerExtension
+from orchestrator.graphql.mutations.customer_description import CustomerSubscriptionDescriptionMutation
+from orchestrator.graphql.mutations.start_process import ProcessMutation
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.resolvers import (
     SettingsMutation,
     resolve_customer,
     resolve_processes,
     resolve_product_blocks,
     resolve_products,
@@ -50,14 +52,15 @@
 from orchestrator.graphql.schemas.product_block import ProductBlock
 from orchestrator.graphql.schemas.resource_type import ResourceType
 from orchestrator.graphql.schemas.settings import StatusType
 from orchestrator.graphql.schemas.subscription import SubscriptionInterface, federation_key_directives
 from orchestrator.graphql.schemas.workflow import Workflow
 from orchestrator.graphql.types import SCALAR_OVERRIDES, OrchestratorContext
 from orchestrator.security import get_oidc_user, get_opa_security_graphql
+from orchestrator.services.process_broadcast_thread import ProcessDataBroadcastThread
 from orchestrator.settings import app_settings
 
 api_router = APIRouter()
 
 logger = structlog.get_logger(__name__)
 
 
@@ -89,15 +92,15 @@
         description="Returns information about cache, workers, and global engine settings",
     )
     customers: Connection[CustomerType] = authenticated_field(
         resolver=resolve_customer, description="Returns default customer information"
     )
 
 
-Mutation = merge_types("Mutation", (SettingsMutation,))
+Mutation = merge_types("Mutation", (SettingsMutation, CustomerSubscriptionDescriptionMutation, ProcessMutation))
 
 OrchestratorGraphqlRouter = GraphQLRouter
 
 
 class OrchestratorSchema(strawberry.federation.Schema):
     def process_errors(
         self,
@@ -122,26 +125,35 @@
 def custom_context_dependency(
     get_current_user: Callable = Depends(get_oidc_user),  # noqa: B008
     get_opa_decision: Callable = Depends(get_opa_security_graphql),  # noqa: B008
 ) -> OrchestratorContext:
     return OrchestratorContext(get_current_user=get_current_user, get_opa_decision=get_opa_decision)
 
 
-async def get_context(custom_context=Depends(custom_context_dependency)) -> OrchestratorContext:  # type: ignore # noqa: B008
-    return custom_context
+def get_context(
+    broadcast_thread: ProcessDataBroadcastThread | None = None,
+) -> Callable[[OrchestratorContext], Coroutine[Any, Any, OrchestratorContext]]:
+    async def _get_context(
+        custom_context: OrchestratorContext = Depends(custom_context_dependency),  # noqa: B008
+    ) -> OrchestratorContext:
+        custom_context.broadcast_thread = broadcast_thread
+        return custom_context
+
+    return _get_context
 
 
 GRAPHQL_MODELS_INITIAL = dict(GRAPHQL_MODELS)
 
 
 def create_graphql_router(
     query: Any = Query,
     mutation: Any = Mutation,
     register_models: bool = True,
     subscription_interface: type | None = SubscriptionInterface,
+    broadcast_thread: ProcessDataBroadcastThread | None = None,
 ) -> OrchestratorGraphqlRouter:
     @strawberry.experimental.pydantic.type(
         model=SubscriptionModel, all_fields=True, directives=federation_key_directives
     )
     class Subscription(SubscriptionInterface):
         pass
 
@@ -157,11 +169,13 @@
         mutation=mutation,
         enable_federation_2=app_settings.FEDERATION_ENABLED,
         types=tuple(models.values()),
         extensions=[ErrorHandlerExtension, make_deprecation_checker_extension(query=query)],
         scalar_overrides=SCALAR_OVERRIDES,
     )
 
-    return OrchestratorGraphqlRouter(schema, context_getter=get_context, graphiql=app_settings.SERVE_GRAPHQL_UI)
+    return OrchestratorGraphqlRouter(
+        schema, context_getter=get_context(broadcast_thread), graphiql=app_settings.SERVE_GRAPHQL_UI
+    )
 
 
 graphql_router = create_graphql_router()
```

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/process.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/product.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/product_block.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/resource_type.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/subscription.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,40 +10,35 @@
 
 from oauth2_lib.strawberry import authenticated_field
 from orchestrator.db import FixedInputTable, ProductTable, SubscriptionTable, db
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY
 from orchestrator.graphql.pagination import EMPTY_PAGE, Connection
 from orchestrator.graphql.resolvers.process import resolve_processes
 from orchestrator.graphql.schemas.customer import CustomerType
+from orchestrator.graphql.schemas.customer_description import CustomerDescription
 from orchestrator.graphql.schemas.process import ProcessType
 from orchestrator.graphql.schemas.product import ProductModelGraphql
 from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
 from orchestrator.graphql.utils.get_subscription_product_blocks import (
     ProductBlockInstance,
     get_subscription_product_blocks,
 )
-from orchestrator.schemas import SubscriptionDescriptionBaseSchema
 from orchestrator.services.fixed_inputs import get_fixed_inputs
 from orchestrator.services.subscriptions import (
     get_subscription_metadata,
 )
 from orchestrator.settings import app_settings
 from orchestrator.types import SubscriptionLifecycle
 
 federation_key_directives = [Key(fields="subscriptionId", resolvable=UNSET)]
 
 MetadataDict: dict[str, type[BaseModel] | None] = {"metadata": None}
 static_metadata_schema = {"title": "SubscriptionMetadata", "type": "object", "properties": {}, "definitions": {}}
 
 
-@strawberry.experimental.pydantic.type(model=SubscriptionDescriptionBaseSchema, all_fields=True)
-class CustomerDescription:
-    pass
-
-
 @strawberry.federation.interface(description="Virtual base interface for subscriptions", keys=["subscriptionId"])
 class SubscriptionInterface:
     subscription_id: UUID
     customer_id: str
     product: ProductModelGraphql
     description: str
     start_date: datetime | None
```

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/schemas/workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/utils/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/utils/create_resolver_error_handler.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/create_resolver_error_handler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/utils/get_subscription_product_blocks.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/get_subscription_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/utils/is_query_detailed.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/utils/override_class.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/graphql/utils/to_graphql_result_page.py` & `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/to_graphql_result_page.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/alembic.ini` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/env.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py` & `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schedules/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-2.2.2rc1/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schedules/scheduling.py` & `orchestrator_core-2.2.2rc1/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-2.2.2rc1/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schedules/validate_products.py` & `orchestrator_core-2.2.2rc1/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-2.2.2rc1/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/base.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/engine_settings.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/fixed_input.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/problem_detail.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/process.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/product.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/product_block.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/resource_type.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/subscription.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/schemas/workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/security.py` & `orchestrator_core-2.2.2rc1/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/celery.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/fixed_inputs.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/processes.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/processes.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,23 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import asyncio
-import queue
-import threading
 from collections.abc import Callable, Sequence
 from concurrent.futures.thread import ThreadPoolExecutor
 from functools import partial
 from http import HTTPStatus
 from typing import Any
 from uuid import UUID, uuid4
 
 import structlog
 from deepmerge import Merger
-from fastapi import Request
 from sqlalchemy import select
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.orm import joinedload
 
 from nwastdlib.ex import show_ex
 from orchestrator.api.error_handling import raise_status
 from orchestrator.config.assignee import Assignee
@@ -43,20 +39,18 @@
 from orchestrator.services.workflows import get_workflow_by_name
 from orchestrator.settings import ExecutorType, app_settings
 from orchestrator.targets import Target
 from orchestrator.types import BroadcastFunc, State
 from orchestrator.utils.datetime import nowtz
 from orchestrator.utils.errors import error_state_to_dict
 from orchestrator.websocket import (
-    WS_CHANNELS,
     create_process_websocket_data,
     send_process_data_to_websocket,
     websocket_manager,
 )
-from orchestrator.websocket.websocket_manager import WebSocketManager
 from orchestrator.workflow import (
     CALLBACK_TOKEN_KEY,
     Failed,
     ProcessStat,
     ProcessStatus,
     Step,
     StepList,
@@ -759,68 +753,14 @@
     except ValueError:
         logger.exception("Encountered an anomaly, locking the engine; manual intervention necessary to fix")
         engine_settings.global_lock = True
         db.session.commit()
         return None
 
 
-class ProcessDataBroadcastThread(threading.Thread):
-    def __init__(self, _websocket_manager: WebSocketManager, *args, **kwargs) -> None:  # type: ignore
-        super().__init__(*args, **kwargs)
-        self.shutdown = False
-        self.queue: queue.Queue = queue.Queue()
-        self.websocket_manager = _websocket_manager
-
-    def run(self) -> None:
-        logger.info("Starting ProcessDataBroadcastThread")
-        try:
-            loop = asyncio.new_event_loop()  # Create an eventloop specifically for this thread
-
-            while not self.shutdown:
-                try:
-                    process_id, data = self.queue.get(block=True, timeout=1)
-                except queue.Empty:
-                    continue
-                logger.debug(
-                    "Threadsafe broadcast data through websocket manager",
-                    process_id=process_id,
-                    where="ProcessDataBroadcastThread",
-                    channels=WS_CHANNELS.ALL_PROCESSES,
-                )
-                loop.run_until_complete(self.websocket_manager.broadcast_data([WS_CHANNELS.ALL_PROCESSES], data))
-
-            loop.close()
-            logger.info("Shutdown ProcessDataBroadcastThread")
-        except Exception:
-            logger.exception("Unhandled exception in ProcessDataBroadcastThread, exiting")
-
-    def stop(self) -> None:
-        logger.debug("Sending shutdown signal to ProcessDataBroadcastThread")
-        self.shutdown = True
-        self.join(timeout=5)
-        self.is_alive()
-
-
-def api_broadcast_process_data(request: Request) -> BroadcastFunc | None:
-    """Given a FastAPI request, creates a threadsafe callable for broadcasting process data.
-
-    The callable should be created in API endpoints and provided to start_process,
-    resume_process, etc. through the `broadcast_func` param.
-    """
-    if not request.app.broadcast_thread:
-        return None
-
-    broadcast_queue: queue.Queue = request.app.broadcast_thread.queue
-
-    def _queue_put(process_id: UUID, data: dict) -> None:
-        broadcast_queue.put((str(process_id), data))
-
-    return _queue_put
-
-
 class ThreadPoolWorkerStatus(WorkerStatus):
     def __init__(self) -> None:
         super().__init__(executor_type="threadpool")
         thread_pool = get_thread_pool()
         self.number_of_workers_online = getattr(thread_pool, "_max_workers", -1)
         self.number_of_queued_jobs = thread_pool._work_queue.qsize() if hasattr(thread_pool, "_work_queue") else 0
         self.number_of_running_jobs = len(getattr(thread_pool, "_threads", []))
```

### Comparing `orchestrator_core-2.2.1/orchestrator/services/products.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/resource_types.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/settings.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/subscriptions.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/tasks.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/translations.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/services/workflows.py` & `orchestrator_core-2.2.2rc1/orchestrator/services/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/settings.py` & `orchestrator_core-2.2.2rc1/orchestrator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/targets.py` & `orchestrator_core-2.2.2rc1/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/types.py` & `orchestrator_core-2.2.2rc1/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/crypt.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/datetime.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/deprecation_logger.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/deprecation_logger.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/docs.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/enrich_process.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/enrich_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/errors.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/fixed_inputs.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/functional.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/get_updated_properties.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/helpers.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/json.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/redis.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/redis.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import functools
 from collections.abc import AsyncGenerator
 from contextlib import asynccontextmanager
 from os import getenv
-from typing import Any
+from typing import Any, Callable
 from uuid import UUID
 
 from redis import Redis
 from redis.asyncio import Redis as AIORedis
 from redis.asyncio.client import Pipeline, PubSub
 from structlog import get_logger
 
@@ -66,14 +67,38 @@
         logger.info("Deleting subscription object from cache", subscription_id=subscription_id)
         cache.delete(f"domain:{subscription_id}")
         cache.delete(f"domain:etag:{subscription_id}")
     else:
         logger.warning("Caching disabled, not deleting subscription", subscription=subscription_id)
 
 
+def default_get_subscription_id(data: Any) -> UUID:
+    if hasattr(data, "subscription_id"):
+        return data.subscription_id
+    if isinstance(data, dict):
+        return data["subscription_id"]
+    return data
+
+
+def delete_subscription_from_redis(
+    extract_fn: Callable[..., UUID] = default_get_subscription_id
+) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
+    def _delete_subscription_from_redis(func: Callable[..., Any]) -> Callable[..., Any]:
+        @functools.wraps(func)
+        def wrapper(*args: tuple, **kwargs: dict[str, Any]) -> Any:
+            data = func(*args, **kwargs)
+            key = extract_fn(data)
+            delete_from_redis(key)
+            return data
+
+        return wrapper
+
+    return _delete_subscription_from_redis
+
+
 async def delete_keys_matching_pattern(_cache: AIORedis, pattern: str, chunksize: int = 5000) -> int:
     """Delete all keys matching the given pattern.
 
     Usage:
         >>> await delete_keys_matching_pattern("orchestrator:foo:*")  # doctest:+SKIP
     """
     deleted = 0
```

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/search_query.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/search_query.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/state.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/utils/strings.py` & `orchestrator_core-2.2.2rc1/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/version.py` & `orchestrator_core-2.2.2rc1/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/websocket/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-2.2.2rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-2.2.2rc1/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-2.2.2rc1/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/modify_note.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/steps.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/orchestrator/workflows/utils.py` & `orchestrator_core-2.2.2rc1/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/pyproject.toml` & `orchestrator_core-2.2.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/setup.cfg` & `orchestrator_core-2.2.2rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/setup.py` & `orchestrator_core-2.2.2rc1/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/acceptance_tests/conftest.py` & `orchestrator_core-2.2.2rc1/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/acceptance_tests/test_test_product.py` & `orchestrator_core-2.2.2rc1/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_caching.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_health.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_helpers.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_models.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_processes.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_products.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_settings.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,25 +66,25 @@
 
 
 def test_update(seed, test_client):
     new_desc = "Updated specific alias"
     body = {
         "id": SUBSCRIPTION_CUSTOMER_DESCRIPTION_ID,
         "subscription_id": SUBSCRIPTION_ID,
-        "customer_id": str(uuid4()),
+        "customer_id": CUSTOMER_ID,
         "description": new_desc,
     }
     response = test_client.put("/api/subscription_customer_descriptions/", json=body)
     assert HTTPStatus.NO_CONTENT == response.status_code
 
     count = db.session.query(SubscriptionCustomerDescriptionTable).count()
     assert 1 == count
 
-    res = db.session.query(SubscriptionCustomerDescriptionTable).first()
-    assert new_desc == res.description
+    customer_description = db.session.query(SubscriptionCustomerDescriptionTable).first()
+    assert new_desc == customer_description.description
 
 
 def test_delete(seed, test_client):
     test_client.delete(f"/api/subscription_customer_descriptions/{SUBSCRIPTION_CUSTOMER_DESCRIPTION_ID}")
 
     count = db.session.query(SubscriptionCustomerDescriptionTable).count()
     assert 0 == count
```

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_workflows.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/api/test_ws.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate.sh` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate.sh`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/alembic.ini` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/env.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_types/example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/products/product_types/example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/__init__.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/generate/workflows/shared.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/product_config1.yaml` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config1.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/product_config2.yaml` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config2.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/data/product_config3.yaml` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config3.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/generator/test_enums.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/generator/test_enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/test_cli_generate.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_cli_generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/test_generate_code.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_generate_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/conftest.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/domain/test_base.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/domain/test_lifecycle.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/processes.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/forms/test_customer_contact_list.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_customer_contact_list.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/forms/test_display_subscription.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/conftest.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_customer.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_product.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_product_blocks.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_resource_types.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_sort_and_filter_fields.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_sort_and_filter_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_subscription.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_subscriptions.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/test_workflows.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/utils/test_autoregistration.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_autoregistration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/utils/test_is_query_detailed.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/utils/test_is_querying_page_data.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_is_querying_page_data.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/graphql/utils/test_override_class.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/helpers.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/services/test_processes.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/services/test_products.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/services/test_translations.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/test_db.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/test_workflow.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/utils/test_errors.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/utils/test_functional.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/utils/test_get_updated_properties.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/utils/test_json.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/utils/test_search_query.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_search_query.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/utils/test_state.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/websocket/test_broadcast.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/websocket/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/workflows/__init__.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/workflows/test_async_workflow.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_async_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.1/PKG-INFO` & `orchestrator_core-2.2.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 2.2.1
+Version: 2.2.2rc1
 Summary: This is the orchestrator workflow engine.
 Requires-Python: >=3.11,<3.13
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
```

