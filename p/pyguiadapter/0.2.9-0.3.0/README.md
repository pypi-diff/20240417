# Comparing `tmp/pyguiadapter-0.2.9.tar.gz` & `tmp/pyguiadapter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyguiadapter-0.2.9.tar", max compression
+gzip compressed data, was "pyguiadapter-0.3.0.tar", max compression
```

## Comparing `pyguiadapter-0.2.9.tar` & `pyguiadapter-0.3.0.tar`

### file list

```diff
@@ -1,245 +1,260 @@
--rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 pyguiadapter-0.2.9/License
--rw-r--r--   0        0        0        0 2024-03-17 02:32:55.457540 pyguiadapter-0.2.9/pyguiadapter/__init__.py
--rw-r--r--   0        0        0       53 2024-03-17 02:29:22.426087 pyguiadapter-0.2.9/pyguiadapter/adapter/__init__.py
--rw-r--r--   0        0        0     8327 2024-03-22 15:02:32.806769 pyguiadapter-0.2.9/pyguiadapter/adapter/adapter.py
--rw-r--r--   0        0        0     2840 2024-03-22 15:03:36.779855 pyguiadapter-0.2.9/pyguiadapter/adapter/bundle.py
--rw-r--r--   0        0        0      910 2024-03-17 02:30:34.866408 pyguiadapter-0.2.9/pyguiadapter/adapter/executor.py
--rw-r--r--   0        0        0     1985 2024-03-24 10:04:25.514442 pyguiadapter-0.2.9/pyguiadapter/commons.py
--rw-r--r--   0        0        0      212 2024-03-15 13:59:57.444102 pyguiadapter-0.2.9/pyguiadapter/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-16 03:25:43.591074 pyguiadapter-0.2.9/pyguiadapter/interact/__init__.py
--rw-r--r--   0        0        0     5010 2024-03-21 10:36:00.956016 pyguiadapter-0.2.9/pyguiadapter/interact/ulogging.py
--rw-r--r--   0        0        0    12531 2024-03-22 15:12:24.013998 pyguiadapter-0.2.9/pyguiadapter/interact/upopup.py
--rw-r--r--   0        0        0      793 2024-03-19 13:00:20.549109 pyguiadapter-0.2.9/pyguiadapter/interact/uprint.py
--rw-r--r--   0        0        0      753 2024-03-09 14:42:49.269579 pyguiadapter-0.2.9/pyguiadapter/res/icons/abnormal.svg
--rw-r--r--   0        0        0      563 2024-03-09 14:42:49.301675 pyguiadapter-0.2.9/pyguiadapter/res/icons/acoustic.svg
--rw-r--r--   0        0        0      437 2024-03-09 14:42:49.334414 pyguiadapter-0.2.9/pyguiadapter/res/icons/activity-source.svg
--rw-r--r--   0        0        0      721 2024-03-09 14:42:49.367533 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-computer.svg
--rw-r--r--   0        0        0     1074 2024-03-09 14:42:49.400158 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-picture.svg
--rw-r--r--   0        0        0      556 2024-03-09 14:42:49.432714 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-print.svg
--rw-r--r--   0        0        0      611 2024-03-09 14:42:49.462803 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-user.svg
--rw-r--r--   0        0        0      820 2024-03-09 14:42:49.493344 pyguiadapter-0.2.9/pyguiadapter/res/icons/add-web.svg
--rw-r--r--   0        0        0      444 2024-03-09 14:42:49.525909 pyguiadapter-0.2.9/pyguiadapter/res/icons/airplay.svg
--rw-r--r--   0        0        0      744 2024-03-09 14:42:49.557957 pyguiadapter-0.2.9/pyguiadapter/res/icons/api-app.svg
--rw-r--r--   0        0        0      915 2024-03-09 14:42:49.595156 pyguiadapter-0.2.9/pyguiadapter/res/icons/application-effect.svg
--rw-r--r--   0        0        0      513 2024-03-09 14:42:49.627840 pyguiadapter-0.2.9/pyguiadapter/res/icons/application-one.svg
--rw-r--r--   0        0        0      471 2024-03-09 14:42:49.662047 pyguiadapter-0.2.9/pyguiadapter/res/icons/application-two.svg
--rw-r--r--   0        0        0      444 2024-03-09 14:42:49.695595 pyguiadapter-0.2.9/pyguiadapter/res/icons/area-map.svg
--rw-r--r--   0        0        0     1704 2024-03-09 14:42:49.730658 pyguiadapter-0.2.9/pyguiadapter/res/icons/arithmetic-buttons.svg
--rw-r--r--   0        0        0      886 2024-03-09 14:42:49.763713 pyguiadapter-0.2.9/pyguiadapter/res/icons/arithmetic-one.svg
--rw-r--r--   0        0        0     1051 2024-03-09 14:42:49.803740 pyguiadapter-0.2.9/pyguiadapter/res/icons/arrow-keys.svg
--rw-r--r--   0        0        0      510 2024-03-09 14:42:49.839218 pyguiadapter-0.2.9/pyguiadapter/res/icons/audio-file.svg
--rw-r--r--   0        0        0      806 2024-03-09 14:42:49.874542 pyguiadapter-0.2.9/pyguiadapter/res/icons/audit.svg
--rw-r--r--   0        0        0      503 2024-03-09 14:42:49.912111 pyguiadapter-0.2.9/pyguiadapter/res/icons/average.svg
--rw-r--r--   0        0        0      871 2024-03-09 14:42:49.953498 pyguiadapter-0.2.9/pyguiadapter/res/icons/bitcoin.svg
--rw-r--r--   0        0        0      753 2024-03-09 14:42:50.007926 pyguiadapter-0.2.9/pyguiadapter/res/icons/blackboard.svg
--rw-r--r--   0        0        0      633 2024-03-09 14:42:50.054525 pyguiadapter-0.2.9/pyguiadapter/res/icons/blocks-and-arrows.svg
--rw-r--r--   0        0        0      261 2024-03-09 14:42:50.096249 pyguiadapter-0.2.9/pyguiadapter/res/icons/bluetooth.svg
--rw-r--r--   0        0        0      794 2024-03-09 14:42:50.134304 pyguiadapter-0.2.9/pyguiadapter/res/icons/bookmark-three.svg
--rw-r--r--   0        0        0      981 2024-03-09 14:42:50.168174 pyguiadapter-0.2.9/pyguiadapter/res/icons/broadcast.svg
--rw-r--r--   0        0        0      993 2024-03-09 14:42:50.199705 pyguiadapter-0.2.9/pyguiadapter/res/icons/browser.svg
--rw-r--r--   0        0        0     1399 2024-03-09 14:42:50.232340 pyguiadapter-0.2.9/pyguiadapter/res/icons/bug.svg
--rw-r--r--   0        0        0      978 2024-03-09 14:42:50.265457 pyguiadapter-0.2.9/pyguiadapter/res/icons/bytedance-mini-app.svg
--rw-r--r--   0        0        0      334 2024-03-09 14:42:50.311121 pyguiadapter-0.2.9/pyguiadapter/res/icons/card-two.svg
--rw-r--r--   0        0        0      643 2024-03-09 14:42:50.383849 pyguiadapter-0.2.9/pyguiadapter/res/icons/carousel-video.svg
--rw-r--r--   0        0        0      849 2024-03-09 14:42:50.350168 pyguiadapter-0.2.9/pyguiadapter/res/icons/carousel.svg
--rw-r--r--   0        0        0      685 2024-03-09 14:42:50.414066 pyguiadapter-0.2.9/pyguiadapter/res/icons/cast-screen.svg
--rw-r--r--   0        0        0      472 2024-03-09 14:42:50.447609 pyguiadapter-0.2.9/pyguiadapter/res/icons/category-management.svg
--rw-r--r--   0        0        0      443 2024-03-09 14:42:50.478933 pyguiadapter-0.2.9/pyguiadapter/res/icons/caution.svg
--rw-r--r--   0        0        0     1016 2024-03-09 14:42:50.509609 pyguiadapter-0.2.9/pyguiadapter/res/icons/certificate.svg
--rw-r--r--   0        0        0      634 2024-03-09 14:42:50.540729 pyguiadapter-0.2.9/pyguiadapter/res/icons/check-one.svg
--rw-r--r--   0        0        0      697 2024-03-09 14:42:50.572289 pyguiadapter-0.2.9/pyguiadapter/res/icons/checklist.svg
--rw-r--r--   0        0        0     1023 2024-03-09 14:42:50.603351 pyguiadapter-0.2.9/pyguiadapter/res/icons/chip.svg
--rw-r--r--   0        0        0      519 2024-03-09 14:42:50.635463 pyguiadapter-0.2.9/pyguiadapter/res/icons/classroom.svg
--rw-r--r--   0        0        0      478 2024-03-09 14:42:50.667994 pyguiadapter-0.2.9/pyguiadapter/res/icons/clipboard.svg
--rw-r--r--   0        0        0      576 2024-03-09 14:42:50.700513 pyguiadapter-0.2.9/pyguiadapter/res/icons/close-one.svg
--rw-r--r--   0        0        0     1211 2024-03-09 14:42:50.732035 pyguiadapter-0.2.9/pyguiadapter/res/icons/cloud-storage.svg
--rw-r--r--   0        0        0      536 2024-03-09 14:42:50.795255 pyguiadapter-0.2.9/pyguiadapter/res/icons/code-brackets.svg
--rw-r--r--   0        0        0      547 2024-03-09 14:42:50.826965 pyguiadapter-0.2.9/pyguiadapter/res/icons/code-download.svg
--rw-r--r--   0        0        0      639 2024-03-09 14:42:50.860630 pyguiadapter-0.2.9/pyguiadapter/res/icons/code-laptop.svg
--rw-r--r--   0        0        0      346 2024-03-09 14:42:50.893306 pyguiadapter-0.2.9/pyguiadapter/res/icons/code-one.svg
--rw-r--r--   0        0        0      441 2024-03-09 14:42:50.764191 pyguiadapter-0.2.9/pyguiadapter/res/icons/code.svg
--rw-r--r--   0        0        0      831 2024-03-09 14:42:50.925357 pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-computer.svg
--rw-r--r--   0        0        0      732 2024-03-09 14:42:50.958885 pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-laptop.svg
--rw-r--r--   0        0        0     1181 2024-03-09 14:42:50.991576 pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-picture.svg
--rw-r--r--   0        0        0     1118 2024-03-09 14:42:51.022102 pyguiadapter-0.2.9/pyguiadapter/res/icons/color-card.svg
--rw-r--r--   0        0        0     1289 2024-03-09 14:42:51.052795 pyguiadapter-0.2.9/pyguiadapter/res/icons/command.svg
--rw-r--r--   0        0        0      371 2024-03-09 14:42:51.119127 pyguiadapter-0.2.9/pyguiadapter/res/icons/comment-one.svg
--rw-r--r--   0        0        0      581 2024-03-09 14:42:51.085912 pyguiadapter-0.2.9/pyguiadapter/res/icons/comment.svg
--rw-r--r--   0        0        0      553 2024-03-09 14:42:51.153360 pyguiadapter-0.2.9/pyguiadapter/res/icons/comments.svg
--rw-r--r--   0        0        0      628 2024-03-09 14:42:51.186924 pyguiadapter-0.2.9/pyguiadapter/res/icons/communication.svg
--rw-r--r--   0        0        0      753 2024-03-09 14:42:51.219995 pyguiadapter-0.2.9/pyguiadapter/res/icons/compass.svg
--rw-r--r--   0        0        0     1110 2024-03-09 14:42:51.250504 pyguiadapter-0.2.9/pyguiadapter/res/icons/compression.svg
--rw-r--r--   0        0        0      556 2024-03-09 14:42:51.284109 pyguiadapter-0.2.9/pyguiadapter/res/icons/computer.svg
--rw-r--r--   0        0        0      447 2024-03-09 14:42:51.317638 pyguiadapter-0.2.9/pyguiadapter/res/icons/cones.svg
--rw-r--r--   0        0        0     1850 2024-03-09 14:42:51.350759 pyguiadapter-0.2.9/pyguiadapter/res/icons/connect.svg
--rw-r--r--   0        0        0      620 2024-03-09 14:42:51.382155 pyguiadapter-0.2.9/pyguiadapter/res/icons/copy-one.svg
--rw-r--r--   0        0        0      524 2024-03-09 14:42:51.414093 pyguiadapter-0.2.9/pyguiadapter/res/icons/copyright.svg
--rw-r--r--   0        0        0     2644 2024-03-09 14:42:51.445689 pyguiadapter-0.2.9/pyguiadapter/res/icons/cpu.svg
--rw-r--r--   0        0        0      516 2024-03-09 14:42:51.477786 pyguiadapter-0.2.9/pyguiadapter/res/icons/cross-ring-two.svg
--rw-r--r--   0        0        0      895 2024-03-09 14:42:51.510328 pyguiadapter-0.2.9/pyguiadapter/res/icons/cube-four.svg
--rw-r--r--   0        0        0      369 2024-03-09 14:42:51.543870 pyguiadapter-0.2.9/pyguiadapter/res/icons/curve-adjustment.svg
--rw-r--r--   0        0        0     1177 2024-03-09 14:42:51.576599 pyguiadapter-0.2.9/pyguiadapter/res/icons/cuvette.svg
--rw-r--r--   0        0        0     1199 2024-03-09 14:42:51.608710 pyguiadapter-0.2.9/pyguiadapter/res/icons/dashboard-one.svg
--rw-r--r--   0        0        0     1332 2024-03-09 14:42:51.643261 pyguiadapter-0.2.9/pyguiadapter/res/icons/dashboard-two.svg
--rw-r--r--   0        0        0     1221 2024-03-09 14:42:51.709446 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-all.svg
--rw-r--r--   0        0        0     1239 2024-03-09 14:42:51.742529 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-display.svg
--rw-r--r--   0        0        0     1255 2024-03-09 14:42:51.777672 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-lock.svg
--rw-r--r--   0        0        0      829 2024-03-09 14:42:51.813216 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-screen.svg
--rw-r--r--   0        0        0      833 2024-03-09 14:42:51.846297 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-server.svg
--rw-r--r--   0        0        0     1448 2024-03-09 14:42:51.879954 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-switching.svg
--rw-r--r--   0        0        0     1209 2024-03-09 14:42:51.911088 pyguiadapter-0.2.9/pyguiadapter/res/icons/data-user.svg
--rw-r--r--   0        0        0      794 2024-03-09 14:42:51.675906 pyguiadapter-0.2.9/pyguiadapter/res/icons/data.svg
--rw-r--r--   0        0        0     1588 2024-03-09 14:42:51.944604 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-alert.svg
--rw-r--r--   0        0        0     1606 2024-03-09 14:42:51.977363 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-code.svg
--rw-r--r--   0        0        0     1596 2024-03-09 14:42:52.007892 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-config.svg
--rw-r--r--   0        0        0     1513 2024-03-09 14:42:52.040009 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-download.svg
--rw-r--r--   0        0        0     1516 2024-03-09 14:42:52.074200 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-enter.svg
--rw-r--r--   0        0        0     1528 2024-03-09 14:42:52.106242 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-fail.svg
--rw-r--r--   0        0        0     1513 2024-03-09 14:42:52.137391 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-first.svg
--rw-r--r--   0        0        0     1492 2024-03-09 14:42:52.170998 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-forbid.svg
--rw-r--r--   0        0        0     1738 2024-03-09 14:42:52.201569 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-lock.svg
--rw-r--r--   0        0        0     1195 2024-03-09 14:42:52.268001 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-network-point.svg
--rw-r--r--   0        0        0     1770 2024-03-09 14:42:52.234122 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-network.svg
--rw-r--r--   0        0        0     1637 2024-03-09 14:42:52.300547 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-point.svg
--rw-r--r--   0        0        0     1390 2024-03-09 14:42:52.333068 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-position.svg
--rw-r--r--   0        0        0     1504 2024-03-09 14:42:52.364241 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-power.svg
--rw-r--r--   0        0        0     1528 2024-03-09 14:42:52.397951 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-proportion.svg
--rw-r--r--   0        0        0     1908 2024-03-09 14:42:52.428304 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-search.svg
--rw-r--r--   0        0        0     1542 2024-03-09 14:42:52.460505 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-setting.svg
--rw-r--r--   0        0        0     1504 2024-03-09 14:42:52.494171 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-success.svg
--rw-r--r--   0        0        0     1638 2024-03-09 14:42:52.525731 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-sync.svg
--rw-r--r--   0        0        0     1492 2024-03-09 14:42:52.559018 pyguiadapter-0.2.9/pyguiadapter/res/icons/database-time.svg
--rw-r--r--   0        0        0      762 2024-03-09 14:42:52.591111 pyguiadapter-0.2.9/pyguiadapter/res/icons/date-comes-back.svg
--rw-r--r--   0        0        0      470 2024-03-09 14:42:52.624367 pyguiadapter-0.2.9/pyguiadapter/res/icons/diamond-one.svg
--rw-r--r--   0        0        0      470 2024-03-09 14:42:52.657545 pyguiadapter-0.2.9/pyguiadapter/res/icons/diamond-three.svg
--rw-r--r--   0        0        0      466 2024-03-09 14:42:52.689586 pyguiadapter-0.2.9/pyguiadapter/res/icons/diamond-two.svg
--rw-r--r--   0        0        0      855 2024-03-09 14:42:52.754775 pyguiadapter-0.2.9/pyguiadapter/res/icons/disk-one.svg
--rw-r--r--   0        0        0      533 2024-03-09 14:42:52.788667 pyguiadapter-0.2.9/pyguiadapter/res/icons/disk-two.svg
--rw-r--r--   0        0        0      599 2024-03-09 14:42:52.722118 pyguiadapter-0.2.9/pyguiadapter/res/icons/disk.svg
--rw-r--r--   0        0        0      646 2024-03-09 14:42:52.821412 pyguiadapter-0.2.9/pyguiadapter/res/icons/document-folder.svg
--rw-r--r--   0        0        0      957 2024-03-09 14:42:52.852474 pyguiadapter-0.2.9/pyguiadapter/res/icons/download-one.svg
--rw-r--r--   0        0        0      649 2024-03-09 14:42:52.884528 pyguiadapter-0.2.9/pyguiadapter/res/icons/download-three.svg
--rw-r--r--   0        0        0      730 2024-03-09 14:42:52.917857 pyguiadapter-0.2.9/pyguiadapter/res/icons/download-two.svg
--rw-r--r--   0        0        0      827 2024-03-09 14:42:52.952370 pyguiadapter-0.2.9/pyguiadapter/res/icons/download-web.svg
--rw-r--r--   0        0        0      500 2024-03-09 14:42:52.983983 pyguiadapter-0.2.9/pyguiadapter/res/icons/electrocardiogram.svg
--rw-r--r--   0        0        0      568 2024-03-09 14:42:53.017497 pyguiadapter-0.2.9/pyguiadapter/res/icons/email-down.svg
--rw-r--r--   0        0        0      567 2024-03-09 14:42:53.052087 pyguiadapter-0.2.9/pyguiadapter/res/icons/email-push.svg
--rw-r--r--   0        0        0      634 2024-03-09 14:42:53.117840 pyguiadapter-0.2.9/pyguiadapter/res/icons/experiment-one.svg
--rw-r--r--   0        0        0      731 2024-03-09 14:42:53.084199 pyguiadapter-0.2.9/pyguiadapter/res/icons/experiment.svg
--rw-r--r--   0        0        0      680 2024-03-09 14:42:53.152428 pyguiadapter-0.2.9/pyguiadapter/res/icons/figma-component.svg
--rw-r--r--   0        0        0      652 2024-03-09 14:42:53.185744 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-addition.svg
--rw-r--r--   0        0        0      664 2024-03-09 14:42:53.217973 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-code.svg
--rw-r--r--   0        0        0      856 2024-03-09 14:42:53.249496 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-conversion.svg
--rw-r--r--   0        0        0      772 2024-03-09 14:42:53.281733 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-display.svg
--rw-r--r--   0        0        0     1316 2024-03-09 14:42:53.313837 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-pdf-one.svg
--rw-r--r--   0        0        0     1381 2024-03-09 14:42:53.347168 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-ppt.svg
--rw-r--r--   0        0        0      658 2024-03-09 14:42:53.382365 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-protection.svg
--rw-r--r--   0        0        0      652 2024-03-09 14:42:53.417579 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-text.svg
--rw-r--r--   0        0        0      468 2024-03-09 14:42:53.455122 pyguiadapter-0.2.9/pyguiadapter/res/icons/file-word.svg
--rw-r--r--   0        0        0      931 2024-03-09 14:42:53.486147 pyguiadapter-0.2.9/pyguiadapter/res/icons/film.svg
--rw-r--r--   0        0        0      734 2024-03-09 14:42:53.517258 pyguiadapter-0.2.9/pyguiadapter/res/icons/flask.svg
--rw-r--r--   0        0        0      851 2024-03-09 14:42:53.549857 pyguiadapter-0.2.9/pyguiadapter/res/icons/game-handle.svg
--rw-r--r--   0        0        0      989 2024-03-09 14:42:53.581226 pyguiadapter-0.2.9/pyguiadapter/res/icons/help.svg
--rw-r--r--   0        0        0      545 2024-03-09 14:42:53.612330 pyguiadapter-0.2.9/pyguiadapter/res/icons/hexagon-one.svg
--rw-r--r--   0        0        0      794 2024-03-09 14:42:53.643884 pyguiadapter-0.2.9/pyguiadapter/res/icons/id-card-h.svg
--rw-r--r--   0        0        0      935 2024-03-09 14:42:53.676625 pyguiadapter-0.2.9/pyguiadapter/res/icons/info.svg
--rw-r--r--   0        0        0      696 2024-03-09 14:42:53.708204 pyguiadapter-0.2.9/pyguiadapter/res/icons/install.svg
--rw-r--r--   0        0        0    11551 2024-03-17 02:22:55.741177 pyguiadapter-0.2.9/pyguiadapter/res/icons/LICENSE.txt
--rw-r--r--   0        0        0      683 2024-03-09 14:42:53.741316 pyguiadapter-0.2.9/pyguiadapter/res/icons/many-to-many.svg
--rw-r--r--   0        0        0      602 2024-03-09 14:42:53.805746 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-emoji.svg
--rw-r--r--   0        0        0      522 2024-03-09 14:42:53.840353 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-one.svg
--rw-r--r--   0        0        0      763 2024-03-09 14:42:53.871762 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-privacy.svg
--rw-r--r--   0        0        0      648 2024-03-09 14:42:53.905271 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-search.svg
--rw-r--r--   0        0        0      679 2024-03-09 14:42:53.935786 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-security.svg
--rw-r--r--   0        0        0      485 2024-03-09 14:42:53.970910 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-sent.svg
--rw-r--r--   0        0        0      577 2024-03-09 14:42:54.004586 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-success.svg
--rw-r--r--   0        0        0      550 2024-03-09 14:42:54.037266 pyguiadapter-0.2.9/pyguiadapter/res/icons/message-unread.svg
--rw-r--r--   0        0        0      738 2024-03-09 14:42:53.773734 pyguiadapter-0.2.9/pyguiadapter/res/icons/message.svg
--rw-r--r--   0        0        0      537 2024-03-09 14:42:54.071502 pyguiadapter-0.2.9/pyguiadapter/res/icons/mini-sd-card.svg
--rw-r--r--   0        0        0      521 2024-03-09 14:42:54.103643 pyguiadapter-0.2.9/pyguiadapter/res/icons/monitor.svg
--rw-r--r--   0        0        0     1053 2024-03-09 14:42:54.135574 pyguiadapter-0.2.9/pyguiadapter/res/icons/more-app.svg
--rw-r--r--   0        0        0      971 2024-03-09 14:42:54.204781 pyguiadapter-0.2.9/pyguiadapter/res/icons/movie-board.svg
--rw-r--r--   0        0        0     1213 2024-03-09 14:42:54.169203 pyguiadapter-0.2.9/pyguiadapter/res/icons/movie.svg
--rw-r--r--   0        0        0      995 2024-03-09 14:42:54.236957 pyguiadapter-0.2.9/pyguiadapter/res/icons/multi-function-knife.svg
--rw-r--r--   0        0        0      835 2024-03-09 14:42:54.270059 pyguiadapter-0.2.9/pyguiadapter/res/icons/notebook-one.svg
--rw-r--r--   0        0        0      626 2024-03-09 14:42:54.305013 pyguiadapter-0.2.9/pyguiadapter/res/icons/octagon.svg
--rw-r--r--   0        0        0      575 2024-03-09 14:42:54.338102 pyguiadapter-0.2.9/pyguiadapter/res/icons/online-meeting.svg
--rw-r--r--   0        0        0      227 2024-03-09 14:42:54.370839 pyguiadapter-0.2.9/pyguiadapter/res/icons/oval-one.svg
--rw-r--r--   0        0        0      537 2024-03-09 14:42:54.440082 pyguiadapter-0.2.9/pyguiadapter/res/icons/page-template.svg
--rw-r--r--   0        0        0      440 2024-03-09 14:42:54.403964 pyguiadapter-0.2.9/pyguiadapter/res/icons/page.svg
--rw-r--r--   0        0        0      412 2024-03-09 14:42:54.473151 pyguiadapter-0.2.9/pyguiadapter/res/icons/parallelogram.svg
--rw-r--r--   0        0        0      633 2024-03-09 14:42:54.508004 pyguiadapter-0.2.9/pyguiadapter/res/icons/pay-code.svg
--rw-r--r--   0        0        0      509 2024-03-09 14:42:54.540081 pyguiadapter-0.2.9/pyguiadapter/res/icons/pentagon-one.svg
--rw-r--r--   0        0        0      980 2024-03-09 14:42:54.573293 pyguiadapter-0.2.9/pyguiadapter/res/icons/people-plus-one.svg
--rw-r--r--   0        0        0     1040 2024-03-09 14:42:54.640249 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-incoming-one.svg
--rw-r--r--   0        0        0     1029 2024-03-09 14:42:54.606929 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-incoming.svg
--rw-r--r--   0        0        0     1083 2024-03-09 14:42:54.672454 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-missed.svg
--rw-r--r--   0        0        0     1015 2024-03-09 14:42:54.735192 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-outgoing-one.svg
--rw-r--r--   0        0        0     1008 2024-03-09 14:42:54.704958 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-outgoing.svg
--rw-r--r--   0        0        0      811 2024-03-09 14:42:54.769268 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-telephone.svg
--rw-r--r--   0        0        0      935 2024-03-09 14:42:54.800614 pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-video-call.svg
--rw-r--r--   0        0        0      974 2024-03-09 14:42:54.832344 pyguiadapter-0.2.9/pyguiadapter/res/icons/platte.svg
--rw-r--r--   0        0        0      473 2024-03-09 14:42:54.868011 pyguiadapter-0.2.9/pyguiadapter/res/icons/play.svg
--rw-r--r--   0        0        0      434 2024-03-09 14:42:54.900949 pyguiadapter-0.2.9/pyguiadapter/res/icons/powerpoint.svg
--rw-r--r--   0        0        0      612 2024-03-09 14:42:54.933463 pyguiadapter-0.2.9/pyguiadapter/res/icons/ppt.svg
--rw-r--r--   0        0        0      427 2024-03-09 14:42:54.965026 pyguiadapter-0.2.9/pyguiadapter/res/icons/puzzle.svg
--rw-r--r--   0        0        0      364 2024-03-09 14:42:54.997189 pyguiadapter-0.2.9/pyguiadapter/res/icons/quadrilateral.svg
--rw-r--r--   0        0        0      783 2024-03-09 14:42:55.060859 pyguiadapter-0.2.9/pyguiadapter/res/icons/record-disc.svg
--rw-r--r--   0        0        0      880 2024-03-09 14:42:55.028755 pyguiadapter-0.2.9/pyguiadapter/res/icons/record.svg
--rw-r--r--   0        0        0      319 2024-03-09 14:42:55.123563 pyguiadapter-0.2.9/pyguiadapter/res/icons/rectangle-one.svg
--rw-r--r--   0        0        0      328 2024-03-09 14:42:55.156079 pyguiadapter-0.2.9/pyguiadapter/res/icons/rectangle-small.svg
--rw-r--r--   0        0        0      319 2024-03-09 14:42:55.092477 pyguiadapter-0.2.9/pyguiadapter/res/icons/rectangle.svg
--rw-r--r--   0        0        0      591 2024-03-09 16:01:09.963050 pyguiadapter-0.2.9/pyguiadapter/res/icons/rename.py
--rw-r--r--   0        0        0      425 2024-03-09 14:42:55.187919 pyguiadapter-0.2.9/pyguiadapter/res/icons/right-angle.svg
--rw-r--r--   0        0        0      217 2024-03-09 14:42:55.218332 pyguiadapter-0.2.9/pyguiadapter/res/icons/round.svg
--rw-r--r--   0        0        0      901 2024-03-09 14:42:55.250585 pyguiadapter-0.2.9/pyguiadapter/res/icons/rule-two.svg
--rw-r--r--   0        0        0      794 2024-03-09 14:42:55.314442 pyguiadapter-0.2.9/pyguiadapter/res/icons/ruler-one.svg
--rw-r--r--   0        0        0      926 2024-03-09 14:42:55.282289 pyguiadapter-0.2.9/pyguiadapter/res/icons/ruler.svg
--rw-r--r--   0        0        0      583 2024-03-09 14:42:55.344890 pyguiadapter-0.2.9/pyguiadapter/res/icons/sd-card.svg
--rw-r--r--   0        0        0     1259 2024-03-09 14:42:55.377061 pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-computer.svg
--rw-r--r--   0        0        0     1148 2024-03-09 14:42:55.409597 pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-laptop.svg
--rw-r--r--   0        0        0     1443 2024-03-09 14:42:55.444676 pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-two.svg
--rw-r--r--   0        0        0      980 2024-03-09 14:42:55.477262 pyguiadapter-0.2.9/pyguiadapter/res/icons/share-one.svg
--rw-r--r--   0        0        0      328 2024-03-09 14:42:55.541521 pyguiadapter-0.2.9/pyguiadapter/res/icons/square-small.svg
--rw-r--r--   0        0        0      317 2024-03-09 14:42:55.509301 pyguiadapter-0.2.9/pyguiadapter/res/icons/square.svg
--rw-r--r--   0        0        0      954 2024-03-09 14:42:55.574211 pyguiadapter-0.2.9/pyguiadapter/res/icons/system.svg
--rw-r--r--   0        0        0      895 2024-03-09 14:42:55.606324 pyguiadapter-0.2.9/pyguiadapter/res/icons/table-file.svg
--rw-r--r--   0        0        0     1216 2024-03-09 14:42:55.637907 pyguiadapter-0.2.9/pyguiadapter/res/icons/tape.svg
--rw-r--r--   0        0        0      465 2024-03-09 14:42:55.669026 pyguiadapter-0.2.9/pyguiadapter/res/icons/terminal.svg
--rw-r--r--   0        0        0      751 2024-03-09 14:42:55.704103 pyguiadapter-0.2.9/pyguiadapter/res/icons/test-tube.svg
--rw-r--r--   0        0        0      724 2024-03-09 14:42:55.736266 pyguiadapter-0.2.9/pyguiadapter/res/icons/thermometer.svg
--rw-r--r--   0        0        0      425 2024-03-09 14:42:55.768900 pyguiadapter-0.2.9/pyguiadapter/res/icons/tips-one.svg
--rw-r--r--   0        0        0      510 2024-03-09 14:42:55.800445 pyguiadapter-0.2.9/pyguiadapter/res/icons/tool.svg
--rw-r--r--   0        0        0      587 2024-03-09 14:42:55.867211 pyguiadapter-0.2.9/pyguiadapter/res/icons/topic-discussion.svg
--rw-r--r--   0        0        0     1027 2024-03-09 14:42:55.835066 pyguiadapter-0.2.9/pyguiadapter/res/icons/topic.svg
--rw-r--r--   0        0        0      413 2024-03-09 14:42:55.900240 pyguiadapter-0.2.9/pyguiadapter/res/icons/trapezoid.svg
--rw-r--r--   0        0        0      831 2024-03-09 14:42:55.935077 pyguiadapter-0.2.9/pyguiadapter/res/icons/tree-list.svg
--rw-r--r--   0        0        0     1970 2024-03-09 14:42:55.998698 pyguiadapter-0.2.9/pyguiadapter/res/icons/triangle-ruler.svg
--rw-r--r--   0        0        0      468 2024-03-09 14:42:55.966416 pyguiadapter-0.2.9/pyguiadapter/res/icons/triangle.svg
--rw-r--r--   0        0        0      717 2024-03-09 14:42:56.029033 pyguiadapter-0.2.9/pyguiadapter/res/icons/vial.svg
--rw-r--r--   0        0        0     1823 2024-03-09 14:42:56.061697 pyguiadapter-0.2.9/pyguiadapter/res/icons/video.svg
--rw-r--r--   0        0        0      706 2024-03-09 14:42:56.093308 pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-card.svg
--rw-r--r--   0        0        0      775 2024-03-09 14:42:56.123098 pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-detail.svg
--rw-r--r--   0        0        0      887 2024-03-09 14:42:56.156703 pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-list.svg
--rw-r--r--   0        0        0      642 2024-03-09 14:42:56.218845 pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-input.svg
--rw-r--r--   0        0        0      903 2024-03-09 14:42:56.251446 pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-message.svg
--rw-r--r--   0        0        0      685 2024-03-09 14:42:56.284535 pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-one.svg
--rw-r--r--   0        0        0      508 2024-03-09 14:42:56.187304 pyguiadapter-0.2.9/pyguiadapter/res/icons/voice.svg
--rw-r--r--   0        0        0     1173 2024-03-09 14:42:56.317102 pyguiadapter-0.2.9/pyguiadapter/res/icons/weixin-mini-app.svg
--rw-r--r--   0        0        0      809 2024-03-09 14:42:56.349946 pyguiadapter-0.2.9/pyguiadapter/res/icons/wifi.svg
--rw-r--r--   0        0        0      976 2024-03-09 14:42:56.381588 pyguiadapter-0.2.9/pyguiadapter/res/icons/zip.svg
--rw-r--r--   0        0        0        0 2024-03-15 05:08:37.625966 pyguiadapter-0.2.9/pyguiadapter/ui/__init__.py
--rw-r--r--   0        0        0     1462 2024-03-22 14:55:24.908558 pyguiadapter-0.2.9/pyguiadapter/ui/config.py
--rw-r--r--   0        0        0        0 2024-03-15 11:37:47.907987 pyguiadapter-0.2.9/pyguiadapter/ui/generated/__init__.py
--rw-r--r--   0        0        0     6996 2024-03-22 12:51:51.481008 pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_execution_window.py
--rw-r--r--   0        0        0     2844 2024-03-22 12:51:51.656489 pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_initialization_window.py
--rw-r--r--   0        0        0     4413 2024-03-22 12:51:51.830703 pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_selection_window.py
--rw-r--r--   0        0        0     1460 2024-03-19 13:11:31.754220 pyguiadapter-0.2.9/pyguiadapter/ui/styles.py
--rw-r--r--   0        0        0     1109 2024-03-19 13:11:19.291844 pyguiadapter-0.2.9/pyguiadapter/ui/utils.py
--rw-r--r--   0        0        0        0 2024-03-15 12:09:31.827626 pyguiadapter-0.2.9/pyguiadapter/ui/window/__init__.py
--rw-r--r--   0        0        0    17385 2024-03-25 16:57:48.958090 pyguiadapter-0.2.9/pyguiadapter/ui/window/execution.py
--rw-r--r--   0        0        0     6185 2024-03-22 14:58:04.952081 pyguiadapter-0.2.9/pyguiadapter/ui/window/initialization.py
--rw-r--r--   0        0        0     8273 2024-03-22 14:56:06.155478 pyguiadapter-0.2.9/pyguiadapter/ui/window/selection.py
--rw-r--r--   0        0        0      688 2024-03-26 15:38:08.448955 pyguiadapter-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     8610 2024-03-24 02:40:52.393460 pyguiadapter-0.2.9/README.md
--rw-r--r--   0        0        0     9140 1970-01-01 00:00:00.000000 pyguiadapter-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-14 16:11:23.455323 pyguiadapter-0.3.0/License
+-rw-r--r--   0        0        0      108 2024-04-17 16:38:11.248187 pyguiadapter-0.3.0/pyguiadapter/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-17 15:57:53.099012 pyguiadapter-0.3.0/pyguiadapter/adapter/__init__.py
+-rw-r--r--   0        0        0     9710 2024-04-17 16:28:00.062087 pyguiadapter-0.3.0/pyguiadapter/adapter/adapter.py
+-rw-r--r--   0        0        0     5096 2024-04-17 16:22:01.436361 pyguiadapter-0.3.0/pyguiadapter/adapter/bundle.py
+-rw-r--r--   0        0        0      198 2024-04-17 15:43:54.841916 pyguiadapter-0.3.0/pyguiadapter/adapter/constants.py
+-rw-r--r--   0        0        0     1684 2024-04-17 15:48:37.357738 pyguiadapter-0.3.0/pyguiadapter/adapter/executor.py
+-rw-r--r--   0        0        0     1593 2024-04-17 15:52:24.455478 pyguiadapter-0.3.0/pyguiadapter/commons.py
+-rw-r--r--   0        0        0      199 2024-04-14 16:11:23.461322 pyguiadapter-0.3.0/pyguiadapter/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:11:23.461322 pyguiadapter-0.3.0/pyguiadapter/interact/__init__.py
+-rw-r--r--   0        0        0     5119 2024-04-17 16:06:29.919169 pyguiadapter-0.3.0/pyguiadapter/interact/ulogging.py
+-rw-r--r--   0        0        0    12531 2024-04-14 16:11:23.461322 pyguiadapter-0.3.0/pyguiadapter/interact/upopup.py
+-rw-r--r--   0        0        0      730 2024-04-17 15:50:59.280655 pyguiadapter-0.3.0/pyguiadapter/interact/uprint.py
+-rw-r--r--   0        0        0      753 2024-04-14 16:11:23.462322 pyguiadapter-0.3.0/pyguiadapter/res/icons/abnormal.svg
+-rw-r--r--   0        0        0      563 2024-04-14 16:11:23.462322 pyguiadapter-0.3.0/pyguiadapter/res/icons/acoustic.svg
+-rw-r--r--   0        0        0      437 2024-04-14 16:11:23.462322 pyguiadapter-0.3.0/pyguiadapter/res/icons/activity-source.svg
+-rw-r--r--   0        0        0      721 2024-04-14 16:11:23.462322 pyguiadapter-0.3.0/pyguiadapter/res/icons/add-computer.svg
+-rw-r--r--   0        0        0     1074 2024-04-14 16:11:23.463322 pyguiadapter-0.3.0/pyguiadapter/res/icons/add-picture.svg
+-rw-r--r--   0        0        0      556 2024-04-14 16:11:23.463322 pyguiadapter-0.3.0/pyguiadapter/res/icons/add-print.svg
+-rw-r--r--   0        0        0      611 2024-04-14 16:11:23.463322 pyguiadapter-0.3.0/pyguiadapter/res/icons/add-user.svg
+-rw-r--r--   0        0        0      820 2024-04-14 16:11:23.463322 pyguiadapter-0.3.0/pyguiadapter/res/icons/add-web.svg
+-rw-r--r--   0        0        0      444 2024-04-14 16:11:23.463322 pyguiadapter-0.3.0/pyguiadapter/res/icons/airplay.svg
+-rw-r--r--   0        0        0      744 2024-04-14 16:11:23.463322 pyguiadapter-0.3.0/pyguiadapter/res/icons/api-app.svg
+-rw-r--r--   0        0        0      915 2024-04-14 16:11:23.463322 pyguiadapter-0.3.0/pyguiadapter/res/icons/application-effect.svg
+-rw-r--r--   0        0        0      513 2024-04-14 16:11:23.464322 pyguiadapter-0.3.0/pyguiadapter/res/icons/application-one.svg
+-rw-r--r--   0        0        0      471 2024-04-14 16:11:23.464322 pyguiadapter-0.3.0/pyguiadapter/res/icons/application-two.svg
+-rw-r--r--   0        0        0      444 2024-04-14 16:11:23.464322 pyguiadapter-0.3.0/pyguiadapter/res/icons/area-map.svg
+-rw-r--r--   0        0        0     1704 2024-04-14 16:11:23.464322 pyguiadapter-0.3.0/pyguiadapter/res/icons/arithmetic-buttons.svg
+-rw-r--r--   0        0        0      886 2024-04-14 16:11:23.464322 pyguiadapter-0.3.0/pyguiadapter/res/icons/arithmetic-one.svg
+-rw-r--r--   0        0        0     1051 2024-04-14 16:11:23.464322 pyguiadapter-0.3.0/pyguiadapter/res/icons/arrow-keys.svg
+-rw-r--r--   0        0        0      510 2024-04-14 16:11:23.464322 pyguiadapter-0.3.0/pyguiadapter/res/icons/audio-file.svg
+-rw-r--r--   0        0        0      806 2024-04-14 16:11:23.464322 pyguiadapter-0.3.0/pyguiadapter/res/icons/audit.svg
+-rw-r--r--   0        0        0      503 2024-04-14 16:11:23.465322 pyguiadapter-0.3.0/pyguiadapter/res/icons/average.svg
+-rw-r--r--   0        0        0      871 2024-04-14 16:11:23.465322 pyguiadapter-0.3.0/pyguiadapter/res/icons/bitcoin.svg
+-rw-r--r--   0        0        0      753 2024-04-14 16:11:23.465322 pyguiadapter-0.3.0/pyguiadapter/res/icons/blackboard.svg
+-rw-r--r--   0        0        0      633 2024-04-14 16:11:23.465322 pyguiadapter-0.3.0/pyguiadapter/res/icons/blocks-and-arrows.svg
+-rw-r--r--   0        0        0      261 2024-04-14 16:11:23.465322 pyguiadapter-0.3.0/pyguiadapter/res/icons/bluetooth.svg
+-rw-r--r--   0        0        0      794 2024-04-14 16:11:23.466322 pyguiadapter-0.3.0/pyguiadapter/res/icons/bookmark-three.svg
+-rw-r--r--   0        0        0      981 2024-04-14 16:11:23.466322 pyguiadapter-0.3.0/pyguiadapter/res/icons/broadcast.svg
+-rw-r--r--   0        0        0      993 2024-04-14 16:11:23.466322 pyguiadapter-0.3.0/pyguiadapter/res/icons/browser.svg
+-rw-r--r--   0        0        0     1399 2024-04-14 16:11:23.466322 pyguiadapter-0.3.0/pyguiadapter/res/icons/bug.svg
+-rw-r--r--   0        0        0      978 2024-04-14 16:11:23.466322 pyguiadapter-0.3.0/pyguiadapter/res/icons/bytedance-mini-app.svg
+-rw-r--r--   0        0        0      334 2024-04-14 16:11:23.466322 pyguiadapter-0.3.0/pyguiadapter/res/icons/card-two.svg
+-rw-r--r--   0        0        0      643 2024-04-14 16:11:23.466322 pyguiadapter-0.3.0/pyguiadapter/res/icons/carousel-video.svg
+-rw-r--r--   0        0        0      849 2024-04-14 16:11:23.466322 pyguiadapter-0.3.0/pyguiadapter/res/icons/carousel.svg
+-rw-r--r--   0        0        0      685 2024-04-14 16:11:23.467323 pyguiadapter-0.3.0/pyguiadapter/res/icons/cast-screen.svg
+-rw-r--r--   0        0        0      472 2024-04-14 16:11:23.467323 pyguiadapter-0.3.0/pyguiadapter/res/icons/category-management.svg
+-rw-r--r--   0        0        0      443 2024-04-14 16:11:23.467323 pyguiadapter-0.3.0/pyguiadapter/res/icons/caution.svg
+-rw-r--r--   0        0        0     1016 2024-04-14 16:11:23.467323 pyguiadapter-0.3.0/pyguiadapter/res/icons/certificate.svg
+-rw-r--r--   0        0        0      634 2024-04-14 16:11:23.467323 pyguiadapter-0.3.0/pyguiadapter/res/icons/check-one.svg
+-rw-r--r--   0        0        0      697 2024-04-14 16:11:23.467323 pyguiadapter-0.3.0/pyguiadapter/res/icons/checklist.svg
+-rw-r--r--   0        0        0     1023 2024-04-14 16:11:23.467323 pyguiadapter-0.3.0/pyguiadapter/res/icons/chip.svg
+-rw-r--r--   0        0        0      519 2024-04-14 16:11:23.467323 pyguiadapter-0.3.0/pyguiadapter/res/icons/classroom.svg
+-rw-r--r--   0        0        0      478 2024-04-14 16:11:23.468322 pyguiadapter-0.3.0/pyguiadapter/res/icons/clipboard.svg
+-rw-r--r--   0        0        0      576 2024-04-14 16:11:23.468322 pyguiadapter-0.3.0/pyguiadapter/res/icons/close-one.svg
+-rw-r--r--   0        0        0     1211 2024-04-14 16:11:23.468322 pyguiadapter-0.3.0/pyguiadapter/res/icons/cloud-storage.svg
+-rw-r--r--   0        0        0      536 2024-04-14 16:11:23.468322 pyguiadapter-0.3.0/pyguiadapter/res/icons/code-brackets.svg
+-rw-r--r--   0        0        0      547 2024-04-14 16:11:23.468322 pyguiadapter-0.3.0/pyguiadapter/res/icons/code-download.svg
+-rw-r--r--   0        0        0      639 2024-04-14 16:11:23.468322 pyguiadapter-0.3.0/pyguiadapter/res/icons/code-laptop.svg
+-rw-r--r--   0        0        0      346 2024-04-14 16:11:23.468322 pyguiadapter-0.3.0/pyguiadapter/res/icons/code-one.svg
+-rw-r--r--   0        0        0      441 2024-04-14 16:11:23.468322 pyguiadapter-0.3.0/pyguiadapter/res/icons/code.svg
+-rw-r--r--   0        0        0      831 2024-04-14 16:11:23.469322 pyguiadapter-0.3.0/pyguiadapter/res/icons/collect-computer.svg
+-rw-r--r--   0        0        0      732 2024-04-14 16:11:23.469322 pyguiadapter-0.3.0/pyguiadapter/res/icons/collect-laptop.svg
+-rw-r--r--   0        0        0     1181 2024-04-14 16:11:23.469322 pyguiadapter-0.3.0/pyguiadapter/res/icons/collect-picture.svg
+-rw-r--r--   0        0        0     1118 2024-04-14 16:11:23.469322 pyguiadapter-0.3.0/pyguiadapter/res/icons/color-card.svg
+-rw-r--r--   0        0        0     1289 2024-04-14 16:11:23.469322 pyguiadapter-0.3.0/pyguiadapter/res/icons/command.svg
+-rw-r--r--   0        0        0      371 2024-04-14 16:11:23.469322 pyguiadapter-0.3.0/pyguiadapter/res/icons/comment-one.svg
+-rw-r--r--   0        0        0      581 2024-04-14 16:11:23.469322 pyguiadapter-0.3.0/pyguiadapter/res/icons/comment.svg
+-rw-r--r--   0        0        0      553 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/comments.svg
+-rw-r--r--   0        0        0      628 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/communication.svg
+-rw-r--r--   0        0        0      753 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/compass.svg
+-rw-r--r--   0        0        0     1110 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/compression.svg
+-rw-r--r--   0        0        0      556 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/computer.svg
+-rw-r--r--   0        0        0      447 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/cones.svg
+-rw-r--r--   0        0        0     1850 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/connect.svg
+-rw-r--r--   0        0        0      620 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/copy-one.svg
+-rw-r--r--   0        0        0      524 2024-04-14 16:11:23.470322 pyguiadapter-0.3.0/pyguiadapter/res/icons/copyright.svg
+-rw-r--r--   0        0        0     2644 2024-04-14 16:11:23.471322 pyguiadapter-0.3.0/pyguiadapter/res/icons/cpu.svg
+-rw-r--r--   0        0        0      516 2024-04-14 16:11:23.471322 pyguiadapter-0.3.0/pyguiadapter/res/icons/cross-ring-two.svg
+-rw-r--r--   0        0        0      895 2024-04-14 16:11:23.471322 pyguiadapter-0.3.0/pyguiadapter/res/icons/cube-four.svg
+-rw-r--r--   0        0        0      369 2024-04-14 16:11:23.471322 pyguiadapter-0.3.0/pyguiadapter/res/icons/curve-adjustment.svg
+-rw-r--r--   0        0        0     1177 2024-04-14 16:11:23.471322 pyguiadapter-0.3.0/pyguiadapter/res/icons/cuvette.svg
+-rw-r--r--   0        0        0     1199 2024-04-14 16:11:23.472322 pyguiadapter-0.3.0/pyguiadapter/res/icons/dashboard-one.svg
+-rw-r--r--   0        0        0     1332 2024-04-14 16:11:23.472322 pyguiadapter-0.3.0/pyguiadapter/res/icons/dashboard-two.svg
+-rw-r--r--   0        0        0     1221 2024-04-14 16:11:23.472322 pyguiadapter-0.3.0/pyguiadapter/res/icons/data-all.svg
+-rw-r--r--   0        0        0     1239 2024-04-14 16:11:23.472322 pyguiadapter-0.3.0/pyguiadapter/res/icons/data-display.svg
+-rw-r--r--   0        0        0     1255 2024-04-14 16:11:23.472322 pyguiadapter-0.3.0/pyguiadapter/res/icons/data-lock.svg
+-rw-r--r--   0        0        0      829 2024-04-14 16:11:23.472322 pyguiadapter-0.3.0/pyguiadapter/res/icons/data-screen.svg
+-rw-r--r--   0        0        0      833 2024-04-14 16:11:23.472322 pyguiadapter-0.3.0/pyguiadapter/res/icons/data-server.svg
+-rw-r--r--   0        0        0     1448 2024-04-14 16:11:23.472322 pyguiadapter-0.3.0/pyguiadapter/res/icons/data-switching.svg
+-rw-r--r--   0        0        0     1209 2024-04-14 16:11:23.473322 pyguiadapter-0.3.0/pyguiadapter/res/icons/data-user.svg
+-rw-r--r--   0        0        0      794 2024-04-14 16:11:23.473322 pyguiadapter-0.3.0/pyguiadapter/res/icons/data.svg
+-rw-r--r--   0        0        0     1588 2024-04-14 16:11:23.473322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-alert.svg
+-rw-r--r--   0        0        0     1606 2024-04-14 16:11:23.473322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-code.svg
+-rw-r--r--   0        0        0     1596 2024-04-14 16:11:23.473322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-config.svg
+-rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.473322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-download.svg
+-rw-r--r--   0        0        0     1516 2024-04-14 16:11:23.473322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-enter.svg
+-rw-r--r--   0        0        0     1528 2024-04-14 16:11:23.473322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-fail.svg
+-rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.474322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-first.svg
+-rw-r--r--   0        0        0     1492 2024-04-14 16:11:23.474322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-forbid.svg
+-rw-r--r--   0        0        0     1738 2024-04-14 16:11:23.474322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-lock.svg
+-rw-r--r--   0        0        0     1195 2024-04-14 16:11:23.474322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-network-point.svg
+-rw-r--r--   0        0        0     1770 2024-04-14 16:11:23.474322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-network.svg
+-rw-r--r--   0        0        0     1637 2024-04-14 16:11:23.474322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-point.svg
+-rw-r--r--   0        0        0     1390 2024-04-14 16:11:23.474322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-position.svg
+-rw-r--r--   0        0        0     1504 2024-04-14 16:11:23.475322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-power.svg
+-rw-r--r--   0        0        0     1528 2024-04-14 16:11:23.475322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-proportion.svg
+-rw-r--r--   0        0        0     1908 2024-04-14 16:11:23.475322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-search.svg
+-rw-r--r--   0        0        0     1542 2024-04-14 16:11:23.475322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-setting.svg
+-rw-r--r--   0        0        0     1504 2024-04-14 16:11:23.475322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-success.svg
+-rw-r--r--   0        0        0     1638 2024-04-14 16:11:23.475322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-sync.svg
+-rw-r--r--   0        0        0     1492 2024-04-14 16:11:23.475322 pyguiadapter-0.3.0/pyguiadapter/res/icons/database-time.svg
+-rw-r--r--   0        0        0      762 2024-04-14 16:11:23.475322 pyguiadapter-0.3.0/pyguiadapter/res/icons/date-comes-back.svg
+-rw-r--r--   0        0        0      470 2024-04-14 16:11:23.476322 pyguiadapter-0.3.0/pyguiadapter/res/icons/diamond-one.svg
+-rw-r--r--   0        0        0      470 2024-04-14 16:11:23.476322 pyguiadapter-0.3.0/pyguiadapter/res/icons/diamond-three.svg
+-rw-r--r--   0        0        0      466 2024-04-14 16:11:23.476322 pyguiadapter-0.3.0/pyguiadapter/res/icons/diamond-two.svg
+-rw-r--r--   0        0        0      855 2024-04-14 16:11:23.476322 pyguiadapter-0.3.0/pyguiadapter/res/icons/disk-one.svg
+-rw-r--r--   0        0        0      533 2024-04-14 16:11:23.476322 pyguiadapter-0.3.0/pyguiadapter/res/icons/disk-two.svg
+-rw-r--r--   0        0        0      599 2024-04-14 16:11:23.476322 pyguiadapter-0.3.0/pyguiadapter/res/icons/disk.svg
+-rw-r--r--   0        0        0      646 2024-04-14 16:11:23.476322 pyguiadapter-0.3.0/pyguiadapter/res/icons/document-folder.svg
+-rw-r--r--   0        0        0      957 2024-04-14 16:11:23.476322 pyguiadapter-0.3.0/pyguiadapter/res/icons/download-one.svg
+-rw-r--r--   0        0        0      649 2024-04-14 16:11:23.477322 pyguiadapter-0.3.0/pyguiadapter/res/icons/download-three.svg
+-rw-r--r--   0        0        0      730 2024-04-14 16:11:23.477322 pyguiadapter-0.3.0/pyguiadapter/res/icons/download-two.svg
+-rw-r--r--   0        0        0      827 2024-04-14 16:11:23.477322 pyguiadapter-0.3.0/pyguiadapter/res/icons/download-web.svg
+-rw-r--r--   0        0        0      500 2024-04-14 16:11:23.477322 pyguiadapter-0.3.0/pyguiadapter/res/icons/electrocardiogram.svg
+-rw-r--r--   0        0        0      568 2024-04-14 16:11:23.477322 pyguiadapter-0.3.0/pyguiadapter/res/icons/email-down.svg
+-rw-r--r--   0        0        0      567 2024-04-14 16:11:23.477322 pyguiadapter-0.3.0/pyguiadapter/res/icons/email-push.svg
+-rw-r--r--   0        0        0      634 2024-04-14 16:11:23.477322 pyguiadapter-0.3.0/pyguiadapter/res/icons/experiment-one.svg
+-rw-r--r--   0        0        0      731 2024-04-14 16:11:23.477322 pyguiadapter-0.3.0/pyguiadapter/res/icons/experiment.svg
+-rw-r--r--   0        0        0      680 2024-04-14 16:11:23.478322 pyguiadapter-0.3.0/pyguiadapter/res/icons/figma-component.svg
+-rw-r--r--   0        0        0      652 2024-04-14 16:11:23.478322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-addition.svg
+-rw-r--r--   0        0        0      664 2024-04-14 16:11:23.478322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-code.svg
+-rw-r--r--   0        0        0      856 2024-04-14 16:11:23.478322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-conversion.svg
+-rw-r--r--   0        0        0      772 2024-04-14 16:11:23.478322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-display.svg
+-rw-r--r--   0        0        0     1316 2024-04-14 16:11:23.478322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-pdf-one.svg
+-rw-r--r--   0        0        0     1381 2024-04-14 16:11:23.478322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-ppt.svg
+-rw-r--r--   0        0        0      658 2024-04-14 16:11:23.478322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-protection.svg
+-rw-r--r--   0        0        0      652 2024-04-14 16:11:23.479322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-text.svg
+-rw-r--r--   0        0        0      468 2024-04-14 16:11:23.479322 pyguiadapter-0.3.0/pyguiadapter/res/icons/file-word.svg
+-rw-r--r--   0        0        0      931 2024-04-14 16:11:23.479322 pyguiadapter-0.3.0/pyguiadapter/res/icons/film.svg
+-rw-r--r--   0        0        0      734 2024-04-14 16:11:23.479322 pyguiadapter-0.3.0/pyguiadapter/res/icons/flask.svg
+-rw-r--r--   0        0        0      455 2024-04-14 16:11:23.479322 pyguiadapter-0.3.0/pyguiadapter/res/icons/folder-open.svg
+-rw-r--r--   0        0        0      851 2024-04-14 16:11:23.479322 pyguiadapter-0.3.0/pyguiadapter/res/icons/game-handle.svg
+-rw-r--r--   0        0        0      989 2024-04-14 16:11:23.479322 pyguiadapter-0.3.0/pyguiadapter/res/icons/help.svg
+-rw-r--r--   0        0        0      545 2024-04-14 16:11:23.480322 pyguiadapter-0.3.0/pyguiadapter/res/icons/hexagon-one.svg
+-rw-r--r--   0        0        0      794 2024-04-14 16:11:23.480322 pyguiadapter-0.3.0/pyguiadapter/res/icons/id-card-h.svg
+-rw-r--r--   0        0        0      935 2024-04-14 16:11:23.480322 pyguiadapter-0.3.0/pyguiadapter/res/icons/info.svg
+-rw-r--r--   0        0        0      696 2024-04-14 16:11:23.480322 pyguiadapter-0.3.0/pyguiadapter/res/icons/install.svg
+-rw-r--r--   0        0        0    11553 2024-04-14 16:11:23.462322 pyguiadapter-0.3.0/pyguiadapter/res/icons/LICENSE
+-rw-r--r--   0        0        0      683 2024-04-14 16:11:23.480322 pyguiadapter-0.3.0/pyguiadapter/res/icons/many-to-many.svg
+-rw-r--r--   0        0        0      602 2024-04-14 16:11:23.480322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message-emoji.svg
+-rw-r--r--   0        0        0      522 2024-04-14 16:11:23.481322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message-one.svg
+-rw-r--r--   0        0        0      763 2024-04-14 16:11:23.481322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message-privacy.svg
+-rw-r--r--   0        0        0      648 2024-04-14 16:11:23.481322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message-search.svg
+-rw-r--r--   0        0        0      679 2024-04-14 16:11:23.481322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message-security.svg
+-rw-r--r--   0        0        0      485 2024-04-14 16:11:23.481322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message-sent.svg
+-rw-r--r--   0        0        0      577 2024-04-14 16:11:23.481322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message-success.svg
+-rw-r--r--   0        0        0      550 2024-04-14 16:11:23.481322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message-unread.svg
+-rw-r--r--   0        0        0      738 2024-04-14 16:11:23.481322 pyguiadapter-0.3.0/pyguiadapter/res/icons/message.svg
+-rw-r--r--   0        0        0      537 2024-04-14 16:11:23.482322 pyguiadapter-0.3.0/pyguiadapter/res/icons/mini-sd-card.svg
+-rw-r--r--   0        0        0      521 2024-04-14 16:11:23.482322 pyguiadapter-0.3.0/pyguiadapter/res/icons/monitor.svg
+-rw-r--r--   0        0        0     1053 2024-04-14 16:11:23.482322 pyguiadapter-0.3.0/pyguiadapter/res/icons/more-app.svg
+-rw-r--r--   0        0        0      971 2024-04-14 16:11:23.482322 pyguiadapter-0.3.0/pyguiadapter/res/icons/movie-board.svg
+-rw-r--r--   0        0        0     1213 2024-04-14 16:11:23.482322 pyguiadapter-0.3.0/pyguiadapter/res/icons/movie.svg
+-rw-r--r--   0        0        0      995 2024-04-14 16:11:23.482322 pyguiadapter-0.3.0/pyguiadapter/res/icons/multi-function-knife.svg
+-rw-r--r--   0        0        0      835 2024-04-14 16:11:23.482322 pyguiadapter-0.3.0/pyguiadapter/res/icons/notebook-one.svg
+-rw-r--r--   0        0        0      626 2024-04-14 16:11:23.482322 pyguiadapter-0.3.0/pyguiadapter/res/icons/octagon.svg
+-rw-r--r--   0        0        0      575 2024-04-14 16:11:23.483322 pyguiadapter-0.3.0/pyguiadapter/res/icons/online-meeting.svg
+-rw-r--r--   0        0        0      227 2024-04-14 16:11:23.483322 pyguiadapter-0.3.0/pyguiadapter/res/icons/oval-one.svg
+-rw-r--r--   0        0        0      537 2024-04-14 16:11:23.483322 pyguiadapter-0.3.0/pyguiadapter/res/icons/page-template.svg
+-rw-r--r--   0        0        0      440 2024-04-14 16:11:23.483322 pyguiadapter-0.3.0/pyguiadapter/res/icons/page.svg
+-rw-r--r--   0        0        0      412 2024-04-14 16:11:23.483322 pyguiadapter-0.3.0/pyguiadapter/res/icons/parallelogram.svg
+-rw-r--r--   0        0        0      633 2024-04-14 16:11:23.483322 pyguiadapter-0.3.0/pyguiadapter/res/icons/pay-code.svg
+-rw-r--r--   0        0        0      509 2024-04-14 16:11:23.483322 pyguiadapter-0.3.0/pyguiadapter/res/icons/pentagon-one.svg
+-rw-r--r--   0        0        0      980 2024-04-14 16:11:23.483322 pyguiadapter-0.3.0/pyguiadapter/res/icons/people-plus-one.svg
+-rw-r--r--   0        0        0     1040 2024-04-14 16:11:23.484322 pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-incoming-one.svg
+-rw-r--r--   0        0        0     1029 2024-04-14 16:11:23.484322 pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-incoming.svg
+-rw-r--r--   0        0        0     1083 2024-04-14 16:11:23.484322 pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-missed.svg
+-rw-r--r--   0        0        0     1015 2024-04-14 16:11:23.484322 pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-outgoing-one.svg
+-rw-r--r--   0        0        0     1008 2024-04-14 16:11:23.484322 pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-outgoing.svg
+-rw-r--r--   0        0        0      811 2024-04-14 16:11:23.484322 pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-telephone.svg
+-rw-r--r--   0        0        0      935 2024-04-14 16:11:23.484322 pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-video-call.svg
+-rw-r--r--   0        0        0      974 2024-04-14 16:11:23.484322 pyguiadapter-0.3.0/pyguiadapter/res/icons/platte.svg
+-rw-r--r--   0        0        0      473 2024-04-14 16:11:23.485322 pyguiadapter-0.3.0/pyguiadapter/res/icons/play.svg
+-rw-r--r--   0        0        0      434 2024-04-14 16:11:23.485322 pyguiadapter-0.3.0/pyguiadapter/res/icons/powerpoint.svg
+-rw-r--r--   0        0        0      612 2024-04-14 16:11:23.485322 pyguiadapter-0.3.0/pyguiadapter/res/icons/ppt.svg
+-rw-r--r--   0        0        0      427 2024-04-14 16:11:23.485322 pyguiadapter-0.3.0/pyguiadapter/res/icons/puzzle.svg
+-rw-r--r--   0        0        0      364 2024-04-14 16:11:23.485322 pyguiadapter-0.3.0/pyguiadapter/res/icons/quadrilateral.svg
+-rw-r--r--   0        0        0      783 2024-04-14 16:11:23.485322 pyguiadapter-0.3.0/pyguiadapter/res/icons/record-disc.svg
+-rw-r--r--   0        0        0      880 2024-04-14 16:11:23.486322 pyguiadapter-0.3.0/pyguiadapter/res/icons/record.svg
+-rw-r--r--   0        0        0      319 2024-04-14 16:11:23.486322 pyguiadapter-0.3.0/pyguiadapter/res/icons/rectangle-one.svg
+-rw-r--r--   0        0        0      328 2024-04-14 16:11:23.486322 pyguiadapter-0.3.0/pyguiadapter/res/icons/rectangle-small.svg
+-rw-r--r--   0        0        0      319 2024-04-14 16:11:23.486322 pyguiadapter-0.3.0/pyguiadapter/res/icons/rectangle.svg
+-rw-r--r--   0        0        0      591 2024-04-14 16:11:23.486322 pyguiadapter-0.3.0/pyguiadapter/res/icons/rename.py
+-rw-r--r--   0        0        0      425 2024-04-14 16:11:23.486322 pyguiadapter-0.3.0/pyguiadapter/res/icons/right-angle.svg
+-rw-r--r--   0        0        0      217 2024-04-14 16:11:23.486322 pyguiadapter-0.3.0/pyguiadapter/res/icons/round.svg
+-rw-r--r--   0        0        0      901 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/rule-two.svg
+-rw-r--r--   0        0        0      794 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/ruler-one.svg
+-rw-r--r--   0        0        0      926 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/ruler.svg
+-rw-r--r--   0        0        0      583 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/sd-card.svg
+-rw-r--r--   0        0        0     1259 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/setting-computer.svg
+-rw-r--r--   0        0        0     1148 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/setting-laptop.svg
+-rw-r--r--   0        0        0     1443 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/setting-two.svg
+-rw-r--r--   0        0        0      980 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/share-one.svg
+-rw-r--r--   0        0        0      328 2024-04-14 16:11:23.487322 pyguiadapter-0.3.0/pyguiadapter/res/icons/square-small.svg
+-rw-r--r--   0        0        0      317 2024-04-14 16:11:23.488322 pyguiadapter-0.3.0/pyguiadapter/res/icons/square.svg
+-rw-r--r--   0        0        0      954 2024-04-14 16:11:23.488322 pyguiadapter-0.3.0/pyguiadapter/res/icons/system.svg
+-rw-r--r--   0        0        0      895 2024-04-14 16:11:23.488322 pyguiadapter-0.3.0/pyguiadapter/res/icons/table-file.svg
+-rw-r--r--   0        0        0     1216 2024-04-14 16:11:23.488322 pyguiadapter-0.3.0/pyguiadapter/res/icons/tape.svg
+-rw-r--r--   0        0        0      465 2024-04-14 16:11:23.488322 pyguiadapter-0.3.0/pyguiadapter/res/icons/terminal.svg
+-rw-r--r--   0        0        0      751 2024-04-14 16:11:23.488322 pyguiadapter-0.3.0/pyguiadapter/res/icons/test-tube.svg
+-rw-r--r--   0        0        0      724 2024-04-14 16:11:23.488322 pyguiadapter-0.3.0/pyguiadapter/res/icons/thermometer.svg
+-rw-r--r--   0        0        0      425 2024-04-14 16:11:23.488322 pyguiadapter-0.3.0/pyguiadapter/res/icons/tips-one.svg
+-rw-r--r--   0        0        0      510 2024-04-14 16:11:23.489322 pyguiadapter-0.3.0/pyguiadapter/res/icons/tool.svg
+-rw-r--r--   0        0        0      587 2024-04-14 16:11:23.489322 pyguiadapter-0.3.0/pyguiadapter/res/icons/topic-discussion.svg
+-rw-r--r--   0        0        0     1027 2024-04-14 16:11:23.489322 pyguiadapter-0.3.0/pyguiadapter/res/icons/topic.svg
+-rw-r--r--   0        0        0      413 2024-04-14 16:11:23.489322 pyguiadapter-0.3.0/pyguiadapter/res/icons/trapezoid.svg
+-rw-r--r--   0        0        0      831 2024-04-14 16:11:23.489322 pyguiadapter-0.3.0/pyguiadapter/res/icons/tree-list.svg
+-rw-r--r--   0        0        0     1970 2024-04-14 16:11:23.489322 pyguiadapter-0.3.0/pyguiadapter/res/icons/triangle-ruler.svg
+-rw-r--r--   0        0        0      468 2024-04-14 16:11:23.489322 pyguiadapter-0.3.0/pyguiadapter/res/icons/triangle.svg
+-rw-r--r--   0        0        0      717 2024-04-14 16:11:23.489322 pyguiadapter-0.3.0/pyguiadapter/res/icons/vial.svg
+-rw-r--r--   0        0        0     1823 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/video.svg
+-rw-r--r--   0        0        0      706 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/view-grid-card.svg
+-rw-r--r--   0        0        0      775 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/view-grid-detail.svg
+-rw-r--r--   0        0        0      887 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/view-grid-list.svg
+-rw-r--r--   0        0        0      642 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/voice-input.svg
+-rw-r--r--   0        0        0      903 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/voice-message.svg
+-rw-r--r--   0        0        0      685 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/voice-one.svg
+-rw-r--r--   0        0        0      508 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/voice.svg
+-rw-r--r--   0        0        0     1173 2024-04-14 16:11:23.490322 pyguiadapter-0.3.0/pyguiadapter/res/icons/weixin-mini-app.svg
+-rw-r--r--   0        0        0      809 2024-04-14 16:11:23.491322 pyguiadapter-0.3.0/pyguiadapter/res/icons/wifi.svg
+-rw-r--r--   0        0        0      976 2024-04-14 16:11:23.491322 pyguiadapter-0.3.0/pyguiadapter/res/icons/zip.svg
+-rw-r--r--   0        0        0      358 2024-04-17 16:40:54.565013 pyguiadapter-0.3.0/pyguiadapter/ui/__init__.py
+-rw-r--r--   0        0        0     1513 2024-04-14 16:11:23.491322 pyguiadapter-0.3.0/pyguiadapter/ui/config.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:11:23.491322 pyguiadapter-0.3.0/pyguiadapter/ui/generated/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-16 16:25:55.273398 pyguiadapter-0.3.0/pyguiadapter/ui/generated/ui_class_init_window.py
+-rw-r--r--   0        0        0     7696 2024-04-16 16:25:55.346941 pyguiadapter-0.3.0/pyguiadapter/ui/generated/ui_execution_window.py
+-rw-r--r--   0        0        0     3700 2024-04-16 16:25:55.416780 pyguiadapter-0.3.0/pyguiadapter/ui/generated/ui_selection_window.py
+-rw-r--r--   0        0        0     1418 2024-04-17 16:04:29.140320 pyguiadapter-0.3.0/pyguiadapter/ui/menus.py
+-rw-r--r--   0        0        0     1457 2024-04-14 16:11:23.492322 pyguiadapter-0.3.0/pyguiadapter/ui/styles.py
+-rw-r--r--   0        0        0     3874 2024-04-17 16:07:29.237029 pyguiadapter-0.3.0/pyguiadapter/ui/utils.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:23:22.163246 pyguiadapter-0.3.0/pyguiadapter/ui/window/__init__.py
+-rw-r--r--   0        0        0       78 2024-04-14 16:11:23.493322 pyguiadapter-0.3.0/pyguiadapter/ui/window/class_init/__init__.py
+-rw-r--r--   0        0        0      260 2024-04-17 16:16:41.343493 pyguiadapter-0.3.0/pyguiadapter/ui/window/class_init/config.py
+-rw-r--r--   0        0        0      160 2024-04-14 16:11:23.493322 pyguiadapter-0.3.0/pyguiadapter/ui/window/class_init/constants.py
+-rw-r--r--   0        0        0     5367 2024-04-17 16:16:05.127955 pyguiadapter-0.3.0/pyguiadapter/ui/window/class_init/impl.py
+-rw-r--r--   0        0        0       78 2024-04-14 16:11:23.493322 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_execution/__init__.py
+-rw-r--r--   0        0        0     5243 2024-04-17 16:10:52.573365 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_execution/base.py
+-rw-r--r--   0        0        0     2713 2024-04-17 16:17:12.915519 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_execution/config.py
+-rw-r--r--   0        0        0      726 2024-04-14 16:11:23.494322 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_execution/constants.py
+-rw-r--r--   0        0        0     4121 2024-04-14 16:11:23.494322 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_execution/context.py
+-rw-r--r--   0        0        0      288 2024-04-14 16:11:23.494322 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_execution/exceptions.py
+-rw-r--r--   0        0        0    18087 2024-04-17 16:26:37.127247 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_execution/impl.py
+-rw-r--r--   0        0        0       78 2024-04-14 16:11:23.494322 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_selection/__init__.py
+-rw-r--r--   0        0        0      830 2024-04-14 16:11:23.495322 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_selection/config.py
+-rw-r--r--   0        0        0      305 2024-04-14 16:11:23.495322 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_selection/constants.py
+-rw-r--r--   0        0        0     7509 2024-04-17 16:30:44.468256 pyguiadapter-0.3.0/pyguiadapter/ui/window/func_selection/impl.py
+-rw-r--r--   0        0        0      685 2024-04-17 16:45:12.577415 pyguiadapter-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8722 2024-04-14 16:11:23.455323 pyguiadapter-0.3.0/README.md
+-rw-r--r--   0        0        0     9251 1970-01-01 00:00:00.000000 pyguiadapter-0.3.0/PKG-INFO
```

### Comparing `pyguiadapter-0.2.9/License` & `pyguiadapter-0.3.0/License`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/adapter/executor.py` & `pyguiadapter-0.3.0/pyguiadapter/adapter/executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,51 @@
 import copy
+import threading
 import traceback
+from typing import Optional
 
 from PyQt6.QtCore import QThread, pyqtSignal
 
-from pyguiadapter.adapter.bundle import FunctionBundle
+from .bundle import FunctionBundle
 
 
 class FunctionExecutor(QThread):
     exception_occurred = pyqtSignal(BaseException)
     result_ready = pyqtSignal(object)
+    cancel_requested = pyqtSignal()
 
-    def __init__(self, function: FunctionBundle, arguments: dict, parent=None):
+    def __init__(self, func_bundle: FunctionBundle, arguments: dict, parent=None):
         super().__init__(parent)
-        self._function = function
+        self._func_bundle = func_bundle
         self._arguments = copy.deepcopy(arguments)
 
+        self._cancel_event: Optional[threading.Event] = None
+        if func_bundle.cancelable:
+            # noinspection PyUnresolvedReferences
+            self.cancel_requested.connect(self._on_cancel_requested)
+
     def run(self):
         try:
             result = self.on_execute()
         except BaseException as e:
             traceback.print_exc()
             # noinspection PyUnresolvedReferences
             self.exception_occurred.emit(e)
         else:
             # noinspection PyUnresolvedReferences
             self.result_ready.emit(result)
 
     def on_execute(self):
-        return self._function.execute(**self._arguments)
+        arguments = {**self._arguments}
+        if self._func_bundle.cancelable:
+            self._cancel_event = threading.Event()
+            cancel_event_param_name = self._func_bundle.cancel_event_param_name
+            arguments[cancel_event_param_name] = self._cancel_event
+
+        ret = self._func_bundle.execute_function(**arguments)
+        self._cancel_event = None
+        return ret
+
+    def _on_cancel_requested(self):
+        if self._cancel_event is None:
+            return
+        self._cancel_event.set()
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/commons.py` & `pyguiadapter-0.3.0/pyguiadapter/commons.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 import enum
+import importlib.resources
 import os
 import warnings
-import importlib.resources
 from typing import TypeVar, Optional
 
-from PyQt6.QtWidgets import QLayout
-from function2widgets.parser import FunctionDescriptionParser
 from function2widgets.factory import ParameterWidgetFactory
+from function2widgets.parser.function_parser import FunctionInfoParser
 
 T = TypeVar("T")
 
-
 ICON_FILE_EXT = ".svg"
 
-__function_parser = FunctionDescriptionParser()
+__func_parser = FunctionInfoParser()
 __widget_factory = ParameterWidgetFactory()
 
 
 class DocumentFormat(enum.Enum):
     HTML = "html"
     MARKDOWN = "markdown"
     PLAIN = "plain"
 
 
-def get_function_parser() -> FunctionDescriptionParser:
-    global __function_parser
-    return __function_parser
+def get_function_parser() -> FunctionInfoParser:
+    return __func_parser
 
 
-def get_widget_factory() -> ParameterWidgetFactory:
-    global __widget_factory
+def get_param_widget_factory() -> ParameterWidgetFactory:
     return __widget_factory
 
 
 def get_res_dir() -> str:
     with importlib.resources.path("pyguiadapter", "res") as res_dir:
         return str(res_dir)
 
@@ -54,25 +50,13 @@
         with open(filename, "r", encoding=encoding) as f:
             return f.read()
     except BaseException as e:
         warnings.warn(f"failed to read file '{filename}': {e}")
         return None
 
 
-def clear_layout(layout: QLayout) -> None:
-    if not layout:
-        return
-    while layout.count() > 0:
-        item = layout.takeAt(0)
-
-        widget = item.widget()
-        if widget:
-            widget.deleteLater()
-
-        child_layout = item.layout()
-        if child_layout:
-            clear_layout(child_layout)
-            continue
-
-        spacer_item = item.spacerItem()
-        if spacer_item:
-            layout.removeItem(spacer_item)
+def safe_del(d: dict, key_to_del: str, *more_keys: str) -> dict:
+    keys = {key_to_del, *more_keys}
+    for key in keys:
+        if key in d:
+            del d[key]
+    return d
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/interact/ulogging.py` & `pyguiadapter-0.3.0/pyguiadapter/interact/ulogging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import enum
+import html
 from datetime import datetime
 
-from pyguiadapter.interact.uprint import uprint
+from .uprint import uprint
 
-COLOR_INFO = "#00FF00"
-COLOR_DEBUG = "#FFFFFF"
-COLOR_WARNING = "#FFFF00"
-COLOR_CRITICAL = "#FF0000"
-COLOR_FATAL = "#FF0000"
+DEFAULT_COLOR_INFO = "#00FF00"
+DEFAULT_COLOR_DEBUG = "#FFFFFF"
+DEFAULT_COLOR_WARNING = "#FFFF00"
+DEFAULT_COLOR_CRITICAL = "#FF0000"
+DEFAULT_COLOR_FATAL = "#A61C00"
 
 
 class LogLevel(enum.Enum):
     INFO = 0
     DEBUG = 1
     WARNING = 2
     CRITICAL = 3
@@ -19,19 +20,19 @@
 
 
 __colored_msg_template = "<font color=%s>%s</font>"
 __timestamp = False
 __timestamp_pattern = "%Y-%m-%d %H:%M:%S"
 __print_func = uprint
 __additional_newline = False
-__color_info = COLOR_INFO
-__color_warning = COLOR_WARNING
-__color_debug = COLOR_DEBUG
-__color_critical = COLOR_CRITICAL
-__color_fatal = COLOR_FATAL
+__color_info = DEFAULT_COLOR_INFO
+__color_warning = DEFAULT_COLOR_WARNING
+__color_debug = DEFAULT_COLOR_DEBUG
+__color_critical = DEFAULT_COLOR_CRITICAL
+__color_fatal = DEFAULT_COLOR_FATAL
 
 
 def set_print_func(print_func):
     global __print_func
     __print_func = print_func
 
 
@@ -99,32 +100,35 @@
         timestamp_pattern = __timestamp_pattern
     if additional_nl is None:
         additional_nl = __additional_newline
     if print_func is None:
         print_func = __print_func
 
     global __color_info, __color_warning, __color_debug, __color_critical, __color_fatal
+
+    msg = html.escape(msg)
     if level == LogLevel.INFO:
         msg = _message(msg, __color_info)
     elif level == LogLevel.DEBUG:
         msg = _message(msg, __color_debug)
     elif level == LogLevel.WARNING:
         msg = _message(msg, __color_warning)
     elif level == LogLevel.CRITICAL:
         msg = _message(msg, __color_critical)
     elif level == LogLevel.FATAL:
         msg = _message(msg, __color_critical)
     elif level == LogLevel.FATAL:
         msg = _message(msg, __color_fatal)
     else:
         pass
+
     if timestamp:
         timestamp_str = datetime.now().strftime(timestamp_pattern)
         msg = f"[{timestamp_str}] {msg}"
-    print_func(msg, html=True)
+    print_func(f"{msg}", html=True)
     if additional_nl:
         print_func(html=False)
 
 
 def info(
     msg: str,
     timestamp: bool = None,
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/interact/upopup.py` & `pyguiadapter-0.3.0/pyguiadapter/interact/upopup.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/interact/uprint.py` & `pyguiadapter-0.3.0/pyguiadapter/interact/uprint.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,18 @@
         self.printed.emit(text, html)
 
 
 __uprint = UPrint()
 
 
 def set_print_destination(func: callable):
-    global __uprint
     # noinspection PyUnresolvedReferences
     __uprint.printed.connect(func)
 
 
 def remove_print_destination(func: callable):
-    global __uprint
     # noinspection PyUnresolvedReferences
     __uprint.printed.disconnect(func)
 
 
 def uprint(*args, sep=" ", end="\n", html: bool = False):
-    global __uprint
     __uprint.print(*args, sep=sep, end=end, html=html)
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/abnormal.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/abnormal.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/acoustic.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/acoustic.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-computer.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/add-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-picture.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/add-picture.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-print.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/add-print.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-user.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/add-user.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/add-web.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/add-web.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/api-app.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/api-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/application-effect.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/application-effect.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/application-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/application-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/arithmetic-buttons.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/arithmetic-buttons.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/arithmetic-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/arithmetic-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/arrow-keys.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/arrow-keys.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/audit.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/audit.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/bitcoin.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/bitcoin.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/blackboard.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/blackboard.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/blocks-and-arrows.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/blocks-and-arrows.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/bookmark-three.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/bookmark-three.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/broadcast.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/broadcast.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/browser.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/browser.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/bug.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/bytedance-mini-app.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/bytedance-mini-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/carousel-video.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/carousel-video.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/carousel.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/carousel.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/cast-screen.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/cast-screen.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/certificate.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/certificate.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/check-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/check-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/checklist.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/checklist.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/chip.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/chip.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/classroom.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/classroom.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/close-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/close-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/cloud-storage.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/cloud-storage.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/code-brackets.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/code-brackets.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/code-download.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/code-download.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/code-laptop.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/code-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-computer.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/collect-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-laptop.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/collect-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/collect-picture.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/collect-picture.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/color-card.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/color-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/command.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/command.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/comment.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/comment.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/comments.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/comments.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/communication.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/communication.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/compass.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/compass.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/compression.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/compression.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/computer.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/connect.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/connect.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/copy-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/copy-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/copyright.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/copyright.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/cpu.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/cross-ring-two.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/cross-ring-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/cube-four.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/cube-four.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/cuvette.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/cuvette.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/dashboard-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/dashboard-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/dashboard-two.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/dashboard-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-all.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/data-all.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-display.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/data-display.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-lock.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/data-lock.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-screen.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/data-screen.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-server.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/data-server.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-switching.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/data-switching.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/data-user.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/data-user.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/data.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/data.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-alert.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-alert.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-code.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-config.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-config.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-download.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-download.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-enter.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-enter.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-fail.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-fail.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-first.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-first.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-forbid.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-forbid.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-lock.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-lock.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-network-point.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-network-point.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-network.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-network.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-point.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-point.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-position.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-position.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-power.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-power.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-proportion.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-proportion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-search.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-search.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-setting.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-setting.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-success.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-success.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-sync.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-sync.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/database-time.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/database-time.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/date-comes-back.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/date-comes-back.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/disk-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/disk-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/disk-two.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/disk-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/disk.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/disk.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/document-folder.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/document-folder.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/download-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/download-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/download-three.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/download-three.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/download-two.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/download-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/download-web.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/download-web.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/email-down.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/email-down.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/email-push.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/email-push.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/experiment-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/experiment-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/experiment.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/experiment.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/figma-component.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/figma-component.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-addition.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/file-addition.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-code.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/file-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-conversion.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/file-conversion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-display.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/file-display.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-pdf-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/file-pdf-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-ppt.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/file-ppt.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-protection.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/file-protection.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/file-text.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/file-text.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/film.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/film.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/flask.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/flask.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/game-handle.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/game-handle.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/help.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/hexagon-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/hexagon-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/id-card-h.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/id-card-h.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/info.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/install.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/install.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/LICENSE.txt` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/many-to-many.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/many-to-many.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-emoji.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/message-emoji.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/message-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-privacy.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/message-privacy.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-search.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/message-search.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-security.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/message-security.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-success.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/message-success.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/message-unread.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/message-unread.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/message.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/message.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/mini-sd-card.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/mini-sd-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/monitor.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/monitor.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/more-app.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/more-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/movie-board.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/movie-board.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/movie.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/movie.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/multi-function-knife.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/multi-function-knife.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/notebook-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/notebook-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/octagon.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/octagon.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/online-meeting.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/online-meeting.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/page-template.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/page-template.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/pay-code.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/pay-code.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/people-plus-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/people-plus-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-incoming-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-incoming-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-incoming.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-missed.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-outgoing-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-outgoing-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-outgoing.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-telephone.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-telephone.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/phone-video-call.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/phone-video-call.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/platte.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/platte.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/ppt.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/ppt.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/record-disc.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/record-disc.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/record.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/record.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/rename.py` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/rename.py`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/rule-two.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/rule-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/ruler-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/ruler-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/ruler.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/ruler.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/sd-card.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/sd-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-computer.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/setting-computer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-laptop.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/setting-laptop.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/setting-two.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/setting-two.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/share-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/share-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/system.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/system.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/table-file.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/table-file.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/tape.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/tape.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/test-tube.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/test-tube.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/thermometer.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/thermometer.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/topic-discussion.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/topic-discussion.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/topic.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/topic.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/tree-list.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/tree-list.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/triangle-ruler.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/triangle-ruler.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/vial.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/vial.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/video.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/video.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-card.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/view-grid-card.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-detail.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/view-grid-detail.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/view-grid-list.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/view-grid-list.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-input.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/voice-input.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-message.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/voice-message.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/voice-one.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/voice-one.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/weixin-mini-app.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/weixin-mini-app.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/wifi.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/wifi.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/res/icons/zip.svg` & `pyguiadapter-0.3.0/pyguiadapter/res/icons/zip.svg`

 * *Files identical despite different names*

### Comparing `pyguiadapter-0.2.9/pyguiadapter/ui/config.py` & `pyguiadapter-0.3.0/pyguiadapter/ui/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 import warnings
-from typing import Optional, Union
+from typing import Optional, Union, NoReturn
 
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import QMainWindow, QDialog
 
 from pyguiadapter.commons import safe_read
 
 
