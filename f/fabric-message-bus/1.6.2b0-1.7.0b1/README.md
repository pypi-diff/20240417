# Comparing `tmp/fabric-message-bus-1.6.2b0.tar.gz` & `tmp/fabric-message-bus-1.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-message-bus-1.6.2b0.tar", last modified: Thu Feb  8 14:27:05 2024, max compression
+gzip compressed data, was "fabric-message-bus-1.7.0b1.tar", last modified: Wed Apr 17 02:32:24 2024, max compression
```

## Comparing `fabric-message-bus-1.6.2b0.tar` & `fabric-message-bus-1.7.0b1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0     1856 2024-02-01 20:45:02.611265 fabric-message-bus-1.6.2b0/.gitignore
--rw-r--r--   0        0        0     1071 2024-02-01 20:45:02.611432 fabric-message-bus-1.6.2b0/LICENSE
--rw-r--r--   0        0        0     3990 2024-02-01 20:45:02.611629 fabric-message-bus-1.6.2b0/README.md
--rwxr-xr-x   0        0        0      203 2024-02-01 20:45:02.611753 fabric-message-bus-1.6.2b0/clean.sh
--rw-r--r--   0        0        0     1560 2024-02-01 20:45:02.611912 fabric-message-bus-1.6.2b0/docker-compose-no-ssl-kafka.yaml
--rw-r--r--   0        0        0     2857 2024-02-01 20:45:02.612029 fabric-message-bus-1.6.2b0/docker-compose.yml
--rw-r--r--   0        0        0       24 2024-02-08 14:26:16.407474 fabric-message-bus-1.6.2b0/fabric_mb/__init__.py
--rw-r--r--   0        0        0        0 2024-02-01 20:45:02.612321 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/__init__.py
--rw-r--r--   0        0        0     2089 2024-02-01 20:45:02.612507 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/abc_mb_api.py
--rw-r--r--   0        0        0     5899 2024-02-01 20:45:02.612717 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/admin.py
--rw-r--r--   0        0        0     7829 2024-02-08 14:26:09.575065 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/consumer.py
--rw-r--r--   0        0        0     1301 2024-02-01 20:45:02.613001 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/message_bus_exception.py
--rw-r--r--   0        0        0        0 2024-02-01 20:45:02.613124 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/__init__.py
--rw-r--r--   0        0        0     8272 2024-02-01 20:45:02.613376 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/abc_message_avro.py
--rw-r--r--   0        0        0     3915 2024-02-01 20:45:02.613562 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/abc_object_avro.py
--rw-r--r--   0        0        0     6737 2024-02-01 20:45:02.613760 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/actor_avro.py
--rw-r--r--   0        0        0     2306 2024-02-01 20:45:02.613943 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_peer_avro.py
--rw-r--r--   0        0        0     1620 2024-02-01 20:45:02.614086 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_reservation_avro.py
--rw-r--r--   0        0        0     3647 2024-02-01 20:45:02.614205 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_reservations_avro.py
--rw-r--r--   0        0        0     1578 2024-02-01 20:45:02.614328 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_slice_avro.py
--rw-r--r--   0        0        0     3815 2024-02-01 20:45:02.614472 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_update_reservation_record.py
--rw-r--r--   0        0        0     3068 2024-02-01 20:45:02.614714 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_update_slice_record.py
--rw-r--r--   0        0        0     2077 2024-02-01 20:45:02.615017 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/auth_avro.py
--rw-r--r--   0        0        0     2275 2024-02-01 20:45:02.615336 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/broker_query_model_avro.py
--rw-r--r--   0        0        0     1965 2024-02-01 20:45:02.615561 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/claim_delegation_avro.py
--rw-r--r--   0        0        0     2036 2024-02-01 20:45:02.615826 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/claim_resources_avro.py
--rw-r--r--   0        0        0     1924 2024-02-01 20:45:02.615996 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/close_avro.py
--rw-r--r--   0        0        0     2025 2024-02-01 20:45:02.616331 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/close_delegations_avro.py
--rw-r--r--   0        0        0     2029 2024-02-01 20:45:02.616774 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/close_reservations_avro.py
--rw-r--r--   0        0        0     3122 2024-02-01 20:45:02.617126 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/constants.py
--rw-r--r--   0        0        0     3946 2024-02-01 20:45:02.617405 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/delegation_avro.py
--rw-r--r--   0        0        0     2063 2024-02-01 20:45:02.617651 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/demand_reservation_avro.py
--rw-r--r--   0        0        0     1950 2024-02-01 20:45:02.617864 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/extend_lease_avro.py
--rw-r--r--   0        0        0     3384 2024-02-01 20:45:02.618112 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/extend_reservation_avro.py
--rw-r--r--   0        0        0     1977 2024-02-01 20:45:02.618311 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/extend_ticket_avro.py
--rw-r--r--   0        0        0     2199 2024-02-01 20:45:02.618579 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/failed_rpc_avro.py
--rw-r--r--   0        0        0     1593 2024-02-01 20:45:02.618817 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_actors_request_avro.py
--rw-r--r--   0        0        0     1628 2024-02-01 20:45:02.619343 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py
--rw-r--r--   0        0        0     1591 2024-02-01 20:45:02.619621 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_delegations_avro.py
--rw-r--r--   0        0        0     2016 2024-02-01 20:45:02.619886 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py
--rw-r--r--   0        0        0     1967 2024-02-01 20:45:02.620095 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_reservations_request_avro.py
--rw-r--r--   0        0        0     2544 2024-02-01 20:45:02.620291 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py
--rw-r--r--   0        0        0     1939 2024-02-01 20:45:02.620518 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_sites_request_avro.py
--rw-r--r--   0        0        0     1943 2024-02-01 20:45:02.620711 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_slices_request_avro.py
--rw-r--r--   0        0        0     1959 2024-02-01 20:45:02.620883 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_unit_request_avro.py
--rw-r--r--   0        0        0     5914 2024-02-01 20:45:02.621151 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/lease_reservation_avro.py
--rw-r--r--   0        0        0     1891 2024-02-01 20:45:02.621436 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/lease_reservation_state_avro.py
--rw-r--r--   0        0        0     3444 2024-02-01 20:45:02.621699 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/maintenance_request_avro.py
--rw-r--r--   0        0        0     1970 2024-02-01 20:45:02.621953 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/modify_lease_avro.py
--rw-r--r--   0        0        0     3804 2024-02-01 20:45:02.622256 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/poa_avro.py
--rw-r--r--   0        0        0     2961 2024-02-01 20:45:02.622499 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/poa_info_avro.py
--rw-r--r--   0        0        0     3103 2024-02-01 20:45:02.622781 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/proxy_avro.py
--rw-r--r--   0        0        0     2020 2024-02-01 20:45:02.623045 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/query_avro.py
--rw-r--r--   0        0        0     1904 2024-02-01 20:45:02.623304 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/query_result_avro.py
--rw-r--r--   0        0        0     1972 2024-02-01 20:45:02.623510 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reclaim_delegation_avro.py
--rw-r--r--   0        0        0     2043 2024-02-01 20:45:02.623703 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reclaim_resources_avro.py
--rw-r--r--   0        0        0     1948 2024-02-01 20:45:02.623914 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/redeem_avro.py
--rw-r--r--   0        0        0     1964 2024-02-01 20:45:02.624121 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/relinquish_avro.py
--rw-r--r--   0        0        0     1995 2024-02-01 20:45:02.624323 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/remove_delegation_avro.py
--rw-r--r--   0        0        0     1982 2024-02-01 20:45:02.624498 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/remove_reservation_avro.py
--rw-r--r--   0        0        0     1952 2024-02-01 20:45:02.624677 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/remove_slice_avro.py
--rw-r--r--   0        0        0     4120 2024-02-01 20:45:02.624988 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/request_by_id_record.py
--rw-r--r--   0        0        0     3019 2024-02-01 20:45:02.625318 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_avro.py
--rw-r--r--   0        0        0     7721 2024-02-01 20:45:02.625643 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_mng.py
--rw-r--r--   0        0        0     3126 2024-02-01 20:45:02.625868 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_or_delegation_record.py
--rw-r--r--   0        0        0     2059 2024-02-01 20:45:02.626114 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_predecessor_avro.py
--rw-r--r--   0        0        0     2513 2024-02-01 20:45:02.626339 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_state_avro.py
--rw-r--r--   0        0        0     3193 2024-02-01 20:45:02.626534 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/resource_set_avro.py
--rw-r--r--   0        0        0     3431 2024-02-01 20:45:02.626791 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/resource_ticket_avro.py
--rw-r--r--   0        0        0     1587 2024-02-01 20:45:02.627025 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_actor_avro.py
--rw-r--r--   0        0        0     2550 2024-02-01 20:45:02.627241 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_avro.py
--rw-r--r--   0        0        0     1625 2024-02-01 20:45:02.627434 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_broker_query_model_avro.py
--rw-r--r--   0        0        0     1607 2024-02-01 20:45:02.627610 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_delegation_avro.py
--rw-r--r--   0        0        0     1581 2024-02-01 20:45:02.627822 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_poa_avro.py
--rw-r--r--   0        0        0     1588 2024-02-01 20:45:02.628012 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_proxy_avro.py
--rw-r--r--   0        0        0    11980 2024-02-01 20:45:02.628320 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_record_list.py
--rw-r--r--   0        0        0     1611 2024-02-01 20:45:02.628568 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_reservation_avro.py
--rw-r--r--   0        0        0     1633 2024-02-01 20:45:02.628898 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_reservation_state_avro.py
--rw-r--r--   0        0        0     1662 2024-02-01 20:45:02.629195 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_sites_avro.py
--rw-r--r--   0        0        0     1587 2024-02-01 20:45:02.629448 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_slice_avro.py
--rw-r--r--   0        0        0     3167 2024-02-01 20:45:02.629639 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_string_avro.py
--rw-r--r--   0        0        0     3191 2024-02-01 20:45:02.629853 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_strings_avro.py
--rw-r--r--   0        0        0     1662 2024-02-01 20:45:02.630040 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_units_avro.py
--rw-r--r--   0        0        0     1900 2024-02-01 20:45:02.630237 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/site_avro.py
--rw-r--r--   0        0        0     8670 2024-02-01 20:45:02.630540 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/slice_avro.py
--rw-r--r--   0        0        0     1844 2024-02-01 20:45:02.630768 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/term_avro.py
--rw-r--r--   0        0        0     3474 2024-02-01 20:45:02.630986 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/ticket.py
--rw-r--r--   0        0        0     2810 2024-02-01 20:45:02.631270 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/ticket_avro.py
--rw-r--r--   0        0        0     4436 2024-02-01 20:45:02.631688 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/ticket_reservation_avro.py
--rw-r--r--   0        0        0     3512 2024-02-01 20:45:02.632022 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/unit_avro.py
--rw-r--r--   0        0        0     1759 2024-02-01 20:45:02.632338 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_data_avro.py
--rw-r--r--   0        0        0     1969 2024-02-01 20:45:02.632567 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_delegation_avro.py
--rw-r--r--   0        0        0     1971 2024-02-01 20:45:02.632790 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_lease_avro.py
--rw-r--r--   0        0        0     1631 2024-02-01 20:45:02.632988 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_reservation_avro.py
--rw-r--r--   0        0        0     1588 2024-02-01 20:45:02.633254 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_slice_avro.py
--rw-r--r--   0        0        0     1975 2024-02-01 20:45:02.633489 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_ticket_avro.py
--rw-r--r--   0        0        0     7894 2024-02-01 20:45:02.633756 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/producer.py
--rw-r--r--   0        0        0       92 2024-02-01 20:45:02.634223 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/schema/key.avsc
--rw-r--r--   0        0        0    30908 2024-02-01 20:45:02.634583 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/schema/message.avsc
--rw-r--r--   0        0        0        0 2024-02-01 20:45:02.634885 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/test/__init__.py
--rw-r--r--   0        0        0    15232 2024-02-01 20:45:02.635402 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/test/abqm.graphml
--rw-r--r--   0        0        0    44737 2024-02-01 20:45:02.635872 fabric-message-bus-1.6.2b0/fabric_mb/message_bus/test/message_bus_test.py
--rw-r--r--   0        0        0      747 2024-02-01 20:45:02.636181 fabric-message-bus-1.6.2b0/pyproject.toml
--rwxr-xr-x   0        0        0     2190 2024-02-01 20:45:02.636517 fabric-message-bus-1.6.2b0/secrets/create-certs.sh
--rw-r--r--   0        0        0     4553 1970-01-01 00:00:00.000000 fabric-message-bus-1.6.2b0/PKG-INFO
+-rw-r--r--   0        0        0     1856 2024-04-05 21:47:59.954924 fabric-message-bus-1.7.0b1/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-05 21:47:59.955071 fabric-message-bus-1.7.0b1/LICENSE
+-rw-r--r--   0        0        0     3990 2024-04-05 21:47:59.955200 fabric-message-bus-1.7.0b1/README.md
+-rwxr-xr-x   0        0        0      203 2024-04-05 21:47:59.955313 fabric-message-bus-1.7.0b1/clean.sh
+-rw-r--r--   0        0        0     1560 2024-04-05 21:47:59.955460 fabric-message-bus-1.7.0b1/docker-compose-no-ssl-kafka.yaml
+-rw-r--r--   0        0        0     2857 2024-04-05 21:47:59.955580 fabric-message-bus-1.7.0b1/docker-compose.yml
+-rw-r--r--   0        0        0       24 2024-04-17 02:32:19.505276 fabric-message-bus-1.7.0b1/fabric_mb/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:47:59.955928 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/__init__.py
+-rw-r--r--   0        0        0     2089 2024-04-05 21:47:59.956105 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/abc_mb_api.py
+-rw-r--r--   0        0        0     5899 2024-04-05 21:47:59.956269 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/admin.py
+-rw-r--r--   0        0        0     7829 2024-04-05 21:47:59.956409 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/consumer.py
+-rw-r--r--   0        0        0     1301 2024-04-05 21:47:59.956525 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/message_bus_exception.py
+-rw-r--r--   0        0        0        0 2024-04-05 21:47:59.956635 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/__init__.py
+-rw-r--r--   0        0        0     8272 2024-04-05 21:47:59.956828 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/abc_message_avro.py
+-rw-r--r--   0        0        0     3915 2024-04-05 21:47:59.957020 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/abc_object_avro.py
+-rw-r--r--   0        0        0     6737 2024-04-05 21:47:59.957168 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/actor_avro.py
+-rw-r--r--   0        0        0     2306 2024-04-05 21:47:59.957351 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_peer_avro.py
+-rw-r--r--   0        0        0     1620 2024-04-05 21:47:59.957495 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_reservation_avro.py
+-rw-r--r--   0        0        0     3647 2024-04-05 21:47:59.957615 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_reservations_avro.py
+-rw-r--r--   0        0        0     1578 2024-04-05 21:47:59.957728 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_slice_avro.py
+-rw-r--r--   0        0        0     3815 2024-04-05 21:47:59.957878 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_update_reservation_record.py
+-rw-r--r--   0        0        0     3068 2024-04-05 21:47:59.957993 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_update_slice_record.py
+-rw-r--r--   0        0        0     2077 2024-04-05 21:47:59.958132 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/auth_avro.py
+-rw-r--r--   0        0        0     2275 2024-04-05 21:47:59.958269 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/broker_query_model_avro.py
+-rw-r--r--   0        0        0     1965 2024-04-05 21:47:59.958396 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/claim_delegation_avro.py
+-rw-r--r--   0        0        0     2036 2024-04-05 21:47:59.958555 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/claim_resources_avro.py
+-rw-r--r--   0        0        0     1924 2024-04-05 21:47:59.958755 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/close_avro.py
+-rw-r--r--   0        0        0     2025 2024-04-05 21:47:59.958954 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/close_delegations_avro.py
+-rw-r--r--   0        0        0     2029 2024-04-05 21:47:59.959160 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/close_reservations_avro.py
+-rw-r--r--   0        0        0     3122 2024-04-05 21:47:59.959371 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/constants.py
+-rw-r--r--   0        0        0     3946 2024-04-05 21:47:59.959570 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/delegation_avro.py
+-rw-r--r--   0        0        0     2063 2024-04-05 21:47:59.959718 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/demand_reservation_avro.py
+-rw-r--r--   0        0        0     1950 2024-04-05 21:47:59.959843 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/extend_lease_avro.py
+-rw-r--r--   0        0        0     3384 2024-04-05 21:47:59.960198 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/extend_reservation_avro.py
+-rw-r--r--   0        0        0     1977 2024-04-05 21:47:59.960457 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/extend_ticket_avro.py
+-rw-r--r--   0        0        0     2199 2024-04-05 21:47:59.960698 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/failed_rpc_avro.py
+-rw-r--r--   0        0        0     1593 2024-04-05 21:47:59.960893 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_actors_request_avro.py
+-rw-r--r--   0        0        0     1628 2024-04-05 21:47:59.961088 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py
+-rw-r--r--   0        0        0     1591 2024-04-05 21:47:59.961277 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_delegations_avro.py
+-rw-r--r--   0        0        0     2016 2024-04-05 21:47:59.961487 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py
+-rw-r--r--   0        0        0     1967 2024-04-05 21:47:59.961682 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_reservations_request_avro.py
+-rw-r--r--   0        0        0     2544 2024-04-05 21:47:59.961996 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py
+-rw-r--r--   0        0        0     1939 2024-04-05 21:47:59.962264 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_sites_request_avro.py
+-rw-r--r--   0        0        0     1943 2024-04-05 21:47:59.962461 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_slices_request_avro.py
+-rw-r--r--   0        0        0     1959 2024-04-05 21:47:59.962710 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_unit_request_avro.py
+-rw-r--r--   0        0        0     5838 2024-04-05 22:14:17.899208 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/lease_reservation_avro.py
+-rw-r--r--   0        0        0     1891 2024-04-05 21:47:59.963327 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/lease_reservation_state_avro.py
+-rw-r--r--   0        0        0     3444 2024-04-05 21:47:59.963575 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/maintenance_request_avro.py
+-rw-r--r--   0        0        0     1970 2024-04-05 21:47:59.964451 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/modify_lease_avro.py
+-rw-r--r--   0        0        0     3804 2024-04-05 21:47:59.964813 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/poa_avro.py
+-rw-r--r--   0        0        0     2961 2024-04-05 21:47:59.965110 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/poa_info_avro.py
+-rw-r--r--   0        0        0     3103 2024-04-05 21:47:59.965367 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/proxy_avro.py
+-rw-r--r--   0        0        0     2020 2024-04-05 21:47:59.965586 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/query_avro.py
+-rw-r--r--   0        0        0     1904 2024-04-05 21:47:59.965809 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/query_result_avro.py
+-rw-r--r--   0        0        0     1972 2024-04-05 21:47:59.966025 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reclaim_delegation_avro.py
+-rw-r--r--   0        0        0     2043 2024-04-05 21:47:59.966210 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reclaim_resources_avro.py
+-rw-r--r--   0        0        0     1948 2024-04-05 21:47:59.966392 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/redeem_avro.py
+-rw-r--r--   0        0        0     1964 2024-04-05 21:47:59.966588 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/relinquish_avro.py
+-rw-r--r--   0        0        0     1995 2024-04-05 21:47:59.966791 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/remove_delegation_avro.py
+-rw-r--r--   0        0        0     1982 2024-04-05 21:47:59.966985 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/remove_reservation_avro.py
+-rw-r--r--   0        0        0     1952 2024-04-05 21:47:59.967157 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/remove_slice_avro.py
+-rw-r--r--   0        0        0     4723 2024-04-05 22:14:17.904022 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/request_by_id_record.py
+-rw-r--r--   0        0        0     3019 2024-04-05 21:47:59.967651 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_avro.py
+-rw-r--r--   0        0        0     7721 2024-04-05 21:47:59.967861 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_mng.py
+-rw-r--r--   0        0        0     3126 2024-04-05 21:47:59.968058 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_or_delegation_record.py
+-rw-r--r--   0        0        0     2059 2024-04-05 21:47:59.968309 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_predecessor_avro.py
+-rw-r--r--   0        0        0     2513 2024-04-05 21:47:59.968549 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_state_avro.py
+-rw-r--r--   0        0        0     3193 2024-04-05 21:47:59.968747 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/resource_set_avro.py
+-rw-r--r--   0        0        0     3431 2024-04-05 21:47:59.969413 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/resource_ticket_avro.py
+-rw-r--r--   0        0        0     1587 2024-04-05 21:47:59.969674 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_actor_avro.py
+-rw-r--r--   0        0        0     2550 2024-04-05 21:47:59.969908 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_avro.py
+-rw-r--r--   0        0        0     1625 2024-04-05 21:47:59.970150 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_broker_query_model_avro.py
+-rw-r--r--   0        0        0     1607 2024-04-05 21:47:59.970366 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_delegation_avro.py
+-rw-r--r--   0        0        0     1581 2024-04-05 21:47:59.970571 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_poa_avro.py
+-rw-r--r--   0        0        0     1588 2024-04-05 21:47:59.970785 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_proxy_avro.py
+-rw-r--r--   0        0        0    11980 2024-04-05 21:47:59.971056 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_record_list.py
+-rw-r--r--   0        0        0     1611 2024-04-05 21:47:59.971275 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_reservation_avro.py
+-rw-r--r--   0        0        0     1633 2024-04-05 21:47:59.971499 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_reservation_state_avro.py
+-rw-r--r--   0        0        0     1662 2024-04-05 21:47:59.971690 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_sites_avro.py
+-rw-r--r--   0        0        0     1587 2024-04-05 21:47:59.972335 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_slice_avro.py
+-rw-r--r--   0        0        0     3167 2024-04-05 21:47:59.972607 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_string_avro.py
+-rw-r--r--   0        0        0     3191 2024-04-05 21:47:59.972928 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_strings_avro.py
+-rw-r--r--   0        0        0     1662 2024-04-05 21:47:59.973154 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_units_avro.py
+-rw-r--r--   0        0        0     1900 2024-04-05 21:47:59.973694 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/site_avro.py
+-rw-r--r--   0        0        0     8670 2024-04-05 21:47:59.973937 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/slice_avro.py
+-rw-r--r--   0        0        0     1844 2024-04-05 21:47:59.974104 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/term_avro.py
+-rw-r--r--   0        0        0     3474 2024-04-05 21:47:59.974647 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/ticket.py
+-rw-r--r--   0        0        0     2810 2024-04-05 21:47:59.974852 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/ticket_avro.py
+-rw-r--r--   0        0        0     4436 2024-04-05 21:47:59.975096 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/ticket_reservation_avro.py
+-rw-r--r--   0        0        0     3512 2024-04-05 21:47:59.975751 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/unit_avro.py
+-rw-r--r--   0        0        0     1759 2024-04-05 21:47:59.976526 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_data_avro.py
+-rw-r--r--   0        0        0     1969 2024-04-05 21:47:59.976855 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_delegation_avro.py
+-rw-r--r--   0        0        0     1971 2024-04-05 21:47:59.977162 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_lease_avro.py
+-rw-r--r--   0        0        0     1631 2024-04-05 21:47:59.977424 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_reservation_avro.py
+-rw-r--r--   0        0        0     1588 2024-04-05 21:47:59.977697 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_slice_avro.py
+-rw-r--r--   0        0        0     1975 2024-04-05 21:47:59.977912 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_ticket_avro.py
+-rw-r--r--   0        0        0     7894 2024-04-05 21:47:59.978130 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/producer.py
+-rw-r--r--   0        0        0       92 2024-04-05 21:47:59.978494 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/schema/key.avsc
+-rw-r--r--   0        0        0    31074 2024-04-05 21:56:58.730974 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/schema/message.avsc
+-rw-r--r--   0        0        0        0 2024-04-05 21:47:59.979064 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/test/__init__.py
+-rw-r--r--   0        0        0    15232 2024-04-05 21:47:59.979351 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/test/abqm.graphml
+-rw-r--r--   0        0        0    44737 2024-04-05 21:47:59.979689 fabric-message-bus-1.7.0b1/fabric_mb/message_bus/test/message_bus_test.py
+-rw-r--r--   0        0        0      747 2024-04-05 21:47:59.980369 fabric-message-bus-1.7.0b1/pyproject.toml
+-rwxr-xr-x   0        0        0     2190 2024-04-05 21:47:59.980748 fabric-message-bus-1.7.0b1/secrets/create-certs.sh
+-rw-r--r--   0        0        0     4553 1970-01-01 00:00:00.000000 fabric-message-bus-1.7.0b1/PKG-INFO
```

### Comparing `fabric-message-bus-1.6.2b0/.gitignore` & `fabric-message-bus-1.7.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/LICENSE` & `fabric-message-bus-1.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/README.md` & `fabric-message-bus-1.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/docker-compose-no-ssl-kafka.yaml` & `fabric-message-bus-1.7.0b1/docker-compose-no-ssl-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/docker-compose.yml` & `fabric-message-bus-1.7.0b1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/abc_mb_api.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/abc_mb_api.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/admin.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/admin.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/consumer.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/consumer.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/message_bus_exception.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/message_bus_exception.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/abc_message_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/abc_message_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/abc_object_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/abc_object_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/actor_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/actor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_peer_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_peer_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_reservations_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_reservations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_slice_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_update_reservation_record.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_update_reservation_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/add_update_slice_record.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/add_update_slice_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/auth_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/auth_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/broker_query_model_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/broker_query_model_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/claim_delegation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/claim_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/claim_resources_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/claim_resources_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/close_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/close_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/close_delegations_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/close_delegations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/close_reservations_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/close_reservations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/constants.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/constants.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/delegation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/demand_reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/demand_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/extend_lease_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/extend_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/extend_reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/extend_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/extend_ticket_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/extend_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/failed_rpc_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/failed_rpc_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_actors_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_actors_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_delegations_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_delegations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_reservations_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_reservations_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_sites_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_sites_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_slices_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_slices_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/get_unit_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/get_unit_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/lease_reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/lease_reservation_avro.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 import pickle
 from typing import List
 
