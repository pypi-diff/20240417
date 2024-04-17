# Comparing `tmp/screwmpcpy-0.5.0.tar.gz` & `tmp/screwmpcpy-0.5.1.tar.gz`

## Comparing `screwmpcpy-0.5.0.tar` & `screwmpcpy-0.5.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.readthedocs.yaml
--rw-r--r--   0        0        0    18294 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/logo.jpg
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/noxfile.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.github/workflows/precommit.yml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.vscode/extensions.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.vscode/tasks.json
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/docs/index.md
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/docs/api/screwmpcpy.rst
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/examples/motiongenerator.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/examples/panda_screwmotion_ik.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/_version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/_version.pyi
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/basemg.py
--rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/dqutil.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/mpcutil.py
--rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/pandamg.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/posegen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/py.typed
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/screwintegrator.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/screwmpc.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_dqutil.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_mpcutil.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_package.py
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_pandamg.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_screwintegrator.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_screwmpc_ctrl_signal.py
--rw-r--r--   0        0        0    18967 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_screwmpc_matrices.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/LICENSE
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/README.md
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    18294 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/logo.jpg
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/noxfile.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.github/workflows/precommit.yml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.vscode/tasks.json
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/docs/index.md
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/docs/api/screwmpcpy.rst
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/examples/motiongenerator.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/examples/panda_screwmotion_ik.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/_version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/_version.pyi
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/basemg.py
+-rw-r--r--   0        0        0    10134 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/dqutil.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/mpcutil.py
+-rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/pandamg.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/posegen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/py.typed
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/screwintegrator.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/src/screwmpcpy/screwmpc.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/tests/test_dqutil.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/tests/test_mpcutil.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/tests/test_package.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/tests/test_pandamg.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/tests/test_screwintegrator.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/tests/test_screwmpc_ctrl_signal.py
+-rw-r--r--   0        0        0    18967 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/tests/test_screwmpc_matrices.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/README.md
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 screwmpcpy-0.5.1/PKG-INFO
```

### Comparing `screwmpcpy-0.5.0/.pre-commit-config.yaml` & `screwmpcpy-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/logo.jpg` & `screwmpcpy-0.5.1/logo.jpg`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/noxfile.py` & `screwmpcpy-0.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/.devcontainer/devcontainer.json` & `screwmpcpy-0.5.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/.github/workflows/python-package.yml` & `screwmpcpy-0.5.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/.github/workflows/python-publish.yml` & `screwmpcpy-0.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/.vscode/tasks.json` & `screwmpcpy-0.5.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/docs/conf.py` & `screwmpcpy-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/docs/api/screwmpcpy.rst` & `screwmpcpy-0.5.1/docs/api/screwmpcpy.rst`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/examples/motiongenerator.py` & `screwmpcpy-0.5.1/examples/motiongenerator.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/examples/panda_screwmotion_ik.py` & `screwmpcpy-0.5.1/examples/panda_screwmotion_ik.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/src/screwmpcpy/__init__.py` & `screwmpcpy-0.5.1/src/screwmpcpy/__init__.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/src/screwmpcpy/basemg.py` & `screwmpcpy-0.5.1/src/screwmpcpy/basemg.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/src/screwmpcpy/dqutil.py` & `screwmpcpy-0.5.1/src/screwmpcpy/dqutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
        Screw angle is forced between :math:`\left[-\pi, +\pi\right]`
 
     :param dq_in: Input dual quaternion
     :type dq_in: DQ
     :return: Minimum screw angle DQ.
     :rtype: DQ
     """
-    theta_half = np.arccos(dq_in.q[0])
+    theta_half = np.arccos(np.clip(dq_in.q[0], -1, 1))
     u_vec = vec3(dq_in.P())
     out = np.zeros((8,))
 
     if not np.isclose(theta_half, 0.0):
         denom = np.sin(theta_half)
         theta_eps_half = -(dq_in.q[4] / denom)
         s = u_vec / denom
@@ -95,15 +95,15 @@
     :param dq_in: Input unit dual quaternion :math:`\boldsymbol{h}`.
     :type dq_in: DQ
     :param alpha: Power raising the dual quaternion :math:`\boldsymbol{h}^\alpha`.
     :type alpha: float
     :return: :math:`\boldsymbol{h}^\alpha`.
     :rtype: DQ
     """
