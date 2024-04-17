# Comparing `tmp/lxfcode-0.2.7-py2.py3-none-any.whl.zip` & `tmp/lxfcode-0.2.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 99166 bytes, number of entries: 92
+Zip file size: 153008 bytes, number of entries: 137
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 01:49 lxf_code/__init__.py
 -rw-rw-r--  2.0 unx      592 b- defN 24-Apr-12 01:49 lxf_code/instances.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 01:49 lxf_code/calcores/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 01:49 lxf_code/calcores/abc/__init__.py
 -rw-rw-r--  2.0 unx      853 b- defN 24-Apr-12 01:49 lxf_code/calcores/abc/abcal.py
 -rw-rw-r--  2.0 unx    11208 b- defN 24-Apr-12 01:49 lxf_code/calcores/abc/abmoire.py
 -rw-rw-r--  2.0 unx    15061 b- defN 24-Apr-12 01:49 lxf_code/calcores/abc/aboptics.py
@@ -83,12 +83,57 @@
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 02:09 lxfcode/calcores/raman/__init__.py
 -rw-rw-r--  2.0 unx     3396 b- defN 24-Apr-12 02:09 lxfcode/calcores/raman/raman_cal.py
 -rw-rw-r--  2.0 unx    16985 b- defN 24-Apr-12 02:09 lxfcode/calcores/raman/raman_plot.py
 -rw-rw-r--  2.0 unx     8465 b- defN 24-Apr-12 02:09 lxfcode/calcores/superlattices/TwistedGra.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-12 02:09 lxfcode/calcores/superlattices/__init__.py
 -rw-rw-r--  2.0 unx     2845 b- defN 24-Apr-12 02:09 lxfcode/calcores/superlattices/comm_stru.py
 -rw-rw-r--  2.0 unx     2448 b- defN 24-Apr-12 02:09 lxfcode/calcores/superlattices/stru_plot.py
