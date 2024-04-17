# Comparing `tmp/mmrotate_dev-1.0.0rc1.tar.gz` & `tmp/mmrotate_dev-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmrotate_dev-1.0.0rc1.tar", last modified: Mon Apr 15 17:53:56 2024, max compression
+gzip compressed data, was "mmrotate_dev-1.0.0rc2.tar", last modified: Wed Apr 17 02:30:51 2024, max compression
```

## Comparing `mmrotate_dev-1.0.0rc1.tar` & `mmrotate_dev-1.0.0rc2.tar`

### file list

```diff
@@ -1,362 +1,362 @@
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.409901 mmrotate_dev-1.0.0rc1/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    11357 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/LICENSE
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      164 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 xuchenjie  (1004) xuchenjie  (1004)    18090 2024-04-15 17:53:56.408901 mmrotate_dev-1.0.0rc1/PKG-INFO
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    15007 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/README.md
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.257901 mmrotate_dev-1.0.0rc1/mmrotate/
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.258901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.231901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.259900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.272900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2829 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dior.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2920 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3470 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dota_coco.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3036 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dota_ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2847 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dota_qbox.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2966 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dotav15.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2963 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dotav2.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2346 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2591 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/hrsid.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2503 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/rsdd.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2590 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/srsdd.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2505 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/ssdd.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      768 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/default_runtime.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.277901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      655 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/schedule_1x.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      656 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/schedule_3x.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      660 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/schedule_40e.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      656 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/schedule_6x.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.278900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/cfa/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2956 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/cfa/cfa-qbox_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2915 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/cfa/cfa-qbox_r50_fpn_40e_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1350 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/cfa/metafile.yml
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.280901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/convnext/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      928 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/convnext/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      896 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/convnext/rotated-retinanet-rbox-le90_convnext-tiny_fpn_kld-stable_adamw-1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.280901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/csl/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      953 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/csl/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      461 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/csl/rotated-retinanet-rbox-le90_r50_fpn_csl-gaussian_amp-1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.281901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gliding_vertex/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4691 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gliding_vertex/gliding-vertex-qbox_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4729 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gliding_vertex/gliding-vertex-rbox_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      894 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gliding_vertex/metafile.yml
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.282900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gwd/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      882 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gwd/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      217 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gwd/rotated-retinanet-hbox-oc_r50_fpn_gwd_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      219 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gwd/rotated-retinanet-rbox-le135_r50_fpn_gwd_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      227 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gwd/rotated-retinanet-rbox-le90_r50_fpn_gwd_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.283901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.283901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dior/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4687 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dior/h2rbox-le90_r50_fpn_adamw-1x_dior.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.284901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dotav15/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3442 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dotav15/h2rbox-le90_r50_fpn_adamw-1x_dotav15.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      447 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dotav15/h2rbox-le90_r50_fpn_adamw-3x_dotav15.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.284901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dotav2/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3533 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dotav2/h2rbox-le90_r50_fpn_adamw-1x_dotav2.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      446 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dotav2/h2rbox-le90_r50_fpn_adamw-3x_dotav2.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      286 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/h2rbox-le90_r50_fpn_adamw-1x_dota-ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3430 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/h2rbox-le90_r50_fpn_adamw-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      444 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/h2rbox-le90_r50_fpn_adamw-3x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4012 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/metafile.yml
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.286901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3756 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3759 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dotav15.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3762 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dotav2.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4491 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-6x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1035 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn_ms_rr-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      829 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn_rr-6x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3060 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/metafile.yml
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.287901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2319 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1268 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/r3det-oc_r50_fpn_kfiou-ln_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2017 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/roi-trans-le90_r50_fpn_kfiou-ln_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      331 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/rotated-retinanet-hbox-le135_r50_fpn_kfiou_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      330 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/rotated-retinanet-hbox-le90_r50_fpn_kfiou_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      328 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/rotated-retinanet-hbox-oc_r50_fpn_kfiou_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1340 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/s2anet-le135_r50_fpn_kfiou-ln_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.290901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4862 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1545 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/r3det-oc_r50_fpn_kld-stable_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1499 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/r3det-oc_r50_fpn_kld_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1499 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/r3det-tiny-oc_r50_fpn_kld_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      349 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/rotated-retinanet-hbox-oc_r50_fpn_kld-stable_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      352 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/rotated-retinanet-hbox-oc_r50_fpn_kld-stable_rr-6x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      328 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/rotated-retinanet-hbox-oc_r50_fpn_kld_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      351 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/rotated-retinanet-rbox-le90_r50_fpn_kld-stable_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      234 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/rotated-retinanet-rbox-le90_r50_fpn_kld-stable_adamw-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      362 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/rotated-retinanet-rbox-le90_r50_fpn_kld-stable_rr-6x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      330 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/rotated-retinanet-rbox-le90_r50_fpn_kld_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.292900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1414 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4764 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4764 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_hrsid.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4763 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_rsdd.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4764 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_srsdd.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4763 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_ssdd.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       97 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_amp-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2107 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_swin-tiny_fpn_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.293901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_reppoints/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1517 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_reppoints/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3097 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_reppoints/oriented-reppoints-qbox_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3180 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_reppoints/oriented-reppoints-qbox_r50_fpn_mstrain-40e_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.306901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2401 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      786 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/rotated-fcos-hbox-le90_r50_fpn_psc-dual_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      790 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/rotated-fcos-hbox-le90_r50_fpn_psc_rr-6x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      719 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/rotated-retinanet-rbox-le90_r50_fpn_psc-dual_amp-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      744 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/rotated-retinanet-rbox-le90_r50_fpn_psc_rr-6x_hrsc.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.308900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1240 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4049 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/r3det-oc_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5521 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/r3det-refine-oc_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4049 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/r3det-tiny-oc_r50_fpn_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.322901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2251 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7013 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7010 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_3x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       92 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_amp-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7016 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_rr-1x_dota-ms.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.323901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2375 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7000 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le135_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      592 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_1x_dota-ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6999 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       93 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_amp-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6999 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_rr-1x_dota-ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2158 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_swin-tiny_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6997 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-oc_r50_fpn_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.323901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_atss/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1872 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_atss/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2500 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_atss/rotated-atss-le90_r50_fpn_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.324900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_faster_rcnn/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      992 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_faster_rcnn/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4623 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_faster_rcnn/rotated-faster-rcnn-le90_r50_fpn_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.325900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2334 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      337 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-hbox-le90_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      604 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-hbox-le90_r50_fpn_csl-gaussian_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2054 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      268 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_kld_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2648 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_rr-6x_hrsc.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.325900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_reppoints/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      889 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_reppoints/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2927 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_reppoints/rotated-reppoints-qbox_r50_fpn_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.327901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5080 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      630 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-le135_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      631 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-le90_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      627 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-oc_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3078 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-oc_r50_fpn_rr-6x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      328 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le135_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2482 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_1x_dior.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2482 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      108 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_amp-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2485 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_rr-1x_dota-ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3076 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_rr-6x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      329 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-oc_r50_fpn_1x_dior.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      329 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-oc_r50_fpn_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.330901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.330901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      999 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/default_runtime.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3361 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/dota_rr.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3360 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/dota_rr_ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2937 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/hrsc_rr.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      820 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/schedule_3x.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5172 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5564 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-100e-aug-dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5664 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-300e-aug-hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2551 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-3x-dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2554 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-3x-dota_ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3168 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-9x-hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      674 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-coco_pretrain-3x-dota_ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      712 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_m-3x-dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      715 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_m-3x-dota_ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      724 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_s-3x-dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      727 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_s-3x-dota_ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3037 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-300e-aug-hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      726 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-3x-dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      729 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-3x-dota_ms.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      622 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-9x-hrsc.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.331900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5601 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/cascade-s2anet-le135_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1255 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4063 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4211 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_3x_hrsc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       91 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_amp-1x_dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4142 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/s2anet-le90_r50_fpn_1x_dota.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.332901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/sasm_reppoints/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      772 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/sasm_reppoints/metafile.yml
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2775 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/sasm_reppoints/sasm-reppoints-qbox_r50_fpn_1x_dota.py
--rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)      789 2024-04-15 17:53:55.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/model-index.yml
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.333901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.343901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7656 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/analyze_logs.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4211 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/benchmark.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3000 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/browse_dataset.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    10098 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/confusion_matrix.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2736 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/get_flops.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.233901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/data/
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.343901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/data/dota/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5386 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/data/dota/dota2coco.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.343901 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/data/dota/split/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    19194 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/data/dota/split/img_split.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.344900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/deployment/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3748 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/deployment/mmrotate2torchserve.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3711 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/deployment/mmrotate_handler.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      479 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/dist_test.sh
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      442 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/dist_train.sh
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.344900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/misc/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1110 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/misc/print_config.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.344900 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/model_converters/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1553 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/model_converters/publish_model.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      566 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/slurm_test.sh
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      574 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/slurm_train.sh
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4556 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/test.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4611 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/train.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1544 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/__init__.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.345901 mmrotate_dev-1.0.0rc1/mmrotate/apis/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      146 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/apis/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3738 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/apis/inference.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.345901 mmrotate_dev-1.0.0rc1/mmrotate/datasets/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      394 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/datasets/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8494 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/datasets/dior.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7487 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/datasets/dota.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     9357 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/datasets/hrsc.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.346901 mmrotate_dev-1.0.0rc1/mmrotate/datasets/transforms/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      354 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/datasets/transforms/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1919 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/datasets/transforms/loading.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    17011 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/datasets/transforms/transforms.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.346901 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      135 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/__init__.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.347900 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/functional/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      114 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/functional/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    14364 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/functional/mean_ap.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.347900 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/metrics/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      182 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/metrics/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    15515 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/metrics/dota_metric.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    15435 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/evaluation/metrics/rotated_coco_metric.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.348900 mmrotate_dev-1.0.0rc1/mmrotate/models/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      443 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/__init__.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.348900 mmrotate_dev-1.0.0rc1/mmrotate/models/backbones/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      104 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/backbones/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    23583 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/backbones/re_resnet.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.352901 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1082 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    28883 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/angle_branch_retina_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    25015 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/cfa_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    31406 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/h2rbox_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    30770 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/h2rbox_v2_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    44051 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/oriented_reppoints_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3765 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/oriented_rpn_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    13175 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/r3_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    17066 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_atss_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    29983 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_fcos_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    22704 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_reppoints_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4253 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_retina_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    37558 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_rtmdet_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    14810 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/s2a_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    21390 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/sam_reppoints_head.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.365901 mmrotate_dev-1.0.0rc1/mmrotate/models/detectors/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      261 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/detectors/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6207 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/detectors/h2rbox.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7893 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/detectors/h2rbox_v2.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8666 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/detectors/refine_single_stage.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.366901 mmrotate_dev-1.0.0rc1/mmrotate/models/layers/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      188 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/layers/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6875 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/layers/align.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.369901 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      700 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    12436 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/convex_giou_loss.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    13176 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/gaussian_dist_loss.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7558 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/gaussian_dist_loss_v1.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3420 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/h2rbox_consistency_loss.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2774 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/h2rbox_v2_consistency_loss.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5206 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/kf_iou_loss.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4866 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/rotated_iou_loss.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4774 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/smooth_focal_loss.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3306 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/losses/spatial_border_loss.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.369901 mmrotate_dev-1.0.0rc1/mmrotate/models/necks/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       95 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/necks/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    14000 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/necks/re_fpn.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.370900 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      290 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/__init__.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.371900 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/bbox_heads/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      195 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/bbox_heads/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6928 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/bbox_heads/convfc_rbbox_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    34752 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/bbox_heads/gv_bbox_head.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7847 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/gv_ratio_roi_head.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.372901 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/roi_extractors/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      162 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/roi_extractors/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6171 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/roi_extractors/rotate_single_level_roi_extractor.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.372901 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      184 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/__init__.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.374900 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      639 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8072 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/convex_assigner.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    10401 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/max_convex_iou_assigner.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     9246 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/rotate_iou2d_calculator.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    10770 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/rotated_atss_assigner.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8308 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/sas_assigner.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.376901 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      775 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     9808 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/angle_coder.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    10219 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_midpointoffset_rbbox_coder.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1654 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_xywh_hbbox_coder.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1648 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_xywh_qbbox_coder.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    12455 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_xywht_hbbox_coder.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    13212 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_xywht_rbbox_coder.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4554 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/distance_angle_point_coder.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4916 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/gliding_vertex_coder.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.376901 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/prior_generators/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      242 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/prior_generators/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2821 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/prior_generators/anchor_generator.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.390900 mmrotate_dev-1.0.0rc1/mmrotate/models/utils/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      398 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/utils/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5303 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/utils/enn.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3268 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/utils/misc.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5327 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/utils/orconv.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      691 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/mmrotate/models/utils/ripool.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3637 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/registry.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.390900 mmrotate_dev-1.0.0rc1/mmrotate/structures/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       88 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/structures/__init__.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.392901 mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      628 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3931 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/bbox_overlaps.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3782 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/box_converters.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    14250 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/quadri_boxes.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    19126 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/rotated_boxes.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3577 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/transforms.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.392901 mmrotate_dev-1.0.0rc1/mmrotate/testing/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      191 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/testing/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8215 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/testing/_utils.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.393900 mmrotate_dev-1.0.0rc1/mmrotate/utils/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      395 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/utils/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      486 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/utils/collect_env.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1073 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/utils/misc.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.394900 mmrotate_dev-1.0.0rc1/mmrotate/utils/patch/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      226 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/utils/patch/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4356 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/utils/patch/merge_results.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2931 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/utils/patch/split.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1874 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/utils/setup_env.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      102 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/version.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.395901 mmrotate_dev-1.0.0rc1/mmrotate/visualization/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      179 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/visualization/__init__.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5837 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/visualization/local_visualizer.py
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1720 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/mmrotate/visualization/palette.py
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.398901 mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/
--rw-r--r--   0 xuchenjie  (1004) xuchenjie  (1004)    18090 2024-04-15 17:53:56.000000 mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/PKG-INFO
--rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)    15662 2024-04-15 17:53:56.000000 mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)        1 2024-04-15 17:53:56.000000 mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)        1 2024-04-15 17:53:56.000000 mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/not-zip-safe
--rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)      594 2024-04-15 17:53:56.000000 mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/requires.txt
--rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)        9 2024-04-15 17:53:56.000000 mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/top_level.txt
-drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-15 17:53:56.398901 mmrotate_dev-1.0.0rc1/requirements/
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       64 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/requirements/build.txt
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      195 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/requirements/docs.txt
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       62 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/requirements/mminstall.txt
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       36 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc1/requirements/optional.txt
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       71 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/requirements/readthedocs.txt
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       54 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/requirements/runtime.txt
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      289 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc1/requirements/tests.txt
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      646 2024-04-15 17:53:56.409901 mmrotate_dev-1.0.0rc1/setup.cfg
--rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7304 2024-04-15 17:52:35.000000 mmrotate_dev-1.0.0rc1/setup.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.534031 mmrotate_dev-1.0.0rc2/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    11357 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/LICENSE
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      164 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/MANIFEST.in
+-rw-r--r--   0 xuchenjie  (1004) xuchenjie  (1004)    18090 2024-04-17 02:30:51.534031 mmrotate_dev-1.0.0rc2/PKG-INFO
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    15007 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/README.md
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.500031 mmrotate_dev-1.0.0rc2/mmrotate/
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.501031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.497031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.501031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.502031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2829 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dior.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2920 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3470 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dota_coco.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3036 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dota_ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2847 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dota_qbox.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2966 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dotav15.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2963 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dotav2.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2346 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2591 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/hrsid.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2503 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/rsdd.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2590 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/srsdd.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2505 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/ssdd.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      768 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/default_runtime.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.502031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      655 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/schedule_1x.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      656 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/schedule_3x.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      660 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/schedule_40e.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      656 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/schedule_6x.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.502031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/cfa/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2956 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/cfa/cfa-qbox_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2915 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/cfa/cfa-qbox_r50_fpn_40e_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1350 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/cfa/metafile.yml
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.503031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/convnext/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      928 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/convnext/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      896 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/convnext/rotated-retinanet-rbox-le90_convnext-tiny_fpn_kld-stable_adamw-1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.503031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/csl/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      953 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/csl/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      461 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/csl/rotated-retinanet-rbox-le90_r50_fpn_csl-gaussian_amp-1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.503031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gliding_vertex/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4691 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gliding_vertex/gliding-vertex-qbox_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4729 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gliding_vertex/gliding-vertex-rbox_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      894 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gliding_vertex/metafile.yml
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.504031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gwd/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      882 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gwd/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      217 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gwd/rotated-retinanet-hbox-oc_r50_fpn_gwd_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      219 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gwd/rotated-retinanet-rbox-le135_r50_fpn_gwd_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      227 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gwd/rotated-retinanet-rbox-le90_r50_fpn_gwd_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.504031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.504031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dior/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4687 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dior/h2rbox-le90_r50_fpn_adamw-1x_dior.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.504031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dotav15/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3442 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dotav15/h2rbox-le90_r50_fpn_adamw-1x_dotav15.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      447 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dotav15/h2rbox-le90_r50_fpn_adamw-3x_dotav15.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.504031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dotav2/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3533 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dotav2/h2rbox-le90_r50_fpn_adamw-1x_dotav2.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      446 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dotav2/h2rbox-le90_r50_fpn_adamw-3x_dotav2.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      286 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/h2rbox-le90_r50_fpn_adamw-1x_dota-ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3430 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/h2rbox-le90_r50_fpn_adamw-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      444 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/h2rbox-le90_r50_fpn_adamw-3x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4012 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/metafile.yml
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.505031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3756 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3759 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dotav15.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3762 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dotav2.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4491 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-6x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1035 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn_ms_rr-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      829 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn_rr-6x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3060 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/metafile.yml
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.506031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2319 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1268 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/r3det-oc_r50_fpn_kfiou-ln_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2017 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/roi-trans-le90_r50_fpn_kfiou-ln_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      331 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/rotated-retinanet-hbox-le135_r50_fpn_kfiou_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      330 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/rotated-retinanet-hbox-le90_r50_fpn_kfiou_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      328 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/rotated-retinanet-hbox-oc_r50_fpn_kfiou_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1340 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/s2anet-le135_r50_fpn_kfiou-ln_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.507031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4862 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1545 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/r3det-oc_r50_fpn_kld-stable_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1499 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/r3det-oc_r50_fpn_kld_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1499 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/r3det-tiny-oc_r50_fpn_kld_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      349 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/rotated-retinanet-hbox-oc_r50_fpn_kld-stable_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      352 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/rotated-retinanet-hbox-oc_r50_fpn_kld-stable_rr-6x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      328 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/rotated-retinanet-hbox-oc_r50_fpn_kld_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      351 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/rotated-retinanet-rbox-le90_r50_fpn_kld-stable_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      234 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/rotated-retinanet-rbox-le90_r50_fpn_kld-stable_adamw-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      362 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/rotated-retinanet-rbox-le90_r50_fpn_kld-stable_rr-6x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      330 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/rotated-retinanet-rbox-le90_r50_fpn_kld_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.508031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1414 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4764 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4764 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_hrsid.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4763 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_rsdd.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4764 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_srsdd.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4763 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_ssdd.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       97 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_amp-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2107 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_swin-tiny_fpn_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.508031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_reppoints/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1517 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_reppoints/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3097 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_reppoints/oriented-reppoints-qbox_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3180 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_reppoints/oriented-reppoints-qbox_r50_fpn_mstrain-40e_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.509031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2401 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      786 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/rotated-fcos-hbox-le90_r50_fpn_psc-dual_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      790 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/rotated-fcos-hbox-le90_r50_fpn_psc_rr-6x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      719 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/rotated-retinanet-rbox-le90_r50_fpn_psc-dual_amp-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      744 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/rotated-retinanet-rbox-le90_r50_fpn_psc_rr-6x_hrsc.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.509031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1240 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4049 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/r3det-oc_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5521 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/r3det-refine-oc_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4049 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/r3det-tiny-oc_r50_fpn_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.509031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2251 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7013 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7010 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_3x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       92 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_amp-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7016 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_rr-1x_dota-ms.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.510031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2375 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7000 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le135_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      592 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_1x_dota-ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6999 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       93 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_amp-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6999 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_rr-1x_dota-ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2158 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_swin-tiny_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6997 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-oc_r50_fpn_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.510031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_atss/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1872 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_atss/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2500 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_atss/rotated-atss-le90_r50_fpn_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.511031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_faster_rcnn/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      992 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_faster_rcnn/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4623 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_faster_rcnn/rotated-faster-rcnn-le90_r50_fpn_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.511031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2334 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      337 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-hbox-le90_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      604 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-hbox-le90_r50_fpn_csl-gaussian_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2054 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      268 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_kld_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2648 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_rr-6x_hrsc.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.511031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_reppoints/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      889 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_reppoints/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2927 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_reppoints/rotated-reppoints-qbox_r50_fpn_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.513031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5080 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      630 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-le135_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      631 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-le90_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      627 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-oc_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3078 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-oc_r50_fpn_rr-6x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      328 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le135_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2482 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_1x_dior.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2482 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      108 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_amp-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2485 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_rr-1x_dota-ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3076 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_rr-6x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      329 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-oc_r50_fpn_1x_dior.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      329 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-oc_r50_fpn_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.515031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.515031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      999 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/default_runtime.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3361 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/dota_rr.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3360 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/dota_rr_ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2937 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/hrsc_rr.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      820 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/schedule_3x.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5172 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5564 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-100e-aug-dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5664 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-300e-aug-hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2551 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-3x-dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2554 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-3x-dota_ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3168 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-9x-hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      674 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-coco_pretrain-3x-dota_ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      712 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_m-3x-dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      715 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_m-3x-dota_ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      724 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_s-3x-dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      727 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_s-3x-dota_ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3037 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-300e-aug-hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      726 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-3x-dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      729 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-3x-dota_ms.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      622 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-9x-hrsc.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.516031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5601 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/cascade-s2anet-le135_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1255 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4063 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4211 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_3x_hrsc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       91 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_amp-1x_dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4142 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/s2anet-le90_r50_fpn_1x_dota.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.516031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/sasm_reppoints/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      772 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/sasm_reppoints/metafile.yml
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2775 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/sasm_reppoints/sasm-reppoints-qbox_r50_fpn_1x_dota.py
+-rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)      789 2024-04-17 02:30:51.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/model-index.yml
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.516031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.517031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7656 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/analyze_logs.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4211 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/benchmark.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3000 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/browse_dataset.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    10098 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/confusion_matrix.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2736 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/get_flops.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.497031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/data/
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.517031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/data/dota/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5386 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/data/dota/dota2coco.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.517031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/data/dota/split/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    19194 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/data/dota/split/img_split.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.517031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/deployment/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3748 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/deployment/mmrotate2torchserve.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3711 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/deployment/mmrotate_handler.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      479 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/dist_test.sh
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      442 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/dist_train.sh
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.517031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/misc/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1110 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/misc/print_config.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.518031 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/model_converters/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1553 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/model_converters/publish_model.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      566 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/slurm_test.sh
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      574 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/slurm_train.sh
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4556 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/test.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4611 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/train.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1544 2024-04-17 02:09:40.000000 mmrotate_dev-1.0.0rc2/mmrotate/__init__.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.518031 mmrotate_dev-1.0.0rc2/mmrotate/apis/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      146 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/apis/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3738 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/apis/inference.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.518031 mmrotate_dev-1.0.0rc2/mmrotate/datasets/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      394 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/datasets/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8494 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/datasets/dior.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7487 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/datasets/dota.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     9357 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/datasets/hrsc.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.519031 mmrotate_dev-1.0.0rc2/mmrotate/datasets/transforms/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      354 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/datasets/transforms/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1919 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/datasets/transforms/loading.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    17011 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/datasets/transforms/transforms.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.519031 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      135 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/__init__.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.519031 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/functional/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      114 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/functional/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    14364 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/functional/mean_ap.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.519031 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/metrics/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      182 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/metrics/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    15515 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/metrics/dota_metric.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    15435 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/evaluation/metrics/rotated_coco_metric.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.519031 mmrotate_dev-1.0.0rc2/mmrotate/models/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      443 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/__init__.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.519031 mmrotate_dev-1.0.0rc2/mmrotate/models/backbones/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      104 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/backbones/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    23583 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/backbones/re_resnet.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.521031 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1082 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    28883 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/angle_branch_retina_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    25015 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/cfa_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    31406 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/h2rbox_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    30770 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/h2rbox_v2_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    44051 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/oriented_reppoints_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3765 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/oriented_rpn_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    13175 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/r3_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    17066 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_atss_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    29983 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_fcos_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    22704 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_reppoints_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4253 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_retina_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    37558 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_rtmdet_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    14810 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/s2a_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    21390 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/sam_reppoints_head.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.522031 mmrotate_dev-1.0.0rc2/mmrotate/models/detectors/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      261 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/detectors/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6207 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/detectors/h2rbox.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7893 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/detectors/h2rbox_v2.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8666 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/detectors/refine_single_stage.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.522031 mmrotate_dev-1.0.0rc2/mmrotate/models/layers/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      188 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/layers/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6875 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/layers/align.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.523031 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      700 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    12436 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/convex_giou_loss.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    13176 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/gaussian_dist_loss.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7558 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/gaussian_dist_loss_v1.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3420 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/h2rbox_consistency_loss.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2774 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/h2rbox_v2_consistency_loss.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5206 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/kf_iou_loss.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4866 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/rotated_iou_loss.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4774 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/smooth_focal_loss.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3306 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/losses/spatial_border_loss.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.523031 mmrotate_dev-1.0.0rc2/mmrotate/models/necks/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       95 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/necks/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    14000 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/necks/re_fpn.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.523031 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      290 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/__init__.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.524031 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/bbox_heads/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      195 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/bbox_heads/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6928 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/bbox_heads/convfc_rbbox_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    34752 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/bbox_heads/gv_bbox_head.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7847 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/gv_ratio_roi_head.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.524031 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/roi_extractors/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      162 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/roi_extractors/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     6171 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/roi_extractors/rotate_single_level_roi_extractor.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.524031 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      184 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/__init__.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.525031 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      639 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8072 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/convex_assigner.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    10401 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/max_convex_iou_assigner.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     9246 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/rotate_iou2d_calculator.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    10770 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/rotated_atss_assigner.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8308 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/sas_assigner.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.525031 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      775 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     9808 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/angle_coder.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    10219 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_midpointoffset_rbbox_coder.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1654 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_xywh_hbbox_coder.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1648 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_xywh_qbbox_coder.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    12455 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_xywht_hbbox_coder.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    13212 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_xywht_rbbox_coder.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4554 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/distance_angle_point_coder.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4916 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/gliding_vertex_coder.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.526031 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/prior_generators/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      242 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/prior_generators/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2821 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/prior_generators/anchor_generator.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.526031 mmrotate_dev-1.0.0rc2/mmrotate/models/utils/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      398 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/utils/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5303 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/utils/enn.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3268 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/utils/misc.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5327 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/utils/orconv.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      691 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/mmrotate/models/utils/ripool.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3637 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/registry.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.526031 mmrotate_dev-1.0.0rc2/mmrotate/structures/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       88 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/structures/__init__.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.527031 mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      628 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3931 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/bbox_overlaps.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3782 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/box_converters.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    14250 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/quadri_boxes.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)    19126 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/rotated_boxes.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     3577 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/transforms.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.527031 mmrotate_dev-1.0.0rc2/mmrotate/testing/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      191 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/testing/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     8215 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/testing/_utils.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.528031 mmrotate_dev-1.0.0rc2/mmrotate/utils/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      395 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/utils/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      486 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/utils/collect_env.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1073 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/utils/misc.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.528031 mmrotate_dev-1.0.0rc2/mmrotate/utils/patch/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      226 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/utils/patch/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     4356 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/utils/patch/merge_results.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     2931 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/utils/patch/split.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1874 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/utils/setup_env.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      337 2024-04-17 02:27:11.000000 mmrotate_dev-1.0.0rc2/mmrotate/version.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.528031 mmrotate_dev-1.0.0rc2/mmrotate/visualization/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      179 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/visualization/__init__.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     5837 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/visualization/local_visualizer.py
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     1720 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/mmrotate/visualization/palette.py
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.529031 mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/
+-rw-r--r--   0 xuchenjie  (1004) xuchenjie  (1004)    18090 2024-04-17 02:30:51.000000 mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)    15662 2024-04-17 02:30:51.000000 mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)        1 2024-04-17 02:30:51.000000 mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)        1 2024-04-15 17:53:56.000000 mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/not-zip-safe
+-rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)      594 2024-04-17 02:30:51.000000 mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/requires.txt
+-rw-rw-r--   0 xuchenjie  (1004) xuchenjie  (1004)        9 2024-04-17 02:30:51.000000 mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/top_level.txt
+drwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)        0 2024-04-17 02:30:51.529031 mmrotate_dev-1.0.0rc2/requirements/
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       64 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/requirements/build.txt
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      195 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/requirements/docs.txt
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       62 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/requirements/mminstall.txt
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       36 2024-04-13 14:16:36.000000 mmrotate_dev-1.0.0rc2/requirements/optional.txt
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       71 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/requirements/readthedocs.txt
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)       54 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/requirements/runtime.txt
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      289 2024-04-13 14:16:39.000000 mmrotate_dev-1.0.0rc2/requirements/tests.txt
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)      646 2024-04-17 02:30:51.534031 mmrotate_dev-1.0.0rc2/setup.cfg
+-rwxrwxr-x   0 xuchenjie  (1004) xuchenjie  (1004)     7304 2024-04-15 17:52:35.000000 mmrotate_dev-1.0.0rc2/setup.py
```

### Comparing `mmrotate_dev-1.0.0rc1/LICENSE` & `mmrotate_dev-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/PKG-INFO` & `mmrotate_dev-1.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmrotate_dev
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Rotation Detection Toolbox and Benchmark
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmrotate_dev Version: 1.0.0rc1 Summary: Rotation
+Metadata-Version: 2.1 Name: mmrotate_dev Version: 1.0.0rc2 Summary: Rotation
 Detection Toolbox and Benchmark License: Apache License 2.0 Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `mmrotate_dev-1.0.0rc1/README.md` & `mmrotate_dev-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dior.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dior.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dota_coco.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dota_coco.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dota_ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dota_ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dota_qbox.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dota_qbox.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dotav15.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dotav15.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/dotav2.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/dotav2.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/hrsid.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/hrsid.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/rsdd.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/rsdd.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/srsdd.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/srsdd.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/datasets/ssdd.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/datasets/ssdd.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/default_runtime.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/schedule_1x.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/schedule_1x.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/schedule_3x.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/schedule_3x.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/schedule_40e.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/schedule_40e.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/_base_/schedules/schedule_6x.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/_base_/schedules/schedule_6x.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/cfa/cfa-qbox_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/cfa/cfa-qbox_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/cfa/cfa-qbox_r50_fpn_40e_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/cfa/cfa-qbox_r50_fpn_40e_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/cfa/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/cfa/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/convnext/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/convnext/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/convnext/rotated-retinanet-rbox-le90_convnext-tiny_fpn_kld-stable_adamw-1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/convnext/rotated-retinanet-rbox-le90_convnext-tiny_fpn_kld-stable_adamw-1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/csl/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/csl/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gliding_vertex/gliding-vertex-qbox_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gliding_vertex/gliding-vertex-qbox_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gliding_vertex/gliding-vertex-rbox_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gliding_vertex/gliding-vertex-rbox_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gliding_vertex/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gliding_vertex/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/gwd/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/gwd/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dior/h2rbox-le90_r50_fpn_adamw-1x_dior.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dior/h2rbox-le90_r50_fpn_adamw-1x_dior.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dotav15/h2rbox-le90_r50_fpn_adamw-1x_dotav15.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dotav15/h2rbox-le90_r50_fpn_adamw-1x_dotav15.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/dotav2/h2rbox-le90_r50_fpn_adamw-1x_dotav2.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/dotav2/h2rbox-le90_r50_fpn_adamw-1x_dotav2.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/h2rbox-le90_r50_fpn_adamw-1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/h2rbox-le90_r50_fpn_adamw-1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dotav15.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dotav15.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dotav2.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-1x_dotav2.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-6x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn-6x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn_ms_rr-1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn_ms_rr-1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn_rr-6x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/h2rbox_v2-le90_r50_fpn_rr-6x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/h2rbox_v2/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/h2rbox_v2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/r3det-oc_r50_fpn_kfiou-ln_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/r3det-oc_r50_fpn_kfiou-ln_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/roi-trans-le90_r50_fpn_kfiou-ln_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/roi-trans-le90_r50_fpn_kfiou-ln_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kfiou/s2anet-le135_r50_fpn_kfiou-ln_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kfiou/s2anet-le135_r50_fpn_kfiou-ln_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/r3det-oc_r50_fpn_kld-stable_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/r3det-oc_r50_fpn_kld-stable_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/r3det-oc_r50_fpn_kld_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/r3det-oc_r50_fpn_kld_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/kld/r3det-tiny-oc_r50_fpn_kld_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/kld/r3det-tiny-oc_r50_fpn_kld_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_hrsid.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_hrsid.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_rsdd.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_rsdd.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_srsdd.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_srsdd.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_ssdd.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_r50_fpn_6x_ssdd.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_swin-tiny_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_rcnn/oriented-rcnn-le90_swin-tiny_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_reppoints/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_reppoints/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_reppoints/oriented-reppoints-qbox_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_reppoints/oriented-reppoints-qbox_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/oriented_reppoints/oriented-reppoints-qbox_r50_fpn_mstrain-40e_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/oriented_reppoints/oriented-reppoints-qbox_r50_fpn_mstrain-40e_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/rotated-fcos-hbox-le90_r50_fpn_psc-dual_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/rotated-fcos-hbox-le90_r50_fpn_psc-dual_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/rotated-fcos-hbox-le90_r50_fpn_psc_rr-6x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/rotated-fcos-hbox-le90_r50_fpn_psc_rr-6x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/rotated-retinanet-rbox-le90_r50_fpn_psc-dual_amp-1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/rotated-retinanet-rbox-le90_r50_fpn_psc-dual_amp-1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/psc/rotated-retinanet-rbox-le90_r50_fpn_psc_rr-6x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/psc/rotated-retinanet-rbox-le90_r50_fpn_psc_rr-6x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/r3det-oc_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/r3det-oc_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/r3det-refine-oc_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/r3det-refine-oc_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/r3det/r3det-tiny-oc_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/r3det/r3det-tiny-oc_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_3x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_3x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_rr-1x_dota-ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/redet/redet-le90_re50_refpn_rr-1x_dota-ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le135_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le135_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_1x_dota-ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_1x_dota-ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_rr-1x_dota-ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_r50_fpn_rr-1x_dota-ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-le90_swin-tiny_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-le90_swin-tiny_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/roi_trans/roi-trans-oc_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/roi_trans/roi-trans-oc_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_atss/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_atss/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_atss/rotated-atss-le90_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_atss/rotated-atss-le90_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_faster_rcnn/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_faster_rcnn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_faster_rcnn/rotated-faster-rcnn-le90_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_faster_rcnn/rotated-faster-rcnn-le90_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-hbox-le90_r50_fpn_csl-gaussian_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-hbox-le90_r50_fpn_csl-gaussian_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_rr-6x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_fcos/rotated-fcos-le90_r50_fpn_rr-6x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_reppoints/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_reppoints/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_reppoints/rotated-reppoints-qbox_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_reppoints/rotated-reppoints-qbox_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-le135_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-le135_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-le90_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-le90_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-oc_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-oc_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-oc_r50_fpn_rr-6x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-hbox-oc_r50_fpn_rr-6x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_1x_dior.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_1x_dior.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_rr-1x_dota-ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_rr-1x_dota-ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_rr-6x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_retinanet/rotated-retinanet-rbox-le90_r50_fpn_rr-6x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/default_runtime.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/dota_rr.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/dota_rr.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/dota_rr_ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/dota_rr_ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/hrsc_rr.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/hrsc_rr.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/_base_/schedule_3x.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/_base_/schedule_3x.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-100e-aug-dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-100e-aug-dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-300e-aug-hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-300e-aug-hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-3x-dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-3x-dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-3x-dota_ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-3x-dota_ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-9x-hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-9x-hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-coco_pretrain-3x-dota_ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_l-coco_pretrain-3x-dota_ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_m-3x-dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_m-3x-dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_m-3x-dota_ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_m-3x-dota_ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_s-3x-dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_s-3x-dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_s-3x-dota_ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_s-3x-dota_ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-300e-aug-hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-300e-aug-hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-3x-dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-3x-dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-3x-dota_ms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-3x-dota_ms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-9x-hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/rotated_rtmdet/rotated_rtmdet_tiny-9x-hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/cascade-s2anet-le135_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/cascade-s2anet-le135_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_3x_hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/s2anet-le135_r50_fpn_3x_hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/s2anet/s2anet-le90_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/s2anet/s2anet-le90_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/sasm_reppoints/metafile.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/sasm_reppoints/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/configs/sasm_reppoints/sasm-reppoints-qbox_r50_fpn_1x_dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/configs/sasm_reppoints/sasm-reppoints-qbox_r50_fpn_1x_dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/model-index.yml` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/model-index.yml`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/analyze_logs.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/benchmark.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/benchmark.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/browse_dataset.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/browse_dataset.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/confusion_matrix.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/analysis_tools/get_flops.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/analysis_tools/get_flops.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/data/dota/dota2coco.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/data/dota/dota2coco.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/data/dota/split/img_split.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/data/dota/split/img_split.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/deployment/mmrotate2torchserve.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/deployment/mmrotate2torchserve.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/deployment/mmrotate_handler.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/deployment/mmrotate_handler.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/misc/print_config.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/misc/print_config.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/model_converters/publish_model.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/model_converters/publish_model.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/slurm_test.sh` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/slurm_test.sh`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/slurm_train.sh` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/test.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/test.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/.mim/tools/train.py` & `mmrotate_dev-1.0.0rc2/mmrotate/.mim/tools/train.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/__init__.py` & `mmrotate_dev-1.0.0rc2/mmrotate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 assert (mmengine_version >= digit_version(mmengine_minimum_version)
         and mmengine_version < digit_version(mmengine_maximum_version)), \
     f'MMEngine=={mmengine.__version__} is used but incompatible. ' \
     f'Please install mmengine>={mmengine_minimum_version}, ' \
     f'<{mmengine_maximum_version}.'
 
 mmdet_minimum_version = '3.0.0rc6'
