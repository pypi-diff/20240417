# Comparing `tmp/mloggers-1.1.7.tar.gz` & `tmp/mloggers-1.2.0.tar.gz`

## Comparing `mloggers-1.1.7.tar` & `mloggers-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.1.7/.taplo.toml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/__init__.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/_log_levels.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/console_logger.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/file_logger.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/logger.py
--rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/multi_logger.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/progress.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 mloggers-1.1.7/mloggers/wandb_logger.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.1.7/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.1.7/LICENSE
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 mloggers-1.1.7/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mloggers-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 mloggers-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.2.0/.taplo.toml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/__init__.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/_log_levels.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/console_logger.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/file_logger.py
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/logger.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/multi_logger.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/progress.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 mloggers-1.2.0/mloggers/wandb_logger.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 mloggers-1.2.0/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mloggers-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 mloggers-1.2.0/PKG-INFO
```

### Comparing `mloggers-1.1.7/mloggers/_log_levels.py` & `mloggers-1.2.0/mloggers/_log_levels.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.7/mloggers/console_logger.py` & `mloggers-1.2.0/mloggers/console_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,20 +12,19 @@
     """Logs to the console (i.e., standard I/O)."""
 
     def __init__(self, default_level: LogLevel = LogLevel.INFO):  # type:ignore[reportArgumentType]
         super().__init__(default_level)
 
     def log(
         self,
-        message: str | dict[str, Any],
+        *messages: str | dict[str, Any],
         level: LogLevel | str | None = None,
-        *args: Any,
         **kwargs: Any,
     ):
-        if not super(ConsoleLogger, self).log(message, level, *args, **kwargs):
+        if not super(ConsoleLogger, self).log(*messages, level=level, **kwargs):
             return
 
         time = "[" + datetime.now().strftime("%H:%M:%S") + "]"
 
         if level is None:
             level_str = ""
             level_clr = ""
@@ -41,18 +40,38 @@
                 level_clr = colored(level_str, level.value["color"])
             else:
                 level_clr = colored(level_str, "green")
 
         # The first level of the dictionary is printed as a multiline
         # indented message.
         # The rest of the levels are printed as a single line
-        # pretifyed depending on the type of the value.
-        if isinstance(message, dict):
+        # prettifyed depending on the type of the value.
+
+        # Handle multiple messages
+        if len(messages) > 1:
+            messages = list(messages)
+            # If the messages are strings, join them into a single string.
+            if all(
+                hasattr(message, "__str__")
+                and callable(getattr(message, "__str__"))
+                and not isinstance(message, dict)
+                for message in messages
+            ):
+                messages = " ".join([str(message) for message in messages])
+            # If the messages are dictionaries, log them separately.
+            else:
+                for message in messages:
+                    self.log(message, level=level)
+                return
+        else:
+            messages = messages[0]
+
+        if isinstance(messages, dict):
             first = True
-            for key, value in message.items():
+            for key, value in messages.items():
                 if not first:
                     time = " " * len(time)
                     level_clr = " " * len(level_str)
 
                 if isinstance(value, float):
                     print(f"{level_clr}{time} {key}: {value:.5f}")
                 elif isinstance(value, dict | list):
@@ -61,9 +80,10 @@
                 elif value is None:  # Used for headers, titles, etc.
                     print(f"{level_clr}{time} {key}")
                 else:
                     print(f"{level_clr}{time} {key}: {value}")
 
                 first = False
 
-        elif hasattr(message, "__str__") and callable(getattr(message, "__str__")):
-            print(f"{level_clr}{time} {str(message)}")
+        elif hasattr(messages, "__str__") and callable(getattr(messages, "__str__")):
+            print(f"{level_clr}{time} {str(messages)}")
+
```

### Comparing `mloggers-1.1.7/mloggers/file_logger.py` & `mloggers-1.2.0/mloggers/file_logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,22 +41,40 @@
 
         print(f'{colored("[INFO]", "cyan")} [FileLogger] Logging to file {file_path}')
 
         self._file_path = file_path
 
     def log(
         self,
-        message: str | dict[str, Any],
+        *messages: str | dict[str, Any],
         level: LogLevel | str | None = None,
-        *args: Any,
         **kwargs: Any,
     ):
