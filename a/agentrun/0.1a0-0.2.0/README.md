# Comparing `tmp/agentrun-0.1a0.tar.gz` & `tmp/agentrun-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentrun-0.1a0.tar", last modified: Fri Apr 12 01:30:58 2024, max compression
+gzip compressed data, was "agentrun-0.2.0.tar", last modified: Wed Apr 17 02:15:23 2024, max compression
```

## Comparing `agentrun-0.1a0.tar` & `agentrun-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:30:58.671492 agentrun-0.1a0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 01:30:51.000000 agentrun-0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-12 01:30:58.671492 agentrun-0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-12 01:30:51.000000 agentrun-0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:30:58.671492 agentrun-0.1a0/agentrun/
--rw-r--r--   0 runner    (1001) docker     (127)    14134 2024-04-12 01:30:51.000000 agentrun-0.1a0/agentrun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:30:58.671492 agentrun-0.1a0/agentrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 01:30:58.000000 agentrun-0.1a0/agentrun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-12 01:30:51.000000 agentrun-0.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:30:58.671492 agentrun-0.1a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:30:58.671492 agentrun-0.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-12 01:30:51.000000 agentrun-0.1a0/tests/test_agentrun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:15:23.533288 agentrun-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-17 02:15:17.000000 agentrun-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-04-17 02:15:23.533288 agentrun-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14680 2024-04-17 02:15:17.000000 agentrun-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:15:23.529288 agentrun-0.2.0/agentrun/
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-17 02:15:17.000000 agentrun-0.2.0/agentrun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:15:23.533288 agentrun-0.2.0/agentrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 02:15:17.000000 agentrun-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:15:23.533288 agentrun-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:15:23.533288 agentrun-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-17 02:15:17.000000 agentrun-0.2.0/tests/test_agentrun.py
```

### Comparing `agentrun-0.1a0/LICENSE` & `agentrun-0.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2024 Jonathan Adly
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `agentrun-0.1a0/agentrun/__init__.py` & `agentrun-0.2.0/agentrun/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,52 +14,114 @@
 from RestrictedPython import compile_restricted
 
 
 class AgentRun:
     """Class to execute Python code in an isolated Docker container.
 
     Example usage:
-        from agentrun import AgentRun
-        runner = AgentRun(container_name="my_container") # container should be running
-        result = runner.execute_code_in_container("print('Hello, world!')")
+        from agentrun import AgentRun\n
+        runner = AgentRun(container_name="my_container") # container should be running\n
+        result = runner.execute_code_in_container("print('Hello, world!')")\n
         print(result)
 
     Args:
         container_name: Name of the Docker container to use
         dependencies_whitelist: List of whitelisted dependencies to install. By default, all dependencies are allowed.
+        cached_dependencies: List of dependencies to cache in the container
         cpu_quota: CPU quota in microseconds (default: 50,000)
         default_timeout: Default timeout in seconds (default: 20)
         memory_limit: Memory limit for the container (default: 100m)
         memswap_limit: Memory + swap limit for the container (default: 512m)
         client: Docker client object (default: docker.from_env())
     """
 
     def __init__(
         self,
         container_name,
         dependencies_whitelist=["*"],
+        cached_dependencies=[],
         cpu_quota=50000,
         default_timeout=20,
         memory_limit="100m",
         memswap_limit="512m",
         client=None,
-    ):
+    ) -> None:
 
         self.cpu_quota = cpu_quota
         self.default_timeout = default_timeout
         self.memory_limit = memory_limit
         self.memswap_limit = memswap_limit
         self.container_name = container_name
         self.dependencies_whitelist = dependencies_whitelist
         # this is to allow a mock client to be passed in for testing if docker is not available (not implemented yet)
         self.client = client or docker.from_env()
+        self.cached_dependencies = cached_dependencies
+
+        try:
+            self.client = client or docker.from_env()
+            self.client.ping()
+        except docker.errors.DockerException as e:
+            raise RuntimeError(
+                f"Failed to connect to Docker daemon. Please make sure Docker is running. {e}"
+            )
+
+        try:
+            container = self.client.containers.get(self.container_name)
+            if container.status != "running":
+                raise ValueError(f"Container {self.container_name} is not running.")
+        except docker.errors.NotFound:
+            raise ValueError(f"Container {self.container_name} not found.")
+
+        if (
+            not self.is_everything_whitelisted()
+            and not self.validate_cached_dependencies()
+        ):
+            raise ValueError("Some cached dependencies are not in the whitelist.")
+
+        if self.cached_dependencies:
+            self.install_cached_dependencies()
 
     class CommandTimeout(Exception):
+        """Exception raised when a command execution times out."""
+
         pass
 
+    def is_everything_whitelisted(self) -> bool:
+        """
+        Check if everything is whitelisted.
+
+        Returns:
+            bool: True if everything is whitelisted, False otherwise.
+        """
+        return "*" in self.dependencies_whitelist
+
+    def validate_cached_dependencies(self) -> bool:
+        """
+        Validates the cached dependencies against the whitelist.
+
+        Returns:
+            bool: True if all cached dependencies are whitelisted, False otherwise.
+        """
+        if self.is_everything_whitelisted():
+            return True
+        return all(
+            dep in self.dependencies_whitelist for dep in self.cached_dependencies
+        )
+
+    def install_cached_dependencies(self) -> None:
+        """
+        Attempts to install cached dependencies into the specified Docker container.
+        Raises:
+            ValueError: If the dependencies could not be successfully installed.
+        """
+        container = self.client.containers.get(self.container_name)
+        output = self.install_dependencies(container, self.cached_dependencies)
+        if output != "Dependencies installed successfully.":
+            raise ValueError(output)
+
     def execute_command_in_container(
         self, container: Container, cmd: str, timeout: int
     ) -> tuple[Any | None, Any | str]:
         """Execute a command in a Docker container with a timeout.
 
         This function runs the command in a separate thread and waits for the specified timeout.
 
@@ -218,23 +280,35 @@
         Args:
             container: Docker container object
             dependencies: List of dependencies to install
         Returns:
             Success message or error message
 
         """
-        everything_whitelisted = "*" in self.dependencies_whitelist
+        everything_whitelisted = self.is_everything_whitelisted()
 
         # Perform a pre-check to ensure all dependencies are in the whitelist (or everything is whitelisted)
         if not everything_whitelisted:
             for dep in dependencies:
                 if dep not in self.dependencies_whitelist:
                     return f"Dependency: {dep} is not in the whitelist."
+        # if we are doing caching, we need to check if the dependencies are already installed
+        if self.cached_dependencies:
+            exec_log = container.exec_run(cmd="pip list", workdir="/code")
+            exit_code, output = exec_log.exit_code, exec_log.output.decode("utf-8")
+            installed_packages = output.splitlines()
+            installed_packages = [
+                line.split()[0].lower() for line in installed_packages if " " in line
+            ]
+        else:
+            installed_packages = []
 
         for dep in dependencies:
+            if dep.lower() in installed_packages:
+                continue
             command = f"pip install --user {dep}"
             exit_code, output = self.execute_command_in_container(
                 container, command, timeout=120
             )
             if exit_code != 0:
                 return f"Failed to install dependency {dep}"
 
@@ -245,14 +319,17 @@
         Args:
             container: Docker container object
             dependencies: List of dependencies to uninstall
         Returns:
             Success message or error message
         """
         for dep in dependencies:
+            # do not uninstall dependencies that are cached_dependencies
+            if dep in self.cached_dependencies:
+                continue
             command = f"pip uninstall -y {dep}"
             exit_code, output = self.execute_command_in_container(
                 container, command, timeout=120
             )
 
         return "Dependencies uninstalled successfully."
 
@@ -322,33 +399,30 @@
             # check  if the code is safe to execute
             safety_result = self.safety_check(python_code)
             safety_message = safety_result["message"]
             safe = safety_result["safe"]
             if not safe:
                 return safety_message
 
-            try:
-                container = client.containers.get(self.container_name)
-            except docker.errors.NotFound:
-                return f"Container with name {self.container_name} not found."
+            container = client.containers.get(self.container_name)
+
             # update the container with the new limits
             container.update(
                 cpu_quota=self.cpu_quota,
                 mem_limit=self.memory_limit,
                 memswap_limit=self.memswap_limit,
             )
             # Copy the code to the container
             exec_result = self.copy_code_to_container(container, python_code)
             successful_copy = exec_result["success"]
-            copy_message = exec_result["message"]
+            message = exec_result["message"]
             if not successful_copy:
-                copy_message = exec_result["message"]
-                return copy_message
+                return message
 
-            script_name = copy_message
+            script_name = message
 
             # Install dependencies in the container
             dependencies = self.parse_dependencies(python_code)
             dep_install_result = self.install_dependencies(container, dependencies)
             if dep_install_result != "Dependencies installed successfully.":
                 return dep_install_result
 
@@ -360,10 +434,14 @@
                 return "Execution timed out."
 
         except Exception as e:
             return str(e)
 
         finally:
             if container:
-                self.clean_up(container, script_name, dependencies)
+                # run clean up in a seperate thread to avoid blocking the main thread
+                thread = Thread(
+                    target=self.clean_up, args=(container, script_name, dependencies)
+                )
+                thread.start()
 
         return output
```

### Comparing `agentrun-0.1a0/pyproject.toml` & `agentrun-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 [project]
 name = "agentrun"
-version = "v0.1-alpha"
+version = "v0.2.0"
 description = "The easiest way to run AI or user generated python code safely in a docker container"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{name = "Jonathan Adly", email = "gadly0123@gmail.com"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
  "docker", "RestrictedPython", 
 ]
 
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+include-package-data = false
+
+[tool.setuptools.packages.find]
+include = ["agentrun*"]
+exclude = ["agentrun-api*", "docs*", "examples*", "tests*", ".github*"]
+
 [project.urls]
 Homepage = "https://github.com/jonathan-adly/agentrun"
 Changelog = "https://github.com/jonathan-adly/agentrun/releases"
 Issues = "https://github.com/jonathan-adly/agentrun/issues"
 CI = "https://github.com/jonathan-adly/agentrun/actions"
 
 
 [project.optional-dependencies]
-test = ["pytest"]
+test = ["pytest", "pytest-cov", "pytest-benchmark", "mypy", "mkdocs", "mkdocs-material", 'mkdocstrings[python]', "mkdocs-jupyter"]
```