@@ -15,32 +15,32 @@
     width: Optional[int] = None
     height: Optional[int] = None
     x: Optional[int] = None
     y: Optional[int] = None
 
     stylesheet: Optional[str] = None
 
-    def apply_to(self, w: Union[QMainWindow, QDialog]) -> None:
+    def apply_basic_configs(self, win: Union[QMainWindow, QDialog]) -> NoReturn:
         if self.title is not None:
-            w.setWindowTitle(self.title)
+            win.setWindowTitle(self.title)
         if self.icon is not None:
-            self._set_icon(w)
+            self._set_icon(win)
         if self.width is not None and self.height is not None:
-            w.resize(self.width, self.height)
+            win.resize(self.width, self.height)
         if self.x is not None and self.y is not None:
-            w.move(self.x, self.y)
+            win.move(self.x, self.y)
 
         if self.stylesheet:
             stylesheet = safe_read(self.stylesheet)
             if stylesheet is not None:
-                w.setStyleSheet(stylesheet)
+                win.setStyleSheet(stylesheet)
             else:
-                w.setStyleSheet(self.stylesheet)
+                win.setStyleSheet(self.stylesheet)
 
-    def _set_icon(self, w: Union[QMainWindow, QDialog]):
+    def _set_icon(self, w: Union[QMainWindow, QDialog]) -> NoReturn:
         if self.icon is None:
             return
         try:
             icon = QIcon(self.icon)
         except BaseException as e:
             warnings.warn(w.tr(f"failed to load icon {self.icon}: {e}"))
         else:
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_execution_window.py` & `pyguiadapter-0.3.0/pyguiadapter/ui/generated/ui_execution_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Form implementation generated from reading ui file 'D:\Projects\PyGUIAdapter\designer\execution_window.ui'
+# Form implementation generated from reading ui file 'C:\Users\zyzz_\Projects\PyGUIAdapter\designer\execution_window.ui'
 #
 # Created by: PyQt6 UI code generator 6.6.1
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
@@ -18,41 +18,44 @@
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.centralwidget.sizePolicy().hasHeightForWidth())
         self.centralwidget.setSizePolicy(sizePolicy)
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.centralwidget)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.groupbox_parameters = QtWidgets.QGroupBox(parent=self.centralwidget)
-        self.groupbox_parameters.setEnabled(True)
-        self.groupbox_parameters.setFlat(False)
-        self.groupbox_parameters.setCheckable(False)
-        self.groupbox_parameters.setObjectName("groupbox_parameters")
-        self.vlayout_4 = QtWidgets.QVBoxLayout(self.groupbox_parameters)
+        self.groupbox_params = QtWidgets.QGroupBox(parent=self.centralwidget)
+        self.groupbox_params.setEnabled(True)
+        self.groupbox_params.setFlat(False)
+        self.groupbox_params.setCheckable(False)
+        self.groupbox_params.setObjectName("groupbox_params")
+        self.vlayout_4 = QtWidgets.QVBoxLayout(self.groupbox_params)
         self.vlayout_4.setContentsMargins(2, 2, 2, 2)
         self.vlayout_4.setSpacing(0)
         self.vlayout_4.setObjectName("vlayout_4")