-        if not super(FileLogger, self).log(message, level, *args, **kwargs):
+        if not super(FileLogger, self).log(*messages, level=level, **kwargs):
             return
 
+        # Handle multiple messages
+        if len(messages) > 1:
+            messages = list(messages)
+            # If the messages are strings, join them into a single string.
+            if all(
+                hasattr(message, "__str__")
+                and callable(getattr(message, "__str__"))
+                and not isinstance(message, dict)
+                for message in messages
+            ):
+                message = " ".join([str(message) for message in messages])
+            # If the messages are dictionaries, log them separately.
+            else:
+                for message in messages:
+                    self.log(message, level=level)
+                return
+        else:
+            message = messages[0]
+
         # Convert numpy's ndarrays to lists so that they are JSON serializable
         if isinstance(message, dict):
             for key, value in message.items():
                 if isinstance(value, np.ndarray):
                     message[key] = value.tolist()
         elif hasattr(message, "__str__") and callable(getattr(message, "__str__")):
             message = str(message)
```

### Comparing `mloggers-1.1.7/mloggers/logger.py` & `mloggers-1.2.0/mloggers/multi_logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,173 +1,183 @@
-from abc import ABC, abstractmethod
-from typing import Any, Callable
+from typing import Any
 
 from mloggers._log_levels import LogLevel
+from mloggers.logger import Logger
 
-# This constant is used to assign an importance level to anything not using the LogLevel enum.
-# It was chosen to be the same as LogLevel.INFO, but it can be changed to any other value.
-DEFAULT_IMPORTANCE = LogLevel.INFO.value["level"]  # type:ignore[reportAttributeAccessIssue]
 
+class MultiLogger(Logger):
+    """Logs to multiple loggers."""
 
-class Logger(ABC):
-    """The abstract class for a logger."""
+    def __init__(
+        self,
+        loggers: list[Logger],
+        default_mask: list[type[Logger]] = [],
+        default_level: LogLevel | int = LogLevel.INFO,  # type:ignore[reportArgumentType]
+    ):
+        """
+        Initializes a multi-logger.
 
-    def __init__(self, default_level: LogLevel | int = LogLevel.INFO):  # type:ignore[reportArgumentType]
+        ### Parameters
+        ----------
+        `loggers`: a list of the initialized loggers to use.
+        `default_mask`: the default mask to use when logging.
+        `default_level`: the default log level to use.
         """
-        Initialize the logger.
+
+        super().__init__(default_level)
+
+        self._loggers = loggers
+        self._default_mask = default_mask
+
+        for logger in self._loggers:
+            logger.set_level(self._log_level)
+
+    def set_level(self, level: LogLevel | int):
+        """
+        Sets the log level of the multi-logger.
 
         ### Parameters
         ----------
-        `log_level`: the default log level to use.
-        - This parameter filters out messages with a lower importance level than the one provided. It can be either a `LogLevel` object or an integer.
-        - When calling the logger with a level not from the `LogLevel` enum, the importance level will be set to 0 (same as `LogLevel.INFO`).
-        - For example, if the log level is set to `LogLevel.INFO`, only messages with a level of `LogLevel.INFO` or higher will be printed (which excludes `LogLevel.DEBUG`).
+        `level`: the level to set.
         """
 
-        self._log_level = (
-            default_level.value["level"]
-            if isinstance(default_level, LogLevel)
-            else default_level
-        )
+        super(MultiLogger, self).set_level(level)
+
+        for logger in self._loggers:
+            logger.set_level(self._log_level)
 
