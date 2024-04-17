# Comparing `tmp/botmom-0.2.tar.gz` & `tmp/botmom-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botmom-0.2.tar", last modified: Wed Apr  3 09:59:39 2024, max compression
+gzip compressed data, was "botmom-1.0.tar", last modified: Wed Apr 17 09:35:50 2024, max compression
```

## Comparing `botmom-0.2.tar` & `botmom-1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 09:59:38.997443 botmom-0.2/
--rw-rw-rw-   0        0        0     1332 2024-04-03 09:59:38.997443 botmom-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      766 2024-04-03 09:19:17.000000 botmom-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 09:59:38.924924 botmom-0.2/botmom/
--rw-rw-rw-   0        0        0       25 2024-04-03 09:59:01.000000 botmom-0.2/botmom/__init__.py
--rw-rw-rw-   0        0        0     4115 2024-04-03 09:18:54.000000 botmom-0.2/botmom/handlers.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:59:38.990267 botmom-0.2/botmom.egg-info/
--rw-rw-rw-   0        0        0     1332 2024-04-03 09:59:38.000000 botmom-0.2/botmom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-03 09:59:38.000000 botmom-0.2/botmom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 09:59:38.000000 botmom-0.2/botmom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-03 09:59:38.000000 botmom-0.2/botmom.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 09:59:38.000000 botmom-0.2/botmom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 09:59:39.011060 botmom-0.2/setup.cfg
--rw-rw-rw-   0        0        0      891 2024-04-03 09:59:05.000000 botmom-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:35:50.256980 botmom-1.0/
+-rw-rw-rw-   0        0        0     3448 2024-04-17 09:35:50.256980 botmom-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2829 2024-04-17 09:26:29.000000 botmom-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 09:35:50.205756 botmom-1.0/botmom/
+-rw-rw-rw-   0        0        0       49 2024-04-17 09:26:39.000000 botmom-1.0/botmom/__init__.py
+-rw-rw-rw-   0        0        0     1410 2024-04-17 07:55:36.000000 botmom-1.0/botmom/buttons.py
+-rw-rw-rw-   0        0        0     5907 2024-04-17 09:26:47.000000 botmom-1.0/botmom/handlers.py
+drwxrwxrwx   0        0        0        0 2024-04-17 09:35:50.254531 botmom-1.0/botmom.egg-info/
+-rw-rw-rw-   0        0        0     3448 2024-04-17 09:35:50.000000 botmom-1.0/botmom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-04-17 09:35:50.000000 botmom-1.0/botmom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 09:35:50.000000 botmom-1.0/botmom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-17 09:35:50.000000 botmom-1.0/botmom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 09:35:50.000000 botmom-1.0/botmom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 09:35:50.270911 botmom-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      891 2024-04-17 09:27:10.000000 botmom-1.0/setup.py
```

### Comparing `botmom-0.2/botmom/handlers.py` & `botmom-1.0/botmom/handlers.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,83 +4,145 @@
 import logging
 import sys
 import aiohttp
 import re
 from os import getenv
 
 from aiogram import Bot, Dispatcher
-from aiogram.types import Message
+from aiogram.types import Message, CallbackQuery
 from aiogram import F
+from .buttons import InlineButtons, ReplyButtons
 
 
 already_started = False
 dp = Dispatcher()
 
 
 @dp.message(~F.text.startswith("/"))
 async def message_handler(msg: Message) -> None:
     on_message = getattr(main_module, "on_message", None)
     if not on_message:
-        raise ValueError("Нет функции on_message. Пример:\ndef on_message(msg: str):\n    return \"Твоё сообщение: \" + msg")
+        raise ValueError("Нет функции on_message")
+    
+    
+    async def answer(text, keyboard=None):
+        if isinstance(keyboard, (InlineButtons, ReplyButtons)):
+            message_instance = await msg.answer(text, reply_markup=keyboard.as_markup())
+        else:
+            message_instance = await msg.answer(text)
+        
+        return message_instance
+    
     
     num_parms = len(inspect.signature(on_message).parameters)
-
+    
+    message = lambda: None
+    message.answer = answer
+    message.text = msg.text
+    message.chat_id = msg.chat.id
+    
     if num_parms == 0:
         args = tuple()
     elif num_parms == 1:
-        args = (msg.text,)
-    elif num_parms == 2:
-        args = (msg.text, msg.chat.id)
+        args = (message,)
     else:
-        raise ValueError("Функция on_message не должна иметь больше двух параметров")
+        raise ValueError("Функция on_message не должна иметь больше одного параметра")
     
     try:
-        answer = on_message(*args)
+        await on_message(*args)
     except Exception as e:
         await msg.answer("Возникла ошибка")
         raise e
-    
-    await msg.answer(answer)
 
 
 @dp.message(F.text.startswith("/"))
-async def commands_handler(msg: Message) -> None:
+async def command_handler(msg: Message) -> None:
     cmd = re.search(r"(?<=\/)[a-zA-Z_]*", msg.text).group()
     
     if cmd == "start":
         try:
             await set_chat_commands(dp.token, dp.commands, msg.from_user.id)
         except:
             pass
     
     on_command = getattr(main_module, f"on_command_{cmd}", None)
     
     if not on_command and cmd == "start":
         on_command = lambda msg: "Начинаем!"
     elif not on_command:
-        raise ValueError(f"Нет функции для отработки команды {cmd}. Пример:\ndef on_command_{cmd}(cmd: str):\n    return \"Введена команда \" + cmd")
+        raise ValueError(f"Нет функции для отработки команды {cmd}")
 
+    
+    async def answer(text, keyboard=None):
+        if isinstance(keyboard, (InlineButtons, ReplyButtons)):
+            message_instance = await msg.answer(text, reply_markup=keyboard.as_markup())
+        else:
+            message_instance = await msg.answer(text)
+        
+        return message_instance
+    
+    
     num_parms = len(inspect.signature(on_command).parameters)
     
+    message = lambda: None
+    message.answer = answer
+    message.text = msg.text
+    message.chat_id = msg.chat.id
+    
     if num_parms == 0:
         args = tuple()
     elif num_parms == 1:
-        args = (msg.text,)
-    elif num_parms == 2:
-        args = (msg.text, msg.chat.id)
+        args = (message, )
     else:
-        raise ValueError(f"Функция on_command_{cmd} не должна иметь больше двух параметров")
+        raise ValueError(f"Функция on_command_{cmd} не должна иметь больше одного параметров")
     
     try:
-        answer = on_command(*args)
+        await on_command(*args)
     except Exception as e:
         await msg.answer("Возникла ошибка")
         raise e
     
-    await msg.answer(answer)
+
+@dp.callback_query()
+async def inline_button_handler(callback: CallbackQuery):
+    on_button = getattr(main_module, "on_button", None)
+    if not on_button:
+        raise ValueError("Нет функции on_button")
+    
+    
+    async def answer(text, keyboard=None):
+        await callback.answer()
+        if isinstance(keyboard, (InlineButtons, ReplyButtons)):
+            message_instance = await callback.message.answer(text, reply_markup=keyboard.as_markup())
+        else:
+            message_instance = await callback.message.answer(text)
+        
+        return message_instance
+    
+    
+    num_parms = len(inspect.signature(on_button).parameters)
+    
+    call = lambda: None
+    call.answer = answer
+    call.chat_id = callback.message.chat.id
+    call.data = callback.data
+    call.delete = callback.message.delete
+    
+    if num_parms == 0:
+        args = tuple()
+    elif num_parms == 1:
+        args = (call,)
+    else:
+        raise ValueError("Функция on_button не должна иметь больше одного параметра")
+    
+    try:
+        await on_button(*args)
+    except Exception as e:
+        await callback.message.answer("Возникла ошибка")
+        raise e
 
 
 async def set_chat_commands(token, commands, chat_id) -> None:
     payload = {
         "commands": commands,
         "scope": {
             "type": "chat",
@@ -129,8 +191,9 @@
     raise ValueError("Необходимо добавить вызов функции run_bot(\"ВАШ ТОКЕН\") в самый конец кода для запуска бота")
 
 
 if __name__ == "__main__":
     print("Модуль должен быть импортирован:\nfrom botmom import *")
     sys.exit()
 
+
 atexit.register(check_run_bot)
```

### Comparing `botmom-0.2/setup.py` & `botmom-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md", "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="botmom",
-    version="0.2",
+    version="1.0",
     author="Arsenii Misiurenko",
     author_email="2028misyurenko.ad@student.letovo.ru",
     description="Easiest and most variable module for creating telegram bots",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/Arsenii22/botmom",
     packages=find_packages(),
```