-        self.scrollarea = QtWidgets.QScrollArea(parent=self.groupbox_parameters)
+        self.scrollarea = QtWidgets.QScrollArea(parent=self.groupbox_params)
         self.scrollarea.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
         self.scrollarea.setWidgetResizable(True)
         self.scrollarea.setObjectName("scrollarea")
         self.scrollarea_content = QtWidgets.QWidget()
-        self.scrollarea_content.setGeometry(QtCore.QRect(0, 0, 507, 469))
+        self.scrollarea_content.setGeometry(QtCore.QRect(0, 0, 512, 452))
         self.scrollarea_content.setObjectName("scrollarea_content")
         self.scrollarea.setWidget(self.scrollarea_content)
         self.vlayout_4.addWidget(self.scrollarea)
-        self.verticalLayout.addWidget(self.groupbox_parameters)
-        self.checkbox_auto_clear = QtWidgets.QCheckBox(parent=self.centralwidget)
-        self.checkbox_auto_clear.setObjectName("checkbox_auto_clear")
-        self.verticalLayout.addWidget(self.checkbox_auto_clear)
+        self.verticalLayout.addWidget(self.groupbox_params)
+        self.checkbox_autoclear = QtWidgets.QCheckBox(parent=self.centralwidget)
+        self.checkbox_autoclear.setObjectName("checkbox_autoclear")
+        self.verticalLayout.addWidget(self.checkbox_autoclear)
         self.hlayout_1 = QtWidgets.QHBoxLayout()
         self.hlayout_1.setObjectName("hlayout_1")
         self.button_execute = QtWidgets.QPushButton(parent=self.centralwidget)
         self.button_execute.setObjectName("button_execute")
         self.hlayout_1.addWidget(self.button_execute)
