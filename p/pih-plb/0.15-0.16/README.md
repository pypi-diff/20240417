# Comparing `tmp/pih-plb-0.15.tar.gz` & `tmp/pih-plb-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.15.tar", last modified: Tue Apr 16 02:00:00 2024, max compression
+gzip compressed data, was "pih-plb-0.16.tar", last modified: Wed Apr 17 06:01:55 2024, max compression
```

## Comparing `pih-plb-0.15.tar` & `pih-plb-0.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 02:00:00.522837 pih-plb-0.15/
--rw-rw-rw-   0        0        0      293 2024-04-16 02:00:00.491587 pih-plb-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 01:59:59.722820 pih-plb-0.15/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.15/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.15/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    44594 2024-04-15 05:12:25.000000 pih-plb-0.15/PolibaseService/api.py
--rw-rw-rw-   0        0        0     3553 2024-04-16 01:59:05.000000 pih-plb-0.15/PolibaseService/const.py
--rw-rw-rw-   0        0        0    14584 2024-02-27 00:46:55.000000 pih-plb-0.15/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:00:00.444714 pih-plb-0.15/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      293 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 02:00:00.585365 pih-plb-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 06:01:55.706368 pih-plb-0.16/
+-rw-rw-rw-   0        0        0      293 2024-04-17 06:01:55.659489 pih-plb-0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 06:01:55.298030 pih-plb-0.16/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.16/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.16/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    45743 2024-04-16 23:44:39.000000 pih-plb-0.16/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     3618 2024-04-17 05:59:44.000000 pih-plb-0.16/PolibaseService/const.py
+-rw-rw-rw-   0        0        0    14873 2024-04-16 23:48:02.000000 pih-plb-0.16/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:01:55.628245 pih-plb-0.16/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-17 06:01:55.000000 pih-plb-0.16/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 06:01:54.000000 pih-plb-0.16/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:01:55.706368 pih-plb-0.16/setup.cfg
```

### Comparing `pih-plb-0.15/PolibaseService/api.py` & `pih-plb-0.16/PolibaseService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from contextlib import contextmanager
 
 import oracledb
 from oracledb import SessionPool, DatabaseError, Cursor
 
-oracledb.init_oracle_client()
-# lib_dir="C:\\oracle"
 import ipih
 from pih import A, PIHThread
+from PolibaseService.const import HOST
+
+if not A.D.contains(A.SYS.host(), HOST.name):
+    oracledb.init_oracle_client(lib_dir=r"C:\instantclient")
+
+
 from pih.consts.errors import Error
 from PolibaseService.const import *
 from pih.collections import (
     PolibasePersonVisit,
     PolibasePersonVisitSearchCritery,
 )
 from pih.tools import (
     j,
     e,
     n,
     js,
     nn,
     ne,
     nl,
+    nnt,
     one,
     esc,
     escs,
     BitMask as BM,
     while_not_do,
 )
 
@@ -45,17 +50,17 @@
         "/",
     )
 
 
 class PolibaseApi:
     pool_map: dict[bool, SessionPool] = {}
     # handlers
-    on_note_emailed_update_handler: Callable[[int, int], None]
-    on_person_creation_or_update_handler: Callable[[dict[str, Any], bool], None]
-    on_person_saldo_update_handler: Callable[[dict[str, float | int]], None]
+    on_note_emailed_update_handler: Callable[[int, int], None] | None = None
+    on_person_creation_or_update_handler: Callable[[dict[str, Any], bool], None] | None = None
+    on_person_saldo_update_handler: Callable[[dict[str, float | int]], None] | None = None
 
     @staticmethod
     def init(debug: bool) -> None:
         if not debug:
             PIHThread(PolibaseApi.create_cqn_for_person_update)
             PIHThread(PolibaseApi.create_cqn_for_note_emailed_update)
             PIHThread(PolibaseApi.create_cqn_for_person_saldo_insert)
@@ -618,29 +623,29 @@
         result: list[dict[str, Any]] = []
         with PolibaseApi.get_cursor(test) as cursor:
             fetch_result: Any = cursor.execute(
                 PolibaseApi.get_person_query_with_condition(
                     j((PERSON_TELEPHONE_NUMBER, index, " = ", escs(value)))
                 )
             )
-            result = PolibaseApi.fill_data(fetch_result, cursor.description)
+            result = nnt(PolibaseApi.fill_data(fetch_result, cursor.description))
         return result
 
     @staticmethod
     def get_person_by_email(
         value: str, test: bool | None = None
     ) -> list[dict[str, Any]]:
         result: list[dict[str, Any]] = []
         with PolibaseApi.get_cursor(test) as cursor:
             fetch_result: Any = cursor.execute(
                 PolibaseApi.get_person_query_with_condition(
                     j((PERSON_EMAIL, "=", escs(value)))
                 )
             )
-            result = PolibaseApi.fill_data(fetch_result, cursor.description)
+            result = nnt(PolibaseApi.fill_data(fetch_result, cursor.description))
         return result
 
     @staticmethod
     def get_person_list_in_card_registry_folder(
         name: str, test: bool | None = None
     ) -> list[dict[str, Any]]:
         name = name.lower()