-    theta_half = np.arccos(dq_in.q[0])
+    theta_half = np.arccos(np.clip(dq_in.q[0], -1, 1))
     out = np.zeros((8,))
     v_vec = vec3(dq_in)
     dual = vec3(dq_in.D())
 
     if not np.isclose(theta_half, 0.0):
         denom = np.sin(theta_half)
         theta_eps_half = -(dq_in.q[4] / denom)
@@ -129,15 +129,15 @@
 
     :param dq_in: Input unit dual quaternion.
     :type dq_in: DQ
     :return: The dual quaternion logartihm log(dq_in).
     :rtype: DQ
     """
     out = np.zeros((8,))
-    theta_half = np.arccos(dq_in.q[0])
+    theta_half = np.arccos(np.clip(dq_in.q[0], -1, 1))
     v_hat = dq_in.q[5:]
     if not np.isclose(theta_half, 0.0):
         sin_theta_half = np.sin(theta_half)
         theta_eps_half = -dq_in.q[4] / sin_theta_half
         v_vec = vec3(dq_in.P()) / sin_theta_half  # dq_in.q[1:4] / sin_theta_half
         v_eps = (
             v_hat - theta_eps_half * np.cos(theta_eps_half) * v_vec
```

### Comparing `screwmpcpy-0.5.0/src/screwmpcpy/mpcutil.py` & `screwmpcpy-0.5.1/src/screwmpcpy/mpcutil.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/src/screwmpcpy/pandamg.py` & `screwmpcpy-0.5.1/src/screwmpcpy/pandamg.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/src/screwmpcpy/posegen.py` & `screwmpcpy-0.5.1/src/screwmpcpy/posegen.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/src/screwmpcpy/screwintegrator.py` & `screwmpcpy-0.5.1/src/screwmpcpy/screwintegrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import numpy as np
-from dqrobotics import DQ
+from dqrobotics import DQ, robots
 
+from . import dqutil
 from .pandamg import PandaScrewMotionGenerator
 
 
 def simulate_joint_waypoints(
     mg: PandaScrewMotionGenerator,
     q_init: np.ndarray,
     ee_goal_pose: DQ,
@@ -32,17 +33,19 @@
     :rtype: tuple[list[np.ndarray], bool]
     """
     error: float = float("inf")
     q_robot: np.ndarray = q_init.copy()
     joint_angles: list[np.ndarray] = [q_init]
     step: int = 0
     done: bool = False
-
+    kin = robots.FrankaEmikaPandaRobot.kinematics()
     while not done:
         dq = mg.step(q_robot, ee_goal_pose)
         q_robot += dq * dt
         joint_angles.append(q_robot.copy())
-        error = np.linalg.norm(mg.dqerror.vec8())
+        error = np.linalg.norm(
+            dqutil.dq_pose_error(kin.fkm(q_robot), ee_goal_pose).vec8()
+        )
         done = error < eps or step >= max_steps
         step += 1
 
     return joint_angles, error < eps
```

### Comparing `screwmpcpy-0.5.0/src/screwmpcpy/screwmpc.py` & `screwmpcpy-0.5.1/src/screwmpcpy/screwmpc.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/tests/test_dqutil.py` & `screwmpcpy-0.5.1/tests/test_dqutil.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/tests/test_mpcutil.py` & `screwmpcpy-0.5.1/tests/test_mpcutil.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/tests/test_pandamg.py` & `screwmpcpy-0.5.1/tests/test_pandamg.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/tests/test_screwmpc_ctrl_signal.py` & `screwmpcpy-0.5.1/tests/test_screwmpc_ctrl_signal.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/tests/test_screwmpc_matrices.py` & `screwmpcpy-0.5.1/tests/test_screwmpc_matrices.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/.gitignore` & `screwmpcpy-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/LICENSE` & `screwmpcpy-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/README.md` & `screwmpcpy-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/pyproject.toml` & `screwmpcpy-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.5.0/PKG-INFO` & `screwmpcpy-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: screwmpcpy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Dual Quaternion based MPC generating screw motion for n-DOF robot arm.
 Project-URL: Homepage, https://github.com/greinerth/screwmpcpy
 Project-URL: Bug Tracker, https://github.com/greinerth/screwmpcpy/issues
 Project-URL: Discussions, https://github.com/greinerth/screwmpcpy/discussions
 Project-URL: Changelog, https://github.com/greinerth/screwmpcpy/releases
 Author-email: Gerhard Reinerth <g.reinerth@tum.de>
 License: Copyright 2024 Gerhard Reinerth
```