+        self.button_cancel = QtWidgets.QPushButton(parent=self.centralwidget)
+        self.button_cancel.setObjectName("button_cancel")
+        self.hlayout_1.addWidget(self.button_cancel)
         self.button_clear = QtWidgets.QPushButton(parent=self.centralwidget)
         self.button_clear.setObjectName("button_clear")
         self.hlayout_1.addWidget(self.button_clear)
         self.verticalLayout.addLayout(self.hlayout_1)
         ExecutionWindow.setCentralWidget(self.centralwidget)
         self.statusbar = QtWidgets.QStatusBar(parent=ExecutionWindow)
         self.statusbar.setObjectName("statusbar")
@@ -61,33 +64,39 @@
         self.dockwidget_output.setObjectName("dockwidget_output")
         self.dockwidget_content = QtWidgets.QWidget()
         self.dockwidget_content.setObjectName("dockwidget_content")
         self.vlayout_3 = QtWidgets.QVBoxLayout(self.dockwidget_content)
         self.vlayout_3.setContentsMargins(2, 2, 2, 5)
         self.vlayout_3.setSpacing(2)
         self.vlayout_3.setObjectName("vlayout_3")
-        self.textedit_output = QtWidgets.QTextEdit(parent=self.dockwidget_content)
+        self.textedit_output = QtWidgets.QTextBrowser(parent=self.dockwidget_content)
         self.textedit_output.setObjectName("textedit_output")
         self.vlayout_3.addWidget(self.textedit_output)
         self.dockwidget_output.setWidget(self.dockwidget_content)
         ExecutionWindow.addDockWidget(QtCore.Qt.DockWidgetArea(2), self.dockwidget_output)
         self.dockwidget_document = QtWidgets.QDockWidget(parent=ExecutionWindow)
         self.dockwidget_document.setObjectName("dockwidget_document")
         self.dockwidget_content_2 = QtWidgets.QWidget()
         self.dockwidget_content_2.setObjectName("dockwidget_content_2")
         self.vlayout_2 = QtWidgets.QVBoxLayout(self.dockwidget_content_2)
         self.vlayout_2.setContentsMargins(2, 2, 2, 5)
         self.vlayout_2.setSpacing(2)
         self.vlayout_2.setObjectName("vlayout_2")