--rw-rw-r--  2.0 unx      754 b- defN 24-Apr-12 02:10 lxfcode-0.2.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 24-Apr-12 02:10 lxfcode-0.2.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-12 02:10 lxfcode-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8365 b- defN 24-Apr-12 02:10 lxfcode-0.2.7.dist-info/RECORD
-92 files, 350605 bytes uncompressed, 85640 bytes compressed:  75.6%
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /abc/__init__.py
+-rw-rw-r--  2.0 unx      914 b- defN 24-Apr-17 10:20 lxfcode/calcores /abc/abcal.py
+-rw-rw-r--  2.0 unx    11576 b- defN 24-Apr-17 10:20 lxfcode/calcores /abc/abmoire.py
+-rw-rw-r--  2.0 unx    15061 b- defN 24-Apr-17 10:20 lxfcode/calcores /abc/aboptics.py
+-rw-rw-r--  2.0 unx     8539 b- defN 24-Apr-17 10:20 lxfcode/calcores /abc/abpshe.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /absorption/__init__.py
+-rw-rw-r--  2.0 unx     4403 b- defN 24-Apr-17 10:20 lxfcode/calcores /absorption/absorption_cal.py
+-rw-rw-r--  2.0 unx    16281 b- defN 24-Apr-17 10:20 lxfcode/calcores /absorption/absorption_plot.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /bands/__init__.py
+-rw-rw-r--  2.0 unx     2254 b- defN 24-Apr-17 10:20 lxfcode/calcores /bands/bands_cal.py
+-rw-rw-r--  2.0 unx     2048 b- defN 24-Apr-17 10:20 lxfcode/calcores /bands/bands_plot.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /dos/__init__.py
+-rw-rw-r--  2.0 unx     1916 b- defN 24-Apr-17 10:20 lxfcode/calcores /dos/dos_cal.py
+-rw-rw-r--  2.0 unx     3162 b- defN 24-Apr-17 10:20 lxfcode/calcores /dos/dos_plot.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /filesop/__init__.py
+-rw-rw-r--  2.0 unx     7799 b- defN 24-Apr-17 10:20 lxfcode/calcores /filesop/filesave.py
+-rw-rw-r--  2.0 unx     1157 b- defN 24-Apr-17 10:20 lxfcode/calcores /hamiltonians/SK_potential.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /hamiltonians/__init__.py
+-rw-rw-r--  2.0 unx     4469 b- defN 24-Apr-17 10:20 lxfcode/calcores /hamiltonians/conti_h.py
+-rw-rw-r--  2.0 unx     1803 b- defN 24-Apr-17 10:20 lxfcode/calcores /hamiltonians/klattices.py
+-rw-rw-r--  2.0 unx     3039 b- defN 24-Apr-17 10:20 lxfcode/calcores /hamiltonians/tb_h.py
+-rw-rw-r--  2.0 unx     1726 b- defN 24-Apr-17 10:20 lxfcode/calcores /hamiltonians/vel_op.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /jdos/__init__.py
+-rw-rw-r--  2.0 unx     2734 b- defN 24-Apr-17 10:20 lxfcode/calcores /jdos/jdos_cal.py
+-rw-rw-r--  2.0 unx     2839 b- defN 24-Apr-17 10:20 lxfcode/calcores /jdos/jdos_plot.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /materials/__init__.py
+-rw-rw-r--  2.0 unx     3746 b- defN 24-Apr-17 10:20 lxfcode/calcores /materials/graphene.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /multical/__init__.py
+-rw-rw-r--  2.0 unx     2375 b- defN 24-Apr-17 10:20 lxfcode/calcores /multical/multicorecal.py
+-rw-rw-r--  2.0 unx    14517 b- defN 24-Apr-17 10:20 lxfcode/calcores /multical/raman_scan.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /pshe/__init__.py
+-rw-rw-r--  2.0 unx    16920 b- defN 24-Apr-17 10:20 lxfcode/calcores /pshe/fitexp.py
+-rw-rw-r--  2.0 unx    12738 b- defN 24-Apr-17 10:20 lxfcode/calcores /pshe/shift.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /pubmeth/__init__.py
+-rw-rw-r--  2.0 unx      965 b- defN 24-Apr-17 10:20 lxfcode/calcores /pubmeth/consts.py
+-rw-rw-r--  2.0 unx     2706 b- defN 24-Apr-17 10:20 lxfcode/calcores /pubmeth/pointset.py
+-rw-rw-r--  2.0 unx    11854 b- defN 24-Apr-17 10:20 lxfcode/calcores /pubmeth/pubmeth.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /raman/__init__.py
+-rw-rw-r--  2.0 unx     3428 b- defN 24-Apr-17 10:20 lxfcode/calcores /raman/raman_cal.py
+-rw-rw-r--  2.0 unx    16985 b- defN 24-Apr-17 10:20 lxfcode/calcores /raman/raman_plot.py
+-rw-rw-r--  2.0 unx    10022 b- defN 24-Apr-17 10:20 lxfcode/calcores /superlattices/TwistedGra.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-17 10:20 lxfcode/calcores /superlattices/__init__.py
+-rw-rw-r--  2.0 unx     2845 b- defN 24-Apr-17 10:20 lxfcode/calcores /superlattices/comm_stru.py
+-rw-rw-r--  2.0 unx     2448 b- defN 24-Apr-17 10:20 lxfcode/calcores /superlattices/stru_plot.py
+-rw-rw-r--  2.0 unx      754 b- defN 24-Apr-17 10:21 lxfcode-0.2.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-17 10:21 lxfcode-0.2.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-17 10:21 lxfcode-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    12573 b- defN 24-Apr-17 10:21 lxfcode-0.2.8.dist-info/RECORD
+137 files, 548082 bytes uncompressed, 132706 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -258,20 +258,155 @@
 
 Filename: lxfcode/calcores/superlattices/comm_stru.py
 Comment: 
 
 Filename: lxfcode/calcores/superlattices/stru_plot.py
 Comment: 
 
-Filename: lxfcode-0.2.7.dist-info/METADATA
+Filename: lxfcode/calcores /__init__.py
 Comment: 
 
