# Comparing `tmp/netsblox-0.6.7.tar.gz` & `tmp/netsblox-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsblox-0.6.7.tar", last modified: Tue Apr  2 18:56:50 2024, max compression
+gzip compressed data, was "netsblox-0.6.8.tar", last modified: Wed Apr 17 14:41:25 2024, max compression
```

## Comparing `netsblox-0.6.7.tar` & `netsblox-0.6.8.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.566968 netsblox-0.6.7/
--rw-rw-r--   0 devin     (1000) devin     (1000)    11340 2022-02-12 05:03:57.000000 netsblox-0.6.7/LICENSE
--rw-rw-r--   0 devin     (1000) devin     (1000)       53 2023-10-30 19:53:51.000000 netsblox-0.6.7/MANIFEST.in
--rw-r--r--   0 devin     (1000) devin     (1000)     4857 2024-04-02 18:56:50.566968 netsblox-0.6.7/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)     4009 2024-03-17 12:42:56.000000 netsblox-0.6.7/README.md
--rw-rw-r--   0 devin     (1000) devin     (1000)      432 2024-04-02 18:54:26.000000 netsblox-0.6.7/meta.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.546968 netsblox-0.6.7/netsblox/
--rw-rw-r--   0 devin     (1000) devin     (1000)      472 2024-04-02 18:54:31.000000 netsblox-0.6.7/netsblox/__init__.py
--rwxrwxr-x   0 devin     (1000) devin     (1000)       29 2022-03-06 23:53:14.000000 netsblox-0.6.7/netsblox/__main__.py
--rw-rw-r--   0 devin     (1000) devin     (1000)   104349 2024-04-01 19:15:38.000000 netsblox-0.6.7/netsblox/app.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.546968 netsblox-0.6.7/netsblox/assets/
--rw-rw-r--   0 devin     (1000) devin     (1000)    34644 2024-03-29 13:19:04.000000 netsblox-0.6.7/netsblox/assets/default-blocks.json
--rw-rw-r--   0 devin     (1000) devin     (1000)     4371 2022-02-12 05:03:57.000000 netsblox-0.6.7/netsblox/assets/default-imports.json
--rw-rw-r--   0 devin     (1000) devin     (1000)     1069 2024-03-29 13:17:54.000000 netsblox-0.6.7/netsblox/assets/default-project.json
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.546968 netsblox-0.6.7/netsblox/assets/examples/
--rw-rw-r--   0 devin     (1000) devin     (1000)     6332 2024-03-29 13:28:17.000000 netsblox-0.6.7/netsblox/assets/examples/covid-19-daily.json
--rw-rw-r--   0 devin     (1000) devin     (1000)     4896 2024-03-29 13:28:20.000000 netsblox-0.6.7/netsblox/assets/examples/street-view.json
--rw-rw-r--   0 devin     (1000) devin     (1000)     2246 2024-03-29 13:28:25.000000 netsblox-0.6.7/netsblox/assets/examples/weather-app.json
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.542968 netsblox-0.6.7/netsblox/assets/fonts/
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.550968 netsblox-0.6.7/netsblox/assets/fonts/Droid/
--rw-rw-r--   0 devin     (1000) devin     (1000)  3022632 2022-02-12 05:03:57.000000 netsblox-0.6.7/netsblox/assets/fonts/Droid/DroidSansFallback.ttf
--rw-rw-r--   0 devin     (1000) devin     (1000)      791 2022-02-12 05:03:57.000000 netsblox-0.6.7/netsblox/assets/fonts/Droid/README.md
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.542968 netsblox-0.6.7/netsblox/assets/img/
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.542968 netsblox-0.6.7/netsblox/assets/img/blocks/
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.550968 netsblox-0.6.7/netsblox/assets/img/blocks/control/
--rw-rw-r--   0 devin     (1000) devin     (1000)     3335 2024-03-21 14:33:07.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/broadcast.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2998 2024-03-21 16:17:09.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/clone-expr.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3117 2024-03-21 16:16:51.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/clone-stmt.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     4265 2024-03-21 15:20:03.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/if-else-expr.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3566 2024-03-21 15:16:26.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/if-else.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2674 2024-03-21 15:16:11.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/if.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3712 2024-03-21 15:14:00.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/loop-for.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1928 2024-03-21 15:07:31.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/loop-forever.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2551 2024-03-21 15:09:05.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/loop-repeat.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3997 2024-03-21 15:11:28.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/loop-until.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1348 2024-03-21 14:34:57.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/no-yield.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     4111 2024-03-21 14:26:09.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/onkey.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3175 2024-03-21 14:27:18.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/onmouse.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3528 2024-03-21 16:15:01.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/onstart-clone.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2890 2024-03-21 14:24:19.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/onstart.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     4139 2024-03-21 14:32:52.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/receive.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1687 2024-03-21 16:09:16.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/return.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2187 2024-03-21 15:03:47.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/sleep.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1566 2024-03-21 16:12:39.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/throw.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     4056 2024-03-21 16:10:49.000000 netsblox-0.6.7/netsblox/assets/img/blocks/control/try.png
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.550968 netsblox-0.6.7/netsblox/assets/img/blocks/looks/
--rw-rw-r--   0 devin     (1000) devin     (1000)     2997 2024-03-22 03:57:01.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/change-scale.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1761 2024-03-22 03:54:11.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/get-costume-num.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1024 2024-03-22 03:59:06.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/get-scale.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1595 2024-03-22 04:00:41.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/get-visible.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3146 2024-03-22 03:55:12.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/say-duration.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1625 2024-03-22 03:55:51.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/say.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3981 2024-03-22 03:52:26.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/set-costume.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2925 2024-03-22 03:57:28.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/set-scale.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1118 2024-03-22 04:00:25.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/set-visible-false.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1256 2024-03-22 04:00:12.000000 netsblox-0.6.7/netsblox/assets/img/blocks/looks/set-visible-true.png
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.554968 netsblox-0.6.7/netsblox/assets/img/blocks/motion/
--rw-rw-r--   0 devin     (1000) devin     (1000)     2722 2024-03-21 14:04:23.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/change-pos-x.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2746 2024-03-21 14:04:38.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/change-pos-y.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2696 2024-03-21 14:06:20.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/edge-bounce.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2611 2024-03-21 14:02:04.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/forward.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1599 2024-03-21 14:07:10.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/get-heading.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1726 2024-03-21 14:06:41.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/get-pos-x.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1752 2024-03-21 14:06:56.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/get-pos-y.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3175 2024-03-21 14:03:34.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/set-heading.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2032 2024-03-21 14:04:52.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/set-pos-x.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2066 2024-03-21 14:05:08.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/set-pos-y.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2876 2024-03-21 14:04:01.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/set-pos.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2971 2024-03-21 14:03:18.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/turn-left.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2977 2024-03-21 14:02:56.000000 netsblox-0.6.7/netsblox/assets/img/blocks/motion/turn-right.png
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.554968 netsblox-0.6.7/netsblox/assets/img/blocks/network/
--rw-rw-r--   0 devin     (1000) devin     (1000)     5159 2024-03-22 12:36:19.000000 netsblox-0.6.7/netsblox/assets/img/blocks/network/receive.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     5394 2024-03-22 12:45:26.000000 netsblox-0.6.7/netsblox/assets/img/blocks/network/rpc-call.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     5498 2024-03-22 12:48:41.000000 netsblox-0.6.7/netsblox/assets/img/blocks/network/rpc-run.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     5004 2024-03-22 12:39:10.000000 netsblox-0.6.7/netsblox/assets/img/blocks/network/send.png
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.558968 netsblox-0.6.7/netsblox/assets/img/blocks/operators/
--rw-rw-r--   0 devin     (1000) devin     (1000)     1827 2024-03-22 15:15:25.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/add.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2259 2024-03-22 15:27:12.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/and.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1760 2024-03-22 15:17:03.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/div.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1357 2024-03-22 15:21:44.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/eq.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1713 2024-03-22 15:29:03.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/false.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1477 2024-03-22 15:22:19.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/great-eq.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1440 2024-03-22 15:23:50.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/great.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2234 2024-03-22 15:42:33.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/isinstance-list.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2348 2024-03-22 15:45:31.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/isinstance-str.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2388 2024-03-22 15:29:58.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/join.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1488 2024-03-22 15:21:16.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/less-eq.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1435 2024-03-22 15:20:43.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/less.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2151 2024-03-22 15:17:57.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/mod.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1883 2024-03-22 15:16:35.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/mul.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1493 2024-03-22 15:24:17.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/neq.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1687 2024-03-22 15:28:17.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/not.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1876 2024-03-22 15:27:43.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/or.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1783 2024-03-22 15:17:32.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/pow.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3218 2024-03-22 15:10:05.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/randrange.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1992 2024-03-22 15:18:20.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/round.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2820 2024-03-22 15:35:31.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/split-space.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2276 2024-03-22 15:18:44.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/sqrt.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3156 2024-03-22 15:41:30.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-chr.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2732 2024-03-22 15:36:12.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-index-first.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2960 2024-03-22 15:37:42.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-index-last.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3208 2024-03-22 15:38:51.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-index-rand.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2773 2024-03-22 15:39:22.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-len.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2168 2024-03-22 15:39:51.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-ord.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1694 2024-03-22 15:16:11.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/sub.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1631 2024-03-22 15:28:54.000000 netsblox-0.6.7/netsblox/assets/img/blocks/operators/true.png
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.562968 netsblox-0.6.7/netsblox/assets/img/blocks/pen/
--rw-rw-r--   0 devin     (1000) devin     (1000)     3222 2024-03-22 16:53:32.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/change-pen-size.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1127 2024-03-22 16:19:43.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/clear.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1809 2024-03-22 16:21:16.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/get-drawing.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1533 2024-03-22 17:03:23.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/get-drawings.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1801 2024-03-22 16:52:13.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/get-pen-color.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1776 2024-03-22 16:49:46.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/get-pen-size.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1206 2024-03-22 16:21:02.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/set-drawing-false.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1561 2024-03-22 16:20:41.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/set-drawing-true.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2326 2024-03-22 16:23:56.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/set-pen-color.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2553 2024-03-22 16:54:07.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/set-pen-size.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1313 2024-03-22 16:54:42.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/stamp.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2854 2024-03-22 17:01:48.000000 netsblox-0.6.7/netsblox/assets/img/blocks/pen/write.png
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.562968 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/
--rw-rw-r--   0 devin     (1000) devin     (1000)     1349 2024-03-22 04:07:56.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/answer.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3644 2024-03-22 04:06:57.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/ask.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2606 2024-03-22 04:22:35.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-image-self.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2631 2024-03-22 04:21:17.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-image-stage.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3200 2024-03-22 04:24:32.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-key-down.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1829 2024-03-22 04:16:20.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-latitude.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2028 2024-03-22 04:16:30.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-longitude.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1408 2024-03-22 04:10:47.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-mouse-x.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1444 2024-03-22 04:11:05.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-mouse-y.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1913 2024-03-22 04:19:11.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-stage-height.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     1954 2024-03-22 04:19:00.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-stage-width.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3041 2024-03-22 04:04:21.000000 netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-touching.png
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.566968 netsblox-0.6.7/netsblox/assets/img/blocks/variables/
--rw-rw-r--   0 devin     (1000) devin     (1000)     3108 2024-03-22 12:26:16.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-cat.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3060 2024-03-22 12:10:36.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-cdr.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3347 2024-03-22 12:11:42.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-cons.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3095 2024-03-22 12:15:09.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-empty.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     5514 2024-03-22 12:32:02.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-filter.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3494 2024-03-22 12:14:10.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-in.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3137 2024-03-22 12:11:15.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-index-first.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3407 2024-03-22 12:11:01.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-index-last.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3659 2024-03-22 15:55:02.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-index-rand.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     4213 2024-03-22 12:21:53.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-insert-first.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     4484 2024-03-22 12:22:33.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-insert-last.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2933 2024-03-22 12:10:05.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-len.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     5358 2024-03-22 12:30:47.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-map.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3188 2024-03-22 12:18:27.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-push.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3266 2024-03-22 04:34:00.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-range.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3596 2024-03-22 12:20:42.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-remove-all.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3385 2024-03-22 12:19:15.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-remove-first.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3648 2024-03-22 12:19:57.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-remove-last.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     5201 2024-03-22 12:23:50.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-replace-first.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     5442 2024-03-22 12:24:33.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-replace-last.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     3075 2024-03-22 12:09:33.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-rev.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2257 2024-03-22 12:29:27.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-sort.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2305 2024-03-22 04:33:22.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/list.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     4784 2024-03-22 12:17:15.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/loop-foreach.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     2841 2024-03-22 04:31:32.000000 netsblox-0.6.7/netsblox/assets/img/blocks/variables/var-local.png
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.566968 netsblox-0.6.7/netsblox/assets/img/logo/
--rw-rw-r--   0 devin     (1000) devin     (1000)    16709 2022-03-09 09:21:40.000000 netsblox-0.6.7/netsblox/assets/img/logo/logo-256.png
--rw-rw-r--   0 devin     (1000) devin     (1000)     4022 2022-03-09 09:20:32.000000 netsblox-0.6.7/netsblox/assets/img/logo/logo.svg
--rw-rw-r--   0 devin     (1000) devin     (1000)     6563 2022-02-12 05:03:57.000000 netsblox-0.6.7/netsblox/colors.py
--rwxrwxr-x   0 devin     (1000) devin     (1000)    11477 2024-03-29 13:26:02.000000 netsblox-0.6.7/netsblox/common.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     4373 2024-03-21 14:40:26.000000 netsblox-0.6.7/netsblox/concurrency.py
--rw-rw-r--   0 devin     (1000) devin     (1000)   284156 2024-04-02 18:54:32.000000 netsblox-0.6.7/netsblox/dev.py
--rw-rw-r--   0 devin     (1000) devin     (1000)   284152 2024-04-02 18:54:32.000000 netsblox-0.6.7/netsblox/editor.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     1427 2022-02-12 05:03:57.000000 netsblox-0.6.7/netsblox/events.py
--rw-rw-r--   0 devin     (1000) devin     (1000)    67958 2024-04-02 18:45:21.000000 netsblox-0.6.7/netsblox/graphical.py
--rw-rw-r--   0 devin     (1000) devin     (1000)     7801 2022-02-16 19:46:30.000000 netsblox-0.6.7/netsblox/rooms.py
--rw-rw-r--   0 devin     (1000) devin     (1000)    52250 2024-04-02 11:59:10.000000 netsblox-0.6.7/netsblox/snap.py
--rwxrwxr-x   0 devin     (1000) devin     (1000)     7799 2022-03-20 23:37:09.000000 netsblox-0.6.7/netsblox/transform.py
-drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 18:56:50.566968 netsblox-0.6.7/netsblox.egg-info/
--rw-r--r--   0 devin     (1000) devin     (1000)     4857 2024-04-02 18:56:50.000000 netsblox-0.6.7/netsblox.egg-info/PKG-INFO
--rw-rw-r--   0 devin     (1000) devin     (1000)     7108 2024-04-02 18:56:50.000000 netsblox-0.6.7/netsblox.egg-info/SOURCES.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-02 18:56:50.000000 netsblox-0.6.7/netsblox.egg-info/dependency_links.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)      111 2024-04-02 18:56:50.000000 netsblox-0.6.7/netsblox.egg-info/requires.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)        9 2024-04-02 18:56:50.000000 netsblox-0.6.7/netsblox.egg-info/top_level.txt
--rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-02 18:56:50.566968 netsblox-0.6.7/setup.cfg
--rwxrwxr-x   0 devin     (1000) devin     (1000)     1059 2024-03-29 12:54:40.000000 netsblox-0.6.7/setup.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.190870 netsblox-0.6.8/
+-rw-rw-r--   0 devin     (1000) devin     (1000)    11340 2022-02-12 05:03:57.000000 netsblox-0.6.8/LICENSE
+-rw-rw-r--   0 devin     (1000) devin     (1000)       53 2023-10-30 19:53:51.000000 netsblox-0.6.8/MANIFEST.in
+-rw-r--r--   0 devin     (1000) devin     (1000)     4857 2024-04-17 14:41:25.190870 netsblox-0.6.8/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4009 2024-03-17 12:42:56.000000 netsblox-0.6.8/README.md
+-rw-rw-r--   0 devin     (1000) devin     (1000)      432 2024-04-17 14:40:23.000000 netsblox-0.6.8/meta.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.166870 netsblox-0.6.8/netsblox/
+-rw-rw-r--   0 devin     (1000) devin     (1000)      472 2024-04-17 14:40:29.000000 netsblox-0.6.8/netsblox/__init__.py
+-rwxrwxr-x   0 devin     (1000) devin     (1000)       29 2022-03-06 23:53:14.000000 netsblox-0.6.8/netsblox/__main__.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)   105517 2024-04-17 14:37:09.000000 netsblox-0.6.8/netsblox/app.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.166870 netsblox-0.6.8/netsblox/assets/
+-rw-rw-r--   0 devin     (1000) devin     (1000)    34644 2024-03-29 13:19:04.000000 netsblox-0.6.8/netsblox/assets/default-blocks.json
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4371 2022-02-12 05:03:57.000000 netsblox-0.6.8/netsblox/assets/default-imports.json
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1069 2024-03-29 13:17:54.000000 netsblox-0.6.8/netsblox/assets/default-project.json
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.166870 netsblox-0.6.8/netsblox/assets/examples/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     6332 2024-03-29 13:28:17.000000 netsblox-0.6.8/netsblox/assets/examples/covid-19-daily.json
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4896 2024-03-29 13:28:20.000000 netsblox-0.6.8/netsblox/assets/examples/street-view.json
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2246 2024-03-29 13:28:25.000000 netsblox-0.6.8/netsblox/assets/examples/weather-app.json
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.158871 netsblox-0.6.8/netsblox/assets/fonts/
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.170870 netsblox-0.6.8/netsblox/assets/fonts/Droid/
+-rw-rw-r--   0 devin     (1000) devin     (1000)  3022632 2022-02-12 05:03:57.000000 netsblox-0.6.8/netsblox/assets/fonts/Droid/DroidSansFallback.ttf
+-rw-rw-r--   0 devin     (1000) devin     (1000)      791 2022-02-12 05:03:57.000000 netsblox-0.6.8/netsblox/assets/fonts/Droid/README.md
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.158871 netsblox-0.6.8/netsblox/assets/img/
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.158871 netsblox-0.6.8/netsblox/assets/img/blocks/
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.174870 netsblox-0.6.8/netsblox/assets/img/blocks/control/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3335 2024-03-21 14:33:07.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/broadcast.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2998 2024-03-21 16:17:09.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/clone-expr.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3117 2024-03-21 16:16:51.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/clone-stmt.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4265 2024-03-21 15:20:03.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/if-else-expr.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3566 2024-03-21 15:16:26.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/if-else.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2674 2024-03-21 15:16:11.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/if.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3712 2024-03-21 15:14:00.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/loop-for.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1928 2024-03-21 15:07:31.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/loop-forever.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2551 2024-03-21 15:09:05.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/loop-repeat.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3997 2024-03-21 15:11:28.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/loop-until.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1348 2024-03-21 14:34:57.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/no-yield.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4111 2024-03-21 14:26:09.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/onkey.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3175 2024-03-21 14:27:18.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/onmouse.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3528 2024-03-21 16:15:01.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/onstart-clone.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2890 2024-03-21 14:24:19.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/onstart.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4139 2024-03-21 14:32:52.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/receive.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1687 2024-03-21 16:09:16.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/return.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2187 2024-03-21 15:03:47.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/sleep.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1566 2024-03-21 16:12:39.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/throw.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4056 2024-03-21 16:10:49.000000 netsblox-0.6.8/netsblox/assets/img/blocks/control/try.png
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.174870 netsblox-0.6.8/netsblox/assets/img/blocks/looks/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2997 2024-03-22 03:57:01.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/change-scale.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1761 2024-03-22 03:54:11.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/get-costume-num.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1024 2024-03-22 03:59:06.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/get-scale.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1595 2024-03-22 04:00:41.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/get-visible.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3146 2024-03-22 03:55:12.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/say-duration.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1625 2024-03-22 03:55:51.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/say.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3981 2024-03-22 03:52:26.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/set-costume.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2925 2024-03-22 03:57:28.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/set-scale.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1118 2024-03-22 04:00:25.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/set-visible-false.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1256 2024-03-22 04:00:12.000000 netsblox-0.6.8/netsblox/assets/img/blocks/looks/set-visible-true.png
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.178870 netsblox-0.6.8/netsblox/assets/img/blocks/motion/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2722 2024-03-21 14:04:23.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/change-pos-x.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2746 2024-03-21 14:04:38.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/change-pos-y.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2696 2024-03-21 14:06:20.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/edge-bounce.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2611 2024-03-21 14:02:04.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/forward.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1599 2024-03-21 14:07:10.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/get-heading.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1726 2024-03-21 14:06:41.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/get-pos-x.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1752 2024-03-21 14:06:56.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/get-pos-y.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3175 2024-03-21 14:03:34.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/set-heading.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2032 2024-03-21 14:04:52.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/set-pos-x.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2066 2024-03-21 14:05:08.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/set-pos-y.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2876 2024-03-21 14:04:01.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/set-pos.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2971 2024-03-21 14:03:18.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/turn-left.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2977 2024-03-21 14:02:56.000000 netsblox-0.6.8/netsblox/assets/img/blocks/motion/turn-right.png
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.178870 netsblox-0.6.8/netsblox/assets/img/blocks/network/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5159 2024-03-22 12:36:19.000000 netsblox-0.6.8/netsblox/assets/img/blocks/network/receive.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5394 2024-03-22 12:45:26.000000 netsblox-0.6.8/netsblox/assets/img/blocks/network/rpc-call.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5498 2024-03-22 12:48:41.000000 netsblox-0.6.8/netsblox/assets/img/blocks/network/rpc-run.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5004 2024-03-22 12:39:10.000000 netsblox-0.6.8/netsblox/assets/img/blocks/network/send.png
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.182870 netsblox-0.6.8/netsblox/assets/img/blocks/operators/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1827 2024-03-22 15:15:25.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/add.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2259 2024-03-22 15:27:12.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/and.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1760 2024-03-22 15:17:03.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/div.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1357 2024-03-22 15:21:44.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/eq.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1713 2024-03-22 15:29:03.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/false.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1477 2024-03-22 15:22:19.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/great-eq.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1440 2024-03-22 15:23:50.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/great.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2234 2024-03-22 15:42:33.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/isinstance-list.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2348 2024-03-22 15:45:31.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/isinstance-str.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2388 2024-03-22 15:29:58.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/join.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1488 2024-03-22 15:21:16.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/less-eq.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1435 2024-03-22 15:20:43.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/less.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2151 2024-03-22 15:17:57.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/mod.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1883 2024-03-22 15:16:35.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/mul.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1493 2024-03-22 15:24:17.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/neq.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1687 2024-03-22 15:28:17.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/not.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1876 2024-03-22 15:27:43.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/or.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1783 2024-03-22 15:17:32.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/pow.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3218 2024-03-22 15:10:05.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/randrange.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1992 2024-03-22 15:18:20.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/round.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2820 2024-03-22 15:35:31.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/split-space.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2276 2024-03-22 15:18:44.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/sqrt.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3156 2024-03-22 15:41:30.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-chr.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2732 2024-03-22 15:36:12.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-index-first.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2960 2024-03-22 15:37:42.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-index-last.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3208 2024-03-22 15:38:51.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-index-rand.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2773 2024-03-22 15:39:22.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-len.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2168 2024-03-22 15:39:51.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-ord.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1694 2024-03-22 15:16:11.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/sub.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1631 2024-03-22 15:28:54.000000 netsblox-0.6.8/netsblox/assets/img/blocks/operators/true.png
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.182870 netsblox-0.6.8/netsblox/assets/img/blocks/pen/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3222 2024-03-22 16:53:32.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/change-pen-size.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1127 2024-03-22 16:19:43.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/clear.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1809 2024-03-22 16:21:16.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/get-drawing.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1533 2024-03-22 17:03:23.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/get-drawings.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1801 2024-03-22 16:52:13.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/get-pen-color.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1776 2024-03-22 16:49:46.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/get-pen-size.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1206 2024-03-22 16:21:02.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/set-drawing-false.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1561 2024-03-22 16:20:41.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/set-drawing-true.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2326 2024-03-22 16:23:56.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/set-pen-color.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2553 2024-03-22 16:54:07.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/set-pen-size.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1313 2024-03-22 16:54:42.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/stamp.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2854 2024-03-22 17:01:48.000000 netsblox-0.6.8/netsblox/assets/img/blocks/pen/write.png
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.182870 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1349 2024-03-22 04:07:56.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/answer.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3644 2024-03-22 04:06:57.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/ask.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2606 2024-03-22 04:22:35.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-image-self.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2631 2024-03-22 04:21:17.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-image-stage.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3200 2024-03-22 04:24:32.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-key-down.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1829 2024-03-22 04:16:20.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-latitude.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2028 2024-03-22 04:16:30.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-longitude.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1408 2024-03-22 04:10:47.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-mouse-x.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1444 2024-03-22 04:11:05.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-mouse-y.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1913 2024-03-22 04:19:11.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-stage-height.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1954 2024-03-22 04:19:00.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-stage-width.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3041 2024-03-22 04:04:21.000000 netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-touching.png
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.186870 netsblox-0.6.8/netsblox/assets/img/blocks/variables/
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3108 2024-03-22 12:26:16.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-cat.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3060 2024-03-22 12:10:36.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-cdr.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3347 2024-03-22 12:11:42.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-cons.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3095 2024-03-22 12:15:09.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-empty.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5514 2024-03-22 12:32:02.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-filter.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3494 2024-03-22 12:14:10.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-in.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3137 2024-03-22 12:11:15.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-index-first.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3407 2024-03-22 12:11:01.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-index-last.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3659 2024-03-22 15:55:02.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-index-rand.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4213 2024-03-22 12:21:53.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-insert-first.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4484 2024-03-22 12:22:33.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-insert-last.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2933 2024-03-22 12:10:05.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-len.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5358 2024-03-22 12:30:47.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-map.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3188 2024-03-22 12:18:27.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-push.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3266 2024-03-22 04:34:00.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-range.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3596 2024-03-22 12:20:42.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-remove-all.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3385 2024-03-22 12:19:15.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-remove-first.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3648 2024-03-22 12:19:57.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-remove-last.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5201 2024-03-22 12:23:50.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-replace-first.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     5442 2024-03-22 12:24:33.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-replace-last.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     3075 2024-03-22 12:09:33.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-rev.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2257 2024-03-22 12:29:27.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-sort.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2305 2024-03-22 04:33:22.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/list.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4784 2024-03-22 12:17:15.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/loop-foreach.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     2841 2024-03-22 04:31:32.000000 netsblox-0.6.8/netsblox/assets/img/blocks/variables/var-local.png
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.186870 netsblox-0.6.8/netsblox/assets/img/logo/
+-rw-rw-r--   0 devin     (1000) devin     (1000)    16709 2022-03-09 09:21:40.000000 netsblox-0.6.8/netsblox/assets/img/logo/logo-256.png
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4022 2022-03-09 09:20:32.000000 netsblox-0.6.8/netsblox/assets/img/logo/logo.svg
+-rw-rw-r--   0 devin     (1000) devin     (1000)     6563 2022-02-12 05:03:57.000000 netsblox-0.6.8/netsblox/colors.py
+-rwxrwxr-x   0 devin     (1000) devin     (1000)    11477 2024-03-29 13:26:02.000000 netsblox-0.6.8/netsblox/common.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     4373 2024-03-21 14:40:26.000000 netsblox-0.6.8/netsblox/concurrency.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)   284156 2024-04-17 14:40:30.000000 netsblox-0.6.8/netsblox/dev.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)   284152 2024-04-17 14:40:30.000000 netsblox-0.6.8/netsblox/editor.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     1427 2022-02-12 05:03:57.000000 netsblox-0.6.8/netsblox/events.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)    67958 2024-04-02 18:45:21.000000 netsblox-0.6.8/netsblox/graphical.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)     7801 2022-02-16 19:46:30.000000 netsblox-0.6.8/netsblox/rooms.py
+-rw-rw-r--   0 devin     (1000) devin     (1000)    52250 2024-04-02 11:59:10.000000 netsblox-0.6.8/netsblox/snap.py
+-rwxrwxr-x   0 devin     (1000) devin     (1000)     7799 2022-03-20 23:37:09.000000 netsblox-0.6.8/netsblox/transform.py
+drwxrwxr-x   0 devin     (1000) devin     (1000)        0 2024-04-17 14:41:25.186870 netsblox-0.6.8/netsblox.egg-info/
+-rw-r--r--   0 devin     (1000) devin     (1000)     4857 2024-04-17 14:41:24.000000 netsblox-0.6.8/netsblox.egg-info/PKG-INFO
+-rw-rw-r--   0 devin     (1000) devin     (1000)     7108 2024-04-17 14:41:25.000000 netsblox-0.6.8/netsblox.egg-info/SOURCES.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)        1 2024-04-17 14:41:24.000000 netsblox-0.6.8/netsblox.egg-info/dependency_links.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)      111 2024-04-17 14:41:24.000000 netsblox-0.6.8/netsblox.egg-info/requires.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)        9 2024-04-17 14:41:24.000000 netsblox-0.6.8/netsblox.egg-info/top_level.txt
+-rw-rw-r--   0 devin     (1000) devin     (1000)       38 2024-04-17 14:41:25.190870 netsblox-0.6.8/setup.cfg
+-rwxrwxr-x   0 devin     (1000) devin     (1000)     1059 2024-03-29 12:54:40.000000 netsblox-0.6.8/setup.py
```

### Comparing `netsblox-0.6.7/LICENSE` & `netsblox-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/PKG-INFO` & `netsblox-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsblox
-Version: 0.6.7
+Version: 0.6.8
 Summary: A python interface for accessing NetsBlox services
 Home-page: https://github.com/dragazo/NetsBlox-python
 Author: Devin Jean
 Author-email: devin.c.jean@vanderbilt.edu
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `netsblox-0.6.7/README.md` & `netsblox-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/app.py` & `netsblox-0.6.8/netsblox/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -583,30 +583,73 @@
             return # fail silently, but don't hide later errors if we get past this point
 
         for target in self.targets:
             if dest_widget is target.widget:
                 target.on_drop(e)
                 break
 
+class ColoredButton(tk.Frame):
+    def __init__(self, parent, *, text = 'Button', command = None):
+        super().__init__(parent)
+
+        self.label = tk.Label(self, text = text)
+        self.label.pack()
+
+        self.default_bg = self.cget('background')
+        self.default_fg = self.label.cget('foreground')
+
+        self.bg = None
+        self.fg = None
+        self.over_bg = None
+        self.over_fg = None
+
+        self.over = False
+        def on_enter(e):
+            self.over = True
+            self.redraw()
+        def on_leave(e):
+            self.over = False
+            self.redraw()
+        self.bind('<Enter>', on_enter)
+        self.bind('<Leave>', on_leave)
+
+        if command is not None:
+            self.bind('<Button-1>', lambda e: command())
+            self.label.bind('<Button-1>', lambda e: command())
+
+    def set_color(self, *, bg = None, fg = None, over_bg = None, over_fg = None):
+        self.bg = bg
+        self.fg = fg
+        self.over_bg = over_bg
+        self.over_fg = over_fg
+        self.redraw()
+
+    def redraw(self):
+        bg = (self.over_bg if self.over else self.bg) or self.default_bg
+        fg = (self.over_fg if self.over else self.fg) or self.default_fg
+
+        self.configure(bg = bg)
+        self.label.configure(bg = bg, fg = fg)
+
 class BlocksCategorySelector(tk.Frame):
     def __init__(self, parent):
         super().__init__(parent)
 
         self.default_button_color = None
         self.buttons = []
         for i, name in enumerate(BLOCK_CATEGORIES_ORDER):
             category = BLOCK_CATEGORIES[name]
             def make_clicker(name):
                 def clicker():
                     self.selected = name
                     content.project.on_tab_change()
                 return clicker
-            button = tk.Button(self, text = category.name, width = 1, height = 1, padx = 0, pady = 0, border = 0, relief = 'flat', command = make_clicker(name))
+            button = ColoredButton(self, text = category.name, command = make_clicker(name))
             button.grid(row = i // 2, column = i % 2, sticky = 'nesw')
-            self.default_button_color = button.cget('background')
+            self.default_button_color = parent.cget('background')
             self.buttons.append(button)
         for col in [0, 1]:
             self.columnconfigure(col, weight = 1, minsize = 80)
 
         self.selected = BLOCK_CATEGORIES_ORDER[0]
 
     @property
@@ -616,17 +659,17 @@
     @selected.setter
     def selected(self, name: str):
         assert name in BLOCK_CATEGORIES
         self.__selected = name
         for i in range(len(BLOCK_CATEGORIES_ORDER)):
             category = BLOCK_CATEGORIES[BLOCK_CATEGORIES_ORDER[i]]
             if BLOCK_CATEGORIES_ORDER[i] == self.__selected:
-                self.buttons[i].configure(bg = f'#{category.color}', activebackground = f'#{category.color}', fg = 'white', activeforeground = 'white')
+                self.buttons[i].set_color(bg = f'#{category.color}', fg = 'white', over_bg = f'#{category.color}', over_fg = 'white')
             else:
-                self.buttons[i].configure(bg = self.default_button_color, activebackground = f'#{category.color}', fg = 'black', activeforeground = 'white')
+                self.buttons[i].set_color(fg = None, bg = None, over_bg = f'#{category.color}', over_fg = 'white')
 
 class BlocksList(tk.Frame):
     def __init__(self, parent):
         super().__init__(parent)
 
         self.category_selector = BlocksCategorySelector(self)
         self.category_selector.pack(side = tk.TOP, fill = tk.X, expand = False)
```

