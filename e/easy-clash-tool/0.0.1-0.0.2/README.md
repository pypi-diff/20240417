# Comparing `tmp/easy_clash_tool-0.0.1.tar.gz` & `tmp/easy_clash_tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_clash_tool-0.0.1.tar", last modified: Wed Apr 17 12:01:04 2024, max compression
+gzip compressed data, was "easy_clash_tool-0.0.2.tar", last modified: Wed Apr 17 13:21:59 2024, max compression
```

## Comparing `easy_clash_tool-0.0.1.tar` & `easy_clash_tool-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 12:01:04.071280 easy_clash_tool-0.0.1/
--rw-rw-rw-   0        0        0     4977 2024-04-17 12:01:04.070272 easy_clash_tool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3032 2024-03-31 08:13:19.000000 easy_clash_tool-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 12:01:04.059720 easy_clash_tool-0.0.1/easy_clash_tool/
--rw-rw-rw-   0        0        0       24 2024-03-31 06:22:23.000000 easy_clash_tool-0.0.1/easy_clash_tool/__init__.py
--rw-rw-rw-   0        0        0     6560 2024-03-31 07:34:52.000000 easy_clash_tool-0.0.1/easy_clash_tool/clash.py
-drwxrwxrwx   0        0        0        0 2024-04-17 12:01:04.066730 easy_clash_tool-0.0.1/easy_clash_tool.egg-info/
--rw-rw-rw-   0        0        0     4977 2024-04-17 12:01:03.000000 easy_clash_tool-0.0.1/easy_clash_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-17 12:01:04.000000 easy_clash_tool-0.0.1/easy_clash_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 12:01:03.000000 easy_clash_tool-0.0.1/easy_clash_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-17 12:01:03.000000 easy_clash_tool-0.0.1/easy_clash_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 12:01:03.000000 easy_clash_tool-0.0.1/easy_clash_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 12:01:04.072288 easy_clash_tool-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2623 2024-04-17 12:00:51.000000 easy_clash_tool-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:21:59.910109 easy_clash_tool-0.0.2/
+-rw-rw-rw-   0        0        0     6355 2024-04-17 13:21:59.910109 easy_clash_tool-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4202 2024-04-17 13:11:51.000000 easy_clash_tool-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 13:21:59.881070 easy_clash_tool-0.0.2/easy_clash_tool/
+-rw-rw-rw-   0        0        0       24 2024-04-17 13:21:32.000000 easy_clash_tool-0.0.2/easy_clash_tool/__init__.py
+-rw-rw-rw-   0        0        0     5415 2024-04-17 13:06:26.000000 easy_clash_tool-0.0.2/easy_clash_tool/clash.py
+-rw-rw-rw-   0        0        0     2006 2024-04-17 13:11:51.000000 easy_clash_tool-0.0.2/easy_clash_tool/main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:21:59.906182 easy_clash_tool-0.0.2/easy_clash_tool.egg-info/
+-rw-rw-rw-   0        0        0     6355 2024-04-17 13:21:59.000000 easy_clash_tool-0.0.2/easy_clash_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-17 13:21:59.000000 easy_clash_tool-0.0.2/easy_clash_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:21:59.000000 easy_clash_tool-0.0.2/easy_clash_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-17 13:21:59.000000 easy_clash_tool-0.0.2/easy_clash_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2024-04-17 13:21:59.000000 easy_clash_tool-0.0.2/easy_clash_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 13:21:59.000000 easy_clash_tool-0.0.2/easy_clash_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 13:21:59.910109 easy_clash_tool-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2764 2024-04-17 12:21:11.000000 easy_clash_tool-0.0.2/setup.py
```

### Comparing `easy_clash_tool-0.0.1/PKG-INFO` & `easy_clash_tool-0.0.2/easy_clash_tool.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: easy_clash_tool
-Version: 0.0.1
+Name: easy-clash-tool
+Version: 0.0.2
 Summary: easy_clash_tool是一个clash的python库,可以很便捷的自动切换可用节点
 Home-page: https://easy-clash-tool.xink.top/
 Author: hanxinkong
 Author-email: xinkonghan@gmail.com
 License: MIT
 Description: # easy-clash-tool
         
@@ -44,46 +44,72 @@
         </div>
         
         ## 简单使用
         
         ### demo.py
         
         ```python
+        import time
         from easy_clash_tool.clash import Clash
         
         clash = Clash(
-            base_api='http://127.0.0.1:9090',
+            base_api='http://127.0.0.1:24621',
+            secret='0367e21c-cceb-43a8-a2db-ad990e80dc28',
+            group_name='',
         )
-        clash.clash_cli(timeout=10)
-        ```
         