-        self.textedit_document = QtWidgets.QTextEdit(parent=self.dockwidget_content_2)
-        self.textedit_document.setReadOnly(True)
+        self.textedit_document = QtWidgets.QTextBrowser(parent=self.dockwidget_content_2)
         self.textedit_document.setObjectName("textedit_document")
         self.vlayout_2.addWidget(self.textedit_document)
         self.dockwidget_document.setWidget(self.dockwidget_content_2)
         ExecutionWindow.addDockWidget(QtCore.Qt.DockWidgetArea(2), self.dockwidget_document)
+        self.toolbar = QtWidgets.QToolBar(parent=ExecutionWindow)
+        self.toolbar.setObjectName("toolbar")
+        ExecutionWindow.addToolBar(QtCore.Qt.ToolBarArea.TopToolBarArea, self.toolbar)
+        self.menubar = QtWidgets.QMenuBar(parent=ExecutionWindow)
+        self.menubar.setGeometry(QtCore.QRect(0, 0, 800, 21))
+        self.menubar.setObjectName("menubar")
+        ExecutionWindow.setMenuBar(self.menubar)
         self.action_output_view = QtGui.QAction(parent=ExecutionWindow)
         self.action_output_view.setCheckable(True)
         self.action_output_view.setChecked(True)
         self.action_output_view.setObjectName("action_output_view")
         self.action_document_view = QtGui.QAction(parent=ExecutionWindow)
         self.action_document_view.setCheckable(True)
         self.action_document_view.setChecked(True)
@@ -99,17 +108,19 @@
 
         self.retranslateUi(ExecutionWindow)
         QtCore.QMetaObject.connectSlotsByName(ExecutionWindow)
 
     def retranslateUi(self, ExecutionWindow):
         _translate = QtCore.QCoreApplication.translate
         ExecutionWindow.setWindowTitle(_translate("ExecutionWindow", "Function Execution"))
-        self.groupbox_parameters.setTitle(_translate("ExecutionWindow", "Parameters"))
-        self.checkbox_auto_clear.setText(_translate("ExecutionWindow", "clear output before execution"))
+        self.groupbox_params.setTitle(_translate("ExecutionWindow", "Parameters"))
+        self.checkbox_autoclear.setText(_translate("ExecutionWindow", "clear output before execution"))
         self.button_execute.setText(_translate("ExecutionWindow", "Execute"))
+        self.button_cancel.setText(_translate("ExecutionWindow", "Cancel"))
         self.button_clear.setText(_translate("ExecutionWindow", "Clear Output"))
         self.dockwidget_output.setWindowTitle(_translate("ExecutionWindow", "Output"))
         self.dockwidget_document.setWindowTitle(_translate("ExecutionWindow", "Document"))
+        self.toolbar.setWindowTitle(_translate("ExecutionWindow", "toolBar"))
         self.action_output_view.setText(_translate("ExecutionWindow", "Output View"))
         self.action_document_view.setText(_translate("ExecutionWindow", "Document View"))
         self.actionAbout.setText(_translate("ExecutionWindow", "About"))
         self.actionHelp.setText(_translate("ExecutionWindow", "Help"))
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_initialization_window.py` & `pyguiadapter-0.3.0/pyguiadapter/ui/generated/ui_class_init_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-# Form implementation generated from reading ui file 'D:\Projects\PyGUIAdapter\designer\initialization_window.ui'
+# Form implementation generated from reading ui file 'C:\Users\zyzz_\Projects\PyGUIAdapter\designer\class_init_window.ui'
 #
 # Created by: PyQt6 UI code generator 6.6.1
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
-class Ui_InitializationWindow(object):
-    def setupUi(self, InitializationWindow):
-        InitializationWindow.setObjectName("InitializationWindow")
-        InitializationWindow.resize(410, 619)
-        self.verticalLayout = QtWidgets.QVBoxLayout(InitializationWindow)
+class Ui_ClassInitWindow(object):
+    def setupUi(self, ClassInitWindow):
+        ClassInitWindow.setObjectName("ClassInitWindow")
+        ClassInitWindow.resize(410, 619)
+        self.verticalLayout = QtWidgets.QVBoxLayout(ClassInitWindow)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.label = QtWidgets.QLabel(parent=InitializationWindow)
-        self.label.setObjectName("label")
-        self.verticalLayout.addWidget(self.label)
-        self.line = QtWidgets.QFrame(parent=InitializationWindow)
+        self.label_title = QtWidgets.QLabel(parent=ClassInitWindow)
+        self.label_title.setObjectName("label_title")
+        self.verticalLayout.addWidget(self.label_title)
+        self.line = QtWidgets.QFrame(parent=ClassInitWindow)
         self.line.setFrameShape(QtWidgets.QFrame.Shape.HLine)
         self.line.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.line.setObjectName("line")
         self.verticalLayout.addWidget(self.line)
