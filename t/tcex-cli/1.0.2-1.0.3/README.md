# Comparing `tmp/tcex_cli-1.0.2.tar.gz` & `tmp/tcex_cli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcex_cli-1.0.2.tar", last modified: Mon Sep 18 21:53:03 2023, max compression
+gzip compressed data, was "tcex_cli-1.0.3.tar", last modified: Wed Apr 17 16:18:24 2024, max compression
```

## Comparing `tcex_cli-1.0.2.tar` & `tcex_cli-1.0.3.tar`

### file list

```diff
@@ -1,185 +1,189 @@
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.630439 tcex_cli-1.0.2/
--rw-rw-r--   0 bsummers   (503) staff       (20)    11357 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/LICENSE
--rw-r--r--   0 bsummers   (503) staff       (20)     3407 2023-09-18 21:53:03.629830 tcex_cli-1.0.2/PKG-INFO
--rw-rw-r--   0 bsummers   (503) staff       (20)     1710 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/README.md
--rw-rw-r--   0 bsummers   (503) staff       (20)     3552 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/pyproject.toml
--rw-rw-r--   0 bsummers   (503) staff       (20)       38 2023-09-18 21:53:03.630570 tcex_cli-1.0.2/setup.cfg
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.080534 tcex_cli-1.0.2/tcex_cli/
--rw-rw-r--   0 bsummers   (503) staff       (20)     1659 2023-03-31 01:13:13.000000 tcex_cli-1.0.2/tcex_cli/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)       80 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/__metadata__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.106129 tcex_cli-1.0.2/tcex_cli/app/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/app/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2385 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/app/app.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.133016 tcex_cli-1.0.2/tcex_cli/app/config/
--rw-rw-r--   0 bsummers   (503) staff       (20)      331 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    18720 2023-09-18 21:52:19.000000 tcex_cli-1.0.2/tcex_cli/app/config/app_spec_yml.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9253 2023-07-27 00:00:15.000000 tcex_cli-1.0.2/tcex_cli/app/config/install_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4215 2023-09-18 21:52:19.000000 tcex_cli-1.0.2/tcex_cli/app/config/install_json_update.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1558 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/install_json_validate.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1598 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/job_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4504 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/layout_json.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.164403 tcex_cli-1.0.2/tcex_cli/app/config/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)      382 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13740 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/model/app_spec_yml_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    35922 2023-08-25 18:13:07.000000 tcex_cli-1.0.2/tcex_cli/app/config/model/install_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2942 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/model/job_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2921 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/model/layout_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1120 2023-08-25 18:13:07.000000 tcex_cli-1.0.2/tcex_cli/app/config/model/tcex_json_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    24522 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/permutation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2070 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/app/config/tcex_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2469 2023-04-12 21:00:12.000000 tcex_cli-1.0.2/tcex_cli/app/config/tcex_json_update.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.173186 tcex_cli-1.0.2/tcex_cli/cli/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3210 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/cli.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3697 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/cli_abc.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.179714 tcex_cli-1.0.2/tcex_cli/cli/deploy/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/deploy/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1953 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/deploy/deploy.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5326 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/deploy/deploy_cli.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.196202 tcex_cli-1.0.2/tcex_cli/cli/deps/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/deps/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2383 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/deps/deps.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    14461 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/deps/deps_cli.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.214435 tcex_cli-1.0.2/tcex_cli/cli/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      220 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/model/app_metadata_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      901 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/model/file_metadata_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      164 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/model/key_value_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1093 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/model/validation_data_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.223967 tcex_cli-1.0.2/tcex_cli/cli/package/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/package/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2983 2023-04-07 18:36:45.000000 tcex_cli-1.0.2/tcex_cli/cli/package/package.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8222 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/package/package_cli.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.305510 tcex_cli-1.0.2/tcex_cli/cli/run/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6863 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/run/launch_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      513 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/launch_organization.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1439 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/launch_playbook.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8921 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_api.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4714 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_common_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4503 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_common_trigger_abc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2494 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_custom_trigger.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4312 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_webhook_trigger.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.373486 tcex_cli-1.0.2/tcex_cli/cli/run/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1790 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/api_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1400 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/app_api_service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      890 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/app_organization_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1104 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/app_playbook_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      972 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/app_trigger_service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1249 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/app_webhook_trigger_service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      566 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/batch_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      376 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/common_app_input_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      488 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/common_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      545 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/logging_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      322 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/module_request_tc_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      392 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/organization_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      541 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/path_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      538 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/playbook_common_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      711 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/playbook_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      707 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/proxy_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      947 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/model/service_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     8946 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/playbook_create.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5917 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/request_handler_api.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3747 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/request_handler_webhook.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1081 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/run/run.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5027 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/run/run_cli.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2988 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/run/web_server.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.407548 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    20695 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_app_input.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    12835 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_app_input_static.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    11481 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_app_spec_yml.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5847 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_install_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1300 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_job_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      702 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_layout_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13891 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_readme_md.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      892 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_tcex_json.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1892 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/spec_tool.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     9297 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/spec_tool/spec_tool_cli.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.418567 tcex_cli-1.0.2/tcex_cli/cli/template/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/template/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3408 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/template/init.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2036 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/template/list_.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.424399 tcex_cli-1.0.2/tcex_cli/cli/template/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/template/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1050 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/template/model/template_config_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    25826 2023-09-18 21:50:44.000000 tcex_cli-1.0.2/tcex_cli/cli/template/template_cli.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3231 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/cli/template/update.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.434391 tcex_cli-1.0.2/tcex_cli/cli/validate/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/cli/validate/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1686 2023-04-07 18:36:45.000000 tcex_cli-1.0.2/tcex_cli/cli/validate/validate.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    13325 2023-04-12 21:02:42.000000 tcex_cli-1.0.2/tcex_cli/cli/validate/validate_cli.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.445869 tcex_cli-1.0.2/tcex_cli/input/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.459944 tcex_cli-1.0.2/tcex_cli/input/field_type/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/field_type/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3130 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/field_type/exception.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5602 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/field_type/sensitive.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.483270 tcex_cli-1.0.2/tcex_cli/input/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2994 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/model/api_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      546 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/model/module_app_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      388 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/model/module_requests_session_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1097 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/model/path_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1040 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/input/model/playbook_common_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      833 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/input/model/playbook_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1256 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/input/model/proxy_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.506554 tcex_cli-1.0.2/tcex_cli/logger/
--rw-rw-r--   0 bsummers   (503) staff       (20)      171 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/logger/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1904 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/logger/rotating_file_handler_custom.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      969 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/logger/sensitive_filter.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1582 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/logger/test_logger.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1257 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/logger/trace_logger.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.515224 tcex_cli-1.0.2/tcex_cli/message_broker/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/message_broker/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10410 2023-07-26 23:51:46.000000 tcex_cli-1.0.2/tcex_cli/message_broker/mqtt_message_broker.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.549980 tcex_cli-1.0.2/tcex_cli/pleb/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      936 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/cached_property.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1647 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/env_path.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      817 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/event.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      758 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/exception_thread.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      285 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/none_model.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1372 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/proxies.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2749 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/scoped_property.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      418 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/pleb/singleton.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5873 2023-04-01 13:14:35.000000 tcex_cli-1.0.2/tcex_cli/registry.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.555157 tcex_cli-1.0.2/tcex_cli/render/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.2/tcex_cli/render/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     6942 2023-08-25 18:12:50.000000 tcex_cli-1.0.2/tcex_cli/render/render.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.563822 tcex_cli-1.0.2/tcex_cli/requests_tc/
--rw-rw-r--   0 bsummers   (503) staff       (20)      137 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/requests_tc/__init__.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.574186 tcex_cli-1.0.2/tcex_cli/requests_tc/auth/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/requests_tc/auth/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1606 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/requests_tc/auth/hmac_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1449 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/requests_tc/auth/tc_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1414 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/requests_tc/auth/token_auth.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     3416 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/requests_tc/requests_tc.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4417 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/requests_tc/tc_session.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.611137 tcex_cli-1.0.2/tcex_cli/util/
--rw-rw-r--   0 bsummers   (503) staff       (20)       71 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1827 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/aes_operation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4044 2023-07-27 00:01:10.000000 tcex_cli-1.0.2/tcex_cli/util/code_operation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)    10014 2023-07-27 00:01:10.000000 tcex_cli-1.0.2/tcex_cli/util/datetime_operation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7162 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/file_operation.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.615134 tcex_cli-1.0.2/tcex_cli/util/model/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/model/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      668 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/model/playbook_variable_model.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.627314 tcex_cli-1.0.2/tcex_cli/util/render/
--rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/render/__init__.py
--rw-rw-r--   0 bsummers   (503) staff       (20)      455 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/render/render.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     4672 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/render/render_panel.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1243 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/render/render_prompt.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     1855 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/render/render_table.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     5807 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/requests_to_curl.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7034 2023-07-27 00:01:10.000000 tcex_cli-1.0.2/tcex_cli/util/string_operation.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     2856 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/util.py
--rw-rw-r--   0 bsummers   (503) staff       (20)     7699 2023-03-31 01:41:44.000000 tcex_cli-1.0.2/tcex_cli/util/variable.py
-drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2023-09-18 21:53:03.098668 tcex_cli-1.0.2/tcex_cli.egg-info/
--rw-r--r--   0 bsummers   (503) staff       (20)     3407 2023-09-18 21:53:02.000000 tcex_cli-1.0.2/tcex_cli.egg-info/PKG-INFO
--rw-rw-r--   0 bsummers   (503) staff       (20)     5515 2023-09-18 21:53:03.000000 tcex_cli-1.0.2/tcex_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)        1 2023-09-18 21:53:02.000000 tcex_cli-1.0.2/tcex_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)       46 2023-09-18 21:53:02.000000 tcex_cli-1.0.2/tcex_cli.egg-info/entry_points.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)      236 2023-09-18 21:53:02.000000 tcex_cli-1.0.2/tcex_cli.egg-info/requires.txt
--rw-rw-r--   0 bsummers   (503) staff       (20)       14 2023-09-18 21:53:02.000000 tcex_cli-1.0.2/tcex_cli.egg-info/top_level.txt
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.434402 tcex_cli-1.0.3/
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11357 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/LICENSE
+-rw-r--r--   0 bsummers   (503) staff       (20)     3422 2024-04-17 16:18:24.433515 tcex_cli-1.0.3/PKG-INFO
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1716 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/README.md
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3725 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/pyproject.toml
+-rw-rw-r--   0 bsummers   (503) staff       (20)       38 2024-04-17 16:18:24.434556 tcex_cli-1.0.3/setup.cfg
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.229045 tcex_cli-1.0.3/tcex_cli/
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1659 2023-03-31 01:13:13.000000 tcex_cli-1.0.3/tcex_cli/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)       81 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/__metadata__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.234919 tcex_cli-1.0.3/tcex_cli/app/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/app/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2385 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/app/app.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.244744 tcex_cli-1.0.3/tcex_cli/app/config/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      331 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    18720 2023-09-18 21:52:19.000000 tcex_cli-1.0.3/tcex_cli/app/config/app_spec_yml.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9253 2023-07-27 00:00:15.000000 tcex_cli-1.0.3/tcex_cli/app/config/install_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4215 2023-09-18 21:52:19.000000 tcex_cli-1.0.3/tcex_cli/app/config/install_json_update.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1558 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/install_json_validate.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1598 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/job_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4504 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/layout_json.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.251632 tcex_cli-1.0.3/tcex_cli/app/config/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      382 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13740 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/model/app_spec_yml_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    36010 2024-04-17 16:18:06.000000 tcex_cli-1.0.3/tcex_cli/app/config/model/install_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2942 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/model/job_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2921 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/model/layout_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1120 2023-08-25 18:13:07.000000 tcex_cli-1.0.3/tcex_cli/app/config/model/tcex_json_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    24583 2024-04-17 16:18:06.000000 tcex_cli-1.0.3/tcex_cli/app/config/permutation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2070 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/app/config/tcex_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2469 2023-04-12 21:00:12.000000 tcex_cli-1.0.3/tcex_cli/app/config/tcex_json_update.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.254742 tcex_cli-1.0.3/tcex_cli/cli/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3291 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/cli.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3697 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/cli_abc.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.267043 tcex_cli-1.0.3/tcex_cli/cli/deploy/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/deploy/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1953 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/deploy/deploy.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5326 2023-09-18 21:50:44.000000 tcex_cli-1.0.3/tcex_cli/cli/deploy/deploy_cli.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.273561 tcex_cli-1.0.3/tcex_cli/cli/deps/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/deps/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2383 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/deps/deps.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    14461 2023-09-18 21:50:44.000000 tcex_cli-1.0.3/tcex_cli/cli/deps/deps_cli.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.279651 tcex_cli-1.0.3/tcex_cli/cli/migrate/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/migrate/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      930 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/migrate/migrate.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    15479 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/migrate/migrate_cli.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.293112 tcex_cli-1.0.3/tcex_cli/cli/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      238 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/model/app_metadata_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      901 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/model/file_metadata_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      164 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/model/key_value_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1093 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/model/validation_data_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.299083 tcex_cli-1.0.3/tcex_cli/cli/package/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/package/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2983 2023-04-07 18:36:45.000000 tcex_cli-1.0.3/tcex_cli/cli/package/package.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8283 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/package/package_cli.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.321066 tcex_cli-1.0.3/tcex_cli/cli/run/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6863 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/run/launch_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      513 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/launch_organization.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1439 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/launch_playbook.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8985 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_api.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4714 2023-09-18 21:50:44.000000 tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_common_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4503 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_common_trigger_abc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2558 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_custom_trigger.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4376 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_webhook_trigger.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.346767 tcex_cli-1.0.3/tcex_cli/cli/run/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1790 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/api_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1400 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/app_api_service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      890 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/app_organization_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1104 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/app_playbook_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      972 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/app_trigger_service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1249 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/app_webhook_trigger_service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      566 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/batch_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      376 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/common_app_input_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      488 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/common_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      545 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/logging_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      322 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/module_request_tc_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      392 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/organization_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      541 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/path_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      538 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/playbook_common_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      711 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/playbook_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      707 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/proxy_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      948 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/run/model/service_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     8946 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/playbook_create.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5917 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/request_handler_api.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3747 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/request_handler_webhook.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1088 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/run/run.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5068 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/run/run_cli.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2988 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/run/web_server.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.361307 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    20695 2023-09-18 21:50:44.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_app_input.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    12835 2023-09-18 21:50:44.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_app_input_static.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    11481 2023-09-18 21:50:44.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_app_spec_yml.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5847 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_install_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1300 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_job_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      702 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_layout_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13891 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_readme_md.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      892 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_tcex_json.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1892 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/spec_tool.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     9297 2023-09-18 21:50:44.000000 tcex_cli-1.0.3/tcex_cli/cli/spec_tool/spec_tool_cli.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.368369 tcex_cli-1.0.3/tcex_cli/cli/template/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/template/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3408 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/template/init.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2036 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/template/list_.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.370654 tcex_cli-1.0.3/tcex_cli/cli/template/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/template/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1050 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/template/model/template_config_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    25826 2023-09-18 21:50:44.000000 tcex_cli-1.0.3/tcex_cli/cli/template/template_cli.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3231 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/cli/template/update.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.374159 tcex_cli-1.0.3/tcex_cli/cli/validate/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/cli/validate/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1686 2023-04-07 18:36:45.000000 tcex_cli-1.0.3/tcex_cli/cli/validate/validate.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    13358 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/cli/validate/validate_cli.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.375590 tcex_cli-1.0.3/tcex_cli/input/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.379475 tcex_cli-1.0.3/tcex_cli/input/field_type/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/field_type/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3130 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/field_type/exception.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5645 2024-04-17 16:17:53.000000 tcex_cli-1.0.3/tcex_cli/input/field_type/sensitive.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.387098 tcex_cli-1.0.3/tcex_cli/input/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2994 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/model/api_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      546 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/model/module_app_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      388 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/model/module_requests_session_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1097 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/model/path_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1040 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/input/model/playbook_common_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      833 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/input/model/playbook_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1256 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/input/model/proxy_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.393139 tcex_cli-1.0.3/tcex_cli/logger/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      171 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/logger/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1904 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/logger/rotating_file_handler_custom.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      969 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/logger/sensitive_filter.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1582 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/logger/test_logger.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1257 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/logger/trace_logger.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.395332 tcex_cli-1.0.3/tcex_cli/message_broker/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/message_broker/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10410 2023-07-26 23:51:46.000000 tcex_cli-1.0.3/tcex_cli/message_broker/mqtt_message_broker.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.405387 tcex_cli-1.0.3/tcex_cli/pleb/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      936 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/cached_property.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1647 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/env_path.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      817 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/event.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      758 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/exception_thread.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      285 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/none_model.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1372 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/proxies.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2749 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/scoped_property.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      418 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/pleb/singleton.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5873 2023-04-01 13:14:35.000000 tcex_cli-1.0.3/tcex_cli/registry.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.407611 tcex_cli-1.0.3/tcex_cli/render/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 00:29:24.000000 tcex_cli-1.0.3/tcex_cli/render/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6942 2023-08-25 18:12:50.000000 tcex_cli-1.0.3/tcex_cli/render/render.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.411229 tcex_cli-1.0.3/tcex_cli/requests_tc/
+-rw-rw-r--   0 bsummers   (503) staff       (20)      137 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/requests_tc/__init__.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.415094 tcex_cli-1.0.3/tcex_cli/requests_tc/auth/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/requests_tc/auth/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1606 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/requests_tc/auth/hmac_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1449 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/requests_tc/auth/tc_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1414 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/requests_tc/auth/token_auth.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     3416 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/requests_tc/requests_tc.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4417 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/requests_tc/tc_session.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.423468 tcex_cli-1.0.3/tcex_cli/util/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       71 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1827 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/aes_operation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4044 2023-07-27 00:01:10.000000 tcex_cli-1.0.3/tcex_cli/util/code_operation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)    10014 2023-07-27 00:01:10.000000 tcex_cli-1.0.3/tcex_cli/util/datetime_operation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7162 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/file_operation.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.425157 tcex_cli-1.0.3/tcex_cli/util/model/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/model/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      668 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/model/playbook_variable_model.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.430065 tcex_cli-1.0.3/tcex_cli/util/render/
+-rw-rw-r--   0 bsummers   (503) staff       (20)       28 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/render/__init__.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)      455 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/render/render.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     4672 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/render/render_panel.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1243 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/render/render_prompt.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     1855 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/render/render_table.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5807 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/requests_to_curl.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     6914 2024-04-17 16:18:15.000000 tcex_cli-1.0.3/tcex_cli/util/string_operation.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     2856 2023-03-31 01:41:44.000000 tcex_cli-1.0.3/tcex_cli/util/util.py
+-rw-rw-r--   0 bsummers   (503) staff       (20)     7992 2024-04-17 16:18:15.000000 tcex_cli-1.0.3/tcex_cli/util/variable.py
+drwxrwxr-x   0 bsummers   (503) staff       (20)        0 2024-04-17 16:18:24.431238 tcex_cli-1.0.3/tcex_cli.egg-info/
+-rw-r--r--   0 bsummers   (503) staff       (20)     3422 2024-04-17 16:18:24.000000 tcex_cli-1.0.3/tcex_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 bsummers   (503) staff       (20)     5616 2024-04-17 16:18:24.000000 tcex_cli-1.0.3/tcex_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)        1 2024-04-17 16:18:24.000000 tcex_cli-1.0.3/tcex_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)       46 2024-04-17 16:18:24.000000 tcex_cli-1.0.3/tcex_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)      245 2024-04-17 16:18:24.000000 tcex_cli-1.0.3/tcex_cli.egg-info/requires.txt
+-rw-rw-r--   0 bsummers   (503) staff       (20)       14 2024-04-17 16:18:24.000000 tcex_cli-1.0.3/tcex_cli.egg-info/top_level.txt
```

### Comparing `tcex_cli-1.0.2/LICENSE` & `tcex_cli-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/PKG-INFO` & `tcex_cli-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcex_cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: ThreatConnect Exchange App CLI Tool
 Author-email: ThreatConnect <support@threatconnect.com>
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/ThreatConnect-Inc/tcex-cli
 Project-URL: Source, https://github.com/ThreatConnect-Inc/tcex-cli
 Keywords: tcex,threatconnect
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,17 +19,17 @@
 Classifier: Topic :: Security
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arrow
 Requires-Dist: black
 Requires-Dist: debugpy