-from fabric_mb.message_bus.message_bus_exception import MessageBusException
 from fabric_mb.message_bus.messages.constants import Constants
 from fabric_mb.message_bus.messages.reservation_predecessor_avro import ReservationPredecessorAvro
 from fabric_mb.message_bus.messages.ticket_reservation_avro import TicketReservationAvro
 
 
 class LeaseReservationAvro(TicketReservationAvro):
     """
```

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/lease_reservation_state_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/lease_reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/maintenance_request_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/maintenance_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/modify_lease_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/modify_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/poa_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/poa_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/poa_info_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/poa_info_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/proxy_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/proxy_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/query_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/query_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/query_result_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/query_result_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reclaim_delegation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reclaim_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reclaim_resources_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reclaim_resources_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/redeem_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/redeem_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/relinquish_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/relinquish_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/remove_delegation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/remove_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/remove_reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/remove_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/remove_slice_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/remove_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/request_by_id_record.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/unit_avro.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,132 +19,104 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-from typing import List
+import pickle
+from fabric_mb.message_bus.messages.abc_object_avro import AbcObjectAvro
 
-from fabric_mb.message_bus.messages.abc_message_avro import AbcMessageAvro
 
-
-class RequestByIdRecord(AbcMessageAvro):
+class UnitAvro(AbcObjectAvro):
     """