-        self.scrollarea = QtWidgets.QScrollArea(parent=InitializationWindow)
+        self.scrollarea = QtWidgets.QScrollArea(parent=ClassInitWindow)
         self.scrollarea.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
         self.scrollarea.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.scrollarea.setWidgetResizable(True)
         self.scrollarea.setObjectName("scrollarea")
         self.param_widgets_container = QtWidgets.QWidget()
         self.param_widgets_container.setGeometry(QtCore.QRect(0, 0, 388, 520))
         self.param_widgets_container.setObjectName("param_widgets_container")
         self.scrollarea.setWidget(self.param_widgets_container)
         self.verticalLayout.addWidget(self.scrollarea)
-        self.line_2 = QtWidgets.QFrame(parent=InitializationWindow)
+        self.line_2 = QtWidgets.QFrame(parent=ClassInitWindow)
         self.line_2.setFrameShape(QtWidgets.QFrame.Shape.HLine)
         self.line_2.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.line_2.setObjectName("line_2")
         self.verticalLayout.addWidget(self.line_2)
-        self.button_initialize = QtWidgets.QPushButton(parent=InitializationWindow)
+        self.button_initialize = QtWidgets.QPushButton(parent=ClassInitWindow)
         self.button_initialize.setObjectName("button_initialize")
         self.verticalLayout.addWidget(self.button_initialize)
 
-        self.retranslateUi(InitializationWindow)
-        QtCore.QMetaObject.connectSlotsByName(InitializationWindow)
+        self.retranslateUi(ClassInitWindow)
+        QtCore.QMetaObject.connectSlotsByName(ClassInitWindow)
 
-    def retranslateUi(self, InitializationWindow):
+    def retranslateUi(self, ClassInitWindow):
         _translate = QtCore.QCoreApplication.translate
-        InitializationWindow.setWindowTitle(_translate("InitializationWindow", "Initialization"))
-        self.label.setText(_translate("InitializationWindow", "Initialization Parameters"))
-        self.button_initialize.setText(_translate("InitializationWindow", "Initialize"))
+        ClassInitWindow.setWindowTitle(_translate("ClassInitWindow", "Initialization"))
+        self.label_title.setText(_translate("ClassInitWindow", "Initialization Parameters"))
+        self.button_initialize.setText(_translate("ClassInitWindow", "Initialize"))
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/ui/generated/ui_selection_window.py` & `pyguiadapter-0.3.0/pyguiadapter/ui/generated/ui_selection_window.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Form implementation generated from reading ui file 'D:\Projects\PyGUIAdapter\designer\selection_window.ui'
+# Form implementation generated from reading ui file 'C:\Users\zyzz_\Projects\PyGUIAdapter\designer\selection_window.ui'
 #
 # Created by: PyQt6 UI code generator 6.6.1
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
@@ -21,17 +21,17 @@
         self.splitter.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.splitter.setObjectName("splitter")
         self.layoutWidget = QtWidgets.QWidget(parent=self.splitter)
         self.layoutWidget.setObjectName("layoutWidget")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.layoutWidget)
         self.verticalLayout.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.label_functions = QtWidgets.QLabel(parent=self.layoutWidget)
-        self.label_functions.setObjectName("label_functions")
-        self.verticalLayout.addWidget(self.label_functions)
+        self.label_func_list = QtWidgets.QLabel(parent=self.layoutWidget)
+        self.label_func_list.setObjectName("label_func_list")
+        self.verticalLayout.addWidget(self.label_func_list)
         self.listwidget_functions = QtWidgets.QListWidget(parent=self.layoutWidget)
         self.listwidget_functions.setObjectName("listwidget_functions")
         self.verticalLayout.addWidget(self.listwidget_functions)
         self.hlayout_bottom = QtWidgets.QHBoxLayout()
         self.hlayout_bottom.setObjectName("hlayout_bottom")
         self.button_select = QtWidgets.QPushButton(parent=self.layoutWidget)
         self.button_select.setObjectName("button_select")
@@ -41,32 +41,25 @@
         self.layoutWidget1.setObjectName("layoutWidget1")
         self.vlayout_right = QtWidgets.QVBoxLayout(self.layoutWidget1)
         self.vlayout_right.setContentsMargins(0, 0, 0, 0)
         self.vlayout_right.setObjectName("vlayout_right")
         self.label_document = QtWidgets.QLabel(parent=self.layoutWidget1)
         self.label_document.setObjectName("label_document")
         self.vlayout_right.addWidget(self.label_document)
-        self.textedit_document = QtWidgets.QTextEdit(parent=self.layoutWidget1)
-        self.textedit_document.setLineWrapMode(QtWidgets.QTextEdit.LineWrapMode.WidgetWidth)
-        self.textedit_document.setReadOnly(True)
+        self.textedit_document = QtWidgets.QTextBrowser(parent=self.layoutWidget1)
         self.textedit_document.setObjectName("textedit_document")
         self.vlayout_right.addWidget(self.textedit_document)
         self.verticalLayout_2.addWidget(self.splitter)
         SelectionWindow.setCentralWidget(self.centralwidget)
         self.statusbar = QtWidgets.QStatusBar(parent=SelectionWindow)
         self.statusbar.setObjectName("statusbar")
         SelectionWindow.setStatusBar(self.statusbar)
 
         self.retranslateUi(SelectionWindow)
         QtCore.QMetaObject.connectSlotsByName(SelectionWindow)
 
     def retranslateUi(self, SelectionWindow):
         _translate = QtCore.QCoreApplication.translate
         SelectionWindow.setWindowTitle(_translate("SelectionWindow", "Select Function"))
-        self.label_functions.setText(_translate("SelectionWindow", "Functions"))
+        self.label_func_list.setText(_translate("SelectionWindow", "Functions"))
         self.button_select.setText(_translate("SelectionWindow", "Select"))
         self.label_document.setText(_translate("SelectionWindow", "Documentation"))
-        self.textedit_document.setHtml(_translate("SelectionWindow", "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
-"<html><head><meta name=\"qrichtext\" content=\"1\" /><style type=\"text/css\">\n"
-"p, li { white-space: pre-wrap; }\n"
-"</style></head><body style=\" font-family:\'SimSun\'; font-size:9pt; font-weight:400; font-style:normal;\">\n"
-"<p style=\"-qt-paragraph-type:empty; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><br /></p></body></html>"))
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/ui/styles.py` & `pyguiadapter-0.3.0/pyguiadapter/ui/styles.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DEFAULT_DOCUMENT_FONT_FAMILY = "Arial, sans-serif"
 DEFAULT_DOCUMENT_BG_COLOR = "#FFFFFF"
 DEFAULT_DOCUMENT_TEXT_COLOR = "#000000"
 DEFAULT_DOCUMENT_FONT_SIZE = 16
 
 
