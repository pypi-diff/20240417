# Comparing `tmp/jellyash-0.5.2.tar.gz` & `tmp/jellyash-0.5.3.tar.gz`

## Comparing `jellyash-0.5.2.tar` & `jellyash-0.5.3.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jellyash-0.5.2/tox.ini
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 jellyash-0.5.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/bundle.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/cli.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/client.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/duration.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/nextup.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/search.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/token.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 jellyash-0.5.2/jellyash/unwatched.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/test_bundle.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/test_client.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/test_duration.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/test_nextup.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/test_search.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/test_token.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/test_unwatched.py
--rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_bundle/TestApiResponse.client.yaml
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_bool_response.yaml
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_dict_response.yaml
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_client/TestAuthedClient.client.yaml
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_duration/TestDuration.client.yaml
--rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact_with_space.yaml
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_single_term.yaml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_term_not_found.yaml
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.client.yaml
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_season.yaml
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_with_season.yaml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jellyash-0.5.2/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 jellyash-0.5.2/LICENSE
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 jellyash-0.5.2/README.md
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 jellyash-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 jellyash-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jellyash-0.5.3/tox.ini
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 jellyash-0.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/bundle.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/cli.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/client.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/duration.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/nextup.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/search.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/token.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/unwatched.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_bundle.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_client.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_duration.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_nextup.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_search.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_token.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_unwatched.py
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestApiResponse.client.yaml
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_bool_response.yaml
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_dict_response.yaml
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.client.yaml
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.client.yaml
+-rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact_with_space.yaml
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_single_term.yaml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_term_not_found.yaml
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.client.yaml
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_season.yaml
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_special_season.yaml
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_with_season.yaml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jellyash-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 jellyash-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 jellyash-0.5.3/README.md
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 jellyash-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 jellyash-0.5.3/PKG-INFO
```

### Comparing `jellyash-0.5.2/.github/workflows/ci.yml` & `jellyash-0.5.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/jellyash/bundle.py` & `jellyash-0.5.3/jellyash/bundle.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/jellyash/client.py` & `jellyash-0.5.3/jellyash/client.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/jellyash/duration.py` & `jellyash-0.5.3/jellyash/duration.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/jellyash/nextup.py` & `jellyash-0.5.3/jellyash/nextup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 
 def episode_str(episode: Item) -> str:
     seasonindex = f"{episode.ParentIndexNumber}x{episode.IndexNumber:0>2}"
     return f"{episode.SeriesName} [{seasonindex}] {episode.Name}"
 
 
 def nextup() -> None:
-    client = authed_client()
     parser = argparse_parser()
     parser.add_argument("-l", "--limit", dest="limit", type=int, default=30)
     args = parser.parse_args()
+    client = authed_client()
     for episode in client.jellyfin.get_next(limit=args.limit):
         print(episode_str(episode))
```

### Comparing `jellyash-0.5.2/jellyash/search.py` & `jellyash-0.5.3/jellyash/search.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/jellyash/token.py` & `jellyash-0.5.3/jellyash/token.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from getpass import getuser
 
 from .cli import argparse_parser
 from .client import CREDENTIALS_FILE, auth_with_password, create_client
 
 
 def create_jellyfin_token() -> None:
-    client = create_client("create_jellyfin_token")
     parser = argparse_parser()
     parser.add_argument("-u", "--user", dest="user", default=getuser())
     parser.add_argument(
         "server", nargs="?", default="https://jellyfin.wedontsleep.org/"
     )
     args = parser.parse_args()
     password = getpassword()
+    client = create_client("create_jellyfin_token")
     result = auth_with_password(client, args.server, args.user, password)
     if "AccessToken" in result:
         credentials = client.auth.credentials.get_credentials()
         server = credentials["Servers"][0]
         server["username"] = args.user
         with open(CREDENTIALS_FILE, "w") as f:
             json.dump(server, f)
```

### Comparing `jellyash-0.5.2/jellyash/unwatched.py` & `jellyash-0.5.3/jellyash/unwatched.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 
 def pluralized_str(count: int, prefix: str = "un") -> str:
     return f"{count} {prefix}watched episode{'s' if count != 1 else ''}"
 
 
 def unwatched() -> None:
-    client = authed_client()
     parser = argparse_parser()
     parser.add_argument("show", nargs="*")
     parser.add_argument("-s", "--season", type=int)
     args = parser.parse_args()
+    client = authed_client()
     if args.season and not args.show:
         parser.error("Need to specify a show when specifiying a season")
     if not args.show:
         all_unwatched(client)
     else:
         specific_unwatched(client, " ".join(args.show), season=args.season)
 
@@ -40,20 +40,23 @@
     try:
         show = search_single_show(client, term)
     except ValueError as e:
         print(str(e))
         return
     seasons = client.jellyfin.get_seasons(show.Id)
     name = f"{show.Name}"
-    if season:
+    if season is not None:
         try:
             show = next(s for s in seasons if s.IndexNumber == season)
         except StopIteration:
             print(f"Can not find season {season} of {name}")
             return
-        name += f", Season {season}"
+        if season >= 1:
+            name += f", Season {season}"
+        else:
+            name += ", Specials"
         total = show.ChildCount
     else:
         total = sum(s.ChildCount for s in seasons)
     unwatched = show.UserData.UnplayedItemCount
     print(f"{name}: {pluralized_str(total - unwatched, prefix='')}")
     print(f"{name}: {pluralized_str(unwatched)}")
```

### Comparing `jellyash-0.5.2/tests/conftest.py` & `jellyash-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/test_bundle.py` & `jellyash-0.5.3/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/test_client.py` & `jellyash-0.5.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/test_duration.py` & `jellyash-0.5.3/tests/test_duration.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/test_nextup.py` & `jellyash-0.5.3/tests/test_nextup.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/test_search.py` & `jellyash-0.5.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/test_token.py` & `jellyash-0.5.3/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_bundle/TestApiResponse.client.yaml` & `jellyash-0.5.3/tests/cassettes/test_bundle/TestApiResponse.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml` & `jellyash-0.5.3/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml` & `jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_bool_response.yaml` & `jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_bool_response.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_dict_response.yaml` & `jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_dict_response.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_client/TestAuthedClient.client.yaml` & `jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml` & `jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml` & `jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml` & `jellyash-0.5.3/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_duration/TestDuration.client.yaml` & `jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml` & `jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml` & `jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml` & `jellyash-0.5.3/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml` & `jellyash-0.5.3/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml` & `jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact_with_space.yaml` & `jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact_with_space.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml` & `jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_search/TestSearch.test_single_term.yaml` & `jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_single_term.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml` & `jellyash-0.5.3/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.client.yaml` & `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml` & `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml` & `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml` & `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_season.yaml` & `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_season.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_with_season.yaml` & `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_with_season.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/LICENSE` & `jellyash-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/README.md` & `jellyash-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/pyproject.toml` & `jellyash-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.2/PKG-INFO` & `jellyash-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jellyash
-Version: 0.5.2
+Version: 0.5.3
 Project-URL: Source, https://github.com/s-t-e-v-e-n-k/jellyash
 License: Copyright 2023 Steve Kowalik <steven@wedontsleep.org>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

