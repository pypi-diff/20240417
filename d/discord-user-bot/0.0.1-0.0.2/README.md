# Comparing `tmp/discord-user-bot-0.0.1.tar.gz` & `tmp/discord-user-bot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-user-bot-0.0.1.tar", last modified: Tue Apr 16 12:32:35 2024, max compression
+gzip compressed data, was "discord-user-bot-0.0.2.tar", last modified: Tue Apr 16 13:07:58 2024, max compression
```

## Comparing `discord-user-bot-0.0.1.tar` & `discord-user-bot-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 12:32:35.802139 discord-user-bot-0.0.1/
--rw-rw-rw-   0        0        0      388 2024-04-16 12:32:35.798139 discord-user-bot-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 12:32:35.684140 discord-user-bot-0.0.1/discord_user_bot/
--rw-rw-rw-   0        0        0      457 2024-04-15 12:57:12.000000 discord-user-bot-0.0.1/discord_user_bot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 12:32:35.790140 discord-user-bot-0.0.1/discord_user_bot.egg-info/
--rw-rw-rw-   0        0        0      388 2024-04-16 12:32:34.000000 discord-user-bot-0.0.1/discord_user_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-04-16 12:32:35.000000 discord-user-bot-0.0.1/discord_user_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 12:32:34.000000 discord-user-bot-0.0.1/discord_user_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 12:32:34.000000 discord-user-bot-0.0.1/discord_user_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-16 12:32:34.000000 discord-user-bot-0.0.1/discord_user_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 12:32:35.803139 discord-user-bot-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-04-16 12:06:54.000000 discord-user-bot-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:07:58.725821 discord-user-bot-0.0.2/
+-rw-rw-rw-   0        0        0      430 2024-04-16 13:07:58.720820 discord-user-bot-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 13:07:58.532822 discord-user-bot-0.0.2/discord_user_bot/
+-rw-rw-rw-   0        0        0      457 2024-04-15 12:57:12.000000 discord-user-bot-0.0.2/discord_user_bot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:07:58.713822 discord-user-bot-0.0.2/discord_user_bot.egg-info/
+-rw-rw-rw-   0        0        0      430 2024-04-16 13:07:57.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-04-16 13:07:58.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 13:07:57.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 13:07:57.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-16 13:07:57.000000 discord-user-bot-0.0.2/discord_user_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 13:07:58.779822 discord-user-bot-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-04-16 13:07:48.000000 discord-user-bot-0.0.2/setup.py
```

### Comparing `discord-user-bot-0.0.1/setup.py` & `discord-user-bot-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='discord-user-bot',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[
         'urllib'
     ],
     author='TVOFFicial1',
     author_email='kirill.shishkov2007@gmail.com',
     description='Discord user bot library python',
-    license='MIT',
+    url='https://github.com/CCCProo/discord-user-bot',
+
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
 )
```