-Requires-Dist: inflect
+Requires-Dist: inflection
 Requires-Dist: isort
-Requires-Dist: paho.mqtt
+Requires-Dist: paho-mqtt<2.0.0
 Requires-Dist: pyaes
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: python-dateutil
 Requires-Dist: PyYAML
 Requires-Dist: redis<5.0.0
 Requires-Dist: requests
 Requires-Dist: rich
@@ -51,15 +51,15 @@
 
 The TcEx CLI package provides functionality for creating ThreatConnect Apps and Integrations.
 
 ## Requirements
 
  * arrow (https://pypi.python.org/pypi/arrow)
  * black (https://pypi.org/project/black/)
- * inflect (https://pypi.python.org/pypi/inflect)
+ * inflection (https://pypi.python.org/pypi/inflection)
  * isort (https://pypi.org/project/isort/)
  * paho-mqtt (https://pypi.org/project/paho-mqtt/)
  * pyaes (https://pypi.org/project/pyaes/)
  * pydantic (https://pypi.org/project/pydantic/)
  * python-dateutil (https://pypi.python.org/pypi/python-dateutil)
  * redis (https://pypi.python.org/pypi/redis)
  * requests (http://docs.python-requests.org/en/latest)
```

### Comparing `tcex_cli-1.0.2/README.md` & `tcex_cli-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 The TcEx CLI package provides functionality for creating ThreatConnect Apps and Integrations.
 
 ## Requirements
 
  * arrow (https://pypi.python.org/pypi/arrow)
  * black (https://pypi.org/project/black/)
- * inflect (https://pypi.python.org/pypi/inflect)
+ * inflection (https://pypi.python.org/pypi/inflection)
  * isort (https://pypi.org/project/isort/)
  * paho-mqtt (https://pypi.org/project/paho-mqtt/)
  * pyaes (https://pypi.org/project/pyaes/)
  * pydantic (https://pypi.org/project/pydantic/)
  * python-dateutil (https://pypi.python.org/pypi/python-dateutil)
  * redis (https://pypi.python.org/pypi/redis)
  * requests (http://docs.python-requests.org/en/latest)
```

### Comparing `tcex_cli-1.0.2/pyproject.toml` & `tcex_cli-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Security",
 ]
 dependencies = [
   "arrow",
   "black",
   "debugpy",
-  "inflect",
+  "inflection",
   "isort",
-  "paho.mqtt",
+  "paho-mqtt<2.0.0",
   "pyaes",
   "pydantic<2.0.0",
   "python-dateutil",
   "PyYAML",
   "redis<5.0.0",
   "requests",
   "rich",
@@ -129,17 +129,23 @@
 extension-pkg-whitelist = "pydantic"
 
 [tool.pyright]
 # https://github.com/microsoft/pyright/blob/main/docs/configuration.md#sample-pyprojecttoml-file
 exclude = [
   "**/.history",
   "**/__pycache__",
+  "**/local-*",
+  "tcex/api/tc/v2",
+  "tests",
 ]
 pythonPlatform = "Linux"
 pythonVersion = "3.11"
+reportIncompatibleMethodOverride = false
+reportIncompatibleVariableOverride = false
+reportPrivateImportUsage = false
 
 [tool.pytest.ini_options]
 filterwarnings = []
 junit_family = "xunit2"
 testpaths = [
   "tests",
 ]
```

### Comparing `tcex_cli-1.0.2/tcex_cli/__init__.py` & `tcex_cli-1.0.3/tcex_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/app.py` & `tcex_cli-1.0.3/tcex_cli/app/app.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/app_spec_yml.py` & `tcex_cli-1.0.3/tcex_cli/app/config/app_spec_yml.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/install_json.py` & `tcex_cli-1.0.3/tcex_cli/app/config/install_json.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/install_json_update.py` & `tcex_cli-1.0.3/tcex_cli/app/config/install_json_update.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/install_json_validate.py` & `tcex_cli-1.0.3/tcex_cli/app/config/install_json_validate.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/job_json.py` & `tcex_cli-1.0.3/tcex_cli/app/config/job_json.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/layout_json.py` & `tcex_cli-1.0.3/tcex_cli/app/config/layout_json.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/model/app_spec_yml_model.py` & `tcex_cli-1.0.3/tcex_cli/app/config/model/app_spec_yml_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/model/install_json_model.py` & `tcex_cli-1.0.3/tcex_cli/app/config/model/install_json_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TcEx Framework Module"""
+
 # pylint: disable=no-self-argument
 # standard library
 import logging
 import os
 import platform
 import re
 import uuid
@@ -498,15 +499,15 @@
         commit_hash = os.getenv('CI_COMMIT_SHA') or os.getenv('GITHUB_SHA')
 
     return commit_hash
 
 
 def gen_app_id() -> UUID5:
     """Return a generate id for the current App."""
-    return uuid.uuid5(uuid.NAMESPACE_X500, os.path.basename(os.getcwd()).lower())
+    return uuid.uuid4()
 
 
 class InstallJsonCommonModel(BaseModel):
     """Model definition for install.json common configuration
 
     This model contains the common fields for the install.json file and
     the app_spec.yaml file.
@@ -769,18 +770,14 @@
     def known_features(self) -> dict[str, _FeatureModel]:
         """Return all known features."""
 
         feature_data = {
             'advancedRequest': {
                 'runtime_levels': ['playbook'],
             },
-            'aotExecutionEnabled': {
-                'default': True,
-                'runtime_levels': ['playbook'],
-            },
             'appBuilderCompliant': {
                 'default': True,
                 'runtime_levels': ['playbook', 'triggerservice', 'webhooktriggerservice'],
             },
             'CALSettings': {},
             'fileParams': {
                 'default': True,
@@ -793,14 +790,15 @@
             },
             'redisPasswordSupport': {
                 'default': True,
                 'version': Version('3.0.9'),
             },
             'runtimeVariables': {
                 'default': True,
+                'runtime_levels': ['playbook'],
                 'version': Version('3.0.2'),
             },
             # 'secureParams': {
             #     'default': True,
             #     'runtime_levels': ['organization', 'playbook'],
             # },
             'smtpSettings': {},
@@ -844,14 +842,17 @@
     def updated_features(self) -> list[str]:
         """Update feature set based on App type."""
         try:
             tcex_version = Version.coerce(get_version('tcex'))
         except Exception:
             tcex_version = Version('2.0.0')
 
+        # define deprecated features that should be removed
+        deprecated_features = ['aotExecutionEnabled']
+
         # normalize features based on App type and TcEx version
         features = []
         for feature, model in self.known_features.items():
             if (
                 model.default is True
                 and (model.version is None or model.version <= tcex_version)
                 and (
@@ -865,14 +866,18 @@
         if os.path.isfile('layout.json'):
             features.append('layoutEnabledApp')
 
         # extend feature list with features defined by developer
         for feature in self.features:
             model = self.known_features.get(feature)
 
+            # exclude deprecated features
+            if feature in deprecated_features:
+                continue
+
             if model is None:
                 # not sure what the feature is, but add it anyway
                 features.append(feature)
 
                 # log unknown features
                 _logger.warning(f'Unknown feature found in install.json: {feature}')
             else:
```

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/model/job_json_model.py` & `tcex_cli-1.0.3/tcex_cli/app/config/model/job_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/model/layout_json_model.py` & `tcex_cli-1.0.3/tcex_cli/app/config/model/layout_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/model/tcex_json_model.py` & `tcex_cli-1.0.3/tcex_cli/app/config/model/tcex_json_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/permutation.py` & `tcex_cli-1.0.3/tcex_cli/app/config/permutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TcEx Framework Module"""
+
 # standard library
 import json
 import logging
 import os
 import random
 import re
 import sys
@@ -201,16 +202,16 @@
 
         return _action_configurations
 
     @cached_property
     def db_conn(self) -> sqlite3.Connection:  # type: ignore
         """Create a temporary in memory DB and return the connection."""
         try:
-            return sqlite3.connect(':memory:')
-        except sqlite3.Error as ex:  # pragma: no cover
+            return sqlite3.connect(':memory:')  # type: ignore
+        except sqlite3.Error as ex:  # type: ignore # pragma: no cover
             Render.panel.failure(f'Failed initializing database ({ex}).')
 
     def db_create_table(self, table_name: str, columns: list[str]):
         """Create a temporary DB table.
 
         Args:
             table_name: The DB table name.
@@ -218,28 +219,28 @@
         """
         columns_ = ', '.join([f'''"{c.strip('"').strip("'")}" text''' for c in set(columns)])
         self.log.debug(f'action=db-create-table, table-name={table_name}, columns={columns_}')
         sql = f'CREATE TABLE IF NOT EXISTS {table_name} ({columns_});'
         try:
             cr = self.db_conn.cursor()
             cr.execute(sql)
-        except sqlite3.Error as e:  # pragma: no cover
+        except sqlite3.Error as e:  # type: ignore # pragma: no cover
             Render.panel.failure(f'SQL create db failed - SQL: "{sql}", Error: "{e}"')
 
     def db_drop_table(self, table_name: str):
         """Drop a DB table.
 
         Args:
             table_name: The DB table name.
         """
         sql = f'DROP TABLE IF EXISTS {table_name};'
         try:
             cr = self.db_conn.cursor()
             cr.execute(sql)
-        except sqlite3.Error as e:  # pragma: no cover
+        except sqlite3.Error as e:  # type: ignore # pragma: no cover
             Render.panel.failure(f'SQL drop db failed - SQL: "{sql}", Error: "{e}"')
 
     def db_insert_record(self, table_name: str, columns: list[str]):
         """Insert records into DB.
 
         A single row will all values as None so that values can be updated one at a
         time during parsing. The row and values will be used to determine permutations.
@@ -281,15 +282,15 @@
         # only column defined in install.json can be updated
         if column in self.ij.model.param_names:
             # value should be wrapped in single quotes to be properly parsed
             sql = f'UPDATE {table_name} SET {column} = \'{value}\''
             try:
                 cur = self.db_conn.cursor()
                 cur.execute(sql)
-            except sqlite3.OperationalError as ex:  # pragma: no cover
+            except sqlite3.OperationalError as ex:  # type: ignore # pragma: no cover
                 Render.panel.failure(f'SQL update failed - SQL: "{sql}", Error: "{ex}"')
 
     def get_action_input_names(self, action: str) -> list[str]:
         """Return the input names for the provided action."""
         return [i.name for i in self.get_action_inputs(action)]
 
     def get_action_inputs(self, action: str) -> list[InputModel]:
@@ -337,16 +338,15 @@
         """
         if self.lj.has_layout:
             for name in self.lj.model.param_names:
                 param = self.ij.model.get_param(name)
                 if param is not None:
                     yield param
         else:
-            for param in self.ij.model.params:
-                yield param
+            yield from self.ij.model.params
 
     # TODO: [low] improve this logic
     def init_permutations(self):
         """Process layout.json names/display to get all permutations of args."""
         if not all([self._input_permutations, self._output_permutations]):
             self._input_permutations = []
             self._output_permutations = []
@@ -562,15 +562,15 @@
             display_query = f'SELECT count(*) from {table} where {display_condition}'  # nosec
             try:
                 cur = self.db_conn.cursor()
                 cur.execute(display_query.replace('"', ''))
                 rows = cur.fetchall()
                 if rows[0][0] > 0:
                     display = True
-            except sqlite3.Error as e:  # pragma: no cover
+            except sqlite3.Error as e:  # type: ignore # pragma: no cover
                 Render.panel.failure(f'"{display_query}" query returned an error: ({e}).')
         return display
 
     def write_permutations_file(self):
         """Write permutations file."""
         _permutations = []
         for index, permutations in enumerate(self.input_permutations):
```

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/tcex_json.py` & `tcex_cli-1.0.3/tcex_cli/app/config/tcex_json.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/app/config/tcex_json_update.py` & `tcex_cli-1.0.3/tcex_cli/app/config/tcex_json_update.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/cli.py` & `tcex_cli-1.0.3/tcex_cli/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # third-party
 import typer
 from semantic_version import Version
 
 # first-party
 from tcex_cli.cli.deploy import deploy
 from tcex_cli.cli.deps import deps
+from tcex_cli.cli.migrate import migrate
 from tcex_cli.cli.package import package
 from tcex_cli.cli.run import run
 from tcex_cli.cli.spec_tool import spec_tool
 from tcex_cli.cli.template import init, list_, update
 from tcex_cli.cli.validate import validate
 from tcex_cli.render.render import Render
 
@@ -89,14 +90,15 @@
 
 # initialize typer
 app = typer.Typer(callback=version_callback, invoke_without_command=True)
 app.command('deploy')(deploy.command)
 app.command('deps')(deps.command)
 app.command('init')(init.command)
 app.command('list')(list_.command)
+app.command('migrate')(migrate.command)
 app.command('package')(package.command)
 app.command('run')(run.command)
 app.command('spec-tool')(spec_tool.command)
 app.command('update')(update.command)
 app.command('validate')(validate.command)
 
 # add test command
```

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/cli_abc.py` & `tcex_cli-1.0.3/tcex_cli/cli/cli_abc.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/deploy/deploy.py` & `tcex_cli-1.0.3/tcex_cli/cli/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/deploy/deploy_cli.py` & `tcex_cli-1.0.3/tcex_cli/cli/deploy/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/deps/deps.py` & `tcex_cli-1.0.3/tcex_cli/cli/deps/deps.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/deps/deps_cli.py` & `tcex_cli-1.0.3/tcex_cli/cli/deps/deps_cli.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/model/file_metadata_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/model/file_metadata_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/model/validation_data_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/model/validation_data_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/package/package.py` & `tcex_cli-1.0.3/tcex_cli/cli/package/package.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/package/package_cli.py` & `tcex_cli-1.0.3/tcex_cli/cli/package/package_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TcEx Framework Module"""
+
 # standard library
 import fnmatch
 import json
 import os
 import shutil
 from pathlib import Path
 
@@ -158,14 +159,15 @@
 
         # create app metadata for output
         self.app_metadata = AppMetadataModel(
             name=self.app.tj.model.package.app_name,
             package_name=package_name,
             template_directory=self.template_fqpn.name,
             version=str(self.app.ij.model.program_version),
+            features=', '.join(ij_template.model.features),
         )
 
         # cleanup build directory
         shutil.rmtree(app_path_fqpn)
 
     @cached_property
     def template_fqpn(self) -> Path:
```

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/launch_abc.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/launch_abc.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/launch_organization.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/launch_organization.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/launch_playbook.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/launch_playbook.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_api.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,15 @@
                 )
 
             case 'shutdown':
                 self.stop_server = True
 
         self.event.set()
 
-    def setup(self):
+    def setup(self, debug: bool = False):
         """Configure the API Web Server."""
         # setup web server
         self.api_web_server.setup()
 
         # start keyboard listener
         kl = Thread(target=self.keyboard_listener, name='KeyboardListener', daemon=True)
         kl.start()
@@ -247,11 +247,12 @@
         self.message_broker.add_on_message_callback(
             callback=self.process_server_channel,
             index=0,
             topics=[self.model.inputs.tc_svc_server_topic],
         )
 
         # start live display
-        self.display_thread = Thread(
-            target=self.live_data_display, name='LiveDataDisplay', daemon=True
-        )
-        self.display_thread.start()
+        if debug is False:
+            self.display_thread = Thread(
+                target=self.live_data_display, name='LiveDataDisplay', daemon=True
+            )
+            self.display_thread.start()
```

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_common_abc.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_common_abc.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_common_trigger_abc.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_common_trigger_abc.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_custom_trigger.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_custom_trigger.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             while True:
                 self.event.wait()
                 self.log.trace('Updating live data table.')
                 layout['main'].update(self.live_data_table())
                 layout['commands'].update(self.live_data_commands())
                 self.event.clear()
 
-    def setup(self):
+    def setup(self, debug: bool = False):
         """Configure the API Web Server."""
         # start keyboard listener
         kl = Thread(target=self.keyboard_listener, name='KeyboardListener', daemon=True)
         kl.start()
 
         # start message broker listener
         self.message_broker_listen()
@@ -66,11 +66,12 @@
         self.message_broker.add_on_message_callback(
             callback=self.process_server_channel,
             index=0,
             topics=[self.model.inputs.tc_svc_server_topic],
         )
 
         # start live display
-        self.display_thread = Thread(
-            target=self.live_data_display, name='LiveDataDisplay', daemon=True
-        )
-        self.display_thread.start()
+        if debug is False:
+            self.display_thread = Thread(
+                target=self.live_data_display, name='LiveDataDisplay', daemon=True
+            )
+            self.display_thread.start()
```

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/launch_service_webhook_trigger.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/launch_service_webhook_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         return Panel(
             '\n'.join(panel_data),
             expand=True,
             title=f'[{self.panel_title}]HTTP Server[/]',
             title_align='left',
         )
 
-    def setup(self):
+    def setup(self, debug: bool = False):
         """Configure the API Web Server."""
         # setup web server
         self.api_web_server.setup()
 
         # start keyboard listener
         kl = Thread(target=self.keyboard_listener, name='KeyboardListener', daemon=True)
         kl.start()
@@ -110,11 +110,12 @@
         self.message_broker.add_on_message_callback(
             callback=self.process_server_channel,
             index=0,
             topics=[self.model.inputs.tc_svc_server_topic],
         )
 
         # start live display
-        self.display_thread = Thread(
-            target=self.live_data_display, name='LiveDataDisplay', daemon=True
-        )
-        self.display_thread.start()
+        if debug is False:
+            self.display_thread = Thread(
+                target=self.live_data_display, name='LiveDataDisplay', daemon=True
+            )
+            self.display_thread.start()
```

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/api_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/api_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/app_api_service_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/app_api_service_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/app_organization_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/app_organization_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/app_playbook_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/app_playbook_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/app_trigger_service_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/app_trigger_service_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/app_webhook_trigger_service_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/app_webhook_trigger_service_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/batch_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/batch_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/logging_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/logging_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/path_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/path_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/playbook_common_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/playbook_common_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/playbook_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/playbook_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/proxy_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/proxy_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/model/service_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/model/service_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     tc_svc_broker_cert_file: str | None = None
     tc_svc_broker_conn_timeout: int = 60
     tc_svc_broker_host: str = 'localhost'
     tc_svc_broker_port: int = 1883
     tc_svc_broker_timeout: int = 60
     tc_svc_broker_token: Sensitive | None = None
     tc_svc_client_topic: str = 'tcex-app-testing-client-topic'
-    tc_svc_hb_timeout_seconds: int = 600
+    tc_svc_hb_timeout_seconds: int = 3600
     tc_svc_id: int | None = None
     tc_svc_server_topic: str = 'tcex-app-testing-server-topic'
 
     class Config:
         """DataModel Config"""
 
         extra = Extra.allow
```

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/playbook_create.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/playbook_create.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/request_handler_api.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/request_handler_api.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/request_handler_webhook.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/request_handler_webhook.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/run.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,12 +29,12 @@
             Render.panel.failure(f'Config file not found [{config_json}]')
 
         # run in debug mode
         if debug is True:
             cli.debug(debug_port)
 
         # run the App
-        cli.run(config_json)
+        cli.run(config_json, debug)
 
     except Exception as ex:
         cli.log.exception('Failed to run "tcex run" command.')
         Render.panel.failure(f'Exception: {ex}')
```

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/run_cli.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/run_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,32 +63,32 @@
         debugpy.wait_for_client()
 
     def exit_cli(self, exit_code):
         """Exit the CLI command."""
         Render.panel.info(f'{exit_code}', f'[{self.panel_title}]Exit Code[/]')
         sys.exit(exit_code)
 
-    def run(self, config_json: Path):
+    def run(self, config_json: Path, debug: bool = False):
         """Run the App"""
 
         match self.ij.model.runtime_level.lower():
             case 'apiservice':
                 Render.panel.info('Launching API Service', f'[{self.panel_title}]Running App[/]')
                 launch_app = LaunchServiceApi(config_json)
                 self._display_api_settings(launch_app.model.inputs)
-                launch_app.setup()
+                launch_app.setup(debug)
                 exit_code = launch_app.launch()
                 self.exit_cli(exit_code)
 
             case 'feedapiservice':
                 Render.panel.info(
                     'Launching Feed API Service', f'[{self.panel_title}]Running App[/]'
                 )
                 launch_app = LaunchServiceApi(config_json)
-                launch_app.setup()
+                launch_app.setup(debug)
                 exit_code = launch_app.launch()
                 self.exit_cli(exit_code)
 
             case 'organization':
                 Render.panel.info('Launching Job App', f'[{self.panel_title}]Running App[/]')
                 launch_app = LaunchOrganization(config_json)
                 exit_code = launch_app.launch()
@@ -105,20 +105,20 @@
                 self.exit_cli(exit_code)
 
             case 'triggerservice':
                 Render.panel.info(
                     'Launching Trigger Service', f'[{self.panel_title}]Running App[/]'
                 )
                 launch_app = LaunchServiceCustomTrigger(config_json)
-                launch_app.setup()
+                launch_app.setup(debug)
                 exit_code = launch_app.launch()
                 self.exit_cli(exit_code)
 
             case 'webhooktriggerservice':
                 Render.panel.info(
                     'Launching Webhook Trigger Service', f'[{self.panel_title}]Running App[/]'
                 )
                 launch_app = LaunchServiceWebhookTrigger(config_json)
                 self._display_api_settings(launch_app.model.inputs)
-                launch_app.setup()
+                launch_app.setup(debug)
                 exit_code = launch_app.launch()
                 self.exit_cli(exit_code)
```

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/run/web_server.py` & `tcex_cli-1.0.3/tcex_cli/cli/run/web_server.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_app_input.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_app_input.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_app_input_static.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_app_input_static.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_app_spec_yml.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_app_spec_yml.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_install_json.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_install_json.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_job_json.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_job_json.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_layout_json.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_layout_json.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_readme_md.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_readme_md.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/gen_tcex_json.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/gen_tcex_json.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/spec_tool.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/spec_tool.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/spec_tool/spec_tool_cli.py` & `tcex_cli-1.0.3/tcex_cli/cli/spec_tool/spec_tool_cli.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/template/init.py` & `tcex_cli-1.0.3/tcex_cli/cli/template/init.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/template/list_.py` & `tcex_cli-1.0.3/tcex_cli/cli/template/list_.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/template/model/template_config_model.py` & `tcex_cli-1.0.3/tcex_cli/cli/template/model/template_config_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/template/template_cli.py` & `tcex_cli-1.0.3/tcex_cli/cli/template/template_cli.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/template/update.py` & `tcex_cli-1.0.3/tcex_cli/cli/template/update.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/validate/validate.py` & `tcex_cli-1.0.3/tcex_cli/cli/validate/validate.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/cli/validate/validate_cli.py` & `tcex_cli-1.0.3/tcex_cli/cli/validate/validate_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TcEx Framework Module"""
+
 # standard library
 import ast
 import json
 import os
 import sys
 import traceback
 from pathlib import Path
@@ -218,15 +219,15 @@
                     if p.display:
                         display_query = (
                             f'SELECT * FROM {self.app.permutation.input_table}'  # nosec
                             f' WHERE {p.display}'
                         )
                         try:
                             self.app.permutation.db_conn.execute(display_query.replace('"', ''))
-                        except sqlite3.Error:
+                        except sqlite3.Error:  # type: ignore
                             self.validation_data.errors.append(
                                 'Layouts input.parameters[].display validations failed '
                                 f'("{p.display}" query is an invalid statement).'
                             )
                             status = False
 
         # update validation data for module
@@ -258,15 +259,15 @@
                 if o.display:
                     display_query = (
                         f'SELECT * FROM {self.app.permutation.input_table} '  # nosec
                         f'WHERE {o.display}'
                     )
                     try:
                         self.app.permutation.db_conn.execute(display_query.replace('"', ''))
-                    except sqlite3.Error:
+                    except sqlite3.Error:  # type: ignore
                         self.validation_data.errors.append(
                             f"""Layouts outputs.display validations failed ("{o.display}" """
                             f"""query is an invalid statement)."""
                         )
                         status = False
 
         # update validation data for module
```

### Comparing `tcex_cli-1.0.2/tcex_cli/input/field_type/exception.py` & `tcex_cli-1.0.3/tcex_cli/input/field_type/exception.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/input/field_type/sensitive.py` & `tcex_cli-1.0.3/tcex_cli/input/field_type/sensitive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TcEx Framework Module"""
+
 # standard library
 import logging
 from collections.abc import Generator
 from typing import Any, Self
 
 # third-party
 from pydantic.fields import ModelField  # TYPE-CHECKING
@@ -115,15 +116,17 @@
         return value
 
     @classmethod
     def validate_type(cls, value: bytes | str | Self, field: ModelField) -> bytes | str | Self:
         """Raise exception if value is not a String type."""
         if not isinstance(value, (bytes, str, Sensitive)):
             raise InvalidType(
-                field_name=field.name, expected_types='(bytes, str)', provided_type=type(value)
+                field_name=field.name,
+                expected_types='(bytes, str)',
+                provided_type=type(value).__name__,
             )
         return value
 
     @property
     def value(self) -> str:
         """Return the actual value."""
         if not isinstance(self._sensitive_value, (BinaryVariable, bytes)):
```

### Comparing `tcex_cli-1.0.2/tcex_cli/input/model/api_model.py` & `tcex_cli-1.0.3/tcex_cli/input/model/api_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/input/model/module_app_model.py` & `tcex_cli-1.0.3/tcex_cli/input/model/module_app_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/input/model/path_model.py` & `tcex_cli-1.0.3/tcex_cli/input/model/path_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/input/model/playbook_common_model.py` & `tcex_cli-1.0.3/tcex_cli/input/model/playbook_common_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/input/model/playbook_model.py` & `tcex_cli-1.0.3/tcex_cli/input/model/playbook_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/input/model/proxy_model.py` & `tcex_cli-1.0.3/tcex_cli/input/model/proxy_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/logger/rotating_file_handler_custom.py` & `tcex_cli-1.0.3/tcex_cli/logger/rotating_file_handler_custom.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/logger/sensitive_filter.py` & `tcex_cli-1.0.3/tcex_cli/logger/sensitive_filter.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/logger/test_logger.py` & `tcex_cli-1.0.3/tcex_cli/logger/test_logger.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/logger/trace_logger.py` & `tcex_cli-1.0.3/tcex_cli/logger/trace_logger.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/message_broker/mqtt_message_broker.py` & `tcex_cli-1.0.3/tcex_cli/message_broker/mqtt_message_broker.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/pleb/cached_property.py` & `tcex_cli-1.0.3/tcex_cli/pleb/cached_property.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/pleb/env_path.py` & `tcex_cli-1.0.3/tcex_cli/pleb/env_path.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/pleb/event.py` & `tcex_cli-1.0.3/tcex_cli/pleb/event.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/pleb/exception_thread.py` & `tcex_cli-1.0.3/tcex_cli/pleb/exception_thread.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/pleb/proxies.py` & `tcex_cli-1.0.3/tcex_cli/pleb/proxies.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/pleb/scoped_property.py` & `tcex_cli-1.0.3/tcex_cli/pleb/scoped_property.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/registry.py` & `tcex_cli-1.0.3/tcex_cli/registry.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/render/render.py` & `tcex_cli-1.0.3/tcex_cli/render/render.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/requests_tc/auth/hmac_auth.py` & `tcex_cli-1.0.3/tcex_cli/requests_tc/auth/hmac_auth.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/requests_tc/auth/tc_auth.py` & `tcex_cli-1.0.3/tcex_cli/requests_tc/auth/tc_auth.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/requests_tc/auth/token_auth.py` & `tcex_cli-1.0.3/tcex_cli/requests_tc/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/requests_tc/requests_tc.py` & `tcex_cli-1.0.3/tcex_cli/requests_tc/requests_tc.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/requests_tc/tc_session.py` & `tcex_cli-1.0.3/tcex_cli/requests_tc/tc_session.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/aes_operation.py` & `tcex_cli-1.0.3/tcex_cli/util/aes_operation.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/code_operation.py` & `tcex_cli-1.0.3/tcex_cli/util/code_operation.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/datetime_operation.py` & `tcex_cli-1.0.3/tcex_cli/util/datetime_operation.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/file_operation.py` & `tcex_cli-1.0.3/tcex_cli/util/file_operation.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/model/playbook_variable_model.py` & `tcex_cli-1.0.3/tcex_cli/util/model/playbook_variable_model.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/render/render_panel.py` & `tcex_cli-1.0.3/tcex_cli/util/render/render_panel.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/render/render_prompt.py` & `tcex_cli-1.0.3/tcex_cli/util/render/render_prompt.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/render/render_table.py` & `tcex_cli-1.0.3/tcex_cli/util/render/render_table.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/requests_to_curl.py` & `tcex_cli-1.0.3/tcex_cli/util/requests_to_curl.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/string_operation.py` & `tcex_cli-1.0.3/tcex_cli/util/string_operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 """TcEx Framework Module"""
+
 # standard library
 import random
-import re
 from functools import cached_property, reduce
 from string import ascii_letters
 
 # third-party
-import inflect
+import inflection
 
 
 class StringOperation:
     """TcEx Utilities String Operations Class"""
 
     @staticmethod
     def camel_string(string: str) -> 'CamelString':
         """Return str with custom properties/methods."""
         return CamelString(string)
 
     def camel_to_snake(self, string: str) -> str:
         """Return snake_case string from a camelCase string."""
-        return self._camel_pattern.sub('_', string).lower()
+        return inflection.underscore(string)
 
     def camel_to_space(self, string: str) -> str:
         """Return space case string from a camelCase string."""
-        return self._camel_pattern.sub(' ', string).lower()
+        return inflection.underscore(string).replace('_', ' ')
 
     @cached_property
-    def inflect(self) -> inflect.engine:
+    def inflect(self):
         """Return instance of inflect."""
-        return inflect.engine()
+        return inflection
+
+    @cached_property
+    def inflection(self):
+        """Return instance of inflect."""
+        return inflection
 
     @staticmethod
     def random_string(string_length: int = 10) -> str:
         """Generate a random string of fixed length."""
         return ''.join(random.choice(ascii_letters) for _ in range(string_length))  # nosec
 
     @staticmethod
     def snake_string(string: str) -> 'SnakeString':
         """Return custom str with custom properties/methods."""
         return SnakeString(string)
 
     @staticmethod
     def snake_to_pascal(string: str) -> str:
         """Convert snake_case to PascalCase."""
-        return string.replace('_', ' ').title().replace(' ', '')
+        return inflection.camelize(string, uppercase_first_letter=True)
 
     @staticmethod
     def snake_to_camel(string: str) -> str:
         """Convert snake_case to camelCase."""
-        components = string.split('_')
-        return components[0] + ''.join(x.title() for x in components[1:])
+        return inflection.camelize(string, uppercase_first_letter=False)
 
     @staticmethod
     def to_bool(value: bool | int | str) -> bool:
         """Convert value to bool."""
         return str(value).lower() in ['1', 't', 'true', 'y', 'yes']
 
     @staticmethod
@@ -93,19 +97,14 @@
         if spaces is True:
             if not output.endswith(' '):
                 # split output on spaces and drop last item to terminate string on word
                 output = ' '.join(output.split(' ')[:-1])
 
         return f'{output.rstrip()}{append_chars}'
 
-    @property
-    def _camel_pattern(self) -> re.Pattern:
-        """Return compiled re pattern for converting to camelCase."""
-        return re.compile(r'(?<!^)(?=[A-Z])')
-
     @staticmethod
     def wrap_string(
         line: str,
         wrap_chars: list[str] | None = None,
         length: int = 100,
         force_wrap: bool = True,
     ) -> str:
@@ -159,19 +158,19 @@
 
     def pascal_case(self):
         """Return a PascalCase version of a camelCase string."""
         return CamelString(self.so.camel_to_space(self).title().replace(' ', ''))
 
     def plural(self):
         """Return the plural spelling of a camelCase string."""
-        return CamelString(self.so.inflect.plural(self.singular()))
+        return CamelString(self.so.inflection.pluralize(self.singular()))
 
     def singular(self):
         """Return the singular spelling of a camelCase string."""
-        _singular = self.so.inflect.singular_noun(self)
+        _singular = self.so.inflection.singularize(self)
 
         if not _singular:
             _singular = self
         return CamelString(_singular)
 
     def snake_case(self):
         """Return a snake_case version of a camelCase string."""
@@ -194,19 +193,19 @@
 
     def pascal_case(self):
         """Return a PascalCase version of a snake_case string."""
         return SnakeString(self.so.snake_to_pascal(self))
 
     def plural(self):
         """Return the plural spelling of a snake_case string."""
-        return SnakeString(self.so.inflect.plural(self.singular()))
+        return SnakeString(self.so.inflection.pluralize(self.singular()))
 
     def singular(self):
         """Return the singular spelling of a snake_case string."""
-        _singular = self.so.inflect.singular_noun(self)
+        _singular = self.so.inflection.singularize(self)
 
         if not _singular:
             _singular = self
         return SnakeString(_singular)
 
     def space_case(self, title: bool = True):
         """Return a "space case" version of a snake_case string."""
```

### Comparing `tcex_cli-1.0.2/tcex_cli/util/util.py` & `tcex_cli-1.0.3/tcex_cli/util/util.py`

 * *Files identical despite different names*

### Comparing `tcex_cli-1.0.2/tcex_cli/util/variable.py` & `tcex_cli-1.0.3/tcex_cli/util/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,23 @@
         if not isinstance(key, str):
             return False
 
         if re.search(self.variable_playbook_pattern, key):
             return True
         return False
 
+    def contains_tc_variable(self, key: str):
+        """Return True if provided key contains a properly formatted TC variable."""
+        if not isinstance(key, str):
+            return False
+
+        if re.search(self.variable_tc_pattern, key):
+            return True
+        return False
+
     def get_playbook_variable_model(self, variable: str | None) -> PlaybookVariableModel | None:
         """Return data model of playbook variable (e.g., #App:1234:output!String)."""
         if variable is None:
             return None
 
         data = None
         variable = variable.strip()
```

### Comparing `tcex_cli-1.0.2/tcex_cli.egg-info/PKG-INFO` & `tcex_cli-1.0.3/tcex_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tcex-cli
-Version: 1.0.2
+Name: tcex_cli
+Version: 1.0.3
 Summary: ThreatConnect Exchange App CLI Tool
 Author-email: ThreatConnect <support@threatconnect.com>
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/ThreatConnect-Inc/tcex-cli
 Project-URL: Source, https://github.com/ThreatConnect-Inc/tcex-cli
 Keywords: tcex,threatconnect
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,17 +19,17 @@
 Classifier: Topic :: Security
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: arrow
 Requires-Dist: black
 Requires-Dist: debugpy
-Requires-Dist: inflect
+Requires-Dist: inflection
 Requires-Dist: isort
-Requires-Dist: paho.mqtt
+Requires-Dist: paho-mqtt<2.0.0
 Requires-Dist: pyaes
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: python-dateutil
 Requires-Dist: PyYAML
 Requires-Dist: redis<5.0.0
 Requires-Dist: requests
 Requires-Dist: rich
@@ -51,15 +51,15 @@
 
 The TcEx CLI package provides functionality for creating ThreatConnect Apps and Integrations.
 
 ## Requirements
 
  * arrow (https://pypi.python.org/pypi/arrow)
  * black (https://pypi.org/project/black/)
- * inflect (https://pypi.python.org/pypi/inflect)
+ * inflection (https://pypi.python.org/pypi/inflection)
  * isort (https://pypi.org/project/isort/)
  * paho-mqtt (https://pypi.org/project/paho-mqtt/)
  * pyaes (https://pypi.org/project/pyaes/)
  * pydantic (https://pypi.org/project/pydantic/)
  * python-dateutil (https://pypi.python.org/pypi/python-dateutil)
  * redis (https://pypi.python.org/pypi/redis)
  * requests (http://docs.python-requests.org/en/latest)
```

### Comparing `tcex_cli-1.0.2/tcex_cli.egg-info/SOURCES.txt` & `tcex_cli-1.0.3/tcex_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 tcex_cli/cli/cli_abc.py
 tcex_cli/cli/deploy/__init__.py
 tcex_cli/cli/deploy/deploy.py
 tcex_cli/cli/deploy/deploy_cli.py
 tcex_cli/cli/deps/__init__.py
 tcex_cli/cli/deps/deps.py
 tcex_cli/cli/deps/deps_cli.py
+tcex_cli/cli/migrate/__init__.py
+tcex_cli/cli/migrate/migrate.py
+tcex_cli/cli/migrate/migrate_cli.py
 tcex_cli/cli/model/__init__.py
 tcex_cli/cli/model/app_metadata_model.py
 tcex_cli/cli/model/file_metadata_model.py
 tcex_cli/cli/model/key_value_model.py
 tcex_cli/cli/model/validation_data_model.py
 tcex_cli/cli/package/__init__.py
 tcex_cli/cli/package/package.py
```

