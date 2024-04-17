# Comparing `tmp/RsCmwWlanSig-3.8.20.40.tar.gz` & `tmp/RsCmwWlanSig-4.0.110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCmwWlanSig-3.8.20.40.tar", last modified: Sun May 16 18:16:19 2021, max compression
+gzip compressed data, was "dist\RsCmwWlanSig-4.0.110.tar", last modified: Wed Apr 17 08:14:04 2024, max compression
```

## Comparing `RsCmwWlanSig-3.8.20.40.tar` & `RsCmwWlanSig-4.0.110.tar`

### file list

```diff
@@ -1,383 +1,364 @@
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.661909 RsCmwWlanSig-3.8.20.40/
--rw-rw-rw-   0        0        0     3889 2021-05-16 18:16:19.661909 RsCmwWlanSig-3.8.20.40/PKG-INFO
--rw-rw-rw-   0        0        0     2691 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/README.md
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.250673 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.293559 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/CustomFiles/
--rw-rw-rw-   0        0        0        0 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     3304 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4517 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    18659 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.360381 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/
--rw-rw-rw-   0        0        0     1188 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.378332 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/
--rw-rw-rw-   0        0        0     1453 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.407256 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/
--rw-rw-rw-   0        0        0     1269 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Station.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.423215 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Station_/
--rw-rw-rw-   0        0        0     1332 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Station_/Connect.py
--rw-rw-rw-   0        0        0     1548 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Station_/Reconnect.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Station_/__init__.py
--rw-rw-rw-   0        0        0     1043 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wdirect.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.432189 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wdirect_/
--rw-rw-rw-   0        0        0     1138 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wdirect_/Sconnection.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wdirect_/__init__.py
--rw-rw-rw-   0        0        0     1019 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wps.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.444157 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wps_/
--rw-rw-rw-   0        0        0     1114 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wps_/Sconnection.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wps_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/__init__.py
--rw-rw-rw-   0        0        0     1807 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.454131 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta_/
--rw-rw-rw-   0        0        0     1029 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta_/Action.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.463106 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta_/Action_/
--rw-rw-rw-   0        0        0     1774 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta_/Action_/Disconnect.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta_/Action_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/__init__.py
--rw-rw-rw-   0        0        0     1003 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Clean.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.474077 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Clean_/
--rw-rw-rw-   0        0        0     1015 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Clean_/Elogging.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Clean_/__init__.py
--rw-rw-rw-   0        0        0     4085 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.546883 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/
--rw-rw-rw-   0        0        0    23149 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.634650 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/
--rw-rw-rw-   0        0        0     5031 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.644623 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/
--rw-rw-rw-   0        0        0     1847 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.654596 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta_/
--rw-rw-rw-   0        0        0     2957 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta_/MacReserve.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/__init__.py
--rw-rw-rw-   0        0        0     1886 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.663572 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/
--rw-rw-rw-   0        0        0     1975 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.693492 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/
--rw-rw-rw-   0        0        0     1699 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Enable.py
--rw-rw-rw-   0        0        0     1916 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Ftype.py
--rw-rw-rw-   0        0        0     1895 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/MwDuration.py
--rw-rw-rw-   0        0        0     1798 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Stime.py
--rw-rw-rw-   0        0        0     1772 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Tenable.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/__init__.py
--rw-rw-rw-   0        0        0     3547 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Ccode.py
--rw-rw-rw-   0        0        0     7006 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Edca.py
--rw-rw-rw-   0        0        0     1345 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hemac.py
--rw-rw-rw-   0        0        0    11380 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.704463 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf_/
--rw-rw-rw-   0        0        0     1127 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf_/SsTx.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf_/__init__.py
--rw-rw-rw-   0        0        0    11840 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.724410 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/
--rw-rw-rw-   0        0        0     3971 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Dname.py
--rw-rw-rw-   0        0        0     4186 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Plmn.py
--rw-rw-rw-   0        0        0     4324 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Realm.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/__init__.py
--rw-rw-rw-   0        0        0     7220 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Muedca.py
--rw-rw-rw-   0        0        0    15097 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.734383 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding_/
--rw-rw-rw-   0        0        0     1233 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding_/SsTx.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding_/__init__.py
--rw-rw-rw-   0        0        0     2822 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Qos.py
--rw-rw-rw-   0        0        0     6461 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Security.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.753333 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/
--rw-rw-rw-   0        0        0     2235 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/Eaka.py
--rw-rw-rw-   0        0        0     5334 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/Esim.py
--rw-rw-rw-   0        0        0     5193 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/Rserver.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/__init__.py
--rw-rw-rw-   0        0        0    10858 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Srates.py
--rw-rw-rw-   0        0        0     1811 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.762308 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/
--rw-rw-rw-   0        0        0      983 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.773279 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/
--rw-rw-rw-   0        0        0     2001 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.804196 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/
--rw-rw-rw-   0        0        0     3471 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/AlsField.py
--rw-rw-rw-   0        0        0     4478 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/BlAllocation.py
--rw-rw-rw-   0        0        0     1789 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.812175 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy_/
--rw-rw-rw-   0        0        0     2838 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy_/Mcs.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy_/__init__.py
--rw-rw-rw-   0        0        0     3921 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/RuAllocation.py
--rw-rw-rw-   0        0        0     2497 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.835114 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/
--rw-rw-rw-   0        0        0     3308 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Allocation.py
--rw-rw-rw-   0        0        0     2606 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Ctype.py
--rw-rw-rw-   0        0        0     2848 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Mcs.py
--rw-rw-rw-   0        0        0     2643 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Streams.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/__init__.py
--rw-rw-rw-   0        0        0     3316 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Station.py
--rw-rw-rw-   0        0        0     1216 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Twt.py
--rw-rw-rw-   0        0        0     3719 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Wdirect.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/__init__.py
--rw-rw-rw-   0        0        0     3061 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Edau.py
--rw-rw-rw-   0        0        0     2791 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.844090 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe_/
--rw-rw-rw-   0        0        0     1029 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.853067 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList_/
--rw-rw-rw-   0        0        0     4894 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList_/IprAddress.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe_/__init__.py
--rw-rw-rw-   0        0        0     1244 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.866031 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/
--rw-rw-rw-   0        0        0     2818 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.875007 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn_/
--rw-rw-rw-   0        0        0     1377 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn_/Bandwidth.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn_/__init__.py
--rw-rw-rw-   0        0        0     3016 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.882986 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator_/
--rw-rw-rw-   0        0        0      890 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator_/Iloss.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/__init__.py
--rw-rw-rw-   0        0        0     1421 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/HetBased.py
--rw-rw-rw-   0        0        0     2017 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.892959 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/
--rw-rw-rw-   0        0        0     3649 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.902934 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/
--rw-rw-rw-   0        0        0     9344 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/IpAddress.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.911909 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/IpAddress_/
--rw-rw-rw-   0        0        0     2845 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/IpAddress_/Sta.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/IpAddress_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/__init__.py
--rw-rw-rw-   0        0        0     1281 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvSix.py
--rw-rw-rw-   0        0        0     3130 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Mimo.py
--rw-rw-rw-   0        0        0     1899 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Mmonitor.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.920885 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Mmonitor_/
--rw-rw-rw-   0        0        0     2300 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Mmonitor_/IpAddress.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Mmonitor_/__init__.py
--rw-rw-rw-   0        0        0    12626 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.933851 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/
--rw-rw-rw-   0        0        0      981 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.941829 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/
--rw-rw-rw-   0        0        0     1999 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.970753 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/
--rw-rw-rw-   0        0        0     2826 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/AlsField.py
--rw-rw-rw-   0        0        0     4138 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/BlAllocation.py
--rw-rw-rw-   0        0        0     1785 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.979728 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy_/
--rw-rw-rw-   0        0        0     2219 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy_/Mcs.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy_/__init__.py
--rw-rw-rw-   0        0        0     3275 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/RuAllocation.py
--rw-rw-rw-   0        0        0     2493 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.003665 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/
--rw-rw-rw-   0        0        0     2688 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Allocation.py
--rw-rw-rw-   0        0        0     1987 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Ctype.py
--rw-rw-rw-   0        0        0     2215 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Mcs.py
--rw-rw-rw-   0        0        0     2066 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Streams.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/__init__.py
--rw-rw-rw-   0        0        0     1295 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Payload.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/__init__.py
--rw-rw-rw-   0        0        0     2905 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.030592 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/
--rw-rw-rw-   0        0        0     3396 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/Config.py
--rw-rw-rw-   0        0        0     2213 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/Destination.py
--rw-rw-rw-   0        0        0     2076 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/IpVersion.py
--rw-rw-rw-   0        0        0     2064 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/Protocol.py
--rw-rw-rw-   0        0        0     2543 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/Uports.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/__init__.py
--rw-rw-rw-   0        0        0    13543 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.043558 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/
--rw-rw-rw-   0        0        0     2383 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.059515 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/
--rw-rw-rw-   0        0        0     1282 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.074476 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/
--rw-rw-rw-   0        0        0     2237 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/InputPy.py
--rw-rw-rw-   0        0        0     2252 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/Output.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/__init__.py
--rw-rw-rw-   0        0        0     2444 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/EpePower.py
--rw-rw-rw-   0        0        0     2112 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/MlOffset.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/__init__.py
--rw-rw-rw-   0        0        0     1341 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Eattenuation.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/__init__.py
--rw-rw-rw-   0        0        0     1840 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.084450 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/
--rw-rw-rw-   0        0        0     1677 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.107387 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/
--rw-rw-rw-   0        0        0     2697 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Ampdu.py
--rw-rw-rw-   0        0        0     5203 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Dfdef.py
--rw-rw-rw-   0        0        0     2739 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.154263 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/
--rw-rw-rw-   0        0        0     1965 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Ctyp.py
--rw-rw-rw-   0        0        0     1834 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Dcm.py
--rw-rw-rw-   0        0        0     2198 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Mcs.py
--rw-rw-rw-   0        0        0     1837 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Nss.py
--rw-rw-rw-   0        0        0     3500 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Rual.py
--rw-rw-rw-   0        0        0     1138 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Sss.py
--rw-rw-rw-   0        0        0     2528 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/TrsMode.py
--rw-rw-rw-   0        0        0     1867 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Trssi.py
--rw-rw-rw-   0        0        0     2113 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/TsrControl.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/__init__.py
--rw-rw-rw-   0        0        0     1227 2021-05-16 18:16:15.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.167229 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/
--rw-rw-rw-   0        0        0     2190 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/BarMethod.py
--rw-rw-rw-   0        0        0     3072 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/Black.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/__init__.py
--rw-rw-rw-   0        0        0     2686 2021-05-16 18:16:14.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/UesInfo.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/__init__.py
--rw-rw-rw-   0        0        0     6283 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/HetBased.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.180193 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/HetBased_/
--rw-rw-rw-   0        0        0     1338 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/HetBased_/State.py
--rw-rw-rw-   0        0        0     2250 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/HetBased_/UphInfo.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/HetBased_/__init__.py
--rw-rw-rw-   0        0        0     1450 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/PackRate.py
--rw-rw-rw-   0        0        0     8648 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.188172 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per_/
--rw-rw-rw-   0        0        0     1897 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per_/State.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.197148 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per_/State_/
--rw-rw-rw-   0        0        0     2549 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per_/State_/All.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per_/State_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per_/__init__.py
--rw-rw-rw-   0        0        0     1003 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Pswitched.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.209117 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Pswitched_/
--rw-rw-rw-   0        0        0     1017 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Pswitched_/State.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Pswitched_/__init__.py
--rw-rw-rw-   0        0        0     3887 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.218093 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/
--rw-rw-rw-   0        0        0     2375 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.242028 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/
--rw-rw-rw-   0        0        0     3680 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/MimFading.py
--rw-rw-rw-   0        0        0     3521 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/Mimo.py
--rw-rw-rw-   0        0        0     2933 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/ScFading.py
--rw-rw-rw-   0        0        0     2702 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/Scell.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/__init__.py
--rw-rw-rw-   0        0        0      985 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Second.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.249009 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Second_/
--rw-rw-rw-   0        0        0     1008 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Second_/State.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Second_/__init__.py
--rw-rw-rw-   0        0        0     1892 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.275938 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/
--rw-rw-rw-   0        0        0     2066 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Elogging.py
--rw-rw-rw-   0        0        0     1909 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Pgen.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.283916 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Pgen_/
--rw-rw-rw-   0        0        0     2376 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Pgen_/PgStats.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Pgen_/__init__.py
--rw-rw-rw-   0        0        0     2240 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.293890 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo_/
--rw-rw-rw-   0        0        0     1883 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.300874 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna_/
--rw-rw-rw-   0        0        0     1892 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna_/RxpIndicator.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo_/__init__.py
--rw-rw-rw-   0        0        0     2340 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.320819 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/
--rw-rw-rw-   0        0        0     1017 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.329794 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo_/
--rw-rw-rw-   0        0        0     1939 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo_/UphInfo.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo_/__init__.py
--rw-rw-rw-   0        0        0     1216 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.342759 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/
--rw-rw-rw-   0        0        0     2436 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/He.py
--rw-rw-rw-   0        0        0      989 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/Mac.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.350738 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/Mac_/
--rw-rw-rw-   0        0        0     1173 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/Mac_/Address.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/Mac_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/__init__.py
--rw-rw-rw-   0        0        0     1996 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.376670 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/
--rw-rw-rw-   0        0        0     2652 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/AbsReport.py
--rw-rw-rw-   0        0        0     2742 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/Drate.py
--rw-rw-rw-   0        0        0     2052 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.410579 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/
--rw-rw-rw-   0        0        0     3352 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hemu.py
--rw-rw-rw-   0        0        0     3358 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hesu.py
--rw-rw-rw-   0        0        0     3352 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hetb.py
--rw-rw-rw-   0        0        0     3346 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Ht.py
--rw-rw-rw-   0        0        0     3364 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/NoNht.py
--rw-rw-rw-   0        0        0     3352 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Vht.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/__init__.py
--rw-rw-rw-   0        0        0     1136 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxbPower.py
--rw-rw-rw-   0        0        0     1846 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/UeAddress.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.419555 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/UeAddress_/
--rw-rw-rw-   0        0        0     1468 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/UeAddress_/Ipv.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/UeAddress_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/__init__.py
--rw-rw-rw-   0        0        0     2823 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.433517 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/
--rw-rw-rw-   0        0        0     1859 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.444490 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna_/
--rw-rw-rw-   0        0        0     1275 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna_/ArxbPower.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna_/__init__.py
--rw-rw-rw-   0        0        0     1848 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.454461 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress_/
--rw-rw-rw-   0        0        0     1161 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress_/Ipv.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/__init__.py
--rw-rw-rw-   0        0        0      985 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Source.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.462441 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Source_/
--rw-rw-rw-   0        0        0     3054 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Source_/State.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Source_/__init__.py
--rw-rw-rw-   0        0        0      979 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Third.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.471417 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Third_/
--rw-rw-rw-   0        0        0     1005 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Third_/State.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Third_/__init__.py
--rw-rw-rw-   0        0        0     1170 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.485381 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/
--rw-rw-rw-   0        0        0      988 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.494356 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx_/
--rw-rw-rw-   0        0        0    15732 2021-05-16 18:16:16.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.504329 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame_/
--rw-rw-rw-   0        0        0     2914 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame_/Plength.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx_/__init__.py
--rw-rw-rw-   0        0        0      987 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.514303 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx_/
--rw-rw-rw-   0        0        0     2144 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.524275 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame_/
--rw-rw-rw-   0        0        0     3082 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame_/Plength.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx_/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:19.654928 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/
--rw-rw-rw-   0        0        0      541 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4003 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1061 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1000 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9026 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5624 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3354 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2446 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5176 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    20227 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3618 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4409 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    10299 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Core.py
--rw-rw-rw-   0        0        0    38340 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Instrument.py
--rw-rw-rw-   0        0        0     3918 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2081 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0     5101 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3380 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4331 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0     3841 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4719 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     4938 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1040 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/StructBase.py
--rw-rw-rw-   0        0        0     2893 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Types.py
--rw-rw-rw-   0        0        0     4530 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Utilities.py
--rw-rw-rw-   0        0        0     4850 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    44232 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     6999 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0        0 2021-05-01 19:09:01.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/__init__.py
--rw-rw-rw-   0        0        0    10718 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/RsCmwWlanSig.py
--rw-rw-rw-   0        0        0      837 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/__init__.py
--rw-rw-rw-   0        0        0    22224 2021-05-16 18:16:13.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/enums.py
--rw-rw-rw-   0        0        0     2319 2021-05-16 18:16:13.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/repcap.py
-drwxrwxrwx   0        0        0        0 2021-05-16 18:16:18.274610 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig.egg-info/
--rw-rw-rw-   0        0        0     3889 2021-05-16 18:16:18.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17643 2021-05-16 18:16:18.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-16 18:16:18.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-05-16 18:16:18.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-05-16 18:16:18.000000 RsCmwWlanSig-3.8.20.40/RsCmwWlanSig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-16 18:16:19.664901 RsCmwWlanSig-3.8.20.40/setup.cfg
--rw-rw-rw-   0        0        0      860 2021-05-16 18:16:17.000000 RsCmwWlanSig-3.8.20.40/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.263920 RsCmwWlanSig-4.0.110/
+-rw-rw-rw-   0        0        0     4328 2024-04-17 08:14:04.263920 RsCmwWlanSig-4.0.110/PKG-INFO
+-rw-rw-rw-   0        0        0     2596 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.566891 RsCmwWlanSig-4.0.110/RsCmwWlanSig/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.593386 RsCmwWlanSig-4.0.110/RsCmwWlanSig/CustomFiles/
+-rw-rw-rw-   0        0        0       90 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     3725 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4916 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    21849 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.593386 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.603385 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.603385 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.613381 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Station/
+-rw-rw-rw-   0        0        0      912 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Station/Connect.py
+-rw-rw-rw-   0        0        0     1023 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Station/Reconnect.py
+-rw-rw-rw-   0        0        0     1297 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Station/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.613381 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Wdirect/
+-rw-rw-rw-   0        0        0      821 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Wdirect/Sconnection.py
+-rw-rw-rw-   0        0        0     1069 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Wdirect/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.623375 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Wps/
+-rw-rw-rw-   0        0        0      809 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Wps/Sconnection.py
+-rw-rw-rw-   0        0        0     1049 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Wps/__init__.py
+-rw-rw-rw-   0        0        0     1486 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.623375 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Sta/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.623375 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Sta/Action/
+-rw-rw-rw-   0        0        0     1158 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Sta/Action/Disconnect.py
+-rw-rw-rw-   0        0        0     1056 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Sta/Action/__init__.py
+-rw-rw-rw-   0        0        0     1853 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Sta/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.633370 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Clean/
+-rw-rw-rw-   0        0        0     1151 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Clean/Elogging.py
+-rw-rw-rw-   0        0        0     1031 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Clean/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.643364 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.663354 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/
+-rw-rw-rw-   0        0        0     2048 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Aid.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.673349 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Association/
+-rw-rw-rw-   0        0        0     2490 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Association/Disass.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.673349 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Association/Sta/
+-rw-rw-rw-   0        0        0     3423 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Association/Sta/MacReserve.py
+-rw-rw-rw-   0        0        0     1893 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Association/Sta/__init__.py
+-rw-rw-rw-   0        0        0     3495 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Association/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.673349 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.701552 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/
+-rw-rw-rw-   0        0        0     1706 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Enable.py
+-rw-rw-rw-   0        0        0     1939 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Ftype.py
+-rw-rw-rw-   0        0        0     1902 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/MwDuration.py
+-rw-rw-rw-   0        0        0     1805 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Stime.py
+-rw-rw-rw-   0        0        0     1779 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Tenable.py
+-rw-rw-rw-   0        0        0     2004 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/__init__.py
+-rw-rw-rw-   0        0        0     1916 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.704144 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Ccode/
+-rw-rw-rw-   0        0        0     3182 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Ccode/Ccconf.py
+-rw-rw-rw-   0        0        0     2139 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Ccode/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/DyFragment.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.721294 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Edca/
+-rw-rw-rw-   0        0        0     2763 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Edca/Acbe.py
+-rw-rw-rw-   0        0        0     2763 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Edca/Acbk.py
+-rw-rw-rw-   0        0        0     2763 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Edca/Acvi.py
+-rw-rw-rw-   0        0        0     2763 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Edca/Acvo.py
+-rw-rw-rw-   0        0        0     1658 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Edca/__init__.py
+-rw-rw-rw-   0        0        0     1352 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hemac.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.727280 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hetf/
+-rw-rw-rw-   0        0        0     1263 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hetf/SsTx.py
+-rw-rw-rw-   0        0        0    11466 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hetf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.740243 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/
+-rw-rw-rw-   0        0        0     3103 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Cutil.py
+-rw-rw-rw-   0        0        0     4290 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Dname.py
+-rw-rw-rw-   0        0        0     4918 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Plmn.py
+-rw-rw-rw-   0        0        0     4679 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Realm.py
+-rw-rw-rw-   0        0        0    11444 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/__init__.py
+-rw-rw-rw-   0        0        0     4305 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/MfDef.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.750394 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Muedca/
+-rw-rw-rw-   0        0        0     2841 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Muedca/Acbe.py
+-rw-rw-rw-   0        0        0     2841 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Muedca/Acbk.py
+-rw-rw-rw-   0        0        0     2841 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Muedca/Acvi.py
+-rw-rw-rw-   0        0        0     2841 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Muedca/Acvo.py
+-rw-rw-rw-   0        0        0     1668 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Muedca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.750394 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/NdpSounding/
+-rw-rw-rw-   0        0        0     1369 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/NdpSounding/SsTx.py
+-rw-rw-rw-   0        0        0    15067 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/NdpSounding/__init__.py
+-rw-rw-rw-   0        0        0     8623 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/OobDiscovery.py
+-rw-rw-rw-   0        0        0     2829 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Qos.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.760390 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.770385 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Eaka/
+-rw-rw-rw-   0        0        0     2927 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Eaka/Kalgo.py
+-rw-rw-rw-   0        0        0     1008 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Eaka/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.780380 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/
+-rw-rw-rw-   0        0        0     2587 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/KtThree.py
+-rw-rw-rw-   0        0        0     2561 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/KtTwo.py
+-rw-rw-rw-   0        0        0     2559 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/Ktone.py
+-rw-rw-rw-   0        0        0     1480 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/__init__.py
+-rw-rw-rw-   0        0        0     3670 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Passphrase.py
+-rw-rw-rw-   0        0        0     2459 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Pkey.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.780380 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Rserver/
+-rw-rw-rw-   0        0        0     2814 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Rserver/Iconf.py
+-rw-rw-rw-   0        0        0     4042 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Rserver/__init__.py
+-rw-rw-rw-   0        0        0     3919 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/TypePy.py
+-rw-rw-rw-   0        0        0     7600 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.790373 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Srates/
+-rw-rw-rw-   0        0        0     3515 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Srates/DsssConf.py
+-rw-rw-rw-   0        0        0    10675 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Srates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.790373 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.790373 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.800368 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/
+-rw-rw-rw-   0        0        0     3530 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/AlsField.py
+-rw-rw-rw-   0        0        0     4490 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/BlAllocation.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.810363 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/Dummy/
+-rw-rw-rw-   0        0        0     2868 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/Dummy/Mcs.py
+-rw-rw-rw-   0        0        0     1829 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/Dummy/__init__.py
+-rw-rw-rw-   0        0        0     4020 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/RuAllocation.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.820358 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/
+-rw-rw-rw-   0        0        0     3734 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Allocation.py
+-rw-rw-rw-   0        0        0     2636 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Ctype.py
+-rw-rw-rw-   0        0        0     2878 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Mcs.py
+-rw-rw-rw-   0        0        0     2673 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Streams.py
+-rw-rw-rw-   0        0        0     2551 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/__init__.py
+-rw-rw-rw-   0        0        0     2050 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/__init__.py
+-rw-rw-rw-   0        0        0     1010 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/__init__.py
+-rw-rw-rw-   0        0        0     1857 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/__init__.py
+-rw-rw-rw-   0        0        0     3323 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Station.py
+-rw-rw-rw-   0        0        0     2843 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/TpControl.py
+-rw-rw-rw-   0        0        0     1223 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Twt.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.820358 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Wdirect/
+-rw-rw-rw-   0        0        0     2445 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Wdirect/Atype.py
+-rw-rw-rw-   0        0        0     2930 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Wdirect/Wdconf.py
+-rw-rw-rw-   0        0        0     1257 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Wdirect/__init__.py
+-rw-rw-rw-   0        0        0    19128 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/__init__.py
+-rw-rw-rw-   0        0        0     3068 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Edau.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.830353 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/
+-rw-rw-rw-   0        0        0     2930 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/DuIp.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.830353 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/IrList/
+-rw-rw-rw-   0        0        0     5299 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/IrList/IprAddress.py
+-rw-rw-rw-   0        0        0     1056 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/IrList/__init__.py
+-rw-rw-rw-   0        0        0     1232 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.840347 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.840347 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Awgn/
+-rw-rw-rw-   0        0        0     1384 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Awgn/Bandwidth.py
+-rw-rw-rw-   0        0        0     2848 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Awgn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.850341 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Fsimulator/
+-rw-rw-rw-   0        0        0      897 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Fsimulator/Iloss.py
+-rw-rw-rw-   0        0        0     3041 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Fsimulator/__init__.py
+-rw-rw-rw-   0        0        0     1274 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/__init__.py
+-rw-rw-rw-   0        0        0     1428 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/HetBased.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.850341 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.860337 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.880326 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/
+-rw-rw-rw-   0        0        0     2592 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Cmw.py
+-rw-rw-rw-   0        0        0     2772 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Destination.py
+-rw-rw-rw-   0        0        0     2630 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Dns.py
+-rw-rw-rw-   0        0        0     2646 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Gateway.py
+-rw-rw-rw-   0        0        0     3440 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Sta.py
+-rw-rw-rw-   0        0        0     2464 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Stack.py
+-rw-rw-rw-   0        0        0     2189 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/__init__.py
+-rw-rw-rw-   0        0        0     2775 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/Smask.py
+-rw-rw-rw-   0        0        0     2124 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/__init__.py
+-rw-rw-rw-   0        0        0     2044 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/__init__.py
+-rw-rw-rw-   0        0        0     1290 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvSix.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.880326 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mimo/
+-rw-rw-rw-   0        0        0     1908 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mimo/Tcsd.py
+-rw-rw-rw-   0        0        0     2484 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mimo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.890320 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mmonitor/
+-rw-rw-rw-   0        0        0     2307 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mmonitor/IpAddress.py
+-rw-rw-rw-   0        0        0     1925 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mmonitor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.893945 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.901860 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.908063 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/
+-rw-rw-rw-   0        0        0     2872 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/AlsField.py
+-rw-rw-rw-   0        0        0     4145 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/BlAllocation.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.916924 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/Dummy/
+-rw-rw-rw-   0        0        0     2239 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/Dummy/Mcs.py
+-rw-rw-rw-   0        0        0     1825 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/Dummy/__init__.py
+-rw-rw-rw-   0        0        0     3361 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/RuAllocation.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.926918 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/
+-rw-rw-rw-   0        0        0     3101 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Allocation.py
+-rw-rw-rw-   0        0        0     2007 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Ctype.py
+-rw-rw-rw-   0        0        0     2235 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Mcs.py
+-rw-rw-rw-   0        0        0     2086 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Streams.py
+-rw-rw-rw-   0        0        0     2547 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/__init__.py
+-rw-rw-rw-   0        0        0     2048 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/__init__.py
+-rw-rw-rw-   0        0        0     1008 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/__init__.py
+-rw-rw-rw-   0        0        0     1302 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Payload.py
+-rw-rw-rw-   0        0        0    13605 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.949070 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/
+-rw-rw-rw-   0        0        0     4545 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/Config.py
+-rw-rw-rw-   0        0        0     2233 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/Destination.py
+-rw-rw-rw-   0        0        0     2096 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/IpVersion.py
+-rw-rw-rw-   0        0        0     2084 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/Protocol.py
+-rw-rw-rw-   0        0        0     2886 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/Uports.py
+-rw-rw-rw-   0        0        0     2986 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.953060 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.960041 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.967060 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/
+-rw-rw-rw-   0        0        0     2257 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/InputPy.py
+-rw-rw-rw-   0        0        0     2272 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/Output.py
+-rw-rw-rw-   0        0        0     1300 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/__init__.py
+-rw-rw-rw-   0        0        0     2502 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/EpePower.py
+-rw-rw-rw-   0        0        0     2132 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/MlOffset.py
+-rw-rw-rw-   0        0        0     2429 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/__init__.py
+-rw-rw-rw-   0        0        0     1348 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Eattenuation.py
+-rw-rw-rw-   0        0        0    13605 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.967060 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.977057 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/
+-rw-rw-rw-   0        0        0     3330 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Ampdu.py
+-rw-rw-rw-   0        0        0     5998 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Dfdef.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.007040 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/
+-rw-rw-rw-   0        0        0     1985 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Ctyp.py
+-rw-rw-rw-   0        0        0     1854 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Dcm.py
+-rw-rw-rw-   0        0        0     2218 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Mcs.py
+-rw-rw-rw-   0        0        0     1857 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Nss.py
+-rw-rw-rw-   0        0        0     4656 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Rual.py
+-rw-rw-rw-   0        0        0     1150 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Sss.py
+-rw-rw-rw-   0        0        0     2548 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/TrsMode.py
+-rw-rw-rw-   0        0        0     1879 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Trssi.py
+-rw-rw-rw-   0        0        0     2133 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/TsrControl.py
+-rw-rw-rw-   0        0        0     2808 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.007040 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/
+-rw-rw-rw-   0        0        0     2210 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/BarMethod.py
+-rw-rw-rw-   0        0        0     3442 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/Black.py
+-rw-rw-rw-   0        0        0     1263 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/__init__.py
+-rw-rw-rw-   0        0        0     1697 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/__init__.py
+-rw-rw-rw-   0        0        0     1886 2024-04-17 08:14:00.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.017035 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/UesInfo/
+-rw-rw-rw-   0        0        0     2262 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/UesInfo/Settings.py
+-rw-rw-rw-   0        0        0     1945 2024-04-17 08:13:59.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/UesInfo/__init__.py
+-rw-rw-rw-   0        0        0     4109 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.027029 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/HetBased/
+-rw-rw-rw-   0        0        0     1345 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/HetBased/State.py
+-rw-rw-rw-   0        0        0     2257 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/HetBased/UphInfo.py
+-rw-rw-rw-   0        0        0     6696 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/HetBased/__init__.py
+-rw-rw-rw-   0        0        0     1461 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/PackRate.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.027029 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Per/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.037024 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Per/State/
+-rw-rw-rw-   0        0        0     2556 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Per/State/All.py
+-rw-rw-rw-   0        0        0     1927 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Per/State/__init__.py
+-rw-rw-rw-   0        0        0     7236 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Per/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.037024 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Pswitched/
+-rw-rw-rw-   0        0        0     1024 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Pswitched/State.py
+-rw-rw-rw-   0        0        0     1027 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Pswitched/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.037024 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.047018 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/
+-rw-rw-rw-   0        0        0     4539 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/MimFading.py
+-rw-rw-rw-   0        0        0     4398 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/Mimo.py
+-rw-rw-rw-   0        0        0     3495 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/ScFading.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.057013 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/Scell/
+-rw-rw-rw-   0        0        0     3732 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/Scell/Flexible.py
+-rw-rw-rw-   0        0        0     1035 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/Scell/__init__.py
+-rw-rw-rw-   0        0        0     2405 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/__init__.py
+-rw-rw-rw-   0        0        0     3941 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.057013 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Second/
+-rw-rw-rw-   0        0        0     1015 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Second/State.py
+-rw-rw-rw-   0        0        0     1012 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Second/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.067008 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/
+-rw-rw-rw-   0        0        0     2096 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Elogging.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.067008 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Pgen/
+-rw-rw-rw-   0        0        0     2388 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Pgen/PgStats.py
+-rw-rw-rw-   0        0        0     1970 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Pgen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.077003 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sinfo/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.077003 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sinfo/Antenna/
+-rw-rw-rw-   0        0        0     1904 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sinfo/Antenna/RxpIndicator.py
+-rw-rw-rw-   0        0        0     1925 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sinfo/Antenna/__init__.py
+-rw-rw-rw-   0        0        0     2294 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sinfo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.077003 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.086997 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/HetbInfo/
+-rw-rw-rw-   0        0        0     1951 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/HetbInfo/UphInfo.py
+-rw-rw-rw-   0        0        0     1042 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/HetbInfo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.086997 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/
+-rw-rw-rw-   0        0        0     2448 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/He.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.102153 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/Mac/
+-rw-rw-rw-   0        0        0     1185 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/Mac/Address.py
+-rw-rw-rw-   0        0        0     1019 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/Mac/__init__.py
+-rw-rw-rw-   0        0        0     1234 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.106892 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/
+-rw-rw-rw-   0        0        0     2664 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/AbsReport.py
+-rw-rw-rw-   0        0        0     2754 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/Drate.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.133111 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/
+-rw-rw-rw-   0        0        0     3355 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hemu.py
+-rw-rw-rw-   0        0        0     3370 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hesu.py
+-rw-rw-rw-   0        0        0     3355 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hetb.py
+-rw-rw-rw-   0        0        0     3358 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Ht.py
+-rw-rw-rw-   0        0        0     3376 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/NoNht.py
+-rw-rw-rw-   0        0        0     3364 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Vht.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/__init__.py
+-rw-rw-rw-   0        0        0     1148 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxbPower.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.133111 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/UeAddress/
+-rw-rw-rw-   0        0        0     1485 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/UeAddress/Ipv.py
+-rw-rw-rw-   0        0        0     1890 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/UeAddress/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/__init__.py
+-rw-rw-rw-   0        0        0     2398 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.133111 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.143106 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/Antenna/
+-rw-rw-rw-   0        0        0     1287 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/Antenna/ArxbPower.py
+-rw-rw-rw-   0        0        0     1901 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/Antenna/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.153030 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/CmwAddress/
+-rw-rw-rw-   0        0        0     1173 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/CmwAddress/Ipv.py
+-rw-rw-rw-   0        0        0     1891 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/CmwAddress/__init__.py
+-rw-rw-rw-   0        0        0     2907 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.158016 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Source/
+-rw-rw-rw-   0        0        0     3114 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Source/State.py
+-rw-rw-rw-   0        0        0     1012 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Source/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.163003 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Third/
+-rw-rw-rw-   0        0        0     1012 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Third/State.py
+-rw-rw-rw-   0        0        0     1007 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Third/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.165972 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.168965 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.176943 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/
+-rw-rw-rw-   0        0        0     2594 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/DsmLength.py
+-rw-rw-rw-   0        0        0     2572 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/OfmLength.py
+-rw-rw-rw-   0        0        0     2959 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/Plength.py
+-rw-rw-rw-   0        0        0    12818 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/__init__.py
+-rw-rw-rw-   0        0        0     1019 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.179936 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Tx/
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.183960 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Tx/MacFrame/
+-rw-rw-rw-   0        0        0     3127 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Tx/MacFrame/Plength.py
+-rw-rw-rw-   0        0        0     2171 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Tx/MacFrame/__init__.py
+-rw-rw-rw-   0        0        0     1018 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Tx/__init__.py
+-rw-rw-rw-   0        0        0     1198 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:04.263920 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/
+-rw-rw-rw-   0        0        0      586 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4165 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1116 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1145 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9097 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5751 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3439 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2546 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5238 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    25419 2024-04-03 11:15:31.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3775 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4768 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    14213 2024-04-03 11:15:31.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Core.py
+-rw-rw-rw-   0        0        0     1386 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/GlobalData.py
+-rw-rw-rw-   0        0        0    60862 2024-04-03 11:15:31.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4785 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2225 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0    16156 2024-04-03 11:15:31.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3518 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4390 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0      387 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Properties.py
+-rw-rw-rw-   0        0        0     4289 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4745 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ScpiEnums.py
+-rw-rw-rw-   0        0        0    35525 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ScpiLogger.py
+-rw-rw-rw-   0        0        0     5098 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5856 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1114 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3608 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Types.py
+-rw-rw-rw-   0        0        0     5498 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5716 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    51976 2024-04-03 11:15:31.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7512 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0       29 2024-02-28 16:27:53.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/__init__.py
+-rw-rw-rw-   0        0        0    15042 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/RsCmwWlanSig.py
+-rw-rw-rw-   0        0        0      912 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/__init__.py
+-rw-rw-rw-   0        0        0    23478 2024-04-17 08:13:58.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/enums.py
+-rw-rw-rw-   0        0        0     2155 2024-04-17 08:13:57.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig/repcap.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:14:03.576887 RsCmwWlanSig-4.0.110/RsCmwWlanSig.egg-info/
+-rw-rw-rw-   0        0        0     4328 2024-04-17 08:14:03.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    15975 2024-04-17 08:14:03.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 08:14:03.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 08:14:03.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-17 08:14:03.000000 RsCmwWlanSig-4.0.110/RsCmwWlanSig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 08:14:04.263920 RsCmwWlanSig-4.0.110/setup.cfg
+-rw-rw-rw-   0        0        0     1473 2024-04-17 08:14:01.000000 RsCmwWlanSig-4.0.110/setup.py
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/CustomFiles/events.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/CustomFiles/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,89 @@
-from typing import Callable
-
-from ..Internal import Core
-
-
-class Events:
-	"""Common Events class.
-	Event-related methods common for all types of drivers."""
-	def __init__(self, core: Core):
-		self._core = core
-
-	@property
-	def io_events_include_data(self) -> bool:
-		"""Returns the current state of the io_events_include_data See the setter for more details."""
-		return self._core.io.io_events_include_data
-
-	@io_events_include_data.setter
-	def io_events_include_data(self, value: bool) -> None:
-		"""If True, the on_write and on_read events include also the sent/received data.
-		Default value is False, to avoid handling potentially big data."""
-		self._core.io.io_events_include_data = value
-
-	@property
-	def before_write_handler(self) -> Callable:
-		"""Returns the handler of before_write events. \n
-		:return: current before_write_handler"""
-		return self._core.io.before_write_handler
-
-	@before_write_handler.setter
-	def before_write_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_write events.
-		The before_write event is invoked before each write operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, cmd: str)
-		:param handler: new handler"""
-		self._core.io.before_write_handler = handler
-
-	@property
-	def on_write_handler(self) -> Callable:
-		"""Returns the handler of on_write events. \n
-		:return: current on_write_handler"""
-		return self._core.io.on_write_handler
-
-	@on_write_handler.setter
-	def on_write_handler(self, handler: Callable) -> None:
-		"""Sets handler for on_write events.
-		The on_write event is invoked every time the driver performs a write operation to the instrument (for each write chunk)
-		Event arguments type: IoTransferEventArgs
-		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
-		:param handler: new handler for all write operations"""
-		self._core.io.on_write_handler = handler
-
-	@property
-	def on_read_handler(self) -> Callable:
-		"""Returns the handler of on_read events. \n
-		:return: current on_read_handler"""
-		return self._core.io.on_read_handler
-
-	@on_read_handler.setter
-	def on_read_handler(self, handler: Callable) -> None:
-		"""Sets handler for on_read events.
-		The on_read event is invoked every time the driver performs a read operation to the instrument.
-		Event arguments type: IoTransferEventArgs
-		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
-		:param handler: new handler for all read operations"""
-		self._core.io.on_read_handler = handler
-
-	@property
-	def before_query_handler(self) -> Callable:
-		"""Returns the handler of before_query events. \n
-		:return: current before_query_handler"""
-		return self._core.io.before_query_handler
-
-	@before_query_handler.setter
-	def before_query_handler(self, handler: Callable) -> None:
-		"""Sets handler for before_query events.
-		The before_query event is invoked before each query operation (only once, not for every chunk)
-		Event prototype: handler(io: Instrument, query: str)
-		:param handler: new handler"""
-		self._core.io.before_query_handler = handler
+"""Event-related methods and properties. Here you can set all the event handlers."""
+
+from typing import Callable
+
+from ..Internal import Core
+
+
+class Events:
+	"""Common Events class.
+	Event-related methods and properties. Here you can set all the event handlers."""
+	def __init__(self, core: Core):
+		self._core = core
+
+	@property
+	def io_events_include_data(self) -> bool:
+		"""Returns the current state of the io_events_include_data See the setter for more details."""
+		return self._core.io.io_events_include_data
+
+	@io_events_include_data.setter
+	def io_events_include_data(self, value: bool) -> None:
+		"""If True, the on_write and on_read events include also the transferred data.
+		Default value is False, to avoid handling potentially big data."""
+		self._core.io.io_events_include_data = value
+
+	@property
+	def before_write_handler(self) -> Callable:
+		"""Returns the handler of before_write events. \n
+		:return: current ``before_write_handler``"""
+		return self._core.io.before_write_handler
+
+	@before_write_handler.setter
+	def before_write_handler(self, handler: Callable) -> None:
+		"""Sets handler for before_write events.
+		The before_write event is invoked before each write operation (only once, not for every chunk)
+		Event prototype: handler(io: Instrument, cmd: str)
+		:param handler: new handler"""
+		self._core.io.before_write_handler = handler
+
+	@property
+	def on_write_handler(self) -> Callable:
+		"""Returns the handler of on_write events. \n
+		:return: current ``on_write_handler``"""
+		return self._core.io.on_write_handler
+
+	@on_write_handler.setter
+	def on_write_handler(self, handler: Callable) -> None:
+		"""Sets handler for on_write events.
+		The on_write event is invoked every time the driver performs a write operation to the instrument (for each write chunk)
+		Event arguments type: IoTransferEventArgs
+		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
+		:param handler: new handler for all write operations"""
+		self._core.io.on_write_handler = handler
+
+	@property
+	def on_read_handler(self) -> Callable:
+		"""Returns the handler of on_read events. \n
+		:return: current ``on_read_handler``"""
+		return self._core.io.on_read_handler
+
+	@on_read_handler.setter
+	def on_read_handler(self, handler: Callable) -> None:
+		"""Sets handler for on_read events.
+		The on_read event is invoked every time the driver performs a read operation to the instrument.
+		Event arguments type: IoTransferEventArgs
+		By default, the event_args do not contain the actual data sent. If you wish to receive them, set the driver.Events.io_events_include_data to True \n
+		:param handler: new handler for all read operations"""
+		self._core.io.on_read_handler = handler
+
+	@property
+	def before_query_handler(self) -> Callable:
+		"""Returns the handler of before_query events. \n
+		:return: current ``before_query_handler``"""
+		return self._core.io.before_query_handler
+
+	@before_query_handler.setter
+	def before_query_handler(self, handler: Callable) -> None:
+		"""Sets handler for before_query events.
+		The before_query event is invoked before each query operation (only once, not for every chunk)
+		Event prototype: handler(io: Instrument, query: str)
+		:param handler: new handler"""
+		self._core.io.before_query_handler = handler
+
+	def sync_from(self, source: 'Events') -> None:
+		"""Synchronises these Events with the source."""
+		self.before_query_handler = source.before_query_handler
+		self.before_write_handler = source.before_write_handler
+		self.io_events_include_data = source.io_events_include_data
+		self.on_read_handler = source.on_read_handler
+		self.on_write_handler = source.on_write_handler
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/CustomFiles/reliability.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/CustomFiles/reliability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Class for R&S Mobile Radio Test instruments that use reliability indicators."""
+
+
 import time
 from typing import Callable
 
 from ..Internal import ArgLinkedEventArgs
 from ..Internal import Core
 
 codes_table = {
@@ -60,25 +63,25 @@
 		self.context = context
 
 
 class Reliability:
 	"""Reliability class that handles all the necessary tasks related to reliability indicator."""
 
 	def __init__(self, core: Core):
-		self._core = core
-		self._last_value = 0
-		self._last_context = ''
+		self._core: Core = core
+		self._last_value: int = 0
+		self._last_context: str = ''
 		self._last_timestamp = None
 		self._exception_on_error = False
 		# noinspection PyTypeChecker
 		self._on_update_handler: Callable = None
 		self._core.set_link_handler('Reliability', self._permanent_on_update_handler)
 
 	@property
-	def last_value(self):
+	def last_value(self) -> int:
 		"""Returns the last updated Reliability code."""
 		return self._last_value
 
 	@property
 	def last_context(self) -> str:
 		"""Returns the last updated Context of the reliability code - usually the SCPI query on which the instrument responded with the Reliability code."""
 		return self._last_context
@@ -94,36 +97,39 @@
 		if self._last_value in codes_table:
 			return codes_table[self._last_value]
 		else:
 			return f'Undefined reliability code {self._last_value}.'
 
 	@property
 	def exception_on_error(self) -> bool:
-		"""see the exception_on_error.setter."""
+		"""If True, (default is False) the object throws an exception if the updated reliability is not 0 (non-OK)."""
 		return self._exception_on_error
 
 	@exception_on_error.setter
 	def exception_on_error(self, value) -> None:
 		"""If True, (default is False) the object throws an exception if the updated reliability is not 0 (non-OK)."""
 		self._exception_on_error = value
 
 	def on_update_handler(self, handler: Callable) -> None:
 		"""Register the handler for on_update event.
 		This handler is invoked with each update of the reliability indicator.
 		Handler API: handler(event_args: ReliabilityEventArgs)"""
 		self._on_update_handler = handler
 
-	def _permanent_on_update_handler(self, event_args: ArgLinkedEventArgs):
+	def _permanent_on_update_handler(self, event_args: ArgLinkedEventArgs) -> None:
 		"""Permanent on_update handler. Takes care of updating all the 'last_xxx' values and calling a user-defined updated_handler."""
 		self._last_value = int(str(event_args.value))
 		self._last_context = event_args.context
 		self._last_timestamp = event_args.timestamp
-
 		if self._on_update_handler:
 			# Call the additional handler if registered
 			rel_events_args = ReliabilityEventArgs(self._last_timestamp, self._last_value, self.last_message, self._last_context)
 			self._on_update_handler(rel_events_args)
-
 		if self._exception_on_error and self._last_value != 0:
 			raise Exception(
 				f'Reliability indicator error. Time: {time.strftime("%H:%M:%S", time.localtime(self._last_timestamp))}, '
 				f'Context: {self._last_context}, Value {self._last_value}: {self.last_message}')
+
+	def sync_from(self, source: 'Reliability') -> None:
+		"""Synchronises this Reliability with the source."""
+		self.exception_on_error = source.exception_on_error
+		self.on_update_handler(source._on_update_handler)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Call:
-	"""Call commands group definition. 5 total commands, 2 Sub-groups, 0 group commands"""
+class ActionCls:
+	"""Action commands group definition. 4 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("call", core, parent)
+		self._cmd_group = CommandsGroup("action", core, parent)
 
 	@property
-	def action(self):
-		"""action commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_action'):
-			from .Call_.Action import Action
-			self._action = Action(self._core, self._base)
-		return self._action
+	def wps(self):
+		"""wps commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_wps'):
+			from .Wps import WpsCls
+			self._wps = WpsCls(self._core, self._cmd_group)
+		return self._wps
 
 	@property
-	def sta(self):
-		"""sta commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_sta'):
-			from .Call_.Sta import Sta
-			self._sta = Sta(self._core, self._base)
-		return self._sta
+	def wdirect(self):
+		"""wdirect commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_wdirect'):
+			from .Wdirect import WdirectCls
+			self._wdirect = WdirectCls(self._core, self._cmd_group)
+		return self._wdirect
 
-	def clone(self) -> 'Call':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def station(self):
+		"""station commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_station'):
+			from .Station import StationCls
+			self._station = StationCls(self._core, self._cmd_group)
+		return self._station
+
+	def clone(self) -> 'ActionCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Call(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = ActionCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Action:
-	"""Action commands group definition. 4 total commands, 3 Sub-groups, 0 group commands"""
+class CallCls:
+	"""Call commands group definition. 5 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("action", core, parent)
+		self._cmd_group = CommandsGroup("call", core, parent)
 
 	@property
-	def wps(self):
-		"""wps commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_wps'):
-			from .Action_.Wps import Wps
-			self._wps = Wps(self._core, self._base)
-		return self._wps
+	def action(self):
+		"""action commands group. 3 Sub-classes, 0 commands."""
+		if not hasattr(self, '_action'):
+			from .Action import ActionCls
+			self._action = ActionCls(self._core, self._cmd_group)
+		return self._action
 
 	@property
-	def wdirect(self):
-		"""wdirect commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_wdirect'):
-			from .Action_.Wdirect import Wdirect
-			self._wdirect = Wdirect(self._core, self._base)
-		return self._wdirect
+	def sta(self):
+		"""sta commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_sta'):
+			from .Sta import StaCls
+			self._sta = StaCls(self._core, self._cmd_group)
+		return self._sta
 
-	@property
-	def station(self):
-		"""station commands group. 2 Sub-classes, 0 commands."""
-		if not hasattr(self, '_station'):
-			from .Action_.Station import Station
-			self._station = Station(self._core, self._base)
-		return self._station
-
-	def clone(self) -> 'Action':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'CallCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Action(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = CallCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Station.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Wdirect/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Station:
-	"""Station commands group definition. 2 total commands, 2 Sub-groups, 0 group commands"""
+class WdirectCls:
+	"""Wdirect commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("station", core, parent)
+		self._cmd_group = CommandsGroup("wdirect", core, parent)
 
 	@property
-	def reconnect(self):
-		"""reconnect commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_reconnect'):
-			from .Station_.Reconnect import Reconnect
-			self._reconnect = Reconnect(self._core, self._base)
-		return self._reconnect
+	def sconnection(self):
+		"""sconnection commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_sconnection'):
+			from .Sconnection import SconnectionCls
+			self._sconnection = SconnectionCls(self._core, self._cmd_group)
+		return self._sconnection
 
-	@property
-	def connect(self):
-		"""connect commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_connect'):
-			from .Station_.Connect import Connect
-			self._connect = Connect(self._core, self._base)
-		return self._connect
-
-	def clone(self) -> 'Station':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'WdirectCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Station(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = WdirectCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Station_/Connect.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Station/Reconnect.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Connect:
-	"""Connect commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class ReconnectCls:
+	"""Reconnect commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("connect", core, parent)
+		self._cmd_group = CommandsGroup("reconnect", core, parent)
 
-	def set(self) -> None:
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:CONNect \n
-		Snippet: driver.call.action.station.connect.set() \n
-		Initiates an association to the AP under test. The command is only relevant in the operation mode 'Station' with
-		connection mode 'Manual'. \n
-		"""
-		self._core.io.write(f'CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:CONNect')
-
-	def set_with_opc(self) -> None:
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:CONNect \n
-		Snippet: driver.call.action.station.connect.set_with_opc() \n
-		Initiates an association to the AP under test. The command is only relevant in the operation mode 'Station' with
-		connection mode 'Manual'. \n
-		Same as set, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:CONNect')
+	def set(self, opc_timeout_ms: int = -1) -> None:
+		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:REConnect \n
+		Snippet: driver.call.action.station.reconnect.set() \n
+		Re-establishes the existing association to the AP under test. The command has the same effect as a disconnect, followed
+		immediately by a connect. The command is only relevant in the operation mode 'Station' with connection mode 'Manual'. \n
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:REConnect', opc_timeout_ms)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Station_/Reconnect.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hetf/SsTx.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Reconnect:
-	"""Reconnect commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class SsTxCls:
+	"""SsTx commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("reconnect", core, parent)
+		self._cmd_group = CommandsGroup("ssTx", core, parent)
 
 	def set(self) -> None:
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:REConnect \n
-		Snippet: driver.call.action.station.reconnect.set() \n
-		Re-establishes the existing association to the AP under test. The command has the same effect as a disconnect, followed
-		immediately by a connect. The command is only relevant in the operation mode 'Station' with connection mode 'Manual'. \n
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HETF:SSTX \n
+		Snippet: driver.configure.connection.hetf.ssTx.set() \n
+		Transmits the trigger frame once. \n
 		"""
-		self._core.io.write(f'CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:REConnect')
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HETF:SSTX')
 
-	def set_with_opc(self) -> None:
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:REConnect \n
-		Snippet: driver.call.action.station.reconnect.set_with_opc() \n
-		Re-establishes the existing association to the AP under test. The command has the same effect as a disconnect, followed
-		immediately by a connect. The command is only relevant in the operation mode 'Station' with connection mode 'Manual'. \n
+	def set_with_opc(self, opc_timeout_ms: int = -1) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HETF:SSTX \n
+		Snippet: driver.configure.connection.hetf.ssTx.set_with_opc() \n
+		Transmits the trigger frame once. \n
 		Same as set, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:REConnect')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HETF:SSTX', opc_timeout_ms)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wdirect.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Sta/Action/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Wdirect:
-	"""Wdirect commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class ActionCls:
+	"""Action commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("wdirect", core, parent)
+		self._cmd_group = CommandsGroup("action", core, parent)
 
 	@property
-	def sconnection(self):
-		"""sconnection commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_sconnection'):
-			from .Wdirect_.Sconnection import Sconnection
-			self._sconnection = Sconnection(self._core, self._base)
-		return self._sconnection
+	def disconnect(self):
+		"""disconnect commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_disconnect'):
+			from .Disconnect import DisconnectCls
+			self._disconnect = DisconnectCls(self._core, self._cmd_group)
+		return self._disconnect
 
-	def clone(self) -> 'Wdirect':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'ActionCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Wdirect(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = ActionCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wdirect_/Sconnection.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Station/Connect.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sconnection:
-	"""Sconnection commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class ConnectCls:
+	"""Connect commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sconnection", core, parent)
+		self._cmd_group = CommandsGroup("connect", core, parent)
 
-	def set(self) -> None:
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:WDIRect:SCONnection \n
-		Snippet: driver.call.action.wdirect.sconnection.set() \n
-		No command help available \n
-		"""
-		self._core.io.write(f'CALL:WLAN:SIGNaling<Instance>:ACTion:WDIRect:SCONnection')
-
-	def set_with_opc(self) -> None:
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:WDIRect:SCONnection \n
-		Snippet: driver.call.action.wdirect.sconnection.set_with_opc() \n
-		No command help available \n
-		Same as set, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'CALL:WLAN:SIGNaling<Instance>:ACTion:WDIRect:SCONnection')
+	def set(self, opc_timeout_ms: int = -1) -> None:
+		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:CONNect \n
+		Snippet: driver.call.action.station.connect.set() \n
+		Initiates an association to the AP under test. The command is only relevant in the operation mode 'Station' with
+		connection mode 'Manual'. \n
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'CALL:WLAN:SIGNaling<Instance>:ACTion:STATion:CONNect', opc_timeout_ms)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wps.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Station/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Wps:
-	"""Wps commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class StationCls:
+	"""Station commands group definition. 2 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("wps", core, parent)
+		self._cmd_group = CommandsGroup("station", core, parent)
 
 	@property
-	def sconnection(self):
-		"""sconnection commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_sconnection'):
-			from .Wps_.Sconnection import Sconnection
-			self._sconnection = Sconnection(self._core, self._base)
-		return self._sconnection
+	def reconnect(self):
+		"""reconnect commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_reconnect'):
+			from .Reconnect import ReconnectCls
+			self._reconnect = ReconnectCls(self._core, self._cmd_group)
+		return self._reconnect
 
-	def clone(self) -> 'Wps':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def connect(self):
+		"""connect commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_connect'):
+			from .Connect import ConnectCls
+			self._connect = ConnectCls(self._core, self._cmd_group)
+		return self._connect
+
+	def clone(self) -> 'StationCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Wps(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = StationCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Action_/Wps_/Sconnection.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Action/Wps/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sconnection:
-	"""Sconnection commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class WpsCls:
+	"""Wps commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sconnection", core, parent)
+		self._cmd_group = CommandsGroup("wps", core, parent)
 
-	def set(self) -> None:
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:WPS:SCONnection \n
-		Snippet: driver.call.action.wps.sconnection.set() \n
-		No command help available \n
-		"""
-		self._core.io.write(f'CALL:WLAN:SIGNaling<Instance>:ACTion:WPS:SCONnection')
+	@property
+	def sconnection(self):
+		"""sconnection commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_sconnection'):
+			from .Sconnection import SconnectionCls
+			self._sconnection = SconnectionCls(self._core, self._cmd_group)
+		return self._sconnection
 
-	def set_with_opc(self) -> None:
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:ACTion:WPS:SCONnection \n
-		Snippet: driver.call.action.wps.sconnection.set_with_opc() \n
-		No command help available \n
-		Same as set, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'CALL:WLAN:SIGNaling<Instance>:ACTion:WPS:SCONnection')
+	def clone(self) -> 'WpsCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
+		Also copies all the existing default Repeated Capabilities setting,
+		which you can change independently without affecting the original group"""
+		new_group = WpsCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
+		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Sta/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal.RepeatedCapability import RepeatedCapability
-from ... import repcap
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.RepeatedCapability import RepeatedCapability
+from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sta:
-	"""Sta commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
+class StaCls:
+	"""Sta commands group definition. 1 total commands, 1 Subgroups, 0 group commands
 	Repeated Capability: Station, default value after init: Station.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sta", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
+		self._cmd_group = CommandsGroup("sta", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
 
-	def repcap_station_set(self, enum_value: repcap.Station) -> None:
+	def repcap_station_set(self, station: repcap.Station) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Station.Default
 		Default value after init: Station.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(station)
 
 	def repcap_station_get(self) -> repcap.Station:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def action(self):
 		"""action commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_action'):
-			from .Sta_.Action import Action
-			self._action = Action(self._core, self._base)
+			from .Action import ActionCls
+			self._action = ActionCls(self._core, self._cmd_group)
 		return self._action
 
-	def clone(self) -> 'Sta':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'StaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Sta(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = StaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta_/Action.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Pswitched/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Action:
-	"""Action commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class PswitchedCls:
+	"""Pswitched commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("action", core, parent)
+		self._cmd_group = CommandsGroup("pswitched", core, parent)
 
 	@property
-	def disconnect(self):
-		"""disconnect commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_disconnect'):
-			from .Action_.Disconnect import Disconnect
-			self._disconnect = Disconnect(self._core, self._base)
-		return self._disconnect
+	def state(self):
+		"""state commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_state'):
+			from .State import StateCls
+			self._state = StateCls(self._core, self._cmd_group)
+		return self._state
 
-	def clone(self) -> 'Action':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PswitchedCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Action(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PswitchedCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Call_/Sta_/Action_/Disconnect.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Call/Sta/Action/Disconnect.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Disconnect:
-	"""Disconnect commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class DisconnectCls:
+	"""Disconnect commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("disconnect", core, parent)
+		self._cmd_group = CommandsGroup("disconnect", core, parent)
 
-	def set(self, station=repcap.Station.Default) -> None:
+	def set(self, station=repcap.Station.Default, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: CALL:WLAN:SIGNaling<Instance>:STA<s>:ACTion:DISConnect \n
 		Snippet: driver.call.sta.action.disconnect.set(station = repcap.Station.Default) \n
 		Disassociates and deauthenticates the DUT by sending a deauthentication frame. \n
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		self._core.io.write(f'CALL:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:ACTion:DISConnect')
-
-	def set_with_opc(self, station=repcap.Station.Default) -> None:
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		"""SCPI: CALL:WLAN:SIGNaling<Instance>:STA<s>:ACTion:DISConnect \n
-		Snippet: driver.call.sta.action.disconnect.set_with_opc(station = repcap.Station.Default) \n
-		Disassociates and deauthenticates the DUT by sending a deauthentication frame. \n
-		Same as set, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		self._core.io.write_with_opc(f'CALL:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:ACTion:DISConnect')
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		self._core.io.write_with_opc(f'CALL:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:ACTion:DISConnect', opc_timeout_ms)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Clean.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Clean:
-	"""Clean commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class QosCls:
+	"""Qos commands group definition. 2 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("clean", core, parent)
+		self._cmd_group = CommandsGroup("qos", core, parent)
 
 	@property
-	def elogging(self):
-		"""elogging commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_elogging'):
-			from .Clean_.Elogging import Elogging
-			self._elogging = Elogging(self._core, self._base)
-		return self._elogging
+	def barMethod(self):
+		"""barMethod commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_barMethod'):
+			from .BarMethod import BarMethodCls
+			self._barMethod = BarMethodCls(self._core, self._cmd_group)
+		return self._barMethod
 
-	def clone(self) -> 'Clean':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def black(self):
+		"""black commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_black'):
+			from .Black import BlackCls
+			self._black = BlackCls(self._core, self._cmd_group)
+		return self._black
+
+	def clone(self) -> 'QosCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Clean(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = QosCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Clean_/Elogging.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Clean/Elogging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Elogging:
-	"""Elogging commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class EloggingCls:
+	"""Elogging commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("elogging", core, parent)
+		self._cmd_group = CommandsGroup("elogging", core, parent)
 
 	def set(self) -> None:
 		"""SCPI: CLEan:WLAN:SIGNaling<instance>:ELOGging \n
 		Snippet: driver.clean.elogging.set() \n
 		Clears the event log. \n
 		"""
 		self._core.io.write(f'CLEan:WLAN:SIGNaling<Instance>:ELOGging')
 
-	def set_with_opc(self) -> None:
+	def set_with_opc(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: CLEan:WLAN:SIGNaling<instance>:ELOGging \n
 		Snippet: driver.clean.elogging.set_with_opc() \n
 		Clears the event log. \n
 		Same as set, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'CLEan:WLAN:SIGNaling<Instance>:ELOGging')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'CLEan:WLAN:SIGNaling<Instance>:ELOGging', opc_timeout_ms)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Configure:
-	"""Configure commands group definition. 179 total commands, 14 Sub-groups, 0 group commands"""
+class ConfigureCls:
+	"""Configure commands group definition. 193 total commands, 14 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("configure", core, parent)
+		self._cmd_group = CommandsGroup("configure", core, parent)
 
 	@property
 	def fading(self):
 		"""fading commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_fading'):
-			from .Configure_.Fading import Fading
-			self._fading = Fading(self._core, self._base)
+			from .Fading import FadingCls
+			self._fading = FadingCls(self._core, self._cmd_group)
 		return self._fading
 
 	@property
 	def edau(self):
 		"""edau commands group. 0 Sub-classes, 3 commands."""
 		if not hasattr(self, '_edau'):
-			from .Configure_.Edau import Edau
-			self._edau = Edau(self._core, self._base)
+			from .Edau import EdauCls
+			self._edau = EdauCls(self._core, self._cmd_group)
 		return self._edau
 
 	@property
 	def mimo(self):
-		"""mimo commands group. 0 Sub-classes, 2 commands."""
+		"""mimo commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mimo'):
-			from .Configure_.Mimo import Mimo
-			self._mimo = Mimo(self._core, self._base)
+			from .Mimo import MimoCls
+			self._mimo = MimoCls(self._core, self._cmd_group)
 		return self._mimo
 
 	@property
 	def uesInfo(self):
-		"""uesInfo commands group. 0 Sub-classes, 2 commands."""
+		"""uesInfo commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_uesInfo'):
-			from .Configure_.UesInfo import UesInfo
-			self._uesInfo = UesInfo(self._core, self._base)
+			from .UesInfo import UesInfoCls
+			self._uesInfo = UesInfoCls(self._core, self._cmd_group)
 		return self._uesInfo
 
 	@property
 	def etoe(self):
-		"""etoe commands group. 1 Sub-classes, 1 commands."""
+		"""etoe commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_etoe'):
-			from .Configure_.Etoe import Etoe
-			self._etoe = Etoe(self._core, self._base)
+			from .Etoe import EtoeCls
+			self._etoe = EtoeCls(self._core, self._cmd_group)
 		return self._etoe
 
 	@property
 	def rfSettings(self):
 		"""rfSettings commands group. 2 Sub-classes, 12 commands."""
 		if not hasattr(self, '_rfSettings'):
-			from .Configure_.RfSettings import RfSettings
-			self._rfSettings = RfSettings(self._core, self._base)
+			from .RfSettings import RfSettingsCls
+			self._rfSettings = RfSettingsCls(self._core, self._cmd_group)
 		return self._rfSettings
 
 	@property
 	def connection(self):
-		"""connection commands group. 16 Sub-classes, 16 commands."""
+		"""connection commands group. 21 Sub-classes, 13 commands."""
 		if not hasattr(self, '_connection'):
-			from .Configure_.Connection import Connection
-			self._connection = Connection(self._core, self._base)
+			from .Connection import ConnectionCls
+			self._connection = ConnectionCls(self._core, self._cmd_group)
 		return self._connection
 
 	@property
 	def sta(self):
 		"""sta commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_sta'):
-			from .Configure_.Sta import Sta
-			self._sta = Sta(self._core, self._base)
+			from .Sta import StaCls
+			self._sta = StaCls(self._core, self._cmd_group)
 		return self._sta
 
 	@property
 	def pgen(self):
 		"""pgen commands group. 5 Sub-classes, 0 commands."""
 		if not hasattr(self, '_pgen'):
-			from .Configure_.Pgen import Pgen
-			self._pgen = Pgen(self._core, self._base)
+			from .Pgen import PgenCls
+			self._pgen = PgenCls(self._core, self._cmd_group)
 		return self._pgen
 
 	@property
 	def ipvSix(self):
 		"""ipvSix commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ipvSix'):
-			from .Configure_.IpvSix import IpvSix
-			self._ipvSix = IpvSix(self._core, self._base)
+			from .IpvSix import IpvSixCls
+			self._ipvSix = IpvSixCls(self._core, self._cmd_group)
 		return self._ipvSix
 
 	@property
 	def ipvFour(self):
 		"""ipvFour commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ipvFour'):
-			from .Configure_.IpvFour import IpvFour
-			self._ipvFour = IpvFour(self._core, self._base)
+			from .IpvFour import IpvFourCls
+			self._ipvFour = IpvFourCls(self._core, self._cmd_group)
 		return self._ipvFour
 
 	@property
 	def hetBased(self):
 		"""hetBased commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_hetBased'):
-			from .Configure_.HetBased import HetBased
-			self._hetBased = HetBased(self._core, self._base)
+			from .HetBased import HetBasedCls
+			self._hetBased = HetBasedCls(self._core, self._cmd_group)
 		return self._hetBased
 
 	@property
 	def per(self):
 		"""per commands group. 2 Sub-classes, 8 commands."""
 		if not hasattr(self, '_per'):
-			from .Configure_.Per import Per
-			self._per = Per(self._core, self._base)
+			from .Per import PerCls
+			self._per = PerCls(self._core, self._cmd_group)
 		return self._per
 
 	@property
 	def mmonitor(self):
 		"""mmonitor commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mmonitor'):
-			from .Configure_.Mmonitor import Mmonitor
-			self._mmonitor = Mmonitor(self._core, self._base)
+			from .Mmonitor import MmonitorCls
+			self._mmonitor = MmonitorCls(self._core, self._cmd_group)
 		return self._mmonitor
 
-	def clone(self) -> 'Configure':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'ConfigureCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Configure(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = ConfigureCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,150 +1,188 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal import Conversions
-from ...Internal.Utilities import trim_str_response
-from ...Internal.StructBase import StructBase
-from ...Internal.ArgStruct import ArgStruct
-from ... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
+from ....Internal.Utilities import trim_str_response
+from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Connection:
-	"""Connection commands group definition. 100 total commands, 16 Sub-groups, 16 group commands"""
+class ConnectionCls:
+	"""Connection commands group definition. 114 total commands, 21 Subgroups, 13 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("connection", core, parent)
+		self._cmd_group = CommandsGroup("connection", core, parent)
 
 	@property
 	def association(self):
-		"""association commands group. 1 Sub-classes, 3 commands."""
+		"""association commands group. 2 Sub-classes, 2 commands."""
 		if not hasattr(self, '_association'):
-			from .Connection_.Association import Association
-			self._association = Association(self._core, self._base)
+			from .Association import AssociationCls
+			self._association = AssociationCls(self._core, self._cmd_group)
 		return self._association
 
 	@property
 	def hotspot(self):
-		"""hotspot commands group. 3 Sub-classes, 4 commands."""
+		"""hotspot commands group. 4 Sub-classes, 3 commands."""
 		if not hasattr(self, '_hotspot'):
-			from .Connection_.Hotspot import Hotspot
-			self._hotspot = Hotspot(self._core, self._base)
+			from .Hotspot import HotspotCls
+			self._hotspot = HotspotCls(self._core, self._cmd_group)
 		return self._hotspot
 
 	@property
 	def wdirect(self):
-		"""wdirect commands group. 0 Sub-classes, 2 commands."""
+		"""wdirect commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_wdirect'):
-			from .Connection_.Wdirect import Wdirect
-			self._wdirect = Wdirect(self._core, self._base)
+			from .Wdirect import WdirectCls
+			self._wdirect = WdirectCls(self._core, self._cmd_group)
 		return self._wdirect
 
 	@property
 	def station(self):
 		"""station commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_station'):
-			from .Connection_.Station import Station
-			self._station = Station(self._core, self._base)
+			from .Station import StationCls
+			self._station = StationCls(self._core, self._cmd_group)
 		return self._station
 
 	@property
 	def security(self):
-		"""security commands group. 3 Sub-classes, 3 commands."""
+		"""security commands group. 6 Sub-classes, 4 commands."""
 		if not hasattr(self, '_security'):
-			from .Connection_.Security import Security
-			self._security = Security(self._core, self._base)
+			from .Security import SecurityCls
+			self._security = SecurityCls(self._core, self._cmd_group)
 		return self._security
 
 	@property
 	def qos(self):
 		"""qos commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_qos'):
-			from .Connection_.Qos import Qos
-			self._qos = Qos(self._core, self._base)
+			from .Qos import QosCls
+			self._qos = QosCls(self._core, self._cmd_group)
 		return self._qos
 
 	@property
 	def srates(self):
-		"""srates commands group. 0 Sub-classes, 5 commands."""
+		"""srates commands group. 1 Sub-classes, 4 commands."""
 		if not hasattr(self, '_srates'):
-			from .Connection_.Srates import Srates
-			self._srates = Srates(self._core, self._base)
+			from .Srates import SratesCls
+			self._srates = SratesCls(self._core, self._cmd_group)
 		return self._srates
 
 	@property
+	def mfDef(self):
+		"""mfDef commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_mfDef'):
+			from .MfDef import MfDefCls
+			self._mfDef = MfDefCls(self._core, self._cmd_group)
+		return self._mfDef
+
+	@property
 	def sta(self):
 		"""sta commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_sta'):
-			from .Connection_.Sta import Sta
-			self._sta = Sta(self._core, self._base)
+			from .Sta import StaCls
+			self._sta = StaCls(self._core, self._cmd_group)
 		return self._sta
 
 	@property
 	def hetf(self):
 		"""hetf commands group. 1 Sub-classes, 10 commands."""
 		if not hasattr(self, '_hetf'):
-			from .Connection_.Hetf import Hetf
-			self._hetf = Hetf(self._core, self._base)
+			from .Hetf import HetfCls
+			self._hetf = HetfCls(self._core, self._cmd_group)
 		return self._hetf
 
 	@property
 	def ccode(self):
-		"""ccode commands group. 0 Sub-classes, 2 commands."""
+		"""ccode commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ccode'):
-			from .Connection_.Ccode import Ccode
-			self._ccode = Ccode(self._core, self._base)
+			from .Ccode import CcodeCls
+			self._ccode = CcodeCls(self._core, self._cmd_group)
 		return self._ccode
 
 	@property
 	def edca(self):
-		"""edca commands group. 0 Sub-classes, 4 commands."""
+		"""edca commands group. 4 Sub-classes, 0 commands."""
 		if not hasattr(self, '_edca'):
-			from .Connection_.Edca import Edca
-			self._edca = Edca(self._core, self._base)
+			from .Edca import EdcaCls
+			self._edca = EdcaCls(self._core, self._cmd_group)
 		return self._edca
 
 	@property
 	def muedca(self):
-		"""muedca commands group. 0 Sub-classes, 4 commands."""
+		"""muedca commands group. 4 Sub-classes, 0 commands."""
 		if not hasattr(self, '_muedca'):
-			from .Connection_.Muedca import Muedca
-			self._muedca = Muedca(self._core, self._base)
+			from .Muedca import MuedcaCls
+			self._muedca = MuedcaCls(self._core, self._cmd_group)
 		return self._muedca
 
 	@property
+	def tpControl(self):
+		"""tpControl commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_tpControl'):
+			from .TpControl import TpControlCls
+			self._tpControl = TpControlCls(self._core, self._cmd_group)
+		return self._tpControl
+
+	@property
+	def oobDiscovery(self):
+		"""oobDiscovery commands group. 0 Sub-classes, 8 commands."""
+		if not hasattr(self, '_oobDiscovery'):
+			from .OobDiscovery import OobDiscoveryCls
+			self._oobDiscovery = OobDiscoveryCls(self._core, self._cmd_group)
+		return self._oobDiscovery
+
+	@property
 	def hemac(self):
 		"""hemac commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_hemac'):
-			from .Connection_.Hemac import Hemac
-			self._hemac = Hemac(self._core, self._base)
+			from .Hemac import HemacCls
+			self._hemac = HemacCls(self._core, self._cmd_group)
 		return self._hemac
 
 	@property
 	def ndpSounding(self):
 		"""ndpSounding commands group. 1 Sub-classes, 13 commands."""
 		if not hasattr(self, '_ndpSounding'):
-			from .Connection_.NdpSounding import NdpSounding
-			self._ndpSounding = NdpSounding(self._core, self._base)
+			from .NdpSounding import NdpSoundingCls
+			self._ndpSounding = NdpSoundingCls(self._core, self._cmd_group)
 		return self._ndpSounding
 
 	@property
+	def aid(self):
+		"""aid commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_aid'):
+			from .Aid import AidCls
+			self._aid = AidCls(self._core, self._cmd_group)
+		return self._aid
+
+	@property
+	def dyFragment(self):
+		"""dyFragment commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_dyFragment'):
+			from .DyFragment import DyFragmentCls
+			self._dyFragment = DyFragmentCls(self._core, self._cmd_group)
+		return self._dyFragment
+
+	@property
 	def twt(self):
 		"""twt commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_twt'):
-			from .Connection_.Twt import Twt
-			self._twt = Twt(self._core, self._base)
+			from .Twt import TwtCls
+			self._twt = TwtCls(self._core, self._cmd_group)
 		return self._twt
 
 	@property
 	def btwt(self):
 		"""btwt commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_btwt'):
-			from .Connection_.Btwt import Btwt
-			self._btwt = Btwt(self._core, self._base)
+			from .Btwt import BtwtCls
+			self._btwt = BtwtCls(self._core, self._cmd_group)
 		return self._btwt
 
 	# noinspection PyTypeChecker
 	def get_iv_support(self) -> enums.IpVersionExt:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:IVSupport \n
 		Snippet: value: enums.IpVersionExt = driver.configure.connection.get_iv_support() \n
 		Defines the required IP version support. \n
@@ -232,63 +270,29 @@
 		Snippet: driver.configure.connection.set_pa_interrupt(enable = False) \n
 		No command help available \n
 			:param enable: No help available
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:PAINterrupt {param}')
 
-	# noinspection PyTypeChecker
-	class MfDefStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- State: enums.EnableState: DISable | ENABle Disables/enables the user-defined frame rate control
-			- Format_Py: enums.DataFormatExt: NHT | HTM | VHT | HES | HEM Selects the frame format NHT: non-high throughput format (non-HT) HTM: HT mixed format (HT MF) VHT: very high throughput format HES: high efficiency single-user format (HE SU) HEM: high efficiency multi-user format (HE MU)
-			- Rate: enums.Coderate: D1MBit | D2MBits | C55Mbits | C11Mbits | BR12 | BR34 | QR12 | QR34 | Q1M12 | Q1M34 | Q6M23 | Q6M34 | MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 | MCS12 | MCS13 | MCS14 | MCS15 Sets the rate D1MBit: DSSS, 1 Mbit/s D2MBits: DSSS, 2 Mbit/s C55Mbits: CCK, 5.5 Mbit/s C11Mbits: CCK, 11 Mbit/s BR12: BPSK, 1/2, 6 Mbit/s BR34: BPSK, 3/4, 9 Mbit/s QR12: QPSK, 1/2, 12 Mbit/s QR34: QPSK, 3/4, 18 Mbit/s Q1M12: 16-QAM, 1/2, 24 Mbit/s Q1M34: 16-QAM, 3/4, 36 Mbit/s Q6M23: 64-QAM, 2/3, 48 Mbit/s Q6M34: 64-QAM, 3/4, 54 Mbit/s MCS, MCS1,...,MCS15: MCS 0 to MCS 15"""
-		__meta_args_list = [
-			ArgStruct.scalar_enum('State', enums.EnableState),
-			ArgStruct.scalar_enum('Format_Py', enums.DataFormatExt),
-			ArgStruct.scalar_enum('Rate', enums.Coderate)]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.State: enums.EnableState = None
-			self.Format_Py: enums.DataFormatExt = None
-			self.Rate: enums.Coderate = None
-
-	# noinspection PyTypeChecker
-	def get_mf_def(self) -> MfDefStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MFDef \n
-		Snippet: value: MfDefStruct = driver.configure.connection.get_mf_def() \n
-		Enables and configures the user-defined frame rate control for management frames. \n
-			:return: structure: for return value, see the help for MfDefStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MFDef?', self.__class__.MfDefStruct())
-
-	def set_mf_def(self, value: MfDefStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MFDef \n
-		Snippet: driver.configure.connection.set_mf_def(value = MfDefStruct()) \n
-		Enables and configures the user-defined frame rate control for management frames. \n
-			:param value: see the help for MfDefStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MFDef', value)
-
 	def get_sync(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SYNC \n
 		Snippet: value: bool = driver.configure.connection.get_sync() \n
 		If enabled, the PER measurements use identical settings as configured in the signaling application. Refer to the 'Data
-		Frame Control Settings'. \n
+		frame control settings'. \n
 			:return: sync: OFF | ON
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SYNC?')
 		return Conversions.str_to_bool(response)
 
 	def set_sync(self, sync: bool) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SYNC \n
 		Snippet: driver.configure.connection.set_sync(sync = False) \n
 		If enabled, the PER measurements use identical settings as configured in the signaling application. Refer to the 'Data
-		Frame Control Settings'. \n
+		frame control settings'. \n
 			:param sync: OFF | ON
 		"""
 		param = Conversions.bool_to_str(sync)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:SYNC {param}')
 
 	def get_ssid(self) -> str:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SSID \n
@@ -297,51 +301,21 @@
 			:return: ssid: string String with up to 32 characters (7-bit ASCII only)
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SSID?')
 		return trim_str_response(response)
 
 	def set_ssid(self, ssid: str) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SSID \n
-		Snippet: driver.configure.connection.set_ssid(ssid = '1') \n
+		Snippet: driver.configure.connection.set_ssid(ssid = 'abc') \n
 		Sets the service set identifier (SSID) . \n
 			:param ssid: string String with up to 32 characters (7-bit ASCII only)
 		"""
 		param = Conversions.value_to_quoted_str(ssid)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:SSID {param}')
 
-	# noinspection PyTypeChecker
-	class AidStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Start: int: numeric Range: 1 to 2007
-			- Stop: int: numeric Range: 1 to 2007"""
-		__meta_args_list = [
-			ArgStruct.scalar_int('Start'),
-			ArgStruct.scalar_int('Stop')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Start: int = None
-			self.Stop: int = None
-
-	def get_aid(self) -> AidStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:AID \n
-		Snippet: value: AidStruct = driver.configure.connection.get_aid() \n
-		Specifies the range of IDs to be assigned by the access point to the connected DUTs. \n
-			:return: structure: for return value, see the help for AidStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:AID?', self.__class__.AidStruct())
-
-	def set_aid(self, value: AidStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:AID \n
-		Snippet: driver.configure.connection.set_aid(value = AidStruct()) \n
-		Specifies the range of IDs to be assigned by the access point to the connected DUTs. \n
-			:param value: see the help for AidStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:AID', value)
-
 	def get_bss_color(self) -> int:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BSSColor \n
 		Snippet: value: int = driver.configure.connection.get_bss_color() \n
 		Specifies the color code of basic service set (BSS) . \n
 			:return: value: numeric Range: 1 to 63
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:CONNection:BSSColor?')
@@ -363,15 +337,15 @@
 			:return: bssid: hex Hexadecimal number with 12 digits Leading zeros can be omitted. Range: #H0 to #HFFFFFFFFFFFF
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:CONNection:BSSid?')
 		return trim_str_response(response)
 
 	def set_bssid(self, bssid: str) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BSSid \n
-		Snippet: driver.configure.connection.set_bssid(bssid = r1) \n
+		Snippet: driver.configure.connection.set_bssid(bssid = rawAbc) \n
 		Sets the 48-bit MAC address of the WLAN interface. \n
 			:param bssid: hex Hexadecimal number with 12 digits Leading zeros can be omitted. Range: #H0 to #HFFFFFFFFFFFF
 		"""
 		param = Conversions.value_to_str(bssid)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:BSSid {param}')
 
 	def get_beacon(self) -> int:
@@ -425,45 +399,14 @@
 		Snippet: driver.configure.connection.set_standard(typ = enums.StandardType.ACSTd) \n
 		Selects the IEEE 802.11 WLAN standard to be used. \n
 			:param typ: ASTD | GOSTd | ANSTd | GONStd | BSTD | GSTD | GNSTd | ACSTd | AXSTd BSTD: 802.11b ASTD: 802.11a GSTD: 802.11g GOSTd: 802.11g (OFDM) ANSTd: 802.11a/n GNSTd: 802.11g/n GONStd: 802.11g (OFDM) /n ACSTd: 802.11ac AXSTd: 802.11ax
 		"""
 		param = Conversions.enum_scalar_to_str(typ, enums.StandardType)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STANdard {param}')
 
-	# noinspection PyTypeChecker
-	class DyFragmentStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Level: enums.Level: No parameter help available
-			- Enable_Tx: enums.EnableState: No parameter help available"""
-		__meta_args_list = [
-			ArgStruct.scalar_enum('Level', enums.Level),
-			ArgStruct.scalar_enum('Enable_Tx', enums.EnableState)]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Level: enums.Level = None
-			self.Enable_Tx: enums.EnableState = None
-
-	# noinspection PyTypeChecker
-	def get_dy_fragment(self) -> DyFragmentStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:DYFRagment \n
-		Snippet: value: DyFragmentStruct = driver.configure.connection.get_dy_fragment() \n
-		No command help available \n
-			:return: structure: for return value, see the help for DyFragmentStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:DYFRagment?', self.__class__.DyFragmentStruct())
-
-	def set_dy_fragment(self, value: DyFragmentStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:DYFRagment \n
-		Snippet: driver.configure.connection.set_dy_fragment(value = DyFragmentStruct()) \n
-		No command help available \n
-			:param value: see the help for DyFragmentStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:DYFRagment', value)
-
 	def get_dsss(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:DSSS \n
 		Snippet: value: bool = driver.configure.connection.get_dsss() \n
 		Enables you to associate an 802.11b device using 802.11ac or ax standard. Also, it enables you to use non-HT management
 		frames within 802.11ac and ax. \n
 			:return: support_of_dsss: OFF | ON
 		"""
@@ -476,14 +419,14 @@
 		Enables you to associate an 802.11b device using 802.11ac or ax standard. Also, it enables you to use non-HT management
 		frames within 802.11ac and ax. \n
 			:param support_of_dsss: OFF | ON
 		"""
 		param = Conversions.bool_to_str(support_of_dsss)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:DSSS {param}')
 
-	def clone(self) -> 'Connection':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'ConnectionCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Connection(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = ConnectionCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Association/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,36 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Association:
-	"""Association commands group definition. 4 total commands, 1 Sub-groups, 3 group commands"""
+class AssociationCls:
+	"""Association commands group definition. 4 total commands, 2 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("association", core, parent)
+		self._cmd_group = CommandsGroup("association", core, parent)
 
 	@property
 	def sta(self):
 		"""sta commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_sta'):
-			from .Association_.Sta import Sta
-			self._sta = Sta(self._core, self._base)
+			from .Sta import StaCls
+			self._sta = StaCls(self._core, self._cmd_group)
 		return self._sta
 
-	# noinspection PyTypeChecker
-	class DisassStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Enable: bool: OFF | ON
-			- Timeout: int: numeric Range: 1 s to 3600 s"""
-		__meta_args_list = [
-			ArgStruct.scalar_bool('Enable'),
-			ArgStruct.scalar_int('Timeout')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Enable: bool = None
-			self.Timeout: int = None
-
-	def get_disass(self) -> DisassStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:ASSociation:DISass \n
-		Snippet: value: DisassStruct = driver.configure.connection.association.get_disass() \n
-		Enables or disables automatic STA disassociation, when a STA is no longer present. If enabled, the R&S CMW detects that a
-		STA is absent, it automatically removes its association after some user-specified period of time. \n
-			:return: structure: for return value, see the help for DisassStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:ASSociation:DISass?', self.__class__.DisassStruct())
-
-	def set_disass(self, value: DisassStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:ASSociation:DISass \n
-		Snippet: driver.configure.connection.association.set_disass(value = DisassStruct()) \n
-		Enables or disables automatic STA disassociation, when a STA is no longer present. If enabled, the R&S CMW detects that a
-		STA is absent, it automatically removes its association after some user-specified period of time. \n
-			:param value: see the help for DisassStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:ASSociation:DISass', value)
+	@property
+	def disass(self):
+		"""disass commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_disass'):
+			from .Disass import DisassCls
+			self._disass = DisassCls(self._core, self._cmd_group)
+		return self._disass
 
 	def get_preemption(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:ASSociation:PREemption \n
 		Snippet: value: bool = driver.configure.connection.association.get_preemption() \n
 		If enabled, then the existing association possible with any MAC addresses is replaced by a new incoming one. \n
 			:return: enable: OFF | ON
 		"""
@@ -87,14 +61,14 @@
 		Snippet: driver.configure.connection.association.set_sta_priority(mode = enums.PrioModeB.AUTO) \n
 		Specifies how the stack prioritizes one STA over another in multi-STA connections. \n
 			:param mode: AUTO | ROURobin Automatic or round robin
 		"""
 		param = Conversions.enum_scalar_to_str(mode, enums.PrioModeB)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:ASSociation:STAPriority {param}')
 
-	def clone(self) -> 'Association':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'AssociationCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Association(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = AssociationCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.RepeatedCapability import RepeatedCapability
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sta:
-	"""Sta commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
+class StaticCls:
+	"""Static commands group definition. 7 total commands, 2 Subgroups, 0 group commands
 	Repeated Capability: Station, default value after init: Station.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sta", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
+		self._cmd_group = CommandsGroup("static", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
 
-	def repcap_station_set(self, enum_value: repcap.Station) -> None:
+	def repcap_station_set(self, station: repcap.Station) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Station.Default
 		Default value after init: Station.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(station)
 
 	def repcap_station_get(self) -> repcap.Station:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
-	def macReserve(self):
-		"""macReserve commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_macReserve'):
-			from .Sta_.MacReserve import MacReserve
-			self._macReserve = MacReserve(self._core, self._base)
-		return self._macReserve
+	def smask(self):
+		"""smask commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_smask'):
+			from .Smask import SmaskCls
+			self._smask = SmaskCls(self._core, self._cmd_group)
+		return self._smask
 
-	def clone(self) -> 'Sta':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def ipAddress(self):
+		"""ipAddress commands group. 6 Sub-classes, 0 commands."""
+		if not hasattr(self, '_ipAddress'):
+			from .IpAddress import IpAddressCls
+			self._ipAddress = IpAddressCls(self._core, self._cmd_group)
+		return self._ipAddress
+
+	def clone(self) -> 'StaticCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Sta(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = StaticCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta_/MacReserve.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/HetbInfo/UphInfo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,40 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.StructBase import StructBase
-from ......Internal.ArgStruct import ArgStruct
-from ...... import enums
-from ...... import repcap
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.StructBase import StructBase
+from .....Internal.ArgStruct import ArgStruct
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MacReserve:
-	"""MacReserve commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class UphInfoCls:
+	"""UphInfo commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("macReserve", core, parent)
+		self._cmd_group = CommandsGroup("uphInfo", core, parent)
 
 	# noinspection PyTypeChecker
-	class MacReserveStruct(StructBase):
-		"""Structure for setting input parameters. Contains optional setting parameters. Fields: \n
-			- Reservation: enums.Reservation: ANY | SET | OFF ANY - the slot is available to a STA of any MAC address SET - reserves the slot for a particular MAC address OFF - the slot is disabled
-			- Address: str: Optional setting parameter. string MAC address of the DUT for Reservation = SET"""
+	class GetStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Burst_Power: float: float Indication of HE TB burst power. Range: -999 dBm to 999 dBm
+			- Uph: int: decimal Indication of UL power headroom. Range: 0 dB to 31 dB
+			- Min_Tx_Power_Flag: bool: OFF | ON Indication whether the HE TB bursts are sent at the minimum transmit power of the station."""
 		__meta_args_list = [
-			ArgStruct.scalar_enum('Reservation', enums.Reservation),
-			ArgStruct.scalar_str('Address')]
+			ArgStruct.scalar_float('Burst_Power'),
+			ArgStruct.scalar_int('Uph'),
+			ArgStruct.scalar_bool('Min_Tx_Power_Flag')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Reservation: enums.Reservation = None
-			self.Address: str = None
-
-	def set(self, structure: MacReserveStruct, station=repcap.Station.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:ASSociation:STA<s>:MACReserve \n
-		Snippet: driver.configure.connection.association.sta.macReserve.set(value = [PROPERTY_STRUCT_NAME](), station = repcap.Station.Default) \n
-		Configures three slots available for STAs, if method RsCmwWlanSig.Configure.Connection.mstation is set to ON \n
-			:param structure: for set value, see the help for MacReserveStruct structure arguments.
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:ASSociation:STA{station_cmd_val}:MACReserve', structure)
-
-	def get(self, station=repcap.Station.Default) -> MacReserveStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:ASSociation:STA<s>:MACReserve \n
-		Snippet: value: MacReserveStruct = driver.configure.connection.association.sta.macReserve.get(station = repcap.Station.Default) \n
-		Configures three slots available for STAs, if method RsCmwWlanSig.Configure.Connection.mstation is set to ON \n
+			self.Burst_Power: float = None
+			self.Uph: int = None
+			self.Min_Tx_Power_Flag: bool = None
+
+	def get(self, station=repcap.Station.Default) -> GetStruct:
+		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:HETBinfo:UPHinfo \n
+		Snippet: value: GetStruct = driver.sense.sta.hetbInfo.uphInfo.get(station = repcap.Station.Default) \n
+		Queries actual information related to uplink power headroom (UPH) control. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:return: structure: for return value, see the help for MacReserveStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:ASSociation:STA{station_cmd_val}:MACReserve?', self.__class__.MacReserveStruct())
+			:return: structure: for return value, see the help for GetStruct structure arguments."""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:HETBinfo:UPHinfo?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Btwt:
-	"""Btwt commands group definition. 6 total commands, 1 Sub-groups, 1 group commands"""
+class BtwtCls:
+	"""Btwt commands group definition. 6 total commands, 1 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("btwt", core, parent)
+		self._cmd_group = CommandsGroup("btwt", core, parent)
 
 	@property
 	def schedule(self):
 		"""schedule commands group. 5 Sub-classes, 0 commands."""
 		if not hasattr(self, '_schedule'):
-			from .Btwt_.Schedule import Schedule
-			self._schedule = Schedule(self._core, self._base)
+			from .Schedule import ScheduleCls
+			self._schedule = ScheduleCls(self._core, self._cmd_group)
 		return self._schedule
 
 	def get_enable(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BTWT:ENABle \n
 		Snippet: value: bool = driver.configure.connection.btwt.get_enable() \n
 		Enables/ disables broadcast target wake time (TWT) operation. \n
 			:return: enable: OFF | ON
@@ -33,14 +33,14 @@
 		Snippet: driver.configure.connection.btwt.set_enable(enable = False) \n
 		Enables/ disables broadcast target wake time (TWT) operation. \n
 			:param enable: OFF | ON
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:BTWT:ENABle {param}')
 
-	def clone(self) -> 'Btwt':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'BtwtCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Btwt(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = BtwtCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,43 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Schedule:
-	"""Schedule commands group definition. 5 total commands, 5 Sub-groups, 0 group commands"""
+class EsimCls:
+	"""Esim commands group definition. 3 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("schedule", core, parent)
+		self._cmd_group = CommandsGroup("esim", core, parent)
 
 	@property
-	def enable(self):
-		"""enable commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_enable'):
-			from .Schedule_.Enable import Enable
-			self._enable = Enable(self._core, self._base)
-		return self._enable
+	def ktThree(self):
+		"""ktThree commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ktThree'):
+			from .KtThree import KtThreeCls
+			self._ktThree = KtThreeCls(self._core, self._cmd_group)
+		return self._ktThree
 
 	@property
-	def ftype(self):
-		"""ftype commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_ftype'):
-			from .Schedule_.Ftype import Ftype
-			self._ftype = Ftype(self._core, self._base)
-		return self._ftype
+	def ktTwo(self):
+		"""ktTwo commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ktTwo'):
+			from .KtTwo import KtTwoCls
+			self._ktTwo = KtTwoCls(self._core, self._cmd_group)
+		return self._ktTwo
 
 	@property
-	def stime(self):
-		"""stime commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_stime'):
-			from .Schedule_.Stime import Stime
-			self._stime = Stime(self._core, self._base)
-		return self._stime
+	def ktone(self):
+		"""ktone commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ktone'):
+			from .Ktone import KtoneCls
+			self._ktone = KtoneCls(self._core, self._cmd_group)
+		return self._ktone
 
-	@property
-	def mwDuration(self):
-		"""mwDuration commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_mwDuration'):
-			from .Schedule_.MwDuration import MwDuration
-			self._mwDuration = MwDuration(self._core, self._base)
-		return self._mwDuration
-
-	@property
-	def tenable(self):
-		"""tenable commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_tenable'):
-			from .Schedule_.Tenable import Tenable
-			self._tenable = Tenable(self._core, self._base)
-		return self._tenable
-
-	def clone(self) -> 'Schedule':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'EsimCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Schedule(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = EsimCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Enable.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Enable.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from ......Internal import Conversions
 from ......Internal.Types import DataType
 from ......Internal.ArgSingleList import ArgSingleList
 from ......Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Enable:
-	"""Enable commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class EnableCls:
+	"""Enable commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("enable", core, parent)
+		self._cmd_group = CommandsGroup("enable", core, parent)
 
 	def set(self, flow_id: int, enable: bool) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BTWT:SCHedule:ENABle \n
 		Snippet: driver.configure.connection.btwt.schedule.enable.set(flow_id = 1, enable = False) \n
 		Enables/ disables particular schedule period. \n
 			:param flow_id: integer
 			:param enable: OFF | ON
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Ftype.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Ftype.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from ......Internal.Types import DataType
 from ......Internal.ArgSingleList import ArgSingleList
 from ......Internal.ArgSingle import ArgSingle
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Ftype:
-	"""Ftype commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class FtypeCls:
+	"""Ftype commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ftype", core, parent)
+		self._cmd_group = CommandsGroup("ftype", core, parent)
 
 	def set(self, flow_id: int, flow_type: enums.FlowType) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BTWT:SCHedule:FTYPe \n
 		Snippet: driver.configure.connection.btwt.schedule.ftype.set(flow_id = 1, flow_type = enums.FlowType.ANNounced) \n
 		Specifies the broadcast TWT flow type for the specified schedule period. \n
 			:param flow_id: integer
 			:param flow_type: ANNounced | UNANnounced
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('flow_id', flow_id, DataType.Integer), ArgSingle('flow_type', flow_type, DataType.Enum))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('flow_id', flow_id, DataType.Integer), ArgSingle('flow_type', flow_type, DataType.Enum, enums.FlowType))
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:BTWT:SCHedule:FTYPe {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	def get(self, flow_id: int) -> enums.FlowType:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BTWT:SCHedule:FTYPe \n
 		Snippet: value: enums.FlowType = driver.configure.connection.btwt.schedule.ftype.get(flow_id = 1) \n
 		Specifies the broadcast TWT flow type for the specified schedule period. \n
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/MwDuration.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/MwDuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from ......Internal import Conversions
 from ......Internal.Types import DataType
 from ......Internal.ArgSingleList import ArgSingleList
 from ......Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MwDuration:
-	"""MwDuration commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class MwDurationCls:
+	"""MwDuration commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mwDuration", core, parent)
+		self._cmd_group = CommandsGroup("mwDuration", core, parent)
 
 	def set(self, flow_id: int, min_wake_duration: float) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BTWT:SCHedule:MWDuration \n
 		Snippet: driver.configure.connection.btwt.schedule.mwDuration.set(flow_id = 1, min_wake_duration = 1.0) \n
 		Specifies the minimum wake duration for the specified scheduled period. \n
 			:param flow_id: integer
 			:param min_wake_duration: numeric Range: 0 ms to 100 ms
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Stime.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Stime.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from ......Internal import Conversions
 from ......Internal.Types import DataType
 from ......Internal.ArgSingleList import ArgSingleList
 from ......Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Stime:
-	"""Stime commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class StimeCls:
+	"""Stime commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("stime", core, parent)
+		self._cmd_group = CommandsGroup("stime", core, parent)
 
 	def set(self, flow_id: int, start_time: float) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BTWT:SCHedule:STIMe \n
 		Snippet: driver.configure.connection.btwt.schedule.stime.set(flow_id = 1, start_time = 1.0) \n
 		Specifies the offset of the specified schedule period from beacon. \n
 			:param flow_id: integer
 			:param start_time: numeric Range: 0 ms to 100 ms
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Tenable.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Tenable.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from ......Internal import Conversions
 from ......Internal.Types import DataType
 from ......Internal.ArgSingleList import ArgSingleList
 from ......Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Tenable:
-	"""Tenable commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class TenableCls:
+	"""Tenable commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("tenable", core, parent)
+		self._cmd_group = CommandsGroup("tenable", core, parent)
 
 	def set(self, flow_id: int, enable: bool) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:BTWT:SCHedule:TENable \n
 		Snippet: driver.configure.connection.btwt.schedule.tenable.set(flow_id = 1, enable = False) \n
 		Enables/disables the broadcast TWT trigger for the specified schedule period. \n
 			:param flow_id: integer
 			:param enable: OFF | ON
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hemac.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hemac.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hemac:
-	"""Hemac commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class HemacCls:
+	"""Hemac commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hemac", core, parent)
+		self._cmd_group = CommandsGroup("hemac", core, parent)
 
 	def get_bsr_support(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HEMac:BSRSupport \n
 		Snippet: value: bool = driver.configure.connection.hemac.get_bsr_support() \n
 		Indicates, whether the R&S CMW supports the buffer status report (BSR) . \n
 			:return: supported: OFF | ON
 		"""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hetf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.StructBase import StructBase
+from .....Internal.ArgStruct import ArgStruct
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hetf:
-	"""Hetf commands group definition. 11 total commands, 1 Sub-groups, 10 group commands"""
+class HetfCls:
+	"""Hetf commands group definition. 11 total commands, 1 Subgroups, 10 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hetf", core, parent)
+		self._cmd_group = CommandsGroup("hetf", core, parent)
 
 	@property
 	def ssTx(self):
 		"""ssTx commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ssTx'):
-			from .Hetf_.SsTx import SsTx
-			self._ssTx = SsTx(self._core, self._base)
+			from .SsTx import SsTxCls
+			self._ssTx = SsTxCls(self._core, self._cmd_group)
 		return self._ssTx
 
 	def get_txp(self) -> int:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HETF:TXP \n
 		Snippet: value: int = driver.configure.connection.hetf.get_txp() \n
 		Sets the interval for periodical trigger frame. \n
 			:return: interval: integer Range: 1 to 10E+3, Unit: ms
@@ -73,15 +73,15 @@
 		Specifies the support of LDPC extra symbol segment. \n
 			:param extra_symbol: OFF | ON
 		"""
 		param = Conversions.bool_to_str(extra_symbol)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HETF:LDPC {param}')
 
 	# noinspection PyTypeChecker
-	class ApTxPowerStruct(StructBase):
+	class ApTxPowerStruct(StructBase):  # From ReadStructDefinition CmdPropertyTemplate.xml
 		"""Structure for reading output parameters. Fields: \n
 			- Int_Value: int: decimal Range: 0 to 60
 			- Dbm_Value: int: decimal Range: -20 dBm to 40 dBm, Unit: dBm"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Int_Value'),
 			ArgStruct.scalar_int('Dbm_Value')]
 
@@ -208,14 +208,14 @@
 		Snippet: driver.configure.connection.hetf.set_ttyp(type_py = enums.TriggerType.BQRP) \n
 		Specifies the trigger type as specified in the Common Info field. \n
 			:param type_py: BTR | BRP | MRTS | BSRP | BQRP BTR: Basic Trigger BRP: Beamforming Report Poll MRTS: MU-RTS BSRP: Buffer Status Report Poll BQRP: Bandwidth Query Report Poll
 		"""
 		param = Conversions.enum_scalar_to_str(type_py, enums.TriggerType)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HETF:TTYP {param}')
 
-	def clone(self) -> 'Hetf':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'HetfCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Hetf(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = HetfCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf_/SsTx.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Twt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SsTx:
-	"""SsTx commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class TwtCls:
+	"""Twt commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ssTx", core, parent)
+		self._cmd_group = CommandsGroup("twt", core, parent)
 
-	def set(self) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HETF:SSTX \n
-		Snippet: driver.configure.connection.hetf.ssTx.set() \n
-		Transmits the trigger frame once. \n
+	def get_required(self) -> bool:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:TWT:REQuired \n
+		Snippet: value: bool = driver.configure.connection.twt.get_required() \n
+		No command help available \n
+			:return: enable: No help available
 		"""
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HETF:SSTX')
+		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:CONNection:TWT:REQuired?')
+		return Conversions.str_to_bool(response)
 
-	def set_with_opc(self) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HETF:SSTX \n
-		Snippet: driver.configure.connection.hetf.ssTx.set_with_opc() \n
-		Transmits the trigger frame once. \n
-		Same as set, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
+	def set_required(self, enable: bool) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:TWT:REQuired \n
+		Snippet: driver.configure.connection.twt.set_required(enable = False) \n
+		No command help available \n
+			:param enable: No help available
 		"""
-		self._core.io.write_with_opc(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HETF:SSTX')
+		param = Conversions.bool_to_str(enable)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:TWT:REQuired {param}')
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,64 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.StructBase import StructBase
+from .....Internal.ArgStruct import ArgStruct
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hotspot:
-	"""Hotspot commands group definition. 7 total commands, 3 Sub-groups, 4 group commands"""
+class HotspotCls:
+	"""Hotspot commands group definition. 7 total commands, 4 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hotspot", core, parent)
+		self._cmd_group = CommandsGroup("hotspot", core, parent)
+
+	@property
+	def cutil(self):
+		"""cutil commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_cutil'):
+			from .Cutil import CutilCls
+			self._cutil = CutilCls(self._core, self._cmd_group)
+		return self._cutil
 
 	@property
 	def realm(self):
 		"""realm commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_realm'):
-			from .Hotspot_.Realm import Realm
-			self._realm = Realm(self._core, self._base)
+			from .Realm import RealmCls
+			self._realm = RealmCls(self._core, self._cmd_group)
 		return self._realm
 
 	@property
 	def dname(self):
 		"""dname commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_dname'):
-			from .Hotspot_.Dname import Dname
-			self._dname = Dname(self._core, self._base)
+			from .Dname import DnameCls
+			self._dname = DnameCls(self._core, self._cmd_group)
 		return self._dname
 
 	@property
 	def plmn(self):
 		"""plmn commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_plmn'):
-			from .Hotspot_.Plmn import Plmn
-			self._plmn = Plmn(self._core, self._base)
+			from .Plmn import PlmnCls
+			self._plmn = PlmnCls(self._core, self._cmd_group)
 		return self._plmn
 
 	# noinspection PyTypeChecker
-	class CutilStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Station_Count: int: numeric Number of stations that are currently associated with the BSS Range: 0 to 65535
-			- Channel_Utilization: int: numeric Percentage of time, that the access point sensed the primary channel was busy Range: 0 % to 100 %, Unit: %
-			- Available_Admission_Capacity: int: numeric Remaining time available via explicit admission control, in units of 32 μs/s Range: 0 to 31250"""
-		__meta_args_list = [
-			ArgStruct.scalar_int('Station_Count'),
-			ArgStruct.scalar_int('Channel_Utilization'),
-			ArgStruct.scalar_int('Available_Admission_Capacity')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Station_Count: int = None
-			self.Channel_Utilization: int = None
-			self.Available_Admission_Capacity: int = None
-
-	def get_cutil(self) -> CutilStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:CUTil \n
-		Snippet: value: CutilStruct = driver.configure.connection.hotspot.get_cutil() \n
-		Configures the contents of the BSS load element. \n
-			:return: structure: for return value, see the help for CutilStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:CUTil?', self.__class__.CutilStruct())
-
-	def set_cutil(self, value: CutilStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:CUTil \n
-		Snippet: driver.configure.connection.hotspot.set_cutil(value = CutilStruct()) \n
-		Configures the contents of the BSS load element. \n
-			:param value: see the help for CutilStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:CUTil', value)
-
-	# noinspection PyTypeChecker
-	class HssparStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+	class HssparStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
+		"""Structure for setting input parameters. Fields: \n
 			- Downlink_Speed: int: numeric Range: 0 kbit/s to 300000 kbit/s, Unit: kbit/s
 			- Uplink_Speed: int: numeric Range: 0 kbit/s to 300000 kbit/s, Unit: kbit/s
 			- Ip_V_6_Add_Field: enums.IpV6AddField: ATNavailable | ATAVailable | AATNknown Indicates whether an IPv6 address can be allocated to the station ATNavailable: address type not available ATAVailable: address type available AATNknown: availability of the address type is not known
 			- Ip_V_4_Add_Field: enums.IpV6AddFieldExt: ATNavailable | PIAavailable | PRIaavailabl | SNPiaavailab | DNPiaavailab | PSNiaavailab | PDNiaavailab | AATNknown Indicates whether an IPv4 address can be allocated to the station ATNavailable: address type not available PIAavailable: public IPv4 address available PRIaavailabl: port-restricted IPv4 address available SNPiaavailab: single-NATed private IPv4 address available DNPiaavailab: double-NATed private IPv4 address available PSNiaavailab: port-restricted and single-NATed IPv4 address available PDNiaavailab: port-restricted and double-NATed IPv4 address available AATNknown: availability of the address type not known
-			- Realm_Name: str: string Name of reachable NAI realm as string To configure more than one realm, use [CMDLINK: CONFigure:WLAN:SIGNi:CONNection:HOTSpot:REALmno CMDLINK].
-			- Eap_Type: enums.EapType: SIM | TTLS | AKA | APRime | TLS Supported extensible authorization protocol type EAP-SIM, EAP-TTLS, EAP-AKA, EAP-AKA' or EAP-TLS To enable multiple EAP types, use [CMDLINK: CONFigure:WLAN:SIGNi:CONNection:HOTSpot:REALmno CMDLINK].
+			- Realm_Name: str: string Name of reachable NAI realm as string To configure more than one realm, use [CMDLINKRESOLVED Configure.Connection.Hotspot.Realm#set CMDLINKRESOLVED].
+			- Eap_Type: enums.EapType: SIM | TTLS | AKA | APRime | TLS Supported extensible authorization protocol type EAP-SIM, EAP-TTLS, EAP-AKA, EAP-AKA' or EAP-TLS To enable multiple EAP types, use [CMDLINKRESOLVED Configure.Connection.Hotspot.Realm#set CMDLINKRESOLVED].
 			- Internet_Access: bool: OFF | ON Specifies whether the hotspot provides internet access
 			- Net_Auth_Type_Ind: enums.NetAuthTypeInd: ATConditions | OESupported | HREDirection | DREDirection Network authentication type ATConditions: acceptance of terms and conditions OESupported: on-line enrollment supported HREDirection: http/https redirection DREDirection: DNS redirection"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Downlink_Speed'),
 			ArgStruct.scalar_int('Uplink_Speed'),
 			ArgStruct.scalar_enum('Ip_V_6_Add_Field', enums.IpV6AddField),
 			ArgStruct.scalar_enum('Ip_V_4_Add_Field', enums.IpV6AddFieldExt),
@@ -109,15 +84,25 @@
 		Defines supplementary parameters of the Hotspot 2.0 operation mode. \n
 			:return: structure: for return value, see the help for HssparStruct structure arguments.
 		"""
 		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:HSSPar?', self.__class__.HssparStruct())
 
 	def set_hsspar(self, value: HssparStruct) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:HSSPar \n
-		Snippet: driver.configure.connection.hotspot.set_hsspar(value = HssparStruct()) \n
+		Snippet with structure: \n
+		structure = driver.configure.connection.hotspot.HssparStruct() \n
+		structure.Downlink_Speed: int = 1 \n
+		structure.Uplink_Speed: int = 1 \n
+		structure.Ip_V_6_Add_Field: enums.IpV6AddField = enums.IpV6AddField.AATNknown \n
+		structure.Ip_V_4_Add_Field: enums.IpV6AddFieldExt = enums.IpV6AddFieldExt.AATNknown \n
+		structure.Realm_Name: str = 'abc' \n
+		structure.Eap_Type: enums.EapType = enums.EapType.AKA \n
+		structure.Internet_Access: bool = False \n
+		structure.Net_Auth_Type_Ind: enums.NetAuthTypeInd = enums.NetAuthTypeInd.ATConditions \n
+		driver.configure.connection.hotspot.set_hsspar(value = structure) \n
 		Defines supplementary parameters of the Hotspot 2.0 operation mode. \n
 			:param value: see the help for HssparStruct structure arguments.
 		"""
 		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:HSSPar', value)
 
 	# noinspection PyTypeChecker
 	def get_mn_digits(self) -> enums.NumOfDigits:
@@ -135,24 +120,24 @@
 		Defines the length of the MNC of the first PLMN in Hotspot 2.0 operation mode. \n
 			:param num_of_digits: TWDigits | THDigits TWDigits: two digits THDigits: three digits
 		"""
 		param = Conversions.enum_scalar_to_str(num_of_digits, enums.NumOfDigits)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:MNDigits {param}')
 
 	# noinspection PyTypeChecker
-	class HsparStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+	class HsparStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
+		"""Structure for setting input parameters. Fields: \n
 			- Access_Net_Type: enums.AccessNetType: PNETwork | PNWGaccess | CPNetwork | FPNetwork | PDNetwork | ESONetwork | TOEXperiment | WILDcard PNETwork: private network PNWGaccess: private network with guest access CPNetwork: chargeable public network FPNetwork: free public network PDNetwork: personal device network ESONetwork: emergency services only network TOEXperiment: test or experimental WILDcard: wildcard
 			- Venue_Group: float: numeric | UNSPecified | ASSembly | BUSiness | EDUCational | FAINdustrial | INSTitutional | MERCantile | RESidential | STORage | UAMisc | VEHicular | OUTDoor FAINdustrial: factory and industrial UAMisc: utility and miscellaneous
 			- Venue_Type: float: numeric Range: 0 to 255
 			- He_Ssid: float: numeric Homogeneous extended service set identifier Range: #H0 to #HFFFFFFFFFFFF
 			- Venue_Name: str: string String with up to 252 ASCII characters
-			- Mcc: int: numeric Mobile country code of 3GPP network reachable via the hotspot To configure more than one PLMN, use [CMDLINK: CONFigure:WLAN:SIGNi:CONNection:HOTSpot:PLMNno CMDLINK]. Range: 1 to 999
-			- Mnc: int: numeric Mobile network code of 3GPP network reachable via the hotspot To configure more than one PLMN, use [CMDLINK: CONFigure:WLAN:SIGNi:CONNection:HOTSpot:PLMNno CMDLINK]. Range: 1 to 9991)
-			- Domain_Name: str: string Domain name of the network operator as string To configure more than one domain name, use [CMDLINK: CONFigure:WLAN:SIGNi:CONNection:HOTSpot:DNAMeno CMDLINK].
+			- Mcc: int: numeric Mobile country code of 3GPP network reachable via the hotspot To configure more than one PLMN, use [CMDLINKRESOLVED Configure.Connection.Hotspot.Plmn#set CMDLINKRESOLVED]. Range: 1 to 999
+			- Mnc: int: numeric Mobile network code of 3GPP network reachable via the hotspot To configure more than one PLMN, use [CMDLINKRESOLVED Configure.Connection.Hotspot.Plmn#set CMDLINKRESOLVED]. Range: 1 to 9991)
+			- Domain_Name: str: string Domain name of the network operator as string To configure more than one domain name, use [CMDLINKRESOLVED Configure.Connection.Hotspot.Dname#set CMDLINKRESOLVED].
 			- Op_Frie_Name: str: string Friendly name of the network operator as string"""
 		__meta_args_list = [
 			ArgStruct.scalar_enum('Access_Net_Type', enums.AccessNetType),
 			ArgStruct.scalar_float('Venue_Group'),
 			ArgStruct.scalar_float('Venue_Type'),
 			ArgStruct.scalar_float('He_Ssid'),
 			ArgStruct.scalar_str('Venue_Name'),
@@ -169,31 +154,41 @@
 			self.He_Ssid: float = None
 			self.Venue_Name: str = None
 			self.Mcc: int = None
 			self.Mnc: int = None
 			self.Domain_Name: str = None
 			self.Op_Frie_Name: str = None
 
-	# noinspection PyTypeChecker
 	def get_hspar(self) -> HsparStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:HSPar \n
 		Snippet: value: HsparStruct = driver.configure.connection.hotspot.get_hspar() \n
 		Defines basic parameters of the Hotspot 2.0 operation mode. \n
 			:return: structure: for return value, see the help for HsparStruct structure arguments.
 		"""
 		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:HSPar?', self.__class__.HsparStruct())
 
 	def set_hspar(self, value: HsparStruct) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:HSPar \n
-		Snippet: driver.configure.connection.hotspot.set_hspar(value = HsparStruct()) \n
+		Snippet with structure: \n
+		structure = driver.configure.connection.hotspot.HsparStruct() \n
+		structure.Access_Net_Type: enums.AccessNetType = enums.AccessNetType.CPNetwork \n
+		structure.Venue_Group: float = 1.0 \n
+		structure.Venue_Type: float = 1.0 \n
+		structure.He_Ssid: float = 1.0 \n
+		structure.Venue_Name: str = 'abc' \n
+		structure.Mcc: int = 1 \n
+		structure.Mnc: int = 1 \n
+		structure.Domain_Name: str = 'abc' \n
+		structure.Op_Frie_Name: str = 'abc' \n
+		driver.configure.connection.hotspot.set_hspar(value = structure) \n
 		Defines basic parameters of the Hotspot 2.0 operation mode. \n
 			:param value: see the help for HsparStruct structure arguments.
 		"""
 		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:HSPar', value)
 
-	def clone(self) -> 'Hotspot':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'HotspotCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Hotspot(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = HotspotCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Dname.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Dname.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,76 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Types import DataType
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
 from .....Internal.RepeatedCapability import RepeatedCapability
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dname:
-	"""Dname commands group definition. 1 total commands, 0 Sub-groups, 1 group commands
+class DnameCls:
+	"""Dname commands group definition. 1 total commands, 0 Subgroups, 1 group commands
 	Repeated Capability: DomainName, default value after init: DomainName.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dname", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_domainName_get', 'repcap_domainName_set', repcap.DomainName.Nr1)
+		self._cmd_group = CommandsGroup("dname", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_domainName_get', 'repcap_domainName_set', repcap.DomainName.Nr1)
 
-	def repcap_domainName_set(self, enum_value: repcap.DomainName) -> None:
+	def repcap_domainName_set(self, domainName: repcap.DomainName) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to DomainName.Default
 		Default value after init: DomainName.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(domainName)
 
 	def repcap_domainName_get(self) -> repcap.DomainName:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
+
+	def set(self, state: bool, name: str, domainName=repcap.DomainName.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:DNAMe<nr> \n
+		Snippet: driver.configure.connection.hotspot.dname.set(state = False, name = 'abc', domainName = repcap.DomainName.Default) \n
+		Defines a list of domain names of the entity operating the IEEE 802.11 access network. The first domain name can also be
+		defined via method RsCmwWlanSig.Configure.Connection.Hotspot.hspar. \n
+			:param state: OFF | ON Disables/enables the list entry
+			:param name: string Domain name as string
+			:param domainName: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Dname')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('state', state, DataType.Boolean), ArgSingle('name', name, DataType.String))
+		domainName_cmd_val = self._cmd_group.get_repcap_cmd_value(domainName, repcap.DomainName)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:DNAMe{domainName_cmd_val} {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class DnameStruct(StructBase):
-		"""Structure for setting input parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- State: bool: OFF | ON Disables/enables the list entry
 			- Name: str: string Domain name as string"""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('State'),
 			ArgStruct.scalar_str('Name')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.State: bool = None
 			self.Name: str = None
 
-	def set(self, structure: DnameStruct, domainName=repcap.DomainName.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:DNAMe<nr> \n
-		Snippet: driver.configure.connection.hotspot.dname.set(value = [PROPERTY_STRUCT_NAME](), domainName = repcap.DomainName.Default) \n
-		Defines a list of domain names of the entity operating the IEEE 802.11 access network. The first domain name can also be
-		defined via method RsCmwWlanSig.Configure.Connection.Hotspot.hspar. \n
-			:param structure: for set value, see the help for DnameStruct structure arguments.
-			:param domainName: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Dname')"""
-		domainName_cmd_val = self._base.get_repcap_cmd_value(domainName, repcap.DomainName)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:DNAMe{domainName_cmd_val}', structure)
-
 	def get(self, domainName=repcap.DomainName.Default) -> DnameStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:DNAMe<nr> \n
 		Snippet: value: DnameStruct = driver.configure.connection.hotspot.dname.get(domainName = repcap.DomainName.Default) \n
 		Defines a list of domain names of the entity operating the IEEE 802.11 access network. The first domain name can also be
 		defined via method RsCmwWlanSig.Configure.Connection.Hotspot.hspar. \n
 			:param domainName: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Dname')
 			:return: structure: for return value, see the help for DnameStruct structure arguments."""
-		domainName_cmd_val = self._base.get_repcap_cmd_value(domainName, repcap.DomainName)
+		domainName_cmd_val = self._cmd_group.get_repcap_cmd_value(domainName, repcap.DomainName)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:DNAMe{domainName_cmd_val}?', self.__class__.DnameStruct())
 
-	def clone(self) -> 'Dname':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'DnameCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Dname(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = DnameCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Plmn.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Plmn.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,58 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Types import DataType
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
 from .....Internal.RepeatedCapability import RepeatedCapability
 from ..... import enums
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Plmn:
-	"""Plmn commands group definition. 1 total commands, 0 Sub-groups, 1 group commands
+class PlmnCls:
+	"""Plmn commands group definition. 1 total commands, 0 Subgroups, 1 group commands
 	Repeated Capability: Plnm, default value after init: Plnm.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("plmn", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_plnm_get', 'repcap_plnm_set', repcap.Plnm.Nr1)
+		self._cmd_group = CommandsGroup("plmn", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_plnm_get', 'repcap_plnm_set', repcap.Plnm.Nr1)
 
-	def repcap_plnm_set(self, enum_value: repcap.Plnm) -> None:
+	def repcap_plnm_set(self, plnm: repcap.Plnm) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Plnm.Default
 		Default value after init: Plnm.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(plnm)
 
 	def repcap_plnm_get(self) -> repcap.Plnm:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
+
+	def set(self, state: bool, mcc: int, mnc: int, num_of_digits: enums.NumOfDigits, plnm=repcap.Plnm.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:PLMN<nr> \n
+		Snippet: driver.configure.connection.hotspot.plmn.set(state = False, mcc = 1, mnc = 1, num_of_digits = enums.NumOfDigits.THDigits, plnm = repcap.Plnm.Default) \n
+		Defines a list of 3GPP networks that the hotspot provides service for. The MCC and MNC of the first PLMN can also be
+		defined via method RsCmwWlanSig.Configure.Connection.Hotspot.hspar. \n
+			:param state: OFF | ON Disables/enables the list entry
+			:param mcc: integer Mobile country code Range: 1 to 999
+			:param mnc: integer Mobile network code Range: Depends on NumOfDigits
+			:param num_of_digits: TWDigits | THDigits Length of the MNC TWDigits: two digits (1 to 99) THDigits: three digits (1 to 999)
+			:param plnm: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Plmn')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('state', state, DataType.Boolean), ArgSingle('mcc', mcc, DataType.Integer), ArgSingle('mnc', mnc, DataType.Integer), ArgSingle('num_of_digits', num_of_digits, DataType.Enum, enums.NumOfDigits))
+		plnm_cmd_val = self._cmd_group.get_repcap_cmd_value(plnm, repcap.Plnm)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:PLMN{plnm_cmd_val} {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class PlmnStruct(StructBase):
-		"""Structure for setting input parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- State: bool: OFF | ON Disables/enables the list entry
 			- Mcc: int: integer Mobile country code Range: 1 to 999
 			- Mnc: int: integer Mobile network code Range: Depends on NumOfDigits
 			- Num_Of_Digits: enums.NumOfDigits: TWDigits | THDigits Length of the MNC TWDigits: two digits (1 to 99) THDigits: three digits (1 to 999)"""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('State'),
 			ArgStruct.scalar_int('Mcc'),
@@ -44,34 +62,24 @@
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.State: bool = None
 			self.Mcc: int = None
 			self.Mnc: int = None
 			self.Num_Of_Digits: enums.NumOfDigits = None
 
-	def set(self, structure: PlmnStruct, plnm=repcap.Plnm.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:PLMN<nr> \n
-		Snippet: driver.configure.connection.hotspot.plmn.set(value = [PROPERTY_STRUCT_NAME](), plnm = repcap.Plnm.Default) \n
-		Defines a list of 3GPP networks that the hotspot provides service for. The MCC and MNC of the first PLMN can also be
-		defined via method RsCmwWlanSig.Configure.Connection.Hotspot.hspar. \n
-			:param structure: for set value, see the help for PlmnStruct structure arguments.
-			:param plnm: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Plmn')"""
-		plnm_cmd_val = self._base.get_repcap_cmd_value(plnm, repcap.Plnm)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:PLMN{plnm_cmd_val}', structure)
-
 	def get(self, plnm=repcap.Plnm.Default) -> PlmnStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:PLMN<nr> \n
 		Snippet: value: PlmnStruct = driver.configure.connection.hotspot.plmn.get(plnm = repcap.Plnm.Default) \n
 		Defines a list of 3GPP networks that the hotspot provides service for. The MCC and MNC of the first PLMN can also be
 		defined via method RsCmwWlanSig.Configure.Connection.Hotspot.hspar. \n
 			:param plnm: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Plmn')
 			:return: structure: for return value, see the help for PlmnStruct structure arguments."""
-		plnm_cmd_val = self._base.get_repcap_cmd_value(plnm, repcap.Plnm)
+		plnm_cmd_val = self._cmd_group.get_repcap_cmd_value(plnm, repcap.Plnm)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:PLMN{plnm_cmd_val}?', self.__class__.PlmnStruct())
 
-	def clone(self) -> 'Plmn':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PlmnCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Plmn(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PlmnCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Realm.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Realm.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
 from .....Internal.RepeatedCapability import RepeatedCapability
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Realm:
-	"""Realm commands group definition. 1 total commands, 0 Sub-groups, 1 group commands
+class RealmCls:
+	"""Realm commands group definition. 1 total commands, 0 Subgroups, 1 group commands
 	Repeated Capability: Realm, default value after init: Realm.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("realm", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_realm_get', 'repcap_realm_set', repcap.Realm.Nr1)
+		self._cmd_group = CommandsGroup("realm", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_realm_get', 'repcap_realm_set', repcap.Realm.Nr1)
 
-	def repcap_realm_set(self, enum_value: repcap.Realm) -> None:
+	def repcap_realm_set(self, realm: repcap.Realm) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Realm.Default
 		Default value after init: Realm.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(realm)
 
 	def repcap_realm_get(self) -> repcap.Realm:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	# noinspection PyTypeChecker
 	class RealmStruct(StructBase):
 		"""Structure for setting input parameters. Fields: \n
 			- State: bool: OFF | ON Disables/enables the list entry
 			- Name: str: string Realm name as string
 			- Sim: bool: OFF | ON Realm supports EAP-SIM
@@ -54,32 +54,42 @@
 			self.Tls: bool = None
 			self.Ttls: bool = None
 			self.Aka: bool = None
 			self.Aka_Prime: bool = None
 
 	def set(self, structure: RealmStruct, realm=repcap.Realm.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:REALm<nr> \n
-		Snippet: driver.configure.connection.hotspot.realm.set(value = [PROPERTY_STRUCT_NAME](), realm = repcap.Realm.Default) \n
+		Snippet with structure: \n
+		structure = driver.configure.connection.hotspot.realm.RealmStruct() \n
+		structure.State: bool = False \n
+		structure.Name: str = 'abc' \n
+		structure.Sim: bool = False \n
+		structure.Tls: bool = False \n
+		structure.Ttls: bool = False \n
+		structure.Aka: bool = False \n
+		structure.Aka_Prime: bool = False \n
+		driver.configure.connection.hotspot.realm.set(structure, realm = repcap.Realm.Default) \n
 		Defines a list of NAI realms that are reachable via the hotspot. The first realm can also be defined via method
 		RsCmwWlanSig.Configure.Connection.Hotspot.hsspar. \n
 			:param structure: for set value, see the help for RealmStruct structure arguments.
-			:param realm: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Realm')"""
-		realm_cmd_val = self._base.get_repcap_cmd_value(realm, repcap.Realm)
+			:param realm: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Realm')
+		"""
+		realm_cmd_val = self._cmd_group.get_repcap_cmd_value(realm, repcap.Realm)
 		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:REALm{realm_cmd_val}', structure)
 
 	def get(self, realm=repcap.Realm.Default) -> RealmStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:HOTSpot:REALm<nr> \n
 		Snippet: value: RealmStruct = driver.configure.connection.hotspot.realm.get(realm = repcap.Realm.Default) \n
 		Defines a list of NAI realms that are reachable via the hotspot. The first realm can also be defined via method
 		RsCmwWlanSig.Configure.Connection.Hotspot.hsspar. \n
 			:param realm: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Realm')
 			:return: structure: for return value, see the help for RealmStruct structure arguments."""
-		realm_cmd_val = self._base.get_repcap_cmd_value(realm, repcap.Realm)
+		realm_cmd_val = self._cmd_group.get_repcap_cmd_value(realm, repcap.Realm)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:HOTSpot:REALm{realm_cmd_val}?', self.__class__.RealmStruct())
 
-	def clone(self) -> 'Realm':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'RealmCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Realm(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = RealmCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Muedca.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Per/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,137 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
+from ...Internal.StructBase import StructBase
+from ...Internal.ArgStruct import ArgStruct
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Muedca:
-	"""Muedca commands group definition. 4 total commands, 0 Sub-groups, 4 group commands"""
+class PerCls:
+	"""Per commands group definition. 7 total commands, 1 Subgroups, 5 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("muedca", core, parent)
+		self._cmd_group = CommandsGroup("per", core, parent)
 
-	# noinspection PyTypeChecker
-	class AcbeStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Aif_Sn: int: integer Arbitration inter-frame space number. Zero disables channel access. Range: 0, 2 to 15
-			- Ecw_Min: int: integer Minimal contention window Range: 0 to 15
-			- Ecw_Max: int: integer Maximal contention window Range: 0 to 15
-			- Timer: int: integer MU EDCA timer Range: 1 to 255 , Unit: 8x TUs (8x 1024 µs)"""
-		__meta_args_list = [
-			ArgStruct.scalar_int('Aif_Sn'),
-			ArgStruct.scalar_int('Ecw_Min'),
-			ArgStruct.scalar_int('Ecw_Max'),
-			ArgStruct.scalar_int('Timer')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Aif_Sn: int = None
-			self.Ecw_Min: int = None
-			self.Ecw_Max: int = None
-			self.Timer: int = None
-
-	def get_acbe(self) -> AcbeStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MUEDca:ACBE \n
-		Snippet: value: AcbeStruct = driver.configure.connection.muedca.get_acbe() \n
-		Configures the record fields of MU EDCA parameter set. \n
-			:return: structure: for return value, see the help for AcbeStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MUEDca:ACBE?', self.__class__.AcbeStruct())
-
-	def set_acbe(self, value: AcbeStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MUEDca:ACBE \n
-		Snippet: driver.configure.connection.muedca.set_acbe(value = AcbeStruct()) \n
-		Configures the record fields of MU EDCA parameter set. \n
-			:param value: see the help for AcbeStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MUEDca:ACBE', value)
+	@property
+	def state(self):
+		"""state commands group. 1 Sub-classes, 1 commands."""
+		if not hasattr(self, '_state'):
+			from .State import StateCls
+			self._state = StateCls(self._core, self._cmd_group)
+		return self._state
 
 	# noinspection PyTypeChecker
-	class AcbkStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Aif_Sn: int: integer Arbitration inter-frame space number. Zero disables channel access. Range: 0, 2 to 15
-			- Ecw_Min: int: integer Minimal contention window Range: 0 to 15
-			- Ecw_Max: int: integer Maximal contention window Range: 0 to 15
-			- Timer: int: integer MU EDCA timer Range: 1 to 255 , Unit: 8x TUs (8x 1024 µs)"""
+	class ReadStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Reliability: int: decimal 'Reliability indicator'
+			- Per: float: float Range: 0 % to 100 %
+			- Current_No_Frames: int: No parameter help available
+			- Frames_Lost: int: No parameter help available
+			- Frame_Transmitted: int: No parameter help available
+			- Rx_Burst_Power: float: float Average received burst power of uplink ACK frames Unit: dBm"""
 		__meta_args_list = [
-			ArgStruct.scalar_int('Aif_Sn'),
-			ArgStruct.scalar_int('Ecw_Min'),
-			ArgStruct.scalar_int('Ecw_Max'),
-			ArgStruct.scalar_int('Timer')]
+			ArgStruct.scalar_int('Reliability', 'Reliability'),
+			ArgStruct.scalar_float('Per'),
+			ArgStruct.scalar_int('Current_No_Frames'),
+			ArgStruct.scalar_int('Frames_Lost'),
+			ArgStruct.scalar_int('Frame_Transmitted'),
+			ArgStruct.scalar_float('Rx_Burst_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Aif_Sn: int = None
-			self.Ecw_Min: int = None
-			self.Ecw_Max: int = None
-			self.Timer: int = None
-
-	def get_acbk(self) -> AcbkStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MUEDca:ACBK \n
-		Snippet: value: AcbkStruct = driver.configure.connection.muedca.get_acbk() \n
-		Configures the record fields of MU EDCA parameter set. \n
-			:return: structure: for return value, see the help for AcbkStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MUEDca:ACBK?', self.__class__.AcbkStruct())
-
-	def set_acbk(self, value: AcbkStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MUEDca:ACBK \n
-		Snippet: driver.configure.connection.muedca.set_acbk(value = AcbkStruct()) \n
-		Configures the record fields of MU EDCA parameter set. \n
-			:param value: see the help for AcbkStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MUEDca:ACBK', value)
+			self.Reliability: int = None
+			self.Per: float = None
+			self.Current_No_Frames: int = None
+			self.Frames_Lost: int = None
+			self.Frame_Transmitted: int = None
+			self.Rx_Burst_Power: float = None
+
+	def read(self) -> ReadStruct:
+		"""SCPI: READ:WLAN:SIGNaling<instance>:PER \n
+		Snippet: value: ReadStruct = driver.per.read() \n
+		Returns all results of the PER measurement. \n
+			:return: structure: for return value, see the help for ReadStruct structure arguments."""
+		return self._core.io.query_struct(f'READ:WLAN:SIGNaling<Instance>:PER?', self.__class__.ReadStruct())
 
 	# noinspection PyTypeChecker
-	class AcviStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Aif_Sn: int: integer Arbitration inter-frame space number. Zero disables channel access. Range: 0, 2 to 15
-			- Ecw_Min: int: integer Minimal contention window Range: 0 to 15
-			- Ecw_Max: int: integer Maximal contention window Range: 0 to 15
-			- Timer: int: integer MU EDCA timer Range: 1 to 255 , Unit: 8x TUs (8x 1024 µs)"""
+	class FetchStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Reliability: int: decimal 'Reliability indicator'
+			- Per: float: float Range: 0 % to 100 %
+			- Current_No_Frames: int: No parameter help available
+			- Frames_Lost: int: No parameter help available
+			- Rx_Burst_Power: float: float Average received burst power of uplink ACK frames Unit: dBm"""
 		__meta_args_list = [
-			ArgStruct.scalar_int('Aif_Sn'),
-			ArgStruct.scalar_int('Ecw_Min'),
-			ArgStruct.scalar_int('Ecw_Max'),
-			ArgStruct.scalar_int('Timer')]
+			ArgStruct.scalar_int('Reliability', 'Reliability'),
+			ArgStruct.scalar_float('Per'),
+			ArgStruct.scalar_int('Current_No_Frames'),
+			ArgStruct.scalar_int('Frames_Lost'),
+			ArgStruct.scalar_float('Rx_Burst_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Aif_Sn: int = None
-			self.Ecw_Min: int = None
-			self.Ecw_Max: int = None
-			self.Timer: int = None
-
-	def get_acvi(self) -> AcviStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MUEDca:ACVI \n
-		Snippet: value: AcviStruct = driver.configure.connection.muedca.get_acvi() \n
-		Configures the record fields of MU EDCA parameter set. \n
-			:return: structure: for return value, see the help for AcviStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MUEDca:ACVI?', self.__class__.AcviStruct())
-
-	def set_acvi(self, value: AcviStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MUEDca:ACVI \n
-		Snippet: driver.configure.connection.muedca.set_acvi(value = AcviStruct()) \n
-		Configures the record fields of MU EDCA parameter set. \n
-			:param value: see the help for AcviStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MUEDca:ACVI', value)
-
-	# noinspection PyTypeChecker
-	class AcvoStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Aif_Sn: int: integer Arbitration inter-frame space number. Zero disables channel access. Range: 0, 2 to 15
-			- Ecw_Min: int: integer Minimal contention window Range: 0 to 15
-			- Ecw_Max: int: integer Maximal contention window Range: 0 to 15
-			- Timer: int: integer MU EDCA timer Range: 1 to 255 , Unit: 8x TUs (8x 1024 µs)"""
-		__meta_args_list = [
-			ArgStruct.scalar_int('Aif_Sn'),
-			ArgStruct.scalar_int('Ecw_Min'),
-			ArgStruct.scalar_int('Ecw_Max'),
-			ArgStruct.scalar_int('Timer')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Aif_Sn: int = None
-			self.Ecw_Min: int = None
-			self.Ecw_Max: int = None
-			self.Timer: int = None
-
-	def get_acvo(self) -> AcvoStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MUEDca:ACVO \n
-		Snippet: value: AcvoStruct = driver.configure.connection.muedca.get_acvo() \n
-		Configures the record fields of MU EDCA parameter set. \n
-			:return: structure: for return value, see the help for AcvoStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MUEDca:ACVO?', self.__class__.AcvoStruct())
-
-	def set_acvo(self, value: AcvoStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:MUEDca:ACVO \n
-		Snippet: driver.configure.connection.muedca.set_acvo(value = AcvoStruct()) \n
-		Configures the record fields of MU EDCA parameter set. \n
-			:param value: see the help for AcvoStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:MUEDca:ACVO', value)
+			self.Reliability: int = None
+			self.Per: float = None
+			self.Current_No_Frames: int = None
+			self.Frames_Lost: int = None
+			self.Rx_Burst_Power: float = None
+
+	def fetch(self) -> FetchStruct:
+		"""SCPI: FETCh:WLAN:SIGNaling<instance>:PER \n
+		Snippet: value: FetchStruct = driver.per.fetch() \n
+		Returns all results of the PER measurement. \n
+			:return: structure: for return value, see the help for FetchStruct structure arguments."""
+		return self._core.io.query_struct(f'FETCh:WLAN:SIGNaling<Instance>:PER?', self.__class__.FetchStruct())
+
+	def stop(self) -> None:
+		"""SCPI: STOP:WLAN:SIGNaling<instance>:PER \n
+		Snippet: driver.per.stop() \n
+			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
+			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
+			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
+		Use FETCh...STATe? to query the current measurement state. \n
+		"""
+		self._core.io.write(f'STOP:WLAN:SIGNaling<Instance>:PER')
+
+	def stop_with_opc(self, opc_timeout_ms: int = -1) -> None:
+		"""SCPI: STOP:WLAN:SIGNaling<instance>:PER \n
+		Snippet: driver.per.stop_with_opc() \n
+			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
+			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
+			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
+		Use FETCh...STATe? to query the current measurement state. \n
+		Same as stop, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'STOP:WLAN:SIGNaling<Instance>:PER', opc_timeout_ms)
+
+	def abort(self, opc_timeout_ms: int = -1) -> None:
+		"""SCPI: ABORt:WLAN:SIGNaling<instance>:PER \n
+		Snippet: driver.per.abort() \n
+			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
+			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
+			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
+		Use FETCh...STATe? to query the current measurement state. \n
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'ABORt:WLAN:SIGNaling<Instance>:PER', opc_timeout_ms)
+
+	def initiate(self, opc_timeout_ms: int = -1) -> None:
+		"""SCPI: INITiate:WLAN:SIGNaling<instance>:PER \n
+		Snippet: driver.per.initiate() \n
+			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
+			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
+			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
+		Use FETCh...STATe? to query the current measurement state. \n
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'INITiate:WLAN:SIGNaling<Instance>:PER', opc_timeout_ms)
+
+	def clone(self) -> 'PerCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
+		Also copies all the existing default Repeated Capabilities setting,
+		which you can change independently without affecting the original group"""
+		new_group = PerCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
+		return new_group
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/NdpSounding/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class NdpSounding:
-	"""NdpSounding commands group definition. 14 total commands, 1 Sub-groups, 13 group commands"""
+class NdpSoundingCls:
+	"""NdpSounding commands group definition. 14 total commands, 1 Subgroups, 13 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ndpSounding", core, parent)
+		self._cmd_group = CommandsGroup("ndpSounding", core, parent)
 
 	@property
 	def ssTx(self):
 		"""ssTx commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ssTx'):
-			from .NdpSounding_.SsTx import SsTx
-			self._ssTx = SsTx(self._core, self._base)
+			from .SsTx import SsTxCls
+			self._ssTx = SsTxCls(self._core, self._cmd_group)
 		return self._ssTx
 
 	# noinspection PyTypeChecker
 	def get_method(self) -> enums.NdpSoundingMethod:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:NDPSounding:METHod \n
 		Snippet: value: enums.NdpSoundingMethod = driver.configure.connection.ndpSounding.get_method() \n
 		Sets the feedback method for NDP sounding procedure. \n
@@ -210,25 +210,25 @@
 		param = Conversions.enum_scalar_to_str(num_col, enums.NumColumns)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:NDPSounding:NUMColumns {param}')
 
 	# noinspection PyTypeChecker
 	def get_sub_grouping(self) -> enums.Ngrouping:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:NDPSounding:SUBGrouping \n
 		Snippet: value: enums.Ngrouping = driver.configure.connection.ndpSounding.get_sub_grouping() \n
-		Sets the subcarrier grouping value Ng for HE TB sounding. \n
-			:return: ng: GRP4 | GRP16
+		No command help available \n
+			:return: ng: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:CONNection:NDPSounding:SUBGrouping?')
 		return Conversions.str_to_scalar_enum(response, enums.Ngrouping)
 
 	def set_sub_grouping(self, ng: enums.Ngrouping) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:NDPSounding:SUBGrouping \n
 		Snippet: driver.configure.connection.ndpSounding.set_sub_grouping(ng = enums.Ngrouping.GRP16) \n
-		Sets the subcarrier grouping value Ng for HE TB sounding. \n
-			:param ng: GRP4 | GRP16
+		No command help available \n
+			:param ng: No help available
 		"""
 		param = Conversions.enum_scalar_to_str(ng, enums.Ngrouping)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:NDPSounding:SUBGrouping {param}')
 
 	def get_txp(self) -> int:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:NDPSounding:TXP \n
 		Snippet: value: int = driver.configure.connection.ndpSounding.get_txp() \n
@@ -261,14 +261,14 @@
 		Snippet: driver.configure.connection.ndpSounding.set_txen(state = False) \n
 		Switches on or off the periodic transmission for NDP sounding procedure. \n
 			:param state: OFF | ON
 		"""
 		param = Conversions.bool_to_str(state)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:NDPSounding:TXEN {param}')
 
-	def clone(self) -> 'NdpSounding':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'NdpSoundingCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = NdpSounding(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = NdpSoundingCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding_/SsTx.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/NdpSounding/SsTx.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SsTx:
-	"""SsTx commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class SsTxCls:
+	"""SsTx commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ssTx", core, parent)
+		self._cmd_group = CommandsGroup("ssTx", core, parent)
 
 	def set(self) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:NDPSounding:SSTX \n
 		Snippet: driver.configure.connection.ndpSounding.ssTx.set() \n
 		Triggers the single-shot transmission for NDP sounding procedure. \n
 		"""
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:NDPSounding:SSTX')
 
-	def set_with_opc(self) -> None:
+	def set_with_opc(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:NDPSounding:SSTX \n
 		Snippet: driver.configure.connection.ndpSounding.ssTx.set_with_opc() \n
 		Triggers the single-shot transmission for NDP sounding procedure. \n
 		Same as set, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:NDPSounding:SSTX')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:NDPSounding:SSTX', opc_timeout_ms)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Qos.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Qos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Qos:
-	"""Qos commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class QosCls:
+	"""Qos commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("qos", core, parent)
+		self._cmd_group = CommandsGroup("qos", core, parent)
 
 	# noinspection PyTypeChecker
 	def get_etoe(self) -> enums.Tid:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:QOS:ETOE \n
 		Snippet: value: enums.Tid = driver.configure.connection.qos.get_etoe() \n
 		Sets the TID value to be used for the end-to-end connection using DAU. \n
 			:return: tid: TID0 | TID1 | TID2 | TID3 | TID4 | TID5 | TID6 | TID7
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/Eaka.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Eaka/Kalgo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,40 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal.StructBase import StructBase
-from .....Internal.ArgStruct import ArgStruct
-from ..... import enums
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal.Types import DataType
+from ......Internal.StructBase import StructBase
+from ......Internal.ArgStruct import ArgStruct
+from ......Internal.ArgSingleList import ArgSingleList
+from ......Internal.ArgSingle import ArgSingle
+from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Eaka:
-	"""Eaka commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class KalgoCls:
+	"""Kalgo commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("eaka", core, parent)
+		self._cmd_group = CommandsGroup("kalgo", core, parent)
+
+	def set(self, ki: str, opc: str, rand: str, algorithm: enums.AuthAlgorithm) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SECurity:EAKA:KALGo \n
+		Snippet: driver.configure.connection.security.eaka.kalgo.set(ki = 'abc', opc = 'abc', rand = 'abc', algorithm = enums.AuthAlgorithm.MILenage) \n
+		Configures EAP-AKA on the internal RADIUS server. \n
+			:param ki: string Secret key as string with 32 hexadecimal digits
+			:param opc: string Operator variant key as string with 32 hexadecimal digits
+			:param rand: string Random number as string with 32 hexadecimal digits
+			:param algorithm: MILenage | XOR Authentication algorithm to be used
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ki', ki, DataType.String), ArgSingle('opc', opc, DataType.String), ArgSingle('rand', rand, DataType.String), ArgSingle('algorithm', algorithm, DataType.Enum, enums.AuthAlgorithm))
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:SECurity:EAKA:KALGo {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class KalgoStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- Ki: str: string Secret key as string with 32 hexadecimal digits
 			- Opc: str: string Operator variant key as string with 32 hexadecimal digits
 			- Rand: str: string Random number as string with 32 hexadecimal digits
 			- Algorithm: enums.AuthAlgorithm: MILenage | XOR Authentication algorithm to be used"""
 		__meta_args_list = [
 			ArgStruct.scalar_str('Ki'),
 			ArgStruct.scalar_str('Opc'),
@@ -29,22 +44,13 @@
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Ki: str = None
 			self.Opc: str = None
 			self.Rand: str = None
 			self.Algorithm: enums.AuthAlgorithm = None
 
-	def get_kalgo(self) -> KalgoStruct:
+	def get(self) -> KalgoStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SECurity:EAKA:KALGo \n
-		Snippet: value: KalgoStruct = driver.configure.connection.security.eaka.get_kalgo() \n
+		Snippet: value: KalgoStruct = driver.configure.connection.security.eaka.kalgo.get() \n
 		Configures EAP-AKA on the internal RADIUS server. \n
-			:return: structure: for return value, see the help for KalgoStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SECurity:EAKA:KALGo?', self.__class__.KalgoStruct())
-
-	def set_kalgo(self, value: KalgoStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SECurity:EAKA:KALGo \n
-		Snippet: driver.configure.connection.security.eaka.set_kalgo(value = KalgoStruct()) \n
-		Configures EAP-AKA on the internal RADIUS server. \n
-			:param value: see the help for KalgoStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SECurity:EAKA:KALGo', value)
+			:return: structure: for return value, see the help for KalgoStruct structure arguments."""
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:SECurity:EAKA:KALGo?', self.__class__.KalgoStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Srates.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Srates/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,30 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from .....Internal.StructBase import StructBase
+from .....Internal.ArgStruct import ArgStruct
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Srates:
-	"""Srates commands group definition. 5 total commands, 0 Sub-groups, 5 group commands"""
+class SratesCls:
+	"""Srates commands group definition. 5 total commands, 1 Subgroups, 4 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("srates", core, parent)
+		self._cmd_group = CommandsGroup("srates", core, parent)
+
+	@property
+	def dsssConf(self):
+		"""dsssConf commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_dsssConf'):
+			from .DsssConf import DsssConfCls
+			self._dsssConf = DsssConfCls(self._core, self._cmd_group)
+		return self._dsssConf
 
 	# noinspection PyTypeChecker
 	def get_vht_conf(self) -> enums.VhtRates:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes:VHTConf \n
 		Snippet: value: enums.VhtRates = driver.configure.connection.srates.get_vht_conf() \n
 		Definition of supported OFDM VHT modulation and coding schemes (MCS) . These settings apply only if user-defined
 		supported rates are enabled, see method RsCmwWlanSig.Configure.Connection.Srates.value. \n
@@ -32,16 +40,16 @@
 		supported rates are enabled, see method RsCmwWlanSig.Configure.Connection.Srates.value. \n
 			:param vht_rates: MC07 | MC08 | MC09 MC07: MCS 0 to MCS 7 MC08: MCS 0 to MCS 8 MC09: MCS 0 to MCS 9
 		"""
 		param = Conversions.enum_scalar_to_str(vht_rates, enums.VhtRates)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes:VHTConf {param}')
 
 	# noinspection PyTypeChecker
-	class OmcsConfStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+	class OmcsConfStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
+		"""Structure for setting input parameters. Fields: \n
 			- Mcs_0: enums.McsSupport: NOTSupported | SUPPorted
 			- Mcs_1: enums.McsSupport: NOTSupported | SUPPorted
 			- Mcs_2: enums.McsSupport: NOTSupported | SUPPorted
 			- Mcs_3: enums.McsSupport: NOTSupported | SUPPorted
 			- Mcs_4: enums.McsSupport: NOTSupported | SUPPorted
 			- Mcs_5: enums.McsSupport: NOTSupported | SUPPorted
 			- Mcs_6: enums.McsSupport: NOTSupported | SUPPorted
@@ -63,36 +71,45 @@
 			self.Mcs_2: enums.McsSupport = None
 			self.Mcs_3: enums.McsSupport = None
 			self.Mcs_4: enums.McsSupport = None
 			self.Mcs_5: enums.McsSupport = None
 			self.Mcs_6: enums.McsSupport = None
 			self.Mcs_7: enums.McsSupport = None
 
-	# noinspection PyTypeChecker
 	def get_omcs_conf(self) -> OmcsConfStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes:OMCSconf \n
 		Snippet: value: OmcsConfStruct = driver.configure.connection.srates.get_omcs_conf() \n
 		Definition of supported OFDM HT modulation and coding schemes (MCS) . These settings apply only if user-defined supported
 		rates are enabled, see method RsCmwWlanSig.Configure.Connection.Srates.value. \n
 			:return: structure: for return value, see the help for OmcsConfStruct structure arguments.
 		"""
 		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes:OMCSconf?', self.__class__.OmcsConfStruct())
 
 	def set_omcs_conf(self, value: OmcsConfStruct) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes:OMCSconf \n
-		Snippet: driver.configure.connection.srates.set_omcs_conf(value = OmcsConfStruct()) \n
+		Snippet with structure: \n
+		structure = driver.configure.connection.srates.OmcsConfStruct() \n
+		structure.Mcs_0: enums.McsSupport = enums.McsSupport.NOTSupported \n
+		structure.Mcs_1: enums.McsSupport = enums.McsSupport.NOTSupported \n
+		structure.Mcs_2: enums.McsSupport = enums.McsSupport.NOTSupported \n
+		structure.Mcs_3: enums.McsSupport = enums.McsSupport.NOTSupported \n
+		structure.Mcs_4: enums.McsSupport = enums.McsSupport.NOTSupported \n
+		structure.Mcs_5: enums.McsSupport = enums.McsSupport.NOTSupported \n
+		structure.Mcs_6: enums.McsSupport = enums.McsSupport.NOTSupported \n
+		structure.Mcs_7: enums.McsSupport = enums.McsSupport.NOTSupported \n
+		driver.configure.connection.srates.set_omcs_conf(value = structure) \n
 		Definition of supported OFDM HT modulation and coding schemes (MCS) . These settings apply only if user-defined supported
 		rates are enabled, see method RsCmwWlanSig.Configure.Connection.Srates.value. \n
 			:param value: see the help for OmcsConfStruct structure arguments.
 		"""
 		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes:OMCSconf', value)
 
 	# noinspection PyTypeChecker
-	class OfdmConfStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+	class OfdmConfStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
+		"""Structure for setting input parameters. Fields: \n
 			- Br_12: enums.RateSupport: DISabled | MANDatory | OPTional Support for BPSK, 1/2, 6 Mbit/s
 			- Br_34: enums.RateSupport: DISabled | MANDatory | OPTional Support for BPSK, 3/4, 9 Mbit/s
 			- Qr_12: enums.RateSupport: DISabled | MANDatory | OPTional Support for QPSK, 1/2, 12 Mbit/s
 			- Qr_34: enums.RateSupport: DISabled | MANDatory | OPTional Support for QPSK, 3/4, 18 Mbit/s
 			- Q_1_M_12: enums.RateSupport: DISabled | MANDatory | OPTional Support for 16-QAM, 1/2, 24 Mbit/s
 			- Q_1_M_34: enums.RateSupport: DISabled | MANDatory | OPTional Support for 16-QAM, 3/4, 36 Mbit/s
 			- Q_6_M_23: enums.RateSupport: DISabled | MANDatory | OPTional Support for 64-QAM, 2/3, 48 Mbit/s
@@ -114,73 +131,43 @@
 			self.Qr_12: enums.RateSupport = None
 			self.Qr_34: enums.RateSupport = None
 			self.Q_1_M_12: enums.RateSupport = None
 			self.Q_1_M_34: enums.RateSupport = None
 			self.Q_6_M_23: enums.RateSupport = None
 			self.Q_6_M_34: enums.RateSupport = None
 
-	# noinspection PyTypeChecker
 	def get_ofdm_conf(self) -> OfdmConfStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes:OFDMconf \n
 		Snippet: value: OfdmConfStruct = driver.configure.connection.srates.get_ofdm_conf() \n
 		Definition of OFDM non-HT supported rates (modulation, coding rate, data rate) . These settings apply only if
 		user-defined supported rates are enabled, see method RsCmwWlanSig.Configure.Connection.Srates.value. \n
 			:return: structure: for return value, see the help for OfdmConfStruct structure arguments.
 		"""
 		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes:OFDMconf?', self.__class__.OfdmConfStruct())
 
 	def set_ofdm_conf(self, value: OfdmConfStruct) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes:OFDMconf \n
-		Snippet: driver.configure.connection.srates.set_ofdm_conf(value = OfdmConfStruct()) \n
+		Snippet with structure: \n
+		structure = driver.configure.connection.srates.OfdmConfStruct() \n
+		structure.Br_12: enums.RateSupport = enums.RateSupport.DISabled \n
+		structure.Br_34: enums.RateSupport = enums.RateSupport.DISabled \n
+		structure.Qr_12: enums.RateSupport = enums.RateSupport.DISabled \n
+		structure.Qr_34: enums.RateSupport = enums.RateSupport.DISabled \n
+		structure.Q_1_M_12: enums.RateSupport = enums.RateSupport.DISabled \n
+		structure.Q_1_M_34: enums.RateSupport = enums.RateSupport.DISabled \n
+		structure.Q_6_M_23: enums.RateSupport = enums.RateSupport.DISabled \n
+		structure.Q_6_M_34: enums.RateSupport = enums.RateSupport.DISabled \n
+		driver.configure.connection.srates.set_ofdm_conf(value = structure) \n
 		Definition of OFDM non-HT supported rates (modulation, coding rate, data rate) . These settings apply only if
 		user-defined supported rates are enabled, see method RsCmwWlanSig.Configure.Connection.Srates.value. \n
 			:param value: see the help for OfdmConfStruct structure arguments.
 		"""
 		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes:OFDMconf', value)
 
 	# noinspection PyTypeChecker
-	class DsssConfStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- D_1_Mb: enums.RateSupport: DISabled | MANDatory | OPTional Support for DSSS, 1 Mbit/s
-			- D_2_Mb: enums.RateSupport: DISabled | MANDatory | OPTional Support for DSSS, 2 Mbit/s
-			- C_55_M: enums.RateSupport: DISabled | MANDatory | OPTional Support for CCK, 5.5 Mbit/s
-			- C_11_M: enums.RateSupport: DISabled | MANDatory | OPTional Support for CCK, 11 Mbit/s"""
-		__meta_args_list = [
-			ArgStruct.scalar_enum('D_1_Mb', enums.RateSupport),
-			ArgStruct.scalar_enum('D_2_Mb', enums.RateSupport),
-			ArgStruct.scalar_enum('C_55_M', enums.RateSupport),
-			ArgStruct.scalar_enum('C_11_M', enums.RateSupport)]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.D_1_Mb: enums.RateSupport = None
-			self.D_2_Mb: enums.RateSupport = None
-			self.C_55_M: enums.RateSupport = None
-			self.C_11_M: enums.RateSupport = None
-
-	# noinspection PyTypeChecker
-	def get_dsss_conf(self) -> DsssConfStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes:DSSSconf \n
-		Snippet: value: DsssConfStruct = driver.configure.connection.srates.get_dsss_conf() \n
-		Definition of DSSS/CCK supported rates. These settings apply only if user-defined supported rates are enabled, see method
-		RsCmwWlanSig.Configure.Connection.Srates.value. \n
-			:return: structure: for return value, see the help for DsssConfStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes:DSSSconf?', self.__class__.DsssConfStruct())
-
-	def set_dsss_conf(self, value: DsssConfStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes:DSSSconf \n
-		Snippet: driver.configure.connection.srates.set_dsss_conf(value = DsssConfStruct()) \n
-		Definition of DSSS/CCK supported rates. These settings apply only if user-defined supported rates are enabled, see method
-		RsCmwWlanSig.Configure.Connection.Srates.value. \n
-			:param value: see the help for DsssConfStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes:DSSSconf', value)
-
-	# noinspection PyTypeChecker
 	def get_value(self) -> enums.EnableState:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes \n
 		Snippet: value: enums.EnableState = driver.configure.connection.srates.get_value() \n
 		Enables/disables user-defined supported rates. \n
 			:return: state: ENABle | DISable
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes?')
@@ -190,7 +177,15 @@
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:SRATes \n
 		Snippet: driver.configure.connection.srates.set_value(state = enums.EnableState.DISable) \n
 		Enables/disables user-defined supported rates. \n
 			:param state: ENABle | DISable
 		"""
 		param = Conversions.enum_scalar_to_str(state, enums.EnableState)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:SRATes {param}')
+
+	def clone(self) -> 'SratesCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
+		Also copies all the existing default Repeated Capabilities setting,
+		which you can change independently without affecting the original group"""
+		new_group = SratesCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
+		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal.RepeatedCapability import RepeatedCapability
 from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sta:
-	"""Sta commands group definition. 8 total commands, 1 Sub-groups, 0 group commands
+class StaCls:
+	"""Sta commands group definition. 13 total commands, 1 Subgroups, 0 group commands
 	Repeated Capability: Station, default value after init: Station.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sta", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
+		self._cmd_group = CommandsGroup("sta", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
 
-	def repcap_station_set(self, enum_value: repcap.Station) -> None:
+	def repcap_station_set(self, station: repcap.Station) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Station.Default
 		Default value after init: Station.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(station)
 
 	def repcap_station_get(self) -> repcap.Station:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
-	def dframe(self):
-		"""dframe commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_dframe'):
-			from .Sta_.Dframe import Dframe
-			self._dframe = Dframe(self._core, self._base)
-		return self._dframe
+	def connection(self):
+		"""connection commands group. 4 Sub-classes, 0 commands."""
+		if not hasattr(self, '_connection'):
+			from .Connection import ConnectionCls
+			self._connection = ConnectionCls(self._core, self._cmd_group)
+		return self._connection
 
-	def clone(self) -> 'Sta':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'StaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Sta(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = StaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dframe:
-	"""Dframe commands group definition. 8 total commands, 1 Sub-groups, 0 group commands"""
+class DframeCls:
+	"""Dframe commands group definition. 8 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dframe", core, parent)
+		self._cmd_group = CommandsGroup("dframe", core, parent)
 
 	@property
 	def hemu(self):
 		"""hemu commands group. 5 Sub-classes, 0 commands."""
 		if not hasattr(self, '_hemu'):
-			from .Dframe_.Hemu import Hemu
-			self._hemu = Hemu(self._core, self._base)
+			from .Hemu import HemuCls
+			self._hemu = HemuCls(self._core, self._cmd_group)
 		return self._hemu
 
-	def clone(self) -> 'Dframe':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'DframeCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Dframe(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = DframeCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hemu:
-	"""Hemu commands group definition. 8 total commands, 5 Sub-groups, 0 group commands"""
+class HemuCls:
+	"""Hemu commands group definition. 8 total commands, 5 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hemu", core, parent)
+		self._cmd_group = CommandsGroup("hemu", core, parent)
 
 	@property
 	def alsField(self):
 		"""alsField commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_alsField'):
-			from .Hemu_.AlsField import AlsField
-			self._alsField = AlsField(self._core, self._base)
+			from .AlsField import AlsFieldCls
+			self._alsField = AlsFieldCls(self._core, self._cmd_group)
 		return self._alsField
 
 	@property
 	def ruAllocation(self):
 		"""ruAllocation commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ruAllocation'):
-			from .Hemu_.RuAllocation import RuAllocation
-			self._ruAllocation = RuAllocation(self._core, self._base)
+			from .RuAllocation import RuAllocationCls
+			self._ruAllocation = RuAllocationCls(self._core, self._cmd_group)
 		return self._ruAllocation
 
 	@property
 	def blAllocation(self):
 		"""blAllocation commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_blAllocation'):
-			from .Hemu_.BlAllocation import BlAllocation
-			self._blAllocation = BlAllocation(self._core, self._base)
+			from .BlAllocation import BlAllocationCls
+			self._blAllocation = BlAllocationCls(self._core, self._cmd_group)
 		return self._blAllocation
 
 	@property
 	def user(self):
 		"""user commands group. 4 Sub-classes, 0 commands."""
 		if not hasattr(self, '_user'):
-			from .Hemu_.User import User
-			self._user = User(self._core, self._base)
+			from .User import UserCls
+			self._user = UserCls(self._core, self._cmd_group)
 		return self._user
 
 	@property
 	def dummy(self):
 		"""dummy commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_dummy'):
-			from .Hemu_.Dummy import Dummy
-			self._dummy = Dummy(self._core, self._base)
+			from .Dummy import DummyCls
+			self._dummy = DummyCls(self._core, self._cmd_group)
 		return self._dummy
 
-	def clone(self) -> 'Hemu':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'HemuCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Hemu(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = HemuCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/AlsField.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/AlsField.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,39 +5,40 @@
 from .......Internal.ArgSingleList import ArgSingleList
 from .......Internal.ArgSingle import ArgSingle
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class AlsField:
-	"""AlsField commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class AlsFieldCls:
+	"""AlsField commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("alsField", core, parent)
+		self._cmd_group = CommandsGroup("alsField", core, parent)
 
 	def set(self, ch_20_index: enums.Ch20Index, subfield: enums.Subfield, station=repcap.Station.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:ALSField \n
 		Snippet: driver.configure.connection.sta.dframe.hemu.alsField.set(ch_20_index = enums.Ch20Index.CHA1, subfield = enums.Subfield.A000, station = repcap.Station.Default) \n
 		Sets 8-bit indices for resource unit (RU) allocation for the selected channel. The <Subfield> parameter specifies the
-		number of RUs, their position and size. Refer to IEEE P802.11ax/D8.0, table 27-26, RU allocation subfield. \n
+		number of RUs, their position and size. Refer to IEEE Std 802.11ax-2021, table 27-26, RU allocation subfield. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:param subfield: A000 | A001 | A002 | A003 | A004 | A005 | A006 | A007 | A008 | A009 | A010 | A011 | A012 | A013 | A014 | A015 | A016 | A024 | A032 | A040 | A048 | A056 | A064 | A072 | A080 | A088 | A096 | A112 | A113 | A114 | A115 | A116 | A120 | A128 | A192 | A200 | A208 | A216 | A224
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum), ArgSingle('subfield', subfield, DataType.Enum))
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum, enums.Ch20Index), ArgSingle('subfield', subfield, DataType.Enum, enums.Subfield))
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:ALSField {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	def get(self, ch_20_index: enums.Ch20Index, station=repcap.Station.Default) -> enums.Subfield:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:ALSField \n
 		Snippet: value: enums.Subfield = driver.configure.connection.sta.dframe.hemu.alsField.get(ch_20_index = enums.Ch20Index.CHA1, station = repcap.Station.Default) \n
 		Sets 8-bit indices for resource unit (RU) allocation for the selected channel. The <Subfield> parameter specifies the
-		number of RUs, their position and size. Refer to IEEE P802.11ax/D8.0, table 27-26, RU allocation subfield. \n
+		number of RUs, their position and size. Refer to IEEE Std 802.11ax-2021, table 27-26, RU allocation subfield. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: subfield: A000 | A001 | A002 | A003 | A004 | A005 | A006 | A007 | A008 | A009 | A010 | A011 | A012 | A013 | A014 | A015 | A016 | A024 | A032 | A040 | A048 | A056 | A064 | A072 | A080 | A088 | A096 | A112 | A113 | A114 | A115 | A116 | A120 | A128 | A192 | A200 | A208 | A216 | A224"""
 		param = Conversions.enum_scalar_to_str(ch_20_index, enums.Ch20Index)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:ALSField? {param}')
 		return Conversions.str_to_scalar_enum(response, enums.Subfield)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/BlAllocation.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/BlAllocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from .......Internal.StructBase import StructBase
 from .......Internal.ArgStruct import ArgStruct
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class BlAllocation:
-	"""BlAllocation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class BlAllocationCls:
+	"""BlAllocation commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("blAllocation", core, parent)
+		self._cmd_group = CommandsGroup("blAllocation", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Ru_1: enums.RuAlloc: OFF | USR1 | DMY1 | DMY2 | DMY3 User mapping for to the corresponding RU (no user, user 1 or dummy user)
 			- Size_1: enums.AllocSize: No parameter help available
 			- Ru_2: enums.RuAlloc: No parameter help available
@@ -81,9 +81,9 @@
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:BLALlocation \n
 		Snippet: value: GetStruct = driver.configure.connection.sta.dframe.hemu.blAllocation.get(ch_20_index = enums.Ch20Index.CHA1, station = repcap.Station.Default) \n
 		Queries the allocation state and size of an entire 20MHz block for the specified channel. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
 		param = Conversions.enum_scalar_to_str(ch_20_index, enums.Ch20Index)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:BLALlocation? {param}', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/Dummy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from .......Internal.Core import Core
 from .......Internal.CommandsGroup import CommandsGroup
 from .......Internal.RepeatedCapability import RepeatedCapability
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dummy:
-	"""Dummy commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
+class DummyCls:
+	"""Dummy commands group definition. 1 total commands, 1 Subgroups, 0 group commands
 	Repeated Capability: Dummy, default value after init: Dummy.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dummy", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_dummy_get', 'repcap_dummy_set', repcap.Dummy.Nr1)
+		self._cmd_group = CommandsGroup("dummy", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_dummy_get', 'repcap_dummy_set', repcap.Dummy.Nr1)
 
-	def repcap_dummy_set(self, enum_value: repcap.Dummy) -> None:
+	def repcap_dummy_set(self, dummy: repcap.Dummy) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Dummy.Default
 		Default value after init: Dummy.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(dummy)
 
 	def repcap_dummy_get(self) -> repcap.Dummy:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def mcs(self):
 		"""mcs commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mcs'):
-			from .Dummy_.Mcs import Mcs
-			self._mcs = Mcs(self._core, self._base)
+			from .Mcs import McsCls
+			self._mcs = McsCls(self._core, self._cmd_group)
 		return self._mcs
 
-	def clone(self) -> 'Dummy':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'DummyCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Dummy(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = DummyCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy_/Mcs.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Mcs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 from ........Internal.CommandsGroup import CommandsGroup
 from ........Internal import Conversions
 from ........ import enums
 from ........ import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mcs:
-	"""Mcs commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class McsCls:
+	"""Mcs commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mcs", core, parent)
+		self._cmd_group = CommandsGroup("mcs", core, parent)
 
-	def set(self, mcs_index: enums.McsIndex, station=repcap.Station.Default, dummy=repcap.Dummy.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:DUMMy<index>:MCS \n
-		Snippet: driver.configure.connection.sta.dframe.hemu.dummy.mcs.set(mcs_index = enums.McsIndex.MCS, station = repcap.Station.Default, dummy = repcap.Dummy.Default) \n
-		Sets the modulation and coding scheme for the corresponding dummy user. \n
-			:param mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11
+	def set(self, mcs_index: enums.McsIndex, station=repcap.Station.Default, user=repcap.User.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:MCS \n
+		Snippet: driver.configure.connection.sta.dframe.hemu.user.mcs.set(mcs_index = enums.McsIndex.MCS, station = repcap.Station.Default, user = repcap.User.Default) \n
+		Sets the modulation and coding scheme for user 1 (user data assigned to the DUT) . \n
+			:param mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0, MCS 1 to MCS 11
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:param dummy: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Dummy')"""
+			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
+		"""
 		param = Conversions.enum_scalar_to_str(mcs_index, enums.McsIndex)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		dummy_cmd_val = self._base.get_repcap_cmd_value(dummy, repcap.Dummy)
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:DUMMy{dummy_cmd_val}:MCS {param}')
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:MCS {param}')
 
 	# noinspection PyTypeChecker
-	def get(self, station=repcap.Station.Default, dummy=repcap.Dummy.Default) -> enums.McsIndex:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:DUMMy<index>:MCS \n
-		Snippet: value: enums.McsIndex = driver.configure.connection.sta.dframe.hemu.dummy.mcs.get(station = repcap.Station.Default, dummy = repcap.Dummy.Default) \n
-		Sets the modulation and coding scheme for the corresponding dummy user. \n
+	def get(self, station=repcap.Station.Default, user=repcap.User.Default) -> enums.McsIndex:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:MCS \n
+		Snippet: value: enums.McsIndex = driver.configure.connection.sta.dframe.hemu.user.mcs.get(station = repcap.Station.Default, user = repcap.User.Default) \n
+		Sets the modulation and coding scheme for user 1 (user data assigned to the DUT) . \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:param dummy: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Dummy')
-			:return: mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		dummy_cmd_val = self._base.get_repcap_cmd_value(dummy, repcap.Dummy)
-		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:DUMMy{dummy_cmd_val}:MCS?')
+			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
+			:return: mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0, MCS 1 to MCS 11"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
+		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:MCS?')
 		return Conversions.str_to_scalar_enum(response, enums.McsIndex)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/RuAllocation.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/RuAllocation.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 from .......Internal.ArgSingleList import ArgSingleList
 from .......Internal.ArgSingle import ArgSingle
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RuAllocation:
-	"""RuAllocation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class RuAllocationCls:
+	"""RuAllocation commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ruAllocation", core, parent)
+		self._cmd_group = CommandsGroup("ruAllocation", core, parent)
 
 	def set(self, ch_20_index: enums.Ch20Index, ru_index: enums.RuIndex, alloc_state: enums.RuAlloc, station=repcap.Station.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:RUALlocation \n
 		Snippet: driver.configure.connection.sta.dframe.hemu.ruAllocation.set(ch_20_index = enums.Ch20Index.CHA1, ru_index = enums.RuIndex.RU1, alloc_state = enums.RuAlloc.DMY1, station = repcap.Station.Default) \n
 		Configures allocations for specified channel and resource unit (RU) . Maps a user to the RU, sets the size of allocation. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:param ru_index: RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9 Resource unit selection
 			:param alloc_state: OFF | USR1 | DMY1 | DMY2 | DMY3 User mapping for to the selected RU
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum), ArgSingle('ru_index', ru_index, DataType.Enum), ArgSingle('alloc_state', alloc_state, DataType.Enum))
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum, enums.Ch20Index), ArgSingle('ru_index', ru_index, DataType.Enum, enums.RuIndex), ArgSingle('alloc_state', alloc_state, DataType.Enum, enums.RuAlloc))
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:RUALlocation {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Alloc_State: enums.RuAlloc: OFF | USR1 | DMY1 | DMY2 | DMY3 User mapping for to the selected RU
 			- Size: enums.AllocSize: T26 | T52 | T106 | T242 | T484 | T996 | T2X9 RU size: 26-, 52-, 106-, 242-, 484, 996-tone RU, 2x996-tone RU"""
@@ -47,10 +48,10 @@
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:RUALlocation \n
 		Snippet: value: GetStruct = driver.configure.connection.sta.dframe.hemu.ruAllocation.get(ch_20_index = enums.Ch20Index.CHA1, ru_index = enums.RuIndex.RU1, station = repcap.Station.Default) \n
 		Configures allocations for specified channel and resource unit (RU) . Maps a user to the RU, sets the size of allocation. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:param ru_index: RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9 Resource unit selection
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum), ArgSingle('ru_index', ru_index, DataType.Enum))
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum, enums.Ch20Index), ArgSingle('ru_index', ru_index, DataType.Enum, enums.RuIndex))
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:RUALlocation? {param}'.rstrip(), self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from .......Internal.Core import Core
-from .......Internal.CommandsGroup import CommandsGroup
-from .......Internal.RepeatedCapability import RepeatedCapability
-from ....... import repcap
+from ........Internal.Core import Core
+from ........Internal.CommandsGroup import CommandsGroup
+from ........Internal.RepeatedCapability import RepeatedCapability
+from ........ import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class User:
-	"""User commands group definition. 4 total commands, 4 Sub-groups, 0 group commands
+class UserCls:
+	"""User commands group definition. 4 total commands, 4 Subgroups, 0 group commands
 	Repeated Capability: User, default value after init: User.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("user", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_user_get', 'repcap_user_set', repcap.User.Nr1)
+		self._cmd_group = CommandsGroup("user", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_user_get', 'repcap_user_set', repcap.User.Nr1)
 
-	def repcap_user_set(self, enum_value: repcap.User) -> None:
+	def repcap_user_set(self, user: repcap.User) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to User.Default
 		Default value after init: User.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(user)
 
 	def repcap_user_get(self) -> repcap.User:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def allocation(self):
 		"""allocation commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_allocation'):
-			from .User_.Allocation import Allocation
-			self._allocation = Allocation(self._core, self._base)
+			from .Allocation import AllocationCls
+			self._allocation = AllocationCls(self._core, self._cmd_group)
 		return self._allocation
 
 	@property
 	def mcs(self):
 		"""mcs commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mcs'):
-			from .User_.Mcs import Mcs
-			self._mcs = Mcs(self._core, self._base)
+			from .Mcs import McsCls
+			self._mcs = McsCls(self._core, self._cmd_group)
 		return self._mcs
 
 	@property
 	def streams(self):
 		"""streams commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_streams'):
-			from .User_.Streams import Streams
-			self._streams = Streams(self._core, self._base)
+			from .Streams import StreamsCls
+			self._streams = StreamsCls(self._core, self._cmd_group)
 		return self._streams
 
 	@property
 	def ctype(self):
 		"""ctype commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ctype'):
-			from .User_.Ctype import Ctype
-			self._ctype = Ctype(self._core, self._base)
+			from .Ctype import CtypeCls
+			self._ctype = CtypeCls(self._core, self._cmd_group)
 		return self._ctype
 
-	def clone(self) -> 'User':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'UserCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = User(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = UserCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Allocation.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Ampdu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-from ........Internal.Core import Core
-from ........Internal.CommandsGroup import CommandsGroup
-from ........Internal.StructBase import StructBase
-from ........Internal.ArgStruct import ArgStruct
-from ........ import enums
-from ........ import repcap
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Types import DataType
+from .....Internal.StructBase import StructBase
+from .....Internal.ArgStruct import ArgStruct
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
+from ..... import enums
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Allocation:
-	"""Allocation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class AmpduCls:
+	"""Ampdu commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("allocation", core, parent)
+		self._cmd_group = CommandsGroup("ampdu", core, parent)
+
+	def set(self, enable: enums.EnableState, multi_tid: enums.EnableState, max_length: int, station=repcap.Station.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:AMPDu \n
+		Snippet: driver.configure.sta.connection.ampdu.set(enable = enums.EnableState.DISable, multi_tid = enums.EnableState.DISable, max_length = 1, station = repcap.Station.Default) \n
+		Configures aggregate MPDUs (A-MPDU) . \n
+			:param enable: DISable | ENABle Enables/ disables the A-MPDUs
+			:param multi_tid: DISable | ENABle Enables/ disables multi-TID A-MPDU
+			:param max_length: integer The maximal length of entire A-MPDU Range: 50 to 131.071E+3, Unit: byte
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Enum, enums.EnableState), ArgSingle('multi_tid', multi_tid, DataType.Enum, enums.EnableState), ArgSingle('max_length', max_length, DataType.Integer))
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:AMPDu {param}'.rstrip())
 
 	# noinspection PyTypeChecker
-	class AllocationStruct(StructBase):
-		"""Structure for setting input parameters. Fields: \n
-			- Ch_20_Index: enums.Ch20Index: CHA1 | CHA2 | CHA3 | CHA4
-			- Ru_Index: enums.RuIndex: RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9"""
+	class AmpduStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Enable: enums.EnableState: DISable | ENABle Enables/ disables the A-MPDUs
+			- Multi_Tid: enums.EnableState: DISable | ENABle Enables/ disables multi-TID A-MPDU
+			- Max_Length: int: integer The maximal length of entire A-MPDU Range: 50 to 131.071E+3, Unit: byte"""
 		__meta_args_list = [
-			ArgStruct.scalar_enum('Ch_20_Index', enums.Ch20Index),
-			ArgStruct.scalar_enum('Ru_Index', enums.RuIndex)]
+			ArgStruct.scalar_enum('Enable', enums.EnableState),
+			ArgStruct.scalar_enum('Multi_Tid', enums.EnableState),
+			ArgStruct.scalar_int('Max_Length')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Ch_20_Index: enums.Ch20Index = None
-			self.Ru_Index: enums.RuIndex = None
-
-	def set(self, structure: AllocationStruct, station=repcap.Station.Default, user=repcap.User.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:ALLocation \n
-		Snippet: driver.configure.connection.sta.dframe.hemu.user.allocation.set(value = [PROPERTY_STRUCT_NAME](), station = repcap.Station.Default, user = repcap.User.Default) \n
-		Configures allocations for the user in HE MU PPDU. Maps the user to a resource unit (RU) . \n
-			:param structure: for set value, see the help for AllocationStruct structure arguments.
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:ALLocation', structure)
-
-	def get(self, station=repcap.Station.Default, user=repcap.User.Default) -> AllocationStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:ALLocation \n
-		Snippet: value: AllocationStruct = driver.configure.connection.sta.dframe.hemu.user.allocation.get(station = repcap.Station.Default, user = repcap.User.Default) \n
-		Configures allocations for the user in HE MU PPDU. Maps the user to a resource unit (RU) . \n
+			self.Enable: enums.EnableState = None
+			self.Multi_Tid: enums.EnableState = None
+			self.Max_Length: int = None
+
+	def get(self, station=repcap.Station.Default) -> AmpduStruct:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:AMPDu \n
+		Snippet: value: AmpduStruct = driver.configure.sta.connection.ampdu.get(station = repcap.Station.Default) \n
+		Configures aggregate MPDUs (A-MPDU) . \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
-			:return: structure: for return value, see the help for AllocationStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
-		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:ALLocation?', self.__class__.AllocationStruct())
+			:return: structure: for return value, see the help for AmpduStruct structure arguments."""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:AMPDu?', self.__class__.AmpduStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Ctype.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Ctype.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 from ........Internal.CommandsGroup import CommandsGroup
 from ........Internal import Conversions
 from ........ import enums
 from ........ import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Ctype:
-	"""Ctype commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class CtypeCls:
+	"""Ctype commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ctype", core, parent)
+		self._cmd_group = CommandsGroup("ctype", core, parent)
 
 	def set(self, coding_type: enums.CodingType, station=repcap.Station.Default, user=repcap.User.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:CTYPe \n
 		Snippet: driver.configure.connection.sta.dframe.hemu.user.ctype.set(coding_type = enums.CodingType.BCC, station = repcap.Station.Default, user = repcap.User.Default) \n
 		Selects the coding type related to a user for HE MU PPDU. \n
 			:param coding_type: LDPC | BCC
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')"""
+			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
+		"""
 		param = Conversions.enum_scalar_to_str(coding_type, enums.CodingType)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:CTYPe {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, station=repcap.Station.Default, user=repcap.User.Default) -> enums.CodingType:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:CTYPe \n
 		Snippet: value: enums.CodingType = driver.configure.connection.sta.dframe.hemu.user.ctype.get(station = repcap.Station.Default, user = repcap.User.Default) \n
 		Selects the coding type related to a user for HE MU PPDU. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
 			:return: coding_type: LDPC | BCC"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:CTYPe?')
 		return Conversions.str_to_scalar_enum(response, enums.CodingType)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Mcs.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Mcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-from ........Internal.Core import Core
-from ........Internal.CommandsGroup import CommandsGroup
-from ........Internal import Conversions
-from ........ import enums
-from ........ import repcap
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
+from ....... import enums
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mcs:
-	"""Mcs commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class McsCls:
+	"""Mcs commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mcs", core, parent)
+		self._cmd_group = CommandsGroup("mcs", core, parent)
 
-	def set(self, mcs_index: enums.McsIndex, station=repcap.Station.Default, user=repcap.User.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:MCS \n
-		Snippet: driver.configure.connection.sta.dframe.hemu.user.mcs.set(mcs_index = enums.McsIndex.MCS, station = repcap.Station.Default, user = repcap.User.Default) \n
+	def set(self, mcs_index: enums.McsIndex, user=repcap.User.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:MCS \n
+		Snippet: driver.configure.per.dframe.hemu.user.mcs.set(mcs_index = enums.McsIndex.MCS, user = repcap.User.Default) \n
 		Sets the modulation and coding scheme for user 1 (user data assigned to the DUT) . \n
-			:param mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0, MCS 1 to MCS 11
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')"""
+			:param mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11
+			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
+		"""
 		param = Conversions.enum_scalar_to_str(mcs_index, enums.McsIndex)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:MCS {param}')
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:MCS {param}')
 
 	# noinspection PyTypeChecker
-	def get(self, station=repcap.Station.Default, user=repcap.User.Default) -> enums.McsIndex:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:MCS \n
-		Snippet: value: enums.McsIndex = driver.configure.connection.sta.dframe.hemu.user.mcs.get(station = repcap.Station.Default, user = repcap.User.Default) \n
+	def get(self, user=repcap.User.Default) -> enums.McsIndex:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:MCS \n
+		Snippet: value: enums.McsIndex = driver.configure.per.dframe.hemu.user.mcs.get(user = repcap.User.Default) \n
 		Sets the modulation and coding scheme for user 1 (user data assigned to the DUT) . \n
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
-			:return: mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0, MCS 1 to MCS 11"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
-		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:MCS?')
+			:return: mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11"""
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
+		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:MCS?')
 		return Conversions.str_to_scalar_enum(response, enums.McsIndex)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Streams.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Streams.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 from ........Internal.CommandsGroup import CommandsGroup
 from ........Internal import Conversions
 from ........ import enums
 from ........ import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Streams:
-	"""Streams commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class StreamsCls:
+	"""Streams commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("streams", core, parent)
+		self._cmd_group = CommandsGroup("streams", core, parent)
 
 	def set(self, streams: enums.Streams, station=repcap.Station.Default, user=repcap.User.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:STReams \n
 		Snippet: driver.configure.connection.sta.dframe.hemu.user.streams.set(streams = enums.Streams.STR1, station = repcap.Station.Default, user = repcap.User.Default) \n
 		Sets the number of streams used by the user for MIMO connections. \n
 			:param streams: STR1 | STR2 One or two streams
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')"""
+			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
+		"""
 		param = Conversions.enum_scalar_to_str(streams, enums.Streams)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:STReams {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, station=repcap.Station.Default, user=repcap.User.Default) -> enums.Streams:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STA<s>:DFRame:HEMU:USER<index>:STReams \n
 		Snippet: value: enums.Streams = driver.configure.connection.sta.dframe.hemu.user.streams.get(station = repcap.Station.Default, user = repcap.User.Default) \n
 		Sets the number of streams used by the user for MIMO connections. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
 			:return: streams: STR1 | STR2 One or two streams"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:STA{station_cmd_val}:DFRame:HEMU:USER{user_cmd_val}:STReams?')
 		return Conversions.str_to_scalar_enum(response, enums.Streams)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Station.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Station.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Station:
-	"""Station commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class StationCls:
+	"""Station commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("station", core, parent)
+		self._cmd_group = CommandsGroup("station", core, parent)
 
 	# noinspection PyTypeChecker
 	def get_sconnection(self) -> enums.ConnectionAllowed:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:STATion:SCONnection \n
 		Snippet: value: enums.ConnectionAllowed = driver.configure.connection.station.get_sconnection() \n
 		Specifies to which access points the simulated station is allowed to connect (operation mode 'Station') . \n
 			:return: mode: ANY | SSID ANY: Any AP is allowed. SSID: Only a specific AP is allowed, identified by the configured SSID, see method RsCmwWlanSig.Configure.Connection.ssid.
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Connection_/Wdirect.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Ht.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,68 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from typing import List
+
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal.Types import DataType
+from ......Internal.StructBase import StructBase
+from ......Internal.ArgStruct import ArgStruct
+from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Wdirect:
-	"""Wdirect commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class HtCls:
+	"""Ht commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("wdirect", core, parent)
-
-	# noinspection PyTypeChecker
-	class AtypeStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Method: enums.AuthMethod: No parameter help available
-			- Mode: enums.AutoManualMode: No parameter help available
-			- Pin: str: No parameter help available"""
-		__meta_args_list = [
-			ArgStruct.scalar_enum('Method', enums.AuthMethod),
-			ArgStruct.scalar_enum('Mode', enums.AutoManualMode),
-			ArgStruct.scalar_str('Pin')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Method: enums.AuthMethod = None
-			self.Mode: enums.AutoManualMode = None
-			self.Pin: str = None
-
-	# noinspection PyTypeChecker
-	def get_atype(self) -> AtypeStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:WDIRect:ATYPe \n
-		Snippet: value: AtypeStruct = driver.configure.connection.wdirect.get_atype() \n
-		No command help available \n
-			:return: structure: for return value, see the help for AtypeStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:WDIRect:ATYPe?', self.__class__.AtypeStruct())
-
-	def set_atype(self, value: AtypeStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:WDIRect:ATYPe \n
-		Snippet: driver.configure.connection.wdirect.set_atype(value = AtypeStruct()) \n
-		No command help available \n
-			:param value: see the help for AtypeStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:WDIRect:ATYPe', value)
+		self._cmd_group = CommandsGroup("ht", core, parent)
 
 	# noinspection PyTypeChecker
-	class WdconfStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Manufacturer: str: No parameter help available
-			- Model_Name: str: No parameter help available
-			- Model_Number: str: No parameter help available
-			- Serial_Number: str: No parameter help available
-			- Device_Name: str: No parameter help available"""
+	class GetStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Rate: List[enums.DataRate]: No parameter help available
+			- Bw: List[enums.ChannelBandwidth]: No parameter help available
+			- Nss: List[enums.SpacialStreamsNr]: No parameter help available
+			- Frames_Curr: List[int]: No parameter help available
+			- Frames_Tot: List[int]: No parameter help available
+			- Bytes_Curr: List[float]: No parameter help available
+			- Bytes_Tot: List[float]: No parameter help available
+			- Mbps_Curr: List[float]: No parameter help available
+			- Mbps_Tot: List[float]: No parameter help available
+			- Power_Curr: List[float]: No parameter help available
+			- Power_Tot: List[float]: No parameter help available"""
 		__meta_args_list = [
-			ArgStruct.scalar_str('Manufacturer'),
-			ArgStruct.scalar_str('Model_Name'),
-			ArgStruct.scalar_str('Model_Number'),
-			ArgStruct.scalar_str('Serial_Number'),
-			ArgStruct.scalar_str('Device_Name')]
+			ArgStruct('Rate', DataType.EnumList, enums.DataRate, False, True, 1),
+			ArgStruct('Bw', DataType.EnumList, enums.ChannelBandwidth, False, True, 1),
+			ArgStruct('Nss', DataType.EnumList, enums.SpacialStreamsNr, False, True, 1),
+			ArgStruct('Frames_Curr', DataType.IntegerList, None, False, True, 1),
+			ArgStruct('Frames_Tot', DataType.IntegerList, None, False, True, 1),
+			ArgStruct('Bytes_Curr', DataType.FloatList, None, False, True, 1),
+			ArgStruct('Bytes_Tot', DataType.FloatList, None, False, True, 1),
+			ArgStruct('Mbps_Curr', DataType.FloatList, None, False, True, 1),
+			ArgStruct('Mbps_Tot', DataType.FloatList, None, False, True, 1),
+			ArgStruct('Power_Curr', DataType.FloatList, None, False, True, 1),
+			ArgStruct('Power_Tot', DataType.FloatList, None, False, True, 1)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Manufacturer: str = None
-			self.Model_Name: str = None
-			self.Model_Number: str = None
-			self.Serial_Number: str = None
-			self.Device_Name: str = None
-
-	def get_wdconf(self) -> WdconfStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:WDIRect:WDConf \n
-		Snippet: value: WdconfStruct = driver.configure.connection.wdirect.get_wdconf() \n
-		No command help available \n
-			:return: structure: for return value, see the help for WdconfStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:WDIRect:WDConf?', self.__class__.WdconfStruct())
-
-	def set_wdconf(self, value: WdconfStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:WDIRect:WDConf \n
-		Snippet: driver.configure.connection.wdirect.set_wdconf(value = WdconfStruct()) \n
+			self.Rate: List[enums.DataRate] = None
+			self.Bw: List[enums.ChannelBandwidth] = None
+			self.Nss: List[enums.SpacialStreamsNr] = None
+			self.Frames_Curr: List[int] = None
+			self.Frames_Tot: List[int] = None
+			self.Bytes_Curr: List[float] = None
+			self.Bytes_Tot: List[float] = None
+			self.Mbps_Curr: List[float] = None
+			self.Mbps_Tot: List[float] = None
+			self.Power_Curr: List[float] = None
+			self.Power_Tot: List[float] = None
+
+	def get(self, station=repcap.Station.Default) -> GetStruct:
+		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:HT \n
+		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.ht.get(station = repcap.Station.Default) \n
 		No command help available \n
-			:param value: see the help for WdconfStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:CONNection:WDIRect:WDConf', value)
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+			:return: structure: for return value, see the help for GetStruct structure arguments."""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:HT?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Edau.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Edau.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 from ...Internal import Conversions
 from ... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Edau:
-	"""Edau commands group definition. 3 total commands, 0 Sub-groups, 3 group commands"""
+class EdauCls:
+	"""Edau commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("edau", core, parent)
+		self._cmd_group = CommandsGroup("edau", core, parent)
 
 	def get_nid(self) -> int:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:EDAU:NID \n
 		Snippet: value: int = driver.configure.edau.get_nid() \n
 		Specifies the subnet node ID of the instrument where the external DAU is installed. \n
 			:return: node_id: integer Range: 1 to 254
 		"""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/DuIp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal.StructBase import StructBase
-from ...Internal.ArgStruct import ArgStruct
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Types import DataType
+from ....Internal.StructBase import StructBase
+from ....Internal.ArgStruct import ArgStruct
+from ....Internal.ArgSingleList import ArgSingleList
+from ....Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Etoe:
-	"""Etoe commands group definition. 2 total commands, 1 Sub-groups, 1 group commands"""
+class DuIpCls:
+	"""DuIp commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("etoe", core, parent)
+		self._cmd_group = CommandsGroup("duIp", core, parent)
 
-	@property
-	def irList(self):
-		"""irList commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_irList'):
-			from .Etoe_.IrList import IrList
-			self._irList = IrList(self._core, self._base)
-		return self._irList
+	def set(self, state: bool, first_number: int, sec_number: int, third_number: int, fourth_number: int) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:ETOE:DUIP \n
+		Snippet: driver.configure.etoe.duIp.set(state = False, first_number = 1, sec_number = 1, third_number = 1, fourth_number = 1) \n
+		Allows you to specify the IPv4 address that the DAU assigns to the DUT via DHCP. \n
+			:param state: OFF | ON Disables/enables the IP address configuration
+			:param first_number: No help available
+			:param sec_number: No help available
+			:param third_number: No help available
+			:param fourth_number: No help available
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('state', state, DataType.Boolean), ArgSingle('first_number', first_number, DataType.Integer), ArgSingle('sec_number', sec_number, DataType.Integer), ArgSingle('third_number', third_number, DataType.Integer), ArgSingle('fourth_number', fourth_number, DataType.Integer))
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:ETOE:DUIP {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class DuIpStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- State: bool: OFF | ON Disables/enables the IP address configuration
 			- First_Number: int: No parameter help available
 			- Sec_Number: int: No parameter help available
 			- Third_Number: int: No parameter help available
 			- Fourth_Number: int: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('State'),
@@ -39,30 +47,13 @@
 			StructBase.__init__(self, self)
 			self.State: bool = None
 			self.First_Number: int = None
 			self.Sec_Number: int = None
 			self.Third_Number: int = None
 			self.Fourth_Number: int = None
 
-	def get_du_ip(self) -> DuIpStruct:
+	def get(self) -> DuIpStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:ETOE:DUIP \n
-		Snippet: value: DuIpStruct = driver.configure.etoe.get_du_ip() \n
+		Snippet: value: DuIpStruct = driver.configure.etoe.duIp.get() \n
 		Allows you to specify the IPv4 address that the DAU assigns to the DUT via DHCP. \n
-			:return: structure: for return value, see the help for DuIpStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:ETOE:DUIP?', self.__class__.DuIpStruct())
-
-	def set_du_ip(self, value: DuIpStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:ETOE:DUIP \n
-		Snippet: driver.configure.etoe.set_du_ip(value = DuIpStruct()) \n
-		Allows you to specify the IPv4 address that the DAU assigns to the DUT via DHCP. \n
-			:param value: see the help for DuIpStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:ETOE:DUIP', value)
-
-	def clone(self) -> 'Etoe':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
-		Also copies all the existing default Repeated Capabilities setting,
-		which you can change independently without affecting the original group"""
-		new_group = Etoe(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
-		return new_group
+			:return: structure: for return value, see the help for DuIpStruct structure arguments."""
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:ETOE:DUIP?', self.__class__.DuIpStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/IrList/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IrList:
-	"""IrList commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class IrListCls:
+	"""IrList commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("irList", core, parent)
+		self._cmd_group = CommandsGroup("irList", core, parent)
 
 	@property
 	def iprAddress(self):
 		"""iprAddress commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_iprAddress'):
-			from .IrList_.IprAddress import IprAddress
-			self._iprAddress = IprAddress(self._core, self._base)
+			from .IprAddress import IprAddressCls
+			self._iprAddress = IprAddressCls(self._core, self._cmd_group)
 		return self._iprAddress
 
-	def clone(self) -> 'IrList':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'IrListCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = IrList(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = IrListCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList_/IprAddress.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/IrList/IprAddress.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
 from .....Internal.RepeatedCapability import RepeatedCapability
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IprAddress:
-	"""IprAddress commands group definition. 1 total commands, 0 Sub-groups, 1 group commands
+class IprAddressCls:
+	"""IprAddress commands group definition. 1 total commands, 0 Subgroups, 1 group commands
 	Repeated Capability: IpRouteAddress, default value after init: IpRouteAddress.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("iprAddress", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_ipRouteAddress_get', 'repcap_ipRouteAddress_set', repcap.IpRouteAddress.Nr1)
+		self._cmd_group = CommandsGroup("iprAddress", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_ipRouteAddress_get', 'repcap_ipRouteAddress_set', repcap.IpRouteAddress.Nr1)
 
-	def repcap_ipRouteAddress_set(self, enum_value: repcap.IpRouteAddress) -> None:
+	def repcap_ipRouteAddress_set(self, ipRouteAddress: repcap.IpRouteAddress) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to IpRouteAddress.Default
 		Default value after init: IpRouteAddress.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(ipRouteAddress)
 
 	def repcap_ipRouteAddress_get(self) -> repcap.IpRouteAddress:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	# noinspection PyTypeChecker
 	class IprAddressStruct(StructBase):
 		"""Structure for setting input parameters. Fields: \n
 			- State: bool: OFF | ON Entry disabled or enabled
 			- Ip_41: int: integer First octet of the IPv4 destination address Range: 0 to 255
 			- Ip_42: int: integer Second octet Range: 0 to 255
@@ -57,32 +57,43 @@
 			self.Ip_44: int = None
 			self.Ip_4_Netmask: int = None
 			self.Ip_6_Prefix: str = None
 			self.Ip_6_Netmask: int = None
 
 	def set(self, structure: IprAddressStruct, ipRouteAddress=repcap.IpRouteAddress.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:ETOE:IRList:IPRaddress<n> \n
-		Snippet: driver.configure.etoe.irList.iprAddress.set(value = [PROPERTY_STRUCT_NAME](), ipRouteAddress = repcap.IpRouteAddress.Default) \n
+		Snippet with structure: \n
+		structure = driver.configure.etoe.irList.iprAddress.IprAddressStruct() \n
+		structure.State: bool = False \n
+		structure.Ip_41: int = 1 \n
+		structure.Ip_42: int = 1 \n
+		structure.Ip_43: int = 1 \n
+		structure.Ip_44: int = 1 \n
+		structure.Ip_4_Netmask: int = 1 \n
+		structure.Ip_6_Prefix: str = 'abc' \n
+		structure.Ip_6_Netmask: int = 1 \n
+		driver.configure.etoe.irList.iprAddress.set(structure, ipRouteAddress = repcap.IpRouteAddress.Default) \n
 		Configures an entry of the routes list. The routes list defines destination addresses for which the DAU routes packets to
 		the DUT. \n
 			:param structure: for set value, see the help for IprAddressStruct structure arguments.
-			:param ipRouteAddress: optional repeated capability selector. Default value: Nr1 (settable in the interface 'IprAddress')"""
-		ipRouteAddress_cmd_val = self._base.get_repcap_cmd_value(ipRouteAddress, repcap.IpRouteAddress)
+			:param ipRouteAddress: optional repeated capability selector. Default value: Nr1 (settable in the interface 'IprAddress')
+		"""
+		ipRouteAddress_cmd_val = self._cmd_group.get_repcap_cmd_value(ipRouteAddress, repcap.IpRouteAddress)
 		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:ETOE:IRList:IPRaddress{ipRouteAddress_cmd_val}', structure)
 
 	def get(self, ipRouteAddress=repcap.IpRouteAddress.Default) -> IprAddressStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:ETOE:IRList:IPRaddress<n> \n
 		Snippet: value: IprAddressStruct = driver.configure.etoe.irList.iprAddress.get(ipRouteAddress = repcap.IpRouteAddress.Default) \n
 		Configures an entry of the routes list. The routes list defines destination addresses for which the DAU routes packets to
 		the DUT. \n
 			:param ipRouteAddress: optional repeated capability selector. Default value: Nr1 (settable in the interface 'IprAddress')
 			:return: structure: for return value, see the help for IprAddressStruct structure arguments."""
-		ipRouteAddress_cmd_val = self._base.get_repcap_cmd_value(ipRouteAddress, repcap.IpRouteAddress)
+		ipRouteAddress_cmd_val = self._cmd_group.get_repcap_cmd_value(ipRouteAddress, repcap.IpRouteAddress)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:ETOE:IRList:IPRaddress{ipRouteAddress_cmd_val}?', self.__class__.IprAddressStruct())
 
-	def clone(self) -> 'IprAddress':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'IprAddressCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = IprAddress(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = IprAddressCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,51 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Fading:
-	"""Fading commands group definition. 6 total commands, 2 Sub-groups, 0 group commands"""
+class ConnectionCls:
+	"""Connection commands group definition. 13 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("fading", core, parent)
+		self._cmd_group = CommandsGroup("connection", core, parent)
 
 	@property
-	def fsimulator(self):
-		"""fsimulator commands group. 1 Sub-classes, 2 commands."""
-		if not hasattr(self, '_fsimulator'):
-			from .Fading_.Fsimulator import Fsimulator
-			self._fsimulator = Fsimulator(self._core, self._base)
-		return self._fsimulator
+	def qos(self):
+		"""qos commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_qos'):
+			from .Qos import QosCls
+			self._qos = QosCls(self._core, self._cmd_group)
+		return self._qos
 
 	@property
-	def awgn(self):
-		"""awgn commands group. 1 Sub-classes, 2 commands."""
-		if not hasattr(self, '_awgn'):
-			from .Fading_.Awgn import Awgn
-			self._awgn = Awgn(self._core, self._base)
-		return self._awgn
+	def dfdef(self):
+		"""dfdef commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_dfdef'):
+			from .Dfdef import DfdefCls
+			self._dfdef = DfdefCls(self._core, self._cmd_group)
+		return self._dfdef
 
-	def clone(self) -> 'Fading':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def hetf(self):
+		"""hetf commands group. 9 Sub-classes, 0 commands."""
+		if not hasattr(self, '_hetf'):
+			from .Hetf import HetfCls
+			self._hetf = HetfCls(self._core, self._cmd_group)
+		return self._hetf
+
+	@property
+	def ampdu(self):
+		"""ampdu commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ampdu'):
+			from .Ampdu import AmpduCls
+			self._ampdu = AmpduCls(self._core, self._cmd_group)
+		return self._ampdu
+
+	def clone(self) -> 'ConnectionCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Fading(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = ConnectionCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Awgn/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Awgn:
-	"""Awgn commands group definition. 3 total commands, 1 Sub-groups, 2 group commands"""
+class AwgnCls:
+	"""Awgn commands group definition. 3 total commands, 1 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("awgn", core, parent)
+		self._cmd_group = CommandsGroup("awgn", core, parent)
 
 	@property
 	def bandwidth(self):
 		"""bandwidth commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_bandwidth'):
-			from .Awgn_.Bandwidth import Bandwidth
-			self._bandwidth = Bandwidth(self._core, self._base)
+			from .Bandwidth import BandwidthCls
+			self._bandwidth = BandwidthCls(self._core, self._cmd_group)
 		return self._bandwidth
 
 	def get_enable(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:FADing:AWGN:ENABle \n
 		Snippet: value: bool = driver.configure.fading.awgn.get_enable() \n
 		Enables or disables AWGN insertion via the fading module. \n
 			:return: enable: OFF | ON
@@ -51,14 +51,14 @@
 		Snippet: driver.configure.fading.awgn.set_sn_ratio(ratio = 1.0) \n
 		Specifies the signal to noise ratio for the AWGN inserted on the internal fading module. \n
 			:param ratio: numeric Range: 0 dB to 40 dB, Unit: dB
 		"""
 		param = Conversions.decimal_value_to_str(ratio)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:FADing:AWGN:SNRatio {param}')
 
-	def clone(self) -> 'Awgn':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'AwgnCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Awgn(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = AwgnCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn_/Bandwidth.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Awgn/Bandwidth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Bandwidth:
-	"""Bandwidth commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class BandwidthCls:
+	"""Bandwidth commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("bandwidth", core, parent)
+		self._cmd_group = CommandsGroup("bandwidth", core, parent)
 
 	def get_ratio(self) -> float:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:FADing:AWGN:BWIDth:RATio \n
 		Snippet: value: float = driver.configure.fading.awgn.bandwidth.get_ratio() \n
 		Specifies the minimum ratio between the noise bandwidth and the channel bandwidth. \n
 			:return: ratio: numeric Range: 1 to 1000
 		"""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Fsimulator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Fsimulator:
-	"""Fsimulator commands group definition. 3 total commands, 1 Sub-groups, 2 group commands"""
+class FsimulatorCls:
+	"""Fsimulator commands group definition. 3 total commands, 1 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("fsimulator", core, parent)
+		self._cmd_group = CommandsGroup("fsimulator", core, parent)
 
 	@property
 	def iloss(self):
 		"""iloss commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_iloss'):
-			from .Fsimulator_.Iloss import Iloss
-			self._iloss = Iloss(self._core, self._base)
+			from .Iloss import IlossCls
+			self._iloss = IlossCls(self._core, self._cmd_group)
 		return self._iloss
 
 	# noinspection PyTypeChecker
 	def get_standard(self) -> enums.Profile:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:FADing:FSIMulator:STANdard \n
 		Snippet: value: enums.Profile = driver.configure.fading.fsimulator.get_standard() \n
-		Selects a propagation condition profile for fading, see 'Predefined Fading Settings'. \n
+		Selects a propagation condition profile for fading, see 'Predefined fading settings'. \n
 			:return: profile: MODA | MODB | MODC | MODD | MODE | MODF Mode A to F
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:FADing:FSIMulator:STANdard?')
 		return Conversions.str_to_scalar_enum(response, enums.Profile)
 
 	def set_standard(self, profile: enums.Profile) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:FADing:FSIMulator:STANdard \n
 		Snippet: driver.configure.fading.fsimulator.set_standard(profile = enums.Profile.MODA) \n
-		Selects a propagation condition profile for fading, see 'Predefined Fading Settings'. \n
+		Selects a propagation condition profile for fading, see 'Predefined fading settings'. \n
 			:param profile: MODA | MODB | MODC | MODD | MODE | MODF Mode A to F
 		"""
 		param = Conversions.enum_scalar_to_str(profile, enums.Profile)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:FADing:FSIMulator:STANdard {param}')
 
 	def get_enable(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:FADing:FSIMulator:ENABle \n
@@ -53,14 +53,14 @@
 		Snippet: driver.configure.fading.fsimulator.set_enable(enable = False) \n
 		Enables/disables the fading simulator. \n
 			:param enable: OFF | ON
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:FADing:FSIMulator:ENABle {param}')
 
-	def clone(self) -> 'Fsimulator':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'FsimulatorCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Fsimulator(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = FsimulatorCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator_/Iloss.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/Fsimulator/Iloss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Iloss:
-	"""Iloss commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class IlossCls:
+	"""Iloss commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("iloss", core, parent)
+		self._cmd_group = CommandsGroup("iloss", core, parent)
 
 	def get_loss(self) -> float:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:FADing:FSIMulator:ILOSs:LOSS \n
 		Snippet: value: float = driver.configure.fading.fsimulator.iloss.get_loss() \n
 		Sets the insertion loss for the fading simulator. \n
 			:return: insertion_loss: float Range: -3.02 dB to 30 dB, Unit: dB
 		"""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/HetBased.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/HetBased.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 from ...Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class HetBased:
-	"""HetBased commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class HetBasedCls:
+	"""HetBased commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hetBased", core, parent)
+		self._cmd_group = CommandsGroup("hetBased", core, parent)
 
 	def get_frames(self) -> int:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:HETBased:FRAMes \n
 		Snippet: value: int = driver.configure.hetBased.get_frames() \n
 		Sets the number of frames for HE TB list mode measurements. This setting determines the statistic count of the
 		measurement. \n
 			:return: no_of_frames: integer Range: 1 to 2000
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal import Conversions
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IpvFour:
-	"""IpvFour commands group definition. 8 total commands, 1 Sub-groups, 1 group commands"""
+class IpvFourCls:
+	"""IpvFour commands group definition. 8 total commands, 1 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ipvFour", core, parent)
+		self._cmd_group = CommandsGroup("ipvFour", core, parent)
 
 	@property
 	def static(self):
-		"""static commands group. 1 Sub-classes, 1 commands."""
+		"""static commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_static'):
-			from .IpvFour_.Static import Static
-			self._static = Static(self._core, self._base)
+			from .Static import StaticCls
+			self._static = StaticCls(self._core, self._cmd_group)
 		return self._static
 
 	def get_dhcp(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVFour:DHCP \n
 		Snippet: value: bool = driver.configure.ipvFour.get_dhcp() \n
 		Enables or disables the built-in DHCP server. The setting is relevant for station mode, with or without a DAU.
 		This setting is not relevant for AP mode. \n
@@ -35,14 +35,14 @@
 		Enables or disables the built-in DHCP server. The setting is relevant for station mode, with or without a DAU.
 		This setting is not relevant for AP mode. \n
 			:param activate: OFF | ON
 		"""
 		param = Conversions.bool_to_str(activate)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:IPVFour:DHCP {param}')
 
-	def clone(self) -> 'IpvFour':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'IpvFourCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = IpvFour(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = IpvFourCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Association/Sta/MacReserve.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,53 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from ....Internal.RepeatedCapability import RepeatedCapability
-from .... import repcap
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal.Types import DataType
+from ......Internal.StructBase import StructBase
+from ......Internal.ArgStruct import ArgStruct
+from ......Internal.ArgSingleList import ArgSingleList
+from ......Internal.ArgSingle import ArgSingle
+from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Static:
-	"""Static commands group definition. 7 total commands, 1 Sub-groups, 1 group commands
-	Repeated Capability: Station, default value after init: Station.Nr1"""
+class MacReserveCls:
+	"""MacReserve commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("static", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
+		self._cmd_group = CommandsGroup("macReserve", core, parent)
 
-	def repcap_station_set(self, enum_value: repcap.Station) -> None:
-		"""Repeated Capability default value numeric suffix.
-		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Station.Default
-		Default value after init: Station.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
-
-	def repcap_station_get(self) -> repcap.Station:
-		"""Returns the current default repeated capability for the child set/get methods"""
-		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
-
-	@property
-	def ipAddress(self):
-		"""ipAddress commands group. 1 Sub-classes, 5 commands."""
-		if not hasattr(self, '_ipAddress'):
-			from .Static_.IpAddress import IpAddress
-			self._ipAddress = IpAddress(self._core, self._base)
-		return self._ipAddress
+	def set(self, reservation: enums.Reservation, address: str = None, station=repcap.Station.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:ASSociation:STA<s>:MACReserve \n
+		Snippet: driver.configure.connection.association.sta.macReserve.set(reservation = enums.Reservation.ANY, address = 'abc', station = repcap.Station.Default) \n
+		Configures three slots available for STAs, if method RsCmwWlanSig.Configure.Connection.mstation is set to ON \n
+			:param reservation: ANY | SET | OFF ANY - the slot is available to a STA of any MAC address SET - reserves the slot for a particular MAC address OFF - the slot is disabled
+			:param address: string MAC address of the DUT for Reservation = SET
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('reservation', reservation, DataType.Enum, enums.Reservation), ArgSingle('address', address, DataType.String, None, is_optional=True))
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:ASSociation:STA{station_cmd_val}:MACReserve {param}'.rstrip())
 
 	# noinspection PyTypeChecker
-	class SmaskStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- First_Octet: int: No parameter help available
-			- Second_Octet: int: No parameter help available
-			- Third_Octet: int: No parameter help available
-			- Fourth_Octet: int: No parameter help available"""
+	class MacReserveStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Reservation: enums.Reservation: ANY | SET | OFF ANY - the slot is available to a STA of any MAC address SET - reserves the slot for a particular MAC address OFF - the slot is disabled
+			- Address: str: string MAC address of the DUT for Reservation = SET"""
 		__meta_args_list = [
-			ArgStruct.scalar_int('First_Octet'),
-			ArgStruct.scalar_int('Second_Octet'),
-			ArgStruct.scalar_int('Third_Octet'),
-			ArgStruct.scalar_int('Fourth_Octet')]
+			ArgStruct.scalar_enum('Reservation', enums.Reservation),
+			ArgStruct.scalar_str('Address')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.First_Octet: int = None
-			self.Second_Octet: int = None
-			self.Third_Octet: int = None
-			self.Fourth_Octet: int = None
-
-	def get_smask(self) -> SmaskStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVFour:STATic:SMASk \n
-		Snippet: value: SmaskStruct = driver.configure.ipvFour.static.get_smask() \n
-		Specifies the subnet mask of the built-in IPv4 stack. The setting is relevant for instruments without DAU. \n
-			:return: structure: for return value, see the help for SmaskStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:IPVFour:STATic:SMASk?', self.__class__.SmaskStruct())
-
-	def set_smask(self, value: SmaskStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVFour:STATic:SMASk \n
-		Snippet: driver.configure.ipvFour.static.set_smask(value = SmaskStruct()) \n
-		Specifies the subnet mask of the built-in IPv4 stack. The setting is relevant for instruments without DAU. \n
-			:param value: see the help for SmaskStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:IPVFour:STATic:SMASk', value)
+			self.Reservation: enums.Reservation = None
+			self.Address: str = None
 
-	def clone(self) -> 'Static':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
-		Also copies all the existing default Repeated Capabilities setting,
-		which you can change independently without affecting the original group"""
-		new_group = Static(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
-		return new_group
+	def get(self, station=repcap.Station.Default) -> MacReserveStruct:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:ASSociation:STA<s>:MACReserve \n
+		Snippet: value: MacReserveStruct = driver.configure.connection.association.sta.macReserve.get(station = repcap.Station.Default) \n
+		Configures three slots available for STAs, if method RsCmwWlanSig.Configure.Connection.mstation is set to ON \n
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+			:return: structure: for return value, see the help for MacReserveStruct structure arguments."""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:ASSociation:STA{station_cmd_val}:MACReserve?', self.__class__.MacReserveStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/IpAddress_/Sta.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Dns.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal.Types import DataType
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
-from ...... import repcap
+from ......Internal.ArgSingleList import ArgSingleList
+from ......Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sta:
-	"""Sta commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class DnsCls:
+	"""Dns commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sta", core, parent)
+		self._cmd_group = CommandsGroup("dns", core, parent)
+
+	def set(self, first: int, sec: int, third: int, fourth: int) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVFour:STATic:IPADdress:DNS \n
+		Snippet: driver.configure.ipvFour.static.ipAddress.dns.set(first = 1, sec = 1, third = 1, fourth = 1) \n
+		Provides the IPv4 address of a DNS server to the built-in IPv4 stack. The setting is relevant for instruments without DAU. \n
+			:param first: No help available
+			:param sec: No help available
+			:param third: No help available
+			:param fourth: No help available
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('first', first, DataType.Integer), ArgSingle('sec', sec, DataType.Integer), ArgSingle('third', third, DataType.Integer), ArgSingle('fourth', fourth, DataType.Integer))
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:IPVFour:STATic:IPADdress:DNS {param}'.rstrip())
 
 	# noinspection PyTypeChecker
-	class StaStruct(StructBase):
-		"""Structure for setting input parameters. Fields: \n
-			- First_Number: int: No parameter help available
-			- Sec_Number: int: No parameter help available
-			- Third_Number: int: No parameter help available
-			- Fourth_Number: int: No parameter help available"""
+	class DnsStruct(StructBase):
+		"""Response structure. Fields: \n
+			- First: int: No parameter help available
+			- Sec: int: No parameter help available
+			- Third: int: No parameter help available
+			- Fourth: int: No parameter help available"""
 		__meta_args_list = [
-			ArgStruct.scalar_int('First_Number'),
-			ArgStruct.scalar_int('Sec_Number'),
-			ArgStruct.scalar_int('Third_Number'),
-			ArgStruct.scalar_int('Fourth_Number')]
+			ArgStruct.scalar_int('First'),
+			ArgStruct.scalar_int('Sec'),
+			ArgStruct.scalar_int('Third'),
+			ArgStruct.scalar_int('Fourth')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.First_Number: int = None
-			self.Sec_Number: int = None
-			self.Third_Number: int = None
-			self.Fourth_Number: int = None
-
-	def set(self, structure: StaStruct, station=repcap.Station.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVFour:STATic:IPADdress:STA<s> \n
-		Snippet: driver.configure.ipvFour.static.ipAddress.sta.set(value = [PROPERTY_STRUCT_NAME](), station = repcap.Station.Default) \n
-		Defines the static IP V4 address of the DUT. The setting is only relevant for access point and instruments without a DAU. \n
-			:param structure: for set value, see the help for StaStruct structure arguments.
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Static')"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:IPVFour:STATic:IPADdress:STA{station_cmd_val}', structure)
-
-	def get(self, station=repcap.Station.Default) -> StaStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVFour:STATic:IPADdress:STA<s> \n
-		Snippet: value: StaStruct = driver.configure.ipvFour.static.ipAddress.sta.get(station = repcap.Station.Default) \n
-		Defines the static IP V4 address of the DUT. The setting is only relevant for access point and instruments without a DAU. \n
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Static')
-			:return: structure: for return value, see the help for StaStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:IPVFour:STATic:IPADdress:STA{station_cmd_val}?', self.__class__.StaStruct())
+			self.First: int = None
+			self.Sec: int = None
+			self.Third: int = None
+			self.Fourth: int = None
+
+	def get(self) -> DnsStruct:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVFour:STATic:IPADdress:DNS \n
+		Snippet: value: DnsStruct = driver.configure.ipvFour.static.ipAddress.dns.get() \n
+		Provides the IPv4 address of a DNS server to the built-in IPv4 stack. The setting is relevant for instruments without DAU. \n
+			:return: structure: for return value, see the help for DnsStruct structure arguments."""
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:IPVFour:STATic:IPADdress:DNS?', self.__class__.DnsStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/IpvSix.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvSix.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 from ...Internal import Conversions
 from ...Internal.Utilities import trim_str_response
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IpvSix:
-	"""IpvSix commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class IpvSixCls:
+	"""IpvSix commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ipvSix", core, parent)
+		self._cmd_group = CommandsGroup("ipvSix", core, parent)
 
 	def get_prefix(self) -> str:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVSix:PREFix \n
 		Snippet: value: str = driver.configure.ipvSix.get_prefix() \n
 		Defines the IPv6 prefix of the built-in IPv6 stack. \n
 			:return: prefix: string IPv6 prefix as string
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:IPVSix:PREFix?')
 		return trim_str_response(response)
 
 	def set_prefix(self, prefix: str) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:IPVSix:PREFix \n
-		Snippet: driver.configure.ipvSix.set_prefix(prefix = '1') \n
+		Snippet: driver.configure.ipvSix.set_prefix(prefix = 'abc') \n
 		Defines the IPv6 prefix of the built-in IPv6 stack. \n
 			:param prefix: string IPv6 prefix as string
 		"""
 		param = Conversions.value_to_quoted_str(prefix)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:IPVSix:PREFix {param}')
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Mimo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mimo/Tcsd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,47 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal import Conversions
-from ...Internal.StructBase import StructBase
-from ...Internal.ArgStruct import ArgStruct
-from ... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Types import DataType
+from ....Internal.StructBase import StructBase
+from ....Internal.ArgStruct import ArgStruct
+from ....Internal.ArgSingleList import ArgSingleList
+from ....Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mimo:
-	"""Mimo commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class TcsdCls:
+	"""Tcsd commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mimo", core, parent)
+		self._cmd_group = CommandsGroup("tcsd", core, parent)
 
-	# noinspection PyTypeChecker
-	def get_tm_mode(self) -> enums.MimoMode:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:MIMO:TMMode \n
-		Snippet: value: enums.MimoMode = driver.configure.mimo.get_tm_mode() \n
-		Selects the transmission mode for MIMO connections. This command supports only spatial multiplexing and space time block
-		coding (STBC) . In addition, to enable STBC in a particular data frame, use the commands: method RsCmwWlanSig.Configure.
-		Sta.Connection.Dfdef.set or method RsCmwWlanSig.Configure.Per.fdef \n
-			:return: mode: STBC | SMULtiplexin
-		"""
-		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:MIMO:TMMode?')
-		return Conversions.str_to_scalar_enum(response, enums.MimoMode)
-
-	def set_tm_mode(self, mode: enums.MimoMode) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:MIMO:TMMode \n
-		Snippet: driver.configure.mimo.set_tm_mode(mode = enums.MimoMode.SMULtiplexin) \n
-		Selects the transmission mode for MIMO connections. This command supports only spatial multiplexing and space time block
-		coding (STBC) . In addition, to enable STBC in a particular data frame, use the commands: method RsCmwWlanSig.Configure.
-		Sta.Connection.Dfdef.set or method RsCmwWlanSig.Configure.Per.fdef \n
-			:param mode: STBC | SMULtiplexin
+	def set(self, csd_1: int, csd_2: int) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:MIMO:TCSD \n
+		Snippet: driver.configure.mimo.tcsd.set(csd_1 = 1, csd_2 = 1) \n
+		No command help available \n
+			:param csd_1: No help available
+			:param csd_2: No help available
 		"""
-		param = Conversions.enum_scalar_to_str(mode, enums.MimoMode)
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:MIMO:TMMode {param}')
+		param = ArgSingleList().compose_cmd_string(ArgSingle('csd_1', csd_1, DataType.Integer), ArgSingle('csd_2', csd_2, DataType.Integer))
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:MIMO:TCSD {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class TcsdStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- Csd_1: int: No parameter help available
 			- Csd_2: int: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Csd_1'),
 			ArgStruct.scalar_int('Csd_2')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Csd_1: int = None
 			self.Csd_2: int = None
 
-	def get_tcsd(self) -> TcsdStruct:
+	def get(self) -> TcsdStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:MIMO:TCSD \n
-		Snippet: value: TcsdStruct = driver.configure.mimo.get_tcsd() \n
+		Snippet: value: TcsdStruct = driver.configure.mimo.tcsd.get() \n
 		No command help available \n
-			:return: structure: for return value, see the help for TcsdStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:MIMO:TCSD?', self.__class__.TcsdStruct())
-
-	def set_tcsd(self, value: TcsdStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:MIMO:TCSD \n
-		Snippet: driver.configure.mimo.set_tcsd(value = TcsdStruct()) \n
-		No command help available \n
-			:param value: see the help for TcsdStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:MIMO:TCSD', value)
+			:return: structure: for return value, see the help for TcsdStruct structure arguments."""
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:MIMO:TCSD?', self.__class__.TcsdStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Mmonitor.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mmonitor/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal import Conversions
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mmonitor:
-	"""Mmonitor commands group definition. 2 total commands, 1 Sub-groups, 1 group commands"""
+class MmonitorCls:
+	"""Mmonitor commands group definition. 2 total commands, 1 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mmonitor", core, parent)
+		self._cmd_group = CommandsGroup("mmonitor", core, parent)
 
 	@property
 	def ipAddress(self):
 		"""ipAddress commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ipAddress'):
-			from .Mmonitor_.IpAddress import IpAddress
-			self._ipAddress = IpAddress(self._core, self._base)
+			from .IpAddress import IpAddressCls
+			self._ipAddress = IpAddressCls(self._core, self._cmd_group)
 		return self._ipAddress
 
 	def get_enable(self) -> bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:MMONitor:ENABle \n
 		Snippet: value: bool = driver.configure.mmonitor.get_enable() \n
 		Enables or disables message monitoring for the WLAN signaling application. \n
 			:return: enable: OFF | ON
@@ -33,14 +33,14 @@
 		Snippet: driver.configure.mmonitor.set_enable(enable = False) \n
 		Enables or disables message monitoring for the WLAN signaling application. \n
 			:param enable: OFF | ON
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:MMONitor:ENABle {param}')
 
-	def clone(self) -> 'Mmonitor':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MmonitorCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Mmonitor(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MmonitorCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Mmonitor_/IpAddress.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Mmonitor/IpAddress.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from ....Internal import Conversions
 from ....Internal.StructBase import StructBase
 from ....Internal.ArgStruct import ArgStruct
 from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IpAddress:
-	"""IpAddress commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class IpAddressCls:
+	"""IpAddress commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ipAddress", core, parent)
+		self._cmd_group = CommandsGroup("ipAddress", core, parent)
 
 	def set(self, index: enums.IpAddrIndex) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:MMONitor:IPADdress \n
 		Snippet: driver.configure.mmonitor.ipAddress.set(index = enums.IpAddrIndex.IP1) \n
 		Selects the IP address to which signaling messages are sent for message monitoring. The address pool is configured
 		globally via CONFigure:BASE:MMONitor:IPADdress<n>. A query returns both the current index and the resulting IP address. \n
 			:param index: IP1 | IP2 | IP3 Address pool index
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,96 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal import Conversions
-from ...Internal.StructBase import StructBase
-from ...Internal.ArgStruct import ArgStruct
-from ... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
+from ....Internal.StructBase import StructBase
+from ....Internal.ArgStruct import ArgStruct
+from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Per:
-	"""Per commands group definition. 17 total commands, 2 Sub-groups, 8 group commands"""
+class PerCls:
+	"""Per commands group definition. 17 total commands, 2 Subgroups, 8 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("per", core, parent)
+		self._cmd_group = CommandsGroup("per", core, parent)
 
 	@property
 	def dframe(self):
 		"""dframe commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_dframe'):
-			from .Per_.Dframe import Dframe
-			self._dframe = Dframe(self._core, self._base)
+			from .Dframe import DframeCls
+			self._dframe = DframeCls(self._core, self._cmd_group)
 		return self._dframe
 
 	@property
 	def payload(self):
 		"""payload commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_payload'):
-			from .Per_.Payload import Payload
-			self._payload = Payload(self._core, self._base)
+			from .Payload import PayloadCls
+			self._payload = PayloadCls(self._core, self._cmd_group)
 		return self._payload
 
 	# noinspection PyTypeChecker
-	class FdefStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+	class FdefStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
+		"""Structure for setting input parameters. Contains optional set arguments. Fields: \n
 			- Format_Py: enums.DataFormatExt: NHT | HTM | VHT | HES | HEM Selects the frame format NHT: non-high throughput format (non-HT) HTM: HT mixed format (HT MF) VHT: very high throughput format HES: high efficiency single-user format (HE SU) HEM: high efficiency multi-user format (HE MU)
-			- Bandwidth: enums.ChannelBandwidthDut: BW20 | BW40 | BW80 | BW160 Channel bandwidth The value must not exceed the operating channel bandwidth, see [CMDLINK: CONFigure:WLAN:SIGNi:RFSettings:OCWidth CMDLINK].
-			- Coderate: enums.Coderate: BR12 | QR12 | QR34 | Q1M12 | Q1M34 | Q6M23 | Q6M34 | BR34 | MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | D1MBit | D2MBits | C55Mbits | C11Mbits | MCS8 | MCS9 | MCS10 | MCS11 | MCS12 | MCS13 | MCS14 | MCS15 See rate list in [CMDLINK: CONFigure:WLAN:SIGNi:CONNection:MFDef CMDLINK]
-			- Guard_Interval: enums.GuardInterval: LONG | SHORt | GI08 | GI16 | GI32 SHORt, LONG: short or long guard interval (up to 802.11ac) GI08, GI16, GI32: 0.8 μs, 1.6 μs, and 3.2 μs guard interval durations (for 802.11ax)
-			- Ltf_Type: enums.LtfType: X1 | X2 | X4 1x HE-LTF, 2x HE-LTF, 4x HE-LTF for 802.11ax
-			- Pe_Duration: enums.PeDuration: PE0 | PE4 | PE8 | PE12 | PE16 | AUTO PEx: additional receive processing time of x μs signaled in packet extension (PE) field (only for 802.11ax) AUTO: automatic setting based on the reported DUTs capabilities
-			- Ctype: enums.CodingType: LDPC | BCC Coding type (for 802.11ax - VHT, HE_SU, HE_MU frames only) : low density parity check or binary convolution code
-			- Streams: enums.Streams: STR1 | STR2 Number of streams
-			- Stbc: bool: OFF | ON Enables / disables space time block coding (STBC) . If disabled, spatial multiplexing is used."""
+			- Bandwidth: enums.ChannelBandwidthDut: BW20 | BW40 | BW80 | BW160 Channel bandwidth The value must not exceed the operating channel bandwidth, see [CMDLINKRESOLVED Configure.RfSettings#OcWidth CMDLINKRESOLVED].
+			- Coderate: enums.Coderate: BR12 | QR12 | QR34 | Q1M12 | Q1M34 | Q6M23 | Q6M34 | BR34 | MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | D1MBit | D2MBits | C55Mbits | C11Mbits | MCS8 | MCS9 | MCS10 | MCS11 | MCS12 | MCS13 | MCS14 | MCS15 See rate list in [CMDLINKRESOLVED Configure.Connection.MfDef#set CMDLINKRESOLVED]
+			- Guard_Interval: enums.GuardInterval: Optional setting parameter. LONG | SHORt | GI08 | GI16 | GI32 SHORt, LONG: short or long guard interval (up to 802.11ac) GI08, GI16, GI32: 0.8 μs, 1.6 μs, and 3.2 μs guard interval durations (for 802.11ax)
+			- Ltf_Type: enums.LtfType: Optional setting parameter. X1 | X2 | X4 1x HE-LTF, 2x HE-LTF, 4x HE-LTF for 802.11ax
+			- Pe_Duration: enums.PeDuration: Optional setting parameter. PE0 | PE4 | PE8 | PE12 | PE16 | AUTO PEx: additional receive processing time of x μs signaled in packet extension (PE) field (only for 802.11ax) AUTO: automatic setting based on the reported DUTs capabilities
+			- Ctype: enums.CodingType: Optional setting parameter. LDPC | BCC Coding type (for 802.11ax - VHT, HE_SU, HE_MU frames only) : low density parity check or binary convolution code
+			- Streams: enums.Streams: Optional setting parameter. STR1 | STR2 Number of streams
+			- Stbc: bool: Optional setting parameter. OFF | ON Enables / disables space time block coding (STBC) . If disabled, spatial multiplexing is used."""
 		__meta_args_list = [
 			ArgStruct.scalar_enum('Format_Py', enums.DataFormatExt),
 			ArgStruct.scalar_enum('Bandwidth', enums.ChannelBandwidthDut),
 			ArgStruct.scalar_enum('Coderate', enums.Coderate),
-			ArgStruct.scalar_enum('Guard_Interval', enums.GuardInterval),
-			ArgStruct.scalar_enum('Ltf_Type', enums.LtfType),
-			ArgStruct.scalar_enum('Pe_Duration', enums.PeDuration),
-			ArgStruct.scalar_enum('Ctype', enums.CodingType),
-			ArgStruct.scalar_enum('Streams', enums.Streams),
-			ArgStruct.scalar_bool('Stbc')]
+			ArgStruct.scalar_enum_optional('Guard_Interval', enums.GuardInterval),
+			ArgStruct.scalar_enum_optional('Ltf_Type', enums.LtfType),
+			ArgStruct.scalar_enum_optional('Pe_Duration', enums.PeDuration),
+			ArgStruct.scalar_enum_optional('Ctype', enums.CodingType),
+			ArgStruct.scalar_enum_optional('Streams', enums.Streams),
+			ArgStruct.scalar_bool_optional('Stbc')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Format_Py: enums.DataFormatExt = None
 			self.Bandwidth: enums.ChannelBandwidthDut = None
 			self.Coderate: enums.Coderate = None
 			self.Guard_Interval: enums.GuardInterval = None
 			self.Ltf_Type: enums.LtfType = None
 			self.Pe_Duration: enums.PeDuration = None
 			self.Ctype: enums.CodingType = None
 			self.Streams: enums.Streams = None
 			self.Stbc: bool = None
 
-	# noinspection PyTypeChecker
 	def get_fdef(self) -> FdefStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:FDEF \n
 		Snippet: value: FdefStruct = driver.configure.per.get_fdef() \n
 		Configures the downlink data frames for PER measurements. \n
 			:return: structure: for return value, see the help for FdefStruct structure arguments.
 		"""
 		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:PER:FDEF?', self.__class__.FdefStruct())
 
 	def set_fdef(self, value: FdefStruct) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:FDEF \n
-		Snippet: driver.configure.per.set_fdef(value = FdefStruct()) \n
+		Snippet with structure: \n
+		structure = driver.configure.per.FdefStruct() \n
+		structure.Format_Py: enums.DataFormatExt = enums.DataFormatExt.HEES \n
+		structure.Bandwidth: enums.ChannelBandwidthDut = enums.ChannelBandwidthDut.BW160 \n
+		structure.Coderate: enums.Coderate = enums.Coderate.BR12 \n
+		structure.Guard_Interval: enums.GuardInterval = enums.GuardInterval.GI08 \n
+		structure.Ltf_Type: enums.LtfType = enums.LtfType.X1 \n
+		structure.Pe_Duration: enums.PeDuration = enums.PeDuration.AUTO \n
+		structure.Ctype: enums.CodingType = enums.CodingType.BCC \n
+		structure.Streams: enums.Streams = enums.Streams.STR1 \n
+		structure.Stbc: bool = False \n
+		driver.configure.per.set_fdef(value = structure) \n
 		Configures the downlink data frames for PER measurements. \n
 			:param value: see the help for FdefStruct structure arguments.
 		"""
 		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:PER:FDEF', value)
 
 	# noinspection PyTypeChecker
 	def get_dpattern(self) -> enums.Pattern:
@@ -209,14 +219,14 @@
 		Snippet: driver.configure.per.set_repetition(repetition = enums.Repeat.CONTinuous) \n
 		No command help available \n
 			:param repetition: No help available
 		"""
 		param = Conversions.enum_scalar_to_str(repetition, enums.Repeat)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:REPetition {param}')
 
-	def clone(self) -> 'Per':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PerCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Per(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PerCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dframe:
-	"""Dframe commands group definition. 8 total commands, 1 Sub-groups, 0 group commands"""
+class DframeCls:
+	"""Dframe commands group definition. 8 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dframe", core, parent)
+		self._cmd_group = CommandsGroup("dframe", core, parent)
 
 	@property
 	def hemu(self):
 		"""hemu commands group. 5 Sub-classes, 0 commands."""
 		if not hasattr(self, '_hemu'):
-			from .Dframe_.Hemu import Hemu
-			self._hemu = Hemu(self._core, self._base)
+			from .Hemu import HemuCls
+			self._hemu = HemuCls(self._core, self._cmd_group)
 		return self._hemu
 
-	def clone(self) -> 'Dframe':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'DframeCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Dframe(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = DframeCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hemu:
-	"""Hemu commands group definition. 8 total commands, 5 Sub-groups, 0 group commands"""
+class HemuCls:
+	"""Hemu commands group definition. 8 total commands, 5 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hemu", core, parent)
+		self._cmd_group = CommandsGroup("hemu", core, parent)
 
 	@property
 	def alsField(self):
 		"""alsField commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_alsField'):
-			from .Hemu_.AlsField import AlsField
-			self._alsField = AlsField(self._core, self._base)
+			from .AlsField import AlsFieldCls
+			self._alsField = AlsFieldCls(self._core, self._cmd_group)
 		return self._alsField
 
 	@property
 	def ruAllocation(self):
 		"""ruAllocation commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ruAllocation'):
-			from .Hemu_.RuAllocation import RuAllocation
-			self._ruAllocation = RuAllocation(self._core, self._base)
+			from .RuAllocation import RuAllocationCls
+			self._ruAllocation = RuAllocationCls(self._core, self._cmd_group)
 		return self._ruAllocation
 
 	@property
 	def blAllocation(self):
 		"""blAllocation commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_blAllocation'):
-			from .Hemu_.BlAllocation import BlAllocation
-			self._blAllocation = BlAllocation(self._core, self._base)
+			from .BlAllocation import BlAllocationCls
+			self._blAllocation = BlAllocationCls(self._core, self._cmd_group)
 		return self._blAllocation
 
 	@property
 	def user(self):
 		"""user commands group. 4 Sub-classes, 0 commands."""
 		if not hasattr(self, '_user'):
-			from .Hemu_.User import User
-			self._user = User(self._core, self._base)
+			from .User import UserCls
+			self._user = UserCls(self._core, self._cmd_group)
 		return self._user
 
 	@property
 	def dummy(self):
 		"""dummy commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_dummy'):
-			from .Hemu_.Dummy import Dummy
-			self._dummy = Dummy(self._core, self._base)
+			from .Dummy import DummyCls
+			self._dummy = DummyCls(self._core, self._cmd_group)
 		return self._dummy
 
-	def clone(self) -> 'Hemu':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'HemuCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Hemu(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = HemuCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/AlsField.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/AlsField.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 from ......Internal.Types import DataType
 from ......Internal.ArgSingleList import ArgSingleList
 from ......Internal.ArgSingle import ArgSingle
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class AlsField:
-	"""AlsField commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class AlsFieldCls:
+	"""AlsField commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("alsField", core, parent)
+		self._cmd_group = CommandsGroup("alsField", core, parent)
 
 	def set(self, ch_20_index: enums.Ch20Index, subfield: enums.Subfield) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:ALSField \n
 		Snippet: driver.configure.per.dframe.hemu.alsField.set(ch_20_index = enums.Ch20Index.CHA1, subfield = enums.Subfield.A000) \n
 		Sets 8-bit indices for resource unit (RU) allocation for the selected channel. The <Subfield> parameter specifies the
-		number of RUs, their position and size. Refer to IEEE P802.11ax/D8.0, table 27-26, RU allocation subfield. \n
+		number of RUs, their position and size. Refer to IEEE Std 802.11ax-2021, table 27-26, RU allocation subfield. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:param subfield: A000 | A001 | A002 | A003 | A004 | A005 | A006 | A007 | A008 | A009 | A010 | A011 | A012 | A013 | A014 | A015 | A016 | A024 | A032 | A040 | A048 | A056 | A064 | A072 | A080 | A088 | A096 | A112 | A113 | A114 | A115 | A116 | A120 | A128 | A192 | A200 | A208 | A216 | A224
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum), ArgSingle('subfield', subfield, DataType.Enum))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum, enums.Ch20Index), ArgSingle('subfield', subfield, DataType.Enum, enums.Subfield))
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:ALSField {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	def get(self, ch_20_index: enums.Ch20Index) -> enums.Subfield:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:ALSField \n
 		Snippet: value: enums.Subfield = driver.configure.per.dframe.hemu.alsField.get(ch_20_index = enums.Ch20Index.CHA1) \n
 		Sets 8-bit indices for resource unit (RU) allocation for the selected channel. The <Subfield> parameter specifies the
-		number of RUs, their position and size. Refer to IEEE P802.11ax/D8.0, table 27-26, RU allocation subfield. \n
+		number of RUs, their position and size. Refer to IEEE Std 802.11ax-2021, table 27-26, RU allocation subfield. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:return: subfield: A000 | A001 | A002 | A003 | A004 | A005 | A006 | A007 | A008 | A009 | A010 | A011 | A012 | A013 | A014 | A015 | A016 | A024 | A032 | A040 | A048 | A056 | A064 | A072 | A080 | A088 | A096 | A112 | A113 | A114 | A115 | A116 | A120 | A128 | A192 | A200 | A208 | A216 | A224"""
 		param = Conversions.enum_scalar_to_str(ch_20_index, enums.Ch20Index)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:ALSField? {param}')
 		return Conversions.str_to_scalar_enum(response, enums.Subfield)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/BlAllocation.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/BlAllocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from ......Internal import Conversions
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class BlAllocation:
-	"""BlAllocation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class BlAllocationCls:
+	"""BlAllocation commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("blAllocation", core, parent)
+		self._cmd_group = CommandsGroup("blAllocation", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Ru_1: enums.RuAlloc: OFF | USR1 | DMY1 | DMY2 | DMY3 User mapping for to the corresponding RU (no user, user 1 or dummy user)
 			- Size_1: enums.AllocSize: No parameter help available
 			- Ru_2: enums.RuAlloc: No parameter help available
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/Dummy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.RepeatedCapability import RepeatedCapability
-from ...... import repcap
+from ........Internal.Core import Core
+from ........Internal.CommandsGroup import CommandsGroup
+from ........Internal.RepeatedCapability import RepeatedCapability
+from ........ import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dummy:
-	"""Dummy commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
+class DummyCls:
+	"""Dummy commands group definition. 1 total commands, 1 Subgroups, 0 group commands
 	Repeated Capability: Dummy, default value after init: Dummy.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dummy", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_dummy_get', 'repcap_dummy_set', repcap.Dummy.Nr1)
+		self._cmd_group = CommandsGroup("dummy", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_dummy_get', 'repcap_dummy_set', repcap.Dummy.Nr1)
 
-	def repcap_dummy_set(self, enum_value: repcap.Dummy) -> None:
+	def repcap_dummy_set(self, dummy: repcap.Dummy) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Dummy.Default
 		Default value after init: Dummy.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(dummy)
 
 	def repcap_dummy_get(self) -> repcap.Dummy:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def mcs(self):
 		"""mcs commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mcs'):
-			from .Dummy_.Mcs import Mcs
-			self._mcs = Mcs(self._core, self._base)
+			from .Mcs import McsCls
+			self._mcs = McsCls(self._core, self._cmd_group)
 		return self._mcs
 
-	def clone(self) -> 'Dummy':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'DummyCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Dummy(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = DummyCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy_/Mcs.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/Dummy/Mcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from .......Internal.CommandsGroup import CommandsGroup
 from .......Internal import Conversions
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mcs:
-	"""Mcs commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class McsCls:
+	"""Mcs commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mcs", core, parent)
+		self._cmd_group = CommandsGroup("mcs", core, parent)
 
 	def set(self, mcs_index: enums.McsIndex, dummy=repcap.Dummy.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:DUMMy<index>:MCS \n
 		Snippet: driver.configure.per.dframe.hemu.dummy.mcs.set(mcs_index = enums.McsIndex.MCS, dummy = repcap.Dummy.Default) \n
 		Sets the modulation and coding scheme for the corresponding dummy user. \n
 			:param mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11
-			:param dummy: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Dummy')"""
+			:param dummy: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Dummy')
+		"""
 		param = Conversions.enum_scalar_to_str(mcs_index, enums.McsIndex)
-		dummy_cmd_val = self._base.get_repcap_cmd_value(dummy, repcap.Dummy)
+		dummy_cmd_val = self._cmd_group.get_repcap_cmd_value(dummy, repcap.Dummy)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:DUMMy{dummy_cmd_val}:MCS {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, dummy=repcap.Dummy.Default) -> enums.McsIndex:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:DUMMy<index>:MCS \n
 		Snippet: value: enums.McsIndex = driver.configure.per.dframe.hemu.dummy.mcs.get(dummy = repcap.Dummy.Default) \n
 		Sets the modulation and coding scheme for the corresponding dummy user. \n
 			:param dummy: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Dummy')
 			:return: mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11"""
-		dummy_cmd_val = self._base.get_repcap_cmd_value(dummy, repcap.Dummy)
+		dummy_cmd_val = self._cmd_group.get_repcap_cmd_value(dummy, repcap.Dummy)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:DUMMy{dummy_cmd_val}:MCS?')
 		return Conversions.str_to_scalar_enum(response, enums.McsIndex)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/RuAllocation.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/RuAllocation.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 from ......Internal.ArgStruct import ArgStruct
 from ......Internal.ArgSingleList import ArgSingleList
 from ......Internal.ArgSingle import ArgSingle
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RuAllocation:
-	"""RuAllocation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class RuAllocationCls:
+	"""RuAllocation commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ruAllocation", core, parent)
+		self._cmd_group = CommandsGroup("ruAllocation", core, parent)
 
 	def set(self, ch_20_index: enums.Ch20Index, ru_index: enums.RuIndex, alloc_state: enums.RuAlloc) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:RUALlocation \n
 		Snippet: driver.configure.per.dframe.hemu.ruAllocation.set(ch_20_index = enums.Ch20Index.CHA1, ru_index = enums.RuIndex.RU1, alloc_state = enums.RuAlloc.DMY1) \n
 		Configures allocations for specified channel and resource unit (RU) . Maps a user to the RU, sets the size of allocation. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:param ru_index: RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9 Resource unit selection
 			:param alloc_state: OFF | USR1 | DMY1 | DMY2 | DMY3 User mapping for to the selected RU
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum), ArgSingle('ru_index', ru_index, DataType.Enum), ArgSingle('alloc_state', alloc_state, DataType.Enum))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum, enums.Ch20Index), ArgSingle('ru_index', ru_index, DataType.Enum, enums.RuIndex), ArgSingle('alloc_state', alloc_state, DataType.Enum, enums.RuAlloc))
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:RUALlocation {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Alloc_State: enums.RuAlloc: OFF | USR1 | DMY1 | DMY2 | DMY3 User mapping for to the selected RU
 			- Size: enums.AllocSize: T26 | T52 | T106 | T242 | T484 | T996 | T2X9 RU size: 26-, 52-, 106-, 242-, 484, 996-tone RU, 2x996-tone RU"""
@@ -44,9 +44,9 @@
 	def get(self, ch_20_index: enums.Ch20Index, ru_index: enums.RuIndex) -> GetStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:RUALlocation \n
 		Snippet: value: GetStruct = driver.configure.per.dframe.hemu.ruAllocation.get(ch_20_index = enums.Ch20Index.CHA1, ru_index = enums.RuIndex.RU1) \n
 		Configures allocations for specified channel and resource unit (RU) . Maps a user to the RU, sets the size of allocation. \n
 			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
 			:param ru_index: RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9 Resource unit selection
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum), ArgSingle('ru_index', ru_index, DataType.Enum))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum, enums.Ch20Index), ArgSingle('ru_index', ru_index, DataType.Enum, enums.RuIndex))
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:RUALlocation? {param}'.rstrip(), self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Allocation.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Allocation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 from .......Internal.Core import Core
 from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal.Types import DataType
 from .......Internal.StructBase import StructBase
 from .......Internal.ArgStruct import ArgStruct
+from .......Internal.ArgSingleList import ArgSingleList
+from .......Internal.ArgSingle import ArgSingle
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Allocation:
-	"""Allocation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class AllocationCls:
+	"""Allocation commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("allocation", core, parent)
+		self._cmd_group = CommandsGroup("allocation", core, parent)
+
+	def set(self, ch_20_index: enums.Ch20Index, ru_index: enums.RuIndex, user=repcap.User.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:ALLocation \n
+		Snippet: driver.configure.per.dframe.hemu.user.allocation.set(ch_20_index = enums.Ch20Index.CHA1, ru_index = enums.RuIndex.RU1, user = repcap.User.Default) \n
+		Configures allocations for the user in HE MU PPDU. Maps the user to a resource unit (RU) . \n
+			:param ch_20_index: CHA1 | CHA2 | CHA3 | CHA4
+			:param ru_index: RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9
+			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ch_20_index', ch_20_index, DataType.Enum, enums.Ch20Index), ArgSingle('ru_index', ru_index, DataType.Enum, enums.RuIndex))
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:ALLocation {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class AllocationStruct(StructBase):
-		"""Structure for setting input parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- Ch_20_Index: enums.Ch20Index: CHA1 | CHA2 | CHA3 | CHA4
 			- Ru_Index: enums.RuIndex: RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9"""
 		__meta_args_list = [
 			ArgStruct.scalar_enum('Ch_20_Index', enums.Ch20Index),
 			ArgStruct.scalar_enum('Ru_Index', enums.RuIndex)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Ch_20_Index: enums.Ch20Index = None
 			self.Ru_Index: enums.RuIndex = None
 
-	def set(self, structure: AllocationStruct, user=repcap.User.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:ALLocation \n
-		Snippet: driver.configure.per.dframe.hemu.user.allocation.set(value = [PROPERTY_STRUCT_NAME](), user = repcap.User.Default) \n
-		Configures allocations for the user in HE MU PPDU. Maps the user to a resource unit (RU) . \n
-			:param structure: for set value, see the help for AllocationStruct structure arguments.
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')"""
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:ALLocation', structure)
-
 	def get(self, user=repcap.User.Default) -> AllocationStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:ALLocation \n
 		Snippet: value: AllocationStruct = driver.configure.per.dframe.hemu.user.allocation.get(user = repcap.User.Default) \n
 		Configures allocations for the user in HE MU PPDU. Maps the user to a resource unit (RU) . \n
 			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
 			:return: structure: for return value, see the help for AllocationStruct structure arguments."""
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:ALLocation?', self.__class__.AllocationStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Ctype.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Ctype.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from .......Internal.CommandsGroup import CommandsGroup
 from .......Internal import Conversions
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Ctype:
-	"""Ctype commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class CtypeCls:
+	"""Ctype commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ctype", core, parent)
+		self._cmd_group = CommandsGroup("ctype", core, parent)
 
 	def set(self, coding_type: enums.CodingType, user=repcap.User.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:CTYPe \n
 		Snippet: driver.configure.per.dframe.hemu.user.ctype.set(coding_type = enums.CodingType.BCC, user = repcap.User.Default) \n
 		Selects the coding type related to a user for HE MU PPDU. \n
 			:param coding_type: LDPC | BCC
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')"""
+			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
+		"""
 		param = Conversions.enum_scalar_to_str(coding_type, enums.CodingType)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:CTYPe {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, user=repcap.User.Default) -> enums.CodingType:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:CTYPe \n
 		Snippet: value: enums.CodingType = driver.configure.per.dframe.hemu.user.ctype.get(user = repcap.User.Default) \n
 		Selects the coding type related to a user for HE MU PPDU. \n
 			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
 			:return: coding_type: LDPC | BCC"""
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:CTYPe?')
 		return Conversions.str_to_scalar_enum(response, enums.CodingType)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Mcs.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Mcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from .......Internal.Core import Core
-from .......Internal.CommandsGroup import CommandsGroup
-from .......Internal import Conversions
-from ....... import enums
-from ....... import repcap
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ...... import enums
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mcs:
-	"""Mcs commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class McsCls:
+	"""Mcs commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mcs", core, parent)
+		self._cmd_group = CommandsGroup("mcs", core, parent)
 
-	def set(self, mcs_index: enums.McsIndex, user=repcap.User.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:MCS \n
-		Snippet: driver.configure.per.dframe.hemu.user.mcs.set(mcs_index = enums.McsIndex.MCS, user = repcap.User.Default) \n
-		Sets the modulation and coding scheme for user 1 (user data assigned to the DUT) . \n
-			:param mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')"""
-		param = Conversions.enum_scalar_to_str(mcs_index, enums.McsIndex)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:MCS {param}')
+	def set(self, mcs: enums.McsIndex, station=repcap.Station.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:MCS \n
+		Snippet: driver.configure.sta.connection.hetf.mcs.set(mcs = enums.McsIndex.MCS, station = repcap.Station.Default) \n
+		Specifies the modulation and coding scheme (MCS) used by the HE TB PPDU. \n
+			:param mcs: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		param = Conversions.enum_scalar_to_str(mcs, enums.McsIndex)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:MCS {param}')
 
 	# noinspection PyTypeChecker
-	def get(self, user=repcap.User.Default) -> enums.McsIndex:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:MCS \n
-		Snippet: value: enums.McsIndex = driver.configure.per.dframe.hemu.user.mcs.get(user = repcap.User.Default) \n
-		Sets the modulation and coding scheme for user 1 (user data assigned to the DUT) . \n
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
-			:return: mcs_index: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11"""
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
-		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:MCS?')
+	def get(self, station=repcap.Station.Default) -> enums.McsIndex:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:MCS \n
+		Snippet: value: enums.McsIndex = driver.configure.sta.connection.hetf.mcs.get(station = repcap.Station.Default) \n
+		Specifies the modulation and coding scheme (MCS) used by the HE TB PPDU. \n
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+			:return: mcs: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:MCS?')
 		return Conversions.str_to_scalar_enum(response, enums.McsIndex)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Streams.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Streams.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from .......Internal.CommandsGroup import CommandsGroup
 from .......Internal import Conversions
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Streams:
-	"""Streams commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class StreamsCls:
+	"""Streams commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("streams", core, parent)
+		self._cmd_group = CommandsGroup("streams", core, parent)
 
 	def set(self, streams: enums.Streams, user=repcap.User.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:STReams \n
 		Snippet: driver.configure.per.dframe.hemu.user.streams.set(streams = enums.Streams.STR1, user = repcap.User.Default) \n
 		Sets the number of streams for PER measurements used by the user for MIMO connections. \n
 			:param streams: STR1 | STR2 One or two streams
-			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')"""
+			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
+		"""
 		param = Conversions.enum_scalar_to_str(streams, enums.Streams)
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:STReams {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, user=repcap.User.Default) -> enums.Streams:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:DFRame:HEMU:USER<index>:STReams \n
 		Snippet: value: enums.Streams = driver.configure.per.dframe.hemu.user.streams.get(user = repcap.User.Default) \n
 		Sets the number of streams for PER measurements used by the user for MIMO connections. \n
 			:param user: optional repeated capability selector. Default value: Nr1 (settable in the interface 'User')
 			:return: streams: STR1 | STR2 One or two streams"""
-		user_cmd_val = self._base.get_repcap_cmd_value(user, repcap.User)
+		user_cmd_val = self._cmd_group.get_repcap_cmd_value(user, repcap.User)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PER:DFRame:HEMU:USER{user_cmd_val}:STReams?')
 		return Conversions.str_to_scalar_enum(response, enums.Streams)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Per_/Payload.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Per/Payload.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Payload:
-	"""Payload commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class PayloadCls:
+	"""Payload commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("payload", core, parent)
+		self._cmd_group = CommandsGroup("payload", core, parent)
 
 	def get_size(self) -> int:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PER:PAYLoad:SIZE \n
 		Snippet: value: int = driver.configure.per.payload.get_size() \n
 		Specifies the payload size (in bytes) for the PER measurement. \n
 			:return: size: integer Range: see table below , Unit: byte
 		"""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal.RepeatedCapability import RepeatedCapability
-from ... import repcap
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.RepeatedCapability import RepeatedCapability
+from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Pgen:
-	"""Pgen commands group definition. 5 total commands, 5 Sub-groups, 0 group commands
+class PgenCls:
+	"""Pgen commands group definition. 5 total commands, 5 Subgroups, 0 group commands
 	Repeated Capability: PacketGenerator, default value after init: PacketGenerator.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("pgen", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_packetGenerator_get', 'repcap_packetGenerator_set', repcap.PacketGenerator.Nr1)
+		self._cmd_group = CommandsGroup("pgen", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_packetGenerator_get', 'repcap_packetGenerator_set', repcap.PacketGenerator.Nr1)
 
-	def repcap_packetGenerator_set(self, enum_value: repcap.PacketGenerator) -> None:
+	def repcap_packetGenerator_set(self, packetGenerator: repcap.PacketGenerator) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to PacketGenerator.Default
 		Default value after init: PacketGenerator.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(packetGenerator)
 
 	def repcap_packetGenerator_get(self) -> repcap.PacketGenerator:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def ipVersion(self):
 		"""ipVersion commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ipVersion'):
-			from .Pgen_.IpVersion import IpVersion
-			self._ipVersion = IpVersion(self._core, self._base)
+			from .IpVersion import IpVersionCls
+			self._ipVersion = IpVersionCls(self._core, self._cmd_group)
 		return self._ipVersion
 
 	@property
 	def uports(self):
 		"""uports commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_uports'):
-			from .Pgen_.Uports import Uports
-			self._uports = Uports(self._core, self._base)
+			from .Uports import UportsCls
+			self._uports = UportsCls(self._core, self._cmd_group)
 		return self._uports
 
 	@property
 	def protocol(self):
 		"""protocol commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_protocol'):
-			from .Pgen_.Protocol import Protocol
-			self._protocol = Protocol(self._core, self._base)
+			from .Protocol import ProtocolCls
+			self._protocol = ProtocolCls(self._core, self._cmd_group)
 		return self._protocol
 
 	@property
 	def config(self):
 		"""config commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_config'):
-			from .Pgen_.Config import Config
-			self._config = Config(self._core, self._base)
+			from .Config import ConfigCls
+			self._config = ConfigCls(self._core, self._cmd_group)
 		return self._config
 
 	@property
 	def destination(self):
 		"""destination commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_destination'):
-			from .Pgen_.Destination import Destination
-			self._destination = Destination(self._core, self._base)
+			from .Destination import DestinationCls
+			self._destination = DestinationCls(self._core, self._cmd_group)
 		return self._destination
 
-	def clone(self) -> 'Pgen':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'PgenCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Pgen(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = PgenCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/Config.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/Uports.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Types import DataType
 from ....Internal.StructBase import StructBase
 from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from ....Internal.ArgSingleList import ArgSingleList
+from ....Internal.ArgSingle import ArgSingle
 from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Config:
-	"""Config commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class UportsCls:
+	"""Uports commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("config", core, parent)
+		self._cmd_group = CommandsGroup("uports", core, parent)
+
+	def set(self, source_port: int, destination_port: int, packetGenerator=repcap.PacketGenerator.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:UPORts \n
+		Snippet: driver.configure.pgen.uports.set(source_port = 1, destination_port = 1, packetGenerator = repcap.PacketGenerator.Default) \n
+		Sets the source and destination ports for the UDP protocol. \n
+			:param source_port: integer Range: 0 to 65535
+			:param destination_port: integer Range: 0 to 65535
+			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('source_port', source_port, DataType.Integer), ArgSingle('destination_port', destination_port, DataType.Integer))
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:UPORts {param}'.rstrip())
 
 	# noinspection PyTypeChecker
-	class ConfigStruct(StructBase):
-		"""Structure for setting input parameters. Contains optional setting parameters. Fields: \n
-			- State: bool: OFF | ON Disables/enables the packet generator
-			- Interval: int: integer Time interval between packet transmissions in units of 1024 μs Range: 0 to 10E+3
-			- Payload_Size: int: integer Payload size of generated packets in bytes Range: 0 to 1472
-			- Payload_Type: enums.PayloadType: DEFault | AZERoes | AONes | BP01 | BP10 | PRANdom Bit sequence to be transmitted as payload DEFault: an implementation-specific default pattern AZERoes: all zeroes AONes: all ones BP01: bit pattern 010101... BP10: bit pattern 101010... PRANdom: a pseudo-random bit sequence
-			- Tid: enums.Tid: Optional setting parameter. TID0 | TID1 | TID2 | TID3 | TID4 | TID5 | TID6 | TID7 TID signaled by the packet generator"""
+	class UportsStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Source_Port: int: integer Range: 0 to 65535
+			- Destination_Port: int: integer Range: 0 to 65535"""
 		__meta_args_list = [
-			ArgStruct.scalar_bool('State'),
-			ArgStruct.scalar_int('Interval'),
-			ArgStruct.scalar_int('Payload_Size'),
-			ArgStruct.scalar_enum('Payload_Type', enums.PayloadType),
-			ArgStruct.scalar_enum('Tid', enums.Tid)]
+			ArgStruct.scalar_int('Source_Port'),
+			ArgStruct.scalar_int('Destination_Port')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.State: bool = None
-			self.Interval: int = None
-			self.Payload_Size: int = None
-			self.Payload_Type: enums.PayloadType = None
-			self.Tid: enums.Tid = None
-
-	def set(self, structure: ConfigStruct, packetGenerator=repcap.PacketGenerator.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:CONFig \n
-		Snippet: driver.configure.pgen.config.set(value = [PROPERTY_STRUCT_NAME](), packetGenerator = repcap.PacketGenerator.Default) \n
-		Configures the packet generator. \n
-			:param structure: for set value, see the help for ConfigStruct structure arguments.
-			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')"""
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:CONFig', structure)
-
-	def get(self, packetGenerator=repcap.PacketGenerator.Default) -> ConfigStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:CONFig \n
-		Snippet: value: ConfigStruct = driver.configure.pgen.config.get(packetGenerator = repcap.PacketGenerator.Default) \n
-		Configures the packet generator. \n
+			self.Source_Port: int = None
+			self.Destination_Port: int = None
+
+	def get(self, packetGenerator=repcap.PacketGenerator.Default) -> UportsStruct:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:UPORts \n
+		Snippet: value: UportsStruct = driver.configure.pgen.uports.get(packetGenerator = repcap.PacketGenerator.Default) \n
+		Sets the source and destination ports for the UDP protocol. \n
 			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
-			:return: structure: for return value, see the help for ConfigStruct structure arguments."""
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
-		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:CONFig?', self.__class__.ConfigStruct())
+			:return: structure: for return value, see the help for UportsStruct structure arguments."""
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:UPORts?', self.__class__.UportsStruct())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/Destination.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/Destination.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 from .... import enums
 from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Destination:
-	"""Destination commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class DestinationCls:
+	"""Destination commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("destination", core, parent)
+		self._cmd_group = CommandsGroup("destination", core, parent)
 
 	def set(self, station: enums.Station, packetGenerator=repcap.PacketGenerator.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:DESTination \n
 		Snippet: driver.configure.pgen.destination.set(station = enums.Station.STA1, packetGenerator = repcap.PacketGenerator.Default) \n
 		Specifies the STA to which the packets are addressed to. This parameter is visible, if 'Multi STA' is enabled. \n
 			:param station: STA1 | STA2 | STA3
-			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')"""
+			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
+		"""
 		param = Conversions.enum_scalar_to_str(station, enums.Station)
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:DESTination {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, packetGenerator=repcap.PacketGenerator.Default) -> enums.Station:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:DESTination \n
 		Snippet: value: enums.Station = driver.configure.pgen.destination.get(packetGenerator = repcap.PacketGenerator.Default) \n
 		Specifies the STA to which the packets are addressed to. This parameter is visible, if 'Multi STA' is enabled. \n
 			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
 			:return: station: STA1 | STA2 | STA3"""
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:DESTination?')
 		return Conversions.str_to_scalar_enum(response, enums.Station)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/IpVersion.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/IpVersion.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 from .... import enums
 from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class IpVersion:
-	"""IpVersion commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class IpVersionCls:
+	"""IpVersion commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ipVersion", core, parent)
+		self._cmd_group = CommandsGroup("ipVersion", core, parent)
 
 	def set(self, version: enums.IpVersion, packetGenerator=repcap.PacketGenerator.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:IPVersion \n
 		Snippet: driver.configure.pgen.ipVersion.set(version = enums.IpVersion.IV4, packetGenerator = repcap.PacketGenerator.Default) \n
 		Sets the IP version to be used for generating packets. \n
 			:param version: IV4 | IV6
-			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')"""
+			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
+		"""
 		param = Conversions.enum_scalar_to_str(version, enums.IpVersion)
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:IPVersion {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, packetGenerator=repcap.PacketGenerator.Default) -> enums.IpVersion:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:IPVersion \n
 		Snippet: value: enums.IpVersion = driver.configure.pgen.ipVersion.get(packetGenerator = repcap.PacketGenerator.Default) \n
 		Sets the IP version to be used for generating packets. \n
 			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
 			:return: version: IV4 | IV6"""
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:IPVersion?')
 		return Conversions.str_to_scalar_enum(response, enums.IpVersion)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/Protocol.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Pgen/Protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 from .... import enums
 from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Protocol:
-	"""Protocol commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class ProtocolCls:
+	"""Protocol commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("protocol", core, parent)
+		self._cmd_group = CommandsGroup("protocol", core, parent)
 
 	def set(self, type_py: enums.ProtocolType, packetGenerator=repcap.PacketGenerator.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:PROTocol \n
 		Snippet: driver.configure.pgen.protocol.set(type_py = enums.ProtocolType.ICMP, packetGenerator = repcap.PacketGenerator.Default) \n
 		Sets the protocol of the packet generator. \n
 			:param type_py: ICMP | UDP
-			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')"""
+			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
+		"""
 		param = Conversions.enum_scalar_to_str(type_py, enums.ProtocolType)
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:PROTocol {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, packetGenerator=repcap.PacketGenerator.Default) -> enums.ProtocolType:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:PROTocol \n
 		Snippet: value: enums.ProtocolType = driver.configure.pgen.protocol.get(packetGenerator = repcap.PacketGenerator.Default) \n
 		Sets the protocol of the packet generator. \n
 			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
 			:return: type_py: ICMP | UDP"""
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:PROTocol?')
 		return Conversions.str_to_scalar_enum(response, enums.ProtocolType)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Pgen_/Uports.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/DsmLength.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import repcap
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Types import DataType
+from .....Internal.StructBase import StructBase
+from .....Internal.ArgStruct import ArgStruct
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Uports:
-	"""Uports commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class DsmLengthCls:
+	"""DsmLength commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uports", core, parent)
+		self._cmd_group = CommandsGroup("dsmLength", core, parent)
+
+	def set(self, mode: enums.LenMode, length: int = None) -> None:
+		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:DSMLength \n
+		Snippet: driver.trigger.rx.macFrame.dsmLength.set(mode = enums.LenMode.DEFault, length = 1) \n
+		Defines the minimum length for the RX frame trigger mode DSSS/CCK Bursts, see method RsCmwWlanSig.Trigger.Rx.MacFrame.
+		btype. \n
+			:param mode: DEFault | UDEFined DEFault: automatically calculated value UDEFined: configured Length
+			:param length: numeric Minimum number of bytes for UDEFined mode Range: 16 to 1500, Unit: byte
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('mode', mode, DataType.Enum, enums.LenMode), ArgSingle('length', length, DataType.Integer, None, is_optional=True))
+		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:DSMLength {param}'.rstrip())
 
 	# noinspection PyTypeChecker
-	class UportsStruct(StructBase):
-		"""Structure for setting input parameters. Fields: \n
-			- Source_Port: int: integer Range: 0 to 65535
-			- Destination_Port: int: integer Range: 0 to 65535"""
+	class DsmLengthStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Mode: enums.LenMode: DEFault | UDEFined DEFault: automatically calculated value UDEFined: configured Length
+			- Length: int: numeric Minimum number of bytes for UDEFined mode Range: 16 to 1500, Unit: byte"""
 		__meta_args_list = [
-			ArgStruct.scalar_int('Source_Port'),
-			ArgStruct.scalar_int('Destination_Port')]
+			ArgStruct.scalar_enum('Mode', enums.LenMode),
+			ArgStruct.scalar_int('Length')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Source_Port: int = None
-			self.Destination_Port: int = None
+			self.Mode: enums.LenMode = None
+			self.Length: int = None
 
-	def set(self, structure: UportsStruct, packetGenerator=repcap.PacketGenerator.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:UPORts \n
-		Snippet: driver.configure.pgen.uports.set(value = [PROPERTY_STRUCT_NAME](), packetGenerator = repcap.PacketGenerator.Default) \n
-		Sets the source and destination ports for the UDP protocol. \n
-			:param structure: for set value, see the help for UportsStruct structure arguments.
-			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')"""
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:UPORts', structure)
-
-	def get(self, packetGenerator=repcap.PacketGenerator.Default) -> UportsStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:PGEN<index>:UPORts \n
-		Snippet: value: UportsStruct = driver.configure.pgen.uports.get(packetGenerator = repcap.PacketGenerator.Default) \n
-		Sets the source and destination ports for the UDP protocol. \n
-			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
-			:return: structure: for return value, see the help for UportsStruct structure arguments."""
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
-		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:UPORts?', self.__class__.UportsStruct())
+	def get(self) -> DsmLengthStruct:
+		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:DSMLength \n
+		Snippet: value: DsmLengthStruct = driver.trigger.rx.macFrame.dsmLength.get() \n
+		Defines the minimum length for the RX frame trigger mode DSSS/CCK Bursts, see method RsCmwWlanSig.Trigger.Rx.MacFrame.
+		btype. \n
+			:return: structure: for return value, see the help for DsmLengthStruct structure arguments."""
+		return self._core.io.query_struct(f'TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:DSMLength?', self.__class__.DsmLengthStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal import Conversions
-from ... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
+from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RfSettings:
-	"""RfSettings commands group definition. 17 total commands, 2 Sub-groups, 12 group commands"""
+class RfSettingsCls:
+	"""RfSettings commands group definition. 17 total commands, 2 Subgroups, 12 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rfSettings", core, parent)
+		self._cmd_group = CommandsGroup("rfSettings", core, parent)
 
 	@property
 	def antenna(self):
 		"""antenna commands group. 3 Sub-classes, 0 commands."""
 		if not hasattr(self, '_antenna'):
-			from .RfSettings_.Antenna import Antenna
-			self._antenna = Antenna(self._core, self._base)
+			from .Antenna import AntennaCls
+			self._antenna = AntennaCls(self._core, self._cmd_group)
 		return self._antenna
 
 	@property
 	def eattenuation(self):
 		"""eattenuation commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_eattenuation'):
-			from .RfSettings_.Eattenuation import Eattenuation
-			self._eattenuation = Eattenuation(self._core, self._base)
+			from .Eattenuation import EattenuationCls
+			self._eattenuation = EattenuationCls(self._core, self._cmd_group)
 		return self._eattenuation
 
 	# noinspection PyTypeChecker
 	def get_oc_width(self) -> enums.ChannelBandwidthDut:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:OCWidth \n
 		Snippet: value: enums.ChannelBandwidthDut = driver.configure.rfSettings.get_oc_width() \n
 		Sets the operating channel bandwidth. \n
@@ -192,24 +192,24 @@
 		param = Conversions.decimal_value_to_str(value)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:MLOFfset {param}')
 
 	def get_epe_power(self) -> float or bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:EPEPower \n
 		Snippet: value: float or bool = driver.configure.rfSettings.get_epe_power() \n
 		No command help available \n
-			:return: expected_peak_envelop_power: No help available
+			:return: expected_peak_envelop_power: (float or boolean) No help available
 		"""
 		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:RFSettings:EPEPower?')
 		return Conversions.str_to_float_or_bool(response)
 
 	def set_epe_power(self, expected_peak_envelop_power: float or bool) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:EPEPower \n
 		Snippet: driver.configure.rfSettings.set_epe_power(expected_peak_envelop_power = 1.0) \n
 		No command help available \n
-			:param expected_peak_envelop_power: No help available
+			:param expected_peak_envelop_power: (float or boolean) No help available
 		"""
 		param = Conversions.decimal_or_bool_value_to_str(expected_peak_envelop_power)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:EPEPower {param}')
 
 	def get_ts_ratio(self) -> float:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:TSRatio \n
 		Snippet: value: float = driver.configure.rfSettings.get_ts_ratio() \n
@@ -248,14 +248,14 @@
 		With levelconnector, min = -145.98 dBm (-137.98 dBm) , levelconnector, max = -15.98 dBm (-2.98 dBm) for RF COM (RF OUT) ;
 		please also notice the ranges quoted in the data sheet. \n
 			:param burst_output_pow: numeric Range: see above , Unit: dBm
 		"""
 		param = Conversions.decimal_value_to_str(burst_output_pow)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:BOPower {param}')
 
-	def clone(self) -> 'RfSettings':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'RfSettingsCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = RfSettings(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = RfSettingsCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.RepeatedCapability import RepeatedCapability
-from .... import repcap
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.RepeatedCapability import RepeatedCapability
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Antenna:
-	"""Antenna commands group definition. 4 total commands, 3 Sub-groups, 0 group commands
+class AntennaCls:
+	"""Antenna commands group definition. 4 total commands, 3 Subgroups, 0 group commands
 	Repeated Capability: Antenna, default value after init: Antenna.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("antenna", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_antenna_get', 'repcap_antenna_set', repcap.Antenna.Nr1)
+		self._cmd_group = CommandsGroup("antenna", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_antenna_get', 'repcap_antenna_set', repcap.Antenna.Nr1)
 
-	def repcap_antenna_set(self, enum_value: repcap.Antenna) -> None:
+	def repcap_antenna_set(self, antenna: repcap.Antenna) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Antenna.Default
 		Default value after init: Antenna.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(antenna)
 
 	def repcap_antenna_get(self) -> repcap.Antenna:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def mlOffset(self):
 		"""mlOffset commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mlOffset'):
-			from .Antenna_.MlOffset import MlOffset
-			self._mlOffset = MlOffset(self._core, self._base)
+			from .MlOffset import MlOffsetCls
+			self._mlOffset = MlOffsetCls(self._core, self._cmd_group)
 		return self._mlOffset
 
 	@property
 	def epePower(self):
 		"""epePower commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_epePower'):
-			from .Antenna_.EpePower import EpePower
-			self._epePower = EpePower(self._core, self._base)
+			from .EpePower import EpePowerCls
+			self._epePower = EpePowerCls(self._core, self._cmd_group)
 		return self._epePower
 
 	@property
 	def eattenuation(self):
 		"""eattenuation commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_eattenuation'):
-			from .Antenna_.Eattenuation import Eattenuation
-			self._eattenuation = Eattenuation(self._core, self._base)
+			from .Eattenuation import EattenuationCls
+			self._eattenuation = EattenuationCls(self._core, self._cmd_group)
 		return self._eattenuation
 
-	def clone(self) -> 'Antenna':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'AntennaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Antenna(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = AntennaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/Mac/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Eattenuation:
-	"""Eattenuation commands group definition. 2 total commands, 2 Sub-groups, 0 group commands"""
+class MacCls:
+	"""Mac commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("eattenuation", core, parent)
+		self._cmd_group = CommandsGroup("mac", core, parent)
 
 	@property
-	def inputPy(self):
-		"""inputPy commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_inputPy'):
-			from .Eattenuation_.InputPy import InputPy
-			self._inputPy = InputPy(self._core, self._base)
-		return self._inputPy
+	def address(self):
+		"""address commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_address'):
+			from .Address import AddressCls
+			self._address = AddressCls(self._core, self._cmd_group)
+		return self._address
 
-	@property
-	def output(self):
-		"""output commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_output'):
-			from .Eattenuation_.Output import Output
-			self._output = Output(self._core, self._base)
-		return self._output
-
-	def clone(self) -> 'Eattenuation':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MacCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Eattenuation(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MacCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/InputPy.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/InputPy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class InputPy:
-	"""InputPy commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class InputPyCls:
+	"""InputPy commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("inputPy", core, parent)
+		self._cmd_group = CommandsGroup("inputPy", core, parent)
 
 	def set(self, ext_attenuation: float, antenna=repcap.Antenna.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:ANTenna<n>:EATTenuation:INPut \n
 		Snippet: driver.configure.rfSettings.antenna.eattenuation.inputPy.set(ext_attenuation = 1.0, antenna = repcap.Antenna.Default) \n
 		Specifies the external attenuation for the specified antenna in the analyzer path. Antenna 2 is only available in a MIMO
 		scenario with two input paths. \n
 			:param ext_attenuation: numeric Range: -50 dB to 55 dB, Unit: dB
-			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')"""
+			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
+		"""
 		param = Conversions.decimal_value_to_str(ext_attenuation)
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:ANTenna{antenna_cmd_val}:EATTenuation:INPut {param}')
 
 	def get(self, antenna=repcap.Antenna.Default) -> float:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:ANTenna<n>:EATTenuation:INPut \n
 		Snippet: value: float = driver.configure.rfSettings.antenna.eattenuation.inputPy.get(antenna = repcap.Antenna.Default) \n
 		Specifies the external attenuation for the specified antenna in the analyzer path. Antenna 2 is only available in a MIMO
 		scenario with two input paths. \n
 			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
 			:return: ext_attenuation: numeric Range: -50 dB to 55 dB, Unit: dB"""
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:ANTenna{antenna_cmd_val}:EATTenuation:INPut?')
 		return Conversions.str_to_float(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/Output.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/Output.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Output:
-	"""Output commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class OutputCls:
+	"""Output commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("output", core, parent)
+		self._cmd_group = CommandsGroup("output", core, parent)
 
 	def set(self, ext_attenuation: float, antenna=repcap.Antenna.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:ANTenna<n>:EATTenuation:OUTPut \n
 		Snippet: driver.configure.rfSettings.antenna.eattenuation.output.set(ext_attenuation = 1.0, antenna = repcap.Antenna.Default) \n
 		Defines an external attenuation (or gain, if the value is negative) , to be applied to the individual antennas. Antenna 2
 		is only available in a MIMO scenario. \n
 			:param ext_attenuation: numeric Range: -50 dB to 90 dB, Unit: dB
-			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')"""
+			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
+		"""
 		param = Conversions.decimal_value_to_str(ext_attenuation)
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:ANTenna{antenna_cmd_val}:EATTenuation:OUTPut {param}')
 
 	def get(self, antenna=repcap.Antenna.Default) -> float:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:ANTenna<n>:EATTenuation:OUTPut \n
 		Snippet: value: float = driver.configure.rfSettings.antenna.eattenuation.output.get(antenna = repcap.Antenna.Default) \n
 		Defines an external attenuation (or gain, if the value is negative) , to be applied to the individual antennas. Antenna 2
 		is only available in a MIMO scenario. \n
 			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
 			:return: ext_attenuation: numeric Range: -50 dB to 90 dB, Unit: dB"""
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:ANTenna{antenna_cmd_val}:EATTenuation:OUTPut?')
 		return Conversions.str_to_float(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/EpePower.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/EpePower.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class EpePower:
-	"""EpePower commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class EpePowerCls:
+	"""EpePower commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("epePower", core, parent)
+		self._cmd_group = CommandsGroup("epePower", core, parent)
 
 	def set(self, expected_peak_envelop_power: float or bool, antenna=repcap.Antenna.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:ANTenna<n>:EPEPower \n
 		Snippet: driver.configure.rfSettings.antenna.epePower.set(expected_peak_envelop_power = 1.0, antenna = repcap.Antenna.Default) \n
 		Specifies the expected peak envelope power of the specified antenna at the I/Q input. Antenna 2 is only available in MIMO
 		scenarios with two input paths. The correct DUT range to be set is (-20 dBm + external attenuation) to (55 dBm + external
 		attenuation) . \n
-			:param expected_peak_envelop_power: No help available
-			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')"""
+			:param expected_peak_envelop_power: (float or boolean) No help available
+			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
+		"""
 		param = Conversions.decimal_or_bool_value_to_str(expected_peak_envelop_power)
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:ANTenna{antenna_cmd_val}:EPEPower {param}')
 
 	def get(self, antenna=repcap.Antenna.Default) -> float or bool:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:ANTenna<n>:EPEPower \n
 		Snippet: value: float or bool = driver.configure.rfSettings.antenna.epePower.get(antenna = repcap.Antenna.Default) \n
 		Specifies the expected peak envelope power of the specified antenna at the I/Q input. Antenna 2 is only available in MIMO
 		scenarios with two input paths. The correct DUT range to be set is (-20 dBm + external attenuation) to (55 dBm + external
 		attenuation) . \n
 			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
-			:return: expected_peak_envelop_power: No help available"""
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+			:return: expected_peak_envelop_power: (float or boolean) No help available"""
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:ANTenna{antenna_cmd_val}:EPEPower?')
 		return Conversions.str_to_float_or_bool(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/MlOffset.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/MlOffset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MlOffset:
-	"""MlOffset commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class MlOffsetCls:
+	"""MlOffset commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mlOffset", core, parent)
+		self._cmd_group = CommandsGroup("mlOffset", core, parent)
 
 	def set(self, value: int, antenna=repcap.Antenna.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:ANTenna<n>:MLOFfset \n
 		Snippet: driver.configure.rfSettings.antenna.mlOffset.set(value = 1, antenna = repcap.Antenna.Default) \n
 		Varies the input level of the mixer for the specified antenna in the analyzer path. Antenna 2 is only available in MIMO
 		scenarios with two input paths. \n
 			:param value: integer Range: -10 dB to 12dB , Unit: dB
-			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')"""
+			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
+		"""
 		param = Conversions.decimal_value_to_str(value)
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:ANTenna{antenna_cmd_val}:MLOFfset {param}')
 
 	def get(self, antenna=repcap.Antenna.Default) -> int:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:ANTenna<n>:MLOFfset \n
 		Snippet: value: int = driver.configure.rfSettings.antenna.mlOffset.get(antenna = repcap.Antenna.Default) \n
 		Varies the input level of the mixer for the specified antenna in the analyzer path. Antenna 2 is only available in MIMO
 		scenarios with two input paths. \n
 			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
 			:return: value: integer Range: -10 dB to 12dB , Unit: dB"""
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:RFSettings:ANTenna{antenna_cmd_val}:MLOFfset?')
 		return Conversions.str_to_int(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/RfSettings_/Eattenuation.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/RfSettings/Eattenuation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Eattenuation:
-	"""Eattenuation commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class EattenuationCls:
+	"""Eattenuation commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("eattenuation", core, parent)
+		self._cmd_group = CommandsGroup("eattenuation", core, parent)
 
 	def get_input_py(self) -> float:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:RFSettings:EATTenuation:INPut \n
 		Snippet: value: float = driver.configure.rfSettings.eattenuation.get_input_py() \n
 		No command help available \n
 			:return: ext_attenuation: No help available
 		"""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,58 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal.RepeatedCapability import RepeatedCapability
-from ... import repcap
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.RepeatedCapability import RepeatedCapability
+from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sta:
-	"""Sta commands group definition. 13 total commands, 1 Sub-groups, 0 group commands
+class StaCls:
+	"""Sta commands group definition. 13 total commands, 3 Subgroups, 0 group commands
 	Repeated Capability: Station, default value after init: Station.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sta", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
+		self._cmd_group = CommandsGroup("sta", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_station_get', 'repcap_station_set', repcap.Station.Nr1)
 
-	def repcap_station_set(self, enum_value: repcap.Station) -> None:
+	def repcap_station_set(self, station: repcap.Station) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Station.Default
 		Default value after init: Station.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(station)
 
 	def repcap_station_get(self) -> repcap.Station:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
-	def connection(self):
-		"""connection commands group. 4 Sub-classes, 0 commands."""
-		if not hasattr(self, '_connection'):
-			from .Sta_.Connection import Connection
-			self._connection = Connection(self._core, self._base)
-		return self._connection
+	def uesInfo(self):
+		"""uesInfo commands group. 5 Sub-classes, 0 commands."""
+		if not hasattr(self, '_uesInfo'):
+			from .UesInfo import UesInfoCls
+			self._uesInfo = UesInfoCls(self._core, self._cmd_group)
+		return self._uesInfo
 
-	def clone(self) -> 'Sta':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def ueCapability(self):
+		"""ueCapability commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_ueCapability'):
+			from .UeCapability import UeCapabilityCls
+			self._ueCapability = UeCapabilityCls(self._core, self._cmd_group)
+		return self._ueCapability
+
+	@property
+	def hetbInfo(self):
+		"""hetbInfo commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_hetbInfo'):
+			from .HetbInfo import HetbInfoCls
+			self._hetbInfo = HetbInfoCls(self._core, self._cmd_group)
+		return self._hetbInfo
+
+	def clone(self) -> 'StaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Sta(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = StaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Etoe/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,35 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Connection:
-	"""Connection commands group definition. 13 total commands, 4 Sub-groups, 0 group commands"""
+class EtoeCls:
+	"""Etoe commands group definition. 2 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("connection", core, parent)
+		self._cmd_group = CommandsGroup("etoe", core, parent)
 
 	@property
-	def qos(self):
-		"""qos commands group. 2 Sub-classes, 0 commands."""
-		if not hasattr(self, '_qos'):
-			from .Connection_.Qos import Qos
-			self._qos = Qos(self._core, self._base)
-		return self._qos
+	def irList(self):
+		"""irList commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_irList'):
+			from .IrList import IrListCls
+			self._irList = IrListCls(self._core, self._cmd_group)
+		return self._irList
 
 	@property
-	def dfdef(self):
-		"""dfdef commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_dfdef'):
-			from .Connection_.Dfdef import Dfdef
-			self._dfdef = Dfdef(self._core, self._base)
-		return self._dfdef
+	def duIp(self):
+		"""duIp commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_duIp'):
+			from .DuIp import DuIpCls
+			self._duIp = DuIpCls(self._core, self._cmd_group)
+		return self._duIp
 
-	@property
-	def hetf(self):
-		"""hetf commands group. 9 Sub-classes, 0 commands."""
-		if not hasattr(self, '_hetf'):
-			from .Connection_.Hetf import Hetf
-			self._hetf = Hetf(self._core, self._base)
-		return self._hetf
-
-	@property
-	def ampdu(self):
-		"""ampdu commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_ampdu'):
-			from .Connection_.Ampdu import Ampdu
-			self._ampdu = Ampdu(self._core, self._base)
-		return self._ampdu
-
-	def clone(self) -> 'Connection':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'EtoeCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Connection(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = EtoeCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Ampdu.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Trssi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,37 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal.StructBase import StructBase
-from .....Internal.ArgStruct import ArgStruct
-from ..... import enums
-from ..... import repcap
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal.StructBase import StructBase
+from ......Internal.ArgStruct import ArgStruct
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Ampdu:
-	"""Ampdu commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class TrssiCls:
+	"""Trssi commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ampdu", core, parent)
+		self._cmd_group = CommandsGroup("trssi", core, parent)
 
 	# noinspection PyTypeChecker
-	class AmpduStruct(StructBase):
-		"""Structure for setting input parameters. Fields: \n
-			- Enable: enums.EnableState: DISable | ENABle Enables/ disables the A-MPDUs
-			- Multi_Tid: enums.EnableState: DISable | ENABle Enables/ disables multi-TID A-MPDU
-			- Max_Length: int: integer The maximal length of entire A-MPDU Range: 50 to 131.071E+3, Unit: byte"""
+	class GetStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Int_Value: int: decimal Target_RSSI index 0 to 90: map to -110 dBm to -20 dBm 91-126: reserved 127: station is commanded to transmit at maximum power for the assigned MCS Range: 0 to 127
+			- Dbm_Value: int: decimal Target_RSSI value Range: -110 dBm to -20 dBm"""
 		__meta_args_list = [
-			ArgStruct.scalar_enum('Enable', enums.EnableState),
-			ArgStruct.scalar_enum('Multi_Tid', enums.EnableState),
-			ArgStruct.scalar_int('Max_Length')]
+			ArgStruct.scalar_int('Int_Value'),
+			ArgStruct.scalar_int('Dbm_Value')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Enable: enums.EnableState = None
-			self.Multi_Tid: enums.EnableState = None
-			self.Max_Length: int = None
-
-	def set(self, structure: AmpduStruct, station=repcap.Station.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:AMPDu \n
-		Snippet: driver.configure.sta.connection.ampdu.set(value = [PROPERTY_STRUCT_NAME](), station = repcap.Station.Default) \n
-		Configures aggregate MPDUs (A-MPDU) . \n
-			:param structure: for set value, see the help for AmpduStruct structure arguments.
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:AMPDu', structure)
-
-	def get(self, station=repcap.Station.Default) -> AmpduStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:AMPDu \n
-		Snippet: value: AmpduStruct = driver.configure.sta.connection.ampdu.get(station = repcap.Station.Default) \n
-		Configures aggregate MPDUs (A-MPDU) . \n
+			self.Int_Value: int = None
+			self.Dbm_Value: int = None
+
+	def get(self, station=repcap.Station.Default) -> GetStruct:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:TRSSi \n
+		Snippet: value: GetStruct = driver.configure.sta.connection.hetf.trssi.get(station = repcap.Station.Default) \n
+		Specifies the expected Rx power of HE TB PPDU transmission as a response to trigger frame. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:return: structure: for return value, see the help for AmpduStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:AMPDu?', self.__class__.AmpduStruct())
+			:return: structure: for return value, see the help for GetStruct structure arguments."""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:TRSSi?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Dfdef.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Dfdef.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,45 +3,45 @@
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
 from ..... import enums
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dfdef:
-	"""Dfdef commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class DfdefCls:
+	"""Dfdef commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dfdef", core, parent)
+		self._cmd_group = CommandsGroup("dfdef", core, parent)
 
 	# noinspection PyTypeChecker
 	class DfdefStruct(StructBase):
 		"""Structure for setting input parameters. Contains optional setting parameters. Fields: \n
 			- State: enums.EnableState: DISable | ENABle Disables/enables the user-defined frame rate control
 			- Format_Py: enums.DataFormatExt: NHT | HTM | VHT | HES | HEM Selects the frame format NHT: non-high throughput format (non-HT) HTM: HT mixed format (HT MF) VHT: very high throughput format HES: high efficiency single-user format (HE SU) HEM: high efficiency multi-user format (HE MU)
-			- Chan_Bw: enums.ChannelBandwidthDut: BW20 | BW40 | BW80 | BW160 Channel bandwidth The value must not exceed the operating channel bandwidth, see [CMDLINK: CONFigure:WLAN:SIGNi:RFSettings:OCWidth CMDLINK].
-			- Rate: enums.Coderate: D1MBit | D2MBits | C55Mbits | C11Mbits | BR12 | BR34 | QR12 | QR34 | Q1M12 | Q1M34 | Q6M23 | Q6M34 | MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 | MCS12 | MCS13 | MCS14 | MCS15 See rate list in [CMDLINK: CONFigure:WLAN:SIGNi:CONNection:MFDef CMDLINK]
+			- Chan_Bw: enums.ChannelBandwidthDut: BW20 | BW40 | BW80 | BW160 Channel bandwidth The value must not exceed the operating channel bandwidth, see [CMDLINKRESOLVED Configure.RfSettings#OcWidth CMDLINKRESOLVED].
+			- Rate: enums.Coderate: D1MBit | D2MBits | C55Mbits | C11Mbits | BR12 | BR34 | QR12 | QR34 | Q1M12 | Q1M34 | Q6M23 | Q6M34 | MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 | MCS12 | MCS13 | MCS14 | MCS15 See rate list in [CMDLINKRESOLVED Configure.Connection.MfDef#set CMDLINKRESOLVED]
 			- Guard_Interval: enums.GuardInterval: Optional setting parameter. LONG | SHORt | GI08 | GI16 | GI32 SHORt, LONG: short or long guard interval (up to 802.11ac) GI08, GI16, GI32: 0.8 μs, 1.6 μs, and 3.2 μs guard interval durations (for 802.11ax)
 			- Ltf_Type: enums.LtfType: Optional setting parameter. X1 | X2 | X4 1x HE-LTF, 2x HE-LTF, 4x HE-LTF for 802.11ax
 			- Pe_Duration: enums.PeDuration: Optional setting parameter. PE0 | PE4 | PE8 | PE12 | PE16 | AUTO PEx: additional receive processing time of x μs signaled in packet extension (PE) field (only for 802.11ax) AUTO: automatic setting based on the reported DUTs capabilities
 			- Ctype: enums.CodingType: Optional setting parameter. LDPC | BCC Coding type (for 802.11ax - VHT, HE_SU, HE_MU frames only) : low density parity check or binary convolution code
 			- Streams: enums.Streams: Optional setting parameter. STR1 | STR2 Number of streams
 			- Stbc: bool: Optional setting parameter. OFF | ON Enables / disables space time block coding (STBC) . If disabled, spatial multiplexing is used."""
 		__meta_args_list = [
 			ArgStruct.scalar_enum('State', enums.EnableState),
 			ArgStruct.scalar_enum('Format_Py', enums.DataFormatExt),
 			ArgStruct.scalar_enum('Chan_Bw', enums.ChannelBandwidthDut),
 			ArgStruct.scalar_enum('Rate', enums.Coderate),
-			ArgStruct.scalar_enum('Guard_Interval', enums.GuardInterval),
-			ArgStruct.scalar_enum('Ltf_Type', enums.LtfType),
-			ArgStruct.scalar_enum('Pe_Duration', enums.PeDuration),
-			ArgStruct.scalar_enum('Ctype', enums.CodingType),
-			ArgStruct.scalar_enum('Streams', enums.Streams),
-			ArgStruct.scalar_bool('Stbc')]
+			ArgStruct.scalar_enum_optional('Guard_Interval', enums.GuardInterval),
+			ArgStruct.scalar_enum_optional('Ltf_Type', enums.LtfType),
+			ArgStruct.scalar_enum_optional('Pe_Duration', enums.PeDuration),
+			ArgStruct.scalar_enum_optional('Ctype', enums.CodingType),
+			ArgStruct.scalar_enum_optional('Streams', enums.Streams),
+			ArgStruct.scalar_bool_optional('Stbc')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.State: enums.EnableState = None
 			self.Format_Py: enums.DataFormatExt = None
 			self.Chan_Bw: enums.ChannelBandwidthDut = None
 			self.Rate: enums.Coderate = None
@@ -50,22 +50,35 @@
 			self.Pe_Duration: enums.PeDuration = None
 			self.Ctype: enums.CodingType = None
 			self.Streams: enums.Streams = None
 			self.Stbc: bool = None
 
 	def set(self, structure: DfdefStruct, station=repcap.Station.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:DFDef \n
-		Snippet: driver.configure.sta.connection.dfdef.set(value = [PROPERTY_STRUCT_NAME](), station = repcap.Station.Default) \n
+		Snippet with structure: \n
+		structure = driver.configure.sta.connection.dfdef.DfdefStruct() \n
+		structure.State: enums.EnableState = enums.EnableState.DISable \n
+		structure.Format_Py: enums.DataFormatExt = enums.DataFormatExt.HEES \n
+		structure.Chan_Bw: enums.ChannelBandwidthDut = enums.ChannelBandwidthDut.BW160 \n
+		structure.Rate: enums.Coderate = enums.Coderate.BR12 \n
+		structure.Guard_Interval: enums.GuardInterval = enums.GuardInterval.GI08 \n
+		structure.Ltf_Type: enums.LtfType = enums.LtfType.X1 \n
+		structure.Pe_Duration: enums.PeDuration = enums.PeDuration.AUTO \n
+		structure.Ctype: enums.CodingType = enums.CodingType.BCC \n
+		structure.Streams: enums.Streams = enums.Streams.STR1 \n
+		structure.Stbc: bool = False \n
+		driver.configure.sta.connection.dfdef.set(structure, station = repcap.Station.Default) \n
 		Enables and configures the user-defined frame rate control for data frames. \n
 			:param structure: for set value, see the help for DfdefStruct structure arguments.
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:DFDef', structure)
 
 	def get(self, station=repcap.Station.Default) -> DfdefStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:DFDef \n
 		Snippet: value: DfdefStruct = driver.configure.sta.connection.dfdef.get(station = repcap.Station.Default) \n
 		Enables and configures the user-defined frame rate control for data frames. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for DfdefStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:DFDef?', self.__class__.DfdefStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hetf:
-	"""Hetf commands group definition. 9 total commands, 9 Sub-groups, 0 group commands"""
+class HetfCls:
+	"""Hetf commands group definition. 9 total commands, 9 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hetf", core, parent)
+		self._cmd_group = CommandsGroup("hetf", core, parent)
 
 	@property
 	def nss(self):
 		"""nss commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_nss'):
-			from .Hetf_.Nss import Nss
-			self._nss = Nss(self._core, self._base)
+			from .Nss import NssCls
+			self._nss = NssCls(self._core, self._cmd_group)
 		return self._nss
 
 	@property
 	def sss(self):
 		"""sss commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_sss'):
-			from .Hetf_.Sss import Sss
-			self._sss = Sss(self._core, self._base)
+			from .Sss import SssCls
+			self._sss = SssCls(self._core, self._cmd_group)
 		return self._sss
 
 	@property
 	def dcm(self):
 		"""dcm commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_dcm'):
-			from .Hetf_.Dcm import Dcm
-			self._dcm = Dcm(self._core, self._base)
+			from .Dcm import DcmCls
+			self._dcm = DcmCls(self._core, self._cmd_group)
 		return self._dcm
 
 	@property
 	def mcs(self):
 		"""mcs commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mcs'):
-			from .Hetf_.Mcs import Mcs
-			self._mcs = Mcs(self._core, self._base)
+			from .Mcs import McsCls
+			self._mcs = McsCls(self._core, self._cmd_group)
 		return self._mcs
 
 	@property
 	def ctyp(self):
 		"""ctyp commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ctyp'):
-			from .Hetf_.Ctyp import Ctyp
-			self._ctyp = Ctyp(self._core, self._base)
+			from .Ctyp import CtypCls
+			self._ctyp = CtypCls(self._core, self._cmd_group)
 		return self._ctyp
 
 	@property
 	def rual(self):
 		"""rual commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_rual'):
-			from .Hetf_.Rual import Rual
-			self._rual = Rual(self._core, self._base)
+			from .Rual import RualCls
+			self._rual = RualCls(self._core, self._cmd_group)
 		return self._rual
 
 	@property
 	def trssi(self):
 		"""trssi commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_trssi'):
-			from .Hetf_.Trssi import Trssi
-			self._trssi = Trssi(self._core, self._base)
+			from .Trssi import TrssiCls
+			self._trssi = TrssiCls(self._core, self._cmd_group)
 		return self._trssi
 
 	@property
 	def trsMode(self):
 		"""trsMode commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_trsMode'):
-			from .Hetf_.TrsMode import TrsMode
-			self._trsMode = TrsMode(self._core, self._base)
+			from .TrsMode import TrsModeCls
+			self._trsMode = TrsModeCls(self._core, self._cmd_group)
 		return self._trsMode
 
 	@property
 	def tsrControl(self):
 		"""tsrControl commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_tsrControl'):
-			from .Hetf_.TsrControl import TsrControl
-			self._tsrControl = TsrControl(self._core, self._base)
+			from .TsrControl import TsrControlCls
+			self._tsrControl = TsrControlCls(self._core, self._cmd_group)
 		return self._tsrControl
 
-	def clone(self) -> 'Hetf':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'HetfCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Hetf(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = HetfCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Ctyp.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Ctyp.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Ctyp:
-	"""Ctyp commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class CtypCls:
+	"""Ctyp commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ctyp", core, parent)
+		self._cmd_group = CommandsGroup("ctyp", core, parent)
 
 	def set(self, type_py: enums.CodingType, station=repcap.Station.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:CTYP \n
 		Snippet: driver.configure.sta.connection.hetf.ctyp.set(type_py = enums.CodingType.BCC, station = repcap.Station.Default) \n
 		Specifies the coding used by the HE TB PPDU. \n
 			:param type_py: BCC | LDPC
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
 		param = Conversions.enum_scalar_to_str(type_py, enums.CodingType)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:CTYP {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, station=repcap.Station.Default) -> enums.CodingType:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:CTYP \n
 		Snippet: value: enums.CodingType = driver.configure.sta.connection.hetf.ctyp.get(station = repcap.Station.Default) \n
 		Specifies the coding used by the HE TB PPDU. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: type_py: BCC | LDPC"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:CTYP?')
 		return Conversions.str_to_scalar_enum(response, enums.CodingType)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Dcm.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Nss.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Dcm:
-	"""Dcm commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class NssCls:
+	"""Nss commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("dcm", core, parent)
+		self._cmd_group = CommandsGroup("nss", core, parent)
 
-	def set(self, dcm: bool, station=repcap.Station.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:DCM \n
-		Snippet: driver.configure.sta.connection.hetf.dcm.set(dcm = False, station = repcap.Station.Default) \n
-		Specifies whether the HE TB response uses dual carrier modulation (DCM) . \n
-			:param dcm: OFF | ON
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		param = Conversions.bool_to_str(dcm)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:DCM {param}')
+	def set(self, number_ss: int, station=repcap.Station.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:NSS \n
+		Snippet: driver.configure.sta.connection.hetf.nss.set(number_ss = 1, station = repcap.Station.Default) \n
+		Sets the number of HE TB PPDU spatial streams. \n
+			:param number_ss: integer Range: 1 to 8
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		param = Conversions.decimal_value_to_str(number_ss)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:NSS {param}')
 
-	def get(self, station=repcap.Station.Default) -> bool:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:DCM \n
-		Snippet: value: bool = driver.configure.sta.connection.hetf.dcm.get(station = repcap.Station.Default) \n
-		Specifies whether the HE TB response uses dual carrier modulation (DCM) . \n
+	def get(self, station=repcap.Station.Default) -> int:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:NSS \n
+		Snippet: value: int = driver.configure.sta.connection.hetf.nss.get(station = repcap.Station.Default) \n
+		Sets the number of HE TB PPDU spatial streams. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:return: dcm: OFF | ON"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:DCM?')
-		return Conversions.str_to_bool(response)
+			:return: number_ss: integer Range: 1 to 8"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:NSS?')
+		return Conversions.str_to_int(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Mcs.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Dcm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
-from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mcs:
-	"""Mcs commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class DcmCls:
+	"""Dcm commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mcs", core, parent)
+		self._cmd_group = CommandsGroup("dcm", core, parent)
 
-	def set(self, mcs: enums.McsIndex, station=repcap.Station.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:MCS \n
-		Snippet: driver.configure.sta.connection.hetf.mcs.set(mcs = enums.McsIndex.MCS, station = repcap.Station.Default) \n
-		Specifies the modulation and coding scheme (MCS) used by the HE TB PPDU. \n
-			:param mcs: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		param = Conversions.enum_scalar_to_str(mcs, enums.McsIndex)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:MCS {param}')
+	def set(self, dcm: bool, station=repcap.Station.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:DCM \n
+		Snippet: driver.configure.sta.connection.hetf.dcm.set(dcm = False, station = repcap.Station.Default) \n
+		Specifies whether the HE TB response uses dual carrier modulation (DCM) . \n
+			:param dcm: OFF | ON
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		param = Conversions.bool_to_str(dcm)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:DCM {param}')
 
-	# noinspection PyTypeChecker
-	def get(self, station=repcap.Station.Default) -> enums.McsIndex:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:MCS \n
-		Snippet: value: enums.McsIndex = driver.configure.sta.connection.hetf.mcs.get(station = repcap.Station.Default) \n
-		Specifies the modulation and coding scheme (MCS) used by the HE TB PPDU. \n
+	def get(self, station=repcap.Station.Default) -> bool:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:DCM \n
+		Snippet: value: bool = driver.configure.sta.connection.hetf.dcm.get(station = repcap.Station.Default) \n
+		Specifies whether the HE TB response uses dual carrier modulation (DCM) . \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:return: mcs: MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 MCS, MCS1,...,MCS11: MCS 0 to MCS 11"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:MCS?')
-		return Conversions.str_to_scalar_enum(response, enums.McsIndex)
+			:return: dcm: OFF | ON"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:DCM?')
+		return Conversions.str_to_bool(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Nss.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Sss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Nss:
-	"""Nss commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class SssCls:
+	"""Sss commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("nss", core, parent)
-
-	def set(self, number_ss: int, station=repcap.Station.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:NSS \n
-		Snippet: driver.configure.sta.connection.hetf.nss.set(number_ss = 1, station = repcap.Station.Default) \n
-		Sets the number of HE TB PPDU spatial streams. \n
-			:param number_ss: integer Range: 1 to 8
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		param = Conversions.decimal_value_to_str(number_ss)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:NSS {param}')
+		self._cmd_group = CommandsGroup("sss", core, parent)
 
 	def get(self, station=repcap.Station.Default) -> int:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:NSS \n
-		Snippet: value: int = driver.configure.sta.connection.hetf.nss.get(station = repcap.Station.Default) \n
-		Sets the number of HE TB PPDU spatial streams. \n
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:SSS \n
+		Snippet: value: int = driver.configure.sta.connection.hetf.sss.get(station = repcap.Station.Default) \n
+		Sets the starting spatial stream for the HE TB PPDU. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:return: number_ss: integer Range: 1 to 8"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:NSS?')
+			:return: starting_ss: decimal Range: 1 to 8"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:SSS?')
 		return Conversions.str_to_int(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Rual.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Rual.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal.Types import DataType
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
+from ......Internal.ArgSingleList import ArgSingleList
+from ......Internal.ArgSingle import ArgSingle
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Rual:
-	"""Rual commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class RualCls:
+	"""Rual commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rual", core, parent)
+		self._cmd_group = CommandsGroup("rual", core, parent)
+
+	def set(self, ru_allocation: enums.RuAllocation, channel_80_mh_z: enums.Channel80MhZ = None, station=repcap.Station.Default) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:RUAL \n
+		Snippet: driver.configure.sta.connection.hetf.rual.set(ru_allocation = enums.RuAllocation.OFF, channel_80_mh_z = enums.Channel80MhZ.PRIMary, station = repcap.Station.Default) \n
+		Specifies the RU used by the HE TB PPDU. Refer to IEEE Std 802.11ax-2021, table 9-29i B7–B1 of the RU Allocation subfield. \n
+			:param ru_allocation: RU0 | RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9 | RU10 | RU11 | RU12 | RU13 | RU14 | RU15 | RU16 | RU17 | RU18 | RU19 | RU20 | RU21 | RU22 | RU23 | RU24 | RU25 | RU26 | RU27 | RU28 | RU29 | RU30 | RU31 | RU32 | RU33 | RU34 | RU35 | RU36 | RU37 | RU38 | RU39 | RU40 | RU41 | RU42 | RU43 | RU44 | RU45 | RU46 | RU47 | RU48 | RU49 | RU50 | RU51 | RU52 | RU53 | RU54 | RU55 | RU56 | RU57 | RU58 | RU59 | RU60 | RU61 | RU62 | RU63 | RU64 | RU65 | RU66 | RU67 | RU68 | OFF 'OFF': No resource unit for the specified station is allocated 'RUx': Bits 7 to 1 of the RU allocation subfield, see table below.
+			:param channel_80_mh_z: PRIMary | SECondary For RU67 and RU68 applying 160 MHz channel, sets the bit 0 of the RU allocation subfield that indicates primary 80 MHz or secondary 80 MHz channel.
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('ru_allocation', ru_allocation, DataType.Enum, enums.RuAllocation), ArgSingle('channel_80_mh_z', channel_80_mh_z, DataType.Enum, enums.Channel80MhZ, is_optional=True))
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:RUAL {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class RualStruct(StructBase):
-		"""Structure for setting input parameters. Contains optional setting parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- Ru_Allocation: enums.RuAllocation: RU0 | RU1 | RU2 | RU3 | RU4 | RU5 | RU6 | RU7 | RU8 | RU9 | RU10 | RU11 | RU12 | RU13 | RU14 | RU15 | RU16 | RU17 | RU18 | RU19 | RU20 | RU21 | RU22 | RU23 | RU24 | RU25 | RU26 | RU27 | RU28 | RU29 | RU30 | RU31 | RU32 | RU33 | RU34 | RU35 | RU36 | RU37 | RU38 | RU39 | RU40 | RU41 | RU42 | RU43 | RU44 | RU45 | RU46 | RU47 | RU48 | RU49 | RU50 | RU51 | RU52 | RU53 | RU54 | RU55 | RU56 | RU57 | RU58 | RU59 | RU60 | RU61 | RU62 | RU63 | RU64 | RU65 | RU66 | RU67 | RU68 | OFF 'OFF': No resource unit for the specified station is allocated 'RUx': Bits 7 to 1 of the RU allocation subfield, see table below.
-			- Channel_80_Mh_Z: enums.Channel80MhZ: Optional setting parameter. PRIMary | SECondary For RU67 and RU68 applying 160 MHz channel, sets the bit 0 of the RU allocation subfield that indicates primary 80 MHz or secondary 80 MHz channel."""
+			- Channel_80_Mh_Z: enums.Channel80MhZ: PRIMary | SECondary For RU67 and RU68 applying 160 MHz channel, sets the bit 0 of the RU allocation subfield that indicates primary 80 MHz or secondary 80 MHz channel."""
 		__meta_args_list = [
 			ArgStruct.scalar_enum('Ru_Allocation', enums.RuAllocation),
 			ArgStruct.scalar_enum('Channel_80_Mh_Z', enums.Channel80MhZ)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Ru_Allocation: enums.RuAllocation = None
 			self.Channel_80_Mh_Z: enums.Channel80MhZ = None
 
-	def set(self, structure: RualStruct, station=repcap.Station.Default) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:RUAL \n
-		Snippet: driver.configure.sta.connection.hetf.rual.set(value = [PROPERTY_STRUCT_NAME](), station = repcap.Station.Default) \n
-		Specifies the RU used by the HE TB PPDU. Refer to IEEE P802.11ax/D8.0, table 9-29i B7–B1 of the RU Allocation subfield. \n
-			:param structure: for set value, see the help for RualStruct structure arguments.
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:RUAL', structure)
-
 	def get(self, station=repcap.Station.Default) -> RualStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:RUAL \n
 		Snippet: value: RualStruct = driver.configure.sta.connection.hetf.rual.get(station = repcap.Station.Default) \n
-		Specifies the RU used by the HE TB PPDU. Refer to IEEE P802.11ax/D8.0, table 9-29i B7–B1 of the RU Allocation subfield. \n
+		Specifies the RU used by the HE TB PPDU. Refer to IEEE Std 802.11ax-2021, table 9-29i B7–B1 of the RU Allocation subfield. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for RualStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:RUAL?', self.__class__.RualStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Sss.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxbPower.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ...... import repcap
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sss:
-	"""Sss commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class RxbPowerCls:
+	"""RxbPower commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sss", core, parent)
+		self._cmd_group = CommandsGroup("rxbPower", core, parent)
 
-	def get(self, station=repcap.Station.Default) -> int:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:SSS \n
-		Snippet: value: int = driver.configure.sta.connection.hetf.sss.get(station = repcap.Station.Default) \n
-		Sets the starting spatial stream for the HE TB PPDU. \n
+	def get(self, station=repcap.Station.Default) -> float:
+		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXBPower \n
+		Snippet: value: float = driver.sense.sta.uesInfo.rxbPower.get(station = repcap.Station.Default) \n
+		Queries the average power of the last burst received from the DUT. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:return: starting_ss: decimal Range: 1 to 8"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:SSS?')
-		return Conversions.str_to_int(response)
+			:return: power: float Unit: dBm"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		response = self._core.io.query_str(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXBPower?')
+		return Conversions.str_to_float(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/TrsMode.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/TrsMode.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class TrsMode:
-	"""TrsMode commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class TrsModeCls:
+	"""TrsMode commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("trsMode", core, parent)
+		self._cmd_group = CommandsGroup("trsMode", core, parent)
 
 	def set(self, mode: enums.TriggerFrmPowerMode, station=repcap.Station.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:TRSMode \n
 		Snippet: driver.configure.sta.connection.hetf.trsMode.set(mode = enums.TriggerFrmPowerMode.AUTO, station = repcap.Station.Default) \n
 		Specifies the trigger frame power control mode. \n
 			:param mode: AUTO | MANual | MAXPower AUTO: AP_TX_Power and Target_RSSI calculated automatically MAN: The value Target RSSI Control defines adjustment to the Target_RSSI calculation MAXP: Sets the Target_RSSI to 127, the UE transmits the HE TB PPDU at maximum Tx power
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
 		param = Conversions.enum_scalar_to_str(mode, enums.TriggerFrmPowerMode)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:TRSMode {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, station=repcap.Station.Default) -> enums.TriggerFrmPowerMode:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:TRSMode \n
 		Snippet: value: enums.TriggerFrmPowerMode = driver.configure.sta.connection.hetf.trsMode.get(station = repcap.Station.Default) \n
 		Specifies the trigger frame power control mode. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: mode: AUTO | MANual | MAXPower AUTO: AP_TX_Power and Target_RSSI calculated automatically MAN: The value Target RSSI Control defines adjustment to the Target_RSSI calculation MAXP: Sets the Target_RSSI to 127, the UE transmits the HE TB PPDU at maximum Tx power"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:TRSMode?')
 		return Conversions.str_to_scalar_enum(response, enums.TriggerFrmPowerMode)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Trssi.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/Mac/Address.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal.StructBase import StructBase
-from ......Internal.ArgStruct import ArgStruct
+from ......Internal.Utilities import trim_str_response
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Trssi:
-	"""Trssi commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class AddressCls:
+	"""Address commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("trssi", core, parent)
+		self._cmd_group = CommandsGroup("address", core, parent)
 
-	# noinspection PyTypeChecker
-	class GetStruct(StructBase):
-		"""Response structure. Fields: \n
-			- Int_Value: int: decimal Target_RSSI index 0 to 90: map to -110 dBm to -20 dBm 91-126: reserved 127: station is commanded to transmit at maximum power for the assigned MCS Range: 0 to 127
-			- Dbm_Value: int: decimal Target_RSSI value Range: -110 dBm to -20 dBm"""
-		__meta_args_list = [
-			ArgStruct.scalar_int('Int_Value'),
-			ArgStruct.scalar_int('Dbm_Value')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Int_Value: int = None
-			self.Dbm_Value: int = None
-
-	def get(self, station=repcap.Station.Default) -> GetStruct:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:TRSSi \n
-		Snippet: value: GetStruct = driver.configure.sta.connection.hetf.trssi.get(station = repcap.Station.Default) \n
-		Specifies the expected Rx power of HE TB PPDU transmission as a response to trigger frame. \n
+	def get(self, station=repcap.Station.Default) -> str:
+		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UECapability:MAC:ADDRess \n
+		Snippet: value: str = driver.sense.sta.ueCapability.mac.address.get(station = repcap.Station.Default) \n
+		Gets the MAC address of an associated DUT. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:TRSSi?', self.__class__.GetStruct())
+			:return: mac_address: string Hexadecimal MAC address as string"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		response = self._core.io.query_str(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UECapability:MAC:ADDRess?')
+		return trim_str_response(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/TsrControl.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/TsrControl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class TsrControl:
-	"""TsrControl commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class TsrControlCls:
+	"""TsrControl commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("tsrControl", core, parent)
+		self._cmd_group = CommandsGroup("tsrControl", core, parent)
 
 	def set(self, pwr_db: int, station=repcap.Station.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:TSRControl \n
 		Snippet: driver.configure.sta.connection.hetf.tsrControl.set(pwr_db = 1, station = repcap.Station.Default) \n
 		Specifies the value Target RSSI Control for adjustment to the Target_RSSI. This parameter is only relevant in manual mode
 		for target RSSI calculation. \n
 			:param pwr_db: integer Range: -40 dB to 0 dB
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
 		param = Conversions.decimal_value_to_str(pwr_db)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:TSRControl {param}')
 
 	def get(self, station=repcap.Station.Default) -> int:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:HETF:TSRControl \n
 		Snippet: value: int = driver.configure.sta.connection.hetf.tsrControl.get(station = repcap.Station.Default) \n
 		Specifies the value Target RSSI Control for adjustment to the Target_RSSI. This parameter is only relevant in manual mode
 		for target RSSI calculation. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: pwr_db: integer Range: -40 dB to 0 dB"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:HETF:TSRControl?')
 		return Conversions.str_to_int(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Third/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Qos:
-	"""Qos commands group definition. 2 total commands, 2 Sub-groups, 0 group commands"""
+class ThirdCls:
+	"""Third commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("qos", core, parent)
+		self._cmd_group = CommandsGroup("third", core, parent)
 
 	@property
-	def barMethod(self):
-		"""barMethod commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_barMethod'):
-			from .Qos_.BarMethod import BarMethod
-			self._barMethod = BarMethod(self._core, self._base)
-		return self._barMethod
+	def state(self):
+		"""state commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_state'):
+			from .State import StateCls
+			self._state = StateCls(self._core, self._cmd_group)
+		return self._state
 
-	@property
-	def black(self):
-		"""black commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_black'):
-			from .Qos_.Black import Black
-			self._black = Black(self._core, self._base)
-		return self._black
-
-	def clone(self) -> 'Qos':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'ThirdCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Qos(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = ThirdCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/BarMethod.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/BarMethod.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class BarMethod:
-	"""BarMethod commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class BarMethodCls:
+	"""BarMethod commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("barMethod", core, parent)
+		self._cmd_group = CommandsGroup("barMethod", core, parent)
 
 	def set(self, method: enums.BarMethod, station=repcap.Station.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:QOS:BARMethod \n
 		Snippet: driver.configure.sta.connection.qos.barMethod.set(method = enums.BarMethod.EXPBar, station = repcap.Station.Default) \n
 		Specifies the method used to request a BlockAck frame from the DUT \n
 			:param method: IMPBar | EXPBar | MUBar Implicit, explicit or multi-user block acknowledgment request
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
 		param = Conversions.enum_scalar_to_str(method, enums.BarMethod)
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:QOS:BARMethod {param}')
 
 	# noinspection PyTypeChecker
 	def get(self, station=repcap.Station.Default) -> enums.BarMethod:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:QOS:BARMethod \n
 		Snippet: value: enums.BarMethod = driver.configure.sta.connection.qos.barMethod.get(station = repcap.Station.Default) \n
 		Specifies the method used to request a BlockAck frame from the DUT \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: method: IMPBar | EXPBar | MUBar Implicit, explicit or multi-user block acknowledgment request"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		response = self._core.io.query_str(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:QOS:BARMethod?')
 		return Conversions.str_to_scalar_enum(response, enums.BarMethod)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/Black.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/Black.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Black:
-	"""Black commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class BlackCls:
+	"""Black commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("black", core, parent)
+		self._cmd_group = CommandsGroup("black", core, parent)
 
 	# noinspection PyTypeChecker
 	class BlackStruct(StructBase):
 		"""Structure for setting input parameters. Fields: \n
 			- Tid_0: bool: No parameter help available
 			- Tid_1: bool: No parameter help available
 			- Tid_2: bool: No parameter help available
@@ -43,22 +43,33 @@
 			self.Tid_4: bool = None
 			self.Tid_5: bool = None
 			self.Tid_6: bool = None
 			self.Tid_7: bool = None
 
 	def set(self, structure: BlackStruct, station=repcap.Station.Default) -> None:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:QOS:BLACk \n
-		Snippet: driver.configure.sta.connection.qos.black.set(value = [PROPERTY_STRUCT_NAME](), station = repcap.Station.Default) \n
+		Snippet with structure: \n
+		structure = driver.configure.sta.connection.qos.black.BlackStruct() \n
+		structure.Tid_0: bool = False \n
+		structure.Tid_1: bool = False \n
+		structure.Tid_2: bool = False \n
+		structure.Tid_3: bool = False \n
+		structure.Tid_4: bool = False \n
+		structure.Tid_5: bool = False \n
+		structure.Tid_6: bool = False \n
+		structure.Tid_7: bool = False \n
+		driver.configure.sta.connection.qos.black.set(structure, station = repcap.Station.Default) \n
 		Enables/ disables a block ack session per TID (8 values) . \n
 			:param structure: for set value, see the help for BlackStruct structure arguments.
-			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')"""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
+		"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		self._core.io.write_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:QOS:BLACk', structure)
 
 	def get(self, station=repcap.Station.Default) -> BlackStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:STA<s>:CONNection:QOS:BLACk \n
 		Snippet: value: BlackStruct = driver.configure.sta.connection.qos.black.get(station = repcap.Station.Default) \n
 		Enables/ disables a block ack session per TID (8 values) . \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for BlackStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:CONNection:QOS:BLACk?', self.__class__.BlackStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Configure_/UesInfo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/UesInfo/Settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,47 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal.StructBase import StructBase
-from ...Internal.ArgStruct import ArgStruct
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Types import DataType
+from ....Internal.StructBase import StructBase
+from ....Internal.ArgStruct import ArgStruct
+from ....Internal.ArgSingleList import ArgSingleList
+from ....Internal.ArgSingle import ArgSingle
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UesInfo:
-	"""UesInfo commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class SettingsCls:
+	"""Settings commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uesInfo", core, parent)
+		self._cmd_group = CommandsGroup("settings", core, parent)
 
-	def reset(self) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:UESinfo:RESet \n
-		Snippet: driver.configure.uesInfo.reset() \n
-		Clears entries in all statistic tables concerning user data traffic. \n
-		"""
-		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:UESinfo:RESet')
-
-	def reset_with_opc(self) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:UESinfo:RESet \n
-		Snippet: driver.configure.uesInfo.reset_with_opc() \n
-		Clears entries in all statistic tables concerning user data traffic. \n
-		Same as reset, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
+	def set(self, reporting_interval: float, time_span: int) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:UESinfo:SETTings \n
+		Snippet: driver.configure.uesInfo.settings.set(reporting_interval = 1.0, time_span = 1) \n
+		Sets reporting interval and time span used for enhanced statistics of user data traffic. \n
+			:param reporting_interval: float Range: 0.2 s to 5 s
+			:param time_span: integer Range: 1 to 1500
 		"""
-		self._core.io.write_with_opc(f'CONFigure:WLAN:SIGNaling<Instance>:UESinfo:RESet')
+		param = ArgSingleList().compose_cmd_string(ArgSingle('reporting_interval', reporting_interval, DataType.Float), ArgSingle('time_span', time_span, DataType.Integer))
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:UESinfo:SETTings {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class SettingsStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+		"""Response structure. Fields: \n
 			- Reporting_Interval: float: float Range: 0.2 s to 5 s
 			- Time_Span: int: integer Range: 1 to 1500"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Reporting_Interval'),
 			ArgStruct.scalar_int('Time_Span')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reporting_Interval: float = None
 			self.Time_Span: int = None
 
-	def get_settings(self) -> SettingsStruct:
+	def get(self) -> SettingsStruct:
 		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:UESinfo:SETTings \n
-		Snippet: value: SettingsStruct = driver.configure.uesInfo.get_settings() \n
+		Snippet: value: SettingsStruct = driver.configure.uesInfo.settings.get() \n
 		Sets reporting interval and time span used for enhanced statistics of user data traffic. \n
-			:return: structure: for return value, see the help for SettingsStruct structure arguments.
-		"""
-		return self._core.io.query_struct('CONFigure:WLAN:SIGNaling<Instance>:UESinfo:SETTings?', self.__class__.SettingsStruct())
-
-	def set_settings(self, value: SettingsStruct) -> None:
-		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:UESinfo:SETTings \n
-		Snippet: driver.configure.uesInfo.set_settings(value = SettingsStruct()) \n
-		Sets reporting interval and time span used for enhanced statistics of user data traffic. \n
-			:param value: see the help for SettingsStruct structure arguments.
-		"""
-		self._core.io.write_struct('CONFigure:WLAN:SIGNaling<Instance>:UESinfo:SETTings', value)
+			:return: structure: for return value, see the help for SettingsStruct structure arguments."""
+		return self._core.io.query_struct(f'CONFigure:WLAN:SIGNaling<Instance>:UESinfo:SETTings?', self.__class__.SettingsStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/HetBased.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/HetBased/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class HetBased:
-	"""HetBased commands group definition. 5 total commands, 2 Sub-groups, 3 group commands"""
+class HetBasedCls:
+	"""HetBased commands group definition. 5 total commands, 2 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hetBased", core, parent)
+		self._cmd_group = CommandsGroup("hetBased", core, parent)
 
 	@property
 	def state(self):
 		"""state commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_state'):
-			from .HetBased_.State import State
-			self._state = State(self._core, self._base)
+			from .State import StateCls
+			self._state = StateCls(self._core, self._cmd_group)
 		return self._state
 
 	@property
 	def uphInfo(self):
 		"""uphInfo commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_uphInfo'):
-			from .HetBased_.UphInfo import UphInfo
-			self._uphInfo = UphInfo(self._core, self._base)
+			from .UphInfo import UphInfoCls
+			self._uphInfo = UphInfoCls(self._core, self._cmd_group)
 		return self._uphInfo
 
 	def initiate(self) -> None:
 		"""SCPI: INITiate:WLAN:SIGNaling<instance>:HETBased \n
 		Snippet: driver.hetBased.initiate() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		"""
 		self._core.io.write(f'INITiate:WLAN:SIGNaling<Instance>:HETBased')
 
-	def initiate_with_opc(self) -> None:
+	def initiate_with_opc(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: INITiate:WLAN:SIGNaling<instance>:HETBased \n
 		Snippet: driver.hetBased.initiate_with_opc() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		Same as initiate, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'INITiate:WLAN:SIGNaling<Instance>:HETBased')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'INITiate:WLAN:SIGNaling<Instance>:HETBased', opc_timeout_ms)
 
 	def stop(self) -> None:
 		"""SCPI: STOP:WLAN:SIGNaling<instance>:HETBased \n
 		Snippet: driver.hetBased.stop() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		"""
 		self._core.io.write(f'STOP:WLAN:SIGNaling<Instance>:HETBased')
 
-	def stop_with_opc(self) -> None:
+	def stop_with_opc(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: STOP:WLAN:SIGNaling<instance>:HETBased \n
 		Snippet: driver.hetBased.stop_with_opc() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		Same as stop, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'STOP:WLAN:SIGNaling<Instance>:HETBased')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'STOP:WLAN:SIGNaling<Instance>:HETBased', opc_timeout_ms)
 
 	def abort(self) -> None:
 		"""SCPI: ABORt:WLAN:SIGNaling<instance>:HETBased \n
 		Snippet: driver.hetBased.abort() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		"""
 		self._core.io.write(f'ABORt:WLAN:SIGNaling<Instance>:HETBased')
 
-	def abort_with_opc(self) -> None:
+	def abort_with_opc(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: ABORt:WLAN:SIGNaling<instance>:HETBased \n
 		Snippet: driver.hetBased.abort_with_opc() \n
 			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
 			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 		Same as abort, but waits for the operation to complete before continuing further. Use the RsCmwWlanSig.utilities.opc_timeout_set() to set the timeout value. \n
-		"""
-		self._core.io.write_with_opc(f'ABORt:WLAN:SIGNaling<Instance>:HETBased')
+			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
+		self._core.io.write_with_opc(f'ABORt:WLAN:SIGNaling<Instance>:HETBased', opc_timeout_ms)
 
-	def clone(self) -> 'HetBased':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'HetBasedCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = HetBased(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = HetBasedCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/HetBased_/State.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/HetBased/State.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 from ...Internal import Conversions
 from ... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class State:
-	"""State commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class StateCls:
+	"""State commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("state", core, parent)
+		self._cmd_group = CommandsGroup("state", core, parent)
 
 	# noinspection PyTypeChecker
 	def fetch(self) -> enums.HeTbMainMeasState:
 		"""SCPI: FETCh:WLAN:SIGNaling<instance>:HETBased:STATe \n
 		Snippet: value: enums.HeTbMainMeasState = driver.hetBased.state.fetch() \n
 		Queries the main measurement state. Use FETCh:...:STATe:ALL? to query the measurement state including the substates. Use
 		INITiate..., STOP..., ABORt... to change the measurement state. \n
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/HetBased_/UphInfo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/HetBased/UphInfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from ...Internal.CommandsGroup import CommandsGroup
 from ...Internal.Types import DataType
 from ...Internal.StructBase import StructBase
 from ...Internal.ArgStruct import ArgStruct
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UphInfo:
-	"""UphInfo commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class UphInfoCls:
+	"""UphInfo commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uphInfo", core, parent)
+		self._cmd_group = CommandsGroup("uphInfo", core, parent)
 
 	# noinspection PyTypeChecker
 	class FetchStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Burst_Power: List[float]: float Measured burst power in uplink Range: -999 dBm to 999 dBm, Unit: dBm
 			- Uph: List[int]: decimal UL power headroom Range: 0 dB to 31 dB, Unit: dB
 			- Min_Tx_Power_Flag: List[bool]: OFF | ON Indication whether the HE TB bursts are sent at the minimum transmit power of the station
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/PackRate.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/PackRate.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from ..Internal import Conversions
 from ..Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from ..Internal.Types import DataType
 from .. import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class PackRate:
-	"""PackRate commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class PackRateCls:
+	"""PackRate commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("packRate", core, parent)
+		self._cmd_group = CommandsGroup("packRate", core, parent)
 
 	# noinspection PyTypeChecker
 	def fetch(self) -> enums.Coderate:
 		"""SCPI: FETCh:WLAN:SIGNaling<instance>:PACKrate \n
 		Snippet: value: enums.Coderate = driver.packRate.fetch() \n
 		Returns the modulation and coding rate/scheme of the last received ACK frame. \n
 		Use RsCmwWlanSig.reliability.last_value to read the updated reliability indicator. \n
-			:return: rate: BR12 | QR12 | QR34 | Q1M12 | Q1M34 | Q6M23 | Q6M34 | BR34 | MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | D1MBit | D2MBits | C55Mbits | C11Mbits | MCS8 | MCS9 | MCS10 | MCS11 | MCS12 | MCS13 | MCS14 | MCS15 See rate list in method RsCmwWlanSig.Configure.Connection.mfDef"""
+			:return: rate: BR12 | QR12 | QR34 | Q1M12 | Q1M34 | Q6M23 | Q6M34 | BR34 | MCS | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | D1MBit | D2MBits | C55Mbits | C11Mbits | MCS8 | MCS9 | MCS10 | MCS11 | MCS12 | MCS13 | MCS14 | MCS15 See rate list in method RsCmwWlanSig.Configure.Connection.MfDef.set"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:WLAN:SIGNaling<Instance>:PACKrate?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.Coderate)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per_/State.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Per/State/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal import Conversions
-from ... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
+from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class State:
-	"""State commands group definition. 2 total commands, 1 Sub-groups, 1 group commands"""
+class StateCls:
+	"""State commands group definition. 2 total commands, 1 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("state", core, parent)
+		self._cmd_group = CommandsGroup("state", core, parent)
 
 	@property
 	def all(self):
 		"""all commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_all'):
-			from .State_.All import All
-			self._all = All(self._core, self._base)
+			from .All import AllCls
+			self._all = AllCls(self._core, self._cmd_group)
 		return self._all
 
 	# noinspection PyTypeChecker
 	def fetch(self) -> enums.ResourceState:
 		"""SCPI: FETCh:WLAN:SIGNaling<instance>:PER:STATe \n
 		Snippet: value: enums.ResourceState = driver.per.state.fetch() \n
 		Queries the main measurement state. Use FETCh:...:STATe:ALL? to query the measurement state including the substates. Use
 		INITiate..., STOP..., ABORt... to change the measurement state. \n
 			:return: state: OFF | RDY | RUN OFF: measurement switched off, no resources allocated, no results available (when entered after ABORt...) RDY: measurement has been terminated, valid results can be available RUN: measurement running (after INITiate..., READ...) , synchronization pending or adjusted, resources active or queued"""
 		response = self._core.io.query_str(f'FETCh:WLAN:SIGNaling<Instance>:PER:STATe?')
 		return Conversions.str_to_scalar_enum(response, enums.ResourceState)
 
-	def clone(self) -> 'State':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'StateCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = State(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = StateCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Per_/State_/All.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Per/State/All.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal.StructBase import StructBase
 from ....Internal.ArgStruct import ArgStruct
 from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class All:
-	"""All commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class AllCls:
+	"""All commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("all", core, parent)
+		self._cmd_group = CommandsGroup("all", core, parent)
 
 	# noinspection PyTypeChecker
 	class FetchStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Main_State: enums.ResourceState: OFF | RDY | RUN OFF: measurement switched off, no resources allocated, no results available (when entered after STOP...) RDY: measurement has been terminated, valid results can be available RUN: measurement running (after INITiate..., READ...) , synchronization pending or adjusted, resources active or queued
 			- Sync_State: enums.ResourceState: PEND | ADJ | INV PEND: waiting for resource allocation, adjustment, hardware switching ('pending') ADJ: all necessary adjustments finished, measurement running ('adjusted') INV: not applicable because main_state: OFF or RDY ('invalid')
 			- Resource_State: enums.ResourceState: QUE | ACT | INV QUE: measurement without resources, no results available ('queued') ACT: resources allocated, acquisition of results in progress but not complete ('active') INV: not applicable because main_state: OFF or RDY ('invalid')"""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Pswitched.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Second/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Pswitched:
-	"""Pswitched commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class SecondCls:
+	"""Second commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("pswitched", core, parent)
+		self._cmd_group = CommandsGroup("second", core, parent)
 
 	@property
 	def state(self):
 		"""state commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_state'):
-			from .Pswitched_.State import State
-			self._state = State(self._core, self._base)
+			from .State import StateCls
+			self._state = StateCls(self._core, self._cmd_group)
 		return self._state
 
-	def clone(self) -> 'Pswitched':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SecondCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Pswitched(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SecondCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Pswitched_/State.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Pswitched/State.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 from ...Internal import Conversions
 from ... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class State:
-	"""State commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class StateCls:
+	"""State commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("state", core, parent)
+		self._cmd_group = CommandsGroup("state", core, parent)
 
 	# noinspection PyTypeChecker
 	def fetch(self) -> enums.PsState:
 		"""SCPI: FETCh:WLAN:SIGNaling<instance>:PSWitched:STATe \n
 		Snippet: value: enums.PsState = driver.pswitched.state.fetch() \n
-		Gets the connection status, refer to 'Connection Status'. Commands for station one, two and three are available. \n
+		Gets the connection status, refer to 'Connection status'. Commands for station one, two and three are available. \n
 			:return: ps_state: IDLE | PROBed | AUTHenticated | ASSociated | DEAuthenticated | DISassociated | CTIMeout"""
 		response = self._core.io.query_str(f'FETCh:WLAN:SIGNaling<Instance>:PSWitched:STATe?')
 		return Conversions.str_to_scalar_enum(response, enums.PsState)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
-from ..Internal.StructBase import StructBase
-from ..Internal.ArgStruct import ArgStruct
-from .. import enums
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
+from ...Internal.StructBase import StructBase
+from ...Internal.ArgStruct import ArgStruct
+from ... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Route:
-	"""Route commands group definition. 6 total commands, 1 Sub-groups, 1 group commands"""
+class RouteCls:
+	"""Route commands group definition. 6 total commands, 1 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("route", core, parent)
+		self._cmd_group = CommandsGroup("route", core, parent)
 
 	@property
 	def scenario(self):
 		"""scenario commands group. 4 Sub-classes, 1 commands."""
 		if not hasattr(self, '_scenario'):
-			from .Route_.Scenario import Scenario
-			self._scenario = Scenario(self._core, self._base)
+			from .Scenario import ScenarioCls
+			self._scenario = ScenarioCls(self._core, self._cmd_group)
 		return self._scenario
 
 	# noinspection PyTypeChecker
-	class ValueStruct(StructBase):
+	class ValueStruct(StructBase):  # From ReadStructDefinition CmdPropertyTemplate.xml
 		"""Structure for reading output parameters. Fields: \n
 			- Scenario: enums.Scenario: STANdard cell | MIMO2 | SCFading | MIMFading STANdard Standard SISO scenario MIMO2 MIMO 2x2 (DL and UL) SCFading Standard SISO scenario with fading MIMFading MIMO 2x2 scenario with fading
 			- Master: str: string For future use - returned value not relevant
 			- Rx_Connector: enums.RxConnector: RF connector for the input path 1
 			- Rx_Converter: enums.RxConverter: RX module for the input path 1
 			- Tx_Connector: enums.TxConnector: RF connector for output path 1
 			- Tx_Converter: enums.TxConverter: TX module for output path 1
@@ -55,25 +55,24 @@
 			self.Tx_Connector: enums.TxConnector = None
 			self.Tx_Converter: enums.TxConverter = None
 			self.Tx_Connector_2: enums.TxConnector = None
 			self.Tx_Converter_2: enums.TxConverter = None
 			self.Rx_Connector_2: enums.RxConnector = None
 			self.Rx_Converter_2: enums.RxConverter = None
 
-	# noinspection PyTypeChecker
 	def get_value(self) -> ValueStruct:
 		"""SCPI: ROUTe:WLAN:SIGNaling<instance> \n
 		Snippet: value: ValueStruct = driver.route.get_value() \n
 		Queries the active test scenario, the used TRX modules and the used RF connectors. For the STANdard and SCFading
 		scenarios, the first six parameters are returned. For the MIMO scenario, all eight parameters are returned. For possible
-		connector and converter values, see 'Values for Signal Path Selection'. \n
+		connector and converter values, see 'Values for signal path selection'. \n
 			:return: structure: for return value, see the help for ValueStruct structure arguments.
 		"""
 		return self._core.io.query_struct('ROUTe:WLAN:SIGNaling<Instance>?', self.__class__.ValueStruct())
 
-	def clone(self) -> 'Route':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'RouteCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Route(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = RouteCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal import Conversions
-from ... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal import Conversions
+from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Scenario:
-	"""Scenario commands group definition. 5 total commands, 4 Sub-groups, 1 group commands"""
+class ScenarioCls:
+	"""Scenario commands group definition. 5 total commands, 4 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("scenario", core, parent)
+		self._cmd_group = CommandsGroup("scenario", core, parent)
 
 	@property
 	def mimo(self):
 		"""mimo commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mimo'):
-			from .Scenario_.Mimo import Mimo
-			self._mimo = Mimo(self._core, self._base)
+			from .Mimo import MimoCls
+			self._mimo = MimoCls(self._core, self._cmd_group)
 		return self._mimo
 
 	@property
 	def scell(self):
-		"""scell commands group. 0 Sub-classes, 1 commands."""
+		"""scell commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_scell'):
-			from .Scenario_.Scell import Scell
-			self._scell = Scell(self._core, self._base)
+			from .Scell import ScellCls
+			self._scell = ScellCls(self._core, self._cmd_group)
 		return self._scell
 
 	@property
 	def scFading(self):
 		"""scFading commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_scFading'):
-			from .Scenario_.ScFading import ScFading
-			self._scFading = ScFading(self._core, self._base)
+			from .ScFading import ScFadingCls
+			self._scFading = ScFadingCls(self._core, self._cmd_group)
 		return self._scFading
 
 	@property
 	def mimFading(self):
 		"""mimFading commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_mimFading'):
-			from .Scenario_.MimFading import MimFading
-			self._mimFading = MimFading(self._core, self._base)
+			from .MimFading import MimFadingCls
+			self._mimFading = MimFadingCls(self._core, self._cmd_group)
 		return self._mimFading
 
 	# noinspection PyTypeChecker
 	def get_value(self) -> enums.Scenario:
 		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario \n
 		Snippet: value: enums.Scenario = driver.route.scenario.get_value() \n
 		Returns the active scenario. \n
 			:return: scenario: STANdard | MIMO2 | SCFading | MIMFading STANdard Standard SISO scenario MIMO2 MIMO 2x2 (DL and UL) SCFading Standard SISO scenario with fading MIMFading MIMO 2x2 scenario with fading
 		"""
 		response = self._core.io.query_str('ROUTe:WLAN:SIGNaling<Instance>:SCENario?')
 		return Conversions.str_to_scalar_enum(response, enums.Scenario)
 
-	def clone(self) -> 'Scenario':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'ScenarioCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Scenario(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = ScenarioCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/MimFading.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/ScFading.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,70 +2,65 @@
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal.StructBase import StructBase
 from ....Internal.ArgStruct import ArgStruct
 from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MimFading:
-	"""MimFading commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class ScFadingCls:
+	"""ScFading commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mimFading", core, parent)
+		self._cmd_group = CommandsGroup("scFading", core, parent)
 
 	# noinspection PyTypeChecker
-	class FlexibleStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+	class FlexibleStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
+		"""Structure for setting input parameters. Fields: \n
 			- Pcc_Bb_Board: enums.PccBasebandBoard: Signaling unit
-			- Rx_Connector: enums.RxConnector: RF connector for the input path 1
-			- Rx_Converter: enums.RxConverter: RX module for the input path 1
-			- Tx_Connector: enums.TxConnector: RF connector for the output path 1
-			- Tx_Converter: enums.TxConverter: TX module for the output path 1
-			- Tx_2_Connector: enums.TxConnector: RF connector for the output path 2
-			- Tx_2_Converter: enums.TxConverter: TX module for the output path 2
-			- Rx_2_Connector: enums.RxConnector: RF connector for the input path 2
-			- Rx_2_Converter: enums.RxConverter: RX module for the input path 2
+			- Rx_Connector: enums.RxConnector: RF connector for the input path
+			- Rx_Converter: enums.RxConverter: RX module for the input path
+			- Tx_Connector: enums.TxConnector: RF connector for the output path
+			- Tx_Converter: enums.TxConverter: TX module for the output path
 			- Pcc_Fading_Board: enums.PccFadingBoard: Internal fader"""
 		__meta_args_list = [
 			ArgStruct.scalar_enum('Pcc_Bb_Board', enums.PccBasebandBoard),
 			ArgStruct.scalar_enum('Rx_Connector', enums.RxConnector),
 			ArgStruct.scalar_enum('Rx_Converter', enums.RxConverter),
 			ArgStruct.scalar_enum('Tx_Connector', enums.TxConnector),
 			ArgStruct.scalar_enum('Tx_Converter', enums.TxConverter),
-			ArgStruct.scalar_enum('Tx_2_Connector', enums.TxConnector),
-			ArgStruct.scalar_enum('Tx_2_Converter', enums.TxConverter),
-			ArgStruct.scalar_enum('Rx_2_Connector', enums.RxConnector),
-			ArgStruct.scalar_enum('Rx_2_Converter', enums.RxConverter),
 			ArgStruct.scalar_enum('Pcc_Fading_Board', enums.PccFadingBoard)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Pcc_Bb_Board: enums.PccBasebandBoard = None
 			self.Rx_Connector: enums.RxConnector = None
 			self.Rx_Converter: enums.RxConverter = None
 			self.Tx_Connector: enums.TxConnector = None
 			self.Tx_Converter: enums.TxConverter = None
-			self.Tx_2_Connector: enums.TxConnector = None
-			self.Tx_2_Converter: enums.TxConverter = None
-			self.Rx_2_Connector: enums.RxConnector = None
-			self.Rx_2_Converter: enums.RxConverter = None
 			self.Pcc_Fading_Board: enums.PccFadingBoard = None
 
-	# noinspection PyTypeChecker
 	def get_flexible(self) -> FlexibleStruct:
-		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:MIMFading:FLEXible \n
-		Snippet: value: FlexibleStruct = driver.route.scenario.mimFading.get_flexible() \n
-		Activates the 'MIMO 2x2 Fading' scenario and selects the signal paths. For possible parameter values, see 'Values for
-		Signal Path Selection'. \n
+		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:SCFading:FLEXible \n
+		Snippet: value: FlexibleStruct = driver.route.scenario.scFading.get_flexible() \n
+		Activates the 'Standard Cell Fading' scenario and selects the signal paths. For possible parameter values, see 'Values
+		for signal path selection'. \n
 			:return: structure: for return value, see the help for FlexibleStruct structure arguments.
 		"""
-		return self._core.io.query_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:MIMFading:FLEXible?', self.__class__.FlexibleStruct())
+		return self._core.io.query_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:SCFading:FLEXible?', self.__class__.FlexibleStruct())
 
 	def set_flexible(self, value: FlexibleStruct) -> None:
-		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:MIMFading:FLEXible \n
-		Snippet: driver.route.scenario.mimFading.set_flexible(value = FlexibleStruct()) \n
-		Activates the 'MIMO 2x2 Fading' scenario and selects the signal paths. For possible parameter values, see 'Values for
-		Signal Path Selection'. \n
+		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:SCFading:FLEXible \n
+		Snippet with structure: \n
+		structure = driver.route.scenario.scFading.FlexibleStruct() \n
+		structure.Pcc_Bb_Board: enums.PccBasebandBoard = enums.PccBasebandBoard.BBR1 \n
+		structure.Rx_Connector: enums.RxConnector = enums.RxConnector.I11I \n
+		structure.Rx_Converter: enums.RxConverter = enums.RxConverter.IRX1 \n
+		structure.Tx_Connector: enums.TxConnector = enums.TxConnector.I12O \n
+		structure.Tx_Converter: enums.TxConverter = enums.TxConverter.ITX1 \n
+		structure.Pcc_Fading_Board: enums.PccFadingBoard = enums.PccFadingBoard.FAD012 \n
+		driver.route.scenario.scFading.set_flexible(value = structure) \n
+		Activates the 'Standard Cell Fading' scenario and selects the signal paths. For possible parameter values, see 'Values
+		for signal path selection'. \n
 			:param value: see the help for FlexibleStruct structure arguments.
 		"""
-		self._core.io.write_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:MIMFading:FLEXible', value)
+		self._core.io.write_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:SCFading:FLEXible', value)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/Mimo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Route/Scenario/Mimo.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,67 +2,77 @@
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal.StructBase import StructBase
 from ....Internal.ArgStruct import ArgStruct
 from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mimo:
-	"""Mimo commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class MimoCls:
+	"""Mimo commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mimo", core, parent)
+		self._cmd_group = CommandsGroup("mimo", core, parent)
 
 	# noinspection PyTypeChecker
-	class FlexibleStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
+	class FlexibleStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
+		"""Structure for setting input parameters. Contains optional set arguments. Fields: \n
 			- Pcc_Bb_Board: enums.PccBasebandBoard: Signaling unit
 			- Rx_Connector: enums.RxConnector: RF connector for the input path 1
 			- Rx_Converter: enums.RxConverter: RX module for the input path 1
 			- Tx_Connector: enums.TxConnector: RF connector for output path 1
 			- Tx_Converter: enums.TxConverter: TX module for output path 1
 			- Tx_2_Connector: enums.TxConnector: RF connector for output path 2
 			- Tx_2_Converter: enums.TxConverter: TX module for output path 2. Select different modules for the two paths.
-			- Rx_2_Connector: enums.RxConnector: RF connector for the input path 2
-			- Rx_2_Converter: enums.RxConverter: RX module for the input path 2. Select different modules for the two paths."""
+			- Rx_2_Connector: enums.RxConnector: Optional setting parameter. RF connector for the input path 2
+			- Rx_2_Converter: enums.RxConverter: Optional setting parameter. RX module for the input path 2. Select different modules for the two paths."""
 		__meta_args_list = [
 			ArgStruct.scalar_enum('Pcc_Bb_Board', enums.PccBasebandBoard),
 			ArgStruct.scalar_enum('Rx_Connector', enums.RxConnector),
 			ArgStruct.scalar_enum('Rx_Converter', enums.RxConverter),
 			ArgStruct.scalar_enum('Tx_Connector', enums.TxConnector),
 			ArgStruct.scalar_enum('Tx_Converter', enums.TxConverter),
 			ArgStruct.scalar_enum('Tx_2_Connector', enums.TxConnector),
 			ArgStruct.scalar_enum('Tx_2_Converter', enums.TxConverter),
-			ArgStruct.scalar_enum('Rx_2_Connector', enums.RxConnector),
-			ArgStruct.scalar_enum('Rx_2_Converter', enums.RxConverter)]
+			ArgStruct.scalar_enum_optional('Rx_2_Connector', enums.RxConnector),
+			ArgStruct.scalar_enum_optional('Rx_2_Converter', enums.RxConverter)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Pcc_Bb_Board: enums.PccBasebandBoard = None
 			self.Rx_Connector: enums.RxConnector = None
 			self.Rx_Converter: enums.RxConverter = None
 			self.Tx_Connector: enums.TxConnector = None
 			self.Tx_Converter: enums.TxConverter = None
 			self.Tx_2_Connector: enums.TxConnector = None
 			self.Tx_2_Converter: enums.TxConverter = None
 			self.Rx_2_Connector: enums.RxConnector = None
 			self.Rx_2_Converter: enums.RxConverter = None
 
-	# noinspection PyTypeChecker
 	def get_flexible(self) -> FlexibleStruct:
 		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:MIMO:FLEXible \n
 		Snippet: value: FlexibleStruct = driver.route.scenario.mimo.get_flexible() \n
-		Defines the RX and TX routing for the MIMO scenarios. For possible connector and converter values, see 'Values for Signal
-		Path Selection'. \n
+		Defines the RX and TX routing for the MIMO scenarios. For possible connector and converter values, see 'Values for signal
+		path selection'. \n
 			:return: structure: for return value, see the help for FlexibleStruct structure arguments.
 		"""
 		return self._core.io.query_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:MIMO:FLEXible?', self.__class__.FlexibleStruct())
 
 	def set_flexible(self, value: FlexibleStruct) -> None:
 		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:MIMO:FLEXible \n
-		Snippet: driver.route.scenario.mimo.set_flexible(value = FlexibleStruct()) \n
-		Defines the RX and TX routing for the MIMO scenarios. For possible connector and converter values, see 'Values for Signal
-		Path Selection'. \n
+		Snippet with structure: \n
+		structure = driver.route.scenario.mimo.FlexibleStruct() \n
+		structure.Pcc_Bb_Board: enums.PccBasebandBoard = enums.PccBasebandBoard.BBR1 \n
+		structure.Rx_Connector: enums.RxConnector = enums.RxConnector.I11I \n
+		structure.Rx_Converter: enums.RxConverter = enums.RxConverter.IRX1 \n
+		structure.Tx_Connector: enums.TxConnector = enums.TxConnector.I12O \n
+		structure.Tx_Converter: enums.TxConverter = enums.TxConverter.ITX1 \n
+		structure.Tx_2_Connector: enums.TxConnector = enums.TxConnector.I12O \n
+		structure.Tx_2_Converter: enums.TxConverter = enums.TxConverter.ITX1 \n
+		structure.Rx_2_Connector: enums.RxConnector = enums.RxConnector.I11I \n
+		structure.Rx_2_Converter: enums.RxConverter = enums.RxConverter.IRX1 \n
+		driver.route.scenario.mimo.set_flexible(value = structure) \n
+		Defines the RX and TX routing for the MIMO scenarios. For possible connector and converter values, see 'Values for signal
+		path selection'. \n
 			:param value: see the help for FlexibleStruct structure arguments.
 		"""
 		self._core.io.write_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:MIMO:FLEXible', value)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/ScFading.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/OfmLength.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,50 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Types import DataType
+from .....Internal.StructBase import StructBase
+from .....Internal.ArgStruct import ArgStruct
+from .....Internal.ArgSingleList import ArgSingleList
+from .....Internal.ArgSingle import ArgSingle
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class ScFading:
-	"""ScFading commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class OfmLengthCls:
+	"""OfmLength commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("scFading", core, parent)
+		self._cmd_group = CommandsGroup("ofmLength", core, parent)
+
+	def set(self, mode: enums.LenMode, length: int = None) -> None:
+		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:OFMLength \n
+		Snippet: driver.trigger.rx.macFrame.ofmLength.set(mode = enums.LenMode.DEFault, length = 1) \n
+		Defines the minimum length for the all OFDM RX frame trigger modes (all modes except All Bursts and DSSS/CCK Bursts) ,
+		see method RsCmwWlanSig.Trigger.Rx.MacFrame.btype. \n
+			:param mode: DEFault | UDEFined DEFault: automatically calculated value UDEFined: configured Length
+			:param length: numeric Range: 1 to 1500
+		"""
+		param = ArgSingleList().compose_cmd_string(ArgSingle('mode', mode, DataType.Enum, enums.LenMode), ArgSingle('length', length, DataType.Integer, None, is_optional=True))
+		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:OFMLength {param}'.rstrip())
 
 	# noinspection PyTypeChecker
-	class FlexibleStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Pcc_Bb_Board: enums.PccBasebandBoard: Signaling unit
-			- Rx_Connector: enums.RxConnector: RF connector for the input path
-			- Rx_Converter: enums.RxConverter: RX module for the input path
-			- Tx_Connector: enums.TxConnector: RF connector for the output path
-			- Tx_Converter: enums.TxConverter: TX module for the output path
-			- Pcc_Fading_Board: enums.PccFadingBoard: Internal fader"""
+	class OfmLengthStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Mode: enums.LenMode: DEFault | UDEFined DEFault: automatically calculated value UDEFined: configured Length
+			- Length: int: numeric Range: 1 to 1500"""
 		__meta_args_list = [
-			ArgStruct.scalar_enum('Pcc_Bb_Board', enums.PccBasebandBoard),
-			ArgStruct.scalar_enum('Rx_Connector', enums.RxConnector),
-			ArgStruct.scalar_enum('Rx_Converter', enums.RxConverter),
-			ArgStruct.scalar_enum('Tx_Connector', enums.TxConnector),
-			ArgStruct.scalar_enum('Tx_Converter', enums.TxConverter),
-			ArgStruct.scalar_enum('Pcc_Fading_Board', enums.PccFadingBoard)]
+			ArgStruct.scalar_enum('Mode', enums.LenMode),
+			ArgStruct.scalar_int('Length')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Pcc_Bb_Board: enums.PccBasebandBoard = None
-			self.Rx_Connector: enums.RxConnector = None
-			self.Rx_Converter: enums.RxConverter = None
-			self.Tx_Connector: enums.TxConnector = None
-			self.Tx_Converter: enums.TxConverter = None
-			self.Pcc_Fading_Board: enums.PccFadingBoard = None
-
-	# noinspection PyTypeChecker
-	def get_flexible(self) -> FlexibleStruct:
-		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:SCFading:FLEXible \n
-		Snippet: value: FlexibleStruct = driver.route.scenario.scFading.get_flexible() \n
-		Activates the 'Standard Cell Fading' scenario and selects the signal paths. For possible parameter values, see 'Values
-		for Signal Path Selection'. \n
-			:return: structure: for return value, see the help for FlexibleStruct structure arguments.
-		"""
-		return self._core.io.query_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:SCFading:FLEXible?', self.__class__.FlexibleStruct())
+			self.Mode: enums.LenMode = None
+			self.Length: int = None
 
-	def set_flexible(self, value: FlexibleStruct) -> None:
-		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:SCFading:FLEXible \n
-		Snippet: driver.route.scenario.scFading.set_flexible(value = FlexibleStruct()) \n
-		Activates the 'Standard Cell Fading' scenario and selects the signal paths. For possible parameter values, see 'Values
-		for Signal Path Selection'. \n
-			:param value: see the help for FlexibleStruct structure arguments.
-		"""
-		self._core.io.write_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:SCFading:FLEXible', value)
+	def get(self) -> OfmLengthStruct:
+		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:OFMLength \n
+		Snippet: value: OfmLengthStruct = driver.trigger.rx.macFrame.ofmLength.get() \n
+		Defines the minimum length for the all OFDM RX frame trigger modes (all modes except All Bursts and DSSS/CCK Bursts) ,
+		see method RsCmwWlanSig.Trigger.Rx.MacFrame.btype. \n
+			:return: structure: for return value, see the help for OfmLengthStruct structure arguments."""
+		return self._core.io.query_struct(f'TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:OFMLength?', self.__class__.OfmLengthStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Route_/Scenario_/Scell.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Source/State.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,65 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
+from ...Internal import Conversions
+from ...Internal.StructBase import StructBase
+from ...Internal.ArgStruct import ArgStruct
+from ... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Scell:
-	"""Scell commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class StateCls:
+	"""State commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("scell", core, parent)
+		self._cmd_group = CommandsGroup("state", core, parent)
 
 	# noinspection PyTypeChecker
-	class FlexibleStruct(StructBase):
+	class AllStruct(StructBase):  # From ReadStructDefinition CmdPropertyTemplate.xml
 		"""Structure for reading output parameters. Fields: \n
-			- Pcc_Bb_Board: enums.PccBasebandBoard: Signaling unit
-			- Rx_Connector: enums.RxConnector: RF connector for the input path
-			- Rx_Converter: enums.RxConverter: RX module for the input path
-			- Tx_Connector: enums.TxConnector: RF connector for the output path
-			- Tx_Converter: enums.TxConverter: TX module for the output path"""
+			- Main_State: bool: OFF | ON
+			- Sync_State: enums.SyncState: PENDing | ADJusted PENDing: The generator has been turned on (off) but the signal is not yet (still) available. ADJusted: The physical output signal corresponds to the main generator state.
+			- Dut_1: enums.PsState: IDLE | AUTHenticated | ASSociated | DEAuthenticated | DISassociated | CTIMeout
+			- Dut_2: enums.PsState: IDLE | AUTHenticated | ASSociated | DEAuthenticated | DISassociated | CTIMeout
+			- Dut_3: enums.PsState: IDLE | AUTHenticated | ASSociated | DEAuthenticated | DISassociated | CTIMeout"""
 		__meta_args_list = [
-			ArgStruct.scalar_enum('Pcc_Bb_Board', enums.PccBasebandBoard),
-			ArgStruct.scalar_enum('Rx_Connector', enums.RxConnector),
-			ArgStruct.scalar_enum('Rx_Converter', enums.RxConverter),
-			ArgStruct.scalar_enum('Tx_Connector', enums.TxConnector),
-			ArgStruct.scalar_enum('Tx_Converter', enums.TxConverter)]
+			ArgStruct.scalar_bool('Main_State'),
+			ArgStruct.scalar_enum('Sync_State', enums.SyncState),
+			ArgStruct.scalar_enum('Dut_1', enums.PsState),
+			ArgStruct.scalar_enum('Dut_2', enums.PsState),
+			ArgStruct.scalar_enum('Dut_3', enums.PsState)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
-			self.Pcc_Bb_Board: enums.PccBasebandBoard = None
-			self.Rx_Connector: enums.RxConnector = None
-			self.Rx_Converter: enums.RxConverter = None
-			self.Tx_Connector: enums.TxConnector = None
-			self.Tx_Converter: enums.TxConverter = None
+			self.Main_State: bool = None
+			self.Sync_State: enums.SyncState = None
+			self.Dut_1: enums.PsState = None
+			self.Dut_2: enums.PsState = None
+			self.Dut_3: enums.PsState = None
+
+	def get_all(self) -> AllStruct:
+		"""SCPI: SOURce:WLAN:SIGNaling<instance>:STATe:ALL \n
+		Snippet: value: AllStruct = driver.source.state.get_all() \n
+		Returns detailed information about the WLAN signaling generator state and the connection state of station one to three.
+		See also 'Connection status'. \n
+			:return: structure: for return value, see the help for AllStruct structure arguments.
+		"""
+		return self._core.io.query_struct('SOURce:WLAN:SIGNaling<Instance>:STATe:ALL?', self.__class__.AllStruct())
 
-	# noinspection PyTypeChecker
-	def get_flexible(self) -> FlexibleStruct:
-		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:SCELl:FLEXible \n
-		Snippet: value: FlexibleStruct = driver.route.scenario.scell.get_flexible() \n
-		Defines the standard RX and TX routing (no MIMO) . For possible connector and converter values, see 'Values for Signal
-		Path Selection'. \n
-			:return: structure: for return value, see the help for FlexibleStruct structure arguments.
+	def get_value(self) -> bool:
+		"""SCPI: SOURce:WLAN:SIGNaling<instance>:STATe \n
+		Snippet: value: bool = driver.source.state.get_value() \n
+		Turns the generator (the cell) on or off. \n
+			:return: main_state: ON | OFF | 1 | 0 Switch generator ON or OFF
 		"""
-		return self._core.io.query_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:SCELl:FLEXible?', self.__class__.FlexibleStruct())
+		response = self._core.io.query_str_with_opc('SOURce:WLAN:SIGNaling<Instance>:STATe?')
+		return Conversions.str_to_bool(response)
 
-	def set_flexible(self, value: FlexibleStruct) -> None:
-		"""SCPI: ROUTe:WLAN:SIGNaling<instance>:SCENario:SCELl:FLEXible \n
-		Snippet: driver.route.scenario.scell.set_flexible(value = FlexibleStruct()) \n
-		Defines the standard RX and TX routing (no MIMO) . For possible connector and converter values, see 'Values for Signal
-		Path Selection'. \n
-			:param value: see the help for FlexibleStruct structure arguments.
+	def set_value(self, main_state: bool) -> None:
+		"""SCPI: SOURce:WLAN:SIGNaling<instance>:STATe \n
+		Snippet: driver.source.state.set_value(main_state = False) \n
+		Turns the generator (the cell) on or off. \n
+			:param main_state: ON | OFF | 1 | 0 Switch generator ON or OFF
 		"""
-		self._core.io.write_struct('ROUTe:WLAN:SIGNaling<Instance>:SCENario:SCELl:FLEXible', value)
+		param = Conversions.bool_to_str(main_state)
+		self._core.io.write_with_opc(f'SOURce:WLAN:SIGNaling<Instance>:STATe {param}')
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Second.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Source/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Second:
-	"""Second commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class SourceCls:
+	"""Source commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("second", core, parent)
+		self._cmd_group = CommandsGroup("source", core, parent)
 
 	@property
 	def state(self):
-		"""state commands group. 0 Sub-classes, 1 commands."""
+		"""state commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_state'):
-			from .Second_.State import State
-			self._state = State(self._core, self._base)
+			from .State import StateCls
+			self._state = StateCls(self._core, self._cmd_group)
 		return self._state
 
-	def clone(self) -> 'Second':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SourceCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Second(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SourceCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Second_/State.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Second/State.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 from ...Internal import Conversions
 from ... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class State:
-	"""State commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class StateCls:
+	"""State commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("state", core, parent)
+		self._cmd_group = CommandsGroup("state", core, parent)
 
 	# noinspection PyTypeChecker
 	def fetch(self) -> enums.PsState:
 		"""SCPI: FETCh:WLAN:SIGNaling<instance>:SECond:STATe \n
 		Snippet: value: enums.PsState = driver.second.state.fetch() \n
-		Gets the connection status, refer to 'Connection Status'. Commands for station one, two and three are available. \n
+		Gets the connection status, refer to 'Connection status'. Commands for station one, two and three are available. \n
 			:return: ps_state: IDLE | PROBed | AUTHenticated | ASSociated | DEAuthenticated | DISassociated | CTIMeout"""
 		response = self._core.io.query_str(f'FETCh:WLAN:SIGNaling<Instance>:SECond:STATe?')
 		return Conversions.str_to_scalar_enum(response, enums.PsState)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Muedca/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,51 @@
-from ..Internal.Core import Core
-from ..Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sense:
-	"""Sense commands group definition. 21 total commands, 5 Sub-groups, 0 group commands"""
+class MuedcaCls:
+	"""Muedca commands group definition. 4 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sense", core, parent)
+		self._cmd_group = CommandsGroup("muedca", core, parent)
 
 	@property
-	def uesInfo(self):
-		"""uesInfo commands group. 2 Sub-classes, 2 commands."""
-		if not hasattr(self, '_uesInfo'):
-			from .Sense_.UesInfo import UesInfo
-			self._uesInfo = UesInfo(self._core, self._base)
-		return self._uesInfo
+	def acbe(self):
+		"""acbe commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_acbe'):
+			from .Acbe import AcbeCls
+			self._acbe = AcbeCls(self._core, self._cmd_group)
+		return self._acbe
 
 	@property
-	def sta(self):
-		"""sta commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_sta'):
-			from .Sense_.Sta import Sta
-			self._sta = Sta(self._core, self._base)
-		return self._sta
+	def acbk(self):
+		"""acbk commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_acbk'):
+			from .Acbk import AcbkCls
+			self._acbk = AcbkCls(self._core, self._cmd_group)
+		return self._acbk
 
 	@property
-	def pgen(self):
-		"""pgen commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_pgen'):
-			from .Sense_.Pgen import Pgen
-			self._pgen = Pgen(self._core, self._base)
-		return self._pgen
+	def acvi(self):
+		"""acvi commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_acvi'):
+			from .Acvi import AcviCls
+			self._acvi = AcviCls(self._core, self._cmd_group)
+		return self._acvi
 
 	@property
-	def sinfo(self):
-		"""sinfo commands group. 1 Sub-classes, 1 commands."""
-		if not hasattr(self, '_sinfo'):
-			from .Sense_.Sinfo import Sinfo
-			self._sinfo = Sinfo(self._core, self._base)
-		return self._sinfo
+	def acvo(self):
+		"""acvo commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_acvo'):
+			from .Acvo import AcvoCls
+			self._acvo = AcvoCls(self._core, self._cmd_group)
+		return self._acvo
 
-	@property
-	def elogging(self):
-		"""elogging commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_elogging'):
-			from .Sense_.Elogging import Elogging
-			self._elogging = Elogging(self._core, self._base)
-		return self._elogging
-
-	def clone(self) -> 'Sense':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MuedcaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Sense(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MuedcaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Elogging.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Elogging.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from ...Internal.Types import DataType
 from ...Internal.StructBase import StructBase
 from ...Internal.ArgStruct import ArgStruct
 from ... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Elogging:
-	"""Elogging commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class EloggingCls:
+	"""Elogging commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("elogging", core, parent)
+		self._cmd_group = CommandsGroup("elogging", core, parent)
 
 	# noinspection PyTypeChecker
-	class AllStruct(StructBase):
+	class AllStruct(StructBase):  # From ReadStructDefinition CmdPropertyTemplate.xml
 		"""Structure for reading output parameters. Fields: \n
 			- Category: List[enums.LogCategoryB]: INFO | WARNing | ERRor | EMPTy Category of the entry, as indicated in the main view by an icon EMPTy means that there are no entries.
 			- Timestamp: List[str]: string Timestamp of the entry as string in the format 'hh:mm:ss'
 			- Description: List[str]: string Text string describing the event"""
 		__meta_args_list = [
 			ArgStruct('Category', DataType.EnumList, enums.LogCategoryB, False, True, 1),
 			ArgStruct('Timestamp', DataType.StringList, None, False, True, 1),
@@ -29,15 +29,14 @@
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Category: List[enums.LogCategoryB] = None
 			self.Timestamp: List[str] = None
 			self.Description: List[str] = None
 
-	# noinspection PyTypeChecker
 	def get_all(self) -> AllStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:ELOGging:ALL \n
 		Snippet: value: AllStruct = driver.sense.elogging.get_all() \n
 		Queries all entries of the event log. For each entry, three parameters are returned, from oldest to latest entry:
 		{<Category>, <Timestamp>, <Description>}entry 1, {<Category>, <Timestamp>, <Description>}entry 2, ... \n
 			:return: structure: for return value, see the help for AllStruct structure arguments.
 		"""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Pgen.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/UeAddress/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal.RepeatedCapability import RepeatedCapability
-from ... import repcap
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal.RepeatedCapability import RepeatedCapability
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Pgen:
-	"""Pgen commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
-	Repeated Capability: PacketGenerator, default value after init: PacketGenerator.Nr1"""
+class UeAddressCls:
+	"""UeAddress commands group definition. 1 total commands, 1 Subgroups, 0 group commands
+	Repeated Capability: IpVersion, default value after init: IpVersion.V4"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("pgen", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_packetGenerator_get', 'repcap_packetGenerator_set', repcap.PacketGenerator.Nr1)
+		self._cmd_group = CommandsGroup("ueAddress", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_ipVersion_get', 'repcap_ipVersion_set', repcap.IpVersion.V4)
 
-	def repcap_packetGenerator_set(self, enum_value: repcap.PacketGenerator) -> None:
+	def repcap_ipVersion_set(self, ipVersion: repcap.IpVersion) -> None:
 		"""Repeated Capability default value numeric suffix.
-		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to PacketGenerator.Default
-		Default value after init: PacketGenerator.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to IpVersion.Default
+		Default value after init: IpVersion.V4"""
+		self._cmd_group.set_repcap_enum_value(ipVersion)
 
-	def repcap_packetGenerator_get(self) -> repcap.PacketGenerator:
+	def repcap_ipVersion_get(self) -> repcap.IpVersion:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
-	def pgStats(self):
-		"""pgStats commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_pgStats'):
-			from .Pgen_.PgStats import PgStats
-			self._pgStats = PgStats(self._core, self._base)
-		return self._pgStats
+	def ipv(self):
+		"""ipv commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ipv'):
+			from .Ipv import IpvCls
+			self._ipv = IpvCls(self._core, self._cmd_group)
+		return self._ipv
 
-	def clone(self) -> 'Pgen':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'UeAddressCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Pgen(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = UeAddressCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Pgen_/PgStats.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Pgen/PgStats.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from ....Internal.CommandsGroup import CommandsGroup
 from ....Internal.StructBase import StructBase
 from ....Internal.ArgStruct import ArgStruct
 from .... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class PgStats:
-	"""PgStats commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class PgStatsCls:
+	"""PgStats commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("pgStats", core, parent)
+		self._cmd_group = CommandsGroup("pgStats", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Icmp_Req_Frames: int: No parameter help available
 			- Icmp_Req_Bytes: int: No parameter help available
 			- Icmp_Resp_Frames: int: No parameter help available
@@ -44,9 +44,9 @@
 
 	def get(self, packetGenerator=repcap.PacketGenerator.Default) -> GetStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:PGEN<index>:PGSTats \n
 		Snippet: value: GetStruct = driver.sense.pgen.pgStats.get(packetGenerator = repcap.PacketGenerator.Default) \n
 		No command help available \n
 			:param packetGenerator: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Pgen')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		packetGenerator_cmd_val = self._base.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
+		packetGenerator_cmd_val = self._cmd_group.get_repcap_cmd_value(packetGenerator, repcap.PacketGenerator)
 		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:PGEN{packetGenerator_cmd_val}:PGSTats?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sinfo/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal.StructBase import StructBase
-from ...Internal.ArgStruct import ArgStruct
-from ... import enums
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.StructBase import StructBase
+from ....Internal.ArgStruct import ArgStruct
+from .... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Sinfo:
-	"""Sinfo commands group definition. 2 total commands, 1 Sub-groups, 1 group commands"""
+class SinfoCls:
+	"""Sinfo commands group definition. 2 total commands, 1 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("sinfo", core, parent)
+		self._cmd_group = CommandsGroup("sinfo", core, parent)
 
 	@property
 	def antenna(self):
 		"""antenna commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_antenna'):
-			from .Sinfo_.Antenna import Antenna
-			self._antenna = Antenna(self._core, self._base)
+			from .Antenna import AntennaCls
+			self._antenna = AntennaCls(self._core, self._cmd_group)
 		return self._antenna
 
 	# noinspection PyTypeChecker
-	class EapStatStruct(StructBase):
+	class EapStatStruct(StructBase):  # From ReadStructDefinition CmdPropertyTemplate.xml
 		"""Structure for reading output parameters. Fields: \n
 			- State: enums.ResultState: IDLE | SUCCess | FAILure EAP connection state
 			- Type_Py: enums.AuthType: IDENtity | NOTification | NAK | MD5 | OTP | GTC | TLS | CLEap | SIM | TTLS | AKA | AKAPrime Authentication stage"""
 		__meta_args_list = [
 			ArgStruct.scalar_enum('State', enums.ResultState),
 			ArgStruct.scalar_enum('Type_Py', enums.AuthType)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.State: enums.ResultState = None
 			self.Type_Py: enums.AuthType = None
 
-	# noinspection PyTypeChecker
 	def get_eap_stat(self) -> EapStatStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:SINFo:EAPStat \n
 		Snippet: value: EapStatStruct = driver.sense.sinfo.get_eap_stat() \n
 		Queries the current state of the EAP connection for the security mode 'WPA / WPA2 Enterprise'. \n
 			:return: structure: for return value, see the help for EapStatStruct structure arguments.
 		"""
 		return self._core.io.query_struct('SENSe:WLAN:SIGNaling<Instance>:SINFo:EAPStat?', self.__class__.EapStatStruct())
 
-	def clone(self) -> 'Sinfo':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'SinfoCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Sinfo(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = SinfoCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sinfo/Antenna/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.RepeatedCapability import RepeatedCapability
-from .... import repcap
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.RepeatedCapability import RepeatedCapability
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Antenna:
-	"""Antenna commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
+class AntennaCls:
+	"""Antenna commands group definition. 1 total commands, 1 Subgroups, 0 group commands
 	Repeated Capability: Antenna, default value after init: Antenna.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("antenna", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_antenna_get', 'repcap_antenna_set', repcap.Antenna.Nr1)
+		self._cmd_group = CommandsGroup("antenna", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_antenna_get', 'repcap_antenna_set', repcap.Antenna.Nr1)
 
-	def repcap_antenna_set(self, enum_value: repcap.Antenna) -> None:
+	def repcap_antenna_set(self, antenna: repcap.Antenna) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Antenna.Default
 		Default value after init: Antenna.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(antenna)
 
 	def repcap_antenna_get(self) -> repcap.Antenna:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def rxpIndicator(self):
 		"""rxpIndicator commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_rxpIndicator'):
-			from .Antenna_.RxpIndicator import RxpIndicator
-			self._rxpIndicator = RxpIndicator(self._core, self._base)
+			from .RxpIndicator import RxpIndicatorCls
+			self._rxpIndicator = RxpIndicatorCls(self._core, self._cmd_group)
 		return self._rxpIndicator
 
-	def clone(self) -> 'Antenna':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'AntennaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Antenna(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = AntennaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna_/RxpIndicator.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sinfo/Antenna/RxpIndicator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
 from ..... import enums
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RxpIndicator:
-	"""RxpIndicator commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class RxpIndicatorCls:
+	"""RxpIndicator commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rxpIndicator", core, parent)
+		self._cmd_group = CommandsGroup("rxpIndicator", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Power_Value: float: float Unit: dBm
 			- Power_Indicator: enums.PowerIndicator: UNDerdriven | RANGe | OVERdriven"""
 		__meta_args_list = [
@@ -31,9 +31,9 @@
 	def get(self, antenna=repcap.Antenna.Default) -> GetStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:SINFo[:ANTenna<n>]:RXPindicator \n
 		Snippet: value: GetStruct = driver.sense.sinfo.antenna.rxpIndicator.get(antenna = repcap.Antenna.Default) \n
 		Queries the Rx burst power per individual antenna and evaluates the quality of the RX signal from the connected DUT.
 		Antenna 2 is only available in a MIMO scenario. \n
 			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:SINFo:ANTenna{antenna_cmd_val}:RXPindicator?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Fading/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class HetbInfo:
-	"""HetbInfo commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class FadingCls:
+	"""Fading commands group definition. 6 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hetbInfo", core, parent)
+		self._cmd_group = CommandsGroup("fading", core, parent)
 
 	@property
-	def uphInfo(self):
-		"""uphInfo commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_uphInfo'):
-			from .HetbInfo_.UphInfo import UphInfo
-			self._uphInfo = UphInfo(self._core, self._base)
-		return self._uphInfo
+	def fsimulator(self):
+		"""fsimulator commands group. 1 Sub-classes, 2 commands."""
+		if not hasattr(self, '_fsimulator'):
+			from .Fsimulator import FsimulatorCls
+			self._fsimulator = FsimulatorCls(self._core, self._cmd_group)
+		return self._fsimulator
 
-	def clone(self) -> 'HetbInfo':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def awgn(self):
+		"""awgn commands group. 1 Sub-classes, 2 commands."""
+		if not hasattr(self, '_awgn'):
+			from .Awgn import AwgnCls
+			self._awgn = AwgnCls(self._core, self._cmd_group)
+		return self._awgn
+
+	def clone(self) -> 'FadingCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = HetbInfo(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = FadingCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo_/UphInfo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/UeAddress/Ipv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,25 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal.StructBase import StructBase
-from .....Internal.ArgStruct import ArgStruct
-from ..... import repcap
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal.Utilities import trim_str_response
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UphInfo:
-	"""UphInfo commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class IpvCls:
+	"""Ipv commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uphInfo", core, parent)
+		self._cmd_group = CommandsGroup("ipv", core, parent)
 
-	# noinspection PyTypeChecker
-	class GetStruct(StructBase):
-		"""Response structure. Fields: \n
-			- Burst_Power: float: float Indication of HE TB burst power. Range: -999 dBm to 999 dBm
-			- Uph: int: decimal Indication of UL power headroom. Range: 0 dB to 31 dB
-			- Min_Tx_Power_Flag: bool: OFF | ON Indication whether the HE TB bursts are sent at the minimum transmit power of the station."""
-		__meta_args_list = [
-			ArgStruct.scalar_float('Burst_Power'),
-			ArgStruct.scalar_int('Uph'),
-			ArgStruct.scalar_bool('Min_Tx_Power_Flag')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Burst_Power: float = None
-			self.Uph: int = None
-			self.Min_Tx_Power_Flag: bool = None
-
-	def get(self, station=repcap.Station.Default) -> GetStruct:
-		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:HETBinfo:UPHinfo \n
-		Snippet: value: GetStruct = driver.sense.sta.hetbInfo.uphInfo.get(station = repcap.Station.Default) \n
-		Queries actual information related to uplink power headroom (UPH) control. \n
+	def get(self, station=repcap.Station.Default, ipVersion=repcap.IpVersion.Default) -> str:
+		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:UEADdress:IPV<n> \n
+		Snippet: value: str = driver.sense.sta.uesInfo.ueAddress.ipv.get(station = repcap.Station.Default, ipVersion = repcap.IpVersion.Default) \n
+		Queries the detected IPv4 / IPv6 addresses of the connected DUT. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
-			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:HETBinfo:UPHinfo?', self.__class__.GetStruct())
+			:param ipVersion: optional repeated capability selector. Default value: V4 (settable in the interface 'UeAddress')
+			:return: ip_address: string IPv4 / IPv6 addresses as string"""
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		ipVersion_cmd_val = self._cmd_group.get_repcap_cmd_value(ipVersion, repcap.IpVersion)
+		response = self._core.io.query_str(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:UEADdress:IPV{ipVersion_cmd_val}?')
+		return trim_str_response(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Wdirect/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UeCapability:
-	"""UeCapability commands group definition. 2 total commands, 2 Sub-groups, 0 group commands"""
+class WdirectCls:
+	"""Wdirect commands group definition. 2 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ueCapability", core, parent)
+		self._cmd_group = CommandsGroup("wdirect", core, parent)
 
 	@property
-	def mac(self):
-		"""mac commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_mac'):
-			from .UeCapability_.Mac import Mac
-			self._mac = Mac(self._core, self._base)
-		return self._mac
+	def atype(self):
+		"""atype commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_atype'):
+			from .Atype import AtypeCls
+			self._atype = AtypeCls(self._core, self._cmd_group)
+		return self._atype
 
 	@property
-	def he(self):
-		"""he commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_he'):
-			from .UeCapability_.He import He
-			self._he = He(self._core, self._base)
-		return self._he
+	def wdconf(self):
+		"""wdconf commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_wdconf'):
+			from .Wdconf import WdconfCls
+			self._wdconf = WdconfCls(self._core, self._cmd_group)
+		return self._wdconf
 
-	def clone(self) -> 'UeCapability':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'WdirectCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UeCapability(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = WdirectCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/He.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/He.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
 from ..... import enums
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class He:
-	"""He commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class HeCls:
+	"""He commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("he", core, parent)
+		self._cmd_group = CommandsGroup("he", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Device_Class: enums.DeviceClass: A | B
 			- Dyn_Fragment: enums.DynFragment: NO | L1 | L2 | L3 Dynamic fragmentation not supported, or dynamic fragmentation supported with level 1 to 3.
 			- Absr: enums.YesNoStatus: NO | YES Indicates support of a buffer status report (BSR) control field.
@@ -39,9 +39,9 @@
 
 	def get(self, station=repcap.Station.Default) -> GetStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UECapability:HE \n
 		Snippet: value: GetStruct = driver.sense.sta.ueCapability.he.get(station = repcap.Station.Default) \n
 		Indicates the reported UE HE capabilities. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UECapability:HE?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/Mac.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Security/Eaka/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Mac:
-	"""Mac commands group definition. 1 total commands, 1 Sub-groups, 0 group commands"""
+class EakaCls:
+	"""Eaka commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("mac", core, parent)
+		self._cmd_group = CommandsGroup("eaka", core, parent)
 
 	@property
-	def address(self):
-		"""address commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_address'):
-			from .Mac_.Address import Address
-			self._address = Address(self._core, self._base)
-		return self._address
+	def kalgo(self):
+		"""kalgo commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_kalgo'):
+			from .Kalgo import KalgoCls
+			self._kalgo = KalgoCls(self._core, self._cmd_group)
+		return self._kalgo
 
-	def clone(self) -> 'Mac':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'EakaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Mac(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = EakaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Edca/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,51 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UesInfo:
-	"""UesInfo commands group definition. 10 total commands, 5 Sub-groups, 0 group commands"""
+class EdcaCls:
+	"""Edca commands group definition. 4 total commands, 4 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uesInfo", core, parent)
+		self._cmd_group = CommandsGroup("edca", core, parent)
 
 	@property
-	def rxbPower(self):
-		"""rxbPower commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_rxbPower'):
-			from .UesInfo_.RxbPower import RxbPower
-			self._rxbPower = RxbPower(self._core, self._base)
-		return self._rxbPower
+	def acbe(self):
+		"""acbe commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_acbe'):
+			from .Acbe import AcbeCls
+			self._acbe = AcbeCls(self._core, self._cmd_group)
+		return self._acbe
 
 	@property
-	def drate(self):
-		"""drate commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_drate'):
-			from .UesInfo_.Drate import Drate
-			self._drate = Drate(self._core, self._base)
-		return self._drate
+	def acbk(self):
+		"""acbk commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_acbk'):
+			from .Acbk import AcbkCls
+			self._acbk = AcbkCls(self._core, self._cmd_group)
+		return self._acbk
 
 	@property
-	def absReport(self):
-		"""absReport commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_absReport'):
-			from .UesInfo_.AbsReport import AbsReport
-			self._absReport = AbsReport(self._core, self._base)
-		return self._absReport
+	def acvi(self):
+		"""acvi commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_acvi'):
+			from .Acvi import AcviCls
+			self._acvi = AcviCls(self._core, self._cmd_group)
+		return self._acvi
 
 	@property
-	def rxPsdu(self):
-		"""rxPsdu commands group. 6 Sub-classes, 0 commands."""
-		if not hasattr(self, '_rxPsdu'):
-			from .UesInfo_.RxPsdu import RxPsdu
-			self._rxPsdu = RxPsdu(self._core, self._base)
-		return self._rxPsdu
+	def acvo(self):
+		"""acvo commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_acvo'):
+			from .Acvo import AcvoCls
+			self._acvo = AcvoCls(self._core, self._cmd_group)
+		return self._acvo
 
-	@property
-	def ueAddress(self):
-		"""ueAddress commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_ueAddress'):
-			from .UesInfo_.UeAddress import UeAddress
-			self._ueAddress = UeAddress(self._core, self._base)
-		return self._ueAddress
-
-	def clone(self) -> 'UesInfo':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'EdcaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UesInfo(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = EdcaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/AbsReport.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/AbsReport.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
 from ..... import enums
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class AbsReport:
-	"""AbsReport commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class AbsReportCls:
+	"""AbsReport commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("absReport", core, parent)
+		self._cmd_group = CommandsGroup("absReport", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Total: int: decimal Maximum of all reports received in preceding interval Range: 0 KB to 4.145152E+6 KB, Unit: kB
 			- Buffered_Data_Tid: int: decimal Maximum of all QoS control reports Range: 0 KB to 4.145152E+6 KB, Unit: kB
 			- Tidx: enums.Tid: TID0 | TID1 | TID2 | TID3 | TID4 | TID5 | TID6 | TID7 Indication of TID, for which the buffer status BufferedData_TID is reported
@@ -39,9 +39,9 @@
 
 	def get(self, station=repcap.Station.Default) -> GetStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:ABSReport \n
 		Snippet: value: GetStruct = driver.sense.sta.uesInfo.absReport.get(station = repcap.Station.Default) \n
 		Indicates reported buffered data for a UE supporting a HE buffer status report (BSR) control field. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:ABSReport?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/Drate.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/Drate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from .....Internal.StructBase import StructBase
 from .....Internal.ArgStruct import ArgStruct
 from ..... import enums
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Drate:
-	"""Drate commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class DrateCls:
+	"""Drate commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("drate", core, parent)
+		self._cmd_group = CommandsGroup("drate", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Format_Py: enums.FrameFormat: NHT | HT | VHT | HESU | HEMU | HETB Frame format NHT: non-high throughput format (non-HT) HT: high throughput format VHT: very high throughput format HESU: high efficiency format, single user MIMO HEMU: high efficiency format, multi user MIMO HETB: high efficiency format, trigger based uplink single user MIMO
 			- Rate: enums.DataRate: MB1 | MB2 | MB5 | MB6 | MB9 | MB11 | MB12 | MB18 | MB24 | MB36 | MB48 | MB54 | MCS0 | MCS1 | MCS2 | MCS3 | MCS4 | MCS5 | MCS6 | MCS7 | MCS8 | MCS9 | MCS10 | MCS11 | MCS12 | MCS13 | MCS14 | MCS15 MBx: data rate for NHT in Mbit/s {1, 2, 5.5, 6, 9, 11, 12, 18, 24, 36, 48, 54} MCSx: modulation and coding scheme x for HT, VHT and HE
 			- Cbw: enums.ChannelBandwidth: BW20 | BW40 | BW80 | BW88 | BW16 Channel bandwidth in MHz: 20, 40, 80, 80+80, 160
@@ -36,9 +36,9 @@
 
 	def get(self, station=repcap.Station.Default) -> GetStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:DRATe \n
 		Snippet: value: GetStruct = driver.sense.sta.uesInfo.drate.get(station = repcap.Station.Default) \n
 		Queries information related to the data rate of the DUT signal. \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:DRATe?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RxPsdu:
-	"""RxPsdu commands group definition. 6 total commands, 6 Sub-groups, 0 group commands"""
+class IpAddressCls:
+	"""IpAddress commands group definition. 6 total commands, 6 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rxPsdu", core, parent)
+		self._cmd_group = CommandsGroup("ipAddress", core, parent)
 
 	@property
-	def noNht(self):
-		"""noNht commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_noNht'):
-			from .RxPsdu_.NoNht import NoNht
-			self._noNht = NoNht(self._core, self._base)
-		return self._noNht
-
-	@property
-	def ht(self):
-		"""ht commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_ht'):
-			from .RxPsdu_.Ht import Ht
-			self._ht = Ht(self._core, self._base)
-		return self._ht
-
-	@property
-	def vht(self):
-		"""vht commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_vht'):
-			from .RxPsdu_.Vht import Vht
-			self._vht = Vht(self._core, self._base)
-		return self._vht
-
-	@property
-	def hesu(self):
-		"""hesu commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_hesu'):
-			from .RxPsdu_.Hesu import Hesu
-			self._hesu = Hesu(self._core, self._base)
-		return self._hesu
-
-	@property
-	def hemu(self):
-		"""hemu commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_hemu'):
-			from .RxPsdu_.Hemu import Hemu
-			self._hemu = Hemu(self._core, self._base)
-		return self._hemu
-
-	@property
-	def hetb(self):
-		"""hetb commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_hetb'):
-			from .RxPsdu_.Hetb import Hetb
-			self._hetb = Hetb(self._core, self._base)
-		return self._hetb
+	def cmw(self):
+		"""cmw commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_cmw'):
+			from .Cmw import CmwCls
+			self._cmw = CmwCls(self._core, self._cmd_group)
+		return self._cmw
+
+	@property
+	def sta(self):
+		"""sta commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_sta'):
+			from .Sta import StaCls
+			self._sta = StaCls(self._core, self._cmd_group)
+		return self._sta
+
+	@property
+	def gateway(self):
+		"""gateway commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_gateway'):
+			from .Gateway import GatewayCls
+			self._gateway = GatewayCls(self._core, self._cmd_group)
+		return self._gateway
+
+	@property
+	def dns(self):
+		"""dns commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_dns'):
+			from .Dns import DnsCls
+			self._dns = DnsCls(self._core, self._cmd_group)
+		return self._dns
+
+	@property
+	def stack(self):
+		"""stack commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_stack'):
+			from .Stack import StackCls
+			self._stack = StackCls(self._core, self._cmd_group)
+		return self._stack
+
+	@property
+	def destination(self):
+		"""destination commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_destination'):
+			from .Destination import DestinationCls
+			self._destination = DestinationCls(self._core, self._cmd_group)
+		return self._destination
 
-	def clone(self) -> 'RxPsdu':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'IpAddressCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = RxPsdu(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = IpAddressCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hemu.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hesu.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,63 +6,63 @@
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hemu:
-	"""Hemu commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class HesuCls:
+	"""Hesu commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hemu", core, parent)
+		self._cmd_group = CommandsGroup("hesu", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Rate: List[enums.DataRate]: No parameter help available
-			- Ru_Size: List[enums.AllocSize]: No parameter help available
+			- Bw: List[enums.ChannelBandwidth]: No parameter help available
 			- Nss: List[enums.SpacialStreamsNr]: No parameter help available
 			- Frames_Curr: List[int]: No parameter help available
 			- Frames_Tot: List[int]: No parameter help available
 			- Bytes_Curr: List[float]: No parameter help available
 			- Bytes_Tot: List[float]: No parameter help available
 			- Mbps_Curr: List[float]: No parameter help available
 			- Mbps_Tot: List[float]: No parameter help available
 			- Power_Curr: List[float]: No parameter help available
 			- Power_Tot: List[float]: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct('Rate', DataType.EnumList, enums.DataRate, False, True, 1),
-			ArgStruct('Ru_Size', DataType.EnumList, enums.AllocSize, False, True, 1),
+			ArgStruct('Bw', DataType.EnumList, enums.ChannelBandwidth, False, True, 1),
 			ArgStruct('Nss', DataType.EnumList, enums.SpacialStreamsNr, False, True, 1),
 			ArgStruct('Frames_Curr', DataType.IntegerList, None, False, True, 1),
 			ArgStruct('Frames_Tot', DataType.IntegerList, None, False, True, 1),
 			ArgStruct('Bytes_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Bytes_Tot', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Mbps_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Mbps_Tot', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Power_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Power_Tot', DataType.FloatList, None, False, True, 1)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Rate: List[enums.DataRate] = None
-			self.Ru_Size: List[enums.AllocSize] = None
+			self.Bw: List[enums.ChannelBandwidth] = None
 			self.Nss: List[enums.SpacialStreamsNr] = None
 			self.Frames_Curr: List[int] = None
 			self.Frames_Tot: List[int] = None
 			self.Bytes_Curr: List[float] = None
 			self.Bytes_Tot: List[float] = None
 			self.Mbps_Curr: List[float] = None
 			self.Mbps_Tot: List[float] = None
 			self.Power_Curr: List[float] = None
 			self.Power_Tot: List[float] = None
 
 	def get(self, station=repcap.Station.Default) -> GetStruct:
-		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:HEMU \n
-		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.hemu.get(station = repcap.Station.Default) \n
+		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:HESU \n
+		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.hesu.get(station = repcap.Station.Default) \n
 		No command help available \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:HEMU?', self.__class__.GetStruct())
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:HESU?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hesu.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Vht.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hesu:
-	"""Hesu commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class VhtCls:
+	"""Vht commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hesu", core, parent)
+		self._cmd_group = CommandsGroup("vht", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Rate: List[enums.DataRate]: No parameter help available
 			- Bw: List[enums.ChannelBandwidth]: No parameter help available
 			- Nss: List[enums.SpacialStreamsNr]: No parameter help available
@@ -55,14 +55,14 @@
 			self.Bytes_Tot: List[float] = None
 			self.Mbps_Curr: List[float] = None
 			self.Mbps_Tot: List[float] = None
 			self.Power_Curr: List[float] = None
 			self.Power_Tot: List[float] = None
 
 	def get(self, station=repcap.Station.Default) -> GetStruct:
-		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:HESU \n
-		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.hesu.get(station = repcap.Station.Default) \n
+		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:VHT \n
+		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.vht.get(station = repcap.Station.Default) \n
 		No command help available \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:HESU?', self.__class__.GetStruct())
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:VHT?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hetb.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hetb.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,52 +6,52 @@
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Hetb:
-	"""Hetb commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class HetbCls:
+	"""Hetb commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("hetb", core, parent)
+		self._cmd_group = CommandsGroup("hetb", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Rate: List[enums.DataRate]: No parameter help available
-			- Ru_Size: List[enums.AllocSize]: No parameter help available
+			- Ru_Size: List[enums.RuSize]: No parameter help available
 			- Nss: List[enums.SpacialStreamsNr]: No parameter help available
 			- Frames_Curr: List[int]: No parameter help available
 			- Frames_Tot: List[int]: No parameter help available
 			- Bytes_Curr: List[float]: No parameter help available
 			- Bytes_Tot: List[float]: No parameter help available
 			- Mbps_Curr: List[float]: No parameter help available
 			- Mbps_Tot: List[float]: No parameter help available
 			- Power_Curr: List[float]: No parameter help available
 			- Power_Tot: List[float]: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct('Rate', DataType.EnumList, enums.DataRate, False, True, 1),
-			ArgStruct('Ru_Size', DataType.EnumList, enums.AllocSize, False, True, 1),
+			ArgStruct('Ru_Size', DataType.EnumList, enums.RuSize, False, True, 1),
 			ArgStruct('Nss', DataType.EnumList, enums.SpacialStreamsNr, False, True, 1),
 			ArgStruct('Frames_Curr', DataType.IntegerList, None, False, True, 1),
 			ArgStruct('Frames_Tot', DataType.IntegerList, None, False, True, 1),
 			ArgStruct('Bytes_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Bytes_Tot', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Mbps_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Mbps_Tot', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Power_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Power_Tot', DataType.FloatList, None, False, True, 1)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Rate: List[enums.DataRate] = None
-			self.Ru_Size: List[enums.AllocSize] = None
+			self.Ru_Size: List[enums.RuSize] = None
 			self.Nss: List[enums.SpacialStreamsNr] = None
 			self.Frames_Curr: List[int] = None
 			self.Frames_Tot: List[int] = None
 			self.Bytes_Curr: List[float] = None
 			self.Bytes_Tot: List[float] = None
 			self.Mbps_Curr: List[float] = None
 			self.Mbps_Tot: List[float] = None
@@ -60,9 +60,9 @@
 
 	def get(self, station=repcap.Station.Default) -> GetStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:HETB \n
 		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.hetb.get(station = repcap.Station.Default) \n
 		No command help available \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:HETB?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Ht.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hemu.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,63 +6,63 @@
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Ht:
-	"""Ht commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class HemuCls:
+	"""Hemu commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ht", core, parent)
+		self._cmd_group = CommandsGroup("hemu", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Rate: List[enums.DataRate]: No parameter help available
-			- Bw: List[enums.ChannelBandwidth]: No parameter help available
+			- Ru_Size: List[enums.RuSize]: No parameter help available
 			- Nss: List[enums.SpacialStreamsNr]: No parameter help available
 			- Frames_Curr: List[int]: No parameter help available
 			- Frames_Tot: List[int]: No parameter help available
 			- Bytes_Curr: List[float]: No parameter help available
 			- Bytes_Tot: List[float]: No parameter help available
 			- Mbps_Curr: List[float]: No parameter help available
 			- Mbps_Tot: List[float]: No parameter help available
 			- Power_Curr: List[float]: No parameter help available
 			- Power_Tot: List[float]: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct('Rate', DataType.EnumList, enums.DataRate, False, True, 1),
-			ArgStruct('Bw', DataType.EnumList, enums.ChannelBandwidth, False, True, 1),
+			ArgStruct('Ru_Size', DataType.EnumList, enums.RuSize, False, True, 1),
 			ArgStruct('Nss', DataType.EnumList, enums.SpacialStreamsNr, False, True, 1),
 			ArgStruct('Frames_Curr', DataType.IntegerList, None, False, True, 1),
 			ArgStruct('Frames_Tot', DataType.IntegerList, None, False, True, 1),
 			ArgStruct('Bytes_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Bytes_Tot', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Mbps_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Mbps_Tot', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Power_Curr', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Power_Tot', DataType.FloatList, None, False, True, 1)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Rate: List[enums.DataRate] = None
-			self.Bw: List[enums.ChannelBandwidth] = None
+			self.Ru_Size: List[enums.RuSize] = None
 			self.Nss: List[enums.SpacialStreamsNr] = None
 			self.Frames_Curr: List[int] = None
 			self.Frames_Tot: List[int] = None
 			self.Bytes_Curr: List[float] = None
 			self.Bytes_Tot: List[float] = None
 			self.Mbps_Curr: List[float] = None
 			self.Mbps_Tot: List[float] = None
 			self.Power_Curr: List[float] = None
 			self.Power_Tot: List[float] = None
 
 	def get(self, station=repcap.Station.Default) -> GetStruct:
-		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:HT \n
-		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.ht.get(station = repcap.Station.Default) \n
+		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:HEMU \n
+		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.hemu.get(station = repcap.Station.Default) \n
 		No command help available \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
-		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:HT?', self.__class__.GetStruct())
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
+		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:HEMU?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/NoNht.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/NoNht.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class NoNht:
-	"""NoNht commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class NoNhtCls:
+	"""NoNht commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("noNht", core, parent)
+		self._cmd_group = CommandsGroup("noNht", core, parent)
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Rate: List[enums.DataRate]: No parameter help available
 			- Bw: List[enums.ChannelBandwidth]: No parameter help available
 			- Nss: List[enums.SpacialStreamsNr]: No parameter help available
@@ -60,9 +60,9 @@
 
 	def get(self, station=repcap.Station.Default) -> GetStruct:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:STA<s>:UESinfo:RXPSdu:NONHt \n
 		Snippet: value: GetStruct = driver.sense.sta.uesInfo.rxPsdu.noNht.get(station = repcap.Station.Default) \n
 		No command help available \n
 			:param station: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Sta')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
-		station_cmd_val = self._base.get_repcap_cmd_value(station, repcap.Station)
+		station_cmd_val = self._cmd_group.get_repcap_cmd_value(station, repcap.Station)
 		return self._core.io.query_struct(f'SENSe:WLAN:SIGNaling<Instance>:STA{station_cmd_val}:UESinfo:RXPSdu:NONHt?', self.__class__.GetStruct())
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/UeAddress.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/CmwAddress/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.RepeatedCapability import RepeatedCapability
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UeAddress:
-	"""UeAddress commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
+class CmwAddressCls:
+	"""CmwAddress commands group definition. 1 total commands, 1 Subgroups, 0 group commands
 	Repeated Capability: IpVersion, default value after init: IpVersion.V4"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ueAddress", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_ipVersion_get', 'repcap_ipVersion_set', repcap.IpVersion.V4)
+		self._cmd_group = CommandsGroup("cmwAddress", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_ipVersion_get', 'repcap_ipVersion_set', repcap.IpVersion.V4)
 
-	def repcap_ipVersion_set(self, enum_value: repcap.IpVersion) -> None:
+	def repcap_ipVersion_set(self, ipVersion: repcap.IpVersion) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to IpVersion.Default
 		Default value after init: IpVersion.V4"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(ipVersion)
 
 	def repcap_ipVersion_get(self) -> repcap.IpVersion:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def ipv(self):
 		"""ipv commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_ipv'):
-			from .UeAddress_.Ipv import Ipv
-			self._ipv = Ipv(self._core, self._base)
+			from .Ipv import IpvCls
+			self._ipv = IpvCls(self._core, self._cmd_group)
 		return self._ipv
 
-	def clone(self) -> 'UeAddress':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'CmwAddressCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UeAddress(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = CmwAddressCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
-from ...Internal.Utilities import trim_str_response
-from ...Internal.StructBase import StructBase
-from ...Internal.ArgStruct import ArgStruct
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Utilities import trim_str_response
+from ....Internal.StructBase import StructBase
+from ....Internal.ArgStruct import ArgStruct
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class UesInfo:
-	"""UesInfo commands group definition. 4 total commands, 2 Sub-groups, 2 group commands"""
+class UesInfoCls:
+	"""UesInfo commands group definition. 4 total commands, 2 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("uesInfo", core, parent)
+		self._cmd_group = CommandsGroup("uesInfo", core, parent)
 
 	@property
 	def antenna(self):
 		"""antenna commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_antenna'):
-			from .UesInfo_.Antenna import Antenna
-			self._antenna = Antenna(self._core, self._base)
+			from .Antenna import AntennaCls
+			self._antenna = AntennaCls(self._core, self._cmd_group)
 		return self._antenna
 
 	@property
 	def cmwAddress(self):
 		"""cmwAddress commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_cmwAddress'):
-			from .UesInfo_.CmwAddress import CmwAddress
-			self._cmwAddress = CmwAddress(self._core, self._base)
+			from .CmwAddress import CmwAddressCls
+			self._cmwAddress = CmwAddressCls(self._core, self._cmd_group)
 		return self._cmwAddress
 
 	def get_ap_ssid(self) -> str:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:UESinfo:APSSid \n
 		Snippet: value: str = driver.sense.uesInfo.get_ap_ssid() \n
 		Returns the SSID of the associated access point. The command is only relevant in operation mode 'Station'. \n
 			:return: ssid: string Service set identifier as string
 		"""
 		response = self._core.io.query_str('SENSe:WLAN:SIGNaling<Instance>:UESinfo:APSSid?')
 		return trim_str_response(response)
 
 	# noinspection PyTypeChecker
-	class RxTrigFrameStruct(StructBase):
+	class RxTrigFrameStruct(StructBase):  # From ReadStructDefinition CmdPropertyTemplate.xml
 		"""Structure for reading output parameters. Fields: \n
 			- Total_Tf: int: decimal
 			- Station_Tf: int: decimal"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Total_Tf'),
 			ArgStruct.scalar_int('Station_Tf')]
 
@@ -56,14 +56,14 @@
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:UESinfo:RXTRigframe \n
 		Snippet: value: RxTrigFrameStruct = driver.sense.uesInfo.get_rx_trig_frame() \n
 		Queries the total trigger frames received and the number of trigger frames directed to the station, i.e. R&S CMW. \n
 			:return: structure: for return value, see the help for RxTrigFrameStruct structure arguments.
 		"""
 		return self._core.io.query_struct('SENSe:WLAN:SIGNaling<Instance>:UESinfo:RXTRigframe?', self.__class__.RxTrigFrameStruct())
 
-	def clone(self) -> 'UesInfo':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'UesInfoCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = UesInfo(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = UesInfoCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/Antenna/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.RepeatedCapability import RepeatedCapability
-from .... import repcap
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal.RepeatedCapability import RepeatedCapability
+from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Antenna:
-	"""Antenna commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
+class AntennaCls:
+	"""Antenna commands group definition. 1 total commands, 1 Subgroups, 0 group commands
 	Repeated Capability: Antenna, default value after init: Antenna.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("antenna", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_antenna_get', 'repcap_antenna_set', repcap.Antenna.Nr1)
+		self._cmd_group = CommandsGroup("antenna", core, parent)
+		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_antenna_get', 'repcap_antenna_set', repcap.Antenna.Nr1)
 
-	def repcap_antenna_set(self, enum_value: repcap.Antenna) -> None:
+	def repcap_antenna_set(self, antenna: repcap.Antenna) -> None:
 		"""Repeated Capability default value numeric suffix.
 		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Antenna.Default
 		Default value after init: Antenna.Nr1"""
-		self._base.set_repcap_enum_value(enum_value)
+		self._cmd_group.set_repcap_enum_value(antenna)
 
 	def repcap_antenna_get(self) -> repcap.Antenna:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		return self._cmd_group.get_repcap_enum_value()
 
 	@property
 	def arxbPower(self):
 		"""arxbPower commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_arxbPower'):
-			from .Antenna_.ArxbPower import ArxbPower
-			self._arxbPower = ArxbPower(self._core, self._base)
+			from .ArxbPower import ArxbPowerCls
+			self._arxbPower = ArxbPowerCls(self._core, self._cmd_group)
 		return self._arxbPower
 
-	def clone(self) -> 'Antenna':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'AntennaCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Antenna(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = AntennaCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna_/ArxbPower.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/Antenna/ArxbPower.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class ArxbPower:
-	"""ArxbPower commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class ArxbPowerCls:
+	"""ArxbPower commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("arxbPower", core, parent)
+		self._cmd_group = CommandsGroup("arxbPower", core, parent)
 
 	def get(self, antenna=repcap.Antenna.Default) -> float:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:UESinfo[:ANTenna<n>]:ARXBpower \n
 		Snippet: value: float = driver.sense.uesInfo.antenna.arxbPower.get(antenna = repcap.Antenna.Default) \n
 		Queries the approximate RX burst power per individual antenna, calculated from the expected PEP and the configured
 		standard. Antenna 2 is only available in a MIMO scenario. \n
 			:param antenna: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Antenna')
 			:return: approx_power: float Unit: dBm"""
-		antenna_cmd_val = self._base.get_repcap_cmd_value(antenna, repcap.Antenna)
+		antenna_cmd_val = self._cmd_group.get_repcap_cmd_value(antenna, repcap.Antenna)
 		response = self._core.io.query_str(f'SENSe:WLAN:SIGNaling<Instance>:UESinfo:ANTenna{antenna_cmd_val}:ARXBpower?')
 		return Conversions.str_to_float(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Configure/Connection/Ccode/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal.RepeatedCapability import RepeatedCapability
-from .... import repcap
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CmwAddress:
-	"""CmwAddress commands group definition. 1 total commands, 1 Sub-groups, 0 group commands
-	Repeated Capability: IpVersion, default value after init: IpVersion.V4"""
+class CcodeCls:
+	"""Ccode commands group definition. 2 total commands, 1 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("cmwAddress", core, parent)
-		self._base.rep_cap = RepeatedCapability(self._base.group_name, 'repcap_ipVersion_get', 'repcap_ipVersion_set', repcap.IpVersion.V4)
-
-	def repcap_ipVersion_set(self, enum_value: repcap.IpVersion) -> None:
-		"""Repeated Capability default value numeric suffix.
-		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to IpVersion.Default
-		Default value after init: IpVersion.V4"""
-		self._base.set_repcap_enum_value(enum_value)
-
-	def repcap_ipVersion_get(self) -> repcap.IpVersion:
-		"""Returns the current default repeated capability for the child set/get methods"""
-		# noinspection PyTypeChecker
-		return self._base.get_repcap_enum_value()
+		self._cmd_group = CommandsGroup("ccode", core, parent)
 
 	@property
-	def ipv(self):
-		"""ipv commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_ipv'):
-			from .CmwAddress_.Ipv import Ipv
-			self._ipv = Ipv(self._core, self._base)
-		return self._ipv
+	def ccconf(self):
+		"""ccconf commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ccconf'):
+			from .Ccconf import CcconfCls
+			self._ccconf = CcconfCls(self._core, self._cmd_group)
+		return self._ccconf
+
+	# noinspection PyTypeChecker
+	def get_cc_state(self) -> enums.EnableState:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:CCODe:CCSTate \n
+		Snippet: value: enums.EnableState = driver.configure.connection.ccode.get_cc_state() \n
+		Enables/disables the broadcast of regulatory domain information in beacon frames. \n
+			:return: state: DISable | ENABle
+		"""
+		response = self._core.io.query_str('CONFigure:WLAN:SIGNaling<Instance>:CONNection:CCODe:CCSTate?')
+		return Conversions.str_to_scalar_enum(response, enums.EnableState)
+
+	def set_cc_state(self, state: enums.EnableState) -> None:
+		"""SCPI: CONFigure:WLAN:SIGNaling<instance>:CONNection:CCODe:CCSTate \n
+		Snippet: driver.configure.connection.ccode.set_cc_state(state = enums.EnableState.DISable) \n
+		Enables/disables the broadcast of regulatory domain information in beacon frames. \n
+			:param state: DISable | ENABle
+		"""
+		param = Conversions.enum_scalar_to_str(state, enums.EnableState)
+		self._core.io.write(f'CONFigure:WLAN:SIGNaling<Instance>:CONNection:CCODe:CCSTate {param}')
 
-	def clone(self) -> 'CmwAddress':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'CcodeCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = CmwAddress(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = CcodeCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress_/Ipv.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Sense/UesInfo/CmwAddress/Ipv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal.Utilities import trim_str_response
 from ..... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Ipv:
-	"""Ipv commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class IpvCls:
+	"""Ipv commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("ipv", core, parent)
+		self._cmd_group = CommandsGroup("ipv", core, parent)
 
 	def get(self, ipVersion=repcap.IpVersion.Default) -> str:
 		"""SCPI: SENSe:WLAN:SIGNaling<instance>:UESinfo:CMWaddress:IPV<n> \n
 		Snippet: value: str = driver.sense.uesInfo.cmwAddress.ipv.get(ipVersion = repcap.IpVersion.Default) \n
 		Queries the IP address of the R&S CMW. \n
 			:param ipVersion: optional repeated capability selector. Default value: V4 (settable in the interface 'CmwAddress')
 			:return: ip_address: string The assigned IPv4 or IPv6 addresses."""
-		ipVersion_cmd_val = self._base.get_repcap_cmd_value(ipVersion, repcap.IpVersion)
+		ipVersion_cmd_val = self._cmd_group.get_repcap_cmd_value(ipVersion, repcap.IpVersion)
 		response = self._core.io.query_str(f'SENSe:WLAN:SIGNaling<Instance>:UESinfo:CMWaddress:IPV{ipVersion_cmd_val}?')
 		return trim_str_response(response)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Third_/State.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Third/State.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 from ...Internal import Conversions
 from ... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class State:
-	"""State commands group definition. 1 total commands, 0 Sub-groups, 1 group commands"""
+class StateCls:
+	"""State commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("state", core, parent)
+		self._cmd_group = CommandsGroup("state", core, parent)
 
 	# noinspection PyTypeChecker
 	def fetch(self) -> enums.PsState:
 		"""SCPI: FETCh:WLAN:SIGNaling<instance>:THIRd:STATe \n
 		Snippet: value: enums.PsState = driver.third.state.fetch() \n
-		Gets the connection status, refer to 'Connection Status'. Commands for station one, two and three are available. \n
+		Gets the connection status, refer to 'Connection status'. Commands for station one, two and three are available. \n
 			:return: ps_state: IDLE | PROBed | AUTHenticated | ASSociated | DEAuthenticated | DISassociated | CTIMeout"""
 		response = self._core.io.query_str(f'FETCh:WLAN:SIGNaling<Instance>:THIRd:STATe?')
 		return Conversions.str_to_scalar_enum(response, enums.PsState)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Rx:
-	"""Rx commands group definition. 11 total commands, 1 Sub-groups, 0 group commands"""
+class RxCls:
+	"""Rx commands group definition. 11 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("rx", core, parent)
+		self._cmd_group = CommandsGroup("rx", core, parent)
 
 	@property
 	def macFrame(self):
-		"""macFrame commands group. 1 Sub-classes, 9 commands."""
+		"""macFrame commands group. 3 Sub-classes, 7 commands."""
 		if not hasattr(self, '_macFrame'):
-			from .Rx_.MacFrame import MacFrame
-			self._macFrame = MacFrame(self._core, self._base)
+			from .MacFrame import MacFrameCls
+			self._macFrame = MacFrameCls(self._core, self._cmd_group)
 		return self._macFrame
 
-	def clone(self) -> 'Rx':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'RxCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Rx(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = RxCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,63 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from ....Internal.StructBase import StructBase
-from ....Internal.ArgStruct import ArgStruct
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MacFrame:
-	"""MacFrame commands group definition. 11 total commands, 1 Sub-groups, 9 group commands"""
+class MacFrameCls:
+	"""MacFrame commands group definition. 11 total commands, 3 Subgroups, 7 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("macFrame", core, parent)
+		self._cmd_group = CommandsGroup("macFrame", core, parent)
+
+	@property
+	def dsmLength(self):
+		"""dsmLength commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_dsmLength'):
+			from .DsmLength import DsmLengthCls
+			self._dsmLength = DsmLengthCls(self._core, self._cmd_group)
+		return self._dsmLength
+
+	@property
+	def ofmLength(self):
+		"""ofmLength commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ofmLength'):
+			from .OfmLength import OfmLengthCls
+			self._ofmLength = OfmLengthCls(self._core, self._cmd_group)
+		return self._ofmLength
 
 	@property
 	def plength(self):
 		"""plength commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_plength'):
-			from .MacFrame_.Plength import Plength
-			self._plength = Plength(self._core, self._base)
+			from .Plength import PlengthCls
+			self._plength = PlengthCls(self._core, self._cmd_group)
 		return self._plength
 
 	# noinspection PyTypeChecker
-	class DsmLengthStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Mode: enums.LenMode: DEFault | UDEFined DEFault: automatically calculated value UDEFined: configured Length
-			- Length: int: numeric Minimum number of bytes for UDEFined mode Range: 16 to 1500, Unit: byte"""
-		__meta_args_list = [
-			ArgStruct.scalar_enum('Mode', enums.LenMode),
-			ArgStruct.scalar_int('Length')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Mode: enums.LenMode = None
-			self.Length: int = None
-
-	# noinspection PyTypeChecker
-	def get_dsm_length(self) -> DsmLengthStruct:
-		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:DSMLength \n
-		Snippet: value: DsmLengthStruct = driver.trigger.rx.macFrame.get_dsm_length() \n
-		Defines the minimum length for the RX frame trigger mode DSSS/CCK Bursts, see method RsCmwWlanSig.Trigger.Rx.MacFrame.
-		btype. \n
-			:return: structure: for return value, see the help for DsmLengthStruct structure arguments.
-		"""
-		return self._core.io.query_struct('TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:DSMLength?', self.__class__.DsmLengthStruct())
-
-	def set_dsm_length(self, value: DsmLengthStruct) -> None:
-		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:DSMLength \n
-		Snippet: driver.trigger.rx.macFrame.set_dsm_length(value = DsmLengthStruct()) \n
-		Defines the minimum length for the RX frame trigger mode DSSS/CCK Bursts, see method RsCmwWlanSig.Trigger.Rx.MacFrame.
-		btype. \n
-			:param value: see the help for DsmLengthStruct structure arguments.
-		"""
-		self._core.io.write_struct('TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:DSMLength', value)
-
-	# noinspection PyTypeChecker
-	class OfmLengthStruct(StructBase):
-		"""Structure for reading output parameters. Fields: \n
-			- Mode: enums.LenMode: DEFault | UDEFined DEFault: automatically calculated value UDEFined: configured Length
-			- Length: int: numeric Range: 1 to 1500"""
-		__meta_args_list = [
-			ArgStruct.scalar_enum('Mode', enums.LenMode),
-			ArgStruct.scalar_int('Length')]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Mode: enums.LenMode = None
-			self.Length: int = None
-
-	# noinspection PyTypeChecker
-	def get_ofm_length(self) -> OfmLengthStruct:
-		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:OFMLength \n
-		Snippet: value: OfmLengthStruct = driver.trigger.rx.macFrame.get_ofm_length() \n
-		Defines the minimum length for the all OFDM RX frame trigger modes (all modes except All Bursts and DSSS/CCK Bursts) ,
-		see method RsCmwWlanSig.Trigger.Rx.MacFrame.btype. \n
-			:return: structure: for return value, see the help for OfmLengthStruct structure arguments.
-		"""
-		return self._core.io.query_struct('TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:OFMLength?', self.__class__.OfmLengthStruct())
-
-	def set_ofm_length(self, value: OfmLengthStruct) -> None:
-		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:OFMLength \n
-		Snippet: driver.trigger.rx.macFrame.set_ofm_length(value = OfmLengthStruct()) \n
-		Defines the minimum length for the all OFDM RX frame trigger modes (all modes except All Bursts and DSSS/CCK Bursts) ,
-		see method RsCmwWlanSig.Trigger.Rx.MacFrame.btype. \n
-			:param value: see the help for OfmLengthStruct structure arguments.
-		"""
-		self._core.io.write_struct('TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:OFMLength', value)
-
-	# noinspection PyTypeChecker
 	def get_btype(self) -> enums.BurstType:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:BTYPe \n
 		Snippet: value: enums.BurstType = driver.trigger.rx.macFrame.get_btype() \n
 		Defines for which bursts a trigger pulse is generated for the RX frame trigger signal. Note that the trigger pulse is
-		generated only for bursts matching the specified trigger bandwidth and trigger rate, see: method RsCmwWlanSig.Trigger.Rx.
-		MacFrame.bw method RsCmwWlanSig.Trigger.Rx.MacFrame.rate \n
+		generated only for bursts matching the specified trigger bandwidth and trigger rate. Refer to: method RsCmwWlanSig.
+		Trigger.Rx.MacFrame.bw method RsCmwWlanSig.Trigger.Rx.MacFrame.rate \n
 			:return: type_py: ABURsts | OBURsts | DCBursts | NHTBursts | HTBursts | VHTBursts | HESBursts ABURsts All received bursts result in an RX frame trigger pulse. OBURsts Only OFDM bursts with the configured minimum length result in an RX frame trigger pulse. DCBursts Only DSSS/CCK bursts with the configured minimum length result in an RX frame trigger pulse. NHTBursts Only non-HT bursts with the configured minimum length result in an RX frame trigger pulse. HTBursts Only HT bursts with the configured minimum length result in an RX frame trigger pulse. VHTBursts Only VHT bursts with the configured minimum length result in an RX frame trigger pulse. HESBursts Only HE SU bursts with the configured minimum length result in an RX frame trigger pulse.
 		"""
 		response = self._core.io.query_str('TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:BTYPe?')
 		return Conversions.str_to_scalar_enum(response, enums.BurstType)
 
 	def set_btype(self, type_py: enums.BurstType) -> None:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:BTYPe \n
 		Snippet: driver.trigger.rx.macFrame.set_btype(type_py = enums.BurstType.ABURsts) \n
 		Defines for which bursts a trigger pulse is generated for the RX frame trigger signal. Note that the trigger pulse is
-		generated only for bursts matching the specified trigger bandwidth and trigger rate, see: method RsCmwWlanSig.Trigger.Rx.
-		MacFrame.bw method RsCmwWlanSig.Trigger.Rx.MacFrame.rate \n
+		generated only for bursts matching the specified trigger bandwidth and trigger rate. Refer to: method RsCmwWlanSig.
+		Trigger.Rx.MacFrame.bw method RsCmwWlanSig.Trigger.Rx.MacFrame.rate \n
 			:param type_py: ABURsts | OBURsts | DCBursts | NHTBursts | HTBursts | VHTBursts | HESBursts ABURsts All received bursts result in an RX frame trigger pulse. OBURsts Only OFDM bursts with the configured minimum length result in an RX frame trigger pulse. DCBursts Only DSSS/CCK bursts with the configured minimum length result in an RX frame trigger pulse. NHTBursts Only non-HT bursts with the configured minimum length result in an RX frame trigger pulse. HTBursts Only HT bursts with the configured minimum length result in an RX frame trigger pulse. VHTBursts Only VHT bursts with the configured minimum length result in an RX frame trigger pulse. HESBursts Only HE SU bursts with the configured minimum length result in an RX frame trigger pulse.
 		"""
 		param = Conversions.enum_scalar_to_str(type_py, enums.BurstType)
 		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:BTYPe {param}')
 
 	# noinspection PyTypeChecker
 	def get_bw(self) -> enums.TriggerBandwidth:
@@ -220,14 +168,14 @@
 		Snippet: driver.trigger.rx.macFrame.set_slope(trig_slope = enums.TriggerSlope.FEDGe) \n
 		Aligns either the rising edge or the falling edge of the trigger pulses with the start of the MAC frames. \n
 			:param trig_slope: REDGe | FEDGe
 		"""
 		param = Conversions.enum_scalar_to_str(trig_slope, enums.TriggerSlope)
 		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:SLOPe {param}')
 
-	def clone(self) -> 'MacFrame':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MacFrameCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = MacFrame(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MacFrameCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame_/Plength.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/Plength.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Plength:
-	"""Plength commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class PlengthCls:
+	"""Plength commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("plength", core, parent)
+		self._cmd_group = CommandsGroup("plength", core, parent)
 
 	# noinspection PyTypeChecker
 	def get_mode(self) -> enums.LenMode:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:PLENgth:MODE \n
 		Snippet: value: enums.LenMode = driver.trigger.rx.macFrame.plength.get_mode() \n
 		Configures the length of generated RX MAC frame trigger pulses. \n
 			:return: pulse_length_mode: DEFault | UDEFined DEFault The pulse length is 1 µs. UDEFined The pulse length is specified via method RsCmwWlanSig.Trigger.Rx.MacFrame.Plength.value.
@@ -32,21 +32,21 @@
 		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:PLENgth:MODE {param}')
 
 	def get_value(self) -> float or bool:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:PLENgth:VALue \n
 		Snippet: value: float or bool = driver.trigger.rx.macFrame.plength.get_value() \n
 		Sets the pulse length for the mode UDEFined of the RX frame trigger, see method RsCmwWlanSig.Trigger.Rx.MacFrame.Plength.
 		mode. \n
-			:return: pulse_length_val: numeric | ON | OFF Range: 1E-6 s to 0.01 s
+			:return: pulse_length_val: (float or boolean) numeric | ON | OFF Range: 1E-6 s to 0.01 s
 		"""
 		response = self._core.io.query_str('TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:PLENgth:VALue?')
 		return Conversions.str_to_float_or_bool(response)
 
 	def set_value(self, pulse_length_val: float or bool) -> None:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:RX:MACFrame:PLENgth:VALue \n
 		Snippet: driver.trigger.rx.macFrame.plength.set_value(pulse_length_val = 1.0) \n
 		Sets the pulse length for the mode UDEFined of the RX frame trigger, see method RsCmwWlanSig.Trigger.Rx.MacFrame.Plength.
 		mode. \n
-			:param pulse_length_val: numeric | ON | OFF Range: 1E-6 s to 0.01 s
+			:param pulse_length_val: (float or boolean) numeric | ON | OFF Range: 1E-6 s to 0.01 s
 		"""
 		param = Conversions.decimal_or_bool_value_to_str(pulse_length_val)
 		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:RX:MACFrame:PLENgth:VALue {param}')
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Tx:
-	"""Tx commands group definition. 3 total commands, 1 Sub-groups, 0 group commands"""
+class TriggerCls:
+	"""Trigger commands group definition. 14 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("tx", core, parent)
+		self._cmd_group = CommandsGroup("trigger", core, parent)
 
 	@property
-	def macFrame(self):
-		"""macFrame commands group. 1 Sub-classes, 1 commands."""
-		if not hasattr(self, '_macFrame'):
-			from .Tx_.MacFrame import MacFrame
-			self._macFrame = MacFrame(self._core, self._base)
-		return self._macFrame
+	def rx(self):
+		"""rx commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_rx'):
+			from .Rx import RxCls
+			self._rx = RxCls(self._core, self._cmd_group)
+		return self._rx
 
-	def clone(self) -> 'Tx':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	@property
+	def tx(self):
+		"""tx commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_tx'):
+			from .Tx import TxCls
+			self._tx = TxCls(self._core, self._cmd_group)
+		return self._tx
+
+	def clone(self) -> 'TriggerCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = Tx(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = TriggerCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Tx/MacFrame/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
-from ....Internal import Conversions
-from .... import enums
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
+from .....Internal import Conversions
+from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MacFrame:
-	"""MacFrame commands group definition. 3 total commands, 1 Sub-groups, 1 group commands"""
+class MacFrameCls:
+	"""MacFrame commands group definition. 3 total commands, 1 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("macFrame", core, parent)
+		self._cmd_group = CommandsGroup("macFrame", core, parent)
 
 	@property
 	def plength(self):
 		"""plength commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_plength'):
-			from .MacFrame_.Plength import Plength
-			self._plength = Plength(self._core, self._base)
+			from .Plength import PlengthCls
+			self._plength = PlengthCls(self._core, self._cmd_group)
 		return self._plength
 
 	# noinspection PyTypeChecker
 	def get_slope(self) -> enums.TriggerSlope:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:TX:MACFrame:SLOPe \n
 		Snippet: value: enums.TriggerSlope = driver.trigger.tx.macFrame.get_slope() \n
 		Aligns either the rising edge or the falling edge of the trigger pulses with the start of the MAC frames. \n
@@ -35,14 +35,14 @@
 		Snippet: driver.trigger.tx.macFrame.set_slope(trig_slope = enums.TriggerSlope.FEDGe) \n
 		Aligns either the rising edge or the falling edge of the trigger pulses with the start of the MAC frames. \n
 			:param trig_slope: REDGe | FEDGe
 		"""
 		param = Conversions.enum_scalar_to_str(trig_slope, enums.TriggerSlope)
 		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:TX:MACFrame:SLOPe {param}')
 
-	def clone(self) -> 'MacFrame':
-		"""Clones the group by creating new object from it and its whole existing sub-groups
+	def clone(self) -> 'MacFrameCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = MacFrame(self._core, self._base.parent)
-		self._base.synchronize_repcaps(new_group)
+		new_group = MacFrameCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame_/Plength.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Implementations/Trigger/Tx/MacFrame/Plength.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class Plength:
-	"""Plength commands group definition. 2 total commands, 0 Sub-groups, 2 group commands"""
+class PlengthCls:
+	"""Plength commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._base = CommandsGroup("plength", core, parent)
+		self._cmd_group = CommandsGroup("plength", core, parent)
 
 	# noinspection PyTypeChecker
 	def get_mode(self) -> enums.PulseLengthMode:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:TX:MACFrame:PLENgth:MODE \n
 		Snippet: value: enums.PulseLengthMode = driver.trigger.tx.macFrame.plength.get_mode() \n
 		Configures the length of generated TX MAC frame trigger pulses. \n
 			:return: pulse_length_mode: DEFault | BLENgth | UDEFined DEFault The pulse length is 1 µs. BLENgth The pulse length equals the burst length. UDEFined The pulse length is specified via method RsCmwWlanSig.Trigger.Tx.MacFrame.Plength.value.
@@ -32,21 +32,21 @@
 		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:TX:MACFrame:PLENgth:MODE {param}')
 
 	def get_value(self) -> float or bool:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:TX:MACFrame:PLENgth:VALue \n
 		Snippet: value: float or bool = driver.trigger.tx.macFrame.plength.get_value() \n
 		Sets the pulse length for the mode UDEFined of the TX frame trigger, see method RsCmwWlanSig.Trigger.Tx.MacFrame.Plength.
 		mode. \n
-			:return: pulse_length_val: numeric | ON | OFF Range: 1E-6 s to 0.01 s
+			:return: pulse_length_val: (float or boolean) numeric | ON | OFF Range: 1E-6 s to 0.01 s
 		"""
 		response = self._core.io.query_str('TRIGger:WLAN:SIGNaling<Instance>:TX:MACFrame:PLENgth:VALue?')
 		return Conversions.str_to_float_or_bool(response)
 
 	def set_value(self, pulse_length_val: float or bool) -> None:
 		"""SCPI: TRIGger:WLAN:SIGNaling<instance>:TX:MACFrame:PLENgth:VALue \n
 		Snippet: driver.trigger.tx.macFrame.plength.set_value(pulse_length_val = 1.0) \n
 		Sets the pulse length for the mode UDEFined of the TX frame trigger, see method RsCmwWlanSig.Trigger.Tx.MacFrame.Plength.
 		mode. \n
-			:param pulse_length_val: numeric | ON | OFF Range: 1E-6 s to 0.01 s
+			:param pulse_length_val: (float or boolean) numeric | ON | OFF Range: 1E-6 s to 0.01 s
 		"""
 		param = Conversions.decimal_or_bool_value_to_str(pulse_length_val)
 		self._core.io.write(f'TRIGger:WLAN:SIGNaling<Instance>:TX:MACFrame:PLENgth:VALue {param}')
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgLinkedEventArgs.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgLinkedEventArgs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Class defining Linked argument Event."""
+
 import time
 
 
 class ArgLinkedEventArgs(object):
 	"""Contains event data for suppressed argument."""
 
 	def __init__(self, link_name: str, arg_name: str, value: object = None, context: str = '', timestamp: time = None):
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgSingle.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgSingle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,57 @@
+"""Single argument definition for a scalar argument."""
+
 from .ConverterFromScpiString import ConverterFromScpiString
 from .ConverterToScpiString import ConverterToScpiString
+from .InstrumentErrors import RsInstrException
+
 from .Types import DataType
 
 
 class ArgSingle(object):
 	"""Single Argument outside a structure - used for composing query arguments.
 	Contains the argument value as well (self.value)."""
 
-	def __init__(self, name: str, value, data_type: DataType, is_optional: bool = False, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
+	def __init__(self, name: str, value, data_type: DataType, enum_type=None, is_optional: bool = False, is_open_list: bool = False, repetition: int = 1, intern_link: str = None):
 		self.name = name if name else ''
 		self.argument_ix = None
 		self.value = value
 		self.data_type = data_type
+		self.enum_type = enum_type
 		self.is_optional = is_optional
 		self.is_open_list = is_open_list
 		self.repetition = repetition
 		self.intern_link = intern_link
 		self.conv_from_scpi_string = None
 		self.conv_to_scpi_string = None
 
-		if self.data_type == DataType.Enum:
-			self.assert_mandatory_has_value(self)
-			if self.value is not None:
-				self.enum_type = type(self.value)
-				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
-				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
-		elif self.data_type == DataType.EnumList:
-			self.assert_mandatory_has_value(self)
+		if self.data_type.is_scalar_enum:
+			# self.assert_mandatory_has_value(self)
+			self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
+			self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
+		elif self.data_type.is_list_enum:
+			# self.assert_mandatory_has_value(self)
 			if self.value is not None:
-				self.enum_type = type(self.value[0])
 				self.conv_from_scpi_string = ConverterFromScpiString(self.data_type, self.enum_type)
 				self.conv_to_scpi_string = ConverterToScpiString(self.data_type, self.enum_type)
 		else:
 			self.conv_from_scpi_string = ConverterFromScpiString(self.data_type)
 			self.conv_to_scpi_string = ConverterToScpiString(self.data_type)
 
 		self.check_consistency()
 
 	@classmethod
-	def as_open_list(cls, name: str, value: object, data_type: DataType) -> 'ArgSingle':
+	def as_open_list(cls, name: str, value: object, data_type: DataType, enum_type=None) -> 'ArgSingle':
 		"""Creates new ArgSingle of open list type.Use this method for all non-interleaved list types. \n
-		:param name: name of the argument.
-		:param value: value of the argument.
-		:param data_type: data type of the argument.
-		:return: ArgSingle object of an open list type."""
-		return cls(name, value, data_type, False, True, 1, None)
+		:param name: name of the argument
+		:param value: value of the argument
+		:param data_type: data type of the argument
+		:param enum_type: enum type if the data_type is Enum or EnumExt (or list of those)
+		:return: ArgSingle object of an open list type"""
+		return cls(name, value, data_type, enum_type, False, True, 1, None)
 
 	def __str__(self):
 		opt = '~' if self.is_optional else ''
 		name = f" '{self.name}'" if self.name != '' else ''
 		out = f"SingleArg {opt}{self.data_type.name}{name}"
 
 		if self.is_open_list is False and self.repetition > 1:
@@ -72,15 +75,15 @@
 
 	# noinspection PyUnusedLocal
 	def assert_is_optional(self, obj=None) -> None:
 		"""Asserts that the parameter is optional.
 		If not, the method throws an exception."""
 		if self.is_optional:
 			return
-		raise Exception(f'Single argument is not optional: {self}')
+		raise RsInstrException(f'Single argument is not optional: {self}')
 
 	# noinspection PyUnusedLocal
 	def assert_mandatory_has_value(self, value_obj=None) -> None:
 		"""Asserts that if the parameter is mandatory, it must have value assigned.
 		If not, the method throws an exception."""
 		if self.is_optional:
 			return
@@ -93,11 +96,11 @@
 
 	def check_consistency(self) -> None:
 		"""Checks the consistency of the object"""
 		if self.value is None:
 			return
 		if isinstance(self.value, list):
 			if self.data_type.is_scalar:
-				raise Exception(f'Argument real data type is list, but it is declared as {self.data_type}. Value: {self.value}')
+				raise RsInstrException(f'Argument real data type is list, but it is declared as {self.data_type}. Value: {self.value}')
 		else:
 			if self.data_type.is_list:
-				raise Exception(f'Argument real data type is scalar, but it is declared as {self.data_type}. Value: {self.value}')
+				raise RsInstrException(f'Argument real data type is scalar, but it is declared as {self.data_type}. Value: {self.value}')
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgSingleList.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgSingleList.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Single argument definition for a list argument."""
+
 from .ArgSingle import ArgSingle
 from .ArgStringComposer import compose_cmd_string_from_single_args
 
 
 class ArgSingleList(object):
 	"""Contains methods for composing cmd string for the list of single arguments.
 	Used in methods with 1+ set or query arguments.
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgSingleSuppressed.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgSingleSuppressed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Contains definition for an argument that is suppressed and not exposed to the user.
+Usually such arguments are also linked to a callback."""
+
 from .Types import DataType
 
 
 class ArgSingleSuppressed(object):
 	"""Single suppressed Argument - used in Query_XxXx_Suppressed() to remove it from the returned value.
 	It does not contain:
 	- 'value' attribute, since this is discarded or linked internally directly  in the Query_XxXx_Suppressed().
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgStringComposer.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgStringComposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 The composing of the SCPI parameter string is similar for the ArgStruct and ArgSingle[] objects, therefore they share the same module."""
 
 from typing import Dict
 
 from .ArgSingle import ArgSingle
 from .ArgStruct import ArgStruct
 from .Utilities import get_plural_string
+from .InstrumentErrors import RsInstrException
 
 
 class SingleComposer:
 	"""Composes strings for single argument.
 	Provides Composer interface with 3 functions:
 	- from_scalar_arg
 	- from_list_arg
@@ -135,15 +136,15 @@
 					# The last argument, ignore the repetitions and convert the whole list to string
 					string_arg.append(composer.from_list_arg(arg))
 				else:
 					# The optional argument, which has no value. End the entire string_arg composition
 					arg.assert_is_optional(values_obj)
 					opt_null_ix = arg_ix
 			else:
-				# More than one arguments remaining. Loop through them interleaving the result strings
+				# More than one argument remaining. Loop through them interleaving the result strings
 				# Interleaving arguments must all have values
 
 				# Check if each list has at least Repetition number of elements
 				cycles_error = False
 				alignments_error = False
 				cycle = -1
 				data = {}
@@ -151,19 +152,18 @@
 					arg = args[x]
 					curr_size: int = composer.get_arg_list_size(arg)
 					curr_cycle: int = curr_size // arg.repetition
 					curr_align: int = curr_size % arg.repetition
 					data[x] = (curr_size, curr_cycle, curr_align)
 
 					if curr_size < 0:
-						raise Exception(
-							f"Argument '{arg.name}' has repetitions, therefore it must be declared as a list. Current Declaration: '{arg.data_type}'")
+						raise RsInstrException(f"Argument '{arg.name}' has repetitions, therefore it must be declared as a list. Current Declaration: '{arg.data_type}'")
 
 					if arg.repetition > curr_size:
-						raise Exception(f"Argument '{arg.name}' has repetitions {arg.repetition}, but its list size is only {curr_size}")
+						raise RsInstrException(f"Argument '{arg.name}' has repetitions {arg.repetition}, but its list size is only {curr_size}")
 
 					# noinspection PyChainedComparisons
 					if cycle >= 0 and curr_cycle != cycle:
 						cycles_error = True
 
 					cycle = curr_cycle
 
@@ -171,23 +171,21 @@
 						alignments_error = True
 
 				if cycles_error:
 					message = 'Arguments interleaving is not aligned - all the cycles must be the same. Actual cycles:\n'
 					for x in range(arg_ix, arg_count):
 						message += f'{args[x].name}[{data[x][0]}] sliced by {get_plural_string("element", args[x].repetition)} ' \
 							f'results in {data[x][0] / args[x].repetition} cycles\n'
-
-					raise Exception(message)
+					raise RsInstrException(message)
 
 				if alignments_error:
 					message = 'At least one argument has a list size not dividable by the defined repetitions:\n'
 					for x in range(arg_ix, arg_count):
 						message += f'{args[x].name}[{data[x][0]}] modulo {args[x].repetition}x results in {data[x][0] % args[x].repetition}\n'
-
-					raise Exception(message)
+					raise RsInstrException(message)
 
 				for x in range(cycle):
 					for y in range(arg_ix, arg_count):
 						arg = args[y]
 						string_arg.append(composer.from_list_arg(arg, arg.repetition * x, arg.repetition))
 
 	if opt_null_ix >= 0:
@@ -198,15 +196,15 @@
 			if arg.has_value(values_obj):
 				rest.append(arg.name)
 
 		if len(rest):
 			msg = f"Optional Argument '{args[opt_null_ix].name}' has no value, but the further ones do. " \
 				f"If you skip an optional argument, you have to skip all the ones following it. " \
 				f"Clear the values for the rest of the argument(s):\n{', '.join(rest)}"
-			raise Exception(msg)
+			raise RsInstrException(msg)
 
 	return ','.join(string_arg)
 
 
 def compose_cmd_string_from_single_args(args: Dict[int, ArgSingle]) -> str:
 	"""Returns SCPI-composed string based on the single args specification.
 	We can use the same function as for the struct arguments, with the difference of providing a SingleComposer.
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgStruct.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgStruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+"""Definition for an argument which is a part of a structure."""
+
 from .ConverterFromScpiString import ConverterFromScpiString
 from .ConverterToScpiString import ConverterToScpiString
 from .Types import DataType
+from .InstrumentErrors import RsInstrException
 
 
 class ArgStruct(object):
 	"""Describes an argument in data structures.
 	This info is used to parse a string query response to the output structure,
 	or to parse the output structure to the string parameter for writing.
 	Contains reference to the value in the owning structure."""
@@ -121,17 +124,17 @@
 	def assert_is_optional(self, obj) -> None:
 		"""Asserts that the parameter is optional.
 		If not, the method throws an exception."""
 		if self.is_optional:
 			return
 		value = getattr(obj, self.name)
 		if value is None:
-			raise Exception(f"Structure '{obj}', argument without value is not optional: {self}")
+			raise RsInstrException(f"Structure '{obj}', argument without value is not optional: {self}")
 		else:
-			raise Exception(f"Structure '{obj}', argument is not optional: {self}', value '{value}'")
+			raise RsInstrException(f"Structure '{obj}', argument is not optional: {self}', value '{value}'")
 
 	def assert_mandatory_has_value(self, obj) -> None:
 		"""Asserts that if the parameter is mandatory, it must have value assigned.
 		If not, the method throws an exception."""
 		if self.is_optional:
 			return
 		if getattr(obj, self.name) is None:
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgStructList.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgStructList.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+"""See the class docstring."""
+
 from .ArgStringComposer import StructComposer, compose_cmd_string_from_struct_args
 from .ArgStructStringParser import ArgStructStringParser
 from .StructBase import StructBase
+from .InstrumentErrors import RsInstrException
 
 
 class ArgStructList(object):
 	"""Contains methods for composing cmd string and parsing cmd response to the provided structure instance."""
 
 	RAW_DATA_PROP_NAME = 'RawReturnData'
 
@@ -53,22 +56,22 @@
 			# Still some args to go
 			if arg.is_open_list is True:
 				# The previous loop ended because the next argument had is_open_list True
 				if arg_ix == (arg_count - 1):
 					# This is the last argument, ignore the repetitions and take the whole rest of the elements
 					parser.to_list_value(arg, True, 0, parser.remaining, parser.remaining, 1)
 				else:
-					# More than one arguments remaining. Loop through them interleaving the result strings
+					# More than one argument remaining. Loop through them interleaving the result strings
 					open_list_args = {key: value for key, value in self.args.items() if key >= arg_ix}
 
 					# Accumulate the number of repetitions from all the open_list_args
 					period: int = sum(open_list_args[ix].repetition for ix in open_list_args)
 					reminder: int = parser.remaining % period
 					if reminder != 0:
-						raise Exception(
+						raise RsInstrException(
 							f'Arguments parsing is not aligned - source string elements remaining to parse {parser.remaining}'
 							f'is not dividable by the summary Period {period} of all the open list arguments:\n' + '\n'.join(['{}'.format(x) for x in open_list_args]))
 					# Go through the arguments and accumulate the list content
 					offset = 0
 					for x in open_list_args:
 						arg = open_list_args[x]
 						parser.to_list_value(arg, False, offset, arg.repetition, period, -1)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ArgStructStringParser.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ArgStructStringParser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+"""See the class docstring."""
+
 from . import Utilities
 from .ArgStruct import ArgStruct
+from .InstrumentErrors import RsInstrException
 
 
 class ArgStructStringParser:
 	"""Class for parsing a response from the instrument to an output structure of arguments.
 	It is used by the ArgStructList class for filling structures with return values."""
 
 	def __init__(self, struct, value: str):
@@ -17,34 +20,34 @@
 		"""Remaining items to parse."""
 		return self.count - self.position
 
 	def to_scalar_value(self, arg: ArgStruct):
 		"""Parses the current element to a scalar argument."""
 		assert arg.data_type.is_scalar, f'to_scalar_value() method only works with scalar values. Data type: {arg.data_type}'
 		if self.position >= self.count:
-			raise Exception(
+			raise RsInstrException(
 				f"Cannot parse a scalar value to structure argument. Response contains only {self.count} elements, "
 				f"argument '{arg.name}' has position {self.position + 1}.\n"
 				f"Response (commas replaced by new lines):\n" + Utilities.truncate_string_from_end('\n'.join(self.elements), 1000))
 		string = self.elements[self.position]
 		value = arg.conv_from_scpi_string.get_one_element_value(string)
 		setattr(self.struct, arg.name, value)
 		self.position += 1
 
 	def to_list_value(self, arg: ArgStruct, increase_pos: bool, offset: int, count: int, period: int, cycles: int) -> None:
 		"""Parses more elements to the list argument - slicing."""
 		assert arg.data_type.is_list, f'to_list_value method only works with list values. Data type: {arg.data_type}'
 		if cycles < 0:
 			cycles = self.remaining // period
 		if self.position >= self.count:
-			raise Exception(
+			raise RsInstrException(
 				f"Cannot parse an list value to the argument '{arg.name}', "
 				f"because the element position {self.position} is over the parsed list length {self.count}")
 		if (self.position + offset + count) > self.count:
-			raise Exception(
+			raise RsInstrException(
 				f"Cannot parse the whole list value to the argument '{arg.name}', because the element position {self.position} "
 				f"plus the argument offset {offset} and argument length {count} would be over the parsed list length {self.count}")
 
 		result = []
 		for cycle in range(cycles):
 			start_ix = self.position + (cycle * period) + offset
 			for i in range(count):
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/CommandsGroup.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/CommandsGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""See the class docstring."""
+
 from enum import Enum
 from typing import List
 from .Core import Core
 from .RepeatedCapability import RepeatedCapability as RepCap
 from .InstrumentErrors import DriverValueError
 
 
@@ -38,27 +40,27 @@
 		return self.multi_repcap_types != ''
 
 	def add_existing_child(self, child: 'CommandsGroup') -> None:
 		"""Adds the child to the parent's list of created children.
 		This is used when the group is cloned, where the whole existing tree of groups have to be recreated"""
 		self.existing_children.append(child)
 
-	def set_repcap_enum_value(self, enum_value: Enum) -> None:
-		"""Sets RepCap value as enum
-		Default is not allowed."""
+	def set_repcap_enum_value(self, enum_value: Enum or int) -> None:
+		"""Sets RepCap value as enum or integer
+		Default is not allowed here."""
 		try:
 			self.rep_cap.set_enum_value(enum_value)
 		except ValueError:
 			raise DriverValueError(self.io.resource_name, f"Commands group RepCap value '{self.rep_cap.name}.Default' cannot be set. Please select a concrete value.")
 
 	def get_repcap_enum_value(self) -> Enum:
 		"""Returns RepCap value as enum"""
 		return self.rep_cap.get_enum_value()
 
-	def get_repcap_cmd_value(self, enum_value: Enum, enum_type) -> str:
+	def get_repcap_cmd_value(self, enum_value: Enum or int, enum_type) -> str:
 		"""Returns the current string of RepCapCmdValue for the entered RepCapEnumName
 		The enum_value can be a repcap of the current CommandsGroup or any of their parents"""
 		# Use the static functions of the RepeatedCapability to get the non-default value
 		# It is faster, since there is no need to use the RepCap instance
 		if not RepCap.clsm_is_default_value(enum_value, enum_type):
 			return RepCap.clsm_get_cmd_string_value(enum_value, enum_type)
 		# Default value - get it from the group or the parent groups
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Conversions.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Conversions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+"""Contains conversion functions for SCPI string -> parameter and vice versa."""
+
 import math
 import struct
 import sys
 from enum import Enum
-from typing import List
+from typing import List, Tuple
+from .ScpiEnums import ScpiEnum, enum_spec_prefixes, enum_spec_strings
+from .Properties import Properties
+from datetime import datetime
 
 from . import Utilities
+from .InstrumentErrors import RsInstrException
 
 
 class BinFloatFormat(Enum):
 	"""Binary format of a float number."""
 	Single_4bytes = 1
 	Single_4bytes_swapped = 2
 	Double_8bytes = 3
@@ -24,15 +30,15 @@
 
 
 def assert_string_data(value: str) -> None:
 	"""Asserts value is string type."""
 	assert isinstance(value, str), f"Input value type must be string. Actual type: {type(value)}, value: {value}"
 
 
-def assert_list_data(value: list) -> None:
+def assert_list_data(value: List) -> None:
 	"""Asserts value is list type."""
 	assert isinstance(value, list), f"Input value type must be a list. Actual type: {type(value)}, value: {value}"
 
 
 def _get_endianness_symbol(swap_endianness: bool) -> str:
 	"""Based on the current endianness returns the symbol used in the 'struct' module."""
 	if swap_endianness is False:
@@ -143,15 +149,15 @@
 bool_true_lookup = frozenset(['1', 'on', 'On', 'ON', 'true', 'True', 'TRUE'])
 bool_false_lookup = frozenset(['0', 'off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
 pure_bool_false_lookup = frozenset(['off', 'Off', 'OFF', 'false', 'False', 'FALSE'])
 
 
 def str_to_bool(string: str) -> bool:
 	"""Converts string to boolean value.
-	The function robust, and case insensitive.
+	The function is robust, and case-insensitive.
 	If the string can not be converted to a boolean, the function returns False."""
 	assert_string_data(string)
 	if string in bool_true_lookup:
 		return True
 	if string in bool_false_lookup:
 		return False
 	# If leading/trailing spaces
@@ -193,24 +199,38 @@
 
 
 number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
 number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
 number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
 number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
 number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
+number_si_suffix = {
+	'pHz': 1E-12, 'MHz': 1E+6, 'kHz': 1E+3, 'GHz': 1E+9, 'mHz': 1E-3, 'uHz': 1E-6, 'µHz': 1E-6, 'THz': 1E+12, 'nHz': 1E-9, 'ns': 1E-9, 'fW': 1E-15,
+	'pW': 1E-12, 'nW': 1E-9, 'uW': 1E-6, 'µW': 1E-6, 'mW': 1E-3, 'kW': 1E3, 'MW': 1E6, 'GW': 1E9, 'MV': 1E+6, 'MA': 1E+6, 'ps': 1E-12, 'fs': 1E-15,
+	'km': 1E+3, 'kV': 1E+3, 'kA': 1E+3, 'pF': 1E-2, 'Hz': 1.0, 'mm': 1E-3, 'mA': 1E-3, 'mF': 1E-3, 'mV': 1E-3, 'pV': 1E-12, 'nF': 1E-9, 'nA': 1E-9,
+	'nV': 1E-9, 'nm': 1E-9, 'pm': 1E-12, 'us': 1E-6, 'µs': 1E-6, 'uF': 1E-6, 'µF': 1E-6, 'ms': 1E-3, 'uA': 1E-6, 'µA': 1E-6, 'uV': 1E-6, 'µV': 1E-6,
+	'um': 1E-6, 'µm': 1E-6, 'pA': 1E-12, 'V': 1, 'W': 1, 'A': 1, 'F': 1, 's': 1, 'm': 1}
 int_neg_inf = -(sys.maxsize - 1)
-enum_spec_prefixes = {'_minus': '-', '_plus': '+', '_': ''}
-enum_spec_strings = {'_dash_': '-', '_dot_': '.'}
+
+
+def strip_si_suffix(string: str) -> Tuple[bool, str, float]:
+	"""Tries to find defined suffixes in the text and returns the stripped text and the multiplier as double number.
+	If no known suffix is detected, the method returns false, strippedText=text, multiplier=1.0
+	Example: text='123 MHz' strippedText='123' multiplier=1E6"""
+	for suffix in number_si_suffix.keys():
+		if string.endswith(suffix):
+			return True, string[:-len(suffix)].rstrip(), number_si_suffix[suffix]
+	return False, string, 1.0
 
 
 def str_to_int(string: str) -> int:
 	"""Converts string to integer value. Float values are coerced to integer.
-	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
+	Also recognizes case-insensitive special values like NaN, INV, NCAP..."""
 	assert_string_data(string)
-	string = string.strip()
+	string = string.strip(" \t\r\n'\"")
 	if string == '':
 		return 0
 	value = str_special_values_to_int(string)
 	if value:
 		return value
 
 	# Hexadecimal numbers
@@ -232,15 +252,24 @@
 		if ',' in string:
 			return int(string[2:string.find(',')], 8)
 		else:
 			return int(string[2:], 8)
 	# Simulation
 	if string == 'Simulating':
 		return 0
-	return int(round(float(string)))
+	try:
+		return int(round(float(string)))
+	except ValueError:
+		result = strip_si_suffix(string)
+		if result[0] is False:
+			raise
+		try:
+			return int(round(float(result[1]) * result[2]))
+		except ValueError:
+			raise ValueError(f"could not convert string to integer: '{string}'")
 
 
 def str_special_values_to_int(string: str) -> int:
 	"""Converts special string values to integer. Returns None if no special value was found."""
 	assert_string_data(string)
 	if string in number_plus_inf_lookup or string in number_max_lookup:
 		return sys.maxsize
@@ -270,17 +299,17 @@
 	if result is not None:
 		return result
 	return str_to_int(string)
 
 
 def str_to_float(string: str) -> float:
 	"""Converts string to float value.
-	Also recognizes case insensitive special values like NaN, INV, NCAP..."""
+	Also recognizes case-insensitive special values like NaN, INV, NCAP..."""
 	assert_string_data(string)
-	string = string.strip()
+	string = string.strip(" \t\r\n'\"")
 	if string == '':
 		return 0.0
 	if string in number_plus_inf_lookup:
 		return math.inf
 	if string in number_minus_inf_lookup:
 		return -math.inf
 	if string in number_nan_lookup:
@@ -299,15 +328,24 @@
 		return -sys.float_info.max / 100
 	if string == 'ULEU':
 		return sys.float_info.max / 10
 	if string == 'ULEL':
 		return -sys.float_info.max / 10
 	if string == 'Simulating':
 		return 0.0
-	return float(string)
+	try:
+		return float(string)
+	except ValueError:
+		result = strip_si_suffix(string)
+		if result[0] is False:
+			raise
+		try:
+			return float(result[1]) * result[2]
+		except ValueError:
+			raise ValueError(f"could not convert string to float: '{string}'")
 
 
 def str_to_float_or_bool(string: str) -> float or bool:
 	"""Similar to str_to_float, but for special values "ON/OFF" the function returns boolean"""
 	result = string_to_pure_bool(string)
 	if result is not None:
 		return result
@@ -320,24 +358,24 @@
 
 
 def bool_to_str(value: bool) -> str:
 	"""Converts boolean to 'ON' or 'OFF' string."""
 	if type(value) is bool:
 		return 'ON' if value is True else 'OFF'
 	else:
-		raise Exception(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
+		raise RsInstrException(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
 
 
 def str_enclose_by_quotes(string: str) -> str:
 	"""Returns string enclosed by single quotes."""
 	assert_string_data(string)
-	return "'" + string + "'"
+	return Properties.scpi_quotes + string + Properties.scpi_quotes
 
 
-def list_to_csv_str(value: list) -> str:
+def list_to_csv_str(value: List, delimiter: str = ',') -> str:
 	"""Converts list of elements to strings separated by commas.
 	Element types can differ on an individual basis.
 	Supported element types:
 	- int
 	- bool
 	- float
 	- string -> string no quotes
@@ -345,18 +383,18 @@
 	assert_list_data(value)
 	result = []
 	for x in value:
 		el = value_to_str(x)
 		if not el:
 			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_str: '{x}'")
 		result.append(el)
-	return ','.join(result)
+	return delimiter.join(result)
 
 
-def list_to_csv_quoted_str(value: list) -> str:
+def list_to_csv_quoted_str(value: List) -> str:
 	"""Converts list of elements to quoted strings separated by commas.
 	Only string elements are enclosed by single quotes
 	Element types can differ on an individual basis.
 	Supported element types:
 	- int
 	- bool
 	- float
@@ -368,29 +406,28 @@
 		if isinstance(x, str):
 			el = str_enclose_by_quotes(x)
 		else:
 			el = value_to_str(x)
 		if not el:
 			raise TypeError(f"List element type is not supported by Conversions.list_to_csv_quoted_str: '{x}'")
 		result.append(el)
-
 	return ','.join(result)
 
 
 def decimal_value_to_str(x: int or float) -> str:
 	"""Converts scalar decimal value to string.
 	Supported element types:
 	- int
 	- float"""
 	if isinstance(x, int) and type(x) is not bool:
 		return str(x)
 	elif isinstance(x, float):
 		return float_to_str(x)
 	else:
-		raise Exception(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
+		raise RsInstrException(f"decimal_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer and float types are supported.")
 
 
 def decimal_or_bool_value_to_str(x: int or float or bool) -> str:
 	"""Converts scalar decimal value to string.
 	Supported element types:
 	- int
 	- float
@@ -398,15 +435,15 @@
 	if type(x) is bool:
 		return bool_to_str(x)
 	if isinstance(x, int):
 		return str(x)
 	elif isinstance(x, float):
 		return float_to_str(x)
 	else:
-		raise Exception(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
+		raise RsInstrException(f"decimal_or_bool_value_to_str: unsupported variable type '{type(x)}', value '{x}'. Only integer, float and boolean types are supported.")
 
 
 def value_to_str(x: int or bool or float or str or Enum) -> str:
 	"""Converts scalar value to string.
 	Supported element types:
 	- int
 	- bool
@@ -418,17 +455,19 @@
 	elif isinstance(x, int):
 		return str(x)
 	elif isinstance(x, float):
 		return float_to_str(x)
 	elif isinstance(x, str):
 		return x
 	elif isinstance(x, Enum):
+		if isinstance(x.value, str):
+			return enum_value_to_scpi_string(x.value)
 		return enum_value_to_scpi_string(x.name)
 	else:
-		raise Exception(f"value_to_str: unsupported variable type '{type(x)}', value '{x}'. Supported types: int, bool, float, str, enum.")
+		raise RsInstrException(f"value_to_str: unsupported variable type '{type(x)}', value '{x}'. Supported types: int, bool, float, str, enum.")
 
 
 def enum_value_to_scpi_string(enum_value: str) -> str:
 	"""Conversion EnumValue -> SCPI_String
 	Unescapes all the special characters that can not be contained in the enum member definition, but can be sent to the instrument as enum string.
 	Use this to send the scpi enum value to the instrument."""
 	for key in enum_spec_prefixes:
@@ -443,15 +482,15 @@
 	"""Converts scalar value to string enclosed by single quotes.
 	Supported element types:
 	- int
 	- bool
 	- float
 	- string
 	- enum"""
-	return f"'{value_to_str(x)}'"
+	return Properties.scpi_quotes + value_to_str(x) + Properties.scpi_quotes
 
 
 def str_to_float_list(string: str) -> List[float]:
 	"""Converts string with comma-separated values to list of Floats."""
 	assert_string_data(string)
 	if not string:
 		return []
@@ -504,103 +543,158 @@
 		return []
 	result = [*map(Utilities.trim_str_response, string.split(','))]
 	if clear_one_empty_item and len(result) == 1 and result[0] == '':
 		return []
 	return result
 
 
-def _find_in_enum_members(item: str, enum_members: List[str]) -> int:
-	"""Matches a string in the provided list of member strings.
-	The item must be not fully matched.
-	The item is matched if a member string starts with the item (the item is a prefix of the member).
-	Example: item='CONN' will match the enum_member 'CONNected'
-	If the item contains a comma, only the value before comma is considered
-	Returns found index in the enum_members list"""
-	if ',' in item:
-		item = item[:item.index(',')].strip()
-	i = 0
-	for x in enum_members:
-		if x.startswith(item):
-			return i
-		i += 1
-
-	# smart matching:
-	# item = 'MAX' matches enum 'MAXpeak'
-	# item = 'SPECtrum1' matches enum 'SPEC1'
-	# item = 'SPEC' matches enum 'SPECtrum1'
-
-	item = ''.join([c for c in item if not c.islower()])
-	# item must be longer than 1 character
-	if len(item) < 2:
-		return -1
-	i = 0
-	for x in enum_members:
-		x_uc = ''.join([c for c in x if not c.islower()])
-		if x_uc == item:
-			return i
-		i += 1
-	return -1
-
-
-def str_to_scalar_enum_helper(string: str, enum_type: Enum, enum_members=None) -> Enum:
+def str_to_scalar_enum_helper(string: str, scpi_enum: ScpiEnum, array_search: bool, exc_if_not_found) -> Enum:
 	"""Converts string to one enum element.
-	enum_members are optional to improve the performance for repeated conversions.
-	If you do not provide them, they are generated inside the function."""
-	value = Utilities.trim_str_response(string)
-	if not enum_members:
-		# noinspection PyTypeChecker
-		enum_members = [x.name for x in enum_type]
-
-	# Search in the enum member and return the index of the matched item
-	ix = _find_in_enum_members(value, enum_members)
-	if ix >= 0:
-		# noinspection PyUnresolvedReferences
-		return enum_type[enum_members[ix]]
-
-	# If the result is -1 (not found), try to replace the special values and search again
-	# This is done to improve the performance, since most of the enums have no special values
-	enum_members_conv = [enum_value_to_scpi_string(x) for x in enum_members]
-	ix = _find_in_enum_members(value, enum_members_conv)
-	if ix >= 0:
-		# noinspection PyUnresolvedReferences
-		return enum_type[enum_members[ix]]
-
+	array_search signal no need to force the comma removing,
+	because the elements definitely do not have any commas - commas have been used to split string to the list of strings
+	The function can also return:
+	- integer special value, if the string was not found in the enum, and it is a special value.
+	- input string, if the string was not found and raise_if_not_found is set to False - used for the EnumExt types."""
+	if scpi_enum.has_quotes:
+		value = Utilities.trim_str_response(string, mode=Utilities.TrimStringMode.white_chars_double_quotes)
+	else:
+		value = Utilities.trim_str_response(string)
+	enum_value = scpi_enum.find_in_enum_members(value, False)
+	if enum_value is not None:
+		return enum_value
+	if array_search is False:
+		# If the result is still -1 (not found), try to force removing the comma in the string.
+		enum_value = scpi_enum.find_in_enum_members(value, True)
+		if enum_value is not None:
+			return enum_value
 	# If not found, search in the special integer numbers:
 	spec_value = str_special_values_to_int(value)
-	if not spec_value:
-		raise Exception(f"String '{value}' can not be found in the enum type '{enum_type}'")
+	if spec_value:
+		# noinspection PyTypeChecker
+		return spec_value
+	if exc_if_not_found:
+		raise RsInstrException(f"String '{value}' can not be found in the enum type '{scpi_enum.enum_type}'")
 	# noinspection PyTypeChecker
-	return spec_value
+	return Utilities.trim_str_response(string)
 
 
-def str_to_list_enum_helper(string: str, enum_type: Enum, enum_members=None) -> List[Enum]:
-	"""Converts string to list of enum elements.
-	enum_members are optional to improve the performance for repeated conversions.
-	If you do not provide them, they are generated inside the function."""
-	if not enum_members:
-		# noinspection PyTypeChecker
-		enum_members = [x.name for x in enum_type]
+def str_to_simple_scalar_enum(string: str, enum_type, case_sensitive: bool = True, ignore_underscores: bool = False) -> Enum or None:
+	"""Converts string to one enum element.
+	Does not handle special value or non-mandatory parts.
+	The function is used in core only for standard enum conversions, not for SCPI enum conversions."""
+	value = Utilities.trim_str_response(string)
+	enum_members = [x.name for x in enum_type]
+	enum_members_mod = [x.name for x in enum_type]
+	if not case_sensitive:
+		enum_members_mod = [x.upper() for x in enum_members]
+		value = value.upper()
+	if ignore_underscores:
+		enum_members_mod = [x.replace('_', '') for x in enum_members_mod]
+		value = value.replace('_', '')
+	if value in enum_members_mod:
+		return enum_type[enum_members[enum_members_mod.index(value)]]
+	return None
+
+
+def str_to_list_enum_helper(string: str, scpi_enum: ScpiEnum, exc_if_not_found: bool = True) -> List[Enum]:
+	"""Converts string to list of enum elements. separated by comma"""
 	elements = string.split(',')
-	return [str_to_scalar_enum_helper(x, enum_type, enum_members) for x in elements]
+	return [str_to_scalar_enum_helper(x, scpi_enum, True, exc_if_not_found) for x in elements]
 
 
 def enum_scalar_to_str(data, enum_type) -> str:
 	"""Converts enum scalar value to string."""
 	assert isinstance(data, enum_type), f"Expected command parameter {enum_type}, actual data type: {type(data)}. Value: {data}"
 	return value_to_str(data)
 
 
+def enum_ext_scalar_to_str(data, enum_type) -> str:
+	"""Converts enum scalar value to string.
+	If the input value is string, the function returns the string with single quotes."""
+	if isinstance(data, str):
+		# Return string with quotes
+		return value_to_quoted_str(Utilities.trim_str_response(data))
+	assert isinstance(data, enum_type), f"Expected command parameter string or {enum_type}, actual data type: {type(data)}. Value: {data}"
+	return value_to_str(data)
+
+
 def enum_list_to_str(data: List, enum_type) -> str:
 	"""Converts enum list to csv-string."""
 	# For enums, check that each element is an enum
 	assert all(isinstance(x, enum_type) for x in data), f"Expected command parameter list of {enum_type}, detected one or more elements of non-enum type. Value: {data}"
 	return list_to_csv_str(data)
 
 
+def enum_ext_list_to_str(data: List, enum_type) -> str:
+	"""Converts enum list to csv-string. Allows the elements to be either enum or string."""
+	assert all((isinstance(x, enum_type or str) or isinstance(x, str)) for x in data), f"Expected command parameter list of strings or {enum_type}, detected one or more elements of non-enum/non-string type. Value: {data}"
+	return list_to_csv_quoted_str(data)
+
+
 def str_to_scalar_enum(string: str, enum_type) -> Enum:
-	"""Converts string to one enum element."""
-	return str_to_scalar_enum_helper(string, enum_type)
+	"""Converts string to one enum element.
+	Throws exception if the string can not be converted to an enum element or a special value."""
+	return str_to_scalar_enum_helper(string, ScpiEnum(enum_type), False, exc_if_not_found=True)
+
+
+def str_to_scalar_enum_ext(string: str, enum_type) -> Enum:
+	"""Converts string to one enum element.
+	Compared to str_to_scalar_enum, in case the string can not be converted, it is returned trimmed for quotes and ."""
+	return str_to_scalar_enum_helper(string, ScpiEnum(enum_type), False, exc_if_not_found=False)
 
 
 def str_to_list_enum(string: str, enum_type) -> List[Enum]:
 	"""Converts string to list of enum elements."""
-	return str_to_list_enum_helper(string, enum_type)
+	return str_to_list_enum_helper(string, ScpiEnum(enum_type))
+
+
+def str_to_list_enum_ext(string: str, enum_type) -> List[Enum]:
+	"""Converts string to list of enum or string elements."""
+	return str_to_list_enum_helper(string, ScpiEnum(enum_type), exc_if_not_found=False)
+
+
+def convert_ts_to_datetime(timestamp: datetime or float) -> datetime:
+	"""Converts timestamp as float to datetime. For datetime tuple it just passes the value."""
+	if isinstance(timestamp, float) or isinstance(timestamp, int):
+		return datetime.fromtimestamp(timestamp)
+	return timestamp
+
+
+def get_timestamp_string(timestamp: datetime or float) -> str:
+	"""Returns the timestamp as string. The timestamp can be a datetime tuple or float seconds coming from the time.time()."""
+	timestamp = convert_ts_to_datetime(timestamp)
+	cur_time = timestamp.strftime('%H:%M:%S.%f')[:-3]
+	return cur_time
+
+
+def get_timedelta_fixed_string(time_start: datetime or float, time_end: datetime or float) -> str:
+	"""Returns the time span as string - fixed in the format of '%H:%M:%S.%f'."""
+	time_a = convert_ts_to_datetime(time_start)
+	time_b = convert_ts_to_datetime(time_end)
+	frac = (time_b - time_a).total_seconds()
+	wh = math.floor(frac)
+	d = int(wh / 86400)
+	h = int((wh - (d * 86400)) / 3600)
+	m = int((wh - (d * 86400 + h * 3600)) / 60)
+	s = int((wh - (d * 86400 + h * 3600 + m * 60)))
+	ms = int((frac - wh) * 1000)
+	res = f'{h:02d}:{m:02d}:{s:02d}.{ms:03d}'
+	if d > 0:
+		res = f'{d}d ' + res
+	return res
+
+
+def get_timedelta_string(time_a: datetime or float, time_b: datetime or float) -> str:
+	"""Returns the time span as string - dynamic based on the difference."""
+	time_a = convert_ts_to_datetime(time_a)
+	time_b = convert_ts_to_datetime(time_b)
+	if time_b < time_a:
+		return '0.000 ms'
+	diff = time_b - time_a
+	if diff.seconds < 10:
+		return f'{diff.total_seconds() * 1000:0.3f} ms'
+	elif diff.seconds < 1000:
+		a = diff.total_seconds()
+		return f'{a:0.3f} secs'
+	hours, remainder = divmod(diff.seconds, 3600)
+	minutes, seconds = divmod(remainder, 60)
+	return f'{hours:02d}:{minutes:02d}:{seconds:02d}'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ConverterFromScpiString.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ConverterFromScpiString.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+"""See the class docstring."""
+
 from enum import Enum
 
 from .Conversions import str_to_bool, str_to_int, str_to_int_or_bool, str_to_float, str_to_float_or_bool, str_to_scalar_enum_helper
 from .Conversions import str_to_str_list, str_to_bool_list, str_to_int_list, str_to_int_or_bool_list, str_to_float_list, str_to_float_or_bool_list, str_to_list_enum_helper
 from .Types import DataType
 from .Utilities import trim_str_response
+from .InstrumentErrors import RsInstrException
+from .ScpiEnums import ScpiEnum
 
 
 class ConverterFromScpiString:
 	"""Converter from SCPI response string to argument value
 	For list argument types, you must use the method get_one_element_value in a loop for each element.
 	Provides methods:
 	- get_one_element_value(str): returns one scalar value converted from the SCPI string.
 	- get_list_value(str): return complete list value converted from the SCPI string.
 	- get_value(str): calls either get_one_element_value or get_list_value() depending on the data type. \n
 	The reason for the different methods is, that sometimes the list data are interleaved with other arguments.
 	In order to parse them properly, the ArgStructStringParser module must be able to set the argument value element-by-element.
-	On the other side, the driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
+	The driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
 
 	def __init__(self, data_type: DataType, enum_type: Enum = None):
-		self.enum_type = enum_type
+		self.scpi_enum = None
 		self.data_type = data_type
 		self.element_type = self.data_type.element_type
 
 		if self.element_type == DataType.RawString:
 			self.converter = trim_str_response
 			self.list_converter = str_to_str_list
 
@@ -46,30 +50,29 @@
 			self.converter = str_to_float
 			self.list_converter = str_to_float_list
 
 		elif self.element_type == DataType.FloatExt:
 			self.converter = str_to_float_or_bool
 			self.list_converter = str_to_float_or_bool_list
 
-		elif self.element_type == DataType.Enum:
-			assert self.enum_type, f"For data type enum, you have to define the enum_type variable."
+		elif self.element_type.is_scalar_enum:
+			assert enum_type, f"For data type enum, you have to define the enum_type variable."
 			# noinspection PyTypeChecker
-			self.enum_members = [x.name for x in self.enum_type]
+			self.scpi_enum = ScpiEnum(enum_type)
 		else:
-			raise Exception(f"Unsupported data type '{data_type}'")
+			raise RsInstrException(f"Unsupported data type '{data_type}'")
 
 	def get_one_element_value(self, scpi_string: str):
-		"""Returns single element !!! of the argument value converted from the SCPI string (single element)"""
+		"""Returns single element (not an array!!!) of the argument value converted from the SCPI string (single element)"""
 		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
-		if self.element_type is DataType.Enum:
-			return str_to_scalar_enum_helper(scpi_string, self.enum_type, self.enum_members)
+		if self.element_type.is_scalar_enum:
+			return str_to_scalar_enum_helper(scpi_string, self.scpi_enum, False, exc_if_not_found=self.element_type == DataType.Enum)
 		return self.converter(scpi_string)
 
 	def get_value(self, scpi_string: str):
 		"""Returns complete value of the argument converted from the SCPI string (list or scalar)"""
 		if not self.data_type.is_list:
 			return self.get_one_element_value(scpi_string)
-
 		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
 		if self.element_type is DataType.Enum:
-			return str_to_list_enum_helper(scpi_string, self.enum_type, self.enum_members)
+			return str_to_list_enum_helper(scpi_string, self.scpi_enum, exc_if_not_found=self.element_type == DataType.Enum)
 		return self.list_converter(scpi_string)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/ConverterToScpiString.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/ConverterToScpiString.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""See the class docstring."""
+
 from enum import Enum
 
-from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str
+from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str, enum_ext_scalar_to_str, enum_ext_list_to_str
 from .Types import DataType
+from .InstrumentErrors import RsInstrException
 
 
-def value_to_scpi_string(data, data_type: DataType):
-	"""Method to be used in the driver implementation.
-	Convert data to SCPI string parameter: data -> str"""
+def value_to_scpi_string(data, data_type: DataType) -> str:
+	"""Convert data to SCPI string parameter: data -> str.
+	Does not work with enum data types."""
 	if data_type.is_list:
 		assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
 	else:
 		assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
 	# Strings are enclosed by single quotes
 	if data_type == DataType.StringList:
 		assert all(isinstance(x, str) for x in data), f"Expected command parameter list of strings, detected one or more elements of non-string type. Value: {data}"
@@ -46,35 +49,37 @@
 	elif data_type == DataType.IntegerExtList or data_type == DataType.FloatExtList:
 		assert all((isinstance(x, int) or isinstance(x, float) or isinstance(x, bool)) for x in data), f"Expected command parameter list of numbers or booleans, detected one or more elements of non-number type. Value: {data}"
 		return list_to_csv_str(data)
 	elif data_type == DataType.IntegerExt or data_type == DataType.FloatExt:
 		assert (isinstance(data, int) or isinstance(data, float) or isinstance(data, bool)), f"Expected command parameter number or boolean, actual data type: {type(data)}. Value: {data}"
 		return value_to_str(data)
 	else:
-		raise Exception(f"Unsupported data type: '{type(data_type)}'.")
+		raise RsInstrException(f"Unsupported data type: '{type(data_type)}'.")
 
 
 class ConverterToScpiString:
 	"""Converter from argument value to SCPI string.
 	Provides method get_value(arg_value) -> str
 	"""
 
 	def __init__(self, data_type: DataType, enum_type: Enum = None):
 		self.enum_type = enum_type
 		self.data_type = data_type
 		self.element_type = self.data_type.element_type
-		if self.element_type == DataType.Enum:
+		if self.element_type == DataType.Enum or self.element_type == DataType.EnumExt:
 			assert self.enum_type, f"For data_type {data_type.name}, you have to define the enum_type variable."
 
 	def get_value(self, data) -> str:
 		"""Returns SCPI string converted from the argument data."""
 		if self.data_type.is_list:
 			assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
 		else:
 			assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
-
 		if self.data_type == DataType.Enum:
 			return enum_scalar_to_str(data, self.enum_type)
-		elif self.data_type == DataType.EnumList:
+		if self.data_type == DataType.EnumExt:
+			return enum_ext_scalar_to_str(data, self.enum_type)
+		if self.data_type == DataType.EnumList:
 			return enum_list_to_str(data, self.enum_type)
-
+		if self.data_type == DataType.EnumExtList:
+			return enum_ext_list_to_str(data, self.enum_type)
 		return value_to_scpi_string(data, self.data_type)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Core.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,126 @@
-import re
+"""See the class docstring."""
+
 from typing import Callable
 
-from . import InstrumentOptions as Options, Conversions as Conv
+from . import InstrumentOptions as Options
 from .ArgSingle import ArgSingle
 from .ArgSingleList import ArgSingleList
 from .Conversions import BinFloatFormat, BinIntFormat
 from .Instrument import Instrument
-from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode
-from .Utilities import parse_token_to_key_and_value, trim_str_response
+from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode, OpcSyncQueryMechanism
+from .ScpiLogger import LoggingMode
+from .InstrumentErrors import RsInstrException
+from .Properties import Properties
 
 
 class Core(object):
 	"""Main driver component. Provides: \n
 		- Main core constructor
 		- 'io' interface for all the write / query operations
 		- Command parameters string composer for single arguments...
 		- Link handlers adding / changing / deleting
 
 		Version history:
 
+		1.70.0 (27.02.2024)
+			- Added settings profile 'XK41' for R&S Software Defined Radios.
+			- Added settings 'FirstCmds' where you can send the defined commands right after the init. Send more commands in a row with ';;' separator.
+			- Added settings 'EachCmdPrefix' - this prefix is added to each command sent to the instrument. Supported values are also 'lf', 'cr', 'tab'
+
+		1.60.0 (31.01.2024)
+			- Added Properties script for global properties.
+			- Added Properties.scpi_quotes, string option settings token: 'ScpiQuotes'. Example: ScpiQuotes=double. Default: Single
+			- Fixed VisaPluginSocketIo read() method for cases where the session is lost. The method now generates exception in that case.
+			- Added settings 'OpcSyncQueryMechanism' with values: Standard, AlsoCheckMav, ClsOnlyCheckMavErrQueue, OnlyCheckMavErrQueue
+
+		1.54.0 (27.06.2023)
+			- Added new options profile for ATS chambers.
+			- Added settings boolean token EachCmdAsQuery. Example: EachCmdAsQuery=True. Default: False
+
+		1.53.0 (18.10.2022)
+			- Improved mode where the instrument works with a session from another object.
+			- Silently ignoring invalid *IDN? string.
+			- Added new options profile 'Minimal' for non-SCPI-99 instruments.
+
+		1.52.0 (28.09.2022)
+			- Fixed DisableOpcQuery=True settings effect.
+			- Improved robustness of the TerminationCharacter option value entry.
+			- Added new options profile for CMQ500.
+
+		1.51.0 (08.09.2022)
+			- Changed the accepted IDN? response to more permissive.
+			- added methods go_to_remote() and go_to_local()
+			- added methods file_exists() and get_file_size()
+
+		1.50.0 (23.06.2022)
+			- Added relative timestamp to the logger.
+			- ScpiLogger can read GlobalData class variables making it possible to define common target and reference timestamp for all instances.
+			- Logger stream entries are by default immediately flushed, making sure that the log is complete.
+			- Added time statistic methods get_total_execution_time(), get_total_time(), reset_time_statistics().
+
+		1.24.0 (03.06.2022)
+			- Changed parsing of SYST:ERR? response to tolerate +0,"No Error" response.
+			- Added settings integer token OpenTimeout. Example: OpenTimeout=5000. Default: 0
+			- Added settings boolean token ExclusiveLock. Example: ExclusiveLock=True. Default: False
+
+		1.23.0 (24.05.2022)
+			- Added stripping of trailing commas when parsing the *IDN? response.
+			- If the Resource Manager does not find any default VISA implementation, it falls back to R&S VISA - relevant for LINUX or macOS
+			- Other typos and formatting corrections.
+
+		1.22.0 (20.04.2022)
+			- Added optional parameter timeout to reset()
+			- Added query list methods:  query_bool_list, query_bool_list_with_opc
+
+		1.21.0 (07.01.2022)
+			- Added logging to UDP port (49200) to integrate with new R&S Instrument Control plugin for Pycharm
+
+		1.20.0 (19.11.2021)
+			- Fixed logging strings when device name was a substring of the resource name
+
+		1.18.0 (build 64) 05.11.2021
+			- Added setting profile for non-standard instruments. Example of the options string: options='Profile=hm8123'
+
+		1.17.0 (build 63) 15.10.2021
+			- Added correct conversion of strings with SI suffixes (e.g.: MHz, KHz, THz, GHz, ms, us) to float and integer
+
+		1.16.0 (build 62) 31.08.2021
+			- Changed default encoding of string<=>bin from utf-8 to charmap.
+			- Added settable encoding for the session. Property: RsInstrument.encoding
+
+		1.15.0 (build 61) 17.08.2021
+			- Added support for EnumExt and EnumExtList
+			- Added support for custom scpi enums
+			- Improved exception handling in cases where the instrument session is closed.
+			- Fixed warning in Instrument.py
+			- Fixed Instrument.query_bin_block() for timeout errors
+			- Repeated capabilities are now allowed to be integer numbers as well
+
+		1.14.0 (build 53) 12.07.2021
+			- Scpi logger time entries now support not only datetime tuples, but also float timestamps
+			- changed handling of the syst:err? responses - now they are always Tuple (code, message)
+			- StatusException has new field errors_list: List[ Tuple[code, message] ]
+			- Added logger.log_status_check_ok property. This allows for skipping lines with 'Status check: OK'
+
+		1.12.0 (build 50) 26.06.2021
+			- Added SCPI Logger
+			- Simplified constructor's options string format - removed DriverSetup=() syntax:
+			Instead of "DriverSetup=(TerminationCharacter='\n')", you use "TerminationCharacter='\n'"
+			The original format is still supported.
+
+			- Fixed calling SYST:ERR? even if *STB? returned 0
+			- Replaced @ni backend with @ivi for resource manager - this is necessary for the future pyvisa version 1.12+
+
+		1.11.0 (build 49) 09.06.2021
+			- Added is_connection_active() + reconnect()
+
+		1.10.1 (build 47) 01.06.2021
+			- Fixed bug with error checking when events are defined
+
 		1.10.0 (build 46) 03.05.2021
 			- Added methods to Instrument: query_struct_with_opc(), query_str_suppressed_with_opc()
 
 		1.9.0 (build 45) 13.04.2021
 			- Added option to set callbacks before_write and before_query
 			- When a RepCap has a member with integer number 0 defined, the command string interpretation of such member is '0', not empty string
 
@@ -32,15 +130,15 @@
 		1.7.7 (build 42) 26.11.2020
 			- Extended ArgSingleList.compose_cmd_string() to 9 arguments
 
 		1.7.6 (build 41) 23.11.2020
 			- Extended data types for IntegerExt, FloatExt, IntegerExtArray, FloatExtArray
 
 		1.7.5 (build 40) 12.11.2020
-			- Extended Conversions method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
+			- Extended 'Conversions' method str_to_str_list() by parameter 'clear_one_empty_item' with default value False
 
 		1.7.4 (build 39) 11.09.2020
 			- Fixed parsing of the instrument errors when an error message contains two double quotes
 
 		1.7.3 (build 38) 21.10.2020
 			- Added 'UND' to the list of float numbers that are represented as NaN
 
@@ -60,15 +158,15 @@
 
 		1.4.0 (build 32) 17.09.2020
 			- Added recognition of RsVisa library location for linux when using options string 'SelectVisa=rs'
 			- Fixed bug in reading binary data 16 bit
 
 		1.3.0 (build 31) 04.09.2020
 			- added DRIVERSETUP_QUERYOPT to the driver's option string
-			- *OPT? is no longer performed at the init, but only at the first access to options string.
+			- *OPT? is no longer performed at the init, but only at the first access to the options string.
 				In addition, the *OPT? query is executed with 1000 ms timeout, and the errors are suppressed
 
 		1.2.0 (build 30), 03.08.2020
 			- Fixed NRP-Z session parameters: vxi_capable = False, io_segment_size = 1000000
 
 		1.1.0 (build 29), 20.06.2020
 			- Added RepeatedCapability and base class CommandsGroup
@@ -89,85 +187,94 @@
 			reset: bool = False,
 			driver_options: str = None,
 			user_options: str = None,
 			direct_session: object = None):
 		"""Initializes new driver session. For cleaner code, use the class methods: \n
 		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
 
-		self.core_version = '1.9.0'
-		self.simulating = False
-		self.supported_idn_patterns = []
-		self.supported_instr_models = []
-
-		self._args_single_list = ArgSingleList()
-		sett_dr = self._parse_init_settings_string(driver_options)
-		self._apply_settings_to_core(sett_dr)
-		sett_user = self._parse_init_settings_string(user_options)
-		self._apply_settings_to_core(sett_user)
+		self.core_version = '1.55.0'
+		self.resource_name = resource_name
 
 		# Typical settings for the Core
 		self._instrumentSettings = InstrumentSettings(
 			InstrViClearMode.execute_on_all,  # Instrument viClear mode
 			False,  # Full model name. True: SMW200A, False: SMW
 			0,  # Delay by each write
 			0,  # Delay by each read
-			100000,  # Max chunk read / write size in bytes
+			1000000,  # Max chunk read / write size in bytes
 			WaitForOpcMode.stb_poll,  # Waiting for OPC Mode: Status byte polling
 			30000,  # OPC timeout
 			10000,  # VISA timeout
 			60000,  # Self-test timeout
 			Options.ParseMode.Auto,  # *OPT? response parsing mode
 			BinFloatFormat.Single_4bytes,  # Format for parsing of binary float numbers
 			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
-			False  # OPC query after each setting
+			False,  # OPC query after each setting
+			LoggingMode.Off,
+			OpcSyncQueryMechanism.only_check_mav_err_queue
+			# Logging mode
 		)
 
-		self._instrumentSettings.apply_option_settings(sett_dr)
-		self._instrumentSettings.apply_option_settings(sett_user)
+		self._instrumentSettings.apply_option_settings(driver_options)
+		self._instrumentSettings.apply_option_settings(user_options)
 
-		# Resolve the direct_session to handle. Options for direct_session type:
-		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
-		# - string in case of a simulation session
-		handle = direct_session
-		if handle:
-			# Check if the entered 'direct_session' is either the driver object or the Visa session
-			if hasattr(direct_session, 'get_session_handle'):
-				assert hasattr(direct_session, '_core'), f"Direct session is a class type. It must be an instance of the top-level driver class."
-				handle = direct_session.get_session_handle()
-			# Check if the handle is not a simulation mode string
-			if isinstance(handle, str):
-				if "Simulating session, resource name " in handle:
-					self.simulating = True
-					handle = None
+		self.simulating = self._instrumentSettings.simulating
+		self.supported_idn_patterns = self._instrumentSettings.supported_idn_patterns
+		self.supported_instr_models = self._instrumentSettings.supported_instr_models
 
-		self.io = Instrument(resource_name, self.simulating, self._instrumentSettings, handle)
+		self._args_single_list = ArgSingleList()
+		handle = self._resolve_direct_session(direct_session)
+		self.io = Instrument(self.resource_name, self.simulating, self._instrumentSettings, handle)
 		self.io.query_instr_status = True
+		# Update the resource name if it changed, for example because of the direct session
+		self.resource_name = self.io.resource_name
+		self.allow_reconnect = self.io.allow_reconnect
 
-		self._apply_settings_to_instrument(sett_dr)
-		self._apply_settings_to_instrument(sett_user)
-
+		self._apply_settings_to_instrument(self._instrumentSettings)
+		self._apply_global_properties(self._instrumentSettings)
 		self.io.set_simulating_cmds()
 
 		if id_query:
 			self.io.fits_idn_pattern(self.supported_idn_patterns, self.supported_instr_models)
 
 		if reset:
 			self.io.reset()
 		else:
 			self.io.check_status()
 
 	@classmethod
 	def from_existing_session(cls, session: object, driver_options: str = None) -> 'Core':
 		"""Creates a new Core object with the entered 'session' reused."""
 		# noinspection PyTypeChecker
-		return cls(None, False, False, driver_options, None, session)
+		return cls(resource_name=None, id_query=False, reset=False, driver_options=driver_options, user_options=None, direct_session=session)
 
 	def __str__(self):
 		return f"Core session '{self.io.resource_name}'"
 
+	def _resolve_direct_session(self, direct_session):
+		# Resolve the direct_session to handle. Options for direct_session type:
+		# - VisaSession object, retrieved from the driver's RsInstrument.get_session_handle() method
+		# - string in case of a simulation session
+		handle = direct_session
+		if not direct_session:
+			return None
+		# Check if the entered 'direct_session' is either the driver object or the Visa session
+		if hasattr(direct_session, 'get_session_handle'):
+			if not hasattr(direct_session, '_core'):
+				raise RsInstrException('Direct session is a class type. It must be an instance of the top-level driver class.')
+			handle = direct_session.get_session_handle()
+		# If the handle is a simulating session, change the session to simulating and set disable the 'from existing session' feature
+		if isinstance(handle, str):
+			mand_string = 'Simulating session, resource name '
+			if mand_string in handle:
+				self.resource_name = handle[len(mand_string):].strip().strip("'").strip()
+				self.simulating = True
+				handle = None
+		return handle
+
 	def set_link_handler(self, link_name: str, handler: Callable) -> Callable:
 		"""Adds / Updates link handler for the entered link_name.
 		Handler API: handler(event_args: ArgLinkedEventArgs)
 		Returns the previous registered handler, or None if no handler was registered before."""
 		return self.io.set_link_handler(link_name, handler)
 
 	def del_link_handler(self, link_name: str) -> Callable:
@@ -176,82 +283,30 @@
 		return self.io.del_link_handler(link_name)
 
 	def del_all_link_handlers(self) -> int:
 		"""Deletes all the link handlers.
 		Returns number of deleted links."""
 		return self.io.del_all_link_handlers()
 
-	# noinspection PyMethodMayBeStatic
-	def _parse_init_settings_string(self, text: str) -> dict:
-		"""Parses init string to a dictionary of settings: name -> value."""
-		tokens = {}
-		if not text:
-			return tokens
-
-		# Text enclosed in single brackets '' must have the commas escaped
-		literal_pattern = r"'([^']+)'"
-		while True:
-			# literal loop
-			m = re.search(literal_pattern, text)
-			if not m:
-				break
-			lit_part = '"' + m.group(1).replace(',', '<COMMA_ESC>') + '"'
-			text = text.replace(m.group(0), lit_part)
-
-		# Remove all the class-options enclosed by round brackets e.g. "<groupName>=(<groupTokens>)"
-		group_pattern = r'(\w+)\s*=\s*\(([^\)]*)\)'
-		# Match class-settings, add them as separate keys with groupName_Key
-		while True:
-			# Group loop
-			m = re.search(group_pattern, text)
-			if not m:
-				break
-			text = text.replace(m.group(0), '')
-			group_name = m.group(1).upper()
-			group_tokens = m.group(2).strip().split(',')
-			for token in group_tokens:
-				key, value = parse_token_to_key_and_value(token)
-				if value:
-					tokens[f'{group_name}_{key.upper()}'] = value
-
-		# All groups are removed from the text, now we can use splitting on commas and remove white-space-only elements
-		for token in text.split(','):
-			key, value = parse_token_to_key_and_value(token.replace('<COMMA_ESC>', ','))
-			if value:
-				tokens[key.upper()] = value
-		return tokens
-
-	def _apply_settings_to_core(self, settings: dict) -> None:
-		"""Applies settings relevant for the Core from the dictionary."""
-		value = settings.get('SIMULATE')
-		if value:
-			self.simulating = Conv.str_to_bool(value)
-
-		value = settings.get('SUPPORTEDINSTRMODELS')
-		if value:
-			self.supported_instr_models = [*map(trim_str_response, value.split('/'))]
-
-		value = settings.get('SUPPORTEDIDNPATTERNS')
-		if value:
-			self.supported_idn_patterns = [*map(trim_str_response, value.split('/'))]
-
-	def _apply_settings_to_instrument(self, settings: dict) -> None:
-		"""Applies settings relevant for the Instrument from the dictionary."""
-		value = settings.get('QUERYINSTRUMENTSTATUS')
-		if value:
-			self.io.query_instr_status = Conv.str_to_bool(value)
-
-		value = settings.get('SIMULATIONIDNSTRING')
-		if value and self.simulating:
-			# Use the '*' instead of the ',' in the value to avoid comma as token delimiter
-			self.io.idn_string = value.replace('*', ',')
+	def _apply_settings_to_instrument(self, settings: InstrumentSettings) -> None:
+		"""Applies settings relevant for the Instrument from the InstrumentSettings structure."""
+		if settings.instrument_status_check is not None:
+			self.io.query_instr_status = settings.instrument_status_check
+		if self.simulating and settings.instrument_simulation_idn_string is not None:
+			self.io.idn_string = settings.instrument_simulation_idn_string
+
+	@staticmethod
+	def _apply_global_properties(settings: InstrumentSettings) -> None:
+		"""Applies settings valid for the entire module. All are available in the module 'Properties'."""
+		if settings.scpi_quotes is not None:
+			Properties.scpi_quotes = settings.scpi_quotes
 
 	def compose_cmd_arg_param(
 			self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None) -> str:
-		"""Composes command parameter string based on the single arguments definition."""
+		"""Composes command parameter string based on the single argument definition."""
 		return self._args_single_list.compose_cmd_string(arg1, arg2, arg3, arg4, arg5, arg6)
 
 	def get_last_sent_cmd(self) -> str:
 		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
 		return self.io.get_last_sent_cmd()
 
 	def get_session_handle(self):
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/InstrumentErrors.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/InstrumentErrors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,79 @@
+"""Definition of RsInstrument exceptions, assert functions, and other error-related functions."""
+
+from typing import List, Tuple
+
+
 class RsInstrException(Exception):
 	"""Exception base class for all the RsInstrument exceptions."""
 	def __init__(self, message: str):
 		super(RsInstrException, self).__init__(message)
+		self.message = message
 
 
 class TimeoutException(RsInstrException):
 	"""Exception for timeout errors."""
 	def __init__(self, message: str):
 		super(TimeoutException, self).__init__(message)
 
 
 class StatusException(RsInstrException):
-	"""Exception for instrument status errors."""
-	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
+	"""Exception for instrument status errors.
+	Tje field  errors_list contains the complete list of all the errors with messages and codes."""
+	def __init__(self, rsrc_name: str, message: str, errors_list: List[Tuple[int, str]], first_exc: Exception = None):
+		self.rsrc_name: str = rsrc_name
+		self.first_exc: Exception = first_exc
+		self.errors_list: List[Tuple[int, str]] = errors_list
 		super(StatusException, self).__init__(message)
 
 
 class UnexpectedResponseException(RsInstrException):
 	"""Exception for instrument unexpected responses."""
 	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
+		self.rsrc_name: str = rsrc_name
 		super(UnexpectedResponseException, self).__init__(message)
 
 
 class ResourceError(RsInstrException):
 	"""Exception for resource name - e.g. resource not found."""
 	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
+		self.rsrc_name: str = rsrc_name
 		super(ResourceError, self).__init__(message)
 
 
 class DriverValueError(RsInstrException):
 	"""Exception for different driver value settings e.g. RepCap values or Enum values."""
 	def __init__(self, rsrc_name: str, message: str):
-		self.rsrc_name = rsrc_name
+		self.rsrc_name: str = rsrc_name
 		super(DriverValueError, self).__init__(message)
 
 
-def assert_no_instrument_status_errors(rsrc_name: str, errors: list, context: str = '') -> None:
-	"""Checks the errors list and of it contains at least one element, it throws StatusException."""
-	if errors is None:
-		return
-	if len(errors) == 0:
+def get_instrument_status_errors(rsrc_name: str, errors: List[Tuple[int, str]], context: str = '') -> str or None:
+	"""Checks the errors list and of it contains at least one element, it returns the error message.
+	Otherwise, it returns None."""
+	if errors is None or len(errors) == 0:
 		return
 	if context:
 		message = f"'{rsrc_name}': {context} "
 	else:
 		message = f"'{rsrc_name}': "
+	errors_msg = '\n'.join([f'{x[0]},"{x[1]}"' for x in errors])
 	if len(errors) == 1:
-		message += f'Instrument error detected: {errors[0]}'
-		raise StatusException(rsrc_name, message)
+		message += f'Instrument error detected: {errors_msg}'
+		return message
 	if len(errors) > 1:
-		message += '{} Instrument errors detected:\n{}'.format(len(errors), '\n'.join(errors))
-		raise StatusException(rsrc_name, message)
+		message += f'{len(errors)} Instrument errors detected:\n{errors_msg}'
+		return message
+
+
+def assert_no_instrument_status_errors(rsrc_name: str, errors: List[Tuple[int, str]], context: str = '', first_exc=None) -> None:
+	"""Checks the errors list and of it contains at least one element, it throws StatusException."""
+	msg = get_instrument_status_errors(rsrc_name, errors, context)
+	if msg:
+		raise StatusException(rsrc_name, msg, errors, first_exc=first_exc)
 
 
 def throw_opc_tout_exception(opc_tout: int, used_tout: int, context: str = '') -> None:
 	"""Throws TimeoutException - use it for any timeout error."""
 	if not context:
 		message = ''
 	else:
@@ -83,21 +99,21 @@
 
 def assert_query_has_qmark(query: str, context: str = '') -> None:
 	"""Throws Exception if the query does not contain any question marks."""
 	if '?' in query:
 		return
 	message = ''
 	if context:
-		message = ' ' + context
+		message = context.strip() + ': '
 	message = message + "Query commands must contain question-marks. Sent query: '{0}'".format(query.strip('\n'))
-	raise Exception(message)
+	raise RsInstrException(message)
 
 
 def assert_cmd_has_no_qmark(command: str, context: str = '') -> None:
 	"""Throws Exception if the query contains a question marks."""
 	if '?' not in command:
 		return
 	message = ''
 	if context:
-		message = ' ' + context
+		message = context.strip() + ': '
 	message = message + "Set commands must not contain question-marks. Sent command: '{0}'".format(command.strip('\n'))
-	raise Exception(message)
+	raise RsInstrException(message)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/InstrumentOptions.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/InstrumentOptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""See the class docstring."""
+
 import re
 from enum import Enum
 
 from .Utilities import trim_str_response
 
 
 class ParseMode(Enum):
@@ -10,14 +12,15 @@
 	KeepOriginal = 1
 	KeepBeforeDash = 2
 	KeepAfterDash = 3
 	Auto = 4
 
 
 class Options(object):
+	"""Class for handling the instrument options - parsing from the *OPT? string and providing method get_all()"""
 	_optionsList = []
 
 	def __init__(self, options_str: str, mode=ParseMode.Auto):
 		"""Initializes the options with the *OPT? return string."""
 		self._initialize_from_string(options_str, mode)
 
 	def __str__(self):
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/InternalLinker.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/InternalLinker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Links a variable from a structure to a callback in the driver."""
+
 from time import time
 from typing import Dict, Callable
 
 from . import ArgSingle, ArgSingleSuppressed
 from .ArgLinkedEventArgs import ArgLinkedEventArgs
 from .Utilities import get_plural_string
+from .InstrumentErrors import RsInstrException
 
 
 class InternalLinker(object):
 	"""Class for:
 		- cutting out suppressed arguments from a device response.
 		- invoking a handler if the argument has InternalLinking defined.
 		- holds dictionary of handlers where the dict_key is the InternalLinking string.
@@ -44,22 +47,22 @@
 		Returns number of deleted links."""
 		count = len(self._handlers)
 		self._handlers = {}
 		return count
 
 	def cut_from_response_string(self, arg: ArgSingleSuppressed, response: str, context: str) -> str:
 		"""Takes the string 'response', removes the suppressed argument value from it and returns the rest.
-		The cut out part is sent via handler if the internal linking exists for that argument exists."""
+		The cut-out part is sent via handler if the internal linking exists for that argument exists."""
 		result = ''
 		if arg.argument_ix is None:
-			raise Exception(f'Argument has argument_ix attribute not assigned (equals None). Argument: {arg}')
+			raise RsInstrException(f'Argument has argument_ix attribute not assigned (equals None). Argument: {arg}')
 		if arg.argument_ix != 0:
-			raise Exception(f'Only arguments with index 0 can be suppressed. Argument: {arg}')
+			raise RsInstrException(f'Only arguments with index 0 can be suppressed. Argument: {arg}')
 		if arg.is_open_list:
-			raise Exception(f'Open List arguments can not be suppressed. Argument: {arg}')
+			raise RsInstrException(f'Open List arguments can not be suppressed. Argument: {arg}')
 		repetition = 0
 		i = 0
 		for c in response:
 			if c == ',':
 				repetition += 1
 			if repetition == arg.repetition:
 				break
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/IoTransferEventArgs.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/IoTransferEventArgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""See the docstring for the IoTransferEventArgs class."""
+
 import itertools
 from typing import AnyStr
 
 from .Utilities import size_to_kb_mb_string
 
 
 class IoTransferEventArgs(object):
@@ -48,25 +50,25 @@
 		return cls(True, opc_sync, None, context)
 
 	@classmethod
 	def write_str(cls, opc_sync: bool, total_size: int, context: str) -> 'IoTransferEventArgs':
 		"""Creates new IoTransferEventArgs of write string \n
 		:param opc_sync: defines if the command is OPC-synchronised
 		:param total_size: size of the data to write
-		:param context: SCPI command write. It is truncated to maximum of 100 characters.
-		:return: IoTransferEventArgs object of a write string operation."""
+		:param context: SCPI command write. It is truncated to maximum of 100 characters
+		:return: IoTransferEventArgs object of a write-string operation."""
 		obj = cls(False, opc_sync, total_size, context)
 		obj.binary = False
 		return obj
 
 	@classmethod
 	def write_bin(cls, context: str) -> 'IoTransferEventArgs':
 		"""Creates new IoTransferEventArgs of read binary data \n
 		:param context: SCPI command. It is truncated to maximum of 100 characters.
-		:return: IoTransferEventArgs object of a write binary data operation."""
+		:return: IoTransferEventArgs object of a write-binary-data operation."""
 		# noinspection PyTypeChecker
 		obj = cls(False, False, None, context.rstrip())
 		obj.binary = True
 		return obj
 
 	def __str__(self):
 		if self.binary:
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/RepeatedCapability.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/RepeatedCapability.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""See the docstring for the RepeatedCapability class."""
+
 from enum import Enum
 
 
 # Command integer value that signals Default value "DEFAULT"
 VALUE_DEFAULT = -1
 
 # Command integer value that signals "EMPTY"
@@ -26,39 +28,47 @@
 	def __str__(self) -> str:
 		out = f'RepCap {self.name}'
 		if self._enum_value is not None:
 			out += f" = {self._enum_value}"
 		return out
 
 	@classmethod
-	def clsm_assert_type(cls, enum_value: Enum, enum_type) -> None:
-		"""Static assertion function to check if the entered value is a member of the defined repcap enum"""
+	def clsm_assert_type(cls, enum_value: Enum or int, enum_type) -> None:
+		"""Static assertion function to check if the entered value is a member of the defined repcap enum.
+		In addition, the integer value is also supported."""
+		if isinstance(enum_value, int):
+			return
 		if not isinstance(enum_value, enum_type):
 			raise TypeError(f"RepCap value must be of type '{enum_type}'. Entered value type: {type(enum_value)}, value '{enum_value}'")
 
 	@classmethod
-	def clsm_get_direct_cmd_value_int(cls, enum_value: Enum, enum_type) -> int:
+	def clsm_get_direct_cmd_value_int(cls, enum_value: Enum or int, enum_type) -> int:
 		"""Static function to get an integer interpretation of a direct enum value
 		Does not work with Empty or Default"""
 		RepeatedCapability.clsm_assert_type(enum_value, enum_type)
+		if isinstance(enum_value, int):
+			return enum_value
 		return enum_value.value
 
 	@classmethod
-	def clsm_is_default_value(cls, enum_value: Enum, enum_type) -> bool:
+	def clsm_is_default_value(cls, enum_value: Enum or int, enum_type) -> bool:
 		"""Returns True, if the entered value is enum.Default"""
 		return cls.clsm_get_direct_cmd_value_int(enum_value, enum_type) == VALUE_DEFAULT
 
 	def is_default_value(self) -> bool:
 		"""Returns True, if the repcap value is enum.Default"""
 		return RepeatedCapability.clsm_is_default_value(self._enum_value, self.enum_type)
 
-	def set_enum_value(self, enum_value: Enum) -> None:
+	def set_enum_value(self, enum_value: Enum or int) -> None:
 		"""Sets new enum value. Can not be Default"""
 		if RepeatedCapability.clsm_is_default_value(enum_value, self.enum_type):
 			raise ValueError(f"Setting RepCap enum value '{enum_value}' is not allowed. Please select a concrete value")
+		if isinstance(enum_value, int):
+			# Find the enum value that corresponds to the entered integer value
+			enum_value = self.enum_type(enum_value)
 		self._enum_value = enum_value
 
 	def get_enum_value(self) -> Enum:
 		"""Returns the actual enum value"""
 		return self._enum_value
 
 	def set_to_start_value(self) -> None:
@@ -66,16 +76,17 @@
 		self.set_enum_value(self._start_value)
 
 	def matches_type(self, enum_type) -> bool:
 		"""Returns true, if the entered type matches the EnumType"""
 		return self.enum_type == enum_type
 
 	@classmethod
-	def clsm_get_cmd_string_value(cls, enum_value: Enum, enum_type) -> str:
-		"""Converts RepCap integer value to string
+	def clsm_get_cmd_string_value(cls, enum_value: Enum or int, enum_type) -> str:
+		"""Class method version of the get_cmd_string_value().
+		Converts RepCap integer value to string
 		ValueEmpty is converted to "" (Not valid, but tolerated)
 		ValueDefault throws an exception
 		0 is converted to "" (Not valid, but tolerated)
 		Positive numbers are converted to integer strings e.g. 1 => '1' """
 		number = cls.clsm_get_direct_cmd_value_int(enum_value, enum_type)
 		if number == VALUE_EMPTY:
 			return ''
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/StreamReader.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/StreamReader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+"""See the docstring for the StreamReader class."""
+
 from enum import Enum
 from os import path
 from typing import AnyStr
 
 from .Utilities import size_to_kb_mb_string
+from .InstrumentErrors import RsInstrException
 
 
 class Type(Enum):
+	"""Defines type of the stream - variable or file."""
 	Variable = 1
 	File = 2
 
 
 class StreamReader:
 	"""Lightweight stream reader implementation. Data source can be: \n
 	- variable
@@ -21,31 +25,32 @@
 		:param source: Source type for the stream. Variable / File
 		:param data: Depending on the 'binary' and 'source':
 		For source type Variable the data must be either bytes() or str
 		For source type File data must be string with existing file path."""
 		self._source = source
 		self._binary = binary
 		self._start_ptr = 0
+		self._read_len = 0
 
 		if self._source == Type.Variable:
 			if self._binary:
 				assert isinstance(data, bytes), f'Data must be of bytes type. Actual type: {type(data)}'
 			else:
 				assert isinstance(data, str), f'Data must be of string type. Actual type: {type(data)}'
 			self._data = data
 			self._full_len = len(self._data)
 		elif self._source == Type.File:
 			assert isinstance(data, str), f'Data must be of string type (file path). Actual type: {type(data)}'
 			if not path.isfile(data):
-				raise Exception(f'File does not exist. File path: {data}')
+				raise RsInstrException(f'File does not exist. File path: {data}')
 			self.file_path = data
 			self._data = open(self.file_path, 'rb' if self._binary else 'r')
 			self._full_len = path.getsize(self.file_path)
 		else:
-			raise Exception(f'StreamReader unknown type {source}')
+			raise RsInstrException(f'StreamReader unknown type {source}')
 
 	@classmethod
 	def as_bin_var(cls, data: bytes) -> 'StreamReader':
 		"""Creates new StreamReader from bytes.
 		:param data: [bytes] data for the stream."""
 		return cls(True, Type.Variable, data)
 
@@ -100,29 +105,34 @@
 		If the remaining length is smaller than the chunk_size, the method returns the remaining length only.
 		:param chunk_size: chunk to read. If not set, the method reads the entire data."""
 		assert self._data is not None, 'StreamReader buffer is invalid. You have probably closed it already.'
 		chunk_size = len(self) if chunk_size is None else chunk_size
 		chunk_size = min(chunk_size, len(self))
 		if chunk_size < 0:
 			raise ValueError(f'Chunk size can not be negative number: {chunk_size}')
-
+		self._read_len += chunk_size
 		if self._source == Type.Variable:
 			self._start_ptr += chunk_size
 			return self._data[self._start_ptr - chunk_size: self._start_ptr]
 		elif self._source == Type.File:
 			self._start_ptr += chunk_size
 			return self._data.read(chunk_size)
 
-	def read_as_binary(self, chunk_size: int = None) -> bytes:
+	@property
+	def read_len(self) -> int:
+		"""Returns number of bytes read from the stream since its creation."""
+		return self._read_len
+
+	def read_as_binary(self, encoding: str, chunk_size: int = None) -> bytes:
 		"""Same as read(), but always returns the data in binary format.
 		Practically works exactly as read() for binary streams.
-		For string streams, the method converts the returned data using utf-8 encoding to bytes()."""
+		For string streams, the method converts the returned data using the provided encoding to bytes()."""
 		if self._binary:
 			return self.read(chunk_size)
 		else:
-			return self.read(chunk_size).encode('utf-8')
+			return self.read(chunk_size).encode(encoding)
 
 	def close(self):
 		"""Closes the StreamReader. You can not use its instance afterwards."""
 		if self._source == Type.File and self._data:
 			self._data.close()
 		self._data = None
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/StreamWriter.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/StreamWriter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+"""See the docstring for the StreamWriter class."""
+
 from enum import Flag
 from typing import AnyStr
+from io import BytesIO, StringIO
 
 from .Utilities import size_to_kb_mb_string
+from .InstrumentErrors import RsInstrException
 
 
 class Type(Flag):
+	"""Defines type of the stream - variable or file."""
 	Variable = 1
-	File = 2
-	FileAppend = 6
+	Forget = 2
+	File = 4
+	FileAppend = 12
 
 
 class StreamWriter:
 	"""Lightweight stream writer implementation. Data target can be: \n
 	- bytes
 	- string
 	- file"""
@@ -19,41 +25,48 @@
 	def __init__(self, binary: bool, target: Type, meta_data=None):
 		"""Initializes StreamWriter instance.\n
 		:param binary: True: Binary data, False: ASCII data
 		:param target: Target for the stream. Variable / File (FileAppend)
 		:param meta_data: Only valid for File and FileAppend - define file path as string:
 		For Type.File, data must be string with file path. If the file exists, it will be overwritten.
 		For Type.FileAppend, data must be string with file path. If the file exists, it will be appended."""
-		self._binary = binary
-		self._written_len = 0
+		self._binary: bool = binary
+		self._written_len: int = 0
 		self._target = target
 
 		if Type.Variable in self._target:
 			assert meta_data is None, f'You can not define input meta_data for a Variable StreamWriter.'
-			self._data: AnyStr = bytes() if binary else ''
+			self._data = BytesIO() if binary else StringIO()
+		elif Type.Forget in self._target:
+			self._data: AnyStr = ''
 		elif Type.File in self._target:
 			assert isinstance(meta_data, str), f'Additional data must be of string type (file path). Actual type: {type(meta_data)}'
 			self._file_path = meta_data
 			mode = 'w' if self._target == Type.File else 'a'
 			mode += 'b' if self._binary else ''
 			self._data = open(self._file_path, mode)
 		else:
-			raise Exception(f'StreamWriter unknown target {target}')
+			raise RsInstrException(f'StreamWriter unknown target {target}')
 
 	@classmethod
 	def as_bin_var(cls) -> 'StreamWriter':
 		"""Creates new StreamWriter with bytes variable."""
 		return cls(True, Type.Variable)
 
 	@classmethod
 	def as_string_var(cls) -> 'StreamWriter':
 		"""Creates new StreamWriter with string variable."""
 		return cls(False, Type.Variable)
 
 	@classmethod
+	def as_forget(cls) -> 'StreamWriter':
+		"""Creates new StreamWriter which writes to nowhere - forgets the data."""
+		return cls(False, Type.Forget)
+
+	@classmethod
 	def as_bin_file(cls, file_path: str, append: bool = False) -> 'StreamWriter':
 		"""Creates new StreamWriter to binary file.
 		:param file_path: [str] Path to the file.
 		:param append: Optional [bool] If True, the content is appended to the existing content."""
 		return cls(True, Type.FileAppend if append else Type.File, file_path)
 
 	@classmethod
@@ -67,14 +80,16 @@
 		if Type.Variable in self._target:
 			mode = 'binary' if self._binary else 'string'
 			return f'StreamWriter {mode} variable, current size {size_to_kb_mb_string(len(self), True)}'
 		if Type.File in self._target:
 			mode = 'binary' if self._binary else 'text'
 			append = ' appended' if Type.FileAppend in self._target else ''
 			return f'StreamWriter {mode} file{append}, current{append} size {size_to_kb_mb_string(len(self), True)}, file: {self._file_path}'
+		if Type.Forget in self._target:
+			return 'StreamWriter to nowhere.'
 
 	def __len__(self):
 		"""Returns remaining length."""
 		return self._written_len
 
 	def __enter__(self):
 		return self
@@ -88,49 +103,62 @@
 		File streams are always binary."""
 		return self._binary
 
 	def write(self, data: AnyStr) -> None:
 		"""Writes chunk to the stream.
 			- For Type.Bytes data must be bytes.
 			- For Type.String, data must be string.
-			- For Type.File and Type.FileAppend, data must be bytes"""
+			- For Type.File and Type.FileAppend, data must be bytes."""
+		if Type.Forget in self._target:
+			self._written_len += len(data)
+			return
+
 		assert self._data is not None, 'StreamWriter buffer is invalid. You have probably closed it already.'
 		if self._binary:
 			assert isinstance(data, bytes), f'Bytes data is required. Actual type: {type(data)}. {self}'
 		else:
 			assert isinstance(data, str), f'String data is required. Actual type: {type(data)}. {self}'
-
 		if Type.Variable in self._target:
-			self._data += data
+			self._data.write(data)
 		elif Type.File in self._target:
 			self._data.write(data)
 		self._written_len += len(data)
 
-	def switch_to_string_data(self) -> None:
+	def switch_to_string_data(self, encoding: str) -> None:
 		"""Switches from binary to string data.
-		For variables, the current content is converted.
+		For variables, the current content is converted to string using the provided encoding.
 		For files, they are closed and reopened as for appended text writing."""
 		if self._binary is False:
 			return
 		self._binary = False
 		if Type.Variable in self._target:
-			if len(self) == 0:
-				self._data = ''
-			else:
-				# noinspection PyUnresolvedReferences
-				self._data = self._data.decode('utf-8')
+			self._data = StringIO(self.content.decode(encoding))
 		elif Type.File in self._target:
 			self._data.close()
 			self._data = open(self._file_path, 'a')
 
+	# noinspection PyTypeChecker
 	@property
 	def content(self) -> AnyStr:
-		"""Returns content of the writer. Does only work with variable types."""
-		assert Type.Variable in self._target, f'Can not return content for the current {self}'
+		"""Returns content of the writer. Only works with variable types."""
+		if self._target == Type.Forget:
+			return ''
+		if self._target != Type.Variable:
+			raise RsInstrException(f'Can not return content for the current {self}')
 		# noinspection PyTypeChecker
-		return self._data
+		if not self._data:
+			return None
+		self._data.seek(0)
+		ret_val = self._data.read()
+		self._data.close()
+		return ret_val
+
+	@property
+	def written_len(self) -> int:
+		"""Returns number of bytes written to the stream since its creation."""
+		return self._written_len
 
 	def close(self) -> None:
 		"""Closes the StreamWriter. You can not use its instance afterwards."""
 		if Type.File in self._target and self._data:
 			self._data.close()
 		self._data = None
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/StructBase.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/StructBase.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+"""See the docstring for the StructBase class."""
+
 from .Types import DataType
 
 
 class StructBase:
 	"""Base class for all the driver's argument structures."""
 	def __init__(self, owner):
 		self.__meta_args_link = dict()
 		ix = 0
 		for arg in self.__get_meta_args_list(owner):
 			arg.argument_ix = ix
 			ix += 1
 
-			if arg.data_type == DataType.Enum or arg.data_type == DataType.EnumList:
+			if arg.data_type in [DataType.Enum, DataType.EnumExt, DataType.EnumList, DataType.EnumExtList]:
 				assert arg.enum_type, f"Struct Argument '{arg.name}' is of enum type, you must define the parameter 'enum_type'"
 			else:
 				assert not arg.enum_type, f"Struct Argument '{arg.name}' data type is '{arg.data_type.name}'. You must set the parameter 'enum_type' to None"
 
 			if arg.is_optional:
 				# set all optional values to None
 				setattr(self, arg.name, None)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Types.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,70 @@
+"""Data type class for the variables containing all the methods related to data types."""
+
 from enum import Enum, auto
 from typing import Any
 
 
+# noinspection PyArgumentList
 class DataType(Enum):
-	"""Data type of a variable in the driver."""
+	"""Data type of variable in the driver."""
 	String = auto()
 	RawString = auto()
 	Integer = auto()
 	IntegerExt = auto()
 	Boolean = auto()
 	Float = auto()
 	FloatExt = auto()
 	Enum = auto()
+	EnumExt = auto()
 	StringList = auto()
 	RawStringList = auto()
 	IntegerList = auto()
 	IntegerExtList = auto()
 	BooleanList = auto()
 	FloatList = auto()
 	FloatExtList = auto()
 	EnumList = auto()
+	EnumExtList = auto()
 
 	@property
 	def is_list(self) -> bool:
 		"""Returns True, if the data type is a list."""
 		return self in frozenset(
 			{
 				DataType.StringList,
 				DataType.RawStringList,
 				DataType.IntegerList,
 				DataType.IntegerExtList,
 				DataType.BooleanList,
 				DataType.FloatList,
 				DataType.FloatExtList,
-				DataType.EnumList
+				DataType.EnumList,
+				DataType.EnumExtList
 			})
 
 	@property
 	def is_scalar(self) -> bool:
 		"""Returns True, if the data type is a scalar."""
 		return not self.is_list
 
 	@property
+	def is_scalar_enum(self) -> bool:
+		"""Returns True, if the data type is a scalar enum or enum_ext."""
+		return self == DataType.Enum or self == DataType.EnumExt
+
+	@property
+	def is_list_enum(self) -> bool:
+		"""Returns True, if the data type is a list enum or list enum_ext."""
+		return self == DataType.EnumList or self == DataType.EnumExtList
+
+	@property
 	def is_enum(self) -> bool:
-		"""Returns True, if the data type is enum or enum array."""
-		return self == DataType.Enum or self == DataType.EnumList
+		"""Returns True, if the data type is enum or enum array - including the extended."""
+		return self in [DataType.Enum, DataType.EnumExt, DataType.EnumList, DataType.EnumExtList]
 
 	@property
 	def is_raw_string(self) -> bool:
 		"""Returns True for raw string and raw string list."""
 		return self == DataType.RawString or self == DataType.RawStringList
 
 	@property
@@ -81,14 +97,16 @@
 			return DataType.IntegerExt
 		elif self == DataType.FloatList:
 			return DataType.Float
 		elif self == DataType.FloatExtList:
 			return DataType.FloatExt
 		elif self == DataType.EnumList:
 			return DataType.Enum
+		elif self == DataType.EnumExtList:
+			return DataType.EnumExt
 
 	def get_default_value(self, enm: Enum = None) -> Any:
 		"""Returns default value for the current type.
 		If the data type is Enum or EnumString, you have to provide the enum class."""
 		if self.is_list:
 			return []
 		if self == DataType.RawString:
@@ -103,7 +121,9 @@
 			return 0
 		elif self == DataType.Float:
 			return 0.0
 		elif self == DataType.FloatExt:
 			return 0.0
 		elif self == DataType.Enum:
 			return enm(0)
+		elif self == DataType.EnumExt:
+			return enm(0)
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/Utilities.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/Utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Utilities for string manipulation and string formatting for the user."""
+
 from enum import Flag
 from typing import Tuple
 
 
 class TrimStringMode(Flag):
 	"""Trimming mode for strings."""
 	white_chars_only = 1
@@ -133,7 +135,41 @@
 
 
 def calculate_chunks_count(data_size: int, chunk_size: int) -> int:
 	"""Returns number of chunks needed to transfer the data_size split to maximum of chunk_size blocks. \n
 	:param data_size: total data size
 	:param chunk_size: maximum size of one block"""
 	return (data_size // chunk_size) + (1 if (data_size % chunk_size) > 0 else 0)
+
+
+def escape_nonprintable_chars(string: str, encoding: str = 'charmap') -> str:
+	"""
+	Replace nonprintable characters in string s by its hex representation.
+	"""
+	if string.isprintable():
+		return string
+	new_string = ''
+	for char in string:
+		if char.isprintable():
+			new_string += char
+		elif char == '\n':
+			new_string += r'\n'
+		elif char == '\r':
+			new_string += r'\r'
+		elif char == '\t':
+			new_string += r'\t'
+		else:
+			byte = bytes(char, encoding)
+			char = byte.hex()
+			new_string += r'\x' + char
+	return new_string
+
+
+def shorten_string_middle(string: str, max_len: int) -> str:
+	"""If the length of the string is bigger than the max_len,
+	the middle of the string is abbreviated with ' .... ' """
+	count = len(string)
+	if count <= max_len:
+		return string
+	half = int((max_len - 6) / 2)
+	md = (max_len - 6) % 2
+	return string[:half + md] + ' .... ' + string[(count - half):]
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/VisaPluginSocketIo.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/VisaPluginSocketIo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+"""See the docstring for the SocketIo class."""
+
 import socket
 import re
 from contextlib import contextmanager
+from typing import Any
+
+from .InstrumentErrors import RsInstrException
 
 # noinspection PyPackageRequirements
 import pyvisa
 
 
 class SocketIo:
-
+	"""Socket IO plugin providing implementations for all the necessary VISA functions. This class does not need the underlying VISA installation."""
 	def __init__(self, resource_name: str):
 		self.session = socket.socket()
 		self.resource_name = resource_name
 		m = re.search(r'TCPIP::([^:]+)::([^:]+)::SOCKET', self.resource_name)
 		if not m:
-			raise Exception(f"SocketIO instrument unsupported resource name. '{self.resource_name}' Supported resource name example: 'TCPIP::192.168.1.100::5025::SOCKET'")
+			raise RsInstrException(f"SocketIO instrument unsupported resource name. '{self.resource_name}' Supported resource name example: 'TCPIP::192.168.1.100::5025::SOCKET'")
 		self.host = m.group(1).strip()
 		self.port = int(m.group(2).strip())
 		self._read_termination = None
 		self._chunk_size = 1024
 		self._timeout = 5000
 		self.visalib = VisaLib(self)
 
@@ -90,14 +95,22 @@
 
 	# noinspection PyUnusedLocal
 	def read_bytes(self, count: int, **kwargs) -> bytes:
 		"""Reads count bytes"""
 		data, status = self.visalib.read(self.session, count)
 		return data
 
+	def go_to_local(self) -> None:
+		"""Puts the instrument into local state."""
+		self.write("&GTL")
+
+	def go_to_remote(self) -> None:
+		"""Puts the instrument into remote state."""
+		self.write("&GTR")
+
 	# noinspection PyUnusedLocal
 	@contextmanager
 	def ignore_warning(self, filter_value: int) -> None:
 		"""Context property with no effect for the socket connection"""
 		try:
 			yield None
 		finally:
@@ -106,15 +119,15 @@
 
 	def close(self) -> None:
 		"""Closes the socket connection"""
 		self.session.close()
 
 
 class VisaLib:
-
+	"""Implementation of the pyvisa's VisaLib providing the method read()"""
 	def __init__(self, socket_io: SocketIo):
 		self._socket_io = socket_io
 
 	def __str__(self):
 		return "SocketIO"
 
 	# noinspection PyUnresolvedReferences
@@ -127,14 +140,16 @@
 
 		try:
 			while True:
 				to_read_len = chunk_size - read_len
 				if to_read_len <= 0:
 					break
 				data = session.recv(to_read_len)
+				if not data:
+					raise pyvisa.VisaIOError(pyvisa.constants.VI_ERROR_CONN_LOST)
 				chunk += data
 				read_len += len(data)
 
 				if self._socket_io.read_termination is not None:
 					# Read termination character is ON, look for it and stop the reading if found
 					term_char = self._socket_io.read_termination.encode()
 					if term_char in data:
@@ -159,17 +174,18 @@
 				more_data_available = True
 
 		return_code = pyvisa.constants.StatusCode.success_max_count_read if more_data_available else pyvisa.constants.StatusCode.success
 		return chunk, return_code
 
 
 class ResourceManager:
-
+	"""Implementation of the VISA's Resource Manager."""
 	def __init__(self):
 		self.VisaManufacturerName = "SocketIO"
 		self.connection = None
 
-	def open_resource(self, resource_name: str) -> SocketIo:
-		"""Creates new Socket connection"""
+	# noinspection PyUnusedLocal
+	def open_resource(self, resource_name: str, access_mode: Any = None, open_timeout: Any = None) -> SocketIo:
+		"""Creates new Socket connection. access_mode and open_timeout are here for compatibility reasons with the pyvisa rm.open_resource()"""
 		self.connection = SocketIo(resource_name)
 		self.connection.connect()
 		return self.connection
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/VisaSession.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/VisaSession.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+"""Visa Session is an extension of the pure VISA providing higher level of methods regardless of the session kind."""
+
 import time
 from enum import Enum, Flag
-from typing import Tuple, Callable, AnyStr
+from typing import List, Tuple, Callable, AnyStr
 import os.path
 import re
 import threading
 
 # noinspection PyPackageRequirements
 import pyvisa
+from pyvisa.errors import StatusCode
 
 from .VisaPluginSocketIo import ResourceManager, SocketIo
 from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
-from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
+from .InstrumentSettings import WaitForOpcMode, OpcSyncQueryMechanism, InstrViClearMode as ViClearMode
 from .StreamReader import StreamReader
 from .StreamWriter import StreamWriter
 from .Utilities import size_to_kb_mb_string, calculate_chunks_count
 import platform
 import struct
 
 
@@ -37,14 +40,16 @@
 	bin_known_len = 3
 	bin_unknown_len = 4
 
 
 class StatusByte(Flag):
 	"""Status Byte flags."""
 	NONE = 0x00
+	custom_bit_0 = 0x01
+	custom_bit_1 = 0x02
 	error_queue_not_empty = 0x04
 	questionable_status_reg = 0x08
 	message_available = 0x10
 	event_status_byte = 0x20
 	request_service = 0x40
 	operation_status_reg = 0x80
 
@@ -64,14 +69,22 @@
 		# noinspection PyTypeChecker
 		self._data_chunk_size: int = None
 		self._std_bin_block_header_max_len: int = 999999999
 		self._lock = None
 		self.disable_opc_query: bool = settings.disable_opc_query
 		self.last_status = None
 		self.visa_library_name = None
+		self.resource_name = resource_name  # might be changed later if direct_session is used
+		self.encoding = settings.encoding  # default encoder between bytes and string
+		self.cmd_idn = settings.cmd_idn
+		self.skip_status_system_setting = settings.skip_status_system_setting
+		self.skip_clear_status = settings.skip_clear_status
+		self.stb_in_error_check = settings.stb_in_error_check
+		self.opc_sync_query_mechanism = settings.opc_query_sync_mechanism
+		self.each_cmd_prefix = settings.each_cmd_prefix
 
 		# Implemented for interface compatibility with VisaSessionSim
 		self.cached_to_stream = False
 
 		# Event handlers
 		# noinspection PyTypeChecker
 		self.on_read_chunk_handler: Callable = None
@@ -80,36 +93,36 @@
 		self.on_write_chunk_handler: Callable = None
 		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
 		self.io_events_include_data: bool = False
 		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
 
 		if self.reusing_session:
 			# Reuse the session
-			assert isinstance(direct_session, pyvisa.Resource) or isinstance(direct_session, SocketIo), f"Direct_session must be a VISA resource object. Actual type: '{type(direct_session)}', value: '{direct_session}'"
-			self._session = direct_session
-			self._resource_name = self._session.resource_name
+			self._session = VisaSession.get_and_check_direct_session(direct_session)
+			self.resource_name = self._session.resource_name
 		else:
 			# Create new session
 			# Check resource_name for the trailing (SelectVisa=..)
 			pure_resource_name, visa_select = self._get_pure_resource_name(resource_name)
 			if settings.visa_select is not None:
 				visa_select = settings.visa_select
 			self._rm = VisaSession.get_resource_manager(visa_select)
 			self.manufacturer = self._get_visa_manufacturer()
 
 			# Resource manager opening
 			try:
-				self._session = self._rm.open_resource(pure_resource_name)
+				acc_mode = pyvisa.constants.AccessModes.no_lock if settings.exclusive_lock is False else pyvisa.constants.AccessModes.exclusive_lock
+				self._session = self._rm.open_resource(resource_name=pure_resource_name, open_timeout=settings.open_timeout, access_mode=acc_mode)
 			except pyvisa.VisaIOError as e:
 				if e.error_code != pyvisa.constants.StatusCode.error_resource_not_found:
 					raise e
 				message = e.description
 				message += f"\nLibrary: {self._rm.visalib}\nManufacturer: {self.manufacturer}\nResource Name: '{resource_name}'"
 				raise InstrumentErrors.ResourceError(resource_name, message)
-			self._resource_name = resource_name
+			self.resource_name = resource_name
 
 		# Decide, whether to create a new thread lock or the existing one from the session
 		if hasattr(self._session, 'session_thread_rlock'):
 			rlock = self._session.session_thread_rlock
 			if isinstance(rlock, type(threading.RLock())):
 				self.assign_lock(rlock)
 		if self.get_lock() is None:
@@ -136,28 +149,22 @@
 			self._interface_type = SessionKind.vxi11
 			if self._session.resource_class == 'SOCKET':
 				self._interface_type = SessionKind.socket
 
 		# Specifics for different interfaces
 		self._assure_write_with_tc = settings.assure_write_with_tc
 		self._term_char = settings.term_char
-		self._term_char_bin = self._term_char.encode('utf-8')
+		self._term_char_bin = self._term_char.encode(self.encoding)
 		self._session.write_termination = ''
-		self.vxi_capable = True
+		self.vxi_capable = settings.vxi_capable
 
 		if self._interface_type == SessionKind.serial:
-			self._session.read_termination = self._term_char
 			self.vxi_capable = False
-			self._assure_write_with_tc = True
 		elif self._interface_type == SessionKind.socket:
-			self._session.read_termination = self._term_char
 			self.vxi_capable = False
-			self._assure_write_with_tc = True
-		else:
-			self._session.read_termination = ''
 
 		# NRP-Z specific settings
 		if self.is_rsnrp_session():
 			self.disable_opc_query = True
 			# NRP-Z does not support chunk reading, therefore the segment must be in one piece
 			settings.io_segment_size = 1000000
 			self.vxi_capable = False
@@ -166,78 +173,125 @@
 		self.read_delay = settings.read_delay
 		self._viclear_exe_mode = settings.viclear_exe_mode
 		self._opc_wait_mode = settings.opc_wait_mode
 
 		# Parameters that need to be coerced based on Vxi-capability
 		if self.vxi_capable:
 			self._add_term_char_to_write_bin_block = settings.add_term_char_to_write_bin_block
+			self._session.read_termination = ''
 		else:
 			self._add_term_char_to_write_bin_block = True
+			self._session.read_termination = self._term_char
+			self._assure_write_with_tc = True
 
 		# Changeable settings
 		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
 		self.visa_timeout = settings.visa_timeout
 		self._session.chunk_size = settings.io_segment_size
 		self._data_chunk_size = settings.io_segment_size
 
-		# Must call the VISA viClear() before the any communication with the instrument
+		# Must call the VISA viClear() before any communication with the instrument
 		self.clear()
 
 		# Further steps are for NRP-Z session not valid
 		if self.is_rsnrp_session():
 			return
 
+		# First commands, can be more than one, separated by ';;'
+		if settings.first_cmds:
+			cmds = settings.first_cmds.split(';;')
+			for cmd in cmds:
+				if cmd.startswith('<w>'):
+					self.write(cmd[3:])
+				elif cmd.startswith('<q>'):
+					_ = self._query_str_no_events(cmd[3:])
+				elif '?' in cmd:
+					_ = self._query_str_no_events(cmd)
+				else:
+					self.write(cmd)
+
 		# Clear instrument status
-		self.write('*CLS')
-		if self.vxi_capable:
-			stb = self._read_stb()
-			if stb & StatusByte.message_available:
-				self._flush_junk_data()
+		if self.skip_clear_status is False:
+			self.write('*CLS')
+			if self.vxi_capable:
+				stb = self._read_stb()
+				if stb & StatusByte.message_available:
+					self._flush_junk_data()
 
 		# Apply settings for ESE and SRE, plus coerce the _opcWaitMode if necessary
 		self._opc_wait_mode = self._set_regs_ese_sre(self._opc_wait_mode)
 
 	@staticmethod
+	def get_and_check_direct_session(direct_session):
+		"""Returns direct session if it's a proper type.
+		If the direct_session is None, the function returns None.
+		If the direct_session is of an unsupported type, the function raises RsInstrException."""
+		if direct_session is None:
+			return None
+		# Reuse the session
+		if not isinstance(direct_session, pyvisa.Resource) and not isinstance(direct_session, SocketIo):
+			raise InstrumentErrors.RsInstrException(f"Direct_session must be a VISA resource object. Actual type: '{type(direct_session)}', value: '{direct_session}'")
+		return direct_session
+
+	@staticmethod
 	def _get_pure_resource_name(resource_name: str):
 		"""Returns pure resource name stripped of the (SelectVisa) part and the visa_select string"""
 		m = re.search(r'(.+)\(SelectVisa=([^),]+)\)', resource_name)
 		if not m:
 			return resource_name, None
 		resource_name = m.group(1).strip()
 		visa_select = m.group(2).strip()
 		return resource_name, visa_select
 
 	@classmethod
 	def get_resource_manager(cls, visa_select: str) -> pyvisa.ResourceManager:
 		"""Returns resource manager for the desired VISA implementation"""
 		operating_system = platform.system().lower()
+		vsl = None if visa_select is None else visa_select.lower()
 		bittness = struct.calcsize('P') * 8
-		if visa_select is None or visa_select in ['@default', '@standard', 'default', 'standard', 'defaultvisa', 'standardvisa', '@defaultvisa', '@standardvisa']:
-			return pyvisa.ResourceManager()
-		if visa_select.lower() in ['@ni', 'ni', 'visa-ni', 'nivisa', 'ni-visa', 'nationalinstruments', 'nationalinstrumentsvisa']:
-			return pyvisa.ResourceManager('@ni')
-		if visa_select.lower() in ['@py', 'pyvisa', 'visa-py', 'pyvisa-py']:
-			return pyvisa.ResourceManager('@py')
-		if 'rohde&schwarz' in visa_select.lower() or 'rohdeschwarz' in visa_select.lower() or visa_select.lower() == 'rsvisa' or visa_select.lower() == 'rs' or visa_select.lower() == 'r&s':
+		# Try if you find the default VISA dll
+		try:
+			if visa_select is None or visa_select in ['@default', '@standard', 'default', 'standard', 'defaultvisa', 'standardvisa', '@defaultvisa', '@standardvisa']:
+				return pyvisa.ResourceManager()
+
+			if vsl in ['@ni', 'ni', 'ivi', '@ivi', 'visa-ni', 'nivisa', 'ni-visa', 'nationalinstruments', 'nationalinstrumentsvisa']:
+				return pyvisa.ResourceManager()
+
+			if vsl in ['@py', 'pyvisa', 'visa-py', 'pyvisa-py']:
+				return pyvisa.ResourceManager('@py')
+		except ValueError:
+			# None of the required implementations found, fall back to the R&S VISA
+			visa_select = 'rsvisa'
+			vsl = visa_select.lower()
+
+		# from here, RsVisa implementation is considered
+		if 'rohde&schwarz' in vsl or 'rohdeschwarz' in vsl or vsl == 'rsvisa' or vsl == 'rs' or vsl == 'r&s':
 			if operating_system == 'windows':
 				if bittness == 32:
 					visa_select = r'c:\Windows\SysWOW64\RsVisa32.dll'
 				else:
 					visa_select = r'c:\Windows\system32\RsVisa32.dll'
 				return pyvisa.ResourceManager(visa_select)
 			elif operating_system == 'linux':
 				# The default install location may be different
 				# for debian/red hat/opensuse derived distributions
 				check_visa = [f'/usr/lib{bittness}/librsvisa.so', r'/usr/lib/librsvisa.so']
 				for check in check_visa:
 					if os.path.isfile(check):
 						return pyvisa.ResourceManager(check)
+			elif operating_system == 'darwin':
+				# MacOS
+				check_visa = [f'/Library/Frameworks/RsVisa.framework/Versions/Current/RsVisa/librsvisa.dylib']
+				for check in check_visa:
+					if os.path.isfile(check):
+						return pyvisa.ResourceManager(check)
 
-		if visa_select.lower() in ['socketio', 'socket', 'none']:
+		if vsl in ['socketio', 'socket', 'none']:
 			return ResourceManager()
+
 		return pyvisa.ResourceManager(visa_select)
 
 	def _get_visa_manufacturer(self) -> str:
 		"""Returns manufacturer of the current VISA"""
 		if hasattr(self._rm, 'VisaManufacturerName'):
 			return self._rm.VisaManufacturerName
 		try:
@@ -256,14 +310,26 @@
 		setattr(self._session, 'session_thread_rlock', lock)
 		self._lock = lock
 
 	def get_lock(self) -> threading.RLock:
 		"""Returns the current RLock object."""
 		return self._lock
 
+	def lock_resource(self, timeout: int, requested_key: str or bytes = None) -> bytes or None:
+		"""Locks the instrument to prevent it from communicating with other clients."""
+		if requested_key is None:
+			self._session.lock_excl(timeout)
+			return None
+		else:
+			return self._session.lock(timeout, requested_key)
+
+	def unlock_resource(self) -> None:
+		"""Unlocks the instrument to other clients."""
+		self._session.unlock()
+
 	@property
 	def visa_timeout(self) -> int:
 		"""See the visa_timeout.setter."""
 		return int(self._session.timeout)
 
 	@visa_timeout.setter
 	def visa_timeout(self, value: int) -> None:
@@ -278,73 +344,96 @@
 	@data_chunk_size.setter
 	def data_chunk_size(self, chunk_size: int) -> None:
 		"""Sets the maximum size of one block transferred during write/read operations."""
 		self._data_chunk_size = int(chunk_size)
 		self._session.chunk_size = int(chunk_size)
 
 	def _resolve_opc_timeout(self, timeout: int) -> int:
-		"""Resolves entered timeout value - if the input value is less than 1, it is replaces with opc_timeout."""
+		"""Resolves entered timeout value - if the input value is less than 1, it is replaced with opc_timeout."""
 		if timeout is None or timeout < 1:
 			return self.opc_timeout
 		else:
 			return timeout
 
 	def _set_regs_ese_sre(self, mode: WaitForOpcMode) -> WaitForOpcMode:
 		"""Based on the WaitForOpcMode, it sets the ESE and SRE register masks.
 		Returns coerced WaitForOpcMode."""
 		# Set the SRE and ESE registers accordingly
 		# No SRE is supported
+		if self.skip_status_system_setting:
+			return mode
 		self._set_ese_mask(EventStatusRegister.operation_complete)
 		self._set_sre_mask(StatusByte.NONE)
 		return mode
 
+	# noinspection PyTypeChecker
 	def _set_ese_mask(self, mask: EventStatusRegister, reset: bool = True) -> None:
 		"""Sends *ESE command with mask parameter."""
 		if reset is False:
 			current_value = int(self._query_str_no_events('*ESE?'))
 			mask = current_value | mask.value
 		self.write("*ESE %d" % mask.value)
 
+	# noinspection PyTypeChecker
 	def _set_sre_mask(self, mask: StatusByte, reset: bool = True) -> None:
 		"""Sends *SRE command with StatusByte mask parameter."""
 		if reset is False:
 			current_value = int(self._query_str_no_events('*SRE?'))
 			mask = current_value | mask.value
 		# Also affect the _opc_wait_mode:
 		# If the mask has event_status_byte == false, and the _opc_wait_mode is service_request, set it to stb_poll
 		# If the mask has event_status_byte == true, do not change anything
 		self.write(f'*SRE {mask.value}')
 
-	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int, end_mask: StatusByte) -> StatusByte:
+	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int) -> StatusByte:
 		"""Reads Status Byte Register and ends if the ESB bit (5) is set to 1.
 		Also works with the SOCKET and SERIAL interface by sending *STB? query.
 		In that case however, command cannot be a query.
 		Returns the last read Status Byte value."""
 		timeout_secs = timeout / 1000
-		self.clear_before_read()
+		end_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
 		if command.endswith(self._term_char):
 			command = command.rstrip(self._term_char)
-		self.write(command + ';*OPC')
-		# Use catch to return the VISA Timeout back
+
+		if is_query is True:
+			if self.opc_sync_query_mechanism == OpcSyncQueryMechanism.standard or self.opc_sync_query_mechanism == OpcSyncQueryMechanism.also_check_mav:
+				self.clear_before_read()
+				self.write(command + ';*OPC')
+				if self.opc_sync_query_mechanism == OpcSyncQueryMechanism.also_check_mav:
+					end_mask |= StatusByte.message_available
+
+			elif self.opc_sync_query_mechanism == OpcSyncQueryMechanism.only_check_mav_err_queue:
+				self.write(command)
+				end_mask = StatusByte.error_queue_not_empty | StatusByte.message_available
+
+			elif self.opc_sync_query_mechanism == OpcSyncQueryMechanism.cls_only_check_mav_err_queue:
+				self.clear_before_read()
+				self.write(command)
+				end_mask = StatusByte.error_queue_not_empty | StatusByte.message_available
+		else:
+			self.clear_before_read()
+			self.write(command + ';*OPC')
+
 		start = time.time()
 		# STB polling loop
 		while True:
 			stb = self._read_stb()
 			elapsed = self._polling_delay(start)
 			if elapsed > timeout_secs:
 				self._narrow_down_opc_tout_error(command, is_query, timeout)
 			if end_mask & stb:
 				break
 		return stb
 
-	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int, end_mask: StatusByte) -> StatusByte:
+	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int) -> StatusByte:
 		"""Queries Status Byte Register (*STB?) and ends if the ESB bit (5) is set to 1.
 			The command must not be a query. Also works with the SOCKET and SERIAL interface.
 			Returns the last read Status Byte value."""
 		timeout_secs = timeout / 1000
+		end_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
 		self.clear_before_read()
 		if command.endswith(self._term_char):
 			command = command.rstrip(self._term_char)
 		self.write(command + ';*OPC')
 		start = time.time()
 		# STB polling loop
 		while True:
@@ -360,43 +449,47 @@
 		"""Called by the _write_and_poll_stb_vxi when the timeout expires.
 		The method tries to closer identify the cause of the timeout."""
 		stb = self._read_stb()
 		timeout = self._resolve_opc_timeout(timeout)
 		if is_query:
 			if stb & StatusByte.error_queue_not_empty:
 				self.clear()
-				context = f"Sending query '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
-				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
-			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending query '{command.strip()}'.")
+				context = f"Query '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
+				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, self.query_all_syst_errors(), context, first_exc=InstrumentErrors.TimeoutException)
+			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Query '{command.strip()}'.")
 		else:
 			if stb & StatusByte.error_queue_not_empty:
 				self.clear()
-				context = f"Sending command '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
-				InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
-			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Sending command '{command.strip()}'.")
+				context = f"Command '{command.strip()}' with OPC Wait resulted in timeout. OPC Timeout is set to {timeout} ms. Additionally, "
+				InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, self.query_all_syst_errors(), context, first_exc=InstrumentErrors.TimeoutException)
+			InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f"Command '{command.strip()}'.")
 
 	def _narrow_down_io_tout_error(self, context: str, visa_timeout: int = 0) -> None:
 		"""Called internally after IOTimeoutException can narrow down the error to more specific exception.
-		You can define the visa_timeout value for the error message. Otherwise the current visa_timeout is reported."""
+		You can define the visa_timeout value for the error message. Otherwise, the current visa_timeout is reported."""
+		context_stripped = context.strip().rstrip("- ")
+		if self.stb_in_error_check is False:
+			raise InstrumentErrors.TimeoutException(context_stripped)
 		if self.vxi_capable:
 			stb = self._read_stb()
 		else:
 			# Non-Vxi session
 			old_tout = self.visa_timeout
 			try:
 				self.visa_timeout = 500
-				stb = self._query_stb()
+				stb = self._query_stb(False)
 			finally:
 				self.visa_timeout = old_tout
 		if visa_timeout <= 0:
 			visa_timeout = self.visa_timeout
+
 		context = context + f'VISA Timeout error occurred ({visa_timeout} milliseconds)'
 		if stb & StatusByte.error_queue_not_empty:
-			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context + ' and ...')
-		# In case the previous exception is not thrown
+			InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, self.query_all_syst_errors(), context + ' and ...', first_exc=InstrumentErrors.TimeoutException)
+		# In case none of the previous exceptions is thrown
 		raise InstrumentErrors.TimeoutException(context)
 
 	def _polling_delay(self, start):
 		"""Generates progressive polling delay."""
 
 		elapsed = time.time() - start
 		if self._opc_wait_mode == WaitForOpcMode.stb_poll:
@@ -445,59 +538,80 @@
 			if elapsed < 20:
 				time.sleep(1)
 				return elapsed
 			time.sleep(2)
 
 		return elapsed
 
-	def query_syst_error(self) -> str or None:
-		"""Returns one response to the SYSTEM:ERROR? query."""
-		error = self.query_str('SYST:ERR?')
-		if error.startswith('0,'):
+	@staticmethod
+	def _parse_err_query_response(response: str) -> Tuple[int, str]:
+		"""
+		Parses entered response string to Tuple(code, message).
+		E.g.: response = '-110,"Command error"' returns: (-110,'Command error')
+		"""
+		m = re.match(r'([-+]?\d+).*?[\'"](.*)[\'"]', response)
+		code = 0
+		if m:
+			try:
+				code = int(m.group(1))
+			except ValueError:
+				pass
+			return code, m.group(2)
+		else:
+			return code, response
+
+	def query_syst_error(self) -> Tuple[int, str] or None:
+		"""Returns one response to the SYSTEM:ERROR? query.
+		The response is a Tuple of (code: int, message: str)"""
+		error = self._query_str_no_events('SYST:ERR?')
+		if error.startswith('0,') or error.startswith('+0,'):
 			return None
-		return error.strip()
+		return self._parse_err_query_response(error.strip())
 
-	def query_all_syst_errors(self) -> list or None:
-		"""Returns all errors in the instrument's error queue."""
+	def query_all_syst_errors(self) -> List[Tuple[int, str]] or None:
+		"""Returns all errors in the instrument's error queue.
+		If no error is detected, the return value is None."""
 		errors = []
 		while True:
 			entry = self.query_syst_error()
 			if entry is None:
 				break
 			errors.append(entry)
 			if len(errors) > 50:
 				# Safety stop
 				errors.append('query_all_syst_errors - max limit 50 of SYST:ERR? sent.')
 				break
-
 		if len(errors) == 0:
 			return None
 		else:
 			return errors
 
-	def _query_stb(self) -> StatusByte:
+	def _query_stb(self, allow_tout_error_narrow_down: bool = True) -> StatusByte:
 		"""Sends *STB? query and reads the result."""
-		return StatusByte(int(self._query_str_no_events('*STB?')))
+		return StatusByte(int(self._query_str_no_events('*STB?', allow_tout_error_narrow_down)))
 
 	def _read_stb(self) -> StatusByte:
 		"""Calls viReadStb and returns the result."""
 		return StatusByte(self._session.read_stb())
 
 	def clear_before_read(self) -> None:
 		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
 
 		# For NRP-Z sessions, skip this completely
-		if self.is_rsnrp_session():
+		if self.is_rsnrp_session() or self.skip_clear_status:
 			return
 
 		if not self.vxi_capable:
 			# Non-Vxi session must use *CLS in any case
 			self.write('*CLS')
 			correct = False
-			opc = self._query_str_no_events('*OPC?')
+			if self.disable_opc_query:
+				opc = '1'
+			else:
+				opc = self._query_str_no_events('*OPC?')
 			repeat = 0
 			while not correct:
 				if len(opc) <= 2:
 					opc = opc.strip()
 					correct = opc == '0' or opc == '1'
 				if not correct:
 					# Read again with a small VISA timeout
@@ -525,15 +639,15 @@
 				self.query_and_clear_esr()
 			# Check if the status byte value changed
 			previous_stb = stb
 			stb = self._query_stb()
 			if stb == previous_stb:
 				repeat += 1
 				if repeat > 10:
-					raise Exception(f"Cannot clear the instrument's status subsystem. Status Byte: '{stb}'")
+					raise RsInstrException(f"Cannot clear the instrument's status subsystem. Status Byte: '{stb}'")
 
 	def _flush_junk_data(self) -> None:
 		"""Reads junk bytes to clear the instrument's output buffer."""
 		if self.read_delay > 0:
 			time.sleep(self.read_delay / 1000)
 		self._read_unknown_len(StreamWriter.as_bin_var(), False)
 
@@ -568,39 +682,55 @@
 			try:
 				self._session.clear()
 			except Exception:
 				pass
 		else:
 			self._session.clear()
 
+	def is_connection_active(self) -> bool:
+		"""Returns true, if the VISA connection is active and the communication with the instrument still works.
+		This is achieved by:
+		- checking the session property timeout
+		- sending the *IDN? query"""
+		if self._session is None:
+			return False
+		# noinspection PyBroadException
+		try:
+			old_tout = self.visa_timeout
+			self.visa_timeout = 2000
+			if len(self.cmd_idn) > 0:
+				self.write(self.cmd_idn)
+				_ = self._read_str_no_events()
+			self.visa_timeout = old_tout
+			return True
+		except Exception:
+			return False
+
 	def _write_and_wait_for_opc(self, command: str, is_query: bool, timeout: int) -> StatusByte:
 		"""Internal method to synchronise a command with OPC timeout.
 		Timeout value 0 means the OPC timeout is used."""
 		timeout = self._resolve_opc_timeout(timeout)
 
 		if command.endswith(self._term_char):
 			command = command.rstrip(self._term_char)
 		if is_query:
 			InstrumentErrors.assert_query_has_qmark(command, 'Query with OPC')
 		else:
 			InstrumentErrors.assert_cmd_has_no_qmark(command, 'Write with OPC')
 
 		if self._opc_wait_mode == WaitForOpcMode.opc_query:
 			if is_query:
-				raise Exception('Sending a query with OpcQuery synchronization is not possible')
+				raise RsInstrException('Sending a query with OpcQuery synchronization is not possible')
 			stb = self._write_and_query_opc(command, timeout)
 		else:
 			# STB polling
-			end_stb_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
-			if is_query:
-				end_stb_mask |= StatusByte.message_available
 			if self.vxi_capable:
-				stb = self._write_and_poll_stb_vxi(command, is_query, timeout, end_stb_mask)
+				stb = self._write_and_poll_stb_vxi(command, is_query, timeout)
 			else:
-				stb = self._write_and_poll_stb_non_vxi(command, timeout, end_stb_mask)
+				stb = self._write_and_poll_stb_non_vxi(command, timeout)
 
 		return stb
 
 	def _write_and_query_opc(self, cmd: str, timeout: int) -> StatusByte:
 		"""Internal method to write a command followed by query_opc().
 		Used for opc-synchronization if the mode is set to WaitForOpcMode.opc_query or the session is not-vxi.
 		Timeout value 0 means the OPC timeout is used."""
@@ -614,40 +744,52 @@
 			self.write(cmd)
 			self.query_opc()
 		finally:
 			if old_tout != timeout:
 				self.visa_timeout = old_tout
 		return self._query_stb()
 
+	def clear_status_after_query_with_opc(self) -> bool:
+		"""Returns true, if the opc-sync queries require status clearing afterward."""
+		if self.vxi_capable is False or self._opc_wait_mode is WaitForOpcMode.opc_query:
+			return False
+		if self.opc_sync_query_mechanism == InstrumentSettings.OpcSyncQueryMechanism.standard:
+			return True
+		if self.opc_sync_query_mechanism == InstrumentSettings.OpcSyncQueryMechanism.also_check_mav:
+			return True
+		return False
+
 	def write(self, cmd: str) -> None:
 		"""Writes command to the instrument."""
 		if self.write_delay > 0:
 			time.sleep(self.write_delay / 1000)
 		add_tc = False
 		if self._assure_write_with_tc and not cmd.endswith(self._term_char):
 			add_tc = True
+		if self.each_cmd_prefix:
+			cmd = self.each_cmd_prefix + cmd
+		cmd_bytes = cmd.encode(self.encoding)
 		if add_tc:
-			self._session.write(cmd + self._term_char)
-		else:
-			self._session.write(cmd)
+			cmd_bytes += self._term_char.encode(self.encoding)
+		self._session.write_raw(cmd_bytes)
 
 	def _read_unknown_len(self, stream: StreamWriter, allow_chunk_events: bool, prepend_data: AnyStr = None) -> None:
 		"""Reads data of unknown length to the provided WriteStream.
 		The read is performed in an incremental chunk steps to optimize memory use (for NRP-Z session it is set to fixed self._data_chunk_size):
 			- The first read is performed with the fixed size of 1024 bytes
 			- The 2nd one reads 64 kBytes
 			- The 3rd one reads 128 kBytes
 			- The 4th one reads 256 kBytes and so on, with the max cap of self._data_chunk_size
 		:param stream: [StreamWriter] target for the read data
 		:param allow_chunk_events: [bool] if True, the method can send the chunk_events. If False, sending events is blocked.
-		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first chunk read
+		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first read chunk
 		:return: read data [bytes or string], depending on the parameter binary."""
 		with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
 			if prepend_data and isinstance(prepend_data, str):
-				prepend_data = prepend_data.encode('utf-8')
+				prepend_data = prepend_data.encode(self.encoding)
 			chunk_ix = 0
 			eot = False
 			while not eot:
 				if self.is_rsnrp_session():
 					chunk_size = self._data_chunk_size
 				else:
 					if chunk_ix == 0:
@@ -660,15 +802,15 @@
 				if chunk_size > self._data_chunk_size:
 					chunk_size = self._data_chunk_size
 				chunk, self.last_status = self._session.visalib.read(self._session.session, chunk_size)
 				if chunk_ix == 0 and prepend_data:
 					chunk = prepend_data + chunk
 				eot = not self._last_status_more_data_available()
 				if not stream.binary:
-					chunk = chunk.decode('utf-8')
+					chunk = chunk.decode(self.encoding)
 					if eot:
 						chunk = chunk.rstrip(self._term_char)
 				stream.write(chunk)
 				if self.on_read_chunk_handler and allow_chunk_events:
 					total_size = len(stream) if eot is True else None
 					event_args = EventArgsChunk(stream.binary, chunk_ix, len(chunk), total_size, len(stream), eot, None, chunk if self.io_events_include_data else None)
 					self.on_read_chunk_handler(event_args)
@@ -683,37 +825,44 @@
 		Sending of any read events is blocked."""
 		if self.read_delay > 0:
 			time.sleep(self.read_delay / 1000)
 		stream = StreamWriter.as_string_var()
 		self._read_unknown_len(stream, False)
 		return stream.content
 
-	def _query_str_no_events(self, query: str) -> str:
+	def _query_str_no_events(self, query: str, allow_tout_error_narrow_down: bool = True) -> str:
 		"""Queries the instrument and reads the response as string.
 		The length of the string is not limited. The response is then trimmed for trailing LF.
 		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
 		response = ''
 		self.write(query)
 		try:
 			response = self._read_str_no_events()
-		except pyvisa.VisaIOError:
-			self._narrow_down_io_tout_error(f"Querying '{query.rstrip(self._term_char)}' - ")
+		except pyvisa.VisaIOError as e:
+			context = f"Query '{query.rstrip(self._term_char)}'"
+			if e.error_code == StatusCode.error_timeout:
+				if allow_tout_error_narrow_down:
+					self._narrow_down_io_tout_error(context + ' - ')
+				else:
+					raise InstrumentErrors.TimeoutException(context)
+			else:
+				raise InstrumentErrors.RsInstrException(context)
 		return response
 
 	def _query_str_no_events_timed(self, query: str, timeout: int, suppress_read_tout: bool = False) -> str:
 		"""Queries the instrument and reads the response as string.
 		The entered timeout sets the VISA timeout just for this call. You can suppress the timeout error.
 		The length of the string is not limited. The response is then trimmed for trailing LF.
 		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
 		response = ''
 		self.write(query)
 		try:
 			response = self._read_str_timed(timeout, suppress_read_tout)
 		except pyvisa.VisaIOError:
-			self._narrow_down_io_tout_error(f"Querying with timeout {timeout} ms '{query.rstrip(self._term_char)}' - ", timeout)
+			self._narrow_down_io_tout_error(f"Query with timeout {timeout} ms '{query.rstrip(self._term_char)}' - ", timeout)
 		return response
 
 	def _read_str_timed(self, timeout: int, suppress_read_tout: bool = False) -> str:
 		"""Reads response from the instrument with a VISA timeout temporarily set for the read.
 		The VISA timeout is set back to the previous value before the method finishes even if an exception occurs.
 		Sending of any read events is blocked."""
 		old_visa_tout = self.visa_timeout
@@ -748,15 +897,15 @@
 		"""Queries the instrument and reads the response as string.
 		The length of the string is not limited. The response is then trimmed for trailing LF."""
 		response = ''
 		self.write(query)
 		try:
 			response = self._read_str()
 		except pyvisa.VisaIOError:
-			self._narrow_down_io_tout_error(f"Querying '{query.rstrip(self._term_char)}' - ")
+			self._narrow_down_io_tout_error(f"Query '{query.rstrip(self._term_char)}' - ")
 		return response
 
 	def query_str_no_tout_err(self, query: str, tout: int) -> str:
 		"""Same as query_str, but you can set the timeout just for this one call.
 		If the timeout exception occurs, it is suppressed and the method returns Null"""
 		response = None
 		old_tout = self.visa_timeout
@@ -770,23 +919,23 @@
 		return response
 
 	def write_with_opc(self, command: str, timeout: int = None) -> None:
 		"""Sends command with OPC-sync.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		self._write_and_wait_for_opc(command, False, timeout)
 
-	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
+	def query_str_with_opc(self, query: str, timeout: int = None, context: str = 'Query string with OPC') -> str:
 		"""Query string with OPC synchronization.
 		The response is trimmed for any trailing LF.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		timeout = self._resolve_opc_timeout(timeout)
 		if self.vxi_capable and self._opc_wait_mode is not WaitForOpcMode.opc_query:
 			# For Vxi session, use the STB poll or SRQ wait and then read the response
 			stb = self._write_and_wait_for_opc(query, True, timeout)
-			self._check_msg_available_after_opc_wait(stb, query, timeout, 'Query String With OPC')
+			self._check_msg_available_after_opc_wait(stb, query, timeout, context)
 			response = self._read_str()
 		else:
 			# For non-Vxi sessions, use the longer VISA Timeout without the *OPC?
 			# Same is valid for WaitForOpcMode.OpcQuery
 			InstrumentErrors.assert_query_has_qmark(query, 'Query with VISA timeout')
 			self.write(query)
 			old_tout = self.visa_timeout
@@ -824,57 +973,59 @@
 		"""Used internally after _StbPolling() to check if the message is available.
 		Throws an exception in case of MAV not available."""
 		if not self.vxi_capable:
 			return
 		if stb & StatusByte.message_available:
 			return
 		# Message not available
-		context = context + f" SCPI query '{query.rstrip(self._term_char)}'"
+		context = context + f" Query '{query.rstrip(self._term_char)}'"
 		if stb & StatusByte.error_queue_not_empty:
 			# Instrument reports an error
-			InstrumentErrors.assert_no_instrument_status_errors(self._resource_name, self.query_all_syst_errors(), context)
+			InstrumentErrors.assert_no_instrument_status_errors(self.resource_name, self.query_all_syst_errors(), context)
 		else:
 			# Sometimes even if the StatusByte.MessageAvailable is false, the message is available.
 			# Try to read the STB again
 			stb = self._read_stb()
 			if not stb & StatusByte.event_status_byte:
 				# Instrument did not respond within the defined time
 				InstrumentErrors.throw_opc_tout_exception(self.opc_timeout, timeout, f'{context} No response from the instrument.')
 
 	def error_in_error_queue(self) -> bool:
 		"""Returns true, if error queue contains at least one error."""
 		stb = self._query_stb()
-		return (stb & StatusByte.error_queue_not_empty) != 0
+		if stb & StatusByte.error_queue_not_empty:
+			return True
+		return False
 
 	def reset_ese_sre(self) -> None:
 		"""Resets the status of ESE and SRE registers to default values."""
 		self._set_regs_ese_sre(self._opc_wait_mode)
 
 	def write_bin_block(self, cmd: str, data_stream: StreamReader) -> None:
 		"""Writes all the payload as binary data block to the instrument.
 		The binary data header is added at the beginning of the transmission automatically.
 		:param cmd: [str] SCPI command with which to send the data
 		:param data_stream: [StreamReader] data provider for the payload"""
 		data_size = len(data_stream)
 		len_str = f'{data_size}'
 		cmd = cmd.rstrip(self._term_char)
 		if '#' in cmd:
-			raise Exception(
+			raise RsInstrException(
 				f"Command '{cmd}' must be provided without the binary data header. "
 				f"The method 'write_bin_block' composes and prepends the binary data header automatically.")
 		if data_size <= self._std_bin_block_header_max_len:
 			# Standard bin data header for sizes below 1E9 bytes, e.g.: '#512345'
-			cmd_plus_header = f'{cmd}#{len(len_str)}{len_str}'.encode('utf-8')
+			cmd_plus_header = f'{cmd}#{len(len_str)}{len_str}'.encode(self.encoding)
 		else:
 			# Big sizes bin data header: e.g.: '#(3000000000)'
-			cmd_plus_header = f'{cmd}#({len_str})'.encode('utf-8')
+			cmd_plus_header = f'{cmd}#({len_str})'.encode(self.encoding)
 
 		if data_size <= self._data_chunk_size:
 			# Write all in one step
-			full_chunk = data_stream.read_as_binary()
+			full_chunk = data_stream.read_as_binary(self.encoding)
 			write_buf = cmd_plus_header + full_chunk
 			if self._add_term_char_to_write_bin_block:
 				write_buf += self._term_char_bin
 			self._session.write_raw(write_buf)
 			# Event sending
 			if self.on_write_chunk_handler:
 				event_args = EventArgsChunk(True, 0, data_size, data_size, data_size, True, 1, full_chunk if self.io_events_include_data else None)
@@ -890,24 +1041,24 @@
 					time.sleep(self.write_delay / 1000)
 				# Write bin header
 				self._session.write_raw(cmd_plus_header)
 				# Write chunks
 				while True:
 					if len(data_stream) > self._data_chunk_size:
 						#  Not the last segment
-						chunk = data_stream.read_as_binary(self._data_chunk_size)
+						chunk = data_stream.read_as_binary(self.encoding, self._data_chunk_size)
 						self._session.write_raw(chunk)
 						# Event sending
 						if self.on_write_chunk_handler:
 							event_args = EventArgsChunk(
 								True, chunk_ix, self._data_chunk_size, data_size, data_size - len(data_stream), False, total_chunks, chunk if self.io_events_include_data else None)
 							self.on_write_chunk_handler(event_args)
 					else:
 						# Last segment, indicate end of message again
-						chunk = data_stream.read_as_binary()
+						chunk = data_stream.read_as_binary(self.encoding)
 						if self._add_term_char_to_write_bin_block:
 							# Append LF
 							self._session.write_raw(chunk)
 							self._session.send_end = True
 							self._session.write_raw(self._term_char_bin)
 						else:
 							self._session.send_end = True
@@ -936,60 +1087,88 @@
 			char = self._session.read_bytes(1, break_on_termchar=True)
 			if char == b'0':
 				data_type = ReadDataType.bin_unknown_len
 				return data_type, '#0', -1
 			if char == b'(':
 				# format for big lengths i.e. > 1E9 bytes: '#(1234567890123)...'
 				data_type = ReadDataType.bin_known_len
-				len_str = (self.read_up_to_char(b')', 100)[:-1]).decode('utf-8')
+				len_str = (self.read_up_to_char(b')', 100)[:-1]).decode(self.encoding)
 				whole_hdr = '#(' + len_str + ')'
 				length = int(len_str)
 				return data_type, whole_hdr, length
 
 			# classic format for < 1E9 bytes: '#9123456789...'
 			data_type = ReadDataType.bin_known_len
 			len_of_len = int(char)
-			len_str = self._session.read_bytes(len_of_len).decode('utf-8')
+			len_str = self._session.read_bytes(len_of_len).decode(self.encoding)
 			length = int(len_str)
-			whole_hdr = '#' + char.decode('utf-8') + len_str
+			whole_hdr = '#' + char.decode(self.encoding) + len_str
 			return data_type, whole_hdr, length
 
 		data_type = ReadDataType.ascii
 		if char == self._term_char_bin:
 			data_type = ReadDataType.null
 		if self.vxi_capable:
 			# For Vxi session, to be sure, check whether there are more chars in the read buffer
 			stb = self._read_stb()
 			if stb & StatusByte.message_available:
 				data_type = ReadDataType.ascii
-		whole_hdr = char.decode('utf-8')
+		whole_hdr = char.decode(self.encoding)
 		if exc_if_not_bin:
 			if data_type == ReadDataType.null:
-				InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, self._term_char)
+				InstrumentErrors.throw_bin_block_unexp_resp_exception(self.resource_name, self._term_char)
 			# Read 20 more characters to compose a better exception message
-			whole_hdr += self.read_up_to_char(self._term_char_bin, 20).decode('utf-8')
+			whole_hdr += self.read_up_to_char(self._term_char_bin, 20).decode(self.encoding)
 			if self.last_status == pyvisa.constants.StatusCode.success_max_count_read:
 				self._flush_junk_data()
-			InstrumentErrors.throw_bin_block_unexp_resp_exception(self._resource_name, whole_hdr)
+			InstrumentErrors.throw_bin_block_unexp_resp_exception(self.resource_name, whole_hdr)
 		return data_type, whole_hdr, length
 
+	def get_bin_data_length(self, query: str) -> int or None:
+		"""Returns only the length binary data header, and discards the actual data.
+		Any timeout error is suppressed, and the method returns None instead.
+		Warning!!! - for non-VXI sessions (SOCKET, ASRL) this method transfers the entire file to the control PC, which might take a long time."""
+		if self.vxi_capable and self._opc_wait_mode != WaitForOpcMode.opc_query:
+			# For Vxi session, use the STB poll and read the header
+			stb = self._write_and_wait_for_opc(query, True, 0)
+			try:
+				self._check_msg_available_after_opc_wait(stb, query, 0, 'get_bin_data_length')
+			except InstrumentErrors.StatusException:
+				return None
+			data_type, header, length = self._parse_bin_data_header(True)
+			self.clear()
+			self.clear_before_read()
+			return length
+		else:
+			with StreamWriter.as_forget() as stream:
+				old_timeout = self.visa_timeout
+				try:
+					self.visa_timeout = 2000
+					self.query_bin_block(query, stream, True)
+				except InstrumentErrors.StatusException:
+					return None
+				finally:
+					self.visa_timeout = old_timeout
+				length = stream.written_len
+		return length
+
 	def read_bin_block(self, stream: StreamWriter, exc_if_not_bin: bool) -> None:
 		"""Reads binary data block to the provided stream. \n
 		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
 		:param exc_if_not_bin: if True, the method throws exception if the received data is not binary"""
 		data_type, header, length = self._parse_bin_data_header(exc_if_not_bin)
 		if data_type == ReadDataType.ascii:
-			stream.switch_to_string_data()
+			stream.switch_to_string_data(self.encoding)
 			self._read_unknown_len(stream, True, header)
 		elif data_type == ReadDataType.null:
-			# No data, consider it ASCII, Return empty string, and False (signaling ASCII transfer)
-			stream.switch_to_string_data()
+			# No data, consider it ASCII. Change the stream type to ASCII and return empty string
+			stream.switch_to_string_data(self.encoding)
 		elif data_type == ReadDataType.bin_unknown_len:
 			if not self.vxi_capable:
-				raise Exception(f'Non-Vxi11 sessions can not read binary data block of unknown length.')
+				raise RsInstrException(f'Non-Vxi11 sessions can not read binary data block of unknown length.')
 			self._read_unknown_len(stream, True)
 		elif length == 0:
 			self._flush_junk_data()
 		else:
 			self._read_bin_block_known_len(stream, length)
 
 	def _read_bin_block_known_len(self, stream: StreamWriter, length: int) -> None:
@@ -1027,15 +1206,18 @@
 
 	def query_bin_block(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True) -> None:
 		"""Query binary data block and returns it as byte data. \n
 		:param query: [str] query to send to the instrument
 		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
 		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary"""
 		self.write(query)
-		self.read_bin_block(stream, exc_if_not_bin)
+		try:
+			self.read_bin_block(stream, exc_if_not_bin)
+		except pyvisa.VisaIOError:
+			self._narrow_down_io_tout_error(f"Query bin block '{query.rstrip(self._term_char)}' - ")
 		return
 
 	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
 		"""Query binary data block with OPC and returns it as byte data.
 		:param query: [str] query to send to the instrument
 		:param stream: [StreamWriter] target for the read data. Can be string, bytes, or a file
 		:param exc_if_not_bin: [Boolean] if True, the method throws exception if the received data is not binary
@@ -1073,14 +1255,28 @@
 			response += char
 			if char in stop_chars:
 				break
 			if self.last_status != pyvisa.constants.StatusCode.success_max_count_read:
 				break
 		return response
 
+	def go_to_local(self) -> None:
+		"""Puts the instrument into local state."""
+		if self.vxi_capable:
+			self._session.control_ren(pyvisa.constants.RENLineOperation.deassert_gtl)
+		else:
+			self.write("&GTL")
+
+	def go_to_remote(self) -> None:
+		"""Puts the instrument into remote state."""
+		if self.vxi_capable:
+			self._session.control_ren(pyvisa.constants.RENLineOperation.asrt_address)
+		else:
+			self.write("&GTR")
+
 	def get_session_handle(self) -> object:
 		"""Returns the underlying pyvisa session."""
 		return self._session
 
 	def close(self) -> None:
 		"""Closes the Visa session.
 		If the object was created with the direct session input, the session is not closed."""
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/Internal/VisaSessionSim.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/Internal/VisaSessionSim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""VisaSession for simulated sessions."""
+
 import threading
 from typing import Callable, Dict, AnyStr
 
 from . import InstrumentSettings
 from .StreamReader import StreamReader
 from .StreamWriter import StreamWriter
 
@@ -9,14 +11,15 @@
 # noinspection PyMethodMayBeStatic,PyUnusedLocal
 class VisaSessionSim(object):
 	"""Visa session in simulation mode.
 	Provides the properties for the simulation mode.
 	Also serves as a cache for the SCPI command values: If you query a SCPI command value, it returns the last set value by that SCPI command."""
 
 	def __init__(self, resource_name: str, settings: InstrumentSettings, direct_session=None):
+		self.reusing_session = direct_session is not None
 		# noinspection PyTypeChecker
 		self._data_chunk_size: int = None
 		# noinspection PyTypeChecker
 		self._lock: threading.RLock = None
 
 		# Event handlers
 		# noinspection PyTypeChecker
@@ -25,16 +28,17 @@
 		# noinspection PyTypeChecker
 		self.on_write_chunk_handler: Callable = None
 		"""If assigned a handler, the VisaSession sends it event on each write chunk transfer."""
 		self.io_events_include_data: bool = False
 		"""If true, the VisaSession events sent to on_read_chunk_handler and on_write_chunk_handler contain transferred data."""
 
 		self.manufacturer: str = 'Rohde&Schwarz'
-		self._resource_name = resource_name
+		self.resource_name = resource_name
 		self.vxi_capable = True
+		self.encoding = settings.encoding  # default encoder between bytes and string
 
 		# Changeable settings
 		self.opc_timeout = 10000 if settings.opc_timeout == 0 else settings.opc_timeout
 		self.visa_timeout = settings.visa_timeout
 		self.data_chunk_size = settings.io_segment_size
 
 		self._last_cmd = None
@@ -50,14 +54,17 @@
 			rlock = direct_session.session_thread_rlock
 			if isinstance(rlock, type(threading.RLock())):
 				self.assign_lock(rlock)
 		if self.get_lock() is None:
 			# The existing session did not have a thread lock, assign a new one
 			self.assign_lock(threading.RLock())
 
+		if self.reusing_session:
+			self.resource_name = direct_session.resource_name
+
 	def assign_lock(self, lock: threading.RLock) -> None:
 		"""Assigns the provided thread lock. The lock is only used by the parent class Instrument."""
 		self._lock = lock
 
 	def get_lock(self) -> threading.RLock:
 		"""Returns the current RLock object."""
 		return self._lock
@@ -92,25 +99,30 @@
 		return False
 
 	def query_syst_error(self) -> str or None:
 		"""Returns one response to the SYSTEM:ERROR? query."""
 		return None
 
 	def query_all_syst_errors(self) -> list or None:
-		"""Returns all errors in the instrument's error queue."""
-		return []
+		"""Returns all errors in the instrument's error queue.
+		If no error is detected, the return value is None."""
+		return None
 
 	def clear_before_read(self) -> None:
 		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
 		return
 
 	def clear(self) -> None:
 		"""Perform VISA viClear conditionally based on the instrument settings."""
 		return
 
+	def clear_status_after_query_with_opc(self) -> bool:
+		"""Returns true, if the opc-sync queries require status clearing afterward."""
+		return False
+
 	def write(self, cmd: str) -> None:
 		"""Writes command to the instrument."""
 		self._last_cmd = cmd
 		self._update_cmd_vals_cache(cmd)
 		return
 
 	def query_str(self, query: str) -> str:
@@ -121,15 +133,15 @@
 		return 'Simulating' if cached is None else cached
 
 	def write_with_opc(self, cmd: str, timeout: int = None) -> None:
 		"""Sends command with OPC-sync.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		self.write(cmd)
 
-	def query_str_with_opc(self, query: str, timeout: int = None) -> str:
+	def query_str_with_opc(self, query: str, timeout: int = None, context: str = 'Query string with OPC') -> str:
 		"""Query string with OPC synchronization.
 		The response is trimmed for any trailing LF.
 		If you do not provide timeout, the method uses current opc_timeout."""
 		return self.query_str(query)
 
 	def query_opc(self, timeout: int = 0) -> bool:
 		"""Sends *OPC? query and reads the result."""
@@ -160,28 +172,28 @@
 		cached = self._get_cmd_cached_value(query)
 
 		if cached is None:
 			stream.write(bytes([0, 1, 2, 3, 4, 5, 6, 7, 8, 65, 66]))
 			self.cached_to_stream = False
 		else:
 			if isinstance(cached, str):
-				stream.switch_to_string_data()
+				stream.switch_to_string_data(self.encoding)
 			stream.write(cached)
 			self.cached_to_stream = True
 
 	def query_bin_block_with_opc(self, query: str, stream: StreamWriter, exc_if_not_bin: bool = True, timeout: int = None) -> None:
 		"""Query binary data block with OPC and returns it as byte data."""
 		self.query_bin_block(query, stream)
 
 	def read_up_to_char(self, stop_chars: bytes, max_cnt: int) -> bytes:
 		"""Reads until one of the stop_chars is read or the max_cnt is reached, or EOT is detected.
 		Returns the read data including the stop character."""
 		return b'Simulating'
 
 	def get_session_handle(self) -> object:
 		"""Returns the underlying pyvisa session."""
-		return f"Simulating session, resource name '{self._resource_name}'"
+		return f"Simulating session, resource name '{self.resource_name}'"
 
 	def close(self) -> None:
 		"""Closes the Visa session.
 		If the object was created with the direct session input, the session is not closed."""
 		return
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/__init__.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """RsCmwWlanSig instrument driver
-	:version: 3.8.20.40
-	:copyright: 2021 by Rohde & Schwarz GMBH & Co. KG
+	:version: 4.0.110.44
+	:copyright: 2023 by Rohde & Schwarz GMBH & Co. KG
 	:license: MIT, see LICENSE for more details.
 """
 
-__version__ = '3.8.20.40'
+__version__ = '4.0.110.44'
 
 # Main class
 from RsCmwWlanSig.RsCmwWlanSig import RsCmwWlanSig
 
 # Bin data format
 from RsCmwWlanSig.Internal.Conversions import BinIntFormat, BinFloatFormat
 
 # Exceptions
 from RsCmwWlanSig.Internal.InstrumentErrors import RsInstrException, TimeoutException, StatusException, UnexpectedResponseException, ResourceError, DriverValueError
 
 # Callback Event Argument prototypes
 from RsCmwWlanSig.Internal.IoTransferEventArgs import IoTransferEventArgs
 
+# Logging Mode
+from RsCmwWlanSig.Internal.ScpiLogger import LoggingMode
+
 # enums
 from RsCmwWlanSig import enums
 
 # repcaps
 from RsCmwWlanSig import repcap
 
 # Reliability interface
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig/enums.py` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,32 +274,41 @@
 	"""2 Members, DISable ... ENABle"""
 	DISable = 0
 	ENABle = 1
 
 
 # noinspection SpellCheckingInspection
 class EncryptionType(Enum):
-	"""3 Members, AES ... TKIP"""
+	"""4 Members, AES ... TKIP"""
 	AES = 0
 	DISabled = 1
-	TKIP = 2
+	GCMP = 2
+	TKIP = 3
 
 
 # noinspection SpellCheckingInspection
 class EntityOperationMode(Enum):
 	"""6 Members, AP ... WDIRect"""
 	AP = 0
 	HSPot2 = 1
 	IBSS = 2
 	STATion = 3
 	TESTmode = 4
 	WDIRect = 5
 
 
 # noinspection SpellCheckingInspection
+class FilsProbe(Enum):
+	"""3 Members, FILS ... PROBe"""
+	FILS = 0
+	OFF = 1
+	PROBe = 2
+
+
+# noinspection SpellCheckingInspection
 class FlowType(Enum):
 	"""2 Members, ANNounced ... UNANnounced"""
 	ANNounced = 0
 	UNANnounced = 1
 
 
 # noinspection SpellCheckingInspection
@@ -325,24 +334,39 @@
 	"""3 Members, L116 ... L432"""
 	L116 = 0
 	L216 = 1
 	L432 = 2
 
 
 # noinspection SpellCheckingInspection
+class GroupTransform(Enum):
+	"""2 Members, ECP256 ... ECP384"""
+	ECP256 = 0
+	ECP384 = 1
+
+
+# noinspection SpellCheckingInspection
 class GuardInterval(Enum):
 	"""5 Members, GI08 ... SHORt"""
 	GI08 = 0
 	GI16 = 1
 	GI32 = 2
 	LONG = 3
 	SHORt = 4
 
 
 # noinspection SpellCheckingInspection
+class HashMode(Enum):
+	"""3 Members, BOTH ... HUNT"""
+	BOTH = 0
+	H2E = 1
+	HUNT = 2
+
+
+# noinspection SpellCheckingInspection
 class HeTbMainMeasState(Enum):
 	"""3 Members, OFF ... RUN"""
 	OFF = 0
 	RDY = 1
 	RUN = 2
 
 
@@ -387,14 +411,21 @@
 	"""3 Members, IV4 ... IV6"""
 	IV4 = 0
 	IV4V6 = 1
 	IV6 = 2
 
 
 # noinspection SpellCheckingInspection
+class KeyMode(Enum):
+	"""2 Members, FIXed ... RANDom"""
+	FIXed = 0
+	RANDom = 1
+
+
+# noinspection SpellCheckingInspection
 class LenMode(Enum):
 	"""4 Members, DEFault ... UDEFined"""
 	DEFault = 0
 	OFF = 1
 	ON = 2
 	UDEFined = 3
 
@@ -822,14 +853,22 @@
 	MODC = 2
 	MODD = 3
 	MODE = 4
 	MODF = 5
 
 
 # noinspection SpellCheckingInspection
+class Protection(Enum):
+	"""3 Members, REQuired ... UNSupported"""
+	REQuired = 0
+	SUPPorted = 1
+	UNSupported = 2
+
+
+# noinspection SpellCheckingInspection
 class ProtocolType(Enum):
 	"""2 Members, ICMP ... UDP"""
 	ICMP = 0
 	UDP = 1
 
 
 # noinspection SpellCheckingInspection
@@ -994,16 +1033,27 @@
 	RU6 = 5
 	RU7 = 6
 	RU8 = 7
 	RU9 = 8
 
 
 # noinspection SpellCheckingInspection
+class RuSize(Enum):
+	"""6 Members, T106 ... T996"""
+	T106 = 0
+	T242 = 1
+	T26 = 2
+	T484 = 3
+	T52 = 4
+	T996 = 5
+
+
+# noinspection SpellCheckingInspection
 class RxConnector(Enum):
-	"""154 Members, I11I ... RH8"""
+	"""163 Members, I11I ... RH8"""
 	I11I = 0
 	I13I = 1
 	I15I = 2
 	I17I = 3
 	I21I = 4
 	I23I = 5
 	I25I = 6
@@ -1012,152 +1062,161 @@
 	I33I = 9
 	I35I = 10
 	I37I = 11
 	I41I = 12
 	I43I = 13
 	I45I = 14
 	I47I = 15
-	IF1 = 16
-	IF2 = 17
-	IF3 = 18
-	IQ1I = 19
-	IQ3I = 20
-	IQ5I = 21
-	IQ7I = 22
-	R11 = 23
-	R11C = 24
-	R12 = 25
-	R12C = 26
-	R12I = 27
-	R13 = 28
-	R13C = 29
-	R14 = 30
-	R14C = 31
-	R14I = 32
-	R15 = 33
-	R16 = 34
-	R17 = 35
-	R18 = 36
-	R21 = 37
-	R21C = 38
-	R22 = 39
-	R22C = 40
-	R22I = 41
-	R23 = 42
-	R23C = 43
-	R24 = 44
-	R24C = 45
-	R24I = 46
-	R25 = 47
-	R26 = 48
-	R27 = 49
-	R28 = 50
-	R31 = 51
-	R31C = 52
-	R32 = 53
-	R32C = 54
-	R32I = 55
-	R33 = 56
-	R33C = 57
-	R34 = 58
-	R34C = 59
-	R34I = 60
-	R35 = 61
-	R36 = 62
-	R37 = 63
-	R38 = 64
-	R41 = 65
-	R41C = 66
-	R42 = 67
-	R42C = 68
-	R42I = 69
-	R43 = 70
-	R43C = 71
-	R44 = 72
-	R44C = 73
-	R44I = 74
-	R45 = 75
-	R46 = 76
-	R47 = 77
-	R48 = 78
-	RA1 = 79
-	RA2 = 80
-	RA3 = 81
-	RA4 = 82
-	RA5 = 83
-	RA6 = 84
-	RA7 = 85
-	RA8 = 86
-	RB1 = 87
-	RB2 = 88
-	RB3 = 89
-	RB4 = 90
-	RB5 = 91
-	RB6 = 92
-	RB7 = 93
-	RB8 = 94
-	RC1 = 95
-	RC2 = 96
-	RC3 = 97
-	RC4 = 98
-	RC5 = 99
-	RC6 = 100
-	RC7 = 101
-	RC8 = 102
-	RD1 = 103
-	RD2 = 104
-	RD3 = 105
-	RD4 = 106
-	RD5 = 107
-	RD6 = 108
-	RD7 = 109
-	RD8 = 110
-	RE1 = 111
-	RE2 = 112
-	RE3 = 113
-	RE4 = 114
-	RE5 = 115
-	RE6 = 116
-	RE7 = 117
-	RE8 = 118
-	RF1 = 119
-	RF1C = 120
-	RF2 = 121
-	RF2C = 122
-	RF2I = 123
-	RF3 = 124
-	RF3C = 125
-	RF4 = 126
-	RF4C = 127
-	RF4I = 128
-	RF5 = 129
-	RF5C = 130
-	RF6 = 131
-	RF6C = 132
-	RF7 = 133
-	RF8 = 134
-	RFAC = 135
-	RFBC = 136
-	RFBI = 137
-	RG1 = 138
-	RG2 = 139
-	RG3 = 140
-	RG4 = 141
-	RG5 = 142
-	RG6 = 143
-	RG7 = 144
-	RG8 = 145
-	RH1 = 146
-	RH2 = 147
-	RH3 = 148
-	RH4 = 149
-	RH5 = 150
-	RH6 = 151
-	RH7 = 152
-	RH8 = 153
+	IFI1 = 16
+	IFI2 = 17
+	IFI3 = 18
+	IFI4 = 19
+	IFI5 = 20
+	IFI6 = 21
+	IQ1I = 22
+	IQ3I = 23
+	IQ5I = 24
+	IQ7I = 25
+	R10D = 26
+	R11 = 27
+	R11C = 28
+	R11D = 29
+	R12 = 30
+	R12C = 31
+	R12D = 32
+	R12I = 33
+	R13 = 34
+	R13C = 35
+	R14 = 36
+	R14C = 37
+	R14I = 38
+	R15 = 39
+	R16 = 40
+	R17 = 41
+	R18 = 42
+	R21 = 43
+	R21C = 44
+	R22 = 45
+	R22C = 46
+	R22I = 47
+	R23 = 48
+	R23C = 49
+	R24 = 50
+	R24C = 51
+	R24I = 52
+	R25 = 53
+	R26 = 54
+	R27 = 55
+	R28 = 56
+	R31 = 57
+	R31C = 58
+	R32 = 59
+	R32C = 60
+	R32I = 61
+	R33 = 62
+	R33C = 63
+	R34 = 64
+	R34C = 65
+	R34I = 66
+	R35 = 67
+	R36 = 68
+	R37 = 69
+	R38 = 70
+	R41 = 71
+	R41C = 72
+	R42 = 73
+	R42C = 74
+	R42I = 75
+	R43 = 76
+	R43C = 77
+	R44 = 78
+	R44C = 79
+	R44I = 80
+	R45 = 81
+	R46 = 82
+	R47 = 83
+	R48 = 84
+	RA1 = 85
+	RA2 = 86
+	RA3 = 87
+	RA4 = 88
+	RA5 = 89
+	RA6 = 90
+	RA7 = 91
+	RA8 = 92
+	RB1 = 93
+	RB2 = 94
+	RB3 = 95
+	RB4 = 96
+	RB5 = 97
+	RB6 = 98
+	RB7 = 99
+	RB8 = 100
+	RC1 = 101
+	RC2 = 102
+	RC3 = 103
+	RC4 = 104
+	RC5 = 105
+	RC6 = 106
+	RC7 = 107
+	RC8 = 108
+	RD1 = 109
+	RD2 = 110
+	RD3 = 111
+	RD4 = 112
+	RD5 = 113
+	RD6 = 114
+	RD7 = 115
+	RD8 = 116
+	RE1 = 117
+	RE2 = 118
+	RE3 = 119
+	RE4 = 120
+	RE5 = 121
+	RE6 = 122
+	RE7 = 123
+	RE8 = 124
+	RF1 = 125
+	RF1C = 126
+	RF2 = 127
+	RF2C = 128
+	RF2I = 129
+	RF3 = 130
+	RF3C = 131
+	RF4 = 132
+	RF4C = 133
+	RF4I = 134
+	RF5 = 135
+	RF5C = 136
+	RF6 = 137
+	RF6C = 138
+	RF7 = 139
+	RF7C = 140
+	RF8 = 141
+	RF8C = 142
+	RF9C = 143
+	RFAC = 144
+	RFBC = 145
+	RFBI = 146
+	RG1 = 147
+	RG2 = 148
+	RG3 = 149
+	RG4 = 150
+	RG5 = 151
+	RG6 = 152
+	RG7 = 153
+	RG8 = 154
+	RH1 = 155
+	RH2 = 156
+	RH3 = 157
+	RH4 = 158
+	RH5 = 159
+	RH6 = 160
+	RH7 = 161
+	RH8 = 162
 
 
 # noinspection SpellCheckingInspection
 class RxConverter(Enum):
 	"""40 Members, IRX1 ... RX44"""
 	IRX1 = 0
 	IRX11 = 1
@@ -1210,20 +1269,24 @@
 	SCFading = 3
 	STANdard = 4
 	UNDefined = 5
 
 
 # noinspection SpellCheckingInspection
 class SecurityType(Enum):
-	"""5 Members, DISabled ... WPERsonal"""
-	DISabled = 0
-	W2ENterprise = 1
-	W2Personal = 2
-	WENTerprise = 3
-	WPERsonal = 4
+	"""9 Members, AUTO ... WPERsonal"""
+	AUTO = 0
+	DISabled = 1
+	OWE = 2
+	W2ENterprise = 3
+	W2Personal = 4
+	W3ENterprise = 5
+	W3Personal = 6
+	WENTerprise = 7
+	WPERsonal = 8
 
 
 # noinspection SpellCheckingInspection
 class SegmentNumber(Enum):
 	"""3 Members, A ... C"""
 	A = 0
 	B = 1
@@ -1370,14 +1433,24 @@
 	TID4 = 4
 	TID5 = 5
 	TID6 = 6
 	TID7 = 7
 
 
 # noinspection SpellCheckingInspection
+class TpControl(Enum):
+	"""5 Members, INDoor ... VERYlowpow"""
+	INDoor = 0
+	INENabled = 1
+	INSTdpower = 2
+	STANdard = 3
+	VERYlowpow = 4
+
+
+# noinspection SpellCheckingInspection
 class TriggerBandwidth(Enum):
 	"""7 Members, ALL ... ON"""
 	ALL = 0
 	BW160 = 1
 	BW20 = 2
 	BW40 = 3
 	BW80 = 4
@@ -1446,15 +1519,15 @@
 	BSRP = 2
 	BTR = 3
 	MRTS = 4
 
 
 # noinspection SpellCheckingInspection
 class TxConnector(Enum):
-	"""77 Members, I12O ... RH18"""
+	"""86 Members, I12O ... RH18"""
 	I12O = 0
 	I14O = 1
 	I16O = 2
 	I18O = 3
 	I22O = 4
 	I24O = 5
 	I26O = 6
@@ -1463,75 +1536,84 @@
 	I34O = 9
 	I36O = 10
 	I38O = 11
 	I42O = 12
 	I44O = 13
 	I46O = 14
 	I48O = 15
-	IF1 = 16
-	IF2 = 17
-	IF3 = 18
-	IQ2O = 19
-	IQ4O = 20
-	IQ6O = 21
-	IQ8O = 22
-	R118 = 23
-	R1183 = 24
-	R1184 = 25
-	R11C = 26
-	R11O = 27
-	R11O3 = 28
-	R11O4 = 29
-	R12C = 30
-	R13C = 31
-	R13O = 32
-	R14C = 33
-	R214 = 34
-	R218 = 35
-	R21C = 36
-	R21O = 37
-	R22C = 38
-	R23C = 39
-	R23O = 40
-	R24C = 41
-	R258 = 42
-	R318 = 43
-	R31C = 44
-	R31O = 45
-	R32C = 46
-	R33C = 47
-	R33O = 48
-	R34C = 49
-	R418 = 50
-	R41C = 51
-	R41O = 52
-	R42C = 53
-	R43C = 54
-	R43O = 55
-	R44C = 56
-	RA18 = 57
-	RB14 = 58
-	RB18 = 59
-	RC18 = 60
-	RD18 = 61
-	RE18 = 62
-	RF18 = 63
-	RF1C = 64
-	RF1O = 65
-	RF2C = 66
-	RF3C = 67
-	RF3O = 68
-	RF4C = 69
-	RF5C = 70
-	RF6C = 71
-	RFAC = 72
-	RFAO = 73
-	RFBC = 74
-	RG18 = 75
-	RH18 = 76
+	IFO1 = 16
+	IFO2 = 17
+	IFO3 = 18
+	IFO4 = 19
+	IFO5 = 20
+	IFO6 = 21
+	IQ2O = 22
+	IQ4O = 23
+	IQ6O = 24
+	IQ8O = 25
+	R10D = 26
+	R118 = 27
+	R1183 = 28
+	R1184 = 29
+	R11C = 30
+	R11D = 31
+	R11O = 32
+	R11O3 = 33
+	R11O4 = 34
+	R12C = 35
+	R12D = 36
+	R13C = 37
+	R13O = 38
+	R14C = 39
+	R214 = 40
+	R218 = 41
+	R21C = 42
+	R21O = 43
+	R22C = 44
+	R23C = 45
+	R23O = 46
+	R24C = 47
+	R258 = 48
+	R318 = 49
+	R31C = 50
+	R31O = 51
+	R32C = 52
+	R33C = 53
+	R33O = 54
+	R34C = 55
+	R418 = 56
+	R41C = 57
+	R41O = 58
+	R42C = 59
+	R43C = 60
+	R43O = 61
+	R44C = 62
+	RA18 = 63
+	RB14 = 64
+	RB18 = 65
+	RC18 = 66
+	RD18 = 67
+	RE18 = 68
+	RF18 = 69
+	RF1C = 70
+	RF1O = 71
+	RF2C = 72
+	RF3C = 73
+	RF3O = 74
+	RF4C = 75
+	RF5C = 76
+	RF6C = 77
+	RF7C = 78
+	RF8C = 79
+	RF9C = 80
+	RFAC = 81
+	RFAO = 82
+	RFBC = 83
+	RG18 = 84
+	RH18 = 85
 
 
 # noinspection SpellCheckingInspection
 class TxConverter(Enum):
 	"""40 Members, ITX1 ... TX44"""
 	ITX1 = 0
 	ITX11 = 1
```

### Comparing `RsCmwWlanSig-3.8.20.40/RsCmwWlanSig.egg-info/SOURCES.txt` & `RsCmwWlanSig-4.0.110/RsCmwWlanSig.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,300 +1,270 @@
-README.md
+README.rst
 setup.py
 RsCmwWlanSig/RsCmwWlanSig.py
 RsCmwWlanSig/__init__.py
 RsCmwWlanSig/enums.py
 RsCmwWlanSig/repcap.py
 RsCmwWlanSig.egg-info/PKG-INFO
 RsCmwWlanSig.egg-info/SOURCES.txt
 RsCmwWlanSig.egg-info/dependency_links.txt
 RsCmwWlanSig.egg-info/requires.txt
 RsCmwWlanSig.egg-info/top_level.txt
 RsCmwWlanSig/CustomFiles/__init__.py
 RsCmwWlanSig/CustomFiles/events.py
 RsCmwWlanSig/CustomFiles/reliability.py
 RsCmwWlanSig/CustomFiles/utilities.py
-RsCmwWlanSig/Implementations/Call.py
-RsCmwWlanSig/Implementations/Clean.py
-RsCmwWlanSig/Implementations/Configure.py
-RsCmwWlanSig/Implementations/HetBased.py
 RsCmwWlanSig/Implementations/PackRate.py
-RsCmwWlanSig/Implementations/Per.py
-RsCmwWlanSig/Implementations/Pswitched.py
-RsCmwWlanSig/Implementations/Route.py
-RsCmwWlanSig/Implementations/Second.py
-RsCmwWlanSig/Implementations/Sense.py
-RsCmwWlanSig/Implementations/Source.py
-RsCmwWlanSig/Implementations/Third.py
-RsCmwWlanSig/Implementations/Trigger.py
 RsCmwWlanSig/Implementations/__init__.py
-RsCmwWlanSig/Implementations/Call_/Action.py
-RsCmwWlanSig/Implementations/Call_/Sta.py
-RsCmwWlanSig/Implementations/Call_/__init__.py
-RsCmwWlanSig/Implementations/Call_/Action_/Station.py
-RsCmwWlanSig/Implementations/Call_/Action_/Wdirect.py
-RsCmwWlanSig/Implementations/Call_/Action_/Wps.py
-RsCmwWlanSig/Implementations/Call_/Action_/__init__.py
-RsCmwWlanSig/Implementations/Call_/Action_/Station_/Connect.py
-RsCmwWlanSig/Implementations/Call_/Action_/Station_/Reconnect.py
-RsCmwWlanSig/Implementations/Call_/Action_/Station_/__init__.py
-RsCmwWlanSig/Implementations/Call_/Action_/Wdirect_/Sconnection.py
-RsCmwWlanSig/Implementations/Call_/Action_/Wdirect_/__init__.py
-RsCmwWlanSig/Implementations/Call_/Action_/Wps_/Sconnection.py
-RsCmwWlanSig/Implementations/Call_/Action_/Wps_/__init__.py
-RsCmwWlanSig/Implementations/Call_/Sta_/Action.py
-RsCmwWlanSig/Implementations/Call_/Sta_/__init__.py
-RsCmwWlanSig/Implementations/Call_/Sta_/Action_/Disconnect.py
-RsCmwWlanSig/Implementations/Call_/Sta_/Action_/__init__.py
-RsCmwWlanSig/Implementations/Clean_/Elogging.py
-RsCmwWlanSig/Implementations/Clean_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection.py
-RsCmwWlanSig/Implementations/Configure_/Edau.py
-RsCmwWlanSig/Implementations/Configure_/Etoe.py
-RsCmwWlanSig/Implementations/Configure_/Fading.py
-RsCmwWlanSig/Implementations/Configure_/HetBased.py
-RsCmwWlanSig/Implementations/Configure_/IpvFour.py
-RsCmwWlanSig/Implementations/Configure_/IpvSix.py
-RsCmwWlanSig/Implementations/Configure_/Mimo.py
-RsCmwWlanSig/Implementations/Configure_/Mmonitor.py
-RsCmwWlanSig/Implementations/Configure_/Per.py
-RsCmwWlanSig/Implementations/Configure_/Pgen.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings.py
-RsCmwWlanSig/Implementations/Configure_/Sta.py
-RsCmwWlanSig/Implementations/Configure_/UesInfo.py
-RsCmwWlanSig/Implementations/Configure_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Association.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Ccode.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Edca.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hemac.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Muedca.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Qos.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Security.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Srates.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Station.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Twt.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Wdirect.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta_/MacReserve.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Association_/Sta_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Enable.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Ftype.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/MwDuration.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Stime.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/Tenable.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Btwt_/Schedule_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf_/SsTx.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hetf_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Dname.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Plmn.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/Realm.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Hotspot_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding_/SsTx.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/NdpSounding_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/Eaka.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/Esim.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/Rserver.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Security_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/AlsField.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/BlAllocation.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/RuAllocation.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy_/Mcs.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/Dummy_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Allocation.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Ctype.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Mcs.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/Streams.py
-RsCmwWlanSig/Implementations/Configure_/Connection_/Sta_/Dframe_/Hemu_/User_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList.py
-RsCmwWlanSig/Implementations/Configure_/Etoe_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList_/IprAddress.py
-RsCmwWlanSig/Implementations/Configure_/Etoe_/IrList_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn.py
-RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator.py
-RsCmwWlanSig/Implementations/Configure_/Fading_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn_/Bandwidth.py
-RsCmwWlanSig/Implementations/Configure_/Fading_/Awgn_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator_/Iloss.py
-RsCmwWlanSig/Implementations/Configure_/Fading_/Fsimulator_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static.py
-RsCmwWlanSig/Implementations/Configure_/IpvFour_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/IpAddress.py
-RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/IpAddress_/Sta.py
-RsCmwWlanSig/Implementations/Configure_/IpvFour_/Static_/IpAddress_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Mmonitor_/IpAddress.py
-RsCmwWlanSig/Implementations/Configure_/Mmonitor_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Payload.py
-RsCmwWlanSig/Implementations/Configure_/Per_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/AlsField.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/BlAllocation.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/RuAllocation.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy_/Mcs.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/Dummy_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Allocation.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Ctype.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Mcs.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/Streams.py
-RsCmwWlanSig/Implementations/Configure_/Per_/Dframe_/Hemu_/User_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Pgen_/Config.py
-RsCmwWlanSig/Implementations/Configure_/Pgen_/Destination.py
-RsCmwWlanSig/Implementations/Configure_/Pgen_/IpVersion.py
-RsCmwWlanSig/Implementations/Configure_/Pgen_/Protocol.py
-RsCmwWlanSig/Implementations/Configure_/Pgen_/Uports.py
-RsCmwWlanSig/Implementations/Configure_/Pgen_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Eattenuation.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/EpePower.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/MlOffset.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/InputPy.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/Output.py
-RsCmwWlanSig/Implementations/Configure_/RfSettings_/Antenna_/Eattenuation_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Ampdu.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Dfdef.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Ctyp.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Dcm.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Mcs.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Nss.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Rual.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Sss.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/TrsMode.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/Trssi.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/TsrControl.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Hetf_/__init__.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/BarMethod.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/Black.py
-RsCmwWlanSig/Implementations/Configure_/Sta_/Connection_/Qos_/__init__.py
-RsCmwWlanSig/Implementations/HetBased_/State.py
-RsCmwWlanSig/Implementations/HetBased_/UphInfo.py
-RsCmwWlanSig/Implementations/HetBased_/__init__.py
-RsCmwWlanSig/Implementations/Per_/State.py
-RsCmwWlanSig/Implementations/Per_/__init__.py
-RsCmwWlanSig/Implementations/Per_/State_/All.py
-RsCmwWlanSig/Implementations/Per_/State_/__init__.py
-RsCmwWlanSig/Implementations/Pswitched_/State.py
-RsCmwWlanSig/Implementations/Pswitched_/__init__.py
-RsCmwWlanSig/Implementations/Route_/Scenario.py
-RsCmwWlanSig/Implementations/Route_/__init__.py
-RsCmwWlanSig/Implementations/Route_/Scenario_/MimFading.py
-RsCmwWlanSig/Implementations/Route_/Scenario_/Mimo.py
-RsCmwWlanSig/Implementations/Route_/Scenario_/ScFading.py
-RsCmwWlanSig/Implementations/Route_/Scenario_/Scell.py
-RsCmwWlanSig/Implementations/Route_/Scenario_/__init__.py
-RsCmwWlanSig/Implementations/Second_/State.py
-RsCmwWlanSig/Implementations/Second_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Elogging.py
-RsCmwWlanSig/Implementations/Sense_/Pgen.py
-RsCmwWlanSig/Implementations/Sense_/Sinfo.py
-RsCmwWlanSig/Implementations/Sense_/Sta.py
-RsCmwWlanSig/Implementations/Sense_/UesInfo.py
-RsCmwWlanSig/Implementations/Sense_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Pgen_/PgStats.py
-RsCmwWlanSig/Implementations/Sense_/Pgen_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna.py
-RsCmwWlanSig/Implementations/Sense_/Sinfo_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna_/RxpIndicator.py
-RsCmwWlanSig/Implementations/Sense_/Sinfo_/Antenna_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo_/UphInfo.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/HetbInfo_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/He.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/Mac.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/Mac_/Address.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UeCapability_/Mac_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/AbsReport.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/Drate.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxbPower.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/UeAddress.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hemu.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hesu.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Hetb.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Ht.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/NoNht.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/Vht.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/RxPsdu_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/UeAddress_/Ipv.py
-RsCmwWlanSig/Implementations/Sense_/Sta_/UesInfo_/UeAddress_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna.py
-RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress.py
-RsCmwWlanSig/Implementations/Sense_/UesInfo_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna_/ArxbPower.py
-RsCmwWlanSig/Implementations/Sense_/UesInfo_/Antenna_/__init__.py
-RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress_/Ipv.py
-RsCmwWlanSig/Implementations/Sense_/UesInfo_/CmwAddress_/__init__.py
-RsCmwWlanSig/Implementations/Source_/State.py
-RsCmwWlanSig/Implementations/Source_/__init__.py
-RsCmwWlanSig/Implementations/Third_/State.py
-RsCmwWlanSig/Implementations/Third_/__init__.py
-RsCmwWlanSig/Implementations/Trigger_/Rx.py
-RsCmwWlanSig/Implementations/Trigger_/Tx.py
-RsCmwWlanSig/Implementations/Trigger_/__init__.py
-RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame.py
-RsCmwWlanSig/Implementations/Trigger_/Rx_/__init__.py
-RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame_/Plength.py
-RsCmwWlanSig/Implementations/Trigger_/Rx_/MacFrame_/__init__.py
-RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame.py
-RsCmwWlanSig/Implementations/Trigger_/Tx_/__init__.py
-RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame_/Plength.py
-RsCmwWlanSig/Implementations/Trigger_/Tx_/MacFrame_/__init__.py
+RsCmwWlanSig/Implementations/Call/__init__.py
+RsCmwWlanSig/Implementations/Call/Action/__init__.py
+RsCmwWlanSig/Implementations/Call/Action/Station/Connect.py
+RsCmwWlanSig/Implementations/Call/Action/Station/Reconnect.py
+RsCmwWlanSig/Implementations/Call/Action/Station/__init__.py
+RsCmwWlanSig/Implementations/Call/Action/Wdirect/Sconnection.py
+RsCmwWlanSig/Implementations/Call/Action/Wdirect/__init__.py
+RsCmwWlanSig/Implementations/Call/Action/Wps/Sconnection.py
+RsCmwWlanSig/Implementations/Call/Action/Wps/__init__.py
+RsCmwWlanSig/Implementations/Call/Sta/__init__.py
+RsCmwWlanSig/Implementations/Call/Sta/Action/Disconnect.py
+RsCmwWlanSig/Implementations/Call/Sta/Action/__init__.py
+RsCmwWlanSig/Implementations/Clean/Elogging.py
+RsCmwWlanSig/Implementations/Clean/__init__.py
+RsCmwWlanSig/Implementations/Configure/Edau.py
+RsCmwWlanSig/Implementations/Configure/HetBased.py
+RsCmwWlanSig/Implementations/Configure/IpvSix.py
+RsCmwWlanSig/Implementations/Configure/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Aid.py
+RsCmwWlanSig/Implementations/Configure/Connection/DyFragment.py
+RsCmwWlanSig/Implementations/Configure/Connection/Hemac.py
+RsCmwWlanSig/Implementations/Configure/Connection/MfDef.py
+RsCmwWlanSig/Implementations/Configure/Connection/OobDiscovery.py
+RsCmwWlanSig/Implementations/Configure/Connection/Qos.py
+RsCmwWlanSig/Implementations/Configure/Connection/Station.py
+RsCmwWlanSig/Implementations/Configure/Connection/TpControl.py
+RsCmwWlanSig/Implementations/Configure/Connection/Twt.py
+RsCmwWlanSig/Implementations/Configure/Connection/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Association/Disass.py
+RsCmwWlanSig/Implementations/Configure/Connection/Association/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Association/Sta/MacReserve.py
+RsCmwWlanSig/Implementations/Configure/Connection/Association/Sta/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Btwt/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Enable.py
+RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Ftype.py
+RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/MwDuration.py
+RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Stime.py
+RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/Tenable.py
+RsCmwWlanSig/Implementations/Configure/Connection/Btwt/Schedule/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Ccode/Ccconf.py
+RsCmwWlanSig/Implementations/Configure/Connection/Ccode/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Edca/Acbe.py
+RsCmwWlanSig/Implementations/Configure/Connection/Edca/Acbk.py
+RsCmwWlanSig/Implementations/Configure/Connection/Edca/Acvi.py
+RsCmwWlanSig/Implementations/Configure/Connection/Edca/Acvo.py
+RsCmwWlanSig/Implementations/Configure/Connection/Edca/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Hetf/SsTx.py
+RsCmwWlanSig/Implementations/Configure/Connection/Hetf/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Cutil.py
+RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Dname.py
+RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Plmn.py
+RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/Realm.py
+RsCmwWlanSig/Implementations/Configure/Connection/Hotspot/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Muedca/Acbe.py
+RsCmwWlanSig/Implementations/Configure/Connection/Muedca/Acbk.py
+RsCmwWlanSig/Implementations/Configure/Connection/Muedca/Acvi.py
+RsCmwWlanSig/Implementations/Configure/Connection/Muedca/Acvo.py
+RsCmwWlanSig/Implementations/Configure/Connection/Muedca/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/NdpSounding/SsTx.py
+RsCmwWlanSig/Implementations/Configure/Connection/NdpSounding/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Passphrase.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Pkey.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/TypePy.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Eaka/Kalgo.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Eaka/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/KtThree.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/KtTwo.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/Ktone.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Esim/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Rserver/Iconf.py
+RsCmwWlanSig/Implementations/Configure/Connection/Security/Rserver/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Srates/DsssConf.py
+RsCmwWlanSig/Implementations/Configure/Connection/Srates/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/AlsField.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/BlAllocation.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/RuAllocation.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/Dummy/Mcs.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/Dummy/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Allocation.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Ctype.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Mcs.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/Streams.py
+RsCmwWlanSig/Implementations/Configure/Connection/Sta/Dframe/Hemu/User/__init__.py
+RsCmwWlanSig/Implementations/Configure/Connection/Wdirect/Atype.py
+RsCmwWlanSig/Implementations/Configure/Connection/Wdirect/Wdconf.py
+RsCmwWlanSig/Implementations/Configure/Connection/Wdirect/__init__.py
+RsCmwWlanSig/Implementations/Configure/Etoe/DuIp.py
+RsCmwWlanSig/Implementations/Configure/Etoe/__init__.py
+RsCmwWlanSig/Implementations/Configure/Etoe/IrList/IprAddress.py
+RsCmwWlanSig/Implementations/Configure/Etoe/IrList/__init__.py
+RsCmwWlanSig/Implementations/Configure/Fading/__init__.py
+RsCmwWlanSig/Implementations/Configure/Fading/Awgn/Bandwidth.py
+RsCmwWlanSig/Implementations/Configure/Fading/Awgn/__init__.py
+RsCmwWlanSig/Implementations/Configure/Fading/Fsimulator/Iloss.py
+RsCmwWlanSig/Implementations/Configure/Fading/Fsimulator/__init__.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/__init__.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/Smask.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/__init__.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Cmw.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Destination.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Dns.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Gateway.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Sta.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/Stack.py
+RsCmwWlanSig/Implementations/Configure/IpvFour/Static/IpAddress/__init__.py
+RsCmwWlanSig/Implementations/Configure/Mimo/Tcsd.py
+RsCmwWlanSig/Implementations/Configure/Mimo/__init__.py
+RsCmwWlanSig/Implementations/Configure/Mmonitor/IpAddress.py
+RsCmwWlanSig/Implementations/Configure/Mmonitor/__init__.py
+RsCmwWlanSig/Implementations/Configure/Per/Payload.py
+RsCmwWlanSig/Implementations/Configure/Per/__init__.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/__init__.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/AlsField.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/BlAllocation.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/RuAllocation.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/__init__.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/Dummy/Mcs.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/Dummy/__init__.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Allocation.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Ctype.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Mcs.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/Streams.py
+RsCmwWlanSig/Implementations/Configure/Per/Dframe/Hemu/User/__init__.py
+RsCmwWlanSig/Implementations/Configure/Pgen/Config.py
+RsCmwWlanSig/Implementations/Configure/Pgen/Destination.py
+RsCmwWlanSig/Implementations/Configure/Pgen/IpVersion.py
+RsCmwWlanSig/Implementations/Configure/Pgen/Protocol.py
+RsCmwWlanSig/Implementations/Configure/Pgen/Uports.py
+RsCmwWlanSig/Implementations/Configure/Pgen/__init__.py
+RsCmwWlanSig/Implementations/Configure/RfSettings/Eattenuation.py
+RsCmwWlanSig/Implementations/Configure/RfSettings/__init__.py
+RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/EpePower.py
+RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/MlOffset.py
+RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/__init__.py
+RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/InputPy.py
+RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/Output.py
+RsCmwWlanSig/Implementations/Configure/RfSettings/Antenna/Eattenuation/__init__.py
+RsCmwWlanSig/Implementations/Configure/Sta/__init__.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Ampdu.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Dfdef.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/__init__.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Ctyp.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Dcm.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Mcs.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Nss.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Rual.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Sss.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/TrsMode.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/Trssi.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/TsrControl.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Hetf/__init__.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/BarMethod.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/Black.py
+RsCmwWlanSig/Implementations/Configure/Sta/Connection/Qos/__init__.py
+RsCmwWlanSig/Implementations/Configure/UesInfo/Settings.py
+RsCmwWlanSig/Implementations/Configure/UesInfo/__init__.py
+RsCmwWlanSig/Implementations/HetBased/State.py
+RsCmwWlanSig/Implementations/HetBased/UphInfo.py
+RsCmwWlanSig/Implementations/HetBased/__init__.py
+RsCmwWlanSig/Implementations/Per/__init__.py
+RsCmwWlanSig/Implementations/Per/State/All.py
+RsCmwWlanSig/Implementations/Per/State/__init__.py
+RsCmwWlanSig/Implementations/Pswitched/State.py
+RsCmwWlanSig/Implementations/Pswitched/__init__.py
+RsCmwWlanSig/Implementations/Route/__init__.py
+RsCmwWlanSig/Implementations/Route/Scenario/MimFading.py
+RsCmwWlanSig/Implementations/Route/Scenario/Mimo.py
+RsCmwWlanSig/Implementations/Route/Scenario/ScFading.py
+RsCmwWlanSig/Implementations/Route/Scenario/__init__.py
+RsCmwWlanSig/Implementations/Route/Scenario/Scell/Flexible.py
+RsCmwWlanSig/Implementations/Route/Scenario/Scell/__init__.py
+RsCmwWlanSig/Implementations/Second/State.py
+RsCmwWlanSig/Implementations/Second/__init__.py
+RsCmwWlanSig/Implementations/Sense/Elogging.py
+RsCmwWlanSig/Implementations/Sense/__init__.py
+RsCmwWlanSig/Implementations/Sense/Pgen/PgStats.py
+RsCmwWlanSig/Implementations/Sense/Pgen/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sinfo/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sinfo/Antenna/RxpIndicator.py
+RsCmwWlanSig/Implementations/Sense/Sinfo/Antenna/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sta/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sta/HetbInfo/UphInfo.py
+RsCmwWlanSig/Implementations/Sense/Sta/HetbInfo/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/He.py
+RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/Mac/Address.py
+RsCmwWlanSig/Implementations/Sense/Sta/UeCapability/Mac/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/AbsReport.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/Drate.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxbPower.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hemu.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hesu.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Hetb.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Ht.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/NoNht.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/Vht.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/RxPsdu/__init__.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/UeAddress/Ipv.py
+RsCmwWlanSig/Implementations/Sense/Sta/UesInfo/UeAddress/__init__.py
+RsCmwWlanSig/Implementations/Sense/UesInfo/__init__.py
+RsCmwWlanSig/Implementations/Sense/UesInfo/Antenna/ArxbPower.py
+RsCmwWlanSig/Implementations/Sense/UesInfo/Antenna/__init__.py
+RsCmwWlanSig/Implementations/Sense/UesInfo/CmwAddress/Ipv.py
+RsCmwWlanSig/Implementations/Sense/UesInfo/CmwAddress/__init__.py
+RsCmwWlanSig/Implementations/Source/State.py
+RsCmwWlanSig/Implementations/Source/__init__.py
+RsCmwWlanSig/Implementations/Third/State.py
+RsCmwWlanSig/Implementations/Third/__init__.py
+RsCmwWlanSig/Implementations/Trigger/__init__.py
+RsCmwWlanSig/Implementations/Trigger/Rx/__init__.py
+RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/DsmLength.py
+RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/OfmLength.py
+RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/Plength.py
+RsCmwWlanSig/Implementations/Trigger/Rx/MacFrame/__init__.py
+RsCmwWlanSig/Implementations/Trigger/Tx/__init__.py
+RsCmwWlanSig/Implementations/Trigger/Tx/MacFrame/Plength.py
+RsCmwWlanSig/Implementations/Trigger/Tx/MacFrame/__init__.py
 RsCmwWlanSig/Internal/ArgLinkedEventArgs.py
 RsCmwWlanSig/Internal/ArgSingle.py
 RsCmwWlanSig/Internal/ArgSingleList.py
 RsCmwWlanSig/Internal/ArgSingleSuppressed.py
 RsCmwWlanSig/Internal/ArgStringComposer.py
 RsCmwWlanSig/Internal/ArgStruct.py
 RsCmwWlanSig/Internal/ArgStructList.py
 RsCmwWlanSig/Internal/ArgStructStringParser.py
 RsCmwWlanSig/Internal/CommandsGroup.py
 RsCmwWlanSig/Internal/Conversions.py
 RsCmwWlanSig/Internal/ConverterFromScpiString.py
 RsCmwWlanSig/Internal/ConverterToScpiString.py
 RsCmwWlanSig/Internal/Core.py
+RsCmwWlanSig/Internal/GlobalData.py
 RsCmwWlanSig/Internal/Instrument.py
 RsCmwWlanSig/Internal/InstrumentErrors.py
 RsCmwWlanSig/Internal/InstrumentOptions.py
 RsCmwWlanSig/Internal/InstrumentSettings.py
 RsCmwWlanSig/Internal/InternalLinker.py
 RsCmwWlanSig/Internal/IoTransferEventArgs.py
+RsCmwWlanSig/Internal/Properties.py
 RsCmwWlanSig/Internal/RepeatedCapability.py
+RsCmwWlanSig/Internal/ScpiEnums.py
+RsCmwWlanSig/Internal/ScpiLogger.py
 RsCmwWlanSig/Internal/StreamReader.py
 RsCmwWlanSig/Internal/StreamWriter.py
 RsCmwWlanSig/Internal/StructBase.py
 RsCmwWlanSig/Internal/Types.py
 RsCmwWlanSig/Internal/Utilities.py
 RsCmwWlanSig/Internal/VisaPluginSocketIo.py
 RsCmwWlanSig/Internal/VisaSession.py
```

