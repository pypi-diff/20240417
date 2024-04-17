# Comparing `tmp/PKDevTools-0.13.20240416.87.tar.gz` & `tmp/PKDevTools-0.13.20240417.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240416.87.tar", last modified: Tue Apr 16 18:46:20 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240417.88.tar", last modified: Wed Apr 17 07:40:27 2024, max compression
```

## Comparing `PKDevTools-0.13.20240416.87.tar` & `PKDevTools-0.13.20240417.88.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/
--rw-rw-rw-   0        0        0     1086 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-16 18:46:20.499032 PKDevTools-0.13.20240416.87/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     3985 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6212 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    13139 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     8048 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14224 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11216 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       27 2024-04-16 18:46:16.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 18:46:14.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      158 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-16 18:46:20.000000 PKDevTools-0.13.20240416.87/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5202 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/README.md
--rw-rw-rw-   0        0        0       86 2024-04-16 18:46:20.514654 PKDevTools-0.13.20240416.87/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-16 18:44:02.000000 PKDevTools-0.13.20240416.87/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:40:27.658351 PKDevTools-0.13.20240417.88/
+-rw-rw-rw-   0        0        0     1086 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-17 07:40:27.642721 PKDevTools-0.13.20240417.88/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:40:27.658351 PKDevTools-0.13.20240417.88/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     3985 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6212 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    13819 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     8048 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14224 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11216 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       27 2024-04-17 07:40:22.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:40:27.658351 PKDevTools-0.13.20240417.88/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5202 2024-04-17 07:40:27.000000 PKDevTools-0.13.20240417.88/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2024-04-17 07:40:27.000000 PKDevTools-0.13.20240417.88/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 07:40:27.000000 PKDevTools-0.13.20240417.88/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-17 07:40:27.000000 PKDevTools-0.13.20240417.88/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 07:40:21.000000 PKDevTools-0.13.20240417.88/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      158 2024-04-17 07:40:27.000000 PKDevTools-0.13.20240417.88/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 07:40:27.000000 PKDevTools-0.13.20240417.88/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5202 2024-04-17 07:40:27.658351 PKDevTools-0.13.20240417.88/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-17 07:40:27.658351 PKDevTools-0.13.20240417.88/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-17 07:39:05.000000 PKDevTools-0.13.20240417.88/setup.py
```

### Comparing `PKDevTools-0.13.20240416.87/LICENSE` & `PKDevTools-0.13.20240417.88/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/__init__.py` & `PKDevTools-0.13.20240417.88/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/PKDateUtilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,22 @@
         return (
             pytz.utc.localize(utc_dt)
             .replace(tzinfo=timezone.utc)
             .astimezone(tz=pytz.timezone("Asia/Kolkata"))
         )
 
     def last_day_of_month(any_day:datetime.datetime):
+        if any_day is None:
+            any_day = PKDateUtilities.currentDateTime()
         weekday, lastDay = calendar.monthrange(any_day.year, any_day.month)
         return PKDateUtilities.currentDateTime(simulate=True,day=lastDay,year=any_day.year,month=any_day.month)
 
     def last_day_of_previous_month(any_day:datetime.datetime):
+        if any_day is None:
+            any_day = PKDateUtilities.currentDateTime()
         first = any_day.replace(day=1)
         last_day_last_month = first - datetime.timedelta(days=1)
         return last_day_last_month
 
     def tradingDate(simulate=False, day=None):
         lastTradingDate = None
         curr = PKDateUtilities.currentDateTime(simulate=simulate, day=day)
@@ -68,42 +72,50 @@
         while PKDateUtilities.isHoliday(lastTradingDate)[0] or not PKDateUtilities.isTradingWeekday(lastTradingDate):
             lastTradingDate = PKDateUtilities.previousTradingDate(lastTradingDate)
         return lastTradingDate
     
     def previousTradingDate(d1:datetime.datetime|str=None):
         if isinstance(d1,str):
             d1 = PKDateUtilities.dateFromYmdString(d1)