-        ![img.png](res%2Fimg.png)
+        # 手动切换
+        nodes, selected = clash.get_proxies()
+        print(nodes)
+        clash.change_node('🎮 Steam 商店/社区')
+        
+        # 自动切换
+        while True:
+            clash.auto_switch()
+            time.sleep(10)
+        
+        ```
         
         参数说明
         
         | 字段名           | 类型     | 必须 | 描述                                       |
         |---------------|--------|----|------------------------------------------|
         | base_api      | string | 否  | clash_api地址端口（默认: http://127.0.0.1:9090） |
         | group_name    | string | 否  | 策略组（默认: GLOBAL）                          |
         | delay_timeout | string | 否  | 节点超时时间（默认: 6秒）                           |
         | verify_url    | string | 否  | 测试超时的站点（默认: https://www.google.com）      |
         | secret        | string | 否  | 安全密钥                                     |
         
         命令行
         
         ```shell
-        usage: demo.py [-h] [--show-group] [--show-proxies] [--show-selected]
+        usage: easy-clash [-h] [--url URL] [--secret SECRET] [--delay DELAY] [--node-delay NODE_DELAY] [--verify-url VERIFY_URL] [--group_name GROUP_NAME] [--show-group] [--show-proxies]
+                       [--show-selected]
         
         optional arguments:
-          -h, --help           show this help message and exit
-          --show-group, -g     查看所有策略组
-          --show-proxies, -p   查看所有代理
-          --show-selected, -s  查看已选择代理
+          -h, --help                                    show this help message and exit
+          --url URL, -u URL                             clash-api 可查看config.yaml文件
+          --secret SECRET, -P SECRET                    密码
+          --delay DELAY, -T DELAY                       自动切换节点间隔时间 单位:秒
+          --node-timeout NODE_TIMEOUT, -t NODE_TIMEOUT  节点超时时间 单位:秒
+          --verify-url VERIFY_URL                       用于测试延时的url
+          --group_name GROUP_NAME                       指定策略组,可先通过 --show-group参数查询可用策略组
+          --show-group, -g                              查看所有策略组
+          --show-proxies, -p                            查看所有代理
+          --show-selected, -s                           查看已选择代理
+        ```
+        
+        命令行示例
+        
+        ```shell
+        easy-clash --url http://127.0.0.1:24621 --secret 0367e21c-cceb-43a8-a2db-ad990e80dc28 --delay 10 --verify-url https://www.google.com
         ```
         
+        ![img.png](res%2Fimg.png)
+        
         ## 链接
         
         Github：https://github.com/hanxinkong/easy-clash-tool
         
         在线文档：https://easy-clash-tool.xink.top
         
         ## 贡献者
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: easy_clash_tool Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: easy-clash-tool Version: 0.0.2 Summary:
 easy_clash_toolæ¯ä¸ä¸ªclashçpythonåº,å¯ä»¥å¾ä¾¿æ·çèªå¨åæ¢å¯ç¨èç¹
 Home-page: https://easy-clash-tool.xink.top/ Author: hanxinkong Author-email:
 xinkonghan@gmail.com License: MIT Description: # easy-clash-tool ![PyPI -
 Python Version](https://img.shields.io/pypi/pyversions/easy-clash-tool) ![PyPI
 - Version](https://img.shields.io/pypi/v/easy-clash-tool) ![PyPI - License]
 (https://img.shields.io/pypi/l/easy-clash-tool) ![PyPI - Format](https://
 img.shields.io/pypi/format/easy-clash-tool) ![GitHub watchers](https://
@@ -15,29 +15,41 @@
 gmail.com>)
 ï¼åéç»æãä»£ç æ ¼å¼æ¯éµå¾ªèªæä¸»è§ï¼å¦å­å¨ä¸è¶³æ¬è¯·æåºï¼
 ---- **ææ¡£å°åï¼ ** _h_t_t_p_s_:_/_/_e_a_s_y_-_c_l_a_s_h_-_t_o_o_l_._x_i_n_k_._t_o_p_/_ **PyPiå°åï¼ **
 _h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_e_a_s_y_-_c_l_a_s_h_-_t_o_o_l_ **GitHubå°åï¼ ** [https://
 github.com/hanxinkong/easy-clash-tool](https://github.com/hanxinkong/easy-
 clash-tool) ---- ## å®è£
 ```console pip install easy-clash-tool ```
-## ç®åä½¿ç¨ ### demo.py ```python from easy_clash_tool.clash import Clash
-clash = Clash( base_api='http://127.0.0.1:9090', ) clash.clash_cli(timeout=10)
-``` ![img.png](res%2Fimg.png) åæ°è¯´æ | å­æ®µå | ç±»å | å¿é¡» |
-æè¿° | |---------------|--------|----|---------------------------------------
----| | base_api | string | å¦ | clash_apiå°åç«¯å£ï¼é»è®¤: http://
-127.0.0.1:9090ï¼ | | group_name | string | å¦ | ç­ç¥ç»ï¼é»è®¤: GLOBALï¼
-| | delay_timeout | string | å¦ | èç¹è¶æ¶æ¶é´ï¼é»è®¤: 6ç§ï¼ | |
-verify_url | string | å¦ | æµè¯è¶æ¶çç«ç¹ï¼é»è®¤: https://
-www.google.comï¼ | | secret | string | å¦ | å®å¨å¯é¥ | å½ä»¤è¡ ```shell
-usage: demo.py [-h] [--show-group] [--show-proxies] [--show-selected] optional
-arguments: -h, --help show this help message and exit --show-group, -
-g æ¥çææç­ç¥ç» --show-proxies, -p æ¥çææä»£ç --show-selected,
--s æ¥çå·²éæ©ä»£ç ``` ## é¾æ¥ Githubï¼https://github.com/hanxinkong/
-easy-clash-tool å¨çº¿ææ¡£ï¼https://easy-clash-tool.xink.top ## è´¡ç®è ##
-è®¸å¯è¯ è¯¥é¡¹ç®æ ¹æ® **MIT** è®¸å¯æ¡æ¬¾è·å¾è®¸å¯. ## åè´£å£°æ 1.
+## ç®åä½¿ç¨ ### demo.py ```python import time from easy_clash_tool.clash
+import Clash clash = Clash( base_api='http://127.0.0.1:24621',
+secret='0367e21c-cceb-43a8-a2db-ad990e80dc28', group_name='', ) # æå¨åæ¢
+nodes, selected = clash.get_proxies() print(nodes) clash.change_node('ð®
+Steam ååº/ç¤¾åº') # èªå¨åæ¢ while True: clash.auto_switch() time.sleep
+(10) ``` åæ°è¯´æ | å­æ®µå | ç±»å | å¿é¡» | æè¿° | |---------------
+|--------|----|------------------------------------------| | base_api | string
+| å¦ | clash_apiå°åç«¯å£ï¼é»è®¤: http://127.0.0.1:9090ï¼ | | group_name
+| string | å¦ | ç­ç¥ç»ï¼é»è®¤: GLOBALï¼ | | delay_timeout | string | å¦
+| èç¹è¶æ¶æ¶é´ï¼é»è®¤: 6ç§ï¼ | | verify_url | string | å¦ |
+æµè¯è¶æ¶çç«ç¹ï¼é»è®¤: https://www.google.comï¼ | | secret | string |
+å¦ | å®å¨å¯é¥ | å½ä»¤è¡ ```shell usage: easy-clash [-h] [--url URL] [--
+secret SECRET] [--delay DELAY] [--node-delay NODE_DELAY] [--verify-url
+VERIFY_URL] [--group_name GROUP_NAME] [--show-group] [--show-proxies] [--show-
+selected] optional arguments: -h, --help show this help message and exit --url
+URL, -u URL clash-api å¯æ¥çconfig.yamlæä»¶ --secret SECRET, -P SECRET
+å¯ç  --delay DELAY, -T DELAY èªå¨åæ¢èç¹é´éæ¶é´ åä½:ç§ --
+node-timeout NODE_TIMEOUT, -t NODE_TIMEOUT èç¹è¶æ¶æ¶é´ åä½:ç§ --
+verify-url VERIFY_URL ç¨äºæµè¯å»¶æ¶çurl --group_name GROUP_NAME
+æå®ç­ç¥ç»,å¯åéè¿ --show-groupåæ°æ¥è¯¢å¯ç¨ç­ç¥ç» --show-
+group, -g æ¥çææç­ç¥ç» --show-proxies, -p æ¥çææä»£ç --show-
+selected, -s æ¥çå·²éæ©ä»£ç ``` å½ä»¤è¡ç¤ºä¾ ```shell easy-clash --
+url http://127.0.0.1:24621 --secret 0367e21c-cceb-43a8-a2db-ad990e80dc28 --
+delay 10 --verify-url https://www.google.com ``` ![img.png](res%2Fimg.png) ##
+é¾æ¥ Githubï¼https://github.com/hanxinkong/easy-clash-tool
+å¨çº¿ææ¡£ï¼https://easy-clash-tool.xink.top ## è´¡ç®è ## è®¸å¯è¯
+è¯¥é¡¹ç®æ ¹æ® **MIT** è®¸å¯æ¡æ¬¾è·å¾è®¸å¯. ## åè´£å£°æ 1.
 è¥ä½¿ç¨èæ»¥ç¨æ¬é¡¹ç®,æ¬äºº **æ éæ¿æ** ä»»ä½æ³å¾è´£ä»». 2.
 æ¬ç¨åºä»ä¾å¨±ä¹,æºç å¨é¨å¼æº,**ç¦æ­¢æ»¥ç¨** åäºæ¬¡
 **è´©åçå©**. **ç¦æ­¢ç¨äºåä¸ç¨é**. Keywords: easy,clash,tool
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Operating
 System :: OS Independent Classifier: Topic :: System :: Monitoring Classifier:
```

### Comparing `easy_clash_tool-0.0.1/README.md` & `easy_clash_tool-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -36,46 +36,72 @@
 </div>
 
 ## 简单使用
 
 ### demo.py
 
 ```python
+import time
 from easy_clash_tool.clash import Clash
 
 clash = Clash(
-    base_api='http://127.0.0.1:9090',
+    base_api='http://127.0.0.1:24621',
+    secret='0367e21c-cceb-43a8-a2db-ad990e80dc28',
+    group_name='',
 )
-clash.clash_cli(timeout=10)
-```
 
-![img.png](res%2Fimg.png)
+# 手动切换
+nodes, selected = clash.get_proxies()
+print(nodes)
+clash.change_node('🎮 Steam 商店/社区')
+
+# 自动切换
+while True:
+    clash.auto_switch()
+    time.sleep(10)
+
+```
 
 参数说明
 
 | 字段名           | 类型     | 必须 | 描述                                       |
 |---------------|--------|----|------------------------------------------|
 | base_api      | string | 否  | clash_api地址端口（默认: http://127.0.0.1:9090） |
 | group_name    | string | 否  | 策略组（默认: GLOBAL）                          |
 | delay_timeout | string | 否  | 节点超时时间（默认: 6秒）                           |
 | verify_url    | string | 否  | 测试超时的站点（默认: https://www.google.com）      |
 | secret        | string | 否  | 安全密钥                                     |
 
 命令行
 
 ```shell
-usage: demo.py [-h] [--show-group] [--show-proxies] [--show-selected]
+usage: easy-clash [-h] [--url URL] [--secret SECRET] [--delay DELAY] [--node-delay NODE_DELAY] [--verify-url VERIFY_URL] [--group_name GROUP_NAME] [--show-group] [--show-proxies]
+               [--show-selected]
 
 optional arguments:
-  -h, --help           show this help message and exit
-  --show-group, -g     查看所有策略组
-  --show-proxies, -p   查看所有代理
-  --show-selected, -s  查看已选择代理
+  -h, --help                                    show this help message and exit
+  --url URL, -u URL                             clash-api 可查看config.yaml文件
+  --secret SECRET, -P SECRET                    密码
+  --delay DELAY, -T DELAY                       自动切换节点间隔时间 单位:秒
+  --node-timeout NODE_TIMEOUT, -t NODE_TIMEOUT  节点超时时间 单位:秒
+  --verify-url VERIFY_URL                       用于测试延时的url
+  --group_name GROUP_NAME                       指定策略组,可先通过 --show-group参数查询可用策略组
+  --show-group, -g                              查看所有策略组
+  --show-proxies, -p                            查看所有代理
+  --show-selected, -s                           查看已选择代理
+```
+
+命令行示例
+
+```shell
+easy-clash --url http://127.0.0.1:24621 --secret 0367e21c-cceb-43a8-a2db-ad990e80dc28 --delay 10 --verify-url https://www.google.com
 ```
 
+![img.png](res%2Fimg.png)
+
 ## 链接
 
 Github：https://github.com/hanxinkong/easy-clash-tool
 
 在线文档：https://easy-clash-tool.xink.top
 
 ## 贡献者
```

#### html2text {}

```diff
@@ -11,25 +11,37 @@
 gmail.com>)
 ï¼åéç»æãä»£ç æ ¼å¼æ¯éµå¾ªèªæä¸»è§ï¼å¦å­å¨ä¸è¶³æ¬è¯·æåºï¼
 ---- **ææ¡£å°åï¼ ** _h_t_t_p_s_:_/_/_e_a_s_y_-_c_l_a_s_h_-_t_o_o_l_._x_i_n_k_._t_o_p_/_ **PyPiå°åï¼ **
 _h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_e_a_s_y_-_c_l_a_s_h_-_t_o_o_l_ **GitHubå°åï¼ ** [https://
 github.com/hanxinkong/easy-clash-tool](https://github.com/hanxinkong/easy-
 clash-tool) ---- ## å®è£
 ```console pip install easy-clash-tool ```
-## ç®åä½¿ç¨ ### demo.py ```python from easy_clash_tool.clash import Clash
-clash = Clash( base_api='http://127.0.0.1:9090', ) clash.clash_cli(timeout=10)
-``` ![img.png](res%2Fimg.png) åæ°è¯´æ | å­æ®µå | ç±»å | å¿é¡» |
-æè¿° | |---------------|--------|----|---------------------------------------
----| | base_api | string | å¦ | clash_apiå°åç«¯å£ï¼é»è®¤: http://
-127.0.0.1:9090ï¼ | | group_name | string | å¦ | ç­ç¥ç»ï¼é»è®¤: GLOBALï¼
-| | delay_timeout | string | å¦ | èç¹è¶æ¶æ¶é´ï¼é»è®¤: 6ç§ï¼ | |
-verify_url | string | å¦ | æµè¯è¶æ¶çç«ç¹ï¼é»è®¤: https://
-www.google.comï¼ | | secret | string | å¦ | å®å¨å¯é¥ | å½ä»¤è¡ ```shell
-usage: demo.py [-h] [--show-group] [--show-proxies] [--show-selected] optional
-arguments: -h, --help show this help message and exit --show-group, -
-g æ¥çææç­ç¥ç» --show-proxies, -p æ¥çææä»£ç --show-selected,
--s æ¥çå·²éæ©ä»£ç ``` ## é¾æ¥ Githubï¼https://github.com/hanxinkong/
-easy-clash-tool å¨çº¿ææ¡£ï¼https://easy-clash-tool.xink.top ## è´¡ç®è ##
-è®¸å¯è¯ è¯¥é¡¹ç®æ ¹æ® **MIT** è®¸å¯æ¡æ¬¾è·å¾è®¸å¯. ## åè´£å£°æ 1.
+## ç®åä½¿ç¨ ### demo.py ```python import time from easy_clash_tool.clash
+import Clash clash = Clash( base_api='http://127.0.0.1:24621',
+secret='0367e21c-cceb-43a8-a2db-ad990e80dc28', group_name='', ) # æå¨åæ¢
+nodes, selected = clash.get_proxies() print(nodes) clash.change_node('ð®
+Steam ååº/ç¤¾åº') # èªå¨åæ¢ while True: clash.auto_switch() time.sleep
+(10) ``` åæ°è¯´æ | å­æ®µå | ç±»å | å¿é¡» | æè¿° | |---------------
+|--------|----|------------------------------------------| | base_api | string
+| å¦ | clash_apiå°åç«¯å£ï¼é»è®¤: http://127.0.0.1:9090ï¼ | | group_name
+| string | å¦ | ç­ç¥ç»ï¼é»è®¤: GLOBALï¼ | | delay_timeout | string | å¦
+| èç¹è¶æ¶æ¶é´ï¼é»è®¤: 6ç§ï¼ | | verify_url | string | å¦ |
+æµè¯è¶æ¶çç«ç¹ï¼é»è®¤: https://www.google.comï¼ | | secret | string |
+å¦ | å®å¨å¯é¥ | å½ä»¤è¡ ```shell usage: easy-clash [-h] [--url URL] [--
+secret SECRET] [--delay DELAY] [--node-delay NODE_DELAY] [--verify-url
+VERIFY_URL] [--group_name GROUP_NAME] [--show-group] [--show-proxies] [--show-
+selected] optional arguments: -h, --help show this help message and exit --url
+URL, -u URL clash-api å¯æ¥çconfig.yamlæä»¶ --secret SECRET, -P SECRET
+å¯ç  --delay DELAY, -T DELAY èªå¨åæ¢èç¹é´éæ¶é´ åä½:ç§ --
+node-timeout NODE_TIMEOUT, -t NODE_TIMEOUT èç¹è¶æ¶æ¶é´ åä½:ç§ --
+verify-url VERIFY_URL ç¨äºæµè¯å»¶æ¶çurl --group_name GROUP_NAME
+æå®ç­ç¥ç»,å¯åéè¿ --show-groupåæ°æ¥è¯¢å¯ç¨ç­ç¥ç» --show-
+group, -g æ¥çææç­ç¥ç» --show-proxies, -p æ¥çææä»£ç --show-
+selected, -s æ¥çå·²éæ©ä»£ç ``` å½ä»¤è¡ç¤ºä¾ ```shell easy-clash --
+url http://127.0.0.1:24621 --secret 0367e21c-cceb-43a8-a2db-ad990e80dc28 --
+delay 10 --verify-url https://www.google.com ``` ![img.png](res%2Fimg.png) ##
+é¾æ¥ Githubï¼https://github.com/hanxinkong/easy-clash-tool
+å¨çº¿ææ¡£ï¼https://easy-clash-tool.xink.top ## è´¡ç®è ## è®¸å¯è¯
+è¯¥é¡¹ç®æ ¹æ® **MIT** è®¸å¯æ¡æ¬¾è·å¾è®¸å¯. ## åè´£å£°æ 1.
 è¥ä½¿ç¨èæ»¥ç¨æ¬é¡¹ç®,æ¬äºº **æ éæ¿æ** ä»»ä½æ³å¾è´£ä»». 2.
 æ¬ç¨åºä»ä¾å¨±ä¹,æºç å¨é¨å¼æº,**ç¦æ­¢æ»¥ç¨** åäºæ¬¡
 **è´©åçå©**. **ç¦æ­¢ç¨äºåä¸ç¨é**.
```

### Comparing `easy_clash_tool-0.0.1/easy_clash_tool/clash.py` & `easy_clash_tool-0.0.2/easy_clash_tool/clash.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-import argparse
 import json
-import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from urllib.parse import urljoin
 from typing import Tuple, List
 import requests
 from easy_spider_tool import jsonpath, retry
 from loguru import logger
 from requests import RequestException
 
 
-def read_cli_args():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--show-group', '-g', action='store_true', default=False, help='查看所有策略组')
-    parser.add_argument('--show-proxies', '-p', action='store_true', default=False, help='查看所有代理')
-    parser.add_argument('--show-selected', '-s', action='store_true', default=False, help='查看已选择代理')
-    return parser.parse_args()
-
-
 class Clash:
-    def __init__(self, base_api: str = 'http://127.0.0.1:9090', group_name: str = 'GLOBAL', delay_timeout: int = 6,
+    def __init__(self, base_api: str = 'http://127.0.0.1:9090', group_name: str = '', delay_timeout: int = 6,
                  verify_url: str = 'https://www.google.com',
                  secret=''):
         self.base_api = base_api
         self.group_name = group_name
         self.delay_timeout = delay_timeout
         self.verify_url = verify_url
         self.secret = secret
@@ -34,15 +24,15 @@
         """获取策略组名称"""
         api_url = urljoin(self.base_api, f'proxies')
         response = requests.get(api_url, timeout=10, headers=self.headers, verify=False)
         rule_group = jsonpath(response.json(), f'$.proxies[?(@.type=="Selector")].name', first=False, default=[])
         selected_rule_group = rule_group[0]
         return rule_group, selected_rule_group
 
-    @retry(num=1)
+    @retry(num=1, )
     def get_proxies(self) -> Tuple[List[str], str]:
         """获取策略组中的所有节点"""
         api_url = urljoin(self.base_api, f'proxies')
         response = requests.get(api_url, timeout=10, headers=self.headers, verify=False)
         all_proxies = jsonpath(response.json(), f'$.proxies.{self.group_name}.all[*]', first=False, default=[])
         selected = jsonpath(response.json(), f'$.proxies.{self.group_name}.now', first=True, default='')
         return all_proxies, selected
@@ -104,15 +94,15 @@
             proxy_name, delay = self.verify_proxy(name=selected)
             if delay is not None:
                 logger.success(f'[{self.group_name}] <{selected}> 延迟:{delay}ms -> 节点正常')
                 return None
 
             proxies.remove(selected)
 
-        with ThreadPoolExecutor(max_workers=10) as pool:
+        with ThreadPoolExecutor(max_workers=20) as pool:
             futures = [pool.submit(self.verify_proxy, proxy_name) for proxy_name in proxies]
             for future in as_completed(futures):
                 try:
                     proxy_name, delay = future.result()
                     if delay is not None and delay > 0:
                         available_nodes.append((proxy_name, delay))
                         break
@@ -128,30 +118,7 @@
                     logger.success(
                         f'[{self.group_name}] <{min_delay_node[0]}> 延迟:{min_delay_node[1]}ms -> 切换到节点')
                 else:
                     logger.error(
                         f'[{self.group_name}] <{min_delay_node[0]}> 延迟:{min_delay_node[1]}ms -> 切换到节点失败')
         else:
             logger.error(f'[{self.group_name}] -> 未找到可用节点')
-
-    def clash_cli(self, timeout: int = 20):
-        args = read_cli_args()
-        if args.show_group:
-            rule_group, selected_rule_group = self.get_rule_group()
-            logger.debug(rule_group)
-
-        if args.show_proxies:
-            proxies, selected = self.get_proxies()
-            print(proxies)
-
-        if args.show_selected:
-            proxies, selected = self.get_proxies()
-            print(selected)
-
-        if not any([
-            args.show_group,
-            args.show_proxies,
-            args.show_selected
-        ]):
-            while True:
-                self.auto_switch()
-                time.sleep(timeout)
```

### Comparing `easy_clash_tool-0.0.1/easy_clash_tool.egg-info/PKG-INFO` & `easy_clash_tool-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: easy-clash-tool
-Version: 0.0.1
+Name: easy_clash_tool
+Version: 0.0.2
 Summary: easy_clash_tool是一个clash的python库,可以很便捷的自动切换可用节点
 Home-page: https://easy-clash-tool.xink.top/
 Author: hanxinkong
 Author-email: xinkonghan@gmail.com
 License: MIT
 Description: # easy-clash-tool
         
@@ -44,46 +44,72 @@
         </div>
         
         ## 简单使用
         
         ### demo.py
         
         ```python
+        import time
         from easy_clash_tool.clash import Clash
         
         clash = Clash(
-            base_api='http://127.0.0.1:9090',
+            base_api='http://127.0.0.1:24621',
+            secret='0367e21c-cceb-43a8-a2db-ad990e80dc28',
+            group_name='',
         )
-        clash.clash_cli(timeout=10)
-        ```
         
-        ![img.png](res%2Fimg.png)
+        # 手动切换
+        nodes, selected = clash.get_proxies()
+        print(nodes)
+        clash.change_node('🎮 Steam 商店/社区')
+        
+        # 自动切换
+        while True:
+            clash.auto_switch()
+            time.sleep(10)
+        
+        ```
         
         参数说明
         
         | 字段名           | 类型     | 必须 | 描述                                       |
         |---------------|--------|----|------------------------------------------|
         | base_api      | string | 否  | clash_api地址端口（默认: http://127.0.0.1:9090） |
         | group_name    | string | 否  | 策略组（默认: GLOBAL）                          |
         | delay_timeout | string | 否  | 节点超时时间（默认: 6秒）                           |
         | verify_url    | string | 否  | 测试超时的站点（默认: https://www.google.com）      |
         | secret        | string | 否  | 安全密钥                                     |
         
         命令行
         
         ```shell
-        usage: demo.py [-h] [--show-group] [--show-proxies] [--show-selected]
+        usage: easy-clash [-h] [--url URL] [--secret SECRET] [--delay DELAY] [--node-delay NODE_DELAY] [--verify-url VERIFY_URL] [--group_name GROUP_NAME] [--show-group] [--show-proxies]
+                       [--show-selected]
         
         optional arguments:
-          -h, --help           show this help message and exit
-          --show-group, -g     查看所有策略组
-          --show-proxies, -p   查看所有代理
-          --show-selected, -s  查看已选择代理
+          -h, --help                                    show this help message and exit
+          --url URL, -u URL                             clash-api 可查看config.yaml文件
+          --secret SECRET, -P SECRET                    密码
+          --delay DELAY, -T DELAY                       自动切换节点间隔时间 单位:秒
+          --node-timeout NODE_TIMEOUT, -t NODE_TIMEOUT  节点超时时间 单位:秒
+          --verify-url VERIFY_URL                       用于测试延时的url
+          --group_name GROUP_NAME                       指定策略组,可先通过 --show-group参数查询可用策略组
+          --show-group, -g                              查看所有策略组
+          --show-proxies, -p                            查看所有代理
+          --show-selected, -s                           查看已选择代理
+        ```
+        
+        命令行示例
+        
+        ```shell
+        easy-clash --url http://127.0.0.1:24621 --secret 0367e21c-cceb-43a8-a2db-ad990e80dc28 --delay 10 --verify-url https://www.google.com
         ```
         
+        ![img.png](res%2Fimg.png)
+        
         ## 链接
         
         Github：https://github.com/hanxinkong/easy-clash-tool
         
         在线文档：https://easy-clash-tool.xink.top
         
         ## 贡献者
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: easy-clash-tool Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: easy_clash_tool Version: 0.0.2 Summary:
 easy_clash_toolæ¯ä¸ä¸ªclashçpythonåº,å¯ä»¥å¾ä¾¿æ·çèªå¨åæ¢å¯ç¨èç¹
 Home-page: https://easy-clash-tool.xink.top/ Author: hanxinkong Author-email:
 xinkonghan@gmail.com License: MIT Description: # easy-clash-tool ![PyPI -
 Python Version](https://img.shields.io/pypi/pyversions/easy-clash-tool) ![PyPI
 - Version](https://img.shields.io/pypi/v/easy-clash-tool) ![PyPI - License]
 (https://img.shields.io/pypi/l/easy-clash-tool) ![PyPI - Format](https://
 img.shields.io/pypi/format/easy-clash-tool) ![GitHub watchers](https://
@@ -15,29 +15,41 @@
 gmail.com>)
 ï¼åéç»æãä»£ç æ ¼å¼æ¯éµå¾ªèªæä¸»è§ï¼å¦å­å¨ä¸è¶³æ¬è¯·æåºï¼
 ---- **ææ¡£å°åï¼ ** _h_t_t_p_s_:_/_/_e_a_s_y_-_c_l_a_s_h_-_t_o_o_l_._x_i_n_k_._t_o_p_/_ **PyPiå°åï¼ **
 _h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_e_a_s_y_-_c_l_a_s_h_-_t_o_o_l_ **GitHubå°åï¼ ** [https://
 github.com/hanxinkong/easy-clash-tool](https://github.com/hanxinkong/easy-
 clash-tool) ---- ## å®è£
 ```console pip install easy-clash-tool ```
-## ç®åä½¿ç¨ ### demo.py ```python from easy_clash_tool.clash import Clash
-clash = Clash( base_api='http://127.0.0.1:9090', ) clash.clash_cli(timeout=10)
-``` ![img.png](res%2Fimg.png) åæ°è¯´æ | å­æ®µå | ç±»å | å¿é¡» |
-æè¿° | |---------------|--------|----|---------------------------------------
----| | base_api | string | å¦ | clash_apiå°åç«¯å£ï¼é»è®¤: http://
-127.0.0.1:9090ï¼ | | group_name | string | å¦ | ç­ç¥ç»ï¼é»è®¤: GLOBALï¼
-| | delay_timeout | string | å¦ | èç¹è¶æ¶æ¶é´ï¼é»è®¤: 6ç§ï¼ | |
-verify_url | string | å¦ | æµè¯è¶æ¶çç«ç¹ï¼é»è®¤: https://
-www.google.comï¼ | | secret | string | å¦ | å®å¨å¯é¥ | å½ä»¤è¡ ```shell
-usage: demo.py [-h] [--show-group] [--show-proxies] [--show-selected] optional
-arguments: -h, --help show this help message and exit --show-group, -
-g æ¥çææç­ç¥ç» --show-proxies, -p æ¥çææä»£ç --show-selected,
--s æ¥çå·²éæ©ä»£ç ``` ## é¾æ¥ Githubï¼https://github.com/hanxinkong/
-easy-clash-tool å¨çº¿ææ¡£ï¼https://easy-clash-tool.xink.top ## è´¡ç®è ##
-è®¸å¯è¯ è¯¥é¡¹ç®æ ¹æ® **MIT** è®¸å¯æ¡æ¬¾è·å¾è®¸å¯. ## åè´£å£°æ 1.
+## ç®åä½¿ç¨ ### demo.py ```python import time from easy_clash_tool.clash
+import Clash clash = Clash( base_api='http://127.0.0.1:24621',
+secret='0367e21c-cceb-43a8-a2db-ad990e80dc28', group_name='', ) # æå¨åæ¢
+nodes, selected = clash.get_proxies() print(nodes) clash.change_node('ð®
+Steam ååº/ç¤¾åº') # èªå¨åæ¢ while True: clash.auto_switch() time.sleep
+(10) ``` åæ°è¯´æ | å­æ®µå | ç±»å | å¿é¡» | æè¿° | |---------------
+|--------|----|------------------------------------------| | base_api | string
+| å¦ | clash_apiå°åç«¯å£ï¼é»è®¤: http://127.0.0.1:9090ï¼ | | group_name
+| string | å¦ | ç­ç¥ç»ï¼é»è®¤: GLOBALï¼ | | delay_timeout | string | å¦
+| èç¹è¶æ¶æ¶é´ï¼é»è®¤: 6ç§ï¼ | | verify_url | string | å¦ |
+æµè¯è¶æ¶çç«ç¹ï¼é»è®¤: https://www.google.comï¼ | | secret | string |
+å¦ | å®å¨å¯é¥ | å½ä»¤è¡ ```shell usage: easy-clash [-h] [--url URL] [--
+secret SECRET] [--delay DELAY] [--node-delay NODE_DELAY] [--verify-url
+VERIFY_URL] [--group_name GROUP_NAME] [--show-group] [--show-proxies] [--show-
+selected] optional arguments: -h, --help show this help message and exit --url
+URL, -u URL clash-api å¯æ¥çconfig.yamlæä»¶ --secret SECRET, -P SECRET
+å¯ç  --delay DELAY, -T DELAY èªå¨åæ¢èç¹é´éæ¶é´ åä½:ç§ --
+node-timeout NODE_TIMEOUT, -t NODE_TIMEOUT èç¹è¶æ¶æ¶é´ åä½:ç§ --
+verify-url VERIFY_URL ç¨äºæµè¯å»¶æ¶çurl --group_name GROUP_NAME
+æå®ç­ç¥ç»,å¯åéè¿ --show-groupåæ°æ¥è¯¢å¯ç¨ç­ç¥ç» --show-
+group, -g æ¥çææç­ç¥ç» --show-proxies, -p æ¥çææä»£ç --show-
+selected, -s æ¥çå·²éæ©ä»£ç ``` å½ä»¤è¡ç¤ºä¾ ```shell easy-clash --
+url http://127.0.0.1:24621 --secret 0367e21c-cceb-43a8-a2db-ad990e80dc28 --
+delay 10 --verify-url https://www.google.com ``` ![img.png](res%2Fimg.png) ##
+é¾æ¥ Githubï¼https://github.com/hanxinkong/easy-clash-tool
+å¨çº¿ææ¡£ï¼https://easy-clash-tool.xink.top ## è´¡ç®è ## è®¸å¯è¯
+è¯¥é¡¹ç®æ ¹æ® **MIT** è®¸å¯æ¡æ¬¾è·å¾è®¸å¯. ## åè´£å£°æ 1.
 è¥ä½¿ç¨èæ»¥ç¨æ¬é¡¹ç®,æ¬äºº **æ éæ¿æ** ä»»ä½æ³å¾è´£ä»». 2.
 æ¬ç¨åºä»ä¾å¨±ä¹,æºç å¨é¨å¼æº,**ç¦æ­¢æ»¥ç¨** åäºæ¬¡
 **è´©åçå©**. **ç¦æ­¢ç¨äºåä¸ç¨é**. Keywords: easy,clash,tool
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Operating
 System :: OS Independent Classifier: Topic :: System :: Monitoring Classifier:
```

### Comparing `easy_clash_tool-0.0.1/setup.py` & `easy_clash_tool-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,9 +63,14 @@
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11'
-        ]
+        ],
+        entry_points={
+            "console_scripts": [
+                "easy-clash = easy_clash_tool:main",
+            ],
+        },
     )
```

