# Comparing `tmp/twitter_openapi_python-0.0.8.tar.gz` & `tmp/twitter_openapi_python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter_openapi_python-0.0.8.tar", last modified: Thu Sep 28 07:14:26 2023, max compression
+gzip compressed data, was "twitter_openapi_python-0.0.9.tar", last modified: Thu Sep 28 07:42:37 2023, max compression
```

## Comparing `twitter_openapi_python-0.0.8.tar` & `twitter_openapi_python-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-09-28 07:14:26.615965 twitter_openapi_python-0.0.8/
--rw-rw-rw-   0        0        0     1524 2023-09-20 00:48:17.000000 twitter_openapi_python-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    35182 2023-09-20 00:48:17.000000 twitter_openapi_python-0.0.8/LICENSE.AGPL
--rw-rw-rw-   0        0        0      461 2023-09-28 07:14:26.615965 twitter_openapi_python-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1442 2023-09-28 07:12:32.000000 twitter_openapi_python-0.0.8/README.md
--rw-rw-rw-   0        0        0      765 2023-09-28 07:14:18.000000 twitter_openapi_python-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-28 07:14:26.616960 twitter_openapi_python-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-09-28 07:14:18.000000 twitter_openapi_python-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-28 07:14:26.566961 twitter_openapi_python-0.0.8/twitter_openapi_python/
--rw-rw-rw-   0        0        0      339 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-28 07:14:26.606963 twitter_openapi_python-0.0.8/twitter_openapi_python/api/
--rw-rw-rw-   0        0        0      643 2023-09-20 02:13:35.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/__init__.py
--rw-rw-rw-   0        0        0     2666 2023-09-28 03:58:19.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/default_api.py
--rw-rw-rw-   0        0        0     2339 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/initial_state_api.py
--rw-rw-rw-   0        0        0     5607 2023-09-20 02:30:21.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/post_api.py
--rw-rw-rw-   0        0        0     9887 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/tweet_api.py
--rw-rw-rw-   0        0        0     2464 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/user_api.py
--rw-rw-rw-   0        0        0     5637 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/user_list_api.py
--rw-rw-rw-   0        0        0     1789 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/users_api.py
--rw-rw-rw-   0        0        0     2254 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/v11_get_api.py
--rw-rw-rw-   0        0        0     2051 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/api/v11_post_api.py
--rw-rw-rw-   0        0        0     5758 2023-09-28 04:24:16.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/client.py
-drwxrwxrwx   0        0        0        0 2023-09-28 07:14:26.611961 twitter_openapi_python-0.0.8/twitter_openapi_python/models/
--rw-rw-rw-   0        0        0      597 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/models/__init__.py
--rw-rw-rw-   0        0        0      327 2023-08-08 05:12:37.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/models/base.py
--rw-rw-rw-   0        0        0      594 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/models/header.py
--rw-rw-rw-   0        0        0      530 2023-08-08 05:11:52.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/models/initial_state.py
--rw-rw-rw-   0        0        0      497 2023-08-08 05:11:54.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/models/response.py
--rw-rw-rw-   0        0        0     1409 2023-08-08 05:11:55.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/models/timeline.py
--rw-rw-rw-   0        0        0        0 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/py.typed
-drwxrwxrwx   0        0        0        0 2023-09-28 07:14:26.614963 twitter_openapi_python-0.0.8/twitter_openapi_python/utils/
--rw-rw-rw-   0        0        0      430 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/utils/__init__.py
--rw-rw-rw-   0        0        0     8762 2023-09-28 04:26:31.000000 twitter_openapi_python-0.0.8/twitter_openapi_python/utils/api.py
-drwxrwxrwx   0        0        0        0 2023-09-28 07:14:26.593971 twitter_openapi_python-0.0.8/twitter_openapi_python.egg-info/
--rw-rw-rw-   0        0        0      461 2023-09-28 07:14:26.000000 twitter_openapi_python-0.0.8/twitter_openapi_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2023-09-28 07:14:26.000000 twitter_openapi_python-0.0.8/twitter_openapi_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-28 07:14:26.000000 twitter_openapi_python-0.0.8/twitter_openapi_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-09-28 07:14:26.000000 twitter_openapi_python-0.0.8/twitter_openapi_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-09-28 07:14:26.000000 twitter_openapi_python-0.0.8/twitter_openapi_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-09-28 07:42:37.678357 twitter_openapi_python-0.0.9/
+-rw-rw-rw-   0        0        0     1524 2023-09-20 00:48:17.000000 twitter_openapi_python-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    35182 2023-09-20 00:48:17.000000 twitter_openapi_python-0.0.9/LICENSE.AGPL
+-rw-rw-rw-   0        0        0      461 2023-09-28 07:42:37.677355 twitter_openapi_python-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1442 2023-09-28 07:12:32.000000 twitter_openapi_python-0.0.9/README.md
+-rw-rw-rw-   0        0        0      765 2023-09-28 07:42:12.000000 twitter_openapi_python-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-09-28 07:42:37.678357 twitter_openapi_python-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-09-28 07:42:13.000000 twitter_openapi_python-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-28 07:42:37.637357 twitter_openapi_python-0.0.9/twitter_openapi_python/
+-rw-rw-rw-   0        0        0      339 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-09-28 07:42:37.668357 twitter_openapi_python-0.0.9/twitter_openapi_python/api/
+-rw-rw-rw-   0        0        0      643 2023-09-20 02:13:35.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/__init__.py
+-rw-rw-rw-   0        0        0     2751 2023-09-28 07:27:53.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/default_api.py
+-rw-rw-rw-   0        0        0     2339 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/initial_state_api.py
+-rw-rw-rw-   0        0        0     5607 2023-09-20 02:30:21.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/post_api.py
+-rw-rw-rw-   0        0        0     9941 2023-09-28 07:32:16.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/tweet_api.py
+-rw-rw-rw-   0        0        0     2619 2023-09-28 07:23:49.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/user_api.py
+-rw-rw-rw-   0        0        0     5637 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/user_list_api.py
+-rw-rw-rw-   0        0        0     1789 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/users_api.py
+-rw-rw-rw-   0        0        0     2254 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/v11_get_api.py
+-rw-rw-rw-   0        0        0     2051 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/api/v11_post_api.py
+-rw-rw-rw-   0        0        0     5758 2023-09-28 04:24:16.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/client.py
+drwxrwxrwx   0        0        0        0 2023-09-28 07:42:37.674356 twitter_openapi_python-0.0.9/twitter_openapi_python/models/
+-rw-rw-rw-   0        0        0      597 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/models/__init__.py
+-rw-rw-rw-   0        0        0      327 2023-08-08 05:12:37.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/models/base.py
+-rw-rw-rw-   0        0        0      594 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/models/header.py
+-rw-rw-rw-   0        0        0      530 2023-08-08 05:11:52.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/models/initial_state.py
+-rw-rw-rw-   0        0        0      497 2023-08-08 05:11:54.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/models/response.py
+-rw-rw-rw-   0        0        0     1409 2023-08-08 05:11:55.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/models/timeline.py
+-rw-rw-rw-   0        0        0        0 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/py.typed
+drwxrwxrwx   0        0        0        0 2023-09-28 07:42:37.676355 twitter_openapi_python-0.0.9/twitter_openapi_python/utils/
+-rw-rw-rw-   0        0        0      430 2023-09-15 02:12:51.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/utils/__init__.py
+-rw-rw-rw-   0        0        0     8894 2023-09-28 07:21:46.000000 twitter_openapi_python-0.0.9/twitter_openapi_python/utils/api.py
+drwxrwxrwx   0        0        0        0 2023-09-28 07:42:37.657363 twitter_openapi_python-0.0.9/twitter_openapi_python.egg-info/
+-rw-rw-rw-   0        0        0      461 2023-09-28 07:42:37.000000 twitter_openapi_python-0.0.9/twitter_openapi_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2023-09-28 07:42:37.000000 twitter_openapi_python-0.0.9/twitter_openapi_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-28 07:42:37.000000 twitter_openapi_python-0.0.9/twitter_openapi_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-09-28 07:42:37.000000 twitter_openapi_python-0.0.9/twitter_openapi_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-09-28 07:42:37.000000 twitter_openapi_python-0.0.9/twitter_openapi_python.egg-info/top_level.txt
```

### Comparing `twitter_openapi_python-0.0.8/LICENSE` & `twitter_openapi_python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/LICENSE.AGPL` & `twitter_openapi_python-0.0.9/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/README.md` & `twitter_openapi_python-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/pyproject.toml` & `twitter_openapi_python-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twitter_openapi_python"
-version = "0.0.8"
+version = "0.0.9"
 description = "Twitter OpenAPI"
 authors = ["fa0311 <yuki@yuki0311.com>"]
 license = "proprietary" # or "AGPL-3.0-only"
 readme = "README.md"
 license_file = "LICENSE"
 repository = "https://github.com/fa0311/twitter_openapi_python"
 keywords = ["twitter", "api", "python", "scraper"]
