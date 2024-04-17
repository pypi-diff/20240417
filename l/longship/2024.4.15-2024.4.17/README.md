# Comparing `tmp/longship-2024.4.15.tar.gz` & `tmp/longship-2024.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longship-2024.4.15.tar", max compression
+gzip compressed data, was "longship-2024.4.17.tar", max compression
```

## Comparing `longship-2024.4.15.tar` & `longship-2024.4.17.tar`

### file list

```diff
@@ -1,331 +1,331 @@
--rw-r--r--   0        0        0     1072 2023-06-26 16:00:19.878825 longship-2024.4.15/LICENSE
--rw-r--r--   0        0        0     4661 2023-06-26 16:47:23.288883 longship-2024.4.15/README.md
--rw-r--r--   0        0        0     7668 2024-03-14 10:00:43.390594 longship-2024.4.15/longship/client.py
--rw-r--r--   0        0        0      112 2023-06-26 16:00:19.886682 longship-2024.4.15/longship/errors.py
--rw-r--r--   0        0        0     4614 2024-03-14 15:13:41.390085 longship-2024.4.15/longship/types.py
--rw-r--r--   0        0        0      155 2024-03-25 19:42:53.022260 longship-2024.4.15/longship_api_client/__init__.py
--rw-r--r--   0        0        0       45 2024-03-25 19:42:53.025427 longship-2024.4.15/longship_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.296257 longship-2024.4.15/longship_api_client/api/cdrs/__init__.py
--rw-r--r--   0        0        0     4458 2024-03-25 20:00:43.969808 longship-2024.4.15/longship_api_client/api/cdrs/cdr_get.py
--rw-r--r--   0        0        0     5023 2024-03-25 20:00:43.970406 longship-2024.4.15/longship_api_client/api/cdrs/cdr_patch.py
--rw-r--r--   0        0        0    19502 2024-03-25 20:00:43.970703 longship-2024.4.15/longship_api_client/api/cdrs/get_all_cdrs.py
--rw-r--r--   0        0        0     7993 2024-03-25 20:00:43.971091 longship-2024.4.15/longship_api_client/api/cdrs/get_all_interchangeformat.py
--rw-r--r--   0        0        0     5989 2024-03-25 20:00:43.971416 longship-2024.4.15/longship_api_client/api/cdrs/get_file_full_download_cdrs.py
--rw-r--r--   0        0        0     5968 2024-03-25 20:00:43.971772 longship-2024.4.15/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.288563 longship-2024.4.15/longship_api_client/api/chargepoint_status/__init__.py
--rw-r--r--   0        0        0     4767 2024-03-25 20:00:43.972132 longship-2024.4.15/longship_api_client/api/chargepoint_status/chargepoint_status_get.py
--rw-r--r--   0        0        0     6490 2024-03-25 20:00:43.972453 longship-2024.4.15/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.289893 longship-2024.4.15/longship_api_client/api/chargepoints/__init__.py
--rw-r--r--   0        0        0     4634 2024-03-25 20:00:43.972876 longship-2024.4.15/longship_api_client/api/chargepoints/chargepoint_get.py
--rw-r--r--   0        0        0     5162 2024-03-25 20:00:43.973593 longship-2024.4.15/longship_api_client/api/chargepoints/chargepoint_put.py
--rw-r--r--   0        0        0     5416 2024-03-25 20:00:43.973998 longship-2024.4.15/longship_api_client/api/chargepoints/chargepointauthorization_get.py
--rw-r--r--   0        0        0     5252 2024-03-25 20:00:43.976187 longship-2024.4.15/longship_api_client/api/chargepoints/chargepointauthorization_post.py
--rw-r--r--   0        0        0     9920 2024-03-25 20:00:43.976569 longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepointauthorizations.py
--rw-r--r--   0        0        0    11723 2024-03-25 20:00:43.976947 longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepointmessages.py
--rw-r--r--   0        0        0    16896 2024-03-25 20:00:43.977268 longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepoints.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.307087 longship-2024.4.15/longship_api_client/api/commands/__init__.py
--rw-r--r--   0        0        0     5151 2024-03-25 20:00:43.977620 longship-2024.4.15/longship_api_client/api/commands/send_cancel_reservation_request.py
--rw-r--r--   0        0        0     5171 2024-03-25 20:00:43.978017 longship-2024.4.15/longship_api_client/api/commands/send_change_availability_request.py
--rw-r--r--   0        0        0     5191 2024-03-25 20:00:43.978353 longship-2024.4.15/longship_api_client/api/commands/send_change_configuration_request.py
--rw-r--r--   0        0        0     5011 2024-03-25 19:42:53.020065 longship-2024.4.15/longship_api_client/api/commands/send_clear_cache_request.py
--rw-r--r--   0        0        0     5212 2024-03-25 20:00:43.978639 longship-2024.4.15/longship_api_client/api/commands/send_clear_charging_profile_request.py
--rw-r--r--   0        0        0     5051 2024-03-25 20:00:43.979167 longship-2024.4.15/longship_api_client/api/commands/send_data_transfer_request.py
--rw-r--r--   0        0        0     5212 2024-03-25 20:00:43.979385 longship-2024.4.15/longship_api_client/api/commands/send_get_composite_schedule_request.py
--rw-r--r--   0        0        0     5131 2024-03-25 19:42:53.015992 longship-2024.4.15/longship_api_client/api/commands/send_get_configuration_request.py
--rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.979633 longship-2024.4.15/longship_api_client/api/commands/send_get_diagnostics_request.py
--rw-r--r--   0        0        0     5193 2024-03-25 20:00:43.979964 longship-2024.4.15/longship_api_client/api/commands/send_get_local_list_version_request.py
--rw-r--r--   0        0        0     5241 2024-03-25 20:00:43.980364 longship-2024.4.15/longship_api_client/api/commands/send_remote_start_transaction_request.py
--rw-r--r--   0        0        0     5221 2024-03-25 20:00:43.980710 longship-2024.4.15/longship_api_client/api/commands/send_remote_stop_transaction_request.py
--rw-r--r--   0        0        0     5011 2024-03-25 20:00:43.981052 longship-2024.4.15/longship_api_client/api/commands/send_reserve_now_request.py
--rw-r--r--   0        0        0     4946 2024-03-25 20:00:43.981436 longship-2024.4.15/longship_api_client/api/commands/send_reset_request.py
--rw-r--r--   0        0        0     5072 2024-03-25 19:42:53.014730 longship-2024.4.15/longship_api_client/api/commands/send_send_local_list_request.py
--rw-r--r--   0        0        0     5172 2024-03-25 20:00:43.981843 longship-2024.4.15/longship_api_client/api/commands/send_set_charging_profile_request.py
--rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.982152 longship-2024.4.15/longship_api_client/api/commands/send_trigger_message_request.py
--rw-r--r--   0        0        0     5111 2024-03-25 19:42:53.021486 longship-2024.4.15/longship_api_client/api/commands/send_unlock_connector_request.py
--rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.982342 longship-2024.4.15/longship_api_client/api/commands/send_update_firmware_request.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.330382 longship-2024.4.15/longship_api_client/api/configurationitems/__init__.py
--rw-r--r--   0        0        0     5527 2024-03-25 20:00:43.982664 longship-2024.4.15/longship_api_client/api/configurationitems/configurationitem_get.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.317516 longship-2024.4.15/longship_api_client/api/localtokengroups/__init__.py
--rw-r--r--   0        0        0     6508 2024-03-25 20:00:43.982954 longship-2024.4.15/longship_api_client/api/localtokengroups/get_all_localtokengroups.py
--rw-r--r--   0        0        0     4437 2024-03-25 19:42:53.009339 longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_delete.py
--rw-r--r--   0        0        0     5028 2024-03-25 19:42:53.008522 longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_post.py
--rw-r--r--   0        0        0     5243 2024-03-25 20:00:43.983235 longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_put.py
--rw-r--r--   0        0        0     4764 2024-03-25 20:00:43.983514 longship-2024.4.15/longship_api_client/api/localtokengroups/localtokengroup_get.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.331027 longship-2024.4.15/longship_api_client/api/localtokengroupstoken/__init__.py
--rw-r--r--   0        0        0     4848 2024-03-25 19:42:53.025042 longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_delete.py
--rw-r--r--   0        0        0     5216 2024-03-25 20:00:43.983719 longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_post.py
--rw-r--r--   0        0        0     6004 2024-03-25 20:00:43.984111 longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_put.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.332975 longship-2024.4.15/longship_api_client/api/location/__init__.py
--rw-r--r--   0        0        0     5151 2024-03-25 20:00:43.984328 longship-2024.4.15/longship_api_client/api/location/location_patch.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.282660 longship-2024.4.15/longship_api_client/api/locations/__init__.py
--rw-r--r--   0        0        0    11635 2024-03-25 20:00:43.984514 longship-2024.4.15/longship_api_client/api/locations/get_all_locations.py
--rw-r--r--   0        0        0     4568 2024-03-25 20:00:43.984928 longship-2024.4.15/longship_api_client/api/locations/location_get.py
--rw-r--r--   0        0        0     5033 2024-03-25 20:00:43.985237 longship-2024.4.15/longship_api_client/api/locations/location_post.py
--rw-r--r--   0        0        0     4850 2024-03-25 20:00:43.985423 longship-2024.4.15/longship_api_client/api/locations/location_put.py
--rw-r--r--   0        0        0     5150 2024-03-25 19:42:53.023748 longship-2024.4.15/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py
--rw-r--r--   0        0        0     5484 2024-03-25 20:00:43.985706 longship-2024.4.15/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.306476 longship-2024.4.15/longship_api_client/api/mspreimbursement/__init__.py
--rw-r--r--   0        0        0     4499 2024-03-25 19:42:53.013509 longship-2024.4.15/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.303969 longship-2024.4.15/longship_api_client/api/organizationunits/__init__.py
--rw-r--r--   0        0        0     6531 2024-03-25 20:00:43.986158 longship-2024.4.15/longship_api_client/api/organizationunits/get_all_organizationunits.py
--rw-r--r--   0        0        0     4787 2024-03-25 20:00:43.986377 longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_get.py
--rw-r--r--   0        0        0     5049 2024-03-25 20:00:43.986553 longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_post.py
--rw-r--r--   0        0        0     5250 2024-03-25 20:00:43.986734 longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_put.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.301307 longship-2024.4.15/longship_api_client/api/reimbursement/__init__.py
--rw-r--r--   0        0        0    10500 2024-03-25 20:00:43.987077 longship-2024.4.15/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py
--rw-r--r--   0        0        0     5141 2024-03-25 19:42:53.009738 longship-2024.4.15/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py
--rw-r--r--   0        0        0     4745 2024-03-25 19:42:53.010083 longship-2024.4.15/longship_api_client/api/reimbursement/reimbursement_cdr_get.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.260831 longship-2024.4.15/longship_api_client/api/sessions/__init__.py
--rw-r--r--   0        0        0    20550 2024-03-25 20:00:43.987351 longship-2024.4.15/longship_api_client/api/sessions/get_all_sessions.py
--rw-r--r--   0        0        0     4546 2024-03-25 20:00:43.987624 longship-2024.4.15/longship_api_client/api/sessions/session_get.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.326877 longship-2024.4.15/longship_api_client/api/tariffdistributions/__init__.py
--rw-r--r--   0        0        0     8625 2024-03-25 20:00:43.988058 longship-2024.4.15/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py
--rw-r--r--   0        0        0     4583 2024-03-25 20:00:43.988413 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_delete.py
--rw-r--r--   0        0        0     4683 2024-03-25 20:00:43.988748 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_get.py
--rw-r--r--   0        0        0     5375 2024-03-25 20:00:43.989159 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_patch.py
--rw-r--r--   0        0        0     4941 2024-03-25 20:00:43.989422 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_post.py
--rw-r--r--   0        0        0     5613 2024-03-25 20:00:43.989810 longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_put.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.323367 longship-2024.4.15/longship_api_client/api/tariffs/__init__.py
--rw-r--r--   0        0        0     7355 2024-03-25 20:00:43.990037 longship-2024.4.15/longship_api_client/api/tariffs/get_all_tariffs.py
--rw-r--r--   0        0        0     4475 2024-03-25 20:00:43.990394 longship-2024.4.15/longship_api_client/api/tariffs/tariff_delete.py
--rw-r--r--   0        0        0     4524 2024-03-25 20:00:43.990763 longship-2024.4.15/longship_api_client/api/tariffs/tariff_get.py
--rw-r--r--   0        0        0     5134 2024-03-25 20:00:43.990994 longship-2024.4.15/longship_api_client/api/tariffs/tariff_patch.py
--rw-r--r--   0        0        0     4836 2024-03-25 20:00:43.991198 longship-2024.4.15/longship_api_client/api/tariffs/tariff_post.py
--rw-r--r--   0        0        0     5052 2024-03-25 20:00:43.991391 longship-2024.4.15/longship_api_client/api/tariffs/tariff_put.py
--rw-r--r--   0        0        0        0 2024-03-25 19:42:52.320418 longship-2024.4.15/longship_api_client/api/webhooks/__init__.py
--rw-r--r--   0        0        0     8087 2024-03-25 20:00:43.991710 longship-2024.4.15/longship_api_client/api/webhooks/get_all_webhooks.py
--rw-r--r--   0        0        0     4365 2024-03-25 19:42:53.011639 longship-2024.4.15/longship_api_client/api/webhooks/webhook_delete.py
--rw-r--r--   0        0        0     4586 2024-03-25 19:42:53.011295 longship-2024.4.15/longship_api_client/api/webhooks/webhook_get.py
--rw-r--r--   0        0        0     4856 2024-03-25 20:00:43.992017 longship-2024.4.15/longship_api_client/api/webhooks/webhook_post.py
--rw-r--r--   0        0        0     5248 2024-03-25 20:00:43.992356 longship-2024.4.15/longship_api_client/api/webhooks/webhook_put.py
--rw-r--r--   0        0        0    12209 2024-03-25 19:42:53.022999 longship-2024.4.15/longship_api_client/client.py
--rw-r--r--   0        0        0      546 2024-03-25 19:42:53.007596 longship-2024.4.15/longship_api_client/errors.py
--rw-r--r--   0        0        0    22439 2024-03-25 19:42:53.021268 longship-2024.4.15/longship_api_client/models/__init__.py
--rw-r--r--   0        0        0     2637 2024-03-25 20:16:22.035460 longship-2024.4.15/longship_api_client/models/additional_geo_location_dto.py
--rw-r--r--   0        0        0     3671 2024-03-25 20:16:03.746432 longship-2024.4.15/longship_api_client/models/authorization_assertion_dto.py
--rw-r--r--   0        0        0      644 2024-03-25 19:42:53.007525 longship-2024.4.15/longship_api_client/models/authorization_assertion_dto_auth_scenario_type.py
--rw-r--r--   0        0        0      278 2024-03-25 19:42:53.011158 longship-2024.4.15/longship_api_client/models/authorization_assertion_dto_status.py
--rw-r--r--   0        0        0     3446 2024-03-25 19:42:53.013517 longship-2024.4.15/longship_api_client/models/authorization_charger_context_dto.py
--rw-r--r--   0        0        0     3198 2024-03-25 20:16:06.745858 longship-2024.4.15/longship_api_client/models/authorization_context_details_dto.py
--rw-r--r--   0        0        0     2334 2024-03-25 20:16:17.147771 longship-2024.4.15/longship_api_client/models/authorization_data.py
--rw-r--r--   0        0        0     4295 2024-03-25 20:16:17.147874 longship-2024.4.15/longship_api_client/models/authorization_result_dto.py
--rw-r--r--   0        0        0      895 2024-03-25 19:42:53.014619 longship-2024.4.15/longship_api_client/models/authorization_result_dto_reason.py
--rw-r--r--   0        0        0      289 2024-03-25 19:42:53.019455 longship-2024.4.15/longship_api_client/models/authorization_result_dto_status.py
--rw-r--r--   0        0        0     2524 2024-03-25 19:42:53.009051 longship-2024.4.15/longship_api_client/models/authorization_tenant_context_dto.py
--rw-r--r--   0        0        0     2507 2024-03-25 20:01:26.710827 longship-2024.4.15/longship_api_client/models/business_details_dto.py
--rw-r--r--   0        0        0     1604 2024-03-25 19:42:53.025922 longship-2024.4.15/longship_api_client/models/cancel_reservation_request.py
--rw-r--r--   0        0        0    16774 2024-03-25 20:16:17.147727 longship-2024.4.15/longship_api_client/models/cdr_dto.py
--rw-r--r--   0        0        0      177 2024-03-25 19:42:53.018594 longship-2024.4.15/longship_api_client/models/cdr_dto_approval_status.py
--rw-r--r--   0        0        0      166 2024-03-25 19:42:53.011820 longship-2024.4.15/longship_api_client/models/cdr_dto_financial_type.py
--rw-r--r--   0        0        0     1903 2024-03-25 19:42:53.021004 longship-2024.4.15/longship_api_client/models/cdr_geo_location_dto.py
--rw-r--r--   0        0        0     6896 2024-03-25 20:16:17.145392 longship-2024.4.15/longship_api_client/models/cdr_location_dto.py
--rw-r--r--   0        0        0      202 2024-03-25 19:42:53.020295 longship-2024.4.15/longship_api_client/models/cdr_location_dto_power_type.py
--rw-r--r--   0        0        0     2261 2024-03-25 20:16:17.145494 longship-2024.4.15/longship_api_client/models/cdr_patch_dto.py
--rw-r--r--   0        0        0      182 2024-03-25 19:42:53.016250 longship-2024.4.15/longship_api_client/models/cdr_patch_dto_approval_status.py
--rw-r--r--   0        0        0     5453 2024-03-25 20:16:17.145534 longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto.py
--rw-r--r--   0        0        0      668 2024-03-25 19:42:53.020391 longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0      185 2024-03-25 19:42:53.015245 longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto_roaming_platform_type.py
--rw-r--r--   0        0        0     5677 2024-03-25 20:16:17.145633 longship-2024.4.15/longship_api_client/models/cdr_started_by_token_dto.py
--rw-r--r--   0        0        0      221 2024-03-25 19:42:53.015398 longship-2024.4.15/longship_api_client/models/cdr_started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      230 2024-03-25 19:42:53.020906 longship-2024.4.15/longship_api_client/models/cdr_started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     2004 2024-03-25 19:42:53.011062 longship-2024.4.15/longship_api_client/models/change_availability_request.py
--rw-r--r--   0        0        0      194 2024-03-25 19:42:53.014134 longship-2024.4.15/longship_api_client/models/change_availability_request_type.py
--rw-r--r--   0        0        0     1659 2024-03-25 19:42:53.012267 longship-2024.4.15/longship_api_client/models/change_configuration_request.py
--rw-r--r--   0        0        0     6741 2024-03-25 20:16:17.148174 longship-2024.4.15/longship_api_client/models/charge_point_authorize_get_dto.py
--rw-r--r--   0        0        0      247 2024-03-25 19:42:53.016677 longship-2024.4.15/longship_api_client/models/charge_point_authorize_get_dto_authorization_request_type.py
--rw-r--r--   0        0        0     1952 2024-03-25 19:42:53.023232 longship-2024.4.15/longship_api_client/models/charge_point_authorize_post_dto.py
--rw-r--r--   0        0        0     3974 2024-03-25 20:16:17.145652 longship-2024.4.15/longship_api_client/models/chargepoint_configuration_items_dto.py
--rw-r--r--   0        0        0     6602 2024-03-25 20:16:17.147802 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto.py
--rw-r--r--   0        0        0      176 2024-03-25 19:42:53.009231 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_format.py
--rw-r--r--   0        0        0      405 2024-03-25 19:42:53.018023 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_operational_status.py
--rw-r--r--   0        0        0      211 2024-03-25 19:42:53.010045 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_power_type.py
--rw-r--r--   0        0        0     1100 2024-03-25 19:42:53.018437 longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_standard.py
--rw-r--r--   0        0        0    17389 2024-03-25 20:16:17.145591 longship-2024.4.15/longship_api_client/models/chargepoint_dto.py
--rw-r--r--   0        0        0      183 2024-03-25 19:42:53.011286 longship-2024.4.15/longship_api_client/models/chargepoint_dto_connectivity_status.py
--rw-r--r--   0        0        0     2642 2024-03-25 19:42:53.024330 longship-2024.4.15/longship_api_client/models/chargepoint_evse_dto.py
--rw-r--r--   0        0        0     3811 2024-03-25 19:42:53.007865 longship-2024.4.15/longship_api_client/models/chargepoint_put_dto.py
--rw-r--r--   0        0        0     7493 2024-03-25 20:16:17.145543 longship-2024.4.15/longship_api_client/models/chargepoint_status_dto.py
--rw-r--r--   0        0        0      189 2024-03-25 19:42:53.009010 longship-2024.4.15/longship_api_client/models/chargepoint_status_dto_connectivity_status.py
--rw-r--r--   0        0        0     3910 2024-03-25 20:16:17.145642 longship-2024.4.15/longship_api_client/models/charging_meter_value_dto.py
--rw-r--r--   0        0        0     1197 2024-03-25 19:42:53.007491 longship-2024.4.15/longship_api_client/models/charging_meter_value_dto_measurand.py
--rw-r--r--   0        0        0      402 2024-03-25 19:42:53.023405 longship-2024.4.15/longship_api_client/models/charging_meter_value_dto_unit.py
--rw-r--r--   0        0        0     3263 2024-03-25 20:16:17.147852 longship-2024.4.15/longship_api_client/models/charging_period_dto.py
--rw-r--r--   0        0        0     6374 2024-03-25 20:16:17.147690 longship-2024.4.15/longship_api_client/models/charging_profile.py
--rw-r--r--   0        0        0      219 2024-03-25 19:42:53.008080 longship-2024.4.15/longship_api_client/models/charging_profile_charging_profile_kind.py
--rw-r--r--   0        0        0      264 2024-03-25 19:42:53.011335 longship-2024.4.15/longship_api_client/models/charging_profile_charging_profile_purpose.py
--rw-r--r--   0        0        0      176 2024-03-25 19:42:53.018510 longship-2024.4.15/longship_api_client/models/charging_profile_recurrency_kind.py
--rw-r--r--   0        0        0     4491 2024-03-25 20:16:17.145717 longship-2024.4.15/longship_api_client/models/charging_schedule.py
--rw-r--r--   0        0        0      161 2024-03-25 19:42:53.009681 longship-2024.4.15/longship_api_client/models/charging_schedule_charging_rate_unit.py
--rw-r--r--   0        0        0     2112 2024-03-25 19:42:53.022080 longship-2024.4.15/longship_api_client/models/charging_schedule_period.py
--rw-r--r--   0        0        0     1234 2024-03-25 19:42:53.014036 longship-2024.4.15/longship_api_client/models/clear_cache_request.py
--rw-r--r--   0        0        0     3655 2024-03-25 20:16:17.145699 longship-2024.4.15/longship_api_client/models/clear_charging_profile_request.py
--rw-r--r--   0        0        0      276 2024-03-25 19:42:53.008242 longship-2024.4.15/longship_api_client/models/clear_charging_profile_request_charging_profile_purpose.py
--rw-r--r--   0        0        0     5941 2024-03-25 20:16:17.148149 longship-2024.4.15/longship_api_client/models/connector_dto.py
--rw-r--r--   0        0        0      165 2024-03-25 19:42:53.010260 longship-2024.4.15/longship_api_client/models/connector_dto_format.py
--rw-r--r--   0        0        0      200 2024-03-25 19:42:53.025462 longship-2024.4.15/longship_api_client/models/connector_dto_power_type.py
--rw-r--r--   0        0        0     1089 2024-03-25 19:42:53.013664 longship-2024.4.15/longship_api_client/models/connector_dto_standard.py
--rw-r--r--   0        0        0     3663 2024-03-25 20:16:17.145707 longship-2024.4.15/longship_api_client/models/connector_operational_status_dto.py
--rw-r--r--   0        0        0      411 2024-03-25 19:42:53.023397 longship-2024.4.15/longship_api_client/models/connector_operational_status_dto_operational_status.py
--rw-r--r--   0        0        0     6482 2024-03-25 20:16:17.256119 longship-2024.4.15/longship_api_client/models/cs_charging_profiles.py
--rw-r--r--   0        0        0      222 2024-03-25 19:42:53.021273 longship-2024.4.15/longship_api_client/models/cs_charging_profiles_charging_profile_kind.py
--rw-r--r--   0        0        0      267 2024-03-25 19:42:53.020067 longship-2024.4.15/longship_api_client/models/cs_charging_profiles_charging_profile_purpose.py
--rw-r--r--   0        0        0      179 2024-03-25 19:42:53.023924 longship-2024.4.15/longship_api_client/models/cs_charging_profiles_recurrency_kind.py
--rw-r--r--   0        0        0     2101 2024-03-25 19:42:53.016959 longship-2024.4.15/longship_api_client/models/data_transfer_request.py
--rw-r--r--   0        0        0     1830 2024-03-25 19:42:53.020953 longship-2024.4.15/longship_api_client/models/display_text_dto.py
--rw-r--r--   0        0        0     3861 2024-03-25 19:42:53.020545 longship-2024.4.15/longship_api_client/models/energy_mix_dto.py
--rw-r--r--   0        0        0     2351 2024-03-25 20:16:17.145600 longship-2024.4.15/longship_api_client/models/energy_source_dto.py
--rw-r--r--   0        0        0      316 2024-03-25 19:42:53.012770 longship-2024.4.15/longship_api_client/models/energy_source_dto_source.py
--rw-r--r--   0        0        0     2298 2024-03-25 20:16:17.145551 longship-2024.4.15/longship_api_client/models/entity_tag_header_value.py
--rw-r--r--   0        0        0     2480 2024-03-25 20:16:17.147583 longship-2024.4.15/longship_api_client/models/environmental_impact_dto.py
--rw-r--r--   0        0        0      209 2024-03-25 19:42:53.026019 longship-2024.4.15/longship_api_client/models/environmental_impact_dto_category.py
--rw-r--r--   0        0        0     2743 2024-03-25 20:16:17.119953 longship-2024.4.15/longship_api_client/models/exceptional_period_dto.py
--rw-r--r--   0        0        0     4820 2024-03-25 20:16:17.148052 longship-2024.4.15/longship_api_client/models/file_content_result.py
--rw-r--r--   0        0        0     1885 2024-03-25 19:42:53.012418 longship-2024.4.15/longship_api_client/models/geo_location_dto.py
--rw-r--r--   0        0        0      190 2024-03-25 19:42:53.008926 longship-2024.4.15/longship_api_client/models/get_all_cdrs_order_by.py
--rw-r--r--   0        0        0      215 2024-03-25 19:42:53.021733 longship-2024.4.15/longship_api_client/models/get_all_chargepoints_accesstype.py
--rw-r--r--   0        0        0      167 2024-03-25 19:42:53.025610 longship-2024.4.15/longship_api_client/models/get_all_chargepoints_chargerpowertype.py
--rw-r--r--   0        0        0      400 2024-03-25 19:42:53.024331 longship-2024.4.15/longship_api_client/models/get_all_chargepoints_operationalstatus.py
--rw-r--r--   0        0        0      224 2024-03-25 19:42:53.016650 longship-2024.4.15/longship_api_client/models/get_all_chargepoints_order_by.py
--rw-r--r--   0        0        0      232 2024-03-25 19:42:53.013135 longship-2024.4.15/longship_api_client/models/get_all_locations_accesstype.py
--rw-r--r--   0        0        0      164 2024-03-25 19:42:53.017035 longship-2024.4.15/longship_api_client/models/get_all_locations_chargerpowertype.py
--rw-r--r--   0        0        0      191 2024-03-25 19:42:53.013268 longship-2024.4.15/longship_api_client/models/get_all_locations_order_by.py
--rw-r--r--   0        0        0      203 2024-03-25 19:42:53.009543 longship-2024.4.15/longship_api_client/models/get_all_reimbursementcdrs_order_by.py
--rw-r--r--   0        0        0      164 2024-03-25 19:42:53.025145 longship-2024.4.15/longship_api_client/models/get_all_sessions_order_by.py
--rw-r--r--   0        0        0      221 2024-03-25 19:42:53.016938 longship-2024.4.15/longship_api_client/models/get_all_tariffdistributions_order_by.py
--rw-r--r--   0        0        0      203 2024-03-25 19:42:53.024996 longship-2024.4.15/longship_api_client/models/get_all_tariffs_order_by.py
--rw-r--r--   0        0        0      144 2024-03-25 19:42:53.012343 longship-2024.4.15/longship_api_client/models/get_all_webhooks_order_by.py
--rw-r--r--   0        0        0     3021 2024-03-25 20:16:17.147746 longship-2024.4.15/longship_api_client/models/get_composite_schedule_request.py
--rw-r--r--   0        0        0      172 2024-03-25 19:42:53.013558 longship-2024.4.15/longship_api_client/models/get_composite_schedule_request_charging_rate_unit.py
--rw-r--r--   0        0        0     1742 2024-03-25 20:00:43.999594 longship-2024.4.15/longship_api_client/models/get_configuration_request.py
--rw-r--r--   0        0        0     3494 2024-03-25 20:16:17.147616 longship-2024.4.15/longship_api_client/models/get_diagnostics_request.py
--rw-r--r--   0        0        0     1285 2024-03-25 19:42:53.022880 longship-2024.4.15/longship_api_client/models/get_local_list_version_request.py
--rw-r--r--   0        0        0     5058 2024-03-25 20:00:43.999981 longship-2024.4.15/longship_api_client/models/hours_dto.py
--rw-r--r--   0        0        0     2708 2024-03-25 20:16:17.147923 longship-2024.4.15/longship_api_client/models/id_tag_info.py
--rw-r--r--   0        0        0      252 2024-03-25 19:42:53.014006 longship-2024.4.15/longship_api_client/models/id_tag_info_status.py
--rw-r--r--   0        0        0     3271 2024-03-25 20:16:17.145569 longship-2024.4.15/longship_api_client/models/image_dto.py
--rw-r--r--   0        0        0      287 2024-03-25 19:42:53.010942 longship-2024.4.15/longship_api_client/models/image_dto_category.py
--rw-r--r--   0        0        0     8733 2024-03-25 20:16:17.148073 longship-2024.4.15/longship_api_client/models/interchange_format_cdr.py
--rw-r--r--   0        0        0     5819 2024-03-25 20:16:17.119922 longship-2024.4.15/longship_api_client/models/local_token_group_get_dto.py
--rw-r--r--   0        0        0     4431 2024-03-25 19:42:53.011938 longship-2024.4.15/longship_api_client/models/local_token_group_post_dto.py
--rw-r--r--   0        0        0     4394 2024-03-25 19:42:53.010143 longship-2024.4.15/longship_api_client/models/local_token_group_put_dto.py
--rw-r--r--   0        0        0     2829 2024-03-25 19:42:53.012581 longship-2024.4.15/longship_api_client/models/local_token_group_token_get_dto.py
--rw-r--r--   0        0        0     2416 2024-03-25 19:42:53.020751 longship-2024.4.15/longship_api_client/models/local_token_group_token_post_dto.py
--rw-r--r--   0        0        0     2411 2024-03-25 19:42:53.025595 longship-2024.4.15/longship_api_client/models/local_token_group_token_put_dto.py
--rw-r--r--   0        0        0     1722 2024-03-25 19:42:53.012238 longship-2024.4.15/longship_api_client/models/location_charge_point_dto.py
--rw-r--r--   0        0        0    19679 2024-03-25 20:16:17.112028 longship-2024.4.15/longship_api_client/models/location_dto.py
--rw-r--r--   0        0        0      706 2024-03-25 19:42:53.011179 longship-2024.4.15/longship_api_client/models/location_dto_facilities_item.py
--rw-r--r--   0        0        0      341 2024-03-25 19:42:53.021534 longship-2024.4.15/longship_api_client/models/location_dto_parking_type.py
--rw-r--r--   0        0        0    11826 2024-03-25 20:16:17.145579 longship-2024.4.15/longship_api_client/models/location_evse_dto.py
--rw-r--r--   0        0        0      698 2024-03-25 19:42:53.012072 longship-2024.4.15/longship_api_client/models/location_evse_dto_capabilities_item.py
--rw-r--r--   0        0        0      277 2024-03-25 19:42:53.009142 longship-2024.4.15/longship_api_client/models/location_evse_dto_parking_restrictions_item.py
--rw-r--r--   0        0        0      364 2024-03-25 19:42:53.014428 longship-2024.4.15/longship_api_client/models/location_evse_dto_status.py
--rw-r--r--   0        0        0    18562 2024-03-25 20:16:17.147645 longship-2024.4.15/longship_api_client/models/location_post_dto.py
--rw-r--r--   0        0        0      710 2024-03-25 19:42:53.024083 longship-2024.4.15/longship_api_client/models/location_post_dto_facilities_item.py
--rw-r--r--   0        0        0      345 2024-03-25 19:42:53.009734 longship-2024.4.15/longship_api_client/models/location_post_dto_parking_type.py
--rw-r--r--   0        0        0    19439 2024-03-25 20:16:17.148097 longship-2024.4.15/longship_api_client/models/location_put_dto.py
--rw-r--r--   0        0        0      709 2024-03-25 19:42:53.024738 longship-2024.4.15/longship_api_client/models/location_put_dto_facilities_item.py
--rw-r--r--   0        0        0      344 2024-03-25 19:42:53.025234 longship-2024.4.15/longship_api_client/models/location_put_dto_parking_type.py
--rw-r--r--   0        0        0     1957 2024-03-25 20:00:44.002906 longship-2024.4.15/longship_api_client/models/location_tariff_distribution_dto.py
--rw-r--r--   0        0        0     2508 2024-03-25 20:16:17.145478 longship-2024.4.15/longship_api_client/models/longship_error.py
--rw-r--r--   0        0        0     2024 2024-03-25 19:42:53.020751 longship-2024.4.15/longship_api_client/models/longship_error_detail.py
--rw-r--r--   0        0        0     6167 2024-03-25 20:16:17.147668 longship-2024.4.15/longship_api_client/models/message_log_dto.py
--rw-r--r--   0        0        0      219 2024-03-25 19:42:53.023217 longship-2024.4.15/longship_api_client/models/message_log_dto_direction.py
--rw-r--r--   0        0        0     1335 2024-03-25 19:42:53.013169 longship-2024.4.15/longship_api_client/models/message_log_dto_ocpp_message_type.py
--rw-r--r--   0        0        0      227 2024-03-25 19:42:53.009907 longship-2024.4.15/longship_api_client/models/message_log_dto_wamp_message_type.py
--rw-r--r--   0        0        0     2240 2024-03-25 19:42:53.013023 longship-2024.4.15/longship_api_client/models/organization_unit_financial_details_dto.py
--rw-r--r--   0        0        0    10170 2024-03-25 20:16:17.147951 longship-2024.4.15/longship_api_client/models/organization_unit_get_dto.py
--rw-r--r--   0        0        0     9395 2024-03-25 20:16:17.147828 longship-2024.4.15/longship_api_client/models/organization_unit_post_dto.py
--rw-r--r--   0        0        0     9143 2024-03-25 20:16:17.145690 longship-2024.4.15/longship_api_client/models/organization_unit_put_dto.py
--rw-r--r--   0        0        0     4903 2024-03-25 19:42:53.018883 longship-2024.4.15/longship_api_client/models/price_info_dto.py
--rw-r--r--   0        0        0     3457 2024-03-25 20:16:17.145445 longship-2024.4.15/longship_api_client/models/private_emp_tariff_dto.py
--rw-r--r--   0        0        0      161 2024-03-25 19:42:53.013747 longship-2024.4.15/longship_api_client/models/private_emp_tariff_dto_power_type.py
--rw-r--r--   0        0        0     3107 2024-03-25 20:16:17.145610 longship-2024.4.15/longship_api_client/models/publish_token_type_dto.py
--rw-r--r--   0        0        0      224 2024-03-25 19:42:53.020185 longship-2024.4.15/longship_api_client/models/publish_token_type_dto_type.py
--rw-r--r--   0        0        0     2202 2024-03-25 19:42:53.008000 longship-2024.4.15/longship_api_client/models/regular_hours_dto.py
--rw-r--r--   0        0        0    11559 2024-03-25 20:16:17.145620 longship-2024.4.15/longship_api_client/models/reimburse_info_dto.py
--rw-r--r--   0        0        0      205 2024-03-25 19:42:53.009099 longship-2024.4.15/longship_api_client/models/reimburse_info_dto_type.py
--rw-r--r--   0        0        0     4113 2024-03-25 20:16:17.120003 longship-2024.4.15/longship_api_client/models/reimburse_started_by_info_dto.py
--rw-r--r--   0        0        0      674 2024-03-25 19:42:53.020677 longship-2024.4.15/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0     5833 2024-03-25 20:16:17.145452 longship-2024.4.15/longship_api_client/models/reimburse_started_by_token_dto.py
--rw-r--r--   0        0        0      227 2024-03-25 19:42:53.007686 longship-2024.4.15/longship_api_client/models/reimburse_started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      236 2024-03-25 19:42:53.014059 longship-2024.4.15/longship_api_client/models/reimburse_started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     3078 2024-03-25 20:16:17.148013 longship-2024.4.15/longship_api_client/models/reimbursement_bank_details_dto.py
--rw-r--r--   0        0        0    21978 2024-03-25 20:16:17.145414 longship-2024.4.15/longship_api_client/models/reimbursement_cdr_dto.py
--rw-r--r--   0        0        0     1971 2024-03-25 19:42:53.010185 longship-2024.4.15/longship_api_client/models/reimbursement_cdr_geo_location_dto.py
--rw-r--r--   0        0        0     7238 2024-03-25 20:16:17.145366 longship-2024.4.15/longship_api_client/models/reimbursement_cdr_location_dto.py
--rw-r--r--   0        0        0      215 2024-03-25 19:42:53.014885 longship-2024.4.15/longship_api_client/models/reimbursement_cdr_location_dto_power_type.py
--rw-r--r--   0        0        0     2435 2024-03-25 19:42:53.015118 longship-2024.4.15/longship_api_client/models/reimbursement_customer_share_dto.py
--rw-r--r--   0        0        0     1917 2024-03-25 19:42:53.007776 longship-2024.4.15/longship_api_client/models/reimbursement_price_dto.py
--rw-r--r--   0        0        0     4783 2024-03-25 20:16:17.148122 longship-2024.4.15/longship_api_client/models/reimbursement_tariff_dto.py
--rw-r--r--   0        0        0      209 2024-03-25 19:42:53.017372 longship-2024.4.15/longship_api_client/models/reimbursement_tariff_dto_status.py
--rw-r--r--   0        0        0     2853 2024-03-25 20:16:17.145486 longship-2024.4.15/longship_api_client/models/remote_start_transaction_request.py
--rw-r--r--   0        0        0     1627 2024-03-25 19:42:53.008755 longship-2024.4.15/longship_api_client/models/remote_stop_transaction_request.py
--rw-r--r--   0        0        0     2644 2024-03-25 20:00:44.006730 longship-2024.4.15/longship_api_client/models/reserve_now_request.py
--rw-r--r--   0        0        0     1609 2024-03-25 19:42:53.019871 longship-2024.4.15/longship_api_client/models/reset_request.py
--rw-r--r--   0        0        0      157 2024-03-25 19:42:53.016585 longship-2024.4.15/longship_api_client/models/reset_request_type.py
--rw-r--r--   0        0        0     3534 2024-03-25 19:42:53.008207 longship-2024.4.15/longship_api_client/models/send_local_list_request.py
--rw-r--r--   0        0        0      187 2024-03-25 19:42:53.008152 longship-2024.4.15/longship_api_client/models/send_local_list_request_update_type.py
--rw-r--r--   0        0        0    20526 2024-03-25 20:16:17.147904 longship-2024.4.15/longship_api_client/models/session_dto.py
--rw-r--r--   0        0        0      194 2024-03-25 19:42:53.016855 longship-2024.4.15/longship_api_client/models/session_dto_approval_status.py
--rw-r--r--   0        0        0      166 2024-03-25 19:42:53.022905 longship-2024.4.15/longship_api_client/models/session_dto_review_scenario_type.py
--rw-r--r--   0        0        0      251 2024-03-25 19:42:53.022178 longship-2024.4.15/longship_api_client/models/session_dto_status.py
--rw-r--r--   0        0        0     1923 2024-03-25 19:42:53.012037 longship-2024.4.15/longship_api_client/models/session_geo_location_dto.py
--rw-r--r--   0        0        0     6980 2024-03-25 20:16:17.145434 longship-2024.4.15/longship_api_client/models/session_location_dto.py
--rw-r--r--   0        0        0      206 2024-03-25 19:42:53.009978 longship-2024.4.15/longship_api_client/models/session_location_dto_power_type.py
--rw-r--r--   0        0        0     3985 2024-03-25 20:16:17.145661 longship-2024.4.15/longship_api_client/models/session_threshold_check_dto.py
--rw-r--r--   0        0        0      265 2024-03-25 19:42:53.014604 longship-2024.4.15/longship_api_client/models/session_threshold_check_dto_status.py
--rw-r--r--   0        0        0      204 2024-03-25 19:42:53.023710 longship-2024.4.15/longship_api_client/models/session_threshold_check_dto_threshold_hit_outcome.py
--rw-r--r--   0        0        0     4525 2024-03-25 20:16:17.145378 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_decimal.py
--rw-r--r--   0        0        0      272 2024-03-25 19:42:53.024219 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_decimal_status.py
--rw-r--r--   0        0        0      211 2024-03-25 19:42:53.023536 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_decimal_threshold_hit_outcome.py
--rw-r--r--   0        0        0     4484 2024-03-25 20:16:17.145503 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_int_32.py
--rw-r--r--   0        0        0      270 2024-03-25 19:42:53.025721 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_int_32_status.py
--rw-r--r--   0        0        0      209 2024-03-25 19:42:53.011068 longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_int_32_threshold_hit_outcome.py
--rw-r--r--   0        0        0    10975 2024-03-25 20:16:17.145734 longship-2024.4.15/longship_api_client/models/session_thresholds_dto.py
--rw-r--r--   0        0        0      462 2024-03-25 19:42:53.010379 longship-2024.4.15/longship_api_client/models/session_thresholds_dto_thresholds_hit_item.py
--rw-r--r--   0        0        0     2133 2024-03-25 19:42:53.011494 longship-2024.4.15/longship_api_client/models/set_charging_profile_request.py
--rw-r--r--   0        0        0     5359 2024-03-25 20:16:17.145671 longship-2024.4.15/longship_api_client/models/started_by_info_dto.py
--rw-r--r--   0        0        0      665 2024-03-25 19:42:53.016182 longship-2024.4.15/longship_api_client/models/started_by_info_dto_authorization_state.py
--rw-r--r--   0        0        0      182 2024-03-25 19:42:53.013508 longship-2024.4.15/longship_api_client/models/started_by_info_dto_roaming_platform_type.py
--rw-r--r--   0        0        0     5597 2024-03-25 20:16:17.147985 longship-2024.4.15/longship_api_client/models/started_by_token_dto.py
--rw-r--r--   0        0        0      218 2024-03-25 19:42:53.016010 longship-2024.4.15/longship_api_client/models/started_by_token_dto_auth_method.py
--rw-r--r--   0        0        0      227 2024-03-25 19:42:53.023627 longship-2024.4.15/longship_api_client/models/started_by_token_dto_token_type.py
--rw-r--r--   0        0        0     3466 2024-03-25 20:16:17.120060 longship-2024.4.15/longship_api_client/models/status_schedule_dto.py
--rw-r--r--   0        0        0      366 2024-03-25 19:42:53.021753 longship-2024.4.15/longship_api_client/models/status_schedule_dto_status.py
--rw-r--r--   0        0        0     2582 2024-03-25 19:42:53.021647 longship-2024.4.15/longship_api_client/models/string_segment.py
--rw-r--r--   0        0        0     2931 2024-03-25 20:16:17.145561 longship-2024.4.15/longship_api_client/models/tariff_assertion_dto.py
--rw-r--r--   0        0        0      283 2024-03-25 19:42:53.021845 longship-2024.4.15/longship_api_client/models/tariff_assertion_dto_tariff_type.py
--rw-r--r--   0        0        0     6670 2024-03-25 20:16:17.145469 longship-2024.4.15/longship_api_client/models/tariff_distribution_get_dto.py
--rw-r--r--   0        0        0     3746 2024-03-25 20:16:17.120079 longship-2024.4.15/longship_api_client/models/tariff_distribution_history_dto.py
--rw-r--r--   0        0        0     3517 2024-03-25 19:42:53.019575 longship-2024.4.15/longship_api_client/models/tariff_distribution_post_dto.py
--rw-r--r--   0        0        0     3512 2024-03-25 19:42:53.024792 longship-2024.4.15/longship_api_client/models/tariff_distribution_put_dto.py
--rw-r--r--   0        0        0    14806 2024-03-25 20:16:17.145460 longship-2024.4.15/longship_api_client/models/tariff_dto.py
--rw-r--r--   0        0        0      186 2024-03-25 19:42:53.025570 longship-2024.4.15/longship_api_client/models/tariff_dto_tariff_type.py
--rw-r--r--   0        0        0      241 2024-03-25 19:42:53.009523 longship-2024.4.15/longship_api_client/models/tariff_dto_usage_type.py
--rw-r--r--   0        0        0     6088 2024-03-25 19:42:53.022020 longship-2024.4.15/longship_api_client/models/tariff_info_dto.py
--rw-r--r--   0        0        0     8582 2024-03-25 20:16:17.119980 longship-2024.4.15/longship_api_client/models/tariff_post_dto.py
--rw-r--r--   0        0        0      245 2024-03-25 19:42:53.009116 longship-2024.4.15/longship_api_client/models/tariff_post_dto_usage_type.py
--rw-r--r--   0        0        0     9227 2024-03-25 20:16:17.145424 longship-2024.4.15/longship_api_client/models/tariff_price_dto.py
--rw-r--r--   0        0        0      209 2024-03-25 19:42:53.023536 longship-2024.4.15/longship_api_client/models/tariff_price_dto_approval_status.py
--rw-r--r--   0        0        0     8440 2024-03-25 20:16:17.120039 longship-2024.4.15/longship_api_client/models/tariff_put_dto.py
--rw-r--r--   0        0        0     4065 2024-03-25 20:16:17.145680 longship-2024.4.15/longship_api_client/models/tariff_restriction.py
--rw-r--r--   0        0        0      244 2024-03-25 19:42:53.009878 longship-2024.4.15/longship_api_client/models/tariff_restriction_day_of_week.py
--rw-r--r--   0        0        0     2668 2024-03-25 20:16:17.145523 longship-2024.4.15/longship_api_client/models/token_info_dto.py
--rw-r--r--   0        0        0      216 2024-03-25 19:42:53.015173 longship-2024.4.15/longship_api_client/models/token_info_dto_token_type.py
--rw-r--r--   0        0        0     2385 2024-03-25 19:42:53.021311 longship-2024.4.15/longship_api_client/models/trigger_message_request.py
--rw-r--r--   0        0        0      420 2024-03-25 19:42:53.016098 longship-2024.4.15/longship_api_client/models/trigger_message_request_requested_message.py
--rw-r--r--   0        0        0     1574 2024-03-25 19:42:53.014314 longship-2024.4.15/longship_api_client/models/unlock_connector_request.py
--rw-r--r--   0        0        0     2514 2024-03-25 20:00:44.012302 longship-2024.4.15/longship_api_client/models/update_firmware_request.py
--rw-r--r--   0        0        0     5538 2024-03-25 20:16:17.145402 longship-2024.4.15/longship_api_client/models/webhook_get_dto.py
--rw-r--r--   0        0        0      578 2024-03-25 19:42:53.025317 longship-2024.4.15/longship_api_client/models/webhook_get_dto_event_types_item.py
--rw-r--r--   0        0        0     1807 2024-03-25 19:42:53.024132 longship-2024.4.15/longship_api_client/models/webhook_header_dto.py
--rw-r--r--   0        0        0     4123 2024-03-25 20:00:44.013135 longship-2024.4.15/longship_api_client/models/webhook_post_dto.py
--rw-r--r--   0        0        0      579 2024-03-25 19:42:53.011270 longship-2024.4.15/longship_api_client/models/webhook_post_dto_event_types_item.py
--rw-r--r--   0        0        0     4113 2024-03-25 19:42:53.010850 longship-2024.4.15/longship_api_client/models/webhook_put_dto.py
--rw-r--r--   0        0        0      578 2024-03-25 19:42:53.014129 longship-2024.4.15/longship_api_client/models/webhook_put_dto_event_types_item.py
--rw-r--r--   0        0        0     4250 2024-03-25 20:16:17.145514 longship-2024.4.15/longship_api_client/models/webhook_summary_get_dto.py
--rw-r--r--   0        0        0      585 2024-03-25 19:42:53.012248 longship-2024.4.15/longship_api_client/models/webhook_summary_get_dto_event_types_item.py
--rw-r--r--   0        0        0       25 2024-03-25 19:42:52.041583 longship-2024.4.15/longship_api_client/py.typed
--rw-r--r--   0        0        0      985 2024-03-25 19:42:53.022168 longship-2024.4.15/longship_api_client/types.py
--rw-r--r--   0        0        0      818 2024-04-15 16:03:15.114118 longship-2024.4.15/pyproject.toml
--rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 longship-2024.4.15/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-26 16:00:19.878825 longship-2024.4.17/LICENSE
+-rw-r--r--   0        0        0     4661 2023-06-26 16:47:23.288883 longship-2024.4.17/README.md
+-rw-r--r--   0        0        0     7668 2024-03-14 10:00:43.390594 longship-2024.4.17/longship/client.py
+-rw-r--r--   0        0        0      112 2023-06-26 16:00:19.886682 longship-2024.4.17/longship/errors.py
+-rw-r--r--   0        0        0     4711 2024-04-17 14:40:28.676585 longship-2024.4.17/longship/types.py
+-rw-r--r--   0        0        0      155 2024-03-25 19:42:53.022260 longship-2024.4.17/longship_api_client/__init__.py
+-rw-r--r--   0        0        0       45 2024-03-25 19:42:53.025427 longship-2024.4.17/longship_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.296257 longship-2024.4.17/longship_api_client/api/cdrs/__init__.py
+-rw-r--r--   0        0        0     4458 2024-03-25 20:00:43.969808 longship-2024.4.17/longship_api_client/api/cdrs/cdr_get.py
+-rw-r--r--   0        0        0     5023 2024-03-25 20:00:43.970406 longship-2024.4.17/longship_api_client/api/cdrs/cdr_patch.py
+-rw-r--r--   0        0        0    19502 2024-03-25 20:00:43.970703 longship-2024.4.17/longship_api_client/api/cdrs/get_all_cdrs.py
+-rw-r--r--   0        0        0     7993 2024-03-25 20:00:43.971091 longship-2024.4.17/longship_api_client/api/cdrs/get_all_interchangeformat.py
+-rw-r--r--   0        0        0     5989 2024-03-25 20:00:43.971416 longship-2024.4.17/longship_api_client/api/cdrs/get_file_full_download_cdrs.py
+-rw-r--r--   0        0        0     5968 2024-03-25 20:00:43.971772 longship-2024.4.17/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.288563 longship-2024.4.17/longship_api_client/api/chargepoint_status/__init__.py
+-rw-r--r--   0        0        0     4767 2024-03-25 20:00:43.972132 longship-2024.4.17/longship_api_client/api/chargepoint_status/chargepoint_status_get.py
+-rw-r--r--   0        0        0     6490 2024-03-25 20:00:43.972453 longship-2024.4.17/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.289893 longship-2024.4.17/longship_api_client/api/chargepoints/__init__.py
+-rw-r--r--   0        0        0     4634 2024-03-25 20:00:43.972876 longship-2024.4.17/longship_api_client/api/chargepoints/chargepoint_get.py
+-rw-r--r--   0        0        0     5162 2024-03-25 20:00:43.973593 longship-2024.4.17/longship_api_client/api/chargepoints/chargepoint_put.py
+-rw-r--r--   0        0        0     5416 2024-03-25 20:00:43.973998 longship-2024.4.17/longship_api_client/api/chargepoints/chargepointauthorization_get.py
+-rw-r--r--   0        0        0     5252 2024-03-25 20:00:43.976187 longship-2024.4.17/longship_api_client/api/chargepoints/chargepointauthorization_post.py
+-rw-r--r--   0        0        0     9920 2024-03-25 20:00:43.976569 longship-2024.4.17/longship_api_client/api/chargepoints/get_all_chargepointauthorizations.py
+-rw-r--r--   0        0        0    11723 2024-03-25 20:00:43.976947 longship-2024.4.17/longship_api_client/api/chargepoints/get_all_chargepointmessages.py
+-rw-r--r--   0        0        0    16896 2024-03-25 20:00:43.977268 longship-2024.4.17/longship_api_client/api/chargepoints/get_all_chargepoints.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.307087 longship-2024.4.17/longship_api_client/api/commands/__init__.py
+-rw-r--r--   0        0        0     5151 2024-03-25 20:00:43.977620 longship-2024.4.17/longship_api_client/api/commands/send_cancel_reservation_request.py
+-rw-r--r--   0        0        0     5171 2024-03-25 20:00:43.978017 longship-2024.4.17/longship_api_client/api/commands/send_change_availability_request.py
+-rw-r--r--   0        0        0     5191 2024-03-25 20:00:43.978353 longship-2024.4.17/longship_api_client/api/commands/send_change_configuration_request.py
+-rw-r--r--   0        0        0     5011 2024-03-25 19:42:53.020065 longship-2024.4.17/longship_api_client/api/commands/send_clear_cache_request.py
+-rw-r--r--   0        0        0     5212 2024-03-25 20:00:43.978639 longship-2024.4.17/longship_api_client/api/commands/send_clear_charging_profile_request.py
+-rw-r--r--   0        0        0     5051 2024-03-25 20:00:43.979167 longship-2024.4.17/longship_api_client/api/commands/send_data_transfer_request.py
+-rw-r--r--   0        0        0     5212 2024-03-25 20:00:43.979385 longship-2024.4.17/longship_api_client/api/commands/send_get_composite_schedule_request.py
+-rw-r--r--   0        0        0     5131 2024-03-25 19:42:53.015992 longship-2024.4.17/longship_api_client/api/commands/send_get_configuration_request.py
+-rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.979633 longship-2024.4.17/longship_api_client/api/commands/send_get_diagnostics_request.py
+-rw-r--r--   0        0        0     5193 2024-03-25 20:00:43.979964 longship-2024.4.17/longship_api_client/api/commands/send_get_local_list_version_request.py
+-rw-r--r--   0        0        0     5241 2024-03-25 20:00:43.980364 longship-2024.4.17/longship_api_client/api/commands/send_remote_start_transaction_request.py
+-rw-r--r--   0        0        0     5221 2024-03-25 20:00:43.980710 longship-2024.4.17/longship_api_client/api/commands/send_remote_stop_transaction_request.py
+-rw-r--r--   0        0        0     5011 2024-03-25 20:00:43.981052 longship-2024.4.17/longship_api_client/api/commands/send_reserve_now_request.py
+-rw-r--r--   0        0        0     4946 2024-03-25 20:00:43.981436 longship-2024.4.17/longship_api_client/api/commands/send_reset_request.py
+-rw-r--r--   0        0        0     5072 2024-03-25 19:42:53.014730 longship-2024.4.17/longship_api_client/api/commands/send_send_local_list_request.py
+-rw-r--r--   0        0        0     5172 2024-03-25 20:00:43.981843 longship-2024.4.17/longship_api_client/api/commands/send_set_charging_profile_request.py
+-rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.982152 longship-2024.4.17/longship_api_client/api/commands/send_trigger_message_request.py
+-rw-r--r--   0        0        0     5111 2024-03-25 19:42:53.021486 longship-2024.4.17/longship_api_client/api/commands/send_unlock_connector_request.py
+-rw-r--r--   0        0        0     5091 2024-03-25 20:00:43.982342 longship-2024.4.17/longship_api_client/api/commands/send_update_firmware_request.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.330382 longship-2024.4.17/longship_api_client/api/configurationitems/__init__.py
+-rw-r--r--   0        0        0     5527 2024-03-25 20:00:43.982664 longship-2024.4.17/longship_api_client/api/configurationitems/configurationitem_get.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.317516 longship-2024.4.17/longship_api_client/api/localtokengroups/__init__.py
+-rw-r--r--   0        0        0     6508 2024-03-25 20:00:43.982954 longship-2024.4.17/longship_api_client/api/localtokengroups/get_all_localtokengroups.py
+-rw-r--r--   0        0        0     4437 2024-03-25 19:42:53.009339 longship-2024.4.17/longship_api_client/api/localtokengroups/local_token_group_delete.py
+-rw-r--r--   0        0        0     5028 2024-03-25 19:42:53.008522 longship-2024.4.17/longship_api_client/api/localtokengroups/local_token_group_post.py
+-rw-r--r--   0        0        0     5243 2024-03-25 20:00:43.983235 longship-2024.4.17/longship_api_client/api/localtokengroups/local_token_group_put.py
+-rw-r--r--   0        0        0     4764 2024-03-25 20:00:43.983514 longship-2024.4.17/longship_api_client/api/localtokengroups/localtokengroup_get.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.331027 longship-2024.4.17/longship_api_client/api/localtokengroupstoken/__init__.py
+-rw-r--r--   0        0        0     4848 2024-03-25 19:42:53.025042 longship-2024.4.17/longship_api_client/api/localtokengroupstoken/local_token_group_token_delete.py
+-rw-r--r--   0        0        0     5216 2024-03-25 20:00:43.983719 longship-2024.4.17/longship_api_client/api/localtokengroupstoken/local_token_group_token_post.py
+-rw-r--r--   0        0        0     6004 2024-03-25 20:00:43.984111 longship-2024.4.17/longship_api_client/api/localtokengroupstoken/local_token_group_token_put.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.332975 longship-2024.4.17/longship_api_client/api/location/__init__.py
+-rw-r--r--   0        0        0     5151 2024-03-25 20:00:43.984328 longship-2024.4.17/longship_api_client/api/location/location_patch.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.282660 longship-2024.4.17/longship_api_client/api/locations/__init__.py
+-rw-r--r--   0        0        0    11635 2024-03-25 20:00:43.984514 longship-2024.4.17/longship_api_client/api/locations/get_all_locations.py
+-rw-r--r--   0        0        0     4568 2024-03-25 20:00:43.984928 longship-2024.4.17/longship_api_client/api/locations/location_get.py
+-rw-r--r--   0        0        0     5033 2024-03-25 20:00:43.985237 longship-2024.4.17/longship_api_client/api/locations/location_post.py
+-rw-r--r--   0        0        0     4850 2024-03-25 20:00:43.985423 longship-2024.4.17/longship_api_client/api/locations/location_put.py
+-rw-r--r--   0        0        0     5150 2024-03-25 19:42:53.023748 longship-2024.4.17/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py
+-rw-r--r--   0        0        0     5484 2024-03-25 20:00:43.985706 longship-2024.4.17/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.306476 longship-2024.4.17/longship_api_client/api/mspreimbursement/__init__.py
+-rw-r--r--   0        0        0     4499 2024-03-25 19:42:53.013509 longship-2024.4.17/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.303969 longship-2024.4.17/longship_api_client/api/organizationunits/__init__.py
+-rw-r--r--   0        0        0     6531 2024-03-25 20:00:43.986158 longship-2024.4.17/longship_api_client/api/organizationunits/get_all_organizationunits.py
+-rw-r--r--   0        0        0     4787 2024-03-25 20:00:43.986377 longship-2024.4.17/longship_api_client/api/organizationunits/organization_unit_get.py
+-rw-r--r--   0        0        0     5049 2024-03-25 20:00:43.986553 longship-2024.4.17/longship_api_client/api/organizationunits/organization_unit_post.py
+-rw-r--r--   0        0        0     5250 2024-03-25 20:00:43.986734 longship-2024.4.17/longship_api_client/api/organizationunits/organization_unit_put.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.301307 longship-2024.4.17/longship_api_client/api/reimbursement/__init__.py
+-rw-r--r--   0        0        0    10500 2024-03-25 20:00:43.987077 longship-2024.4.17/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py
+-rw-r--r--   0        0        0     5141 2024-03-25 19:42:53.009738 longship-2024.4.17/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py
+-rw-r--r--   0        0        0     4745 2024-03-25 19:42:53.010083 longship-2024.4.17/longship_api_client/api/reimbursement/reimbursement_cdr_get.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.260831 longship-2024.4.17/longship_api_client/api/sessions/__init__.py
+-rw-r--r--   0        0        0    20550 2024-03-25 20:00:43.987351 longship-2024.4.17/longship_api_client/api/sessions/get_all_sessions.py
+-rw-r--r--   0        0        0     4546 2024-03-25 20:00:43.987624 longship-2024.4.17/longship_api_client/api/sessions/session_get.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.326877 longship-2024.4.17/longship_api_client/api/tariffdistributions/__init__.py
+-rw-r--r--   0        0        0     8625 2024-03-25 20:00:43.988058 longship-2024.4.17/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py
+-rw-r--r--   0        0        0     4583 2024-03-25 20:00:43.988413 longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_delete.py
+-rw-r--r--   0        0        0     4683 2024-03-25 20:00:43.988748 longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_get.py
+-rw-r--r--   0        0        0     5375 2024-03-25 20:00:43.989159 longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_patch.py
+-rw-r--r--   0        0        0     4941 2024-03-25 20:00:43.989422 longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_post.py
+-rw-r--r--   0        0        0     5613 2024-03-25 20:00:43.989810 longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_put.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.323367 longship-2024.4.17/longship_api_client/api/tariffs/__init__.py
+-rw-r--r--   0        0        0     7355 2024-03-25 20:00:43.990037 longship-2024.4.17/longship_api_client/api/tariffs/get_all_tariffs.py
+-rw-r--r--   0        0        0     4475 2024-03-25 20:00:43.990394 longship-2024.4.17/longship_api_client/api/tariffs/tariff_delete.py
+-rw-r--r--   0        0        0     4524 2024-03-25 20:00:43.990763 longship-2024.4.17/longship_api_client/api/tariffs/tariff_get.py
+-rw-r--r--   0        0        0     5134 2024-03-25 20:00:43.990994 longship-2024.4.17/longship_api_client/api/tariffs/tariff_patch.py
+-rw-r--r--   0        0        0     4836 2024-03-25 20:00:43.991198 longship-2024.4.17/longship_api_client/api/tariffs/tariff_post.py
+-rw-r--r--   0        0        0     5052 2024-03-25 20:00:43.991391 longship-2024.4.17/longship_api_client/api/tariffs/tariff_put.py
+-rw-r--r--   0        0        0        0 2024-03-25 19:42:52.320418 longship-2024.4.17/longship_api_client/api/webhooks/__init__.py
+-rw-r--r--   0        0        0     8087 2024-03-25 20:00:43.991710 longship-2024.4.17/longship_api_client/api/webhooks/get_all_webhooks.py
+-rw-r--r--   0        0        0     4365 2024-03-25 19:42:53.011639 longship-2024.4.17/longship_api_client/api/webhooks/webhook_delete.py
+-rw-r--r--   0        0        0     4586 2024-03-25 19:42:53.011295 longship-2024.4.17/longship_api_client/api/webhooks/webhook_get.py
+-rw-r--r--   0        0        0     4856 2024-03-25 20:00:43.992017 longship-2024.4.17/longship_api_client/api/webhooks/webhook_post.py
+-rw-r--r--   0        0        0     5248 2024-03-25 20:00:43.992356 longship-2024.4.17/longship_api_client/api/webhooks/webhook_put.py
+-rw-r--r--   0        0        0    12209 2024-03-25 19:42:53.022999 longship-2024.4.17/longship_api_client/client.py
+-rw-r--r--   0        0        0      546 2024-03-25 19:42:53.007596 longship-2024.4.17/longship_api_client/errors.py
+-rw-r--r--   0        0        0    22439 2024-03-25 19:42:53.021268 longship-2024.4.17/longship_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2637 2024-03-25 20:16:22.035460 longship-2024.4.17/longship_api_client/models/additional_geo_location_dto.py
+-rw-r--r--   0        0        0     3671 2024-03-25 20:16:03.746432 longship-2024.4.17/longship_api_client/models/authorization_assertion_dto.py
+-rw-r--r--   0        0        0      644 2024-03-25 19:42:53.007525 longship-2024.4.17/longship_api_client/models/authorization_assertion_dto_auth_scenario_type.py
+-rw-r--r--   0        0        0      278 2024-03-25 19:42:53.011158 longship-2024.4.17/longship_api_client/models/authorization_assertion_dto_status.py
+-rw-r--r--   0        0        0     3446 2024-03-25 19:42:53.013517 longship-2024.4.17/longship_api_client/models/authorization_charger_context_dto.py
+-rw-r--r--   0        0        0     3198 2024-03-25 20:16:06.745858 longship-2024.4.17/longship_api_client/models/authorization_context_details_dto.py
+-rw-r--r--   0        0        0     2334 2024-03-25 20:16:17.147771 longship-2024.4.17/longship_api_client/models/authorization_data.py
+-rw-r--r--   0        0        0     4295 2024-03-25 20:16:17.147874 longship-2024.4.17/longship_api_client/models/authorization_result_dto.py
+-rw-r--r--   0        0        0      895 2024-03-25 19:42:53.014619 longship-2024.4.17/longship_api_client/models/authorization_result_dto_reason.py
+-rw-r--r--   0        0        0      289 2024-03-25 19:42:53.019455 longship-2024.4.17/longship_api_client/models/authorization_result_dto_status.py
+-rw-r--r--   0        0        0     2524 2024-03-25 19:42:53.009051 longship-2024.4.17/longship_api_client/models/authorization_tenant_context_dto.py
+-rw-r--r--   0        0        0     2507 2024-03-25 20:01:26.710827 longship-2024.4.17/longship_api_client/models/business_details_dto.py
+-rw-r--r--   0        0        0     1604 2024-03-25 19:42:53.025922 longship-2024.4.17/longship_api_client/models/cancel_reservation_request.py
+-rw-r--r--   0        0        0    16774 2024-03-25 20:16:17.147727 longship-2024.4.17/longship_api_client/models/cdr_dto.py
+-rw-r--r--   0        0        0      177 2024-03-25 19:42:53.018594 longship-2024.4.17/longship_api_client/models/cdr_dto_approval_status.py
+-rw-r--r--   0        0        0      166 2024-03-25 19:42:53.011820 longship-2024.4.17/longship_api_client/models/cdr_dto_financial_type.py
+-rw-r--r--   0        0        0     1903 2024-03-25 19:42:53.021004 longship-2024.4.17/longship_api_client/models/cdr_geo_location_dto.py
+-rw-r--r--   0        0        0     6896 2024-03-25 20:16:17.145392 longship-2024.4.17/longship_api_client/models/cdr_location_dto.py
+-rw-r--r--   0        0        0      202 2024-03-25 19:42:53.020295 longship-2024.4.17/longship_api_client/models/cdr_location_dto_power_type.py
+-rw-r--r--   0        0        0     2261 2024-03-25 20:16:17.145494 longship-2024.4.17/longship_api_client/models/cdr_patch_dto.py
+-rw-r--r--   0        0        0      182 2024-03-25 19:42:53.016250 longship-2024.4.17/longship_api_client/models/cdr_patch_dto_approval_status.py
+-rw-r--r--   0        0        0     5453 2024-03-25 20:16:17.145534 longship-2024.4.17/longship_api_client/models/cdr_started_by_info_dto.py
+-rw-r--r--   0        0        0      668 2024-03-25 19:42:53.020391 longship-2024.4.17/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0      185 2024-03-25 19:42:53.015245 longship-2024.4.17/longship_api_client/models/cdr_started_by_info_dto_roaming_platform_type.py
+-rw-r--r--   0        0        0     5677 2024-03-25 20:16:17.145633 longship-2024.4.17/longship_api_client/models/cdr_started_by_token_dto.py
+-rw-r--r--   0        0        0      221 2024-03-25 19:42:53.015398 longship-2024.4.17/longship_api_client/models/cdr_started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      230 2024-03-25 19:42:53.020906 longship-2024.4.17/longship_api_client/models/cdr_started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     2004 2024-03-25 19:42:53.011062 longship-2024.4.17/longship_api_client/models/change_availability_request.py
+-rw-r--r--   0        0        0      194 2024-03-25 19:42:53.014134 longship-2024.4.17/longship_api_client/models/change_availability_request_type.py
+-rw-r--r--   0        0        0     1659 2024-03-25 19:42:53.012267 longship-2024.4.17/longship_api_client/models/change_configuration_request.py
+-rw-r--r--   0        0        0     6741 2024-03-25 20:16:17.148174 longship-2024.4.17/longship_api_client/models/charge_point_authorize_get_dto.py
+-rw-r--r--   0        0        0      247 2024-03-25 19:42:53.016677 longship-2024.4.17/longship_api_client/models/charge_point_authorize_get_dto_authorization_request_type.py
+-rw-r--r--   0        0        0     1952 2024-03-25 19:42:53.023232 longship-2024.4.17/longship_api_client/models/charge_point_authorize_post_dto.py
+-rw-r--r--   0        0        0     3974 2024-03-25 20:16:17.145652 longship-2024.4.17/longship_api_client/models/chargepoint_configuration_items_dto.py
+-rw-r--r--   0        0        0     6602 2024-03-25 20:16:17.147802 longship-2024.4.17/longship_api_client/models/chargepoint_connector_dto.py
+-rw-r--r--   0        0        0      176 2024-03-25 19:42:53.009231 longship-2024.4.17/longship_api_client/models/chargepoint_connector_dto_format.py
+-rw-r--r--   0        0        0      405 2024-03-25 19:42:53.018023 longship-2024.4.17/longship_api_client/models/chargepoint_connector_dto_operational_status.py
+-rw-r--r--   0        0        0      211 2024-03-25 19:42:53.010045 longship-2024.4.17/longship_api_client/models/chargepoint_connector_dto_power_type.py
+-rw-r--r--   0        0        0     1100 2024-03-25 19:42:53.018437 longship-2024.4.17/longship_api_client/models/chargepoint_connector_dto_standard.py
+-rw-r--r--   0        0        0    17389 2024-03-25 20:16:17.145591 longship-2024.4.17/longship_api_client/models/chargepoint_dto.py
+-rw-r--r--   0        0        0      183 2024-03-25 19:42:53.011286 longship-2024.4.17/longship_api_client/models/chargepoint_dto_connectivity_status.py
+-rw-r--r--   0        0        0     2642 2024-03-25 19:42:53.024330 longship-2024.4.17/longship_api_client/models/chargepoint_evse_dto.py
+-rw-r--r--   0        0        0     3811 2024-03-25 19:42:53.007865 longship-2024.4.17/longship_api_client/models/chargepoint_put_dto.py
+-rw-r--r--   0        0        0     7493 2024-03-25 20:16:17.145543 longship-2024.4.17/longship_api_client/models/chargepoint_status_dto.py
+-rw-r--r--   0        0        0      189 2024-03-25 19:42:53.009010 longship-2024.4.17/longship_api_client/models/chargepoint_status_dto_connectivity_status.py
+-rw-r--r--   0        0        0     3910 2024-03-25 20:16:17.145642 longship-2024.4.17/longship_api_client/models/charging_meter_value_dto.py
+-rw-r--r--   0        0        0     1197 2024-03-25 19:42:53.007491 longship-2024.4.17/longship_api_client/models/charging_meter_value_dto_measurand.py
+-rw-r--r--   0        0        0      402 2024-03-25 19:42:53.023405 longship-2024.4.17/longship_api_client/models/charging_meter_value_dto_unit.py
+-rw-r--r--   0        0        0     3263 2024-03-25 20:16:17.147852 longship-2024.4.17/longship_api_client/models/charging_period_dto.py
+-rw-r--r--   0        0        0     6374 2024-03-25 20:16:17.147690 longship-2024.4.17/longship_api_client/models/charging_profile.py
+-rw-r--r--   0        0        0      219 2024-03-25 19:42:53.008080 longship-2024.4.17/longship_api_client/models/charging_profile_charging_profile_kind.py
+-rw-r--r--   0        0        0      264 2024-03-25 19:42:53.011335 longship-2024.4.17/longship_api_client/models/charging_profile_charging_profile_purpose.py
+-rw-r--r--   0        0        0      176 2024-03-25 19:42:53.018510 longship-2024.4.17/longship_api_client/models/charging_profile_recurrency_kind.py
+-rw-r--r--   0        0        0     4491 2024-03-25 20:16:17.145717 longship-2024.4.17/longship_api_client/models/charging_schedule.py
+-rw-r--r--   0        0        0      161 2024-03-25 19:42:53.009681 longship-2024.4.17/longship_api_client/models/charging_schedule_charging_rate_unit.py
+-rw-r--r--   0        0        0     2112 2024-03-25 19:42:53.022080 longship-2024.4.17/longship_api_client/models/charging_schedule_period.py
+-rw-r--r--   0        0        0     1234 2024-03-25 19:42:53.014036 longship-2024.4.17/longship_api_client/models/clear_cache_request.py
+-rw-r--r--   0        0        0     3655 2024-03-25 20:16:17.145699 longship-2024.4.17/longship_api_client/models/clear_charging_profile_request.py
+-rw-r--r--   0        0        0      276 2024-03-25 19:42:53.008242 longship-2024.4.17/longship_api_client/models/clear_charging_profile_request_charging_profile_purpose.py
+-rw-r--r--   0        0        0     5941 2024-03-25 20:16:17.148149 longship-2024.4.17/longship_api_client/models/connector_dto.py
+-rw-r--r--   0        0        0      165 2024-03-25 19:42:53.010260 longship-2024.4.17/longship_api_client/models/connector_dto_format.py
+-rw-r--r--   0        0        0      200 2024-03-25 19:42:53.025462 longship-2024.4.17/longship_api_client/models/connector_dto_power_type.py
+-rw-r--r--   0        0        0     1089 2024-03-25 19:42:53.013664 longship-2024.4.17/longship_api_client/models/connector_dto_standard.py
+-rw-r--r--   0        0        0     3663 2024-03-25 20:16:17.145707 longship-2024.4.17/longship_api_client/models/connector_operational_status_dto.py
+-rw-r--r--   0        0        0      411 2024-03-25 19:42:53.023397 longship-2024.4.17/longship_api_client/models/connector_operational_status_dto_operational_status.py
+-rw-r--r--   0        0        0     6482 2024-03-25 20:16:17.256119 longship-2024.4.17/longship_api_client/models/cs_charging_profiles.py
+-rw-r--r--   0        0        0      222 2024-03-25 19:42:53.021273 longship-2024.4.17/longship_api_client/models/cs_charging_profiles_charging_profile_kind.py
+-rw-r--r--   0        0        0      267 2024-03-25 19:42:53.020067 longship-2024.4.17/longship_api_client/models/cs_charging_profiles_charging_profile_purpose.py
+-rw-r--r--   0        0        0      179 2024-03-25 19:42:53.023924 longship-2024.4.17/longship_api_client/models/cs_charging_profiles_recurrency_kind.py
+-rw-r--r--   0        0        0     2101 2024-03-25 19:42:53.016959 longship-2024.4.17/longship_api_client/models/data_transfer_request.py
+-rw-r--r--   0        0        0     1830 2024-03-25 19:42:53.020953 longship-2024.4.17/longship_api_client/models/display_text_dto.py
+-rw-r--r--   0        0        0     3861 2024-03-25 19:42:53.020545 longship-2024.4.17/longship_api_client/models/energy_mix_dto.py
+-rw-r--r--   0        0        0     2351 2024-03-25 20:16:17.145600 longship-2024.4.17/longship_api_client/models/energy_source_dto.py
+-rw-r--r--   0        0        0      316 2024-03-25 19:42:53.012770 longship-2024.4.17/longship_api_client/models/energy_source_dto_source.py
+-rw-r--r--   0        0        0     2298 2024-03-25 20:16:17.145551 longship-2024.4.17/longship_api_client/models/entity_tag_header_value.py
+-rw-r--r--   0        0        0     2480 2024-03-25 20:16:17.147583 longship-2024.4.17/longship_api_client/models/environmental_impact_dto.py
+-rw-r--r--   0        0        0      209 2024-03-25 19:42:53.026019 longship-2024.4.17/longship_api_client/models/environmental_impact_dto_category.py
+-rw-r--r--   0        0        0     2743 2024-03-25 20:16:17.119953 longship-2024.4.17/longship_api_client/models/exceptional_period_dto.py
+-rw-r--r--   0        0        0     4820 2024-03-25 20:16:17.148052 longship-2024.4.17/longship_api_client/models/file_content_result.py
+-rw-r--r--   0        0        0     1885 2024-03-25 19:42:53.012418 longship-2024.4.17/longship_api_client/models/geo_location_dto.py
+-rw-r--r--   0        0        0      190 2024-03-25 19:42:53.008926 longship-2024.4.17/longship_api_client/models/get_all_cdrs_order_by.py
+-rw-r--r--   0        0        0      215 2024-03-25 19:42:53.021733 longship-2024.4.17/longship_api_client/models/get_all_chargepoints_accesstype.py
+-rw-r--r--   0        0        0      167 2024-03-25 19:42:53.025610 longship-2024.4.17/longship_api_client/models/get_all_chargepoints_chargerpowertype.py
+-rw-r--r--   0        0        0      400 2024-03-25 19:42:53.024331 longship-2024.4.17/longship_api_client/models/get_all_chargepoints_operationalstatus.py
+-rw-r--r--   0        0        0      224 2024-03-25 19:42:53.016650 longship-2024.4.17/longship_api_client/models/get_all_chargepoints_order_by.py
+-rw-r--r--   0        0        0      232 2024-03-25 19:42:53.013135 longship-2024.4.17/longship_api_client/models/get_all_locations_accesstype.py
+-rw-r--r--   0        0        0      164 2024-03-25 19:42:53.017035 longship-2024.4.17/longship_api_client/models/get_all_locations_chargerpowertype.py
+-rw-r--r--   0        0        0      191 2024-03-25 19:42:53.013268 longship-2024.4.17/longship_api_client/models/get_all_locations_order_by.py
+-rw-r--r--   0        0        0      203 2024-03-25 19:42:53.009543 longship-2024.4.17/longship_api_client/models/get_all_reimbursementcdrs_order_by.py
+-rw-r--r--   0        0        0      164 2024-03-25 19:42:53.025145 longship-2024.4.17/longship_api_client/models/get_all_sessions_order_by.py
+-rw-r--r--   0        0        0      221 2024-03-25 19:42:53.016938 longship-2024.4.17/longship_api_client/models/get_all_tariffdistributions_order_by.py
+-rw-r--r--   0        0        0      203 2024-03-25 19:42:53.024996 longship-2024.4.17/longship_api_client/models/get_all_tariffs_order_by.py
+-rw-r--r--   0        0        0      144 2024-03-25 19:42:53.012343 longship-2024.4.17/longship_api_client/models/get_all_webhooks_order_by.py
+-rw-r--r--   0        0        0     3021 2024-03-25 20:16:17.147746 longship-2024.4.17/longship_api_client/models/get_composite_schedule_request.py
+-rw-r--r--   0        0        0      172 2024-03-25 19:42:53.013558 longship-2024.4.17/longship_api_client/models/get_composite_schedule_request_charging_rate_unit.py
+-rw-r--r--   0        0        0     1742 2024-03-25 20:00:43.999594 longship-2024.4.17/longship_api_client/models/get_configuration_request.py
+-rw-r--r--   0        0        0     3494 2024-03-25 20:16:17.147616 longship-2024.4.17/longship_api_client/models/get_diagnostics_request.py
+-rw-r--r--   0        0        0     1285 2024-03-25 19:42:53.022880 longship-2024.4.17/longship_api_client/models/get_local_list_version_request.py
+-rw-r--r--   0        0        0     5058 2024-03-25 20:00:43.999981 longship-2024.4.17/longship_api_client/models/hours_dto.py
+-rw-r--r--   0        0        0     2708 2024-03-25 20:16:17.147923 longship-2024.4.17/longship_api_client/models/id_tag_info.py
+-rw-r--r--   0        0        0      252 2024-03-25 19:42:53.014006 longship-2024.4.17/longship_api_client/models/id_tag_info_status.py
+-rw-r--r--   0        0        0     3271 2024-03-25 20:16:17.145569 longship-2024.4.17/longship_api_client/models/image_dto.py
+-rw-r--r--   0        0        0      287 2024-03-25 19:42:53.010942 longship-2024.4.17/longship_api_client/models/image_dto_category.py
+-rw-r--r--   0        0        0     8733 2024-03-25 20:16:17.148073 longship-2024.4.17/longship_api_client/models/interchange_format_cdr.py
+-rw-r--r--   0        0        0     5819 2024-03-25 20:16:17.119922 longship-2024.4.17/longship_api_client/models/local_token_group_get_dto.py
+-rw-r--r--   0        0        0     4431 2024-03-25 19:42:53.011938 longship-2024.4.17/longship_api_client/models/local_token_group_post_dto.py
+-rw-r--r--   0        0        0     4394 2024-03-25 19:42:53.010143 longship-2024.4.17/longship_api_client/models/local_token_group_put_dto.py
+-rw-r--r--   0        0        0     2829 2024-03-25 19:42:53.012581 longship-2024.4.17/longship_api_client/models/local_token_group_token_get_dto.py
+-rw-r--r--   0        0        0     2416 2024-03-25 19:42:53.020751 longship-2024.4.17/longship_api_client/models/local_token_group_token_post_dto.py
+-rw-r--r--   0        0        0     2411 2024-03-25 19:42:53.025595 longship-2024.4.17/longship_api_client/models/local_token_group_token_put_dto.py
+-rw-r--r--   0        0        0     1722 2024-03-25 19:42:53.012238 longship-2024.4.17/longship_api_client/models/location_charge_point_dto.py
+-rw-r--r--   0        0        0    19679 2024-03-25 20:16:17.112028 longship-2024.4.17/longship_api_client/models/location_dto.py
+-rw-r--r--   0        0        0      706 2024-03-25 19:42:53.011179 longship-2024.4.17/longship_api_client/models/location_dto_facilities_item.py
+-rw-r--r--   0        0        0      341 2024-03-25 19:42:53.021534 longship-2024.4.17/longship_api_client/models/location_dto_parking_type.py
+-rw-r--r--   0        0        0    11826 2024-03-25 20:16:17.145579 longship-2024.4.17/longship_api_client/models/location_evse_dto.py
+-rw-r--r--   0        0        0      698 2024-03-25 19:42:53.012072 longship-2024.4.17/longship_api_client/models/location_evse_dto_capabilities_item.py
+-rw-r--r--   0        0        0      277 2024-03-25 19:42:53.009142 longship-2024.4.17/longship_api_client/models/location_evse_dto_parking_restrictions_item.py
+-rw-r--r--   0        0        0      364 2024-03-25 19:42:53.014428 longship-2024.4.17/longship_api_client/models/location_evse_dto_status.py
+-rw-r--r--   0        0        0    18562 2024-03-25 20:16:17.147645 longship-2024.4.17/longship_api_client/models/location_post_dto.py
+-rw-r--r--   0        0        0      710 2024-03-25 19:42:53.024083 longship-2024.4.17/longship_api_client/models/location_post_dto_facilities_item.py
+-rw-r--r--   0        0        0      345 2024-03-25 19:42:53.009734 longship-2024.4.17/longship_api_client/models/location_post_dto_parking_type.py
+-rw-r--r--   0        0        0    19439 2024-03-25 20:16:17.148097 longship-2024.4.17/longship_api_client/models/location_put_dto.py
+-rw-r--r--   0        0        0      709 2024-03-25 19:42:53.024738 longship-2024.4.17/longship_api_client/models/location_put_dto_facilities_item.py
+-rw-r--r--   0        0        0      344 2024-03-25 19:42:53.025234 longship-2024.4.17/longship_api_client/models/location_put_dto_parking_type.py
+-rw-r--r--   0        0        0     1957 2024-03-25 20:00:44.002906 longship-2024.4.17/longship_api_client/models/location_tariff_distribution_dto.py
+-rw-r--r--   0        0        0     2508 2024-03-25 20:16:17.145478 longship-2024.4.17/longship_api_client/models/longship_error.py
+-rw-r--r--   0        0        0     2024 2024-03-25 19:42:53.020751 longship-2024.4.17/longship_api_client/models/longship_error_detail.py
+-rw-r--r--   0        0        0     6167 2024-03-25 20:16:17.147668 longship-2024.4.17/longship_api_client/models/message_log_dto.py
+-rw-r--r--   0        0        0      219 2024-03-25 19:42:53.023217 longship-2024.4.17/longship_api_client/models/message_log_dto_direction.py
+-rw-r--r--   0        0        0     1335 2024-03-25 19:42:53.013169 longship-2024.4.17/longship_api_client/models/message_log_dto_ocpp_message_type.py
+-rw-r--r--   0        0        0      227 2024-03-25 19:42:53.009907 longship-2024.4.17/longship_api_client/models/message_log_dto_wamp_message_type.py
+-rw-r--r--   0        0        0     2240 2024-03-25 19:42:53.013023 longship-2024.4.17/longship_api_client/models/organization_unit_financial_details_dto.py
+-rw-r--r--   0        0        0    10170 2024-03-25 20:16:17.147951 longship-2024.4.17/longship_api_client/models/organization_unit_get_dto.py
+-rw-r--r--   0        0        0     9395 2024-03-25 20:16:17.147828 longship-2024.4.17/longship_api_client/models/organization_unit_post_dto.py
+-rw-r--r--   0        0        0     9143 2024-03-25 20:16:17.145690 longship-2024.4.17/longship_api_client/models/organization_unit_put_dto.py
+-rw-r--r--   0        0        0     4903 2024-03-25 19:42:53.018883 longship-2024.4.17/longship_api_client/models/price_info_dto.py
+-rw-r--r--   0        0        0     3457 2024-03-25 20:16:17.145445 longship-2024.4.17/longship_api_client/models/private_emp_tariff_dto.py
+-rw-r--r--   0        0        0      161 2024-03-25 19:42:53.013747 longship-2024.4.17/longship_api_client/models/private_emp_tariff_dto_power_type.py
+-rw-r--r--   0        0        0     3107 2024-03-25 20:16:17.145610 longship-2024.4.17/longship_api_client/models/publish_token_type_dto.py
+-rw-r--r--   0        0        0      224 2024-03-25 19:42:53.020185 longship-2024.4.17/longship_api_client/models/publish_token_type_dto_type.py
+-rw-r--r--   0        0        0     2202 2024-03-25 19:42:53.008000 longship-2024.4.17/longship_api_client/models/regular_hours_dto.py
+-rw-r--r--   0        0        0    11559 2024-03-25 20:16:17.145620 longship-2024.4.17/longship_api_client/models/reimburse_info_dto.py
+-rw-r--r--   0        0        0      205 2024-03-25 19:42:53.009099 longship-2024.4.17/longship_api_client/models/reimburse_info_dto_type.py
+-rw-r--r--   0        0        0     4113 2024-03-25 20:16:17.120003 longship-2024.4.17/longship_api_client/models/reimburse_started_by_info_dto.py
+-rw-r--r--   0        0        0      674 2024-03-25 19:42:53.020677 longship-2024.4.17/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0     5833 2024-03-25 20:16:17.145452 longship-2024.4.17/longship_api_client/models/reimburse_started_by_token_dto.py
+-rw-r--r--   0        0        0      227 2024-03-25 19:42:53.007686 longship-2024.4.17/longship_api_client/models/reimburse_started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      236 2024-03-25 19:42:53.014059 longship-2024.4.17/longship_api_client/models/reimburse_started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     3078 2024-03-25 20:16:17.148013 longship-2024.4.17/longship_api_client/models/reimbursement_bank_details_dto.py
+-rw-r--r--   0        0        0    21978 2024-03-25 20:16:17.145414 longship-2024.4.17/longship_api_client/models/reimbursement_cdr_dto.py
+-rw-r--r--   0        0        0     1971 2024-03-25 19:42:53.010185 longship-2024.4.17/longship_api_client/models/reimbursement_cdr_geo_location_dto.py
+-rw-r--r--   0        0        0     7238 2024-03-25 20:16:17.145366 longship-2024.4.17/longship_api_client/models/reimbursement_cdr_location_dto.py
+-rw-r--r--   0        0        0      215 2024-03-25 19:42:53.014885 longship-2024.4.17/longship_api_client/models/reimbursement_cdr_location_dto_power_type.py
+-rw-r--r--   0        0        0     2435 2024-03-25 19:42:53.015118 longship-2024.4.17/longship_api_client/models/reimbursement_customer_share_dto.py
+-rw-r--r--   0        0        0     1917 2024-03-25 19:42:53.007776 longship-2024.4.17/longship_api_client/models/reimbursement_price_dto.py
+-rw-r--r--   0        0        0     4783 2024-03-25 20:16:17.148122 longship-2024.4.17/longship_api_client/models/reimbursement_tariff_dto.py
+-rw-r--r--   0        0        0      209 2024-03-25 19:42:53.017372 longship-2024.4.17/longship_api_client/models/reimbursement_tariff_dto_status.py
+-rw-r--r--   0        0        0     2853 2024-03-25 20:16:17.145486 longship-2024.4.17/longship_api_client/models/remote_start_transaction_request.py
+-rw-r--r--   0        0        0     1627 2024-03-25 19:42:53.008755 longship-2024.4.17/longship_api_client/models/remote_stop_transaction_request.py
+-rw-r--r--   0        0        0     2644 2024-03-25 20:00:44.006730 longship-2024.4.17/longship_api_client/models/reserve_now_request.py
+-rw-r--r--   0        0        0     1609 2024-03-25 19:42:53.019871 longship-2024.4.17/longship_api_client/models/reset_request.py
+-rw-r--r--   0        0        0      157 2024-03-25 19:42:53.016585 longship-2024.4.17/longship_api_client/models/reset_request_type.py
+-rw-r--r--   0        0        0     3534 2024-03-25 19:42:53.008207 longship-2024.4.17/longship_api_client/models/send_local_list_request.py
+-rw-r--r--   0        0        0      187 2024-03-25 19:42:53.008152 longship-2024.4.17/longship_api_client/models/send_local_list_request_update_type.py
+-rw-r--r--   0        0        0    20526 2024-03-25 20:16:17.147904 longship-2024.4.17/longship_api_client/models/session_dto.py
+-rw-r--r--   0        0        0      194 2024-03-25 19:42:53.016855 longship-2024.4.17/longship_api_client/models/session_dto_approval_status.py
+-rw-r--r--   0        0        0      166 2024-03-25 19:42:53.022905 longship-2024.4.17/longship_api_client/models/session_dto_review_scenario_type.py
+-rw-r--r--   0        0        0      251 2024-03-25 19:42:53.022178 longship-2024.4.17/longship_api_client/models/session_dto_status.py
+-rw-r--r--   0        0        0     1923 2024-03-25 19:42:53.012037 longship-2024.4.17/longship_api_client/models/session_geo_location_dto.py
+-rw-r--r--   0        0        0     6980 2024-03-25 20:16:17.145434 longship-2024.4.17/longship_api_client/models/session_location_dto.py
+-rw-r--r--   0        0        0      206 2024-03-25 19:42:53.009978 longship-2024.4.17/longship_api_client/models/session_location_dto_power_type.py
+-rw-r--r--   0        0        0     3985 2024-03-25 20:16:17.145661 longship-2024.4.17/longship_api_client/models/session_threshold_check_dto.py
+-rw-r--r--   0        0        0      265 2024-03-25 19:42:53.014604 longship-2024.4.17/longship_api_client/models/session_threshold_check_dto_status.py
+-rw-r--r--   0        0        0      204 2024-03-25 19:42:53.023710 longship-2024.4.17/longship_api_client/models/session_threshold_check_dto_threshold_hit_outcome.py
+-rw-r--r--   0        0        0     4525 2024-03-25 20:16:17.145378 longship-2024.4.17/longship_api_client/models/session_threshold_value_dto_decimal.py
+-rw-r--r--   0        0        0      272 2024-03-25 19:42:53.024219 longship-2024.4.17/longship_api_client/models/session_threshold_value_dto_decimal_status.py
+-rw-r--r--   0        0        0      211 2024-03-25 19:42:53.023536 longship-2024.4.17/longship_api_client/models/session_threshold_value_dto_decimal_threshold_hit_outcome.py
+-rw-r--r--   0        0        0     4484 2024-03-25 20:16:17.145503 longship-2024.4.17/longship_api_client/models/session_threshold_value_dto_int_32.py
+-rw-r--r--   0        0        0      270 2024-03-25 19:42:53.025721 longship-2024.4.17/longship_api_client/models/session_threshold_value_dto_int_32_status.py
+-rw-r--r--   0        0        0      209 2024-03-25 19:42:53.011068 longship-2024.4.17/longship_api_client/models/session_threshold_value_dto_int_32_threshold_hit_outcome.py
+-rw-r--r--   0        0        0    10975 2024-03-25 20:16:17.145734 longship-2024.4.17/longship_api_client/models/session_thresholds_dto.py
+-rw-r--r--   0        0        0      462 2024-03-25 19:42:53.010379 longship-2024.4.17/longship_api_client/models/session_thresholds_dto_thresholds_hit_item.py
+-rw-r--r--   0        0        0     2133 2024-03-25 19:42:53.011494 longship-2024.4.17/longship_api_client/models/set_charging_profile_request.py
+-rw-r--r--   0        0        0     5359 2024-03-25 20:16:17.145671 longship-2024.4.17/longship_api_client/models/started_by_info_dto.py
+-rw-r--r--   0        0        0      665 2024-03-25 19:42:53.016182 longship-2024.4.17/longship_api_client/models/started_by_info_dto_authorization_state.py
+-rw-r--r--   0        0        0      182 2024-03-25 19:42:53.013508 longship-2024.4.17/longship_api_client/models/started_by_info_dto_roaming_platform_type.py
+-rw-r--r--   0        0        0     5597 2024-03-25 20:16:17.147985 longship-2024.4.17/longship_api_client/models/started_by_token_dto.py
+-rw-r--r--   0        0        0      218 2024-03-25 19:42:53.016010 longship-2024.4.17/longship_api_client/models/started_by_token_dto_auth_method.py
+-rw-r--r--   0        0        0      227 2024-03-25 19:42:53.023627 longship-2024.4.17/longship_api_client/models/started_by_token_dto_token_type.py
+-rw-r--r--   0        0        0     3466 2024-03-25 20:16:17.120060 longship-2024.4.17/longship_api_client/models/status_schedule_dto.py
+-rw-r--r--   0        0        0      366 2024-03-25 19:42:53.021753 longship-2024.4.17/longship_api_client/models/status_schedule_dto_status.py
+-rw-r--r--   0        0        0     2582 2024-03-25 19:42:53.021647 longship-2024.4.17/longship_api_client/models/string_segment.py
+-rw-r--r--   0        0        0     2931 2024-03-25 20:16:17.145561 longship-2024.4.17/longship_api_client/models/tariff_assertion_dto.py
+-rw-r--r--   0        0        0      283 2024-03-25 19:42:53.021845 longship-2024.4.17/longship_api_client/models/tariff_assertion_dto_tariff_type.py
+-rw-r--r--   0        0        0     6670 2024-03-25 20:16:17.145469 longship-2024.4.17/longship_api_client/models/tariff_distribution_get_dto.py
+-rw-r--r--   0        0        0     3746 2024-03-25 20:16:17.120079 longship-2024.4.17/longship_api_client/models/tariff_distribution_history_dto.py
+-rw-r--r--   0        0        0     3517 2024-03-25 19:42:53.019575 longship-2024.4.17/longship_api_client/models/tariff_distribution_post_dto.py
+-rw-r--r--   0        0        0     3512 2024-03-25 19:42:53.024792 longship-2024.4.17/longship_api_client/models/tariff_distribution_put_dto.py
+-rw-r--r--   0        0        0    14806 2024-03-25 20:16:17.145460 longship-2024.4.17/longship_api_client/models/tariff_dto.py
+-rw-r--r--   0        0        0      186 2024-03-25 19:42:53.025570 longship-2024.4.17/longship_api_client/models/tariff_dto_tariff_type.py
+-rw-r--r--   0        0        0      241 2024-03-25 19:42:53.009523 longship-2024.4.17/longship_api_client/models/tariff_dto_usage_type.py
+-rw-r--r--   0        0        0     6088 2024-03-25 19:42:53.022020 longship-2024.4.17/longship_api_client/models/tariff_info_dto.py
+-rw-r--r--   0        0        0     8582 2024-03-25 20:16:17.119980 longship-2024.4.17/longship_api_client/models/tariff_post_dto.py
+-rw-r--r--   0        0        0      245 2024-03-25 19:42:53.009116 longship-2024.4.17/longship_api_client/models/tariff_post_dto_usage_type.py
+-rw-r--r--   0        0        0     9227 2024-03-25 20:16:17.145424 longship-2024.4.17/longship_api_client/models/tariff_price_dto.py
+-rw-r--r--   0        0        0      209 2024-03-25 19:42:53.023536 longship-2024.4.17/longship_api_client/models/tariff_price_dto_approval_status.py
+-rw-r--r--   0        0        0     8440 2024-03-25 20:16:17.120039 longship-2024.4.17/longship_api_client/models/tariff_put_dto.py
+-rw-r--r--   0        0        0     4065 2024-03-25 20:16:17.145680 longship-2024.4.17/longship_api_client/models/tariff_restriction.py
+-rw-r--r--   0        0        0      244 2024-03-25 19:42:53.009878 longship-2024.4.17/longship_api_client/models/tariff_restriction_day_of_week.py
+-rw-r--r--   0        0        0     2668 2024-03-25 20:16:17.145523 longship-2024.4.17/longship_api_client/models/token_info_dto.py
+-rw-r--r--   0        0        0      216 2024-03-25 19:42:53.015173 longship-2024.4.17/longship_api_client/models/token_info_dto_token_type.py
+-rw-r--r--   0        0        0     2385 2024-03-25 19:42:53.021311 longship-2024.4.17/longship_api_client/models/trigger_message_request.py
+-rw-r--r--   0        0        0      420 2024-03-25 19:42:53.016098 longship-2024.4.17/longship_api_client/models/trigger_message_request_requested_message.py
+-rw-r--r--   0        0        0     1574 2024-03-25 19:42:53.014314 longship-2024.4.17/longship_api_client/models/unlock_connector_request.py
+-rw-r--r--   0        0        0     2514 2024-03-25 20:00:44.012302 longship-2024.4.17/longship_api_client/models/update_firmware_request.py
+-rw-r--r--   0        0        0     5538 2024-03-25 20:16:17.145402 longship-2024.4.17/longship_api_client/models/webhook_get_dto.py
+-rw-r--r--   0        0        0      578 2024-03-25 19:42:53.025317 longship-2024.4.17/longship_api_client/models/webhook_get_dto_event_types_item.py
+-rw-r--r--   0        0        0     1807 2024-03-25 19:42:53.024132 longship-2024.4.17/longship_api_client/models/webhook_header_dto.py
+-rw-r--r--   0        0        0     4123 2024-03-25 20:00:44.013135 longship-2024.4.17/longship_api_client/models/webhook_post_dto.py
+-rw-r--r--   0        0        0      579 2024-03-25 19:42:53.011270 longship-2024.4.17/longship_api_client/models/webhook_post_dto_event_types_item.py
+-rw-r--r--   0        0        0     4113 2024-03-25 19:42:53.010850 longship-2024.4.17/longship_api_client/models/webhook_put_dto.py
+-rw-r--r--   0        0        0      578 2024-03-25 19:42:53.014129 longship-2024.4.17/longship_api_client/models/webhook_put_dto_event_types_item.py
+-rw-r--r--   0        0        0     4250 2024-03-25 20:16:17.145514 longship-2024.4.17/longship_api_client/models/webhook_summary_get_dto.py
+-rw-r--r--   0        0        0      585 2024-03-25 19:42:53.012248 longship-2024.4.17/longship_api_client/models/webhook_summary_get_dto_event_types_item.py
+-rw-r--r--   0        0        0       25 2024-03-25 19:42:52.041583 longship-2024.4.17/longship_api_client/py.typed
+-rw-r--r--   0        0        0      985 2024-03-25 19:42:53.022168 longship-2024.4.17/longship_api_client/types.py
+-rw-r--r--   0        0        0      818 2024-04-17 14:40:33.799071 longship-2024.4.17/pyproject.toml
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 longship-2024.4.17/PKG-INFO
```

### Comparing `longship-2024.4.15/LICENSE` & `longship-2024.4.17/LICENSE`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/README.md` & `longship-2024.4.17/README.md`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship/client.py` & `longship-2024.4.17/longship/client.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship/types.py` & `longship-2024.4.17/longship/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,21 @@
     status: ChargepointDtoConnectivityStatus
 
 
 @attr.s(auto_attribs=True)
 class SessionStartData:
     chargepointid: str
     connectornumber: int