-Filename: lxfcode-0.2.7.dist-info/WHEEL
+Filename: lxfcode/calcores /abc/__init__.py
 Comment: 
 
-Filename: lxfcode-0.2.7.dist-info/top_level.txt
+Filename: lxfcode/calcores /abc/abcal.py
 Comment: 
 
-Filename: lxfcode-0.2.7.dist-info/RECORD
+Filename: lxfcode/calcores /abc/abmoire.py
+Comment: 
+
+Filename: lxfcode/calcores /abc/aboptics.py
+Comment: 
+
+Filename: lxfcode/calcores /abc/abpshe.py
+Comment: 
+
+Filename: lxfcode/calcores /absorption/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /absorption/absorption_cal.py
+Comment: 
+
+Filename: lxfcode/calcores /absorption/absorption_plot.py
+Comment: 
+
+Filename: lxfcode/calcores /bands/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /bands/bands_cal.py
+Comment: 
+
+Filename: lxfcode/calcores /bands/bands_plot.py
+Comment: 
+
+Filename: lxfcode/calcores /dos/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /dos/dos_cal.py
+Comment: 
+
+Filename: lxfcode/calcores /dos/dos_plot.py
+Comment: 
+
+Filename: lxfcode/calcores /filesop/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /filesop/filesave.py
+Comment: 
+
+Filename: lxfcode/calcores /hamiltonians/SK_potential.py
+Comment: 
+
+Filename: lxfcode/calcores /hamiltonians/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /hamiltonians/conti_h.py
+Comment: 
+
+Filename: lxfcode/calcores /hamiltonians/klattices.py
+Comment: 
+
+Filename: lxfcode/calcores /hamiltonians/tb_h.py
+Comment: 
+
+Filename: lxfcode/calcores /hamiltonians/vel_op.py
+Comment: 
+
+Filename: lxfcode/calcores /jdos/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /jdos/jdos_cal.py
+Comment: 
+
+Filename: lxfcode/calcores /jdos/jdos_plot.py
+Comment: 
+
+Filename: lxfcode/calcores /materials/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /materials/graphene.py
+Comment: 
+
+Filename: lxfcode/calcores /multical/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /multical/multicorecal.py
+Comment: 
+
+Filename: lxfcode/calcores /multical/raman_scan.py
+Comment: 
+
+Filename: lxfcode/calcores /pshe/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /pshe/fitexp.py
+Comment: 
+
+Filename: lxfcode/calcores /pshe/shift.py
+Comment: 
+
+Filename: lxfcode/calcores /pubmeth/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /pubmeth/consts.py
+Comment: 
+
+Filename: lxfcode/calcores /pubmeth/pointset.py
+Comment: 
+
+Filename: lxfcode/calcores /pubmeth/pubmeth.py
+Comment: 
+
+Filename: lxfcode/calcores /raman/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /raman/raman_cal.py
+Comment: 
+
+Filename: lxfcode/calcores /raman/raman_plot.py
+Comment: 
+
+Filename: lxfcode/calcores /superlattices/TwistedGra.py
+Comment: 
+
+Filename: lxfcode/calcores /superlattices/__init__.py
+Comment: 
+
+Filename: lxfcode/calcores /superlattices/comm_stru.py
+Comment: 
+
+Filename: lxfcode/calcores /superlattices/stru_plot.py
+Comment: 
+
+Filename: lxfcode-0.2.8.dist-info/METADATA
+Comment: 
+
+Filename: lxfcode-0.2.8.dist-info/WHEEL
+Comment: 
+
+Filename: lxfcode-0.2.8.dist-info/top_level.txt
+Comment: 
+
+Filename: lxfcode-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lxfcode-0.2.7.dist-info/METADATA` & `lxfcode-0.2.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxfcode
-Version: 0.2.7
+Version: 0.2.8
 Summary: Calculation Package for 2D Materials
 Home-page: https://github.com/Aoxv/aoxvli
 Author: Li Xiaofeng
 Author-email: 951973793@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