-    @abstractmethod
     def log(
         self,
-        message: str | dict[str, Any],
+        *messages: str | dict[str, Any],
         level: LogLevel | str | None = None,
-        *args: Any,
+        mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
-        Log a message.
+        Logs a message to multiple loggers.
 
         ### Parameters
         ----------
-        `message`: the message to log.
+        `messages`: the messages to log.
+        - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
         `level`: the level of the message (e.g., INFO, WARN, ERROR, DEBUG, etc.).
         - If None, no level will be printed.
         - If a string is provided, it will be colored in green (when colors are used) and uppercased; otherwise, the color will be the one associated with the `LogLevel` at time of registration.
+        - If multiple messages are provided, they must be either all strings or all dictionaries. Strings will be joined into a single string, while dictionaries will be printed as separate log entries.
 
         ### Raises
         ----------
         `TypeError`: if the message is not a string, a dictionary or does not implement `__str__()`.
+        `TypeError`: if the messages are a mix of strings and dictionaries.
         """
 
-        if (
-            not isinstance(message, dict)
-            and not hasattr(message, "__str__")
-            and not callable(getattr(message, "__str__"))
-        ):
-            raise TypeError(
-                f"Expected message to be a string, a dictionary or to have implemented __str__(), but got {type(message)}."
-            )
-
-        # Filter out messages with a lower importance level than the current log level.
-        if isinstance(level, LogLevel) and level.value["level"] < self._log_level:
-            return False
-        elif isinstance(level, str) and DEFAULT_IMPORTANCE < self._log_level:
-            return False
-        return True
-
-    def set_level(self, level: LogLevel | int):
-        """
-        Set the log level.
-
-        ### Parameters
-        ----------
-        `level`: the log level to set.
-        - If a string, it must be a valid log level (e.g., INFO, WARN, ERROR, DEBUG, etc.).
-        - If a `LogLevel` object, it will be used as-is.
-        """
-        self._log_level = level.value["level"] if isinstance(level, LogLevel) else level
+        # NOTE: No need for checking the validity of the message, as the individual loggers will do that.
+        # super(MultiLogger, self).log(message, level, *args, **kwargs)
 
-    def _call_impl(self, *args, **kwargs):
-        return self.log(*args, **kwargs)
+        if mask is None:
+            mask = self._default_mask
 
-    __call__: Callable[..., Any] = _call_impl
+        for logger in [
+            logger
+            for logger in self._loggers
+            if not any(isinstance(logger, type) for type in mask)
+        ]:
+            logger(*messages, level=level, **kwargs)
 
     def info(
         self,
-        message: str | dict[str, Any],
-        *args: Any,
+        *messages: str | dict[str, Any],
+        mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.INFO.
 
         ### Parameters
         ----------
-        `message`: the message to log.
+        `messages`: the messages to log.
+        - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
+        `mask`: a list of logger names to not be used to log this message.
+        - If None, the default mask will be used.
         """
 
-        self.log(message, LogLevel.INFO, *args, **kwargs)  # type:ignore[reportArgumentType]
+        self.log(*messages, level=LogLevel.INFO, mask=mask, **kwargs)  # type:ignore[reportArgumentType]
 
     def warn(
         self,
-        message: str | dict[str, Any],
-        *args: Any,
+        *messages: str | dict[str, Any],
+        mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.WARN.
 
         ### Parameters
         ----------
-        `message`: the message to log.
+        `messages`: the messages to log.
+        - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
+        `mask`: a list of logger names to not be used to log this message.
+        - If None, the default mask will be used.
         """
 
-        self.log(message, LogLevel.WARN, *args, **kwargs)  # type:ignore[reportArgumentType]
+        self.log(*messages, level=LogLevel.WARN, mask=mask, **kwargs)  # type:ignore[reportArgumentType]
 
     # Alias warning to warn
     warning = warn
 
     def error(
         self,
-        message: str | dict[str, Any],
-        *args: Any,
+        *messages: str | dict[str, Any],
+        mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.ERROR.
 
         ### Parameters
         ----------
-        `message`: the message to log.
+        `messages`: the messages to log.
+        - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
+        `mask`: a list of logger names to not be used to log this message.
+        - If None, the default mask will be used.
         """
 
-        self.log(message, LogLevel.ERROR, *args, **kwargs)  # type:ignore[reportArgumentType]
+        self.log(*messages, level=LogLevel.ERROR, mask=mask, **kwargs)  # type:ignore[reportArgumentType]
 
     def debug(
         self,
-        message: str | dict[str, Any],
-        *args: Any,
+        *messages: str | dict[str, Any],
+        mask: list[type[Logger]] | None = None,
         **kwargs: Any,
     ):
         """
         Wrapper for calling `log` with level=LogLevel.DEBUG.
 
         ### Parameters
         ----------
-        `message`: the message to log.
+        `messages`: the messages to log.
+        - These can be any number of messages, separated by commas. They can be of the following types:
         - If a stringifiable object (implements `__str__()`), the message will be logged as-is.
         - If a dictionary, the message will be logged as a JSON string.
             - The dictionary must be JSON serializable.
             - You can provide None dictionary values to mean that the key is a header or title of the message.
+        `mask`: a list of logger names to not be used to log this message.
+        - If None, the default mask will be used.
         """
 
-        self.log(message, LogLevel.DEBUG, *args, **kwargs)  # type:ignore[reportArgumentType]
+        self.log(*messages, level=LogLevel.DEBUG, mask=mask, **kwargs)  # type:ignore[reportArgumentType]
```

### Comparing `mloggers-1.1.7/mloggers/progress.py` & `mloggers-1.2.0/mloggers/progress.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.7/mloggers/wandb_logger.py` & `mloggers-1.2.0/mloggers/wandb_logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,25 +35,46 @@
 
         if config is not None:
             config = vars(config)
         wandb.init(project=project, group=group, name=experiment, config=config)
 
     def log(
         self,
-        message: str | dict[str, Any],
+        *messages: str | dict[str, Any],
         level: LogLevel | str | None = None,
-        *args: Any,
         **kwargs: Any,
     ):
-        if not super(WandbLogger, self).log(message, level, *args, **kwargs):
+        if not super(WandbLogger, self).log(*messages, level=level, **kwargs):
             return
 
+        # Handle multiple messages
+        if len(messages) > 1:
+            messages = list(messages)
+            # If the messages are strings, join them into a single string.
+            if all(
+                hasattr(message, "__str__")
+                and callable(getattr(message, "__str__"))
+                and not isinstance(message, dict)
+                for message in messages
+            ):
+                message = " ".join([str(message) for message in messages])
+            # If the messages are dictionaries, log them separately.
+            else:
+                for message in messages:
+                    self.log(message, level=level)
+                return
+        else:
+            message = messages[0]
+
         if isinstance(message, dict):
             log = message
         else:
+            message = str(
+                message
+            )  # This should be safe here as the super should have already checked that the message is a string or has a __str__ method.
             if level is not None:
                 level_str = (
                     level.name if isinstance(level, LogLevel) else str(level).upper()
                 )
                 log = {level_str: message}
             else:
                 log = {"message": message}
```

### Comparing `mloggers-1.1.7/.gitignore` & `mloggers-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.7/LICENSE` & `mloggers-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mloggers-1.1.7/README.md` & `mloggers-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -71,18 +71,32 @@
 - `info(message)`: wrapper to call `log(message, LogLevel.INFO)`.
 - `warn(message)`: wrapper to call `log(message, LogLevel.WARN)`.
 - `error(message)`: wrapper to call `log(message, LogLevel.ERROR)`.
 - `debug(message)`: wrapper to call `log(message, LogLevel.DEBUG)`.
 
 In the case of the `MultiLogger`, the methods above have the additional optional argument `mask`, which can be used to prevent the given message from being propagated through the masked loggers.
 
+All logging functions support multiple arguments, similar to the print function. For example, `logger.info("The value of x is ", x)` will log the message `"The value of x is 42"` if `x = 42`.
+The input messages can also be a series of dictionaries, which will be all logged in separate log entries. If the logger is given both a dictionary and a string, it will fail.
+
 ### Masks
 
 Masks are used by the `MultiLogger` to filter loggers which are not supposed to record a given message. At the time of initialization, you can define a default mask to use for all messages for which a mask is not specified when calling `MultiLogger.log(message, level, mask)` or the level-specific variants. To create a mask, simply pass as argument a list of the class references for the loggers you would like to mask out.
 
+### Level filtering
+
+Any logger is initialized with a `default_level` argument, which is set to `LogLevel.INFO` by default. `LogLevel` elements have an `importance` attribute, which defines a hierarchy of levels. When a logger is initialized with a given level, it will only log messages with a level of equal or higher importance. For example, if a logger is initialized with `LogLevel.WARN`, it will log messages with levels `WARN` and `ERROR`, but not `INFO` or `DEBUG`.
+
+The importance values for the built-in levels are:
+
+- `DEBUG`: -1
+- `INFO`: 0
+- `WARN`: 1
+- `ERROR`: `np.inf` (as errors should always be logged)
+
 ### Progress bars
 
 You can make use of a pre-configured wrapper of the progress bars provided by the package `rich.progress`. The wrapper is provided via the function `mloggers.progress.log_progress`. Example usage:
 
 ```python
 import time
 from mloggers.progress import log_progress
```

### Comparing `mloggers-1.1.7/pyproject.toml` & `mloggers-1.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mloggers"
-version = "1.1.7"
+version = "1.2.0"
 authors = [
     { name = "Sergio Hernandez Gutierrez", email = "contact.sergiohernandez@gmail.com" },
     { name = "Matteo Merler", email = "matteo.merler@gmail.com" },
 ]
 description = "A collection of loggers well-suited for machine learning experiments."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mloggers-1.1.7/PKG-INFO` & `mloggers-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mloggers
-Version: 1.1.7
+Version: 1.2.0
 Summary: A collection of loggers well-suited for machine learning experiments.
 Project-URL: Homepage, https://github.com/serhez/mloggers
 Project-URL: Issues, https://github.com/serhez/mloggers/issues
 Author-email: Sergio Hernandez Gutierrez <contact.sergiohernandez@gmail.com>, Matteo Merler <matteo.merler@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -91,18 +91,32 @@
 - `info(message)`: wrapper to call `log(message, LogLevel.INFO)`.
 - `warn(message)`: wrapper to call `log(message, LogLevel.WARN)`.
 - `error(message)`: wrapper to call `log(message, LogLevel.ERROR)`.
 - `debug(message)`: wrapper to call `log(message, LogLevel.DEBUG)`.
 
 In the case of the `MultiLogger`, the methods above have the additional optional argument `mask`, which can be used to prevent the given message from being propagated through the masked loggers.
 
+All logging functions support multiple arguments, similar to the print function. For example, `logger.info("The value of x is ", x)` will log the message `"The value of x is 42"` if `x = 42`.
+The input messages can also be a series of dictionaries, which will be all logged in separate log entries. If the logger is given both a dictionary and a string, it will fail.
+
 ### Masks
 
 Masks are used by the `MultiLogger` to filter loggers which are not supposed to record a given message. At the time of initialization, you can define a default mask to use for all messages for which a mask is not specified when calling `MultiLogger.log(message, level, mask)` or the level-specific variants. To create a mask, simply pass as argument a list of the class references for the loggers you would like to mask out.
 
+### Level filtering
+
+Any logger is initialized with a `default_level` argument, which is set to `LogLevel.INFO` by default. `LogLevel` elements have an `importance` attribute, which defines a hierarchy of levels. When a logger is initialized with a given level, it will only log messages with a level of equal or higher importance. For example, if a logger is initialized with `LogLevel.WARN`, it will log messages with levels `WARN` and `ERROR`, but not `INFO` or `DEBUG`.
+
+The importance values for the built-in levels are:
+
+- `DEBUG`: -1
+- `INFO`: 0
+- `WARN`: 1
+- `ERROR`: `np.inf` (as errors should always be logged)
+
 ### Progress bars
 
 You can make use of a pre-configured wrapper of the progress bars provided by the package `rich.progress`. The wrapper is provided via the function `mloggers.progress.log_progress`. Example usage:
 
 ```python
 import time
 from mloggers.progress import log_progress
```