@@ -650,15 +655,15 @@
             fetch_result: Any = cursor.execute(
                 PolibaseApi.get_person_query_with_condition(
                     (
                         f"lower({PERSON_CARD_REGISTRY_FOLDER}) = {escs(name)} order by {PERSON_FULL_NAME}"
                     )
                 )
             )
-            result = PolibaseApi.fill_data(fetch_result, cursor.description)
+            result = nnt(PolibaseApi.fill_data(fetch_result, cursor.description))
         return result
 
     @staticmethod
     def set_person_barcode_by_pin(
         value: str, pin: int, test: bool | None = None
     ) -> bool:
         return PolibaseApi.set_person_parameter_by_pin(PERSON_BARCODE, value, pin, test)
@@ -743,15 +748,15 @@
     def get_barcode_by_pin(pin: int, test: bool | None = None) -> list[dict[str, Any]]:
         result: list[dict[str, Any]] = []
         with PolibaseApi.get_cursor(test) as cursor:
             fetch_result: Any = cursor.execute(
                 f"select {PolibaseApi.get_person_pin_field()}, {PolibaseApi.get_person_barcode_field()} from {PERSON_TABLE_NAME} where {PERSON_NO}=: pin",
                 pin=pin,
             )
-            result = PolibaseApi.fill_data(fetch_result, cursor.description)
+            result = nnt(PolibaseApi.fill_data(fetch_result, cursor.description))
         return result
 
     @staticmethod
     def get_person_pin_list_with_old_format_barcode(
         test: bool | None = None,
     ) -> list[int]:
         result: list[int] = []
@@ -774,15 +779,15 @@
                         PolibaseApi.get_person_pin_field(),
                         PolibaseApi.get_person_barcode_field(),
                         "from",
                         PERSON_TABLE_NAME,
                     )
                 )
             )
-            result = PolibaseApi.fill_data(fetch_result, cursor.description)
+            result = nnt(PolibaseApi.fill_data(fetch_result, cursor.description))
         return result
 
     @staticmethod
     def set_card_folder_name_for_person(
         chart_folder: str, pin: int, test: bool | None = None
     ) -> bool:
         return PolibaseApi.execute_update_query(
@@ -916,14 +921,39 @@
                 PATIENT_SALDO_TABLE,
                 value,
                 None if for_cqn else "order by psa_date desc",
             )
         )
 
     @staticmethod
+    def get_person_saldo_after_id(
+        value: int, test: bool | None = None
+    ) -> list[dict[str, int | float]]:
+        result_data: list[dict[str, int | float]] = []
+        with PolibaseApi.get_cursor(test) as cursor:
+            result_data.extend(
+                PolibaseApi.fill_data(
+                    cursor.execute(
+                        PolibaseApi.get_person_saldo_query_with_condition(
+                            for_cqn=False,
+                            value=js(
+                                (
+                                    j((PATIENT_SALDO_PREFIX, NUMBER)),
+                                    ">",
+                                    value,
+                                )
+                            ),
+                        )
+                    ),
+                    cursor.description,  # type: ignore
+                )
+            )  # type: ignore
+            return result_data
+
+    @staticmethod
     def get_note_emailed_query(fields: list[str] | None = None) -> str:
         return PolibaseApi.get_note_emailed_query_with_condition(None, fields)
 
     @staticmethod
     def get_person_registrator_by_pin(
         value: int, test: bool | None = None
     ) -> dict[str, Any]:
```

### Comparing `pih-plb-0.15/PolibaseService/const.py` & `pih-plb-0.16/PolibaseService/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.tools import j
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Polibase"
 
-VERSION: str = "0.15"
+VERSION: str = "0.16"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
@@ -96,7 +96,9 @@
 VISIT_PATIENT_TELEPHONE_NUMBER: str = f"{VISIT_PREFIX}place"
 VISIT_PATIENT_REGISTRATION_DATE: str = f"{VISIT_PREFIX}{REGISTRATION_DATE}"
 VISIT_PATIENTS_STATUS: str = f"{VISIT_PREFIX}vst_{NUMBER}"
 VISIT_CABINET_NO: str = f"{VISIT_PREFIX}cab_{NUMBER}"
 VISIT_DOCTOR_NO: str = f"{VISIT_PREFIX}doc_{NUMBER}"
 #
 BONUS_PLUS: str = "POI_INN"
+
+LAST_SALDO_OPERATION_ID_NAME: str = "LAST_SALDO_OPERATION_ID"
```

### Comparing `pih-plb-0.15/PolibaseService/service.py` & `pih-plb-0.16/PolibaseService/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 from pih import A
 from PolibaseService.const import *
 
 SC = A.CT_SC
 ISOLATED: bool = False
 DEBUG: bool = False
 
-
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
 
         from pih.collections import (
             PolibasePersonVisitSearchCritery,
             PolibasePersonVisitDS,
             PolibasePersonVisit,
             PolibasePerson,
         )
         from pih.consts.errors import Error