-    Implements Avro representation of a Get Request Message
+    Implements Avro representation of a Unit
     """
-
     def __init__(self):
-        super(RequestByIdRecord, self).__init__()
-        self.guid = None
-        self.slice_id = None
+        self.rtype = None
+        self.parent_id = None
+        self.state = None
+        self.sequence = 0
+        self.properties = None
         self.reservation_id = None
-        self.delegation_id = None
-        self.type = None
-        self.unit_id = None
-        self.broker_id = None
-        self.reservation_state = None
-        self.delegation_state = None
-        self.auth = None
-        self.id_token = None
-        self.slice_name = None
-        self.level = None
-        self.email = None
-        self.graph_format = None
-        self.site = None
-        self.states = None
-
-    def get_slice_id(self) -> str:
-        """
-        Returns the slice_id
-        """
-        return self.slice_id
+        self.slice_id = None
+        self.actor_id = None
+        self.sliver = None
 
-    def get_reservation_id(self) -> str:
-        """
-        Returns the reservation if
-        """
+    def get_unit_id(self) -> str:
         return self.reservation_id
 
-    def get_delegation_id(self) -> str:
+    def get_properties(self) -> dict:
         """
-        Returns the delegation id
+        Return properties
         """
-        return self.delegation_id
+        return self.properties
 
-    def get_type(self) -> str:
-        """
-        Returns the type
-        """
-        return self.type
+    def get_resource_type(self) -> str:
+        return self.rtype
 
-    def get_unit_id(self) -> str:
-        """
-        Returns the unit_id
-        """
-        return self.unit_id
+    def get_parent_id(self) -> str:
+        return self.parent_id
 
-    def get_broker_id(self) -> str:
-        """
-        Returns the broker_id
-        """
-        return self.broker_id
+    def get_state(self) -> int:
+        return self.state
 
-    def get_reservation_state(self) -> int:
-        """
-        Returns the reservation_state
-        """
-        return self.reservation_state
+    def get_sequence(self) -> int:
+        return self.sequence
+
+    def get_reservation_id(self) -> str:
+        return self.reservation_id
 
-    def get_states(self) -> List[int]:
-        return self.states
+    def get_slice_id(self) -> str:
+        return self.slice_id
 
-    def get_delegation_state(self) -> int:
-        """
-        Returns the delegation_state
-        """
-        return self.delegation_state
+    def get_actor_id(self) -> str:
+        return self.actor_id
 
-    def get_id_token(self) -> str:
+    def set_properties(self, value: dict):
         """