```

### Comparing `twitter_openapi_python-0.0.8/setup.py` & `twitter_openapi_python-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import find_packages, setup
 
 NAME = "twitter_openapi_python"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "twitter_openapi_python_generated == 0.0.6",
     "pydantic >= 1.10.5, < 2",
 ]
 
 setup(
```

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/__init__.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/default_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/default_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,21 +63,23 @@
         )
         return response
 
     def get_tweet_result_by_rest_id(
         self,
         tweet_id: str,
         extra_param: Optional[ParamType] = None,
-    ) -> TwitterApiUtilsResponse[TweetApiUtilsData | None]:
+    ) -> TwitterApiUtilsResponse[TweetApiUtilsData]:
         param: ParamType = {"tweetId": tweet_id}
         if extra_param is not None:
             param.update(extra_param)
 
         response = self.request(
             apiFn=self.api.get_tweet_result_by_rest_id_with_http_info,
             convertFn=lambda x: build_tweet_api_utils(x.data.tweet_result),
             type1=models.TweetResultByRestIdResponse,
             type2=TweetApiUtilsData,
             key="TweetResultByRestId",
             param=param,
         )
-        return response
+        if response.data is None:
+            raise Exception("No tweet")
+        return response  # type: ignore
```

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/initial_state_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/initial_state_api.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/post_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/post_api.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/tweet_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/tweet_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,17 @@
         if count is not None:
             param["count"] = count
         if extra_param is not None:
             param.update(extra_param)
 
         response = self.request(
             apiFn=self.api.get_list_latest_tweets_timeline_with_http_info,
-            convertFn=lambda e: e.data.list.tweets_timeline.timeline.instructions,
+            convertFn=lambda e: []
+            if (x := e.data.list.tweets_timeline.timeline) is None
+            else x.instructions,
             type=models.ListLatestTweetsTimelineResponse,
             key="ListLatestTweetsTimeline",
             param=param,
         )
         return response
 
     def get_user_tweets(
```

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/user_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/user_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,22 @@
         param: ParamType,
     ) -> ResponseType:
         args = get_kwargs(flag=self.flag[key], additional=param)
         res = apiFn(**args)
         checked = check_error(data=res, type=type)
 
         result = convertFn(checked)
+        if result.result is None:
+            # never reach this point.
+            raise Exception("No user")
+
         user = user_or_null_converter(result.result)
 
         if user is None:
+            # never reach this point.
             raise Exception("No user")
 
         data = UserApiUtilsData(
             raw=result,
             user=user,
         )
```

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/user_list_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/user_list_api.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/users_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/users_api.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/v11_get_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/v11_get_api.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/api/v11_post_api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/api/v11_post_api.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/client.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/client.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/models/__init__.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/models/__init__.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/models/header.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/models/header.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/models/initial_state.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/models/initial_state.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/models/timeline.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/models/timeline.py`

 * *Files identical despite different names*

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python/utils/api.py` & `twitter_openapi_python-0.0.9/twitter_openapi_python/utils/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,16 @@
     reply: Optional[List[models.TimelineTweet]] = None,
 ) -> Optional[TweetApiUtilsData]:
     tweet = tweet_results_converter(result)
     if tweet is None:
         return None
     if tweet.core is None:
         return None
+    if tweet.core.user_results.result is None:
+        return None
     user = user_or_null_converter(tweet.core.user_results.result)
     if user is None:
         return None
 
     quoted = tweet.quoted_status_result
 
     retweeted = None if tweet.legacy is None else tweet.legacy.retweeted_status_result
@@ -175,14 +177,16 @@
                 return item.user_results
 
     return non_nullable_list(list(map(map_fn, item)))
 
 
 def user_result_converter(item: list[models.UserResults]) -> List[UserApiUtilsData]:
     def map_fn(raw: models.UserResults) -> Optional[UserApiUtilsData]:
+        if raw.result is None:
+            return None
         user = user_or_null_converter(raw.result)
         if user is None:
             return None
 
         return UserApiUtilsData(
             raw=raw,
             user=user,
@@ -231,15 +235,16 @@
         transaction_id=headers["x-transaction-id"],
         twitter_response_tags=headers["x-twitter-response-tags"],
         xss_protection=int(headers["x-xss-protection"]),
     )
 
 
 def build_response(
-    response: twitter.ApiResponse, data: T1
+    response: twitter.ApiResponse,
+    data: T1,
 ) -> TwitterApiUtilsResponse[T1]:
     if response.headers is None:
         raise Exception("headers is None")
 
     header = build_header(response.headers)
 
     return TwitterApiUtilsResponse(
```

### Comparing `twitter_openapi_python-0.0.8/twitter_openapi_python.egg-info/SOURCES.txt` & `twitter_openapi_python-0.0.9/twitter_openapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