-        from pih.tools import ParameterList, n, ne
+        from pih.tools import ParameterList, n, ne, nn, nnt
         from PolibaseService.api import PolibaseApi as Api
 
         from datetime import datetime
         from typing import Any
 
         def service_call_handler(sc: SC, pl: ParameterList, context) -> Any:
             if sc == SC.get_polibase_person_by_pin:
@@ -134,26 +133,26 @@
                         A.CT_FCA.VALUE,
                         Api.execute_query(pl.next(), pl.next()),
                     )
                 except Error as error:
                     import grpc
 
                     return A.ER.rpc(
-                        context, error.details, grpc.StatusCode.INVALID_ARGUMENT
+                        context, nnt(error.details), grpc.StatusCode.INVALID_ARGUMENT
                     )
 
         def person_visit_list_mapper(
             person_visit_list: list[PolibasePersonVisit], test: bool | None = None
         ) -> list[PolibasePersonVisitDS]:
             result: list[PolibasePersonVisitDS] = []
             if ne(person_visit_list):
                 person_cache: dict[int, dict] = {
                     person[A.CT_FNC.PIN]: person
                     for person in Api.get_person_list_by_pin(
-                        list(set(list(map(lambda item: item.pin, person_visit_list)))),
+                        list(set(A.D.map(lambda item: item.pin, person_visit_list))),
                         test,
                     )
                 }
                 for person_visit_item in person_visit_list:
                     pin: int = person_visit_item.pin  # type: ignore
                     cabinet_id: int = person_visit_item.cabinetID  # type: ignore
                     # default value is Null, None in python, but need convert to 0
@@ -181,22 +180,22 @@
                                 telephone_number = person_visit_item.telephoneNumber
                             if (
                                 cabinet_id
                                 in A.CT_P.AppointmentServiceGroupId._value2member_map_
                             ):
                                 person_visit_item.serviceGroupID = cabinet_id
                             if not (n(full_name) or n(telephone_number)):
-                                full_name = A.D_F.name(full_name, True)
+                                full_name = A.D_F.name(nnt(full_name), True)
                                 telephone_number = A.D_F.telephone_number(
                                     telephone_number
                                 )
-                                begin_date: datetime = person_visit_item.beginDate
-                                complete_date: datetime = person_visit_item.completeDate
-                                begin_date2: datetime = person_visit_item.beginDate2
-                                complete_date2: datetime = (
+                                begin_date: datetime = nnt(person_visit_item.beginDate)
+                                complete_date: datetime = nnt(person_visit_item.completeDate)
+                                begin_date2: datetime = nnt(person_visit_item.beginDate2)
+                                complete_date2: datetime = nnt(
                                     person_visit_item.completeDate2
                                 )
                                 if (
                                     begin_date2 is not None
                                     and begin_date2.year != A.CT_P.DATE_IS_NOT_SET_YEAR
                                 ):
                                     begin_date = begin_date2
@@ -233,15 +232,15 @@
                                 pass
                         else:
                             pass
                     else:
                         pass
             return result
 
-        def check_for_person_card_registry_folder_name(value: str | None) -> bool:
+        def check_for_person_card_registry_folder_name(value: str) -> bool:
             last_is_alpha: bool = value[-1].isalpha() and len(value) > 2
             return ne(value) and (
                 value[0].lower() in A.CT_P.CARD_REGISTRY_FOLDER_NAME_CHECK_PATTERN
                 and len(value) <= 4
                 and (
                     not last_is_alpha
                     and value[1:].isdecimal()
@@ -272,16 +271,16 @@
                     )(person)
                 )
             )
 
         def on_person_saldo_update_handler(
             person_saldo_data: dict[str, float | int]
         ) -> None:
-            print(person_saldo_data)
             id: int = person_saldo_data[A.CT_FNC.ID]  # type: ignore
+            A.D_V.set(LAST_SALDO_OPERATION_ID_NAME, id, section=SD.name)
             doctor_id: int = person_saldo_data[A.CT_FNC.DOCTOR_ID]  # type: ignore
             bonus_minus: int = person_saldo_data["bonus_minus"] or 0  # type: ignore
             bonus_plus: int = person_saldo_data["bonus_plus"] or 0  # type: ignore
             doctor_bonus_pin_list: list[int] = A.S.get(
                 A.CT_S.BONUS_DOCTOR_PERSON_PIN_LIST
             )
             if bonus_plus > 0:
@@ -300,14 +299,17 @@
 
         def service_starts_handler() -> None:
             Api.init(DEBUG)
             Api.on_note_emailed_update_handler = on_note_emailed_update_handler
             Api.on_person_creation_or_update_handler = (
                 on_person_creation_or_update_handler
             )
+            last_id: int | None = A.D_V.value(LAST_SALDO_OPERATION_ID_NAME, section=SD.name)
+            if nn(last_id):
+                A.D.every(on_person_saldo_update_handler, Api.get_person_saldo_after_id(nnt(last_id)))
             Api.on_person_saldo_update_handler = on_person_saldo_update_handler
 
         A.SRV_A.serve(
             SD,
             service_call_handler,
             service_starts_handler,
             isolate=ISOLATED,
```