-mmdet_maximum_version = '3.2.0'
+mmdet_maximum_version = '3.4.0'
 mmdet_version = digit_version(mmdet.__version__)
 
 assert (mmdet_version >= digit_version(mmdet_minimum_version)
         and mmdet_version <= digit_version(mmdet_maximum_version)), \
     f'MMDetection {mmdet.__version__} is incompatible ' \
     f'with MMRotate {__version__}. ' \
     f'Please use MMDetection >= {mmdet_minimum_version}, ' \
```

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/apis/inference.py` & `mmrotate_dev-1.0.0rc2/mmrotate/apis/inference.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/datasets/dior.py` & `mmrotate_dev-1.0.0rc2/mmrotate/datasets/dior.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/datasets/dota.py` & `mmrotate_dev-1.0.0rc2/mmrotate/datasets/dota.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/datasets/hrsc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/datasets/hrsc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/datasets/transforms/loading.py` & `mmrotate_dev-1.0.0rc2/mmrotate/datasets/transforms/loading.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/datasets/transforms/transforms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/datasets/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/evaluation/functional/mean_ap.py` & `mmrotate_dev-1.0.0rc2/mmrotate/evaluation/functional/mean_ap.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/evaluation/metrics/dota_metric.py` & `mmrotate_dev-1.0.0rc2/mmrotate/evaluation/metrics/dota_metric.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/evaluation/metrics/rotated_coco_metric.py` & `mmrotate_dev-1.0.0rc2/mmrotate/evaluation/metrics/rotated_coco_metric.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/backbones/re_resnet.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/backbones/re_resnet.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/__init__.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/angle_branch_retina_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/angle_branch_retina_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/cfa_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/cfa_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/h2rbox_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/h2rbox_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/h2rbox_v2_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/h2rbox_v2_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/oriented_reppoints_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/oriented_reppoints_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/oriented_rpn_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/oriented_rpn_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/r3_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/r3_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_atss_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_atss_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_fcos_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_fcos_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_reppoints_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_reppoints_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_retina_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_retina_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/rotated_rtmdet_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/rotated_rtmdet_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/s2a_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/s2a_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/dense_heads/sam_reppoints_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/dense_heads/sam_reppoints_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/detectors/h2rbox.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/detectors/h2rbox.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/detectors/h2rbox_v2.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/detectors/h2rbox_v2.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/detectors/refine_single_stage.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/detectors/refine_single_stage.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/layers/align.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/layers/align.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/__init__.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/convex_giou_loss.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/convex_giou_loss.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/gaussian_dist_loss.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/gaussian_dist_loss.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/gaussian_dist_loss_v1.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/gaussian_dist_loss_v1.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/h2rbox_consistency_loss.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/h2rbox_consistency_loss.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/h2rbox_v2_consistency_loss.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/h2rbox_v2_consistency_loss.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/kf_iou_loss.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/kf_iou_loss.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/rotated_iou_loss.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/rotated_iou_loss.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/smooth_focal_loss.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/smooth_focal_loss.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/losses/spatial_border_loss.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/losses/spatial_border_loss.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/necks/re_fpn.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/necks/re_fpn.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/bbox_heads/convfc_rbbox_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/bbox_heads/convfc_rbbox_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/bbox_heads/gv_bbox_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/bbox_heads/gv_bbox_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/gv_ratio_roi_head.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/gv_ratio_roi_head.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/roi_heads/roi_extractors/rotate_single_level_roi_extractor.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/roi_heads/roi_extractors/rotate_single_level_roi_extractor.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/__init__.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/__init__.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/convex_assigner.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/convex_assigner.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/max_convex_iou_assigner.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/max_convex_iou_assigner.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/rotate_iou2d_calculator.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/rotate_iou2d_calculator.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/rotated_atss_assigner.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/rotated_atss_assigner.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/assigners/sas_assigner.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/assigners/sas_assigner.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/__init__.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/__init__.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/angle_coder.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/angle_coder.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_midpointoffset_rbbox_coder.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_midpointoffset_rbbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_xywh_hbbox_coder.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_xywh_hbbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_xywh_qbbox_coder.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_xywh_qbbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_xywht_hbbox_coder.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_xywht_hbbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/delta_xywht_rbbox_coder.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/delta_xywht_rbbox_coder.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/distance_angle_point_coder.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/distance_angle_point_coder.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/coders/gliding_vertex_coder.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/coders/gliding_vertex_coder.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/task_modules/prior_generators/anchor_generator.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/task_modules/prior_generators/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/utils/enn.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/utils/enn.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/utils/misc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/utils/orconv.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/utils/orconv.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/models/utils/ripool.py` & `mmrotate_dev-1.0.0rc2/mmrotate/models/utils/ripool.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/registry.py` & `mmrotate_dev-1.0.0rc2/mmrotate/registry.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/__init__.py` & `mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/__init__.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/bbox_overlaps.py` & `mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/bbox_overlaps.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/box_converters.py` & `mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/box_converters.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/quadri_boxes.py` & `mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/quadri_boxes.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/rotated_boxes.py` & `mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/structures/bbox/transforms.py` & `mmrotate_dev-1.0.0rc2/mmrotate/structures/bbox/transforms.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/testing/_utils.py` & `mmrotate_dev-1.0.0rc2/mmrotate/testing/_utils.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/utils/misc.py` & `mmrotate_dev-1.0.0rc2/mmrotate/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/utils/patch/merge_results.py` & `mmrotate_dev-1.0.0rc2/mmrotate/utils/patch/merge_results.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/utils/patch/split.py` & `mmrotate_dev-1.0.0rc2/mmrotate/utils/patch/split.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/utils/setup_env.py` & `mmrotate_dev-1.0.0rc2/mmrotate/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/visualization/local_visualizer.py` & `mmrotate_dev-1.0.0rc2/mmrotate/visualization/local_visualizer.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate/visualization/palette.py` & `mmrotate_dev-1.0.0rc2/mmrotate/visualization/palette.py`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/PKG-INFO` & `mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmrotate_dev
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Rotation Detection Toolbox and Benchmark
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmrotate_dev Version: 1.0.0rc1 Summary: Rotation
+Metadata-Version: 2.1 Name: mmrotate_dev Version: 1.0.0rc2 Summary: Rotation
 Detection Toolbox and Benchmark License: Apache License 2.0 Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/SOURCES.txt` & `mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/mmrotate_dev.egg-info/requires.txt` & `mmrotate_dev-1.0.0rc2/mmrotate_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/setup.cfg` & `mmrotate_dev-1.0.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmrotate_dev-1.0.0rc1/setup.py` & `mmrotate_dev-1.0.0rc2/setup.py`

 * *Files identical despite different names*

