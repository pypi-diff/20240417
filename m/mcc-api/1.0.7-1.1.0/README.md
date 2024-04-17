# Comparing `tmp/mcc_api-1.0.7.tar.gz` & `tmp/mcc_api-1.1.0.tar.gz`

## Comparing `mcc_api-1.0.7.tar` & `mcc_api-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,41 @@
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.0.7/.github/workflows/docs.yml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mcc_api-1.0.7/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mcc_api-1.0.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 mcc_api-1.0.7/docs/conf.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 mcc_api-1.0.7/docs/index.rst
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 mcc_api-1.0.7/mcc_api/__init__.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.0.7/mcc_api/enums.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.0.7/mcc_api/exceptions.py
--rw-r--r--   0        0        0    13133 2020-02-02 00:00:00.000000 mcc_api-1.0.7/mcc_api/responses.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/run_tests.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/test_event.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/test_halloffame.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/test_participants.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/test_rundown.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/200_event.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/200_halloffame.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/200_halloffame_game.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/200_participants.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/200_participants_team.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/200_rundown.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/404_halloffame_game.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/404_participants_team.json
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/404_rundown.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.0.7/tests/mock_data/429_ratelimit.json
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.0.7/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mcc_api-1.0.7/LICENSE
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 mcc_api-1.0.7/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mcc_api-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 mcc_api-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mcc_api-1.1.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mcc_api-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mcc_api-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mcc_api-1.1.0/docs/event.rst
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mcc_api-1.1.0/docs/index.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mcc_api-1.1.0/docs/island.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/__init__.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/event/__init__.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/event/enums.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/event/exceptions.py
+-rw-r--r--   0        0        0    13133 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/event/responses.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/auth.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/directives.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/enums.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/scalars.py
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 mcc_api-1.1.0/mcc_api/island/types.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/run_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/test_event.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/test_halloffame.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/test_participants.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/test_rundown.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_event.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_halloffame.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_halloffame_game.json
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_participants.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_participants_team.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/200_rundown.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/404_halloffame_game.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/404_participants_team.json
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/404_rundown.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/event/mock_data/429_ratelimit.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/island/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 mcc_api-1.1.0/tests/island/test_schema.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mcc_api-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 mcc_api-1.1.0/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mcc_api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mcc_api-1.1.0/PKG-INFO
```

### Comparing `mcc_api-1.0.7/.github/workflows/docs.yml` & `mcc_api-1.1.0/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
   workflow_dispatch:
 jobs:
   build:
     runs-on: ubuntu-latest
 
     steps:
       - name: 📂 Check-Out Repository
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: 🐍 Set Up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
       - name: ⏬ Install Required Packages
         run: |
           python -m pip install --upgrade pip
```

### Comparing `mcc_api-1.0.7/.github/workflows/pypi_publish.yml` & `mcc_api-1.1.0/.github/workflows/pypi_publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
   build:
     runs-on: ubuntu-latest
     permissions:
       id-token: write
 
     steps:
       - name: 📂 Check-Out Repository
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: 🐍 Set Up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
       - name: ⏬ Install Required Packages
         run: |
           python -m pip install --upgrade pip
```

### Comparing `mcc_api-1.0.7/.github/workflows/tests.yml` & `mcc_api-1.1.0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
         python-version:
           - "3.10"
           - "3.11"
           - "3.12"
 
     steps:
       - name: 📂 Check-Out Repository
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: 🐍 Set Up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: "pyproject.toml"
       - name: ⏬ Install Required Packages
         run: |
           python -m pip install --upgrade pip
```

### Comparing `mcc_api-1.0.7/mcc_api/__init__.py` & `mcc_api-1.1.0/mcc_api/event/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .. import __user_agent
 from .enums import (
     Game,
     Team
 )
 from .responses import (
     EventInformationResponse,
     HallOfFameGameResponse,
@@ -21,18 +22,16 @@
     "get_rundown",
     "get_participants",
 
     "enums",
     "exceptions",
     "responses"
 ]
-__version__ = "1.0.7"
 
 __base_url: t.Final[str] = "https://api.mcchampionship.com/v1"