## Comparing `lxfcode-0.2.7.dist-info/RECORD` & `lxfcode-0.2.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -82,11 +82,56 @@
 lxfcode/calcores/raman/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lxfcode/calcores/raman/raman_cal.py,sha256=Mwx4dmHQQqgofmL7RAOodUtN1juSHzUV4fOy7WVR__o,3396
 lxfcode/calcores/raman/raman_plot.py,sha256=yRHEsFiOm9UpPwsJLJw_9WAtDYQDIibmuY6349Vz_pQ,16985
 lxfcode/calcores/superlattices/TwistedGra.py,sha256=ST_y8ias9Sb2cQ0HfQMbKTwqXSG_RVWqQtds5zrLbug,8465
 lxfcode/calcores/superlattices/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lxfcode/calcores/superlattices/comm_stru.py,sha256=96515Sobm_MsipZlWYCDQOgnB_t0eyhwvbog5XWdM4M,2845
 lxfcode/calcores/superlattices/stru_plot.py,sha256=CQ7_krNrH5QE60Ap44jM4NxKGSiKdmDAgTBOYXFzs7A,2448
-lxfcode-0.2.7.dist-info/METADATA,sha256=WPJfN4RkT5qoHdOrbEmMpFmpCGtRG37DIhuZ15p4fwk,754
-lxfcode-0.2.7.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
-lxfcode-0.2.7.dist-info/top_level.txt,sha256=rVo0AXfIl0zZSdE6LL30hTueipmcfN_xwDvOWuojE0Y,8
-lxfcode-0.2.7.dist-info/RECORD,,
+lxfcode/calcores /__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /abc/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /abc/abcal.py,sha256=_MzUHZEziAboqiLHNIt7nGCVOCknHNi4MFRFaYunZ_E,914
+lxfcode/calcores /abc/abmoire.py,sha256=d-tfmaKZ4llJfk3ggrjPWIfGxnhqN5ggVmNUVGvu5bI,11576
+lxfcode/calcores /abc/aboptics.py,sha256=2ksiERrHhA-dVuIOvqunovHZPl4qd_yFp06cP8iRMo4,15061
+lxfcode/calcores /abc/abpshe.py,sha256=sIhc2H2dZ_DFs_2f7RhDtwIZ9_0o5Ua-XGX181sQtqk,8539
+lxfcode/calcores /absorption/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /absorption/absorption_cal.py,sha256=2HgdFEssV-0SOJG5LoS3dnkXs-n5DwShtM0vQzpXAu4,4403
+lxfcode/calcores /absorption/absorption_plot.py,sha256=Qh7-PAsd7cdTMZAXvUDr18NElc6YARDCYnpsObN1HGY,16281
+lxfcode/calcores /bands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /bands/bands_cal.py,sha256=LpmUdKIIQfTtajUXZYXFPEtYlqi46e5KVsuYfmvlNMc,2254
+lxfcode/calcores /bands/bands_plot.py,sha256=tPIvftPy-J64cHVQqvgIiuFOxlbBdxveiIySXbNVkOA,2048
+lxfcode/calcores /dos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /dos/dos_cal.py,sha256=lqgZ9NlfKYiNUTjLej4ojym82OLxxNNXmiAfdzIVmBI,1916
+lxfcode/calcores /dos/dos_plot.py,sha256=4GOjpoWjMN4gaSGwrUyDe05tQAZFkEWf7hVH_cPcTNA,3162
+lxfcode/calcores /filesop/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /filesop/filesave.py,sha256=mbcm9yDxzgT8E8WAW_wsVTUvnisdGYhBI8K5RbqhFIg,7799
+lxfcode/calcores /hamiltonians/SK_potential.py,sha256=ETiGHs2SssyTZL2Jfwr8XdReNUAfNFofbDR6tP97I2A,1157
+lxfcode/calcores /hamiltonians/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /hamiltonians/conti_h.py,sha256=DYbNGl7NjtToqZdioCfYc-_FiCSz-Qa0IOhA42KOAi4,4469
+lxfcode/calcores /hamiltonians/klattices.py,sha256=ilrg8u4N2Wml9X-UQQ1T7w_2gazTwA61OefTT2G0uL0,1803
+lxfcode/calcores /hamiltonians/tb_h.py,sha256=w28MxbaPmQNG-ufSyS96GRj3ZsxWhbfCfbtdqMGv8Js,3039
+lxfcode/calcores /hamiltonians/vel_op.py,sha256=UWOU6dNSgyeFQMiVC_u1Aj5Hbd8jY0k2P9phzUElQBM,1726
+lxfcode/calcores /jdos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /jdos/jdos_cal.py,sha256=oQO5n_M2CB7i9zbDFjT8thmWmP4zOzNdfYGfVeN63j8,2734
+lxfcode/calcores /jdos/jdos_plot.py,sha256=zF1g0kQ8O3kGhuHAty8IocOrSliTrGbmhwG9PLKaS7w,2839
+lxfcode/calcores /materials/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /materials/graphene.py,sha256=KhIY-VgB-DrYyku6GeZZ-tY5GnCn_OQaEZW1KgN4mVE,3746
+lxfcode/calcores /multical/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /multical/multicorecal.py,sha256=hocAF9hRiELg7HbnVJb7Fdeto9oPgT8c3FLyZEOCUUw,2375
+lxfcode/calcores /multical/raman_scan.py,sha256=15XL1f0zVwG2FwjgWUTlfws0nm9qVjvoShNl9TliaIE,14517
+lxfcode/calcores /pshe/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /pshe/fitexp.py,sha256=P5ke_vdK7B_WRqc9K3oZyPL4LxKhKutfxeM6wi9wQrk,16920
+lxfcode/calcores /pshe/shift.py,sha256=XANUiu7JdEsyK1jiUtOGP-zSWj2B23sRU8Ujw_ndprQ,12738
+lxfcode/calcores /pubmeth/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /pubmeth/consts.py,sha256=TMc6UT8bhw-Z1b0aaDovsyK35ZzVpcs_1RAHGlvV0-M,965
+lxfcode/calcores /pubmeth/pointset.py,sha256=dCvSFpFuuWKLB1UT-BHb4kDJEJTVnXwq6Aj5KCX-Tec,2706
+lxfcode/calcores /pubmeth/pubmeth.py,sha256=nbid-WcRoj5HT-MY7DsGHOKGJdfjHYycT-_6H1PXvvw,11854
+lxfcode/calcores /raman/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /raman/raman_cal.py,sha256=LOMa05L3l53GbzLnMVQV1rSvBVQmUMxLJ-A_SntxoZ4,3428
+lxfcode/calcores /raman/raman_plot.py,sha256=yRHEsFiOm9UpPwsJLJw_9WAtDYQDIibmuY6349Vz_pQ,16985
+lxfcode/calcores /superlattices/TwistedGra.py,sha256=jYQcrHIIDQ4LVe1CSzoE7VI_4c2yk5AqvDFLm1Nfauk,10022
+lxfcode/calcores /superlattices/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+lxfcode/calcores /superlattices/comm_stru.py,sha256=96515Sobm_MsipZlWYCDQOgnB_t0eyhwvbog5XWdM4M,2845
+lxfcode/calcores /superlattices/stru_plot.py,sha256=CQ7_krNrH5QE60Ap44jM4NxKGSiKdmDAgTBOYXFzs7A,2448
+lxfcode-0.2.8.dist-info/METADATA,sha256=tSbAW7hB68RIRoWVljyXlLaDulLSrRTgZxosz3ueAys,754
+lxfcode-0.2.8.dist-info/WHEEL,sha256=iYlv5fX357PQyRT2o6tw1bN-YcKFFHKqB_LwHO5wP-g,110
+lxfcode-0.2.8.dist-info/top_level.txt,sha256=rVo0AXfIl0zZSdE6LL30hTueipmcfN_xwDvOWuojE0Y,8
+lxfcode-0.2.8.dist-info/RECORD,,
```

