# Comparing `tmp/ecs_composex-1.1.0rc2.tar.gz` & `tmp/ecs_composex-1.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_composex-1.1.0rc2.tar", max compression
+gzip compressed data, was "ecs_composex-1.1.0rc3.tar", max compression
```

## Comparing `ecs_composex-1.1.0rc2.tar` & `ecs_composex-1.1.0rc3.tar`

### file list

```diff
@@ -1,370 +1,370 @@
--rw-r--r--   0        0        0    16725 2021-05-14 10:51:20.077071 ecs_composex-1.1.0rc2/LICENSE
--rw-r--r--   0        0        0      385 2022-06-16 18:49:16.792466 ecs_composex-1.1.0rc2/MANIFEST.in
--rw-r--r--   0        0        0     1068 2023-08-07 12:54:52.746417 ecs_composex-1.1.0rc2/NOTICES.rst
--rw-r--r--   0        0        0     6976 2023-01-11 09:54:17.357527 ecs_composex-1.1.0rc2/README.rst
--rw-r--r--   0        0        0       19 2021-03-04 09:40:13.458136 ecs_composex-1.1.0rc2/ecs_composex/.gitignore
--rw-r--r--   0        0        0      222 2024-04-14 21:59:40.442106 ecs_composex-1.1.0rc2/ecs_composex/__init__.py
--rw-r--r--   0        0        0      117 2024-03-23 20:44:00.309060 ecs_composex-1.1.0rc2/ecs_composex/acm/__init__.py
--rw-r--r--   0        0        0      419 2024-03-23 20:44:00.401059 ecs_composex-1.1.0rc2/ecs_composex/acm/acm_module.py
--rw-r--r--   0        0        0     1546 2024-03-23 20:44:00.178062 ecs_composex-1.1.0rc2/ecs_composex/acm/acm_params.py
--rw-r--r--   0        0        0     5773 2024-03-23 20:44:00.185062 ecs_composex-1.1.0rc2/ecs_composex/acm/acm_stack.py
--rw-r--r--   0        0        0     7634 2024-03-23 20:44:00.125063 ecs_composex-1.1.0rc2/ecs_composex/acm/acm_stack_helpers.py
--rw-r--r--   0        0        0     1327 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/acm/x-acm.spec.json
--rw-r--r--   0        0        0      416 2024-03-23 20:44:00.390059 ecs_composex-1.1.0rc2/ecs_composex/alarms/__init__.py
--rw-r--r--   0        0        0     9162 2024-03-23 20:44:00.121063 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_ecs.py
--rw-r--r--   0        0        0     6292 2024-03-23 20:44:00.005065 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_elbv2.py
--rw-r--r--   0        0        0     8575 2024-03-23 20:43:59.927066 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_helpers.py
--rw-r--r--   0        0        0      416 2024-03-23 20:44:00.139063 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_module.py
--rw-r--r--   0        0        0      532 2024-03-23 20:44:00.388059 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_params.py
--rw-r--r--   0        0        0     4520 2024-03-23 20:43:59.894066 ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_stack.py
--rw-r--r--   0        0        0     1920 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/alarms/x-alarms.spec.json
--rw-r--r--   0        0        0       44 2022-06-16 18:49:16.909464 ecs_composex-1.1.0rc2/ecs_composex/appmesh/README.rst
--rw-r--r--   0        0        0      288 2024-03-23 20:44:00.220061 ecs_composex-1.1.0rc2/ecs_composex/appmesh/__init__.py
--rw-r--r--   0        0        0     2268 2024-03-23 20:43:59.826068 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_aws.py
--rw-r--r--   0        0        0     1479 2024-03-23 20:44:00.369059 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_conditions.py
--rw-r--r--   0        0        0     9620 2024-03-23 20:44:00.022064 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_mesh.py
--rw-r--r--   0        0        0    12953 2024-03-23 20:44:00.203061 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_node.py
--rw-r--r--   0        0        0     1222 2024-03-23 20:43:59.819068 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_params.py
--rw-r--r--   0        0        0    10944 2024-03-23 20:44:00.127063 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_router.py
--rw-r--r--   0        0        0     6917 2024-03-23 20:44:00.367059 ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_service.py
--rw-r--r--   0        0        0     4576 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/appmesh/x-appmesh.spec.json
--rw-r--r--   0        0        0      121 2024-03-23 20:43:59.931066 ecs_composex-1.1.0rc2/ecs_composex/aps/__init__.py
--rw-r--r--   0        0        0      501 2024-03-23 20:44:00.240061 ecs_composex-1.1.0rc2/ecs_composex/aps/aps_module.py
--rw-r--r--   0        0        0      938 2024-03-23 20:44:00.136062 ecs_composex-1.1.0rc2/ecs_composex/aps/aps_parameters.py
--rw-r--r--   0        0        0      492 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/aps/aps_perms.json
--rw-r--r--   0        0        0     7896 2024-03-23 20:44:00.467057 ecs_composex-1.1.0rc2/ecs_composex/aps/aps_stack.py
--rw-r--r--   0        0        0     1219 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/aps/x-aps.spec.json
--rw-r--r--   0        0        0     6802 2024-03-23 20:44:00.151062 ecs_composex-1.1.0rc2/ecs_composex/cli.py
--rw-r--r--   0        0        0      481 2024-03-23 20:44:00.271061 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/__init__.py
--rw-r--r--   0        0        0     7347 2024-03-23 20:44:00.090063 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_ecs.py
--rw-r--r--   0        0        0     5364 2024-03-23 20:43:59.853067 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_helpers.py
--rw-r--r--   0        0        0      481 2024-03-23 20:43:59.986065 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_module.py
--rw-r--r--   0        0        0     2100 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_params.py
--rw-r--r--   0        0        0    12308 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_stack.py
--rw-r--r--   0        0        0     7790 2024-03-23 20:43:59.886067 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_x_resources.py
--rw-r--r--   0        0        0     1486 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/cloudmap/x-cloudmap.spec.json
--rw-r--r--   0        0        0      500 2024-03-23 20:44:00.107063 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/__init__.py
--rw-r--r--   0        0        0     1761 2024-03-23 20:44:00.321060 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_aws.py
--rw-r--r--   0        0        0      500 2024-03-23 20:44:00.359059 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_module.py
--rw-r--r--   0        0        0      603 2024-03-23 20:44:00.419058 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_params.py
--rw-r--r--   0        0        0      188 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_perms.json
--rw-r--r--   0        0        0     5053 2024-03-23 20:43:59.897066 ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_stack.py
--rw-r--r--   0        0        0      489 2024-03-23 20:44:00.009065 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/__init__.py
--rw-r--r--   0        0        0      909 2024-03-23 20:43:59.840067 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_params.py
--rw-r--r--   0        0        0      489 2024-03-23 20:43:59.828067 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_userpool_module.py
--rw-r--r--   0        0        0     4821 2024-03-23 20:43:59.961065 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_userpool_stack.py
--rw-r--r--   0        0        0      375 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/x-cognito_userpool.spec.json
--rw-r--r--   0        0        0     2314 2024-03-23 20:44:00.088063 ecs_composex-1.1.0rc2/ecs_composex/common/__init__.py
--rw-r--r--   0        0        0    13821 2024-03-23 20:43:59.947065 ecs_composex-1.1.0rc2/ecs_composex/common/aws.py
--rw-r--r--   0        0        0     1209 2024-03-23 20:44:00.432058 ecs_composex-1.1.0rc2/ecs_composex/common/cfn_conditions.py
--rw-r--r--   0        0        0     1258 2024-03-23 20:43:59.901066 ecs_composex-1.1.0rc2/ecs_composex/common/cfn_params.py
--rw-r--r--   0        0        0      408 2024-03-23 20:44:00.103063 ecs_composex-1.1.0rc2/ecs_composex/common/ecs_composex.py
--rw-r--r--   0        0        0     1465 2024-03-23 22:36:48.972815 ecs_composex-1.1.0rc2/ecs_composex/common/envsubst.py
--rw-r--r--   0        0        0     9180 2024-03-23 20:43:59.971065 ecs_composex-1.1.0rc2/ecs_composex/common/files.py
--rw-r--r--   0        0        0     1937 2024-03-23 20:43:59.921066 ecs_composex-1.1.0rc2/ecs_composex/common/logging.py
--rw-r--r--   0        0        0    24735 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc2/ecs_composex/common/settings.py
--rw-r--r--   0        0        0    14081 2024-03-23 20:44:00.463057 ecs_composex-1.1.0rc2/ecs_composex/common/stacks/__init__.py
--rw-r--r--   0        0        0     8705 2024-03-23 20:44:00.333059 ecs_composex-1.1.0rc2/ecs_composex/common/tagging.py
--rw-r--r--   0        0        0    10189 2024-03-23 20:43:59.845067 ecs_composex-1.1.0rc2/ecs_composex/common/troposphere_tools.py
--rw-r--r--   0        0        0       90 2024-03-23 20:44:00.277060 ecs_composex-1.1.0rc2/ecs_composex/compose/__init__.py
--rw-r--r--   0        0        0     1629 2024-03-23 20:44:00.131063 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_networks.py
--rw-r--r--   0        0        0     9238 2024-03-23 20:44:00.042064 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/__init__.py
--rw-r--r--   0        0        0     3632 2024-03-23 20:44:00.229061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/ecs_family_helpers.py
--rw-r--r--   0        0        0     1490 2024-03-23 20:44:00.222061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/helpers.py
--rw-r--r--   0        0        0     1292 2024-03-23 20:44:00.227061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/services_helpers.py
--rw-r--r--   0        0        0    37531 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/__init__.py
--rw-r--r--   0        0        0     6697 2024-03-23 20:43:59.903066 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/docker_tools.py
--rw-r--r--   0        0        0     3399 2024-03-23 20:44:00.001065 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/env_files_helpers.py
--rw-r--r--   0        0        0     9848 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/helpers.py
--rw-r--r--   0        0        0     3658 2024-03-23 20:44:00.275061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/kernel_options_helpers.py
--rw-r--r--   0        0        0     8042 2024-03-23 20:44:00.129063 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/__init__.py
--rw-r--r--   0        0        0     2719 2024-03-23 20:44:00.375059 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/docker_opts.py
--rw-r--r--   0        0        0     3911 2024-03-23 20:43:59.892066 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/ecr_helpers.py
--rw-r--r--   0        0        0    10829 2024-03-23 20:44:00.167062 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/ecr_scans_eval.py
--rw-r--r--   0        0        0     5119 2024-03-23 20:44:00.261061 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_logging/__init__.py
--rw-r--r--   0        0        0     5036 2024-03-23 20:43:59.855067 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_logging/helpers.py
--rw-r--r--   0        0        0     3873 2024-03-23 20:43:59.983065 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/__init__.py
--rw-r--r--   0        0        0     6846 2024-03-23 20:44:00.069064 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/ecs_family_helpers.py
--rw-r--r--   0        0        0     1459 2024-03-23 20:44:00.331060 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/helpers.py
--rw-r--r--   0        0        0     5651 2024-03-23 20:44:00.096063 ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/services_helpers.py
--rw-r--r--   0        0        0    30750 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/__init__.py
--rw-r--r--   0        0        0     1672 2024-03-23 20:43:59.911066 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/api_x_resources.py
--rw-r--r--   0        0        0      922 2024-03-23 20:44:00.461058 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/environment_x_resources.py
--rw-r--r--   0        0        0     4657 2024-03-23 20:44:00.123063 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/helpers.py
--rw-r--r--   0        0        0     6435 2024-03-23 20:44:00.048064 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/network_x_resources.py
--rw-r--r--   0        0        0     8806 2024-03-23 20:43:59.838067 ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/services_resources.py
--rw-r--r--   0        0        0       90 2024-03-23 20:44:00.017064 ecs_composex-1.1.0rc2/ecs_composex/dashboards/__init__.py
--rw-r--r--   0        0        0      472 2024-03-23 20:43:59.842067 ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_module.py
--rw-r--r--   0        0        0     5539 2024-03-23 20:44:00.329059 ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_services_metrics.py
--rw-r--r--   0        0        0     4831 2024-03-23 20:44:00.035064 ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_stack.py
--rw-r--r--   0        0        0     1224 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/dashboards/x-dashboards.spec.json
--rw-r--r--   0        0        0      413 2024-03-23 20:44:00.259061 ecs_composex-1.1.0rc2/ecs_composex/docdb/__init__.py
--rw-r--r--   0        0        0      413 2024-03-23 20:43:59.915066 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_module.py
--rw-r--r--   0        0        0      833 2024-03-23 20:44:00.346059 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_params.py
--rw-r--r--   0        0        0      164 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_perms.json
--rw-r--r--   0        0        0     7772 2024-03-23 20:43:59.876067 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_stack.py
--rw-r--r--   0        0        0     6450 2024-03-23 20:44:00.063064 ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_template.py
--rw-r--r--   0        0        0     2241 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/docdb/x-docdb.spec.json
--rw-r--r--   0        0        0      289 2024-03-23 20:44:00.046064 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/__init__.py
--rw-r--r--   0        0        0     7795 2024-03-23 20:44:00.248061 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_autoscaling.py
--rw-r--r--   0        0        0      422 2024-03-23 20:44:00.117063 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_module.py
--rw-r--r--   0        0        0      412 2024-03-23 20:43:59.966065 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_params.py
--rw-r--r--   0        0        0     1096 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_perms.json
--rw-r--r--   0        0        0     4131 2024-03-23 20:44:00.355059 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_stack.py
--rw-r--r--   0        0        0     2916 2024-03-23 20:44:00.075064 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_template.py
--rw-r--r--   0        0        0     2777 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/dynamodb/x-dynamodb.spec.json
--rw-r--r--   0        0        0     1050 2024-03-23 20:44:00.094063 ecs_composex-1.1.0rc2/ecs_composex/ecs/__init__.py
--rw-r--r--   0        0        0     3532 2024-03-23 20:43:59.955065 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_conditions.py
--rw-r--r--   0        0        0    27604 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/__init__.py
--rw-r--r--   0        0        0    14849 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/__init__.py
--rw-r--r--   0        0        0     1316 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/compute_finalizers.py
--rw-r--r--   0        0        0     1912 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/network_finalizers.py
--rw-r--r--   0        0        0     8788 2024-03-23 20:43:59.870067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_logging/__init__.py
--rw-r--r--   0        0        0     4123 2024-03-23 20:44:00.061064 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_logging/cw_logging.py
--rw-r--r--   0        0        0     2940 2024-03-23 20:43:59.880066 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_template.py
--rw-r--r--   0        0        0     3502 2024-03-23 20:43:59.861067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/task_execute_command.py
--rw-r--r--   0        0        0     2626 2024-03-23 20:44:00.015065 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/task_runtime.py
--rw-r--r--   0        0        0      163 2024-03-23 20:44:00.381059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/__init__.py
--rw-r--r--   0        0        0    10598 2024-03-23 20:43:59.949066 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/__init__.py
--rw-r--r--   0        0        0     5822 2024-03-23 20:44:00.098063 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_firehose.py
--rw-r--r--   0        0        0     5548 2024-03-23 20:44:00.282060 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_kinesis.py
--rw-r--r--   0        0        0     3067 2024-03-23 20:43:59.882067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/config_parameter.py
--rw-r--r--   0        0        0      609 2023-08-07 12:54:52.748417 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/family_fluentbit_managed_config.j2
--rw-r--r--   0        0        0     3408 2024-03-23 20:44:00.451058 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/firelens_config_sidecar.py
--rw-r--r--   0        0        0      613 2023-08-07 12:54:52.748417 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/service_fluentbit_managed_config.j2
--rw-r--r--   0        0        0     3807 2024-03-23 20:44:00.225061 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_advanced_rendered_settings.py
--rw-r--r--   0        0        0     5267 2024-03-23 20:44:00.363059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_logger_helpers.py
--rw-r--r--   0        0        0     6883 2024-03-23 20:44:00.348059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_managed_sidecar_service.py
--rw-r--r--   0        0        0     2548 2024-03-23 20:44:00.323060 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_options_generic_helpers.py
--rw-r--r--   0        0        0      161 2024-03-23 20:43:59.909066 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/__init__.py
--rw-r--r--   0        0        0     2293 2024-03-23 20:44:00.340059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/cloudwatch_helpers.py
--rw-r--r--   0        0        0     3812 2024-03-23 20:44:00.511057 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/firehose_helpers.py
--rw-r--r--   0        0        0     3561 2024-03-23 20:44:00.353059 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/kinesis_helpers.py
--rw-r--r--   0        0        0     5752 2024-03-23 20:44:00.425058 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_params.py
--rw-r--r--   0        0        0     4482 2024-03-23 20:44:00.092063 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/__init__.py
--rw-r--r--   0        0        0     4829 2024-03-23 20:44:00.211061 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/config_ssm_parameters.py
--rw-r--r--   0        0        0     9763 2024-03-23 20:43:59.990065 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/emf_processors.py
--rw-r--r--   0        0        0     6413 2024-03-23 20:43:59.860067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/helpers.py
--rw-r--r--   0        0        0     3525 2024-03-23 20:43:59.866067 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_service/__init__.py
--rw-r--r--   0        0        0     4688 2024-03-23 20:44:00.067064 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_service/helpers.py
--rw-r--r--   0        0        0     5588 2024-03-30 09:27:30.584324 ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_stack.py
--rw-r--r--   0        0        0     1927 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc2/ecs_composex/ecs/helpers/__init__.py
--rw-r--r--   0        0        0     2857 2024-03-23 20:44:00.159062 ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/__init__.py
--rw-r--r--   0        0        0     1414 2024-03-23 20:44:00.284060 ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/aws_cw_agent.py
--rw-r--r--   0        0        0     2805 2024-03-23 20:44:00.200062 ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/aws_xray.py
--rw-r--r--   0        0        0      960 2024-03-23 20:43:59.874067 ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/nginx_prometheus_exporter.py
--rw-r--r--   0        0        0     6182 2024-03-23 20:43:59.907066 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_alarms/__init__.py
--rw-r--r--   0        0        0     3158 2024-03-23 20:44:00.434058 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_alarms/service_predefined_alarms.py
--rw-r--r--   0        0        0     5545 2024-03-23 20:44:00.361059 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_compute/__init__.py
--rw-r--r--   0        0        0     1861 2024-03-23 20:44:00.379059 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_compute/helpers.py
--rw-r--r--   0        0        0    10734 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/helpers.py
--rw-r--r--   0        0        0    15293 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/ingress_helpers.py
--rw-r--r--   0        0        0     9051 2024-03-23 20:44:00.059064 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_scaling/__init__.py
--rw-r--r--   0        0        0    12114 2024-03-23 20:44:00.386059 ecs_composex-1.1.0rc2/ecs_composex/ecs/service_scaling/helpers.py
--rw-r--r--   0        0        0     5012 2024-03-23 20:44:00.206061 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_compute/__init__.py
--rw-r--r--   0        0        0     3831 2024-03-23 20:43:59.847067 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_compute/helpers.py
--rw-r--r--   0        0        0     5414 2024-03-23 20:43:59.884066 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/__init__.py
--rw-r--r--   0        0        0     2208 2024-03-23 20:43:59.943066 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/helpers.py
--rw-r--r--   0        0        0     7042 2024-03-23 20:44:00.056064 ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/task_role.py
--rw-r--r--   0        0        0    20480 2024-03-23 20:44:00.078064 ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/__init__.py
--rw-r--r--   0        0        0      509 2024-03-23 20:44:00.267061 ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/ecs_cluster_params.py
--rw-r--r--   0        0        0     7216 2024-03-23 20:44:00.029064 ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/ecs_family_helpers.py
--rw-r--r--   0        0        0     3504 2024-03-23 20:44:00.101063 ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/helpers.py
--rw-r--r--   0        0        0    12357 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc2/ecs_composex/ecs_composex.py
--rw-r--r--   0        0        0      326 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc2/ecs_composex/ecs_ingress/__init__.py
--rw-r--r--   0        0        0     3409 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc2/ecs_composex/ecs_ingress/ecs_ingress_stack.py
--rw-r--r--   0        0        0      125 2024-03-23 20:44:00.396058 ecs_composex-1.1.0rc2/ecs_composex/efs/__init__.py
--rw-r--r--   0        0        0    12388 2024-03-23 20:44:00.054064 ecs_composex-1.1.0rc2/ecs_composex/efs/efs_ecs.py
--rw-r--r--   0        0        0      403 2024-03-23 20:44:00.286060 ecs_composex-1.1.0rc2/ecs_composex/efs/efs_module.py
--rw-r--r--   0        0        0     1139 2024-03-23 20:44:00.172062 ecs_composex-1.1.0rc2/ecs_composex/efs/efs_params.py
--rw-r--r--   0        0        0     7434 2024-03-23 20:43:59.832067 ecs_composex-1.1.0rc2/ecs_composex/efs/efs_stack.py
--rw-r--r--   0        0        0     1026 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/efs/x-efs.spec.json
--rw-r--r--   0        0        0      482 2024-03-23 20:43:59.933066 ecs_composex-1.1.0rc2/ecs_composex/elasticache/__init__.py
--rw-r--r--   0        0        0     5725 2024-03-23 20:44:00.505057 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_aws.py
--rw-r--r--   0        0        0     3106 2024-03-23 20:44:00.427058 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_ecs.py
--rw-r--r--   0        0        0      482 2024-03-23 20:44:00.342059 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_module.py
--rw-r--r--   0        0        0     2926 2024-03-23 20:43:59.929066 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_params.py
--rw-r--r--   0        0        0     8927 2024-03-23 20:44:00.040064 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_stack.py
--rw-r--r--   0        0        0     8942 2024-03-23 20:44:00.156062 ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_template.py
--rw-r--r--   0        0        0      413 2024-03-23 20:44:00.507057 ecs_composex-1.1.0rc2/ecs_composex/elbv2/__init__.py
--rw-r--r--   0        0        0    27727 2024-03-23 20:44:00.231061 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_ecs.py
--rw-r--r--   0        0        0      413 2024-03-23 20:43:59.899066 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_module.py
--rw-r--r--   0        0        0     2143 2024-03-23 20:43:59.945066 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_params.py
--rw-r--r--   0        0        0     2957 2024-04-03 16:23:37.606364 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/__init__.py
--rw-r--r--   0        0        0    22478 2024-03-23 20:44:00.082064 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2.py
--rw-r--r--   0        0        0    10921 2024-03-23 20:44:00.242061 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2_listener/__init__.py
--rw-r--r--   0        0        0    10216 2024-04-05 21:17:25.394956 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2_listener/lookup_listener.py
--rw-r--r--   0        0        0    22054 2024-03-23 20:44:00.470057 ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/helpers.py
--rw-r--r--   0        0        0    14439 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/elbv2/x-elbv2.spec.json
--rw-r--r--   0        0        0      414 2024-03-23 20:44:00.319060 ecs_composex-1.1.0rc2/ecs_composex/events/__init__.py
--rw-r--r--   0        0        0     8913 2024-03-23 20:44:00.065064 ecs_composex-1.1.0rc2/ecs_composex/events/events_ecs.py
--rw-r--r--   0        0        0     1882 2024-03-23 20:44:00.350059 ecs_composex-1.1.0rc2/ecs_composex/events/events_helpers.py
--rw-r--r--   0        0        0      414 2024-03-23 20:44:00.454058 ecs_composex-1.1.0rc2/ecs_composex/events/events_module.py
--rw-r--r--   0        0        0     6645 2024-03-23 20:44:00.174062 ecs_composex-1.1.0rc2/ecs_composex/events/events_stack.py
--rw-r--r--   0        0        0     2053 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/events/x-events.spec.json
--rw-r--r--   0        0        0      480 2024-03-23 20:44:00.183062 ecs_composex-1.1.0rc2/ecs_composex/exceptions.py
--rw-r--r--   0        0        0     2487 2024-03-23 20:44:00.238061 ecs_composex-1.1.0rc2/ecs_composex/iam/__init__.py
--rw-r--r--   0        0        0     6262 2024-03-23 20:43:59.999065 ecs_composex-1.1.0rc2/ecs_composex/iam/iam_ecs_helpers.py
--rw-r--r--   0        0        0      950 2024-03-23 20:44:00.149062 ecs_composex-1.1.0rc2/ecs_composex/iam/iam_params.py
--rw-r--r--   0        0        0     3415 2024-03-23 20:44:00.503057 ecs_composex-1.1.0rc2/ecs_composex/iam/iam_stack.py
--rw-r--r--   0        0        0     1781 2024-03-23 20:44:00.314060 ecs_composex-1.1.0rc2/ecs_composex/iam/import_sam_policies.py
--rw-r--r--   0        0        0    67793 2024-04-14 21:59:42.080076 ecs_composex-1.1.0rc2/ecs_composex/iam/sam_policies.json
--rw-r--r--   0        0        0    15021 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc2/ecs_composex/ingress_settings.py
--rw-r--r--   0        0        0      421 2024-03-23 20:44:00.080063 ecs_composex-1.1.0rc2/ecs_composex/kinesis/__init__.py
--rw-r--r--   0        0        0     4732 2023-11-29 08:40:57.722589 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kcl_helpers.py
--rw-r--r--   0        0        0     2984 2024-03-23 20:44:00.113063 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_kinesis_firehose.py
--rw-r--r--   0        0        0      421 2024-03-23 20:44:00.013064 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_module.py
--rw-r--r--   0        0        0      535 2024-03-23 20:43:59.864067 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_params.py
--rw-r--r--   0        0        0     1022 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_perms.json
--rw-r--r--   0        0        0     7714 2024-03-23 20:44:00.294060 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_stack.py
--rw-r--r--   0        0        0     2630 2024-03-23 20:44:00.365059 ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_template.py
--rw-r--r--   0        0        0     2692 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/kinesis/x-kinesis.spec.json
--rw-r--r--   0        0        0      501 2024-03-23 20:44:00.213061 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/__init__.py
--rw-r--r--   0        0        0     2946 2024-03-23 20:44:00.246061 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_iam_helpers.py
--rw-r--r--   0        0        0     4602 2024-03-23 20:43:59.821067 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_logging_helpers.py
--rw-r--r--   0        0        0      501 2024-03-23 20:44:00.190062 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_module.py
--rw-r--r--   0        0        0      624 2024-03-23 20:43:59.996065 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_params.py
--rw-r--r--   0        0        0      205 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_perms.json
--rw-r--r--   0        0        0     6686 2024-03-23 20:44:00.421058 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_stack.py
--rw-r--r--   0        0        0     4278 2024-03-23 20:44:00.436058 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_template.py
--rw-r--r--   0        0        0     1858 2024-04-14 21:59:41.106094 ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/x-kinesis_firehose.spec.json
--rw-r--r--   0        0        0      284 2024-03-23 20:44:00.044064 ecs_composex-1.1.0rc2/ecs_composex/kms/__init__.py
--rw-r--r--   0        0        0     2102 2024-03-23 20:44:00.452058 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_ecs_cluster.py
--rw-r--r--   0        0        0     4549 2024-03-23 20:43:59.905066 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_kinesis_firehose.py
--rw-r--r--   0        0        0      409 2024-03-23 20:44:00.312060 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_module.py
--rw-r--r--   0        0        0      956 2024-03-23 20:44:00.327060 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_params.py
--rw-r--r--   0        0        0     1169 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_perms.json
--rw-r--r--   0        0        0     2556 2024-03-23 20:44:00.216061 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_s3.py
--rw-r--r--   0        0        0     2311 2024-03-23 20:43:59.888066 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_sqs.py
--rw-r--r--   0        0        0     9013 2024-03-23 20:44:00.292060 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_stack.py
--rw-r--r--   0        0        0     1479 2024-03-23 20:43:59.951065 ecs_composex-1.1.0rc2/ecs_composex/kms/kms_template.py
--rw-r--r--   0        0        0      826 2024-04-14 21:59:41.110093 ecs_composex-1.1.0rc2/ecs_composex/kms/x-kms.spec.json
--rw-r--r--   0        0        0    12383 2024-03-23 20:43:59.988065 ecs_composex-1.1.0rc2/ecs_composex/mods_manager.py
--rw-r--r--   0        0        0       90 2024-03-23 20:44:00.052064 ecs_composex-1.1.0rc2/ecs_composex/neptune/__init__.py
--rw-r--r--   0        0        0      478 2024-03-23 20:44:00.208062 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_module.py
--rw-r--r--   0        0        0      864 2024-03-23 20:43:59.941066 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_params.py
--rw-r--r--   0        0        0      337 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_perms.json
--rw-r--r--   0        0        0     9212 2024-03-23 20:44:00.459057 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_stack.py
--rw-r--r--   0        0        0     5088 2024-03-23 20:44:00.250061 ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_template.py
--rw-r--r--   0        0        0     3013 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/neptune/x-neptune.spec.json
--rw-r--r--   0        0        0      488 2024-03-23 20:43:59.858067 ecs_composex-1.1.0rc2/ecs_composex/opensearch/__init__.py
--rw-r--r--   0        0        0     2441 2024-03-23 20:44:00.188062 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_aws.py
--rw-r--r--   0        0        0      487 2024-03-23 20:43:59.981065 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_module.py
--rw-r--r--   0        0        0      950 2024-03-23 20:44:00.007065 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_params.py
--rw-r--r--   0        0        0      983 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_perms.json
--rw-r--r--   0        0        0     6315 2024-03-23 20:44:00.073063 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_stack.py
--rw-r--r--   0        0        0    22533 2024-03-23 20:44:00.325060 ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_template.py
--rw-r--r--   0        0        0     3216 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/opensearch/x-opensearch.spec.json
--rw-r--r--   0        0        0       19 2021-03-04 09:40:13.444136 ecs_composex-1.1.0rc2/ecs_composex/rds/.gitignore
--rw-r--r--   0        0        0      146 2024-03-23 20:43:59.813068 ecs_composex-1.1.0rc2/ecs_composex/rds/__init__.py
--rw-r--r--   0        0        0     1703 2024-03-23 20:44:00.465057 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_conditions.py
--rw-r--r--   0        0        0    20461 2024-03-23 20:43:59.939066 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_db_template.py
--rw-r--r--   0        0        0     5939 2024-03-23 20:44:00.180062 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_features.py
--rw-r--r--   0        0        0     5448 2024-03-23 20:44:00.509057 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_features_define.py
--rw-r--r--   0        0        0      455 2024-03-23 20:44:00.417058 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_module.py
--rw-r--r--   0        0        0     3624 2024-03-23 20:44:00.146062 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_parameter_groups_helper.py
--rw-r--r--   0        0        0     2898 2024-03-23 20:44:00.305060 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_params.py
--rw-r--r--   0        0        0      164 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_perms.json
--rw-r--r--   0        0        0    10438 2024-03-23 20:43:59.953065 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_stack.py
--rw-r--r--   0        0        0     4557 2024-03-23 20:44:00.164062 ecs_composex-1.1.0rc2/ecs_composex/rds/rds_template.py
--rw-r--r--   0        0        0     5948 2024-04-14 21:59:41.114093 ecs_composex-1.1.0rc2/ecs_composex/rds/x-rds.spec.json
--rw-r--r--   0        0        0    22462 2024-04-14 21:58:44.889124 ecs_composex-1.1.0rc2/ecs_composex/rds_resources_settings.py
--rw-r--r--   0        0        0    27883 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc2/ecs_composex/resource_settings.py
--rw-r--r--   0        0        0     8660 2024-03-23 20:44:00.440058 ecs_composex-1.1.0rc2/ecs_composex/resources_import.py
--rw-r--r--   0        0        0        0 2022-06-16 20:44:41.834935 ecs_composex-1.1.0rc2/ecs_composex/route53/__init__.py
--rw-r--r--   0        0        0     4385 2024-03-23 20:44:00.037064 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_acm.py
--rw-r--r--   0        0        0     5433 2024-03-23 20:44:00.134063 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_elbv2.py
--rw-r--r--   0        0        0     3983 2024-03-23 20:44:00.371059 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_helpers.py
--rw-r--r--   0        0        0      429 2024-03-23 20:44:00.303060 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_module.py
--rw-r--r--   0        0        0     1136 2024-03-23 20:44:00.154062 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_params.py
--rw-r--r--   0        0        0     7828 2024-03-23 20:44:00.448058 ecs_composex-1.1.0rc2/ecs_composex/route53/route53_stack.py
--rw-r--r--   0        0        0     1476 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/route53/x-route53.spec.json
--rw-r--r--   0        0        0      283 2024-03-23 20:44:00.111063 ecs_composex-1.1.0rc2/ecs_composex/s3/__init__.py
--rw-r--r--   0        0        0     7451 2024-03-23 20:43:59.913066 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_bucket.py
--rw-r--r--   0        0        0     2581 2024-03-23 20:44:00.033064 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_ecs_cluster.py
--rw-r--r--   0        0        0     3848 2024-03-23 20:44:00.307060 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_kinesis_firehose.py
--rw-r--r--   0        0        0      406 2024-03-23 20:44:00.105063 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_module.py
--rw-r--r--   0        0        0     2289 2024-03-23 20:44:00.031064 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_params.py
--rw-r--r--   0        0        0     3566 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_perms.json
--rw-r--r--   0        0        0     5135 2024-03-23 20:44:00.438058 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_stack.py
--rw-r--r--   0        0        0     7858 2024-03-23 20:44:00.115063 ecs_composex-1.1.0rc2/ecs_composex/s3/s3_template.py
--rw-r--r--   0        0        0     3232 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/s3/x-s3.spec.json
--rw-r--r--   0        0        0     2948 2024-03-23 20:44:00.003065 ecs_composex-1.1.0rc2/ecs_composex/secrets/__init__.py
--rw-r--r--   0        0        0     2005 2024-03-23 20:44:00.198062 ecs_composex-1.1.0rc2/ecs_composex/secrets/secrets_aws.py
--rw-r--r--   0        0        0      493 2024-03-23 20:44:00.290060 ecs_composex-1.1.0rc2/ecs_composex/secrets/secrets_params.py
--rw-r--r--   0        0        0      284 2024-03-23 20:44:00.338060 ecs_composex-1.1.0rc2/ecs_composex/sns/__init__.py
--rw-r--r--   0        0        0     2625 2024-03-23 20:44:00.218061 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_helpers.py
--rw-r--r--   0        0        0      407 2024-03-23 20:43:59.872067 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_module.py
--rw-r--r--   0        0        0      698 2024-03-23 20:44:00.257061 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_params.py
--rw-r--r--   0        0        0      128 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_perms.json
--rw-r--r--   0        0        0     2377 2024-03-23 20:44:00.233061 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_stack.py
--rw-r--r--   0        0        0     1286 2024-03-23 20:43:59.823068 ecs_composex-1.1.0rc2/ecs_composex/sns/sns_templates.py
--rw-r--r--   0        0        0      696 2024-04-14 21:59:41.111093 ecs_composex-1.1.0rc2/ecs_composex/sns/x-sns.spec.json
--rw-r--r--   0        0        0      281 2024-03-23 20:44:00.446058 ecs_composex-1.1.0rc2/ecs_composex/specs/__init__.py
--rw-r--r--   0        0        0      742 2024-03-23 20:44:00.143062 ecs_composex-1.1.0rc2/ecs_composex/specs/_core.py
--rw-r--r--   0        0        0    29055 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/compose-spec.json
--rw-r--r--   0        0        0     2455 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/ingress.spec.json
--rw-r--r--   0        0        0     1234 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/secrets.x-secrets.spec.json
--rw-r--r--   0        0        0     2266 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services-xray.spec.json
--rw-r--r--   0        0        0     1404 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-alarms.spec.json
--rw-r--r--   0        0        0      403 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-codeguru_profiler.spec.json
--rw-r--r--   0        0        0      501 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-docker_opts.spec.json
--rw-r--r--   0        0        0     1853 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-ecr.spec.json
--rw-r--r--   0        0        0     2745 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-ecs.spec.json
--rw-r--r--   0        0        0      836 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-environment.spec.json
--rw-r--r--   0        0        0     2175 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-iam.spec.json
--rw-r--r--   0        0        0     7429 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-logging.spec.json
--rw-r--r--   0        0        0     1986 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-monitoring.spec.json
--rw-r--r--   0        0        0     4477 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-network.spec.json
--rw-r--r--   0        0        0     4724 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-prometheus.spec.json
--rw-r--r--   0        0        0     4105 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-scaling.spec.json
--rw-r--r--   0        0        0     2133 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/x-cluster.spec.json
--rw-r--r--   0        0        0     6706 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/x-rds-common.spec.json
--rw-r--r--   0        0        0     6559 2024-04-14 21:59:41.109094 ecs_composex-1.1.0rc2/ecs_composex/specs/x-resources.common.spec.json
--rw-r--r--   0        0        0      816 2024-04-14 21:59:41.108093 ecs_composex-1.1.0rc2/ecs_composex/specs/x-tags.spec.json
--rw-r--r--   0        0        0      285 2024-03-23 20:44:00.279060 ecs_composex-1.1.0rc2/ecs_composex/sqs/__init__.py
--rw-r--r--   0        0        0     4737 2024-03-23 20:43:59.937066 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_ecs_scaling.py
--rw-r--r--   0        0        0     3592 2024-03-23 20:43:59.890066 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_helpers.py
--rw-r--r--   0        0        0      407 2024-03-23 20:43:59.836067 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_module.py
--rw-r--r--   0        0        0      865 2024-03-23 20:44:00.141063 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_params.py
--rw-r--r--   0        0        0      515 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_perms.json
--rw-r--r--   0        0        0     5463 2024-03-23 20:44:00.050064 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_s3.py
--rw-r--r--   0        0        0     2938 2024-03-23 20:44:00.383059 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_sqs.py
--rw-r--r--   0        0        0     4375 2024-03-23 20:43:59.917066 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_stack.py
--rw-r--r--   0        0        0     7648 2024-03-23 20:44:00.273060 ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_template.py
--rw-r--r--   0        0        0      744 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/sqs/x-sqs.spec.json
--rw-r--r--   0        0        0      488 2024-03-23 20:44:00.020064 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/__init__.py
--rw-r--r--   0        0        0     5154 2024-03-23 20:44:00.195062 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_helpers.py
--rw-r--r--   0        0        0      488 2024-03-23 20:43:59.935066 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_module.py
--rw-r--r--   0        0        0      905 2024-03-23 20:44:00.263061 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_params.py
--rw-r--r--   0        0        0      820 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_perms.json
--rw-r--r--   0        0        0     3924 2024-03-23 20:44:00.011065 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_stack.py
--rw-r--r--   0        0        0     2243 2024-04-14 21:59:41.107093 ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/x-ssm_parameter.spec.json
--rw-r--r--   0        0        0       88 2024-03-23 20:44:00.296060 ecs_composex-1.1.0rc2/ecs_composex/utils/__init__.py
--rw-r--r--   0        0        0      820 2024-03-23 20:44:00.344059 ecs_composex-1.1.0rc2/ecs_composex/utils/init_ecs.py
--rw-r--r--   0        0        0     1797 2024-03-23 20:43:59.992065 ecs_composex-1.1.0rc2/ecs_composex/utils/init_s3.py
--rw-r--r--   0        0        0      284 2024-03-23 20:44:00.497057 ecs_composex-1.1.0rc2/ecs_composex/vpc/__init__.py
--rw-r--r--   0        0        0      616 2024-03-23 20:44:00.255061 ecs_composex-1.1.0rc2/ecs_composex/vpc/aws_mappings.py
--rw-r--r--   0        0        0     3997 2024-03-23 20:43:59.919066 ecs_composex-1.1.0rc2/ecs_composex/vpc/helpers.py
--rw-r--r--   0        0        0     5154 2024-03-23 20:44:00.071064 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_aws.py
--rw-r--r--   0        0        0     1338 2024-03-23 20:44:00.357059 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_cloudmap.py
--rw-r--r--   0        0        0       88 2024-03-23 20:43:59.834067 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_conditions.py
--rw-r--r--   0        0        0     1953 2024-03-23 20:44:00.377059 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_maths.py
--rw-r--r--   0        0        0      423 2024-03-23 20:44:00.499057 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_module.py
--rw-r--r--   0        0        0     2217 2024-03-23 20:44:00.253061 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_params.py
--rw-r--r--   0        0        0    14983 2024-03-23 20:44:00.442058 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_stack.py
--rw-r--r--   0        0        0    10517 2024-03-23 20:44:00.161062 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_subnets.py
--rw-r--r--   0        0        0     4709 2024-03-23 20:44:00.109063 ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_template.py
--rw-r--r--   0        0        0     3504 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/vpc/x-vpc.spec.json
--rw-r--r--   0        0        0       90 2024-03-23 20:44:00.336059 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/__init__.py
--rw-r--r--   0        0        0      697 2024-03-23 20:44:00.119063 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/validators_wafv2.py
--rw-r--r--   0        0        0     2255 2024-03-23 20:44:00.288060 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_elbv2.py
--rw-r--r--   0        0        0      497 2024-03-23 20:44:00.169062 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_module.py
--rw-r--r--   0        0        0     1079 2024-03-23 20:43:59.850067 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_params.py
--rw-r--r--   0        0        0      185 2024-04-14 21:59:41.112093 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_perms.json
--rw-r--r--   0        0        0     9460 2024-03-23 20:44:00.373059 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_stack.py
--rw-r--r--   0        0        0     1357 2024-03-23 20:44:00.423058 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_template.py
--rw-r--r--   0        0        0     1772 2024-04-14 21:59:41.113093 ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/x-wafv2_webacl.spec.json
--rw-r--r--   0        0        0     3476 2024-04-14 21:59:40.442106 ecs_composex-1.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     8907 1970-01-01 00:00:00.000000 ecs_composex-1.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2021-05-14 10:51:20.077071 ecs_composex-1.1.0rc3/LICENSE
+-rw-r--r--   0        0        0      385 2022-06-16 18:49:16.792466 ecs_composex-1.1.0rc3/MANIFEST.in
+-rw-r--r--   0        0        0     1068 2023-08-07 12:54:52.746417 ecs_composex-1.1.0rc3/NOTICES.rst
+-rw-r--r--   0        0        0     6976 2023-01-11 09:54:17.357527 ecs_composex-1.1.0rc3/README.rst
+-rw-r--r--   0        0        0       19 2021-03-04 09:40:13.458136 ecs_composex-1.1.0rc3/ecs_composex/.gitignore
+-rw-r--r--   0        0        0      222 2024-04-15 08:30:36.452587 ecs_composex-1.1.0rc3/ecs_composex/__init__.py
+-rw-r--r--   0        0        0      117 2024-03-23 20:44:00.309060 ecs_composex-1.1.0rc3/ecs_composex/acm/__init__.py
+-rw-r--r--   0        0        0      419 2024-03-23 20:44:00.401059 ecs_composex-1.1.0rc3/ecs_composex/acm/acm_module.py
+-rw-r--r--   0        0        0     1546 2024-03-23 20:44:00.178062 ecs_composex-1.1.0rc3/ecs_composex/acm/acm_params.py
+-rw-r--r--   0        0        0     5773 2024-03-23 20:44:00.185062 ecs_composex-1.1.0rc3/ecs_composex/acm/acm_stack.py
+-rw-r--r--   0        0        0     7634 2024-03-23 20:44:00.125063 ecs_composex-1.1.0rc3/ecs_composex/acm/acm_stack_helpers.py
+-rw-r--r--   0        0        0     1327 2024-04-15 08:30:37.402572 ecs_composex-1.1.0rc3/ecs_composex/acm/x-acm.spec.json
+-rw-r--r--   0        0        0      416 2024-03-23 20:44:00.390059 ecs_composex-1.1.0rc3/ecs_composex/alarms/__init__.py
+-rw-r--r--   0        0        0     9162 2024-03-23 20:44:00.121063 ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_ecs.py
+-rw-r--r--   0        0        0     6292 2024-03-23 20:44:00.005065 ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_elbv2.py
+-rw-r--r--   0        0        0     8575 2024-03-23 20:43:59.927066 ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_helpers.py
+-rw-r--r--   0        0        0      416 2024-03-23 20:44:00.139063 ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_module.py
+-rw-r--r--   0        0        0      532 2024-03-23 20:44:00.388059 ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_params.py
+-rw-r--r--   0        0        0     4520 2024-03-23 20:43:59.894066 ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_stack.py
+-rw-r--r--   0        0        0     1920 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/alarms/x-alarms.spec.json
+-rw-r--r--   0        0        0       44 2022-06-16 18:49:16.909464 ecs_composex-1.1.0rc3/ecs_composex/appmesh/README.rst
+-rw-r--r--   0        0        0      288 2024-03-23 20:44:00.220061 ecs_composex-1.1.0rc3/ecs_composex/appmesh/__init__.py
+-rw-r--r--   0        0        0     2268 2024-03-23 20:43:59.826068 ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_aws.py
+-rw-r--r--   0        0        0     1479 2024-03-23 20:44:00.369059 ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_conditions.py
+-rw-r--r--   0        0        0     9620 2024-03-23 20:44:00.022064 ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_mesh.py
+-rw-r--r--   0        0        0    12953 2024-03-23 20:44:00.203061 ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_node.py
+-rw-r--r--   0        0        0     1222 2024-03-23 20:43:59.819068 ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_params.py
+-rw-r--r--   0        0        0    10944 2024-03-23 20:44:00.127063 ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_router.py
+-rw-r--r--   0        0        0     6917 2024-03-23 20:44:00.367059 ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_service.py
+-rw-r--r--   0        0        0     4576 2024-04-15 08:30:37.405572 ecs_composex-1.1.0rc3/ecs_composex/appmesh/x-appmesh.spec.json
+-rw-r--r--   0        0        0      121 2024-03-23 20:43:59.931066 ecs_composex-1.1.0rc3/ecs_composex/aps/__init__.py
+-rw-r--r--   0        0        0      501 2024-03-23 20:44:00.240061 ecs_composex-1.1.0rc3/ecs_composex/aps/aps_module.py
+-rw-r--r--   0        0        0      938 2024-03-23 20:44:00.136062 ecs_composex-1.1.0rc3/ecs_composex/aps/aps_parameters.py
+-rw-r--r--   0        0        0      492 2024-04-15 08:30:37.404572 ecs_composex-1.1.0rc3/ecs_composex/aps/aps_perms.json
+-rw-r--r--   0        0        0     7896 2024-03-23 20:44:00.467057 ecs_composex-1.1.0rc3/ecs_composex/aps/aps_stack.py
+-rw-r--r--   0        0        0     1219 2024-04-15 08:30:37.404572 ecs_composex-1.1.0rc3/ecs_composex/aps/x-aps.spec.json
+-rw-r--r--   0        0        0     6802 2024-03-23 20:44:00.151062 ecs_composex-1.1.0rc3/ecs_composex/cli.py
+-rw-r--r--   0        0        0      481 2024-03-23 20:44:00.271061 ecs_composex-1.1.0rc3/ecs_composex/cloudmap/__init__.py
+-rw-r--r--   0        0        0     7347 2024-03-23 20:44:00.090063 ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_ecs.py
+-rw-r--r--   0        0        0     5364 2024-03-23 20:43:59.853067 ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_helpers.py
+-rw-r--r--   0        0        0      481 2024-03-23 20:43:59.986065 ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_module.py
+-rw-r--r--   0        0        0     2100 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_params.py
+-rw-r--r--   0        0        0    12308 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_stack.py
+-rw-r--r--   0        0        0     7790 2024-03-23 20:43:59.886067 ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_x_resources.py
+-rw-r--r--   0        0        0     1486 2024-04-15 08:30:37.404572 ecs_composex-1.1.0rc3/ecs_composex/cloudmap/x-cloudmap.spec.json
+-rw-r--r--   0        0        0      500 2024-03-23 20:44:00.107063 ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/__init__.py
+-rw-r--r--   0        0        0     1761 2024-03-23 20:44:00.321060 ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/codeguru_profiler_aws.py
+-rw-r--r--   0        0        0      500 2024-03-23 20:44:00.359059 ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/codeguru_profiler_module.py
+-rw-r--r--   0        0        0      603 2024-03-23 20:44:00.419058 ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/codeguru_profiler_params.py
+-rw-r--r--   0        0        0      188 2024-04-15 08:30:37.402572 ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/codeguru_profiler_perms.json
+-rw-r--r--   0        0        0     5053 2024-03-23 20:43:59.897066 ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/codeguru_profiler_stack.py
+-rw-r--r--   0        0        0      489 2024-03-23 20:44:00.009065 ecs_composex-1.1.0rc3/ecs_composex/cognito_userpool/__init__.py
+-rw-r--r--   0        0        0      909 2024-03-23 20:43:59.840067 ecs_composex-1.1.0rc3/ecs_composex/cognito_userpool/cognito_params.py
+-rw-r--r--   0        0        0      489 2024-03-23 20:43:59.828067 ecs_composex-1.1.0rc3/ecs_composex/cognito_userpool/cognito_userpool_module.py
+-rw-r--r--   0        0        0     4821 2024-03-23 20:43:59.961065 ecs_composex-1.1.0rc3/ecs_composex/cognito_userpool/cognito_userpool_stack.py
+-rw-r--r--   0        0        0      375 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/cognito_userpool/x-cognito_userpool.spec.json
+-rw-r--r--   0        0        0     2314 2024-03-23 20:44:00.088063 ecs_composex-1.1.0rc3/ecs_composex/common/__init__.py
+-rw-r--r--   0        0        0    13821 2024-03-23 20:43:59.947065 ecs_composex-1.1.0rc3/ecs_composex/common/aws.py
+-rw-r--r--   0        0        0     1209 2024-03-23 20:44:00.432058 ecs_composex-1.1.0rc3/ecs_composex/common/cfn_conditions.py
+-rw-r--r--   0        0        0     1258 2024-03-23 20:43:59.901066 ecs_composex-1.1.0rc3/ecs_composex/common/cfn_params.py
+-rw-r--r--   0        0        0      408 2024-03-23 20:44:00.103063 ecs_composex-1.1.0rc3/ecs_composex/common/ecs_composex.py
+-rw-r--r--   0        0        0     1465 2024-03-23 22:36:48.972815 ecs_composex-1.1.0rc3/ecs_composex/common/envsubst.py
+-rw-r--r--   0        0        0     9180 2024-03-23 20:43:59.971065 ecs_composex-1.1.0rc3/ecs_composex/common/files.py
+-rw-r--r--   0        0        0     1937 2024-03-23 20:43:59.921066 ecs_composex-1.1.0rc3/ecs_composex/common/logging.py
+-rw-r--r--   0        0        0    24735 2024-03-31 16:04:04.611153 ecs_composex-1.1.0rc3/ecs_composex/common/settings.py
+-rw-r--r--   0        0        0    14081 2024-03-23 20:44:00.463057 ecs_composex-1.1.0rc3/ecs_composex/common/stacks/__init__.py
+-rw-r--r--   0        0        0     8705 2024-03-23 20:44:00.333059 ecs_composex-1.1.0rc3/ecs_composex/common/tagging.py
+-rw-r--r--   0        0        0    10189 2024-03-23 20:43:59.845067 ecs_composex-1.1.0rc3/ecs_composex/common/troposphere_tools.py
+-rw-r--r--   0        0        0       90 2024-03-23 20:44:00.277060 ecs_composex-1.1.0rc3/ecs_composex/compose/__init__.py
+-rw-r--r--   0        0        0     1629 2024-03-23 20:44:00.131063 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_networks.py
+-rw-r--r--   0        0        0     9238 2024-03-23 20:44:00.042064 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_secrets/__init__.py
+-rw-r--r--   0        0        0     3632 2024-03-23 20:44:00.229061 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_secrets/ecs_family_helpers.py
+-rw-r--r--   0        0        0     1490 2024-03-23 20:44:00.222061 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_secrets/helpers.py
+-rw-r--r--   0        0        0     1292 2024-03-23 20:44:00.227061 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_secrets/services_helpers.py
+-rw-r--r--   0        0        0    37531 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/__init__.py
+-rw-r--r--   0        0        0     6697 2024-03-23 20:43:59.903066 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/docker_tools.py
+-rw-r--r--   0        0        0     3399 2024-03-23 20:44:00.001065 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/env_files_helpers.py
+-rw-r--r--   0        0        0     9848 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/helpers.py
+-rw-r--r--   0        0        0     3658 2024-03-23 20:44:00.275061 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/kernel_options_helpers.py
+-rw-r--r--   0        0        0     8042 2024-03-23 20:44:00.129063 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_image/__init__.py
+-rw-r--r--   0        0        0     2719 2024-03-23 20:44:00.375059 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_image/docker_opts.py
+-rw-r--r--   0        0        0     3911 2024-03-23 20:43:59.892066 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_image/ecr_helpers.py
+-rw-r--r--   0        0        0    10829 2024-03-23 20:44:00.167062 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_image/ecr_scans_eval.py
+-rw-r--r--   0        0        0     5119 2024-03-23 20:44:00.261061 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_logging/__init__.py
+-rw-r--r--   0        0        0     5036 2024-03-23 20:43:59.855067 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_logging/helpers.py
+-rw-r--r--   0        0        0     3873 2024-03-23 20:43:59.983065 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_volumes/__init__.py
+-rw-r--r--   0        0        0     6846 2024-03-23 20:44:00.069064 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_volumes/ecs_family_helpers.py
+-rw-r--r--   0        0        0     1459 2024-03-23 20:44:00.331060 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_volumes/helpers.py
+-rw-r--r--   0        0        0     5651 2024-03-23 20:44:00.096063 ecs_composex-1.1.0rc3/ecs_composex/compose/compose_volumes/services_helpers.py
+-rw-r--r--   0        0        0    30750 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/__init__.py
+-rw-r--r--   0        0        0     1672 2024-03-23 20:43:59.911066 ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/api_x_resources.py
+-rw-r--r--   0        0        0      922 2024-03-23 20:44:00.461058 ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/environment_x_resources.py
+-rw-r--r--   0        0        0     4657 2024-03-23 20:44:00.123063 ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/helpers.py
+-rw-r--r--   0        0        0     6435 2024-03-23 20:44:00.048064 ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/network_x_resources.py
+-rw-r--r--   0        0        0     8806 2024-03-23 20:43:59.838067 ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/services_resources.py
+-rw-r--r--   0        0        0       90 2024-03-23 20:44:00.017064 ecs_composex-1.1.0rc3/ecs_composex/dashboards/__init__.py
+-rw-r--r--   0        0        0      472 2024-03-23 20:43:59.842067 ecs_composex-1.1.0rc3/ecs_composex/dashboards/dashboards_module.py
+-rw-r--r--   0        0        0     5539 2024-03-23 20:44:00.329059 ecs_composex-1.1.0rc3/ecs_composex/dashboards/dashboards_services_metrics.py
+-rw-r--r--   0        0        0     4831 2024-03-23 20:44:00.035064 ecs_composex-1.1.0rc3/ecs_composex/dashboards/dashboards_stack.py
+-rw-r--r--   0        0        0     1224 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/dashboards/x-dashboards.spec.json
+-rw-r--r--   0        0        0      413 2024-03-23 20:44:00.259061 ecs_composex-1.1.0rc3/ecs_composex/docdb/__init__.py
+-rw-r--r--   0        0        0      413 2024-03-23 20:43:59.915066 ecs_composex-1.1.0rc3/ecs_composex/docdb/docdb_module.py
+-rw-r--r--   0        0        0      833 2024-03-23 20:44:00.346059 ecs_composex-1.1.0rc3/ecs_composex/docdb/docdb_params.py
+-rw-r--r--   0        0        0      164 2024-04-15 08:30:37.401572 ecs_composex-1.1.0rc3/ecs_composex/docdb/docdb_perms.json
+-rw-r--r--   0        0        0     7772 2024-03-23 20:43:59.876067 ecs_composex-1.1.0rc3/ecs_composex/docdb/docdb_stack.py
+-rw-r--r--   0        0        0     6450 2024-03-23 20:44:00.063064 ecs_composex-1.1.0rc3/ecs_composex/docdb/docdb_template.py
+-rw-r--r--   0        0        0     2241 2024-04-15 08:30:37.402572 ecs_composex-1.1.0rc3/ecs_composex/docdb/x-docdb.spec.json
+-rw-r--r--   0        0        0      289 2024-03-23 20:44:00.046064 ecs_composex-1.1.0rc3/ecs_composex/dynamodb/__init__.py
+-rw-r--r--   0        0        0     7795 2024-03-23 20:44:00.248061 ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_autoscaling.py
+-rw-r--r--   0        0        0      422 2024-03-23 20:44:00.117063 ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_module.py
+-rw-r--r--   0        0        0      412 2024-03-23 20:43:59.966065 ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_params.py
+-rw-r--r--   0        0        0     1096 2024-04-15 08:30:37.405572 ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_perms.json
+-rw-r--r--   0        0        0     4131 2024-03-23 20:44:00.355059 ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_stack.py
+-rw-r--r--   0        0        0     2916 2024-03-23 20:44:00.075064 ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_template.py
+-rw-r--r--   0        0        0     2777 2024-04-15 08:30:37.405572 ecs_composex-1.1.0rc3/ecs_composex/dynamodb/x-dynamodb.spec.json
+-rw-r--r--   0        0        0     1050 2024-03-23 20:44:00.094063 ecs_composex-1.1.0rc3/ecs_composex/ecs/__init__.py
+-rw-r--r--   0        0        0     3532 2024-03-23 20:43:59.955065 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_conditions.py
+-rw-r--r--   0        0        0    27604 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/__init__.py
+-rw-r--r--   0        0        0    14849 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_helpers/__init__.py
+-rw-r--r--   0        0        0     1316 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_helpers/compute_finalizers.py
+-rw-r--r--   0        0        0     1912 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_helpers/network_finalizers.py
+-rw-r--r--   0        0        0     8788 2024-03-23 20:43:59.870067 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_logging/__init__.py
+-rw-r--r--   0        0        0     4123 2024-03-23 20:44:00.061064 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_logging/cw_logging.py
+-rw-r--r--   0        0        0     2940 2024-03-23 20:43:59.880066 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_template.py
+-rw-r--r--   0        0        0     3502 2024-03-23 20:43:59.861067 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/task_execute_command.py
+-rw-r--r--   0        0        0     2626 2024-03-23 20:44:00.015065 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/task_runtime.py
+-rw-r--r--   0        0        0      163 2024-03-23 20:44:00.381059 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/__init__.py
+-rw-r--r--   0        0        0    10598 2024-03-23 20:43:59.949066 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/__init__.py
+-rw-r--r--   0        0        0     5822 2024-03-23 20:44:00.098063 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_firehose.py
+-rw-r--r--   0        0        0     5548 2024-03-23 20:44:00.282060 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_kinesis.py
+-rw-r--r--   0        0        0     3067 2024-03-23 20:43:59.882067 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/config_parameter.py
+-rw-r--r--   0        0        0      609 2023-08-07 12:54:52.748417 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/family_fluentbit_managed_config.j2
+-rw-r--r--   0        0        0     3408 2024-03-23 20:44:00.451058 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/firelens_config_sidecar.py
+-rw-r--r--   0        0        0      613 2023-08-07 12:54:52.748417 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/service_fluentbit_managed_config.j2
+-rw-r--r--   0        0        0     3807 2024-03-23 20:44:00.225061 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/firelens_advanced_rendered_settings.py
+-rw-r--r--   0        0        0     5267 2024-03-23 20:44:00.363059 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/firelens_logger_helpers.py
+-rw-r--r--   0        0        0     6883 2024-03-23 20:44:00.348059 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/firelens_managed_sidecar_service.py
+-rw-r--r--   0        0        0     2548 2024-03-23 20:44:00.323060 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/firelens_options_generic_helpers.py
+-rw-r--r--   0        0        0      161 2024-03-23 20:43:59.909066 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/helpers/__init__.py
+-rw-r--r--   0        0        0     2293 2024-03-23 20:44:00.340059 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/helpers/cloudwatch_helpers.py
+-rw-r--r--   0        0        0     3812 2024-03-23 20:44:00.511057 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/helpers/firehose_helpers.py
+-rw-r--r--   0        0        0     3561 2024-03-23 20:44:00.353059 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/helpers/kinesis_helpers.py
+-rw-r--r--   0        0        0     5752 2024-03-23 20:44:00.425058 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_params.py
+-rw-r--r--   0        0        0     4482 2024-03-23 20:44:00.092063 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_prometheus/__init__.py
+-rw-r--r--   0        0        0     4829 2024-03-23 20:44:00.211061 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_prometheus/config_ssm_parameters.py
+-rw-r--r--   0        0        0     9763 2024-03-23 20:43:59.990065 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_prometheus/emf_processors.py
+-rw-r--r--   0        0        0     6413 2024-03-23 20:43:59.860067 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_prometheus/helpers.py
+-rw-r--r--   0        0        0     3525 2024-03-23 20:43:59.866067 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_service/__init__.py
+-rw-r--r--   0        0        0     4688 2024-03-23 20:44:00.067064 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_service/helpers.py
+-rw-r--r--   0        0        0     5588 2024-03-30 09:27:30.584324 ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_stack.py
+-rw-r--r--   0        0        0     1927 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc3/ecs_composex/ecs/helpers/__init__.py
+-rw-r--r--   0        0        0     2857 2024-03-23 20:44:00.159062 ecs_composex-1.1.0rc3/ecs_composex/ecs/managed_sidecars/__init__.py
+-rw-r--r--   0        0        0     1414 2024-03-23 20:44:00.284060 ecs_composex-1.1.0rc3/ecs_composex/ecs/managed_sidecars/aws_cw_agent.py
+-rw-r--r--   0        0        0     2805 2024-03-23 20:44:00.200062 ecs_composex-1.1.0rc3/ecs_composex/ecs/managed_sidecars/aws_xray.py
+-rw-r--r--   0        0        0      960 2024-03-23 20:43:59.874067 ecs_composex-1.1.0rc3/ecs_composex/ecs/managed_sidecars/nginx_prometheus_exporter.py
+-rw-r--r--   0        0        0     6182 2024-03-23 20:43:59.907066 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_alarms/__init__.py
+-rw-r--r--   0        0        0     3158 2024-03-23 20:44:00.434058 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_alarms/service_predefined_alarms.py
+-rw-r--r--   0        0        0     5545 2024-03-23 20:44:00.361059 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_compute/__init__.py
+-rw-r--r--   0        0        0     1861 2024-03-23 20:44:00.379059 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_compute/helpers.py
+-rw-r--r--   0        0        0    10734 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_networking/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_networking/helpers.py
+-rw-r--r--   0        0        0    15293 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_networking/ingress_helpers.py
+-rw-r--r--   0        0        0     9051 2024-03-23 20:44:00.059064 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_scaling/__init__.py
+-rw-r--r--   0        0        0    12114 2024-03-23 20:44:00.386059 ecs_composex-1.1.0rc3/ecs_composex/ecs/service_scaling/helpers.py
+-rw-r--r--   0        0        0     5012 2024-03-23 20:44:00.206061 ecs_composex-1.1.0rc3/ecs_composex/ecs/task_compute/__init__.py
+-rw-r--r--   0        0        0     3831 2024-03-23 20:43:59.847067 ecs_composex-1.1.0rc3/ecs_composex/ecs/task_compute/helpers.py
+-rw-r--r--   0        0        0     5414 2024-03-23 20:43:59.884066 ecs_composex-1.1.0rc3/ecs_composex/ecs/task_iam/__init__.py
+-rw-r--r--   0        0        0     2208 2024-03-23 20:43:59.943066 ecs_composex-1.1.0rc3/ecs_composex/ecs/task_iam/helpers.py
+-rw-r--r--   0        0        0     7042 2024-03-23 20:44:00.056064 ecs_composex-1.1.0rc3/ecs_composex/ecs/task_iam/task_role.py
+-rw-r--r--   0        0        0    20480 2024-03-23 20:44:00.078064 ecs_composex-1.1.0rc3/ecs_composex/ecs_cluster/__init__.py
+-rw-r--r--   0        0        0      509 2024-03-23 20:44:00.267061 ecs_composex-1.1.0rc3/ecs_composex/ecs_cluster/ecs_cluster_params.py
+-rw-r--r--   0        0        0     7216 2024-03-23 20:44:00.029064 ecs_composex-1.1.0rc3/ecs_composex/ecs_cluster/ecs_family_helpers.py
+-rw-r--r--   0        0        0     3504 2024-03-23 20:44:00.101063 ecs_composex-1.1.0rc3/ecs_composex/ecs_cluster/helpers.py
+-rw-r--r--   0        0        0    12357 2024-03-31 16:04:04.612152 ecs_composex-1.1.0rc3/ecs_composex/ecs_composex.py
+-rw-r--r--   0        0        0      326 2024-03-30 09:27:30.585324 ecs_composex-1.1.0rc3/ecs_composex/ecs_ingress/__init__.py
+-rw-r--r--   0        0        0     3408 2024-04-15 08:29:17.269853 ecs_composex-1.1.0rc3/ecs_composex/ecs_ingress/ecs_ingress_stack.py
+-rw-r--r--   0        0        0      125 2024-03-23 20:44:00.396058 ecs_composex-1.1.0rc3/ecs_composex/efs/__init__.py
+-rw-r--r--   0        0        0    12388 2024-03-23 20:44:00.054064 ecs_composex-1.1.0rc3/ecs_composex/efs/efs_ecs.py
+-rw-r--r--   0        0        0      403 2024-03-23 20:44:00.286060 ecs_composex-1.1.0rc3/ecs_composex/efs/efs_module.py
+-rw-r--r--   0        0        0     1139 2024-03-23 20:44:00.172062 ecs_composex-1.1.0rc3/ecs_composex/efs/efs_params.py
+-rw-r--r--   0        0        0     7434 2024-03-23 20:43:59.832067 ecs_composex-1.1.0rc3/ecs_composex/efs/efs_stack.py
+-rw-r--r--   0        0        0     1026 2024-04-15 08:30:37.402572 ecs_composex-1.1.0rc3/ecs_composex/efs/x-efs.spec.json
+-rw-r--r--   0        0        0      482 2024-03-23 20:43:59.933066 ecs_composex-1.1.0rc3/ecs_composex/elasticache/__init__.py
+-rw-r--r--   0        0        0     5725 2024-03-23 20:44:00.505057 ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_aws.py
+-rw-r--r--   0        0        0     3106 2024-03-23 20:44:00.427058 ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_ecs.py
+-rw-r--r--   0        0        0      482 2024-03-23 20:44:00.342059 ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_module.py
+-rw-r--r--   0        0        0     2926 2024-03-23 20:43:59.929066 ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_params.py
+-rw-r--r--   0        0        0     8927 2024-03-23 20:44:00.040064 ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_stack.py
+-rw-r--r--   0        0        0     8942 2024-03-23 20:44:00.156062 ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_template.py
+-rw-r--r--   0        0        0      413 2024-03-23 20:44:00.507057 ecs_composex-1.1.0rc3/ecs_composex/elbv2/__init__.py
+-rw-r--r--   0        0        0    27727 2024-03-23 20:44:00.231061 ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_ecs.py
+-rw-r--r--   0        0        0      413 2024-03-23 20:43:59.899066 ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_module.py
+-rw-r--r--   0        0        0     2143 2024-03-23 20:43:59.945066 ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_params.py
+-rw-r--r--   0        0        0     2957 2024-04-03 16:23:37.606364 ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/__init__.py
+-rw-r--r--   0        0        0    22478 2024-03-23 20:44:00.082064 ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/elbv2.py
+-rw-r--r--   0        0        0    10921 2024-03-23 20:44:00.242061 ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/elbv2_listener/__init__.py
+-rw-r--r--   0        0        0    10216 2024-04-05 21:17:25.394956 ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/elbv2_listener/lookup_listener.py
+-rw-r--r--   0        0        0    22054 2024-03-23 20:44:00.470057 ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/helpers.py
+-rw-r--r--   0        0        0    14439 2024-04-15 08:30:37.406572 ecs_composex-1.1.0rc3/ecs_composex/elbv2/x-elbv2.spec.json
+-rw-r--r--   0        0        0      414 2024-03-23 20:44:00.319060 ecs_composex-1.1.0rc3/ecs_composex/events/__init__.py
+-rw-r--r--   0        0        0     8913 2024-03-23 20:44:00.065064 ecs_composex-1.1.0rc3/ecs_composex/events/events_ecs.py
+-rw-r--r--   0        0        0     1882 2024-03-23 20:44:00.350059 ecs_composex-1.1.0rc3/ecs_composex/events/events_helpers.py
+-rw-r--r--   0        0        0      414 2024-03-23 20:44:00.454058 ecs_composex-1.1.0rc3/ecs_composex/events/events_module.py
+-rw-r--r--   0        0        0     6645 2024-03-23 20:44:00.174062 ecs_composex-1.1.0rc3/ecs_composex/events/events_stack.py
+-rw-r--r--   0        0        0     2053 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/events/x-events.spec.json
+-rw-r--r--   0        0        0      480 2024-03-23 20:44:00.183062 ecs_composex-1.1.0rc3/ecs_composex/exceptions.py
+-rw-r--r--   0        0        0     2487 2024-03-23 20:44:00.238061 ecs_composex-1.1.0rc3/ecs_composex/iam/__init__.py
+-rw-r--r--   0        0        0     6262 2024-03-23 20:43:59.999065 ecs_composex-1.1.0rc3/ecs_composex/iam/iam_ecs_helpers.py
+-rw-r--r--   0        0        0      950 2024-03-23 20:44:00.149062 ecs_composex-1.1.0rc3/ecs_composex/iam/iam_params.py
+-rw-r--r--   0        0        0     3415 2024-03-23 20:44:00.503057 ecs_composex-1.1.0rc3/ecs_composex/iam/iam_stack.py
+-rw-r--r--   0        0        0     1781 2024-03-23 20:44:00.314060 ecs_composex-1.1.0rc3/ecs_composex/iam/import_sam_policies.py
+-rw-r--r--   0        0        0    67793 2024-04-15 08:30:38.332557 ecs_composex-1.1.0rc3/ecs_composex/iam/sam_policies.json
+-rw-r--r--   0        0        0    15021 2024-04-14 21:58:44.888124 ecs_composex-1.1.0rc3/ecs_composex/ingress_settings.py
+-rw-r--r--   0        0        0      421 2024-03-23 20:44:00.080063 ecs_composex-1.1.0rc3/ecs_composex/kinesis/__init__.py
+-rw-r--r--   0        0        0     4732 2023-11-29 08:40:57.722589 ecs_composex-1.1.0rc3/ecs_composex/kinesis/kcl_helpers.py
+-rw-r--r--   0        0        0     2984 2024-03-23 20:44:00.113063 ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_kinesis_firehose.py
+-rw-r--r--   0        0        0      421 2024-03-23 20:44:00.013064 ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_module.py
+-rw-r--r--   0        0        0      535 2024-03-23 20:43:59.864067 ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_params.py
+-rw-r--r--   0        0        0     1022 2024-04-15 08:30:37.402572 ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_perms.json
+-rw-r--r--   0        0        0     7714 2024-03-23 20:44:00.294060 ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_stack.py
+-rw-r--r--   0        0        0     2630 2024-03-23 20:44:00.365059 ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_template.py
+-rw-r--r--   0        0        0     2692 2024-04-15 08:30:37.402572 ecs_composex-1.1.0rc3/ecs_composex/kinesis/x-kinesis.spec.json
+-rw-r--r--   0        0        0      501 2024-03-23 20:44:00.213061 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/__init__.py
+-rw-r--r--   0        0        0     2946 2024-03-23 20:44:00.246061 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_iam_helpers.py
+-rw-r--r--   0        0        0     4602 2024-03-23 20:43:59.821067 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_logging_helpers.py
+-rw-r--r--   0        0        0      501 2024-03-23 20:44:00.190062 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_module.py
+-rw-r--r--   0        0        0      624 2024-03-23 20:43:59.996065 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_params.py
+-rw-r--r--   0        0        0      205 2024-04-15 08:30:37.399572 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_perms.json
+-rw-r--r--   0        0        0     6686 2024-03-23 20:44:00.421058 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_stack.py
+-rw-r--r--   0        0        0     4278 2024-03-23 20:44:00.436058 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_template.py
+-rw-r--r--   0        0        0     1858 2024-04-15 08:30:37.398572 ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/x-kinesis_firehose.spec.json
+-rw-r--r--   0        0        0      284 2024-03-23 20:44:00.044064 ecs_composex-1.1.0rc3/ecs_composex/kms/__init__.py
+-rw-r--r--   0        0        0     2102 2024-03-23 20:44:00.452058 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_ecs_cluster.py
+-rw-r--r--   0        0        0     4549 2024-03-23 20:43:59.905066 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_kinesis_firehose.py
+-rw-r--r--   0        0        0      409 2024-03-23 20:44:00.312060 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_module.py
+-rw-r--r--   0        0        0      956 2024-03-23 20:44:00.327060 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_params.py
+-rw-r--r--   0        0        0     1169 2024-04-15 08:30:37.402572 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_perms.json
+-rw-r--r--   0        0        0     2556 2024-03-23 20:44:00.216061 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_s3.py
+-rw-r--r--   0        0        0     2311 2024-03-23 20:43:59.888066 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_sqs.py
+-rw-r--r--   0        0        0     9013 2024-03-23 20:44:00.292060 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_stack.py
+-rw-r--r--   0        0        0     1479 2024-03-23 20:43:59.951065 ecs_composex-1.1.0rc3/ecs_composex/kms/kms_template.py
+-rw-r--r--   0        0        0      826 2024-04-15 08:30:37.402572 ecs_composex-1.1.0rc3/ecs_composex/kms/x-kms.spec.json
+-rw-r--r--   0        0        0    12383 2024-03-23 20:43:59.988065 ecs_composex-1.1.0rc3/ecs_composex/mods_manager.py
+-rw-r--r--   0        0        0       90 2024-03-23 20:44:00.052064 ecs_composex-1.1.0rc3/ecs_composex/neptune/__init__.py
+-rw-r--r--   0        0        0      478 2024-03-23 20:44:00.208062 ecs_composex-1.1.0rc3/ecs_composex/neptune/neptune_module.py
+-rw-r--r--   0        0        0      864 2024-03-23 20:43:59.941066 ecs_composex-1.1.0rc3/ecs_composex/neptune/neptune_params.py
+-rw-r--r--   0        0        0      337 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/neptune/neptune_perms.json
+-rw-r--r--   0        0        0     9212 2024-03-23 20:44:00.459057 ecs_composex-1.1.0rc3/ecs_composex/neptune/neptune_stack.py
+-rw-r--r--   0        0        0     5088 2024-03-23 20:44:00.250061 ecs_composex-1.1.0rc3/ecs_composex/neptune/neptune_template.py
+-rw-r--r--   0        0        0     3013 2024-04-15 08:30:37.404572 ecs_composex-1.1.0rc3/ecs_composex/neptune/x-neptune.spec.json
+-rw-r--r--   0        0        0      488 2024-03-23 20:43:59.858067 ecs_composex-1.1.0rc3/ecs_composex/opensearch/__init__.py
+-rw-r--r--   0        0        0     2441 2024-03-23 20:44:00.188062 ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_aws.py
+-rw-r--r--   0        0        0      487 2024-03-23 20:43:59.981065 ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_module.py
+-rw-r--r--   0        0        0      950 2024-03-23 20:44:00.007065 ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_params.py
+-rw-r--r--   0        0        0      983 2024-04-15 08:30:37.406572 ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_perms.json
+-rw-r--r--   0        0        0     6315 2024-03-23 20:44:00.073063 ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_stack.py
+-rw-r--r--   0        0        0    22533 2024-03-23 20:44:00.325060 ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_template.py
+-rw-r--r--   0        0        0     3216 2024-04-15 08:30:37.406572 ecs_composex-1.1.0rc3/ecs_composex/opensearch/x-opensearch.spec.json
+-rw-r--r--   0        0        0       19 2021-03-04 09:40:13.444136 ecs_composex-1.1.0rc3/ecs_composex/rds/.gitignore
+-rw-r--r--   0        0        0      146 2024-03-23 20:43:59.813068 ecs_composex-1.1.0rc3/ecs_composex/rds/__init__.py
+-rw-r--r--   0        0        0     1703 2024-03-23 20:44:00.465057 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_conditions.py
+-rw-r--r--   0        0        0    20461 2024-03-23 20:43:59.939066 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_db_template.py
+-rw-r--r--   0        0        0     5939 2024-03-23 20:44:00.180062 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_features.py
+-rw-r--r--   0        0        0     5448 2024-03-23 20:44:00.509057 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_features_define.py
+-rw-r--r--   0        0        0      455 2024-03-23 20:44:00.417058 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_module.py
+-rw-r--r--   0        0        0     3624 2024-03-23 20:44:00.146062 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_parameter_groups_helper.py
+-rw-r--r--   0        0        0     2898 2024-03-23 20:44:00.305060 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_params.py
+-rw-r--r--   0        0        0      164 2024-04-15 08:30:37.406572 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_perms.json
+-rw-r--r--   0        0        0    10438 2024-03-23 20:43:59.953065 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_stack.py
+-rw-r--r--   0        0        0     4557 2024-03-23 20:44:00.164062 ecs_composex-1.1.0rc3/ecs_composex/rds/rds_template.py
+-rw-r--r--   0        0        0     5948 2024-04-15 08:30:37.406572 ecs_composex-1.1.0rc3/ecs_composex/rds/x-rds.spec.json
+-rw-r--r--   0        0        0    22462 2024-04-14 21:58:44.889124 ecs_composex-1.1.0rc3/ecs_composex/rds_resources_settings.py
+-rw-r--r--   0        0        0    27883 2024-03-23 22:36:48.973815 ecs_composex-1.1.0rc3/ecs_composex/resource_settings.py
+-rw-r--r--   0        0        0     8660 2024-03-23 20:44:00.440058 ecs_composex-1.1.0rc3/ecs_composex/resources_import.py
+-rw-r--r--   0        0        0        0 2022-06-16 20:44:41.834935 ecs_composex-1.1.0rc3/ecs_composex/route53/__init__.py
+-rw-r--r--   0        0        0     4385 2024-03-23 20:44:00.037064 ecs_composex-1.1.0rc3/ecs_composex/route53/route53_acm.py
+-rw-r--r--   0        0        0     5433 2024-03-23 20:44:00.134063 ecs_composex-1.1.0rc3/ecs_composex/route53/route53_elbv2.py
+-rw-r--r--   0        0        0     3983 2024-03-23 20:44:00.371059 ecs_composex-1.1.0rc3/ecs_composex/route53/route53_helpers.py
+-rw-r--r--   0        0        0      429 2024-03-23 20:44:00.303060 ecs_composex-1.1.0rc3/ecs_composex/route53/route53_module.py
+-rw-r--r--   0        0        0     1136 2024-03-23 20:44:00.154062 ecs_composex-1.1.0rc3/ecs_composex/route53/route53_params.py
+-rw-r--r--   0        0        0     7828 2024-03-23 20:44:00.448058 ecs_composex-1.1.0rc3/ecs_composex/route53/route53_stack.py
+-rw-r--r--   0        0        0     1476 2024-04-15 08:30:37.405572 ecs_composex-1.1.0rc3/ecs_composex/route53/x-route53.spec.json
+-rw-r--r--   0        0        0      283 2024-03-23 20:44:00.111063 ecs_composex-1.1.0rc3/ecs_composex/s3/__init__.py
+-rw-r--r--   0        0        0     7451 2024-03-23 20:43:59.913066 ecs_composex-1.1.0rc3/ecs_composex/s3/s3_bucket.py
+-rw-r--r--   0        0        0     2581 2024-03-23 20:44:00.033064 ecs_composex-1.1.0rc3/ecs_composex/s3/s3_ecs_cluster.py
+-rw-r--r--   0        0        0     3848 2024-03-23 20:44:00.307060 ecs_composex-1.1.0rc3/ecs_composex/s3/s3_kinesis_firehose.py
+-rw-r--r--   0        0        0      406 2024-03-23 20:44:00.105063 ecs_composex-1.1.0rc3/ecs_composex/s3/s3_module.py
+-rw-r--r--   0        0        0     2289 2024-03-23 20:44:00.031064 ecs_composex-1.1.0rc3/ecs_composex/s3/s3_params.py
+-rw-r--r--   0        0        0     3566 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/s3/s3_perms.json
+-rw-r--r--   0        0        0     5135 2024-03-23 20:44:00.438058 ecs_composex-1.1.0rc3/ecs_composex/s3/s3_stack.py
+-rw-r--r--   0        0        0     7858 2024-03-23 20:44:00.115063 ecs_composex-1.1.0rc3/ecs_composex/s3/s3_template.py
+-rw-r--r--   0        0        0     3232 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/s3/x-s3.spec.json
+-rw-r--r--   0        0        0     2948 2024-03-23 20:44:00.003065 ecs_composex-1.1.0rc3/ecs_composex/secrets/__init__.py
+-rw-r--r--   0        0        0     2005 2024-03-23 20:44:00.198062 ecs_composex-1.1.0rc3/ecs_composex/secrets/secrets_aws.py
+-rw-r--r--   0        0        0      493 2024-03-23 20:44:00.290060 ecs_composex-1.1.0rc3/ecs_composex/secrets/secrets_params.py
+-rw-r--r--   0        0        0      284 2024-03-23 20:44:00.338060 ecs_composex-1.1.0rc3/ecs_composex/sns/__init__.py
+-rw-r--r--   0        0        0     2625 2024-03-23 20:44:00.218061 ecs_composex-1.1.0rc3/ecs_composex/sns/sns_helpers.py
+-rw-r--r--   0        0        0      407 2024-03-23 20:43:59.872067 ecs_composex-1.1.0rc3/ecs_composex/sns/sns_module.py
+-rw-r--r--   0        0        0      698 2024-03-23 20:44:00.257061 ecs_composex-1.1.0rc3/ecs_composex/sns/sns_params.py
+-rw-r--r--   0        0        0      128 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/sns/sns_perms.json
+-rw-r--r--   0        0        0     2377 2024-03-23 20:44:00.233061 ecs_composex-1.1.0rc3/ecs_composex/sns/sns_stack.py
+-rw-r--r--   0        0        0     1286 2024-03-23 20:43:59.823068 ecs_composex-1.1.0rc3/ecs_composex/sns/sns_templates.py
+-rw-r--r--   0        0        0      696 2024-04-15 08:30:37.403572 ecs_composex-1.1.0rc3/ecs_composex/sns/x-sns.spec.json
+-rw-r--r--   0        0        0      281 2024-03-23 20:44:00.446058 ecs_composex-1.1.0rc3/ecs_composex/specs/__init__.py
+-rw-r--r--   0        0        0      742 2024-03-23 20:44:00.143062 ecs_composex-1.1.0rc3/ecs_composex/specs/_core.py
+-rw-r--r--   0        0        0    29055 2024-04-15 08:30:37.400572 ecs_composex-1.1.0rc3/ecs_composex/specs/compose-spec.json
+-rw-r--r--   0        0        0     2455 2024-04-15 08:30:37.401572 ecs_composex-1.1.0rc3/ecs_composex/specs/ingress.spec.json
+-rw-r--r--   0        0        0     1234 2024-04-15 08:30:37.401572 ecs_composex-1.1.0rc3/ecs_composex/specs/secrets.x-secrets.spec.json
+-rw-r--r--   0        0        0     2266 2024-04-15 08:30:37.401572 ecs_composex-1.1.0rc3/ecs_composex/specs/services-xray.spec.json
+-rw-r--r--   0        0        0     1404 2024-04-15 08:30:37.399572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-alarms.spec.json
+-rw-r--r--   0        0        0      403 2024-04-15 08:30:37.400572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-codeguru_profiler.spec.json
+-rw-r--r--   0        0        0      501 2024-04-15 08:30:37.400572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-docker_opts.spec.json
+-rw-r--r--   0        0        0     1853 2024-04-15 08:30:37.399572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-ecr.spec.json
+-rw-r--r--   0        0        0     2745 2024-04-15 08:30:37.399572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-ecs.spec.json
+-rw-r--r--   0        0        0      836 2024-04-15 08:30:37.401572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-environment.spec.json
+-rw-r--r--   0        0        0     2175 2024-04-15 08:30:37.400572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-iam.spec.json
+-rw-r--r--   0        0        0     7429 2024-04-15 08:30:37.401572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-logging.spec.json
+-rw-r--r--   0        0        0     1986 2024-04-15 08:30:37.401572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-monitoring.spec.json
+-rw-r--r--   0        0        0     4477 2024-04-15 08:30:37.399572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-network.spec.json
+-rw-r--r--   0        0        0     4724 2024-04-15 08:30:37.400572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-prometheus.spec.json
+-rw-r--r--   0        0        0     4105 2024-04-15 08:30:37.399572 ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-scaling.spec.json
+-rw-r--r--   0        0        0     2133 2024-04-15 08:30:37.400572 ecs_composex-1.1.0rc3/ecs_composex/specs/x-cluster.spec.json
+-rw-r--r--   0        0        0     6706 2024-04-15 08:30:37.400572 ecs_composex-1.1.0rc3/ecs_composex/specs/x-rds-common.spec.json
+-rw-r--r--   0        0        0     6559 2024-04-15 08:30:37.401572 ecs_composex-1.1.0rc3/ecs_composex/specs/x-resources.common.spec.json
+-rw-r--r--   0        0        0      816 2024-04-15 08:30:37.400572 ecs_composex-1.1.0rc3/ecs_composex/specs/x-tags.spec.json
+-rw-r--r--   0        0        0      285 2024-03-23 20:44:00.279060 ecs_composex-1.1.0rc3/ecs_composex/sqs/__init__.py
+-rw-r--r--   0        0        0     4737 2024-03-23 20:43:59.937066 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_ecs_scaling.py
+-rw-r--r--   0        0        0     3592 2024-03-23 20:43:59.890066 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_helpers.py
+-rw-r--r--   0        0        0      407 2024-03-23 20:43:59.836067 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_module.py
+-rw-r--r--   0        0        0      865 2024-03-23 20:44:00.141063 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_params.py
+-rw-r--r--   0        0        0      515 2024-04-15 08:30:37.404572 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_perms.json
+-rw-r--r--   0        0        0     5463 2024-03-23 20:44:00.050064 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_s3.py
+-rw-r--r--   0        0        0     2938 2024-03-23 20:44:00.383059 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_sqs.py
+-rw-r--r--   0        0        0     4375 2024-03-23 20:43:59.917066 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_stack.py
+-rw-r--r--   0        0        0     7648 2024-03-23 20:44:00.273060 ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_template.py
+-rw-r--r--   0        0        0      744 2024-04-15 08:30:37.404572 ecs_composex-1.1.0rc3/ecs_composex/sqs/x-sqs.spec.json
+-rw-r--r--   0        0        0      488 2024-03-23 20:44:00.020064 ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/__init__.py
+-rw-r--r--   0        0        0     5154 2024-03-23 20:44:00.195062 ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_helpers.py
+-rw-r--r--   0        0        0      488 2024-03-23 20:43:59.935066 ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_module.py
+-rw-r--r--   0        0        0      905 2024-03-23 20:44:00.263061 ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_params.py
+-rw-r--r--   0        0        0      820 2024-04-15 08:30:37.399572 ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_perms.json
+-rw-r--r--   0        0        0     3924 2024-03-23 20:44:00.011065 ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_stack.py
+-rw-r--r--   0        0        0     2243 2024-04-15 08:30:37.399572 ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/x-ssm_parameter.spec.json
+-rw-r--r--   0        0        0       88 2024-03-23 20:44:00.296060 ecs_composex-1.1.0rc3/ecs_composex/utils/__init__.py
+-rw-r--r--   0        0        0      820 2024-03-23 20:44:00.344059 ecs_composex-1.1.0rc3/ecs_composex/utils/init_ecs.py
+-rw-r--r--   0        0        0     1797 2024-03-23 20:43:59.992065 ecs_composex-1.1.0rc3/ecs_composex/utils/init_s3.py
+-rw-r--r--   0        0        0      284 2024-03-23 20:44:00.497057 ecs_composex-1.1.0rc3/ecs_composex/vpc/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-23 20:44:00.255061 ecs_composex-1.1.0rc3/ecs_composex/vpc/aws_mappings.py
+-rw-r--r--   0        0        0     3997 2024-03-23 20:43:59.919066 ecs_composex-1.1.0rc3/ecs_composex/vpc/helpers.py
+-rw-r--r--   0        0        0     5154 2024-03-23 20:44:00.071064 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_aws.py
+-rw-r--r--   0        0        0     1338 2024-03-23 20:44:00.357059 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_cloudmap.py
+-rw-r--r--   0        0        0       88 2024-03-23 20:43:59.834067 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_conditions.py
+-rw-r--r--   0        0        0     1953 2024-03-23 20:44:00.377059 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_maths.py
+-rw-r--r--   0        0        0      423 2024-03-23 20:44:00.499057 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_module.py
+-rw-r--r--   0        0        0     2217 2024-03-23 20:44:00.253061 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_params.py
+-rw-r--r--   0        0        0    14983 2024-03-23 20:44:00.442058 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_stack.py
+-rw-r--r--   0        0        0    10517 2024-03-23 20:44:00.161062 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_subnets.py
+-rw-r--r--   0        0        0     4709 2024-03-23 20:44:00.109063 ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_template.py
+-rw-r--r--   0        0        0     3504 2024-04-15 08:30:37.405572 ecs_composex-1.1.0rc3/ecs_composex/vpc/x-vpc.spec.json
+-rw-r--r--   0        0        0       90 2024-03-23 20:44:00.336059 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/__init__.py
+-rw-r--r--   0        0        0      697 2024-03-23 20:44:00.119063 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/validators_wafv2.py
+-rw-r--r--   0        0        0     2255 2024-03-23 20:44:00.288060 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_elbv2.py
+-rw-r--r--   0        0        0      497 2024-03-23 20:44:00.169062 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_module.py
+-rw-r--r--   0        0        0     1079 2024-03-23 20:43:59.850067 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_params.py
+-rw-r--r--   0        0        0      185 2024-04-15 08:30:37.404572 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_perms.json
+-rw-r--r--   0        0        0     9460 2024-03-23 20:44:00.373059 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_stack.py
+-rw-r--r--   0        0        0     1357 2024-03-23 20:44:00.423058 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_template.py
+-rw-r--r--   0        0        0     1772 2024-04-15 08:30:37.404572 ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/x-wafv2_webacl.spec.json
+-rw-r--r--   0        0        0     3476 2024-04-15 08:30:36.452587 ecs_composex-1.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     8907 1970-01-01 00:00:00.000000 ecs_composex-1.1.0rc3/PKG-INFO
```

### Comparing `ecs_composex-1.1.0rc2/LICENSE` & `ecs_composex-1.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/NOTICES.rst` & `ecs_composex-1.1.0rc3/NOTICES.rst`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/README.rst` & `ecs_composex-1.1.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/acm/acm_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/acm/acm_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/acm/acm_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/acm/acm_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/acm/acm_stack_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/acm/acm_stack_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/acm/x-acm.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/acm/x-acm.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_ecs.py` & `ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_elbv2.py` & `ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_elbv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/alarms/alarms_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/alarms/alarms_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/alarms/x-alarms.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/alarms/x-alarms.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_aws.py` & `ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_conditions.py` & `ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_mesh.py` & `ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_mesh.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_node.py` & `ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_node.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_router.py` & `ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_router.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/appmesh/appmesh_service.py` & `ecs_composex-1.1.0rc3/ecs_composex/appmesh/appmesh_service.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/appmesh/x-appmesh.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/appmesh/x-appmesh.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/aps/aps_parameters.py` & `ecs_composex-1.1.0rc3/ecs_composex/aps/aps_parameters.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/aps/aps_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/aps/aps_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/aps/x-aps.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/aps/x-aps.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cli.py` & `ecs_composex-1.1.0rc3/ecs_composex/cli.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_ecs.py` & `ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/cloudmap_x_resources.py` & `ecs_composex-1.1.0rc3/ecs_composex/cloudmap/cloudmap_x_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cloudmap/x-cloudmap.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/cloudmap/x-cloudmap.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_aws.py` & `ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/codeguru_profiler_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/codeguru_profiler_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/codeguru_profiler/codeguru_profiler_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/codeguru_profiler/codeguru_profiler_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/cognito_userpool/cognito_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/cognito_userpool/cognito_userpool_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/cognito_userpool/cognito_userpool_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/aws.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/cfn_conditions.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/cfn_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/cfn_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/cfn_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/envsubst.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/envsubst.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/files.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/files.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/logging.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/logging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/settings.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/settings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/stacks/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/tagging.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/tagging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/common/troposphere_tools.py` & `ecs_composex-1.1.0rc3/ecs_composex/common/troposphere_tools.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_networks.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_networks.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/ecs_family_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_secrets/ecs_family_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_secrets/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_secrets/services_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_secrets/services_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/docker_tools.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/docker_tools.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/env_files_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/env_files_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/kernel_options_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/kernel_options_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_image/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/docker_opts.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_image/docker_opts.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/ecr_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_image/ecr_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_image/ecr_scans_eval.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_image/ecr_scans_eval.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_logging/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_services/service_logging/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_services/service_logging/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_volumes/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/ecs_family_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_volumes/ecs_family_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_volumes/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/compose_volumes/services_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/compose_volumes/services_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/api_x_resources.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/api_x_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/environment_x_resources.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/environment_x_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/network_x_resources.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/network_x_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/compose/x_resources/services_resources.py` & `ecs_composex-1.1.0rc3/ecs_composex/compose/x_resources/services_resources.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_services_metrics.py` & `ecs_composex-1.1.0rc3/ecs_composex/dashboards/dashboards_services_metrics.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/dashboards/dashboards_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/dashboards/dashboards_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/dashboards/x-dashboards.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/dashboards/x-dashboards.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/docdb/docdb_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/docdb/docdb_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/docdb/docdb_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/docdb/docdb_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/docdb/x-docdb.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/docdb/x-docdb.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_autoscaling.py` & `ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_autoscaling.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_perms.json` & `ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/dynamodb_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/dynamodb/dynamodb_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/dynamodb/x-dynamodb.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/dynamodb/x-dynamodb.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_conditions.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/compute_finalizers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_helpers/compute_finalizers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_helpers/network_finalizers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_helpers/network_finalizers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_logging/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_logging/cw_logging.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_logging/cw_logging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/family_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/family_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/task_execute_command.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/task_execute_command.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_family/task_runtime.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_family/task_runtime.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_firehose.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_firehose.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_kinesis.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/advanced_kinesis.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/config_parameter.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/config_parameter.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/family_fluentbit_managed_config.j2` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/family_fluentbit_managed_config.j2`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/firelens_config_sidecar.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/firelens_config_sidecar.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/service_fluentbit_managed_config.j2` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/ecs_firelens_advanced/service_fluentbit_managed_config.j2`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_advanced_rendered_settings.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/firelens_advanced_rendered_settings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_logger_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/firelens_logger_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_managed_sidecar_service.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/firelens_managed_sidecar_service.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/firelens_options_generic_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/firelens_options_generic_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/cloudwatch_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/helpers/cloudwatch_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/firehose_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/helpers/firehose_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_firelens/helpers/kinesis_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_firelens/helpers/kinesis_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/config_ssm_parameters.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_prometheus/config_ssm_parameters.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/emf_processors.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_prometheus/emf_processors.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_prometheus/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_prometheus/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_service/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_service/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_service/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_service/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/ecs_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/ecs_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/helpers/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/managed_sidecars/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/aws_cw_agent.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/managed_sidecars/aws_cw_agent.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/aws_xray.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/managed_sidecars/aws_xray.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/managed_sidecars/nginx_prometheus_exporter.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/managed_sidecars/nginx_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_alarms/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_alarms/service_predefined_alarms.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_alarms/service_predefined_alarms.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_compute/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_compute/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_compute/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_networking/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_networking/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_networking/ingress_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_networking/ingress_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_scaling/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_scaling/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/service_scaling/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/service_scaling/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_compute/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/task_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_compute/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/task_compute/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/task_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/task_iam/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs/task_iam/task_role.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs/task_iam/task_role.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/ecs_family_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs_cluster/ecs_family_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs_cluster/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs_cluster/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs_composex.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs_composex.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ecs_ingress/ecs_ingress_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/ecs_ingress/ecs_ingress_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 f"SG for {family.logical_name} in ${{ROOT_STACK}}",
                 ROOT_STACK=define_stack_name(sgs_stack.stack_template),
             ),
             VpcId=Ref(VPC_ID),
             Tags=Tags(
                 {
                     "Name": Sub(
-                        f"${family.logical_name}-${{STACK_NAME}}",
+                        f"{family.logical_name}-${{STACK_NAME}}",
                         STACK_NAME=define_stack_name(),
                     ),
                     "compose-x:family-name": family.name,
                     "compose-x:family-logical-name": family.logical_name,
                 }
             ),
         )
```

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/efs/efs_ecs.py` & `ecs_composex-1.1.0rc3/ecs_composex/efs/efs_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/efs/efs_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/efs/efs_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/efs/efs_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/efs/efs_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/efs/x-efs.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/efs/x-efs.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_aws.py` & `ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_ecs.py` & `ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elasticache/elasticache_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/elasticache/elasticache_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_ecs.py` & `ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2.py` & `ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/elbv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2_listener/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/elbv2_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/elbv2_listener/lookup_listener.py` & `ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/elbv2_listener/lookup_listener.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elbv2/elbv2_stack/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/elbv2/elbv2_stack/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/elbv2/x-elbv2.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/elbv2/x-elbv2.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/events/events_ecs.py` & `ecs_composex-1.1.0rc3/ecs_composex/events/events_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/events/events_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/events/events_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/events/events_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/events/events_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/events/x-events.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/events/x-events.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/iam/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/iam/iam_ecs_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/iam/iam_ecs_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/iam/iam_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/iam/iam_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/iam/iam_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/iam/iam_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/iam/import_sam_policies.py` & `ecs_composex-1.1.0rc3/ecs_composex/iam/import_sam_policies.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/iam/sam_policies.json` & `ecs_composex-1.1.0rc3/ecs_composex/iam/sam_policies.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ingress_settings.py` & `ecs_composex-1.1.0rc3/ecs_composex/ingress_settings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kcl_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis/kcl_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_kinesis_firehose.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_kinesis_firehose.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_perms.json` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis/kinesis_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis/kinesis_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis/x-kinesis.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis/x-kinesis.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_iam_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_iam_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_logging_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_logging_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/kinesis_firehose_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/kinesis_firehose_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kinesis_firehose/x-kinesis_firehose.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/kinesis_firehose/x-kinesis_firehose.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_ecs_cluster.py` & `ecs_composex-1.1.0rc3/ecs_composex/kms/kms_ecs_cluster.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_kinesis_firehose.py` & `ecs_composex-1.1.0rc3/ecs_composex/kms/kms_kinesis_firehose.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/kms/kms_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_perms.json` & `ecs_composex-1.1.0rc3/ecs_composex/kms/kms_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_s3.py` & `ecs_composex-1.1.0rc3/ecs_composex/kms/kms_s3.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_sqs.py` & `ecs_composex-1.1.0rc3/ecs_composex/kms/kms_sqs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/kms/kms_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/kms_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/kms/kms_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/kms/x-kms.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/kms/x-kms.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/mods_manager.py` & `ecs_composex-1.1.0rc3/ecs_composex/mods_manager.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/neptune/neptune_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/neptune/neptune_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/neptune/neptune_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/neptune/neptune_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/neptune/x-neptune.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/neptune/x-neptune.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_aws.py` & `ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_perms.json` & `ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/opensearch/opensearch_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/opensearch/opensearch_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/opensearch/x-opensearch.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/opensearch/x-opensearch.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_conditions.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds/rds_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_db_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds/rds_db_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_features.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds/rds_features.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_features_define.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds/rds_features_define.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_parameter_groups_helper.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds/rds_parameter_groups_helper.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds/rds_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds/rds_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/rds_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds/rds_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds/x-rds.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/rds/x-rds.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/rds_resources_settings.py` & `ecs_composex-1.1.0rc3/ecs_composex/rds_resources_settings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/resource_settings.py` & `ecs_composex-1.1.0rc3/ecs_composex/resource_settings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/resources_import.py` & `ecs_composex-1.1.0rc3/ecs_composex/resources_import.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_acm.py` & `ecs_composex-1.1.0rc3/ecs_composex/route53/route53_acm.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_elbv2.py` & `ecs_composex-1.1.0rc3/ecs_composex/route53/route53_elbv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/route53/route53_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/route53/route53_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/route53/route53_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/route53/route53_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/route53/x-route53.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/route53/x-route53.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_bucket.py` & `ecs_composex-1.1.0rc3/ecs_composex/s3/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_ecs_cluster.py` & `ecs_composex-1.1.0rc3/ecs_composex/s3/s3_ecs_cluster.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_kinesis_firehose.py` & `ecs_composex-1.1.0rc3/ecs_composex/s3/s3_kinesis_firehose.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/s3/s3_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_perms.json` & `ecs_composex-1.1.0rc3/ecs_composex/s3/s3_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/s3/s3_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/s3/s3_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/s3/s3_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/s3/x-s3.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/s3/x-s3.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/secrets/__init__.py` & `ecs_composex-1.1.0rc3/ecs_composex/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/secrets/secrets_aws.py` & `ecs_composex-1.1.0rc3/ecs_composex/secrets/secrets_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sns/sns_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/sns/sns_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sns/sns_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/sns/sns_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sns/sns_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/sns/sns_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sns/sns_templates.py` & `ecs_composex-1.1.0rc3/ecs_composex/sns/sns_templates.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sns/x-sns.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/sns/x-sns.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/_core.py` & `ecs_composex-1.1.0rc3/ecs_composex/specs/_core.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/compose-spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/compose-spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/ingress.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/ingress.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/secrets.x-secrets.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/secrets.x-secrets.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services-xray.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services-xray.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-alarms.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-alarms.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-ecr.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-ecr.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-ecs.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-ecs.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-environment.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-environment.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-iam.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-iam.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-logging.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-logging.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-monitoring.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-monitoring.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-network.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-network.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-prometheus.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-prometheus.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/services.x-scaling.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/services.x-scaling.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/x-cluster.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/x-cluster.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/x-rds-common.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/x-rds-common.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/x-resources.common.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/x-resources.common.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/specs/x-tags.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/specs/x-tags.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_ecs_scaling.py` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_ecs_scaling.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_perms.json` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_s3.py` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_s3.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_sqs.py` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_sqs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/sqs_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/sqs_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/sqs/x-sqs.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/sqs/x-sqs.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_perms.json` & `ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_perms.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/ssm_parameter_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/ssm_parameter_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/ssm_parameter/x-ssm_parameter.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/ssm_parameter/x-ssm_parameter.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/utils/init_ecs.py` & `ecs_composex-1.1.0rc3/ecs_composex/utils/init_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/utils/init_s3.py` & `ecs_composex-1.1.0rc3/ecs_composex/utils/init_s3.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/aws_mappings.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/aws_mappings.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/helpers.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/helpers.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_aws.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_aws.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_cloudmap.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_cloudmap.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_maths.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_maths.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_subnets.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_subnets.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/vpc_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/vpc_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/vpc/x-vpc.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/vpc/x-vpc.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/validators_wafv2.py` & `ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/validators_wafv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_elbv2.py` & `ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_elbv2.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_params.py` & `ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_params.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_stack.py` & `ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/wafv2_webacl_template.py` & `ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/wafv2_webacl_template.py`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/ecs_composex/wafv2_webacl/x-wafv2_webacl.spec.json` & `ecs_composex-1.1.0rc3/ecs_composex/wafv2_webacl/x-wafv2_webacl.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex-1.1.0rc2/pyproject.toml` & `ecs_composex-1.1.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_composex"
-version = "1.1.0-rc2"
+version = "1.1.0-rc3"
 description = "Manage, Configure and Deploy your services and AWS services and applications from your docker-compose definition"
 authors = ["John Preston <john@compose-x.io>"]
 maintainers = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 readme = "README.rst"
 keywords = ["compose-x", "aws", "cloudformation", "docker", "compose"]
 classifiers = [
@@ -80,15 +80,15 @@
 sphinx-jsonschema = "^1.19.1"
 sphinx-material = "^0.0.35"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecs_composex"
 
 [tool.tbump.version]
-current = "1.1.0-rc2"
+current = "1.1.0-rc3"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `ecs_composex-1.1.0rc2/PKG-INFO` & `ecs_composex-1.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs_composex
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: Manage, Configure and Deploy your services and AWS services and applications from your docker-compose definition
 License: MPL-2.0
 Keywords: compose-x,aws,cloudformation,docker,compose
 Author: John Preston
 Author-email: john@compose-x.io
 Maintainer: John Preston
 Maintainer-email: john@compose-x.io
```