### Comparing `netsblox-0.6.7/netsblox/assets/default-blocks.json` & `netsblox-0.6.8/netsblox/assets/default-blocks.json`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/default-imports.json` & `netsblox-0.6.8/netsblox/assets/default-imports.json`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/default-project.json` & `netsblox-0.6.8/netsblox/assets/default-project.json`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/examples/covid-19-daily.json` & `netsblox-0.6.8/netsblox/assets/examples/covid-19-daily.json`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/examples/street-view.json` & `netsblox-0.6.8/netsblox/assets/examples/street-view.json`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/examples/weather-app.json` & `netsblox-0.6.8/netsblox/assets/examples/weather-app.json`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/fonts/Droid/DroidSansFallback.ttf` & `netsblox-0.6.8/netsblox/assets/fonts/Droid/DroidSansFallback.ttf`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/fonts/Droid/README.md` & `netsblox-0.6.8/netsblox/assets/fonts/Droid/README.md`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/broadcast.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/broadcast.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/clone-expr.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/clone-expr.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/clone-stmt.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/clone-stmt.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/if-else-expr.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/if-else-expr.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/if-else.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/if-else.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/if.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/if.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/loop-for.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/loop-for.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/loop-forever.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/loop-forever.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/loop-repeat.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/loop-repeat.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/loop-until.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/loop-until.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/no-yield.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/no-yield.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/onkey.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/onkey.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/onmouse.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/onmouse.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/onstart-clone.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/onstart-clone.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/onstart.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/onstart.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/receive.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/receive.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/return.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/return.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/sleep.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/sleep.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/throw.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/throw.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/control/try.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/control/try.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/change-scale.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/change-scale.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/get-costume-num.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/get-costume-num.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/get-scale.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/get-scale.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/get-visible.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/get-visible.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/say-duration.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/say-duration.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/say.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/say.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/set-costume.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/set-costume.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/set-scale.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/set-scale.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/set-visible-false.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/set-visible-false.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/looks/set-visible-true.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/looks/set-visible-true.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/change-pos-x.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/change-pos-x.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/change-pos-y.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/change-pos-y.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/edge-bounce.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/edge-bounce.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/forward.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/forward.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/get-heading.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/get-heading.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/get-pos-x.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/get-pos-x.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/get-pos-y.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/get-pos-y.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/set-heading.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/set-heading.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/set-pos-x.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/set-pos-x.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/set-pos-y.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/set-pos-y.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/set-pos.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/set-pos.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/turn-left.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/turn-left.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/motion/turn-right.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/motion/turn-right.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/network/receive.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/network/receive.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/network/rpc-call.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/network/rpc-call.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/network/rpc-run.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/network/rpc-run.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/network/send.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/network/send.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/add.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/add.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/and.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/and.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/div.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/div.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/eq.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/eq.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/false.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/false.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/great-eq.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/great-eq.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/great.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/great.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/isinstance-list.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/isinstance-list.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/isinstance-str.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/isinstance-str.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/join.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/join.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/less-eq.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/less-eq.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/less.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/less.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/mod.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/mod.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/mul.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/mul.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/neq.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/neq.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/not.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/not.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/or.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/or.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/pow.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/pow.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/randrange.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/randrange.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/round.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/round.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/split-space.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/split-space.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/sqrt.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/sqrt.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-chr.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-chr.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-index-first.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-index-first.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-index-last.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-index-last.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-index-rand.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-index-rand.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-len.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-len.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/str-ord.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/str-ord.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/sub.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/sub.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/operators/true.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/operators/true.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/change-pen-size.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/change-pen-size.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/clear.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/clear.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/get-drawing.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/get-drawing.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/get-drawings.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/get-drawings.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/get-pen-color.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/get-pen-color.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/get-pen-size.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/get-pen-size.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/set-drawing-false.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/set-drawing-false.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/set-drawing-true.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/set-drawing-true.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/set-pen-color.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/set-pen-color.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/set-pen-size.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/set-pen-size.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/stamp.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/stamp.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/pen/write.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/pen/write.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/answer.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/answer.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/ask.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/ask.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-image-self.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-image-self.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-image-stage.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-image-stage.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-key-down.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-key-down.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-latitude.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-latitude.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-longitude.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-longitude.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-mouse-x.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-mouse-x.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-mouse-y.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-mouse-y.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-stage-height.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-stage-height.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-stage-width.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-stage-width.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/sensing/get-touching.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/sensing/get-touching.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-cat.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-cat.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-cdr.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-cdr.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-cons.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-cons.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-empty.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-empty.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-filter.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-filter.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-in.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-in.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-index-first.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-index-first.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-index-last.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-index-last.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-index-rand.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-index-rand.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-insert-first.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-insert-first.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-insert-last.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-insert-last.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-len.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-len.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-map.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-map.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-push.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-push.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-range.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-range.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-remove-all.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-remove-all.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-remove-first.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-remove-first.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-remove-last.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-remove-last.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-replace-first.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-replace-first.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-replace-last.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-replace-last.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-rev.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-rev.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list-sort.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list-sort.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/list.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/list.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/loop-foreach.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/loop-foreach.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/blocks/variables/var-local.png` & `netsblox-0.6.8/netsblox/assets/img/blocks/variables/var-local.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/logo/logo-256.png` & `netsblox-0.6.8/netsblox/assets/img/logo/logo-256.png`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/assets/img/logo/logo.svg` & `netsblox-0.6.8/netsblox/assets/img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/colors.py` & `netsblox-0.6.8/netsblox/colors.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/common.py` & `netsblox-0.6.8/netsblox/common.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/concurrency.py` & `netsblox-0.6.8/netsblox/concurrency.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/dev.py` & `netsblox-0.6.8/netsblox/dev.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/editor.py` & `netsblox-0.6.8/netsblox/editor.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/events.py` & `netsblox-0.6.8/netsblox/events.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/graphical.py` & `netsblox-0.6.8/netsblox/graphical.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/rooms.py` & `netsblox-0.6.8/netsblox/rooms.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/snap.py` & `netsblox-0.6.8/netsblox/snap.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox/transform.py` & `netsblox-0.6.8/netsblox/transform.py`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/netsblox.egg-info/PKG-INFO` & `netsblox-0.6.8/netsblox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsblox
-Version: 0.6.7
+Version: 0.6.8
 Summary: A python interface for accessing NetsBlox services
 Home-page: https://github.com/dragazo/NetsBlox-python
 Author: Devin Jean
 Author-email: devin.c.jean@vanderbilt.edu
 License: Apache 2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `netsblox-0.6.7/netsblox.egg-info/SOURCES.txt` & `netsblox-0.6.8/netsblox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsblox-0.6.7/setup.py` & `netsblox-0.6.8/setup.py`

 * *Files identical despite different names*

