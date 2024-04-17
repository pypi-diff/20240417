# Comparing `tmp/discord-user-bot-0.0.2.tar.gz` & `tmp/discord-user-bot-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-user-bot-0.0.2.tar", last modified: Tue Apr 16 13:07:58 2024, max compression
+gzip compressed data, was "discord-user-bot-0.0.2.1.tar", last modified: Wed Apr 17 12:00:33 2024, max compression
```

## Comparing `discord-user-bot-0.0.2.tar` & `discord-user-bot-0.0.2.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 13:07:58.725821 discord-user-bot-0.0.2/
--rw-rw-rw-   0        0        0      430 2024-04-16 13:07:58.720820 discord-user-bot-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 13:07:58.532822 discord-user-bot-0.0.2/discord_user_bot/
--rw-rw-rw-   0        0        0      457 2024-04-15 12:57:12.000000 discord-user-bot-0.0.2/discord_user_bot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 13:07:58.713822 discord-user-bot-0.0.2/discord_user_bot.egg-info/
--rw-rw-rw-   0        0        0      430 2024-04-16 13:07:57.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-04-16 13:07:58.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 13:07:57.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 13:07:57.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-16 13:07:57.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 13:07:58.779822 discord-user-bot-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-04-16 13:07:48.000000 discord-user-bot-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:32.977022 discord-user-bot-0.0.2.1/
+-rw-rw-rw-   0        0        0      432 2024-04-17 12:00:32.973021 discord-user-bot-0.0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:32.911021 discord-user-bot-0.0.2.1/discord_user_bot/
+-rw-rw-rw-   0        0        0      457 2024-04-15 12:57:12.000000 discord-user-bot-0.0.2.1/discord_user_bot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:00:32.968021 discord-user-bot-0.0.2.1/discord_user_bot.egg-info/
+-rw-rw-rw-   0        0        0      432 2024-04-17 12:00:32.000000 discord-user-bot-0.0.2.1/discord_user_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-17 12:00:32.000000 discord-user-bot-0.0.2.1/discord_user_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:00:32.000000 discord-user-bot-0.0.2.1/discord_user_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-17 12:00:32.000000 discord-user-bot-0.0.2.1/discord_user_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 12:00:32.991019 discord-user-bot-0.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      583 2024-04-17 12:00:23.000000 discord-user-bot-0.0.2.1/setup.py
```

### Comparing `discord-user-bot-0.0.2/setup.py` & `discord-user-bot-0.0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='discord-user-bot',
-    version='0.0.2',
+    version='0.0.2.1',
     packages=find_packages(),
-    install_requires=[
-        'urllib'
-    ],
+    install_requires=[],
     author='TVOFFicial1',
     author_email='kirill.shishkov2007@gmail.com',
     description='Discord user bot library python',
     url='https://github.com/CCCProo/discord-user-bot',
 
     classifiers=[
         'Programming Language :: Python :: 3',
```