-        Returns the id token
+        Set properties
+        @param value value
         """
-        return self.id_token
-
-    def get_slice_name(self) -> str:
-        return self.slice_name
+        self.properties = value
 
-    def get_level(self) -> int:
-        return self.level
+    def set_unit_id(self, uid: str):
+        self.reservation_id = uid
 
-    def set_level(self, value):
-        self.level = value
+    def set_resource_type(self, rtype: str):
+        self.rtype = rtype
 
-    def set_email(self, email: str):
-        self.email = email
+    def set_parent_id(self, parent_id: str):
+        self.parent_id = parent_id
 
-    def get_email(self) -> str:
-        return self.email
+    def set_state(self, state: int):
+        self.state = state
 
-    def get_graph_format(self) -> int:
-        return self.graph_format
+    def set_sequence(self, sequence: int):
+        self.sequence = sequence
 
-    def set_graph_format(self, graph_format):
-        self.graph_format = graph_format
+    def set_reservation_id(self, reservation_id: str):
+        self.reservation_id = reservation_id
 
-    def set_site(self, site: str):
-        self.site = site
+    def set_slice_id(self, slice_id: str):
+        self.slice_id = slice_id
 
-    def get_site(self) -> str:
-        return self.site
+    def set_actor_id(self, actor_id: str):
+        self.actor_id = actor_id
 
     def validate(self) -> bool:
         """
         Check if the object is valid and contains all mandatory fields
         :return True on success; False on failure
         """
-        ret_val = super().validate()
+        ret_val = True
 
-        if self.guid is None or self.auth is None or self.callback_topic is None:
+        if self.properties is None or self.reservation_id is None:
             ret_val = False
 
         return ret_val
+
+    def set_sliver(self, sliver):
+        self.sliver = sliver
+
+    def get_sliver(self):
+        return self.sliver
```

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_mng.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_mng.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_or_delegation_record.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_or_delegation_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_predecessor_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_predecessor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/reservation_state_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/resource_set_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/resource_set_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/resource_ticket_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/resource_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_actor_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_actor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_broker_query_model_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_broker_query_model_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_delegation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_poa_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_poa_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_proxy_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_proxy_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_record_list.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_record_list.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_reservation_state_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_sites_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_sites_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_slice_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_string_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_string_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_strings_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_strings_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/result_units_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/result_units_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/site_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/site_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/slice_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/term_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/term_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/ticket.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/ticket.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/ticket_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/ticket_reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/ticket_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_data_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_data_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_delegation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_lease_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_reservation_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_slice_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/messages/update_ticket_avro.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/messages/update_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/producer.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/producer.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/schema/message.avsc` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/schema/message.avsc`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99965564738292%*

 * *Differences: {'24': "{'fields': {insert: [(20, OrderedDict([('name', 'start'), ('type', ['null', 'string']), "*

 * *       "('default', None)])), (21, OrderedDict([('name', 'end'), ('type', ['null', 'string']), "*

 * *       "('default', None)]))]}}"}*

```diff
@@ -1566,14 +1566,30 @@
             {
                 "default": null,
                 "name": "site",
                 "type": [
                     "null",
                     "string"
                 ]
+            },
+            {
+                "default": null,
+                "name": "start",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            {
+                "default": null,
+                "name": "end",
+                "type": [
+                    "null",
+                    "string"
+                ]
             }
         ],
         "name": "RequestById",
         "namespace": "fabric.cf.model",
         "type": "record"
     },
     {
```

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/test/abqm.graphml` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/test/abqm.graphml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/fabric_mb/message_bus/test/message_bus_test.py` & `fabric-message-bus-1.7.0b1/fabric_mb/message_bus/test/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/pyproject.toml` & `fabric-message-bus-1.7.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/secrets/create-certs.sh` & `fabric-message-bus-1.7.0b1/secrets/create-certs.sh`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.6.2b0/PKG-INFO` & `fabric-message-bus-1.7.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-message-bus
-Version: 1.6.2b0
+Version: 1.7.0b1
 Summary: Fabric Message Bus Schema
 Keywords: Kafka,Fabric Message Bus Schema,Avro
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