+        if d1 is None:
+            d1 = PKDateUtilities.currentDateTime()
         lastTradingDate = (d1 - datetime.timedelta(days=1))
         while PKDateUtilities.isHoliday(lastTradingDate)[0] or not PKDateUtilities.isTradingWeekday(lastTradingDate):
             lastTradingDate = PKDateUtilities.previousTradingDate(lastTradingDate)
         if isinstance(lastTradingDate,datetime.datetime):
             lastTradingDate = lastTradingDate.date()
         return lastTradingDate
 
     def nextTradingDate(d1:datetime.datetime|str=None, days=1):
+        if d1 is None:
+            d1 = PKDateUtilities.currentDateTime()
         if isinstance(d1,str):
             d1 = PKDateUtilities.dateFromYmdString(d1)
         nextDayCounter = 1
         while nextDayCounter <= days:
             nextTradingDate = (d1 + datetime.timedelta(days=1))
             while PKDateUtilities.isHoliday(nextTradingDate)[0] or not PKDateUtilities.isTradingWeekday(nextTradingDate):
                 nextTradingDate = PKDateUtilities.nextTradingDate(nextTradingDate, days=1)
             if isinstance(nextTradingDate,datetime.datetime):
                 nextTradingDate = nextTradingDate.date()
             nextDayCounter += 1
             d1 = nextTradingDate
         return nextTradingDate
     
     def firstTradingDateOfMonth(any_day:datetime.datetime):
+        if any_day is None:
+            any_day = PKDateUtilities.currentDateTime()
         calcDate = any_day.replace(day=1) # Replace to the first day of the month
         prevTradingDate = PKDateUtilities.previousTradingDate(calcDate)
         firstTradingDate = PKDateUtilities.nextTradingDate(prevTradingDate)
         return firstTradingDate
 
     def lastTradingDateOfMonth(any_day:datetime.datetime):
+        if any_day is None:
+            any_day = PKDateUtilities.currentDateTime()
         calcDate = PKDateUtilities.last_day_of_month(any_day) + datetime.timedelta(days=1)
         lastTradingDate = PKDateUtilities.previousTradingDate(calcDate)
         return lastTradingDate
     
     def dateFromYmdString(Ymd=None):
         today = PKDateUtilities.currentDateTime()
         return datetime.datetime.strptime(Ymd, "%Y-%m-%d").replace(tzinfo=today.tzinfo)
@@ -146,15 +158,15 @@
         else:
             return curr
 
     def isTradingTime():
         curr = PKDateUtilities.currentDateTime()
         openTime = curr.replace(hour=9, minute=15)
         closeTime = curr.replace(hour=15, minute=30)
-        return (openTime <= curr <= closeTime) and PKDateUtilities.isTradingWeekday()
+        return (openTime <= curr <= closeTime) and PKDateUtilities.isTradingWeekday() and not PKDateUtilities.isTodayHoliday()
 
     def isTradingWeekday(checkDate=None):
         if checkDate is None:
             checkDate = PKDateUtilities.currentDateTime()
         return 0 <= checkDate.weekday() <= 4
 
     def nextWeekday(forDate=None):
@@ -253,19 +265,22 @@
             return df, df['tradingDate'].tolist()
         except Exception:  # pragma: no cover
             return None, None
 
     def isHoliday(d1=None):
         if isinstance(d1,str):
             d1 = PKDateUtilities.dateFromYmdString(d1)
+        if d1 is None:
+            d1 = PKDateUtilities.currentDateTime()
+        
         today = datetime.datetime.now(pytz.timezone("Asia/Kolkata"))
         if isinstance(d1,datetime.datetime):
             curr = d1.replace(tzinfo=today.tzinfo)
         else:
-            curr = d1
+            curr = d1 if d1 is not None else PKDateUtilities.currentDateTime()
         holidays,_ = PKDateUtilities.holidayList()
         if holidays is None:
             return False, None
 
         today = curr.strftime("%Y-%m-%d")
         occasion = None
         for holiday in holidays["tradingDate"]:
```

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240417.88/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240417.88/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240416.87
+Version: 0.13.20240417.88
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240416.87.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.88.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240416.87/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240417.88/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/PKG-INFO` & `PKDevTools-0.13.20240417.88/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240416.87
+Version: 0.13.20240417.88
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240416.87.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240417.88.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240416.87/README.md` & `PKDevTools-0.13.20240417.88/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240416.87/setup.py` & `PKDevTools-0.13.20240417.88/setup.py`

 * *Files identical despite different names*