+    transactionid: str
+    locationid: Optional[str] = attr.ib(default=None)
+    evseid: Optional[str] = attr.ib(default=None)
 
 
 @attr.s(auto_attribs=True)
-class SessionUpdateData:
-    chargepointid: str
-    connectornumber: int
+class SessionUpdateData(SessionStartData):
     totalenergyinkwh: float
     totalduration: str
     totalcosts: float
 
 
 @attr.s(auto_attribs=True)
 class SessionStopData(SessionUpdateData):
```

### Comparing `longship-2024.4.15/longship_api_client/api/cdrs/cdr_get.py` & `longship-2024.4.17/longship_api_client/api/cdrs/cdr_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/cdrs/cdr_patch.py` & `longship-2024.4.17/longship_api_client/api/cdrs/cdr_patch.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/cdrs/get_all_cdrs.py` & `longship-2024.4.17/longship_api_client/api/cdrs/get_all_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/cdrs/get_all_interchangeformat.py` & `longship-2024.4.17/longship_api_client/api/cdrs/get_all_interchangeformat.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/cdrs/get_file_full_download_cdrs.py` & `longship-2024.4.17/longship_api_client/api/cdrs/get_file_full_download_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py` & `longship-2024.4.17/longship_api_client/api/cdrs/get_file_intercharge_cdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoint_status/chargepoint_status_get.py` & `longship-2024.4.17/longship_api_client/api/chargepoint_status/chargepoint_status_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py` & `longship-2024.4.17/longship_api_client/api/chargepoint_status/get_all_chargepointstatus.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoints/chargepoint_get.py` & `longship-2024.4.17/longship_api_client/api/chargepoints/chargepoint_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoints/chargepoint_put.py` & `longship-2024.4.17/longship_api_client/api/chargepoints/chargepoint_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoints/chargepointauthorization_get.py` & `longship-2024.4.17/longship_api_client/api/chargepoints/chargepointauthorization_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoints/chargepointauthorization_post.py` & `longship-2024.4.17/longship_api_client/api/chargepoints/chargepointauthorization_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepointauthorizations.py` & `longship-2024.4.17/longship_api_client/api/chargepoints/get_all_chargepointauthorizations.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepointmessages.py` & `longship-2024.4.17/longship_api_client/api/chargepoints/get_all_chargepointmessages.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/chargepoints/get_all_chargepoints.py` & `longship-2024.4.17/longship_api_client/api/chargepoints/get_all_chargepoints.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_cancel_reservation_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_cancel_reservation_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_change_availability_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_change_availability_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_change_configuration_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_change_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_clear_cache_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_clear_cache_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_clear_charging_profile_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_clear_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_data_transfer_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_data_transfer_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_get_composite_schedule_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_get_composite_schedule_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_get_configuration_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_get_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_get_diagnostics_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_get_diagnostics_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_get_local_list_version_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_get_local_list_version_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_remote_start_transaction_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_remote_start_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_remote_stop_transaction_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_remote_stop_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_reserve_now_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_reserve_now_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_reset_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_reset_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_send_local_list_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_send_local_list_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_set_charging_profile_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_set_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_trigger_message_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_trigger_message_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_unlock_connector_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_unlock_connector_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/commands/send_update_firmware_request.py` & `longship-2024.4.17/longship_api_client/api/commands/send_update_firmware_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/configurationitems/configurationitem_get.py` & `longship-2024.4.17/longship_api_client/api/configurationitems/configurationitem_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/localtokengroups/get_all_localtokengroups.py` & `longship-2024.4.17/longship_api_client/api/localtokengroups/get_all_localtokengroups.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_delete.py` & `longship-2024.4.17/longship_api_client/api/localtokengroups/local_token_group_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_post.py` & `longship-2024.4.17/longship_api_client/api/localtokengroups/local_token_group_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/localtokengroups/local_token_group_put.py` & `longship-2024.4.17/longship_api_client/api/localtokengroups/local_token_group_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/localtokengroups/localtokengroup_get.py` & `longship-2024.4.17/longship_api_client/api/localtokengroups/localtokengroup_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_delete.py` & `longship-2024.4.17/longship_api_client/api/localtokengroupstoken/local_token_group_token_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_post.py` & `longship-2024.4.17/longship_api_client/api/localtokengroupstoken/local_token_group_token_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/localtokengroupstoken/local_token_group_token_put.py` & `longship-2024.4.17/longship_api_client/api/localtokengroupstoken/local_token_group_token_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/location/location_patch.py` & `longship-2024.4.17/longship_api_client/api/location/location_patch.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/locations/get_all_locations.py` & `longship-2024.4.17/longship_api_client/api/locations/get_all_locations.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/locations/location_get.py` & `longship-2024.4.17/longship_api_client/api/locations/location_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/locations/location_post.py` & `longship-2024.4.17/longship_api_client/api/locations/location_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/locations/location_put.py` & `longship-2024.4.17/longship_api_client/api/locations/location_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py` & `longship-2024.4.17/longship_api_client/api/locations/relation_between_location_and_charge_point_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py` & `longship-2024.4.17/longship_api_client/api/locations/relation_between_location_and_charge_point_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py` & `longship-2024.4.17/longship_api_client/api/mspreimbursement/reimbursement_webhook_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/organizationunits/get_all_organizationunits.py` & `longship-2024.4.17/longship_api_client/api/organizationunits/get_all_organizationunits.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_get.py` & `longship-2024.4.17/longship_api_client/api/organizationunits/organization_unit_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_post.py` & `longship-2024.4.17/longship_api_client/api/organizationunits/organization_unit_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/organizationunits/organization_unit_put.py` & `longship-2024.4.17/longship_api_client/api/organizationunits/organization_unit_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py` & `longship-2024.4.17/longship_api_client/api/reimbursement/get_all_reimbursementcdrs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py` & `longship-2024.4.17/longship_api_client/api/reimbursement/recalculate_reimbursement_cdr_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/reimbursement/reimbursement_cdr_get.py` & `longship-2024.4.17/longship_api_client/api/reimbursement/reimbursement_cdr_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/sessions/get_all_sessions.py` & `longship-2024.4.17/longship_api_client/api/sessions/get_all_sessions.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/sessions/session_get.py` & `longship-2024.4.17/longship_api_client/api/sessions/session_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py` & `longship-2024.4.17/longship_api_client/api/tariffdistributions/get_all_tariffdistributions.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_delete.py` & `longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_get.py` & `longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_patch.py` & `longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_patch.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_post.py` & `longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffdistributions/tariffdistribution_put.py` & `longship-2024.4.17/longship_api_client/api/tariffdistributions/tariffdistribution_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffs/get_all_tariffs.py` & `longship-2024.4.17/longship_api_client/api/tariffs/get_all_tariffs.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffs/tariff_delete.py` & `longship-2024.4.17/longship_api_client/api/tariffs/tariff_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffs/tariff_get.py` & `longship-2024.4.17/longship_api_client/api/tariffs/tariff_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffs/tariff_patch.py` & `longship-2024.4.17/longship_api_client/api/tariffs/tariff_patch.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffs/tariff_post.py` & `longship-2024.4.17/longship_api_client/api/tariffs/tariff_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/tariffs/tariff_put.py` & `longship-2024.4.17/longship_api_client/api/tariffs/tariff_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/webhooks/get_all_webhooks.py` & `longship-2024.4.17/longship_api_client/api/webhooks/get_all_webhooks.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/webhooks/webhook_delete.py` & `longship-2024.4.17/longship_api_client/api/webhooks/webhook_delete.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/webhooks/webhook_get.py` & `longship-2024.4.17/longship_api_client/api/webhooks/webhook_get.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/webhooks/webhook_post.py` & `longship-2024.4.17/longship_api_client/api/webhooks/webhook_post.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/api/webhooks/webhook_put.py` & `longship-2024.4.17/longship_api_client/api/webhooks/webhook_put.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/client.py` & `longship-2024.4.17/longship_api_client/client.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/errors.py` & `longship-2024.4.17/longship_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/__init__.py` & `longship-2024.4.17/longship_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/additional_geo_location_dto.py` & `longship-2024.4.17/longship_api_client/models/additional_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/authorization_assertion_dto.py` & `longship-2024.4.17/longship_api_client/models/authorization_assertion_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/authorization_assertion_dto_auth_scenario_type.py` & `longship-2024.4.17/longship_api_client/models/authorization_assertion_dto_auth_scenario_type.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/authorization_charger_context_dto.py` & `longship-2024.4.17/longship_api_client/models/authorization_charger_context_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/authorization_context_details_dto.py` & `longship-2024.4.17/longship_api_client/models/authorization_context_details_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/authorization_data.py` & `longship-2024.4.17/longship_api_client/models/authorization_data.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/authorization_result_dto.py` & `longship-2024.4.17/longship_api_client/models/authorization_result_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/authorization_result_dto_reason.py` & `longship-2024.4.17/longship_api_client/models/authorization_result_dto_reason.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/authorization_tenant_context_dto.py` & `longship-2024.4.17/longship_api_client/models/authorization_tenant_context_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/business_details_dto.py` & `longship-2024.4.17/longship_api_client/models/business_details_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cancel_reservation_request.py` & `longship-2024.4.17/longship_api_client/models/cancel_reservation_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cdr_dto.py` & `longship-2024.4.17/longship_api_client/models/cdr_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cdr_geo_location_dto.py` & `longship-2024.4.17/longship_api_client/models/cdr_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cdr_location_dto.py` & `longship-2024.4.17/longship_api_client/models/cdr_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cdr_patch_dto.py` & `longship-2024.4.17/longship_api_client/models/cdr_patch_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto.py` & `longship-2024.4.17/longship_api_client/models/cdr_started_by_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py` & `longship-2024.4.17/longship_api_client/models/cdr_started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cdr_started_by_token_dto.py` & `longship-2024.4.17/longship_api_client/models/cdr_started_by_token_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/change_availability_request.py` & `longship-2024.4.17/longship_api_client/models/change_availability_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/change_configuration_request.py` & `longship-2024.4.17/longship_api_client/models/change_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/charge_point_authorize_get_dto.py` & `longship-2024.4.17/longship_api_client/models/charge_point_authorize_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/charge_point_authorize_post_dto.py` & `longship-2024.4.17/longship_api_client/models/charge_point_authorize_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/chargepoint_configuration_items_dto.py` & `longship-2024.4.17/longship_api_client/models/chargepoint_configuration_items_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto.py` & `longship-2024.4.17/longship_api_client/models/chargepoint_connector_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/chargepoint_connector_dto_standard.py` & `longship-2024.4.17/longship_api_client/models/chargepoint_connector_dto_standard.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/chargepoint_dto.py` & `longship-2024.4.17/longship_api_client/models/chargepoint_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/chargepoint_evse_dto.py` & `longship-2024.4.17/longship_api_client/models/chargepoint_evse_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/chargepoint_put_dto.py` & `longship-2024.4.17/longship_api_client/models/chargepoint_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/chargepoint_status_dto.py` & `longship-2024.4.17/longship_api_client/models/chargepoint_status_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/charging_meter_value_dto.py` & `longship-2024.4.17/longship_api_client/models/charging_meter_value_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/charging_meter_value_dto_measurand.py` & `longship-2024.4.17/longship_api_client/models/charging_meter_value_dto_measurand.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/charging_period_dto.py` & `longship-2024.4.17/longship_api_client/models/charging_period_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/charging_profile.py` & `longship-2024.4.17/longship_api_client/models/charging_profile.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/charging_schedule.py` & `longship-2024.4.17/longship_api_client/models/charging_schedule.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/charging_schedule_period.py` & `longship-2024.4.17/longship_api_client/models/charging_schedule_period.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/clear_cache_request.py` & `longship-2024.4.17/longship_api_client/models/clear_cache_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/clear_charging_profile_request.py` & `longship-2024.4.17/longship_api_client/models/clear_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/connector_dto.py` & `longship-2024.4.17/longship_api_client/models/connector_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/connector_dto_standard.py` & `longship-2024.4.17/longship_api_client/models/connector_dto_standard.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/connector_operational_status_dto.py` & `longship-2024.4.17/longship_api_client/models/connector_operational_status_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/cs_charging_profiles.py` & `longship-2024.4.17/longship_api_client/models/cs_charging_profiles.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/data_transfer_request.py` & `longship-2024.4.17/longship_api_client/models/data_transfer_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/display_text_dto.py` & `longship-2024.4.17/longship_api_client/models/display_text_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/energy_mix_dto.py` & `longship-2024.4.17/longship_api_client/models/energy_mix_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/energy_source_dto.py` & `longship-2024.4.17/longship_api_client/models/energy_source_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/entity_tag_header_value.py` & `longship-2024.4.17/longship_api_client/models/entity_tag_header_value.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/environmental_impact_dto.py` & `longship-2024.4.17/longship_api_client/models/environmental_impact_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/exceptional_period_dto.py` & `longship-2024.4.17/longship_api_client/models/exceptional_period_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/file_content_result.py` & `longship-2024.4.17/longship_api_client/models/file_content_result.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/geo_location_dto.py` & `longship-2024.4.17/longship_api_client/models/geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/get_composite_schedule_request.py` & `longship-2024.4.17/longship_api_client/models/get_composite_schedule_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/get_configuration_request.py` & `longship-2024.4.17/longship_api_client/models/get_configuration_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/get_diagnostics_request.py` & `longship-2024.4.17/longship_api_client/models/get_diagnostics_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/get_local_list_version_request.py` & `longship-2024.4.17/longship_api_client/models/get_local_list_version_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/hours_dto.py` & `longship-2024.4.17/longship_api_client/models/hours_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/id_tag_info.py` & `longship-2024.4.17/longship_api_client/models/id_tag_info.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/image_dto.py` & `longship-2024.4.17/longship_api_client/models/image_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/interchange_format_cdr.py` & `longship-2024.4.17/longship_api_client/models/interchange_format_cdr.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/local_token_group_get_dto.py` & `longship-2024.4.17/longship_api_client/models/local_token_group_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/local_token_group_post_dto.py` & `longship-2024.4.17/longship_api_client/models/local_token_group_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/local_token_group_put_dto.py` & `longship-2024.4.17/longship_api_client/models/local_token_group_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/local_token_group_token_get_dto.py` & `longship-2024.4.17/longship_api_client/models/local_token_group_token_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/local_token_group_token_post_dto.py` & `longship-2024.4.17/longship_api_client/models/local_token_group_token_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/local_token_group_token_put_dto.py` & `longship-2024.4.17/longship_api_client/models/local_token_group_token_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_charge_point_dto.py` & `longship-2024.4.17/longship_api_client/models/location_charge_point_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_dto.py` & `longship-2024.4.17/longship_api_client/models/location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_dto_facilities_item.py` & `longship-2024.4.17/longship_api_client/models/location_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_evse_dto.py` & `longship-2024.4.17/longship_api_client/models/location_evse_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_evse_dto_capabilities_item.py` & `longship-2024.4.17/longship_api_client/models/location_evse_dto_capabilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_post_dto.py` & `longship-2024.4.17/longship_api_client/models/location_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_post_dto_facilities_item.py` & `longship-2024.4.17/longship_api_client/models/location_post_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_put_dto.py` & `longship-2024.4.17/longship_api_client/models/location_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_put_dto_facilities_item.py` & `longship-2024.4.17/longship_api_client/models/location_put_dto_facilities_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/location_tariff_distribution_dto.py` & `longship-2024.4.17/longship_api_client/models/location_tariff_distribution_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/longship_error.py` & `longship-2024.4.17/longship_api_client/models/longship_error.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/longship_error_detail.py` & `longship-2024.4.17/longship_api_client/models/longship_error_detail.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/message_log_dto.py` & `longship-2024.4.17/longship_api_client/models/message_log_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/message_log_dto_ocpp_message_type.py` & `longship-2024.4.17/longship_api_client/models/message_log_dto_ocpp_message_type.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/organization_unit_financial_details_dto.py` & `longship-2024.4.17/longship_api_client/models/organization_unit_financial_details_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/organization_unit_get_dto.py` & `longship-2024.4.17/longship_api_client/models/organization_unit_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/organization_unit_post_dto.py` & `longship-2024.4.17/longship_api_client/models/organization_unit_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/organization_unit_put_dto.py` & `longship-2024.4.17/longship_api_client/models/organization_unit_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/price_info_dto.py` & `longship-2024.4.17/longship_api_client/models/price_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/private_emp_tariff_dto.py` & `longship-2024.4.17/longship_api_client/models/private_emp_tariff_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/publish_token_type_dto.py` & `longship-2024.4.17/longship_api_client/models/publish_token_type_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/regular_hours_dto.py` & `longship-2024.4.17/longship_api_client/models/regular_hours_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimburse_info_dto.py` & `longship-2024.4.17/longship_api_client/models/reimburse_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimburse_started_by_info_dto.py` & `longship-2024.4.17/longship_api_client/models/reimburse_started_by_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py` & `longship-2024.4.17/longship_api_client/models/reimburse_started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimburse_started_by_token_dto.py` & `longship-2024.4.17/longship_api_client/models/reimburse_started_by_token_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimbursement_bank_details_dto.py` & `longship-2024.4.17/longship_api_client/models/reimbursement_bank_details_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimbursement_cdr_dto.py` & `longship-2024.4.17/longship_api_client/models/reimbursement_cdr_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimbursement_cdr_geo_location_dto.py` & `longship-2024.4.17/longship_api_client/models/reimbursement_cdr_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimbursement_cdr_location_dto.py` & `longship-2024.4.17/longship_api_client/models/reimbursement_cdr_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimbursement_customer_share_dto.py` & `longship-2024.4.17/longship_api_client/models/reimbursement_customer_share_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimbursement_price_dto.py` & `longship-2024.4.17/longship_api_client/models/reimbursement_price_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reimbursement_tariff_dto.py` & `longship-2024.4.17/longship_api_client/models/reimbursement_tariff_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/remote_start_transaction_request.py` & `longship-2024.4.17/longship_api_client/models/remote_start_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/remote_stop_transaction_request.py` & `longship-2024.4.17/longship_api_client/models/remote_stop_transaction_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reserve_now_request.py` & `longship-2024.4.17/longship_api_client/models/reserve_now_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/reset_request.py` & `longship-2024.4.17/longship_api_client/models/reset_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/send_local_list_request.py` & `longship-2024.4.17/longship_api_client/models/send_local_list_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/session_dto.py` & `longship-2024.4.17/longship_api_client/models/session_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/session_geo_location_dto.py` & `longship-2024.4.17/longship_api_client/models/session_geo_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/session_location_dto.py` & `longship-2024.4.17/longship_api_client/models/session_location_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/session_threshold_check_dto.py` & `longship-2024.4.17/longship_api_client/models/session_threshold_check_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_decimal.py` & `longship-2024.4.17/longship_api_client/models/session_threshold_value_dto_decimal.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/session_threshold_value_dto_int_32.py` & `longship-2024.4.17/longship_api_client/models/session_threshold_value_dto_int_32.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/session_thresholds_dto.py` & `longship-2024.4.17/longship_api_client/models/session_thresholds_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/set_charging_profile_request.py` & `longship-2024.4.17/longship_api_client/models/set_charging_profile_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/started_by_info_dto.py` & `longship-2024.4.17/longship_api_client/models/started_by_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/started_by_info_dto_authorization_state.py` & `longship-2024.4.17/longship_api_client/models/started_by_info_dto_authorization_state.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/started_by_token_dto.py` & `longship-2024.4.17/longship_api_client/models/started_by_token_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/status_schedule_dto.py` & `longship-2024.4.17/longship_api_client/models/status_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/string_segment.py` & `longship-2024.4.17/longship_api_client/models/string_segment.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_assertion_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_assertion_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_distribution_get_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_distribution_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_distribution_history_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_distribution_history_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_distribution_post_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_distribution_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_distribution_put_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_distribution_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_info_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_post_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_price_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_price_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_put_dto.py` & `longship-2024.4.17/longship_api_client/models/tariff_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/tariff_restriction.py` & `longship-2024.4.17/longship_api_client/models/tariff_restriction.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/token_info_dto.py` & `longship-2024.4.17/longship_api_client/models/token_info_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/trigger_message_request.py` & `longship-2024.4.17/longship_api_client/models/trigger_message_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/unlock_connector_request.py` & `longship-2024.4.17/longship_api_client/models/unlock_connector_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/update_firmware_request.py` & `longship-2024.4.17/longship_api_client/models/update_firmware_request.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_get_dto.py` & `longship-2024.4.17/longship_api_client/models/webhook_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_get_dto_event_types_item.py` & `longship-2024.4.17/longship_api_client/models/webhook_get_dto_event_types_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_header_dto.py` & `longship-2024.4.17/longship_api_client/models/webhook_header_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_post_dto.py` & `longship-2024.4.17/longship_api_client/models/webhook_post_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_post_dto_event_types_item.py` & `longship-2024.4.17/longship_api_client/models/webhook_post_dto_event_types_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_put_dto.py` & `longship-2024.4.17/longship_api_client/models/webhook_put_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_put_dto_event_types_item.py` & `longship-2024.4.17/longship_api_client/models/webhook_put_dto_event_types_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_summary_get_dto.py` & `longship-2024.4.17/longship_api_client/models/webhook_summary_get_dto.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/models/webhook_summary_get_dto_event_types_item.py` & `longship-2024.4.17/longship_api_client/models/webhook_summary_get_dto_event_types_item.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/longship_api_client/types.py` & `longship-2024.4.17/longship_api_client/types.py`

 * *Files identical despite different names*

### Comparing `longship-2024.4.15/pyproject.toml` & `longship-2024.4.17/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "longship"
-version = "2024.04.15"
+version = "2024.04.17"
 description = "A client library for accessing Longship API"
 
 authors = ["Wojtek Siudzinski <admin@suda.pl>"]
 
 readme = "README.md"
 packages = [
     {include = "longship_api_client"},
```

### Comparing `longship-2024.4.15/PKG-INFO` & `longship-2024.4.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: longship
-Version: 2024.4.15
+Version: 2024.4.17
 Summary: A client library for accessing Longship API
 Author: Wojtek Siudzinski
 Author-email: admin@suda.pl
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