-__user_agent: t.Final[str] = f"python_mcc_api/{__version__} (https://github.com/JamesMCo/python_mcc_api)"
 
 
 @ratelimit.sleep_and_retry
 @ratelimit.limits(calls=40, period=60)
 def __request(endpoint: str, timeout: int) -> requests.Response:
     """Make and return a request to the given endpoint of the MCC API.
```

### Comparing `mcc_api-1.0.7/mcc_api/enums.py` & `mcc_api-1.1.0/mcc_api/event/enums.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.7/mcc_api/exceptions.py` & `mcc_api-1.1.0/mcc_api/event/exceptions.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.7/mcc_api/responses.py` & `mcc_api-1.1.0/mcc_api/event/responses.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.7/tests/run_tests.py` & `mcc_api-1.1.0/tests/run_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,48 +4,56 @@
 
 
 class Result(unittest.TextTestResult):
     def __init__(self, stream, descriptions, verbosity):
         super().__init__(stream, descriptions, verbosity)
         if os.getenv("GITHUB_STEP_SUMMARY"):
             self.job_summary = open(os.getenv("GITHUB_STEP_SUMMARY"), "a", encoding="utf-8")
-            self.job_summary.write(f"# Test Results (Python {'.'.join(str(n) for n in sys.version_info[:3])})\n\n")
-            self.job_summary.write("Name|Result\n-|-\n")
+            self.job_summary.write(f"# Test Results (Python {'.'.join(map(str, sys.version_info[:3]))})\n\n")
+            self.job_summary.write("👑 = `mcc_api.event`\n")
+            self.job_summary.write("🏝️ = `mcc_api.island`\n")
+            self.job_summary.write("&nbsp;|Name|Result\n-|-|-\n")
         else:
             self.job_summary = None
 
+    def getTestName(self, test):
+        name_parts = test.id().split(".")
+        match name_parts[0]:
+            case "event":  return f"👑|{name_parts[-1]}"
+            case "island": return f"🏝️|{name_parts[-1]}"
+
     def addSuccess(self, test):
         super().addSuccess(test)
         if self.job_summary:
-            self.job_summary.write(f"{self.getDescription(test).split()[0]}|✅\n")
+            self.job_summary.write(f"{self.getTestName(test)}|✅\n")
 
     def addError(self, test, err):
         super().addError(test, err)
         if self.job_summary:
-            self.job_summary.write(f"{self.getDescription(test).split()[0]}|❗\n")
+            self.job_summary.write(f"{self.getTestName(test)}|❗\n")
 
     def addFailure(self, test, err):
         super().addFailure(test, err)
         if self.job_summary:
-            self.job_summary.write(f"{self.getDescription(test).split()[0]}|❌\n")
+            self.job_summary.write(f"{self.getTestName(test)}|❌\n")
 
     def addSkip(self, test, reason):
         super().addSkip(test, reason)
         if self.job_summary:
-            self.job_summary.write(f"{self.getDescription(test).split()[0]}|↪️\n")
+            self.job_summary.write(f"{self.getTestName(test)}|↪️\n")
 
     def addExpectedFailure(self, test, err):
         super().addExpectedFailure(test, err)
         if self.job_summary:
-            self.job_summary.write(f"{self.getDescription(test).split()[0]}|✅\n")
+            self.job_summary.write(f"{self.getTestName(test)}|✅\n")
 
     def addUnexpectedSuccess(self, test):
         super().addUnexpectedSuccess(test)
         if self.job_summary:
-            self.job_summary.write(f"{self.getDescription(test).split()[0]}|❌\n")
+            self.job_summary.write(f"{self.getTestName(test)}|❌\n")
 
     def printErrors(self):
         super().printErrors()
         if self.job_summary:
             self.job_summary.write("# Statistics\n")
             errors = len(self.errors)
             expected_failures = len(self.expectedFailures)
@@ -77,15 +85,15 @@
             if self.unexpectedSuccesses:
                 self.job_summary.write("# Unexpected Successes\n")
                 for test in self.unexpectedSuccesses:
                     test_name = self.getDescription(test).split()[1].strip("()")
                     self.job_summary.write(f"## {test_name}\n")
 
     def __del__(self):
-        if self.job_summary:
+        if "job_summary" in self.__dict__ and self.job_summary:
             self.job_summary.close()
 
 
 class Runner(unittest.TextTestRunner):
     def __init__(self, stream=None, descriptions=True, verbosity=1,
                  failfast=False, buffer=False, resultclass=Result, warnings=None,
                  *, tb_locals=False):
```

### Comparing `mcc_api-1.0.7/tests/test_event.py` & `mcc_api-1.1.0/tests/event/test_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from datetime import datetime, timezone
-import mcc_api
+import mcc_api.event as event_api
 import json
 import typing as t
 import unittest
 
 
 class TestEventEndpoint200(unittest.TestCase):
     response_json: dict[str, t.Any]
-    response_object: mcc_api.EventInformationResponse
+    response_object: event_api.EventInformationResponse
 
     def setUp(self: "TestEventEndpoint200") -> None:
-        with open("mock_data/200_event.json") as f:
+        with open("event/mock_data/200_event.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
-        self.response_object = mcc_api.EventInformationResponse(self.response_json)
+        self.response_object = event_api.EventInformationResponse(self.response_json)
 
     def test_date(self: "TestEventEndpoint200") -> None:
         self.assertEqual(self.response_object.data.date, datetime(2023, 4, 2, 1, 13, 3, 587000, timezone.utc))
 
     def test_event_name(self: "TestEventEndpoint200") -> None:
         self.assertEqual(self.response_object.data.event, "22")
 
     def test_update_video(self: "TestEventEndpoint200") -> None:
         self.assertEqual(self.response_object.data.updateVideo, "https://www.youtube.com/embed/LdelXw4FsAE")
 
 
 class TestEventEndpoint429(unittest.TestCase):
     def test_event_ratelimit_exception(self: "TestEventEndpoint429") -> None:
-        with open("mock_data/429_ratelimit.json") as f:
+        with open("event/mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.EventInformationResponse, response_json)
+        self.assertRaises(event_api.exceptions.RateLimitError, event_api.EventInformationResponse, response_json)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mcc_api-1.0.7/tests/test_halloffame.py` & `mcc_api-1.1.0/tests/event/test_halloffame.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import mcc_api
+import mcc_api.event as event_api
 import json
 import typing as t
 import unittest
 
 
 class TestHallOfFameEndpoint200(unittest.TestCase):
     response_json: dict[str, t.Any]
-    response_object: mcc_api.HallOfFameResponse
+    response_object: event_api.HallOfFameResponse
 
     def setUp(self: "TestHallOfFameEndpoint200") -> None:
-        with open("mock_data/200_halloffame.json") as f:
+        with open("event/mock_data/200_halloffame.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
-        self.response_object = mcc_api.HallOfFameResponse(self.response_json)
+        self.response_object = event_api.HallOfFameResponse(self.response_json)
 
     def test_game_names(self: "TestHallOfFameEndpoint200") -> None:
-        self.assertIn(mcc_api.Game.GLOBAL_STATISTICS, self.response_object.data)
-        self.assertIn(mcc_api.Game.LEGACY_STATISTICS, self.response_object.data)
+        self.assertIn(event_api.Game.GLOBAL_STATISTICS, self.response_object.data)
+        self.assertIn(event_api.Game.LEGACY_STATISTICS, self.response_object.data)
 
     def test_records(self: "TestHallOfFameEndpoint200") -> None:
-        for game in [mcc_api.Game.GLOBAL_STATISTICS, mcc_api.Game.LEGACY_STATISTICS]:
+        for game in [event_api.Game.GLOBAL_STATISTICS, event_api.Game.LEGACY_STATISTICS]:
             with self.subTest(game=str(game)):
                 self.assertIn(
                     game,
                     self.response_object.data
                 )
 
-                records: dict[str, mcc_api.responses.HallOfFameRecord] = self.response_object.data[game]
+                records: dict[str, event_api.responses.HallOfFameRecord] = self.response_object.data[game]
 
                 self.assertIn("RECORD NAME 1", records)
                 self.assertEqual(records["RECORD NAME 1"].placement, 0)
                 self.assertEqual(records["RECORD NAME 1"].player, "MCChampionship")
                 self.assertEqual(records["RECORD NAME 1"].value, "String value")
                 self.assertFalse(records["RECORD NAME 1"].changedHands)
 
@@ -41,32 +41,32 @@
                 self.assertTrue(records["RECORD NAME 2"].changedHands)
 
 
 class TestHallOfFameEndpoint429(unittest.TestCase):
     response_json: dict[str, t.Any]
 
     def test_halloffame_ratelimit_exception(self: "TestHallOfFameEndpoint429") -> None:
-        with open("mock_data/429_ratelimit.json") as f:
+        with open("event/mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.HallOfFameResponse, response_json)
+        self.assertRaises(event_api.exceptions.RateLimitError, event_api.HallOfFameResponse, response_json)
 
 
 class TestHallOfFameGameEndpoint200(unittest.TestCase):
     response_json: dict[str, t.Any]
-    response_object: mcc_api.HallOfFameGameResponse
+    response_object: event_api.HallOfFameGameResponse
 
     def setUp(self: "TestHallOfFameGameEndpoint200") -> None:
-        with open("mock_data/200_halloffame_game.json") as f:
+        with open("event/mock_data/200_halloffame_game.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
-        self.response_object = mcc_api.HallOfFameGameResponse(self.response_json)
+        self.response_object = event_api.HallOfFameGameResponse(self.response_json)
 
     def test_records(self: "TestHallOfFameGameEndpoint200") -> None:
-        records: dict[str, mcc_api.responses.HallOfFameRecord] = self.response_object.data
+        records: dict[str, event_api.responses.HallOfFameRecord] = self.response_object.data
 
         self.assertIn("RECORD NAME 1", records)
         self.assertEqual(records["RECORD NAME 1"].placement, 0)
         self.assertEqual(records["RECORD NAME 1"].player, "MCChampionship")
         self.assertEqual(records["RECORD NAME 1"].value, "String value")
         self.assertFalse(records["RECORD NAME 1"].changedHands)
 
@@ -75,23 +75,23 @@
         self.assertEqual(records["RECORD NAME 2"].player, "MCChampionship")
         self.assertEqual(records["RECORD NAME 2"].value, 0)
         self.assertTrue(records["RECORD NAME 2"].changedHands)
 
 
 class TestHallOfFameGameEndpoint404(unittest.TestCase):
     def test_halloffame_game_invalid_game_exception(self: "TestHallOfFameGameEndpoint404") -> None:
-        with open("mock_data/404_halloffame_game.json") as f:
+        with open("event/mock_data/404_halloffame_game.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.InvalidGameError, mcc_api.HallOfFameGameResponse, response_json)
+        self.assertRaises(event_api.exceptions.InvalidGameError, event_api.HallOfFameGameResponse, response_json)
 
 
 class TestHallOfFameGameEndpoint429(unittest.TestCase):
     def test_halloffame_game_ratelimit_exception(self: "TestHallOfFameGameEndpoint429") -> None:
-        with open("mock_data/429_ratelimit.json") as f:
+        with open("event/mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.HallOfFameGameResponse, response_json)
+        self.assertRaises(event_api.exceptions.RateLimitError, event_api.HallOfFameGameResponse, response_json)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mcc_api-1.0.7/tests/test_participants.py` & `mcc_api-1.1.0/tests/event/test_participants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-import mcc_api
+import mcc_api.event as event_api
 import json
 import typing as t
 import unittest
 
 
 class TestEventParticipants200(unittest.TestCase):
     response_json: dict[str, t.Any]
-    response_object: mcc_api.ParticipantsResponse
+    response_object: event_api.ParticipantsResponse
 
     def setUp(self: "TestEventParticipants200") -> None:
-        with open("mock_data/200_participants.json") as f:
+        with open("event/mock_data/200_participants.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
-        self.response_object = mcc_api.ParticipantsResponse(self.response_json)
+        self.response_object = event_api.ParticipantsResponse(self.response_json)
 
     def test_all_teams_present(self: "TestEventParticipants200") -> None:
-        for team in mcc_api.Team:
+        for team in event_api.Team:
             with self.subTest(team=str(team)):
                 self.assertIn(team, self.response_object.data)
 
     def test_all_participants_unique(self: "TestEventParticipants200") -> None:
         participants_count: int = 0
         usernames: set[str] = set()
         uuids: set[str] = set()
 
         for _, participants in self.response_object.data.items():
-            participants: list[mcc_api.responses.Creator]
+            participants: list[event_api.responses.Creator]
             for participant in participants:
-                participant: mcc_api.responses.Creator
+                participant: event_api.responses.Creator
 
                 participants_count += 1
                 usernames.add(participant.username)
                 uuids.add(participant.uuid)
 
         self.assertEqual(participants_count, len(usernames))
         self.assertEqual(participants_count, len(uuids))
 
 
 class TestParticipantsEndpoint429(unittest.TestCase):
     def test_participants_ratelimit_exception(self: "TestParticipantsEndpoint429") -> None:
-        with open("mock_data/429_ratelimit.json") as f:
+        with open("event/mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.ParticipantsResponse, response_json)
+        self.assertRaises(event_api.exceptions.RateLimitError, event_api.ParticipantsResponse, response_json)
 
 
 class TestEventParticipantsTeam200(unittest.TestCase):
     response_json: dict[str, t.Any]
-    response_object: mcc_api.ParticipantsTeamResponse
+    response_object: event_api.ParticipantsTeamResponse
 
     def setUp(self: "TestEventParticipantsTeam200") -> None:
-        with open("mock_data/200_participants_team.json") as f:
+        with open("event/mock_data/200_participants_team.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
-        self.response_object = mcc_api.ParticipantsTeamResponse(self.response_json)
+        self.response_object = event_api.ParticipantsTeamResponse(self.response_json)
 
     def test_all_participants_unique(self: "TestEventParticipantsTeam200") -> None:
         participants_count: int = 0
         usernames: set[str] = set()
         uuids: set[str] = set()
 
         for participant in self.response_object.data:
-            participant: mcc_api.responses.Creator
+            participant: event_api.responses.Creator
 
             participants_count += 1
             usernames.add(participant.username)
             uuids.add(participant.uuid)
 
         self.assertEqual(participants_count, len(usernames))
         self.assertEqual(participants_count, len(uuids))
 
 
 class TestParticipantsTeamEndpoint404(unittest.TestCase):
     def test_participants_team_invalid_team_exception(self: "TestParticipantsTeamEndpoint404") -> None:
-        with open("mock_data/404_participants_team.json") as f:
+        with open("event/mock_data/404_participants_team.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.InvalidTeamError, mcc_api.ParticipantsTeamResponse, response_json)
+        self.assertRaises(event_api.exceptions.InvalidTeamError, event_api.ParticipantsTeamResponse, response_json)
 
 
 class TestParticipantsTeamEndpoint429(unittest.TestCase):
     def test_participants_team_ratelimit_exception(self: "TestParticipantsTeamEndpoint429") -> None:
-        with open("mock_data/429_ratelimit.json") as f:
+        with open("event/mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.ParticipantsTeamResponse, response_json)
+        self.assertRaises(event_api.exceptions.RateLimitError, event_api.ParticipantsTeamResponse, response_json)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mcc_api-1.0.7/tests/test_rundown.py` & `mcc_api-1.1.0/tests/event/test_rundown.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import mcc_api
+import mcc_api.event as event_api
 import json
 import typing as t
 import unittest
 
 
 class TestRundownEndpoint200(unittest.TestCase):
     response_json: dict[str, t.Any]
-    response_object: mcc_api.RundownResponse
+    response_object: event_api.RundownResponse
 
     def setUp(self: "TestRundownEndpoint200") -> None:
-        with open("mock_data/200_rundown.json") as f:
+        with open("event/mock_data/200_rundown.json") as f:
             f: t.TextIO
             self.response_json = json.loads(f.read())
-        self.response_object = mcc_api.RundownResponse(self.response_json)
+        self.response_object = event_api.RundownResponse(self.response_json)
 
     def test_dodgebolt(self: "TestRundownEndpoint200") -> None:
         self.assertEqual(len(self.response_object.data.dodgeboltData), 2)
 
-        team_one: mcc_api.Team
-        team_two: mcc_api.Team
+        team_one: event_api.Team
+        team_two: event_api.Team
         team_one, team_two = self.response_object.data.dodgeboltData.keys()
 
         self.assertNotEqual(team_one, team_two)
         self.assertNotEqual(
             self.response_object.data.dodgeboltData[team_one],
             self.response_object.data.dodgeboltData[team_two]
         )
 
     def test_event_placements_and_scores_match(self: "TestRundownEndpoint200") -> None:
-        placements: list[mcc_api.Team] = sorted(
+        placements: list[event_api.Team] = sorted(
             self.response_object.data.eventPlacements.keys(),
             key=lambda team: self.response_object.data.eventPlacements[team],
             reverse=True
         )
-        scores: list[mcc_api.Team] = sorted(
+        scores: list[event_api.Team] = sorted(
             self.response_object.data.eventScores.keys(),
             key=lambda team: self.response_object.data.eventScores[team]
         )
         self.assertEqual(placements, scores)
 
     def test_event_individual_scores_contain_all_participants(self: "TestRundownEndpoint200") -> None:
-        participant_teams: list[mcc_api.Team] = [
-            mcc_api.Team.RED,
-            mcc_api.Team.ORANGE,
-            mcc_api.Team.YELLOW,
-            mcc_api.Team.LIME,
-            mcc_api.Team.GREEN,
-            mcc_api.Team.CYAN,
-            mcc_api.Team.AQUA,
-            mcc_api.Team.BLUE,
-            mcc_api.Team.PURPLE,
-            mcc_api.Team.PINK
+        participant_teams: list[event_api.Team] = [
+            event_api.Team.RED,
+            event_api.Team.ORANGE,
+            event_api.Team.YELLOW,
+            event_api.Team.LIME,
+            event_api.Team.GREEN,
+            event_api.Team.CYAN,
+            event_api.Team.AQUA,
+            event_api.Team.BLUE,
+            event_api.Team.PURPLE,
+            event_api.Team.PINK
         ]
         participants: list[str] = [
             participant
             for team in participant_teams
             for participant in self.response_object.data.creators[team]
         ]
         self.assertEqual(
@@ -69,23 +69,23 @@
         for game, multiplier in zip(range(8), [1, 1.5, 1.5, 2, 2, 2.5, 2.5, 3]):
             with self.subTest(game=game):
                 self.assertEqual(self.response_object.data.history[str(game)].multiplier, multiplier)
 
 
 class TestRundownEndpoint404(unittest.TestCase):
     def test_rundown_invalid_event_exception(self: "TestRundownEndpoint404") -> None:
-        with open("mock_data/404_rundown.json") as f:
+        with open("event/mock_data/404_rundown.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.InvalidEventError, mcc_api.RundownResponse, response_json)
+        self.assertRaises(event_api.exceptions.InvalidEventError, event_api.RundownResponse, response_json)
 
 
 class TestRundownEndpoint429(unittest.TestCase):
     def test_rundown_ratelimit_exception(self: "TestRundownEndpoint429") -> None:
-        with open("mock_data/429_ratelimit.json") as f:
+        with open("event/mock_data/429_ratelimit.json") as f:
             f: t.TextIO
             response_json: dict[str, t.Any] = json.loads(f.read())
-        self.assertRaises(mcc_api.exceptions.RateLimitError, mcc_api.RundownResponse, response_json)
+        self.assertRaises(event_api.exceptions.RateLimitError, event_api.RundownResponse, response_json)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mcc_api-1.0.7/tests/mock_data/200_halloffame.json` & `mcc_api-1.1.0/tests/event/mock_data/200_halloffame.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.7/tests/mock_data/200_participants.json` & `mcc_api-1.1.0/tests/event/mock_data/200_participants.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.7/tests/mock_data/200_participants_team.json` & `mcc_api-1.1.0/tests/event/mock_data/200_participants_team.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.7/tests/mock_data/200_rundown.json` & `mcc_api-1.1.0/tests/event/mock_data/200_rundown.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.7/.gitignore` & `mcc_api-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mcc_api-1.0.7/LICENSE` & `mcc_api-1.1.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 James C
+Copyright (c) 2023-2024 James C
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mcc_api-1.0.7/pyproject.toml` & `mcc_api-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 requires-python = ">= 3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "gql[requests]",
     "ratelimit",
     "requests"
 ]
 dynamic = [
     "version"
 ]
```

