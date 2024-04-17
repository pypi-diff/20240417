# Comparing `tmp/logicmonitor-sdk-3.0.200.tar.gz` & `tmp/logicmonitor-sdk-3.0.203.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logicmonitor-sdk-3.0.200.tar", last modified: Mon Jan 22 11:15:10 2024, max compression
+gzip compressed data, was "dist/logicmonitor-sdk-3.0.203.tar", last modified: Wed Apr 17 07:11:42 2024, max compression
```

## Comparing `logicmonitor-sdk-3.0.200.tar` & `logicmonitor-sdk-3.0.203.tar`

### file list

```diff
@@ -1,1096 +1,1112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/api/
--rw-r--r--   0 root         (0) root         (0)      133 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1081583 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/api/lm_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/
--rw-r--r--   0 root         (0) root         (0)    48894 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5485 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/access_log_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     3936 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ack_collector_down.py
--rw-r--r--   0 root         (0) root         (0)    28825 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/admin.py
--rw-r--r--   0 root         (0) root         (0)     5405 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/admin_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     4250 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aggregate_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    44130 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert.py
--rw-r--r--   0 root         (0) root         (0)     4137 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_ack.py
--rw-r--r--   0 root         (0) root         (0)    16729 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_filters.py
--rw-r--r--   0 root         (0) root         (0)    34050 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_forecasting_report.py
--rw-r--r--   0 root         (0) root         (0)     5510 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_list_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5405 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    47847 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_report.py
--rw-r--r--   0 root         (0) root         (0)    44683 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_response.py
--rw-r--r--   0 root         (0) root         (0)    18556 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_rule.py
--rw-r--r--   0 root         (0) root         (0)     5490 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_rule_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    31680 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_sla_report.py
--rw-r--r--   0 root         (0) root         (0)    33107 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_threshold_report.py
--rw-r--r--   0 root         (0) root         (0)     4834 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_trends_metric.py
--rw-r--r--   0 root         (0) root         (0)    27021 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_trends_report.py
--rw-r--r--   0 root         (0) root         (0)    15220 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_widget.py
--rw-r--r--   0 root         (0) root         (0)     7051 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_widget_data.py
--rw-r--r--   0 root         (0) root         (0)    11241 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/api_perf_metrics.py
--rw-r--r--   0 root         (0) root         (0)    12872 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/api_token.py
--rw-r--r--   0 root         (0) root         (0)     5469 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/api_token_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     9586 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/applies_to_function.py
--rw-r--r--   0 root         (0) root         (0)     7952 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/assignment.py
--rw-r--r--   0 root         (0) root         (0)     8226 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    28756 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/audit_log_report.py
--rw-r--r--   0 root         (0) root         (0)     6135 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/authentication.py
--rw-r--r--   0 root         (0) root         (0)    12116 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/auto_discovery_configuration.py
--rw-r--r--   0 root         (0) root         (0)     6777 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/auto_discovery_filter.py
--rw-r--r--   0 root         (0) root         (0)    12014 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    10539 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/automatic_upgrade_info.py
--rw-r--r--   0 root         (0) root         (0)     3963 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_account_id.py
--rw-r--r--   0 root         (0) root         (0)     5997 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_account_test_result.py
--rw-r--r--   0 root         (0) root         (0)     7334 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_api_gateway_stage_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5143 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_auto_scaling_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_billing_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4306 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_billing_report_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8555 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_billing_report_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5131 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_classic_elb_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4975 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_cloud_watch_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7422 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_cognito_identity_providers_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     5083 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ebs_volume_snapshot_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     5083 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_reserved_instance_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5179 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_reserved_instance_coverage_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7430 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_reserved_instance_coverage_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     8314 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_reserved_instance_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5071 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_scheduled_events_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5047 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5059 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ecs_service_details_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7294 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ecs_service_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_elasti_cache_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4691 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_external_id.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_global_web_acl_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     7318 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_lb_target_group_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7358 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_media_connect_output_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7358 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_media_connect_source_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_rds_performance_insights_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5071 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_rds_service_limits_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7278 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_red_shift_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5143 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_route53_resolver_ip_address_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7406 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_route53_resolver_ip_address_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    22747 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_rss_event_source.py
--rw-r--r--   0 root         (0) root         (0)     7334 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_sage_maker_endpoint_variant_method.py
--rw-r--r--   0 root         (0) root         (0)     6202 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_service_limits_from_trusted_advisor_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8304 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_service_region_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5047 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ses_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_vpn_tunnel_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_web_acl_waf_v2_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5056 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_account_test_result.py
--rw-r--r--   0 root         (0) root         (0)     4410 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_active_directory_app_secret_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7422 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_active_directory_app_secret_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4370 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_active_directory_sync_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4378 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_active_directory_users_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5311 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_app_service_environment_multi_role_pool_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7494 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_app_service_environment_multi_role_pool_discover_method.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_authentication_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5324 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_automation_account_certificate_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7454 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_automation_account_certificate_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5096 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_job_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5300 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_protected_item_backup_job_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7454 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_protected_item_backup_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4418 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_protected_item_health_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4274 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_billing_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8298 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_billing_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4330 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_cost_management_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8669 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_cost_management_dimensions_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7446 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_cost_management_subscriptions_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     8346 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_cost_management_tags_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     9793 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_dimension_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4290 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_ea_billing_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8408 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_ea_billing_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)    23803 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_emerging_issue_event_source.py
--rw-r--r--   0 root         (0) root         (0)     5300 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_express_route_circuit_peering_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7438 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_express_route_circuit_peering_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4975 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_insights_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5276 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_log_analytics_replication_job_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7438 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_log_analytics_replication_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5207 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_log_analytics_workspaces_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     9321 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_log_analytics_workspaces_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7334 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_net_app_volumes_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_network_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5180 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_recovery_service_rto_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7374 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_recovery_service_rto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4394 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_recovery_service_vault_sr_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5288 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_recovery_services_vault_agents_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7310 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_redis_cache_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5288 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_replication_disaster_recovery_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5156 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_replication_job_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7342 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_replication_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5047 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_resource_health_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5351 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_resource_usage_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    22923 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_rss_event_source.py
--rw-r--r--   0 root         (0) root         (0)     7334 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_service_region_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_storage_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_subscription_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5722 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_subscription_id_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     8322 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_synapse_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     5179 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_virtual_desktop_host_pools_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     5215 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7438 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5071 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vm_backup_status_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     5276 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vm_backup_status_log_analytics_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5059 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vm_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5144 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vng_connection_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7334 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vng_connection_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4354 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vwan_vpn_connection_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7294 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vwan_vpn_connection_method.py
--rw-r--r--   0 root         (0) root         (0)     7342 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_web_app_instance_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5060 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_web_job_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7278 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_web_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5931 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/basic_authentication.py
--rw-r--r--   0 root         (0) root         (0)    14502 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/batch_job_execution_item.py
--rw-r--r--   0 root         (0) root         (0)    17697 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/batch_job_widget.py
--rw-r--r--   0 root         (0) root         (0)     5885 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/batch_job_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     9210 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/batch_script_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     9141 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_data.py
--rw-r--r--   0 root         (0) root         (0)    11118 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_data_point.py
--rw-r--r--   0 root         (0) root         (0)     8183 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_info.py
--rw-r--r--   0 root         (0) root         (0)     8905 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_item.py
--rw-r--r--   0 root         (0) root         (0)    14897 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_widget.py
--rw-r--r--   0 root         (0) root         (0)     5840 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     8515 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/cell_data.py
--rw-r--r--   0 root         (0) root         (0)     5810 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/chain.py
--rw-r--r--   0 root         (0) root         (0)     9659 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/cim_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     8560 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/cim_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    12564 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/cloud_watch_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    75716 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector.py
--rw-r--r--   0 root         (0) root         (0)     9807 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8185 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    73785 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_base.py
--rw-r--r--   0 root         (0) root         (0)    17946 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_group.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5510 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    23012 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_sdt.py
--rw-r--r--   0 root         (0) root         (0)    10151 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_version.py
--rw-r--r--   0 root         (0) root         (0)     5637 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_version_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5495 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/color_threshold.py
--rw-r--r--   0 root         (0) root         (0)     6035 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/column_header.py
--rw-r--r--   0 root         (0) root         (0)     5761 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/config_source_update_reasons_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     7210 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/conversation_filter.py
--rw-r--r--   0 root         (0) root         (0)     4480 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/counter.py
--rw-r--r--   0 root         (0) root         (0)    15312 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_flexible_virtual_data_source_ex.py
--rw-r--r--   0 root         (0) root         (0)    13816 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_graph.py
--rw-r--r--   0 root         (0) root         (0)    14681 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)    25497 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_report.py
--rw-r--r--   0 root         (0) root         (0)     6720 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_virtual_data_point.py
--rw-r--r--   0 root         (0) root         (0)    16001 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard.py
--rw-r--r--   0 root         (0) root         (0)     6467 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_data.py
--rw-r--r--   0 root         (0) root         (0)    14261 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_group.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5489 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    30522 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_report.py
--rw-r--r--   0 root         (0) root         (0)    30582 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_point.py
--rw-r--r--   0 root         (0) root         (0)     4242 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_pump_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    26876 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_source.py
--rw-r--r--   0 root         (0) root         (0)     5357 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_source_attribute.py
--rw-r--r--   0 root         (0) root         (0)    16730 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_source_overview_graph.py
--rw-r--r--   0 root         (0) root         (0)     5729 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_source_update_reasons_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5786 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/datasource_overview_graph_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5511 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/datasource_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     6691 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/days_until_alert.py
--rw-r--r--   0 root         (0) root         (0)     6167 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/debug.py
--rw-r--r--   0 root         (0) root         (0)    54658 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device.py
--rw-r--r--   0 root         (0) root         (0)    25341 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_batch_job_sdt.py
--rw-r--r--   0 root         (0) root         (0)    25754 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_cluster_alert_def_sdt.py
--rw-r--r--   0 root         (0) root         (0)    28761 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source.py
--rw-r--r--   0 root         (0) root         (0)     9096 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_associated.py
--rw-r--r--   0 root         (0) root         (0)     5544 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_associated_instance.py
--rw-r--r--   0 root         (0) root         (0)     5849 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_associated_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     6617 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_data.py
--rw-r--r--   0 root         (0) root         (0)    25047 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance.py
--rw-r--r--   0 root         (0) root         (0)    43828 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_alert_setting.py
--rw-r--r--   0 root         (0) root         (0)     4452 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_alert_setting_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    19383 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_config.py
--rw-r--r--   0 root         (0) root         (0)     7749 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_config_alert.py
--rw-r--r--   0 root         (0) root         (0)     5741 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_config_diff.py
--rw-r--r--   0 root         (0) root         (0)     6814 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_data.py
--rw-r--r--   0 root         (0) root         (0)     9626 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_group.py
--rw-r--r--   0 root         (0) root         (0)    29601 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_group_sdt.py
--rw-r--r--   0 root         (0) root         (0)    26558 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_sdt.py
--rw-r--r--   0 root         (0) root         (0)    25629 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_sdt.py
--rw-r--r--   0 root         (0) root         (0)     5767 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_sdt_history_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5894 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_graph.py
--rw-r--r--   0 root         (0) root         (0)     5934 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_instance_config_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5913 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_instance_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5807 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_instance_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5638 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     6230 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_delta_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    25773 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_event_source_sdt.py
--rw-r--r--   0 root         (0) root         (0)     5943 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_filter.py
--rw-r--r--   0 root         (0) root         (0)    47362 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group.py
--rw-r--r--   0 root         (0) root         (0)    15108 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_alert_threshold_info.py
--rw-r--r--   0 root         (0) root         (0)    16977 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_data.py
--rw-r--r--   0 root         (0) root         (0)    11283 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_data_source.py
--rw-r--r--   0 root         (0) root         (0)     5232 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_data_source_alert_config.py
--rw-r--r--   0 root         (0) root         (0)    31103 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_data_source_data_point_config.py
--rw-r--r--   0 root         (0) root         (0)     5744 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_datasource_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5532 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5687 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_sdt_history_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     7938 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_instance_data.py
--rw-r--r--   0 root         (0) root         (0)     5680 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_instance_data_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     4254 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_instances.py
--rw-r--r--   0 root         (0) root         (0)    26766 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_log_pipe_line_resource_sdt.py
--rw-r--r--   0 root         (0) root         (0)    10188 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_noc_item.py
--rw-r--r--   0 root         (0) root         (0)     5426 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     4830 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_property.py
--rw-r--r--   0 root         (0) root         (0)     5607 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_sdt_history_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    26278 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_sla_widget.py
--rw-r--r--   0 root         (0) root         (0)     5963 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_sla_widget_data.py
--rw-r--r--   0 root         (0) root         (0)    15260 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_status.py
--rw-r--r--   0 root         (0) root         (0)     4202 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dns_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    10033 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dummy_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4535 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_column.py
--rw-r--r--   0 root         (0) root         (0)    20003 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_table_widget.py
--rw-r--r--   0 root         (0) root         (0)    13685 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_table_widget_column.py
--rw-r--r--   0 root         (0) root         (0)     6800 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_table_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     6972 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_table_widget_row.py
--rw-r--r--   0 root         (0) root         (0)     9104 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4725 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_ddr.py
--rw-r--r--   0 root         (0) root         (0)    23223 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_netscan.py
--rw-r--r--   0 root         (0) root         (0)     6349 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_netscan_policy_credential.py
--rw-r--r--   0 root         (0) root         (0)     7358 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_scheduled_event_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    21776 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/echo_event_source.py
--rw-r--r--   0 root         (0) root         (0)    32001 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/enhanced_script_netscan.py
--rw-r--r--   0 root         (0) root         (0)     6405 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/entity_property.py
--rw-r--r--   0 root         (0) root         (0)     5712 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/error_response.py
--rw-r--r--   0 root         (0) root         (0)    11330 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/escalating_chain.py
--rw-r--r--   0 root         (0) root         (0)     5616 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/escalation_chain_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     7988 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/esx_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5711 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/esx_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    22412 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/event_source.py
--rw-r--r--   0 root         (0) root         (0)     5532 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/event_source_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     6418 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/exclude_duplicate_ips.py
--rw-r--r--   0 root         (0) root         (0)    14821 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/flash_widget.py
--rw-r--r--   0 root         (0) root         (0)     5527 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/flow_record_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    11579 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gauge_data_point.py
--rw-r--r--   0 root         (0) root         (0)    21714 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gauge_widget.py
--rw-r--r--   0 root         (0) root         (0)    14711 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gauge_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     5997 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_account_test_result.py
--rw-r--r--   0 root         (0) root         (0)     7286 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_app_engine_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    22835 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_atom_event_source.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_backend_service_health_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     4370 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_billing_big_query_source_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     9596 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_billing_big_query_source_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_billing_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8256 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_billing_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_compute_service_limits_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7358 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_lb_backend_service_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     7342 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_pub_sub_snapshot_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     7374 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_pub_sub_subscription_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_stack_driver_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_vpn_tunnel_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     6088 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/generate_report_request.py
--rw-r--r--   0 root         (0) root         (0)     5872 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/generate_report_result.py
--rw-r--r--   0 root         (0) root         (0)     4539 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/glob_match_toggle.py
--rw-r--r--   0 root         (0) root         (0)    19920 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/google_map_widget.py
--rw-r--r--   0 root         (0) root         (0)     5850 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/google_map_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     5675 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_display.py
--rw-r--r--   0 root         (0) root         (0)     8332 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_line.py
--rw-r--r--   0 root         (0) root         (0)     7472 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_ops_note_scope.py
--rw-r--r--   0 root         (0) root         (0)    26433 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_plot.py
--rw-r--r--   0 root         (0) root         (0)    13921 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_plot_line.py
--rw-r--r--   0 root         (0) root         (0)     4753 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_virtual_data_point.py
--rw-r--r--   0 root         (0) root         (0)    22567 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/group_net_flow_record.py
--rw-r--r--   0 root         (0) root         (0)    28465 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_cpu_report.py
--rw-r--r--   0 root         (0) root         (0)    28395 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_group_inventory_report.py
--rw-r--r--   0 root         (0) root         (0)     5838 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_inventory_metric.py
--rw-r--r--   0 root         (0) root         (0)    29610 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_inventory_report.py
--rw-r--r--   0 root         (0) root         (0)    35843 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_metrics_report.py
--rw-r--r--   0 root         (0) root         (0)    15075 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/html_widget.py
--rw-r--r--   0 root         (0) root         (0)    12009 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/http_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4624 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ilp.py
--rw-r--r--   0 root         (0) root         (0)     6235 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/inheritance_prop.py
--rw-r--r--   0 root         (0) root         (0)    13453 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/instance_group_alert_threshold_info.py
--rw-r--r--   0 root         (0) root         (0)    18372 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/integration_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     4228 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/integration_audit_log_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    21356 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/integration_metadata.py
--rw-r--r--   0 root         (0) root         (0)    32736 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/interf_bandwidth_report.py
--rw-r--r--   0 root         (0) root         (0)     4591 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/interface_type.py
--rw-r--r--   0 root         (0) root         (0)     4920 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/interfaces_filter.py
--rw-r--r--   0 root         (0) root         (0)     4242 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/internal_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7915 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ipmi_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4966 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ipmi_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    22743 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ipmi_event_source.py
--rw-r--r--   0 root         (0) root         (0)    18674 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/item_data.py
--rw-r--r--   0 root         (0) root         (0)    11413 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/jdbc_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     6838 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/jdbc_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     9346 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/jmx_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5487 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/jmx_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7588 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/linked_wmi_class.py
--rw-r--r--   0 root         (0) root         (0)     5199 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/location_data.py
--rw-r--r--   0 root         (0) root         (0)     7918 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/log_file.py
--rw-r--r--   0 root         (0) root         (0)    22894 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/log_file_event_source.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/macro.py
--rw-r--r--   0 root         (0) root         (0)    12046 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/map_item_info.py
--rw-r--r--   0 root         (0) root         (0)     4968 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/match_pattern.py
--rw-r--r--   0 root         (0) root         (0)     5484 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/memcached_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7132 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/metric.py
--rw-r--r--   0 root         (0) root         (0)     5105 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/n_map_ddr.py
--rw-r--r--   0 root         (0) root         (0)    24517 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/n_map_netscan.py
--rw-r--r--   0 root         (0) root         (0)     4790 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/name_and_value.py
--rw-r--r--   0 root         (0) root         (0)     4836 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/nbar_application_names.py
--rw-r--r--   0 root         (0) root         (0)    13719 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/net_app_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    15795 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/net_app_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    19373 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/net_flow_record.py
--rw-r--r--   0 root         (0) root         (0)    11502 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_alert_modules_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)    14493 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_application.py
--rw-r--r--   0 root         (0) root         (0)     8968 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_bandwidth.py
--rw-r--r--   0 root         (0) root         (0)     7298 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_bgp_table.py
--rw-r--r--   0 root         (0) root         (0)     4602 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_data_base.py
--rw-r--r--   0 root         (0) root         (0)     5260 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_device_info.py
--rw-r--r--   0 root         (0) root         (0)     7850 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_endpoint.py
--rw-r--r--   0 root         (0) root         (0)    13843 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_filters.py
--rw-r--r--   0 root         (0) root         (0)    17146 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)    15867 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_group_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)    18040 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_group_widget.py
--rw-r--r--   0 root         (0) root         (0)     6555 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_group_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     7637 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_nbar_application.py
--rw-r--r--   0 root         (0) root         (0)     6677 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_port.py
--rw-r--r--   0 root         (0) root         (0)     6403 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_qo_s_report_table_row.py
--rw-r--r--   0 root         (0) root         (0)    28517 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_report.py
--rw-r--r--   0 root         (0) root         (0)    17526 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_widget.py
--rw-r--r--   0 root         (0) root         (0)     6455 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_widget_data.py
--rw-r--r--   0 root         (0) root         (0)    18904 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netscan.py
--rw-r--r--   0 root         (0) root         (0)     5447 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netscan_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     7754 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/next_upgrade_info.py
--rw-r--r--   0 root         (0) root         (0)     4291 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/noc_item_base.py
--rw-r--r--   0 root         (0) root         (0)    21151 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/noc_widget.py
--rw-r--r--   0 root         (0) root         (0)     7184 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/noc_widget_data.py
--rw-r--r--   0 root         (0) root         (0)    19809 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/normal_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)     6556 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ntlm_authentication.py
--rw-r--r--   0 root         (0) root         (0)     9929 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/onetime_upgrade_info.py
--rw-r--r--   0 root         (0) root         (0)     8159 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/open_metric_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)    14851 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/open_metric_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     8566 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note.py
--rw-r--r--   0 root         (0) root         (0)     5525 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_device_group_scope.py
--rw-r--r--   0 root         (0) root         (0)     6885 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_device_scope.py
--rw-r--r--   0 root         (0) root         (0)     4769 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_group_all_scope.py
--rw-r--r--   0 root         (0) root         (0)     5448 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     4455 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_scope.py
--rw-r--r--   0 root         (0) root         (0)     6212 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_tag_base.py
--rw-r--r--   0 root         (0) root         (0)     5541 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_website_group_scope.py
--rw-r--r--   0 root         (0) root         (0)     6949 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_website_scope.py
--rw-r--r--   0 root         (0) root         (0)     8352 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/overview_graph_data_point.py
--rw-r--r--   0 root         (0) root         (0)    19498 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/overview_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)    13675 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/paa_s_json_path_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5161 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/paa_s_mongo_db_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     8834 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pdh_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5080 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/perfmon_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5050 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/perfmon_counter.py
--rw-r--r--   0 root         (0) root         (0)     6757 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/period.py
--rw-r--r--   0 root         (0) root         (0)     5978 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_data.py
--rw-r--r--   0 root         (0) root         (0)    12398 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_data_point.py
--rw-r--r--   0 root         (0) root         (0)    13497 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_info.py
--rw-r--r--   0 root         (0) root         (0)     5455 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_item.py
--rw-r--r--   0 root         (0) root         (0)    14703 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_widget.py
--rw-r--r--   0 root         (0) root         (0)     8818 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_widget_data.py
--rw-r--r--   0 root         (0) root         (0)    38842 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ping_check.py
--rw-r--r--   0 root         (0) root         (0)     5503 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ping_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7467 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/point_source.py
--rw-r--r--   0 root         (0) root         (0)     8660 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/port_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     8038 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/privilege.py
--rw-r--r--   0 root         (0) root         (0)     4846 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/property_match_rule.py
--rw-r--r--   0 root         (0) root         (0)     5499 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/property_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     4266 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/push_modules_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    12660 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rabbit_mq_queue_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5619 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/raw_data_values.py
--rw-r--r--   0 root         (0) root         (0)     7027 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/recipient.py
--rw-r--r--   0 root         (0) root         (0)     6485 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/recipient_group.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/recipient_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    24993 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_base.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_group.py
--rw-r--r--   0 root         (0) root         (0)     5532 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     5447 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     7094 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_recipient.py
--rw-r--r--   0 root         (0) root         (0)    25610 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/resource_group_sdt.py
--rw-r--r--   0 root         (0) root         (0)    22708 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/resource_sdt.py
--rw-r--r--   0 root         (0) root         (0)     5723 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_applies_to_function_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    11433 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_aws_account_test_v3.py
--rw-r--r--   0 root         (0) root         (0)    23363 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_aws_health_event_source.py
--rw-r--r--   0 root         (0) root         (0)    26431 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_aws_rds_performance_insights_event_source.py
--rw-r--r--   0 root         (0) root         (0)    24067 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_aws_trusted_advisor_event_source.py
--rw-r--r--   0 root         (0) root         (0)     8741 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_account_test_v3.py
--rw-r--r--   0 root         (0) root         (0)    23627 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_advisor_event_source.py
--rw-r--r--   0 root         (0) root         (0)    24243 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_resource_health_event_source.py
--rw-r--r--   0 root         (0) root         (0)    27171 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_resource_log_analytics_workspaces_source.py
--rw-r--r--   0 root         (0) root         (0)     9293 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_subscription_v3.py
--rw-r--r--   0 root         (0) root         (0)     7269 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_subscriptions_discover_v3.py
--rw-r--r--   0 root         (0) root         (0)     3315 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_cloud_ok_permissions_v3.py
--rw-r--r--   0 root         (0) root         (0)     4197 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_dashboard_group_async_clone_response.py
--rw-r--r--   0 root         (0) root         (0)    22060 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_device_instance_group_alert_config_v3.py
--rw-r--r--   0 root         (0) root         (0)     7220 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_event_source_filter.py
--rw-r--r--   0 root         (0) root         (0)     6470 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_gcp_account_test_v3.py
--rw-r--r--   0 root         (0) root         (0)     6780 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_highest_priority_collector_status.py
--rw-r--r--   0 root         (0) root         (0)     9563 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_n_map_netscan_policy_credential.py
--rw-r--r--   0 root         (0) root         (0)     5016 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_netscan_ports.py
--rw-r--r--   0 root         (0) root         (0)    10663 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_saa_s_account_test_v3.py
--rw-r--r--   0 root         (0) root         (0)    17140 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_saved_map_widget_v3.py
--rw-r--r--   0 root         (0) root         (0)     7237 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_schedule.py
--rw-r--r--   0 root         (0) root         (0)     4545 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_user_customized_data_v3.py
--rw-r--r--   0 root         (0) root         (0)     5284 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/result_item.py
--rw-r--r--   0 root         (0) root         (0)    15596 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/role.py
--rw-r--r--   0 root         (0) root         (0)     5384 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/role_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    25748 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/role_report.py
--rw-r--r--   0 root         (0) root         (0)     5443 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/row_data.py
--rw-r--r--   0 root         (0) root         (0)     7310 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_s_slack_health_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7318 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_s_webex_license_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     8399 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_s_zoom_plan_usage_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7302 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_s_zoom_status_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7366 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_so365_share_point_site_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     8646 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_account_test_result.py
--rw-r--r--   0 root         (0) root         (0)     4274 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_airbrake_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7286 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_airbrake_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7286 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_o365_skus_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7310 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_o365_mailbox_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7358 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_o365_service_health_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7048 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_csv_report_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     4346 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_health_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     5276 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_sharepoint_report_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     5108 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_skus_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4402 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_teams_calls_qos_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     4418 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_salesforce_instance_status_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     6136 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_salesforce_json_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7358 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_salesforce_license_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     9687 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_salesforce_soql_query_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     7015 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_slack_health_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_status_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7270 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_status_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     7850 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_webex_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     6040 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_zoom_json_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     5911 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_zoom_plan_usage_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     8339 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_zoom_room_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    11902 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    11365 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     9328 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_eri_discovery_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)    28169 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_event_source.py
--rw-r--r--   0 root         (0) root         (0)    29024 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_netscan.py
--rw-r--r--   0 root         (0) root         (0)     6827 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdk_script_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     9803 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdk_script_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    21066 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdt.py
--rw-r--r--   0 root         (0) root         (0)     9554 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdt_history.py
--rw-r--r--   0 root         (0) root         (0)     5363 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdt_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    15260 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/service_alert.py
--rw-r--r--   0 root         (0) root         (0)     5743 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/site_monitor_check_point_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     8541 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/site_monitor_checkpoint.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sla_metric.py
--rw-r--r--   0 root         (0) root         (0)    34917 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sla_report.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/snmp_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     4787 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/snmp_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    22112 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/snmp_trap_event_source.py
--rw-r--r--   0 root         (0) root         (0)     5103 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/snmpilp.py
--rw-r--r--   0 root         (0) root         (0)     7569 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/stats_d_graph.py
--rw-r--r--   0 root         (0) root         (0)     5795 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/stats_d_graph_display.py
--rw-r--r--   0 root         (0) root         (0)     6575 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/stats_d_metric_definition.py
--rw-r--r--   0 root         (0) root         (0)    14422 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/stats_d_widget.py
--rw-r--r--   0 root         (0) root         (0)     9034 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/synthetics_selenium_auto_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     7029 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/synthetics_selenium_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    21944 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sys_log_event_source.py
--rw-r--r--   0 root         (0) root         (0)    16103 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget.py
--rw-r--r--   0 root         (0) root         (0)     9096 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_column.py
--rw-r--r--   0 root         (0) root         (0)     6660 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     7602 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_data_point.py
--rw-r--r--   0 root         (0) root         (0)     7362 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_forecast_configuration.py
--rw-r--r--   0 root         (0) root         (0)     7578 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_instance_cell.py
--rw-r--r--   0 root         (0) root         (0)     7872 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_row.py
--rw-r--r--   0 root         (0) root         (0)     6854 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/tcp_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    14390 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/text_widget.py
--rw-r--r--   0 root         (0) root         (0)     5833 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/tree_node.py
--rw-r--r--   0 root         (0) root         (0)     5488 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/udp_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5663 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/unmonitored_device_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    16516 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/unmonitored_devices.py
--rw-r--r--   0 root         (0) root         (0)     7862 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/update_reason.py
--rw-r--r--   0 root         (0) root         (0)    23013 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/usage.py
--rw-r--r--   0 root         (0) root         (0)     9690 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/user_filter.py
--rw-r--r--   0 root         (0) root         (0)    26447 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/user_report.py
--rw-r--r--   0 root         (0) root         (0)     4449 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/virtual_data_point.py
--rw-r--r--   0 root         (0) root         (0)    40343 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/web_check.py
--rw-r--r--   0 root         (0) root         (0)    25338 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/web_check_step.py
--rw-r--r--   0 root         (0) root         (0)     9319 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/web_page_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4828 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/web_resource.py
--rw-r--r--   0 root         (0) root         (0)    34431 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website.py
--rw-r--r--   0 root         (0) root         (0)     5552 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_check_point.py
--rw-r--r--   0 root         (0) root         (0)     5795 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_checkpoint_raw_data.py
--rw-r--r--   0 root         (0) root         (0)    23943 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_checkpoint_sdt.py
--rw-r--r--   0 root         (0) root         (0)     8469 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_collector_info.py
--rw-r--r--   0 root         (0) root         (0)    17442 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)    18363 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_group.py
--rw-r--r--   0 root         (0) root         (0)     5432 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_group_data.py
--rw-r--r--   0 root         (0) root         (0)     5553 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    23248 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_group_sdt.py
--rw-r--r--   0 root         (0) root         (0)    21417 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_individuals_status_widget.py
--rw-r--r--   0 root         (0) root         (0)     5637 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_item_config.py
--rw-r--r--   0 root         (0) root         (0)     6721 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_location.py
--rw-r--r--   0 root         (0) root         (0)     7157 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_noc_item.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_overall_status_widget.py
--rw-r--r--   0 root         (0) root         (0)    32299 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_overview_report.py
--rw-r--r--   0 root         (0) root         (0)    16966 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_overview_widget.py
--rw-r--r--   0 root         (0) root         (0)     5447 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    22451 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sdt.py
--rw-r--r--   0 root         (0) root         (0)     5623 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sdt_history_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)    28341 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sla_report.py
--rw-r--r--   0 root         (0) root         (0)    19006 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sla_widget.py
--rw-r--r--   0 root         (0) root         (0)     6637 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sla_widget_data.py
--rw-r--r--   0 root         (0) root         (0)    14722 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget.py
--rw-r--r--   0 root         (0) root         (0)     5778 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget_data.py
--rw-r--r--   0 root         (0) root         (0)     5426 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     6565 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget_token.py
--rw-r--r--   0 root         (0) root         (0)     4863 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget_token_inheritance.py
--rw-r--r--   0 root         (0) root         (0)    22700 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/windows_event_log_event_source.py
--rw-r--r--   0 root         (0) root         (0)    15135 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/wmi_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)    10653 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/wmi_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7988 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/xen_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     5790 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/xen_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    49097 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28149 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/api_client.py
--rw-r--r--   0 root         (0) root         (0)     9155 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/configuration.py
--rw-r--r--   0 root         (0) root         (0)    14056 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1294 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    51927 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/logicmonitor_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_access_log_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_ack_collector_down.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_admin.py
--rw-r--r--   0 root         (0) root         (0)     1838 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_admin_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aggregate_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert_ack.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert_filters.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_alert_forecasting_report.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert_list_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1838 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_alert_report.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert_response.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert_rule.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert_rule_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_alert_sla_report.py
--rw-r--r--   0 root         (0) root         (0)     1814 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_alert_threshold_report.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_alert_trends_metric.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_alert_trends_report.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_alert_widget.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_alert_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_api_perf_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_api_token.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_api_token_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_applies_to_function.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_assignment.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_audit_log_report.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_authentication.py
--rw-r--r--   0 root         (0) root         (0)     1862 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_auto_discovery_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_auto_discovery_filter.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1814 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_automatic_upgrade_info.py
--rw-r--r--   0 root         (0) root         (0)     1750 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_aws_account_id.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_aws_account_test_result.py
--rw-r--r--   0 root         (0) root         (0)     1924 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_api_gateway_stage_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_auto_scaling_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1880 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_billing_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_billing_report_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_billing_report_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2014 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_classic_elb_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_cloud_watch_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2014 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_cognito_identity_providers_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1982 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ebs_volume_snapshot_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ec2_reserved_instance_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2046 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ec2_reserved_instance_coverage_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ec2_reserved_instance_coverage_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1956 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ec2_reserved_instance_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ec2_scheduled_events_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1956 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ec2_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ecs_service_details_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1882 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ecs_service_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_elasti_cache_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_aws_external_id.py
--rw-r--r--   0 root         (0) root         (0)     1918 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_global_web_acl_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_lb_target_group_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1948 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_media_connect_output_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1948 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_media_connect_source_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_rds_performance_insights_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1974 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_rds_service_limits_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1866 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_red_shift_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_route53_resolver_ip_address_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1998 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_route53_resolver_ip_address_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_rss_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1924 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_sage_maker_endpoint_variant_method.py
--rw-r--r--   0 root         (0) root         (0)     2080 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_service_limits_from_trusted_advisor_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_service_region_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1956 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_ses_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_vpn_tunnel_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1894 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_aws_web_acl_waf_v2_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_azure_account_test_result.py
--rw-r--r--   0 root         (0) root         (0)     2038 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_active_directory_app_secret_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2014 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_active_directory_app_secret_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_active_directory_sync_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_active_directory_users_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2140 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_app_service_environment_multi_role_pool_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     2090 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_app_service_environment_multi_role_pool_discover_method.py
--rw-r--r--   0 root         (0) root         (0)     1878 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_authentication_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2086 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_automation_account_certificate_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     2044 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_automation_account_certificate_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_backup_job_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_backup_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2072 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_backup_protected_item_backup_job_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2048 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_backup_protected_item_backup_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2046 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_backup_protected_item_health_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_billing_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_billing_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1954 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_cost_management_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2012 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_cost_management_dimensions_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2036 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_cost_management_subscriptions_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_cost_management_tags_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1888 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_dimension_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1914 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_ea_billing_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_ea_billing_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_emerging_issue_event_source.py
--rw-r--r--   0 root         (0) root         (0)     2072 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_express_route_circuit_peering_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_express_route_circuit_peering_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1904 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_insights_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2054 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_log_analytics_replication_job_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_log_analytics_replication_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2020 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_log_analytics_workspaces_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_log_analytics_workspaces_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1924 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_net_app_volumes_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_network_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1988 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_recovery_service_rto_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_recovery_service_rto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_recovery_service_vault_sr_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_recovery_services_vault_agents_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1898 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_redis_cache_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_replication_disaster_recovery_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_replication_job_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_replication_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1954 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_resource_health_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1946 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_resource_usage_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_rss_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_service_region_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_storage_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_subscription_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1954 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_azure_subscription_id_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_synapse_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     2048 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_virtual_desktop_host_pools_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     2072 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_virtual_desktop_session_hosts_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_virtual_desktop_session_hosts_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1974 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_vm_backup_status_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_vm_backup_status_log_analytics_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_vm_service_limits_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_vng_connection_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_vng_connection_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_vwan_vpn_connection_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1882 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_vwan_vpn_connection_method.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_web_app_instance_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_web_job_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1866 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_azure_web_job_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1804 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_basic_authentication.py
--rw-r--r--   0 root         (0) root         (0)     1824 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_batch_job_execution_item.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_batch_job_widget.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_batch_job_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1888 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_batch_script_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_big_number_data.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_big_number_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_big_number_info.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_big_number_item.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_big_number_widget.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_big_number_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_cell_data.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_chain.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_cim_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_cim_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_cloud_watch_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_collector.py
--rw-r--r--   0 root         (0) root         (0)     1796 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1880 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_collector_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_collector_base.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_collector_group.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_collector_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_collector_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_collector_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_collector_version.py
--rw-r--r--   0 root         (0) root         (0)     1928 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_collector_version_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_color_threshold.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_column_header.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_config_source_update_reasons_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1796 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_conversation_filter.py
--rw-r--r--   0 root         (0) root         (0)     1706 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_counter.py
--rw-r--r--   0 root         (0) root         (0)     1924 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_custom_flexible_virtual_data_source_ex.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_custom_graph.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_custom_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_custom_report.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_custom_virtual_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_dashboard_data.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_dashboard_group.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_dashboard_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_dashboard_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_dashboard_report.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_data_pump_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_data_source.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_data_source_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_data_source_overview_graph.py
--rw-r--r--   0 root         (0) root         (0)     1988 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_data_source_update_reasons_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_datasource_overview_graph_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1878 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_datasource_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_days_until_alert.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_debug.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_batch_job_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1850 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_cluster_alert_def_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_associated.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_associated_instance.py
--rw-r--r--   0 root         (0) root         (0)     2012 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_associated_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_data.py
--rw-r--r--   0 root         (0) root         (0)     1848 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance.py
--rw-r--r--   0 root         (0) root         (0)     1948 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_alert_setting.py
--rw-r--r--   0 root         (0) root         (0)     2096 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_alert_setting_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1898 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_config.py
--rw-r--r--   0 root         (0) root         (0)     1940 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_config_alert.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_config_diff.py
--rw-r--r--   0 root         (0) root         (0)     1882 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_data.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_group.py
--rw-r--r--   0 root         (0) root         (0)     1916 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_group_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1874 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_sdt.py
--rw-r--r--   0 root         (0) root         (0)     2014 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_data_source_sdt_history_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_datasource_graph.py
--rw-r--r--   0 root         (0) root         (0)     2044 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_datasource_instance_config_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     2036 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_datasource_instance_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1994 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_datasource_instance_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1928 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_datasource_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1888 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_delta_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_event_source_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group_alert_threshold_info.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group_data.py
--rw-r--r--   0 root         (0) root         (0)     1824 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group_data_source.py
--rw-r--r--   0 root         (0) root         (0)     1916 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group_data_source_alert_config.py
--rw-r--r--   0 root         (0) root         (0)     1950 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group_data_source_data_point_config.py
--rw-r--r--   0 root         (0) root         (0)     1970 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group_datasource_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1888 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_group_sdt_history_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1798 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_instance_data.py
--rw-r--r--   0 root         (0) root         (0)     1946 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_instance_data_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_instances.py
--rw-r--r--   0 root         (0) root         (0)     1884 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_log_pipe_line_resource_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_noc_item.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_property.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-01-22 07:39:47.000000 logicmonitor-sdk-3.0.200/test/test_device_sdt_history_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_sla_widget.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_sla_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_device_status.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_dns_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1848 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_dummy_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_dynamic_column.py
--rw-r--r--   0 root         (0) root         (0)     1798 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_dynamic_table_widget.py
--rw-r--r--   0 root         (0) root         (0)     1848 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_dynamic_table_widget_column.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_dynamic_table_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1824 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_dynamic_table_widget_row.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ec2_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1700 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ec2_ddr.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ec2_netscan.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ec2_netscan_policy_credential.py
--rw-r--r--   0 root         (0) root         (0)     1948 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ec2_scheduled_event_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_echo_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_enhanced_script_netscan.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_entity_property.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_escalating_chain.py
--rw-r--r--   0 root         (0) root         (0)     1920 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_escalation_chain_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_esx_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_esx_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1888 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_event_source_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_exclude_duplicate_ips.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_flash_widget.py
--rw-r--r--   0 root         (0) root         (0)     1880 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_flow_record_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gauge_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gauge_widget.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gauge_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_account_test_result.py
--rw-r--r--   0 root         (0) root         (0)     1874 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_app_engine_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_atom_event_source.py
--rw-r--r--   0 root         (0) root         (0)     2006 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_backend_service_health_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1998 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_billing_big_query_source_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1992 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_billing_big_query_source_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1880 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_billing_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1874 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_billing_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     2006 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_compute_service_limits_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1950 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_lb_backend_service_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1934 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_pub_sub_snapshot_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1966 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_pub_sub_subscription_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_stack_driver_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_gcp_vpn_tunnel_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_generate_report_request.py
--rw-r--r--   0 root         (0) root         (0)     1814 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_generate_report_result.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_glob_match_toggle.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_google_map_widget.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_google_map_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_graph_display.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_graph_line.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_graph_ops_note_scope.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_graph_plot.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_graph_plot_line.py
--rw-r--r--   0 root         (0) root         (0)     1824 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_graph_virtual_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_group_net_flow_record.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_host_cpu_report.py
--rw-r--r--   0 root         (0) root         (0)     1848 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_host_group_inventory_report.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_host_inventory_metric.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_host_inventory_report.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_host_metrics_report.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_html_widget.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_http_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ilp.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_inheritance_prop.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_instance_group_alert_threshold_info.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_integration_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1682 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_role.py
--rw-r--r--   0 root         (0) root         (0)     1954 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_integration_audit_log_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1804 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_integration_metadata.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_interf_bandwidth_report.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_interface_type.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_interfaces_filter.py
--rw-r--r--   0 root         (0) root         (0)     1862 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_internal_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ipmi_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ipmi_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ipmi_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_item_data.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_jdbc_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_jdbc_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_jmx_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_jmx_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_linked_wmi_class.py
--rw-r--r--   0 root         (0) root         (0)    40673 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/test/test_lm_api.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_location_data.py
--rw-r--r--   0 root         (0) root         (0)     1708 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_log_file.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_log_file_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_macro.py
--rw-r--r--   0 root         (0) root         (0)     1742 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_map_item_info.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_match_pattern.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_memcached_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_n_map_ddr.py
--rw-r--r--   0 root         (0) root         (0)     1742 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_n_map_netscan.py
--rw-r--r--   0 root         (0) root         (0)     1750 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_name_and_value.py
--rw-r--r--   0 root         (0) root         (0)     1814 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_nbar_application_names.py
--rw-r--r--   0 root         (0) root         (0)     1858 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_net_app_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1848 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_net_app_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_net_flow_record.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_alert_modules_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1796 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_application.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_bandwidth.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_bgp_table.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_netflow_data_base.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_netflow_device_info.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_endpoint.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_netflow_filters.py
--rw-r--r--   0 root         (0) root         (0)     1798 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_group_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)     1798 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_group_widget.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_group_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_nbar_application.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_port.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_qo_s_report_table_row.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_report.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_widget.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_netflow_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1706 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_netscan.py
--rw-r--r--   0 root         (0) root         (0)     1854 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_netscan_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_next_upgrade_info.py
--rw-r--r--   0 root         (0) root         (0)     1742 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_noc_item_base.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_noc_widget.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_noc_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_normal_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)     1796 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ntlm_authentication.py
--rw-r--r--   0 root         (0) root         (0)     1798 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_onetime_upgrade_info.py
--rw-r--r--   0 root         (0) root         (0)     1898 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_open_metric_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1856 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_open_metric_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1708 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ops_note.py
--rw-r--r--   0 root         (0) root         (0)     1842 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ops_note_device_group_scope.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ops_note_device_scope.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ops_note_group_all_scope.py
--rw-r--r--   0 root         (0) root         (0)     1856 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ops_note_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1750 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ops_note_scope.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_ops_note_tag_base.py
--rw-r--r--   0 root         (0) root         (0)     1850 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ops_note_website_group_scope.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ops_note_website_scope.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_overview_graph_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_overview_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)     1876 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_paa_s_json_path_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_paa_s_mongo_db_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_pdh_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1854 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_perfmon_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_perfmon_counter.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_period.py
--rw-r--r--   0 root         (0) root         (0)     1750 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_pie_chart_data.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_pie_chart_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1750 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_pie_chart_info.py
--rw-r--r--   0 root         (0) root         (0)     1750 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_pie_chart_item.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_pie_chart_widget.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_pie_chart_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ping_check.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_ping_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_point_source.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_port_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_privilege.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_property_match_rule.py
--rw-r--r--   0 root         (0) root         (0)     1862 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_property_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1888 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_push_modules_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1916 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_rabbit_mq_queue_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1758 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_raw_data_values.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_recipient.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_recipient_group.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_recipient_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_report_base.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_report_group.py
--rw-r--r--   0 root         (0) root         (0)     1888 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_report_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_report_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_report_recipient.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_resource_group_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_resource_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_applies_to_function_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_aws_account_test_v3.py
--rw-r--r--   0 root         (0) root         (0)     1850 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_rest_aws_health_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1982 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_rest_aws_rds_performance_insights_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1916 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_rest_aws_trusted_advisor_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1834 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_azure_account_test_v3.py
--rw-r--r--   0 root         (0) root         (0)     1874 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_rest_azure_advisor_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_rest_azure_resource_health_event_source.py
--rw-r--r--   0 root         (0) root         (0)     2022 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_rest_azure_resource_log_analytics_workspaces_source.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_azure_subscription_v3.py
--rw-r--r--   0 root         (0) root         (0)     1914 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_azure_subscriptions_discover_v3.py
--rw-r--r--   0 root         (0) root         (0)     1850 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_cloud_ok_permissions_v3.py
--rw-r--r--   0 root         (0) root         (0)     1948 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_dashboard_group_async_clone_response.py
--rw-r--r--   0 root         (0) root         (0)     1950 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_device_instance_group_alert_config_v3.py
--rw-r--r--   0 root         (0) root         (0)     1824 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_event_source_filter.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_gcp_account_test_v3.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_highest_priority_collector_status.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_n_map_netscan_policy_credential.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_netscan_ports.py
--rw-r--r--   0 root         (0) root         (0)     1828 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_saa_s_account_test_v3.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_rest_saved_map_widget_v3.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1850 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_rest_user_customized_data_v3.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_result_item.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_role_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_role_report.py
--rw-r--r--   0 root         (0) root         (0)     1708 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_row_data.py
--rw-r--r--   0 root         (0) root         (0)     1900 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saa_s_slack_health_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1908 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saa_s_webex_license_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1918 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saa_s_zoom_plan_usage_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saa_s_zoom_status_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saa_so365_share_point_site_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1824 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_saas_account_test_result.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_airbrake_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_airbrake_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1898 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_o365_mailbox_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1948 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_o365_service_health_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1874 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_o365_skus_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1998 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_office365_csv_report_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_office365_health_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     2054 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_office365_sharepoint_report_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_office365_skus_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2032 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_office365_teams_calls_qos_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     2046 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_salesforce_instance_status_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_salesforce_json_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1946 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_salesforce_license_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     2006 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_salesforce_soql_query_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_slack_health_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1880 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_status_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1856 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_status_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_webex_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1916 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_zoom_json_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_zoom_plan_usage_collector_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1874 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_saas_zoom_room_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1856 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_script_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_script_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_script_eri_discovery_attribute_v3.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_script_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1756 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_script_netscan.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_sdk_script_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1848 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_sdk_script_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_sdt_history.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_sdt_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_service_alert.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_site_monitor_check_point_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_site_monitor_checkpoint.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_sla_metric.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_sla_report.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_snmp_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_snmp_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1808 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_snmp_trap_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1706 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_snmpilp.py
--rw-r--r--   0 root         (0) root         (0)     1742 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_stats_d_graph.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_stats_d_graph_display.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_stats_d_metric_definition.py
--rw-r--r--   0 root         (0) root         (0)     1750 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_stats_d_widget.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_synthetics_selenium_auto_discovery_method_v3.py
--rw-r--r--   0 root         (0) root         (0)     1944 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_synthetics_selenium_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_sys_log_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_table_widget.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_table_widget_column.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_table_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_table_widget_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_table_widget_forecast_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_table_widget_instance_cell.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_table_widget_row.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_tcp_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_text_widget.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_tree_node.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_udp_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1936 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_unmonitored_device_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1796 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_unmonitored_devices.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_update_reason.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_usage.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_user_filter.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_user_report.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_virtual_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_web_check.py
--rw-r--r--   0 root         (0) root         (0)     1750 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_web_check_step.py
--rw-r--r--   0 root         (0) root         (0)     1856 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_web_page_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_web_resource.py
--rw-r--r--   0 root         (0) root         (0)     1706 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_check_point.py
--rw-r--r--   0 root         (0) root         (0)     1848 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_checkpoint_raw_data.py
--rw-r--r--   0 root         (0) root         (0)     1814 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_checkpoint_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1814 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_collector_info.py
--rw-r--r--   0 root         (0) root         (0)     1798 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_graph_widget.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_group.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_group_data.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_group_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1774 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_group_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_individuals_status_widget.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_item_config.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_location.py
--rw-r--r--   0 root         (0) root         (0)     1766 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_noc_item.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_overall_status_widget.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_overview_report.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_overview_widget.py
--rw-r--r--   0 root         (0) root         (0)     1854 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_sdt.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_website_sdt_history_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_sla_report.py
--rw-r--r--   0 root         (0) root         (0)     1782 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_sla_widget.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_website_sla_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_widget.py
--rw-r--r--   0 root         (0) root         (0)     1732 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_widget_data.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_widget_pagination_response.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_widget_token.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-01-22 07:39:48.000000 logicmonitor-sdk-3.0.200/test/test_widget_token_inheritance.py
--rw-r--r--   0 root         (0) root         (0)     1866 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_windows_event_log_event_source.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_wmi_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_wmi_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_xen_auto_discovery_method.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-01-22 07:39:49.000000 logicmonitor-sdk-3.0.200/test/test_xen_collector_attribute.py
--rw-r--r--   0 root         (0) root         (0)    72692 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/README.md
--rw-r--r--   0 root         (0) root         (0)     2765 2024-01-22 07:39:50.000000 logicmonitor-sdk-3.0.200/setup.py
--rw-r--r--   0 root         (0) root         (0)     1294 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-22 11:15:10.000000 logicmonitor-sdk-3.0.200/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/api/
+-rw-r--r--   0 root         (0) root         (0)      133 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1110053 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/api/lm_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/
+-rw-r--r--   0 root         (0) root         (0)    49642 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8611 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/access_group.py
+-rw-r--r--   0 root         (0) root         (0)     4123 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/access_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/access_log_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     3936 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ack_collector_down.py
+-rw-r--r--   0 root         (0) root         (0)    30796 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/admin.py
+-rw-r--r--   0 root         (0) root         (0)     5405 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/admin_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aggregate_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    45218 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert.py
+-rw-r--r--   0 root         (0) root         (0)     4137 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_ack.py
+-rw-r--r--   0 root         (0) root         (0)    16729 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_filters.py
+-rw-r--r--   0 root         (0) root         (0)    34050 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_forecasting_report.py
+-rw-r--r--   0 root         (0) root         (0)     5510 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_list_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5405 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    47847 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_report.py
+-rw-r--r--   0 root         (0) root         (0)    45803 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_response.py
+-rw-r--r--   0 root         (0) root         (0)    18556 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_rule_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    31680 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_sla_report.py
+-rw-r--r--   0 root         (0) root         (0)    33107 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_threshold_report.py
+-rw-r--r--   0 root         (0) root         (0)     4834 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_trends_metric.py
+-rw-r--r--   0 root         (0) root         (0)    27021 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_trends_report.py
+-rw-r--r--   0 root         (0) root         (0)    15220 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_widget.py
+-rw-r--r--   0 root         (0) root         (0)     7051 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)    11241 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/api_perf_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    12872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/api_token.py
+-rw-r--r--   0 root         (0) root         (0)     5469 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/api_token_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     9586 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/applies_to_function.py
+-rw-r--r--   0 root         (0) root         (0)     7952 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/assignment.py
+-rw-r--r--   0 root         (0) root         (0)     8226 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    28756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/audit_log_report.py
+-rw-r--r--   0 root         (0) root         (0)     6135 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/authentication.py
+-rw-r--r--   0 root         (0) root         (0)    12116 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/auto_discovery_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6777 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/auto_discovery_filter.py
+-rw-r--r--   0 root         (0) root         (0)    12172 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    10539 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/automatic_upgrade_info.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_account_id.py
+-rw-r--r--   0 root         (0) root         (0)     5997 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_account_test_result.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_api_gateway_stage_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5143 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_auto_scaling_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_billing_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_billing_report_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8555 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_billing_report_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5131 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_classic_elb_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_cloud_watch_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7422 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_cognito_identity_providers_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5083 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ebs_volume_snapshot_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5083 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_reserved_instance_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_reserved_instance_coverage_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7430 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_reserved_instance_coverage_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     8314 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_reserved_instance_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5071 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_scheduled_events_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5047 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ecs_service_details_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7294 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ecs_service_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_elasti_cache_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_external_id.py
+-rw-r--r--   0 root         (0) root         (0)     7294 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_global_network_device_method.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_global_network_link_method.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_global_web_acl_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_lb_target_group_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_media_connect_output_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_media_connect_source_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_rds_performance_insights_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5071 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_rds_service_limits_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_red_shift_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5143 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_route53_resolver_ip_address_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7406 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_route53_resolver_ip_address_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    22799 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_rss_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_sage_maker_endpoint_variant_method.py
+-rw-r--r--   0 root         (0) root         (0)     6202 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_service_limits_from_trusted_advisor_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8304 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_service_region_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5047 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ses_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_vpn_tunnel_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_web_acl_waf_v2_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_account_test_result.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_active_directory_app_secret_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7422 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_active_directory_app_secret_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4370 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_active_directory_sync_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     4378 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_active_directory_users_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5311 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_app_service_environment_multi_role_pool_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)    22975 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_rss_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     7494 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_app_service_environment_multi_role_pool_discover_method.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_authentication_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_automation_account_certificate_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7454 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_automation_account_certificate_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_job_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5300 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_protected_item_backup_job_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7454 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_protected_item_backup_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_protected_item_health_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_billing_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8298 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_billing_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_cost_management_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8669 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_cost_management_dimensions_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7446 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_cost_management_subscriptions_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     8346 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_cost_management_tags_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     9793 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_dimension_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_ea_billing_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8408 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_ea_billing_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)    23855 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_emerging_issue_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     5300 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_express_route_circuit_peering_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_express_route_circuit_peering_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_insights_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_log_analytics_replication_job_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_log_analytics_replication_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_log_analytics_workspaces_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9321 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_log_analytics_workspaces_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_net_app_volumes_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_network_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5180 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_recovery_service_rto_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_recovery_service_rto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_recovery_service_vault_sr_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5288 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_recovery_services_vault_agents_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_redis_cache_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5288 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_replication_disaster_recovery_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_replication_job_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7342 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_replication_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5047 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_resource_health_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5351 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_resource_usage_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7230 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_service_bus_queue.py
+-rw-r--r--   0 root         (0) root         (0)     7230 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_service_bus_topic.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_service_region_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_storage_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_subscription_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5722 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_subscription_id_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     8322 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_synapse_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_virtual_desktop_host_pools_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5215 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5071 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vm_backup_status_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vm_backup_status_log_analytics_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vm_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5144 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vng_connection_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vng_connection_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vwan_vpn_connection_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7294 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vwan_vpn_connection_method.py
+-rw-r--r--   0 root         (0) root         (0)     7342 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_web_app_instance_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_web_job_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_web_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5931 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/basic_authentication.py
+-rw-r--r--   0 root         (0) root         (0)    14502 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/batch_job_execution_item.py
+-rw-r--r--   0 root         (0) root         (0)    17697 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/batch_job_widget.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/batch_job_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     9210 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/batch_script_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_data.py
+-rw-r--r--   0 root         (0) root         (0)    11118 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     8183 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_info.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_item.py
+-rw-r--r--   0 root         (0) root         (0)    14897 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_widget.py
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     8515 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/cell_data.py
+-rw-r--r--   0 root         (0) root         (0)     5810 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/chain.py
+-rw-r--r--   0 root         (0) root         (0)     9659 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/cim_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     8560 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/cim_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    12564 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/cloud_watch_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    75716 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector.py
+-rw-r--r--   0 root         (0) root         (0)     9807 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8185 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    73785 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_base.py
+-rw-r--r--   0 root         (0) root         (0)    17946 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_group.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5510 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    23012 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_sdt.py
+-rw-r--r--   0 root         (0) root         (0)    10151 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_version.py
+-rw-r--r--   0 root         (0) root         (0)     5637 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_version_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/color_threshold.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/column_header.py
+-rw-r--r--   0 root         (0) root         (0)     5761 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/config_source_update_reasons_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     7210 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/conversation_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4480 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/counter.py
+-rw-r--r--   0 root         (0) root         (0)    15312 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_flexible_virtual_data_source_ex.py
+-rw-r--r--   0 root         (0) root         (0)    13816 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_graph.py
+-rw-r--r--   0 root         (0) root         (0)    14681 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)    25497 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_report.py
+-rw-r--r--   0 root         (0) root         (0)     6720 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_virtual_data_point.py
+-rw-r--r--   0 root         (0) root         (0)    16001 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_data.py
+-rw-r--r--   0 root         (0) root         (0)    14261 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_group.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    30522 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_report.py
+-rw-r--r--   0 root         (0) root         (0)    30582 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_point.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_pump_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    26876 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_source_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    16730 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_source_overview_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5729 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_source_update_reasons_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/datasource_overview_graph_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5511 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/datasource_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     6691 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/days_until_alert.py
+-rw-r--r--   0 root         (0) root         (0)     6167 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/debug.py
+-rw-r--r--   0 root         (0) root         (0)    54658 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device.py
+-rw-r--r--   0 root         (0) root         (0)    25341 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_batch_job_sdt.py
+-rw-r--r--   0 root         (0) root         (0)    25754 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_cluster_alert_def_sdt.py
+-rw-r--r--   0 root         (0) root         (0)    28761 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     9096 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_associated.py
+-rw-r--r--   0 root         (0) root         (0)     5544 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_associated_instance.py
+-rw-r--r--   0 root         (0) root         (0)     5849 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_associated_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     6617 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_data.py
+-rw-r--r--   0 root         (0) root         (0)    25047 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance.py
+-rw-r--r--   0 root         (0) root         (0)    45300 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_alert_setting.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_alert_setting_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    20341 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_config.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_config_alert.py
+-rw-r--r--   0 root         (0) root         (0)     5741 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_config_diff.py
+-rw-r--r--   0 root         (0) root         (0)     6814 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_data.py
+-rw-r--r--   0 root         (0) root         (0)     9626 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_group.py
+-rw-r--r--   0 root         (0) root         (0)    29601 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_group_sdt.py
+-rw-r--r--   0 root         (0) root         (0)    26558 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_sdt.py
+-rw-r--r--   0 root         (0) root         (0)    25629 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     5767 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_sdt_history_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5934 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_instance_config_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_instance_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5807 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_instance_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5638 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     6230 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_delta_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    25773 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_event_source_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     5943 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_filter.py
+-rw-r--r--   0 root         (0) root         (0)    47362 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group.py
+-rw-r--r--   0 root         (0) root         (0)    13936 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_alert_threshold_info.py
+-rw-r--r--   0 root         (0) root         (0)    16977 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_data.py
+-rw-r--r--   0 root         (0) root         (0)    11283 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     5232 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_data_source_alert_config.py
+-rw-r--r--   0 root         (0) root         (0)    28724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_data_source_data_point_config.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_datasource_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5687 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_sdt_history_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     7938 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_instance_data.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_instance_data_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     4254 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_instances.py
+-rw-r--r--   0 root         (0) root         (0)    26766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_log_pipe_line_resource_sdt.py
+-rw-r--r--   0 root         (0) root         (0)    10188 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_noc_item.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     4830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_property.py
+-rw-r--r--   0 root         (0) root         (0)     5607 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_sdt_history_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    26278 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_sla_widget.py
+-rw-r--r--   0 root         (0) root         (0)     5963 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_sla_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)    15260 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_status.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dns_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    10033 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dummy_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4535 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_column.py
+-rw-r--r--   0 root         (0) root         (0)    20003 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_table_widget.py
+-rw-r--r--   0 root         (0) root         (0)    13685 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_table_widget_column.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_table_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     6972 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_table_widget_row.py
+-rw-r--r--   0 root         (0) root         (0)     9104 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4725 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_ddr.py
+-rw-r--r--   0 root         (0) root         (0)    23223 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     6349 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_netscan_policy_credential.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_scheduled_event_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    21828 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/echo_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    32001 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/enhanced_script_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     6405 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/entity_property.py
+-rw-r--r--   0 root         (0) root         (0)     5712 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/error_response.py
+-rw-r--r--   0 root         (0) root         (0)    11330 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/escalating_chain.py
+-rw-r--r--   0 root         (0) root         (0)     5616 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/escalation_chain_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     7988 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/esx_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5711 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/esx_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    22518 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/event_source.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/event_source_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     6418 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/exclude_duplicate_ips.py
+-rw-r--r--   0 root         (0) root         (0)    14821 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/flash_widget.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/flow_record_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    11579 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gauge_data_point.py
+-rw-r--r--   0 root         (0) root         (0)    21714 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gauge_widget.py
+-rw-r--r--   0 root         (0) root         (0)    14711 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gauge_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     5997 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_account_test_result.py
+-rw-r--r--   0 root         (0) root         (0)     7286 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_app_engine_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    22887 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_atom_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_backend_service_health_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     4370 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_billing_big_query_source_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9596 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_billing_big_query_source_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_billing_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8256 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_billing_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_compute_service_limits_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_lb_backend_service_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7342 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_pub_sub_snapshot_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_pub_sub_subscription_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_stack_driver_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_vpn_tunnel_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     6088 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/generate_report_request.py
+-rw-r--r--   0 root         (0) root         (0)     5872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/generate_report_result.py
+-rw-r--r--   0 root         (0) root         (0)     4539 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/glob_match_toggle.py
+-rw-r--r--   0 root         (0) root         (0)    19920 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/google_map_widget.py
+-rw-r--r--   0 root         (0) root         (0)     5850 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/google_map_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     5675 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_display.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_line.py
+-rw-r--r--   0 root         (0) root         (0)     7472 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_ops_note_scope.py
+-rw-r--r--   0 root         (0) root         (0)    26433 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_plot.py
+-rw-r--r--   0 root         (0) root         (0)    13921 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_plot_line.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_virtual_data_point.py
+-rw-r--r--   0 root         (0) root         (0)    22567 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/group_net_flow_record.py
+-rw-r--r--   0 root         (0) root         (0)    28465 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_cpu_report.py
+-rw-r--r--   0 root         (0) root         (0)    28395 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_group_inventory_report.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_inventory_metric.py
+-rw-r--r--   0 root         (0) root         (0)    29610 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_inventory_report.py
+-rw-r--r--   0 root         (0) root         (0)    35843 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_metrics_report.py
+-rw-r--r--   0 root         (0) root         (0)    15075 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/html_widget.py
+-rw-r--r--   0 root         (0) root         (0)    12009 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/http_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4624 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ilp.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/inheritance_prop.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/instance_group_alert_threshold_info.py
+-rw-r--r--   0 root         (0) root         (0)    18372 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/integration_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     4228 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/integration_audit_log_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    23132 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/integration_metadata.py
+-rw-r--r--   0 root         (0) root         (0)    32736 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/interf_bandwidth_report.py
+-rw-r--r--   0 root         (0) root         (0)     4591 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/interface_type.py
+-rw-r--r--   0 root         (0) root         (0)     4920 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/interfaces_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/internal_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7915 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ipmi_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4966 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ipmi_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    22795 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ipmi_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    18674 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/item_data.py
+-rw-r--r--   0 root         (0) root         (0)    11413 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/jdbc_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     6838 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/jdbc_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9346 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/jmx_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/jmx_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7588 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/linked_wmi_class.py
+-rw-r--r--   0 root         (0) root         (0)     5199 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/location_data.py
+-rw-r--r--   0 root         (0) root         (0)     7918 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/log_file.py
+-rw-r--r--   0 root         (0) root         (0)    22946 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/log_file_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/macro.py
+-rw-r--r--   0 root         (0) root         (0)    12046 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/map_item_info.py
+-rw-r--r--   0 root         (0) root         (0)     4968 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/match_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     5484 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/memcached_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7132 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/metric.py
+-rw-r--r--   0 root         (0) root         (0)     5105 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/n_map_ddr.py
+-rw-r--r--   0 root         (0) root         (0)    24517 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/n_map_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/name_and_value.py
+-rw-r--r--   0 root         (0) root         (0)     4836 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/nbar_application_names.py
+-rw-r--r--   0 root         (0) root         (0)    13719 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/net_app_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    15795 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/net_app_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    19373 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/net_flow_record.py
+-rw-r--r--   0 root         (0) root         (0)    11502 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_alert_modules_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)    14493 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_application.py
+-rw-r--r--   0 root         (0) root         (0)     8968 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_bandwidth.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_bgp_table.py
+-rw-r--r--   0 root         (0) root         (0)     4602 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_data_base.py
+-rw-r--r--   0 root         (0) root         (0)     5260 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_device_info.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)    13843 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_filters.py
+-rw-r--r--   0 root         (0) root         (0)    17146 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)    15867 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_group_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)    18040 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_group_widget.py
+-rw-r--r--   0 root         (0) root         (0)     6555 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_group_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     7637 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_nbar_application.py
+-rw-r--r--   0 root         (0) root         (0)     6677 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_port.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_qo_s_report_table_row.py
+-rw-r--r--   0 root         (0) root         (0)    28517 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_report.py
+-rw-r--r--   0 root         (0) root         (0)    17526 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_widget.py
+-rw-r--r--   0 root         (0) root         (0)     6455 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)    18904 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netscan.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netscan_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     7754 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/next_upgrade_info.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/noc_item_base.py
+-rw-r--r--   0 root         (0) root         (0)    21151 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/noc_widget.py
+-rw-r--r--   0 root         (0) root         (0)     7184 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/noc_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)    19809 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/normal_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)     6556 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ntlm_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9929 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/onetime_upgrade_info.py
+-rw-r--r--   0 root         (0) root         (0)     8159 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/open_metric_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)    14851 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/open_metric_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     8566 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note.py
+-rw-r--r--   0 root         (0) root         (0)     5525 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_device_group_scope.py
+-rw-r--r--   0 root         (0) root         (0)     6885 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_device_scope.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_group_all_scope.py
+-rw-r--r--   0 root         (0) root         (0)     5448 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     4455 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_scope.py
+-rw-r--r--   0 root         (0) root         (0)     6212 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_tag_base.py
+-rw-r--r--   0 root         (0) root         (0)     5541 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_website_group_scope.py
+-rw-r--r--   0 root         (0) root         (0)     6949 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_website_scope.py
+-rw-r--r--   0 root         (0) root         (0)     8352 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/overview_graph_data_point.py
+-rw-r--r--   0 root         (0) root         (0)    19498 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/overview_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)    13675 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/paa_s_json_path_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5161 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/paa_s_mongo_db_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8834 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pdh_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/perfmon_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/perfmon_counter.py
+-rw-r--r--   0 root         (0) root         (0)     6757 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/period.py
+-rw-r--r--   0 root         (0) root         (0)     5978 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_data.py
+-rw-r--r--   0 root         (0) root         (0)    12398 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_data_point.py
+-rw-r--r--   0 root         (0) root         (0)    13497 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_info.py
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_item.py
+-rw-r--r--   0 root         (0) root         (0)    14703 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_widget.py
+-rw-r--r--   0 root         (0) root         (0)     8818 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)    38842 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ping_check.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ping_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/point_source.py
+-rw-r--r--   0 root         (0) root         (0)     8660 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/port_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     8072 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/privilege.py
+-rw-r--r--   0 root         (0) root         (0)     4846 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/property_match_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5499 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/property_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/push_modules_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    12660 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rabbit_mq_queue_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/raw_data_values.py
+-rw-r--r--   0 root         (0) root         (0)     7027 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/recipient.py
+-rw-r--r--   0 root         (0) root         (0)     6485 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/recipient_group.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/recipient_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    24993 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_base.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_group.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_recipient.py
+-rw-r--r--   0 root         (0) root         (0)    13912 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/resource_data_source_alert_threshold_info.py
+-rw-r--r--   0 root         (0) root         (0)    25610 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/resource_group_sdt.py
+-rw-r--r--   0 root         (0) root         (0)    22708 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/resource_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     5723 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_applies_to_function_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    11433 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_account_test_v3.py
+-rw-r--r--   0 root         (0) root         (0)    23415 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_health_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    24647 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_organizational_health_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    26483 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_rds_performance_insights_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    24119 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_trusted_advisor_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     8741 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_account_test_v3.py
+-rw-r--r--   0 root         (0) root         (0)    23679 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_advisor_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    24295 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_resource_health_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    27223 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_resource_log_analytics_workspaces_source.py
+-rw-r--r--   0 root         (0) root         (0)     9293 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_subscription_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_subscriptions_discover_v3.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_cloud_ok_permissions_v3.py
+-rw-r--r--   0 root         (0) root         (0)     4197 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_dashboard_group_async_clone_response.py
+-rw-r--r--   0 root         (0) root         (0)    19681 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_device_instance_group_alert_config_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7220 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_event_source_filter.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_gcp_account_test_v3.py
+-rw-r--r--   0 root         (0) root         (0)     6780 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_highest_priority_collector_status.py
+-rw-r--r--   0 root         (0) root         (0)     9563 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_n_map_netscan_policy_credential.py
+-rw-r--r--   0 root         (0) root         (0)     5016 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_netscan_ports.py
+-rw-r--r--   0 root         (0) root         (0)    10663 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_saa_s_account_test_v3.py
+-rw-r--r--   0 root         (0) root         (0)    17140 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_saved_map_widget_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7237 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     4545 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_user_customized_data_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5284 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/result_item.py
+-rw-r--r--   0 root         (0) root         (0)    15596 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/role.py
+-rw-r--r--   0 root         (0) root         (0)     5384 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/role_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    25748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/role_report.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/row_data.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_s_slack_health_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    21148 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdt.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_s_webex_license_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     8399 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_s_zoom_plan_usage_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7302 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_s_zoom_status_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7366 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_so365_share_point_site_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     8646 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_account_test_result.py
+-rw-r--r--   0 root         (0) root         (0)     4274 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_airbrake_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7286 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_airbrake_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7310 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_o365_mailbox_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_o365_service_health_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7286 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_o365_skus_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_csv_report_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_health_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_sharepoint_report_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_skus_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     4402 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_teams_calls_qos_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_salesforce_instance_status_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_salesforce_json_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_salesforce_license_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     9687 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_salesforce_soql_query_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7015 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_slack_health_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_status_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7270 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_status_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_webex_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_zoom_json_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     5911 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_zoom_plan_usage_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     8339 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_zoom_room_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    11902 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    11365 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9328 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_eri_discovery_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)    28221 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    29024 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdk_script_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     9803 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdk_script_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdt_history.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdt_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    15260 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/service_alert.py
+-rw-r--r--   0 root         (0) root         (0)     5743 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/site_monitor_check_point_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     8541 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/site_monitor_checkpoint.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sla_metric.py
+-rw-r--r--   0 root         (0) root         (0)    34917 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sla_report.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/snmp_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/snmp_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    22164 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/snmp_trap_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     5103 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/snmpilp.py
+-rw-r--r--   0 root         (0) root         (0)     7569 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/stats_d_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/stats_d_graph_display.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/stats_d_metric_definition.py
+-rw-r--r--   0 root         (0) root         (0)    14422 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/stats_d_widget.py
+-rw-r--r--   0 root         (0) root         (0)     9034 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/synthetics_selenium_auto_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     7029 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/synthetics_selenium_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    21996 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sys_log_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    16103 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget.py
+-rw-r--r--   0 root         (0) root         (0)     9096 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_column.py
+-rw-r--r--   0 root         (0) root         (0)     6660 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     7362 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_forecast_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7578 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_instance_cell.py
+-rw-r--r--   0 root         (0) root         (0)     7872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_row.py
+-rw-r--r--   0 root         (0) root         (0)     6854 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/tcp_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    14390 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/text_widget.py
+-rw-r--r--   0 root         (0) root         (0)     5833 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/tree_node.py
+-rw-r--r--   0 root         (0) root         (0)     5488 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/udp_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     5663 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/unmonitored_device_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    16516 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/unmonitored_devices.py
+-rw-r--r--   0 root         (0) root         (0)     7862 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/update_reason.py
+-rw-r--r--   0 root         (0) root         (0)    23013 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/usage.py
+-rw-r--r--   0 root         (0) root         (0)     9690 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/user_filter.py
+-rw-r--r--   0 root         (0) root         (0)    26447 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/user_report.py
+-rw-r--r--   0 root         (0) root         (0)     4449 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/virtual_data_point.py
+-rw-r--r--   0 root         (0) root         (0)    40343 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/web_check.py
+-rw-r--r--   0 root         (0) root         (0)    25338 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/web_check_step.py
+-rw-r--r--   0 root         (0) root         (0)     9319 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/web_page_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/web_resource.py
+-rw-r--r--   0 root         (0) root         (0)    34431 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_check_point.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_checkpoint_raw_data.py
+-rw-r--r--   0 root         (0) root         (0)    23943 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_checkpoint_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     8469 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_collector_info.py
+-rw-r--r--   0 root         (0) root         (0)    17442 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)    18363 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_group.py
+-rw-r--r--   0 root         (0) root         (0)     5432 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_group_data.py
+-rw-r--r--   0 root         (0) root         (0)     5553 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    23248 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_group_sdt.py
+-rw-r--r--   0 root         (0) root         (0)    21417 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_individuals_status_widget.py
+-rw-r--r--   0 root         (0) root         (0)     5637 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_item_config.py
+-rw-r--r--   0 root         (0) root         (0)     6721 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_location.py
+-rw-r--r--   0 root         (0) root         (0)     7157 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_noc_item.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_overall_status_widget.py
+-rw-r--r--   0 root         (0) root         (0)    32299 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_overview_report.py
+-rw-r--r--   0 root         (0) root         (0)    16966 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_overview_widget.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     5623 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sdt_history_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)    28341 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sla_report.py
+-rw-r--r--   0 root         (0) root         (0)    19006 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sla_widget.py
+-rw-r--r--   0 root         (0) root         (0)     6637 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sla_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)    14722 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget.py
+-rw-r--r--   0 root         (0) root         (0)     5778 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     6565 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget_token.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget_token_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)    22752 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/windows_event_log_event_source.py
+-rw-r--r--   0 root         (0) root         (0)    15135 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/wmi_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)    10653 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/wmi_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     7988 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/xen_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/xen_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    49845 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28149 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     9155 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/configuration.py
+-rw-r--r--   0 root         (0) root         (0)    14056 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    52735 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/logicmonitor_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_access_group.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_access_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_access_log_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ack_collector_down.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_admin.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_admin_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aggregate_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_ack.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_filters.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_forecasting_report.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_list_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_report.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_response.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_rule_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_sla_report.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_threshold_report.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_trends_metric.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_trends_report.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_alert_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_api_perf_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_api_token.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_api_token_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_applies_to_function.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_audit_log_report.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_auto_discovery_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_auto_discovery_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_automatic_upgrade_info.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_account_id.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_account_test_result.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_api_gateway_stage_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_auto_scaling_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_billing_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_billing_report_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_billing_report_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_classic_elb_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_cloud_watch_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_cognito_identity_providers_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ebs_volume_snapshot_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ec2_reserved_instance_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ec2_reserved_instance_coverage_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ec2_reserved_instance_coverage_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ec2_reserved_instance_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ec2_scheduled_events_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ec2_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ecs_service_details_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ecs_service_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_elasti_cache_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_external_id.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_global_network_device_method.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_global_network_link_method.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_global_web_acl_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_lb_target_group_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_media_connect_output_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_media_connect_source_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_rds_performance_insights_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_rds_service_limits_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_red_shift_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_route53_resolver_ip_address_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_route53_resolver_ip_address_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_rss_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_sage_maker_endpoint_variant_method.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_service_limits_from_trusted_advisor_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_service_region_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_ses_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_vpn_tunnel_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_aws_web_acl_waf_v2_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_account_test_result.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ilp.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_active_directory_app_secret_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_active_directory_app_secret_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_active_directory_sync_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_active_directory_users_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_app_service_environment_multi_role_pool_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_app_service_environment_multi_role_pool_discover_method.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_authentication_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_automation_account_certificate_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_automation_account_certificate_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_backup_job_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_backup_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_backup_protected_item_backup_job_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_backup_protected_item_backup_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_backup_protected_item_health_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_billing_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_billing_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_cost_management_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_cost_management_dimensions_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_cost_management_subscriptions_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_cost_management_tags_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_dimension_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_ea_billing_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_ea_billing_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_emerging_issue_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_express_route_circuit_peering_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_express_route_circuit_peering_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_insights_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_log_analytics_replication_job_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_log_analytics_replication_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_log_analytics_workspaces_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_log_analytics_workspaces_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_net_app_volumes_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_network_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_recovery_service_rto_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_recovery_service_rto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_recovery_service_vault_sr_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_recovery_services_vault_agents_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_redis_cache_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_replication_disaster_recovery_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_replication_job_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_replication_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_resource_health_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_resource_usage_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_rss_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_service_bus_queue.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_service_bus_topic.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_service_region_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_storage_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_subscription_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_subscription_id_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_synapse_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_virtual_desktop_host_pools_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_virtual_desktop_session_hosts_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_virtual_desktop_session_hosts_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_vm_backup_status_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_vm_backup_status_log_analytics_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_vm_service_limits_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_vng_connection_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_vng_connection_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_role.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_vwan_vpn_connection_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_vwan_vpn_connection_method.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_web_app_instance_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_web_job_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_azure_web_job_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_basic_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_batch_job_execution_item.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_batch_job_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_batch_job_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_batch_script_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_big_number_data.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_big_number_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_big_number_info.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_big_number_item.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_big_number_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_big_number_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_cell_data.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_chain.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_cim_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_cim_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_cloud_watch_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_base.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_group.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_version.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_collector_version_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_color_threshold.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_column_header.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_config_source_update_reasons_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_conversation_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_counter.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_custom_flexible_virtual_data_source_ex.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_custom_graph.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_custom_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_custom_report.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_custom_virtual_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dashboard_data.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dashboard_group.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dashboard_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dashboard_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dashboard_report.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_data_pump_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_data_source_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_data_source_overview_graph.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_data_source_update_reasons_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_datasource_overview_graph_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_datasource_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_days_until_alert.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_debug.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_batch_job_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_cluster_alert_def_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_associated.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_associated_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_associated_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_data.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_alert_setting.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_alert_setting_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_config.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_config_alert.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_config_diff.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_data.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_group.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_group_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_data_source_sdt_history_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_datasource_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_datasource_instance_config_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_datasource_instance_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_datasource_instance_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_datasource_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_delta_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_event_source_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group_alert_threshold_info.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group_data.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group_data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group_data_source_alert_config.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group_data_source_data_point_config.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group_datasource_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_group_sdt_history_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_instance_data.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_instance_data_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_instances.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_log_pipe_line_resource_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_noc_item.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_property.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_sdt_history_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_sla_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_sla_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_device_status.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dns_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dummy_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dynamic_column.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dynamic_table_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dynamic_table_widget_column.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dynamic_table_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_dynamic_table_widget_row.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ec2_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ec2_ddr.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ec2_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ec2_netscan_policy_credential.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ec2_scheduled_event_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_echo_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_enhanced_script_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_entity_property.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_escalating_chain.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_escalation_chain_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_esx_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_esx_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_event_source_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_exclude_duplicate_ips.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_flash_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_flow_record_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gauge_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gauge_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gauge_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_account_test_result.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_app_engine_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_atom_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_backend_service_health_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_billing_big_query_source_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_billing_big_query_source_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_billing_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_billing_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_compute_service_limits_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_lb_backend_service_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1934 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_pub_sub_snapshot_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_pub_sub_subscription_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_stack_driver_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_gcp_vpn_tunnel_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_generate_report_request.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_generate_report_result.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_glob_match_toggle.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_google_map_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_google_map_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_graph_display.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_graph_line.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_graph_ops_note_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_graph_plot.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_graph_plot_line.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_graph_virtual_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_group_net_flow_record.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_host_cpu_report.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_host_group_inventory_report.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_host_metrics_report.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_host_inventory_metric.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_host_inventory_report.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_html_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_http_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_inheritance_prop.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_instance_group_alert_threshold_info.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_integration_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_integration_audit_log_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_integration_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_interf_bandwidth_report.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_interface_type.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_interfaces_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_internal_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ipmi_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ipmi_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ipmi_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_item_data.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_jdbc_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_jdbc_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_jmx_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_jmx_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_linked_wmi_class.py
+-rw-r--r--   0 root         (0) root         (0)    41751 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_lm_api.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_location_data.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_log_file.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_log_file_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_macro.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_map_item_info.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_match_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_memcached_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_n_map_ddr.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_n_map_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_name_and_value.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_nbar_application_names.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_net_app_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_net_app_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_net_flow_record.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_alert_modules_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_application.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_bandwidth.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_bgp_table.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_data_base.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_device_info.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_filters.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_group_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_group_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_group_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_nbar_application.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_port.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_qo_s_report_table_row.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_report.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netflow_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_netscan_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_next_upgrade_info.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_noc_item_base.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_noc_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_noc_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_normal_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ntlm_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_onetime_upgrade_info.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_open_metric_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_open_metric_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note_device_group_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note_device_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note_group_all_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note_tag_base.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note_website_group_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ops_note_website_scope.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_overview_graph_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_overview_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_paa_s_json_path_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_paa_s_mongo_db_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_pdh_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_perfmon_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_perfmon_counter.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_period.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_pie_chart_data.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_pie_chart_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_pie_chart_info.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_pie_chart_item.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_pie_chart_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_pie_chart_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ping_check.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_ping_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_point_source.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_port_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_property_match_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_property_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_push_modules_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rabbit_mq_queue_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_raw_data_values.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_recipient_group.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_recipient_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_report_base.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_report_group.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_report_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_report_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_report_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_resource_data_source_alert_threshold_info.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_resource_group_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_resource_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_applies_to_function_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_aws_account_test_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_aws_health_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_aws_organizational_health_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_aws_rds_performance_insights_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_aws_trusted_advisor_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_azure_account_test_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_azure_advisor_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_azure_resource_health_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_azure_resource_log_analytics_workspaces_source.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_azure_subscription_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_azure_subscriptions_discover_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_cloud_ok_permissions_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_dashboard_group_async_clone_response.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_device_instance_group_alert_config_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_event_source_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_gcp_account_test_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_highest_priority_collector_status.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_n_map_netscan_policy_credential.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_netscan_ports.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_saa_s_account_test_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_saved_map_widget_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_rest_user_customized_data_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_result_item.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_role_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_role_report.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_row_data.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saa_s_slack_health_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saa_s_webex_license_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saa_s_zoom_plan_usage_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saa_s_zoom_status_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saa_so365_share_point_site_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saas_account_test_result.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saas_airbrake_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saas_airbrake_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saas_o365_mailbox_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saas_o365_service_health_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saas_o365_skus_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_saas_office365_csv_report_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_office365_health_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2054 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_office365_sharepoint_report_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_office365_skus_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_office365_teams_calls_qos_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_salesforce_instance_status_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_salesforce_json_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_salesforce_license_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_salesforce_soql_query_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_slack_health_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_status_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_status_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_webex_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_zoom_json_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_zoom_plan_usage_collector_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_saas_zoom_room_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_script_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_script_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_script_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_script_eri_discovery_attribute_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_script_netscan.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_sdk_script_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_sdk_script_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_sdt_history.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_sdt_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_service_alert.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_site_monitor_check_point_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_site_monitor_checkpoint.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_sla_metric.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_sla_report.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_snmp_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_snmp_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_snmp_trap_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_snmpilp.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_stats_d_graph.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_stats_d_graph_display.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_stats_d_metric_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_stats_d_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_synthetics_selenium_auto_discovery_method_v3.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_synthetics_selenium_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_sys_log_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_table_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_table_widget_column.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_table_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_table_widget_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_table_widget_forecast_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_table_widget_instance_cell.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_table_widget_row.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_tcp_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_text_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_tree_node.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_udp_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_unmonitored_device_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_unmonitored_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_update_reason.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_user_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_user_report.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_virtual_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_web_check.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_web_check_step.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_web_page_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_web_resource.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_check_point.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_checkpoint_raw_data.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_checkpoint_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_collector_info.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_graph_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_group.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_group_data.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_group_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_group_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_individuals_status_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_item_config.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_location.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_noc_item.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_overall_status_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_overview_report.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_overview_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_sdt.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_website_sdt_history_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_sla_report.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_sla_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_website_sla_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_widget.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_widget_data.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_widget_pagination_response.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_widget_token.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-04-17 05:56:12.000000 logicmonitor-sdk-3.0.203/test/test_widget_token_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_windows_event_log_event_source.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_wmi_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_wmi_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_xen_auto_discovery_method.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/test/test_xen_collector_attribute.py
+-rw-r--r--   0 root         (0) root         (0)    74106 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/README.md
+-rw-r--r--   0 root         (0) root         (0)     2765 2024-04-17 05:56:13.000000 logicmonitor-sdk-3.0.203/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 07:11:42.000000 logicmonitor-sdk-3.0.203/setup.cfg
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/api/lm_api.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/api/lm_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,116 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def add_access_group(self, **kwargs):  # noqa: E501
+        """Create a access group  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_access_group(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param AccessGroup body:
+        :return: AccessGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.add_access_group_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.add_access_group_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def add_access_group_with_http_info(self, **kwargs):  # noqa: E501
+        """Create a access group  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.add_access_group_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param AccessGroup body:
+        :return: AccessGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method add_access_group" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['LMv1']  # noqa: E501
+        # if the response type is a file, set _preload_content_value=false.
+        # Because python 3.0+ 'utf-8' codec can't decode the binary string
+        _response_type = 'AccessGroup'
+        _preload_content_value = True
+        if _response_type == 'file':
+          _preload_content_value = False
+
+
+        return self.api_client.call_api(
+            '/setting/accessgroup/add', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=_response_type,
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', _preload_content_value),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def add_admin(self, body, **kwargs):  # noqa: E501
         """add user  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.add_admin(body, async_req=True)
@@ -3455,14 +3557,118 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def delete_access_group(self, id, **kwargs):  # noqa: E501
+        """Delete access group  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_access_group(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int id: (required)
+        :return: object
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.delete_access_group_with_http_info(id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.delete_access_group_with_http_info(id, **kwargs)  # noqa: E501
+            return data
+
+    def delete_access_group_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Delete access group  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.delete_access_group_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int id: (required)
+        :return: object
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_access_group" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `delete_access_group`")  # noqa: E501
+
+        if 'id' in params and not re.search('\d+', params['id'] if type(params['id']) is str else str(params['id'])):  # noqa: E501
+            raise ValueError("Invalid value for parameter `id` when calling `delete_access_group`, must conform to the pattern `/\d+/`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['LMv1']  # noqa: E501
+        # if the response type is a file, set _preload_content_value=false.
+        # Because python 3.0+ 'utf-8' codec can't decode the binary string
+        _response_type = 'object'
+        _preload_content_value = True
+        if _response_type == 'file':
+          _preload_content_value = False
+
+
+        return self.api_client.call_api(
+            '/setting/accessgroup/{id}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=_response_type,
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', _preload_content_value),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def delete_admin_by_id(self, id, **kwargs):  # noqa: E501
         """delete user  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_admin_by_id(id, async_req=True)
@@ -5611,14 +5817,120 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def escalated_alert_by_id(self, id, **kwargs):  # noqa: E501
+        """escalate alert by id  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.escalated_alert_by_id(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str id: (required)
+        :return: object
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.escalated_alert_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.escalated_alert_by_id_with_http_info(id, **kwargs)  # noqa: E501
+            return data
+
+    def escalated_alert_by_id_with_http_info(self, id, **kwargs):  # noqa: E501
+        """escalate alert by id  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.escalated_alert_by_id_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str id: (required)
+        :return: object
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['id']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method escalated_alert_by_id" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `escalated_alert_by_id`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['LMv1']  # noqa: E501
+        # if the response type is a file, set _preload_content_value=false.
+        # Because python 3.0+ 'utf-8' codec can't decode the binary string
+        _response_type = 'object'
+        _preload_content_value = True
+        if _response_type == 'file':
+          _preload_content_value = False
+
+
+        return self.api_client.call_api(
+            '/alert/alerts/{id}/escalate', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=_response_type,
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', _preload_content_value),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def execute_debug_command(self, **kwargs):  # noqa: E501
         """Execute a Collector debug command  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.execute_debug_command(async_req=True)
@@ -6069,14 +6381,232 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_access_group_by_id(self, id, **kwargs):  # noqa: E501
+        """Get access group by id  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_access_group_by_id(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int id: (required)
+        :param str fields:
+        :return: AccessGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_access_group_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_access_group_by_id_with_http_info(id, **kwargs)  # noqa: E501
+            return data
+
+    def get_access_group_by_id_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Get access group by id  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_access_group_by_id_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int id: (required)
+        :param str fields:
+        :return: AccessGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['id', 'fields']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_access_group_by_id" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `get_access_group_by_id`")  # noqa: E501
+
+        if 'id' in params and not re.search('\d+', params['id'] if type(params['id']) is str else str(params['id'])):  # noqa: E501
+            raise ValueError("Invalid value for parameter `id` when calling `get_access_group_by_id`, must conform to the pattern `/\d+/`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
+
+        query_params = []
+        if 'fields' in params:
+            query_params.append(('fields', params['fields']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['LMv1']  # noqa: E501
+        # if the response type is a file, set _preload_content_value=false.
+        # Because python 3.0+ 'utf-8' codec can't decode the binary string
+        _response_type = 'AccessGroup'
+        _preload_content_value = True
+        if _response_type == 'file':
+          _preload_content_value = False
+
+
+        return self.api_client.call_api(
+            '/setting/accessgroup/{id}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=_response_type,
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', _preload_content_value),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_access_group_list(self, **kwargs):  # noqa: E501
+        """Get access group list  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_access_group_list(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str fields:
+        :param int size:
+        :param int offset:
+        :param str filter:
+        :return: AccessGroupPaginationResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_access_group_list_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.get_access_group_list_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def get_access_group_list_with_http_info(self, **kwargs):  # noqa: E501
+        """Get access group list  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_access_group_list_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str fields:
+        :param int size:
+        :param int offset:
+        :param str filter:
+        :return: AccessGroupPaginationResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['fields', 'size', 'offset', 'filter']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_access_group_list" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'fields' in params:
+            query_params.append(('fields', params['fields']))  # noqa: E501
+        if 'size' in params:
+            query_params.append(('size', params['size']))  # noqa: E501
+        if 'offset' in params:
+            query_params.append(('offset', params['offset']))  # noqa: E501
+        if 'filter' in params:
+            query_params.append(('filter', params['filter']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['LMv1']  # noqa: E501
+        # if the response type is a file, set _preload_content_value=false.
+        # Because python 3.0+ 'utf-8' codec can't decode the binary string
+        _response_type = 'AccessGroupPaginationResponse'
+        _preload_content_value = True
+        if _response_type == 'file':
+          _preload_content_value = False
+
+
+        return self.api_client.call_api(
+            '/setting/accessgroup', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=_response_type,
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', _preload_content_value),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_admin_by_id(self, id, **kwargs):  # noqa: E501
         """get user  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_admin_by_id(id, async_req=True)
@@ -11017,14 +11547,142 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_device_datasource_instance_group_by_id(self, device_id, device_ds_id, id, **kwargs):  # noqa: E501
+        """get device datasource instance group   # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_device_datasource_instance_group_by_id(device_id, device_ds_id, id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int device_id: (required)
+        :param int device_ds_id: The device-datasource ID you'd like to add an instance group for (required)
+        :param int id: (required)
+        :param str fields:
+        :return: DeviceDataSourceInstanceGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_device_datasource_instance_group_by_id_with_http_info(device_id, device_ds_id, id, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_device_datasource_instance_group_by_id_with_http_info(device_id, device_ds_id, id, **kwargs)  # noqa: E501
+            return data
+
+    def get_device_datasource_instance_group_by_id_with_http_info(self, device_id, device_ds_id, id, **kwargs):  # noqa: E501
+        """get device datasource instance group   # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_device_datasource_instance_group_by_id_with_http_info(device_id, device_ds_id, id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int device_id: (required)
+        :param int device_ds_id: The device-datasource ID you'd like to add an instance group for (required)
+        :param int id: (required)
+        :param str fields:
+        :return: DeviceDataSourceInstanceGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['device_id', 'device_ds_id', 'id', 'fields']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_device_datasource_instance_group_by_id" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'device_id' is set
+        if ('device_id' not in params or
+                params['device_id'] is None):
+            raise ValueError("Missing the required parameter `device_id` when calling `get_device_datasource_instance_group_by_id`")  # noqa: E501
+        # verify the required parameter 'device_ds_id' is set
+        if ('device_ds_id' not in params or
+                params['device_ds_id'] is None):
+            raise ValueError("Missing the required parameter `device_ds_id` when calling `get_device_datasource_instance_group_by_id`")  # noqa: E501
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `get_device_datasource_instance_group_by_id`")  # noqa: E501
+
+        if 'device_id' in params and not re.search('\d+', params['device_id'] if type(params['device_id']) is str else str(params['device_id'])):  # noqa: E501
+            raise ValueError("Invalid value for parameter `device_id` when calling `get_device_datasource_instance_group_by_id`, must conform to the pattern `/\d+/`")  # noqa: E501
+        if 'device_ds_id' in params and not re.search('\d+', params['device_ds_id'] if type(params['device_ds_id']) is str else str(params['device_ds_id'])):  # noqa: E501
+            raise ValueError("Invalid value for parameter `device_ds_id` when calling `get_device_datasource_instance_group_by_id`, must conform to the pattern `/\d+/`")  # noqa: E501
+        if 'id' in params and not re.search('\d+', params['id'] if type(params['id']) is str else str(params['id'])):  # noqa: E501
+            raise ValueError("Invalid value for parameter `id` when calling `get_device_datasource_instance_group_by_id`, must conform to the pattern `/\d+/`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'device_id' in params:
+            path_params['deviceId'] = params['device_id']  # noqa: E501
+        if 'device_ds_id' in params:
+            path_params['deviceDsId'] = params['device_ds_id']  # noqa: E501
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
+
+        query_params = []
+        if 'fields' in params:
+            query_params.append(('fields', params['fields']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['LMv1']  # noqa: E501
+        # if the response type is a file, set _preload_content_value=false.
+        # Because python 3.0+ 'utf-8' codec can't decode the binary string
+        _response_type = 'DeviceDataSourceInstanceGroup'
+        _preload_content_value = True
+        if _response_type == 'file':
+          _preload_content_value = False
+
+
+        return self.api_client.call_api(
+            '/device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{id}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=_response_type,
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', _preload_content_value),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_device_datasource_instance_group_list(self, device_id, device_ds_id, **kwargs):  # noqa: E501
         """get device datasource instance group list   # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_device_datasource_instance_group_list(device_id, device_ds_id, async_req=True)
@@ -18383,14 +19041,130 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def patch_access_group(self, id, body, **kwargs):  # noqa: E501
+        """Update access group  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.patch_access_group(id, body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int id: (required)
+        :param AccessGroup body: (required)
+        :return: AccessGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.patch_access_group_with_http_info(id, body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.patch_access_group_with_http_info(id, body, **kwargs)  # noqa: E501
+            return data
+
+    def patch_access_group_with_http_info(self, id, body, **kwargs):  # noqa: E501
+        """Update access group  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.patch_access_group_with_http_info(id, body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int id: (required)
+        :param AccessGroup body: (required)
+        :return: AccessGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['id', 'body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method patch_access_group" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `patch_access_group`")  # noqa: E501
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `patch_access_group`")  # noqa: E501
+
+        if 'id' in params and not re.search('\d+', params['id'] if type(params['id']) is str else str(params['id'])):  # noqa: E501
+            raise ValueError("Invalid value for parameter `id` when calling `patch_access_group`, must conform to the pattern `/\d+/`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['LMv1']  # noqa: E501
+        # if the response type is a file, set _preload_content_value=false.
+        # Because python 3.0+ 'utf-8' codec can't decode the binary string
+        _response_type = 'AccessGroup'
+        _preload_content_value = True
+        if _response_type == 'file':
+          _preload_content_value = False
+
+
+        return self.api_client.call_api(
+            '/setting/accessgroup/{id}', 'PATCH',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=_response_type,
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', _preload_content_value),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def patch_admin_by_id(self, id, body, **kwargs):  # noqa: E501
         """update user  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_admin_by_id(id, body, async_req=True)
@@ -20761,156 +21535,14 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def patch_instances_alert_threshold(self, device_id, device_ds_id, dsig_id, dp_id, **kwargs):  # noqa: E501
-        """update instances alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
-
-          # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.patch_instances_alert_threshold(device_id, device_ds_id, dsig_id, dp_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param int device_id: (required)
-        :param int device_ds_id: The device-datasource ID you'd like to add an instance group for (required)
-        :param int dsig_id: (required)
-        :param int dp_id: (required)
-        :param RestDeviceInstanceGroupAlertConfigV3 body:
-        :return: DeviceDataSourceInstanceGroup
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.patch_instances_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, **kwargs)  # noqa: E501
-        else:
-            (data) = self.patch_instances_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, **kwargs)  # noqa: E501
-            return data
-
-    def patch_instances_alert_threshold_with_http_info(self, device_id, device_ds_id, dsig_id, dp_id, **kwargs):  # noqa: E501
-        """update instances alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
-
-          # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.patch_instances_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param int device_id: (required)
-        :param int device_ds_id: The device-datasource ID you'd like to add an instance group for (required)
-        :param int dsig_id: (required)
-        :param int dp_id: (required)
-        :param RestDeviceInstanceGroupAlertConfigV3 body:
-        :return: DeviceDataSourceInstanceGroup
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['device_id', 'device_ds_id', 'dsig_id', 'dp_id', 'body']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method patch_instances_alert_threshold" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'device_id' is set
-        if ('device_id' not in params or
-                params['device_id'] is None):
-            raise ValueError("Missing the required parameter `device_id` when calling `patch_instances_alert_threshold`")  # noqa: E501
-        # verify the required parameter 'device_ds_id' is set
-        if ('device_ds_id' not in params or
-                params['device_ds_id'] is None):
-            raise ValueError("Missing the required parameter `device_ds_id` when calling `patch_instances_alert_threshold`")  # noqa: E501
-        # verify the required parameter 'dsig_id' is set
-        if ('dsig_id' not in params or
-                params['dsig_id'] is None):
-            raise ValueError("Missing the required parameter `dsig_id` when calling `patch_instances_alert_threshold`")  # noqa: E501
-        # verify the required parameter 'dp_id' is set
-        if ('dp_id' not in params or
-                params['dp_id'] is None):
-            raise ValueError("Missing the required parameter `dp_id` when calling `patch_instances_alert_threshold`")  # noqa: E501
-
-        if 'device_id' in params and not re.search('\d+', params['device_id'] if type(params['device_id']) is str else str(params['device_id'])):  # noqa: E501
-            raise ValueError("Invalid value for parameter `device_id` when calling `patch_instances_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
-        if 'device_ds_id' in params and not re.search('\d+', params['device_ds_id'] if type(params['device_ds_id']) is str else str(params['device_ds_id'])):  # noqa: E501
-            raise ValueError("Invalid value for parameter `device_ds_id` when calling `patch_instances_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
-        if 'dsig_id' in params and not re.search('\d+', params['dsig_id'] if type(params['dsig_id']) is str else str(params['dsig_id'])):  # noqa: E501
-            raise ValueError("Invalid value for parameter `dsig_id` when calling `patch_instances_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
-        if 'dp_id' in params and not re.search('\d+', params['dp_id'] if type(params['dp_id']) is str else str(params['dp_id'])):  # noqa: E501
-            raise ValueError("Invalid value for parameter `dp_id` when calling `patch_instances_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
-        collection_formats = {}
-
-        path_params = {}
-        if 'device_id' in params:
-            path_params['deviceId'] = params['device_id']  # noqa: E501
-        if 'device_ds_id' in params:
-            path_params['deviceDsId'] = params['device_ds_id']  # noqa: E501
-        if 'dsig_id' in params:
-            path_params['dsigId'] = params['dsig_id']  # noqa: E501
-        if 'dp_id' in params:
-            path_params['dpId'] = params['dp_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'body' in params:
-            body_params = params['body']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['LMv1']  # noqa: E501
-        # if the response type is a file, set _preload_content_value=false.
-        # Because python 3.0+ 'utf-8' codec can't decode the binary string
-        _response_type = 'DeviceDataSourceInstanceGroup'
-        _preload_content_value = True
-        if _response_type == 'file':
-          _preload_content_value = False
-
-
-        return self.api_client.call_api(
-            '/device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{dsigId}/datapoints/{dpId}/alertconfig', 'PATCH',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type=_response_type,
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', _preload_content_value),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def patch_recipient_group_by_id(self, id, body, **kwargs):  # noqa: E501
         """update recipient group  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.patch_recipient_group_by_id(id, body, async_req=True)
@@ -22381,14 +23013,130 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def update_access_group(self, id, body, **kwargs):  # noqa: E501
+        """Update access group  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_access_group(id, body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int id: (required)
+        :param AccessGroup body: (required)
+        :return: AccessGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.update_access_group_with_http_info(id, body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_access_group_with_http_info(id, body, **kwargs)  # noqa: E501
+            return data
+
+    def update_access_group_with_http_info(self, id, body, **kwargs):  # noqa: E501
+        """Update access group  # noqa: E501
+
+          # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.update_access_group_with_http_info(id, body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int id: (required)
+        :param AccessGroup body: (required)
+        :return: AccessGroup
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['id', 'body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_access_group" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in params or
+                params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `update_access_group`")  # noqa: E501
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `update_access_group`")  # noqa: E501
+
+        if 'id' in params and not re.search('\d+', params['id'] if type(params['id']) is str else str(params['id'])):  # noqa: E501
+            raise ValueError("Invalid value for parameter `id` when calling `update_access_group`, must conform to the pattern `/\d+/`")  # noqa: E501
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['LMv1']  # noqa: E501
+        # if the response type is a file, set _preload_content_value=false.
+        # Because python 3.0+ 'utf-8' codec can't decode the binary string
+        _response_type = 'AccessGroup'
+        _preload_content_value = True
+        if _response_type == 'file':
+          _preload_content_value = False
+
+
+        return self.api_client.call_api(
+            '/setting/accessgroup/{id}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=_response_type,
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', _preload_content_value),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def update_admin_by_id(self, id, body, **kwargs):  # noqa: E501
         """update user  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_admin_by_id(id, body, async_req=True)
@@ -24759,56 +25507,56 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', _preload_content_value),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update_instances_alert_threshold(self, device_id, device_ds_id, dsig_id, dp_id, **kwargs):  # noqa: E501
-        """update instances alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
+    def update_instance_group_alert_threshold(self, device_id, device_ds_id, dsig_id, dp_id, **kwargs):  # noqa: E501
+        """update instance group alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_instances_alert_threshold(device_id, device_ds_id, dsig_id, dp_id, async_req=True)
+        >>> thread = api.update_instance_group_alert_threshold(device_id, device_ds_id, dsig_id, dp_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int device_id: (required)
         :param int device_ds_id: The device-datasource ID you'd like to add an instance group for (required)
         :param int dsig_id: (required)
         :param int dp_id: (required)
         :param RestDeviceInstanceGroupAlertConfigV3 body:
-        :return: DeviceDataSourceInstanceGroup
+        :return: object
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.update_instances_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, **kwargs)  # noqa: E501
+            return self.update_instance_group_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, **kwargs)  # noqa: E501
         else:
-            (data) = self.update_instances_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, **kwargs)  # noqa: E501
+            (data) = self.update_instance_group_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, **kwargs)  # noqa: E501
             return data
 
-    def update_instances_alert_threshold_with_http_info(self, device_id, device_ds_id, dsig_id, dp_id, **kwargs):  # noqa: E501
-        """update instances alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
+    def update_instance_group_alert_threshold_with_http_info(self, device_id, device_ds_id, dsig_id, dp_id, **kwargs):  # noqa: E501
+        """update instance group alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
 
           # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.update_instances_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, async_req=True)
+        >>> thread = api.update_instance_group_alert_threshold_with_http_info(device_id, device_ds_id, dsig_id, dp_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int device_id: (required)
         :param int device_ds_id: The device-datasource ID you'd like to add an instance group for (required)
         :param int dsig_id: (required)
         :param int dp_id: (required)
         :param RestDeviceInstanceGroupAlertConfigV3 body:
-        :return: DeviceDataSourceInstanceGroup
+        :return: object
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['device_id', 'device_ds_id', 'dsig_id', 'dp_id', 'body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -24816,43 +25564,43 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_instances_alert_threshold" % key
+                    " to method update_instance_group_alert_threshold" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'device_id' is set
         if ('device_id' not in params or
                 params['device_id'] is None):
-            raise ValueError("Missing the required parameter `device_id` when calling `update_instances_alert_threshold`")  # noqa: E501
+            raise ValueError("Missing the required parameter `device_id` when calling `update_instance_group_alert_threshold`")  # noqa: E501
         # verify the required parameter 'device_ds_id' is set
         if ('device_ds_id' not in params or
                 params['device_ds_id'] is None):
-            raise ValueError("Missing the required parameter `device_ds_id` when calling `update_instances_alert_threshold`")  # noqa: E501
+            raise ValueError("Missing the required parameter `device_ds_id` when calling `update_instance_group_alert_threshold`")  # noqa: E501
         # verify the required parameter 'dsig_id' is set
         if ('dsig_id' not in params or
                 params['dsig_id'] is None):
-            raise ValueError("Missing the required parameter `dsig_id` when calling `update_instances_alert_threshold`")  # noqa: E501
+            raise ValueError("Missing the required parameter `dsig_id` when calling `update_instance_group_alert_threshold`")  # noqa: E501
         # verify the required parameter 'dp_id' is set
         if ('dp_id' not in params or
                 params['dp_id'] is None):
-            raise ValueError("Missing the required parameter `dp_id` when calling `update_instances_alert_threshold`")  # noqa: E501
+            raise ValueError("Missing the required parameter `dp_id` when calling `update_instance_group_alert_threshold`")  # noqa: E501
 
         if 'device_id' in params and not re.search('\d+', params['device_id'] if type(params['device_id']) is str else str(params['device_id'])):  # noqa: E501
-            raise ValueError("Invalid value for parameter `device_id` when calling `update_instances_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
+            raise ValueError("Invalid value for parameter `device_id` when calling `update_instance_group_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
         if 'device_ds_id' in params and not re.search('\d+', params['device_ds_id'] if type(params['device_ds_id']) is str else str(params['device_ds_id'])):  # noqa: E501
-            raise ValueError("Invalid value for parameter `device_ds_id` when calling `update_instances_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
+            raise ValueError("Invalid value for parameter `device_ds_id` when calling `update_instance_group_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
         if 'dsig_id' in params and not re.search('\d+', params['dsig_id'] if type(params['dsig_id']) is str else str(params['dsig_id'])):  # noqa: E501
-            raise ValueError("Invalid value for parameter `dsig_id` when calling `update_instances_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
+            raise ValueError("Invalid value for parameter `dsig_id` when calling `update_instance_group_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
         if 'dp_id' in params and not re.search('\d+', params['dp_id'] if type(params['dp_id']) is str else str(params['dp_id'])):  # noqa: E501
-            raise ValueError("Invalid value for parameter `dp_id` when calling `update_instances_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
+            raise ValueError("Invalid value for parameter `dp_id` when calling `update_instance_group_alert_threshold`, must conform to the pattern `/\d+/`")  # noqa: E501
         collection_formats = {}
 
         path_params = {}
         if 'device_id' in params:
             path_params['deviceId'] = params['device_id']  # noqa: E501
         if 'device_ds_id' in params:
             path_params['deviceDsId'] = params['device_ds_id']  # noqa: E501
@@ -24879,15 +25627,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['LMv1']  # noqa: E501
         # if the response type is a file, set _preload_content_value=false.
         # Because python 3.0+ 'utf-8' codec can't decode the binary string
-        _response_type = 'DeviceDataSourceInstanceGroup'
+        _response_type = 'object'
         _preload_content_value = True
         if _response_type == 'file':
           _preload_content_value = False
 
 
         return self.api_client.call_api(
             '/device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{dsigId}/datapoints/{dpId}/alertconfig', 'PUT',
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/__init__.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from logicmonitor_sdk.models.api_token import APIToken
+from logicmonitor_sdk.models.access_group import AccessGroup
+from logicmonitor_sdk.models.access_group_pagination_response import AccessGroupPaginationResponse
 from logicmonitor_sdk.models.access_log_pagination_response import AccessLogPaginationResponse
 from logicmonitor_sdk.models.ack_collector_down import AckCollectorDown
 from logicmonitor_sdk.models.admin import Admin
 from logicmonitor_sdk.models.admin_pagination_response import AdminPaginationResponse
 from logicmonitor_sdk.models.alert import Alert
 from logicmonitor_sdk.models.alert_ack import AlertAck
 from logicmonitor_sdk.models.alert_filters import AlertFilters
@@ -190,14 +192,15 @@
 from logicmonitor_sdk.models.recipient_group import RecipientGroup
 from logicmonitor_sdk.models.recipient_group_pagination_response import RecipientGroupPaginationResponse
 from logicmonitor_sdk.models.report_base import ReportBase
 from logicmonitor_sdk.models.report_group import ReportGroup
 from logicmonitor_sdk.models.report_group_pagination_response import ReportGroupPaginationResponse
 from logicmonitor_sdk.models.report_pagination_response import ReportPaginationResponse
 from logicmonitor_sdk.models.report_recipient import ReportRecipient
+from logicmonitor_sdk.models.resource_data_source_alert_threshold_info import ResourceDataSourceAlertThresholdInfo
 from logicmonitor_sdk.models.rest_applies_to_function_pagination_response import RestAppliesToFunctionPaginationResponse
 from logicmonitor_sdk.models.rest_aws_account_test_v3 import RestAwsAccountTestV3
 from logicmonitor_sdk.models.rest_azure_account_test_v3 import RestAzureAccountTestV3
 from logicmonitor_sdk.models.rest_azure_subscription_v3 import RestAzureSubscriptionV3
 from logicmonitor_sdk.models.rest_azure_subscriptions_discover_v3 import RestAzureSubscriptionsDiscoverV3
 from logicmonitor_sdk.models.rest_cloud_ok_permissions_v3 import RestCloudOkPermissionsV3
 from logicmonitor_sdk.models.rest_dashboard_group_async_clone_response import RestDashboardGroupAsyncCloneResponse
@@ -279,14 +282,16 @@
 from logicmonitor_sdk.models.aws_ec2_reserved_instance_discovery_method import AwsEC2ReservedInstanceDiscoveryMethod
 from logicmonitor_sdk.models.aws_ec2_scheduled_events_collector_attribute import AwsEC2ScheduledEventsCollectorAttribute
 from logicmonitor_sdk.models.aws_ebs_volume_snapshot_collector_attribute_v3 import AwsEbsVolumeSnapshotCollectorAttributeV3
 from logicmonitor_sdk.models.aws_ec2_service_limits_collector_attribute import AwsEc2ServiceLimitsCollectorAttribute
 from logicmonitor_sdk.models.aws_ecs_service_details_collector_attribute import AwsEcsServiceDetailsCollectorAttribute
 from logicmonitor_sdk.models.aws_ecs_service_discovery_method import AwsEcsServiceDiscoveryMethod
 from logicmonitor_sdk.models.aws_elasti_cache_discovery_method import AwsElastiCacheDiscoveryMethod
+from logicmonitor_sdk.models.aws_global_network_device_method import AwsGlobalNetworkDeviceMethod
+from logicmonitor_sdk.models.aws_global_network_link_method import AwsGlobalNetworkLinkMethod
 from logicmonitor_sdk.models.aws_global_web_acl_discovery_method_v3 import AwsGlobalWebACLDiscoveryMethodV3
 from logicmonitor_sdk.models.aws_lb_target_group_discovery_method import AwsLBTargetGroupDiscoveryMethod
 from logicmonitor_sdk.models.aws_media_connect_output_discovery_method import AwsMediaConnectOutputDiscoveryMethod
 from logicmonitor_sdk.models.aws_media_connect_source_discovery_method import AwsMediaConnectSourceDiscoveryMethod
 from logicmonitor_sdk.models.aws_rds_performance_insights_collector_attribute import AwsRdsPerformanceInsightsCollectorAttribute
 from logicmonitor_sdk.models.aws_rds_service_limits_collector_attribute_v3 import AwsRdsServiceLimitsCollectorAttributeV3
 from logicmonitor_sdk.models.aws_red_shift_discovery_method import AwsRedShiftDiscoveryMethod
@@ -339,14 +344,16 @@
 from logicmonitor_sdk.models.azure_redis_cache_discovery_method import AzureRedisCacheDiscoveryMethod
 from logicmonitor_sdk.models.azure_replication_disaster_recovery_collector_attribute import AzureReplicationDisasterRecoveryCollectorAttribute
 from logicmonitor_sdk.models.azure_replication_job_collector_attribute_v3 import AzureReplicationJobCollectorAttributeV3
 from logicmonitor_sdk.models.azure_replication_job_discovery_method import AzureReplicationJobDiscoveryMethod
 from logicmonitor_sdk.models.azure_resource_health_collector_attribute import AzureResourceHealthCollectorAttribute
 from logicmonitor_sdk.models.azure_resource_usage_collector_attribute import AzureResourceUsageCollectorAttribute
 from logicmonitor_sdk.models.azure_rss_event_source import AzureRssEventSource
+from logicmonitor_sdk.models.azure_service_bus_queue import AzureServiceBusQueue
+from logicmonitor_sdk.models.azure_service_bus_topic import AzureServiceBusTopic
 from logicmonitor_sdk.models.azure_service_region_discovery_method import AzureServiceRegionDiscoveryMethod
 from logicmonitor_sdk.models.azure_storage_service_limits_collector_attribute import AzureStorageServiceLimitsCollectorAttribute
 from logicmonitor_sdk.models.azure_subscription_discovery_method import AzureSubscriptionDiscoveryMethod
 from logicmonitor_sdk.models.azure_synapse_discovery_method_v3 import AzureSynapseDiscoveryMethodV3
 from logicmonitor_sdk.models.azure_vm_backup_status_collector_attribute_v3 import AzureVMBackupStatusCollectorAttributeV3
 from logicmonitor_sdk.models.azure_vm_backup_status_log_analytics_collector_attribute import AzureVMBackupStatusLogAnalyticsCollectorAttribute
 from logicmonitor_sdk.models.azure_vm_service_limits_collector_attribute import AzureVMServiceLimitsCollectorAttribute
@@ -474,14 +481,15 @@
 from logicmonitor_sdk.models.ping_collector_attribute import PingCollectorAttribute
 from logicmonitor_sdk.models.port_auto_discovery_method import PortAutoDiscoveryMethod
 from logicmonitor_sdk.models.push_modules_collector_attribute import PushModulesCollectorAttribute
 from logicmonitor_sdk.models.rabbit_mq_queue_auto_discovery_method import RabbitMQQueueAutoDiscoveryMethod
 from logicmonitor_sdk.models.resource_group_sdt import ResourceGroupSDT
 from logicmonitor_sdk.models.resource_sdt import ResourceSDT
 from logicmonitor_sdk.models.rest_aws_health_event_source import RestAwsHealthEventSource
+from logicmonitor_sdk.models.rest_aws_organizational_health_event_source import RestAwsOrganizationalHealthEventSource
 from logicmonitor_sdk.models.rest_aws_rds_performance_insights_event_source import RestAwsRdsPerformanceInsightsEventSource
 from logicmonitor_sdk.models.rest_aws_trusted_advisor_event_source import RestAwsTrustedAdvisorEventSource
 from logicmonitor_sdk.models.rest_azure_advisor_event_source import RestAzureAdvisorEventSource
 from logicmonitor_sdk.models.rest_azure_resource_health_event_source import RestAzureResourceHealthEventSource
 from logicmonitor_sdk.models.rest_azure_resource_log_analytics_workspaces_source import RestAzureResourceLogAnalyticsWorkspacesSource
 from logicmonitor_sdk.models.rest_saved_map_widget_v3 import RestSavedMapWidgetV3
 from logicmonitor_sdk.models.role_report import RoleReport
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/access_log_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/access_log_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ack_collector_down.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ack_collector_down.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/admin.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,24 +39,26 @@
         'view_permission': 'object',
         'timezone': 'str',
         'roles': 'list[Role]',
         'last_login_on': 'int',
         'last_action_on_local': 'str',
         'sms_email_format': 'str',
         'apionly': 'bool',
+        'last_auth_ip': 'str',
         'api_tokens': 'list[APIToken]',
         'admin_group_ids': 'list[int]',
         'password': 'str',
         'last_action': 'str',
         'training_email': 'str',
         'last_action_on': 'int',
         'id': 'int',
         'email': 'str',
         'contact_method': 'str',
         'accept_eula_on': 'int',
+        'immediate_force_logout': 'bool',
         'user_permission': 'str',
         'sms_email': 'str',
         'two_fa_enabled': 'bool',
         'first_name': 'str',
         'phone': 'str',
         'created_by': 'str',
         'force_password_change': 'bool',
@@ -72,59 +74,63 @@
         'view_permission': 'viewPermission',
         'timezone': 'timezone',
         'roles': 'roles',
         'last_login_on': 'lastLoginOn',
         'last_action_on_local': 'lastActionOnLocal',
         'sms_email_format': 'smsEmailFormat',
         'apionly': 'apionly',
+        'last_auth_ip': 'lastAuthIp',
         'api_tokens': 'apiTokens',
         'admin_group_ids': 'adminGroupIds',
         'password': 'password',
         'last_action': 'lastAction',
         'training_email': 'trainingEmail',
         'last_action_on': 'lastActionOn',
         'id': 'id',
         'email': 'email',
         'contact_method': 'contactMethod',
         'accept_eula_on': 'acceptEULAOn',
+        'immediate_force_logout': 'immediateForceLogout',
         'user_permission': 'userPermission',
         'sms_email': 'smsEmail',
         'two_fa_enabled': 'twoFAEnabled',
         'first_name': 'firstName',
         'phone': 'phone',
         'created_by': 'createdBy',
         'force_password_change': 'forcePasswordChange',
         'tenant_id': 'tenantId',
         'accept_eula': 'acceptEULA',
         'username': 'username',
         'status': 'status'
     }
 
-    def __init__(self, last_name=None, note=None, view_permission=None, timezone=None, roles=None, last_login_on=None, last_action_on_local=None, sms_email_format=None, apionly=None, api_tokens=None, admin_group_ids=None, password=None, last_action=None, training_email=None, last_action_on=None, id=None, email=None, contact_method=None, accept_eula_on=None, user_permission=None, sms_email=None, two_fa_enabled=None, first_name=None, phone=None, created_by=None, force_password_change=None, tenant_id=None, accept_eula=None, username=None, status=None):  # noqa: E501
+    def __init__(self, last_name=None, note=None, view_permission=None, timezone=None, roles=None, last_login_on=None, last_action_on_local=None, sms_email_format=None, apionly=None, last_auth_ip=None, api_tokens=None, admin_group_ids=None, password=None, last_action=None, training_email=None, last_action_on=None, id=None, email=None, contact_method=None, accept_eula_on=None, immediate_force_logout=None, user_permission=None, sms_email=None, two_fa_enabled=None, first_name=None, phone=None, created_by=None, force_password_change=None, tenant_id=None, accept_eula=None, username=None, status=None):  # noqa: E501
         """Admin - a model defined in Swagger"""  # noqa: E501
 
         self._last_name = None
         self._note = None
         self._view_permission = None
         self._timezone = None
         self._roles = None
         self._last_login_on = None
         self._last_action_on_local = None
         self._sms_email_format = None
         self._apionly = None
+        self._last_auth_ip = None
         self._api_tokens = None
         self._admin_group_ids = None
         self._password = None
         self._last_action = None
         self._training_email = None
         self._last_action_on = None
         self._id = None
         self._email = None
         self._contact_method = None
         self._accept_eula_on = None
+        self._immediate_force_logout = None
         self._user_permission = None
         self._sms_email = None
         self._two_fa_enabled = None
         self._first_name = None
         self._phone = None
         self._created_by = None
         self._force_password_change = None
@@ -147,14 +153,16 @@
             self.last_login_on = last_login_on
         if last_action_on_local is not None:
             self.last_action_on_local = last_action_on_local
         if sms_email_format is not None:
             self.sms_email_format = sms_email_format
         if apionly is not None:
             self.apionly = apionly
+        if last_auth_ip is not None:
+            self.last_auth_ip = last_auth_ip
         if api_tokens is not None:
             self.api_tokens = api_tokens
         if admin_group_ids is not None:
             self.admin_group_ids = admin_group_ids
         self.password = password
         if last_action is not None:
             self.last_action = last_action
@@ -165,14 +173,16 @@
         if id is not None:
             self.id = id
         self.email = email
         if contact_method is not None:
             self.contact_method = contact_method
         if accept_eula_on is not None:
             self.accept_eula_on = accept_eula_on
+        if immediate_force_logout is not None:
+            self.immediate_force_logout = immediate_force_logout
         if user_permission is not None:
             self.user_permission = user_permission
         if sms_email is not None:
             self.sms_email = sms_email
         if two_fa_enabled is not None:
             self.two_fa_enabled = two_fa_enabled
         if first_name is not None:
@@ -397,14 +407,37 @@
         :param apionly: The apionly of this Admin.  # noqa: E501
         :type: bool
         """
 
         self._apionly = apionly
 
     @property
+    def last_auth_ip(self):
+        """Gets the last_auth_ip of this Admin.  # noqa: E501
+
+        The Last User IP  # noqa: E501
+
+        :return: The last_auth_ip of this Admin.  # noqa: E501
+        :rtype: str
+        """
+        return self._last_auth_ip
+
+    @last_auth_ip.setter
+    def last_auth_ip(self, last_auth_ip):
+        """Sets the last_auth_ip of this Admin.
+
+        The Last User IP  # noqa: E501
+
+        :param last_auth_ip: The last_auth_ip of this Admin.  # noqa: E501
+        :type: str
+        """
+
+        self._last_auth_ip = last_auth_ip
+
+    @property
     def api_tokens(self):
         """Gets the api_tokens of this Admin.  # noqa: E501
 
         Any API Tokens associated with the user  # noqa: E501
 
         :return: The api_tokens of this Admin.  # noqa: E501
         :rtype: list[APIToken]
@@ -631,14 +664,37 @@
         :param accept_eula_on: The accept_eula_on of this Admin.  # noqa: E501
         :type: int
         """
 
         self._accept_eula_on = accept_eula_on
 
     @property
+    def immediate_force_logout(self):
+        """Gets the immediate_force_logout of this Admin.  # noqa: E501
+
+        Specifies whether the user need to be logged off, if Force Password Change is enabled. The values can be true|false  # noqa: E501
+
+        :return: The immediate_force_logout of this Admin.  # noqa: E501
+        :rtype: bool
+        """
+        return self._immediate_force_logout
+
+    @immediate_force_logout.setter
+    def immediate_force_logout(self, immediate_force_logout):
+        """Sets the immediate_force_logout of this Admin.
+
+        Specifies whether the user need to be logged off, if Force Password Change is enabled. The values can be true|false  # noqa: E501
+
+        :param immediate_force_logout: The immediate_force_logout of this Admin.  # noqa: E501
+        :type: bool
+        """
+
+        self._immediate_force_logout = immediate_force_logout
+
+    @property
     def user_permission(self):
         """Gets the user_permission of this Admin.  # noqa: E501
 
         The permission of current user with the admin. values can be write|read|none  # noqa: E501
 
         :return: The user_permission of this Admin.  # noqa: E501
         :rtype: str
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/admin_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/admin_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aggregate_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aggregate_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         'type': 'str',
         'start_epoch': 'int',
         'enable_anomaly_alert_generation': 'str',
         'internal_id': 'str',
         'ack_comment': 'str',
         'monitor_object_name': 'str',
         'data_point_name': 'str',
+        'alert_group_entity_value': 'str',
         'instance_id': 'int',
         'data_point_id': 'int',
         'suppress_desc': 'str',
         'next_recipient': 'int',
         'suppressor': 'str',
         'id': 'str',
         'detail_message': 'object',
@@ -91,14 +92,15 @@
         'type': 'type',
         'start_epoch': 'startEpoch',
         'enable_anomaly_alert_generation': 'enableAnomalyAlertGeneration',
         'internal_id': 'internalId',
         'ack_comment': 'ackComment',
         'monitor_object_name': 'monitorObjectName',
         'data_point_name': 'dataPointName',
+        'alert_group_entity_value': 'alertGroupEntityValue',
         'instance_id': 'instanceId',
         'data_point_id': 'dataPointId',
         'suppress_desc': 'suppressDesc',
         'next_recipient': 'nextRecipient',
         'suppressor': 'suppressor',
         'id': 'id',
         'detail_message': 'detailMessage',
@@ -126,15 +128,15 @@
         'chain_id': 'chainId',
         'resource_template_id': 'resourceTemplateId',
         'cleared': 'cleared',
         'ad_alert_desc': 'adAlertDesc',
         'resource_template_name': 'resourceTemplateName'
     }
 
-    def __init__(self, resource_id=None, anomaly=None, instance_name=None, monitor_object_id=None, end_epoch=None, rule=None, threshold=None, type=None, start_epoch=None, enable_anomaly_alert_generation=None, internal_id=None, ack_comment=None, monitor_object_name=None, data_point_name=None, instance_id=None, data_point_id=None, suppress_desc=None, next_recipient=None, suppressor=None, id=None, detail_message=None, rule_id=None, tenant=None, alert_value=None, ad_alert=None, acked_by=None, severity=None, sdted=None, acked_epoch=None, chain=None, sdt=None, sub_chain_id=None, enable_anomaly_alert_suppression=None, received_list=None, monitor_object_type=None, acked=None, resource_template_type=None, clear_value=None, instance_description=None, dependency_routing_state=None, monitor_object_groups=None, dependency_role=None, chain_id=None, resource_template_id=None, cleared=None, ad_alert_desc=None, resource_template_name=None):  # noqa: E501
+    def __init__(self, resource_id=None, anomaly=None, instance_name=None, monitor_object_id=None, end_epoch=None, rule=None, threshold=None, type=None, start_epoch=None, enable_anomaly_alert_generation=None, internal_id=None, ack_comment=None, monitor_object_name=None, data_point_name=None, alert_group_entity_value=None, instance_id=None, data_point_id=None, suppress_desc=None, next_recipient=None, suppressor=None, id=None, detail_message=None, rule_id=None, tenant=None, alert_value=None, ad_alert=None, acked_by=None, severity=None, sdted=None, acked_epoch=None, chain=None, sdt=None, sub_chain_id=None, enable_anomaly_alert_suppression=None, received_list=None, monitor_object_type=None, acked=None, resource_template_type=None, clear_value=None, instance_description=None, dependency_routing_state=None, monitor_object_groups=None, dependency_role=None, chain_id=None, resource_template_id=None, cleared=None, ad_alert_desc=None, resource_template_name=None):  # noqa: E501
         """Alert - a model defined in Swagger"""  # noqa: E501
 
         self._resource_id = None
         self._anomaly = None
         self._instance_name = None
         self._monitor_object_id = None
         self._end_epoch = None
@@ -143,14 +145,15 @@
         self._type = None
         self._start_epoch = None
         self._enable_anomaly_alert_generation = None
         self._internal_id = None
         self._ack_comment = None
         self._monitor_object_name = None
         self._data_point_name = None
+        self._alert_group_entity_value = None
         self._instance_id = None
         self._data_point_id = None
         self._suppress_desc = None
         self._next_recipient = None
         self._suppressor = None
         self._id = None
         self._detail_message = None
@@ -206,14 +209,16 @@
             self.internal_id = internal_id
         if ack_comment is not None:
             self.ack_comment = ack_comment
         if monitor_object_name is not None:
             self.monitor_object_name = monitor_object_name
         if data_point_name is not None:
             self.data_point_name = data_point_name
+        if alert_group_entity_value is not None:
+            self.alert_group_entity_value = alert_group_entity_value
         if instance_id is not None:
             self.instance_id = instance_id
         if data_point_id is not None:
             self.data_point_id = data_point_id
         if suppress_desc is not None:
             self.suppress_desc = suppress_desc
         if next_recipient is not None:
@@ -596,14 +601,37 @@
         :param data_point_name: The data_point_name of this Alert.  # noqa: E501
         :type: str
         """
 
         self._data_point_name = data_point_name
 
     @property
+    def alert_group_entity_value(self):
+        """Gets the alert_group_entity_value of this Alert.  # noqa: E501
+
+        Alert group entity value for stateful log alerts  # noqa: E501
+
+        :return: The alert_group_entity_value of this Alert.  # noqa: E501
+        :rtype: str
+        """
+        return self._alert_group_entity_value
+
+    @alert_group_entity_value.setter
+    def alert_group_entity_value(self, alert_group_entity_value):
+        """Sets the alert_group_entity_value of this Alert.
+
+        Alert group entity value for stateful log alerts  # noqa: E501
+
+        :param alert_group_entity_value: The alert_group_entity_value of this Alert.  # noqa: E501
+        :type: str
+        """
+
+        self._alert_group_entity_value = alert_group_entity_value
+
+    @property
     def instance_id(self):
         """Gets the instance_id of this Alert.  # noqa: E501
 
         The id of the instance in alert  # noqa: E501
 
         :return: The instance_id of this Alert.  # noqa: E501
         :rtype: int
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_ack.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_ack.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_filters.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_filters.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_forecasting_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_forecasting_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_list_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_list_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         'type': 'str',
         'start_epoch': 'int',
         'enable_anomaly_alert_generation': 'str',
         'internal_id': 'str',
         'ack_comment': 'str',
         'monitor_object_name': 'str',
         'data_point_name': 'str',
+        'alert_group_entity_value': 'str',
         'instance_id': 'int',
         'data_point_id': 'int',
         'suppress_desc': 'str',
         'next_recipient': 'int',
         'suppressor': 'str',
         'id': 'str',
         'rule_id': 'int',
@@ -90,14 +91,15 @@
         'type': 'type',
         'start_epoch': 'startEpoch',
         'enable_anomaly_alert_generation': 'enableAnomalyAlertGeneration',
         'internal_id': 'internalId',
         'ack_comment': 'ackComment',
         'monitor_object_name': 'monitorObjectName',
         'data_point_name': 'dataPointName',
+        'alert_group_entity_value': 'alertGroupEntityValue',
         'instance_id': 'instanceId',
         'data_point_id': 'dataPointId',
         'suppress_desc': 'suppressDesc',
         'next_recipient': 'nextRecipient',
         'suppressor': 'suppressor',
         'id': 'id',
         'rule_id': 'ruleId',
@@ -124,15 +126,15 @@
         'chain_id': 'chainId',
         'resource_template_id': 'resourceTemplateId',
         'cleared': 'cleared',
         'ad_alert_desc': 'adAlertDesc',
         'resource_template_name': 'resourceTemplateName'
     }
 
-    def __init__(self, resource_id=None, anomaly=None, instance_name=None, monitor_object_id=None, end_epoch=None, rule=None, threshold=None, type=None, start_epoch=None, enable_anomaly_alert_generation=None, internal_id=None, ack_comment=None, monitor_object_name=None, data_point_name=None, instance_id=None, data_point_id=None, suppress_desc=None, next_recipient=None, suppressor=None, id=None, rule_id=None, tenant=None, alert_value=None, ad_alert=None, acked_by=None, severity=None, sdted=None, acked_epoch=None, chain=None, sdt=None, sub_chain_id=None, enable_anomaly_alert_suppression=None, received_list=None, monitor_object_type=None, acked=None, resource_template_type=None, clear_value=None, instance_description=None, dependency_routing_state=None, monitor_object_groups=None, dependency_role=None, chain_id=None, resource_template_id=None, cleared=None, ad_alert_desc=None, resource_template_name=None):  # noqa: E501
+    def __init__(self, resource_id=None, anomaly=None, instance_name=None, monitor_object_id=None, end_epoch=None, rule=None, threshold=None, type=None, start_epoch=None, enable_anomaly_alert_generation=None, internal_id=None, ack_comment=None, monitor_object_name=None, data_point_name=None, alert_group_entity_value=None, instance_id=None, data_point_id=None, suppress_desc=None, next_recipient=None, suppressor=None, id=None, rule_id=None, tenant=None, alert_value=None, ad_alert=None, acked_by=None, severity=None, sdted=None, acked_epoch=None, chain=None, sdt=None, sub_chain_id=None, enable_anomaly_alert_suppression=None, received_list=None, monitor_object_type=None, acked=None, resource_template_type=None, clear_value=None, instance_description=None, dependency_routing_state=None, monitor_object_groups=None, dependency_role=None, chain_id=None, resource_template_id=None, cleared=None, ad_alert_desc=None, resource_template_name=None):  # noqa: E501
         """AlertResponse - a model defined in Swagger"""  # noqa: E501
 
         self._resource_id = None
         self._anomaly = None
         self._instance_name = None
         self._monitor_object_id = None
         self._end_epoch = None
@@ -141,14 +143,15 @@
         self._type = None
         self._start_epoch = None
         self._enable_anomaly_alert_generation = None
         self._internal_id = None
         self._ack_comment = None
         self._monitor_object_name = None
         self._data_point_name = None
+        self._alert_group_entity_value = None
         self._instance_id = None
         self._data_point_id = None
         self._suppress_desc = None
         self._next_recipient = None
         self._suppressor = None
         self._id = None
         self._rule_id = None
@@ -203,14 +206,16 @@
             self.internal_id = internal_id
         if ack_comment is not None:
             self.ack_comment = ack_comment
         if monitor_object_name is not None:
             self.monitor_object_name = monitor_object_name
         if data_point_name is not None:
             self.data_point_name = data_point_name
+        if alert_group_entity_value is not None:
+            self.alert_group_entity_value = alert_group_entity_value
         if instance_id is not None:
             self.instance_id = instance_id
         if data_point_id is not None:
             self.data_point_id = data_point_id
         if suppress_desc is not None:
             self.suppress_desc = suppress_desc
         if next_recipient is not None:
@@ -591,14 +596,37 @@
         :param data_point_name: The data_point_name of this AlertResponse.  # noqa: E501
         :type: str
         """
 
         self._data_point_name = data_point_name
 
     @property
+    def alert_group_entity_value(self):
+        """Gets the alert_group_entity_value of this AlertResponse.  # noqa: E501
+
+        Alert group entity value for stateful log alerts  # noqa: E501
+
+        :return: The alert_group_entity_value of this AlertResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._alert_group_entity_value
+
+    @alert_group_entity_value.setter
+    def alert_group_entity_value(self, alert_group_entity_value):
+        """Sets the alert_group_entity_value of this AlertResponse.
+
+        Alert group entity value for stateful log alerts  # noqa: E501
+
+        :param alert_group_entity_value: The alert_group_entity_value of this AlertResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._alert_group_entity_value = alert_group_entity_value
+
+    @property
     def instance_id(self):
         """Gets the instance_id of this AlertResponse.  # noqa: E501
 
         The id of the instance in alert  # noqa: E501
 
         :return: The instance_id of this AlertResponse.  # noqa: E501
         :rtype: int
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_rule.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_rule.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_rule_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_rule_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_sla_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_sla_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_threshold_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_threshold_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_trends_metric.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_trends_metric.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_trends_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_trends_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/alert_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/alert_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/api_perf_metrics.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/api_perf_metrics.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/api_token.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/api_token.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/api_token_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/api_token_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/applies_to_function.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/applies_to_function.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/assignment.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/assignment.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/audit_log.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/audit_log_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/audit_log_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/authentication.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/authentication.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/auto_discovery_configuration.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/auto_discovery_configuration.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/auto_discovery_filter.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/auto_discovery_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/auto_discovery_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         'ad_netapp': 'NetAppAutoDiscoveryMethod',
         '': 'AzureAppServiceEnvironmentMultiRolePoolDiscoverMethod',
         '': 'GcpVpnTunnelDiscoveryMethodV3',
         'ad_azurebilling': 'AzureBillingDiscoveryMethod',
         '': 'AzureVwanVpnConnectionMethod',
         '': 'SaaSWebexLicenseDiscoveryMethod',
         '': 'GcpAppEngineDiscoveryMethod',
+        '': 'AwsGlobalNetworkDeviceMethod',
         'ad_pdh': 'PDHAutoDiscoveryMethod',
         '': 'AzureBackupProtectedItemBackupJobDiscoveryMethod',
         'ad_script': 'ScriptAutoDiscoveryMethod',
         'ad_dummy': 'DummyAutoDiscoveryMethod',
         'ad_awsec2reservedinstance': 'AwsEC2ReservedInstanceDiscoveryMethod',
         '': 'AzureCostManagementSubscriptionsDiscoveryMethod',
         '': 'AwsCognitoIdentityProvidersDiscoveryMethodV3',
@@ -67,24 +68,26 @@
         'ad_azureserviceregion': 'AzureServiceRegionDiscoveryMethod',
         '': 'SyntheticsSeleniumAutoDiscoveryMethodV3',
         '': 'GcpPubSubSubscriptionDiscoveryMethodV3',
         '': 'SaaSO365SharePointSiteDiscoveryMethod',
         '': 'AzureEABillingDiscoveryMethodV3',
         'ad_sdkscript': 'SDKScriptDiscoveryMethod',
         '': 'OpenMetricDiscoveryMethod',
+        '': 'AzureServiceBusTopic',
         'ad_awsecsservice': 'AwsEcsServiceDiscoveryMethod',
         'ad_awsapigatewaystage': 'AwsApiGatewayStageDiscoveryMethod',
         '': 'AzureActiveDirectoryAppSecretDiscoveryMethod',
         'ad_cloudwatch': 'CloudWatchAutoDiscoveryMethod',
         '': 'GcpBillingBigQuerySourceDiscoveryMethodV3',
         'ad_awsserviceregion': 'AwsServiceRegionDiscoveryMethod',
         '': 'SaaSSlackHealthDiscoveryMethod',
         '': 'AzureSynapseDiscoveryMethodV3',
         'ad_esx': 'ESXAutoDiscoveryMethod',
         'ad_collector': 'CollectorAutoDiscoveryMethod',
+        '': 'AzureServiceBusQueue',
         'ad_awslbtargetgroups': 'AwsLBTargetGroupDiscoveryMethod',
         '': 'AzureBackupJobDiscoveryMethod',
         'ad_awsec2scheduledevents': 'EC2ScheduledEventAutoDiscoveryMethod',
         'ad_jdbc': 'JDBCAutoDiscoveryMethod',
         'ad_azurevirtualdesktopsessionhosts': 'AzureVirtualDesktopSessionHostsDiscoveryMethod',
         '': 'SaasStatusDiscoveryMethod',
         '': 'SaasO365SkusDiscoveryMethod',
@@ -112,14 +115,15 @@
         'ad_awsec2reservedinstancecoverage': 'AwsEC2ReservedInstanceCoverageDiscoveryMethod',
         '': 'AwsSageMakerEndpointVariantMethod',
         'ad_cim': 'CIMAutoDiscoveryMethod',
         '': 'SaaSZoomPlanUsageDiscoveryMethod',
         '': 'AzureReplicationJobDiscoveryMethod',
         '': 'SaasO365MailboxDiscoveryMethod',
         '': 'SaasSalesforceLicenseDiscoveryMethod',
+        '': 'AwsGlobalNetworkLinkMethod',
         'ad_awsredshift': 'AwsRedShiftDiscoveryMethod',
         '': 'GcpLBBackendServiceDiscoveryMethodV3',
         'ad_awsmediaconnectsource': 'AwsMediaConnectSourceDiscoveryMethod',
         'ad_ec2': 'EC2AutoDiscoveryMethod',
         '': 'RabbitMQQueueAutoDiscoveryMethod',
         '': 'PaaSJsonPathDiscoveryMethod',
         '': 'SaasAirbrakeDiscoveryMethod',
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/automatic_upgrade_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/automatic_upgrade_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_account_id.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_account_id.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_account_test_result.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_account_test_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_api_gateway_stage_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_api_gateway_stage_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_auto_scaling_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_auto_scaling_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_billing_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_billing_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_billing_report_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_billing_report_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_billing_report_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_billing_report_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_classic_elb_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_classic_elb_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_cloud_watch_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_cloud_watch_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_cognito_identity_providers_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_cognito_identity_providers_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ebs_volume_snapshot_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ebs_volume_snapshot_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_reserved_instance_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_reserved_instance_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_reserved_instance_coverage_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_reserved_instance_coverage_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_reserved_instance_coverage_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_reserved_instance_coverage_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_reserved_instance_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_reserved_instance_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_scheduled_events_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_scheduled_events_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ec2_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ec2_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ecs_service_details_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ecs_service_details_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ecs_service_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ecs_service_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_elasti_cache_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_elasti_cache_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_external_id.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_external_id.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_global_web_acl_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_global_web_acl_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_lb_target_group_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_lb_target_group_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_media_connect_output_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_media_connect_output_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_media_connect_source_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_media_connect_source_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_rds_performance_insights_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_rds_performance_insights_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_rds_service_limits_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_rds_service_limits_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_red_shift_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_red_shift_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_route53_resolver_ip_address_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_route53_resolver_ip_address_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_route53_resolver_ip_address_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_route53_resolver_ip_address_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_rss_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_rss_event_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,26 +356,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this AwsRssEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this AwsRssEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this AwsRssEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this AwsRssEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_sage_maker_endpoint_variant_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_sage_maker_endpoint_variant_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_service_limits_from_trusted_advisor_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_service_limits_from_trusted_advisor_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_service_region_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_service_region_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_ses_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_ses_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_vpn_tunnel_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_vpn_tunnel_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/aws_web_acl_waf_v2_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/aws_web_acl_waf_v2_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_account_test_result.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_account_test_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_active_directory_app_secret_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_active_directory_app_secret_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_active_directory_app_secret_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_active_directory_app_secret_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_active_directory_sync_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_active_directory_sync_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_active_directory_users_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_active_directory_users_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_app_service_environment_multi_role_pool_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_app_service_environment_multi_role_pool_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_app_service_environment_multi_role_pool_discover_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_app_service_environment_multi_role_pool_discover_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_authentication_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_authentication_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_automation_account_certificate_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_automation_account_certificate_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_automation_account_certificate_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_automation_account_certificate_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_job_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_job_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_protected_item_backup_job_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_protected_item_backup_job_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_protected_item_backup_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_protected_item_backup_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_backup_protected_item_health_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_backup_protected_item_health_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_billing_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_billing_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_billing_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_billing_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_cost_management_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_cost_management_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_cost_management_dimensions_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_cost_management_dimensions_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_cost_management_subscriptions_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_cost_management_subscriptions_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_cost_management_tags_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_cost_management_tags_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_dimension_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_dimension_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_ea_billing_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_ea_billing_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_ea_billing_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_ea_billing_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_emerging_issue_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_emerging_issue_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,26 +356,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this AzureEmergingIssueEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this AzureEmergingIssueEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this AzureEmergingIssueEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this AzureEmergingIssueEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_express_route_circuit_peering_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_express_route_circuit_peering_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_express_route_circuit_peering_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_express_route_circuit_peering_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_insights_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_insights_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_log_analytics_replication_job_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_log_analytics_replication_job_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_log_analytics_replication_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_log_analytics_replication_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_log_analytics_workspaces_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_log_analytics_workspaces_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_log_analytics_workspaces_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_log_analytics_workspaces_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_net_app_volumes_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_net_app_volumes_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_network_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_network_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_recovery_service_rto_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_recovery_service_rto_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_recovery_service_rto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_recovery_service_rto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_recovery_service_vault_sr_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_recovery_service_vault_sr_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_recovery_services_vault_agents_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_recovery_services_vault_agents_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_redis_cache_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_redis_cache_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_replication_disaster_recovery_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_replication_disaster_recovery_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_replication_job_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_replication_job_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_replication_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_replication_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_resource_health_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_resource_health_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_resource_usage_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_resource_usage_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_rss_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_rss_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,26 +356,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this AzureRssEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this AzureRssEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this AzureRssEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this AzureRssEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_service_region_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_service_region_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_storage_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_storage_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_subscription_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_subscription_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_subscription_id_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_subscription_id_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_synapse_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_synapse_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_virtual_desktop_host_pools_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_virtual_desktop_host_pools_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vm_backup_status_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vm_backup_status_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vm_backup_status_log_analytics_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vm_backup_status_log_analytics_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vm_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vm_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vng_connection_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vng_connection_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vng_connection_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vng_connection_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vwan_vpn_connection_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vwan_vpn_connection_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_vwan_vpn_connection_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_vwan_vpn_connection_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_web_app_instance_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_web_app_instance_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_web_job_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_web_job_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/azure_web_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/azure_web_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/basic_authentication.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/basic_authentication.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/batch_job_execution_item.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/batch_job_execution_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/batch_job_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/batch_job_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/batch_job_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/batch_job_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/batch_script_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/batch_script_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_item.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/big_number_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/big_number_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/cell_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/cell_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/chain.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/chain.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/cim_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/cim_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/cim_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/cim_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/cloud_watch_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/cloud_watch_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_base.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_group.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_version.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_version.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/collector_version_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/collector_version_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/color_threshold.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/color_threshold.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/column_header.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/column_header.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/config_source_update_reasons_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/config_source_update_reasons_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/conversation_filter.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/conversation_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/counter.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/counter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_flexible_virtual_data_source_ex.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_flexible_virtual_data_source_ex.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_graph.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_graph.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_graph_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/custom_virtual_data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/custom_virtual_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_group.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dashboard_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dashboard_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_pump_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_pump_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_source_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_source_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_source_overview_graph.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_source_overview_graph.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/data_source_update_reasons_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/data_source_update_reasons_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/datasource_overview_graph_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/datasource_overview_graph_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/datasource_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/datasource_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/days_until_alert.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/days_until_alert.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/debug.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/debug.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_batch_job_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_batch_job_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_cluster_alert_def_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_cluster_alert_def_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_associated.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_associated.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_associated_instance.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_associated_instance.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_associated_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_associated_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_alert_setting.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_alert_setting.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from logicmonitor_sdk.models.device_group_alert_threshold_info import DeviceGroupAlertThresholdInfo  # noqa: F401,E501
 from logicmonitor_sdk.models.instance_group_alert_threshold_info import InstanceGroupAlertThresholdInfo  # noqa: F401,E501
+from logicmonitor_sdk.models.resource_data_source_alert_threshold_info import ResourceDataSourceAlertThresholdInfo  # noqa: F401,E501
 
 
 class DeviceDataSourceInstanceAlertSetting(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
@@ -35,28 +36,29 @@
     """
     swagger_types = {
         'global_alert_expr': 'str',
         'parent_instance_group_alert_expr': 'InstanceGroupAlertThresholdInfo',
         'alert_for_no_data': 'int',
         'post_processor_param': 'str',
         'disable_alerting': 'bool',
-        'global_alert_transition_interval': 'str',
+        'global_alert_transition_interval': 'int',
         'data_point_description': 'str',
         'global_enable_anomaly_alert_generation': 'str',
         'enable_anomaly_alert_generation': 'str',
         'disable_dp_alert_host_groups': 'str',
         'data_point_name': 'str',
         'data_point_id': 'int',
         'global_enable_anomaly_alert_suppression': 'str',
         'device_group_id': 'int',
         'id': 'int',
-        'global_alert_clear_transition_interval': 'str',
+        'global_alert_clear_transition_interval': 'int',
+        'parent_resource_data_source_alert_expr': 'ResourceDataSourceAlertThresholdInfo',
         'device_group_full_path': 'str',
         'alert_transition_interval': 'int',
-        'global_alert_for_no_data': 'str',
+        'global_alert_for_no_data': 'int',
         'enable_anomaly_alert_suppression': 'str',
         'alert_clear_interval': 'int',
         'critical_ad_adv_setting': 'str',
         'alert_expr_note': 'str',
         'ad_adv_setting_enabled': 'bool',
         'error_ad_adv_setting': 'str',
         'data_source_instance_id': 'int',
@@ -82,14 +84,15 @@
         'disable_dp_alert_host_groups': 'disableDpAlertHostGroups',
         'data_point_name': 'dataPointName',
         'data_point_id': 'dataPointId',
         'global_enable_anomaly_alert_suppression': 'globalEnableAnomalyAlertSuppression',
         'device_group_id': 'deviceGroupId',
         'id': 'id',
         'global_alert_clear_transition_interval': 'globalAlertClearTransitionInterval',
+        'parent_resource_data_source_alert_expr': 'parentResourceDataSourceAlertExpr',
         'device_group_full_path': 'deviceGroupFullPath',
         'alert_transition_interval': 'alertTransitionInterval',
         'global_alert_for_no_data': 'globalAlertForNoData',
         'enable_anomaly_alert_suppression': 'enableAnomalyAlertSuppression',
         'alert_clear_interval': 'alertClearInterval',
         'critical_ad_adv_setting': 'criticalAdAdvSetting',
         'alert_expr_note': 'alertExprNote',
@@ -101,15 +104,15 @@
         'parent_device_group_alert_expr_list': 'parentDeviceGroupAlertExprList',
         'alerting_disabled_on': 'alertingDisabledOn',
         'data_source_instance_alias': 'dataSourceInstanceAlias',
         'collection_interval': 'collectionInterval',
         'alert_expr': 'alertExpr'
     }
 
-    def __init__(self, global_alert_expr=None, parent_instance_group_alert_expr=None, alert_for_no_data=None, post_processor_param=None, disable_alerting=None, global_alert_transition_interval=None, data_point_description=None, global_enable_anomaly_alert_generation=None, enable_anomaly_alert_generation=None, disable_dp_alert_host_groups=None, data_point_name=None, data_point_id=None, global_enable_anomaly_alert_suppression=None, device_group_id=None, id=None, global_alert_clear_transition_interval=None, device_group_full_path=None, alert_transition_interval=None, global_alert_for_no_data=None, enable_anomaly_alert_suppression=None, alert_clear_interval=None, critical_ad_adv_setting=None, alert_expr_note=None, ad_adv_setting_enabled=None, error_ad_adv_setting=None, data_source_instance_id=None, warn_ad_adv_setting=None, global_post_processor_param=None, parent_device_group_alert_expr_list=None, alerting_disabled_on=None, data_source_instance_alias=None, collection_interval=None, alert_expr=None):  # noqa: E501
+    def __init__(self, global_alert_expr=None, parent_instance_group_alert_expr=None, alert_for_no_data=None, post_processor_param=None, disable_alerting=None, global_alert_transition_interval=None, data_point_description=None, global_enable_anomaly_alert_generation=None, enable_anomaly_alert_generation=None, disable_dp_alert_host_groups=None, data_point_name=None, data_point_id=None, global_enable_anomaly_alert_suppression=None, device_group_id=None, id=None, global_alert_clear_transition_interval=None, parent_resource_data_source_alert_expr=None, device_group_full_path=None, alert_transition_interval=None, global_alert_for_no_data=None, enable_anomaly_alert_suppression=None, alert_clear_interval=None, critical_ad_adv_setting=None, alert_expr_note=None, ad_adv_setting_enabled=None, error_ad_adv_setting=None, data_source_instance_id=None, warn_ad_adv_setting=None, global_post_processor_param=None, parent_device_group_alert_expr_list=None, alerting_disabled_on=None, data_source_instance_alias=None, collection_interval=None, alert_expr=None):  # noqa: E501
         """DeviceDataSourceInstanceAlertSetting - a model defined in Swagger"""  # noqa: E501
 
         self._global_alert_expr = None
         self._parent_instance_group_alert_expr = None
         self._alert_for_no_data = None
         self._post_processor_param = None
         self._disable_alerting = None
@@ -120,14 +123,15 @@
         self._disable_dp_alert_host_groups = None
         self._data_point_name = None
         self._data_point_id = None
         self._global_enable_anomaly_alert_suppression = None
         self._device_group_id = None
         self._id = None
         self._global_alert_clear_transition_interval = None
+        self._parent_resource_data_source_alert_expr = None
         self._device_group_full_path = None
         self._alert_transition_interval = None
         self._global_alert_for_no_data = None
         self._enable_anomaly_alert_suppression = None
         self._alert_clear_interval = None
         self._critical_ad_adv_setting = None
         self._alert_expr_note = None
@@ -171,14 +175,16 @@
             self.global_enable_anomaly_alert_suppression = global_enable_anomaly_alert_suppression
         if device_group_id is not None:
             self.device_group_id = device_group_id
         if id is not None:
             self.id = id
         if global_alert_clear_transition_interval is not None:
             self.global_alert_clear_transition_interval = global_alert_clear_transition_interval
+        if parent_resource_data_source_alert_expr is not None:
+            self.parent_resource_data_source_alert_expr = parent_resource_data_source_alert_expr
         if device_group_full_path is not None:
             self.device_group_full_path = device_group_full_path
         if alert_transition_interval is not None:
             self.alert_transition_interval = alert_transition_interval
         if global_alert_for_no_data is not None:
             self.global_alert_for_no_data = global_alert_for_no_data
         if enable_anomaly_alert_suppression is not None:
@@ -256,26 +262,26 @@
 
         self._parent_instance_group_alert_expr = parent_instance_group_alert_expr
 
     @property
     def alert_for_no_data(self):
         """Gets the alert_for_no_data of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
-        alert for no data  # noqa: E501
+        alert for no data (no alert-1, warning-2, error-3, critical-4)  # noqa: E501
 
         :return: The alert_for_no_data of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
         :rtype: int
         """
         return self._alert_for_no_data
 
     @alert_for_no_data.setter
     def alert_for_no_data(self, alert_for_no_data):
         """Sets the alert_for_no_data of this DeviceDataSourceInstanceAlertSetting.
 
-        alert for no data  # noqa: E501
+        alert for no data (no alert-1, warning-2, error-3, critical-4)  # noqa: E501
 
         :param alert_for_no_data: The alert_for_no_data of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
         :type: int
         """
 
         self._alert_for_no_data = alert_for_no_data
 
@@ -325,30 +331,30 @@
 
         self._disable_alerting = disable_alerting
 
     @property
     def global_alert_transition_interval(self):
         """Gets the global_alert_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
+        The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :return: The global_alert_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_transition_interval
 
     @global_alert_transition_interval.setter
     def global_alert_transition_interval(self, global_alert_transition_interval):
         """Sets the global_alert_transition_interval of this DeviceDataSourceInstanceAlertSetting.
 
+        The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :param global_alert_transition_interval: The global_alert_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_transition_interval = global_alert_transition_interval
 
     @property
     def data_point_description(self):
         """Gets the data_point_description of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
@@ -555,34 +561,57 @@
 
         self._id = id
 
     @property
     def global_alert_clear_transition_interval(self):
         """Gets the global_alert_clear_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
+        The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :return: The global_alert_clear_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_clear_transition_interval
 
     @global_alert_clear_transition_interval.setter
     def global_alert_clear_transition_interval(self, global_alert_clear_transition_interval):
         """Sets the global_alert_clear_transition_interval of this DeviceDataSourceInstanceAlertSetting.
 
+        The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :param global_alert_clear_transition_interval: The global_alert_clear_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_clear_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_clear_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_clear_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_clear_transition_interval = global_alert_clear_transition_interval
 
     @property
+    def parent_resource_data_source_alert_expr(self):
+        """Gets the parent_resource_data_source_alert_expr of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
+
+        Resource datasource alert expression list base on the priority. The first is the highest priority and effected on this instance  # noqa: E501
+
+        :return: The parent_resource_data_source_alert_expr of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
+        :rtype: ResourceDataSourceAlertThresholdInfo
+        """
+        return self._parent_resource_data_source_alert_expr
+
+    @parent_resource_data_source_alert_expr.setter
+    def parent_resource_data_source_alert_expr(self, parent_resource_data_source_alert_expr):
+        """Sets the parent_resource_data_source_alert_expr of this DeviceDataSourceInstanceAlertSetting.
+
+        Resource datasource alert expression list base on the priority. The first is the highest priority and effected on this instance  # noqa: E501
+
+        :param parent_resource_data_source_alert_expr: The parent_resource_data_source_alert_expr of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
+        :type: ResourceDataSourceAlertThresholdInfo
+        """
+
+        self._parent_resource_data_source_alert_expr = parent_resource_data_source_alert_expr
+
+    @property
     def device_group_full_path(self):
         """Gets the device_group_full_path of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
         The full path of the device group  # noqa: E501
 
         :return: The device_group_full_path of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
         :rtype: str
@@ -601,53 +630,53 @@
 
         self._device_group_full_path = device_group_full_path
 
     @property
     def alert_transition_interval(self):
         """Gets the alert_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
-        The interval of alert transition  # noqa: E501
+        The polling interval of alert transition (0-60)  # noqa: E501
 
         :return: The alert_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
         :rtype: int
         """
         return self._alert_transition_interval
 
     @alert_transition_interval.setter
     def alert_transition_interval(self, alert_transition_interval):
         """Sets the alert_transition_interval of this DeviceDataSourceInstanceAlertSetting.
 
-        The interval of alert transition  # noqa: E501
+        The polling interval of alert transition (0-60)  # noqa: E501
 
         :param alert_transition_interval: The alert_transition_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
         :type: int
         """
 
         self._alert_transition_interval = alert_transition_interval
 
     @property
     def global_alert_for_no_data(self):
         """Gets the global_alert_for_no_data of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
+        The triggered alert level if we cannot collect data for this datapoint  # noqa: E501
 
         :return: The global_alert_for_no_data of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_for_no_data
 
     @global_alert_for_no_data.setter
     def global_alert_for_no_data(self, global_alert_for_no_data):
         """Sets the global_alert_for_no_data of this DeviceDataSourceInstanceAlertSetting.
 
+        The triggered alert level if we cannot collect data for this datapoint  # noqa: E501
 
         :param global_alert_for_no_data: The global_alert_for_no_data of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_for_no_data is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_for_no_data):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_for_no_data`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_for_no_data = global_alert_for_no_data
 
     @property
     def enable_anomaly_alert_suppression(self):
         """Gets the enable_anomaly_alert_suppression of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
@@ -670,26 +699,26 @@
 
         self._enable_anomaly_alert_suppression = enable_anomaly_alert_suppression
 
     @property
     def alert_clear_interval(self):
         """Gets the alert_clear_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
 
-        The interval of alert clear transition  # noqa: E501
+        The polling interval of alert clear transition (0-60)  # noqa: E501
 
         :return: The alert_clear_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
         :rtype: int
         """
         return self._alert_clear_interval
 
     @alert_clear_interval.setter
     def alert_clear_interval(self, alert_clear_interval):
         """Sets the alert_clear_interval of this DeviceDataSourceInstanceAlertSetting.
 
-        The interval of alert clear transition  # noqa: E501
+        The polling interval of alert clear transition (0-60)  # noqa: E501
 
         :param alert_clear_interval: The alert_clear_interval of this DeviceDataSourceInstanceAlertSetting.  # noqa: E501
         :type: int
         """
 
         self._alert_clear_interval = alert_clear_interval
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_alert_setting_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_alert_setting_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_config.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'instance_name': 'str',
         'device_data_source_id': 'int',
         'exclude_lines': 'list[int]',
         'config_status': 'int',
+        'compared_with': 'str',
         'version': 'int',
         'device_id': 'int',
         'delta_config': 'list[DeviceDataSourceInstanceConfigDiff]',
         'device_display_name': 'str',
         'data_source_name': 'str',
         'alerts': 'list[DeviceDataSourceInstanceConfigAlert]',
         'data_source_id': 'int',
@@ -54,14 +55,15 @@
     }
 
     attribute_map = {
         'instance_name': 'instanceName',
         'device_data_source_id': 'deviceDataSourceId',
         'exclude_lines': 'excludeLines',
         'config_status': 'configStatus',
+        'compared_with': 'comparedWith',
         'version': 'version',
         'device_id': 'deviceId',
         'delta_config': 'deltaConfig',
         'device_display_name': 'deviceDisplayName',
         'data_source_name': 'dataSourceName',
         'alerts': 'alerts',
         'data_source_id': 'dataSourceId',
@@ -69,21 +71,22 @@
         'config_err_msg': 'configErrMsg',
         'change_status': 'changeStatus',
         'id': 'id',
         'poll_timestamp': 'pollTimestamp',
         'config': 'config'
     }
 
-    def __init__(self, instance_name=None, device_data_source_id=None, exclude_lines=None, config_status=None, version=None, device_id=None, delta_config=None, device_display_name=None, data_source_name=None, alerts=None, data_source_id=None, instance_id=None, config_err_msg=None, change_status=None, id=None, poll_timestamp=None, config=None):  # noqa: E501
+    def __init__(self, instance_name=None, device_data_source_id=None, exclude_lines=None, config_status=None, compared_with=None, version=None, device_id=None, delta_config=None, device_display_name=None, data_source_name=None, alerts=None, data_source_id=None, instance_id=None, config_err_msg=None, change_status=None, id=None, poll_timestamp=None, config=None):  # noqa: E501
         """DeviceDataSourceInstanceConfig - a model defined in Swagger"""  # noqa: E501
 
         self._instance_name = None
         self._device_data_source_id = None
         self._exclude_lines = None
         self._config_status = None
+        self._compared_with = None
         self._version = None
         self._device_id = None
         self._delta_config = None
         self._device_display_name = None
         self._data_source_name = None
         self._alerts = None
         self._data_source_id = None
@@ -99,14 +102,16 @@
             self.instance_name = instance_name
         if device_data_source_id is not None:
             self.device_data_source_id = device_data_source_id
         if exclude_lines is not None:
             self.exclude_lines = exclude_lines
         if config_status is not None:
             self.config_status = config_status
+        if compared_with is not None:
+            self.compared_with = compared_with
         if version is not None:
             self.version = version
         if device_id is not None:
             self.device_id = device_id
         if delta_config is not None:
             self.delta_config = delta_config
         if device_display_name is not None:
@@ -219,14 +224,37 @@
         :param config_status: The config_status of this DeviceDataSourceInstanceConfig.  # noqa: E501
         :type: int
         """
 
         self._config_status = config_status
 
     @property
+    def compared_with(self):
+        """Gets the compared_with of this DeviceDataSourceInstanceConfig.  # noqa: E501
+
+        Version compared with and found difference  # noqa: E501
+
+        :return: The compared_with of this DeviceDataSourceInstanceConfig.  # noqa: E501
+        :rtype: str
+        """
+        return self._compared_with
+
+    @compared_with.setter
+    def compared_with(self, compared_with):
+        """Sets the compared_with of this DeviceDataSourceInstanceConfig.
+
+        Version compared with and found difference  # noqa: E501
+
+        :param compared_with: The compared_with of this DeviceDataSourceInstanceConfig.  # noqa: E501
+        :type: str
+        """
+
+        self._compared_with = compared_with
+
+    @property
     def version(self):
         """Gets the version of this DeviceDataSourceInstanceConfig.  # noqa: E501
 
         Config version  # noqa: E501
 
         :return: The version of this DeviceDataSourceInstanceConfig.  # noqa: E501
         :rtype: int
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_config_alert.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_config_alert.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_config_diff.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_config_diff.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_group.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_group_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_group_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_instance_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_instance_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_data_source_sdt_history_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_data_source_sdt_history_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_graph.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_graph.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_instance_config_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_instance_config_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_instance_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_instance_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_instance_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_instance_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_datasource_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_datasource_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_delta_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_delta_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_event_source_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_event_source_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_filter.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_alert_threshold_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_alert_threshold_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,23 +28,23 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'enable_anomaly_alert_generation': 'str',
-        'alert_for_no_data': 'str',
+        'alert_for_no_data': 'int',
         'user_permission': 'str',
         'enable_anomaly_alert_suppression': 'str',
         'group_id': 'int',
-        'alert_clear_transition_interval': 'str',
+        'alert_clear_transition_interval': 'int',
         'alert_enabled': 'bool',
         'group_full_path': 'str',
         'alert_expr': 'str',
-        'alert_transition_interval': 'str'
+        'alert_transition_interval': 'int'
     }
 
     attribute_map = {
         'enable_anomaly_alert_generation': 'enableAnomalyAlertGeneration',
         'alert_for_no_data': 'alertForNoData',
         'user_permission': 'userPermission',
         'enable_anomaly_alert_suppression': 'enableAnomalyAlertSuppression',
@@ -115,32 +115,30 @@
 
         self._enable_anomaly_alert_generation = enable_anomaly_alert_generation
 
     @property
     def alert_for_no_data(self):
         """Gets the alert_for_no_data of this DeviceGroupAlertThresholdInfo.  # noqa: E501
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :return: The alert_for_no_data of this DeviceGroupAlertThresholdInfo.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_for_no_data
 
     @alert_for_no_data.setter
     def alert_for_no_data(self, alert_for_no_data):
         """Sets the alert_for_no_data of this DeviceGroupAlertThresholdInfo.
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :param alert_for_no_data: The alert_for_no_data of this DeviceGroupAlertThresholdInfo.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_for_no_data is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_for_no_data):  # noqa: E501
-            raise ValueError("Invalid value for `alert_for_no_data`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_for_no_data = alert_for_no_data
 
     @property
     def user_permission(self):
         """Gets the user_permission of this DeviceGroupAlertThresholdInfo.  # noqa: E501
 
@@ -208,29 +206,27 @@
     @property
     def alert_clear_transition_interval(self):
         """Gets the alert_clear_transition_interval of this DeviceGroupAlertThresholdInfo.  # noqa: E501
 
         The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :return: The alert_clear_transition_interval of this DeviceGroupAlertThresholdInfo.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_clear_transition_interval
 
     @alert_clear_transition_interval.setter
     def alert_clear_transition_interval(self, alert_clear_transition_interval):
         """Sets the alert_clear_transition_interval of this DeviceGroupAlertThresholdInfo.
 
         The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :param alert_clear_transition_interval: The alert_clear_transition_interval of this DeviceGroupAlertThresholdInfo.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_clear_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_clear_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `alert_clear_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_clear_transition_interval = alert_clear_transition_interval
 
     @property
     def alert_enabled(self):
         """Gets the alert_enabled of this DeviceGroupAlertThresholdInfo.  # noqa: E501
 
@@ -296,29 +292,27 @@
     @property
     def alert_transition_interval(self):
         """Gets the alert_transition_interval of this DeviceGroupAlertThresholdInfo.  # noqa: E501
 
         The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :return: The alert_transition_interval of this DeviceGroupAlertThresholdInfo.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_transition_interval
 
     @alert_transition_interval.setter
     def alert_transition_interval(self, alert_transition_interval):
         """Sets the alert_transition_interval of this DeviceGroupAlertThresholdInfo.
 
         The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :param alert_transition_interval: The alert_transition_interval of this DeviceGroupAlertThresholdInfo.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `alert_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_transition_interval = alert_transition_interval
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_data_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_data_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_data_source_alert_config.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_data_source_alert_config.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_data_source_data_point_config.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_data_source_data_point_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,35 +28,35 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'global_alert_expr': 'str',
-        'alert_for_no_data': 'str',
+        'alert_for_no_data': 'int',
         'enable_anomaly_alert_suppression': 'str',
-        'global_alert_for_no_data': 'str',
+        'global_alert_for_no_data': 'int',
         'critical_ad_adv_setting': 'str',
         'disable_alerting': 'bool',
-        'alert_clear_transition_interval': 'str',
-        'global_alert_transition_interval': 'str',
+        'alert_clear_transition_interval': 'int',
+        'global_alert_transition_interval': 'int',
         'alert_expr_note': 'str',
         'ad_adv_setting_enabled': 'bool',
         'error_ad_adv_setting': 'str',
         'data_point_description': 'str',
         'global_enable_anomaly_alert_generation': 'str',
         'enable_anomaly_alert_generation': 'str',
         'warn_ad_adv_setting': 'str',
         'data_point_name': 'str',
         'data_point_id': 'int',
         'global_enable_anomaly_alert_suppression': 'str',
-        'global_alert_clear_transition_interval': 'str',
+        'global_alert_clear_transition_interval': 'int',
         'collection_interval': 'int',
         'alert_expr': 'str',
-        'alert_transition_interval': 'str'
+        'alert_transition_interval': 'int'
     }
 
     attribute_map = {
         'global_alert_expr': 'globalAlertExpr',
         'alert_for_no_data': 'alertForNoData',
         'enable_anomaly_alert_suppression': 'enableAnomalyAlertSuppression',
         'global_alert_for_no_data': 'globalAlertForNoData',
@@ -170,32 +170,30 @@
 
         self._global_alert_expr = global_alert_expr
 
     @property
     def alert_for_no_data(self):
         """Gets the alert_for_no_data of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :return: The alert_for_no_data of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_for_no_data
 
     @alert_for_no_data.setter
     def alert_for_no_data(self, alert_for_no_data):
         """Sets the alert_for_no_data of this DeviceGroupDataSourceDataPointConfig.
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :param alert_for_no_data: The alert_for_no_data of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_for_no_data is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_for_no_data):  # noqa: E501
-            raise ValueError("Invalid value for `alert_for_no_data`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_for_no_data = alert_for_no_data
 
     @property
     def enable_anomaly_alert_suppression(self):
         """Gets the enable_anomaly_alert_suppression of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
@@ -216,32 +214,30 @@
 
         self._enable_anomaly_alert_suppression = enable_anomaly_alert_suppression
 
     @property
     def global_alert_for_no_data(self):
         """Gets the global_alert_for_no_data of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :return: The global_alert_for_no_data of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_for_no_data
 
     @global_alert_for_no_data.setter
     def global_alert_for_no_data(self, global_alert_for_no_data):
         """Sets the global_alert_for_no_data of this DeviceGroupDataSourceDataPointConfig.
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :param global_alert_for_no_data: The global_alert_for_no_data of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_for_no_data is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_for_no_data):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_for_no_data`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_for_no_data = global_alert_for_no_data
 
     @property
     def critical_ad_adv_setting(self):
         """Gets the critical_ad_adv_setting of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
@@ -283,57 +279,53 @@
 
         self._disable_alerting = disable_alerting
 
     @property
     def alert_clear_transition_interval(self):
         """Gets the alert_clear_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
-        The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
+        The count that the alert must exist for this many poll cycles before the alert will be cleared (0-60)  # noqa: E501
 
         :return: The alert_clear_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_clear_transition_interval
 
     @alert_clear_transition_interval.setter
     def alert_clear_transition_interval(self, alert_clear_transition_interval):
         """Sets the alert_clear_transition_interval of this DeviceGroupDataSourceDataPointConfig.
 
-        The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
+        The count that the alert must exist for this many poll cycles before the alert will be cleared (0-60)  # noqa: E501
 
         :param alert_clear_transition_interval: The alert_clear_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_clear_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_clear_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `alert_clear_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_clear_transition_interval = alert_clear_transition_interval
 
     @property
     def global_alert_transition_interval(self):
         """Gets the global_alert_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
         The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :return: The global_alert_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_transition_interval
 
     @global_alert_transition_interval.setter
     def global_alert_transition_interval(self, global_alert_transition_interval):
         """Sets the global_alert_transition_interval of this DeviceGroupDataSourceDataPointConfig.
 
         The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :param global_alert_transition_interval: The global_alert_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_transition_interval = global_alert_transition_interval
 
     @property
     def alert_expr_note(self):
         """Gets the alert_expr_note of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
@@ -550,29 +542,27 @@
     @property
     def global_alert_clear_transition_interval(self):
         """Gets the global_alert_clear_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
         The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :return: The global_alert_clear_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_clear_transition_interval
 
     @global_alert_clear_transition_interval.setter
     def global_alert_clear_transition_interval(self, global_alert_clear_transition_interval):
         """Sets the global_alert_clear_transition_interval of this DeviceGroupDataSourceDataPointConfig.
 
         The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :param global_alert_clear_transition_interval: The global_alert_clear_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_clear_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_clear_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_clear_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_clear_transition_interval = global_alert_clear_transition_interval
 
     @property
     def collection_interval(self):
         """Gets the collection_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
@@ -618,32 +608,30 @@
 
         self._alert_expr = alert_expr
 
     @property
     def alert_transition_interval(self):
         """Gets the alert_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
 
-        The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
+        The count that the alert must exist for this many poll cycles before it will be triggered (0-60)  # noqa: E501
 
         :return: The alert_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_transition_interval
 
     @alert_transition_interval.setter
     def alert_transition_interval(self, alert_transition_interval):
         """Sets the alert_transition_interval of this DeviceGroupDataSourceDataPointConfig.
 
-        The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
+        The count that the alert must exist for this many poll cycles before it will be triggered (0-60)  # noqa: E501
 
         :param alert_transition_interval: The alert_transition_interval of this DeviceGroupDataSourceDataPointConfig.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `alert_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_transition_interval = alert_transition_interval
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_datasource_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_datasource_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_group_sdt_history_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_group_sdt_history_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_instance_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_instance_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_instance_data_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_instance_data_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_instances.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_instances.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_log_pipe_line_resource_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_log_pipe_line_resource_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_noc_item.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_noc_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_property.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_property.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_sdt_history_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_sdt_history_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_sla_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_sla_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_sla_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_sla_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/device_status.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/device_status.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dns_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dns_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dummy_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dummy_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_column.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_column.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_table_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_table_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_table_widget_column.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_table_widget_column.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_table_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_table_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/dynamic_table_widget_row.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/dynamic_table_widget_row.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_ddr.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_ddr.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_netscan.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_netscan_policy_credential.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_netscan_policy_credential.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ec2_scheduled_event_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ec2_scheduled_event_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/echo_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/echo_event_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,26 +351,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this EchoEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this EchoEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this EchoEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this EchoEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/enhanced_script_netscan.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/enhanced_script_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/entity_property.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/entity_property.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/error_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/error_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/escalating_chain.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/escalating_chain.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/escalation_chain_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/escalation_chain_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/esx_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/esx_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/esx_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/esx_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,16 @@
         '': 'RestAzureAdvisorEventSource',
         'logfile': 'LogFileEventSource',
         '': 'IPMIEventSource',
         '': 'RestAwsTrustedAdvisorEventSource',
         '': 'RestAzureResourceLogAnalyticsWorkspacesSource',
         '': 'RestAzureResourceHealthEventSource',
         '': 'AzureEmergingIssueEventSource',
-        'azurerss': 'AzureRssEventSource'
+        'azurerss': 'AzureRssEventSource',
+        '': 'RestAwsOrganizationalHealthEventSource'
     }
 
     def __init__(self, suppress_duplicates_es=None, alert_subject_template=None, alert_level=None, description=None, applies_to=None, technology=None, filters=None, version=None, lineage_id=None, collector=None, tags=None, audit_version=None, installation_metadata=None, alert_body_template=None, checksum=None, name=None, clear_after_ack=None, id=None, alert_effective_ival=None, group=None):  # noqa: E501
         """EventSource - a model defined in Swagger"""  # noqa: E501
 
         self._suppress_duplicates_es = None
         self._alert_subject_template = None
@@ -370,26 +371,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this EventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this EventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this EventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this EventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/event_source_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/event_source_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/exclude_duplicate_ips.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/exclude_duplicate_ips.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/flash_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/flash_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/flow_record_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/flow_record_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gauge_data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gauge_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gauge_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gauge_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gauge_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gauge_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_account_test_result.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_account_test_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_app_engine_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_app_engine_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_atom_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_atom_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,26 +356,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this GcpAtomEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this GcpAtomEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this GcpAtomEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this GcpAtomEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_backend_service_health_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_backend_service_health_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_billing_big_query_source_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_billing_big_query_source_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_billing_big_query_source_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_billing_big_query_source_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_billing_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_billing_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_billing_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_billing_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_compute_service_limits_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_compute_service_limits_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_lb_backend_service_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_lb_backend_service_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_pub_sub_snapshot_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_pub_sub_snapshot_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_pub_sub_subscription_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_pub_sub_subscription_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_stack_driver_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_stack_driver_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/gcp_vpn_tunnel_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/gcp_vpn_tunnel_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/generate_report_request.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/generate_report_request.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/generate_report_result.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/generate_report_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/glob_match_toggle.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/glob_match_toggle.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/google_map_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/google_map_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/google_map_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/google_map_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_display.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_display.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_line.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_line.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_ops_note_scope.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_ops_note_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_plot.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_plot.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_plot_line.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_plot_line.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/graph_virtual_data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/graph_virtual_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/group_net_flow_record.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/group_net_flow_record.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_cpu_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_cpu_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_group_inventory_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_group_inventory_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_inventory_metric.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_inventory_metric.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_inventory_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_inventory_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/host_metrics_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/host_metrics_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/html_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/html_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/http_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/http_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ilp.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ilp.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/inheritance_prop.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/inheritance_prop.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/instance_group_alert_threshold_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/instance_group_alert_threshold_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,21 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'enable_anomaly_alert_generation': 'str',
-        'alert_for_no_data': 'str',
+        'alert_for_no_data': 'int',
         'enable_anomaly_alert_suppression': 'str',
         'group_id': 'int',
-        'alert_clear_transition_interval': 'str',
+        'alert_clear_transition_interval': 'int',
         'alert_enabled': 'bool',
         'alert_expr': 'str',
-        'alert_transition_interval': 'str'
+        'alert_transition_interval': 'int'
     }
 
     attribute_map = {
         'enable_anomaly_alert_generation': 'enableAnomalyAlertGeneration',
         'alert_for_no_data': 'alertForNoData',
         'enable_anomaly_alert_suppression': 'enableAnomalyAlertSuppression',
         'group_id': 'groupId',
@@ -105,32 +105,30 @@
 
         self._enable_anomaly_alert_generation = enable_anomaly_alert_generation
 
     @property
     def alert_for_no_data(self):
         """Gets the alert_for_no_data of this InstanceGroupAlertThresholdInfo.  # noqa: E501
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 ( 1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :return: The alert_for_no_data of this InstanceGroupAlertThresholdInfo.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_for_no_data
 
     @alert_for_no_data.setter
     def alert_for_no_data(self, alert_for_no_data):
         """Sets the alert_for_no_data of this InstanceGroupAlertThresholdInfo.
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 ( 1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :param alert_for_no_data: The alert_for_no_data of this InstanceGroupAlertThresholdInfo.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_for_no_data is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_for_no_data):  # noqa: E501
-            raise ValueError("Invalid value for `alert_for_no_data`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_for_no_data = alert_for_no_data
 
     @property
     def enable_anomaly_alert_suppression(self):
         """Gets the enable_anomaly_alert_suppression of this InstanceGroupAlertThresholdInfo.  # noqa: E501
 
@@ -177,29 +175,27 @@
     @property
     def alert_clear_transition_interval(self):
         """Gets the alert_clear_transition_interval of this InstanceGroupAlertThresholdInfo.  # noqa: E501
 
         The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :return: The alert_clear_transition_interval of this InstanceGroupAlertThresholdInfo.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_clear_transition_interval
 
     @alert_clear_transition_interval.setter
     def alert_clear_transition_interval(self, alert_clear_transition_interval):
         """Sets the alert_clear_transition_interval of this InstanceGroupAlertThresholdInfo.
 
         The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :param alert_clear_transition_interval: The alert_clear_transition_interval of this InstanceGroupAlertThresholdInfo.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_clear_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_clear_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `alert_clear_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_clear_transition_interval = alert_clear_transition_interval
 
     @property
     def alert_enabled(self):
         """Gets the alert_enabled of this InstanceGroupAlertThresholdInfo.  # noqa: E501
 
@@ -244,29 +240,27 @@
     @property
     def alert_transition_interval(self):
         """Gets the alert_transition_interval of this InstanceGroupAlertThresholdInfo.  # noqa: E501
 
         The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :return: The alert_transition_interval of this InstanceGroupAlertThresholdInfo.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_transition_interval
 
     @alert_transition_interval.setter
     def alert_transition_interval(self, alert_transition_interval):
         """Sets the alert_transition_interval of this InstanceGroupAlertThresholdInfo.
 
         The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :param alert_transition_interval: The alert_transition_interval of this InstanceGroupAlertThresholdInfo.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `alert_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_transition_interval = alert_transition_interval
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/integration_audit_log.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/integration_audit_log.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/integration_audit_log_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/integration_audit_log_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/integration_metadata.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/integration_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,77 +32,85 @@
     """
     swagger_types = {
         'target_last_published_id': 'str',
         'target_last_published_checksum': 'str',
         'target_last_published_version': 'str',
         'origin_checksum': 'str',
         'origin_author_namespace': 'str',
+        'origin_locator': 'str',
         'is_changed_from_origin': 'bool',
         'audited_registry_id': 'str',
         'target_lineage_id': 'str',
         'logic_module_type': 'str',
         'is_changed_from_target_last_published': 'bool',
         'origin_lineage_id': 'str',
         'origin_author_company_uuid': 'str',
         'local_module_id': 'int',
         'origin_registry_id': 'str',
         'origin_version': 'str',
-        'audited_version': 'str'
+        'audited_version': 'str',
+        'origin_name': 'str'
     }
 
     attribute_map = {
         'target_last_published_id': 'targetLastPublishedId',
         'target_last_published_checksum': 'targetLastPublishedChecksum',
         'target_last_published_version': 'targetLastPublishedVersion',
         'origin_checksum': 'originChecksum',
         'origin_author_namespace': 'originAuthorNamespace',
+        'origin_locator': 'originLocator',
         'is_changed_from_origin': 'isChangedFromOrigin',
         'audited_registry_id': 'auditedRegistryId',
         'target_lineage_id': 'targetLineageId',
         'logic_module_type': 'logicModuleType',
         'is_changed_from_target_last_published': 'isChangedFromTargetLastPublished',
         'origin_lineage_id': 'originLineageId',
         'origin_author_company_uuid': 'originAuthorCompanyUUID',
         'local_module_id': 'localModuleId',
         'origin_registry_id': 'originRegistryId',
         'origin_version': 'originVersion',
-        'audited_version': 'auditedVersion'
+        'audited_version': 'auditedVersion',
+        'origin_name': 'originName'
     }
 
-    def __init__(self, target_last_published_id=None, target_last_published_checksum=None, target_last_published_version=None, origin_checksum=None, origin_author_namespace=None, is_changed_from_origin=None, audited_registry_id=None, target_lineage_id=None, logic_module_type=None, is_changed_from_target_last_published=None, origin_lineage_id=None, origin_author_company_uuid=None, local_module_id=None, origin_registry_id=None, origin_version=None, audited_version=None):  # noqa: E501
+    def __init__(self, target_last_published_id=None, target_last_published_checksum=None, target_last_published_version=None, origin_checksum=None, origin_author_namespace=None, origin_locator=None, is_changed_from_origin=None, audited_registry_id=None, target_lineage_id=None, logic_module_type=None, is_changed_from_target_last_published=None, origin_lineage_id=None, origin_author_company_uuid=None, local_module_id=None, origin_registry_id=None, origin_version=None, audited_version=None, origin_name=None):  # noqa: E501
         """IntegrationMetadata - a model defined in Swagger"""  # noqa: E501
 
         self._target_last_published_id = None
         self._target_last_published_checksum = None
         self._target_last_published_version = None
         self._origin_checksum = None
         self._origin_author_namespace = None
+        self._origin_locator = None
         self._is_changed_from_origin = None
         self._audited_registry_id = None
         self._target_lineage_id = None
         self._logic_module_type = None
         self._is_changed_from_target_last_published = None
         self._origin_lineage_id = None
         self._origin_author_company_uuid = None
         self._local_module_id = None
         self._origin_registry_id = None
         self._origin_version = None
         self._audited_version = None
+        self._origin_name = None
         self.discriminator = None
 
         if target_last_published_id is not None:
             self.target_last_published_id = target_last_published_id
         if target_last_published_checksum is not None:
             self.target_last_published_checksum = target_last_published_checksum
         if target_last_published_version is not None:
             self.target_last_published_version = target_last_published_version
         if origin_checksum is not None:
             self.origin_checksum = origin_checksum
         if origin_author_namespace is not None:
             self.origin_author_namespace = origin_author_namespace
+        if origin_locator is not None:
+            self.origin_locator = origin_locator
         if is_changed_from_origin is not None:
             self.is_changed_from_origin = is_changed_from_origin
         if audited_registry_id is not None:
             self.audited_registry_id = audited_registry_id
         if target_lineage_id is not None:
             self.target_lineage_id = target_lineage_id
         if logic_module_type is not None:
@@ -117,14 +125,16 @@
             self.local_module_id = local_module_id
         if origin_registry_id is not None:
             self.origin_registry_id = origin_registry_id
         if origin_version is not None:
             self.origin_version = origin_version
         if audited_version is not None:
             self.audited_version = audited_version
+        if origin_name is not None:
+            self.origin_name = origin_name
 
     @property
     def target_last_published_id(self):
         """Gets the target_last_published_id of this IntegrationMetadata.  # noqa: E501
 
         Specifies the target last published Id  # noqa: E501
 
@@ -234,14 +244,37 @@
         :param origin_author_namespace: The origin_author_namespace of this IntegrationMetadata.  # noqa: E501
         :type: str
         """
 
         self._origin_author_namespace = origin_author_namespace
 
     @property
+    def origin_locator(self):
+        """Gets the origin_locator of this IntegrationMetadata.  # noqa: E501
+
+        Specifies the origin version locator  # noqa: E501
+
+        :return: The origin_locator of this IntegrationMetadata.  # noqa: E501
+        :rtype: str
+        """
+        return self._origin_locator
+
+    @origin_locator.setter
+    def origin_locator(self, origin_locator):
+        """Sets the origin_locator of this IntegrationMetadata.
+
+        Specifies the origin version locator  # noqa: E501
+
+        :param origin_locator: The origin_locator of this IntegrationMetadata.  # noqa: E501
+        :type: str
+        """
+
+        self._origin_locator = origin_locator
+
+    @property
     def is_changed_from_origin(self):
         """Gets the is_changed_from_origin of this IntegrationMetadata.  # noqa: E501
 
         Specifies if the Applies To function is changed from origin or not  # noqa: E501
 
         :return: The is_changed_from_origin of this IntegrationMetadata.  # noqa: E501
         :rtype: bool
@@ -492,14 +525,37 @@
 
         :param audited_version: The audited_version of this IntegrationMetadata.  # noqa: E501
         :type: str
         """
 
         self._audited_version = audited_version
 
+    @property
+    def origin_name(self):
+        """Gets the origin_name of this IntegrationMetadata.  # noqa: E501
+
+        Specifies the origin module name  # noqa: E501
+
+        :return: The origin_name of this IntegrationMetadata.  # noqa: E501
+        :rtype: str
+        """
+        return self._origin_name
+
+    @origin_name.setter
+    def origin_name(self, origin_name):
+        """Sets the origin_name of this IntegrationMetadata.
+
+        Specifies the origin module name  # noqa: E501
+
+        :param origin_name: The origin_name of this IntegrationMetadata.  # noqa: E501
+        :type: str
+        """
+
+        self._origin_name = origin_name
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/interf_bandwidth_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/interf_bandwidth_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/interface_type.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/interface_type.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/interfaces_filter.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/interfaces_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/internal_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/internal_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ipmi_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ipmi_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ipmi_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ipmi_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ipmi_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ipmi_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,26 +355,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this IPMIEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this IPMIEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this IPMIEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this IPMIEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/item_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/item_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/jdbc_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/jdbc_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/jdbc_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/jdbc_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/jmx_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/jmx_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/jmx_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/jmx_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/linked_wmi_class.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/linked_wmi_class.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/location_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/location_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/log_file.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/log_file.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/log_file_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/log_file_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,26 +357,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this LogFileEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this LogFileEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this LogFileEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this LogFileEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/macro.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/macro.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/map_item_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/map_item_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/match_pattern.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/match_pattern.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/memcached_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/memcached_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/metric.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/metric.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/n_map_ddr.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/n_map_ddr.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/n_map_netscan.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/n_map_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/name_and_value.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/name_and_value.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/nbar_application_names.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/nbar_application_names.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/net_app_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/net_app_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/net_app_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/net_app_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/net_flow_record.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/net_flow_record.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_alert_modules_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_alert_modules_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_application.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_application.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_bandwidth.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_bandwidth.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_bgp_table.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_bgp_table.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_data_base.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_data_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_device_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_device_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_endpoint.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_endpoint.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_filters.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_filters.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_graph_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_group_graph_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_group_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_group_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_group_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_group_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_group_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_nbar_application.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_nbar_application.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_port.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_port.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_qo_s_report_table_row.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_qo_s_report_table_row.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netflow_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netflow_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netscan.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/netscan_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/netscan_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/next_upgrade_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/next_upgrade_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/noc_item_base.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/noc_item_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/noc_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/noc_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/noc_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/noc_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/normal_graph_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/normal_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ntlm_authentication.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ntlm_authentication.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/onetime_upgrade_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/onetime_upgrade_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/open_metric_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/open_metric_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/open_metric_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/open_metric_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_device_group_scope.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_device_group_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_device_scope.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_device_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_group_all_scope.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_group_all_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_scope.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_tag_base.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_tag_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_website_group_scope.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_website_group_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ops_note_website_scope.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ops_note_website_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/overview_graph_data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/overview_graph_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/overview_graph_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/overview_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/paa_s_json_path_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/paa_s_json_path_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/paa_s_mongo_db_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/paa_s_mongo_db_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pdh_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pdh_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/perfmon_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/perfmon_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/perfmon_counter.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/perfmon_counter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/period.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/period.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_item.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/pie_chart_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/pie_chart_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ping_check.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ping_check.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/ping_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/ping_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/point_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/point_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/port_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/port_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/privilege.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/privilege.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,26 +160,26 @@
 
         self._object_id = object_id
 
     @property
     def object_type(self):
         """Gets the object_type of this Privilege.  # noqa: E501
 
-        The privilege object type. The values can be dashboard_group|dashboard|host_group|service_group|website_group|report_group|remoteSession|chat|setting|device_dashboard|help|logs|configNeedDeviceManagePermission|map|resourceMapTab|tracesManageTab|dexda|lmSupportAccess  # noqa: E501
+        The privilege object type. The values can be dashboard_group|dashboard|host_group|service_group|website_group|report_group|remoteSession|chat|setting|device_dashboard|help|logs|configNeedDeviceManagePermission|map|resourceMapTab|tracesManageTab|costOptimization|dexda|lmSupportAccess  # noqa: E501
 
         :return: The object_type of this Privilege.  # noqa: E501
         :rtype: str
         """
         return self._object_type
 
     @object_type.setter
     def object_type(self, object_type):
         """Sets the object_type of this Privilege.
 
-        The privilege object type. The values can be dashboard_group|dashboard|host_group|service_group|website_group|report_group|remoteSession|chat|setting|device_dashboard|help|logs|configNeedDeviceManagePermission|map|resourceMapTab|tracesManageTab|dexda|lmSupportAccess  # noqa: E501
+        The privilege object type. The values can be dashboard_group|dashboard|host_group|service_group|website_group|report_group|remoteSession|chat|setting|device_dashboard|help|logs|configNeedDeviceManagePermission|map|resourceMapTab|tracesManageTab|costOptimization|dexda|lmSupportAccess  # noqa: E501
 
         :param object_type: The object_type of this Privilege.  # noqa: E501
         :type: str
         """
         if object_type is None:
             raise ValueError("Invalid value for `object_type`, must not be `None`")  # noqa: E501
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/property_match_rule.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/property_match_rule.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/property_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/property_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/push_modules_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/push_modules_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rabbit_mq_queue_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rabbit_mq_queue_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/raw_data_values.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/raw_data_values.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/recipient.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/recipient.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/recipient_group.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/recipient_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/recipient_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/recipient_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_base.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_group.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/report_recipient.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/report_recipient.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/resource_group_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/resource_group_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/resource_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/resource_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_applies_to_function_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_applies_to_function_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_aws_account_test_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_account_test_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_aws_health_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_health_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,26 +356,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this RestAwsHealthEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this RestAwsHealthEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this RestAwsHealthEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this RestAwsHealthEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_aws_rds_performance_insights_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_rds_performance_insights_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,26 +366,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this RestAwsRdsPerformanceInsightsEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this RestAwsRdsPerformanceInsightsEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this RestAwsRdsPerformanceInsightsEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this RestAwsRdsPerformanceInsightsEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_aws_trusted_advisor_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_aws_trusted_advisor_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,26 +356,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this RestAwsTrustedAdvisorEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this RestAwsTrustedAdvisorEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this RestAwsTrustedAdvisorEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this RestAwsTrustedAdvisorEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_account_test_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_account_test_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_advisor_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_advisor_event_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,26 +356,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this RestAzureAdvisorEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this RestAzureAdvisorEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this RestAzureAdvisorEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this RestAzureAdvisorEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_resource_health_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_resource_health_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,26 +356,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this RestAzureResourceHealthEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this RestAzureResourceHealthEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this RestAzureResourceHealthEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this RestAzureResourceHealthEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_resource_log_analytics_workspaces_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_resource_log_analytics_workspaces_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,26 +366,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this RestAzureResourceLogAnalyticsWorkspacesSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this RestAzureResourceLogAnalyticsWorkspacesSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this RestAzureResourceLogAnalyticsWorkspacesSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this RestAzureResourceLogAnalyticsWorkspacesSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_subscription_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_subscription_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_azure_subscriptions_discover_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_azure_subscriptions_discover_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_cloud_ok_permissions_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_cloud_ok_permissions_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_dashboard_group_async_clone_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_dashboard_group_async_clone_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_device_instance_group_alert_config_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_device_instance_group_alert_config_v3.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'alert_for_no_data': 'str',
+        'alert_for_no_data': 'int',
         'enable_anomaly_alert_suppression': 'str',
-        'global_alert_for_no_data': 'str',
+        'global_alert_for_no_data': 'int',
         'alert_enable': 'bool',
         'critical_ad_adv_setting': 'str',
-        'alert_clear_transition_interval': 'str',
-        'global_alert_transition_interval': 'str',
+        'alert_clear_transition_interval': 'int',
+        'global_alert_transition_interval': 'int',
         'alert_expr_note': 'str',
         'ad_adv_setting_enabled': 'bool',
         'error_ad_adv_setting': 'str',
         'warn_ad_adv_setting': 'str',
-        'global_alert_clear_transition_interval': 'str',
+        'global_alert_clear_transition_interval': 'int',
         'alert_expr': 'str',
-        'alert_transition_interval': 'str'
+        'alert_transition_interval': 'int'
     }
 
     attribute_map = {
         'alert_for_no_data': 'alertForNoData',
         'enable_anomaly_alert_suppression': 'enableAnomalyAlertSuppression',
         'global_alert_for_no_data': 'globalAlertForNoData',
         'alert_enable': 'alertEnable',
@@ -112,32 +112,30 @@
         if alert_transition_interval is not None:
             self.alert_transition_interval = alert_transition_interval
 
     @property
     def alert_for_no_data(self):
         """Gets the alert_for_no_data of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :return: The alert_for_no_data of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_for_no_data
 
     @alert_for_no_data.setter
     def alert_for_no_data(self, alert_for_no_data):
         """Sets the alert_for_no_data of this RestDeviceInstanceGroupAlertConfigV3.
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :param alert_for_no_data: The alert_for_no_data of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_for_no_data is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_for_no_data):  # noqa: E501
-            raise ValueError("Invalid value for `alert_for_no_data`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_for_no_data = alert_for_no_data
 
     @property
     def enable_anomaly_alert_suppression(self):
         """Gets the enable_anomaly_alert_suppression of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
@@ -158,32 +156,30 @@
 
         self._enable_anomaly_alert_suppression = enable_anomaly_alert_suppression
 
     @property
     def global_alert_for_no_data(self):
         """Gets the global_alert_for_no_data of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :return: The global_alert_for_no_data of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_for_no_data
 
     @global_alert_for_no_data.setter
     def global_alert_for_no_data(self, global_alert_for_no_data):
         """Sets the global_alert_for_no_data of this RestDeviceInstanceGroupAlertConfigV3.
 
-        The triggered alert level if we cannot collect data for this datapoint. The values can be 0-4 (0:unused alert, 1:alert ok, 2:warn alert, 2:error alert, 4:critical alert)  # noqa: E501
+        The triggered alert level if we cannot collect data for this datapoint. The values can be 1-4 (1:no alert, 2:warn alert, 3:error alert, 4:critical alert)  # noqa: E501
 
         :param global_alert_for_no_data: The global_alert_for_no_data of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_for_no_data is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_for_no_data):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_for_no_data`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_for_no_data = global_alert_for_no_data
 
     @property
     def alert_enable(self):
         """Gets the alert_enable of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
@@ -225,57 +221,53 @@
 
         self._critical_ad_adv_setting = critical_ad_adv_setting
 
     @property
     def alert_clear_transition_interval(self):
         """Gets the alert_clear_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
-        The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
+        The count that the alert must exist for this many poll cycles before the alert will be cleared (0-60)  # noqa: E501
 
         :return: The alert_clear_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_clear_transition_interval
 
     @alert_clear_transition_interval.setter
     def alert_clear_transition_interval(self, alert_clear_transition_interval):
         """Sets the alert_clear_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.
 
-        The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
+        The count that the alert must exist for this many poll cycles before the alert will be cleared (0-60)  # noqa: E501
 
         :param alert_clear_transition_interval: The alert_clear_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_clear_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_clear_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `alert_clear_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_clear_transition_interval = alert_clear_transition_interval
 
     @property
     def global_alert_transition_interval(self):
         """Gets the global_alert_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
         The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :return: The global_alert_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_transition_interval
 
     @global_alert_transition_interval.setter
     def global_alert_transition_interval(self, global_alert_transition_interval):
         """Sets the global_alert_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.
 
         The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
 
         :param global_alert_transition_interval: The global_alert_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_transition_interval = global_alert_transition_interval
 
     @property
     def alert_expr_note(self):
         """Gets the alert_expr_note of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
@@ -362,29 +354,27 @@
     @property
     def global_alert_clear_transition_interval(self):
         """Gets the global_alert_clear_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
         The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :return: The global_alert_clear_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._global_alert_clear_transition_interval
 
     @global_alert_clear_transition_interval.setter
     def global_alert_clear_transition_interval(self, global_alert_clear_transition_interval):
         """Sets the global_alert_clear_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.
 
         The count that the alert must exist for this many poll cycles before the alert will be cleared  # noqa: E501
 
         :param global_alert_clear_transition_interval: The global_alert_clear_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if global_alert_clear_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', global_alert_clear_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `global_alert_clear_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._global_alert_clear_transition_interval = global_alert_clear_transition_interval
 
     @property
     def alert_expr(self):
         """Gets the alert_expr of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
@@ -405,32 +395,30 @@
 
         self._alert_expr = alert_expr
 
     @property
     def alert_transition_interval(self):
         """Gets the alert_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
 
-        The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
+        The count that the alert must exist for this many poll cycles before it will be triggered (0-60)  # noqa: E501
 
         :return: The alert_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._alert_transition_interval
 
     @alert_transition_interval.setter
     def alert_transition_interval(self, alert_transition_interval):
         """Sets the alert_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.
 
-        The count that the alert must exist for this many poll cycles before it will be triggered  # noqa: E501
+        The count that the alert must exist for this many poll cycles before it will be triggered (0-60)  # noqa: E501
 
         :param alert_transition_interval: The alert_transition_interval of this RestDeviceInstanceGroupAlertConfigV3.  # noqa: E501
-        :type: str
+        :type: int
         """
-        if alert_transition_interval is not None and not re.search('^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$', alert_transition_interval):  # noqa: E501
-            raise ValueError("Invalid value for `alert_transition_interval`, must be a follow pattern or equal to `/^(?:[A-Za-z0-9+\/]{4})*(?:[A-Za-z0-9+\/]{2}==|[A-Za-z0-9+\/]{3}=)?$/`")  # noqa: E501
 
         self._alert_transition_interval = alert_transition_interval
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_event_source_filter.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_event_source_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_gcp_account_test_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_gcp_account_test_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_highest_priority_collector_status.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_highest_priority_collector_status.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_n_map_netscan_policy_credential.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_n_map_netscan_policy_credential.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_netscan_ports.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_netscan_ports.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_saa_s_account_test_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_saa_s_account_test_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_saved_map_widget_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_saved_map_widget_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_schedule.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_schedule.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/rest_user_customized_data_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/rest_user_customized_data_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/result_item.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/result_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/role.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/role.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/role_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/role_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/role_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/role_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/row_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/row_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_s_slack_health_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_s_slack_health_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_s_webex_license_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_s_webex_license_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_s_zoom_plan_usage_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_s_zoom_plan_usage_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_s_zoom_status_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_s_zoom_status_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saa_so365_share_point_site_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saa_so365_share_point_site_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_account_test_result.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_account_test_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_airbrake_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_airbrake_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_airbrake_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_airbrake_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_o365_skus_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_o365_skus_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_o365_mailbox_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_o365_mailbox_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_o365_service_health_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_o365_service_health_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_csv_report_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_csv_report_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_health_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_health_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_sharepoint_report_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_sharepoint_report_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_skus_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_skus_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_office365_teams_calls_qos_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_office365_teams_calls_qos_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_salesforce_instance_status_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_salesforce_instance_status_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_salesforce_json_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_salesforce_json_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_salesforce_license_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_salesforce_license_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_salesforce_soql_query_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_salesforce_soql_query_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_slack_health_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_slack_health_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_status_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_status_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_status_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_status_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_webex_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_webex_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_zoom_json_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_zoom_json_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_zoom_plan_usage_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_zoom_plan_usage_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/saas_zoom_room_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/saas_zoom_room_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_eri_discovery_attribute_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_eri_discovery_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,26 +386,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this ScriptEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this ScriptEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this ScriptEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this ScriptEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/script_netscan.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/script_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdk_script_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdk_script_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdk_script_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdk_script_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdt.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,21 +74,21 @@
         'end_minute': 'endMinute'
     }
 
     discriminator_value_class_map = {
         'websitecheckpointsdt': 'WebsiteCheckpointSDT',
         'websitesdt': 'WebsiteSDT',
         'devicedatasourceinstancegroupsdt': 'DeviceDataSourceInstanceGroupSDT',
-        '': 'ResourceSDT',
+        'resourcesdt': 'ResourceSDT',
         'deviceclusteralertdefsdt': 'DeviceClusterAlertDefSDT',
         'devicebatchjobsdt': 'DeviceBatchJobSDT',
-        '': 'ResourceGroupSDT',
+        'resourcegroupsdt': 'ResourceGroupSDT',
         'collectorsdt': 'CollectorSDT',
-        '': 'DeviceDataSourceInstanceSDT',
-        '': 'DeviceLogPipeLineResourceSDT',
+        'devicedatasourceinstancesdt': 'DeviceDataSourceInstanceSDT',
+        'devicelogpipelineresourcesdt': 'DeviceLogPipeLineResourceSDT',
         'deviceeventsourcesdt': 'DeviceEventSourceSDT',
         'devicedatasourcesdt': 'DeviceDataSourceSDT',
         'websitegroupsdt': 'WebsiteGroupSDT'
     }
 
     def __init__(self, end_date_time_on_local=None, timezone=None, sdt_type=None, month_day=None, week_of_month=None, admin=None, end_date_time=None, type=None, is_effective=None, minute=None, duration=None, end_hour=None, start_date_time=None, hour=None, start_date_time_on_local=None, week_day=None, comment=None, id=None, end_minute=None):  # noqa: E501
         """SDT - a model defined in Swagger"""  # noqa: E501
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdt_history.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdt_history.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sdt_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sdt_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/service_alert.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/service_alert.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/site_monitor_check_point_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/site_monitor_check_point_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/site_monitor_checkpoint.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/site_monitor_checkpoint.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sla_metric.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sla_metric.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sla_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sla_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/snmp_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/snmp_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/snmp_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/snmp_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/snmp_trap_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/snmp_trap_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,26 +351,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this SnmpTrapEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this SnmpTrapEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this SnmpTrapEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this SnmpTrapEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/snmpilp.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/snmpilp.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/stats_d_graph.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/stats_d_graph.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/stats_d_graph_display.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/stats_d_graph_display.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/stats_d_metric_definition.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/stats_d_metric_definition.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/stats_d_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/stats_d_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/synthetics_selenium_auto_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/synthetics_selenium_auto_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/synthetics_selenium_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/synthetics_selenium_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/sys_log_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/sys_log_event_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,26 +351,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this SysLogEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this SysLogEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this SysLogEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this SysLogEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_column.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_column.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_forecast_configuration.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_forecast_configuration.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_instance_cell.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_instance_cell.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/table_widget_row.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/table_widget_row.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/tcp_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/tcp_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/text_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/text_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/tree_node.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/tree_node.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/udp_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/udp_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/unmonitored_device_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/unmonitored_device_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/unmonitored_devices.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/unmonitored_devices.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/update_reason.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/update_reason.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/usage.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/usage.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/user_filter.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/user_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/user_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/user_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/virtual_data_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/virtual_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/web_check.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/web_check.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/web_check_step.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/web_check_step.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/web_page_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/web_page_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/web_resource.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/web_resource.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_check_point.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_check_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_checkpoint_raw_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_checkpoint_raw_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_checkpoint_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_checkpoint_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_collector_info.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_collector_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_graph_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_group.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_group_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_group_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_group_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_group_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_individuals_status_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_individuals_status_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_item_config.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_item_config.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_location.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_location.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_noc_item.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_noc_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_overall_status_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_overall_status_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_overview_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_overview_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_overview_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_overview_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sdt.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sdt_history_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sdt_history_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sla_report.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sla_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sla_widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sla_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/website_sla_widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/website_sla_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget_data.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget_pagination_response.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget_token.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget_token.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/widget_token_inheritance.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/widget_token_inheritance.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/windows_event_log_event_source.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/windows_event_log_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,26 +351,26 @@
 
         self._lineage_id = lineage_id
 
     @property
     def collector(self):
         """Gets the collector of this WindowsEventLogEventSource.  # noqa: E501
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :return: The collector of this WindowsEventLogEventSource.  # noqa: E501
         :rtype: str
         """
         return self._collector
 
     @collector.setter
     def collector(self, collector):
         """Sets the collector of this WindowsEventLogEventSource.
 
-        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | ipmievent  # noqa: E501
+        The EventSource collector type. The values can be wineventlog | syslog | snmptrap | echo | logfile | scriptevent | awsrss | azurerss | azureadvisor | gcpatom | awsrdspievent | azureresourcehealthevent | azureemergingissue | azureloganalyticsworkspacesevent | awstrustedadvisor | awshealth | awsorganizationalhealth | ipmievent  # noqa: E501
 
         :param collector: The collector of this WindowsEventLogEventSource.  # noqa: E501
         :type: str
         """
 
         self._collector = collector
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/wmi_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/wmi_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/wmi_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/wmi_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/xen_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/xen_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/models/xen_collector_attribute.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/models/xen_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/__init__.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from logicmonitor_sdk.api.lm_api import LMApi
 
 # import ApiClient
 from logicmonitor_sdk.api_client import ApiClient
 from logicmonitor_sdk.configuration import Configuration
 # import models into sdk package
 from logicmonitor_sdk.models.api_token import APIToken
+from logicmonitor_sdk.models.access_group import AccessGroup
+from logicmonitor_sdk.models.access_group_pagination_response import AccessGroupPaginationResponse
 from logicmonitor_sdk.models.access_log_pagination_response import AccessLogPaginationResponse
 from logicmonitor_sdk.models.ack_collector_down import AckCollectorDown
 from logicmonitor_sdk.models.admin import Admin
 from logicmonitor_sdk.models.admin_pagination_response import AdminPaginationResponse
 from logicmonitor_sdk.models.alert import Alert
 from logicmonitor_sdk.models.alert_ack import AlertAck
 from logicmonitor_sdk.models.alert_filters import AlertFilters
@@ -197,14 +199,15 @@
 from logicmonitor_sdk.models.recipient_group import RecipientGroup
 from logicmonitor_sdk.models.recipient_group_pagination_response import RecipientGroupPaginationResponse
 from logicmonitor_sdk.models.report_base import ReportBase
 from logicmonitor_sdk.models.report_group import ReportGroup
 from logicmonitor_sdk.models.report_group_pagination_response import ReportGroupPaginationResponse
 from logicmonitor_sdk.models.report_pagination_response import ReportPaginationResponse
 from logicmonitor_sdk.models.report_recipient import ReportRecipient
+from logicmonitor_sdk.models.resource_data_source_alert_threshold_info import ResourceDataSourceAlertThresholdInfo
 from logicmonitor_sdk.models.rest_applies_to_function_pagination_response import RestAppliesToFunctionPaginationResponse
 from logicmonitor_sdk.models.rest_aws_account_test_v3 import RestAwsAccountTestV3
 from logicmonitor_sdk.models.rest_azure_account_test_v3 import RestAzureAccountTestV3
 from logicmonitor_sdk.models.rest_azure_subscription_v3 import RestAzureSubscriptionV3
 from logicmonitor_sdk.models.rest_azure_subscriptions_discover_v3 import RestAzureSubscriptionsDiscoverV3
 from logicmonitor_sdk.models.rest_cloud_ok_permissions_v3 import RestCloudOkPermissionsV3
 from logicmonitor_sdk.models.rest_dashboard_group_async_clone_response import RestDashboardGroupAsyncCloneResponse
@@ -286,14 +289,16 @@
 from logicmonitor_sdk.models.aws_ec2_reserved_instance_discovery_method import AwsEC2ReservedInstanceDiscoveryMethod
 from logicmonitor_sdk.models.aws_ec2_scheduled_events_collector_attribute import AwsEC2ScheduledEventsCollectorAttribute
 from logicmonitor_sdk.models.aws_ebs_volume_snapshot_collector_attribute_v3 import AwsEbsVolumeSnapshotCollectorAttributeV3
 from logicmonitor_sdk.models.aws_ec2_service_limits_collector_attribute import AwsEc2ServiceLimitsCollectorAttribute
 from logicmonitor_sdk.models.aws_ecs_service_details_collector_attribute import AwsEcsServiceDetailsCollectorAttribute
 from logicmonitor_sdk.models.aws_ecs_service_discovery_method import AwsEcsServiceDiscoveryMethod
 from logicmonitor_sdk.models.aws_elasti_cache_discovery_method import AwsElastiCacheDiscoveryMethod
+from logicmonitor_sdk.models.aws_global_network_device_method import AwsGlobalNetworkDeviceMethod
+from logicmonitor_sdk.models.aws_global_network_link_method import AwsGlobalNetworkLinkMethod
 from logicmonitor_sdk.models.aws_global_web_acl_discovery_method_v3 import AwsGlobalWebACLDiscoveryMethodV3
 from logicmonitor_sdk.models.aws_lb_target_group_discovery_method import AwsLBTargetGroupDiscoveryMethod
 from logicmonitor_sdk.models.aws_media_connect_output_discovery_method import AwsMediaConnectOutputDiscoveryMethod
 from logicmonitor_sdk.models.aws_media_connect_source_discovery_method import AwsMediaConnectSourceDiscoveryMethod
 from logicmonitor_sdk.models.aws_rds_performance_insights_collector_attribute import AwsRdsPerformanceInsightsCollectorAttribute
 from logicmonitor_sdk.models.aws_rds_service_limits_collector_attribute_v3 import AwsRdsServiceLimitsCollectorAttributeV3
 from logicmonitor_sdk.models.aws_red_shift_discovery_method import AwsRedShiftDiscoveryMethod
@@ -346,14 +351,16 @@
 from logicmonitor_sdk.models.azure_redis_cache_discovery_method import AzureRedisCacheDiscoveryMethod
 from logicmonitor_sdk.models.azure_replication_disaster_recovery_collector_attribute import AzureReplicationDisasterRecoveryCollectorAttribute
 from logicmonitor_sdk.models.azure_replication_job_collector_attribute_v3 import AzureReplicationJobCollectorAttributeV3
 from logicmonitor_sdk.models.azure_replication_job_discovery_method import AzureReplicationJobDiscoveryMethod
 from logicmonitor_sdk.models.azure_resource_health_collector_attribute import AzureResourceHealthCollectorAttribute
 from logicmonitor_sdk.models.azure_resource_usage_collector_attribute import AzureResourceUsageCollectorAttribute
 from logicmonitor_sdk.models.azure_rss_event_source import AzureRssEventSource
+from logicmonitor_sdk.models.azure_service_bus_queue import AzureServiceBusQueue
+from logicmonitor_sdk.models.azure_service_bus_topic import AzureServiceBusTopic
 from logicmonitor_sdk.models.azure_service_region_discovery_method import AzureServiceRegionDiscoveryMethod
 from logicmonitor_sdk.models.azure_storage_service_limits_collector_attribute import AzureStorageServiceLimitsCollectorAttribute
 from logicmonitor_sdk.models.azure_subscription_discovery_method import AzureSubscriptionDiscoveryMethod
 from logicmonitor_sdk.models.azure_synapse_discovery_method_v3 import AzureSynapseDiscoveryMethodV3
 from logicmonitor_sdk.models.azure_vm_backup_status_collector_attribute_v3 import AzureVMBackupStatusCollectorAttributeV3
 from logicmonitor_sdk.models.azure_vm_backup_status_log_analytics_collector_attribute import AzureVMBackupStatusLogAnalyticsCollectorAttribute
 from logicmonitor_sdk.models.azure_vm_service_limits_collector_attribute import AzureVMServiceLimitsCollectorAttribute
@@ -481,14 +488,15 @@
 from logicmonitor_sdk.models.ping_collector_attribute import PingCollectorAttribute
 from logicmonitor_sdk.models.port_auto_discovery_method import PortAutoDiscoveryMethod
 from logicmonitor_sdk.models.push_modules_collector_attribute import PushModulesCollectorAttribute
 from logicmonitor_sdk.models.rabbit_mq_queue_auto_discovery_method import RabbitMQQueueAutoDiscoveryMethod
 from logicmonitor_sdk.models.resource_group_sdt import ResourceGroupSDT
 from logicmonitor_sdk.models.resource_sdt import ResourceSDT
 from logicmonitor_sdk.models.rest_aws_health_event_source import RestAwsHealthEventSource
+from logicmonitor_sdk.models.rest_aws_organizational_health_event_source import RestAwsOrganizationalHealthEventSource
 from logicmonitor_sdk.models.rest_aws_rds_performance_insights_event_source import RestAwsRdsPerformanceInsightsEventSource
 from logicmonitor_sdk.models.rest_aws_trusted_advisor_event_source import RestAwsTrustedAdvisorEventSource
 from logicmonitor_sdk.models.rest_azure_advisor_event_source import RestAzureAdvisorEventSource
 from logicmonitor_sdk.models.rest_azure_resource_health_event_source import RestAzureResourceHealthEventSource
 from logicmonitor_sdk.models.rest_azure_resource_log_analytics_workspaces_source import RestAzureResourceLogAnalyticsWorkspacesSource
 from logicmonitor_sdk.models.rest_saved_map_widget_v3 import RestSavedMapWidgetV3
 from logicmonitor_sdk.models.role_report import RoleReport
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/api_client.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         self.default_headers = {}
         # Set default API version
         self.default_headers['X-version'] = '3';
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/3.0.200/python'
+        self.user_agent = 'Swagger-Codegen/3.0.203/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/configuration.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,9 +249,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0.0\n"\
-               "SDK Package Version: 3.0.200".\
+               "SDK Package Version: 3.0.203".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk/rest.py` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk.egg-info/PKG-INFO` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: logicmonitor-sdk
-Version: 3.0.200
+Version: 3.0.203
 Summary: LogicMonitor REST API
 Home-page: https://github.com/logicmonitor/lm-sdk-python
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
 Description:     LogicMonitor is a SaaS-based performance monitoring platform that provides full visibility into complex, hybrid infrastructures, offering granular performance monitoring and actionable data and insights. logicmonitor_sdk enables you to manage your LogicMonitor account programmatically. &lt;br&gt; &lt;br&gt; Note: &lt;ul&gt; &lt;li&gt; For Python SDKs, the REQUEST parameters can contain camelCase or an underscore. &lt;/li&gt; &lt;li&gt; Both underscore and camelCase are supported if parameters are encapsulated within the body. &lt;/li&gt; &lt;li&gt; Only camelCase is supported if parameters are encapsulated within the body and also if the user is passing raw JSON as REQUEST parameter. However, the RESPONSE parameters always contain an underscore. For example, you can use testLocation or test_location in the REQUEST parameter. But the RESPONSE parameter will always be test_location. &lt;/li&gt; &lt;li&gt; The fields parameter only supports camelCase. &lt;/li&gt; &lt;/ul&gt;  # noqa: E501
```

### Comparing `logicmonitor-sdk-3.0.200/logicmonitor_sdk.egg-info/SOURCES.txt` & `logicmonitor-sdk-3.0.203/logicmonitor_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 logicmonitor_sdk.egg-info/SOURCES.txt
 logicmonitor_sdk.egg-info/dependency_links.txt
 logicmonitor_sdk.egg-info/requires.txt
 logicmonitor_sdk.egg-info/top_level.txt
 logicmonitor_sdk/api/__init__.py
 logicmonitor_sdk/api/lm_api.py
 logicmonitor_sdk/models/__init__.py
+logicmonitor_sdk/models/access_group.py
+logicmonitor_sdk/models/access_group_pagination_response.py
 logicmonitor_sdk/models/access_log_pagination_response.py
 logicmonitor_sdk/models/ack_collector_down.py
 logicmonitor_sdk/models/admin.py
 logicmonitor_sdk/models/admin_pagination_response.py
 logicmonitor_sdk/models/aggregate_collector_attribute.py
 logicmonitor_sdk/models/alert.py
 logicmonitor_sdk/models/alert_ack.py
@@ -62,14 +64,16 @@
 logicmonitor_sdk/models/aws_ec2_reserved_instance_discovery_method.py
 logicmonitor_sdk/models/aws_ec2_scheduled_events_collector_attribute.py
 logicmonitor_sdk/models/aws_ec2_service_limits_collector_attribute.py
 logicmonitor_sdk/models/aws_ecs_service_details_collector_attribute.py
 logicmonitor_sdk/models/aws_ecs_service_discovery_method.py
 logicmonitor_sdk/models/aws_elasti_cache_discovery_method.py
 logicmonitor_sdk/models/aws_external_id.py
+logicmonitor_sdk/models/aws_global_network_device_method.py
+logicmonitor_sdk/models/aws_global_network_link_method.py
 logicmonitor_sdk/models/aws_global_web_acl_discovery_method_v3.py
 logicmonitor_sdk/models/aws_lb_target_group_discovery_method.py
 logicmonitor_sdk/models/aws_media_connect_output_discovery_method.py
 logicmonitor_sdk/models/aws_media_connect_source_discovery_method.py
 logicmonitor_sdk/models/aws_rds_performance_insights_collector_attribute.py
 logicmonitor_sdk/models/aws_rds_service_limits_collector_attribute_v3.py
 logicmonitor_sdk/models/aws_red_shift_discovery_method.py
@@ -123,14 +127,16 @@
 logicmonitor_sdk/models/azure_redis_cache_discovery_method.py
 logicmonitor_sdk/models/azure_replication_disaster_recovery_collector_attribute.py
 logicmonitor_sdk/models/azure_replication_job_collector_attribute_v3.py
 logicmonitor_sdk/models/azure_replication_job_discovery_method.py
 logicmonitor_sdk/models/azure_resource_health_collector_attribute.py
 logicmonitor_sdk/models/azure_resource_usage_collector_attribute.py
 logicmonitor_sdk/models/azure_rss_event_source.py
+logicmonitor_sdk/models/azure_service_bus_queue.py
+logicmonitor_sdk/models/azure_service_bus_topic.py
 logicmonitor_sdk/models/azure_service_region_discovery_method.py
 logicmonitor_sdk/models/azure_storage_service_limits_collector_attribute.py
 logicmonitor_sdk/models/azure_subscription_discovery_method.py
 logicmonitor_sdk/models/azure_subscription_id_pagination_response.py
 logicmonitor_sdk/models/azure_synapse_discovery_method_v3.py
 logicmonitor_sdk/models/azure_virtual_desktop_host_pools_collector_attribute_v3.py
 logicmonitor_sdk/models/azure_virtual_desktop_session_hosts_collector_attribute_v3.py
@@ -406,19 +412,21 @@
 logicmonitor_sdk/models/recipient_group.py
 logicmonitor_sdk/models/recipient_group_pagination_response.py
 logicmonitor_sdk/models/report_base.py
 logicmonitor_sdk/models/report_group.py
 logicmonitor_sdk/models/report_group_pagination_response.py
 logicmonitor_sdk/models/report_pagination_response.py
 logicmonitor_sdk/models/report_recipient.py
+logicmonitor_sdk/models/resource_data_source_alert_threshold_info.py
 logicmonitor_sdk/models/resource_group_sdt.py
 logicmonitor_sdk/models/resource_sdt.py
 logicmonitor_sdk/models/rest_applies_to_function_pagination_response.py
 logicmonitor_sdk/models/rest_aws_account_test_v3.py
 logicmonitor_sdk/models/rest_aws_health_event_source.py
+logicmonitor_sdk/models/rest_aws_organizational_health_event_source.py
 logicmonitor_sdk/models/rest_aws_rds_performance_insights_event_source.py
 logicmonitor_sdk/models/rest_aws_trusted_advisor_event_source.py
 logicmonitor_sdk/models/rest_azure_account_test_v3.py
 logicmonitor_sdk/models/rest_azure_advisor_event_source.py
 logicmonitor_sdk/models/rest_azure_resource_health_event_source.py
 logicmonitor_sdk/models/rest_azure_resource_log_analytics_workspaces_source.py
 logicmonitor_sdk/models/rest_azure_subscription_v3.py
@@ -545,14 +553,16 @@
 logicmonitor_sdk/models/widget_token_inheritance.py
 logicmonitor_sdk/models/windows_event_log_event_source.py
 logicmonitor_sdk/models/wmi_auto_discovery_method.py
 logicmonitor_sdk/models/wmi_collector_attribute.py
 logicmonitor_sdk/models/xen_auto_discovery_method.py
 logicmonitor_sdk/models/xen_collector_attribute.py
 test/__init__.py
+test/test_access_group.py
+test/test_access_group_pagination_response.py
 test/test_access_log_pagination_response.py
 test/test_ack_collector_down.py
 test/test_admin.py
 test/test_admin_pagination_response.py
 test/test_aggregate_collector_attribute.py
 test/test_alert.py
 test/test_alert_ack.py
@@ -599,14 +609,16 @@
 test/test_aws_ec2_reserved_instance_discovery_method.py
 test/test_aws_ec2_scheduled_events_collector_attribute.py
 test/test_aws_ec2_service_limits_collector_attribute.py
 test/test_aws_ecs_service_details_collector_attribute.py
 test/test_aws_ecs_service_discovery_method.py
 test/test_aws_elasti_cache_discovery_method.py
 test/test_aws_external_id.py
+test/test_aws_global_network_device_method.py
+test/test_aws_global_network_link_method.py
 test/test_aws_global_web_acl_discovery_method_v3.py
 test/test_aws_lb_target_group_discovery_method.py
 test/test_aws_media_connect_output_discovery_method.py
 test/test_aws_media_connect_source_discovery_method.py
 test/test_aws_rds_performance_insights_collector_attribute.py
 test/test_aws_rds_service_limits_collector_attribute_v3.py
 test/test_aws_red_shift_discovery_method.py
@@ -660,14 +672,16 @@
 test/test_azure_redis_cache_discovery_method.py
 test/test_azure_replication_disaster_recovery_collector_attribute.py
 test/test_azure_replication_job_collector_attribute_v3.py
 test/test_azure_replication_job_discovery_method.py
 test/test_azure_resource_health_collector_attribute.py
 test/test_azure_resource_usage_collector_attribute.py
 test/test_azure_rss_event_source.py
+test/test_azure_service_bus_queue.py
+test/test_azure_service_bus_topic.py
 test/test_azure_service_region_discovery_method.py
 test/test_azure_storage_service_limits_collector_attribute.py
 test/test_azure_subscription_discovery_method.py
 test/test_azure_subscription_id_pagination_response.py
 test/test_azure_synapse_discovery_method_v3.py
 test/test_azure_virtual_desktop_host_pools_collector_attribute_v3.py
 test/test_azure_virtual_desktop_session_hosts_collector_attribute_v3.py
@@ -944,19 +958,21 @@
 test/test_recipient_group.py
 test/test_recipient_group_pagination_response.py
 test/test_report_base.py
 test/test_report_group.py
 test/test_report_group_pagination_response.py
 test/test_report_pagination_response.py
 test/test_report_recipient.py
+test/test_resource_data_source_alert_threshold_info.py
 test/test_resource_group_sdt.py
 test/test_resource_sdt.py
 test/test_rest_applies_to_function_pagination_response.py
 test/test_rest_aws_account_test_v3.py
 test/test_rest_aws_health_event_source.py
+test/test_rest_aws_organizational_health_event_source.py
 test/test_rest_aws_rds_performance_insights_event_source.py
 test/test_rest_aws_trusted_advisor_event_source.py
 test/test_rest_azure_account_test_v3.py
 test/test_rest_azure_advisor_event_source.py
 test/test_rest_azure_resource_health_event_source.py
 test/test_rest_azure_resource_log_analytics_workspaces_source.py
 test/test_rest_azure_subscription_v3.py
```

### Comparing `logicmonitor-sdk-3.0.200/test/test_access_log_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_access_log_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ack_collector_down.py` & `logicmonitor-sdk-3.0.203/test/test_ack_collector_down.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_admin.py` & `logicmonitor-sdk-3.0.203/test/test_admin.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_admin_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_admin_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aggregate_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aggregate_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert.py` & `logicmonitor-sdk-3.0.203/test/test_alert.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_ack.py` & `logicmonitor-sdk-3.0.203/test/test_alert_ack.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_filters.py` & `logicmonitor-sdk-3.0.203/test/test_alert_filters.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_forecasting_report.py` & `logicmonitor-sdk-3.0.203/test/test_alert_forecasting_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_list_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_alert_list_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_alert_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_report.py` & `logicmonitor-sdk-3.0.203/test/test_alert_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_response.py` & `logicmonitor-sdk-3.0.203/test/test_alert_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_rule.py` & `logicmonitor-sdk-3.0.203/test/test_alert_rule.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_rule_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_alert_rule_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_sla_report.py` & `logicmonitor-sdk-3.0.203/test/test_alert_sla_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_threshold_report.py` & `logicmonitor-sdk-3.0.203/test/test_alert_threshold_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_trends_metric.py` & `logicmonitor-sdk-3.0.203/test/test_alert_trends_metric.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_trends_report.py` & `logicmonitor-sdk-3.0.203/test/test_alert_trends_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_widget.py` & `logicmonitor-sdk-3.0.203/test/test_alert_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_alert_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_alert_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_api_perf_metrics.py` & `logicmonitor-sdk-3.0.203/test/test_api_perf_metrics.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_api_token.py` & `logicmonitor-sdk-3.0.203/test/test_api_token.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_api_token_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_api_token_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_applies_to_function.py` & `logicmonitor-sdk-3.0.203/test/test_applies_to_function.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_assignment.py` & `logicmonitor-sdk-3.0.203/test/test_assignment.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_audit_log.py` & `logicmonitor-sdk-3.0.203/test/test_audit_log.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_audit_log_report.py` & `logicmonitor-sdk-3.0.203/test/test_audit_log_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_authentication.py` & `logicmonitor-sdk-3.0.203/test/test_authentication.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_auto_discovery_configuration.py` & `logicmonitor-sdk-3.0.203/test/test_auto_discovery_configuration.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_auto_discovery_filter.py` & `logicmonitor-sdk-3.0.203/test/test_auto_discovery_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_automatic_upgrade_info.py` & `logicmonitor-sdk-3.0.203/test/test_automatic_upgrade_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_account_id.py` & `logicmonitor-sdk-3.0.203/test/test_aws_account_id.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_account_test_result.py` & `logicmonitor-sdk-3.0.203/test/test_aws_account_test_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_api_gateway_stage_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_api_gateway_stage_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_auto_scaling_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_auto_scaling_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_billing_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_billing_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_billing_report_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_billing_report_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_billing_report_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_billing_report_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_classic_elb_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_classic_elb_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_cloud_watch_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_cloud_watch_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_cognito_identity_providers_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_aws_cognito_identity_providers_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ebs_volume_snapshot_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ebs_volume_snapshot_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ec2_reserved_instance_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ec2_reserved_instance_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ec2_reserved_instance_coverage_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ec2_reserved_instance_coverage_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ec2_reserved_instance_coverage_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ec2_reserved_instance_coverage_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ec2_reserved_instance_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ec2_reserved_instance_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ec2_scheduled_events_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ec2_scheduled_events_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ec2_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ec2_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ecs_service_details_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ecs_service_details_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ecs_service_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ecs_service_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_elasti_cache_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_elasti_cache_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_external_id.py` & `logicmonitor-sdk-3.0.203/test/test_aws_external_id.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_global_web_acl_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_aws_global_web_acl_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_lb_target_group_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_lb_target_group_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_media_connect_output_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_media_connect_output_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_media_connect_source_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_media_connect_source_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_rds_performance_insights_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_rds_performance_insights_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_rds_service_limits_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_aws_rds_service_limits_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_red_shift_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_red_shift_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_route53_resolver_ip_address_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_route53_resolver_ip_address_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_route53_resolver_ip_address_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_route53_resolver_ip_address_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_rss_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_aws_rss_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_sage_maker_endpoint_variant_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_sage_maker_endpoint_variant_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_service_limits_from_trusted_advisor_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_service_limits_from_trusted_advisor_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_service_region_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_service_region_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_ses_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_aws_ses_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_vpn_tunnel_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_aws_vpn_tunnel_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_aws_web_acl_waf_v2_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_aws_web_acl_waf_v2_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_account_test_result.py` & `logicmonitor-sdk-3.0.203/test/test_azure_account_test_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_active_directory_app_secret_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_active_directory_app_secret_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_active_directory_app_secret_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_active_directory_app_secret_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_active_directory_sync_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_active_directory_sync_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_active_directory_users_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_active_directory_users_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_app_service_environment_multi_role_pool_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_app_service_environment_multi_role_pool_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_app_service_environment_multi_role_pool_discover_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_app_service_environment_multi_role_pool_discover_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_authentication_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_authentication_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_automation_account_certificate_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_automation_account_certificate_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_automation_account_certificate_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_automation_account_certificate_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_backup_job_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_backup_job_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_backup_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_backup_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_backup_protected_item_backup_job_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_backup_protected_item_backup_job_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_backup_protected_item_backup_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_backup_protected_item_backup_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_backup_protected_item_health_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_backup_protected_item_health_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_billing_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_billing_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_billing_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_billing_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_cost_management_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_cost_management_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_cost_management_dimensions_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_cost_management_dimensions_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_cost_management_subscriptions_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_cost_management_subscriptions_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_cost_management_tags_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_cost_management_tags_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_dimension_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_dimension_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_ea_billing_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_ea_billing_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_ea_billing_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_ea_billing_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_emerging_issue_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_azure_emerging_issue_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_express_route_circuit_peering_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_express_route_circuit_peering_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_express_route_circuit_peering_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_express_route_circuit_peering_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_insights_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_insights_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_log_analytics_replication_job_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_log_analytics_replication_job_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_log_analytics_replication_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_log_analytics_replication_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_log_analytics_workspaces_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_log_analytics_workspaces_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_log_analytics_workspaces_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_log_analytics_workspaces_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_net_app_volumes_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_net_app_volumes_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_network_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_network_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_recovery_service_rto_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_recovery_service_rto_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_recovery_service_rto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_recovery_service_rto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_recovery_service_vault_sr_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_recovery_service_vault_sr_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_recovery_services_vault_agents_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_recovery_services_vault_agents_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_redis_cache_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_redis_cache_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_replication_disaster_recovery_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_replication_disaster_recovery_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_replication_job_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_replication_job_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_replication_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_replication_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_resource_health_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_resource_health_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_resource_usage_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_resource_usage_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_rss_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_azure_rss_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_service_region_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_service_region_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_storage_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_storage_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_subscription_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_subscription_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_subscription_id_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_azure_subscription_id_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_synapse_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_synapse_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_virtual_desktop_host_pools_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_virtual_desktop_host_pools_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_virtual_desktop_session_hosts_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_virtual_desktop_session_hosts_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_virtual_desktop_session_hosts_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_virtual_desktop_session_hosts_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_vm_backup_status_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_vm_backup_status_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_vm_backup_status_log_analytics_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_vm_backup_status_log_analytics_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_vm_service_limits_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_vm_service_limits_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_vng_connection_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_vng_connection_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_vng_connection_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_vng_connection_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_vwan_vpn_connection_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_azure_vwan_vpn_connection_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_vwan_vpn_connection_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_vwan_vpn_connection_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_web_app_instance_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_web_app_instance_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_web_job_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_azure_web_job_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_azure_web_job_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_azure_web_job_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_basic_authentication.py` & `logicmonitor-sdk-3.0.203/test/test_basic_authentication.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_batch_job_execution_item.py` & `logicmonitor-sdk-3.0.203/test/test_batch_job_execution_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_batch_job_widget.py` & `logicmonitor-sdk-3.0.203/test/test_batch_job_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_batch_job_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_batch_job_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_batch_script_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_batch_script_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_big_number_data.py` & `logicmonitor-sdk-3.0.203/test/test_big_number_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_big_number_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_big_number_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_big_number_info.py` & `logicmonitor-sdk-3.0.203/test/test_big_number_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_big_number_item.py` & `logicmonitor-sdk-3.0.203/test/test_big_number_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_big_number_widget.py` & `logicmonitor-sdk-3.0.203/test/test_big_number_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_big_number_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_big_number_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_cell_data.py` & `logicmonitor-sdk-3.0.203/test/test_cell_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_chain.py` & `logicmonitor-sdk-3.0.203/test/test_chain.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_cim_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_cim_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_cim_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_cim_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_cloud_watch_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_cloud_watch_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector.py` & `logicmonitor-sdk-3.0.203/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_collector_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_base.py` & `logicmonitor-sdk-3.0.203/test/test_collector_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_group.py` & `logicmonitor-sdk-3.0.203/test/test_collector_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_collector_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_collector_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_collector_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_version.py` & `logicmonitor-sdk-3.0.203/test/test_collector_version.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_collector_version_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_collector_version_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_color_threshold.py` & `logicmonitor-sdk-3.0.203/test/test_color_threshold.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_column_header.py` & `logicmonitor-sdk-3.0.203/test/test_column_header.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_config_source_update_reasons_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_config_source_update_reasons_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_conversation_filter.py` & `logicmonitor-sdk-3.0.203/test/test_conversation_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_counter.py` & `logicmonitor-sdk-3.0.203/test/test_counter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_custom_flexible_virtual_data_source_ex.py` & `logicmonitor-sdk-3.0.203/test/test_custom_flexible_virtual_data_source_ex.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_custom_graph.py` & `logicmonitor-sdk-3.0.203/test/test_custom_graph.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_custom_graph_widget.py` & `logicmonitor-sdk-3.0.203/test/test_custom_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_custom_report.py` & `logicmonitor-sdk-3.0.203/test/test_custom_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_custom_virtual_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_custom_virtual_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dashboard.py` & `logicmonitor-sdk-3.0.203/test/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dashboard_data.py` & `logicmonitor-sdk-3.0.203/test/test_dashboard_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dashboard_group.py` & `logicmonitor-sdk-3.0.203/test/test_dashboard_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dashboard_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_dashboard_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dashboard_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_dashboard_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dashboard_report.py` & `logicmonitor-sdk-3.0.203/test/test_dashboard_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_data_pump_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_data_pump_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_data_source.py` & `logicmonitor-sdk-3.0.203/test/test_data_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_data_source_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_data_source_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_data_source_overview_graph.py` & `logicmonitor-sdk-3.0.203/test/test_data_source_overview_graph.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_data_source_update_reasons_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_data_source_update_reasons_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_datasource_overview_graph_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_datasource_overview_graph_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_datasource_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_datasource_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_days_until_alert.py` & `logicmonitor-sdk-3.0.203/test/test_days_until_alert.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_debug.py` & `logicmonitor-sdk-3.0.203/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device.py` & `logicmonitor-sdk-3.0.203/test/test_device.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_batch_job_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_device_batch_job_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_cluster_alert_def_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_device_cluster_alert_def_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_associated.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_associated.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_associated_instance.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_associated_instance.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_associated_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_associated_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_data.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_alert_setting.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_alert_setting.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_alert_setting_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_alert_setting_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_config.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_config.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_config_alert.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_config_alert.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_config_diff.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_config_diff.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_data.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_group.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_group_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_group_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_instance_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_instance_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_data_source_sdt_history_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_data_source_sdt_history_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_datasource_graph.py` & `logicmonitor-sdk-3.0.203/test/test_device_datasource_graph.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_datasource_instance_config_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_datasource_instance_config_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_datasource_instance_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_datasource_instance_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_datasource_instance_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_datasource_instance_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_datasource_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_datasource_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_delta_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_delta_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_event_source_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_device_event_source_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_filter.py` & `logicmonitor-sdk-3.0.203/test/test_device_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group.py` & `logicmonitor-sdk-3.0.203/test/test_device_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group_alert_threshold_info.py` & `logicmonitor-sdk-3.0.203/test/test_device_group_alert_threshold_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group_data.py` & `logicmonitor-sdk-3.0.203/test/test_device_group_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group_data_source.py` & `logicmonitor-sdk-3.0.203/test/test_device_group_data_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group_data_source_alert_config.py` & `logicmonitor-sdk-3.0.203/test/test_device_group_data_source_alert_config.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group_data_source_data_point_config.py` & `logicmonitor-sdk-3.0.203/test/test_device_group_data_source_data_point_config.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group_datasource_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_group_datasource_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_group_sdt_history_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_group_sdt_history_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_instance_data.py` & `logicmonitor-sdk-3.0.203/test/test_device_instance_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_instance_data_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_instance_data_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_instances.py` & `logicmonitor-sdk-3.0.203/test/test_device_instances.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_log_pipe_line_resource_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_device_log_pipe_line_resource_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_noc_item.py` & `logicmonitor-sdk-3.0.203/test/test_device_noc_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_property.py` & `logicmonitor-sdk-3.0.203/test/test_device_property.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_sdt_history_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_device_sdt_history_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_sla_widget.py` & `logicmonitor-sdk-3.0.203/test/test_device_sla_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_sla_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_device_sla_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_device_status.py` & `logicmonitor-sdk-3.0.203/test/test_device_status.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dns_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_dns_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dummy_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_dummy_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dynamic_column.py` & `logicmonitor-sdk-3.0.203/test/test_dynamic_column.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dynamic_table_widget.py` & `logicmonitor-sdk-3.0.203/test/test_dynamic_table_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dynamic_table_widget_column.py` & `logicmonitor-sdk-3.0.203/test/test_dynamic_table_widget_column.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dynamic_table_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_dynamic_table_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_dynamic_table_widget_row.py` & `logicmonitor-sdk-3.0.203/test/test_dynamic_table_widget_row.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ec2_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_ec2_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ec2_ddr.py` & `logicmonitor-sdk-3.0.203/test/test_ec2_ddr.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ec2_netscan.py` & `logicmonitor-sdk-3.0.203/test/test_ec2_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ec2_netscan_policy_credential.py` & `logicmonitor-sdk-3.0.203/test/test_ec2_netscan_policy_credential.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ec2_scheduled_event_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_ec2_scheduled_event_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_echo_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_echo_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_enhanced_script_netscan.py` & `logicmonitor-sdk-3.0.203/test/test_enhanced_script_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_entity_property.py` & `logicmonitor-sdk-3.0.203/test/test_entity_property.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_error_response.py` & `logicmonitor-sdk-3.0.203/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_escalating_chain.py` & `logicmonitor-sdk-3.0.203/test/test_escalating_chain.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_escalation_chain_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_escalation_chain_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_esx_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_esx_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_esx_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_esx_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_event_source_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_event_source_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_exclude_duplicate_ips.py` & `logicmonitor-sdk-3.0.203/test/test_exclude_duplicate_ips.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_flash_widget.py` & `logicmonitor-sdk-3.0.203/test/test_flash_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_flow_record_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_flow_record_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gauge_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_gauge_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gauge_widget.py` & `logicmonitor-sdk-3.0.203/test/test_gauge_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gauge_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_gauge_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_account_test_result.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_account_test_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_app_engine_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_app_engine_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_atom_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_atom_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_backend_service_health_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_backend_service_health_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_billing_big_query_source_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_billing_big_query_source_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_billing_big_query_source_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_billing_big_query_source_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_billing_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_billing_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_billing_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_billing_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_compute_service_limits_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_compute_service_limits_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_lb_backend_service_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_lb_backend_service_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_pub_sub_snapshot_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_pub_sub_snapshot_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_pub_sub_subscription_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_pub_sub_subscription_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_stack_driver_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_stack_driver_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_gcp_vpn_tunnel_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_gcp_vpn_tunnel_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_generate_report_request.py` & `logicmonitor-sdk-3.0.203/test/test_generate_report_request.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_generate_report_result.py` & `logicmonitor-sdk-3.0.203/test/test_generate_report_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_glob_match_toggle.py` & `logicmonitor-sdk-3.0.203/test/test_glob_match_toggle.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_google_map_widget.py` & `logicmonitor-sdk-3.0.203/test/test_google_map_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_google_map_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_google_map_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_graph_display.py` & `logicmonitor-sdk-3.0.203/test/test_graph_display.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_graph_line.py` & `logicmonitor-sdk-3.0.203/test/test_graph_line.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_graph_ops_note_scope.py` & `logicmonitor-sdk-3.0.203/test/test_graph_ops_note_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_graph_plot.py` & `logicmonitor-sdk-3.0.203/test/test_graph_plot.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_graph_plot_line.py` & `logicmonitor-sdk-3.0.203/test/test_graph_plot_line.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_graph_virtual_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_graph_virtual_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_group_net_flow_record.py` & `logicmonitor-sdk-3.0.203/test/test_group_net_flow_record.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_host_cpu_report.py` & `logicmonitor-sdk-3.0.203/test/test_host_cpu_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_host_group_inventory_report.py` & `logicmonitor-sdk-3.0.203/test/test_host_group_inventory_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_host_inventory_metric.py` & `logicmonitor-sdk-3.0.203/test/test_host_inventory_metric.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_host_inventory_report.py` & `logicmonitor-sdk-3.0.203/test/test_host_inventory_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_host_metrics_report.py` & `logicmonitor-sdk-3.0.203/test/test_host_metrics_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_html_widget.py` & `logicmonitor-sdk-3.0.203/test/test_html_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_http_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_http_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ilp.py` & `logicmonitor-sdk-3.0.203/test/test_ilp.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_inheritance_prop.py` & `logicmonitor-sdk-3.0.203/test/test_inheritance_prop.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_instance_group_alert_threshold_info.py` & `logicmonitor-sdk-3.0.203/test/test_instance_group_alert_threshold_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_integration_audit_log.py` & `logicmonitor-sdk-3.0.203/test/test_integration_audit_log.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_role.py` & `logicmonitor-sdk-3.0.203/test/test_role.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_integration_audit_log_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_integration_audit_log_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_integration_metadata.py` & `logicmonitor-sdk-3.0.203/test/test_integration_metadata.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_interf_bandwidth_report.py` & `logicmonitor-sdk-3.0.203/test/test_interf_bandwidth_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_interface_type.py` & `logicmonitor-sdk-3.0.203/test/test_interface_type.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_interfaces_filter.py` & `logicmonitor-sdk-3.0.203/test/test_interfaces_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_internal_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_internal_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ipmi_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_ipmi_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ipmi_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_ipmi_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ipmi_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_ipmi_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_item_data.py` & `logicmonitor-sdk-3.0.203/test/test_item_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_jdbc_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_jdbc_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_jdbc_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_jdbc_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_jmx_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_jmx_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_jmx_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_jmx_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_linked_wmi_class.py` & `logicmonitor-sdk-3.0.203/test/test_linked_wmi_class.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_lm_api.py` & `logicmonitor-sdk-3.0.203/test/test_lm_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,21 @@
     def test_ack_collector_down_alert_by_id(self):
         """Test case for ack_collector_down_alert_by_id
 
         ack collector down alert  # noqa: E501
         """
         pass
 
+    def test_add_access_group(self):
+        """Test case for add_access_group
+
+        Create a access group  # noqa: E501
+        """
+        pass
+
     def test_add_admin(self):
         """Test case for add_admin
 
         add user  # noqa: E501
         """
         pass
 
@@ -242,14 +249,21 @@
     def test_collect_device_config_source_config(self):
         """Test case for collect_device_config_source_config
 
         collect a config for a device  # noqa: E501
         """
         pass
 
+    def test_delete_access_group(self):
+        """Test case for delete_access_group
+
+        Delete access group  # noqa: E501
+        """
+        pass
+
     def test_delete_admin_by_id(self):
         """Test case for delete_admin_by_id
 
         delete user  # noqa: E501
         """
         pass
 
@@ -382,14 +396,21 @@
     def test_discover_subscriptions(self):
         """Test case for discover_subscriptions
 
         view subscriptions  # noqa: E501
         """
         pass
 
+    def test_escalated_alert_by_id(self):
+        """Test case for escalated_alert_by_id
+
+        escalate alert by id  # noqa: E501
+        """
+        pass
+
     def test_execute_debug_command(self):
         """Test case for execute_debug_command
 
         Execute a Collector debug command  # noqa: E501
         """
         pass
 
@@ -410,14 +431,28 @@
     def test_generate_report_by_id(self):
         """Test case for generate_report_by_id
 
         run a report  # noqa: E501
         """
         pass
 
+    def test_get_access_group_by_id(self):
+        """Test case for get_access_group_by_id
+
+        Get access group by id  # noqa: E501
+        """
+        pass
+
+    def test_get_access_group_list(self):
+        """Test case for get_access_group_list
+
+        Get access group list  # noqa: E501
+        """
+        pass
+
     def test_get_admin_by_id(self):
         """Test case for get_admin_by_id
 
         get user  # noqa: E501
         """
         pass
 
@@ -704,14 +739,21 @@
     def test_get_device_datasource_instance_graph_data(self):
         """Test case for get_device_datasource_instance_graph_data
 
         get device instance graph data   # noqa: E501
         """
         pass
 
+    def test_get_device_datasource_instance_group_by_id(self):
+        """Test case for get_device_datasource_instance_group_by_id
+
+        get device datasource instance group   # noqa: E501
+        """
+        pass
+
     def test_get_device_datasource_instance_group_list(self):
         """Test case for get_device_datasource_instance_group_list
 
         get device datasource instance group list   # noqa: E501
         """
         pass
 
@@ -1145,14 +1187,21 @@
     def test_get_widget_list_by_dashboard_id(self):
         """Test case for get_widget_list_by_dashboard_id
 
         get widget list by DashboardId  # noqa: E501
         """
         pass
 
+    def test_patch_access_group(self):
+        """Test case for patch_access_group
+
+        Update access group  # noqa: E501
+        """
+        pass
+
     def test_patch_admin_by_id(self):
         """Test case for patch_admin_by_id
 
         update user  # noqa: E501
         """
         pass
 
@@ -1278,21 +1327,14 @@
     def test_patch_escalation_chain_by_id(self):
         """Test case for patch_escalation_chain_by_id
 
         update escalation chain  # noqa: E501
         """
         pass
 
-    def test_patch_instances_alert_threshold(self):
-        """Test case for patch_instances_alert_threshold
-
-        update instances alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
-        """
-        pass
-
     def test_patch_recipient_group_by_id(self):
         """Test case for patch_recipient_group_by_id
 
         update recipient group  # noqa: E501
         """
         pass
 
@@ -1376,14 +1418,21 @@
     def test_test_saa_s_account(self):
         """Test case for test_saa_s_account
 
         test SaaS account  # noqa: E501
         """
         pass
 
+    def test_update_access_group(self):
+        """Test case for update_access_group
+
+        Update access group  # noqa: E501
+        """
+        pass
+
     def test_update_admin_by_id(self):
         """Test case for update_admin_by_id
 
         update user  # noqa: E501
         """
         pass
 
@@ -1509,18 +1558,18 @@
     def test_update_escalation_chain_by_id(self):
         """Test case for update_escalation_chain_by_id
 
         update escalation chain  # noqa: E501
         """
         pass
 
-    def test_update_instances_alert_threshold(self):
-        """Test case for update_instances_alert_threshold
+    def test_update_instance_group_alert_threshold(self):
+        """Test case for update_instance_group_alert_threshold
 
-        update instances alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
+        update instance group alert threshold (Setting the threshold at default group is not allowed)  # noqa: E501
         """
         pass
 
     def test_update_recipient_group_by_id(self):
         """Test case for update_recipient_group_by_id
 
         update recipient group  # noqa: E501
```

### Comparing `logicmonitor-sdk-3.0.200/test/test_location_data.py` & `logicmonitor-sdk-3.0.203/test/test_location_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_log_file.py` & `logicmonitor-sdk-3.0.203/test/test_log_file.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_log_file_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_log_file_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_macro.py` & `logicmonitor-sdk-3.0.203/test/test_macro.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_map_item_info.py` & `logicmonitor-sdk-3.0.203/test/test_map_item_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_match_pattern.py` & `logicmonitor-sdk-3.0.203/test/test_match_pattern.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_memcached_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_memcached_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_metric.py` & `logicmonitor-sdk-3.0.203/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_n_map_ddr.py` & `logicmonitor-sdk-3.0.203/test/test_n_map_ddr.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_n_map_netscan.py` & `logicmonitor-sdk-3.0.203/test/test_n_map_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_name_and_value.py` & `logicmonitor-sdk-3.0.203/test/test_name_and_value.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_nbar_application_names.py` & `logicmonitor-sdk-3.0.203/test/test_nbar_application_names.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_net_app_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_net_app_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_net_app_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_net_app_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_net_flow_record.py` & `logicmonitor-sdk-3.0.203/test/test_net_flow_record.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_alert_modules_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_alert_modules_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_application.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_application.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_bandwidth.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_bandwidth.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_bgp_table.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_bgp_table.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_data_base.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_data_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_device_info.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_device_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_endpoint.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_endpoint.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_filters.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_filters.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_graph_widget.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_group_graph_widget.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_group_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_group_widget.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_group_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_group_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_group_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_nbar_application.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_nbar_application.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_port.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_port.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_qo_s_report_table_row.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_qo_s_report_table_row.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_report.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_widget.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netflow_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_netflow_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netscan.py` & `logicmonitor-sdk-3.0.203/test/test_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_netscan_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_netscan_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_next_upgrade_info.py` & `logicmonitor-sdk-3.0.203/test/test_next_upgrade_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_noc_item_base.py` & `logicmonitor-sdk-3.0.203/test/test_noc_item_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_noc_widget.py` & `logicmonitor-sdk-3.0.203/test/test_noc_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_noc_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_noc_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_normal_graph_widget.py` & `logicmonitor-sdk-3.0.203/test/test_normal_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ntlm_authentication.py` & `logicmonitor-sdk-3.0.203/test/test_ntlm_authentication.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_onetime_upgrade_info.py` & `logicmonitor-sdk-3.0.203/test/test_onetime_upgrade_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_open_metric_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_open_metric_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_open_metric_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_open_metric_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note_device_group_scope.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note_device_group_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note_device_scope.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note_device_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note_group_all_scope.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note_group_all_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note_scope.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note_tag_base.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note_tag_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note_website_group_scope.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note_website_group_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ops_note_website_scope.py` & `logicmonitor-sdk-3.0.203/test/test_ops_note_website_scope.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_overview_graph_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_overview_graph_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_overview_graph_widget.py` & `logicmonitor-sdk-3.0.203/test/test_overview_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_paa_s_json_path_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_paa_s_json_path_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_paa_s_mongo_db_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_paa_s_mongo_db_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_pdh_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_pdh_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_perfmon_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_perfmon_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_perfmon_counter.py` & `logicmonitor-sdk-3.0.203/test/test_perfmon_counter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_period.py` & `logicmonitor-sdk-3.0.203/test/test_period.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_pie_chart_data.py` & `logicmonitor-sdk-3.0.203/test/test_pie_chart_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_pie_chart_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_pie_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_pie_chart_info.py` & `logicmonitor-sdk-3.0.203/test/test_pie_chart_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_pie_chart_item.py` & `logicmonitor-sdk-3.0.203/test/test_pie_chart_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_pie_chart_widget.py` & `logicmonitor-sdk-3.0.203/test/test_pie_chart_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_pie_chart_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_pie_chart_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ping_check.py` & `logicmonitor-sdk-3.0.203/test/test_ping_check.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_ping_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_ping_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_point_source.py` & `logicmonitor-sdk-3.0.203/test/test_point_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_port_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_port_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_privilege.py` & `logicmonitor-sdk-3.0.203/test/test_privilege.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_property_match_rule.py` & `logicmonitor-sdk-3.0.203/test/test_property_match_rule.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_property_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_property_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_push_modules_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_push_modules_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rabbit_mq_queue_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_rabbit_mq_queue_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_raw_data_values.py` & `logicmonitor-sdk-3.0.203/test/test_raw_data_values.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_recipient.py` & `logicmonitor-sdk-3.0.203/test/test_recipient.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_recipient_group.py` & `logicmonitor-sdk-3.0.203/test/test_recipient_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_recipient_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_recipient_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_report_base.py` & `logicmonitor-sdk-3.0.203/test/test_report_base.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_report_group.py` & `logicmonitor-sdk-3.0.203/test/test_report_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_report_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_report_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_report_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_report_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_report_recipient.py` & `logicmonitor-sdk-3.0.203/test/test_report_recipient.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_resource_group_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_resource_group_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_resource_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_resource_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_applies_to_function_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_rest_applies_to_function_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_aws_account_test_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_aws_account_test_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_aws_health_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_rest_aws_health_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_aws_rds_performance_insights_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_rest_aws_rds_performance_insights_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_aws_trusted_advisor_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_rest_aws_trusted_advisor_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_azure_account_test_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_azure_account_test_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_azure_advisor_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_rest_azure_advisor_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_azure_resource_health_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_rest_azure_resource_health_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_azure_resource_log_analytics_workspaces_source.py` & `logicmonitor-sdk-3.0.203/test/test_rest_azure_resource_log_analytics_workspaces_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_azure_subscription_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_azure_subscription_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_azure_subscriptions_discover_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_azure_subscriptions_discover_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_cloud_ok_permissions_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_cloud_ok_permissions_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_dashboard_group_async_clone_response.py` & `logicmonitor-sdk-3.0.203/test/test_rest_dashboard_group_async_clone_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_device_instance_group_alert_config_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_device_instance_group_alert_config_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_event_source_filter.py` & `logicmonitor-sdk-3.0.203/test/test_rest_event_source_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_gcp_account_test_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_gcp_account_test_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_highest_priority_collector_status.py` & `logicmonitor-sdk-3.0.203/test/test_rest_highest_priority_collector_status.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_n_map_netscan_policy_credential.py` & `logicmonitor-sdk-3.0.203/test/test_rest_n_map_netscan_policy_credential.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_netscan_ports.py` & `logicmonitor-sdk-3.0.203/test/test_rest_netscan_ports.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_saa_s_account_test_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_saa_s_account_test_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_saved_map_widget_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_saved_map_widget_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_schedule.py` & `logicmonitor-sdk-3.0.203/test/test_rest_schedule.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_rest_user_customized_data_v3.py` & `logicmonitor-sdk-3.0.203/test/test_rest_user_customized_data_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_result_item.py` & `logicmonitor-sdk-3.0.203/test/test_result_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_role_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_role_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_role_report.py` & `logicmonitor-sdk-3.0.203/test/test_role_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_row_data.py` & `logicmonitor-sdk-3.0.203/test/test_row_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saa_s_slack_health_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saa_s_slack_health_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saa_s_webex_license_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saa_s_webex_license_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saa_s_zoom_plan_usage_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saa_s_zoom_plan_usage_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saa_s_zoom_status_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saa_s_zoom_status_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saa_so365_share_point_site_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saa_so365_share_point_site_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_account_test_result.py` & `logicmonitor-sdk-3.0.203/test/test_saas_account_test_result.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_airbrake_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_saas_airbrake_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_airbrake_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saas_airbrake_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_o365_mailbox_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saas_o365_mailbox_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_o365_service_health_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saas_o365_service_health_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_o365_skus_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saas_o365_skus_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_office365_csv_report_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_office365_csv_report_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_office365_health_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_office365_health_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_office365_sharepoint_report_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_office365_sharepoint_report_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_office365_skus_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_saas_office365_skus_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_office365_teams_calls_qos_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_office365_teams_calls_qos_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_salesforce_instance_status_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_salesforce_instance_status_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_salesforce_json_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_salesforce_json_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_salesforce_license_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saas_salesforce_license_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_salesforce_soql_query_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_salesforce_soql_query_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_slack_health_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_saas_slack_health_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_status_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_saas_status_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_status_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saas_status_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_webex_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_saas_webex_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_zoom_json_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_zoom_json_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_zoom_plan_usage_collector_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_saas_zoom_plan_usage_collector_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_saas_zoom_room_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_saas_zoom_room_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_script_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_script_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_script_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_script_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_script_eri_discovery_attribute_v3.py` & `logicmonitor-sdk-3.0.203/test/test_script_eri_discovery_attribute_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_script_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_script_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_script_netscan.py` & `logicmonitor-sdk-3.0.203/test/test_script_netscan.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_sdk_script_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_sdk_script_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_sdk_script_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_sdk_script_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_sdt_history.py` & `logicmonitor-sdk-3.0.203/test/test_sdt_history.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_sdt_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_sdt_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_service_alert.py` & `logicmonitor-sdk-3.0.203/test/test_service_alert.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_site_monitor_check_point_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_site_monitor_check_point_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_site_monitor_checkpoint.py` & `logicmonitor-sdk-3.0.203/test/test_site_monitor_checkpoint.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_sla_metric.py` & `logicmonitor-sdk-3.0.203/test/test_sla_metric.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_sla_report.py` & `logicmonitor-sdk-3.0.203/test/test_sla_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_snmp_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_snmp_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_snmp_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_snmp_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_snmp_trap_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_snmp_trap_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_snmpilp.py` & `logicmonitor-sdk-3.0.203/test/test_snmpilp.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_stats_d_graph.py` & `logicmonitor-sdk-3.0.203/test/test_stats_d_graph.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_stats_d_graph_display.py` & `logicmonitor-sdk-3.0.203/test/test_stats_d_graph_display.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_stats_d_metric_definition.py` & `logicmonitor-sdk-3.0.203/test/test_stats_d_metric_definition.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_stats_d_widget.py` & `logicmonitor-sdk-3.0.203/test/test_stats_d_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_synthetics_selenium_auto_discovery_method_v3.py` & `logicmonitor-sdk-3.0.203/test/test_synthetics_selenium_auto_discovery_method_v3.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_synthetics_selenium_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_synthetics_selenium_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_sys_log_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_sys_log_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_table_widget.py` & `logicmonitor-sdk-3.0.203/test/test_table_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_table_widget_column.py` & `logicmonitor-sdk-3.0.203/test/test_table_widget_column.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_table_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_table_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_table_widget_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_table_widget_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_table_widget_forecast_configuration.py` & `logicmonitor-sdk-3.0.203/test/test_table_widget_forecast_configuration.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_table_widget_instance_cell.py` & `logicmonitor-sdk-3.0.203/test/test_table_widget_instance_cell.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_table_widget_row.py` & `logicmonitor-sdk-3.0.203/test/test_table_widget_row.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_tcp_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_tcp_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_text_widget.py` & `logicmonitor-sdk-3.0.203/test/test_text_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_tree_node.py` & `logicmonitor-sdk-3.0.203/test/test_tree_node.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_udp_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_udp_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_unmonitored_device_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_unmonitored_device_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_unmonitored_devices.py` & `logicmonitor-sdk-3.0.203/test/test_unmonitored_devices.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_update_reason.py` & `logicmonitor-sdk-3.0.203/test/test_update_reason.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_usage.py` & `logicmonitor-sdk-3.0.203/test/test_usage.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_user_filter.py` & `logicmonitor-sdk-3.0.203/test/test_user_filter.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_user_report.py` & `logicmonitor-sdk-3.0.203/test/test_user_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_virtual_data_point.py` & `logicmonitor-sdk-3.0.203/test/test_virtual_data_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_web_check.py` & `logicmonitor-sdk-3.0.203/test/test_web_check.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_web_check_step.py` & `logicmonitor-sdk-3.0.203/test/test_web_check_step.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_web_page_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_web_page_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_web_resource.py` & `logicmonitor-sdk-3.0.203/test/test_web_resource.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website.py` & `logicmonitor-sdk-3.0.203/test/test_website.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_check_point.py` & `logicmonitor-sdk-3.0.203/test/test_website_check_point.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_checkpoint_raw_data.py` & `logicmonitor-sdk-3.0.203/test/test_website_checkpoint_raw_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_checkpoint_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_website_checkpoint_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_collector_info.py` & `logicmonitor-sdk-3.0.203/test/test_website_collector_info.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_graph_widget.py` & `logicmonitor-sdk-3.0.203/test/test_website_graph_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_group.py` & `logicmonitor-sdk-3.0.203/test/test_website_group.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_group_data.py` & `logicmonitor-sdk-3.0.203/test/test_website_group_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_group_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_website_group_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_group_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_website_group_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_individuals_status_widget.py` & `logicmonitor-sdk-3.0.203/test/test_website_individuals_status_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_item_config.py` & `logicmonitor-sdk-3.0.203/test/test_website_item_config.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_location.py` & `logicmonitor-sdk-3.0.203/test/test_website_location.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_noc_item.py` & `logicmonitor-sdk-3.0.203/test/test_website_noc_item.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_overall_status_widget.py` & `logicmonitor-sdk-3.0.203/test/test_website_overall_status_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_overview_report.py` & `logicmonitor-sdk-3.0.203/test/test_website_overview_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_overview_widget.py` & `logicmonitor-sdk-3.0.203/test/test_website_overview_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_website_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_sdt.py` & `logicmonitor-sdk-3.0.203/test/test_website_sdt.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_sdt_history_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_website_sdt_history_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_sla_report.py` & `logicmonitor-sdk-3.0.203/test/test_website_sla_report.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_sla_widget.py` & `logicmonitor-sdk-3.0.203/test/test_website_sla_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_website_sla_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_website_sla_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_widget.py` & `logicmonitor-sdk-3.0.203/test/test_widget.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_widget_data.py` & `logicmonitor-sdk-3.0.203/test/test_widget_data.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_widget_pagination_response.py` & `logicmonitor-sdk-3.0.203/test/test_widget_pagination_response.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_widget_token.py` & `logicmonitor-sdk-3.0.203/test/test_widget_token.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_widget_token_inheritance.py` & `logicmonitor-sdk-3.0.203/test/test_widget_token_inheritance.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_windows_event_log_event_source.py` & `logicmonitor-sdk-3.0.203/test/test_windows_event_log_event_source.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_wmi_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_wmi_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_wmi_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_wmi_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_xen_auto_discovery_method.py` & `logicmonitor-sdk-3.0.203/test/test_xen_auto_discovery_method.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/test/test_xen_collector_attribute.py` & `logicmonitor-sdk-3.0.203/test/test_xen_collector_attribute.py`

 * *Files identical despite different names*

### Comparing `logicmonitor-sdk-3.0.200/README.md` & `logicmonitor-sdk-3.0.203/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # logicmonitor-sdk
 LogicMonitor is a SaaS-based performance monitoring platform that provides full visibility into complex, hybrid infrastructures, offering granular performance monitoring and actionable data and insights. logicmonitor_sdk enables you to manage your LogicMonitor account programmatically. <br> <br> Note: <ul> <li> For Python SDKs, the REQUEST parameters can contain camelCase or an underscore. </li> <li> Both underscore and camelCase are supported if parameters are encapsulated within the body. </li> <li> Only camelCase is supported if parameters are encapsulated within the body and also if the user is passing raw JSON as REQUEST parameter. However, the RESPONSE parameters always contain an underscore. For example, you can use testLocation or test_location in the REQUEST parameter. But the RESPONSE parameter will always be test_location. </li> <li> The fields parameter only supports camelCase. </li> </ul>
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 3.0.0
-- Package version: 3.0.200
+- Package version: 3.0.203
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -75,14 +75,15 @@
 
 All URIs are relative to *https://localhost/santaba/rest*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *LMApi* | [**ack_alert_by_id**](docs/LMApi.md#ack_alert_by_id) | **POST** /alert/alerts/{id}/ack | ack alert by id
 *LMApi* | [**ack_collector_down_alert_by_id**](docs/LMApi.md#ack_collector_down_alert_by_id) | **POST** /setting/collector/collectors/{id}/ackdown | ack collector down alert
+*LMApi* | [**add_access_group**](docs/LMApi.md#add_access_group) | **POST** /setting/accessgroup/add | Create a access group
 *LMApi* | [**add_admin**](docs/LMApi.md#add_admin) | **POST** /setting/admins | add user
 *LMApi* | [**add_alert_note_by_id**](docs/LMApi.md#add_alert_note_by_id) | **POST** /alert/alerts/{id}/note | add alert note
 *LMApi* | [**add_alert_rule**](docs/LMApi.md#add_alert_rule) | **POST** /setting/alert/rules | add alert rule
 *LMApi* | [**add_api_token_by_admin_id**](docs/LMApi.md#add_api_token_by_admin_id) | **POST** /setting/admins/{adminId}/apitokens | add api tokens for a user
 *LMApi* | [**add_applies_to_function**](docs/LMApi.md#add_applies_to_function) | **POST** /setting/functions | add applies to function
 *LMApi* | [**add_collector**](docs/LMApi.md#add_collector) | **POST** /setting/collector/collectors | add collector
 *LMApi* | [**add_collector_group**](docs/LMApi.md#add_collector_group) | **POST** /setting/collector/groups | add collector group
@@ -104,14 +105,15 @@
 *LMApi* | [**add_report_group**](docs/LMApi.md#add_report_group) | **POST** /report/groups | add report group
 *LMApi* | [**add_role**](docs/LMApi.md#add_role) | **POST** /setting/roles | add role
 *LMApi* | [**add_sdt**](docs/LMApi.md#add_sdt) | **POST** /sdt/sdts | add SDT (Response may contain extra fields depending upon the type of SDT being added)
 *LMApi* | [**add_website**](docs/LMApi.md#add_website) | **POST** /website/websites | add website
 *LMApi* | [**add_website_group**](docs/LMApi.md#add_website_group) | **POST** /website/groups | add website group
 *LMApi* | [**add_widget**](docs/LMApi.md#add_widget) | **POST** /dashboard/widgets | add widget (Based upon widget type the request and response may contain additional attributes. Please refer models corresponding to specific widget type at the bottom of this page to check the attributes)
 *LMApi* | [**collect_device_config_source_config**](docs/LMApi.md#collect_device_config_source_config) | **POST** /device/devices/{deviceId}/devicedatasources/{hdsId}/instances/{instanceId}/config/configCollection | collect a config for a device
+*LMApi* | [**delete_access_group**](docs/LMApi.md#delete_access_group) | **DELETE** /setting/accessgroup/{id} | Delete access group
 *LMApi* | [**delete_admin_by_id**](docs/LMApi.md#delete_admin_by_id) | **DELETE** /setting/admins/{id} | delete user
 *LMApi* | [**delete_alert_rule_by_id**](docs/LMApi.md#delete_alert_rule_by_id) | **DELETE** /setting/alert/rules/{id} | delete alert rule
 *LMApi* | [**delete_collector_by_id**](docs/LMApi.md#delete_collector_by_id) | **DELETE** /setting/collector/collectors/{id} | delete collector
 *LMApi* | [**delete_collector_group_by_id**](docs/LMApi.md#delete_collector_group_by_id) | **DELETE** /setting/collector/groups/{id} | delete collector group
 *LMApi* | [**delete_dashboard_by_id**](docs/LMApi.md#delete_dashboard_by_id) | **DELETE** /dashboard/dashboards/{id} | delete dashboard
 *LMApi* | [**delete_dashboard_group_by_id**](docs/LMApi.md#delete_dashboard_group_by_id) | **DELETE** /dashboard/groups/{id} | delete dashboard group
 *LMApi* | [**delete_datasource_by_id**](docs/LMApi.md#delete_datasource_by_id) | **DELETE** /setting/datasources/{id} | delete datasource
@@ -124,18 +126,21 @@
 *LMApi* | [**delete_report_group_by_id**](docs/LMApi.md#delete_report_group_by_id) | **DELETE** /report/groups/{id} | delete report group
 *LMApi* | [**delete_role_by_id**](docs/LMApi.md#delete_role_by_id) | **DELETE** /setting/roles/{id} | delete role
 *LMApi* | [**delete_sdt_by_id**](docs/LMApi.md#delete_sdt_by_id) | **DELETE** /sdt/sdts/{id} | delete SDT
 *LMApi* | [**delete_website_by_id**](docs/LMApi.md#delete_website_by_id) | **DELETE** /website/websites/{id} | delete website
 *LMApi* | [**delete_website_group_by_id**](docs/LMApi.md#delete_website_group_by_id) | **DELETE** /website/groups/{id} | delete website group
 *LMApi* | [**delete_widget_by_id**](docs/LMApi.md#delete_widget_by_id) | **DELETE** /dashboard/widgets/{id} | delete widget
 *LMApi* | [**discover_subscriptions**](docs/LMApi.md#discover_subscriptions) | **POST** /azure/functions/discoverSubscriptions | view subscriptions
+*LMApi* | [**escalated_alert_by_id**](docs/LMApi.md#escalated_alert_by_id) | **POST** /alert/alerts/{id}/escalate | escalate alert by id
 *LMApi* | [**execute_debug_command**](docs/LMApi.md#execute_debug_command) | **POST** /debug | Execute a Collector debug command
 *LMApi* | [**fetch_device_instances_data**](docs/LMApi.md#fetch_device_instances_data) | **POST** /device/instances/datafetch | fetch device instances data
 *LMApi* | [**fetch_report_using_task_id**](docs/LMApi.md#fetch_report_using_task_id) | **GET** /report/reports/{id}/tasks/{taskId} | get report for task Id
 *LMApi* | [**generate_report_by_id**](docs/LMApi.md#generate_report_by_id) | **POST** /report/reports/{id}/executions | run a report
+*LMApi* | [**get_access_group_by_id**](docs/LMApi.md#get_access_group_by_id) | **GET** /setting/accessgroup/{id} | Get access group by id
+*LMApi* | [**get_access_group_list**](docs/LMApi.md#get_access_group_list) | **GET** /setting/accessgroup | Get access group list
 *LMApi* | [**get_admin_by_id**](docs/LMApi.md#get_admin_by_id) | **GET** /setting/admins/{id} | get user
 *LMApi* | [**get_admin_list**](docs/LMApi.md#get_admin_list) | **GET** /setting/admins | get user list
 *LMApi* | [**get_alert_by_id**](docs/LMApi.md#get_alert_by_id) | **GET** /alert/alerts/{id} | get alert
 *LMApi* | [**get_alert_list**](docs/LMApi.md#get_alert_list) | **GET** /alert/alerts | get alert list
 *LMApi* | [**get_alert_list_by_device_group_id**](docs/LMApi.md#get_alert_list_by_device_group_id) | **GET** /device/groups/{id}/alerts | get device group alerts
 *LMApi* | [**get_alert_list_by_device_id**](docs/LMApi.md#get_alert_list_by_device_id) | **GET** /device/devices/{id}/alerts | get alerts
 *LMApi* | [**get_alert_rule_by_id**](docs/LMApi.md#get_alert_rule_by_id) | **GET** /setting/alert/rules/{id} | get alert rule by id
@@ -170,14 +175,15 @@
 *LMApi* | [**get_device_config_source_config_list**](docs/LMApi.md#get_device_config_source_config_list) | **GET** /device/devices/{deviceId}/devicedatasources/{hdsId}/instances/{instanceId}/config | get detailed config information for the instance
 *LMApi* | [**get_device_datasource_by_id**](docs/LMApi.md#get_device_datasource_by_id) | **GET** /device/devices/{deviceId}/devicedatasources/{id} | get device datasource 
 *LMApi* | [**get_device_datasource_data_by_id**](docs/LMApi.md#get_device_datasource_data_by_id) | **GET** /device/devices/{deviceId}/devicedatasources/{id}/data | get device datasource data 
 *LMApi* | [**get_device_datasource_instance_alert_setting_list_of_dsi**](docs/LMApi.md#get_device_datasource_instance_alert_setting_list_of_dsi) | **GET** /device/devices/{deviceId}/devicedatasources/{hdsId}/instances/{instanceId}/alertsettings | get a list of alert settings for a device datasource instance
 *LMApi* | [**get_device_datasource_instance_by_id**](docs/LMApi.md#get_device_datasource_instance_by_id) | **GET** /device/devices/{deviceId}/devicedatasources/{hdsId}/instances/{id} | get device instance 
 *LMApi* | [**get_device_datasource_instance_data**](docs/LMApi.md#get_device_datasource_instance_data) | **GET** /device/devices/{deviceId}/devicedatasources/{hdsId}/instances/{id}/data | get device instance data
 *LMApi* | [**get_device_datasource_instance_graph_data**](docs/LMApi.md#get_device_datasource_instance_graph_data) | **GET** /device/devices/{deviceId}/devicedatasources/{hdsId}/instances/{id}/graphs/{graphId}/data | get device instance graph data 
+*LMApi* | [**get_device_datasource_instance_group_by_id**](docs/LMApi.md#get_device_datasource_instance_group_by_id) | **GET** /device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{id} | get device datasource instance group 
 *LMApi* | [**get_device_datasource_instance_group_list**](docs/LMApi.md#get_device_datasource_instance_group_list) | **GET** /device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups | get device datasource instance group list 
 *LMApi* | [**get_device_datasource_instance_group_overview_graph_data**](docs/LMApi.md#get_device_datasource_instance_group_overview_graph_data) | **GET** /device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{dsigId}/graphs/{ographId}/data | get device instance group overview graph data 
 *LMApi* | [**get_device_datasource_instance_list**](docs/LMApi.md#get_device_datasource_instance_list) | **GET** /device/devices/{deviceId}/devicedatasources/{hdsId}/instances | get device instance list
 *LMApi* | [**get_device_datasource_instance_sdt_history**](docs/LMApi.md#get_device_datasource_instance_sdt_history) | **GET** /device/devices/{deviceId}/devicedatasources/{hdsId}/instances/{id}/historysdts | get device instance SDT history
 *LMApi* | [**get_device_datasource_list**](docs/LMApi.md#get_device_datasource_list) | **GET** /device/devices/{deviceId}/devicedatasources | get device datasource list 
 *LMApi* | [**get_device_group_by_id**](docs/LMApi.md#get_device_group_by_id) | **GET** /device/groups/{id} | get device group
 *LMApi* | [**get_device_group_datasource_alert_setting**](docs/LMApi.md#get_device_group_datasource_alert_setting) | **GET** /device/groups/{deviceGroupId}/datasources/{dsId}/alertsettings | get device group datasource alert setting 
@@ -233,14 +239,15 @@
 *LMApi* | [**get_website_list**](docs/LMApi.md#get_website_list) | **GET** /website/websites | get website list
 *LMApi* | [**get_website_property_list_by_website_id**](docs/LMApi.md#get_website_property_list_by_website_id) | **GET** /website/websites/{id}/properties | get a list of properties for a website
 *LMApi* | [**get_website_sdt_list_by_website_id**](docs/LMApi.md#get_website_sdt_list_by_website_id) | **GET** /website/websites/{id}/sdts | get a list of SDTs for a website
 *LMApi* | [**get_widget_by_id**](docs/LMApi.md#get_widget_by_id) | **GET** /dashboard/widgets/{id} | get widget by id (Based upon widget type the response may contain additional attributes. Please refer models corresponding to specific widget type at the bottom of this page to check the attributes)
 *LMApi* | [**get_widget_data_by_id**](docs/LMApi.md#get_widget_data_by_id) | **GET** /dashboard/widgets/{id}/data | get widget data (Based upon widget type the response may contain additional attributes. Please refer models corresponding to specific widget type at the bottom of this page to check the attributes)
 *LMApi* | [**get_widget_list**](docs/LMApi.md#get_widget_list) | **GET** /dashboard/widgets | get widget list (Based upon widget type the response may contain additional attributes. Please refer models corresponding to specific widget type at the bottom of this page to check the attributes)
 *LMApi* | [**get_widget_list_by_dashboard_id**](docs/LMApi.md#get_widget_list_by_dashboard_id) | **GET** /dashboard/dashboards/{id}/widgets | get widget list by DashboardId
+*LMApi* | [**patch_access_group**](docs/LMApi.md#patch_access_group) | **PATCH** /setting/accessgroup/{id} | Update access group
 *LMApi* | [**patch_admin_by_id**](docs/LMApi.md#patch_admin_by_id) | **PATCH** /setting/admins/{id} | update user
 *LMApi* | [**patch_alert_rule_by_id**](docs/LMApi.md#patch_alert_rule_by_id) | **PATCH** /setting/alert/rules/{id} | update alert rule
 *LMApi* | [**patch_applies_to_function**](docs/LMApi.md#patch_applies_to_function) | **PATCH** /setting/functions/{id} | update applies to function
 *LMApi* | [**patch_collector_by_id**](docs/LMApi.md#patch_collector_by_id) | **PATCH** /setting/collector/collectors/{id} | update collector
 *LMApi* | [**patch_collector_group_by_id**](docs/LMApi.md#patch_collector_group_by_id) | **PATCH** /setting/collector/groups/{id} | update collector group
 *LMApi* | [**patch_dashboard_by_id**](docs/LMApi.md#patch_dashboard_by_id) | **PATCH** /dashboard/dashboards/{id} | update dashboard
 *LMApi* | [**patch_dashboard_group_by_id**](docs/LMApi.md#patch_dashboard_group_by_id) | **PATCH** /dashboard/groups/{id} | update dashboard group
@@ -252,28 +259,28 @@
 *LMApi* | [**patch_device_datasource_instance_group_by_id**](docs/LMApi.md#patch_device_datasource_instance_group_by_id) | **PATCH** /device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{id} | update device datasource instance group
 *LMApi* | [**patch_device_group_by_id**](docs/LMApi.md#patch_device_group_by_id) | **PATCH** /device/groups/{id} | update device group
 *LMApi* | [**patch_device_group_datasource_alert_setting**](docs/LMApi.md#patch_device_group_datasource_alert_setting) | **PATCH** /device/groups/{deviceGroupId}/datasources/{dsId}/alertsettings | update device group datasource alert setting
 *LMApi* | [**patch_device_group_datasource_by_id**](docs/LMApi.md#patch_device_group_datasource_by_id) | **PATCH** /device/groups/{deviceGroupId}/datasources/{id} | update device group datasource
 *LMApi* | [**patch_device_group_property_by_name**](docs/LMApi.md#patch_device_group_property_by_name) | **PATCH** /device/groups/{gid}/properties/{name} | update device group property
 *LMApi* | [**patch_device_property_by_name**](docs/LMApi.md#patch_device_property_by_name) | **PATCH** /device/devices/{deviceId}/properties/{name} | update device property
 *LMApi* | [**patch_escalation_chain_by_id**](docs/LMApi.md#patch_escalation_chain_by_id) | **PATCH** /setting/alert/chains/{id} | update escalation chain
-*LMApi* | [**patch_instances_alert_threshold**](docs/LMApi.md#patch_instances_alert_threshold) | **PATCH** /device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{dsigId}/datapoints/{dpId}/alertconfig | update instances alert threshold (Setting the threshold at default group is not allowed)
 *LMApi* | [**patch_recipient_group_by_id**](docs/LMApi.md#patch_recipient_group_by_id) | **PATCH** /setting/recipientgroups/{id} | update recipient group
 *LMApi* | [**patch_report_by_id**](docs/LMApi.md#patch_report_by_id) | **PATCH** /report/reports/{id} | update report
 *LMApi* | [**patch_report_group_by_id**](docs/LMApi.md#patch_report_group_by_id) | **PATCH** /report/groups/{id} | update report group
 *LMApi* | [**patch_role_by_id**](docs/LMApi.md#patch_role_by_id) | **PATCH** /setting/roles/{id} | update role
 *LMApi* | [**patch_sdt_by_id**](docs/LMApi.md#patch_sdt_by_id) | **PATCH** /sdt/sdts/{id} | update SDT (Response may contain extra fields depending upon the type of SDT being updated)
 *LMApi* | [**patch_website_by_id**](docs/LMApi.md#patch_website_by_id) | **PATCH** /website/websites/{id} | update website
 *LMApi* | [**patch_website_group_by_id**](docs/LMApi.md#patch_website_group_by_id) | **PATCH** /website/groups/{id} | update website group
 *LMApi* | [**patch_widget_by_id**](docs/LMApi.md#patch_widget_by_id) | **PATCH** /dashboard/widgets/{id} | update widget (Based upon widget type the request and response may contain additional attributes. Please refer models corresponding to specific widget type at the bottom of this page to check the attributes)
 *LMApi* | [**schedule_auto_discovery_by_device_id**](docs/LMApi.md#schedule_auto_discovery_by_device_id) | **POST** /device/devices/{id}/scheduleAutoDiscovery | schedule active discovery for a device
 *LMApi* | [**test_aws_account**](docs/LMApi.md#test_aws_account) | **POST** /aws/functions/testAccount | test AWS account
 *LMApi* | [**test_azure_account**](docs/LMApi.md#test_azure_account) | **POST** /azure/functions/testAccount | test Azure account
 *LMApi* | [**test_gcp_account**](docs/LMApi.md#test_gcp_account) | **POST** /gcp/functions/testAccount | test GCP account
 *LMApi* | [**test_saa_s_account**](docs/LMApi.md#test_saa_s_account) | **POST** /saas/functions/testAccount | test SaaS account
+*LMApi* | [**update_access_group**](docs/LMApi.md#update_access_group) | **PUT** /setting/accessgroup/{id} | Update access group
 *LMApi* | [**update_admin_by_id**](docs/LMApi.md#update_admin_by_id) | **PUT** /setting/admins/{id} | update user
 *LMApi* | [**update_alert_rule_by_id**](docs/LMApi.md#update_alert_rule_by_id) | **PUT** /setting/alert/rules/{id} | update alert rule
 *LMApi* | [**update_applies_to_function**](docs/LMApi.md#update_applies_to_function) | **PUT** /setting/functions/{id} | update applies to function
 *LMApi* | [**update_collector_by_id**](docs/LMApi.md#update_collector_by_id) | **PUT** /setting/collector/collectors/{id} | update collector
 *LMApi* | [**update_collector_group_by_id**](docs/LMApi.md#update_collector_group_by_id) | **PUT** /setting/collector/groups/{id} | update collector group
 *LMApi* | [**update_dashboard_by_id**](docs/LMApi.md#update_dashboard_by_id) | **PUT** /dashboard/dashboards/{id} | update dashboard
 *LMApi* | [**update_dashboard_group_by_id**](docs/LMApi.md#update_dashboard_group_by_id) | **PUT** /dashboard/groups/{id} | update dashboard group
@@ -285,28 +292,30 @@
 *LMApi* | [**update_device_datasource_instance_group_by_id**](docs/LMApi.md#update_device_datasource_instance_group_by_id) | **PUT** /device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{id} | update device datasource instance group
 *LMApi* | [**update_device_group_by_id**](docs/LMApi.md#update_device_group_by_id) | **PUT** /device/groups/{id} | update device group
 *LMApi* | [**update_device_group_datasource_alert_setting**](docs/LMApi.md#update_device_group_datasource_alert_setting) | **PUT** /device/groups/{deviceGroupId}/datasources/{dsId}/alertsettings | update device group datasource alert setting
 *LMApi* | [**update_device_group_datasource_by_id**](docs/LMApi.md#update_device_group_datasource_by_id) | **PUT** /device/groups/{deviceGroupId}/datasources/{id} | update device group datasource
 *LMApi* | [**update_device_group_property_by_name**](docs/LMApi.md#update_device_group_property_by_name) | **PUT** /device/groups/{gid}/properties/{name} | update device group property
 *LMApi* | [**update_device_property_by_name**](docs/LMApi.md#update_device_property_by_name) | **PUT** /device/devices/{deviceId}/properties/{name} | update device property
 *LMApi* | [**update_escalation_chain_by_id**](docs/LMApi.md#update_escalation_chain_by_id) | **PUT** /setting/alert/chains/{id} | update escalation chain
-*LMApi* | [**update_instances_alert_threshold**](docs/LMApi.md#update_instances_alert_threshold) | **PUT** /device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{dsigId}/datapoints/{dpId}/alertconfig | update instances alert threshold (Setting the threshold at default group is not allowed)
+*LMApi* | [**update_instance_group_alert_threshold**](docs/LMApi.md#update_instance_group_alert_threshold) | **PUT** /device/devices/{deviceId}/devicedatasources/{deviceDsId}/groups/{dsigId}/datapoints/{dpId}/alertconfig | update instance group alert threshold (Setting the threshold at default group is not allowed)
 *LMApi* | [**update_recipient_group_by_id**](docs/LMApi.md#update_recipient_group_by_id) | **PUT** /setting/recipientgroups/{id} | update recipient group
 *LMApi* | [**update_report_by_id**](docs/LMApi.md#update_report_by_id) | **PUT** /report/reports/{id} | update report
 *LMApi* | [**update_report_group_by_id**](docs/LMApi.md#update_report_group_by_id) | **PUT** /report/groups/{id} | update report group
 *LMApi* | [**update_role_by_id**](docs/LMApi.md#update_role_by_id) | **PUT** /setting/roles/{id} | update role
 *LMApi* | [**update_sdt_by_id**](docs/LMApi.md#update_sdt_by_id) | **PUT** /sdt/sdts/{id} | update SDT (Response may contain extra fields depending upon the type of SDT being updated)
 *LMApi* | [**update_website_by_id**](docs/LMApi.md#update_website_by_id) | **PUT** /website/websites/{id} | update website
 *LMApi* | [**update_website_group_by_id**](docs/LMApi.md#update_website_group_by_id) | **PUT** /website/groups/{id} | update website group
 *LMApi* | [**update_widget_by_id**](docs/LMApi.md#update_widget_by_id) | **PUT** /dashboard/widgets/{id} | update widget (Based upon widget type the request and response may contain additional attributes. Please refer models corresponding to specific widget type at the bottom of this page to check the attributes)
 
 
 ## Documentation For Models
 
  - [APIToken](docs/APIToken.md)
+ - [AccessGroup](docs/AccessGroup.md)
+ - [AccessGroupPaginationResponse](docs/AccessGroupPaginationResponse.md)
  - [AccessLogPaginationResponse](docs/AccessLogPaginationResponse.md)
  - [AckCollectorDown](docs/AckCollectorDown.md)
  - [Admin](docs/Admin.md)
  - [AdminPaginationResponse](docs/AdminPaginationResponse.md)
  - [Alert](docs/Alert.md)
  - [AlertAck](docs/AlertAck.md)
  - [AlertFilters](docs/AlertFilters.md)
@@ -477,14 +486,15 @@
  - [RecipientGroup](docs/RecipientGroup.md)
  - [RecipientGroupPaginationResponse](docs/RecipientGroupPaginationResponse.md)
  - [ReportBase](docs/ReportBase.md)
  - [ReportGroup](docs/ReportGroup.md)
  - [ReportGroupPaginationResponse](docs/ReportGroupPaginationResponse.md)
  - [ReportPaginationResponse](docs/ReportPaginationResponse.md)
  - [ReportRecipient](docs/ReportRecipient.md)
+ - [ResourceDataSourceAlertThresholdInfo](docs/ResourceDataSourceAlertThresholdInfo.md)
  - [RestAppliesToFunctionPaginationResponse](docs/RestAppliesToFunctionPaginationResponse.md)
  - [RestAwsAccountTestV3](docs/RestAwsAccountTestV3.md)
  - [RestAzureAccountTestV3](docs/RestAzureAccountTestV3.md)
  - [RestAzureSubscriptionV3](docs/RestAzureSubscriptionV3.md)
  - [RestAzureSubscriptionsDiscoverV3](docs/RestAzureSubscriptionsDiscoverV3.md)
  - [RestCloudOkPermissionsV3](docs/RestCloudOkPermissionsV3.md)
  - [RestDashboardGroupAsyncCloneResponse](docs/RestDashboardGroupAsyncCloneResponse.md)
@@ -566,14 +576,16 @@
  - [AwsEC2ReservedInstanceDiscoveryMethod](docs/AwsEC2ReservedInstanceDiscoveryMethod.md)
  - [AwsEC2ScheduledEventsCollectorAttribute](docs/AwsEC2ScheduledEventsCollectorAttribute.md)
  - [AwsEbsVolumeSnapshotCollectorAttributeV3](docs/AwsEbsVolumeSnapshotCollectorAttributeV3.md)
  - [AwsEc2ServiceLimitsCollectorAttribute](docs/AwsEc2ServiceLimitsCollectorAttribute.md)
  - [AwsEcsServiceDetailsCollectorAttribute](docs/AwsEcsServiceDetailsCollectorAttribute.md)
  - [AwsEcsServiceDiscoveryMethod](docs/AwsEcsServiceDiscoveryMethod.md)
  - [AwsElastiCacheDiscoveryMethod](docs/AwsElastiCacheDiscoveryMethod.md)
+ - [AwsGlobalNetworkDeviceMethod](docs/AwsGlobalNetworkDeviceMethod.md)
+ - [AwsGlobalNetworkLinkMethod](docs/AwsGlobalNetworkLinkMethod.md)
  - [AwsGlobalWebACLDiscoveryMethodV3](docs/AwsGlobalWebACLDiscoveryMethodV3.md)
  - [AwsLBTargetGroupDiscoveryMethod](docs/AwsLBTargetGroupDiscoveryMethod.md)
  - [AwsMediaConnectOutputDiscoveryMethod](docs/AwsMediaConnectOutputDiscoveryMethod.md)
  - [AwsMediaConnectSourceDiscoveryMethod](docs/AwsMediaConnectSourceDiscoveryMethod.md)
  - [AwsRdsPerformanceInsightsCollectorAttribute](docs/AwsRdsPerformanceInsightsCollectorAttribute.md)
  - [AwsRdsServiceLimitsCollectorAttributeV3](docs/AwsRdsServiceLimitsCollectorAttributeV3.md)
  - [AwsRedShiftDiscoveryMethod](docs/AwsRedShiftDiscoveryMethod.md)
@@ -626,14 +638,16 @@
  - [AzureRedisCacheDiscoveryMethod](docs/AzureRedisCacheDiscoveryMethod.md)
  - [AzureReplicationDisasterRecoveryCollectorAttribute](docs/AzureReplicationDisasterRecoveryCollectorAttribute.md)
  - [AzureReplicationJobCollectorAttributeV3](docs/AzureReplicationJobCollectorAttributeV3.md)
  - [AzureReplicationJobDiscoveryMethod](docs/AzureReplicationJobDiscoveryMethod.md)
  - [AzureResourceHealthCollectorAttribute](docs/AzureResourceHealthCollectorAttribute.md)
  - [AzureResourceUsageCollectorAttribute](docs/AzureResourceUsageCollectorAttribute.md)
  - [AzureRssEventSource](docs/AzureRssEventSource.md)
+ - [AzureServiceBusQueue](docs/AzureServiceBusQueue.md)
+ - [AzureServiceBusTopic](docs/AzureServiceBusTopic.md)
  - [AzureServiceRegionDiscoveryMethod](docs/AzureServiceRegionDiscoveryMethod.md)
  - [AzureStorageServiceLimitsCollectorAttribute](docs/AzureStorageServiceLimitsCollectorAttribute.md)
  - [AzureSubscriptionDiscoveryMethod](docs/AzureSubscriptionDiscoveryMethod.md)
  - [AzureSynapseDiscoveryMethodV3](docs/AzureSynapseDiscoveryMethodV3.md)
  - [AzureVMBackupStatusCollectorAttributeV3](docs/AzureVMBackupStatusCollectorAttributeV3.md)
  - [AzureVMBackupStatusLogAnalyticsCollectorAttribute](docs/AzureVMBackupStatusLogAnalyticsCollectorAttribute.md)
  - [AzureVMServiceLimitsCollectorAttribute](docs/AzureVMServiceLimitsCollectorAttribute.md)
@@ -761,14 +775,15 @@
  - [PingCollectorAttribute](docs/PingCollectorAttribute.md)
  - [PortAutoDiscoveryMethod](docs/PortAutoDiscoveryMethod.md)
  - [PushModulesCollectorAttribute](docs/PushModulesCollectorAttribute.md)
  - [RabbitMQQueueAutoDiscoveryMethod](docs/RabbitMQQueueAutoDiscoveryMethod.md)
  - [ResourceGroupSDT](docs/ResourceGroupSDT.md)
  - [ResourceSDT](docs/ResourceSDT.md)
  - [RestAwsHealthEventSource](docs/RestAwsHealthEventSource.md)
+ - [RestAwsOrganizationalHealthEventSource](docs/RestAwsOrganizationalHealthEventSource.md)
  - [RestAwsRdsPerformanceInsightsEventSource](docs/RestAwsRdsPerformanceInsightsEventSource.md)
  - [RestAwsTrustedAdvisorEventSource](docs/RestAwsTrustedAdvisorEventSource.md)
  - [RestAzureAdvisorEventSource](docs/RestAzureAdvisorEventSource.md)
  - [RestAzureResourceHealthEventSource](docs/RestAzureResourceHealthEventSource.md)
  - [RestAzureResourceLogAnalyticsWorkspacesSource](docs/RestAzureResourceLogAnalyticsWorkspacesSource.md)
  - [RestSavedMapWidgetV3](docs/RestSavedMapWidgetV3.md)
  - [RoleReport](docs/RoleReport.md)
```

### Comparing `logicmonitor-sdk-3.0.200/setup.py` & `logicmonitor-sdk-3.0.203/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "logicmonitor-sdk"
-VERSION = "3.0.200"
+VERSION = "3.0.203"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `logicmonitor-sdk-3.0.200/PKG-INFO` & `logicmonitor-sdk-3.0.203/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: logicmonitor-sdk
-Version: 3.0.200
+Version: 3.0.203
 Summary: LogicMonitor REST API
 Home-page: https://github.com/logicmonitor/lm-sdk-python
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
 Description:     LogicMonitor is a SaaS-based performance monitoring platform that provides full visibility into complex, hybrid infrastructures, offering granular performance monitoring and actionable data and insights. logicmonitor_sdk enables you to manage your LogicMonitor account programmatically. &lt;br&gt; &lt;br&gt; Note: &lt;ul&gt; &lt;li&gt; For Python SDKs, the REQUEST parameters can contain camelCase or an underscore. &lt;/li&gt; &lt;li&gt; Both underscore and camelCase are supported if parameters are encapsulated within the body. &lt;/li&gt; &lt;li&gt; Only camelCase is supported if parameters are encapsulated within the body and also if the user is passing raw JSON as REQUEST parameter. However, the RESPONSE parameters always contain an underscore. For example, you can use testLocation or test_location in the REQUEST parameter. But the RESPONSE parameter will always be test_location. &lt;/li&gt; &lt;li&gt; The fields parameter only supports camelCase. &lt;/li&gt; &lt;/ul&gt;  # noqa: E501
```