-TEXT_EDIT_STYLESHEET = """
+TEXTEDIT_STYLESHEET = """
 QTextEdit{
     background-color: ${bg_color};
     color: ${text_color};
     font-family: ${font_family};
     font-size: ${font_size}px;
 }
 QScrollBar::vertical{
@@ -42,20 +42,20 @@
 }
 QScrollBar::add-page:vertical{
     border:none;
 }
 """
 
 
-def get_text_edit_stylesheet(
+def get_textedit_stylesheet(
     bg_color: str = DEFAULT_OUTPUT_BG_COLOR,
     text_color: str = DEFAULT_OUTPUT_TEXT_COLOR,
     font_family: str = DEFAULT_OUTPUT_FONT_FAMILY,
     font_size: int = DEFAULT_OUTPUT_FONT_SIZE,
 ):
-    css = string.Template(TEXT_EDIT_STYLESHEET).substitute(
+    css = string.Template(TEXTEDIT_STYLESHEET).substitute(
         bg_color=bg_color,
         text_color=text_color,
         font_family=font_family,
         font_size=font_size,
     )
     return css.strip()
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/ui/window/execution.py` & `pyguiadapter-0.3.0/pyguiadapter/ui/window/func_execution/impl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,379 +1,360 @@
-import dataclasses
-import enum
-from typing import Any, Tuple, Callable, Optional, List, Dict
+import warnings
+from typing import Any, Optional, List, Dict, Callable
 
 from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QCloseEvent, QTextCursor, QTextOption
 from PyQt6.QtWidgets import (
-    QMainWindow,
     QVBoxLayout,
     QSpacerItem,
     QSizePolicy,
     QDockWidget,
-    QMessageBox,
-    QApplication,
     QTextEdit,
 )
 from function2widgets.widget import BaseParameterWidget
 
 from pyguiadapter.adapter.bundle import FunctionBundle
 from pyguiadapter.adapter.executor import FunctionExecutor
-from pyguiadapter.commons import clear_layout, get_widget_factory
-from pyguiadapter.interact import uprint, upopup, ulogging
-from pyguiadapter.interact.upopup import UPopup
-from pyguiadapter.ui.config import WindowConfig
+from pyguiadapter.commons import get_param_widget_factory
+from pyguiadapter.interact import upopup, uprint, ulogging
 from pyguiadapter.ui.generated.ui_execution_window import Ui_ExecutionWindow
-from pyguiadapter.ui.styles import (
-    DEFAULT_OUTPUT_BG_COLOR,
-    DEFAULT_OUTPUT_TEXT_COLOR,
-    DEFAULT_OUTPUT_FONT_FAMILY,
-    DEFAULT_OUTPUT_FONT_SIZE,
-    DEFAULT_DOCUMENT_BG_COLOR,
-    DEFAULT_DOCUMENT_TEXT_COLOR,
-    DEFAULT_DOCUMENT_FONT_FAMILY,
-    DEFAULT_DOCUMENT_FONT_SIZE,
+from pyguiadapter.ui.utils import (
+    setup_textedit_stylesheet,
+    set_textedit_text,
+    clear_layout,
+)
+from .base import BaseExecutionWindow
+from .config import DockWidgetState, DockConfig, ExecutionWindowConfig
+from .constants import (
+    BUSY_MSG,
+    BUSY_DIALOG_TITLE,
+    DOCK_SIZES,
+    SOLE_WINDOW_SIZE,
+    ParamInfoType,
+)
+from .context import ExecutionContext
+from .exceptions import (
+    SetParameterValueError,
+    NoSuchParameterError,
+    FunctionNotCancelableError,
+    FunctionNotExecutingError,
 )
-from pyguiadapter.ui.utils import setup_text_edit_stylesheet, set_text_edit_text
-
-
-class DockWidgetState(enum.Enum):
-    Shown = 0
-    Hidden = 1
-    Floating = 3
-
-
-@dataclasses.dataclass
-class DockConfig(object):
-    title: Optional[str] = None
-    state: DockWidgetState = DockWidgetState.Shown
-    floating_size: Tuple[int, int] = dataclasses.field(default=(400, 600))
-
-
-@dataclasses.dataclass
-class ExecutionWindowConfig(WindowConfig):
-
-    tabify_docks: bool = True
-    output_dock_config: DockConfig = DockConfig()
-    document_dock_config: DockConfig = DockConfig()
-
-    parameters_groupbox_title: Optional[str] = None
-    auto_clear_checkbox_text: Optional[str] = None
-    execute_button_text: Optional[str] = None
-    clear_button_text: Optional[str] = None
-
-    output_font_family: str = DEFAULT_OUTPUT_FONT_FAMILY
-    output_font_size: int = DEFAULT_OUTPUT_FONT_SIZE
-    output_bg_color: str = DEFAULT_OUTPUT_BG_COLOR
-    output_text_color: str = DEFAULT_OUTPUT_TEXT_COLOR
-
-    document_font_family: str = DEFAULT_DOCUMENT_FONT_FAMILY
-    document_font_size: int = DEFAULT_DOCUMENT_FONT_SIZE
-    document_bg_color: str = DEFAULT_DOCUMENT_BG_COLOR
-    document_text_color: str = DEFAULT_DOCUMENT_TEXT_COLOR
-
-    auto_clear_output: bool = True
-
-    print_function_result: bool = True
-    function_result_message: str = QApplication.tr("Function result returned: {}")
-    show_function_result_dialog: bool = True
-    function_result_dialog_title: str = QApplication.tr("Function Result")
-    function_result_dialog_message: str = QApplication.tr(
-        "Function result returned: {}"
-    )
-
-    print_function_started_info: bool = True
-    function_started_message: str = QApplication.tr("Start to execute function...")
-
-    print_function_finished_info: bool = True
-    function_finished_message: str = QApplication.tr("Function finished.")
-
-    show_function_error_dialog: bool = True
-    function_error_dialog_title: str = QApplication.tr("Function Exception")
-    function_error_dialog_message: str = QApplication.tr(
-        "A exception raised during the function execution: {}"
-    )
-    print_function_error_info: bool = True
-    function_error_message: str = QApplication.tr(
-        "A exception raised during the function execution: {}"
-    )
-
-    timestamp: bool = True
-    timestamp_pattern: str = "%Y-%m-%d %H:%M:%S"
-
-    def apply_to(self, w: "ExecutionWindow") -> None:
-        super().apply_to(w)
 
 
-class ExecutionWindow(QMainWindow):
+class ExecutionWindow(BaseExecutionWindow):
     def __init__(
         self,
-        function: FunctionBundle,
-        window_config: ExecutionWindowConfig = None,
-        created_callback: Callable[["ExecutionWindow"], None] = None,
+        func_bundle: FunctionBundle,
+        config: ExecutionWindowConfig = None,
+        callback_window_created: Callable[["ExecutionWindow"], None] = None,
         parent=None,
     ):
-        window_config = window_config or ExecutionWindowConfig()
 
         super().__init__(parent=parent)
 
-        self._function = function
-        self._window_config = window_config
-        self._ui = Ui_ExecutionWindow()
+        self._func_bundle = func_bundle
+        self._config = config or ExecutionWindowConfig()
+        self._callback_window_created = callback_window_created
 
-        self._parameter_widgets: List[BaseParameterWidget] = []
+        self._ui = Ui_ExecutionWindow()
 
-        self._layout_parameter_widgets = QVBoxLayout()
+        self._param_widgets: List[BaseParameterWidget] = []
+        self._layout_param_widgets = QVBoxLayout()
 
         self._executor: Optional[FunctionExecutor] = None
-
-        self._created_callback = created_callback
-
-        self._upopup = UPopup(self)
+        self._execution_ctx: ExecutionContext = ExecutionContext(self)
 
         self._setup_ui()
-        self.window_config = window_config
-
-        self._setup_parameter_widgets()
+        self._setup_param_widgets()
+        self.window_config = config
 
+        self._upopup = upopup.UPopup(self)
         uprint.set_print_destination(self.append_output)
         upopup.set_current_window(self)
 
-        if self._created_callback is not None:
-            self._created_callback(self)
+        if self._callback_window_created is not None:
+            self._callback_window_created(self)
 
     @property
-    def popup(self) -> UPopup:
+    def popup(self) -> upopup.UPopup:
         return self._upopup
 
     @property
     def window_config(self) -> ExecutionWindowConfig:
-        return self._window_config
+        return self._config
 
     @window_config.setter
-    def window_config(self, window_config: ExecutionWindowConfig):
-        if not isinstance(window_config, ExecutionWindowConfig):
-            raise TypeError(
-                f"window_config must be an instance of ExecutionWindowConfig, got {type(window_config)}"
-            )
-        self._window_config = window_config
-        self._window_config.apply_to(self)
+    def window_config(self, config: ExecutionWindowConfig):
+        if not isinstance(config, ExecutionWindowConfig):
+            raise TypeError(f"config must be ExecutionWindowConfig, got {type(config)}")
+        self._config = config
+        self._config.apply_basic_configs(self)
+
+    def is_func_executing(self):
+        return self._executor is not None and self._executor.isRunning()
+
+    def get_func(self) -> Callable:
+        return self._func_bundle.func_obj
+
+    def is_func_cancelable(self) -> bool:
+        return self._func_bundle.cancelable
 
     def clear_output(self, force: bool = False):
-        if self._is_busy() and not force:
+        if self.is_func_executing() and not force:
             self._alert_busy()
             return
         self._ui.textedit_output.clear()
 
+    def cancel_executing(self):
+        if not self._func_bundle.cancelable:
+            raise FunctionNotCancelableError("function is not cancelable")
+        if not self.is_func_executing():
+            raise FunctionNotExecutingError("function is not executing now")
+        self._cancel_executing()
+
     def append_output(self, text: str, html: bool = False):
         if text and not html:
             self._ui.textedit_output.insertPlainText(text)
             return
         cursor: QTextCursor = self._ui.textedit_output.textCursor()
         if text:
             cursor.insertHtml(f"<div>{text}</div>")
         cursor.insertHtml("<br>")
         self._ui.textedit_output.ensureCursorVisible()
         self._ui.textedit_output.moveCursor(QTextCursor.MoveOperation.End)
-        # if not text:
-        #     self._ui.textedit_output.append("\n")
-        # else:
-        #     self._ui.textedit_output.append(text)
 
-    def set_parameter_values(
-        self, arguments: Dict[str, Any], ignore_exceptions: bool = False
+    def get_params_info(self) -> Dict[str, ParamInfoType]:
+        return {
+            p.name: (p.typename, p.type_extras)
+            for p in self._func_bundle.func_info.parameters
+        }
+
+    def get_param_values(self) -> Dict[str, Any]:
+        return {
+            param_widget.parameter_name: param_widget.get_value()
+            for param_widget in self._param_widgets
+        }
+
+    def get_param_value(self, param_name: str) -> Any:
+        param_widget = None
+        for widget in self._param_widgets:
+            if widget.parameter_name == param_name:
+                param_widget = widget
+        if param_widget:
+            raise NoSuchParameterError(f"no such parameter {param_name}")
+        return param_widget.get_value()
+
+    def set_param_value(self, param_name: str, value: Any):
+        param_widget = None
+        for widget in self._param_widgets:
+            if widget.parameter_name == param_name:
+                param_widget = widget
+        if param_widget:
+            raise NoSuchParameterError(f"no such parameter {param_name}")
+        return param_widget.set_value(value)
+
+    def set_param_values(
+        self, param_values: Dict[str, Any], ignore_exception: bool = False
     ):
-        if self._is_busy():
-            self._alert_busy()
-            return
-        for widget in self._parameter_widgets:
-            parameter_name = widget.parameter_name
-            if parameter_name not in arguments:
+        # if self.is_func_executing():
+        #     self._alert_busy()
+        #     return
+        for widget in self._param_widgets:
+            param_name = widget.parameter_name
+            if param_name not in param_values:
                 continue
-            arg = arguments[parameter_name]
+            arg = param_values[param_name]
             try:
                 widget.set_value(arg)
             except BaseException as e:
-                msg = QApplication.tr(
-                    f"Can not value of of parameter '{parameter_name}'!\n\n  {e}"
-                )
-                QMessageBox.critical(self, QApplication.tr("Error"), msg)
-                if not ignore_exceptions:
-                    break
+                msg = self.tr(f"failed to set value for parameter {param_name}: {e}")
+                if not ignore_exception:
+                    raise SetParameterValueError(msg) from e
+                else:
+                    warnings.warn(msg)
+
+    @property
+    def execution_context(self) -> Any:
+        return self._execution_ctx
 
     def execute_function(self):
-        if self._is_busy():
+        if self.is_func_executing():
             self._alert_busy()
             return
         if self._executor is not None:
             self._executor.deleteLater()
             self._executor = None
-        arguments = self._get_arguments()
-        self._executor = FunctionExecutor(function=self._function, arguments=arguments)
-        self._executor.started.connect(self._on_function_started)
-        self._executor.finished.connect(self._on_function_finished)
-        self._executor.exception_occurred.connect(self._on_function_error)
-        self._executor.result_ready.connect(self._on_function_result)
-        self._before_function_execution()
+        arguments = self.get_param_values()
+        self._executor = FunctionExecutor(
+            func_bundle=self._func_bundle, arguments=arguments
+        )
+        self._executor.started.connect(self._on_func_started)
+        self._executor.finished.connect(self._on_func_finished)
+        self._executor.exception_occurred.connect(self._on_func_error)
+        self._executor.result_ready.connect(self._on_func_result)
+        self._before_func_execute()
         self._executor.start()
 
     def closeEvent(self, event: QCloseEvent):
-        if self._is_busy():
+        if self.is_func_executing():
             self._alert_busy()
             event.ignore()
             return
 
         self._close_all_docks()
-        clear_layout(self._layout_parameter_widgets)
-        self._cleanup_parameter_widgets()
+        clear_layout(self._layout_param_widgets)
+        self._cleanup_param_widgets()
         event.accept()
 
-    def _before_function_execution(self):
+    def _before_func_execute(self):
         self._ui.button_execute.setEnabled(False)
         self._ui.button_clear.setEnabled(False)
-        if self._ui.checkbox_auto_clear.isChecked():
+        if self._ui.checkbox_autoclear.isChecked():
             self.clear_output()
 
-    def _on_function_started(self):
-        if self.window_config.print_function_started_info:
-            if self.window_config.function_started_message:
-                message = self.window_config.function_started_message.format(
-                    self._function.function.__name__
+    def _on_func_started(self):
+        if self._func_bundle.cancelable:
+            self._ui.button_cancel.setEnabled(True)
+
+        if self.window_config.print_func_start_msg:
+            if self.window_config.func_start_msg:
+                msg = self.window_config.func_start_msg.format(
+                    self._func_bundle.func_obj.__name__
                 )
-                self._ulogging_info(message)
+                self.ulogging_info(msg)
+
+    def _on_func_finished(self):
+        if self._func_bundle.cancelable:
+            self._ui.button_cancel.setEnabled(False)
 
-    def _on_function_finished(self):
         if self._executor is not None:
             self._executor.deleteLater()
             self._executor = None
         self._ui.button_clear.setEnabled(True)
         self._ui.button_execute.setEnabled(True)
-        if self.window_config.print_function_finished_info:
-            if self.window_config.function_finished_message:
-                message = self.window_config.function_finished_message.format(
-                    self._function.function.__name__
+        if self.window_config.print_func_finish_msg:
+            if self.window_config.func_finish_msg:
+                msg = self.window_config.func_finish_msg.format(
+                    self._func_bundle.func_obj.__name__
                 )
-                self._ulogging_info(message)
+                self.ulogging_info(msg)
 
-    def _on_function_error(self, error: BaseException):
-        if self.window_config.print_function_error_info:
-            if self.window_config.function_error_message:
-                message = self.window_config.function_error_message.format(str(error))
-                self._ulogging_error(message)
-
-        if self.window_config.show_function_error_dialog:
-            if self.window_config.function_error_dialog_message:
-                title = (
-                    self.window_config.function_error_dialog_title
-                    or QApplication.tr("Function Exception")
-                )
-                message = self.window_config.function_error_dialog_message.format(
-                    str(error)
-                )
-                QMessageBox.critical(self, title, message)
+    def _on_func_error(self, error: BaseException):
+        if self.window_config.print_func_error:
+            if self.window_config.func_error_msg:
+                msg = self.window_config.func_error_msg.format(str(error))
+                self.ulogging_critical(msg)
+
+        if self.window_config.show_func_error_dialog:
+            if self.window_config.func_error_dialog_msg:
+                title = self.window_config.func_error_dialog_title
+                msg = self.window_config.func_error_dialog_msg.format(str(error))
+                self.show_critical_dialog(title=title, message=msg)
 
-    def _on_function_result(self, result: Any):
+    def _on_func_result(self, result: Any):
         result = str(result)
-        if self.window_config.print_function_result:
-            if self.window_config.function_result_message:
-                message = self.window_config.function_result_message.format(result)
-                self._ulogging_info(message)
-
-        if self.window_config.show_function_result_dialog:
-            if self.window_config.function_result_dialog_message:
-                title = (
-                    self.window_config.function_result_dialog_title
-                    or QApplication.tr("Function Result")
-                )
-                message = self.window_config.function_result_dialog_message.format(
-                    result
-                )
-                QMessageBox.information(self, title, message)
+        if self.window_config.print_func_result:
+            if self.window_config.func_result_msg:
+                msg = self.window_config.func_result_msg.format(result)
+                self.ulogging_info(msg)
+
+        if self.window_config.show_func_result_dialog:
+            if self.window_config.func_result_dialog_msg:
+                title = self.window_config.func_result_dialog_title
+                msg = self.window_config.func_result_dialog_msg.format(result)
+                self.show_info_dialog(title=title, message=msg)
 
     def _setup_ui(self):
         self._ui.setupUi(self)
-        self._layout_parameter_widgets.setParent(self._ui.scrollarea_content)
-        self._ui.scrollarea_content.setLayout(self._layout_parameter_widgets)
 
-        self._setup_docks()
-        self._set_widgets_text()
-        self._set_function_document()
+        self._layout_param_widgets.setParent(self._ui.scrollarea_content)
+        self._ui.scrollarea_content.setLayout(self._layout_param_widgets)
 
-        self._setup_output_widget()
-        self._setup_document_widget()
+        if self.window_config.param_groupbox_title is not None:
+            self._ui.groupbox_params.setTitle(self.window_config.param_groupbox_title)
 
-        self._ui.checkbox_auto_clear.setChecked(
-            self.window_config.auto_clear_output is True
+        if self.window_config.autoclear_checkbox_text is not None:
+            self._ui.checkbox_autoclear.setText(
+                self.window_config.autoclear_checkbox_text
+            )
+        self._ui.checkbox_autoclear.setChecked(
+            self.window_config.autoclear_output is True
         )
 
+        if self.window_config.execute_button_text is not None:
+            self._ui.button_execute.setText(self.window_config.execute_button_text)
+
+        if self.window_config.cancel_button_text is not None:
+            self._ui.button_cancel.setText(self.window_config.cancel_button_text)
+        if self._func_bundle.cancelable:
+            self._ui.button_cancel.show()
+            self._ui.button_cancel.setEnabled(False)
+            self._ui.button_cancel.clicked.connect(self._cancel_executing)
+        else:
+            self._ui.button_cancel.hide()
+            self._ui.button_cancel.setEnabled(False)
+
+        if self.window_config.clear_button_text is not None:
+            self._ui.button_clear.setText(self.window_config.clear_button_text)
+
+        self._setup_docks()
+        self._set_func_document()
+        self._setup_output_widget()
+        self._setup_document_widget()
+        self._clear_actions()
+        self._setup_menus()
+        self._setup_toolbar()
+
         self._ui.button_clear.clicked.connect(self.clear_output)
         self._ui.button_execute.clicked.connect(self.execute_function)
 
-    def _is_busy(self):
-        return self._executor is not None and self._executor.isRunning()
-
     def _alert_busy(self):
-        msg = self.tr("A function is already running!")
-        QMessageBox.warning(self, self.tr("Error"), msg)
-
-    def _setup_parameter_widgets(self):
-        self._cleanup_parameter_widgets()
-        clear_layout(self._layout_parameter_widgets)
-        self._create_parameter_widgets()
-        self._add_parameter_widgets()
+        self.show_warning_dialog(title=BUSY_DIALOG_TITLE, message=BUSY_MSG)
 
-    def _create_parameter_widgets(self):
-        factory = get_widget_factory()
+    def _setup_param_widgets(self):
+        self._cleanup_param_widgets()
+        clear_layout(self._layout_param_widgets)
+        factory = get_param_widget_factory()
+        # create param widgets
         try:
-            for parameter_description in self._function.function_description.parameters:
-                parameter_widget = factory.create_widget_from_description(
-                    parameter_description
-                )
-                self._parameter_widgets.append(parameter_widget)
+            for param_info in self._func_bundle.func_info.parameters:
+                param_widget = factory.create_widget_for_parameter(param_info)
+                self._param_widgets.append(param_widget)
         except BaseException as e:
-            self._cleanup_parameter_widgets()
+            self._cleanup_param_widgets()
             raise e
-
-    def _add_parameter_widgets(self):
-        for widget in self._parameter_widgets:
-            self._layout_parameter_widgets.addWidget(widget)
-        spacer_item = QSpacerItem(
-            0, 0, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding
+        # add param widgets to layout
+        for widget in self._param_widgets:
+            widget.setParent(self._ui.scrollarea_content)
+            self._layout_param_widgets.addWidget(widget)
+        spacer = QSpacerItem(
+            40, 40, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding
         )
-        self._layout_parameter_widgets.addSpacerItem(spacer_item)
+        self._layout_param_widgets.addSpacerItem(spacer)
 
-    def _cleanup_parameter_widgets(self):
-        for widget in self._parameter_widgets:
+    def _cleanup_param_widgets(self):
+        for widget in self._param_widgets:
             widget.deleteLater()
-        self._parameter_widgets.clear()
-
-    def _get_arguments(self) -> Dict[str, Any]:
-        return {
-            param_widget.parameter_name: param_widget.get_value()
-            for param_widget in self._parameter_widgets
-        }
+        self._param_widgets.clear()
 
     def _setup_docks(self):
         if self.window_config.tabify_docks:
             self._tabify_docks()
-        self.resizeDocks(
-            [self._ui.dockwidget_document, self._ui.dockwidget_output],
-            [460, 460],
-            Qt.Orientation.Horizontal,
-        )
+        docks = (self._ui.dockwidget_document, self._ui.dockwidget_output)
+        self.resizeDocks(docks, DOCK_SIZES, Qt.Orientation.Horizontal)
 
         self._setup_dock(
             self._ui.dockwidget_document, self.window_config.document_dock_config
         )
         self._setup_dock(
             self._ui.dockwidget_output, self.window_config.output_dock_config
         )
 
         if self._all_docks_closed() or self._all_docks_floating():
-            self.resize(460, 600)
+            self.resize(*SOLE_WINDOW_SIZE)
 
     def _tabify_docks(self):
         docks = [self._ui.dockwidget_document, self._ui.dockwidget_output]
         if self.window_config.tabify_docks:
             self.tabifyDockWidget(*docks)
 
     def _all_docks_closed(self):
@@ -400,62 +381,103 @@
             dockwidget.close()
         elif config.state == DockWidgetState.Floating:
             dockwidget.setFloating(True)
             dockwidget.resize(*config.floating_size)
         else:
             dockwidget.show()
 
-    def _set_function_document(self):
-        text = self._function.display_document
-        text_format = self._function.document_format
-        set_text_edit_text(self._ui.textedit_document, text, text_format)
-
-    def _set_widgets_text(self):
-        if self.window_config.parameters_groupbox_title is not None:
-            self._ui.groupbox_parameters.setWindowTitle(
-                self.window_config.parameters_groupbox_title
-            )
-        if self.window_config.auto_clear_checkbox_text is not None:
-            self._ui.checkbox_auto_clear.setText(
-                self.window_config.auto_clear_checkbox_text
-            )
-        if self.window_config.execute_button_text is not None:
-            self._ui.button_execute.setText(self.window_config.execute_button_text)
-        if self.window_config.clear_button_text is not None:
-            self._ui.button_clear.setText(self.window_config.clear_button_text)
+    def _set_func_document(self):
+        text = self._func_bundle.display_document
+        text_format = self._func_bundle.document_format
+        set_textedit_text(self._ui.textedit_document, text, text_format)
 
     def _setup_output_widget(self):
-        setup_text_edit_stylesheet(
+        setup_textedit_stylesheet(
             self._ui.textedit_output,
             bg_color=self.window_config.output_bg_color,
             text_color=self.window_config.output_text_color,
             font_family=self.window_config.output_font_family,
             font_size=self.window_config.output_font_size,
         )
         self._ui.textedit_output.setLineWrapMode(QTextEdit.LineWrapMode.WidgetWidth)
         self._ui.textedit_output.setReadOnly(True)
 
     def _setup_document_widget(self):
-        setup_text_edit_stylesheet(
+        setup_textedit_stylesheet(
             self._ui.textedit_document,
             bg_color=self.window_config.document_bg_color,
             text_color=self.window_config.document_text_color,
             font_family=self.window_config.document_font_family,
             font_size=self.window_config.document_font_size,
         )
         self._ui.textedit_document.setLineWrapMode(QTextEdit.LineWrapMode.WidgetWidth)
         self._ui.textedit_document.setWordWrapMode(QTextOption.WrapMode.WordWrap)
         self._ui.textedit_document.setReadOnly(True)
+        self._ui.textedit_document.setOpenExternalLinks(True)
 
-    def _ulogging_info(self, message: str):
+    def _clear_actions(self):
+        self._actions.clear()
+
+    def _setup_menus(self):
+        self._ui.menubar.clear()
+        if not self.window_config.enable_menubar_actions or not self._func_bundle.menus:
+            self._ui.menubar.hide()
+            return
+        self._ui.menubar.show()
+        self._create_menus(self._ui.menubar, self._func_bundle.menus)
+
+    def _setup_toolbar(self):
+        self._ui.toolbar.clear()
+        if (
+            not self.window_config.enable_toolbar_actions
+            or not self._func_bundle.toolbar_actions
+        ):
+            self._ui.toolbar.hide()
+            return
+        self._ui.toolbar.show()
+        self._create_toolbar_actions(
+            self._ui.toolbar, self._func_bundle.toolbar_actions
+        )
+
+    def _cancel_executing(self):
+        if not self.is_func_executing():
+            title = self.tr("Info")
+            msg = self.tr("function is not executing!")
+            self.show_info_dialog(title=title, message=msg)
+            return
+        if self._executor is not None:
+            self._executor.cancel_requested.emit()
+
+    def ulogging_info(self, message: str):
         ulogging.info(
             message,
             timestamp=self.window_config.timestamp,
             timestamp_pattern=self.window_config.timestamp_pattern,
         )
 
-    def _ulogging_error(self, message):
+    def ulogging_critical(self, message):
         ulogging.critical(
             message,
             timestamp=self.window_config.timestamp,
             timestamp_pattern=self.window_config.timestamp_pattern,
         )
+
+    def ulogging_fatal(self, message):
+        ulogging.fatal(
+            message,
+            timestamp=self.window_config.timestamp,
+            timestamp_pattern=self.window_config.timestamp_pattern,
+        )
+
+    def ulogging_debug(self, message):
+        ulogging.debug(
+            message,
+            timestamp=self.window_config.timestamp,
+            timestamp_pattern=self.window_config.timestamp_pattern,
+        )
+
+    def ulogging_warning(self, message):
+        ulogging.warning(
+            message,
+            timestamp=self.window_config.timestamp,
+            timestamp_pattern=self.window_config.timestamp_pattern,
+        )
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/ui/window/initialization.py` & `pyguiadapter-0.3.0/pyguiadapter/ui/window/class_init/impl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,181 +1,151 @@
-import dataclasses
 from typing import Type, Any, Callable, Optional, List, Dict
 
 from PyQt6.QtWidgets import (
     QDialog,
     QVBoxLayout,
     QSpacerItem,
     QSizePolicy,
-    QMessageBox,
 )
-from function2widgets.description import FunctionDescription
-from function2widgets.widget import BaseParameterWidget
+from function2widgets import FunctionInfo, BaseParameterWidget
 
-from pyguiadapter.commons import (
-    T,
-    clear_layout,
-    get_widget_factory,
-    get_function_parser,
-)
+from pyguiadapter.commons import T, get_param_widget_factory, get_function_parser
 from pyguiadapter.interact import upopup
-from pyguiadapter.interact.upopup import UPopup
-from pyguiadapter.ui.config import WindowConfig
-from pyguiadapter.ui.generated.ui_initialization_window import Ui_InitializationWindow
-
-
-@dataclasses.dataclass
-class InitializationWindowConfig(WindowConfig):
-    label_text: Optional[str] = None
-    button_text: Optional[str] = None
-
-    def apply_to(self, w: "InitializationWindow") -> None:
-        super().apply_to(w)
-        if self.label_text is not None:
-            w.set_label_text(self.label_text)
-        if self.button_text is not None:
-            w.set_button_text(self.button_text)
+from pyguiadapter.ui.generated.ui_class_init_window import Ui_ClassInitWindow
+from pyguiadapter.ui.utils import clear_layout, show_critical_dialog
+from .config import ClassInitWindowConfig
+from .constants import CLASS_INIT_FAILED_MSG, ERROR_DIALOG_TITLE
 
 
-class InitializationWindow(QDialog):
+class ClassInitWindow(QDialog):
     def __init__(
         self,
         klass: Type[T],
-        window_config: InitializationWindowConfig = None,
-        window_created_callback: Optional[
-            Callable[["InitializationWindow"], None]
-        ] = None,
+        config: ClassInitWindowConfig = None,
+        callback_window_created: Optional[Callable[["ClassInitWindow"], None]] = None,
         parent=None,
     ):
-        window_config = window_config or InitializationWindowConfig()
+        config = config or ClassInitWindowConfig()
 
         super().__init__(parent=parent)
 
+        self._callback_window_created = callback_window_created
+        self._config: ClassInitWindowConfig = config
+
         self._class: Type[T] = klass
         self._class_instance: Optional[T] = None
-        self._parameter_widgets: List[BaseParameterWidget] = []
-        self._layout_parameter_widgets = QVBoxLayout()
-
-        self._window_create_callback = window_created_callback
-
-        self._ui = Ui_InitializationWindow()
-        self._window_config: InitializationWindowConfig = window_config
 
-        self._upopup = UPopup(self)
+        self._param_widgets: List[BaseParameterWidget] = []
+        self._layout_param_widgets = QVBoxLayout()
+        self._ui = Ui_ClassInitWindow()
 
+        self._upopup = upopup.UPopup(self)
+        upopup.set_current_window(self)
+        self.window_config = config
         self._setup_ui()
-        self.window_config = window_config
-
         self._setup_parameter_widgets()
 
-        upopup.set_current_window(self)
-
-        if self._window_create_callback is not None:
-            self._window_create_callback(self)
+        if self._callback_window_created is not None:
+            self._callback_window_created(self)
 
     @property
-    def popup(self) -> UPopup:
+    def popup(self) -> upopup.UPopup:
         return self._upopup
 
     @property
-    def window_config(self) -> InitializationWindowConfig:
-        return self._window_config
+    def window_config(self) -> ClassInitWindowConfig:
+        return self._config
 
     @window_config.setter
-    def window_config(self, window_config: InitializationWindowConfig):
-        if not isinstance(window_config, InitializationWindowConfig):
+    def window_config(self, config: ClassInitWindowConfig):
+        if not isinstance(config, ClassInitWindowConfig):
             raise TypeError(
-                f"window_config must be an instance of InitializationWindowConfig, got {type(window_config)}"
+                f"window_config must be an instance of InitializationWindowConfig, got {type(config)}"
             )
-        self._window_config = window_config
-        self._window_config.apply_to(self)
-
-    def set_label_text(self, text: str):
-        self._ui.label.setText(text)
-
-    def set_button_text(self, text: str):
-        self._ui.button_initialize.setText(text)
+        self._config = config
+        self._config.apply_basic_configs(self)
 
     def get_class_instance(self) -> Optional[T]:
         return self._class_instance
 
     @classmethod
     def initialize_class(
         cls,
         klass: Type[T],
-        window_config: InitializationWindowConfig = None,
-        window_created_callback: Optional[
-            Callable[["InitializationWindow"], None]
-        ] = None,
+        config: ClassInitWindowConfig = None,
+        callback_window_created: Optional[Callable[["ClassInitWindow"], None]] = None,
         parent=None,
     ) -> Optional[T]:
         _window = cls(
             klass=klass,
-            window_config=window_config,
-            window_created_callback=window_created_callback,
+            config=config,
+            callback_window_created=callback_window_created,
             parent=parent,
         )
         ret = _window.exec()
         if ret == QDialog.DialogCode.Accepted:
             _instance = _window.get_class_instance()
         else:
             _instance = None
         return _instance
 
     def _setup_ui(self):
         self._ui.setupUi(self)
-        self._layout_parameter_widgets.setParent(self._ui.param_widgets_container)
-        self._ui.param_widgets_container.setLayout(self._layout_parameter_widgets)
+        self._layout_param_widgets.setParent(self._ui.param_widgets_container)
+        self._ui.param_widgets_container.setLayout(self._layout_param_widgets)
 
-        self._ui.button_initialize.clicked.connect(self._do_initialization)
+        button_text = self.window_config.init_button_text
+        if button_text:
+            self._ui.button_initialize.setText(button_text)
+        self._ui.button_initialize.clicked.connect(self._do_class_init)
+
+        label_text = self.window_config.title_label_text
+        if label_text:
+            self._ui.label_title.setText(label_text)
 
-    def _do_initialization(self):
+    def _do_class_init(self):
         arguments = self._get_arguments()
         try:
             self._class_instance = self._class(**arguments)
             self.accept()
         except BaseException as e:
             self._class_instance = None
-            msg = self.tr(f"Failed to initialize class {self._class}!\n\nError: \n{e}")
-            QMessageBox.critical(self, self.tr("Error"), msg)
+            msg = CLASS_INIT_FAILED_MSG + "\n\n" + str(e)
+            show_critical_dialog(self, title=ERROR_DIALOG_TITLE, message=msg)
             return
 
     def _setup_parameter_widgets(self):
-        self._cleanup_parameter_widgets()
-        clear_layout(self._layout_parameter_widgets)
+        self._cleanup_param_widgets()
+        clear_layout(self._layout_param_widgets)
         parser = get_function_parser()
-        constructor_description = parser.parse(
-            func=self._class, parse_class=True, ignore_self_param=True
-        )
-        self._create_parameter_widgets(constructor_description)
-        self._add_parameter_widgets()
+        init_func_info = parser.parse(func_obj=self._class, ignore_self_param=True)
+        self._create_param_widgets(init_func_info)
+        self._add_param_widgets()
 
-    def _create_parameter_widgets(self, function_description: FunctionDescription):
-        factory = get_widget_factory()
+    def _create_param_widgets(self, function_info: FunctionInfo):
+        factory = get_param_widget_factory()
         try:
-            for parameter_description in function_description.parameters:
-                parameter_widget = factory.create_widget_from_description(
-                    parameter_description
-                )
-                self._parameter_widgets.append(parameter_widget)
+            for param_info in function_info.parameters:
+                param_widget = factory.create_widget_for_parameter(param_info)
+                self._param_widgets.append(param_widget)
         except BaseException as e:
-            self._cleanup_parameter_widgets()
+            self._cleanup_param_widgets()
             raise e
 
-    def _add_parameter_widgets(self):
-        for widget in self._parameter_widgets:
-            self._layout_parameter_widgets.addWidget(widget)
-        spacer_item = QSpacerItem(
+    def _add_param_widgets(self):
+        for widget in self._param_widgets:
+            self._layout_param_widgets.addWidget(widget)
+        spacer = QSpacerItem(
             0, 0, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding
         )
-        self._layout_parameter_widgets.addSpacerItem(spacer_item)
+        self._layout_param_widgets.addSpacerItem(spacer)
 
-    def _cleanup_parameter_widgets(self):
-        for widget in self._parameter_widgets:
+    def _cleanup_param_widgets(self):
+        for widget in self._param_widgets:
             widget.deleteLater()
-        self._parameter_widgets.clear()
+        self._param_widgets.clear()
 
     def _get_arguments(self) -> Dict[str, Any]:
         return {
             param_widget.parameter_name: param_widget.get_value()
-            for param_widget in self._parameter_widgets
+            for param_widget in self._param_widgets
         }
```

### Comparing `pyguiadapter-0.2.9/pyguiadapter/ui/window/selection.py` & `pyguiadapter-0.3.0/pyguiadapter/ui/window/func_selection/impl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,218 +1,195 @@
-import dataclasses
+import os.path
 import os.path
 import warnings
-from typing import Callable, List, Optional
+from typing import List, Optional, Callable
 
 from PyQt6.QtCore import QSize, Qt
-from PyQt6.QtGui import QIcon, QCloseEvent, QTextOption
+from PyQt6.QtGui import QIcon, QTextOption
 from PyQt6.QtWidgets import (
     QMainWindow,
     QListWidget,
     QListWidgetItem,
-    QMessageBox,
     QTextEdit,
 )
 
-from pyguiadapter.adapter.bundle import FunctionBundle, DEFAULT_ICON
+from pyguiadapter.adapter.bundle import FunctionBundle
+from pyguiadapter.adapter.constants import DEFAULT_ICON
 from pyguiadapter.commons import get_icon_file
 from pyguiadapter.ui.config import WindowConfig
 from pyguiadapter.ui.generated.ui_selection_window import Ui_SelectionWindow
-from pyguiadapter.ui.styles import (
-    DEFAULT_DOCUMENT_FONT_FAMILY,
-    DEFAULT_DOCUMENT_FONT_SIZE,
-    DEFAULT_DOCUMENT_BG_COLOR,
-    DEFAULT_DOCUMENT_TEXT_COLOR,
+from pyguiadapter.ui.utils import setup_textedit_stylesheet, set_textedit_text
+from pyguiadapter.ui.utils import (
+    show_critical_dialog,
+    show_warning_dialog,
+)
+from pyguiadapter.ui.window.func_execution import ExecutionWindow
+from .config import SelectionWindowConfig
+from .constants import (
+    DEFAULT_SPLIT_SIZE,
+    ERROR_DIALOG_TITLE,
+    WARNING_DIALOG_TITLE,
+    NO_FUNC_SELECTED_MSG,
 )
-from pyguiadapter.ui.utils import setup_text_edit_stylesheet, set_text_edit_text
-from pyguiadapter.ui.window.execution import ExecutionWindow
-
-
-@dataclasses.dataclass
-class SelectionWindowConfig(WindowConfig):
-    icon_mode: bool = True
-    icon_size: Optional[int] = 48
-    functions_label_text: Optional[str] = None
-    document_label_text: Optional[str] = None
-    select_button_text: Optional[str] = None
-
-    document_font_family: str = DEFAULT_DOCUMENT_FONT_FAMILY
-    document_font_size: int = DEFAULT_DOCUMENT_FONT_SIZE
-    document_bg_color: str = DEFAULT_DOCUMENT_BG_COLOR
-    document_text_color: str = DEFAULT_DOCUMENT_TEXT_COLOR
-
-    def apply_to(self, w: "SelectionWindow") -> None:
-        super().apply_to(w)
 
 
 class SelectionWindow(QMainWindow):
     def __init__(
         self,
-        functions: List[FunctionBundle],
-        window_config: Optional[SelectionWindowConfig] = None,
-        execution_window_config: Optional[WindowConfig] = None,
-        window_created_callback: Optional[Callable[[QMainWindow], None]] = None,
-        execution_window_created_callback: Optional[
+        func_bundles: List[Callable],
+        config: Optional[SelectionWindowConfig] = None,
+        config_execution_window: Optional[WindowConfig] = None,
+        callback_window_created: Optional[Callable[[QMainWindow], None]] = None,
+        callback_execution_window_created: Optional[
             Callable[[ExecutionWindow], None]
         ] = None,
         parent=None,
     ):
 
-        window_config = window_config or SelectionWindowConfig()
-
         super().__init__(parent=parent)
 
-        self._functions = [*functions]
-        self._window_config = window_config
-        self._execution_window_config = execution_window_config
-
+        self._func_bundles = [*func_bundles]
+        self._config = config or SelectionWindowConfig()
+        self._callback_window_created = callback_window_created
         self._ui = Ui_SelectionWindow()
 
-        self._window_created_callback = window_created_callback
-
+        self._config_execution_window = config_execution_window
+        self._callback_execution_window_created = callback_execution_window_created
         self._execution_window: Optional[ExecutionWindow] = None
-        self._execution_window_started_callback = execution_window_created_callback
 
         self._setup_ui()
-        self.window_config = window_config
+        self.window_config = config
+        self._setup_func_listwidget()
 
-        self._setup_functions_listwidget()
-
-        if self._window_created_callback is not None:
-            self._window_created_callback(self)
+        if self._callback_window_created is not None:
+            self._callback_window_created(self)
 
     @property
     def window_config(self) -> SelectionWindowConfig:
-        return self._window_config
+        return self._config
 
     @window_config.setter
     def window_config(self, window_config: SelectionWindowConfig):
         if not isinstance(window_config, SelectionWindowConfig):
             raise TypeError(
                 f"window_config must be an instance of SelectionWindowConfig, got {type(window_config)}"
             )
-        self._window_config = window_config
-        self._window_config.apply_to(self)
-
-    def closeEvent(self, event: QCloseEvent):
-        super().closeEvent(event)
+        self._config = window_config
+        self._config.apply_basic_configs(self)
 
     def _setup_ui(self):
         self._ui.setupUi(self)
 
-        self._ui.splitter.setSizes([200, 300])
+        self._ui.splitter.setSizes(DEFAULT_SPLIT_SIZE)
 
-        if not self._functions:
+        if not self._func_bundles:
             self._ui.button_select.setEnabled(False)
         else:
             self._ui.button_select.setEnabled(True)
 
         self._ui.listwidget_functions.currentItemChanged.connect(
             self._on_current_item_changed
         )
 
         self._set_view_mode()
         self._setup_document_widget()
 
-        self._set_functions_label_text()
-        self._set_document_label_text()
-        self._set_select_button_text()
+        text = self.window_config.func_list_label_text
+        if text is not None:
+            self._ui.label_func_list.setText(text)
+
+        text = self.window_config.document_label_text
+        if text is not None:
+            self._ui.label_document.setText(text)
+
+        text = self.window_config.select_button_text
+        if text is not None:
+            self._ui.button_select.setText(text)
 
-        self._ui.button_select.clicked.connect(self._on_open_execution_window)
+        self._ui.button_select.clicked.connect(self._open_execution_window)
+        self._ui.listwidget_functions.itemDoubleClicked.connect(
+            self._open_execution_window
+        )
 
     def _on_current_item_changed(self, item: QListWidgetItem):
         if not item:
             self._ui.button_select.setEnabled(False)
             self._ui.textedit_document.setText("")
         else:
             self._ui.button_select.setEnabled(True)
-            self._set_function_document(function=item.data(Qt.ItemDataRole.UserRole))
+            self._set_document(function=item.data(Qt.ItemDataRole.UserRole))
 
-    def _on_open_execution_window(self):
+    def _open_execution_window(self):
         current_item = self._ui.listwidget_functions.currentItem()
         if not current_item:
-            QMessageBox.warning(
-                self, self.tr("Warn"), self.tr("please select a function first!")
+            show_warning_dialog(
+                self, title=WARNING_DIALOG_TITLE, message=NO_FUNC_SELECTED_MSG
             )
             return
-        function = current_item.data(Qt.ItemDataRole.UserRole)
+        func_bundle = current_item.data(Qt.ItemDataRole.UserRole)
         if self._execution_window is not None:
             self._execution_window.close()
             self._execution_window.deleteLater()
             self._execution_window = None
         try:
             self._execution_window = ExecutionWindow(
-                function=function,
-                window_config=self._execution_window_config,
-                created_callback=self._execution_window_started_callback,
+                func_bundle=func_bundle,
+                config=self._config_execution_window,
+                callback_window_created=self._callback_execution_window_created,
                 parent=self,
             )
         except BaseException as e:
-            QMessageBox.critical(self, self.tr("Error"), str(e))
+            show_critical_dialog(self, title=ERROR_DIALOG_TITLE, message=str(e))
         else:
             self._execution_window.setWindowModality(Qt.WindowModality.ApplicationModal)
             self._execution_window.show()
 
-    def _set_function_document(self, function: FunctionBundle):
+    def _set_document(self, function: FunctionBundle):
         text = function.display_document
-        set_text_edit_text(self._ui.textedit_document, text, function.document_format)
+        set_textedit_text(self._ui.textedit_document, text, function.document_format)
 
-    def _setup_functions_listwidget(self):
-        self._cleanup_functions_listwidget()
-        for function in self._functions:
-            item = self._create_function_list_item(function)
+    def _setup_func_listwidget(self):
+        self._cleanup_func_listwidget()
+        for function in self._func_bundles:
+            item = self._create_func_listitem(function)
             self._ui.listwidget_functions.addItem(item)
         self._ui.listwidget_functions.setCurrentRow(0)
 
-    def _cleanup_functions_listwidget(self):
+    def _cleanup_func_listwidget(self):
         for i in range(self._ui.listwidget_functions.count()):
             self._ui.listwidget_functions.takeItem(0)
 
     # noinspection PyMethodMayBeStatic
-    def _create_function_list_item(self, function: FunctionBundle) -> QListWidgetItem:
-        icon_path = get_icon_file(function.display_icon)
+    def _create_func_listitem(self, func: FunctionBundle) -> QListWidgetItem:
+        icon_path = get_icon_file(func.display_icon)
         if not os.path.isfile(icon_path):
             warnings.warn(
                 f"icon file not found, use default one instead: '{icon_path}'"
             )
             icon_path = get_icon_file(DEFAULT_ICON)
         icon = QIcon(icon_path)
-        item = QListWidgetItem(icon, function.display_name)
-        item.setData(Qt.ItemDataRole.UserRole, function)
+        item = QListWidgetItem(icon, func.display_name)
+        item.setData(Qt.ItemDataRole.UserRole, func)
         return item
 
-    def _set_functions_label_text(self):
-        text = self.window_config.functions_label_text
-        if text is not None:
-            self._ui.label_functions.setText(text)
-
-    def _set_document_label_text(self):
-        text = self.window_config.document_label_text
-        if text is not None:
-            self._ui.label_document.setText(text)
-
-    def _set_select_button_text(self):
-        text = self.window_config.select_button_text
-        if text is not None:
-            self._ui.button_select.setText(text)
-
     def _set_view_mode(self):
         icon_mode = self.window_config.icon_mode
         icon_size = self.window_config.icon_size
         if icon_mode:
             self._ui.listwidget_functions.setViewMode(QListWidget.ViewMode.IconMode)
             if icon_size is not None:
                 self._ui.listwidget_functions.setIconSize(QSize(icon_size, icon_size))
         else:
             self._ui.listwidget_functions.setViewMode(QListWidget.ViewMode.ListMode)
 
     def _setup_document_widget(self):
-        setup_text_edit_stylesheet(
+        setup_textedit_stylesheet(
             self._ui.textedit_document,
             bg_color=self.window_config.document_bg_color,
             text_color=self.window_config.document_text_color,
             font_family=self.window_config.document_font_family,
             font_size=self.window_config.document_font_size,
         )
         self._ui.textedit_document.setWordWrapMode(QTextOption.WrapMode.WordWrap)
         self._ui.textedit_document.setLineWrapMode(QTextEdit.LineWrapMode.WidgetWidth)
         self._ui.textedit_document.setReadOnly(True)
+        self._ui.textedit_document.setOpenExternalLinks(True)
```

### Comparing `pyguiadapter-0.2.9/pyproject.toml` & `pyguiadapter-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [tool.poetry]
 name = "pyguiadapter"
-version = "0.2.9"
+version = "0.3.0"
 description = "turn (almost) any python functions into a gui in a few lines of code"
 authors = ["zimolab <zimolab@aliyun.com>"]
 readme = "README.md"
 homepage = "https://github.com/zimolab/PyGUIAdapter"
 repository = "https://github.com/zimolab/PyGUIAdapter"
 documentation = "https://github.com/zimolab/PyGUIAdapter"
 
 
 [tool.poetry.scripts]
 autogen = "autouic:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
-function2widgets = ">=0.5.4"
+function2widgets = ">=0.6.15"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 qt-material = "^2.14"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pyguiadapter-0.2.9/README.md` & `pyguiadapter-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 ### [中文](./README_zh.md) | English
 
 A library that makes it easy to convert (almost) any Python functions into a GUI application.
 
 ![PyGUIAdapter](./screenshoots/pyguiadapter_mid.png)
 
+A real world application using this library: [Simple-OTP](https://github.com/zimolab/simple-otp)
+
 ---
 
 ## 1. Quick Start
 
 ### 1.1 Installation
 
 Using pip
@@ -175,17 +177,17 @@
 
 ```
 
 Next, you need to register the widget type you created(`Point2DInput`) to the parameter widget factory. 
 The code might look like this:
 
 ```python
-from pyguiadapter.commons import get_widget_factory
+from pyguiadapter.commons import get_param_widget_factory
 
-factory = get_widget_factory()
+factory = get_param_widget_factory()
 factory.register("Point2DInput", Point2DInput)
 ```
 
 Finally, let PyGUIAdapter know which parameter should use `Point2DInput` as its widget, 
 There are many ways to do this. Here is a brief introduction to one of them, that is, passing the `widget_configs` 
 argument to the `add()` method. The code might look like this:
```

### Comparing `pyguiadapter-0.2.9/PKG-INFO` & `pyguiadapter-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: pyguiadapter
-Version: 0.2.9
+Version: 0.3.0
 Summary: turn (almost) any python functions into a gui in a few lines of code
 Home-page: https://github.com/zimolab/PyGUIAdapter
 Author: zimolab
 Author-email: zimolab@aliyun.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: function2widgets (>=0.5.4)
+Requires-Dist: function2widgets (>=0.6.15)
 Project-URL: Documentation, https://github.com/zimolab/PyGUIAdapter
 Project-URL: Repository, https://github.com/zimolab/PyGUIAdapter
 Description-Content-Type: text/markdown
 
 # PyGUIAdapter
 
 ---
 
 ### [中文](./README_zh.md) | English
 
 A library that makes it easy to convert (almost) any Python functions into a GUI application.
 
 ![PyGUIAdapter](./screenshoots/pyguiadapter_mid.png)
 
+A real world application using this library: [Simple-OTP](https://github.com/zimolab/simple-otp)
+
 ---
 
 ## 1. Quick Start
 
 ### 1.1 Installation
 
 Using pip
@@ -194,17 +196,17 @@
 
 ```
 
 Next, you need to register the widget type you created(`Point2DInput`) to the parameter widget factory. 
 The code might look like this:
 
 ```python
-from pyguiadapter.commons import get_widget_factory
+from pyguiadapter.commons import get_param_widget_factory
 
-factory = get_widget_factory()
+factory = get_param_widget_factory()
 factory.register("Point2DInput", Point2DInput)
 ```
 
 Finally, let PyGUIAdapter know which parameter should use `Point2DInput` as its widget, 
 There are many ways to do this. Here is a brief introduction to one of them, that is, passing the `widget_configs` 
 argument to the `add()` method. The code might look like this:
```

